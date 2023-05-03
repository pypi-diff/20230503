# Comparing `tmp/ezmote-cmdserver-0.7.9.tar.gz` & `tmp/ezmote-cmdserver-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmote-cmdserver-0.7.9.tar", last modified: Sun Sep 11 20:06:50 2022, max compression
+gzip compressed data, was "ezmote-cmdserver-0.8.0.tar", last modified: Wed May  3 21:55:48 2023, max compression
```

## Comparing `ezmote-cmdserver-0.7.9.tar` & `ezmote-cmdserver-0.8.0.tar`

### file list

```diff
@@ -1,92 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:50.667600 ezmote-cmdserver-0.7.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4345 2022-09-11 20:06:50.667600 ezmote-cmdserver-0.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3834 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:50.647598 ezmote-cmdserver-0.7.9/cmdserver/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:50.655599 ezmote-cmdserver-0.7.9/cmdserver/apis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/command.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/pj.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/playingnow.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/tivo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/tivos.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/apis/wake.py
--rw-r--r--   0 runner    (1001) docker     (121)     2670 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/commandcontroller.py
--rw-r--r--   0 runner    (1001) docker     (121)     6171 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/debounce.py
--rw-r--r--   0 runner    (1001) docker     (121)     8540 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/infoprovider.py
--rw-r--r--   0 runner    (1001) docker     (121)     9681 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/jvc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    25365 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/jvccommands.py
--rw-r--r--   0 runner    (1001) docker     (121)     7036 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3398 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/pjcontroller.py
--rw-r--r--   0 runner    (1001) docker     (121)    12146 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/tivocontroller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:50.655599 ezmote-cmdserver-0.7.9/cmdserver/ui/
--rw-r--r--   0 runner    (1001) docker     (121)     8445 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (121)    22762 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/android-chrome-384x384.png
--rw-r--r--   0 runner    (1001) docker     (121)     6743 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/favicon-32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (121)     7406 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/index.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      455 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     5615 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-09-11 08:09:09.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/safari-pinned-tab.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:50.643598 ezmote-cmdserver-0.7.9/cmdserver/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:50.655599 ezmote-cmdserver-0.7.9/cmdserver/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/css/2.1ca50200.chunk.css
--rw-r--r--   0 runner    (1001) docker     (121)     5628 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/css/2.1ca50200.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:50.663599 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)   770059 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/2.e1be858e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/2.e1be858e.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)  3254278 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/2.e1be858e.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/3.6b0298ca.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     3680 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/3.6b0298ca.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (121)    89708 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/main.8e73262a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)   256674 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/main.8e73262a.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/runtime-main.ba0a062e.js
--rw-r--r--   0 runner    (1001) docker     (121)    12592 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/js/runtime-main.ba0a062e.js.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:50.667600 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (121)    20368 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-100.a45108d3.woff
--rw-r--r--   0 runner    (1001) docker     (121)    15808 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-100.c2aa4ab1.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    21704 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-100italic.451d4e55.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17008 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-100italic.7f839a86.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    15784 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-300.37a7069d.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20348 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-300.865f928c.woff
--rw-r--r--   0 runner    (1001) docker     (121)    22204 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-300italic.bd5b7a13.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17448 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-300italic.c64e7e35.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    15736 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-400.176f8f5b.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20268 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-400.49ae34d4.woff
--rw-r--r--   0 runner    (1001) docker     (121)    21952 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-400italic.b1d9d990.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17324 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-400italic.d022bc70.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20464 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-500.cea99d3e.woff
--rw-r--r--   0 runner    (1001) docker     (121)    15872 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-500.f5b74d7f.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    17316 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-500italic.0d8bb5b3.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    22020 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-500italic.18d00f73.woff
--rw-r--r--   0 runner    (1001) docker     (121)    20356 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-700.2267169e.woff
--rw-r--r--   0 runner    (1001) docker     (121)    15816 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-700.c18ee39f.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    17020 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-700italic.7d8125ff.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    21588 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-700italic.9360531f.woff
--rw-r--r--   0 runner    (1001) docker     (121)    15712 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-900.870c8c14.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20392 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-900.bac8362e.woff
--rw-r--r--   0 runner    (1001) docker     (121)    22304 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-900italic.c20d916c.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17520 2022-09-11 08:09:36.000000 ezmote-cmdserver-0.7.9/cmdserver/ui/static/media/roboto-latin-900italic.cb5ad999.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/ws.py
--rw-r--r--   0 runner    (1001) docker     (121)    69607 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/cmdserver/zeroconf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 20:06:50.667600 ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4345 2022-09-11 20:06:50.000000 ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-09-11 20:06:50.000000 ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-11 20:06:50.000000 ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-11 20:06:50.000000 ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-11 20:06:50.000000 ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-09-11 20:06:50.000000 ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-11 20:06:50.000000 ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-11 20:06:50.671600 ezmote-cmdserver-0.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3066 2022-09-11 20:06:07.000000 ezmote-cmdserver-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:55:48.347572 ezmote-cmdserver-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-03 21:55:48.347572 ezmote-cmdserver-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:55:48.343572 ezmote-cmdserver-0.8.0/cmdserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:55:48.347572 ezmote-cmdserver-0.8.0/cmdserver/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/pj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/playingnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/tivo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/tivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/apis/wake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/commandcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/infoprovider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/jvc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25365 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/jvccommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/pjcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/tivocontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69607 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/cmdserver/zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:55:48.347572 ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-03 21:55:48.000000 ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 21:55:48.000000 ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:55:48.000000 ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 21:55:48.000000 ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:55:48.000000 ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-03 21:55:48.000000 ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 21:55:48.000000 ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:55:48.347572 ezmote-cmdserver-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-03 21:55:04.000000 ezmote-cmdserver-0.8.0/setup.py
```

### Comparing `ezmote-cmdserver-0.7.9/LICENSE` & `ezmote-cmdserver-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/PKG-INFO` & `ezmote-cmdserver-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ezmote-cmdserver
-Version: 0.7.9
+Version: 0.8.0
 Summary: A small webapp which can be used for web based home cinema automation
 Home-page: http://github.com/3ll3d00d/cmdserver
 Author: Matt Khan
 Author-email: mattkhan+cmdserver@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -167,9 +166,7 @@
     debug: false
     debugLogging: true
     host: megatron
     port: 53199
     useTwisted: true
     # use for debug
     webappPath: 'C:\Users\mattk\github\ezmote\build'
