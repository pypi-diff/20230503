# Comparing `tmp/popobot-0.3.tar.gz` & `tmp/popobot-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/popobot-0.3.tar", last modified: Wed May  3 05:26:36 2023, max compression
+gzip compressed data, was "dist/popobot-0.4.tar", last modified: Wed May  3 08:09:45 2023, max compression
```

## Comparing `popobot-0.3.tar` & `popobot-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:26:36.000000 popobot-0.3/
--rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 05:26:36.000000 popobot-0.3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1025 2023-05-03 04:01:13.000000 popobot-0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      183 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)    11140 2023-05-03 05:26:07.000000 popobot-0.3/popobot.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 05:26:36.000000 popobot-0.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1227 2023-05-03 04:09:16.000000 popobot-0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 08:09:45.000000 popobot-0.4/
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-05-03 08:09:45.000000 popobot-0.4/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     1974 2023-05-03 08:09:12.000000 popobot-0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 08:09:45.000000 popobot-0.4/popobot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-05-03 08:09:45.000000 popobot-0.4/popobot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      183 2023-05-03 08:09:45.000000 popobot-0.4/popobot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 08:09:45.000000 popobot-0.4/popobot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-03 08:09:45.000000 popobot-0.4/popobot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-03 08:09:45.000000 popobot-0.4/popobot.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    13457 2023-05-03 08:06:51.000000 popobot-0.4/popobot.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 08:09:45.000000 popobot-0.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1227 2023-05-03 04:09:16.000000 popobot-0.4/setup.py
```

### Comparing `popobot-0.3/popobot.py` & `popobot-0.4/popobot.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 使用方法:
     :from popobot import *
     
 
 开源包，任何人都可以使用并修改！
 """
 
-__version__ = '0.3'
+__version__ = '0.4'
 
 import time
 from requests import get,post
 from json import loads,dumps
 
 class Account:
     def __init__(self, cookie):
@@ -238,15 +238,74 @@
             'X-Requested-With':'XMLHttpRequest'
        }
         url='https://im.popoim.com/web/group/leave'
         data = {
             'gid':group
         }
         return loads(str(post(url,headers=headers,data=data).text))['data']
-        
+    
+    def ApplyFriend(self,friend,content):
+        headers = {
+            'Origin':'https://im.popoim.com',
+            'Host':'im.popoim.com',
+            'Cookie':self.cookie,
+            'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+            'X-Requested-With':'XMLHttpRequest'
+       }
+        url='https://im.popoim.com/web/friend/apply'
+        data = {
+            'friend_uid':friend,
+            'postscript':content
+        }
+        return loads(str(post(url,headers=headers,data=data).text))['data']
+    
+    def UnMute(self,group):
+        headers = {
+            'Origin':'https://im.popoim.com',
+            'Host':'im.popoim.com',
+            'Cookie':self.cookie,
+            'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+            'X-Requested-With':'XMLHttpRequest'
+       }
+        url='https://im.popoim.com/web/group/forbiddenall'
+        data = {
+            'gid':group,
+            'value':'0'
+        }
+        return loads(str(post(url,headers=headers,data=data).text))['data']
+    
+    def Mute(self,group):
+        headers = {
+            'Origin':'https://im.popoim.com',
+            'Host':'im.popoim.com',
+            'Cookie':self.cookie,
+            'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+            'X-Requested-With':'XMLHttpRequest'
+       }
+        url='https://im.popoim.com/web/group/forbiddenall'
+        data = {
+            'gid':group,
+            'value':'1'
+        }
+        return loads(str(post(url,headers=headers,data=data).text))['data']
+    
+    def FriendDel(self,friend):
+        headers = {
+            'Origin':'https://im.popoim.com',
+            'Host':'im.popoim.com',
+            'Cookie':self.cookie,
+            'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
+            'X-Requested-With':'XMLHttpRequest'
+       }
+        url='https://im.popoim.com/web/friend/delete'
+        data = {
+            'friend_uid':friend
+        }
+        return loads(str(post(url,headers=headers,data=data).text))['data']
+    
     def GroupDel(self,group):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
```

### Comparing `popobot-0.3/setup.py` & `popobot-0.4/setup.py`

 * *Files identical despite different names*

