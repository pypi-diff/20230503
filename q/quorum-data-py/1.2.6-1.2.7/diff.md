# Comparing `tmp/quorum_data_py-1.2.6.tar.gz` & `tmp/quorum_data_py-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.2.6.tar", last modified: Sun Apr 30 08:03:49 2023, max compression
+gzip compressed data, was "quorum_data_py-1.2.7.tar", last modified: Wed May  3 15:46:14 2023, max compression
```

## Comparing `quorum_data_py-1.2.6.tar` & `quorum_data_py-1.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 08:03:49.777190 quorum_data_py-1.2.6/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.6/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-30 08:03:49.776194 quorum_data_py-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.6/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-30 08:03:49.761232 quorum_data_py-1.2.6/quorum_data_py/
--rw-rw-rw-   0        0        0      355 2023-04-30 08:03:09.000000 quorum_data_py-1.2.6/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.6/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.6/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5326 2023-04-25 06:32:35.000000 quorum_data_py-1.2.6/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.6/quorum_data_py/trx_type.py
--rw-rw-rw-   0        0        0     1266 2023-04-30 08:02:55.000000 quorum_data_py-1.2.6/quorum_data_py/util.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:03:49.773201 quorum_data_py-1.2.6/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-30 08:03:49.000000 quorum_data_py-1.2.6/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-30 08:03:49.000000 quorum_data_py-1.2.6/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 08:03:49.000000 quorum_data_py-1.2.6/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-30 08:03:49.000000 quorum_data_py-1.2.6/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-30 08:03:49.000000 quorum_data_py-1.2.6/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 08:03:49.777190 quorum_data_py-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-04-30 08:03:09.000000 quorum_data_py-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:46:14.040747 quorum_data_py-1.2.7/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-05-03 15:46:14.039745 quorum_data_py-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.7/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-03 15:46:14.022460 quorum_data_py-1.2.7/quorum_data_py/
+-rw-rw-rw-   0        0        0      355 2023-05-03 15:44:18.000000 quorum_data_py-1.2.7/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.7/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2959 2023-05-03 15:45:18.000000 quorum_data_py-1.2.7/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5326 2023-04-25 06:32:35.000000 quorum_data_py-1.2.7/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.7/quorum_data_py/trx_type.py
+-rw-rw-rw-   0        0        0     1266 2023-05-03 15:45:16.000000 quorum_data_py-1.2.7/quorum_data_py/util.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:46:14.037059 quorum_data_py-1.2.7/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-05-03 15:46:13.000000 quorum_data_py-1.2.7/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-03 15:46:13.000000 quorum_data_py-1.2.7/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 15:46:13.000000 quorum_data_py-1.2.7/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-03 15:46:13.000000 quorum_data_py-1.2.7/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-03 15:46:13.000000 quorum_data_py-1.2.7/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 15:46:14.040747 quorum_data_py-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-05-03 15:44:18.000000 quorum_data_py-1.2.7/setup.py
```

### Comparing `quorum_data_py-1.2.6/LICENSE` & `quorum_data_py-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.6/PKG-INFO` & `quorum_data_py-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.6/README.md` & `quorum_data_py-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.6/quorum_data_py/_utils.py` & `quorum_data_py-1.2.7/quorum_data_py/_utils.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.6/quorum_data_py/converter.py` & `quorum_data_py-1.2.7/quorum_data_py/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 数据结构转换
 
 把 解密后的 trx （通过 get content api 所获得的 trx）转换成新版的 trx data 和 timestamp 等，用来重新发布上链
 """
-from quorum_mininode_py.crypto.account import public_key_to_address
+
+from quorum_mininode_py import pubkey_to_address
 
 from quorum_data_py import feed
 
 
 def from_new_chain(trx: dict):
     """
     把新共识版本的 trx 还原为 trx data 和 timestamp，
@@ -27,25 +28,26 @@
 
 def from_old_chain(trx: dict):
     """
     把旧共识版本的 trx 转换成新版的 trx data 和 timestamp，
     然后通过轻节点的 post to group api 发送上链
     适用场景：把旧链的 trxs 发送到新链
     """
+
     if isinstance(trx.get("Data"), str):
         raise ValueError("trx is encrypted.")
 
     typeurl = trx.get("TypeUrl")
     pubkey = trx.get("Publisher") or trx.get("SenderPubkey")
 
     contentobj = trx.get("Content") or trx.get("Data") or {}
 
     obj = None
     if typeurl == "quorum.pb.Person":
-        address = public_key_to_address(pubkey)
+        address = pubkey_to_address(pubkey)
         obj = {
             "type": "Create",
             "object": {
                 "type": "Profile",
                 "describes": {"type": "Person", "id": address},
             },
         }
```

### Comparing `quorum_data_py-1.2.6/quorum_data_py/feed.py` & `quorum_data_py-1.2.7/quorum_data_py/feed.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.6/quorum_data_py/trx_type.py` & `quorum_data_py-1.2.7/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.6/quorum_data_py/util.py` & `quorum_data_py-1.2.7/quorum_data_py/util.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.2.6/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.2.7/quorum_data_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.2.6/setup.py` & `quorum_data_py-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.2.6",
+    version="1.2.7",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
```