-
-
```

### Comparing `ezmote-cmdserver-0.7.9/README.md` & `ezmote-cmdserver-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/apis/command.py` & `ezmote-cmdserver-0.8.0/cmdserver/apis/command.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/apis/info.py` & `ezmote-cmdserver-0.8.0/cmdserver/apis/info.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/apis/pj.py` & `ezmote-cmdserver-0.8.0/cmdserver/apis/pj.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/apis/tivo.py` & `ezmote-cmdserver-0.8.0/cmdserver/apis/tivo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 
 from flask_restx import Resource, Namespace
+from cmdserver.tivocontroller import Tivo as tivo_data
 
 logger = logging.getLogger('tivo')
 
 api = Namespace('1/tivo', description='Gets info about a named tivo')
 
 
-@api.route('/<string:tivo>')
+@api.route('/<string:tivo_name>')
 class Tivo(Resource):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__controller = kwargs['tivoController']
 
-    def get(self, tivo):
-        tivo = self.__controller.get_tivo(tivo)
+    def get(self, tivo_name):
+        tivo: tivo_data = self.__controller.get_tivo(tivo_name)
         if tivo is None:
             return 404
         else:
-            return {'channel': tivo.currentChannel, 'messages': tivo.messages, 'connected': tivo.connected}, 200
+            return {'channel': tivo.current_channel, 'messages': tivo.messages, 'connected': tivo.connected}, 200
```

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/apis/tivos.py` & `ezmote-cmdserver-0.8.0/cmdserver/apis/tivos.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/apis/wake.py` & `ezmote-cmdserver-0.8.0/cmdserver/apis/wake.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/commandcontroller.py` & `ezmote-cmdserver-0.8.0/cmdserver/commandcontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/config.py` & `ezmote-cmdserver-0.8.0/cmdserver/config.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/debounce.py` & `ezmote-cmdserver-0.8.0/cmdserver/debounce.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/infoprovider.py` & `ezmote-cmdserver-0.8.0/cmdserver/infoprovider.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         for key, value in config.commands.items():
             if 'playingNowId' in value:
                 is_default = value.get('defaultPlayingNowId', False)
                 if is_default is True:
                     self.__default_playing_now_id = value['playingNowId']
         self.__by_playing_now_id = {value['playingNowId']: value['title']
                                     for key, value in config.commands.items() if 'playingNowId' in value}
-        self.__ms: MediaServer = MediaServer('localhost', config.mcws['user'], config.mcws['pass'])
+        self.__ms: MediaServer = MediaServer('localhost', config.mcws.get('user', None), config.mcws.get('pass', None))
         # make sure all calls in pymcws have a timeout not just connection checks
         self.__ms.session.request = functools.partial(self.__ms.session.request, timeout=2)
         self.__ms_mac: str = config.mcws.get('mac', '')
         self.__ms.port = int(config.mcws.get('port', 52199))
         self.__ms.local_ip_list = config.mcws.get('ip', '127.0.0.1')
         self.__ms.local_ip = self.__ms.local_ip_list
         self.__token = None
@@ -80,14 +80,17 @@
             }
             active_command = self.get_active_command(self.__current_state['zones'].get(active_zone.id, None))
             self.__current_state['playingCommand'] = {'active': active_command}
             self.__ws_server.broadcast(json.dumps(self.__current_state, ensure_ascii=False))
         except ConnectTimeout as e:
             logger.warning(f"Unable to connect, MC probably sleeping {e.request.method} {e.request.url}")
             self.__broadcast_down()
+        except ConnectionRefusedError as e:
+            logger.error(f"Unable to connect, MC appears down")
+            self.__broadcast_down()
         except:
             logger.exception(f"Unexpected failure to refresh current state of {self.__ms.address()}")
             self.__broadcast_down()
 
     def __broadcast_down(self):
         was_alive = not self.__current_state or self.__current_state.get('config', {}).get('alive', True) is True
         if was_alive:
```

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/jvc.py` & `ezmote-cmdserver-0.8.0/cmdserver/jvc.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/jvccommands.py` & `ezmote-cmdserver-0.8.0/cmdserver/jvccommands.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/main.py` & `ezmote-cmdserver-0.8.0/cmdserver/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             """
             Handles the react app (excluding the static dir).
             """
 
             def __init__(self, path):
                 # TODO allow this to load when in debug mode even if the files don't exist
                 self.publicFiles = {f: static.File(os.path.join(path, f)) for f in os.listdir(path) if
-                                    os.path.exists(os.path.join(path, f))}
+                                    os.path.exists(os.path.join(path, f))} if os.path.exists(path) else {}
                 self.indexHtml = ReactIndex(os.path.join(path, 'index.html'))
 
             def get_file(self, path):
                 """
                 overrides getChild so it always just serves index.html unless the file does actually exist (i.e. is an
                 icon or something like that)
                 """
