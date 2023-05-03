# Comparing `tmp/recon_lw-2.0.0.dev4859625658.tar.gz` & `tmp/recon_lw-2.0.0.dev4870468547.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4859625658.tar", last modified: Tue May  2 09:22:21 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4870468547.tar", last modified: Wed May  3 09:40:58 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4859625658.tar` & `recon_lw-2.0.0.dev4870468547.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-02 09:21:58.000000 recon_lw-2.0.0.dev4859625658/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13016 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    21293 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:22:21.000000 recon_lw-2.0.0.dev4859625658/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-02 09:21:50.000000 recon_lw-2.0.0.dev4859625658/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-03 09:40:38.000000 recon_lw-2.0.0.dev4870468547/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13016 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21309 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 09:40:58.000000 recon_lw-2.0.0.dev4870468547/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-03 09:40:17.000000 recon_lw-2.0.0.dev4870468547/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4859625658/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4870468547/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4859625658/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4870468547/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4859625658/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4870468547/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4859625658/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4870468547/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     sub_seq = None
     if current_ts is not None:
         edge_timestamp = {"epochSecond": current_ts["epochSecond"] - horizon_delay,
                           "nano": 0}
         horizon_edge = times.bisect_key_left(recon_lw.time_stamp_key(edge_timestamp))
         if horizon_edge < len(times):
             seq_index = times[horizon_edge][1]
-            sub_seq = sequence.irange(None, (seq_index, None))
+            sub_seq = sequence.irange(None, (seq_index, None), (False, False))
             for i in range(0, horizon_edge):
                 times.pop(0)
         else:
             sub_seq = sequence
             times.clear()
         return sub_seq
     else:
```

### Comparing `recon_lw-2.0.0.dev4859625658/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4870468547/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4859625658/setup.py` & `recon_lw-2.0.0.dev4870468547/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4859625658/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4870468547/test/test_recon_ob.py`

 * *Files identical despite different names*

