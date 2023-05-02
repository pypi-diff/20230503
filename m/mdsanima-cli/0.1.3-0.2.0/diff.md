# Comparing `tmp/mdsanima_cli-0.1.3.tar.gz` & `tmp/mdsanima_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdsanima_cli-0.1.3.tar", last modified: Tue Feb 14 01:00:15 2023, max compression
+gzip compressed data, was "mdsanima_cli-0.2.0.tar", last modified: Tue May  2 22:12:21 2023, max compression
```

## Comparing `mdsanima_cli-0.1.3.tar` & `mdsanima_cli-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,57 @@
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-02-14 01:00:15.054505 mdsanima_cli-0.1.3/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1286 2023-02-06 23:07:45.000000 mdsanima_cli-0.1.3/.editorconfig
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-02-14 01:00:14.657504 mdsanima_cli-0.1.3/.github/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       12 2023-02-06 22:39:55.000000 mdsanima_cli-0.1.3/.github/CODEOWNERS
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3976 2023-02-07 03:12:36.000000 mdsanima_cli-0.1.3/.gitignore
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-02-14 01:00:14.678508 mdsanima_cli-0.1.3/.idea/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      207 2023-02-12 01:01:36.000000 mdsanima_cli-0.1.3/.idea/commands.md
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    12949 2023-02-14 00:57:51.000000 mdsanima_cli-0.1.3/CHANGELOG.md
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    11356 2023-02-06 20:37:22.000000 mdsanima_cli-0.1.3/LICENSE
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    18632 2023-02-14 01:00:15.051507 mdsanima_cli-0.1.3/PKG-INFO
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3410 2023-02-14 00:55:44.000000 mdsanima_cli-0.1.3/README.md
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2235 2023-02-14 00:57:40.000000 mdsanima_cli-0.1.3/package.json
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2936 2023-02-13 18:11:57.000000 mdsanima_cli-0.1.3/pyproject.toml
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       49 2023-02-13 18:11:57.000000 mdsanima_cli-0.1.3/requirements-dev.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       34 2023-02-06 21:06:17.000000 mdsanima_cli-0.1.3/requirements.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       38 2023-02-14 01:00:15.055505 mdsanima_cli-0.1.3/setup.cfg
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-02-14 01:00:14.699505 mdsanima_cli-0.1.3/src/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      149 2023-02-06 22:38:19.000000 mdsanima_cli-0.1.3/src/.gitkeep
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-02-14 01:00:14.860507 mdsanima_cli-0.1.3/src/mdsanima_cli/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      599 2023-02-13 23:08:46.000000 mdsanima_cli-0.1.3/src/mdsanima_cli/__init__.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      232 2023-02-12 01:01:36.000000 mdsanima_cli-0.1.3/src/mdsanima_cli/__main__.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      160 2023-02-14 01:00:13.000000 mdsanima_cli-0.1.3/src/mdsanima_cli/_version.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1538 2023-02-13 16:42:30.000000 mdsanima_cli-0.1.3/src/mdsanima_cli/parser.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1940 2023-02-14 00:39:41.000000 mdsanima_cli-0.1.3/src/mdsanima_cli/pixelart.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1028 2023-02-14 00:38:00.000000 mdsanima_cli-0.1.3/src/mdsanima_cli/utils.py
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-02-14 01:00:15.017505 mdsanima_cli-0.1.3/src/mdsanima_cli.egg-info/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    18632 2023-02-14 01:00:13.000000 mdsanima_cli-0.1.3/src/mdsanima_cli.egg-info/PKG-INFO
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      582 2023-02-14 01:00:14.000000 mdsanima_cli-0.1.3/src/mdsanima_cli.egg-info/SOURCES.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        1 2023-02-14 01:00:13.000000 mdsanima_cli-0.1.3/src/mdsanima_cli.egg-info/dependency_links.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       51 2023-02-14 01:00:13.000000 mdsanima_cli-0.1.3/src/mdsanima_cli.egg-info/entry_points.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       34 2023-02-14 01:00:13.000000 mdsanima_cli-0.1.3/src/mdsanima_cli.egg-info/requires.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       13 2023-02-14 01:00:13.000000 mdsanima_cli-0.1.3/src/mdsanima_cli.egg-info/top_level.txt
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:21.734365 mdsanima_cli-0.2.0/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1355 2023-04-29 22:46:08.000000 mdsanima_cli-0.2.0/.editorconfig
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       79 2023-04-29 22:45:41.000000 mdsanima_cli-0.2.0/.flake8
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.511366 mdsanima_cli-0.2.0/.github/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       12 2023-02-06 22:39:55.000000 mdsanima_cli-0.2.0/.github/CODEOWNERS
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3873 2023-04-17 16:49:55.000000 mdsanima_cli-0.2.0/.gitignore
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.535361 mdsanima_cli-0.2.0/.idea/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      969 2023-05-02 21:20:31.000000 mdsanima_cli-0.2.0/.idea/commands.md
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      744 2023-04-29 23:16:48.000000 mdsanima_cli-0.2.0/.pylintrc
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.558364 mdsanima_cli-0.2.0/.vscode/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      149 2023-04-17 16:49:55.000000 mdsanima_cli-0.2.0/.vscode/.gitkeep
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    12450 2023-05-02 22:09:00.000000 mdsanima_cli-0.2.0/CHANGELOG.md
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    11356 2023-02-06 20:37:22.000000 mdsanima_cli-0.2.0/LICENSE
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    20472 2023-05-02 22:12:21.731363 mdsanima_cli-0.2.0/PKG-INFO
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4625 2023-05-02 21:43:43.000000 mdsanima_cli-0.2.0/README.md
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.607367 mdsanima_cli-0.2.0/img/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    61689 2023-04-26 18:07:04.000000 mdsanima_cli-0.2.0/img/logo.png
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    68193 2023-04-01 01:28:09.000000 mdsanima_cli-0.2.0/img/watermark.png
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2566 2023-05-02 21:43:14.000000 mdsanima_cli-0.2.0/package.json
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3616 2023-05-01 19:35:27.000000 mdsanima_cli-0.2.0/pyproject.toml
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      106 2023-04-29 22:32:42.000000 mdsanima_cli-0.2.0/requirements-dev.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       48 2023-04-27 16:55:13.000000 mdsanima_cli-0.2.0/requirements.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       38 2023-05-02 22:12:21.736365 mdsanima_cli-0.2.0/setup.cfg
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.631362 mdsanima_cli-0.2.0/src/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      149 2023-02-06 22:38:19.000000 mdsanima_cli-0.2.0/src/.gitkeep
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.739363 mdsanima_cli-0.2.0/src/mdsanima_cli/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1797 2023-05-02 21:20:31.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/__init__.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      230 2023-05-01 18:23:04.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/__main__.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      160 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/_version.py
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:21.451364 mdsanima_cli-0.2.0/src/mdsanima_cli/command/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       47 2023-05-01 17:52:04.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/__init__.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1445 2023-05-02 12:48:58.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/check.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4013 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/grid.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2495 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/jpg.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3497 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/logo.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2062 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/number.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2817 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/pixelart.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2494 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/png.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2973 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/thumbnail.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2000 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/uuids.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4472 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/watermark.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2510 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/webp.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     5359 2023-05-02 21:20:31.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/parser.py
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:21.692364 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       47 2023-05-01 17:51:47.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/__init__.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     9503 2023-05-02 21:20:54.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/ascii.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      734 2023-05-01 17:54:54.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/exif.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4367 2023-05-02 21:32:20.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/print.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2398 2023-05-01 17:51:14.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/stats.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      564 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/timer.py
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.910361 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    20472 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/PKG-INFO
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1203 2023-05-02 22:12:20.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        1 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       79 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/entry_points.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       48 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/requires.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       13 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/top_level.txt
```

### Comparing `mdsanima_cli-0.1.3/.editorconfig` & `mdsanima_cli-0.2.0/.editorconfig`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright © 2023 Marcin Różewski MDSANIMA
+
 # https://editorconfig.org
 
 root = true
 
 [*]
 charset = utf-8
 end_of_line = lf
@@ -34,29 +36,30 @@
 indent_size = 2
 indent_style = space
 max_line_length = 120
 
 [*.json]
 indent_size = 2
 indent_style = space
-end_of_line = crlf
+end_of_line = lf
 
 [*.md]
 indent_size = 2
 indent_style = space
+max_line_length = 100
 
 [*.ps1]
 indent_size = 2
 indent_style = space
 
 [*.py]
 profile = black
 indent_size = 4
 indent_style = space
-max_line_length = 79
+max_line_length = 100
 
 [*.sh]
 indent_size = 2
 indent_style = space
 
 [*.svg]
 insert_final_newline = false
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mdsanima_cli-0.1.3/.gitignore` & `mdsanima_cli-0.2.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,121 +1,23 @@
-# Logs
-logs
-*.log
-npm-debug.log*
-yarn-debug.log*
-yarn-error.log*
-lerna-debug.log*
-
-# Diagnostic reports (https://nodejs.org/api/report.html)
-report.[0-9]*.[0-9]*.[0-9]*.[0-9]*.json
-
-# Runtime data
-pids
-*.pid
-*.seed
-*.pid.lock
-
-# Directory for instrumented libs generated by jscoverage/JSCover
-lib-cov
-
-# Coverage directory used by tools like istanbul
-coverage
-*.lcov
-
-# nyc test coverage
-.nyc_output
-
-# Grunt intermediate storage (https://gruntjs.com/creating-plugins#storing-task-files)
-.grunt
-
-# Bower dependency directory (https://bower.io/)
-bower_components
-
-# node-waf configuration
-.lock-wscript
-
-# Compiled binary addons (https://nodejs.org/api/addons.html)
-build/Release
-
-# Dependency directories
-node_modules/
-jspm_packages/
-
-# TypeScript v1 declaration files
-typings/
-
-# TypeScript cache
-*.tsbuildinfo
-
-# Optional npm cache directory
-.npm
-
-# Optional eslint cache
-.eslintcache
-
-# Microbundle cache
-.rpt2_cache/
-.rts2_cache_cjs/
-.rts2_cache_es/
-.rts2_cache_umd/
-
-# Optional REPL history
-.node_repl_history
-
-# Output of 'npm pack'
-*.tgz
-
-# Yarn Integrity file
-.yarn-integrity
-
-# parcel-bundler cache (https://parceljs.org/)
-.cache
-
-# Next.js build output
-.next
-
-# Nuxt.js build / generate output
-.nuxt
-dist
-
-# Gatsby files
-.cache/
-# Comment in the public line in if your project uses Gatsby and *not* Next.js
-# https://nextjs.org/blog/next-9-1#public-directory-support
-# public
-
-# vuepress build output
-.vuepress/dist
-
-# Serverless directories
-.serverless/
-
-# FuseBox cache
-.fusebox/
-
-# DynamoDB Local files
-.dynamodb/
-
-# TernJS port file
-.tern-port
+# See https://help.github.com/articles/ignoring-files/ for more about ignoring files
 
+# Python Template
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
-#dist/
+dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
@@ -224,54 +126,146 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
-# See https://help.github.com/articles/ignoring-files/ for more about ignoring files.
+# Kivy Python
+*/.buildozer*
+*/.KivyMD*
+*/.testing/cache*
+*/cache*
+*/build/
+*/.build*
+*/__pyca*
 
-# dependencies
-/node_modules
-/.pnp
+# Node Template
+# Logs
+logs
+*.log
+npm-debug.log*
+yarn-debug.log*
+yarn-error.log*
+lerna-debug.log*
+.pnpm-debug.log*
+
+# Diagnostic reports (https://nodejs.org/api/report.html)
+report.[0-9]*.[0-9]*.[0-9]*.[0-9]*.json
+
+# Runtime data
+pids
+*.pid
+*.seed
+*.pid.lock
+
+# Directory for instrumented libs generated by jscoverage/JSCover
+lib-cov
+
+# Coverage directory used by tools like istanbul
+coverage
+*.lcov
+
+# nyc test coverage
+.nyc_output
+
+# Grunt intermediate storage (https://gruntjs.com/creating-plugins#storing-task-files)
+.grunt
+
+# Bower dependency directory (https://bower.io/)
+bower_components
+
+# node-waf configuration
+.lock-wscript
+
+# Compiled binary addons (https://nodejs.org/api/addons.html)
+build/Release
+
+# Dependency directories
+node_modules/
+jspm_packages/
+.pnp
 .pnp.js
 
-# testing
-/coverage
+# TypeScript v1 declaration files
+typings/
+
+# TypeScript cache
+*.tsbuildinfo
+# next-env.d.ts
 
-# production
-/build
+# Optional npm cache directory
+.npm
 
-# misc
-.DS_Store
+# Optional eslint cache
+.eslintcache
 
-# in this file only store app version for docker compose and show in web
-# .env
+# Microbundle cache
+.rpt2_cache/
+.rts2_cache_cjs/
+.rts2_cache_es/
+.rts2_cache_umd/
+
+# Optional REPL history
+.node_repl_history
+
+# Output of 'npm pack'
+*.tgz
+
+# Yarn Integrity file
+.yarn-integrity
 
 # dotenv environment variables file
+.env
 .env.test
 .env.local
-.env.development.local
 .env.test.local
+.env.development.local
 .env.production.local
+.env*.local
 
-# log files debug
-npm-debug.log*
-yarn-debug.log*
-yarn-error.log*
+# parcel-bundler cache (https://parceljs.org/)
+.cache
 
-# Kivy Python
-*\.buildozer*
-*\.vscode*
-*\.KivyMD*
-*\.testing\cache*
-*\cache*
-*\build\
-*\.build*
-*\__pyca*
+# Next.js build output
+.next
+/out/
 
-# mdsanima folder
-tmp
-temp
+# Nuxt.js build / generate output
+.nuxt
+dist
+
+# vercel
+.vercel
+
+# Gatsby files
+.cache/
+# Comment in the public line in if your project uses Gatsby and *not* Next.js
+# https://nextjs.org/blog/next-9-1#public-directory-support
+# public
+
+# vuepress build output
+.vuepress/dist
+
+# Serverless directories
+.serverless/
+
+# FuseBox cache
+.fusebox/
+
+# DynamoDB Local files
+.dynamodb/
+
+# TernJS port file
+.tern-port
 
+# misc
+.DS_Store
+*.pem
+
+# MDSANIMA Template
 # setuptools_scm
 _version.py
+
+# temp folder
+tmp
+temp
```