@@ -114,15 +114,18 @@
                     uiRoot = os.path.join(sys._MEIPASS, 'ui')
                 elif cfg.webappPath is not None:
                     uiRoot = cfg.webappPath
                 else:
                     # release script moves the ui under the analyser package because setuptools doesn't seem to include
                     # files from outside the package
                     uiRoot = os.path.join(os.path.dirname(__file__), 'ui')
-                logger.info('Serving ui from ' + str(uiRoot))
+                if os.path.exists(uiRoot):
+                    logger.info(f'Serving ui from {uiRoot}')
+                else:
+                    logger.info('No UI, API only')
                 self.react = ReactApp(uiRoot)
                 self.static = static.File(os.path.join(uiRoot, 'static'))
                 self.icons = static.File(cfg.iconPath)
                 ws_server.factory.startFactory()
                 self.ws_resource = WebSocketResource(ws_server.factory)
 
             def getChild(self, path, request):
@@ -157,14 +160,15 @@
                 return self.wsgi.render(request)
 
         application = service.Application('cmdserver')
         if cfg.is_access_logging is True:
             site = server.Site(FlaskAppWrapper(), logPath=path.join(cfg.config_path, 'access.log').encode())
         else:
             site = server.Site(FlaskAppWrapper())
+        logger.info(f'Listening on 0.0.0.0:{cfg.port}')
         endpoint = endpoints.TCP4ServerEndpoint(reactor, cfg.port, interface='0.0.0.0')
         endpoint.listen(site)
         reactor.run()
     else:
         logger.error('Icons are not available in debug mode')
         # get config from a flask standard place not our config yml
         app.run(debug=cfg.run_in_debug, host='0.0.0.0', port=cfg.port, use_reloader=False)
