# Comparing `tmp/types-paramiko-3.0.0.8.tar.gz` & `tmp/types-paramiko-3.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-paramiko-3.0.0.8.tar", last modified: Tue Apr 25 21:13:14 2023, max compression
+gzip compressed data, was "types-paramiko-3.0.0.9.tar", last modified: Wed May  3 15:15:16 2023, max compression
```

## Comparing `types-paramiko-3.0.0.8.tar` & `types-paramiko-3.0.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-25 21:13:13.000000 types-paramiko-3.0.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 21:13:13.000000 types-paramiko-3.0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/paramiko-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 21:13:13.000000 types-paramiko-3.0.0.8/paramiko-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/_winapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/agent.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/auth_handler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ber.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/buffered_pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/channel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/common.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/compress.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/dsskey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ecdsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ed25519key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/hostkeys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_curve25519.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_ecdh_nist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_gex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_group1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_group14.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_group16.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/packet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/pkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/primes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/rsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_attr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_handle.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_si.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ssh_exception.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ssh_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/transport.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/win_openssh.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/win_pageant.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-25 21:13:13.000000 types-paramiko-3.0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/types_paramiko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-03 15:15:14.000000 types-paramiko-3.0.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 15:15:14.000000 types-paramiko-3.0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/paramiko-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 15:15:14.000000 types-paramiko-3.0.0.9/paramiko-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/_winapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/agent.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/auth_handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ber.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/buffered_pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/channel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/compress.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/dsskey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ecdsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ed25519key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/hostkeys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_curve25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_ecdh_nist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_gex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_group1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_group14.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_group16.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/kex_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/packet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/pkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/primes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/rsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_attr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_handle.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/sftp_si.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ssh_exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/ssh_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/transport.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/win_openssh.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-03 15:15:02.000000 types-paramiko-3.0.0.9/paramiko-stubs/win_pageant.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-03 15:15:14.000000 types-paramiko-3.0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:16.141493 types-paramiko-3.0.0.9/types_paramiko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 15:15:16.000000 types-paramiko-3.0.0.9/types_paramiko.egg-info/top_level.txt
```

### Comparing `types-paramiko-3.0.0.8/CHANGELOG.md` & `types-paramiko-3.0.0.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.0.0.9 (2023-05-03)
+
+paramiko: Improve various bytes-related types (#10109)
+
 ## 3.0.0.8 (2023-04-25)
 
 `paramiko`: Be more lenient for client parameter types (#10083)
 
 Use Mapping instead of dict for better covariance
 
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
```

### Comparing `types-paramiko-3.0.0.8/PKG-INFO` & `types-paramiko-3.0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-paramiko
-Version: 3.0.0.8
+Version: 3.0.0.9
 Summary: Typing stubs for paramiko
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `paramiko`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/paramiko. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `c4b6d635abb881f0a3b0e87d4b4f75933bcde317`.
+This package was generated from typeshed commit `ec1130adcc12431ba85415a6533da68c3692b2cb`.
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/__init__.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/_winapi.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/_winapi.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/agent.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/agent.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from _typeshed import ReadableBuffer
 from socket import _RetAddress, socket
 from threading import Thread
 from typing import Protocol
 
 from paramiko.channel import Channel
-from paramiko.message import Message
+from paramiko.message import Message, _LikeBytes
 from paramiko.pkey import PKey
 from paramiko.transport import Transport
 
 class _AgentProxy(Protocol):
     def connect(self) -> None: ...
     def close(self) -> None: ...
 
@@ -57,11 +58,11 @@
     def close(self) -> None: ...
 
 class AgentKey(PKey):
     agent: AgentSSH
     blob: bytes
     public_blob: None
     name: str
-    def __init__(self, agent: AgentSSH, blob: bytes) -> None: ...
+    def __init__(self, agent: AgentSSH, blob: ReadableBuffer) -> None: ...
     def asbytes(self) -> bytes: ...
     def get_name(self) -> str: ...
-    def sign_ssh_data(self, data: bytes, algorithm: str | None = None) -> Message: ...
+    def sign_ssh_data(self, data: _LikeBytes, algorithm: str | None = None) -> Message: ...
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/auth_handler.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/auth_handler.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/ber.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/ber.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/channel.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/channel.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from collections.abc import Callable, Mapping
+from _typeshed import SupportsItems
+from collections.abc import Callable
 from logging import Logger
 from threading import Condition, Event, Lock
 from typing import Any, TypeVar
 from typing_extensions import Literal
 
 from paramiko.buffered_pipe import BufferedPipe
 from paramiko.file import BufferedFile
+from paramiko.message import _LikeBytes
 from paramiko.transport import Transport
 from paramiko.util import ClosingContextManager
 
 _F = TypeVar("_F", bound=Callable[..., Any])
 
 def open_only(func: _F) -> Callable[[_F], _F]: ...
 
@@ -39,30 +41,30 @@
     event_ready: bool
     combine_stderr: bool
     exit_status: int
     origin_addr: None
     def __init__(self, chanid: int) -> None: ...
     def __del__(self) -> None: ...
     def get_pty(
-        self, term: str | bytes = "vt100", width: int = 80, height: int = 24, width_pixels: int = 0, height_pixels: int = 0
+        self, term: _LikeBytes = "vt100", width: int = 80, height: int = 24, width_pixels: int = 0, height_pixels: int = 0
     ) -> None: ...
     def invoke_shell(self) -> None: ...
-    def exec_command(self, command: str | bytes) -> None: ...
-    def invoke_subsystem(self, subsystem: str | bytes) -> None: ...
+    def exec_command(self, command: _LikeBytes) -> None: ...
+    def invoke_subsystem(self, subsystem: _LikeBytes) -> None: ...
     def resize_pty(self, width: int = 80, height: int = 24, width_pixels: int = 0, height_pixels: int = 0) -> None: ...
-    def update_environment(self, environment: Mapping[str | bytes, str | bytes]) -> None: ...
-    def set_environment_variable(self, name: str | bytes, value: str | bytes) -> None: ...
+    def update_environment(self, environment: SupportsItems[_LikeBytes, _LikeBytes]) -> None: ...
+    def set_environment_variable(self, name: _LikeBytes, value: _LikeBytes) -> None: ...
     def exit_status_ready(self) -> bool: ...
     def recv_exit_status(self) -> int: ...
     def send_exit_status(self, status: int) -> None: ...
     def request_x11(
         self,
         screen_number: int = 0,
-        auth_protocol: str | bytes | None = None,
-        auth_cookie: str | bytes | None = None,
+        auth_protocol: _LikeBytes | None = None,
+        auth_cookie: _LikeBytes | None = None,
         single_connection: bool = False,
         handler: Callable[[Channel, tuple[str, int]], object] | None = None,
     ) -> bytes: ...
     def request_forward_agent(self, handler: Callable[[Channel], object]) -> bool: ...
     def get_transport(self) -> Transport: ...
     def set_name(self, name: str) -> None: ...
     def get_name(self) -> str: ...
@@ -74,18 +76,18 @@
     def getpeername(self) -> str: ...
     def close(self) -> None: ...
     def recv_ready(self) -> bool: ...
     def recv(self, nbytes: int) -> bytes: ...
     def recv_stderr_ready(self) -> bool: ...
     def recv_stderr(self, nbytes: int) -> bytes: ...
     def send_ready(self) -> bool: ...
-    def send(self, s: bytes) -> int: ...
-    def send_stderr(self, s: bytes) -> int: ...
-    def sendall(self, s: bytes) -> None: ...
-    def sendall_stderr(self, s: bytes) -> None: ...
+    def send(self, s: bytes | bytearray) -> int: ...
+    def send_stderr(self, s: bytes | bytearray) -> int: ...
+    def sendall(self, s: bytes | bytearray) -> None: ...
+    def sendall_stderr(self, s: bytes | bytearray) -> None: ...
     def makefile(self, *params: Any) -> ChannelFile: ...
     def makefile_stderr(self, *params: Any) -> ChannelStderrFile: ...
     def makefile_stdin(self, *params: Any) -> ChannelStdinFile: ...
     def fileno(self) -> int: ...
     def shutdown(self, how: int) -> None: ...
     def shutdown_read(self) -> None: ...
     def shutdown_write(self) -> None: ...
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/client.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/common.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/common.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/config.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/dsskey.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/dsskey.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from _typeshed import ReadableBuffer
 from collections.abc import Callable
 from typing import IO
 
 from paramiko.message import Message
 from paramiko.pkey import PKey
 
 class DSSKey(PKey):
@@ -11,15 +12,15 @@
     y: int | None
     x: int | None
     public_blob: None
     size: int
     def __init__(
         self,
         msg: Message | None = None,
-        data: bytes | None = None,
+        data: ReadableBuffer | None = None,
         filename: str | None = None,
         password: str | None = None,
         vals: tuple[int, int, int, int] | None = None,
         file_obj: IO[str] | None = None,
     ) -> None: ...
     def asbytes(self) -> bytes: ...
     def __hash__(self) -> int: ...
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/ecdsakey.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/ecdsakey.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from _typeshed import ReadableBuffer
 from collections.abc import Callable, Sequence
 from typing import IO, Any
 
 from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurve, EllipticCurvePrivateKey, EllipticCurvePublicKey
 from cryptography.hazmat.primitives.hashes import HashAlgorithm
 from paramiko.message import Message
 from paramiko.pkey import PKey
@@ -26,15 +27,15 @@
     verifying_key: EllipticCurvePublicKey
     signing_key: EllipticCurvePrivateKey
     public_blob: None
     ecdsa_curve: _ECDSACurve | None
     def __init__(
         self,
         msg: Message | None = None,
-        data: bytes | None = None,
+        data: ReadableBuffer | None = None,
         filename: str | None = None,
         password: str | None = None,
         vals: tuple[EllipticCurvePrivateKey, EllipticCurvePublicKey] | None = None,
         file_obj: IO[str] | None = None,
         validate_point: bool = True,
     ) -> None: ...
     @classmethod
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/ed25519key.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/ed25519key.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from _typeshed import ReadableBuffer
 from typing import IO
 
 from paramiko.message import Message
 from paramiko.pkey import PKey
 
 class Ed25519Key(PKey):
     public_blob: None
     def __init__(
         self,
         msg: Message | None = None,
-        data: bytes | None = None,
+        data: ReadableBuffer | None = None,
         filename: str | None = None,
         password: str | None = None,
         file_obj: IO[str] | None = None,
     ) -> None: ...
     def asbytes(self) -> bytes: ...
     def __hash__(self) -> int: ...
     def get_name(self) -> str: ...
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/file.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/file.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/hostkeys.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/hostkeys.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/kex_curve25519.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/kex_curve25519.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/kex_ecdh_nist.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/kex_ecdh_nist.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/kex_gex.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/kex_gex.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/kex_group1.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/kex_group1.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/kex_gss.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/kex_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/packet.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/packet.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, ReadableBuffer
 from collections.abc import Callable
 from hashlib import _Hash
 from logging import Logger
 from socket import socket
 from typing import Any
 
 from cryptography.hazmat.primitives.ciphers import Cipher
 from paramiko.compress import ZlibCompressor, ZlibDecompressor
 from paramiko.message import Message
 
-def compute_hmac(key: bytes, message: bytes, digest_class: _Hash) -> bytes: ...
+def compute_hmac(key: bytes | bytearray, message: ReadableBuffer, digest_class: _Hash) -> bytes: ...
 
 class NeedRekeyException(Exception): ...
 
 def first_arg(e: Exception) -> Any: ...
 
 class Packetizer:
     REKEY_PACKETS: int
@@ -26,25 +26,25 @@
     def set_log(self, log: Logger) -> None: ...
     def set_outbound_cipher(
         self,
         block_engine: Cipher[Incomplete],
         block_size: int,
         mac_engine: _Hash,
         mac_size: int,
-        mac_key: bytes,
+        mac_key: bytes | bytearray,
         sdctr: bool = False,
         etm: bool = False,
     ) -> None: ...
     def set_inbound_cipher(
         self,
         block_engine: Cipher[Incomplete],
         block_size: int,
         mac_engine: _Hash,
         mac_size: int,
-        mac_key: bytes,
+        mac_key: bytes | bytearray,
         etm: bool = False,
     ) -> None: ...
     def set_outbound_compressor(self, compressor: ZlibCompressor) -> None: ...
     def set_inbound_compressor(self, compressor: ZlibDecompressor) -> None: ...
     def close(self) -> None: ...
     def set_hexdump(self, hexdump: bool) -> None: ...
     def get_hexdump(self) -> bool: ...
@@ -53,11 +53,11 @@
     def need_rekey(self) -> bool: ...
     def set_keepalive(self, interval: int, callback: Callable[[], object]) -> None: ...
     def read_timer(self) -> None: ...
     def start_handshake(self, timeout: float) -> None: ...
     def handshake_timed_out(self) -> bool: ...
     def complete_handshake(self) -> None: ...
     def read_all(self, n: int, check_rekey: bool = False) -> bytes: ...
-    def write_all(self, out: bytes) -> None: ...
+    def write_all(self, out: ReadableBuffer) -> None: ...
     def readline(self, timeout: float) -> str: ...
     def send_message(self, data: Message) -> None: ...
     def read_message(self) -> tuple[int, Message]: ...
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/pipe.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/pipe.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/pkey.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/pkey.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from re import Pattern
-from typing import IO
+from typing import IO, TypeVar
 from typing_extensions import Self
 
 from paramiko.message import Message
 
 OPENSSH_AUTH_MAGIC: bytes
 
-def _unpad_openssh(data: bytes) -> bytes: ...
+_BytesT = TypeVar("_BytesT", bound=bytes | bytearray)
+
+def _unpad_openssh(data: _BytesT) -> _BytesT: ...
 
 class PKey:
     public_blob: PublicBlob | None
     BEGIN_TAG: Pattern[str]
     END_TAG: Pattern[str]
     def __init__(self, msg: Message | None = None, data: str | None = None) -> None: ...
     def asbytes(self) -> bytes: ...
@@ -29,15 +31,15 @@
     def from_private_key(cls, file_obj: IO[str], password: str | None = None) -> Self: ...
     def write_private_key_file(self, filename: str, password: str | None = None) -> None: ...
     def write_private_key(self, file_obj: IO[str], password: str | None = None) -> None: ...
     def load_certificate(self, value: Message | str) -> None: ...
 
 class PublicBlob:
     key_type: str
-    key_blob: str
+    key_blob: bytes
     comment: str
     def __init__(self, type_: str, blob: bytes, comment: str | None = None) -> None: ...
     @classmethod
     def from_file(cls, filename: str) -> Self: ...
     @classmethod
     def from_string(cls, string: str) -> Self: ...
     @classmethod
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/rsakey.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/rsakey.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from _typeshed import ReadableBuffer
 from collections.abc import Callable
 from typing import IO
 
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey, RSAPublicKey, RSAPublicNumbers
 from paramiko.message import Message
 from paramiko.pkey import PKey
 
 class RSAKey(PKey):
     key: None | RSAPublicKey | RSAPrivateKey
     public_blob: None
     def __init__(
         self,
         msg: Message | None = None,
-        data: bytes | None = None,
+        data: ReadableBuffer | None = None,
         filename: str | None = None,
         password: str | None = None,
         key: None | RSAPublicKey | RSAPrivateKey = None,
         file_obj: IO[str] | None = None,
     ) -> None: ...
     @property
     def size(self) -> int: ...
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/server.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/sftp.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/sftp.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/sftp_attr.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/sftp_attr.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/sftp_client.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/sftp_client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from _typeshed import StrOrBytesPath
 from collections.abc import Callable, Iterator
 from logging import Logger
 from typing import IO
 from typing_extensions import Self, TypeAlias
 
 from paramiko.channel import Channel
 from paramiko.sftp import BaseSFTP
@@ -46,15 +47,15 @@
     def normalize(self, path: bytes | str) -> str: ...
     def chdir(self, path: None | bytes | str = None) -> None: ...
     def getcwd(self) -> str | None: ...
     def putfo(
         self, fl: IO[bytes], remotepath: bytes | str, file_size: int = 0, callback: _Callback | None = None, confirm: bool = True
     ) -> SFTPAttributes: ...
     def put(
-        self, localpath: bytes | str, remotepath: bytes | str, callback: _Callback | None = None, confirm: bool = True
+        self, localpath: StrOrBytesPath, remotepath: bytes | str, callback: _Callback | None = None, confirm: bool = True
     ) -> SFTPAttributes: ...
     def getfo(self, remotepath: bytes | str, fl: IO[bytes], callback: _Callback | None = None, prefetch: bool = True) -> int: ...
     def get(
-        self, remotepath: bytes | str, localpath: bytes | str, callback: _Callback | None = None, prefetch: bool = True
+        self, remotepath: bytes | str, localpath: StrOrBytesPath, callback: _Callback | None = None, prefetch: bool = True
     ) -> None: ...
 
 class SFTP(SFTPClient): ...
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/sftp_file.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/sftp_file.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from collections.abc import Iterator, Sequence
 from typing import Any
 
 from paramiko.file import BufferedFile
+from paramiko.message import _LikeBytes
 from paramiko.sftp_attr import SFTPAttributes
 from paramiko.sftp_client import SFTPClient
 from paramiko.sftp_handle import SFTPHandle
 
 class SFTPFile(BufferedFile[Any]):
     MAX_REQUEST_SIZE: int
     sftp: SFTPClient
     handle: SFTPHandle
     pipelined: bool
-    def __init__(self, sftp: SFTPClient, handle: bytes, mode: str = "r", bufsize: int = -1) -> None: ...
+    def __init__(self, sftp: SFTPClient, handle: _LikeBytes, mode: str = "r", bufsize: int = -1) -> None: ...
     def __del__(self) -> None: ...
     def close(self) -> None: ...
     def settimeout(self, timeout: float) -> None: ...
     def gettimeout(self) -> float: ...
     def setblocking(self, blocking: bool) -> None: ...
     def seekable(self) -> bool: ...
     def seek(self, offset: int, whence: int = 0) -> None: ...
```

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/sftp_server.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/sftp_server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/sftp_si.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/sftp_si.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/ssh_exception.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/ssh_exception.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/ssh_gss.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/ssh_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/transport.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/transport.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.8/paramiko-stubs/util.pyi` & `types-paramiko-3.0.0.9/paramiko-stubs/util.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+from _typeshed import ReadableBuffer
+from collections.abc import Iterable
 from hashlib import _Hash
 from logging import Logger, LogRecord
 from types import TracebackType
 from typing import IO, AnyStr, Protocol
 from typing_extensions import Self
 
 from paramiko.config import SSHConfig, SSHConfigDict
 from paramiko.hostkeys import HostKeys
 
 class SupportsClose(Protocol):
     def close(self) -> None: ...
 
-def inflate_long(s: bytes, always_positive: bool = False) -> int: ...
+def inflate_long(s: bytes | bytearray, always_positive: bool = False) -> int: ...
 def deflate_long(n: int, add_sign_padding: bool = True) -> bytes: ...
-def format_binary(data: bytes, prefix: str = "") -> list[str]: ...
-def format_binary_line(data: bytes) -> str: ...
-def safe_string(s: bytes) -> bytes: ...
+def format_binary(data: bytes | bytearray, prefix: str = "") -> list[str]: ...
+def format_binary_line(data: bytes | bytearray) -> str: ...
+def safe_string(s: Iterable[int | str]) -> bytes: ...
 def bit_length(n: int) -> int: ...
 def tb_strings() -> list[str]: ...
-def generate_key_bytes(hash_alg: type[_Hash], salt: bytes, key: bytes | str, nbytes: int) -> bytes: ...
+def generate_key_bytes(hash_alg: type[_Hash], salt: ReadableBuffer, key: bytes | str, nbytes: int) -> bytes: ...
 def load_host_keys(filename: str) -> HostKeys: ...
 def parse_ssh_config(file_obj: IO[str]) -> SSHConfig: ...
 def lookup_ssh_host_config(hostname: str, config: SSHConfig) -> SSHConfigDict: ...
 def mod_inverse(x: int, m: int) -> int: ...
 def get_thread_id() -> int: ...
 def log_to_file(filename: str, level: int = 10) -> None: ...
```

### Comparing `types-paramiko-3.0.0.8/setup.py` & `types-paramiko-3.0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `paramiko`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/paramiko. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `c4b6d635abb881f0a3b0e87d4b4f75933bcde317`.
+This package was generated from typeshed commit `ec1130adcc12431ba85415a6533da68c3692b2cb`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.8",
+      version="3.0.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md",
```

### Comparing `types-paramiko-3.0.0.8/types_paramiko.egg-info/PKG-INFO` & `types-paramiko-3.0.0.9/types_paramiko.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-paramiko
-Version: 3.0.0.8
+Version: 3.0.0.9
 Summary: Typing stubs for paramiko
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `paramiko`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/paramiko. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `c4b6d635abb881f0a3b0e87d4b4f75933bcde317`.
+This package was generated from typeshed commit `ec1130adcc12431ba85415a6533da68c3692b2cb`.
```

### Comparing `types-paramiko-3.0.0.8/types_paramiko.egg-info/SOURCES.txt` & `types-paramiko-3.0.0.9/types_paramiko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

