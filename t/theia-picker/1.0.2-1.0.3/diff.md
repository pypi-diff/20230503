# Comparing `tmp/theia-picker-1.0.2.tar.gz` & `tmp/theia-picker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theia-picker-1.0.2.tar", last modified: Mon Mar 20 20:01:43 2023, max compression
+gzip compressed data, was "theia-picker-1.0.3.tar", last modified: Wed May  3 18:50:27 2023, max compression
```

## Comparing `theia-picker-1.0.2.tar` & `theia-picker-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 20:01:43.115132 theia-picker-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)    11340 2023-03-20 11:11:16.000000 theia-picker-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      193 2023-03-20 20:01:43.115132 theia-picker-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1598 2023-03-20 19:59:51.000000 theia-picker-1.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-20 20:01:43.115132 theia-picker-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-03-20 19:59:51.000000 theia-picker-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 20:01:43.111132 theia-picker-1.0.2/theia_picker/
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-03-20 11:11:16.000000 theia-picker-1.0.2/theia_picker/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5821 2023-03-20 14:25:56.000000 theia-picker-1.0.2/theia_picker/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    26119 2023-03-20 19:59:51.000000 theia-picker-1.0.2/theia_picker/download.py
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-03-20 19:59:51.000000 theia-picker-1.0.2/theia_picker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 20:01:43.115132 theia-picker-1.0.2/theia_picker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      193 2023-03-20 20:01:43.000000 theia-picker-1.0.2/theia_picker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      371 2023-03-20 20:01:43.000000 theia-picker-1.0.2/theia_picker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 20:01:43.000000 theia-picker-1.0.2/theia_picker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-20 20:01:43.000000 theia-picker-1.0.2/theia_picker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 20:01:42.000000 theia-picker-1.0.2/theia_picker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-20 20:01:43.000000 theia-picker-1.0.2/theia_picker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-20 20:01:43.000000 theia-picker-1.0.2/theia_picker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:50:27.380424 theia-picker-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2023-03-20 11:11:16.000000 theia-picker-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      193 2023-05-03 18:50:27.380424 theia-picker-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-03-20 19:59:51.000000 theia-picker-1.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 18:50:27.380424 theia-picker-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-05-03 18:45:31.000000 theia-picker-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:50:27.380424 theia-picker-1.0.3/theia_picker/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-03-20 11:11:16.000000 theia-picker-1.0.3/theia_picker/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5821 2023-03-20 14:25:56.000000 theia-picker-1.0.3/theia_picker/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    26123 2023-05-03 18:44:02.000000 theia-picker-1.0.3/theia_picker/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-03-20 19:59:51.000000 theia-picker-1.0.3/theia_picker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:50:27.380424 theia-picker-1.0.3/theia_picker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      193 2023-05-03 18:50:27.000000 theia-picker-1.0.3/theia_picker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-03 18:50:27.000000 theia-picker-1.0.3/theia_picker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 18:50:27.000000 theia-picker-1.0.3/theia_picker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-03 18:50:27.000000 theia-picker-1.0.3/theia_picker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 18:50:27.000000 theia-picker-1.0.3/theia_picker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-03 18:50:27.000000 theia-picker-1.0.3/theia_picker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-03 18:50:27.000000 theia-picker-1.0.3/theia_picker.egg-info/top_level.txt
```

### Comparing `theia-picker-1.0.2/LICENSE` & `theia-picker-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `theia-picker-1.0.2/README.md` & `theia-picker-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `theia-picker-1.0.2/theia_picker/cli.py` & `theia-picker-1.0.3/theia_picker/cli.py`

 * *Files identical despite different names*

### Comparing `theia-picker-1.0.2/theia_picker/download.py` & `theia-picker-1.0.3/theia_picker/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             Returns:
                 function return value
 
             """
             for retry_nb in range(times):
                 try:
                     extra_opts = {} if retry_nb == 0 else {"renew_token": True}
-                    return function(*args, **kwargs, **extra_opts)
+                    return function(*args, **{**kwargs, **extra_opts})
                 except err_cls as err:
                     log.warning("Failed to %s: %s", action, err)
                     if retry_nb == times - 1:
                         raise
                 log.warning(
                     "%s attempts left. Retry in %s seconds...",
                     times - retry_nb - 1, sleep_duration
```