```

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/pjcontroller.py` & `ezmote-cmdserver-0.8.0/cmdserver/pjcontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/tivocontroller.py` & `ezmote-cmdserver-0.8.0/cmdserver/tivocontroller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import re
 import socket
 import threading
 import time
+from typing import Optional
 
 from cmdserver.zeroconf import Zeroconf, ServiceBrowser
 from cmdserver.config import Config
 
 logger = logging.getLogger('tivocontroller')
 
 
@@ -72,19 +73,19 @@
               '$': 'NUM4', '%': 'NUM5', '^': 'NUM6', '&': 'NUM7',
               '*': 'NUM8', '(': 'NUM9', ')': 'NUM0'}
 
 
 class Tivo:
 
     def __init__(self, tivo: dict):
-        self._sock = None
+        self.__sock = None
         self.__tivo = tivo
         self.__messages = [''] * 5
-        self._messageIdx = 0
-        self.currentChannel = ''
+        self.__message_idx = 0
+        self.current_channel = ''
         if ':' in tivo['address']:
             address, port = tivo['address'].split(':')
             try:
                 port = int(port)
                 self.__tivo['address'] = address
                 self.__tivo['port'] = port
             except:
@@ -108,46 +109,46 @@
         return self.__tivo['version']
 
     def get_tivo_properties(self):
         return {**self.__tivo}
 
     @property
     def connected(self):
-        return self._sock is not None
+        return self.__sock is not None
 
     def __connect(self):
         """ Connect to the TiVo within five seconds or report error. """
         self.__messages = [''] * 5
-        self._messageIdx = 0
+        self.__message_idx = 0
         try:
-            self._sock = socket.socket()
-            self._sock.settimeout(5)
-            self._sock.connect((self.address, self.port))
-            self._sock.settimeout(None)
-            self._statusThread = threading.Thread(name='TivoStatusReader', target=self.__read_from_socket, daemon=True)
-            self._statusThread.start()
+            self.__sock = socket.socket()
+            self.__sock.settimeout(5)
+            self.__sock.connect((self.address, self.port))
+            self.__sock.settimeout(None)
+            self.__status_thread = threading.Thread(name='TivoStatusReader', target=self.__read_from_socket, daemon=True)
+            self.__status_thread.start()
         except Exception as e:
             self.__record_message('Unable to connect - ' + str(e))
             self.disconnect()
 
     def disconnect(self):
-        if self._sock:
+        if self.__sock:
             self.__record_message('Stopping on disconnect')
-            self._sock.close()
+            self.__sock.close()
             self.__record_message('Disconnected')
-            self._sock = None
+            self.__sock = None
         else:
             logger.info(f"Ignoring disconnect {self.name} has no socket")
 
     def __send(self, message):
         """ The core output function. Re-connect if necessary, send message, sleep, and check for errors. """
-        if not self._sock:
+        if not self.__sock:
             self.__connect()
         try:
-            self._sock.sendall(message.encode())
+            self.__sock.sendall(message.encode())
             time.sleep(0.1)
         except Exception as e:
             logger.error(e)
             self.__record_message('Failed to send ' + str(message) + ' - ' + str(e))
             self.disconnect()
             raise e
 
@@ -158,68 +159,69 @@
                 self.send_ir(sent, *each)
             else:
                 if each in CODES:
                     actual = CODES[each]
                     if type(actual) == list:
                         self.send_ir(sent, *actual)
                     else:
-                        toSend = 'IRCODE %s\r' % actual
-                        sent.append(toSend)
-                        self.__send(toSend)
+                        to_send = 'IRCODE %s\r' % actual
+                        sent.append(to_send)
+                        self.__send(to_send)
                 else:
                     raise ValueError('Unknown IR Code ' + each)
-        return {'channel': self.currentChannel, 'sent': sent}
+        return {'channel': self.current_channel, 'sent': sent}
 
     def set_channel(self, channel):
         """ Sends a single SETCH. """
         toSend = 'SETCH %s\r' % channel
         self.__send(toSend)
-        return {'channel': self.currentChannel, 'sent': [toSend]}
+        return {'channel': self.current_channel, 'sent': [toSend]}
 
     def send_text(self, text):
         """ Expand a KEYBOARD command sequence for send(). """
         sent = []
         for ch in text:
             if 'A' <= ch <= 'Z':
                 self.__send_keyboard(sent, 'LSHIFT', ch)
             elif 'a' <= ch <= 'z':
                 self.__send_keyboard(sent, ch.upper())
             elif ch in SYMBOLS:
                 self.__send_keyboard(sent, SYMBOLS[ch])
             elif ch in SHIFT_SYMS:
                 self.__send_keyboard(sent, 'LSHIFT', SHIFT_SYMS[ch])
-        return {'channel': self.currentChannel, 'sent': sent}
+        return {'channel': self.current_channel, 'sent': sent}
 
     def __send_keyboard(self, sent, *codes):
         for each in codes:
-            toSend = 'KEYBOARD %s\r' % each
-            sent.append(toSend)
-            self.__send(toSend)
+            to_send = 'KEYBOARD %s\r' % each
+            sent.append(to_send)
+            self.__send(to_send)
 
     def __record_message(self, msg):
-        idx = self._messageIdx % 5
-        self._messageIdx += 1
+        idx = self.__message_idx % 5
+        self.__message_idx += 1
         self.__messages[idx] = msg
 
     def __read_from_socket(self):
         """ Read incoming messages from the socket in a separate thread.
         """
         logger.info(f"[{self.name}] Initialising status reader")
-        while self._sock is not None:
-            logger.info('Reading')
+        while self.__sock is not None:
+            logger.info(f'[{self.name}] Reading from socket')
             try:
-                status = self._sock.recv(80).decode()
+                status = self.__sock.recv(80).decode()
             except Exception as e:
                 status = str(e)
+                logger.warning(f"Failed to read - {status}")
             status = status.strip().title()
             if not status:
                 self.__record_message('No status read from socket')
                 self.disconnect()
             else:
-                self.currentChannel = status
+                self.current_channel = status
         logger.info(f"[{self.name}] Exiting status reader")
 
     @property
     def messages(self):
         return self.__messages
 
 
@@ -257,40 +259,40 @@
                     logger.info(f"Disconnecting old Tivo {old_tivo.name} @ {old_tivo.address}:{old_tivo.port}")
                     old_tivo.disconnect()
         except:
             logger.exception('Unexpected failure during ping')
         finally:
             self.__ping()
 
-    def has_tivo(self, tivo_name):
+    def has_tivo(self, tivo_name: str) -> bool:
         return True if next((t for t in self.__tivos if t.name == tivo_name), None) else False
 
-    def get_tivo(self, tivo_name):
+    def get_tivo(self, tivo_name: str) -> Optional[Tivo]:
         return next((t for t in self.__tivos if t.name == tivo_name), None)
 
-    def send(self, tivo_name, type, command):
+    def send(self, tivo_name, cmd_type, command):
         tivo = self.get_tivo(tivo_name)
         if tivo is not None:
-            if type == 'keyboard':
+            if cmd_type == 'keyboard':
                 return tivo.send_text(command)
-            elif type == 'ir':
+            elif cmd_type == 'ir':
                 return tivo.send_ir([], command)
-            elif type == 'setch':
+            elif cmd_type == 'setch':
                 return tivo.set_channel(command)
             else:
-                raise ValueError('Unknown command type ' + type)
+                raise ValueError('Unknown command type ' + cmd_type)
         else:
             raise ValueError('Unknown tivo ' + tivo_name)
 
     @property
     def tivos(self):
         return [
             {
                 **t.get_tivo_properties(),
-                **{'connected': t.connected, 'messages': t.messages, 'channel': t.currentChannel}
+                **{'connected': t.connected, 'messages': t.messages, 'channel': t.current_channel}
             }
             for t in self.__tivos
         ]
 
     def __find_tivos(self):
         class ZCListener:
             def __init__(self, names):
```

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/ws.py` & `ezmote-cmdserver-0.8.0/cmdserver/ws.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/cmdserver/zeroconf.py` & `ezmote-cmdserver-0.8.0/cmdserver/zeroconf.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/PKG-INFO` & `ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ezmote-cmdserver
-Version: 0.7.9
+Version: 0.8.0
 Summary: A small webapp which can be used for web based home cinema automation
 Home-page: http://github.com/3ll3d00d/cmdserver
 Author: Matt Khan
 Author-email: mattkhan+cmdserver@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -167,9 +166,7 @@
     debug: false
     debugLogging: true
     host: megatron
     port: 53199
     useTwisted: true
     # use for debug
     webappPath: 'C:\Users\mattk\github\ezmote\build'
