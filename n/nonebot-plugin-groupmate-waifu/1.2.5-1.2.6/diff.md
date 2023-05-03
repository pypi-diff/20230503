# Comparing `tmp/nonebot_plugin_groupmate_waifu-1.2.5.tar.gz` & `tmp/nonebot_plugin_groupmate_waifu-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.2.5.tar", last modified: Sat Feb  4 06:08:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.2.6.tar", last modified: Wed May  3 13:12:14 2023, max compression
```

## Comparing `nonebot_plugin_groupmate_waifu-1.2.5.tar` & `nonebot_plugin_groupmate_waifu-1.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-04 06:08:58.561613 nonebot_plugin_groupmate_waifu-1.2.5/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.2.5/LICENSE
--rw-rw-rw-   0        0        0      279 2023-02-04 06:08:58.561113 nonebot_plugin_groupmate_waifu-1.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-04 06:08:58.552105 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu/
--rw-rw-rw-   0        0        0    19935 2023-02-04 06:03:12.000000 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu/__init__.py
--rw-rw-rw-   0        0        0      305 2023-02-04 06:03:38.000000 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu/config.py
--rw-rw-rw-   0        0        0     2261 2023-02-04 04:51:53.000000 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-04 06:08:58.559612 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu.egg-info/
--rw-rw-rw-   0        0        0      279 2023-02-04 06:08:58.000000 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-02-04 06:08:58.000000 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-04 06:08:58.000000 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-02-04 06:08:58.000000 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-02-04 06:08:58.000000 nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-04 06:08:58.561613 nonebot_plugin_groupmate_waifu-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      583 2023-02-04 06:08:52.000000 nonebot_plugin_groupmate_waifu-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:12:14.630504 nonebot_plugin_groupmate_waifu-1.2.6/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      279 2023-05-03 13:12:14.630004 nonebot_plugin_groupmate_waifu-1.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 13:12:14.618494 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/
+-rw-rw-rw-   0        0        0    20160 2023-05-03 13:08:54.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-02-04 06:03:38.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/config.py
+-rw-rw-rw-   0        0        0     2261 2023-02-04 04:51:53.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:12:14.628503 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 13:12:14.631005 nonebot_plugin_groupmate_waifu-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-05-03 13:12:06.000000 nonebot_plugin_groupmate_waifu-1.2.6/setup.py
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.5/LICENSE` & `nonebot_plugin_groupmate_waifu-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu/__init__.py` & `nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,19 @@
             record_yinpa2 = eval(line)
     else:
         record_yinpa2 = {}
 
     # 重置记录
     @scheduler.scheduled_job("cron",hour = 0)
     def _():
-        global record_yinpa1,record_yinpa2
+        global record_waifu,record_yinpa1,record_yinpa2
+        for group_id in record_waifu:
+            for user_id in record_waifu[group_id]:
+                if record_waifu[group_id][user_id] == user_id:
+                    record_waifu[group_id][user_id] = 0
         record_yinpa1 = {}
         record_yinpa2 = {}
 
 
 
 # 娶群友
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.5/nonebot_plugin_groupmate_waifu/utils.py` & `nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.2.5/setup.py` & `nonebot_plugin_groupmate_waifu-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_groupmate_waifu',
-version='1.2.5',
+version='1.2.6',
 description='娶群友',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_groupmate_waifu"]),
```