### Comparing `mdsanima_cli-0.1.3/CHANGELOG.md` & `mdsanima_cli-0.2.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,128 +1,132 @@
 # CHANGELOG
 
 All notable changes to this project will be documented in this file.
 
-Please check
-[standard-version](https://github.com/conventional-changelog/standard-version)
+Please check [standard-version](https://github.com/conventional-changelog/standard-version)
 and documentation for commit guidelines. Also you should check
-[conventional-changelog](https://github.com/mdsanima/conventional-changelog)
-for more detail.
+[conventional-changelog](https://github.com/mdsanima/conventional-changelog) for more detail.
 
-Docomentation for _MDSANIMA-CLI_
-is available at this repository on `README.md` files be sure to check it.
+Docomentation for _MDSANIMA-CLI_ is available at this repository on [README.md](README.md)
+file be sure to check it.
+
+## 0.2.0 (2023-05-02)
+
+### ⚠ BREAKING CHANGES
+
+- **dev:** helper function for print done message in color
+- module prefix `cli` rename file
+- more stats info for `get_directory_info` function
+
+- module prefix `cli` rename file ([bd745a4](https://github.com/mdsanima-lab/mdsanima-cli/commit/bd745a444d2b481712840951c0ea93133e4555e8))
+
+### BUG FIXES
+
+- calculating align spaces for nice printing ([760a99d](https://github.com/mdsanima-lab/mdsanima-cli/commit/760a99dfa6344260afe71ca2c1d9c4bd66e6aac1))
+- generate pixel art only once closes [#23](https://github.com/mdsanima-lab/mdsanima-cli/issues/23) ([6ef48ec](https://github.com/mdsanima-lab/mdsanima-cli/commit/6ef48ec08424464c91252b4ae0c76d62ff40d7d1))
+
+### DOCUMENTATION
+
+- add documentation for `number` command ([a1f4415](https://github.com/mdsanima-lab/mdsanima-cli/commit/a1f4415e305d175fc3696c2834b6415210d605e9))
+- add documentation for `uuid` command ([81fbc91](https://github.com/mdsanima-lab/mdsanima-cli/commit/81fbc91dfac9c533b413829e6634981bde60a229))
+- adding command ideas and fixing some typos ([28f91ff](https://github.com/mdsanima-lab/mdsanima-cli/commit/28f91ffbcdc0c7c43f6582c7dee2c8674c10501e))
+- fixing typo ([a0416b3](https://github.com/mdsanima-lab/mdsanima-cli/commit/a0416b3a7893421e277c56d16d9e740aeca3cf01))
+- info about always printed in upper caase ([cd0a9e9](https://github.com/mdsanima-lab/mdsanima-cli/commit/cd0a9e9556906237f4c9b27726f2d46be4e2b3f4))
+- more command ideas ([fe56c2b](https://github.com/mdsanima-lab/mdsanima-cli/commit/fe56c2b52dd56939548ca11fca218903e2335545))
+- new commands ideas and fixing some documentation string ([8731ba6](https://github.com/mdsanima-lab/mdsanima-cli/commit/8731ba6a29bec11c0189a606a50fa3398fc7fef6))
+
+### FEATURES
+
+- add parser for check command ([b589d7a](https://github.com/mdsanima-lab/mdsanima-cli/commit/b589d7a8c55c85bd7f6299726ca87445139b7c80))
+- add watermark command closes [#37](https://github.com/mdsanima-lab/mdsanima-cli/issues/37) ([ef714a6](https://github.com/mdsanima-lab/mdsanima-cli/commit/ef714a61174b1d0a61d55387152d623af6d3bb75))
+- adding exif data software and user comment closes [#20](https://github.com/mdsanima-lab/mdsanima-cli/issues/20) ([2753490](https://github.com/mdsanima-lab/mdsanima-cli/commit/2753490779740eebe88a2eb04f2dd357b7297208))
+- adding support for `.webp` files closes [#10](https://github.com/mdsanima-lab/mdsanima-cli/issues/10) ([b6aa51a](https://github.com/mdsanima-lab/mdsanima-cli/commit/b6aa51aeb50c74700ff2970556a658e905da7f41))
+- alias `mds` for main cli closes [#32](https://github.com/mdsanima-lab/mdsanima-cli/issues/32) ([671094c](https://github.com/mdsanima-lab/mdsanima-cli/commit/671094c87529ebf289d1fb5be1ebabd5e3d005e3))
+- append a logo to image closes [#12](https://github.com/mdsanima-lab/mdsanima-cli/issues/12) ([2bab517](https://github.com/mdsanima-lab/mdsanima-cli/commit/2bab5178ab60a8d607a6ac0ec05f5ca39f7c8549))
+- ascii art text for printing title closes [#30](https://github.com/mdsanima-lab/mdsanima-cli/issues/30) ([6f70d61](https://github.com/mdsanima-lab/mdsanima-cli/commit/6f70d61c147489acb9a9a52936dce2bc38bddc8c)), closes [#26](https://github.com/mdsanima-lab/mdsanima-cli/issues/26)
+- checking system dependencies color info print ([139eebe](https://github.com/mdsanima-lab/mdsanima-cli/commit/139eebeec1aaf23f19270e8842d98c9aa9f0dc7a))
+- color print for compute pixelart and show count number ([d46ec2b](https://github.com/mdsanima-lab/mdsanima-cli/commit/d46ec2b9854e4dba89b6573987e08fb6a40b3e6a))
+- converting images to `jpg` format closes [#39](https://github.com/mdsanima-lab/mdsanima-cli/issues/39) ([e51fbea](https://github.com/mdsanima-lab/mdsanima-cli/commit/e51fbeaa3f904e277b4b3106ac93f8d959fa1832))
+- converting images to `png` format closes [#40](https://github.com/mdsanima-lab/mdsanima-cli/issues/40) ([00ba0db](https://github.com/mdsanima-lab/mdsanima-cli/commit/00ba0dbd3403580bffbdfb6bbdc63e10c7ee85b4))
+- converting images to `webp` format closes [#13](https://github.com/mdsanima-lab/mdsanima-cli/issues/13) ([fd1f60d](https://github.com/mdsanima-lab/mdsanima-cli/commit/fd1f60d94ec58940cda3c454d1efa874bfb6229b))
+- **dev:** ascii art `completed` title ([349890a](https://github.com/mdsanima-lab/mdsanima-cli/commit/349890a1cb92d2305e62c81a2c62fe45089bde2a))
+- **dev:** ascii art `config error` title ([c48df0f](https://github.com/mdsanima-lab/mdsanima-cli/commit/c48df0f02713764ae71e3495abfcd6ca3bd68c1e))
+- **dev:** ascii characters numbers and some special closes [#34](https://github.com/mdsanima-lab/mdsanima-cli/issues/34) ([6bf95fa](https://github.com/mdsanima-lab/mdsanima-cli/commit/6bf95fa321544c5c9c1a4b5e77803a51d54b37bb))
+- **dev:** helper for printing multiple colors in on line ([c8824e1](https://github.com/mdsanima-lab/mdsanima-cli/commit/c8824e143c7384eedeffaa24d2363985ac33b3a1))
+- **dev:** helper function for print done message in color ([aaac99f](https://github.com/mdsanima-lab/mdsanima-cli/commit/aaac99f54deb65632d4f360842b0cc66bea407e4))
+- directory info for `gif` file and `get_images_count` function ([769fca2](https://github.com/mdsanima-lab/mdsanima-cli/commit/769fca21214cd66fa8fcc73f71b3e6114a2333d8))
+- execution timer in seconds closes [#38](https://github.com/mdsanima-lab/mdsanima-cli/issues/38) ([d1b37c2](https://github.com/mdsanima-lab/mdsanima-cli/commit/d1b37c2cbc3c5c001be43b503a9b2f3f7126e766))
+- generate grid 2x2 from all images in current dir closes [#15](https://github.com/mdsanima-lab/mdsanima-cli/issues/15) ([9731063](https://github.com/mdsanima-lab/mdsanima-cli/commit/9731063c3068d56333a37b78b373c0776e1eb6dd))
+- generate jpeg thumbnail 128px closes [#17](https://github.com/mdsanima-lab/mdsanima-cli/issues/17) ([8daccc9](https://github.com/mdsanima-lab/mdsanima-cli/commit/8daccc9dfbed5b2d0f01805b1a1c336fda43c832))
+- more stats info for `get_directory_info` function ([c75e825](https://github.com/mdsanima-lab/mdsanima-cli/commit/c75e8254c2b3d3cb100cba15823abb3325496a42))
+- print multiple colors in on line for computing files info ([7874a69](https://github.com/mdsanima-lab/mdsanima-cli/commit/7874a69b81a647deab2ad296146e9f4c867b978a))
+- print multiple colors in on line for processing files info ([75ec73c](https://github.com/mdsanima-lab/mdsanima-cli/commit/75ec73c0a5e8c9f7061c3e65988de8bd90542f37))
+- print nice asci text ([6681b3c](https://github.com/mdsanima-lab/mdsanima-cli/commit/6681b3c5833a25773a35727649f2bbd7c434634b))
+- printing directory info stats in color ([657f230](https://github.com/mdsanima-lab/mdsanima-cli/commit/657f230cd2c3641885dd39e2e1cda10b05f180f8))
+- rename all images to `uuid` in current directory closes [#11](https://github.com/mdsanima-lab/mdsanima-cli/issues/11) ([81be311](https://github.com/mdsanima-lab/mdsanima-cli/commit/81be31170e6b211bd88da287440ae2872a437b40))
+- rename file name to seq number closes [#36](https://github.com/mdsanima-lab/mdsanima-cli/issues/36) ([ab90088](https://github.com/mdsanima-lab/mdsanima-cli/commit/ab90088cc84b56bec932abd1923c57f00d81eef5))
 
 ### 0.1.3 (2023-02-14)
 
 ### FEATURES
 
-- add codeowners file ([f0976fd](https://github.com/mdsanima-lab/mdsanima-cli/commit/f0976fd8bdbd9e5efb1d0c97a7619f822c6fb062))
-- add help for commands closes [#3](https://github.com/mdsanima-lab/mdsanima-cli/issues/3) ([48f3a5b](https://github.com/mdsanima-lab/mdsanima-cli/commit/48f3a5beff1a785e5690b07a01ede87c8dd479af))
 - checking directory and get information closes [#8](https://github.com/mdsanima-lab/mdsanima-cli/issues/8) ([3c098f3](https://github.com/mdsanima-lab/mdsanima-cli/commit/3c098f3f2c6447c286842c30c0127010c1b86189))
 - detecting only `.jpg` and `.png` files closes [#7](https://github.com/mdsanima-lab/mdsanima-cli/issues/7) ([7018793](https://github.com/mdsanima-lab/mdsanima-cli/commit/7018793b3c2eecff09eafe49293dab5af2a05e83))
-- first `mdsanima` test terminal command ([7b986c3](https://github.com/mdsanima-lab/mdsanima-cli/commit/7b986c3d438e2f2732668926fb46fe6fd98c003f))
-- first stage of generate pixelart from images closes [#5](https://github.com/mdsanima-lab/mdsanima-cli/issues/5) ([cffb8db](https://github.com/mdsanima-lab/mdsanima-cli/commit/cffb8db05771742e301963d1578ef332a66f0c11))
-- initial parser for pixelart and gifmaker command closes [#1](https://github.com/mdsanima-lab/mdsanima-cli/issues/1) ([fe93d2d](https://github.com/mdsanima-lab/mdsanima-cli/commit/fe93d2d0b926517cd37821f87a189372e3a834d7))
 - print color info for `compute_pixelart` function closes [#6](https://github.com/mdsanima-lab/mdsanima-cli/issues/6) ([91e1789](https://github.com/mdsanima-lab/mdsanima-cli/commit/91e1789a65c67a401b014531fee16292ffeab624))
 
 ### BUG FIXES
 
-- add build setup python toml and requirements ([7c29973](https://github.com/mdsanima-lab/mdsanima-cli/commit/7c299738195db54de58016dd3d87b94a16ee901e))
-- add specific version and keywords typo ([3264da9](https://github.com/mdsanima-lab/mdsanima-cli/commit/3264da983027df9b1c568130d0def5b309113a52))
-- add year and name ([c5ea0ff](https://github.com/mdsanima-lab/mdsanima-cli/commit/c5ea0ff02f6fea87be7d943df2bad071f3ad4ef7))
-- adding dev python requirements ([53f9c76](https://github.com/mdsanima-lab/mdsanima-cli/commit/53f9c7636e703157e08250c3fb280f88243ce94f))
-- color print closes [#2](https://github.com/mdsanima-lab/mdsanima-cli/issues/2) ([4751202](https://github.com/mdsanima-lab/mdsanima-cli/commit/47512022c47756d026c58d11c4847b9e1d51a9d1))
-- crlf to lf ([b00e68a](https://github.com/mdsanima-lab/mdsanima-cli/commit/b00e68a1552e947196171ab2e0ad1838727b9134))
 - directory info counting files closes [#9](https://github.com/mdsanima-lab/mdsanima-cli/issues/9) ([577f8c5](https://github.com/mdsanima-lab/mdsanima-cli/commit/577f8c56512f38230b84deb2078c316f7a870a1a))
-- editor confit and ignore ([cb55349](https://github.com/mdsanima-lab/mdsanima-cli/commit/cb553492375143bb8394ef4ecef2b91953f90448))
-- ignore `_version.py` file for setuptools_scm ([6105ba8](https://github.com/mdsanima-lab/mdsanima-cli/commit/6105ba88dfd2e83994705ccc9a93d70753671762))
-- main cli entry point ([d126691](https://github.com/mdsanima-lab/mdsanima-cli/commit/d1266918e5ccb3afe7ce83a35339feca6a722bf5))
-- setup toml and init file ([7066cd3](https://github.com/mdsanima-lab/mdsanima-cli/commit/7066cd397d9719fa9ef86a772803319cbcfbddf8))
 
 ### DOCUMENTATION
 
-- add documentation for creating release version and deploying ([32814c3](https://github.com/mdsanima-lab/mdsanima-cli/commit/32814c3cd477643a1f9f60eac561ca0f70ad5ff1))
-- build install and testing package info for development ([a12f572](https://github.com/mdsanima-lab/mdsanima-cli/commit/a12f57281f98ff16768e0c62d7bafca57b1e49c6))
-- commands idea and info before build ([54273aa](https://github.com/mdsanima-lab/mdsanima-cli/commit/54273aac2f67dba808f76d1b3a283bb3dc05bb64))
-- development setup info ([5c23718](https://github.com/mdsanima-lab/mdsanima-cli/commit/5c2371801c5b571c4f85bcd2dbaa9e72402b3f8a))
-- extracts version package from git ([1cb83ee](https://github.com/mdsanima-lab/mdsanima-cli/commit/1cb83ee1626d99f6b07935b84adbccbe9463ff12))
-- first cli command `mdsanima pixelart` documentation info ([09bfd68](https://github.com/mdsanima-lab/mdsanima-cli/commit/09bfd683e259cf7eaa3b97f5c93eb209bd23f46e))
 - fixing command for pushing tag to origin ([91b78a3](https://github.com/mdsanima-lab/mdsanima-cli/commit/91b78a3cd705820b6913321e1351b6ce47d82455))
 - fixing information for updating to pypi ([68d1912](https://github.com/mdsanima-lab/mdsanima-cli/commit/68d1912a26cc93d22cd0804bcdd80f70d9d86d16))
 - info for updating to latest version ([3188ed5](https://github.com/mdsanima-lab/mdsanima-cli/commit/3188ed599592af16143a31f4c0d3f7f51778b866))
-- installation info for first test command ([0a33a76](https://github.com/mdsanima-lab/mdsanima-cli/commit/0a33a76ad6fdbc1ad990b982359435f7cbfce266))
 
 ### 0.1.2 (2023-02-13)
 
 ### FEATURES
 
-- add codeowners file ([f0976fd](https://github.com/mdsanima-lab/mdsanima-cli/commit/f0976fd8bdbd9e5efb1d0c97a7619f822c6fb062))
-- add help for commands closes [#3](https://github.com/mdsanima-lab/mdsanima-cli/issues/3) ([48f3a5b](https://github.com/mdsanima-lab/mdsanima-cli/commit/48f3a5beff1a785e5690b07a01ede87c8dd479af))
-- first `mdsanima` test terminal command ([7b986c3](https://github.com/mdsanima-lab/mdsanima-cli/commit/7b986c3d438e2f2732668926fb46fe6fd98c003f))
 - first stage of generate pixelart from images closes [#5](https://github.com/mdsanima-lab/mdsanima-cli/issues/5) ([cffb8db](https://github.com/mdsanima-lab/mdsanima-cli/commit/cffb8db05771742e301963d1578ef332a66f0c11))
-- initial parser for pixelart and gifmaker command closes [#1](https://github.com/mdsanima-lab/mdsanima-cli/issues/1) ([fe93d2d](https://github.com/mdsanima-lab/mdsanima-cli/commit/fe93d2d0b926517cd37821f87a189372e3a834d7))
 
 ### BUG FIXES
 
-- add build setup python toml and requirements ([7c29973](https://github.com/mdsanima-lab/mdsanima-cli/commit/7c299738195db54de58016dd3d87b94a16ee901e))
 - add specific version and keywords typo ([3264da9](https://github.com/mdsanima-lab/mdsanima-cli/commit/3264da983027df9b1c568130d0def5b309113a52))
-- add year and name ([c5ea0ff](https://github.com/mdsanima-lab/mdsanima-cli/commit/c5ea0ff02f6fea87be7d943df2bad071f3ad4ef7))
 - adding dev python requirements ([53f9c76](https://github.com/mdsanima-lab/mdsanima-cli/commit/53f9c7636e703157e08250c3fb280f88243ce94f))
-- color print closes [#2](https://github.com/mdsanima-lab/mdsanima-cli/issues/2) ([4751202](https://github.com/mdsanima-lab/mdsanima-cli/commit/47512022c47756d026c58d11c4847b9e1d51a9d1))
-- crlf to lf ([b00e68a](https://github.com/mdsanima-lab/mdsanima-cli/commit/b00e68a1552e947196171ab2e0ad1838727b9134))
-- editor confit and ignore ([cb55349](https://github.com/mdsanima-lab/mdsanima-cli/commit/cb553492375143bb8394ef4ecef2b91953f90448))
-- ignore `_version.py` file for setuptools_scm ([6105ba8](https://github.com/mdsanima-lab/mdsanima-cli/commit/6105ba88dfd2e83994705ccc9a93d70753671762))
-- main cli entry point ([d126691](https://github.com/mdsanima-lab/mdsanima-cli/commit/d1266918e5ccb3afe7ce83a35339feca6a722bf5))
-- setup toml and init file ([7066cd3](https://github.com/mdsanima-lab/mdsanima-cli/commit/7066cd397d9719fa9ef86a772803319cbcfbddf8))
 
 ### DOCUMENTATION
 
 - add documentation for creating release version and deploying ([32814c3](https://github.com/mdsanima-lab/mdsanima-cli/commit/32814c3cd477643a1f9f60eac561ca0f70ad5ff1))
-- build install and testing package info for development ([a12f572](https://github.com/mdsanima-lab/mdsanima-cli/commit/a12f57281f98ff16768e0c62d7bafca57b1e49c6))
-- commands idea and info before build ([54273aa](https://github.com/mdsanima-lab/mdsanima-cli/commit/54273aac2f67dba808f76d1b3a283bb3dc05bb64))
-- development setup info ([5c23718](https://github.com/mdsanima-lab/mdsanima-cli/commit/5c2371801c5b571c4f85bcd2dbaa9e72402b3f8a))
-- extracts version package from git ([1cb83ee](https://github.com/mdsanima-lab/mdsanima-cli/commit/1cb83ee1626d99f6b07935b84adbccbe9463ff12))
 - first cli command `mdsanima pixelart` documentation info ([09bfd68](https://github.com/mdsanima-lab/mdsanima-cli/commit/09bfd683e259cf7eaa3b97f5c93eb209bd23f46e))
-- installation info for first test command ([0a33a76](https://github.com/mdsanima-lab/mdsanima-cli/commit/0a33a76ad6fdbc1ad990b982359435f7cbfce266))
 
 ### 0.1.1 (2023-02-12)
 
 ### DOCUMENTATION
 
-- build install and testing package info for development ([a12f572](https://github.com/mdsanima-lab/mdsanima-cli/commit/a12f57281f98ff16768e0c62d7bafca57b1e49c6))
 - commands idea and info before build ([54273aa](https://github.com/mdsanima-lab/mdsanima-cli/commit/54273aac2f67dba808f76d1b3a283bb3dc05bb64))
-- development setup info ([5c23718](https://github.com/mdsanima-lab/mdsanima-cli/commit/5c2371801c5b571c4f85bcd2dbaa9e72402b3f8a))
-- extracts version package from git ([1cb83ee](https://github.com/mdsanima-lab/mdsanima-cli/commit/1cb83ee1626d99f6b07935b84adbccbe9463ff12))
-- installation info for first test command ([0a33a76](https://github.com/mdsanima-lab/mdsanima-cli/commit/0a33a76ad6fdbc1ad990b982359435f7cbfce266))
 
 ### FEATURES
 
-- add codeowners file ([f0976fd](https://github.com/mdsanima-lab/mdsanima-cli/commit/f0976fd8bdbd9e5efb1d0c97a7619f822c6fb062))
 - add help for commands closes [#3](https://github.com/mdsanima-lab/mdsanima-cli/issues/3) ([48f3a5b](https://github.com/mdsanima-lab/mdsanima-cli/commit/48f3a5beff1a785e5690b07a01ede87c8dd479af))
-- first `mdsanima` test terminal command ([7b986c3](https://github.com/mdsanima-lab/mdsanima-cli/commit/7b986c3d438e2f2732668926fb46fe6fd98c003f))
 - initial parser for pixelart and gifmaker command closes [#1](https://github.com/mdsanima-lab/mdsanima-cli/issues/1) ([fe93d2d](https://github.com/mdsanima-lab/mdsanima-cli/commit/fe93d2d0b926517cd37821f87a189372e3a834d7))
 
 ### BUG FIXES
 
-- add build setup python toml and requirements ([7c29973](https://github.com/mdsanima-lab/mdsanima-cli/commit/7c299738195db54de58016dd3d87b94a16ee901e))
-- add year and name ([c5ea0ff](https://github.com/mdsanima-lab/mdsanima-cli/commit/c5ea0ff02f6fea87be7d943df2bad071f3ad4ef7))
 - color print closes [#2](https://github.com/mdsanima-lab/mdsanima-cli/issues/2) ([4751202](https://github.com/mdsanima-lab/mdsanima-cli/commit/47512022c47756d026c58d11c4847b9e1d51a9d1))
 - crlf to lf ([b00e68a](https://github.com/mdsanima-lab/mdsanima-cli/commit/b00e68a1552e947196171ab2e0ad1838727b9134))
-- editor confit and ignore ([cb55349](https://github.com/mdsanima-lab/mdsanima-cli/commit/cb553492375143bb8394ef4ecef2b91953f90448))
-- ignore `_version.py` file for setuptools_scm ([6105ba8](https://github.com/mdsanima-lab/mdsanima-cli/commit/6105ba88dfd2e83994705ccc9a93d70753671762))
 - main cli entry point ([d126691](https://github.com/mdsanima-lab/mdsanima-cli/commit/d1266918e5ccb3afe7ce83a35339feca6a722bf5))
-- setup toml and init file ([7066cd3](https://github.com/mdsanima-lab/mdsanima-cli/commit/7066cd397d9719fa9ef86a772803319cbcfbddf8))
 
 ## 0.1.0 (2023-02-07)
 
 ### BUG FIXES
 
 - add build setup python toml and requirements ([7c29973](https://github.com/mdsanima-lab/mdsanima-cli/commit/7c299738195db54de58016dd3d87b94a16ee901e))
 - add year and name ([c5ea0ff](https://github.com/mdsanima-lab/mdsanima-cli/commit/c5ea0ff02f6fea87be7d943df2bad071f3ad4ef7))
-- editor confit and ignore ([cb55349](https://github.com/mdsanima-lab/mdsanima-cli/commit/cb553492375143bb8394ef4ecef2b91953f90448))
+- editor config and ignore ([cb55349](https://github.com/mdsanima-lab/mdsanima-cli/commit/cb553492375143bb8394ef4ecef2b91953f90448))
 - ignore `_version.py` file for setuptools_scm ([6105ba8](https://github.com/mdsanima-lab/mdsanima-cli/commit/6105ba88dfd2e83994705ccc9a93d70753671762))
 - setup toml and init file ([7066cd3](https://github.com/mdsanima-lab/mdsanima-cli/commit/7066cd397d9719fa9ef86a772803319cbcfbddf8))
 
 ### DOCUMENTATION
 
 - build install and testing package info for development ([a12f572](https://github.com/mdsanima-lab/mdsanima-cli/commit/a12f57281f98ff16768e0c62d7bafca57b1e49c6))
 - development setup info ([5c23718](https://github.com/mdsanima-lab/mdsanima-cli/commit/5c2371801c5b571c4f85bcd2dbaa9e72402b3f8a))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mdsanima_cli-0.1.3/LICENSE` & `mdsanima_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdsanima_cli-0.1.3/PKG-INFO` & `mdsanima_cli-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mdsanima_cli
-Version: 0.1.3
-Summary: Command line tools for images processing, generating pixel art, adding logo to images and many more.
+Version: 0.2.0
+Summary: The package will provide command-line tools for image processing, generating pixel art, adding logos to images, and much more.
 Author-email: Marcin Różewski <marcinrozewski@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -205,16 +205,16 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: homepage, https://github.com/mdsanima-lab/mdsanima-cli
 Project-URL: documentation, https://github.com/mdsanima-lab/mdsanima-cli#readme
 Project-URL: repository, https://github.com/mdsanima-lab/mdsanima-cli.git
 Project-URL: changelog, https://github.com/mdsanima-lab/mdsanima-cli/blob/main/CHANGELOG.md
-Keywords: cli,command-line,console-app,console-application,exif metadata,image-processing,images,mdsanima command line,mdsanima-cli,mdsanima-dev,mdsanima,meta information,pixelart,python-library,python,python3,shell-script
-Classifier: Development Status :: 1 - Planning
+Keywords: bash,cli,command-line,console-app,console-application,exif metadata,exif,image-processing,images,logo,mdsanima command line,mdsanima command-line,mdsanima-cli,mdsanima-dev,mdsanima,meta information,pixel art,pixelart,python-library,python,python3,shell-script,shell,watermark,zsh
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Legal Industry
@@ -229,181 +229,213 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Desktop Environment
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Graphics :: Editors
 Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System
 Classifier: Topic :: System :: Console Fonts
+Classifier: Topic :: System :: Filesystems
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: System :: Operating System
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mdsanima-cli
 
-Command line tools for images processing, generating pixel art, adding logo to
-images and many more.
+The package will provide command-line tools for image processing, generating pixel art, adding logos
+to images, and much more.
 
 ## Installation
 
 Install latest version:
 
-```bash
+```shell
 python3 -m pip install mdsanima-cli
 ```
 
 Updating to latest version:
 
-```bash
+```shell
 python3 -m pip install --upgrade mdsanima-cli
 ```
 
 ## Terminal Commands
 
 Now you can use this command in terminal:
 
-```bash
+```shell
 mdsanima
 ```
 
-The response is printing help how to use this command line tools.
+The response is printing help how to use this command-line tools.
 
-### CLI
+You can use the `mdsanima` command or the `mds` alias, which have the same functionality.
 
-Avaiable command for this package.
+### CLI
 
-```bash
-mdsanima pixelart
-```
+Avaiable command for this package:
 
-This command works in folder that have only `.png` images and convert this
-image to pixel art with creating new file with append suffix `pixelart` to
-original file name.
+- `mdsanima` main command showing help
+- `mdsanima check` print directory info
+- `mdsanima uuid` rename to uuid
+- `mdsanima number` rename to seq numbers
+- `mdsanima logo` append a logo
+- `mdsanima watermark` append a watermark
+- `mdsanima jpg` convert to jpg
+- `mdsanima png` convert to png
+- `mdsanima webp` convert to webp
+- `mdsanima pixelart` generate pixel art 32px
+- `mdsanima grid` generate grid 2x2
+- `mdsanima thumbnail` generate jpeg thumbnail 128px
+
+The `pixelart` command works in folder that have only `.png` images and convert this images to pixel
+art with creating the new file and appending the suffix `pixelart` to original file name.
+
+After executing this command, all image files in the folder you are in will be processed.
+The command does not delete any files in the folder, it only adds new ones and showing the directory
+info.
 
 ## Development Setup
 
 Instruction step how to setup development environent is here on this
-[workflow](https://mdsanima-dev.github.io/mdsanima-dev/development/workflow/)
-instruction.
+[workflow](https://mdsanima-dev.github.io/mdsanima-dev/development/workflow/) instruction.
 
-Creating isolated environment with specific pip version then activate and
-install requirements, type in terminal:
+Creating isolated environment with specific pip version then activate and install requirements, type
+in terminal:
 
-```bash
-virtualenv --pip 23.0 .venv
+```shell
+virtualenv --setuptools 67.7.2 --wheel 0.40.0 --pip 23.1.2 .venv
 source .venv/bin/activate
 pip install -r requirements.txt
 pip install -r requirements-dev.txt
 ```
 
 ### Build Package
 
-Install buil tools for creating distribution, type in terminal:
+Install build tools for creating distribution, type in terminal:
 
-```bash
+```shell
 pip install --upgrade build
 ```
 
 Now you can run:
 
-```bash
+```shell
 python -m build
 ```
 
 ### Install Package
 
 Now you can run:
 
-```bash
-pip install --force-reinstall dist/mdsanima_cli-0.1.0-py3-none-any.whl
+```shell
+pip install --force-reinstall dist/mdsanima_cli-0.2.0-py3-none-any.whl
 ```
 
 ### Testing Package
 
 Finally you can run this command:
 
-```bash
-python -m mdsanima_cli.pixelart
+```shell
+python -m mdsanima_cli.command.pixelart
 ```
 
 Also you can run this command before you build and install:
 
-```bash
-python3 src/mdsanima_cli/pixelart.py
+```shell
+python3 src/mdsanima_cli/command/pixelart.py
 ```
 
 ### Extracts Version Package
 
-This `setuptools-scm` tools allow to extract **Python** package version from
-`git` instead declaring them as the version argument.
+This `setuptools-scm` tools allow to extract **Python** package version from `git` instead declaring
+them as the version argument.
 
 Check the `pyproject.toml` file and this
 [instruction](https://pypi.org/project/setuptools-scm/) for more info.
 
-If you need to confirm which version string is being generated or debug the
-configuration, you can install `setuptools-scm` directly in your working
-environment `pip install setuptools-scm` and run:
+If you need to confirm which version string is being generated or debug the configuration, you can
+install `setuptools-scm` directly in your working environment `pip install setuptools-scm` and run:
 
-```bash
+```shell
 python -m setuptools_scm
 ```
 
 ### Creating Release
 
-This is a steps for creating release version.
+Here are the steps to create a release version:
 
-First add new code to the package and test this functionality.
+- Add new code to the package.
+- Test new functionality.
+- Commit the change.
+- Bump the package version.
+- Generate CHANGELOG.md file.
+- Commit the release.
+- Add and push new tag.
+- Update pypi.
 
-Second steps is commit this change like this, type in terminal:
+Important steps is commit the change like this, type in terminal:
 
-```bash
-git commit -m "feat: new feature generating pixelart"
+```shell
+git commit -m "feat: generating pixel art command"
 ```
 
-The next step is bumping version on `package.json` file and generate
-`CHANGELOG.md` file with new release information, type in terminal:
+Always use this format for commiting to git, becouse this allows to generate changelog from the
+commit message. Check the `package.json` file on `standard-version` section and types lists for
+fist string thats you can type in commit message.
+
+The next step is bumping version on `package.json` file and generate `CHANGELOG.md` file with new
+release information, type in terminal:
 
-```bash
+```shell
 standard-version
 ```
 
 Next is a add this changes to git, type in terminal:
 
-```bash
+```shell
 git commit -am "chore(release): 0.1.2"
 ```
 
-The version abowe is a from `standard-version` command and this is a only
-example version. The version must always be changed when a new version is
-released.
+The version abowe is a from `standard-version` command and this is a only example version.
+The version must always be changed when a new version is released.
 
-The next steps is a creating a tag and pushing the change to origin with tag,
-type in terminal:
+The next steps is a creating a tag and pushing the change to origin with tag, type in terminal:
 
-```bash
+```shell
 git tag 0.1.2
 git push origin && git push origin --tag
 ```
 
 Checking the extracts version, type in terminal:
 
-```bash
+```shell
 python -m setuptools_scm
 ```
 
 Finally create the build and update this build to
 [test.pypi.org](https://test.pypi.org/project/mdsanima-cli/) and
 [pypi.org](https://pypi.org/project/mdsanima-cli/) but first you must check and then update.
 
-```bash
+```shell
 python -m build
 twine check dist/*
 twine upload -r testpypi dist/*
 twine upload dist/*
 ```
```

### Comparing `mdsanima_cli-0.1.3/pyproject.toml` & `mdsanima_cli-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-# Copyritht © 2023 Marcin Różewski MDSANIMA
+# Copyright © 2023 Marcin Różewski MDSANIMA
 
 [build-system]
-requires = ['setuptools>=67.1.0', 'wheel>=0.38.4', 'pip>=23.0', 'setuptools_scm[toml]>=7.1.0']
+requires = ['setuptools>=67.7.2', 'wheel>=0.40.0', 'pip>=23.1.2', 'setuptools_scm[toml]>=7.1.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'mdsanima_cli'
 authors = [{name = 'Marcin Różewski', email = 'marcinrozewski@gmail.com'}]
-description = 'Command line tools for images processing, generating pixel art, adding logo to images and many more.'
+description = 'The package will provide command-line tools for image processing, generating pixel art, adding logos to images, and much more.'
 readme = 'README.md'
 license = {file = 'LICENSE'}
 requires-python = '>=3.10'
 keywords = [
+    'bash',
     'cli',
     'command-line',
     'console-app',
     'console-application',
     'exif metadata',
+    'exif',
     'image-processing',
     'images',
+    'logo',
     'mdsanima command line',
+    'mdsanima command-line',
     'mdsanima-cli',
     'mdsanima-dev',
     'mdsanima',
     'meta information',
+    'pixel art',
     'pixelart',
     'python-library',
     'python',
     'python3',
     'shell-script',
+    'shell',
+    'watermark',
+    'zsh',
 ]
 classifiers = [
-    'Development Status :: 1 - Planning',
+    'Development Status :: 2 - Pre-Alpha',
     'Environment :: Console',
     'Environment :: Plugins',
     'Intended Audience :: Developers',
     'Intended Audience :: Education',
     'Intended Audience :: End Users/Desktop',
     'Intended Audience :: Information Technology',
     'Intended Audience :: Legal Industry',
@@ -50,40 +58,53 @@
     'Operating System :: POSIX :: Linux',
     'Operating System :: Unix',
     'Programming Language :: Python :: 3.10',
     'Topic :: Desktop Environment',
     'Topic :: Documentation :: Sphinx',
     'Topic :: Education :: Testing',
     'Topic :: Multimedia',
+    'Topic :: Multimedia :: Graphics',
+    'Topic :: Multimedia :: Graphics :: Editors',
     'Topic :: Scientific/Engineering :: Image Processing',
+    'Topic :: Scientific/Engineering :: Information Analysis',
+    'Topic :: Software Development',
     'Topic :: Software Development :: Libraries :: Python Modules',
+    'Topic :: System',
     'Topic :: System :: Console Fonts',
+    'Topic :: System :: Filesystems',
+    'Topic :: System :: Logging',
+    'Topic :: System :: Operating System',
     'Topic :: System :: Shells',
     'Topic :: System :: System Shells',
+    'Topic :: System :: Systems Administration',
+    'Topic :: System :: Systems Administration :: Authentication/Directory',
     'Topic :: Terminals',
     'Topic :: Text Processing',
     'Topic :: Utilities',
+    'Typing :: Typed',
 ]
 dependencies = [
-    'Pillow==9.4.0',
     'mdsanima-dev==0.1.1',
+    'piexif==1.1.3',
+    'Pillow==9.4.0',
 ]
 dynamic = ['version']
 
 [project.urls]
 homepage = 'https://github.com/mdsanima-lab/mdsanima-cli'
 documentation = 'https://github.com/mdsanima-lab/mdsanima-cli#readme'
 repository = 'https://github.com/mdsanima-lab/mdsanima-cli.git'
 changelog = 'https://github.com/mdsanima-lab/mdsanima-cli/blob/main/CHANGELOG.md'
 
 [project.scripts]
 mdsanima = 'mdsanima_cli:main_cli'
+mds = 'mdsanima_cli:main_cli'
 
 [tool.black]
-line-length = 79
+line-length = 100
 target-version = ['py310']
 include = '\.pyi?$'
 
 [tool.isort]
 profile = 'black'
 src_paths = ['src', 'tests']
 force_single_line = true
```

### Comparing `mdsanima_cli-0.1.3/src/mdsanima_cli.egg-info/PKG-INFO` & `mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mdsanima-cli
-Version: 0.1.3
-Summary: Command line tools for images processing, generating pixel art, adding logo to images and many more.
+Version: 0.2.0
+Summary: The package will provide command-line tools for image processing, generating pixel art, adding logos to images, and much more.
 Author-email: Marcin Różewski <marcinrozewski@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -205,16 +205,16 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: homepage, https://github.com/mdsanima-lab/mdsanima-cli
 Project-URL: documentation, https://github.com/mdsanima-lab/mdsanima-cli#readme
 Project-URL: repository, https://github.com/mdsanima-lab/mdsanima-cli.git
 Project-URL: changelog, https://github.com/mdsanima-lab/mdsanima-cli/blob/main/CHANGELOG.md
-Keywords: cli,command-line,console-app,console-application,exif metadata,image-processing,images,mdsanima command line,mdsanima-cli,mdsanima-dev,mdsanima,meta information,pixelart,python-library,python,python3,shell-script
-Classifier: Development Status :: 1 - Planning
+Keywords: bash,cli,command-line,console-app,console-application,exif metadata,exif,image-processing,images,logo,mdsanima command line,mdsanima command-line,mdsanima-cli,mdsanima-dev,mdsanima,meta information,pixel art,pixelart,python-library,python,python3,shell-script,shell,watermark,zsh
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Legal Industry
@@ -229,181 +229,213 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Desktop Environment
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Graphics :: Editors
 Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System
 Classifier: Topic :: System :: Console Fonts
+Classifier: Topic :: System :: Filesystems
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: System :: Operating System
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mdsanima-cli
 
-Command line tools for images processing, generating pixel art, adding logo to
-images and many more.
+The package will provide command-line tools for image processing, generating pixel art, adding logos
+to images, and much more.
 
 ## Installation
 
 Install latest version:
 
-```bash
+```shell
 python3 -m pip install mdsanima-cli
 ```
 
 Updating to latest version:
 
-```bash
+```shell
 python3 -m pip install --upgrade mdsanima-cli
 ```
 
 ## Terminal Commands
 
 Now you can use this command in terminal:
 
-```bash
+```shell
 mdsanima
 ```
 
-The response is printing help how to use this command line tools.
+The response is printing help how to use this command-line tools.
 
-### CLI
+You can use the `mdsanima` command or the `mds` alias, which have the same functionality.
 
-Avaiable command for this package.
+### CLI
 
-```bash
-mdsanima pixelart
-```
+Avaiable command for this package:
 
-This command works in folder that have only `.png` images and convert this
-image to pixel art with creating new file with append suffix `pixelart` to
-original file name.
+- `mdsanima` main command showing help
+- `mdsanima check` print directory info
+- `mdsanima uuid` rename to uuid
+- `mdsanima number` rename to seq numbers
+- `mdsanima logo` append a logo
+- `mdsanima watermark` append a watermark
+- `mdsanima jpg` convert to jpg
+- `mdsanima png` convert to png
+- `mdsanima webp` convert to webp
+- `mdsanima pixelart` generate pixel art 32px
+- `mdsanima grid` generate grid 2x2
+- `mdsanima thumbnail` generate jpeg thumbnail 128px
+
+The `pixelart` command works in folder that have only `.png` images and convert this images to pixel
+art with creating the new file and appending the suffix `pixelart` to original file name.
+
+After executing this command, all image files in the folder you are in will be processed.
+The command does not delete any files in the folder, it only adds new ones and showing the directory
+info.
 
 ## Development Setup
 
 Instruction step how to setup development environent is here on this
-[workflow](https://mdsanima-dev.github.io/mdsanima-dev/development/workflow/)
-instruction.
+[workflow](https://mdsanima-dev.github.io/mdsanima-dev/development/workflow/) instruction.
 
-Creating isolated environment with specific pip version then activate and
-install requirements, type in terminal:
+Creating isolated environment with specific pip version then activate and install requirements, type
+in terminal:
 
-```bash
-virtualenv --pip 23.0 .venv
+```shell
+virtualenv --setuptools 67.7.2 --wheel 0.40.0 --pip 23.1.2 .venv
 source .venv/bin/activate
 pip install -r requirements.txt
 pip install -r requirements-dev.txt
 ```
 
 ### Build Package
 
-Install buil tools for creating distribution, type in terminal:
+Install build tools for creating distribution, type in terminal:
 
-```bash
+```shell
 pip install --upgrade build
 ```
 
 Now you can run:
 
-```bash
+```shell
 python -m build
 ```
 
 ### Install Package
 
 Now you can run:
 
-```bash
-pip install --force-reinstall dist/mdsanima_cli-0.1.0-py3-none-any.whl
+```shell
+pip install --force-reinstall dist/mdsanima_cli-0.2.0-py3-none-any.whl
 ```
 
 ### Testing Package
 
 Finally you can run this command:
 
-```bash
-python -m mdsanima_cli.pixelart
+```shell
+python -m mdsanima_cli.command.pixelart
 ```
 
 Also you can run this command before you build and install:
 
-```bash
-python3 src/mdsanima_cli/pixelart.py
+```shell
+python3 src/mdsanima_cli/command/pixelart.py
 ```
 
 ### Extracts Version Package
 
-This `setuptools-scm` tools allow to extract **Python** package version from
-`git` instead declaring them as the version argument.
+This `setuptools-scm` tools allow to extract **Python** package version from `git` instead declaring
+them as the version argument.
 
 Check the `pyproject.toml` file and this
 [instruction](https://pypi.org/project/setuptools-scm/) for more info.
 
-If you need to confirm which version string is being generated or debug the
-configuration, you can install `setuptools-scm` directly in your working
-environment `pip install setuptools-scm` and run:
+If you need to confirm which version string is being generated or debug the configuration, you can
+install `setuptools-scm` directly in your working environment `pip install setuptools-scm` and run:
 
-```bash
+```shell
 python -m setuptools_scm
 ```
 
 ### Creating Release
 
-This is a steps for creating release version.
+Here are the steps to create a release version:
 
-First add new code to the package and test this functionality.
+- Add new code to the package.
+- Test new functionality.
+- Commit the change.
+- Bump the package version.
+- Generate CHANGELOG.md file.
+- Commit the release.
+- Add and push new tag.
+- Update pypi.
 
-Second steps is commit this change like this, type in terminal:
+Important steps is commit the change like this, type in terminal:
 
-```bash
-git commit -m "feat: new feature generating pixelart"
+```shell
+git commit -m "feat: generating pixel art command"
 ```
 
-The next step is bumping version on `package.json` file and generate
-`CHANGELOG.md` file with new release information, type in terminal:
+Always use this format for commiting to git, becouse this allows to generate changelog from the
+commit message. Check the `package.json` file on `standard-version` section and types lists for
+fist string thats you can type in commit message.
+
+The next step is bumping version on `package.json` file and generate `CHANGELOG.md` file with new
+release information, type in terminal:
 
-```bash
+```shell
 standard-version
 ```
 
 Next is a add this changes to git, type in terminal:
 
-```bash
+```shell
 git commit -am "chore(release): 0.1.2"
 ```
 
-The version abowe is a from `standard-version` command and this is a only
-example version. The version must always be changed when a new version is
-released.
+The version abowe is a from `standard-version` command and this is a only example version.
+The version must always be changed when a new version is released.
 
-The next steps is a creating a tag and pushing the change to origin with tag,
-type in terminal:
+The next steps is a creating a tag and pushing the change to origin with tag, type in terminal:
 
-```bash
+```shell
 git tag 0.1.2
 git push origin && git push origin --tag
 ```
 
 Checking the extracts version, type in terminal:
 
-```bash
+```shell
 python -m setuptools_scm
 ```
 
 Finally create the build and update this build to
 [test.pypi.org](https://test.pypi.org/project/mdsanima-cli/) and
 [pypi.org](https://pypi.org/project/mdsanima-cli/) but first you must check and then update.
 
-```bash
+```shell
 python -m build
 twine check dist/*
 twine upload -r testpypi dist/*
 twine upload dist/*
 ```
```