-
-
```

### Comparing `ezmote-cmdserver-0.7.9/ezmote_cmdserver.egg-info/requires.txt` & `ezmote-cmdserver-0.8.0/ezmote_cmdserver.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-autobahn[twisted]==22.7.1
-automat==20.2.0
+autobahn[twisted]==23.1.2
+automat==22.10.0
 cffi==1.15.1
 constantly==15.1.0
-flask==2.1.3
-flask-restx==0.5.1
+flask==2.3.2
+flask-restx==1.1.0
 hyperlink==21.0.0
-incremental==21.3.0
+incremental==22.10.0
 netifaces==0.11.0
-plumbum==1.7.2
+plumbum==1.8.1
 pymcws==1.1.0
-pytz==2022.2.1
+pytz==2023.3
 pyyaml==6.0
-requests==2.28.1
-wakeonlan==2.1.0
-werkzeug==2.1.2
-
-[:python_full_version >= "3.6.0"]
-certifi==2022.6.15.1
-charset-normalizer==2.1.1
-cryptography==38.0.1
-txaio==22.2.1
+requests==2.29.0
+wakeonlan==3.0.0
+werkzeug==2.3.3
+
+[:python_full_version >= "3.7.0"]
+blinker==1.6.2
+charset-normalizer==3.1.0
+click==8.1.3
+itsdangerous==2.1.2
+jinja2==3.1.2
+jsonschema==4.17.3
+markupsafe==2.1.2
+pillow==9.5.0
+pyrsistent==0.19.3
+setuptools==67.7.2
+txaio==23.1.1
+typing-extensions==4.5.0
+zipp==3.15.0
 
 [:python_full_version >= "3.7.1"]
