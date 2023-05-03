# Comparing `tmp/basic_math_operations-1.0.157.tar.gz` & `tmp/basic_math_operations-1.0.158.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_math_operations-1.0.157.tar", last modified: Thu Mar 30 12:15:25 2023, max compression
+gzip compressed data, was "basic_math_operations-1.0.158.tar", last modified: Wed May  3 18:46:27 2023, max compression
```

## Comparing `basic_math_operations-1.0.157.tar` & `basic_math_operations-1.0.158.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:15:25.527015 basic_math_operations-1.0.157/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-30 12:15:05.000000 basic_math_operations-1.0.157/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-30 12:15:25.527015 basic_math_operations-1.0.157/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-03-30 12:15:05.000000 basic_math_operations-1.0.157/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:15:25.527015 basic_math_operations-1.0.157/basic_math_operations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-30 12:15:25.000000 basic_math_operations-1.0.157/basic_math_operations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-30 12:15:25.000000 basic_math_operations-1.0.157/basic_math_operations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 12:15:25.000000 basic_math_operations-1.0.157/basic_math_operations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-30 12:15:25.000000 basic_math_operations-1.0.157/basic_math_operations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 12:15:25.527015 basic_math_operations-1.0.157/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-30 12:15:05.000000 basic_math_operations-1.0.157/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:15:25.527015 basic_math_operations-1.0.157/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:15:25.527015 basic_math_operations-1.0.157/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)    73232 2023-03-30 12:15:25.000000 basic_math_operations-1.0.157/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-03-30 12:15:05.000000 basic_math_operations-1.0.157/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 12:15:25.000000 basic_math_operations-1.0.157/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 18:46:12.000000 basic_math_operations-1.0.158/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-03 18:46:12.000000 basic_math_operations-1.0.158/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/basic_math_operations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/basic_math_operations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/basic_math_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/basic_math_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/basic_math_operations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:46:27.829268 basic_math_operations-1.0.158/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-03 18:46:12.000000 basic_math_operations-1.0.158/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:46:27.825268 basic_math_operations-1.0.158/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)    75056 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-03 18:46:12.000000 basic_math_operations-1.0.158/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:46:27.000000 basic_math_operations-1.0.158/src/python-module/version.txt
```

### Comparing `basic_math_operations-1.0.157/LICENSE` & `basic_math_operations-1.0.158/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.157/README.md` & `basic_math_operations-1.0.158/README.md`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.157/setup.py` & `basic_math_operations-1.0.158/setup.py`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.157/src/python-module/libbasic_math_operations.a` & `basic_math_operations-1.0.158/src/python-module/libbasic_math_operations.a`

 * *Files 1% similar despite different names*

#### nm -s {}

```diff
@@ -39,14 +39,15 @@
 multiplyp in multiplyp.c.o
 multiply in multiply.c.o
 _divide_whole_with_remainder in _divide_whole_with_remainder.asm.o
 divide_whole_with_remainder in divide_whole_with_remainder.c.o
 divide_whole in divide_whole.c.o
 dividep in dividep.c.o
 divide in divide.c.o
+abs_mod in abs_mod.c.o
 asmalloc in asmalloc.asm.o
 multiply_whole in multiply_whole.asm.o
 addp in addp.c.o
 remove_zeroes in remove_zeroes.c.o
 increment_whole in increment_whole.c.o
 
 basic_math_operations.c.o:
@@ -291,14 +292,21 @@
 divide.c.o:
 0000000000000000 T divide
                  U dividep
                  U memmove
                  U remove_zeroes
                  U strlen_asm
 
+abs_mod.c.o:
+0000000000000000 T abs_mod
+                 U calloc
+                 U divide_whole_with_remainder
+                 U free
+                 U strlen
+
 asmalloc.asm.o:
 0000000000000000 T asmalloc
 
 multiply_whole.asm.o:
                  U _multiply_whole
                  U asmalloc
 0000000000000000 T multiply_whole
```

#### file list

```diff
@@ -1,8 +1,8 @@
-----------   0        0        0     2000 1970-01-01 00:00:00.000000 /
+----------   0        0        0     2012 1970-01-01 00:00:00.000000 /
 ----------   0        0        0        0 1970-01-01 00:00:00.000000 //
 ?rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 basic_math_operations.c.o
 ?rw-r--r--   0        0        0    28944 1970-01-01 00:00:00.000000 basic_math_operations.cpp.o
 ?rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 strlen_asm.asm.o
 ?rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 remove_leading_zeroes.asm.o
 ?rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 add_whole.asm.o
 ?rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 add_whole_same_length.asm.o
@@ -15,12 +15,13 @@
 ?rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 multiplyp.c.o
 ?rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 multiply.c.o
 ?rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 _divide_whole_with_remainder.asm.o
 ?rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 divide_whole_with_remainder.c.o
 ?rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 divide_whole.c.o
 ?rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 dividep.c.o
 ?rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 divide.c.o
+?rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 abs_mod.c.o
 ?rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 asmalloc.asm.o
 ?rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 multiply_whole.asm.o
 ?rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 addp.c.o
 ?rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 remove_zeroes.c.o
 ?rw-r--r--   0        0        0     1888 1970-01-01 00:00:00.000000 increment_whole.c.o
```

### Comparing `basic_math_operations-1.0.157/src/python-module/module.c` & `basic_math_operations-1.0.158/src/python-module/module.c`

 * *Files identical despite different names*

