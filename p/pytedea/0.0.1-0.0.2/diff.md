# Comparing `tmp/pytedea-0.0.1.tar.gz` & `tmp/pytedea-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedea-0.0.1.tar", last modified: Wed Apr 26 15:54:24 2023, max compression
+gzip compressed data, was "pytedea-0.0.2.tar", last modified: Wed May  3 15:40:42 2023, max compression
```

## Comparing `pytedea-0.0.1.tar` & `pytedea-0.0.2.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 15:54:24.010974 pytedea-0.0.1/
--rw-rw-rw-   0        0        0     1584 2023-04-26 15:50:35.000000 pytedea-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-26 15:50:35.000000 pytedea-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1184 2023-04-26 15:54:24.010974 pytedea-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-04-26 15:50:35.000000 pytedea-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 15:54:23.780974 pytedea-0.0.1/pytedea/
--rw-rw-rw-   0        0        0     5923 2023-04-26 15:31:43.000000 pytedea-0.0.1/pytedea/DDFt.py
--rw-rw-rw-   0        0        0   139457 2023-04-26 15:27:54.000000 pytedea-0.0.1/pytedea/DEAt.py
--rw-rw-rw-   0        0        0      561 2023-04-26 14:46:11.000000 pytedea-0.0.1/pytedea/__init__.py
--rw-rw-rw-   0        0        0      194 2023-04-26 15:50:35.000000 pytedea-0.0.1/pytedea/common.py
--rw-rw-rw-   0        0        0     1860 2023-04-26 14:46:00.000000 pytedea-0.0.1/pytedea/constant.py
--rw-rw-rw-   0        0        0       20 2023-04-26 15:50:35.000000 pytedea-0.0.1/pytedea/pytedea.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:54:23.996976 pytedea-0.0.1/pytedea/utils/
--rw-rw-rw-   0        0        0     6197 2023-03-08 07:19:14.000000 pytedea-0.0.1/pytedea/utils/CNLSDDFG1.py
--rw-rw-rw-   0        0        0     4769 2023-03-08 07:32:30.000000 pytedea-0.0.1/pytedea/utils/CNLSDDFG2.py
--rw-rw-rw-   0        0        0    13705 2023-03-08 09:38:03.000000 pytedea-0.0.1/pytedea/utils/CNLSDDFZG1.py
--rw-rw-rw-   0        0        0     7183 2023-03-08 07:20:02.000000 pytedea-0.0.1/pytedea/utils/CNLSDDFZG2.py
--rw-rw-rw-   0        0        0     4611 2023-03-08 06:58:51.000000 pytedea-0.0.1/pytedea/utils/CNLSG1.py
--rw-rw-rw-   0        0        0     5046 2023-03-08 09:51:18.000000 pytedea-0.0.1/pytedea/utils/CNLSG2.py
--rw-rw-rw-   0        0        0    12120 2023-03-08 09:14:35.000000 pytedea-0.0.1/pytedea/utils/CNLSZG1.py
--rw-rw-rw-   0        0        0     7064 2023-03-08 06:58:51.000000 pytedea-0.0.1/pytedea/utils/CNLSZG2.py
--rw-rw-rw-   0        0        0     8210 2023-03-08 12:43:32.000000 pytedea-0.0.1/pytedea/utils/CQERDDFG1.py
--rw-rw-rw-   0        0        0     6712 2023-03-08 11:19:30.000000 pytedea-0.0.1/pytedea/utils/CQERDDFG2.py
--rw-rw-rw-   0        0        0    16501 2023-03-08 12:43:32.000000 pytedea-0.0.1/pytedea/utils/CQERDDFZG1.py
--rw-rw-rw-   0        0        0     9161 2023-03-08 11:15:30.000000 pytedea-0.0.1/pytedea/utils/CQERDDFZG2.py
--rw-rw-rw-   0        0        0     6337 2023-03-08 10:23:37.000000 pytedea-0.0.1/pytedea/utils/CQERG1.py
--rw-rw-rw-   0        0        0     5735 2023-03-08 10:27:50.000000 pytedea-0.0.1/pytedea/utils/CQERG2.py
--rw-rw-rw-   0        0        0    14049 2023-03-08 10:23:37.000000 pytedea-0.0.1/pytedea/utils/CQERZG1.py
--rw-rw-rw-   0        0        0     8877 2023-03-08 10:27:50.000000 pytedea-0.0.1/pytedea/utils/CQERZG2.py
--rw-rw-rw-   0        0        0      251 2023-03-05 09:16:09.000000 pytedea-0.0.1/pytedea/utils/__init__.py
--rw-rw-rw-   0        0        0     1159 2023-03-05 09:16:09.000000 pytedea-0.0.1/pytedea/utils/interpolation.py
--rw-rw-rw-   0        0        0     1993 2023-03-16 05:46:55.000000 pytedea-0.0.1/pytedea/utils/sweet.py
--rw-rw-rw-   0        0        0    24603 2023-04-26 15:29:51.000000 pytedea-0.0.1/pytedea/utils/tools.py
--rw-rw-rw-   0        0        0     5650 2023-03-08 08:11:55.000000 pytedea-0.0.1/pytedea/utils/weakCNLSDDFG1.py
--rw-rw-rw-   0        0        0     5646 2023-03-08 15:02:30.000000 pytedea-0.0.1/pytedea/utils/weakCNLSDDFG2.py
--rw-rw-rw-   0        0        0    18293 2023-03-16 10:24:50.000000 pytedea-0.0.1/pytedea/utils/weakCNLSDDFZG1.py
--rw-rw-rw-   0        0        0    15471 2023-03-16 10:24:50.000000 pytedea-0.0.1/pytedea/utils/weakCNLSDDFZG2.py
--rw-rw-rw-   0        0        0     6678 2023-03-14 14:30:31.000000 pytedea-0.0.1/pytedea/utils/weakCNLSG1.py
--rw-rw-rw-   0        0        0     5271 2023-03-08 15:38:44.000000 pytedea-0.0.1/pytedea/utils/weakCNLSG2.py
--rw-rw-rw-   0        0        0    15035 2023-03-14 14:43:12.000000 pytedea-0.0.1/pytedea/utils/weakCNLSZG1.py
--rw-rw-rw-   0        0        0     9053 2023-03-14 15:03:28.000000 pytedea-0.0.1/pytedea/utils/weakCNLSZG2.py
--rw-rw-rw-   0        0        0     5478 2023-03-08 08:33:26.000000 pytedea-0.0.1/pytedea/utils/weakCNLSbG1.py
--rw-rw-rw-   0        0        0     5278 2023-03-08 14:59:46.000000 pytedea-0.0.1/pytedea/utils/weakCNLSbG2.py
--rw-rw-rw-   0        0        0    15094 2023-03-14 15:09:08.000000 pytedea-0.0.1/pytedea/utils/weakCNLSbZG1.py
--rw-rw-rw-   0        0        0     9187 2023-03-14 15:27:58.000000 pytedea-0.0.1/pytedea/utils/weakCNLSbZG2.py
--rw-rw-rw-   0        0        0     5507 2023-03-08 08:53:20.000000 pytedea-0.0.1/pytedea/utils/weakCNLSxG1.py
--rw-rw-rw-   0        0        0     6472 2023-03-08 14:59:46.000000 pytedea-0.0.1/pytedea/utils/weakCNLSxG2.py
--rw-rw-rw-   0        0        0    15197 2023-03-14 15:21:54.000000 pytedea-0.0.1/pytedea/utils/weakCNLSxZG1.py
--rw-rw-rw-   0        0        0     9118 2023-03-14 15:27:58.000000 pytedea-0.0.1/pytedea/utils/weakCNLSxZG2.py
--rw-rw-rw-   0        0        0     7407 2023-03-08 14:31:36.000000 pytedea-0.0.1/pytedea/utils/weakCQERDDFG1.py
--rw-rw-rw-   0        0        0     7370 2023-03-08 15:04:18.000000 pytedea-0.0.1/pytedea/utils/weakCQERDDFG2.py
--rw-rw-rw-   0        0        0    15583 2023-03-08 14:31:35.000000 pytedea-0.0.1/pytedea/utils/weakCQERDDFZG1.py
--rw-rw-rw-   0        0        0    10751 2023-03-08 14:07:00.000000 pytedea-0.0.1/pytedea/utils/weakCQERDDFZG2.py
--rw-rw-rw-   0        0        0     7168 2023-03-08 17:02:19.000000 pytedea-0.0.1/pytedea/utils/weakCQERG1.py
--rw-rw-rw-   0        0        0     6995 2023-03-08 16:09:40.000000 pytedea-0.0.1/pytedea/utils/weakCQERG2.py
--rw-rw-rw-   0        0        0    14548 2023-03-08 17:07:18.000000 pytedea-0.0.1/pytedea/utils/weakCQERZG1.py
--rw-rw-rw-   0        0        0     9918 2023-03-08 16:09:40.000000 pytedea-0.0.1/pytedea/utils/weakCQERZG2.py
--rw-rw-rw-   0        0        0     7245 2023-03-08 13:25:16.000000 pytedea-0.0.1/pytedea/utils/weakCQERbG1.py
--rw-rw-rw-   0        0        0     7001 2023-03-08 14:39:11.000000 pytedea-0.0.1/pytedea/utils/weakCQERbG2.py
--rw-rw-rw-   0        0        0    14602 2023-03-07 16:36:48.000000 pytedea-0.0.1/pytedea/utils/weakCQERbZG1.py
--rw-rw-rw-   0        0        0     9929 2023-03-08 14:31:36.000000 pytedea-0.0.1/pytedea/utils/weakCQERbZG2.py
--rw-rw-rw-   0        0        0     7342 2023-03-08 13:46:35.000000 pytedea-0.0.1/pytedea/utils/weakCQERxG1.py
--rw-rw-rw-   0        0        0     6999 2023-03-08 14:31:36.000000 pytedea-0.0.1/pytedea/utils/weakCQERxG2.py
--rw-rw-rw-   0        0        0    14538 2023-03-08 05:30:13.000000 pytedea-0.0.1/pytedea/utils/weakCQERxZG1.py
--rw-rw-rw-   0        0        0     9852 2023-03-08 14:31:35.000000 pytedea-0.0.1/pytedea/utils/weakCQERxZG2.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:54:23.802977 pytedea-0.0.1/pytedea.egg-info/
--rw-rw-rw-   0        0        0     1184 2023-04-26 15:54:23.000000 pytedea-0.0.1/pytedea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1889 2023-04-26 15:54:23.000000 pytedea-0.0.1/pytedea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       87 2023-04-26 15:54:23.000000 pytedea-0.0.1/pytedea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 15:54:23.000000 pytedea-0.0.1/pytedea.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       86 2023-04-26 15:54:23.000000 pytedea-0.0.1/pytedea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 15:54:23.000000 pytedea-0.0.1/pytedea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-26 15:36:09.000000 pytedea-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      415 2023-04-26 15:54:24.012975 pytedea-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1788 2023-04-26 15:50:35.000000 pytedea-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:54:24.007976 pytedea-0.0.1/tests/
--rw-rw-rw-   0        0        0      615 2023-04-26 15:29:30.000000 pytedea-0.0.1/tests/test_DDFt.py
--rw-rw-rw-   0        0        0      797 2023-04-26 15:08:59.000000 pytedea-0.0.1/tests/test_DEAt.py
--rw-rw-rw-   0        0        0      408 2023-04-26 15:50:35.000000 pytedea-0.0.1/tests/test_pytedea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:40:42.985329 pytedea-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-03 15:40:24.000000 pytedea-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-03 15:40:24.000000 pytedea-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-03 15:40:42.985329 pytedea-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-03 15:40:24.000000 pytedea-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:40:42.977330 pytedea-0.0.2/pytedea/
+-rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/DDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/DDFt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23332 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/DEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139489 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/DEAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/HYPER.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/NDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/pytedea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:40:42.985329 pytedea-0.0.2/pytedea/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/sweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28389 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSbG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSbG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSbZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSbZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSxG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSxG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSxZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSxZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERbG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERbG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERbZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERbZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERxG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERxG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERxZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERxZG2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:40:42.981330 pytedea-0.0.2/pytedea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 15:40:24.000000 pytedea-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-03 15:40:42.985329 pytedea-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-03 15:40:24.000000 pytedea-0.0.2/setup.py
```

### Comparing `pytedea-0.0.1/LICENSE` & `pytedea-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-GNU GENERAL PUBLIC LICENSE
-                      Version 3, 29 June 2007
-
-    Data envelopment analysis using Python.
-    Copyright (C) 2023  advancehs
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
-
+GNU GENERAL PUBLIC LICENSE
+                      Version 3, 29 June 2007
+
+    Data envelopment analysis using Python.
+    Copyright (C) 2023  advancehs
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+
```

### Comparing `pytedea-0.0.1/PKG-INFO` & `pytedea-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: pytedea
-Version: 0.0.1
-Summary: Data envelopment analysis using Python.
-Home-page: https://github.com/advancehs/pytedea
-Author: advancehs
-Author-email: 1019753743@qq.com
-License: GNU General Public License v3
-Keywords: pytedea
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pytedea
-
-
-[![image](https://img.shields.io/pypi/v/pytedea.svg)](https://pypi.python.org/pypi/pytedea)
-[![image](https://img.shields.io/conda/vn/conda-forge/pytedea.svg)](https://anaconda.org/conda-forge/pytedea)
-
-
-**Data envelopment analysis using Python.**
-
-
--   Free software: GNU General Public License v3
--   Documentation: https://advancehs.github.io/pytedea
-    
-
-## Features
-
--   TODO
+Metadata-Version: 2.1
+Name: pytedea
+Version: 0.0.2
+Summary: Data envelopment analysis using Python.
+Home-page: https://github.com/advancehs/pytedea
+Author: advancehs
+Author-email: 1019753743@qq.com
+License: GNU General Public License v3
+Keywords: pytedea
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pytedea
+
+
+[![image](https://img.shields.io/pypi/v/pytedea.svg)](https://pypi.python.org/pypi/pytedea)
+[![image](https://img.shields.io/conda/vn/conda-forge/pytedea.svg)](https://anaconda.org/conda-forge/pytedea)
+
+
+**Data envelopment analysis using Python.**
+
+
+-   Free software: GNU General Public License v3
+-   Documentation: https://advancehs.github.io/pytedea
+    
+
+## Features
+
+-   TODO
```

### Comparing `pytedea-0.0.1/pytedea/DDFt.py` & `pytedea-0.0.2/pytedea/DDFt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Main module."""
 # import dependencies
 
 from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, maximize, Constraint, Reals,PositiveReals
 import numpy as np
 import pandas as pd
-from .constant import CET_ADDI, ORIENT_IO, ORIENT_OO,ORIENT_HYPER, RTS_VRS, RTS_CRS, OPT_DEFAULT, OPT_LOCAL
+from .constant import CET_ADDI, ORIENT_IO, ORIENT_OO,ORIENT_HYPERYB, RTS_VRS, RTS_CRS, OPT_DEFAULT, OPT_LOCAL
 from .utils import tools
 from .DEAt import DEAt
 import ast
 
 class DDFt(DEAt):
     def __init__(self, data,sent = "inputvar=outputvar",  gy=[1], gx=[1],rts=RTS_VRS, baseindex=None,refindex=None):
         """DEA: Directional distance function
@@ -19,16 +19,16 @@
             gy (list, optional): output directional vector. Defaults to [1].
             gx (list, optional): input directional vector. Defaults to [1].
             rts (String): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale)
             baseindex (String, optional): estimate index. Defaults to None. e.g.: "Year=[2010]"
             refindex (String, optional): reference index. Defaults to None. e.g.: "Year=[2010]"
         """
         # Initialize DEA model
-        self.outputvars, self.inputvars,  self.gy, self.gx = tools.assert_valid_ddf(sent,gy,gx)
-        self.y,self.x,self.yref,self.xref = tools.assert_valid_ddf2(data, baseindex, refindex, self.outputvars, self.inputvars)
+        self.outputvars, self.inputvars,  self.gy, self.gx = tools.assert_valid_ddft(sent,gy,gx)
+        self.y,self.x,self.yref,self.xref = tools.assert_valid_ddft2(data, baseindex, refindex, self.outputvars, self.inputvars)
 
         self.xcol = self.x.columns
         self.ycol = self.y.columns
         self.rts = rts
 
         # if orient in [ORIENT_IO, ORIENT_OO, ORIENT_HYPER]:
         #     self.orient = orient
```

### Comparing `pytedea-0.0.1/pytedea/DEAt.py` & `pytedea-0.0.2/pytedea/DEAt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Main module."""
 # import dependencies
 
 from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, maximize, Constraint, Reals,PositiveReals
 import numpy as np
 import pandas as pd
-from .constant import CET_ADDI, ORIENT_IO, ORIENT_OO,ORIENT_HYPER, RTS_VRS, RTS_CRS, OPT_DEFAULT, OPT_LOCAL
+from .constant import CET_ADDI, ORIENT_IO, ORIENT_OO,ORIENT_HYPERYX,ORIENT_HYPERYB, RTS_VRS, RTS_CRS, OPT_DEFAULT, OPT_LOCAL
 from .utils import tools
 import ast
 
 class DEAt:
     """traditional Data Envelopment Analysis (DEA)
     """
     def __init__(self, data,sent = "inputvar=outputvar",  orient=ORIENT_IO, rts=RTS_VRS, baseindex=None,refindex=None):
@@ -21,19 +21,19 @@
             rts (String): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale)
             baseindex (String, optional): estimate index. Defaults to None. e.g.: "Year=[2010]"
             refindex (String, optional): reference index. Defaults to None. e.g.: "Year=[2010]"
         """
         # Initialize DEA model
 
         self.rts = rts
-        self.outputvars, self.inputvars ,self.y, self.x,self.yref, self.xref= tools.assert_valid_dea(sent,data,baseindex,refindex )
+        self.outputvars, self.inputvars ,self.y, self.x,self.yref, self.xref= tools.assert_valid_deat(sent,data,baseindex,refindex )
 
         self.xcol = self.x.columns
         self.ycol = self.y.columns
-        if orient in [ORIENT_IO, ORIENT_OO, ORIENT_HYPER]:
+        if orient in [ORIENT_IO, ORIENT_OO, ORIENT_HYPERYX]:
             self.orient = orient
         else:
             self.orient = None
             if orient in self.xcol:
                 self.xindexs = list(self.xcol).index(orient)
                 self.yindexs = None
             elif orient in self.ycol:
@@ -52,27 +52,27 @@
             self.__model__.I2 = Set(initialize=  self.xref.index)       ## I2 是 参考决策单元的数量
 
             self.__model__.K = Set(initialize=range(len(self.x.iloc[0])))          ## K 是投入个数
             self.__model__.L = Set(initialize=range(len(self.y.iloc[0])))           ## L 是产出个数 被评价单元和参考单元的K，L一样
 
             # Initialize variable
             self.__model__.theta = Var(Set(initialize=range(1)),bounds=(None, None), doc='efficiency')
-            if self.orient == ORIENT_HYPER:
+            if self.orient == ORIENT_HYPERYX:
                 self.__model__.delta = Var(Set(initialize=range(1)),bounds=(None, None), doc='efficiency**2')
 
             self.__model__.lamda = Var(self.__model__.I2, bounds=(0.0, None), doc='intensity variables')
 
             # Setup the objective function and constraints
             if self.orient == ORIENT_IO:
                 self.__model__.objective = Objective(
                     rule=self.__objective_rule(), sense=minimize, doc='objective function')
             elif self.orient == ORIENT_OO:
                 self.__model__.objective = Objective(
                     rule=self.__objective_rule(), sense=maximize, doc='objective function')
-            elif self.orient == ORIENT_HYPER:
+            elif self.orient == ORIENT_HYPERYX:
                 self.__model__.objective = Objective(
                     rule=self.__objective_rule(), sense=minimize, doc='objective function')
             elif type(self.orient) == type(None):
                 if type(self.yindexs)==type(None):
                     self.__model__.objective = Objective(
                         rule=self.__objective_rule(), sense=minimize, doc='objective function')
                 else:
@@ -98,15 +98,15 @@
 
 
         # # Optimize model
 
 
     def __objective_rule(self):
         """Return the proper objective function"""
-        if self.orient != ORIENT_HYPER:
+        if self.orient != ORIENT_HYPERYX:
             def objective_rule(model):
                 return model.theta[0]*1  + sum(model.lamda[i2] *0 for i2 in model.I2)
         else:
             def objective_rule(model):
                 return model.delta[0]*1  + sum(model.lamda[i2] *0 for i2 in model.I2)
         return objective_rule
 
@@ -116,15 +116,15 @@
         if self.orient == ORIENT_OO:
             def input_rule(model, k):
                 return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= self.x.loc[self.I0,self.xcol[k]]
         elif self.orient == ORIENT_IO:
             def input_rule(model, k):
                 return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
                     model.theta * self.x.loc[self.I0,self.xcol[k]]
-        elif self.orient == ORIENT_HYPER:
+        elif self.orient == ORIENT_HYPERYX:
             def input_rule(model, k):
                 return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
                     model.delta * self.x.loc[self.I0,self.xcol[k]]
         elif type(self.yindexs) == type(None):
             def input_rule(model, k):
                 if k != self.xindexs:
                     return Constraint.Skip
@@ -144,15 +144,15 @@
             def output_rule(model, l):
                 return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                     >=model.theta * self.y.loc[self.I0,self.ycol[l]]
         elif self.orient == ORIENT_IO:
             def output_rule(model, l):
                 return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                     >= self.y.loc[self.I0,self.ycol[l]]
-        elif self.orient == ORIENT_HYPER:
+        elif self.orient == ORIENT_HYPERYX:
             def output_rule(model, l):
                 return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                     >= self.y.loc[self.I0,self.ycol[l]]
         elif type(self.yindexs) == type(None):
             def output_rule(model, l):
                 return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                     >= self.y.loc[self.I0,self.ycol[l]]
@@ -162,15 +162,15 @@
                     return Constraint.Skip
                 return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                     >=model.theta * self.y.loc[self.I0,self.ycol[l]]
 
         return output_rule
 
     def __vrs_rule(self):
-        if self.orient != ORIENT_HYPER:
+        if self.orient != ORIENT_HYPERYX:
             def vrs_rule(model):
                 return sum(model.lamda[ i2] for i2 in model.I2) == 1
         else:
             def vrs_rule(model):
                 return sum(model.lamda[ i2] for i2 in model.I2) == model.theta[0] *1
         return vrs_rule
```

### Comparing `pytedea-0.0.1/pytedea/utils/CNLSDDFG1.py` & `pytedea-0.0.2/pytedea/utils/CNLSDDFZG2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,134 +1,143 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import CNLSDDFZG1
-
-
-class CNLSDDFG1(CNLSDDFZG1.CNLSDDFZG1):
-    """initial Group-VC-added CNLSDDF (CNLSDDF+G) model
-    """
-
-    def __init__(self, y, x, b,  cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDF+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float,optional): undersiable variables.
-            cutactive (float, optional): active concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b = x, y, b
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-
-        if type(self.b) != type(None):
-            self.__model__.L = Set(initialize=range(len(self.b[0])))
-            self.__model__.delta = Var(
-                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
-
-
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CNLSDDFZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._CNLSDDFZG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CNLSDDFZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CNLSDDFZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.rts == RTS_VRS:
-            if type(self.b) == type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - model.epsilon[i]
-                return regression_rule
-
-            elif type(self.b) != type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        - model.epsilon[i]
-                return regression_rule
-
-
-        elif self.rts == RTS_CRS:
-            if type(self.b) == type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - model.epsilon[i]
-                return regression_rule
-
-
-            elif type(self.b) != type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        - model.epsilon[i]
-                return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-
-
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from. import CNLSDDFZG1
+class CNLSDDFZG2(CNLSDDFZG1.CNLSDDFZG1):
+    """initial Group-VC-added CNLSDDFZ (CNLSDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, cutactive, active, gy=[1], gx=[1], gb=[1],  fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables.
+            z (float): Contextual variable(s). Defaults to None.
+            cutactive (float, optional): active concavity constraint.
+            active (float or ndarray ): violated concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b,self.z = x, y, b, z
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = active
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+
+        if type(self.b) != type(None):
+            self.__model__.L = Set(initialize=range(len(self.b[0])))
+            self.__model__.delta = Var(
+                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
+
+        # Initialize the set of z
+        self.__model__.M = Set(initialize=range(len(self.z[0])))
+        # Initialize the variables for z variable
+        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
+
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CNLSDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._CNLSDDFZG1__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._CNLSDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CNLSDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CNLSDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __sweet_rule2(self, ):
+        """Return the proper sweet spot (step2) approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
+                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
+                return Constraint.Skip
+
+            return sweet_rule2
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
+                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
+                return Constraint.Skip
+
+            return sweet_rule2
+
+        raise ValueError("Undefined model parameters.")
+
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/CNLSDDFG2.py` & `pytedea-0.0.2/pytedea/utils/CNLSDDFG2.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import CNLSDDFZG2, CNLSDDFG1
-
-class CNLSDDFG2(CNLSDDFZG2.CNLSDDFZG2, CNLSDDFG1.CNLSDDFG1):
-    """initial Group-VC-added CNLSDDF (CNLSDDF+G) model
-    """
-
-    def __init__(self, y, x, b, cutactive, active, gy=[1], gx=[1], gb=[1],  fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDF+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float, optional): undersiable variables.
-            cutactive (float, optional): active concavity constraint.
-            active (float or ndarray ): violated concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b = x, y, b
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = active
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-
-
-        if type(self.b) != type(None):
-            self.__model__.L = Set(initialize=range(len(self.b[0])))
-            self.__model__.delta = Var(
-                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
-
-
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CNLSDDFG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._CNLSDDFG1__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._CNLSDDFG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CNLSDDFG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CNLSDDFG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CNLSDDFZG2__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import CNLSDDFZG2, CNLSDDFG1
+
+class CNLSDDFG2(CNLSDDFZG2.CNLSDDFZG2, CNLSDDFG1.CNLSDDFG1):
+    """initial Group-VC-added CNLSDDF (CNLSDDF+G) model
+    """
+
+    def __init__(self, y, x, b, cutactive, active, gy=[1], gx=[1], gb=[1],  fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDF+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables.
+            cutactive (float, optional): active concavity constraint.
+            active (float or ndarray ): violated concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b = x, y, b
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = active
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+
+
+        if type(self.b) != type(None):
+            self.__model__.L = Set(initialize=range(len(self.b[0])))
+            self.__model__.delta = Var(
+                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
+
+
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CNLSDDFG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._CNLSDDFG1__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._CNLSDDFG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CNLSDDFG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CNLSDDFG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CNLSDDFZG2__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/CNLSDDFZG1.py` & `pytedea-0.0.2/pytedea/utils/weakCQERDDFZG1.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,276 +1,315 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-
-class CNLSDDFZG1():
-    """initial Group-VC-added CNLSDDFZ (CNLSDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float,optional): undersiable variables.
-            z (float): Contextual variable(s). Defaults to None.
-            cutactive (float, optional): active concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b,self.z = x, y, b, z
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-
-        if type(self.b) != type(None):
-            self.__model__.L = Set(initialize=range(len(self.b[0])))
-            self.__model__.delta = Var(
-                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
-
-        # Initialize the set of z
-        self.__model__.M = Set(initialize=range(len(self.z[0])))
-        # Initialize the variables for z variable
-        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
-
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self.__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self.__afriat_rule(),
-                                                doc='elementary Afriat approach')
-
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        # TODO(error/warning handling): Check problem status after optimization
-        self.problem_status, self.optimization_status = optimize_model(
-            self.__model__, email, CET_ADDI, solver)
-
-    def __objective_rule(self):
-        """Return the proper objective function"""
-        def objective_rule(model):
-            return sum(model.epsilon[i] ** 2 for i in model.I)
-        return objective_rule
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.rts == RTS_VRS:
-            if type(self.b) == type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                        - model.epsilon[i]
-                return regression_rule
-
-            elif type(self.b) != type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                        - model.epsilon[i]
-                return regression_rule
-
-
-        elif self.rts == RTS_CRS:
-            if type(self.b) == type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                        - model.epsilon[i]
-                return regression_rule
-
-
-            elif type(self.b) != type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                        - model.epsilon[i]
-                return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __translation_property(self):
-        """Return the proper translation property"""
-        def translation_rule(model, i):
-            return sum(model.beta[i, j] * self.gx[j] for j in model.J) \
-                + sum(model.gamma[i, k] * self.gy[k] for k in model.K) \
-                + sum(model.delta[i, l] * self.gb[l] for l in model.L) == 1
-
-        return translation_rule
-
-    def __afriat_rule(self):
-        """Return the proper elementary Afriat approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def afriat_rule(model, i):
-                return __operator(
-                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
-                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                    model.alpha[self.__model__.I.nextw(i)] \
-                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
-                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
-                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
-
-            return afriat_rule
-
-        elif self.rts == RTS_CRS:
-            def afriat_rule(model, i):
-                return __operator(sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
-                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
-                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
-                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
-
-            return afriat_rule
-        raise ValueError("Undefined model parameters.")
-
-
-    def __sweet_rule(self ):
-        """Return the proper sweet spot approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                      model.alpha[h] \
-                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
-                return Constraint.Skip
-
-            return sweet_rule
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                       sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
-                return Constraint.Skip
-
-            return sweet_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def get_alpha(self):
-        """Return alpha value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        alpha = list(self.__model__.alpha[:].value)
-        return np.asarray(alpha)
-
-    def get_beta(self):
-        """Return beta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
-        return beta.to_numpy()
-
-    def get_delta(self):
-        """Return delta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
-                                                           list(self.__model__.delta[:, :].value))])
-        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
-        delta = delta.pivot(index='Name', columns='Key', values='Value')
-        return delta.to_numpy()
-
-    def get_gamma(self):
-        """Return delta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
-                                                           list(self.__model__.gamma[:, :].value))])
-        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
-        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
-        return gamma.to_numpy()
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+
+
+class weakCQRDDFZG1:
+    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            z (float): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float, optional): active concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b,self.z = x, y, b, z
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.tau = tau
+
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+
+        # Initialize the set of z
+        self.__model__.M = Set(initialize=range(len(self.z[0])))
+        # Initialize the variables for z variable
+        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
+
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self.__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self.__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self.__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self.__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        # TODO(error/warning handling): Check problem status after optimization
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, email, CET_ADDI, solver)
+
+    def __objective_rule(self):
+        """Return the proper objective function"""
+
+        def objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
+        return objective_rule
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.rts == RTS_VRS:
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == model.alpha[i] \
+                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                    - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                    - model.epsilon_minus[i] + model.epsilon_plus[i]
+
+            return regression_rule
+
+
+        elif self.rts == RTS_CRS:
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                    - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                    - model.epsilon_minus[i] + model.epsilon_plus[i]
+
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __translation_property(self):
+        """Return the proper translation property"""
+        def translation_rule(model, i):
+            return sum(model.beta[i, j] * self.gx[j] for j in model.J) \
+                + sum(model.gamma[i, k] * self.gy[k] for k in model.K) \
+                + sum(model.delta[i, l] * self.gb[l] for l in model.L) == 1
+
+        return translation_rule
+
+    def __afriat_rule(self):
+        """Return the proper elementary Afriat approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def afriat_rule(model, i):
+                return __operator(
+                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
+                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                    model.alpha[self.__model__.I.nextw(i)] \
+                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
+                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
+                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
+
+            return afriat_rule
+
+        elif self.rts == RTS_CRS:
+            def afriat_rule(model, i):
+                return __operator(sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
+                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
+                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
+                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
+
+            return afriat_rule
+        raise ValueError("Undefined model parameters.")
+
+    def __disposability_rule(self):
+        """Return the proper elementary weak disposability constraint"""
+        if self.rts == RTS_VRS:
+            def disposability_rule(model, i):
+                return model.alpha[self.__model__.I.nextw(i)] \
+                    + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
+            return disposability_rule
+
+        elif self.rts == RTS_CRS:
+            def disposability_rule(model, i):
+                return sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
+            return disposability_rule
+        raise ValueError("Undefined model parameters.")
+
+
+    def __sweet_rule(self ):
+        """Return the proper sweet spot approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
+                return Constraint.Skip
+
+            return sweet_rule
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                       sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
+                return Constraint.Skip
+
+            return sweet_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def get_alpha(self):
+        """Return alpha value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        alpha = list(self.__model__.alpha[:].value)
+        return np.asarray(alpha)
+
+    def get_beta(self):
+        """Return beta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
+                                                          list(self.__model__.beta[:, :].value))])
+        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
+        beta = beta.pivot(index='Name', columns='Key', values='Value')
+        return beta.to_numpy()
+
+    def get_delta(self):
+        """Return delta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
+                                                           list(self.__model__.delta[:, :].value))])
+        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
+        delta = delta.pivot(index='Name', columns='Key', values='Value')
+        return delta.to_numpy()
+
+    def get_gamma(self):
+        """Return delta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
+                                                           list(self.__model__.gamma[:, :].value))])
+        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
+        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
+        return gamma.to_numpy()
+
+
+class weakCERDDFZG1(weakCQRDDFZG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, z, tau, cutactive, gy, gx, gb, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/CNLSG1.py` & `pytedea-0.0.2/pytedea/utils/CNLSG2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,105 +1,109 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-
-from . import CNLSZG1
-
-
-class CNLSG1(CNLSZG1.CNLSZG1):
-    """initial Group-VC-added CNLS (CNLS+G) model
-    """
-
-    def __init__(self, y, x, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CNLS+G model 1
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CNLSZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._CNLSZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CNLSZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CNLSZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-                def regression_rule(model, i):
-                    return self.y[i] == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - model.epsilon[i]
-
-                return regression_rule
-            elif self.rts == RTS_CRS:
-                def regression_rule(model, i):
-                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - model.epsilon[i]
-
-                return regression_rule
-        elif self.cet == CET_MULT:
-
-            def regression_rule(model, i):
-                return log(
-                    self.y[i]) == log(model.frontier[i] + 1) - model.epsilon[i]
-
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model, trans_list, to_2d_list
+from . import CNLSG1, CNLSZG2, CNLSZG1
+
+class CNLSG2( CNLSZG2.CNLSZG2,CNLSZG1.CNLSZG1 ):
+    """CNLS+G in iterative loop
+    """
+
+    def __init__(self, y, x, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CNLS+G model 
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            cutactive (float): active concavity constraint.
+            active (float): violated concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.epsilon = Var(self.__model__.I, doc='resiudual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CNLSZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._CNLSZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CNLSZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CNLSZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                                self.__model__.I,
+                                                rule=self._CNLSZG2__sweet_rule2(),
+                                                doc='sweet spot-2 approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def regression_rule(model, i):
+                    return self.y[i] == model.alpha[i] + \
+                        sum(model.beta[i, j] * self.x[i][j] for j in model.J) + \
+                        model.epsilon[i]
+
+                return regression_rule
+            elif self.rts == RTS_CRS:
+
+                def regression_rule(model, i):
+                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) + \
+                        model.epsilon[i]
+
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+
+            def regression_rule(model, i):
+                return log(self.y[i]) == log(model.frontier[i] + 1) + model.epsilon[i]
+
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
```

### Comparing `pytedea-0.0.1/pytedea/utils/CNLSG2.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSDDFG2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,102 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import CNLSG1, CNLSZG2, CNLSZG1
-
-class CNLSG2( CNLSZG2.CNLSZG2,CNLSZG1.CNLSZG1 ):
-    """CNLS+G in iterative loop
-    """
-
-    def __init__(self, y, x, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CNLS+G model 
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            cutactive (float): active concavity constraint.
-            active (float): violated concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.epsilon = Var(self.__model__.I, doc='resiudual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CNLSZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._CNLSZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CNLSZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CNLSZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                                self.__model__.I,
-                                                rule=self._CNLSZG2__sweet_rule2(),
-                                                doc='sweet spot-2 approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def regression_rule(model, i):
-                    return self.y[i] == model.alpha[i] + \
-                        sum(model.beta[i, j] * self.x[i][j] for j in model.J) + \
-                        model.epsilon[i]
-
-                return regression_rule
-            elif self.rts == RTS_CRS:
-
-                def regression_rule(model, i):
-                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) + \
-                        model.epsilon[i]
-
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-
-            def regression_rule(model, i):
-                return log(self.y[i]) == log(model.frontier[i] + 1) + model.epsilon[i]
-
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import weakCNLSDDFZG2,weakCNLSDDFG1,weakCNLSDDFZG1
+
+
+class weakCNLSDDFG2(weakCNLSDDFZG2.weakCNLSDDFZG2,weakCNLSDDFG1.weakCNLSDDFG1,weakCNLSDDFZG1.weakCNLSDDFZG1):
+    """initial Group-VC-added weakCNLSDDF (weakCNLSDDF+G) model
+    """
+
+    def __init__(self, y, x, b, cutactive, active, activeweak, gy=[1], gx=[1], gb=[1],  fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSDDF+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            cutactive (float, optional): active concavity constraint.
+            active (float or ndarray ): violated concavity constraint.
+            activeweak (float or ndarray ): violated concavity constraint for weak disposibility.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b = x, y, b
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = active
+        self.activeweak = activeweak
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+
+
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCNLSDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._weakCNLSDDFG1__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._weakCNLSDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCNLSDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCNLSDDFZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCNLSDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.weakCNLSDDFZG2__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.weakCNLSDDFZG2__sweet_rule_weak2(),
+                                               doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
```

### Comparing `pytedea-0.0.1/pytedea/utils/CNLSZG1.py` & `pytedea-0.0.2/pytedea/utils/CNLSZG1.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-
-class CNLSZG1():
-    """initial Group-VC-added CNLSZ (CNLSZ+G) model
-    """
-
-    def __init__(self, y, x, z, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            z (float, optional): Contextual variable(s). Defaults to None.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.z = z
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.z[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self.__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self.__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        # TODO(error/warning handling): Check problem status after optimization
-        self.problem_status, self.optimization_status = optimize_model(
-            self.__model__, email, self.cet, solver)
-
-    def __objective_rule(self):
-        """Return the proper objective function"""
-        def objective_rule(model):
-            return sum(model.epsilon[i] ** 2 for i in model.I)
-        return objective_rule
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-                def regression_rule(model, i):
-                    return self.y[i] == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - sum(model.lamda[k] * self.z[i][k] for k in model.K) - model.epsilon[i]
-                return regression_rule
-            elif self.rts == RTS_CRS:
-
-                def regression_rule(model, i):
-                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - sum(model.lamda[k] * self.z[i][k] for k in model.K) - model.epsilon[i]
-
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-
-            def regression_rule(model, i):
-                return log(self.y[i]) == log(model.frontier[i] + 1) \
-                                - sum(model.lamda[k] * self.z[i][k] for k in model.K) - model.epsilon[i]
-
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __log_rule(self):
-        """Return the proper log constraint"""
-        if self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-                def log_rule(model, i):
-                    return model.frontier[i] == model.alpha[i] + sum(
-                        model.beta[i, j] * self.x[i][j] for j in model.J) - 1
-                return log_rule
-
-            elif self.rts == RTS_CRS:
-                def log_rule(model, i):
-                    return model.frontier[i] == sum(
-                        model.beta[i, j] * self.x[i][j] for j in model.J) - 1
-                return log_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __afriat_rule(self):
-        """Return the proper elementary Afriat approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def afriat_rule(model, i):
-                    return __operator(
-                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                             for j in model.J),
-                        model.alpha[self.__model__.I.nextw(i)] +
-                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
-                            for j in model.J))
-
-                return afriat_rule
-            elif self.rts == RTS_CRS:
-                def afriat_rule(model, i):
-                    return __operator(
-                        sum(model.beta[i, j] * self.x[i][j]
-                            for j in model.J),
-                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
-                            for j in model.J))
-
-                return afriat_rule
-        elif self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-
-                def afriat_rule(model, i):
-                    return __operator(
-                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                             for j in model.J),
-                        model.alpha[self.__model__.I.nextw(i)] +
-                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
-                            for j in model.J))
-
-                return afriat_rule
-            elif self.rts == RTS_CRS:
-
-                def afriat_rule(model, i):
-                    return __operator(
-                        sum(model.beta[i, j] * self.x[i][j] for j in model.J),
-                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J))
-
-                return afriat_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __sweet_rule(self, ):
-        """Return the proper sweet spot approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def sweet_rule(model, i, h):
-                    if self.cutactive[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                                               for j in model.J),
-                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                                               for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule
-            elif self.rts == RTS_CRS:
-
-                def sweet_rule(model, i, h):
-                    if self.cutactive[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(sum(model.beta[i, j] * self.x[i][j]
-                                              for j in model.J),
-                                          sum(model.beta[h, j] * self.x[i][j]
-                                              for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule
-        elif self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-
-                def sweet_rule(model, i, h):
-                    if self.cutactive[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                                               for j in model.J),
-                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                                               for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule
-            elif self.rts == RTS_CRS:
-
-                def sweet_rule(model, i, h):
-                    if self.cutactive[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J),
-                                          sum(model.beta[h, j] * self.x[i][j] for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def get_alpha(self):
-        """Return alpha value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        alpha = list(self.__model__.alpha[:].value)
-        return np.asarray(alpha)
-
-    def get_beta(self):
-        """Return beta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
-        return beta.to_numpy()
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+
+class CNLSZG1():
+    """initial Group-VC-added CNLSZ (CNLSZ+G) model
+    """
+
+    def __init__(self, y, x, z, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            z (float, optional): Contextual variable(s). Defaults to None.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.z = z
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.z[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self.__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self.__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self.__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        # TODO(error/warning handling): Check problem status after optimization
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, email, self.cet, solver)
+
+    def __objective_rule(self):
+        """Return the proper objective function"""
+        def objective_rule(model):
+            return sum(model.epsilon[i] ** 2 for i in model.I)
+        return objective_rule
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+                def regression_rule(model, i):
+                    return self.y[i] == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - sum(model.lamda[k] * self.z[i][k] for k in model.K) - model.epsilon[i]
+                return regression_rule
+            elif self.rts == RTS_CRS:
+
+                def regression_rule(model, i):
+                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - sum(model.lamda[k] * self.z[i][k] for k in model.K) - model.epsilon[i]
+
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+
+            def regression_rule(model, i):
+                return log(self.y[i]) == log(model.frontier[i] + 1) \
+                                - sum(model.lamda[k] * self.z[i][k] for k in model.K) - model.epsilon[i]
+
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __log_rule(self):
+        """Return the proper log constraint"""
+        if self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+                def log_rule(model, i):
+                    return model.frontier[i] == model.alpha[i] + sum(
+                        model.beta[i, j] * self.x[i][j] for j in model.J) - 1
+                return log_rule
+
+            elif self.rts == RTS_CRS:
+                def log_rule(model, i):
+                    return model.frontier[i] == sum(
+                        model.beta[i, j] * self.x[i][j] for j in model.J) - 1
+                return log_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __afriat_rule(self):
+        """Return the proper elementary Afriat approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def afriat_rule(model, i):
+                    return __operator(
+                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                             for j in model.J),
+                        model.alpha[self.__model__.I.nextw(i)] +
+                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
+                            for j in model.J))
+
+                return afriat_rule
+            elif self.rts == RTS_CRS:
+                def afriat_rule(model, i):
+                    return __operator(
+                        sum(model.beta[i, j] * self.x[i][j]
+                            for j in model.J),
+                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
+                            for j in model.J))
+
+                return afriat_rule
+        elif self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+
+                def afriat_rule(model, i):
+                    return __operator(
+                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                             for j in model.J),
+                        model.alpha[self.__model__.I.nextw(i)] +
+                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
+                            for j in model.J))
+
+                return afriat_rule
+            elif self.rts == RTS_CRS:
+
+                def afriat_rule(model, i):
+                    return __operator(
+                        sum(model.beta[i, j] * self.x[i][j] for j in model.J),
+                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J))
+
+                return afriat_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __sweet_rule(self, ):
+        """Return the proper sweet spot approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def sweet_rule(model, i, h):
+                    if self.cutactive[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                                               for j in model.J),
+                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
+                                                               for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule
+            elif self.rts == RTS_CRS:
+
+                def sweet_rule(model, i, h):
+                    if self.cutactive[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(sum(model.beta[i, j] * self.x[i][j]
+                                              for j in model.J),
+                                          sum(model.beta[h, j] * self.x[i][j]
+                                              for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule
+        elif self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+
+                def sweet_rule(model, i, h):
+                    if self.cutactive[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                                               for j in model.J),
+                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
+                                                               for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule
+            elif self.rts == RTS_CRS:
+
+                def sweet_rule(model, i, h):
+                    if self.cutactive[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J),
+                                          sum(model.beta[h, j] * self.x[i][j] for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def get_alpha(self):
+        """Return alpha value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        alpha = list(self.__model__.alpha[:].value)
+        return np.asarray(alpha)
+
+    def get_beta(self):
+        """Return beta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
+                                                          list(self.__model__.beta[:, :].value))])
+        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
+        beta = beta.pivot(index='Name', columns='Key', values='Value')
+        return beta.to_numpy()
```

### Comparing `pytedea-0.0.1/pytedea/utils/CNLSZG2.py` & `pytedea-0.0.2/pytedea/utils/CNLSZG2.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import CNLSZG1
-
-class CNLSZG2(CNLSZG1.CNLSZG1):
-    """CNLSZ+G in iterative loop
-    """
-
-    def __init__(self, y, x, z, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            z (float, optional): Contextual variable(s). Defaults to None.
-            cutactive (float): active concavity constraint.
-            active (float): violated concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.z = z
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.z[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.lamda = Var(self.__model__.K, doc='zvalue')
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CNLSZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._CNLSZG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._CNLSZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CNLSZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CNLSZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                                self.__model__.I,
-                                                rule=self.__sweet_rule2(),
-                                                doc='sweet spot-2 approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-
-    def __sweet_rule2(self, ):
-        """Return the proper sweet spot (step2) approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-                def sweet_rule2(model, i, h):
-                    if self.active[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                                               for j in model.J),
-                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                                               for j in model.J))
-                    return Constraint.Skip
-                return sweet_rule2
-
-            elif self.rts == RTS_CRS:
-                def sweet_rule2(model, i, h):
-                    if self.active[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(sum(model.beta[i, j] * self.x[i][j]
-                                              for j in model.J),
-                                          sum(model.beta[h, j] * self.x[i][j]
-                                              for j in model.J))
-                    return Constraint.Skip
-                return sweet_rule2
-
-        elif self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-                def sweet_rule2(model, i, h):
-                    if self.active[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                                               for j in model.J),
-                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                                               for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule2
-
-            elif self.rts == RTS_CRS:
-                def sweet_rule2(model, i, h):
-                    if self.active[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J),
-                                          sum(model.beta[h, j] * self.x[i][j] for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule2
-
-        raise ValueError("Undefined model parameters.")
-
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model, trans_list, to_2d_list
+from . import CNLSZG1
+
+class CNLSZG2(CNLSZG1.CNLSZG1):
+    """CNLSZ+G in iterative loop
+    """
+
+    def __init__(self, y, x, z, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            z (float, optional): Contextual variable(s). Defaults to None.
+            cutactive (float): active concavity constraint.
+            active (float): violated concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.z = z
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.z[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.lamda = Var(self.__model__.K, doc='zvalue')
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CNLSZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._CNLSZG1__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._CNLSZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CNLSZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CNLSZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                                self.__model__.I,
+                                                rule=self.__sweet_rule2(),
+                                                doc='sweet spot-2 approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+
+    def __sweet_rule2(self, ):
+        """Return the proper sweet spot (step2) approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+                def sweet_rule2(model, i, h):
+                    if self.active[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                                               for j in model.J),
+                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
+                                                               for j in model.J))
+                    return Constraint.Skip
+                return sweet_rule2
+
+            elif self.rts == RTS_CRS:
+                def sweet_rule2(model, i, h):
+                    if self.active[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(sum(model.beta[i, j] * self.x[i][j]
+                                              for j in model.J),
+                                          sum(model.beta[h, j] * self.x[i][j]
+                                              for j in model.J))
+                    return Constraint.Skip
+                return sweet_rule2
+
+        elif self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+                def sweet_rule2(model, i, h):
+                    if self.active[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                                               for j in model.J),
+                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
+                                                               for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule2
+
+            elif self.rts == RTS_CRS:
+                def sweet_rule2(model, i, h):
+                    if self.active[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J),
+                                          sum(model.beta[h, j] * self.x[i][j] for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule2
+
+        raise ValueError("Undefined model parameters.")
+
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/CQERDDFG1.py` & `pytedea-0.0.2/pytedea/utils/CQERDDFG1.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import CQERDDFZG1
-
-class CQRDDFG1(CQERDDFZG1.CQRDDFZG1):
-    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float, optional): undersiable variables.
-            tau (float): quantile.
-            cutactive (float, optional): active concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b = x, y, b
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.tau = tau
-
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-
-
-        if type(self.b) != type(None):
-            self.__model__.L = Set(initialize=range(len(self.b[0])))
-            self.__model__.delta = Var(
-                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-
-
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CQRDDFZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._CQRDDFZG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CQRDDFZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._CQRDDFZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CQRDDFZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.rts == RTS_VRS:
-            if type(self.b) != type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        - model.epsilon_minus[i] + model.epsilon_plus[i]
-                return regression_rule
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == model.alpha[i] \
-                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    - model.epsilon_minus[i] + model.epsilon_plus[i]
-            return regression_rule
-        elif self.rts == RTS_CRS:
-            if type(self.b) != type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        - model.epsilon_minus[i] + model.epsilon_plus[i]
-                return regression_rule
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    - model.epsilon_minus[i] + model.epsilon_plus[i]
-            return regression_rule
-        raise ValueError("Undefined model parameters.")
-
-
-class CERDDFG1(CQRDDFG1):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float, optional): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, tau, cutactive, gy, gx, gb, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import CQERDDFZG1
+
+class CQRDDFG1(CQERDDFZG1.CQRDDFZG1):
+    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables.
+            tau (float): quantile.
+            cutactive (float, optional): active concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b = x, y, b
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.tau = tau
+
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+
+
+        if type(self.b) != type(None):
+            self.__model__.L = Set(initialize=range(len(self.b[0])))
+            self.__model__.delta = Var(
+                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+
+
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CQRDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._CQRDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CQRDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._CQRDDFZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CQRDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.rts == RTS_VRS:
+            if type(self.b) != type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        - model.epsilon_minus[i] + model.epsilon_plus[i]
+                return regression_rule
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == model.alpha[i] \
+                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    - model.epsilon_minus[i] + model.epsilon_plus[i]
+            return regression_rule
+        elif self.rts == RTS_CRS:
+            if type(self.b) != type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        - model.epsilon_minus[i] + model.epsilon_plus[i]
+                return regression_rule
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    - model.epsilon_minus[i] + model.epsilon_plus[i]
+            return regression_rule
+        raise ValueError("Undefined model parameters.")
+
+
+class CERDDFG1(CQRDDFG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, tau, cutactive, gy, gx, gb, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/CQERDDFG2.py` & `pytedea-0.0.2/pytedea/utils/weakCQERDDFG2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,135 +1,138 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import CQERDDFZG1,CQERDDFZG2,CQERDDFG1
-
-class CQRDDFG2(CQERDDFZG2.CQRDDFZG2,CQERDDFG1.CQRDDFG1,CQERDDFZG1.CQRDDFZG1):
-    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive,active, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float, optional): undersiable variables.
-            tau (float): quantile.
-            cutactive (float, optional): active concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b = x, y, b
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.tau = tau
-
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = active
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-
-
-        if type(self.b) != type(None):
-            self.__model__.L = Set(initialize=range(len(self.b[0])))
-            self.__model__.delta = Var(
-                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-
-
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CQRDDFZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._CQRDDFG1__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._CQRDDFZG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CQRDDFZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._CQRDDFZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CQRDDFZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CQRDDFZG2__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-
-class CERDDFG2(CQRDDFG2):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive, active, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float, optional): undersiable variables
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, tau, cutactive,active, gy, gx, gb, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import weakCQERDDFZG1,weakCQERDDFZG2,weakCQERDDFG1
+
+
+class weakCQRDDFG2(weakCQERDDFZG2.weakCQRDDFZG2,weakCQERDDFG1.weakCQRDDFG1,weakCQERDDFZG1.weakCQRDDFZG1):
+    """initial Group-VC-added weakCQRDDFZ (weakCQRDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, active, activeweak, gy=[1], gx=[1], gb=[1],  fun=FUN_PROD, rts=RTS_VRS):
+        """weakCQRDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            tau (float): quantile.
+            cutactive (float, optional): active concavity constraint.
+            active (float or ndarray ): violated concavity constraint.
+            activeweak (float or ndarray ): violated concavity constraint for weak disposibility.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b = x, y, b
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.fun = fun
+        self.rts = rts
+        self.tau = tau
+
+        self.cutactive = cutactive
+        self.active = active
+        self.activeweak = activeweak
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._weakCQERDDFG1__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._weakCQRDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCQRDDFZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRDDFZG2__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRDDFZG2__sweet_rule_weak2(),
+                                               doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+class weakCERDDFG2(weakCQRDDFG2):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b,  tau, cutactive,active, activeweak, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, tau, cutactive, active, activeweak, gy,gx,gb, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/CQERDDFZG1.py` & `pytedea-0.0.2/pytedea/utils/CQERDDFZG1.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-
-
-class CQRDDFZG1:
-    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float, optional): undersiable variables.
-            z (float): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float, optional): active concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b,self.z = x, y, b, z
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.tau = tau
-
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-
-
-        if type(self.b) != type(None):
-            self.__model__.L = Set(initialize=range(len(self.b[0])))
-            self.__model__.delta = Var(
-                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-
-        # Initialize the set of z
-        self.__model__.M = Set(initialize=range(len(self.z[0])))
-        # Initialize the variables for z variable
-        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
-
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self.__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self.__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self.__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        # TODO(error/warning handling): Check problem status after optimization
-        self.problem_status, self.optimization_status = optimize_model(
-            self.__model__, email, CET_ADDI, solver)
-
-    def __objective_rule(self):
-        """Return the proper objective function"""
-
-        def objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
-        return objective_rule
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.rts == RTS_VRS:
-            if type(self.b) != type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                        - model.epsilon_minus[i] + model.epsilon_plus[i]
-                return regression_rule
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == model.alpha[i] \
-                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                    - model.epsilon_minus[i] + model.epsilon_plus[i]
-            return regression_rule
-        elif self.rts == RTS_CRS:
-            if type(self.b) != type(None):
-                def regression_rule(model, i):
-                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                        - model.epsilon_minus[i] + model.epsilon_plus[i]
-                return regression_rule
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                    - model.epsilon_minus[i] + model.epsilon_plus[i]
-            return regression_rule
-        raise ValueError("Undefined model parameters.")
-
-    def __translation_property(self):
-        """Return the proper translation property"""
-        def translation_rule(model, i):
-            return sum(model.beta[i, j] * self.gx[j] for j in model.J) \
-                + sum(model.gamma[i, k] * self.gy[k] for k in model.K) \
-                + sum(model.delta[i, l] * self.gb[l] for l in model.L) == 1
-        return translation_rule
-
-    def __afriat_rule(self):
-        """Return the proper elementary Afriat approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-            def afriat_rule(model, i):
-                return __operator(
-                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
-                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                    model.alpha[self.__model__.I.nextw(i)] \
-                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
-                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
-                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
-            return afriat_rule
-
-        elif self.rts == RTS_CRS:
-            def afriat_rule(model, i):
-                return __operator(sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
-                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
-                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
-                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
-            return afriat_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __disposability_rule(self):
-        """Return the proper elementary weak disposability constraint"""
-        if self.rts == RTS_VRS:
-            def disposability_rule(model, i):
-                return model.alpha[self.__model__.I.nextw(i)] \
-                    + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
-            return disposability_rule
-
-        elif self.rts == RTS_CRS:
-            def disposability_rule(model, i):
-                return sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
-            return disposability_rule
-        raise ValueError("Undefined model parameters.")
-
-
-    def __sweet_rule(self ):
-        """Return the proper sweet spot approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                      model.alpha[h] \
-                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
-                return Constraint.Skip
-
-            return sweet_rule
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                       sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
-                return Constraint.Skip
-
-            return sweet_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def get_alpha(self):
-        """Return alpha value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        alpha = list(self.__model__.alpha[:].value)
-        return np.asarray(alpha)
-
-    def get_beta(self):
-        """Return beta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
-        return beta.to_numpy()
-
-    def get_delta(self):
-        """Return delta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
-                                                           list(self.__model__.delta[:, :].value))])
-        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
-        delta = delta.pivot(index='Name', columns='Key', values='Value')
-        return delta.to_numpy()
-
-    def get_gamma(self):
-        """Return delta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
-                                                           list(self.__model__.gamma[:, :].value))])
-        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
-        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
-        return gamma.to_numpy()
-
-
-class CERDDFZG1(CQRDDFZG1):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float, optional): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, z, tau, cutactive, gy, gx, gb, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+
+
+class CQRDDFZG1:
+    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables.
+            z (float): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float, optional): active concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b,self.z = x, y, b, z
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.tau = tau
+
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+
+
+        if type(self.b) != type(None):
+            self.__model__.L = Set(initialize=range(len(self.b[0])))
+            self.__model__.delta = Var(
+                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+
+        # Initialize the set of z
+        self.__model__.M = Set(initialize=range(len(self.z[0])))
+        # Initialize the variables for z variable
+        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
+
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self.__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self.__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self.__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self.__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        # TODO(error/warning handling): Check problem status after optimization
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, email, CET_ADDI, solver)
+
+    def __objective_rule(self):
+        """Return the proper objective function"""
+
+        def objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
+        return objective_rule
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.rts == RTS_VRS:
+            if type(self.b) != type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                        - model.epsilon_minus[i] + model.epsilon_plus[i]
+                return regression_rule
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == model.alpha[i] \
+                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                    - model.epsilon_minus[i] + model.epsilon_plus[i]
+            return regression_rule
+        elif self.rts == RTS_CRS:
+            if type(self.b) != type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                        - model.epsilon_minus[i] + model.epsilon_plus[i]
+                return regression_rule
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                    - model.epsilon_minus[i] + model.epsilon_plus[i]
+            return regression_rule
+        raise ValueError("Undefined model parameters.")
+
+    def __translation_property(self):
+        """Return the proper translation property"""
+        def translation_rule(model, i):
+            return sum(model.beta[i, j] * self.gx[j] for j in model.J) \
+                + sum(model.gamma[i, k] * self.gy[k] for k in model.K) \
+                + sum(model.delta[i, l] * self.gb[l] for l in model.L) == 1
+        return translation_rule
+
+    def __afriat_rule(self):
+        """Return the proper elementary Afriat approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+            def afriat_rule(model, i):
+                return __operator(
+                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
+                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                    model.alpha[self.__model__.I.nextw(i)] \
+                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
+                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
+                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
+            return afriat_rule
+
+        elif self.rts == RTS_CRS:
+            def afriat_rule(model, i):
+                return __operator(sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
+                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
+                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
+                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
+            return afriat_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __disposability_rule(self):
+        """Return the proper elementary weak disposability constraint"""
+        if self.rts == RTS_VRS:
+            def disposability_rule(model, i):
+                return model.alpha[self.__model__.I.nextw(i)] \
+                    + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
+            return disposability_rule
+
+        elif self.rts == RTS_CRS:
+            def disposability_rule(model, i):
+                return sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
+            return disposability_rule
+        raise ValueError("Undefined model parameters.")
+
+
+    def __sweet_rule(self ):
+        """Return the proper sweet spot approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
+                return Constraint.Skip
+
+            return sweet_rule
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                       sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
+                return Constraint.Skip
+
+            return sweet_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def get_alpha(self):
+        """Return alpha value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        alpha = list(self.__model__.alpha[:].value)
+        return np.asarray(alpha)
+
+    def get_beta(self):
+        """Return beta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
+                                                          list(self.__model__.beta[:, :].value))])
+        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
+        beta = beta.pivot(index='Name', columns='Key', values='Value')
+        return beta.to_numpy()
+
+    def get_delta(self):
+        """Return delta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
+                                                           list(self.__model__.delta[:, :].value))])
+        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
+        delta = delta.pivot(index='Name', columns='Key', values='Value')
+        return delta.to_numpy()
+
+    def get_gamma(self):
+        """Return delta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
+                                                           list(self.__model__.gamma[:, :].value))])
+        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
+        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
+        return gamma.to_numpy()
+
+
+class CERDDFZG1(CQRDDFZG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, z, tau, cutactive, gy, gx, gb, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/CQERDDFZG2.py` & `pytedea-0.0.2/pytedea/utils/weakCQERDDFZG2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,184 +1,213 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import CQERDDFZG1
-
-class CQRDDFZG2(CQERDDFZG1.CQRDDFZG1):
-    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive,active,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float, optional): undersiable variables.
-            z (float): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float, optional): active concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b,self.z = x, y, b, z
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.tau = tau
-
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = active
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-
-
-        if type(self.b) != type(None):
-            self.__model__.L = Set(initialize=range(len(self.b[0])))
-            self.__model__.delta = Var(
-                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-
-        # Initialize the set of z
-        self.__model__.M = Set(initialize=range(len(self.z[0])))
-        # Initialize the variables for z variable
-        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
-
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CQRDDFZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._CQRDDFZG1__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._CQRDDFZG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CQRDDFZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._CQRDDFZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CQRDDFZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def __sweet_rule2(self, ):
-        """Return the proper sweet spot (step2) approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule2(model, i, h):
-                if self.active[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                      model.alpha[h] \
-                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
-                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
-                return Constraint.Skip
-
-            return sweet_rule2
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule2(model, i, h):
-                if self.active[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
-                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
-                return Constraint.Skip
-
-            return sweet_rule2
-
-        raise ValueError("Undefined model parameters.")
-
-
-
-
-class CERDDFZG2(CQRDDFZG2):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive,active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float, optional): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, z, tau, cutactive,active, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import weakCQERDDFZG1
+
+
+class weakCQRDDFZG2(weakCQERDDFZG1.weakCQRDDFZG1):
+    """initial Group-VC-added weakCQRDDFZ (weakCQRDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, active, activeweak, gy=[1], gx=[1], gb=[1],  fun=FUN_PROD, rts=RTS_VRS):
+        """weakCQRDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float, optional): active concavity constraint.
+            active (float or ndarray ): violated concavity constraint.
+            activeweak (float or ndarray ): violated concavity constraint for weak disposibility.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b,self.z = x, y, b, z
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.fun = fun
+        self.rts = rts
+        self.tau = tau
+
+        self.cutactive = cutactive
+        self.active = active
+        self.activeweak = activeweak
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+
+        # Initialize the set of z
+        self.__model__.M = Set(initialize=range(len(self.z[0])))
+        # Initialize the variables for z variable
+        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._weakCQRDDFZG1__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._weakCQRDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCQRDDFZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule_weak2(),
+                                               doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __sweet_rule2(self):
+        """Return the proper sweet spot (step2) approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
+                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
+                return Constraint.Skip
+
+            return sweet_rule2
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
+                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
+                return Constraint.Skip
+
+            return sweet_rule2
+
+        raise ValueError("Undefined model parameters.")
+
+    def __sweet_rule_weak2(self, ):
+        """Return the proper sweet spot (step2) approach constraint for weak dis"""
+
+        if self.rts == RTS_VRS:
+            def sweet_rule_weak2(model, i, h):
+                if self.activeweak[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return model.alpha[i] + sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
+                return Constraint.Skip
+
+            return sweet_rule_weak2
+
+        elif self.rts == RTS_CRS:
+            def sweet_rule_weak2(model, i, h):
+                if self.activeweak[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return  sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
+                return Constraint.Skip
+            return sweet_rule_weak2
+
+        raise ValueError("Undefined model parameters.")
+
+
+
+class weakCERDDFZG2(weakCQRDDFZG2):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive,active, activeweak, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, z, tau, cutactive, active, activeweak, gy,gx,gb, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/CQERG1.py` & `pytedea-0.0.2/pytedea/utils/CQERG1.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import CQERZG1
-
-class CQRG1(CQERZG1.CQRZG1):
-    """initial Group-VC-added CQR (CQR+G) model
-    """
-
-    def __init__(self, y, x, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CQR+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            tau (float): quantile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CQRZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._CQRZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CQRZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CQRZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-                def regression_rule(model, i):
-                    return self.y[i] == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - model.epsilon_minus[i] + model.epsilon_plus[i]
-                return regression_rule
-
-            elif self.rts == RTS_CRS:
-                def regression_rule(model, i):
-                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - model.epsilon_minus[i] + model.epsilon_plus[i]
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-            def regression_rule(model, i):
-                return log(
-                    self.y[i]) == log(model.frontier[i] + 1) \
-                            - model.epsilon_minus[i] + model.epsilon_plus[i]
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-
-class CERG1(CQRG1):
-    """initial Group-VC-added CER (CER+G) model
-    """
-
-    def __init__(self, y, x, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CER+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, tau, cutactive, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * \
-                sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import CQERZG1
+
+class CQRG1(CQERZG1.CQRZG1):
+    """initial Group-VC-added CQR (CQR+G) model
+    """
+
+    def __init__(self, y, x, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CQR+G model
+
+        Args:
+            y (float): output variable. 
+            x (float): input variables.
+            tau (float): quantile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CQRZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._CQRZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CQRZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CQRZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+                def regression_rule(model, i):
+                    return self.y[i] == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - model.epsilon_minus[i] + model.epsilon_plus[i]
+                return regression_rule
+
+            elif self.rts == RTS_CRS:
+                def regression_rule(model, i):
+                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - model.epsilon_minus[i] + model.epsilon_plus[i]
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+            def regression_rule(model, i):
+                return log(
+                    self.y[i]) == log(model.frontier[i] + 1) \
+                            - model.epsilon_minus[i] + model.epsilon_plus[i]
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+
+class CERG1(CQRG1):
+    """initial Group-VC-added CER (CER+G) model
+    """
+
+    def __init__(self, y, x, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CER+G model
+
+        Args:
+            y (float): output variable. 
+            x (float): input variables.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, tau, cutactive, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * \
+                sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
```

### Comparing `pytedea-0.0.1/pytedea/utils/CQERG2.py` & `pytedea-0.0.2/pytedea/utils/CQERDDFG2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,115 +1,135 @@
-# Import pyomo module
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import CQERZG1,CQERZG2,CQERG1
-
-
-class CQRG2(CQERZG2.CQRZG2,CQERG1.CQRG1,CQERZG1.CQRZG1):
-    """CQR+G in iterative loop
-    """
-
-    def __init__(self, y, x, tau, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CQR+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            tau (float): quantile.
-            cutactive (float): active concavity constraint.
-            active (float): violated concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CQRZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self._CQRG1__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._CQRZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CQRZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CQRZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                                self.__model__.I,
-                                                rule=self._CQRZG2__sweet_rule2(),
-                                                doc='sweet spot-2 approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-class CERG2(CQRG2):
-    """CER+G in iterative loop
-    """
-
-    def __init__(self, y, x, tau, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CER+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            active (float): violated concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, tau, cutactive, active, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import CQERDDFZG1,CQERDDFZG2,CQERDDFG1
+
+class CQRDDFG2(CQERDDFZG2.CQRDDFZG2,CQERDDFG1.CQRDDFG1,CQERDDFZG1.CQRDDFZG1):
+    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive,active, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables.
+            tau (float): quantile.
+            cutactive (float, optional): active concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b = x, y, b
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.tau = tau
+
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = active
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+
+
+        if type(self.b) != type(None):
+            self.__model__.L = Set(initialize=range(len(self.b[0])))
+            self.__model__.delta = Var(
+                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+
+
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CQRDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._CQRDDFG1__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._CQRDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CQRDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._CQRDDFZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CQRDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CQRDDFZG2__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+
+class CERDDFG2(CQRDDFG2):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, active, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, tau, cutactive,active, gy, gx, gb, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/CQERZG1.py` & `pytedea-0.0.2/pytedea/utils/weakCQERZG1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,300 +1,297 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-
-class CQRZG1():
-    """initial Group-VC-added CQRZ (CQRZ+G) model
-    """
-
-    def __init__(self, y, x, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CQRZ+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.z = z
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.z[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self.__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self.__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        # TODO(error/warning handling): Check problem status after optimization
-        self.problem_status, self.optimization_status = optimize_model(
-            self.__model__, email, self.cet, solver)
-
-    def __objective_rule(self):
-        """Return the proper objective function"""
-
-        def objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
-        return objective_rule
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def regression_rule(model, i):
-                    return self.y[i] == model.alpha[i] \
-                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                        - model.epsilon_minus[i] + model.epsilon_plus[i]
-
-                return regression_rule
-            elif self.rts == RTS_CRS:
-
-                def regression_rule(model, i):
-                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                        - model.epsilon_minus[i] + model.epsilon_plus[i]
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-
-            def regression_rule(model, i):
-                return log(self.y[i]) == log(model.frontier[i] + 1) \
-                    - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                    - model.epsilon_minus[i] + model.epsilon_plus[i]
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __log_rule(self):
-        """Return the proper log constraint"""
-        if self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-                def log_rule(model, i):
-                    return model.frontier[i] == model.alpha[i] + sum(
-                        model.beta[i, j] * self.x[i][j] for j in model.J) - 1
-                return log_rule
-
-            elif self.rts == RTS_CRS:
-                def log_rule(model, i):
-                    return model.frontier[i] == sum(
-                        model.beta[i, j] * self.x[i][j] for j in model.J) - 1
-                return log_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __afriat_rule(self):
-        """Return the proper elementary Afriat approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-                def afriat_rule(model, i):
-                    return __operator(
-                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                             for j in model.J),
-                        model.alpha[self.__model__.I.nextw(i)] +
-                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
-                            for j in model.J))
-                return afriat_rule
-
-            elif self.rts == RTS_CRS:
-                def afriat_rule(model, i):
-                    return __operator(
-                        sum(model.beta[i, j] * self.x[i][j]
-                            for j in model.J),
-                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
-                            for j in model.J))
-                return afriat_rule
-
-        elif self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-                def afriat_rule(model, i):
-                    return __operator(
-                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                             for j in model.J),
-                        model.alpha[self.__model__.I.nextw(i)] +
-                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
-                            for j in model.J))
-                return afriat_rule
-
-            elif self.rts == RTS_CRS:
-                def afriat_rule(model, i):
-                    return __operator(
-                        sum(model.beta[i, j] * self.x[i][j] for j in model.J),
-                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J))
-                return afriat_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __sweet_rule(self, ):
-        """Return the proper sweet spot approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-                def sweet_rule(model, i, h):
-                    if self.cutactive[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                                               for j in model.J),
-                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                                               for j in model.J))
-                    return Constraint.Skip
-                return sweet_rule
-
-            elif self.rts == RTS_CRS:
-                def sweet_rule(model, i, h):
-                    if self.cutactive[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(sum(model.beta[i, j] * self.x[i][j]
-                                              for j in model.J),
-                                          sum(model.beta[h, j] * self.x[i][j]
-                                              for j in model.J))
-                    return Constraint.Skip
-                return sweet_rule
-
-        elif self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-                def sweet_rule(model, i, h):
-                    if self.cutactive[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                                               for j in model.J),
-                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                                               for j in model.J))
-                    return Constraint.Skip
-                return sweet_rule
-
-            elif self.rts == RTS_CRS:
-                def sweet_rule(model, i, h):
-                    if self.cutactive[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J),
-                                          sum(model.beta[h, j] * self.x[i][j] for j in model.J))
-                    return Constraint.Skip
-                return sweet_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def get_alpha(self):
-        """Return alpha value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        alpha = list(self.__model__.alpha[:].value)
-        return np.asarray(alpha)
-
-    def get_beta(self):
-        """Return beta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
-        return beta.to_numpy()
-
-
-class CERZG1(CQRZG1):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, z, tau, cutactive, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+
+
+class weakCQRZG1:
+    """initial Group-VC-added CQRZ (CQRZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCQRZ+G model
+
+        Args:
+            y (ndarray): output variable.
+            x (ndarray): input variables.
+            b (ndarray): undersiable variables.
+            z (ndarray): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.y, self.x, self.b, self.z = y, x, b, z
+
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+
+        self.__model__.K = Set(initialize=range(len(self.z[0])))
+        self.__model__.lamda = Var(self.__model__.K, doc='z coefficient')
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self.__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self.__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self.__afriat_rule(),
+                                                doc='elementary afriat inequality')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self.__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        # TODO(error/warning handling): Check problem status after optimization
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, email, self.cet, solver)
+
+    def __objective_rule(self):
+        """Return the proper objective function"""
+
+        def objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
+        return objective_rule
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def regression_rule(model, i):
+                    return self.y[i] == model.alpha[i] \
+                            + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                            - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                            + model.epsilon_plus[i] - model.epsilon_minus[i]
+                return regression_rule
+
+            elif self.rts == RTS_CRS:
+                def regression_rule(model, i):
+                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                            - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                            + model.epsilon_plus[i] - model.epsilon_minus[i]
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+
+            def regression_rule(model, i):
+                return log(self.y[i]) == log(model.frontier[i] + 1) \
+                        - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                        + model.epsilon_plus[i] - model.epsilon_minus[i]
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __log_rule(self):
+        """Return the proper log constraint"""
+        if self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+
+                def log_rule(model, i):
+                    return model.frontier[i] == model.alpha[i] + sum(
+                        model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
+                return log_rule
+            elif self.rts == RTS_CRS:
+
+                def log_rule(model, i):
+                    return model.frontier[i] == sum(
+                        model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
+                return log_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __afriat_rule(self):
+        """Return the proper elementary Afriat approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+            def afriat_rule(model, i):
+                return __operator(
+                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
+                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
+                    model.alpha[self.__model__.I.nextw(i)] \
+                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
+                        + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L))
+            return afriat_rule
+
+        elif self.rts == RTS_CRS:
+            def afriat_rule(model, i):
+                return __operator(
+                    sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                           + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
+                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) \
+                            + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L))
+            return afriat_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __disposability_rule(self):
+        """Return the proper elementary weak disposability constraint"""
+        if self.rts == RTS_VRS:
+            def disposability_rule(model, i):
+                return model.alpha[self.__model__.I.nextw(i)] \
+                    + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
+            return disposability_rule
+
+        elif self.rts == RTS_CRS:
+            def disposability_rule(model, i):
+                return sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
+            return disposability_rule
+        raise ValueError("Undefined model parameters.")
+
+    def __sweet_rule(self, ):
+        """Return the proper sweet spot approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J)
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J)
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
+                return Constraint.Skip
+            return sweet_rule
+
+        elif self.rts == RTS_CRS:
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator( sum(model.beta[i, j] * self.x[i][j] for j in model.J)
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
+                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J)
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
+                return Constraint.Skip
+            return sweet_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def get_alpha(self):
+        """Return alpha value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        alpha = list(self.__model__.alpha[:].value)
+        return np.asarray(alpha)
+
+    def get_beta(self):
+        """Return beta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
+                                                          list(self.__model__.beta[:, :].value))])
+        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
+        beta = beta.pivot(index='Name', columns='Key', values='Value')
+        return beta.to_numpy()
+
+    def get_delta(self):
+        """Return delta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
+                                                           list(self.__model__.delta[:, :].value))])
+        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
+        delta = delta.pivot(index='Name', columns='Key', values='Value')
+        return delta.to_numpy()
+
+class weakCERZG1(weakCQRZG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable. 
+            x (float): input variables.
+            b (float): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, z, tau, cutactive, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
```

### Comparing `pytedea-0.0.1/pytedea/utils/CQERZG2.py` & `pytedea-0.0.2/pytedea/utils/CQERZG2.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import CQERZG1
-
-
-class CQRZG2(CQERZG1.CQRZG1):
-    """CQRZ+G in iterative loop
-    """
-
-    def __init__(self, y, x, z, tau, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CQRZ+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float): active concavity constraint.
-            active (float): violated concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.z = z
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.z[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.lamda = Var(self.__model__.K, doc='zvalue')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._CQRZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._CQRZG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._CQRZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._CQRZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._CQRZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                                self.__model__.I,
-                                                rule=self.__sweet_rule2(),
-                                                doc='sweet spot-2 approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-    def __sweet_rule2(self, ):
-        """Return the proper sweet spot (step2) approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def sweet_rule2(model, i, h):
-                    if self.active[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                                               for j in model.J),
-                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                                               for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule2
-            elif self.rts == RTS_CRS:
-                def sweet_rule2(model, i, h):
-                    if self.active[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                                               for j in model.J),
-                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                                               for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule2
-        elif self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-
-                def sweet_rule2(model, i, h):
-                    if self.active[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
-                                                               for j in model.J),
-                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
-                                                               for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule2
-            elif self.rts == RTS_CRS:
-
-                def sweet_rule2(model, i, h):
-                    if self.active[i][h]:
-                        if i == h:
-                            return Constraint.Skip
-                        return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J),
-                                          sum(model.beta[h, j] * self.x[i][j] for j in model.J))
-                    return Constraint.Skip
-
-                return sweet_rule2
-
-        raise ValueError("Undefined model parameters.")
-
-
-class CERZG2(CQRZG2):
-    """CERZ+G in iterative loop
-    """
-
-    def __init__(self, y, x, z, tau, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            active (float): violated concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, z, tau, cutactive, active, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-        return squared_objective_rule
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model, trans_list, to_2d_list
+from . import CQERZG1
+
+
+class CQRZG2(CQERZG1.CQRZG1):
+    """CQRZ+G in iterative loop
+    """
+
+    def __init__(self, y, x, z, tau, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CQRZ+G model
+
+        Args:
+            y (float): output variable. 
+            x (float): input variables.
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float): active concavity constraint.
+            active (float): violated concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.z = z
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.z[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.lamda = Var(self.__model__.K, doc='zvalue')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CQRZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._CQRZG1__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._CQRZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CQRZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CQRZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                                self.__model__.I,
+                                                rule=self.__sweet_rule2(),
+                                                doc='sweet spot-2 approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __sweet_rule2(self, ):
+        """Return the proper sweet spot (step2) approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def sweet_rule2(model, i, h):
+                    if self.active[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                                               for j in model.J),
+                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
+                                                               for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule2
+            elif self.rts == RTS_CRS:
+                def sweet_rule2(model, i, h):
+                    if self.active[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                                               for j in model.J),
+                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
+                                                               for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule2
+        elif self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+
+                def sweet_rule2(model, i, h):
+                    if self.active[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                                               for j in model.J),
+                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
+                                                               for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule2
+            elif self.rts == RTS_CRS:
+
+                def sweet_rule2(model, i, h):
+                    if self.active[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J),
+                                          sum(model.beta[h, j] * self.x[i][j] for j in model.J))
+                    return Constraint.Skip
+
+                return sweet_rule2
+
+        raise ValueError("Undefined model parameters.")
+
+
+class CERZG2(CQRZG2):
+    """CERZ+G in iterative loop
+    """
+
+    def __init__(self, y, x, z, tau, cutactive, active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable. 
+            x (float): input variables.
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            active (float): violated concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, z, tau, cutactive, active, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+        return squared_objective_rule
```

### Comparing `pytedea-0.0.1/pytedea/utils/interpolation.py` & `pytedea-0.0.2/pytedea/utils/interpolation.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# import dependencies
-import numpy as np
-from ..constant import FUN_PROD, FUN_COST
-from .tools import trans_list, to_2d_list
-
-
-def interpolation(alpha, beta, x, fun=FUN_PROD):
-    """Interpolate estimated function/frontier 
-
-    Args:
-        alpha (float): estimated alpha.
-        beta (float): estimated beta.
-        x (float): input variables.
-        fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-
-    Returns:
-        yat: interpolated frontier
-    """
-    x = np.array(to_2d_list(trans_list(x)))
-    n = len(x)
-    d = len(x[0])
-
-    if len(beta[0]) != d:
-        raise ValueError(
-            "The dimensions of x_test must be equal to those of x.")
-
-    if fun == FUN_PROD:
-        def fun_est(x):
-            return min(alpha + np.sum(beta[:, 0:d] * np.tile(x, (len(beta[:, 0:d]), 1)), axis=1))
-    elif fun == FUN_COST:
-        def fun_est(x):
-            return max(alpha + np.sum(beta[:, 0:d] * np.tile(x, (len(beta[:, 0:d]), 1)), axis=1))
-
-    yhat = np.zeros((n, 1))
-    for i in range(n):
-        yhat[i, :] = fun_est(x[i, :])
-
-    return yhat
+# import dependencies
+import numpy as np
+from ..constant import FUN_PROD, FUN_COST
+from .tools import trans_list, to_2d_list
+
+
+def interpolation(alpha, beta, x, fun=FUN_PROD):
+    """Interpolate estimated function/frontier 
+
+    Args:
+        alpha (float): estimated alpha.
+        beta (float): estimated beta.
+        x (float): input variables.
+        fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+
+    Returns:
+        yat: interpolated frontier
+    """
+    x = np.array(to_2d_list(trans_list(x)))
+    n = len(x)
+    d = len(x[0])
+
+    if len(beta[0]) != d:
+        raise ValueError(
+            "The dimensions of x_test must be equal to those of x.")
+
+    if fun == FUN_PROD:
+        def fun_est(x):
+            return min(alpha + np.sum(beta[:, 0:d] * np.tile(x, (len(beta[:, 0:d]), 1)), axis=1))
+    elif fun == FUN_COST:
+        def fun_est(x):
+            return max(alpha + np.sum(beta[:, 0:d] * np.tile(x, (len(beta[:, 0:d]), 1)), axis=1))
+
+    yhat = np.zeros((n, 1))
+    for i in range(n):
+        yhat[i, :] = fun_est(x[i, :])
+
+    return yhat
```

### Comparing `pytedea-0.0.1/pytedea/utils/sweet.py` & `pytedea-0.0.2/pytedea/utils/sweet.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/tools.py` & `pytedea-0.0.2/pytedea/utils/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     if type(li[0]) != list:
         rl = []
         for value in li:
             rl.append([value])
         return rl
     return li
 
-def assert_valid_dea(sent,data,baseindex,refindex):
+def assert_valid_deat(sent,data,baseindex,refindex):
     inputvars = sent.split('=')[0].strip(' ').split(' ')
     outputvars = sent.split('=')[1].strip(' ').split(' ')
 
     if type(baseindex) != type(None):
         varname1 = baseindex.split('=')[0]
         print(baseindex)
         varvalue1 = ast.literal_eval(baseindex.split('=')[1])
@@ -118,26 +118,26 @@
     if x.shape[0] != y.shape[0]:
         raise ValueError(
             "Number of DMUs must be the same in x and y.")
 
 
     return outputvars,inputvars,y, x,yref, xref
 
-def assert_valid_ddf(sent,gy,gx):
+def assert_valid_ddft(sent,gy,gx):
     inputvars = sent.split('=')[0].strip(' ').split(' ')
     outputvars = sent.split('=')[1].split(':')[0].strip(' ').split(' ')
 
     if len(outputvars) != len(gy):
         raise ValueError("Number of outputs must be the same in y and gy.")
     if len(inputvars) != len(gx):
         raise ValueError("Number of inputs must be the same in x and gx.")
 
     return outputvars,inputvars,gy,gx
 
-def assert_valid_ddf2(data,baseindex,refindex,outputvars,inputvars):
+def assert_valid_ddft2(data,baseindex,refindex,outputvars,inputvars):
 
     if type(baseindex) != type(None):
         varname1 = baseindex.split('=')[0]
         varvalue1 = ast.literal_eval(baseindex.split('=')[1])
         y, x = data.loc[data[varname1].isin(varvalue1), outputvars
         ], data.loc[data[varname1].isin(varvalue1), inputvars
         ]
@@ -152,14 +152,109 @@
         yref, xref = data.loc[data[varname].isin(varvalue), outputvars
                                             ], data.loc[data[varname].isin(varvalue), inputvars
                                             ]
     else:
         yref, xref = data.loc[:, outputvars], data.loc[:, inputvars]
     return y,x,yref,xref
 
+def assert_valid_dea(sent,data,baseindex,refindex):
+    inputvars = sent.split('=')[0].strip(' ').split(' ')
+    try:
+        outputvars = sent.split('=')[1].split(':')[0].strip(' ').split(' ')
+        unoutputvars = sent.split('=')[1].split(':')[1].strip(' ').split(' ')
+    except:
+        outputvars = sent.split('=')[1].strip(' ').split(' ')
+        unoutputvars = None
+
+    if type(baseindex) != type(None):
+        varname1 = baseindex.split('=')[0]
+        print(baseindex)
+        varvalue1 = ast.literal_eval(baseindex.split('=')[1])
+        y, x, b = data.loc[data[varname1].isin(varvalue1), outputvars
+        ], data.loc[data[varname1].isin(varvalue1), inputvars
+        ], data.loc[data[varname1].isin(varvalue1), unoutputvars
+        ]
+
+    else:
+        y, x, b = data.loc[:, outputvars
+                         ], data.loc[:, inputvars
+                         ], data.loc[:, unoutputvars]
+
+    # print(type(self.varname1),self.varvalue1,self.x,)
+    if type(refindex) != type(None):
+        varname = refindex.split('=')[0]
+        varvalue = ast.literal_eval(refindex.split('=')[1])
+
+        yref, xref, bref = data.loc[data[varname].isin(varvalue), outputvars
+        ], data.loc[data[varname].isin(varvalue), inputvars
+        ], data.loc[data[varname].isin(varvalue), unoutputvars]
+    else:
+        yref, xref, bref= data.loc[:, outputvars
+                               ], data.loc[:, inputvars
+                                  ], data.loc[:, unoutputvars]
+
+    if x.shape[0] != y.shape[0]:
+        raise ValueError(
+            "Number of DMUs must be the same in x and y.")
+    return outputvars,inputvars, unoutputvars,y, x,b ,yref, xref,bref
+
+def assert_valid_ddf(sent,gy,gx,gb):
+    inputvars = sent.split('=')[0].strip(' ').split(' ')
+    try:
+        outputvars = sent.split('=')[1].split(':')[0].strip(' ').split(' ')
+        unoutputvars = sent.split('=')[1].split(':')[1].strip(' ').split(' ')
+    except:
+        outputvars = sent.split('=')[1].strip(' ').split(' ')
+        unoutputvars = None
+
+    if len(outputvars) != len(gy):
+        raise ValueError("Number of outputs must be the same in y and gy.")
+    if len(inputvars) != len(gx):
+        raise ValueError("Number of inputs must be the same in x and gx.")
+    if len(unoutputvars) != len(gb):
+        raise ValueError("Number of undesirable outputs must be the same in b and gb.")
+    return outputvars,inputvars,unoutputvars,gy,gx,gb
+
+
+def assert_valid_ddf2(data, baseindex, refindex, outputvars, inputvars, unoutputvars):
+
+    if type(baseindex) != type(None):
+        varname1 = baseindex.split('=')[0]
+        print(baseindex)
+        varvalue1 = ast.literal_eval(baseindex.split('=')[1])
+        y, x, b = data.loc[data[varname1].isin(varvalue1), outputvars
+        ], data.loc[data[varname1].isin(varvalue1), inputvars
+        ], data.loc[data[varname1].isin(varvalue1), unoutputvars
+        ]
+
+    else:
+        y, x, b = data.loc[:, outputvars
+                         ], data.loc[:, inputvars
+                         ], data.loc[:, unoutputvars]
+
+    # print(type(self.varname1),self.varvalue1,self.x,)
+    if type(refindex) != type(None):
+        varname = refindex.split('=')[0]
+        varvalue = ast.literal_eval(refindex.split('=')[1])
+
+        yref, xref, bref = data.loc[data[varname].isin(varvalue), outputvars
+        ], data.loc[data[varname].isin(varvalue), inputvars
+        ], data.loc[data[varname].isin(varvalue), unoutputvars]
+    else:
+        yref, xref, bref= data.loc[:, outputvars
+                               ], data.loc[:, inputvars
+                                  ], data.loc[:, unoutputvars]
+
+    if x.shape[0] != y.shape[0]:
+        raise ValueError(
+            "Number of DMUs must be the same in x and y.")
+    return y, x,b ,yref, xref,bref
+
+
+
 
 def assert_valid_basic_data(y, x, z=None):
     y = trans_list(y)
     x = trans_list(x)
 
     y = to_1d_list(y)
     x = to_2d_list(x)
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSDDFG1.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSDDFG1.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import weakCNLSDDFZG1
-
-
-class weakCNLSDDFG1(weakCNLSDDFZG1.weakCNLSDDFZG1):
-    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            cutactive (float, optional): active concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b  = x, y, b
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCNLSDDFZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._weakCNLSDDFZG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCNLSDDFZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCNLSDDFZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSDDFZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.rts == RTS_VRS:
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == model.alpha[i] \
-                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                    - model.epsilon[i]
-            return regression_rule
-
-        elif self.rts == RTS_CRS:
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                    - model.epsilon[i]
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import weakCNLSDDFZG1
+
+
+class weakCNLSDDFG1(weakCNLSDDFZG1.weakCNLSDDFZG1):
+    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            cutactive (float, optional): active concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b  = x, y, b
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCNLSDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._weakCNLSDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCNLSDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCNLSDDFZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCNLSDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.rts == RTS_VRS:
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == model.alpha[i] \
+                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                    - model.epsilon[i]
+            return regression_rule
+
+        elif self.rts == RTS_CRS:
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                    - model.epsilon[i]
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSDDFG2.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSxG2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,127 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import weakCNLSDDFZG2,weakCNLSDDFG1,weakCNLSDDFZG1
-
-
-class weakCNLSDDFG2(weakCNLSDDFZG2.weakCNLSDDFZG2,weakCNLSDDFG1.weakCNLSDDFG1,weakCNLSDDFZG1.weakCNLSDDFZG1):
-    """initial Group-VC-added weakCNLSDDF (weakCNLSDDF+G) model
-    """
-
-    def __init__(self, y, x, b, cutactive, active, activeweak, gy=[1], gx=[1], gb=[1],  fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSDDF+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            cutactive (float, optional): active concavity constraint.
-            active (float or ndarray ): violated concavity constraint.
-            activeweak (float or ndarray ): violated concavity constraint for weak disposibility.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b = x, y, b
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = active
-        self.activeweak = activeweak
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-
-
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCNLSDDFZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCNLSDDFG1__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._weakCNLSDDFZG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCNLSDDFZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCNLSDDFZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSDDFZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.weakCNLSDDFZG2__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.weakCNLSDDFZG2__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import  trans_list, to_2d_list
+from . import weakCNLSxZG1,weakCNLSxZG2,weakCNLSxG1
+
+
+class weakCNLSxG2(weakCNLSxZG2.weakCNLSxZG2,weakCNLSxG1.weakCNLSxG1,weakCNLSxZG1.weakCNLSxZG1):
+    """weakCNLSx+G in iterative loop
+    """
+
+    def __init__(self, y, x, b, cutactive, active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSx+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            cutactive (float or list): active concavity constraint.
+            active (float or ndarray): violated concavity constraint.
+            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+        self.activeweak = to_2d_list(trans_list(activeweak))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.x)))
+        self.__model__.J = Set(initialize=range(len(self.y[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.delta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='delta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCNLSxZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._weakCNLSxG1__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCNLSxZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCNLSxZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCNLSxZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCNLSxZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCNLSxZG2__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCNLSxZG2__sweet_rule_weak2(),
+                                               doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def regression_rule(model, i):
+                    return self.x[i][0] == - model.alpha[i] \
+                        + sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        + model.epsilon[i]
+
+                return regression_rule
+            elif self.rts == RTS_CRS:
+
+                def regression_rule(model, i):
+                    return self.x[i][0] == sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        + model.epsilon[i]
+
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+
+            def regression_rule(model, i):
+                return log(self.x[i][0]) == - log(model.frontier[i] + 1) \
+                     + model.epsilon[i]
+
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSDDFZG1.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSDDFZG2.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSG1.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSG2.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSG2.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import weakCNLSZG2, weakCNLSG1,weakCNLSZG1
-
-
-class weakCNLSG2(weakCNLSG1.weakCNLSG1, weakCNLSZG2.weakCNLSZG2,weakCNLSZG1.weakCNLSZG1):
-    """weakCNLSZ+G in iterative loop
-    """
-
-    def __init__(self, y, x, b, cutactive,active,activeweak,cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            cutactive (list): active concavity constraint.
-            active (float or ndarray ): violated concavity constraint.
-            activeweak (float or ndarray ): violated concavity constraint for weak disposibility.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-        self.activeweak = to_2d_list(trans_list(activeweak))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCNLSZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCNLSG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCNLSZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCNLSZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCNLSZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSZG2__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSZG2__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model, trans_list, to_2d_list
+from . import weakCNLSZG2, weakCNLSG1,weakCNLSZG1
+
+
+class weakCNLSG2(weakCNLSG1.weakCNLSG1, weakCNLSZG2.weakCNLSZG2,weakCNLSZG1.weakCNLSZG1):
+    """weakCNLSZ+G in iterative loop
+    """
+
+    def __init__(self, y, x, b, cutactive,active,activeweak,cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            cutactive (list): active concavity constraint.
+            active (float or ndarray ): violated concavity constraint.
+            activeweak (float or ndarray ): violated concavity constraint for weak disposibility.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+        self.activeweak = to_2d_list(trans_list(activeweak))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCNLSZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._weakCNLSG1__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCNLSZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCNLSZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCNLSZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCNLSZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCNLSZG2__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCNLSZG2__sweet_rule_weak2(),
+                                               doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSZG1.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSZG2.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSbG1.py` & `pytedea-0.0.2/pytedea/utils/CNLSDDFG1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,134 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import weakCNLSbZG1
-
-
-class weakCNLSbG1(weakCNLSbZG1.weakCNLSbZG1):
-    """initial Group-VC-added weakCNLSb (weakCNLSb+G) model
-    """
-
-    def __init__(self, y, x, b, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSb+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.b)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.L = Set(initialize=range(len(self.y[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCNLSbZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCNLSbZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCNLSbZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCNLSbZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSbZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def regression_rule(model, i):
-                    return self.b[i] == -model.alpha[i] \
-                            - sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
-                            + model.epsilon[i]
-
-                return regression_rule
-            elif self.rts == RTS_CRS:
-
-                def regression_rule(model, i):
-                    return self.b[i] == -sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
-                            + model.epsilon[i]
-
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-
-            def regression_rule(model, i):
-                return log(self.b[i]) == - log(model.frontier[i] + 1) \
-                        + model.epsilon[i]
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import CNLSDDFZG1
+
+
+class CNLSDDFG1(CNLSDDFZG1.CNLSDDFZG1):
+    """initial Group-VC-added CNLSDDF (CNLSDDF+G) model
+    """
+
+    def __init__(self, y, x, b,  cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDF+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float,optional): undersiable variables.
+            cutactive (float, optional): active concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b = x, y, b
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+
+        if type(self.b) != type(None):
+            self.__model__.L = Set(initialize=range(len(self.b[0])))
+            self.__model__.delta = Var(
+                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
+
+
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CNLSDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._CNLSDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CNLSDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CNLSDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.rts == RTS_VRS:
+            if type(self.b) == type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - model.epsilon[i]
+                return regression_rule
+
+            elif type(self.b) != type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        - model.epsilon[i]
+                return regression_rule
+
+
+        elif self.rts == RTS_CRS:
+            if type(self.b) == type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - model.epsilon[i]
+                return regression_rule
+
+
+            elif type(self.b) != type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        - model.epsilon[i]
+                return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+
+
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSbG2.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSbG1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,115 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import  trans_list, to_2d_list
-from . import weakCNLSbZG2, weakCNLSbZG1, weakCNLSbG1
-
-
-class weakCNLSbG2(weakCNLSbZG2.weakCNLSbZG2,weakCNLSbG1.weakCNLSbG1,weakCNLSbZG1.weakCNLSbZG1):
-    """weakCNLSb+G in iterative loop
-    """
-
-    def __init__(self, y, x, b, cutactive,active,activeweak,cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSb+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            cutactive (list): active concavity constraint.
-            active (float or ndarray ): violated concavity constraint.
-            activeweak (float or ndarray ): violated concavity constraint for weak disposibility.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-        self.activeweak = to_2d_list(trans_list(activeweak))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.b)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.L = Set(initialize=range(len(self.y[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCNLSbZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCNLSbG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCNLSbZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCNLSbZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCNLSbZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSbZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSbZG2__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSbZG2__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import weakCNLSbZG1
+
+
+class weakCNLSbG1(weakCNLSbZG1.weakCNLSbZG1):
+    """initial Group-VC-added weakCNLSb (weakCNLSb+G) model
+    """
+
+    def __init__(self, y, x, b, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSb+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.b)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.L = Set(initialize=range(len(self.y[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCNLSbZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCNLSbZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCNLSbZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCNLSbZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCNLSbZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def regression_rule(model, i):
+                    return self.b[i] == -model.alpha[i] \
+                            - sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
+                            + model.epsilon[i]
+
+                return regression_rule
+            elif self.rts == RTS_CRS:
+
+                def regression_rule(model, i):
+                    return self.b[i] == -sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
+                            + model.epsilon[i]
+
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+
+            def regression_rule(model, i):
+                return log(self.b[i]) == - log(model.frontier[i] + 1) \
+                        + model.epsilon[i]
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSbZG1.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSbZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSbZG2.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSbZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSxG1.py` & `pytedea-0.0.2/pytedea/utils/CNLSG1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,105 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import weakCNLSxZG1
-
-
-class weakCNLSxG1(weakCNLSxZG1.weakCNLSxZG1):
-    """initial Group-VC-added weakCNLSx (weakCNLSx+G) model
-    """
-
-    def __init__(self, y, x, b, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSx+G model
-
-        Args:
-            y (ndarray): output variable.
-            x (ndarray): input variables.
-            b (ndarray): undersiable variables.
-            cutactive (float or ndarray): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.x))) #i行
-        self.__model__.J = Set(initialize=range(len(self.y[0]))) #j个y
-        self.__model__.L = Set(initialize=range(len(self.b[0])))  # l个b
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.delta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='delta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCNLSxZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCNLSxZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCNLSxZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCNLSxZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSxZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def regression_rule(model, i):
-                    return self.x[i][0] == - model.alpha[i] \
-                        + sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        + model.epsilon[i]
-
-                return regression_rule
-            elif self.rts == RTS_CRS:
-
-                def regression_rule(model, i):
-                    return self.x[i][0] == sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        + model.epsilon[i]
-
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-
-            def regression_rule(model, i):
-                return log(self.x[i][0]) == - log(model.frontier[i] + 1) \
-                     + model.epsilon[i]
-
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+
+from . import CNLSZG1
+
+
+class CNLSG1(CNLSZG1.CNLSZG1):
+    """initial Group-VC-added CNLS (CNLS+G) model
+    """
+
+    def __init__(self, y, x, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CNLS+G model 1
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CNLSZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._CNLSZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CNLSZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CNLSZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+                def regression_rule(model, i):
+                    return self.y[i] == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - model.epsilon[i]
+
+                return regression_rule
+            elif self.rts == RTS_CRS:
+                def regression_rule(model, i):
+                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - model.epsilon[i]
+
+                return regression_rule
+        elif self.cet == CET_MULT:
+
+            def regression_rule(model, i):
+                return log(
+                    self.y[i]) == log(model.frontier[i] + 1) - model.epsilon[i]
+
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSxG2.py` & `pytedea-0.0.2/pytedea/utils/weakCQERDDFG1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,127 +1,151 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import  trans_list, to_2d_list
-from . import weakCNLSxZG1,weakCNLSxZG2,weakCNLSxG1
-
-
-class weakCNLSxG2(weakCNLSxZG2.weakCNLSxZG2,weakCNLSxG1.weakCNLSxG1,weakCNLSxZG1.weakCNLSxZG1):
-    """weakCNLSx+G in iterative loop
-    """
-
-    def __init__(self, y, x, b, cutactive, active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSx+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            cutactive (float or list): active concavity constraint.
-            active (float or ndarray): violated concavity constraint.
-            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-        self.activeweak = to_2d_list(trans_list(activeweak))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.x)))
-        self.__model__.J = Set(initialize=range(len(self.y[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.delta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='delta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCNLSxZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCNLSxG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCNLSxZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCNLSxZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCNLSxZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSxZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSxZG2__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCNLSxZG2__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def regression_rule(model, i):
-                    return self.x[i][0] == - model.alpha[i] \
-                        + sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        + model.epsilon[i]
-
-                return regression_rule
-            elif self.rts == RTS_CRS:
-
-                def regression_rule(model, i):
-                    return self.x[i][0] == sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        + model.epsilon[i]
-
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-
-            def regression_rule(model, i):
-                return log(self.x[i][0]) == - log(model.frontier[i] + 1) \
-                     + model.epsilon[i]
-
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import weakCQERDDFZG1
+
+class weakCQRDDFG1(weakCQERDDFZG1.weakCQRDDFZG1):
+    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            tau (float): quantile.
+            cutactive (float, optional): active concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x, self.y, self.b = x, y, b
+        self.gy, self.gx, self.gb = gy, gx, gb
+        self.tau = tau
+
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.K,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._weakCQRDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                       rule=self._weakCQRDDFZG1__disposability_rule(),
+                                                       doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.rts == RTS_VRS:
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == model.alpha[i] \
+                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                    - model.epsilon_minus[i] + model.epsilon_plus[i]
+
+            return regression_rule
+
+
+        elif self.rts == RTS_CRS:
+            def regression_rule(model, i):
+                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                    - model.epsilon_minus[i] + model.epsilon_plus[i]
+
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+
+class weakCERDDFG1(weakCQRDDFG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b,  tau, cutactive, gy, gx, gb, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSxZG1.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSxZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/weakCNLSxZG2.py` & `pytedea-0.0.2/pytedea/utils/weakCNLSxZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERDDFG1.py` & `pytedea-0.0.2/pytedea/utils/weakCQERG1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,151 +1,148 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import weakCQERDDFZG1
-
-class weakCQRDDFG1(weakCQERDDFZG1.weakCQRDDFZG1):
-    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            tau (float): quantile.
-            cutactive (float, optional): active concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x, self.y, self.b = x, y, b
-        self.gy, self.gx, self.gb = gy, gx, gb
-        self.tau = tau
-
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.K,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCQRDDFZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._weakCQRDDFZG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCQRDDFZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                       rule=self._weakCQRDDFZG1__disposability_rule(),
-                                                       doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRDDFZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.rts == RTS_VRS:
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == model.alpha[i] \
-                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                    - model.epsilon_minus[i] + model.epsilon_plus[i]
-
-            return regression_rule
-
-
-        elif self.rts == RTS_CRS:
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                    - model.epsilon_minus[i] + model.epsilon_plus[i]
-
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-
-class weakCERDDFG1(weakCQRDDFG1):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b,  tau, cutactive, gy, gx, gb, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from . import weakCQERZG1
+
+class weakCQRG1(weakCQERZG1.weakCQRZG1):
+    """initial Group-VC-added CQR (CQR+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCQR+G model
+
+        Args:
+            y (ndarray): output variable.
+            x (ndarray): input variables.
+            b (ndarray): undersiable variables.
+            tau (float): quantile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.y, self.x, self.b = y, x, b
+
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCQRZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRZG1__afriat_rule(),
+                                                doc='elementary afriat inequality')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCQRZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def regression_rule(model, i):
+                    return self.y[i] == model.alpha[i] \
+                            + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                             + model.epsilon_plus[i] - model.epsilon_minus[i]
+                return regression_rule
+
+            elif self.rts == RTS_CRS:
+                def regression_rule(model, i):
+                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                             + model.epsilon_plus[i] - model.epsilon_minus[i]
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+            def regression_rule(model, i):
+                return log(self.y[i]) == log(model.frontier[i] + 1) \
+                            + model.epsilon_plus[i] - model.epsilon_minus[i]
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+
+
+class weakCERG1(weakCQRG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable. 
+            x (float): input variables.
+            b (float): undersiable variables
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, tau, cutactive, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERDDFG2.py` & `pytedea-0.0.2/pytedea/utils/weakCQERxG1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,138 +1,152 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import weakCQERDDFZG1,weakCQERDDFZG2,weakCQERDDFG1
-
-
-class weakCQRDDFG2(weakCQERDDFZG2.weakCQRDDFZG2,weakCQERDDFG1.weakCQRDDFG1,weakCQERDDFZG1.weakCQRDDFZG1):
-    """initial Group-VC-added weakCQRDDFZ (weakCQRDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive, active, activeweak, gy=[1], gx=[1], gb=[1],  fun=FUN_PROD, rts=RTS_VRS):
-        """weakCQRDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            tau (float): quantile.
-            cutactive (float, optional): active concavity constraint.
-            active (float or ndarray ): violated concavity constraint.
-            activeweak (float or ndarray ): violated concavity constraint for weak disposibility.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b = x, y, b
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.fun = fun
-        self.rts = rts
-        self.tau = tau
-
-        self.cutactive = cutactive
-        self.active = active
-        self.activeweak = activeweak
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCQRDDFZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCQERDDFG1__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._weakCQRDDFZG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCQRDDFZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCQRDDFZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRDDFZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRDDFZG2__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRDDFZG2__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-class weakCERDDFG2(weakCQRDDFG2):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b,  tau, cutactive,active, activeweak, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, tau, cutactive, active, activeweak, gy,gx,gb, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import weakCQERxZG1
+
+
+class weakCQRxG1(weakCQERxZG1.weakCQRxZG1):
+    """initial Group-VC-added weakCNLSxZ (weakCNLSxZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSxZ+G model
+
+        Args:
+            y (ndarray): output variable.
+            x (ndarray): input variables.
+            b (ndarray): undersiable variables.
+            tau (float): quantile.
+            cutactive (float or ndarray): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.x))) #i行
+        self.__model__.J = Set(initialize=range(len(self.y[0]))) #j个y
+        self.__model__.L = Set(initialize=range(len(self.b[0])))  # l个b
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.delta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='delta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRxZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCQRxZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRxZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCQRxZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRxZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def regression_rule(model, i):
+                    return self.x[i][0] == - model.alpha[i] \
+                        + sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        + model.epsilon_minus[i] - model.epsilon_plus[i]
+
+                return regression_rule
+            elif self.rts == RTS_CRS:
+
+                def regression_rule(model, i):
+                    return self.x[i][0] == sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        + model.epsilon_minus[i] - model.epsilon_plus[i]
+
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+
+            def regression_rule(model, i):
+                return log(self.x[i][0]) == - log(model.frontier[i] + 1) \
+                    + model.epsilon_minus[i] - model.epsilon_plus[i]
+
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+
+class weakCERxG1(weakCQRxG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b,  tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b,  tau, cutactive, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERDDFZG1.py` & `pytedea-0.0.2/pytedea/utils/weakCQERxZG1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,315 +1,311 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-
-
-class weakCQRDDFZG1:
-    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CNLSDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            z (float): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float, optional): active concavity constraint.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b,self.z = x, y, b, z
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.tau = tau
-
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-
-        # Initialize the set of z
-        self.__model__.M = Set(initialize=range(len(self.z[0])))
-        # Initialize the variables for z variable
-        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
-
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self.__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self.__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self.__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        # TODO(error/warning handling): Check problem status after optimization
-        self.problem_status, self.optimization_status = optimize_model(
-            self.__model__, email, CET_ADDI, solver)
-
-    def __objective_rule(self):
-        """Return the proper objective function"""
-
-        def objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
-        return objective_rule
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.rts == RTS_VRS:
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == model.alpha[i] \
-                    + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                    - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                    - model.epsilon_minus[i] + model.epsilon_plus[i]
-
-            return regression_rule
-
-
-        elif self.rts == RTS_CRS:
-            def regression_rule(model, i):
-                return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
-                    == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                    + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                    - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
-                    - model.epsilon_minus[i] + model.epsilon_plus[i]
-
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __translation_property(self):
-        """Return the proper translation property"""
-        def translation_rule(model, i):
-            return sum(model.beta[i, j] * self.gx[j] for j in model.J) \
-                + sum(model.gamma[i, k] * self.gy[k] for k in model.K) \
-                + sum(model.delta[i, l] * self.gb[l] for l in model.L) == 1
-
-        return translation_rule
-
-    def __afriat_rule(self):
-        """Return the proper elementary Afriat approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def afriat_rule(model, i):
-                return __operator(
-                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
-                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                    model.alpha[self.__model__.I.nextw(i)] \
-                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
-                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
-                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
-
-            return afriat_rule
-
-        elif self.rts == RTS_CRS:
-            def afriat_rule(model, i):
-                return __operator(sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
-                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
-                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
-                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
-
-            return afriat_rule
-        raise ValueError("Undefined model parameters.")
-
-    def __disposability_rule(self):
-        """Return the proper elementary weak disposability constraint"""
-        if self.rts == RTS_VRS:
-            def disposability_rule(model, i):
-                return model.alpha[self.__model__.I.nextw(i)] \
-                    + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
-            return disposability_rule
-
-        elif self.rts == RTS_CRS:
-            def disposability_rule(model, i):
-                return sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
-            return disposability_rule
-        raise ValueError("Undefined model parameters.")
-
-
-    def __sweet_rule(self ):
-        """Return the proper sweet spot approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                      model.alpha[h] \
-                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
-                return Constraint.Skip
-
-            return sweet_rule
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                       sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
-                return Constraint.Skip
-
-            return sweet_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def get_alpha(self):
-        """Return alpha value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        alpha = list(self.__model__.alpha[:].value)
-        return np.asarray(alpha)
-
-    def get_beta(self):
-        """Return beta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
-        return beta.to_numpy()
-
-    def get_delta(self):
-        """Return delta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
-                                                           list(self.__model__.delta[:, :].value))])
-        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
-        delta = delta.pivot(index='Name', columns='Key', values='Value')
-        return delta.to_numpy()
-
-    def get_gamma(self):
-        """Return delta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
-                                                           list(self.__model__.gamma[:, :].value))])
-        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
-        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
-        return gamma.to_numpy()
-
-
-class weakCERDDFZG1(weakCQRDDFZG1):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, z, tau, cutactive, gy, gx, gb, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+
+
+class weakCQRxZG1:
+    """initial Group-VC-added weakCNLSxZ (weakCNLSxZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSxZ+G model
+
+        Args:
+            y (ndarray): output variable.
+            x (ndarray): input variables.
+            b (ndarray): undersiable variables.
+            z (ndarray, optional): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float or ndarray): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.z = z
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.x))) #i行
+        self.__model__.J = Set(initialize=range(len(self.y[0]))) #j个y
+        self.__model__.L = Set(initialize=range(len(self.b[0])))  # l个b
+        self.__model__.K = Set(initialize=range(len(self.z[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.delta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='delta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self.__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self.__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self.__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self.__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        # TODO(error/warning handling): Check problem status after optimization
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, email, self.cet, solver)
+
+    def __objective_rule(self):
+        """Return the proper objective function"""
+
+        def objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
+        return objective_rule
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def regression_rule(model, i):
+                    return self.x[i][0] == - model.alpha[i] \
+                        + sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                        + model.epsilon_minus[i] - model.epsilon_plus[i]
+
+                return regression_rule
+            elif self.rts == RTS_CRS:
+
+                def regression_rule(model, i):
+                    return self.x[i][0] == sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                        + model.epsilon_minus[i] - model.epsilon_plus[i]
+
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+
+            def regression_rule(model, i):
+                return log(self.x[i][0]) == - log(model.frontier[i] + 1) \
+                    + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                    + model.epsilon_minus[i] - model.epsilon_plus[i]
+
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __log_rule(self):
+        """Return the proper log constraint"""
+        if self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+
+                def log_rule(model, i):
+                    return model.frontier[i] == model.alpha[i] - sum(
+                        model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
+
+                return log_rule
+            elif self.rts == RTS_CRS:
+
+                def log_rule(model, i):
+                    return model.frontier[i] == - sum(
+                        model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
+
+                return log_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __afriat_rule(self):
+        """Return the proper elementary Afriat approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def afriat_rule(model, i):
+                return __operator(
+                    model.alpha[i] + sum(model.delta[i, l] * self.b[i][l]for l in model.L) \
+                                   - sum(model.gamma[i, j] * self.y[i][j] for j in model.J),
+                    model.alpha[self.__model__.I.nextw(i)] \
+                           + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l]for l in model.L) \
+                        - sum(model.gamma[self.__model__.I.nextw(i), j] * self.y[i][j] for j in model.J))
+
+            return afriat_rule
+
+        elif self.rts == RTS_CRS:
+            def afriat_rule(model, i):
+                return __operator(
+                    sum(model.delta[i, l] * self.b[i][l]for l in model.L) \
+                                   - sum(model.gamma[i, j] * self.y[i][j] for j in model.J),
+                    sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l]for l in model.L) \
+                        - sum(model.gamma[self.__model__.I.nextw(i), j] * self.y[i][j] for j in model.J))
+
+            return afriat_rule
+        raise ValueError("Undefined model parameters.")
+
+    def __disposability_rule(self):
+        """Return the proper elementary weak disposability constraint"""
+        if self.rts == RTS_VRS:
+            def disposability_rule(model, i):
+                return model.alpha[self.__model__.I.nextw(i)] \
+                    + sum(self.x[i])  >= 0
+
+            return disposability_rule
+
+        elif self.rts == RTS_CRS:
+            def disposability_rule(model, i):
+                return sum(self.x[i])  >= 0
+            return disposability_rule
+        raise ValueError("Undefined model parameters.")
+
+
+    def __sweet_rule(self ):
+        """Return the proper sweet spot approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      - sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
+                                      model.alpha[h] \
+                                      - sum(model.gamma[h, j] * self.y[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
+                return Constraint.Skip
+
+            return sweet_rule
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(- sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
+                                      - sum(model.gamma[h, j] * self.y[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
+                return Constraint.Skip
+
+            return sweet_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def get_alpha(self):
+        """Return alpha value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        alpha = list(self.__model__.alpha[:].value)
+        return np.asarray(alpha)
+
+    def get_delta(self):
+        """Return delta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
+                                                          list(self.__model__.delta[:, :].value))])
+        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
+        delta = delta.pivot(index='Name', columns='Key', values='Value')
+        return delta.to_numpy()
+
+    def get_gamma(self):
+        """Return gamma value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
+                                                           list(self.__model__.gamma[:, :].value))])
+        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
+        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
+        return gamma.to_numpy()
+
+
+class weakCERxZG1(weakCQRxZG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, z, tau, cutactive, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERDDFZG2.py` & `pytedea-0.0.2/pytedea/utils/CQERDDFZG2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,213 +1,184 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-from . import weakCQERDDFZG1
-
-
-class weakCQRDDFZG2(weakCQERDDFZG1.weakCQRDDFZG1):
-    """initial Group-VC-added weakCQRDDFZ (weakCQRDDFZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, active, activeweak, gy=[1], gx=[1], gb=[1],  fun=FUN_PROD, rts=RTS_VRS):
-        """weakCQRDDFZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float, optional): active concavity constraint.
-            active (float or ndarray ): violated concavity constraint.
-            activeweak (float or ndarray ): violated concavity constraint for weak disposibility.
-            gy (list, optional): output directional vector. Defaults to [1].
-            gx (list, optional): input directional vector. Defaults to [1].
-            gb (list, optional): undesirable output directional vector. Defaults to [1].
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x,self.y,self.b,self.z = x, y, b, z
-        self.gy, self.gx, self.gb = gy,gx,gb
-        self.fun = fun
-        self.rts = rts
-        self.tau = tau
-
-        self.cutactive = cutactive
-        self.active = active
-        self.activeweak = activeweak
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.K = Set(initialize=range(len(self.y[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                  self.__model__.K,
-                                  bounds=(0.0, None),
-                                  doc='gamma')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-
-        # Initialize the set of z
-        self.__model__.M = Set(initialize=range(len(self.z[0])))
-        # Initialize the variables for z variable
-        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCQRDDFZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCQRDDFZG1__regression_rule(),
-                                                    doc='regression equation')
-        self.__model__.translation_rule = Constraint(self.__model__.I,
-                                                     rule=self._weakCQRDDFZG1__translation_property(),
-                                                     doc='translation property')
-
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCQRDDFZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCQRDDFZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRDDFZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-    def __sweet_rule2(self):
-        """Return the proper sweet spot (step2) approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule2(model, i, h):
-                if self.active[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                      model.alpha[h] \
-                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
-                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
-                return Constraint.Skip
-
-            return sweet_rule2
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule2(model, i, h):
-                if self.active[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
-                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
-                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
-                return Constraint.Skip
-
-            return sweet_rule2
-
-        raise ValueError("Undefined model parameters.")
-
-    def __sweet_rule_weak2(self, ):
-        """Return the proper sweet spot (step2) approach constraint for weak dis"""
-
-        if self.rts == RTS_VRS:
-            def sweet_rule_weak2(model, i, h):
-                if self.activeweak[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return model.alpha[i] + sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
-                return Constraint.Skip
-
-            return sweet_rule_weak2
-
-        elif self.rts == RTS_CRS:
-            def sweet_rule_weak2(model, i, h):
-                if self.activeweak[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return  sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
-                return Constraint.Skip
-            return sweet_rule_weak2
-
-        raise ValueError("Undefined model parameters.")
-
-
-
-class weakCERDDFZG2(weakCQRDDFZG2):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive,active, activeweak, gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, z, tau, cutactive, active, activeweak, gy,gx,gb, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import CQERDDFZG1
+
+class CQRDDFZG2(CQERDDFZG1.CQRDDFZG1):
+    """initial Group-VC-added weakCNLSDDFZ (weakCNLSDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive,active,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables.
+            z (float): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float, optional): active concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b,self.z = x, y, b, z
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.tau = tau
+
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = active
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+
+
+        if type(self.b) != type(None):
+            self.__model__.L = Set(initialize=range(len(self.b[0])))
+            self.__model__.delta = Var(
+                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+
+        # Initialize the set of z
+        self.__model__.M = Set(initialize=range(len(self.z[0])))
+        # Initialize the variables for z variable
+        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
+
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._CQRDDFZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._CQRDDFZG1__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self._CQRDDFZG1__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._CQRDDFZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._CQRDDFZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._CQRDDFZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def __sweet_rule2(self, ):
+        """Return the proper sweet spot (step2) approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
+                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
+                return Constraint.Skip
+
+            return sweet_rule2
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L)
+                                      - sum(model.gamma[h, k] * self.y[i][k] for k in model.K))
+                return Constraint.Skip
+
+            return sweet_rule2
+
+        raise ValueError("Undefined model parameters.")
+
+
+
+
+class CERDDFZG2(CQRDDFZG2):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive,active, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float, optional): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, z, tau, cutactive,active, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERG1.py` & `pytedea-0.0.2/pytedea/utils/weakCQERbG1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,148 +1,149 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from . import weakCQERZG1
-
-class weakCQRG1(weakCQERZG1.weakCQRZG1):
-    """initial Group-VC-added CQR (CQR+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCQR+G model
-
-        Args:
-            y (ndarray): output variable.
-            x (ndarray): input variables.
-            b (ndarray): undersiable variables.
-            tau (float): quantile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.y, self.x, self.b = y, x, b
-
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCQRZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCQRZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCQRZG1__afriat_rule(),
-                                                doc='elementary afriat inequality')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCQRZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def regression_rule(model, i):
-                    return self.y[i] == model.alpha[i] \
-                            + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                             + model.epsilon_plus[i] - model.epsilon_minus[i]
-                return regression_rule
-
-            elif self.rts == RTS_CRS:
-                def regression_rule(model, i):
-                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                             + model.epsilon_plus[i] - model.epsilon_minus[i]
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-            def regression_rule(model, i):
-                return log(self.y[i]) == log(model.frontier[i] + 1) \
-                            + model.epsilon_plus[i] - model.epsilon_minus[i]
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-
-
-class weakCERG1(weakCQRG1):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            b (float): undersiable variables
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, tau, cutactive, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+from . import weakCQERbZG1
+
+
+class weakCQRbG1(weakCQERbZG1.weakCQRbZG1):
+    """initial Group-VC-added weakCNLSb (weakCNLSb+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSb+G model
+
+        Args:
+            y (ndarray): output variable.
+            x (ndarray): input variables.
+            b (ndarray): undersiable variables.
+            tau (float): quantile.
+            cutactive (float or ndarray): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+
+        self.tau = tau
+
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.b))) #i行
+        self.__model__.J = Set(initialize=range(len(self.x[0]))) #j个x
+        self.__model__.L = Set(initialize=range(len(self.y[0])))  # l个y
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRbZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCQRbZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRbZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCQRbZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRbZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+                def regression_rule(model, i):
+                    return self.b[i] == -model.alpha[i] \
+                        - sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
+                        + model.epsilon_minus[i] - model.epsilon_plus[i]
+                return regression_rule
+
+            elif self.rts == RTS_CRS:
+                def regression_rule(model, i):
+                    return self.b[i] == -sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
+                        + model.epsilon_minus[i] - model.epsilon_plus[i]
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+            def regression_rule(model, i):
+                return log(self.b[i]) == - log(model.frontier[i] + 1) \
+                    + model.epsilon_minus[i] - model.epsilon_plus[i]
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+
+class weakCERbG1(weakCQRbG1):
+    """initial Group-VC-added CERZ (CER+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, tau, cutactive, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERG2.py` & `pytedea-0.0.2/pytedea/utils/weakCQERbG2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,130 +1,133 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import weakCQERZG1,weakCQERZG2,weakCQERG1
-
-
-class weakCQRG2(weakCQERZG2.weakCQRZG2,weakCQERG1.weakCQRG1,weakCQERZG1.weakCQRZG1):
-    """weakCQR+G in iterative loop
-    """
-
-    def __init__(self, y, x, b, tau, cutactive, active, activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCQRZ+G model
-
-        Args:
-            y (ndarray): output variable.
-            x (ndarray): input variables.
-            b (ndarray): undersiable variables.
-            tau (float): quantile.
-            cutactive (float or list): active concavity constraint.
-            active (float or ndarray): violated concavity constraint.
-            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-        self.activeweak = to_2d_list(trans_list(activeweak))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCQRZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCQRG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCQRZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCQRZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                       rule=self._weakCQRZG1__disposability_rule(),
-                                                       doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                                self.__model__.I,
-                                                rule=self._weakCQRZG2__sweet_rule2(),
-                                                doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                                     self.__model__.I,
-                                                     rule=self._weakCQRZG2__sweet_rule_weak2(),
-                                                     doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-class weakCERG2(weakCQRG2):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, tau, cutactive, active,activeweak,cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model, trans_list, to_2d_list
+from . import weakCQERbZG1,weakCQERbZG2,weakCQERbG1
+
+
+class weakCQRbG2(weakCQERbZG2.weakCQRbZG2,weakCQERbG1.weakCQRbG1,weakCQERbZG1.weakCQRbZG1,):
+    """weakCNLSb+G in iterative loop
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, active, activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSb+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            tau (float): quantile.
+            cutactive (float or list): active concavity constraint.
+            active (float or ndarray): violated concavity constraint.
+            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+        self.activeweak = to_2d_list(trans_list(activeweak))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.b)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.L = Set(initialize=range(len(self.y[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRbZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._weakCQRbG1__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCQRbZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRbZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCQRbZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRbZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRbZG2__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRbZG2__sweet_rule_weak2(),
+                                               doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+class weakCERbG2(weakCQRbG2):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, tau, cutactive, active,activeweak, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERZG1.py` & `pytedea-0.0.2/pytedea/utils/weakCQERbZG1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,297 +1,301 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-
-
-class weakCQRZG1:
-    """initial Group-VC-added CQRZ (CQRZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCQRZ+G model
-
-        Args:
-            y (ndarray): output variable.
-            x (ndarray): input variables.
-            b (ndarray): undersiable variables.
-            z (ndarray): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.y, self.x, self.b, self.z = y, x, b, z
-
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-
-        self.__model__.K = Set(initialize=range(len(self.z[0])))
-        self.__model__.lamda = Var(self.__model__.K, doc='z coefficient')
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self.__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self.__afriat_rule(),
-                                                doc='elementary afriat inequality')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self.__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        # TODO(error/warning handling): Check problem status after optimization
-        self.problem_status, self.optimization_status = optimize_model(
-            self.__model__, email, self.cet, solver)
-
-    def __objective_rule(self):
-        """Return the proper objective function"""
-
-        def objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
-        return objective_rule
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def regression_rule(model, i):
-                    return self.y[i] == model.alpha[i] \
-                            + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                            - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                            + model.epsilon_plus[i] - model.epsilon_minus[i]
-                return regression_rule
-
-            elif self.rts == RTS_CRS:
-                def regression_rule(model, i):
-                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                            - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                            + model.epsilon_plus[i] - model.epsilon_minus[i]
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-
-            def regression_rule(model, i):
-                return log(self.y[i]) == log(model.frontier[i] + 1) \
-                        - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                        + model.epsilon_plus[i] - model.epsilon_minus[i]
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __log_rule(self):
-        """Return the proper log constraint"""
-        if self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-
-                def log_rule(model, i):
-                    return model.frontier[i] == model.alpha[i] + sum(
-                        model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
-                return log_rule
-            elif self.rts == RTS_CRS:
-
-                def log_rule(model, i):
-                    return model.frontier[i] == sum(
-                        model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
-                return log_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __afriat_rule(self):
-        """Return the proper elementary Afriat approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-            def afriat_rule(model, i):
-                return __operator(
-                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
-                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                    model.alpha[self.__model__.I.nextw(i)] \
-                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
-                        + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L))
-            return afriat_rule
-
-        elif self.rts == RTS_CRS:
-            def afriat_rule(model, i):
-                return __operator(
-                    sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                           + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) \
-                            + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L))
-            return afriat_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __disposability_rule(self):
-        """Return the proper elementary weak disposability constraint"""
-        if self.rts == RTS_VRS:
-            def disposability_rule(model, i):
-                return model.alpha[self.__model__.I.nextw(i)] \
-                    + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
-            return disposability_rule
-
-        elif self.rts == RTS_CRS:
-            def disposability_rule(model, i):
-                return sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
-            return disposability_rule
-        raise ValueError("Undefined model parameters.")
-
-    def __sweet_rule(self, ):
-        """Return the proper sweet spot approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J)
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                                      model.alpha[h] \
-                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J)
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
-                return Constraint.Skip
-            return sweet_rule
-
-        elif self.rts == RTS_CRS:
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator( sum(model.beta[i, j] * self.x[i][j] for j in model.J)
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J)
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
-                return Constraint.Skip
-            return sweet_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def get_alpha(self):
-        """Return alpha value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        alpha = list(self.__model__.alpha[:].value)
-        return np.asarray(alpha)
-
-    def get_beta(self):
-        """Return beta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
-        return beta.to_numpy()
-
-    def get_delta(self):
-        """Return delta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
-                                                           list(self.__model__.delta[:, :].value))])
-        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
-        delta = delta.pivot(index='Name', columns='Key', values='Value')
-        return delta.to_numpy()
-
-class weakCERZG1(weakCQRZG1):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            b (float): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, z, tau, cutactive, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+
+
+class weakCQRbZG1:
+    """initial Group-VC-added weakCNLSbZ (weakCNLSbZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSbZ+G model
+
+        Args:
+            y (ndarray): output variable.
+            x (ndarray): input variables.
+            b (ndarray): undersiable variables.
+            z (ndarray, optional): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float or ndarray): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.z = z
+        self.tau = tau
+
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.b))) #i行
+        self.__model__.J = Set(initialize=range(len(self.x[0]))) #j个x
+        self.__model__.L = Set(initialize=range(len(self.y[0])))  # l个y
+        self.__model__.K = Set(initialize=range(len(self.z[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self.__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self.__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self.__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self.__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        # TODO(error/warning handling): Check problem status after optimization
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, email, self.cet, solver)
+
+    def __objective_rule(self):
+        """Return the proper objective function"""
+
+        def objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
+        return objective_rule
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+                def regression_rule(model, i):
+                    return self.b[i] == -model.alpha[i] \
+                        - sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
+                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                        + model.epsilon_minus[i] - model.epsilon_plus[i]
+                return regression_rule
+
+            elif self.rts == RTS_CRS:
+                def regression_rule(model, i):
+                    return self.b[i] == -sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
+                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                        + model.epsilon_minus[i] - model.epsilon_plus[i]
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+            def regression_rule(model, i):
+                return log(self.b[i]) == - log(model.frontier[i] + 1) \
+                    + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                    + model.epsilon_minus[i] - model.epsilon_plus[i]
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __log_rule(self):
+        """Return the proper log constraint"""
+        if self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+                def log_rule(model, i):
+                    return model.frontier[i] == model.alpha[i] + sum(
+                        model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            - sum(model.gamma[i, l] * self.y[i][l] for l in model.L) - 1
+                return log_rule
+
+            elif self.rts == RTS_CRS:
+                def log_rule(model, i):
+                    return model.frontier[i] == + sum(
+                        model.beta[i, j] * self.x[i][j] for j in model.J) \
+                            - sum(model.gamma[i, l] * self.y[i][l] for l in model.L) - 1
+                return log_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __afriat_rule(self):
+        """Return the proper elementary Afriat approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+            def afriat_rule(model, i):
+                return __operator(
+                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
+                                   - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
+                    model.alpha[self.__model__.I.nextw(i)] \
+                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
+                        - sum(model.gamma[self.__model__.I.nextw(i), l] * self.y[i][l] for l in model.L))
+            return afriat_rule
+
+        elif self.rts == RTS_CRS:
+            def afriat_rule(model, i):
+                return __operator(
+                    sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                           - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
+                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) \
+                            - sum(model.gamma[self.__model__.I.nextw(i), l] * self.y[i][l] for l in model.L))
+            return afriat_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __disposability_rule(self):
+        """Return the proper elementary weak disposability constraint"""
+        if self.rts == RTS_VRS:
+            def disposability_rule(model, i):
+                return model.alpha[self.__model__.I.nextw(i)] \
+                    + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
+            return disposability_rule
+
+        elif self.rts == RTS_CRS:
+            def disposability_rule(model, i):
+                return sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
+            return disposability_rule
+        raise ValueError("Undefined model parameters.")
+
+
+    def __sweet_rule(self ):
+        """Return the proper sweet spot approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      - sum(model.gamma[h, l] * self.y[i][l] for l in model.L) )
+                return Constraint.Skip
+
+            return sweet_rule
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
+                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      - sum(model.gamma[h, l] * self.y[i][l] for l in model.L))
+                return Constraint.Skip
+
+            return sweet_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def get_alpha(self):
+        """Return alpha value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        alpha = list(self.__model__.alpha[:].value)
+        return np.asarray(alpha)
+
+    def get_beta(self):
+        """Return beta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
+                                                          list(self.__model__.beta[:, :].value))])
+        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
+        beta = beta.pivot(index='Name', columns='Key', values='Value')
+        return beta.to_numpy()
+
+    def get_gamma(self):
+        """Return gamma value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
+                                                           list(self.__model__.gamma[:, :].value))])
+        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
+        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
+        return gamma.to_numpy()
+
+
+class weakCERbZG1(weakCQRbZG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, z, tau, cutactive, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERZG2.py` & `pytedea-0.0.2/pytedea/utils/weakCQERZG2.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import weakCQERZG1
-
-
-class weakCQRZG2(weakCQERZG1.weakCQRZG1):
-    """weakCQRZ+G in iterative loop
-    """
-
-    def __init__(self, y, x, b, z,tau, cutactive, active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCQRZ+G model
-
-        Args:
-            y (ndarray): output variable.
-            x (ndarray): input variables.
-            b (ndarray): undersiable variables.
-            z (ndarray, optional): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float or list): active concavity constraint.
-            active (float or ndarray): violated concavity constraint.
-            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.z = z
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-        self.activeweak = to_2d_list(trans_list(activeweak))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.y)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-        self.__model__.K = Set(initialize=range(len(self.z[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.delta = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='delta')
-        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.weakCQRZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.weakCQRZG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self.weakCQRZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self.weakCQRZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self.weakCQRZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.weakCQRZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-    def __sweet_rule2(self, ):
-        """Return the proper sweet spot (step2) approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule2(model, i, h):
-                if self.active[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                                      model.alpha[h] \
-                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
-                return Constraint.Skip
-
-            return sweet_rule2
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule2(model, i, h):
-                if self.active[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L))
-                return Constraint.Skip
-
-            return sweet_rule2
-
-        raise ValueError("Undefined model parameters.")
-
-    def __sweet_rule_weak2(self, ):
-        """Return the proper sweet spot (step2) approach constraint for weak dis"""
-
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule_weak2(model, i, h):
-                if self.activeweak[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return model.alpha[i] + sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
-
-                return Constraint.Skip
-
-            return sweet_rule_weak2
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule_weak2(model, i, h):
-                if self.activeweak[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return  sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
-
-                return Constraint.Skip
-
-            return sweet_rule_weak2
-
-        raise ValueError("Undefined model parameters.")
-
-
-class weakCERZG2(weakCQRZG2):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, z, tau, cutactive,active,activeweak, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model, trans_list, to_2d_list
+from . import weakCQERZG1
+
+
+class weakCQRZG2(weakCQERZG1.weakCQRZG1):
+    """weakCQRZ+G in iterative loop
+    """
+
+    def __init__(self, y, x, b, z,tau, cutactive, active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCQRZ+G model
+
+        Args:
+            y (ndarray): output variable.
+            x (ndarray): input variables.
+            b (ndarray): undersiable variables.
+            z (ndarray, optional): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float or list): active concavity constraint.
+            active (float or ndarray): violated concavity constraint.
+            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.z = z
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+        self.activeweak = to_2d_list(trans_list(activeweak))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+        self.__model__.K = Set(initialize=range(len(self.z[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self.weakCQRZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.weakCQRZG1__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self.weakCQRZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self.weakCQRZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self.weakCQRZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.weakCQRZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule_weak2(),
+                                               doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+    def __sweet_rule2(self, ):
+        """Return the proper sweet spot (step2) approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
+                return Constraint.Skip
+
+            return sweet_rule2
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
+                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L))
+                return Constraint.Skip
+
+            return sweet_rule2
+
+        raise ValueError("Undefined model parameters.")
+
+    def __sweet_rule_weak2(self, ):
+        """Return the proper sweet spot (step2) approach constraint for weak dis"""
+
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule_weak2(model, i, h):
+                if self.activeweak[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return model.alpha[i] + sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
+
+                return Constraint.Skip
+
+            return sweet_rule_weak2
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule_weak2(model, i, h):
+                if self.activeweak[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return  sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
+
+                return Constraint.Skip
+
+            return sweet_rule_weak2
+
+        raise ValueError("Undefined model parameters.")
+
+
+class weakCERZG2(weakCQRZG2):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, z, tau, cutactive,active,activeweak, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERbG2.py` & `pytedea-0.0.2/pytedea/utils/weakCQERG2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,133 +1,130 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import weakCQERbZG1,weakCQERbZG2,weakCQERbG1
-
-
-class weakCQRbG2(weakCQERbZG2.weakCQRbZG2,weakCQERbG1.weakCQRbG1,weakCQERbZG1.weakCQRbZG1,):
-    """weakCNLSb+G in iterative loop
-    """
-
-    def __init__(self, y, x, b, tau, cutactive, active, activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSb+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            tau (float): quantile.
-            cutactive (float or list): active concavity constraint.
-            active (float or ndarray): violated concavity constraint.
-            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-        self.activeweak = to_2d_list(trans_list(activeweak))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.b)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.L = Set(initialize=range(len(self.y[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCQRbZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCQRbG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCQRbZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCQRbZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCQRbZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRbZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRbZG2__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRbZG2__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-class weakCERbG2(weakCQRbG2):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, tau, cutactive, active,activeweak, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model, trans_list, to_2d_list
+from . import weakCQERZG1,weakCQERZG2,weakCQERG1
+
+
+class weakCQRG2(weakCQERZG2.weakCQRZG2,weakCQERG1.weakCQRG1,weakCQERZG1.weakCQRZG1):
+    """weakCQR+G in iterative loop
+    """
+
+    def __init__(self, y, x, b, tau, cutactive, active, activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCQRZ+G model
+
+        Args:
+            y (ndarray): output variable.
+            x (ndarray): input variables.
+            b (ndarray): undersiable variables.
+            tau (float): quantile.
+            cutactive (float or list): active concavity constraint.
+            active (float or ndarray): violated concavity constraint.
+            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+        self.activeweak = to_2d_list(trans_list(activeweak))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.delta = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='delta')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._weakCQRG1__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCQRZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                       rule=self._weakCQRZG1__disposability_rule(),
+                                                       doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                                self.__model__.I,
+                                                rule=self._weakCQRZG2__sweet_rule2(),
+                                                doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                                     self.__model__.I,
+                                                     rule=self._weakCQRZG2__sweet_rule_weak2(),
+                                                     doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+class weakCERG2(weakCQRG2):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, tau, cutactive, active,activeweak,cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERbZG1.py` & `pytedea-0.0.2/pytedea/utils/CQERZG1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,301 +1,300 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-
-
-class weakCQRbZG1:
-    """initial Group-VC-added weakCNLSbZ (weakCNLSbZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSbZ+G model
-
-        Args:
-            y (ndarray): output variable.
-            x (ndarray): input variables.
-            b (ndarray): undersiable variables.
-            z (ndarray, optional): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float or ndarray): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.z = z
-        self.tau = tau
-
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.b))) #i行
-        self.__model__.J = Set(initialize=range(len(self.x[0]))) #j个x
-        self.__model__.L = Set(initialize=range(len(self.y[0])))  # l个y
-        self.__model__.K = Set(initialize=range(len(self.z[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self.__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self.__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self.__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        # TODO(error/warning handling): Check problem status after optimization
-        self.problem_status, self.optimization_status = optimize_model(
-            self.__model__, email, self.cet, solver)
-
-    def __objective_rule(self):
-        """Return the proper objective function"""
-
-        def objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
-        return objective_rule
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-                def regression_rule(model, i):
-                    return self.b[i] == -model.alpha[i] \
-                        - sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
-                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                        + model.epsilon_minus[i] - model.epsilon_plus[i]
-                return regression_rule
-
-            elif self.rts == RTS_CRS:
-                def regression_rule(model, i):
-                    return self.b[i] == -sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                        + sum(model.gamma[i, l] * self.y[i][l] for l in model.L) \
-                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                        + model.epsilon_minus[i] - model.epsilon_plus[i]
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-            def regression_rule(model, i):
-                return log(self.b[i]) == - log(model.frontier[i] + 1) \
-                    + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                    + model.epsilon_minus[i] - model.epsilon_plus[i]
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __log_rule(self):
-        """Return the proper log constraint"""
-        if self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-                def log_rule(model, i):
-                    return model.frontier[i] == model.alpha[i] + sum(
-                        model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            - sum(model.gamma[i, l] * self.y[i][l] for l in model.L) - 1
-                return log_rule
-
-            elif self.rts == RTS_CRS:
-                def log_rule(model, i):
-                    return model.frontier[i] == + sum(
-                        model.beta[i, j] * self.x[i][j] for j in model.J) \
-                            - sum(model.gamma[i, l] * self.y[i][l] for l in model.L) - 1
-                return log_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __afriat_rule(self):
-        """Return the proper elementary Afriat approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-            def afriat_rule(model, i):
-                return __operator(
-                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
-                                   - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
-                    model.alpha[self.__model__.I.nextw(i)] \
-                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
-                        - sum(model.gamma[self.__model__.I.nextw(i), l] * self.y[i][l] for l in model.L))
-            return afriat_rule
-
-        elif self.rts == RTS_CRS:
-            def afriat_rule(model, i):
-                return __operator(
-                    sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                           - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
-                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) \
-                            - sum(model.gamma[self.__model__.I.nextw(i), l] * self.y[i][l] for l in model.L))
-            return afriat_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __disposability_rule(self):
-        """Return the proper elementary weak disposability constraint"""
-        if self.rts == RTS_VRS:
-            def disposability_rule(model, i):
-                return model.alpha[self.__model__.I.nextw(i)] \
-                    + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
-            return disposability_rule
-
-        elif self.rts == RTS_CRS:
-            def disposability_rule(model, i):
-                return sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J) >= 0
-            return disposability_rule
-        raise ValueError("Undefined model parameters.")
-
-
-    def __sweet_rule(self ):
-        """Return the proper sweet spot approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
-                                      model.alpha[h] \
-                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      - sum(model.gamma[h, l] * self.y[i][l] for l in model.L) )
-                return Constraint.Skip
-
-            return sweet_rule
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
-                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      - sum(model.gamma[h, l] * self.y[i][l] for l in model.L))
-                return Constraint.Skip
-
-            return sweet_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def get_alpha(self):
-        """Return alpha value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        alpha = list(self.__model__.alpha[:].value)
-        return np.asarray(alpha)
-
-    def get_beta(self):
-        """Return beta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
-        return beta.to_numpy()
-
-    def get_gamma(self):
-        """Return gamma value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
-                                                           list(self.__model__.gamma[:, :].value))])
-        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
-        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
-        return gamma.to_numpy()
-
-
-class weakCERbZG1(weakCQRbZG1):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, z, tau, cutactive, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+
+class CQRZG1():
+    """initial Group-VC-added CQRZ (CQRZ+G) model
+    """
+
+    def __init__(self, y, x, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CQRZ+G model
+
+        Args:
+            y (float): output variable. 
+            x (float): input variables.
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.z = z
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.z[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self.__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self.__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self.__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        # TODO(error/warning handling): Check problem status after optimization
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, email, self.cet, solver)
+
+    def __objective_rule(self):
+        """Return the proper objective function"""
+
+        def objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
+        return objective_rule
+
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+
+                def regression_rule(model, i):
+                    return self.y[i] == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                        - model.epsilon_minus[i] + model.epsilon_plus[i]
+
+                return regression_rule
+            elif self.rts == RTS_CRS:
+
+                def regression_rule(model, i):
+                    return self.y[i] == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                        - model.epsilon_minus[i] + model.epsilon_plus[i]
+                return regression_rule
+
+        elif self.cet == CET_MULT:
+
+            def regression_rule(model, i):
+                return log(self.y[i]) == log(model.frontier[i] + 1) \
+                    - sum(model.lamda[k] * self.z[i][k] for k in model.K) \
+                    - model.epsilon_minus[i] + model.epsilon_plus[i]
+            return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __log_rule(self):
+        """Return the proper log constraint"""
+        if self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+                def log_rule(model, i):
+                    return model.frontier[i] == model.alpha[i] + sum(
+                        model.beta[i, j] * self.x[i][j] for j in model.J) - 1
+                return log_rule
+
+            elif self.rts == RTS_CRS:
+                def log_rule(model, i):
+                    return model.frontier[i] == sum(
+                        model.beta[i, j] * self.x[i][j] for j in model.J) - 1
+                return log_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __afriat_rule(self):
+        """Return the proper elementary Afriat approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+                def afriat_rule(model, i):
+                    return __operator(
+                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                             for j in model.J),
+                        model.alpha[self.__model__.I.nextw(i)] +
+                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
+                            for j in model.J))
+                return afriat_rule
+
+            elif self.rts == RTS_CRS:
+                def afriat_rule(model, i):
+                    return __operator(
+                        sum(model.beta[i, j] * self.x[i][j]
+                            for j in model.J),
+                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
+                            for j in model.J))
+                return afriat_rule
+
+        elif self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+                def afriat_rule(model, i):
+                    return __operator(
+                        model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                             for j in model.J),
+                        model.alpha[self.__model__.I.nextw(i)] +
+                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]
+                            for j in model.J))
+                return afriat_rule
+
+            elif self.rts == RTS_CRS:
+                def afriat_rule(model, i):
+                    return __operator(
+                        sum(model.beta[i, j] * self.x[i][j] for j in model.J),
+                        sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j] for j in model.J))
+                return afriat_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __sweet_rule(self, ):
+        """Return the proper sweet spot approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.cet == CET_ADDI:
+            if self.rts == RTS_VRS:
+                def sweet_rule(model, i, h):
+                    if self.cutactive[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                                               for j in model.J),
+                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
+                                                               for j in model.J))
+                    return Constraint.Skip
+                return sweet_rule
+
+            elif self.rts == RTS_CRS:
+                def sweet_rule(model, i, h):
+                    if self.cutactive[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(sum(model.beta[i, j] * self.x[i][j]
+                                              for j in model.J),
+                                          sum(model.beta[h, j] * self.x[i][j]
+                                              for j in model.J))
+                    return Constraint.Skip
+                return sweet_rule
+
+        elif self.cet == CET_MULT:
+            if self.rts == RTS_VRS:
+                def sweet_rule(model, i, h):
+                    if self.cutactive[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]
+                                                               for j in model.J),
+                                          model.alpha[h] + sum(model.beta[h, j] * self.x[i][j]
+                                                               for j in model.J))
+                    return Constraint.Skip
+                return sweet_rule
+
+            elif self.rts == RTS_CRS:
+                def sweet_rule(model, i, h):
+                    if self.cutactive[i][h]:
+                        if i == h:
+                            return Constraint.Skip
+                        return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J),
+                                          sum(model.beta[h, j] * self.x[i][j] for j in model.J))
+                    return Constraint.Skip
+                return sweet_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def get_alpha(self):
+        """Return alpha value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        alpha = list(self.__model__.alpha[:].value)
+        return np.asarray(alpha)
+
+    def get_beta(self):
+        """Return beta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
+                                                          list(self.__model__.beta[:, :].value))])
+        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
+        beta = beta.pivot(index='Name', columns='Key', values='Value')
+        return beta.to_numpy()
+
+
+class CERZG1(CQRZG1):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable. 
+            x (float): input variables.
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, z, tau, cutactive, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERbZG2.py` & `pytedea-0.0.2/pytedea/utils/weakCQERbZG2.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import weakCQERbZG1
-
-class weakCQRbZG2(weakCQERbZG1.weakCQRbZG1):
-    """weakCNLSbZ+G in iterative loop
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSbZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float or list): active concavity constraint.
-            active (float or ndarray): violated concavity constraint.
-            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.z = z
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-        self.activeweak = to_2d_list(trans_list(activeweak))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.b)))
-        self.__model__.J = Set(initialize=range(len(self.x[0])))
-        self.__model__.L = Set(initialize=range(len(self.y[0])))
-        self.__model__.K = Set(initialize=range(len(self.z[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.beta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='beta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCQRbZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCQRbZG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCQRbZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCQRbZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCQRbZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRbZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def __sweet_rule2(self, ):
-        """Return the proper sweet spot (step2) approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule2(model, i, h):
-                if self.active[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
-                                      model.alpha[h] \
-                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      - sum(model.gamma[h, l] * self.y[i][l] for l in model.L) )
-                return Constraint.Skip
-
-            return sweet_rule2
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule2(model, i, h):
-                if self.active[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
-                                      - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
-                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
-                                      - sum(model.gamma[h, l] * self.y[i][l] for l in model.L) )
-                return Constraint.Skip
-
-            return sweet_rule2
-
-        raise ValueError("Undefined model parameters.")
-
-    def __sweet_rule_weak2(self):
-        """Return the proper sweet spot (step2) approach constraint for weak dis"""
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule_weak2(model, i, h):
-                if self.activeweak[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return model.alpha[i] + sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
-
-                return Constraint.Skip
-
-            return sweet_rule_weak2
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule_weak2(model, i, h):
-                if self.activeweak[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return  sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
-
-                return Constraint.Skip
-
-            return sweet_rule_weak2
-
-        raise ValueError("Undefined model parameters.")
-
-
-class weakCERbZG2(weakCQRbZG2):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, z, tau, cutactive,active,activeweak,  cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model, trans_list, to_2d_list
+from . import weakCQERbZG1
+
+class weakCQRbZG2(weakCQERbZG1.weakCQRbZG1):
+    """weakCNLSbZ+G in iterative loop
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive, active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSbZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): quantile.
+            cutactive (float or list): active concavity constraint.
+            active (float or ndarray): violated concavity constraint.
+            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.z = z
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+        self.activeweak = to_2d_list(trans_list(activeweak))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.b)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.L = Set(initialize=range(len(self.y[0])))
+        self.__model__.K = Set(initialize=range(len(self.z[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRbZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._weakCQRbZG1__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCQRbZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRbZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCQRbZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRbZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule_weak2(),
+                                               doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def __sweet_rule2(self, ):
+        """Return the proper sweet spot (step2) approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      - sum(model.gamma[h, l] * self.y[i][l] for l in model.L) )
+                return Constraint.Skip
+
+            return sweet_rule2
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule2(model, i, h):
+                if self.active[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      - sum(model.gamma[i, l] * self.y[i][l] for l in model.L),
+                                      sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      - sum(model.gamma[h, l] * self.y[i][l] for l in model.L) )
+                return Constraint.Skip
+
+            return sweet_rule2
+
+        raise ValueError("Undefined model parameters.")
+
+    def __sweet_rule_weak2(self):
+        """Return the proper sweet spot (step2) approach constraint for weak dis"""
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule_weak2(model, i, h):
+                if self.activeweak[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return model.alpha[i] + sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
+
+                return Constraint.Skip
+
+            return sweet_rule_weak2
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule_weak2(model, i, h):
+                if self.activeweak[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return  sum(model.beta[i, j] * self.x[h][j] for j in model.J) >= 0
+
+                return Constraint.Skip
+
+            return sweet_rule_weak2
+
+        raise ValueError("Undefined model parameters.")
+
+
+class weakCERbZG2(weakCQRbZG2):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            z (float, optional): Contextual variable(s). Defaults to None.
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b, z, tau, cutactive,active,activeweak,  cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERxG2.py` & `pytedea-0.0.2/pytedea/utils/weakCQERxG2.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model, trans_list, to_2d_list
-from . import weakCQERxZG1,weakCQERxZG2,weakCQERxG1
-
-
-class weakCQRxG2(weakCQERxZG2.weakCQRxZG2,weakCQERxG1.weakCQRxG1,weakCQERxZG1.weakCQRxZG1):
-    """weakCNLSx+G in iterative loop
-    """
-
-    def __init__(self, y, x, b, tau,cutactive, active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSx+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables.
-            tau (float): quantile.
-            cutactive (float or list): active concavity constraint.
-            active (float or ndarray): violated concavity constraint.
-            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-        self.active = to_2d_list(trans_list(active))
-        self.activeweak = to_2d_list(trans_list(activeweak))
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.x)))
-        self.__model__.J = Set(initialize=range(len(self.y[0])))
-        self.__model__.L = Set(initialize=range(len(self.b[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.delta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='delta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self._weakCQRxZG1__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self._weakCQRxG1__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self._weakCQRxZG1__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self._weakCQRxZG1__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self._weakCQRxZG1__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRxZG1__sweet_rule(),
-                                               doc='sweet spot approach')
-        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRxZG2__sweet_rule2(),
-                                               doc='sweet spot-2 approach')
-        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self._weakCQRxZG2__sweet_rule_weak2(),
-                                               doc='sweet spot-2 approach for weak dis')
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-
-class weakCERxG2(weakCQRxG2):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b,  tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b,  tau, cutactive,active,activeweak, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model, trans_list, to_2d_list
+from . import weakCQERxZG1,weakCQERxZG2,weakCQERxG1
+
+
+class weakCQRxG2(weakCQERxZG2.weakCQRxZG2,weakCQERxG1.weakCQRxG1,weakCQERxZG1.weakCQRxZG1):
+    """weakCNLSx+G in iterative loop
+    """
+
+    def __init__(self, y, x, b, tau,cutactive, active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """weakCNLSx+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables.
+            tau (float): quantile.
+            cutactive (float or list): active concavity constraint.
+            active (float or ndarray): violated concavity constraint.
+            activeweak (float or ndarray): violated concavity constraint for weak disposibility.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x = x
+        self.y = y
+        self.b = b
+        self.tau = tau
+        self.cet = cet
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+        self.active = to_2d_list(trans_list(active))
+        self.activeweak = to_2d_list(trans_list(activeweak))
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.x)))
+        self.__model__.J = Set(initialize=range(len(self.y[0])))
+        self.__model__.L = Set(initialize=range(len(self.b[0])))
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.delta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='delta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                   self.__model__.L,
+                                   bounds=(0.0, None),
+                                   doc='gamma')
+        self.__model__.epsilon_plus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='positive error term')
+        self.__model__.epsilon_minus = Var(
+            self.__model__.I, bounds=(0.0, None), doc='negative error term')
+
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self._weakCQRxZG1__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self._weakCQRxG1__regression_rule(),
+                                                    doc='regression equation')
+        if self.cet == CET_MULT:
+            self.__model__.log_rule = Constraint(self.__model__.I,
+                                                 rule=self._weakCQRxZG1__log_rule(),
+                                                 doc='log-transformed regression equation')
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self._weakCQRxZG1__afriat_rule(),
+                                                doc='elementary Afriat approach')
+        self.__model__.disposability_rule = Constraint(self.__model__.I,
+                                                        rule=self._weakCQRxZG1__disposability_rule(),
+                                                        doc='elementary weak disposibility')
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRxZG1__sweet_rule(),
+                                               doc='sweet spot approach')
+        self.__model__.sweet_rule2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRxZG2__sweet_rule2(),
+                                               doc='sweet spot-2 approach')
+        self.__model__.sweet_rule_weak2 = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self._weakCQRxZG2__sweet_rule_weak2(),
+                                               doc='sweet spot-2 approach for weak dis')
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+
+class weakCERxG2(weakCQRxG2):
+    """initial Group-VC-added CERZ (CERZ+G) model
+    """
+
+    def __init__(self, y, x, b,  tau, cutactive,active,activeweak, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
+        """CERZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float): undersiable variables
+            tau (float): expectile.
+            cutactive (float): active concavity constraint.
+            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        super().__init__(y, x, b,  tau, cutactive,active,activeweak, cet, fun, rts)
+        self.__model__.objective.deactivate()
+        self.__model__.squared_objective = Objective(
+            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
+
+    def __squared_objective_rule(self):
+        def squared_objective_rule(model):
+            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
+                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
+
+        return squared_objective_rule
+
```

### Comparing `pytedea-0.0.1/pytedea/utils/weakCQERxZG1.py` & `pytedea-0.0.2/pytedea/utils/CNLSDDFZG1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,311 +1,276 @@
-# import dependencies
-from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
-from pyomo.core.expr.numvalue import NumericValue
-import numpy as np
-import pandas as pd
-from ..constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
-from .tools import optimize_model
-
-
-class weakCQRxZG1:
-    """initial Group-VC-added weakCNLSxZ (weakCNLSxZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """weakCNLSxZ+G model
-
-        Args:
-            y (ndarray): output variable.
-            x (ndarray): input variables.
-            b (ndarray): undersiable variables.
-            z (ndarray, optional): Contextual variable(s). Defaults to None.
-            tau (float): quantile.
-            cutactive (float or ndarray): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        # TODO(error/warning handling): Check the configuration of the model exist
-        self.x = x
-        self.y = y
-        self.b = b
-        self.z = z
-        self.tau = tau
-        self.cet = cet
-        self.fun = fun
-        self.rts = rts
-
-        self.cutactive = cutactive
-
-        # Initialize the CNLS model
-        self.__model__ = ConcreteModel()
-
-        # Initialize the sets
-        self.__model__.I = Set(initialize=range(len(self.x))) #i行
-        self.__model__.J = Set(initialize=range(len(self.y[0]))) #j个y
-        self.__model__.L = Set(initialize=range(len(self.b[0])))  # l个b
-        self.__model__.K = Set(initialize=range(len(self.z[0])))
-
-        # Initialize the variables
-        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
-        self.__model__.delta = Var(self.__model__.I,
-                                  self.__model__.J,
-                                  bounds=(0.0, None),
-                                  doc='delta')
-        self.__model__.gamma = Var(self.__model__.I,
-                                   self.__model__.L,
-                                   bounds=(0.0, None),
-                                   doc='gamma')
-        self.__model__.lamda = Var(self.__model__.K, doc='Zvalue')
-        self.__model__.epsilon_plus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='positive error term')
-        self.__model__.epsilon_minus = Var(
-            self.__model__.I, bounds=(0.0, None), doc='negative error term')
-
-        self.__model__.frontier = Var(self.__model__.I,
-                                      bounds=(0.0, None),
-                                      doc='estimated frontier')
-
-        # Setup the objective function and constraints
-        self.__model__.objective = Objective(rule=self.__objective_rule(),
-                                             sense=minimize,
-                                             doc='objective function')
-        self.__model__.regression_rule = Constraint(self.__model__.I,
-                                                    rule=self.__regression_rule(),
-                                                    doc='regression equation')
-        if self.cet == CET_MULT:
-            self.__model__.log_rule = Constraint(self.__model__.I,
-                                                 rule=self.__log_rule(),
-                                                 doc='log-transformed regression equation')
-        self.__model__.afriat_rule = Constraint(self.__model__.I,
-                                                rule=self.__afriat_rule(),
-                                                doc='elementary Afriat approach')
-        self.__model__.disposability_rule = Constraint(self.__model__.I,
-                                                        rule=self.__disposability_rule(),
-                                                        doc='elementary weak disposibility')
-        self.__model__.sweet_rule = Constraint(self.__model__.I,
-                                               self.__model__.I,
-                                               rule=self.__sweet_rule(),
-                                               doc='sweet spot approach')
-
-        # Optimize model
-        self.optimization_status = 0
-        self.problem_status = 0
-
-    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        # TODO(error/warning handling): Check problem status after optimization
-        self.problem_status, self.optimization_status = optimize_model(
-            self.__model__, email, self.cet, solver)
-
-    def __objective_rule(self):
-        """Return the proper objective function"""
-
-        def objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] for i in model.I)
-        return objective_rule
-
-    def __regression_rule(self):
-        """Return the proper regression constraint"""
-        if self.cet == CET_ADDI:
-            if self.rts == RTS_VRS:
-
-                def regression_rule(model, i):
-                    return self.x[i][0] == - model.alpha[i] \
-                        + sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                        + model.epsilon_minus[i] - model.epsilon_plus[i]
-
-                return regression_rule
-            elif self.rts == RTS_CRS:
-
-                def regression_rule(model, i):
-                    return self.x[i][0] == sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                        - sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
-                        + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                        + model.epsilon_minus[i] - model.epsilon_plus[i]
-
-                return regression_rule
-
-        elif self.cet == CET_MULT:
-
-            def regression_rule(model, i):
-                return log(self.x[i][0]) == - log(model.frontier[i] + 1) \
-                    + sum(model.lamda[k] * self.z[i][k] for k in model.K) \
-                    + model.epsilon_minus[i] - model.epsilon_plus[i]
-
-            return regression_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __log_rule(self):
-        """Return the proper log constraint"""
-        if self.cet == CET_MULT:
-            if self.rts == RTS_VRS:
-
-                def log_rule(model, i):
-                    return model.frontier[i] == model.alpha[i] - sum(
-                        model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
-
-                return log_rule
-            elif self.rts == RTS_CRS:
-
-                def log_rule(model, i):
-                    return model.frontier[i] == - sum(
-                        model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                            + sum(model.delta[i, l] * self.b[i][l] for l in model.L) - 1
-
-                return log_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def __afriat_rule(self):
-        """Return the proper elementary Afriat approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def afriat_rule(model, i):
-                return __operator(
-                    model.alpha[i] + sum(model.delta[i, l] * self.b[i][l]for l in model.L) \
-                                   - sum(model.gamma[i, j] * self.y[i][j] for j in model.J),
-                    model.alpha[self.__model__.I.nextw(i)] \
-                           + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l]for l in model.L) \
-                        - sum(model.gamma[self.__model__.I.nextw(i), j] * self.y[i][j] for j in model.J))
-
-            return afriat_rule
-
-        elif self.rts == RTS_CRS:
-            def afriat_rule(model, i):
-                return __operator(
-                    sum(model.delta[i, l] * self.b[i][l]for l in model.L) \
-                                   - sum(model.gamma[i, j] * self.y[i][j] for j in model.J),
-                    sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l]for l in model.L) \
-                        - sum(model.gamma[self.__model__.I.nextw(i), j] * self.y[i][j] for j in model.J))
-
-            return afriat_rule
-        raise ValueError("Undefined model parameters.")
-
-    def __disposability_rule(self):
-        """Return the proper elementary weak disposability constraint"""
-        if self.rts == RTS_VRS:
-            def disposability_rule(model, i):
-                return model.alpha[self.__model__.I.nextw(i)] \
-                    + sum(self.x[i])  >= 0
-
-            return disposability_rule
-
-        elif self.rts == RTS_CRS:
-            def disposability_rule(model, i):
-                return sum(self.x[i])  >= 0
-            return disposability_rule
-        raise ValueError("Undefined model parameters.")
-
-
-    def __sweet_rule(self ):
-        """Return the proper sweet spot approach constraint"""
-        if self.fun == FUN_PROD:
-            __operator = NumericValue.__le__
-        elif self.fun == FUN_COST:
-            __operator = NumericValue.__ge__
-
-        if self.rts == RTS_VRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(model.alpha[i] \
-                                      - sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                                      model.alpha[h] \
-                                      - sum(model.gamma[h, j] * self.y[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
-                return Constraint.Skip
-
-            return sweet_rule
-        elif self.rts == RTS_CRS:
-
-            def sweet_rule(model, i, h):
-                if self.cutactive[i][h]:
-                    if i == h:
-                        return Constraint.Skip
-                    return __operator(- sum(model.gamma[i, j] * self.y[i][j] for j in model.J) \
-                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L),
-                                      - sum(model.gamma[h, j] * self.y[i][j] for j in model.J) \
-                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) )
-                return Constraint.Skip
-
-            return sweet_rule
-
-        raise ValueError("Undefined model parameters.")
-
-    def get_alpha(self):
-        """Return alpha value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        alpha = list(self.__model__.alpha[:].value)
-        return np.asarray(alpha)
-
-    def get_delta(self):
-        """Return delta value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
-                                                          list(self.__model__.delta[:, :].value))])
-        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
-        delta = delta.pivot(index='Name', columns='Key', values='Value')
-        return delta.to_numpy()
-
-    def get_gamma(self):
-        """Return gamma value by array"""
-        if self.optimization_status == 0:
-            self.optimize()
-        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
-                                                           list(self.__model__.gamma[:, :].value))])
-        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
-        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
-        return gamma.to_numpy()
-
-
-class weakCERxZG1(weakCQRxZG1):
-    """initial Group-VC-added CERZ (CERZ+G) model
-    """
-
-    def __init__(self, y, x, b, z, tau, cutactive, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
-        """CERZ+G model
-
-        Args:
-            y (float): output variable.
-            x (float): input variables.
-            b (float): undersiable variables
-            z (float, optional): Contextual variable(s). Defaults to None.
-            tau (float): expectile.
-            cutactive (float): active concavity constraint.
-            cet (String, optional): CET_ADDI (additive composite error term) or CET_MULT (multiplicative composite error term). Defaults to CET_ADDI.
-            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
-            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
-        """
-        super().__init__(y, x, b, z, tau, cutactive, cet, fun, rts)
-        self.__model__.objective.deactivate()
-        self.__model__.squared_objective = Objective(
-            rule=self.__squared_objective_rule(), sense=minimize, doc='squared objective rule')
-
-    def __squared_objective_rule(self):
-        def squared_objective_rule(model):
-            return (1 - self.tau) * sum(model.epsilon_plus[i] ** 2 for i in model.I) \
-                + self.tau * sum(model.epsilon_minus[i] ** 2 for i in model.I)
-
-        return squared_objective_rule
-
+# import dependencies
+from pyomo.environ import ConcreteModel, Set, Var, Objective, minimize, Constraint, log
+from pyomo.core.expr.numvalue import NumericValue
+import numpy as np
+import pandas as pd
+from ..constant import CET_ADDI, FUN_PROD, FUN_COST, RTS_CRS, RTS_VRS, OPT_DEFAULT, OPT_LOCAL
+from .tools import optimize_model
+
+class CNLSDDFZG1():
+    """initial Group-VC-added CNLSDDFZ (CNLSDDFZ+G) model
+    """
+
+    def __init__(self, y, x, b, z, cutactive,gy=[1], gx=[1], gb=[1], fun=FUN_PROD, rts=RTS_VRS):
+        """CNLSDDFZ+G model
+
+        Args:
+            y (float): output variable.
+            x (float): input variables.
+            b (float,optional): undersiable variables.
+            z (float): Contextual variable(s). Defaults to None.
+            cutactive (float, optional): active concavity constraint.
+            gy (list, optional): output directional vector. Defaults to [1].
+            gx (list, optional): input directional vector. Defaults to [1].
+            gb (list, optional): undesirable output directional vector. Defaults to [1].
+            fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+            rts (String, optional): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale). Defaults to RTS_VRS.
+        """
+        # TODO(error/warning handling): Check the configuration of the model exist
+        self.x,self.y,self.b,self.z = x, y, b, z
+        self.gy, self.gx, self.gb = gy,gx,gb
+        self.fun = fun
+        self.rts = rts
+
+        self.cutactive = cutactive
+
+        # Initialize the CNLS model
+        self.__model__ = ConcreteModel()
+
+        # Initialize the sets
+        self.__model__.I = Set(initialize=range(len(self.y)))
+        self.__model__.J = Set(initialize=range(len(self.x[0])))
+        self.__model__.K = Set(initialize=range(len(self.y[0])))
+
+
+        # Initialize the variables
+        self.__model__.alpha = Var(self.__model__.I, doc='alpha')
+        self.__model__.beta = Var(self.__model__.I,
+                                  self.__model__.J,
+                                  bounds=(0.0, None),
+                                  doc='beta')
+        self.__model__.gamma = Var(self.__model__.I,
+                                  self.__model__.K,
+                                  bounds=(0.0, None),
+                                  doc='gamma')
+
+        if type(self.b) != type(None):
+            self.__model__.L = Set(initialize=range(len(self.b[0])))
+            self.__model__.delta = Var(
+                self.__model__.I, self.__model__.L, bounds=(0.0, None), doc='delta')
+
+        # Initialize the set of z
+        self.__model__.M = Set(initialize=range(len(self.z[0])))
+        # Initialize the variables for z variable
+        self.__model__.lamda = Var(self.__model__.M, doc='z coefficient')
+
+        self.__model__.epsilon = Var(self.__model__.I, doc='residual')
+        self.__model__.frontier = Var(self.__model__.I,
+                                      bounds=(0.0, None),
+                                      doc='estimated frontier')
+
+        # Setup the objective function and constraints
+        self.__model__.objective = Objective(rule=self.__objective_rule(),
+                                             sense=minimize,
+                                             doc='objective function')
+        self.__model__.regression_rule = Constraint(self.__model__.I,
+                                                    rule=self.__regression_rule(),
+                                                    doc='regression equation')
+        self.__model__.translation_rule = Constraint(self.__model__.I,
+                                                     rule=self.__translation_property(),
+                                                     doc='translation property')
+
+        self.__model__.afriat_rule = Constraint(self.__model__.I,
+                                                rule=self.__afriat_rule(),
+                                                doc='elementary Afriat approach')
+
+        self.__model__.sweet_rule = Constraint(self.__model__.I,
+                                               self.__model__.I,
+                                               rule=self.__sweet_rule(),
+                                               doc='sweet spot approach')
+
+        # Optimize model
+        self.optimization_status = 0
+        self.problem_status = 0
+
+    def optimize(self, email=OPT_LOCAL, solver=OPT_DEFAULT):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        # TODO(error/warning handling): Check problem status after optimization
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, email, CET_ADDI, solver)
+
+    def __objective_rule(self):
+        """Return the proper objective function"""
+        def objective_rule(model):
+            return sum(model.epsilon[i] ** 2 for i in model.I)
+        return objective_rule
+
+    def __regression_rule(self):
+        """Return the proper regression constraint"""
+        if self.rts == RTS_VRS:
+            if type(self.b) == type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                        - model.epsilon[i]
+                return regression_rule
+
+            elif type(self.b) != type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == model.alpha[i] \
+                        + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                        - model.epsilon[i]
+                return regression_rule
+
+
+        elif self.rts == RTS_CRS:
+            if type(self.b) == type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                        - model.epsilon[i]
+                return regression_rule
+
+
+            elif type(self.b) != type(None):
+                def regression_rule(model, i):
+                    return sum(model.gamma[i, k] * self.y[i][k] for k in model.K) \
+                        == sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                        + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                        - sum(model.lamda[m] * self.z[i][m] for m in model.M) \
+                        - model.epsilon[i]
+                return regression_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def __translation_property(self):
+        """Return the proper translation property"""
+        def translation_rule(model, i):
+            return sum(model.beta[i, j] * self.gx[j] for j in model.J) \
+                + sum(model.gamma[i, k] * self.gy[k] for k in model.K) \
+                + sum(model.delta[i, l] * self.gb[l] for l in model.L) == 1
+
+        return translation_rule
+
+    def __afriat_rule(self):
+        """Return the proper elementary Afriat approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def afriat_rule(model, i):
+                return __operator(
+                    model.alpha[i] + sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
+                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                    model.alpha[self.__model__.I.nextw(i)] \
+                           + sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
+                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
+                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
+
+            return afriat_rule
+
+        elif self.rts == RTS_CRS:
+            def afriat_rule(model, i):
+                return __operator(sum(model.beta[i, j] * self.x[i][j]for j in model.J) \
+                                   + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                    - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                    sum(model.beta[self.__model__.I.nextw(i), j] * self.x[i][j]for j in model.J) \
+                             + sum(model.delta[self.__model__.I.nextw(i), l] * self.b[i][l] for l in model.L)\
+                             - sum(model.gamma[self.__model__.I.nextw(i), k] * self.y[i][k] for k in model.K))
+
+            return afriat_rule
+        raise ValueError("Undefined model parameters.")
+
+
+    def __sweet_rule(self ):
+        """Return the proper sweet spot approach constraint"""
+        if self.fun == FUN_PROD:
+            __operator = NumericValue.__le__
+        elif self.fun == FUN_COST:
+            __operator = NumericValue.__ge__
+
+        if self.rts == RTS_VRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(model.alpha[i] \
+                                      + sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                      model.alpha[h] \
+                                      + sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
+                return Constraint.Skip
+
+            return sweet_rule
+        elif self.rts == RTS_CRS:
+
+            def sweet_rule(model, i, h):
+                if self.cutactive[i][h]:
+                    if i == h:
+                        return Constraint.Skip
+                    return __operator(sum(model.beta[i, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[i, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K),
+                                       sum(model.beta[h, j] * self.x[i][j] for j in model.J) \
+                                      + sum(model.delta[h, l] * self.b[i][l] for l in model.L) \
+                                      - sum(model.gamma[i, k] * self.y[i][k] for k in model.K) )
+                return Constraint.Skip
+
+            return sweet_rule
+
+        raise ValueError("Undefined model parameters.")
+
+    def get_alpha(self):
+        """Return alpha value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        alpha = list(self.__model__.alpha[:].value)
+        return np.asarray(alpha)
+
+    def get_beta(self):
+        """Return beta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
+                                                          list(self.__model__.beta[:, :].value))])
+        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
+        beta = beta.pivot(index='Name', columns='Key', values='Value')
+        return beta.to_numpy()
+
+    def get_delta(self):
+        """Return delta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        delta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.delta),
+                                                           list(self.__model__.delta[:, :].value))])
+        delta = pd.DataFrame(delta, columns=['Name', 'Key', 'Value'])
+        delta = delta.pivot(index='Name', columns='Key', values='Value')
+        return delta.to_numpy()
+
+    def get_gamma(self):
+        """Return delta value by array"""
+        if self.optimization_status == 0:
+            self.optimize()
+        gamma = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.gamma),
+                                                           list(self.__model__.gamma[:, :].value))])
+        gamma = pd.DataFrame(gamma, columns=['Name', 'Key', 'Value'])
+        gamma = gamma.pivot(index='Name', columns='Key', values='Value')
+        return gamma.to_numpy()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytedea-0.0.1/pytedea.egg-info/PKG-INFO` & `pytedea-0.0.2/pytedea.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: pytedea
-Version: 0.0.1
-Summary: Data envelopment analysis using Python.
-Home-page: https://github.com/advancehs/pytedea
-Author: advancehs
-Author-email: 1019753743@qq.com
-License: GNU General Public License v3
-Keywords: pytedea
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pytedea
-
-
-[![image](https://img.shields.io/pypi/v/pytedea.svg)](https://pypi.python.org/pypi/pytedea)
-[![image](https://img.shields.io/conda/vn/conda-forge/pytedea.svg)](https://anaconda.org/conda-forge/pytedea)
-
-
-**Data envelopment analysis using Python.**
-
-
--   Free software: GNU General Public License v3
--   Documentation: https://advancehs.github.io/pytedea
-    
-
-## Features
-
--   TODO
+Metadata-Version: 2.1
+Name: pytedea
+Version: 0.0.2
+Summary: Data envelopment analysis using Python.
+Home-page: https://github.com/advancehs/pytedea
+Author: advancehs
+Author-email: 1019753743@qq.com
+License: GNU General Public License v3
+Keywords: pytedea
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pytedea
+
+
+[![image](https://img.shields.io/pypi/v/pytedea.svg)](https://pypi.python.org/pypi/pytedea)
+[![image](https://img.shields.io/conda/vn/conda-forge/pytedea.svg)](https://anaconda.org/conda-forge/pytedea)
+
+
+**Data envelopment analysis using Python.**
+
+
+-   Free software: GNU General Public License v3
+-   Documentation: https://advancehs.github.io/pytedea
+    
+
+## Features
+
+-   TODO
```

### Comparing `pytedea-0.0.1/pytedea.egg-info/SOURCES.txt` & `pytedea-0.0.2/pytedea.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
+pytedea/DDF.py
 pytedea/DDFt.py
+pytedea/DEA.py
 pytedea/DEAt.py
+pytedea/HYPER.py
+pytedea/NDDF.py
 pytedea/__init__.py
-pytedea/common.py
 pytedea/constant.py
 pytedea/pytedea.py
 pytedea.egg-info/PKG-INFO
 pytedea.egg-info/SOURCES.txt
 pytedea.egg-info/dependency_links.txt
 pytedea.egg-info/not-zip-safe
 pytedea.egg-info/requires.txt
@@ -63,11 +66,8 @@
 pytedea/utils/weakCQERbG1.py
 pytedea/utils/weakCQERbG2.py
 pytedea/utils/weakCQERbZG1.py
 pytedea/utils/weakCQERbZG2.py
 pytedea/utils/weakCQERxG1.py
 pytedea/utils/weakCQERxG2.py
 pytedea/utils/weakCQERxZG1.py
-pytedea/utils/weakCQERxZG2.py
-tests/test_DDFt.py
-tests/test_DEAt.py
-tests/test_pytedea.py
+pytedea/utils/weakCQERxZG2.py
```

### Comparing `pytedea-0.0.1/setup.py` & `pytedea-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = [ ]
-
-test_requirements = [ ]
-
-setup(
-    author="advancehs",
-    author_email='1019753743@qq.com',
-    python_requires='>=3.8',
-    classifiers=[
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
-    description="Data envelopment analysis using Python.",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="GNU General Public License v3",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='pytedea',
-    name='pytedea',
-    packages=find_packages(include=['pytedea', 'pytedea.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/advancehs/pytedea',
-    version='0.0.1',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = [ ]
+
+test_requirements = [ ]
+
+setup(
+    author="advancehs",
+    author_email='1019753743@qq.com',
+    python_requires='>=3.8',
+    classifiers=[
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ],
+    description="Data envelopment analysis using Python.",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="GNU General Public License v3",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='pytedea',
+    name='pytedea',
+    packages=find_packages(include=['pytedea', 'pytedea.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/advancehs/pytedea',
+    version='0.0.2',
+    zip_safe=False,
+)
```