-twisted==22.8.0
+twisted==22.10.0
 
 [:python_version < "3.10"]
-importlib-metadata==4.12.0
+importlib-metadata==6.6.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 pycparser==2.21
 six==1.16.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"]
-zope.interface==5.4.0
+zope.interface==6.0
 
-[:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version < "4"]
-urllib3==1.26.12
+[:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5"]
+urllib3==1.26.15
 
 [:python_version >= "3.5"]
 aniso8601==9.0.1
-attrs==22.1.0
-idna==3.3
+attrs==23.1.0
+idna==3.4
 
-[:python_version >= "3.7"]
-click==8.1.3
-itsdangerous==2.1.2
-jinja2==3.1.2
-jsonschema==4.16.0
-markupsafe==2.1.1
-pillow==9.2.0
-pyrsistent==0.18.1
-setuptools==65.3.0
-typing-extensions==4.3.0
-zipp==3.8.1
+[:python_version >= "3.6"]
+certifi==2022.12.7
+cryptography==40.0.2
```

### Comparing `ezmote-cmdserver-0.7.9/setup.py` & `ezmote-cmdserver-0.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,50 +30,51 @@
     entry_points={
         "console_scripts": [
             "cmdserver = cmdserver.main:main",
         ],
     },
     install_requires=[
         "aniso8601==9.0.1; python_version >= '3.5'",
-        "attrs==22.1.0; python_version >= '3.5'",
-        "autobahn[twisted]==22.7.1",
-        "automat==20.2.0",
-        "certifi==2022.6.15.1; python_full_version >= '3.6.0'",
+        "attrs==23.1.0; python_version >= '3.5'",
+        "autobahn[twisted]==23.1.2",
+        "automat==22.10.0",
+        "blinker==1.6.2; python_full_version >= '3.7.0'",
+        "certifi==2022.12.7; python_version >= '3.6'",
         "cffi==1.15.1",
-        "charset-normalizer==2.1.1; python_full_version >= '3.6.0'",
-        "click==8.1.3; python_version >= '3.7'",
+        "charset-normalizer==3.1.0; python_full_version >= '3.7.0'",
+        "click==8.1.3; python_full_version >= '3.7.0'",
         "constantly==15.1.0",
-        "cryptography==38.0.1; python_full_version >= '3.6.0'",
-        "flask==2.1.3",
-        "flask-restx==0.5.1",
+        "cryptography==40.0.2; python_version >= '3.6'",
+        "flask==2.3.2",
+        "flask-restx==1.1.0",
         "hyperlink==21.0.0",
-        "idna==3.3; python_version >= '3.5'",
-        "importlib-metadata==4.12.0; python_version < '3.10'",
-        "incremental==21.3.0",
-        "itsdangerous==2.1.2; python_version >= '3.7'",
-        "jinja2==3.1.2; python_version >= '3.7'",
-        "jsonschema==4.16.0; python_version >= '3.7'",
-        "markupsafe==2.1.1; python_version >= '3.7'",
+        "idna==3.4; python_version >= '3.5'",
+        "importlib-metadata==6.6.0; python_version < '3.10'",
+        "incremental==22.10.0",
+        "itsdangerous==2.1.2; python_full_version >= '3.7.0'",
+        "jinja2==3.1.2; python_full_version >= '3.7.0'",
+        "jsonschema==4.17.3; python_full_version >= '3.7.0'",
+        "markupsafe==2.1.2; python_full_version >= '3.7.0'",
         "netifaces==0.11.0",
-        "pillow==9.2.0; python_version >= '3.7'",
-        "plumbum==1.7.2",
+        "pillow==9.5.0; python_full_version >= '3.7.0'",
+        "plumbum==1.8.1",
         "pycparser==2.21; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
         "pymcws==1.1.0",
-        "pyrsistent==0.18.1; python_version >= '3.7'",
-        "pytz==2022.2.1",
+        "pyrsistent==0.19.3; python_full_version >= '3.7.0'",
+        "pytz==2023.3",
         "pyyaml==6.0",
-        "requests==2.28.1",
-        "setuptools==65.3.0; python_version >= '3.7'",
+        "requests==2.29.0",
+        "setuptools==67.7.2; python_full_version >= '3.7.0'",
         "six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-        "twisted==22.8.0; python_full_version >= '3.7.1'",
-        "txaio==22.2.1; python_full_version >= '3.6.0'",
-        "typing-extensions==4.3.0; python_version >= '3.7'",
-        "urllib3==1.26.12; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version < '4'",
-        "wakeonlan==2.1.0",
-        "werkzeug==2.1.2",
-        "zipp==3.8.1; python_version >= '3.7'",
-        "zope.interface==5.4.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+        "twisted==22.10.0; python_full_version >= '3.7.1'",
+        "txaio==23.1.1; python_full_version >= '3.7.0'",
+        "typing-extensions==4.5.0; python_full_version >= '3.7.0'",
+        "urllib3==1.26.15; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
+        "wakeonlan==3.0.0",
+        "werkzeug==2.3.3",
+        "zipp==3.15.0; python_full_version >= '3.7.0'",
+        "zope.interface==6.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'"
     ],
     tests_require=["pytest", "pytest-httpserver"],
     include_package_data=True,
     zip_safe=False,
 )
```

