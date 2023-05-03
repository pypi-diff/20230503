# Comparing `tmp/popobot-0.1.tar.gz` & `tmp/popobot-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/popobot-0.1.tar", last modified: Wed May  3 04:15:02 2023, max compression
+gzip compressed data, was "dist/popobot-0.2.tar", last modified: Wed May  3 05:14:45 2023, max compression
```

## Comparing `popobot-0.1.tar` & `popobot-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 04:15:02.000000 popobot-0.1/
--rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 04:15:02.000000 popobot-0.1/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1025 2023-05-03 04:01:13.000000 popobot-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 04:15:02.000000 popobot-0.1/popobot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 04:15:02.000000 popobot-0.1/popobot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      183 2023-05-03 04:15:02.000000 popobot-0.1/popobot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 04:15:02.000000 popobot-0.1/popobot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-03 04:15:02.000000 popobot-0.1/popobot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-03 04:15:02.000000 popobot-0.1/popobot.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)    11040 2023-05-03 04:08:49.000000 popobot-0.1/popobot.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 04:15:02.000000 popobot-0.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1227 2023-05-03 04:09:16.000000 popobot-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:14:45.000000 popobot-0.2/
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 05:14:45.000000 popobot-0.2/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     1025 2023-05-03 04:01:13.000000 popobot-0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      183 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    11128 2023-05-03 05:12:37.000000 popobot-0.2/popobot.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 05:14:45.000000 popobot-0.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1227 2023-05-03 04:09:16.000000 popobot-0.2/setup.py
```

### Comparing `popobot-0.1/PKG-INFO` & `popobot-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popobot
-Version: 0.1
+Version: 0.2
 Summary: 泡泡aiM机器人库
 Home-page: https://github.com/HydroGest/PoPoBot
 Author: HydroGest
 Author-email: me@mkc.icu
 License: MIT
 Classifier: Topic :: Games/Entertainment 
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
```

### Comparing `popobot-0.1/README.md` & `popobot-0.2/README.md`

 * *Files identical despite different names*

### Comparing `popobot-0.1/popobot.egg-info/PKG-INFO` & `popobot-0.2/popobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popobot
-Version: 0.1
+Version: 0.2
 Summary: 泡泡aiM机器人库
 Home-page: https://github.com/HydroGest/PoPoBot
 Author: HydroGest
 Author-email: me@mkc.icu
 License: MIT
 Classifier: Topic :: Games/Entertainment 
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
```

### Comparing `popobot-0.1/popobot.py` & `popobot-0.2/popobot.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 使用方法:
     :from popobot import *
     
 
 开源包，任何人都可以使用并修改！
 """
 
-__version__ = '0.1'
+__version__ = '0.2'
 
 from requests import get,post
 from json import loads,dumps
 
 class Account:
     def __init__(self, cookie):
         self.cookie = cookie
 
-    def SendGroupMessage(group,message):
+    def SendGroupMessage(self,group,message):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Referer':'https://im.popoim.com/im/h5/group/chat/%s'%group,
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
@@ -37,37 +37,37 @@
             "to": to,
             "content": content,
             "type": 'group',
             "uniqueId": "%s"%uniqueId
         }
         return loads(str(post(url,headers=headers,data=data).text))['data']
     
-    def GetInfo():
+    def GetInfo(self):
         url='https://im.popoim.com/web/pop/get'
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         return loads(str(get(url,headers=headers).text))['data']
        
-    def GetFriendsList():
+    def GetFriendsList(self):
         url='https://im.popoim.com/web/friend/getlist'
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         return loads(str(get(url,headers=headers).text))['data']
 
-    def SendFriendMessage(friend,message):
+    def SendFriendMessage(self,friend,message):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Referer':'https://im.popoim.com/im/h5/friend/chat/%s'%friend,
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
@@ -80,201 +80,201 @@
             "to": to,
             "content": content,
             "type": 'friend',
             "uniqueId": "%s"%uniqueId
         }
         return loads(str(post(url,headers=headers,data=data).text))['data']
 
-    def GetGroupMessage(group,limit=20):
+    def GetGroupMessage(self,group,limit=20):
         url='https://im.popoim.com/web/message/get?id=%s&type=group&limit=%s'%(group,limit)
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         return loads(str(get(url,headers=headers).text))['data']
     
-    def GetFriendMessage(friend,limit=20):
+    def GetFriendMessage(self,friend,limit=20):
         url='https://im.popoim.com/web/message/get?id=%s&type=friend&limit=%s'%(friend,limit)
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         return loads(str(get(url,headers=headers).text))['data']
         
-    def GetGroupList():
+    def GetGroupList(self):
         url='https://im.popoim.com/web/pop/get'
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         data= loads(str(get(url,headers=headers).text))['data']
         if 'group' in data:
             return data['group']
     
-    def GetSelfInfo():
+    def GetSelfInfo(self):
         url='https://im.popoim.com/web/pop/get'
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         data= loads(str(get(url,headers=headers).text))['data']
         if 'mine' in data:
             return data['mine']
         else:
             return {}
     
-    def GetChattings():
+    def GetChattings(self):
         url='https://im.popoim.com/web/pop/get'
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         data= loads(str(get(url,headers=headers).text))['data']
         if 'chatting' in data:
             return data['chatting']
         else:
             return {}
 
-    def GetApplyList():
+    def GetApplyList(self):
         url='https://im.popoim.com/web/friend/applylist'
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         return loads(str(get(url,headers=headers).text))['data']
     
-    def GetApplyDetail(nid):
+    def GetApplyDetail(self,nid):
         url='https://im.popoim.com/web/friend/applydetail?nid=%s'%nid
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         data= loads(str(get(url,headers=headers).text))['data']
         return data
     
-    def AgreeApply(nid):
+    def AgreeApply(self,nid):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
        }
         url='https://im.popoim.com/web/friend/agree'
         data = {
             'nid':nid
         }
         return loads(str(post(url,headers=headers,data=data).text))['data']
     
-    def GetGroupInfo(group):
+    def GetGroupInfo(self,group):
         url='https://im.popoim.com/web/group/detail?gid=%s'%group
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
         }
         data= loads(str(get(url,headers=headers).text))['data']
         return data
     
-    def GroupKick(group,friend):
+    def GroupKick(self,group,friend):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
        }
         url='https://im.popoim.com/web/group/memberdel'
         data = {
             'gid':group,
             'members[]':friend
         }
         return loads(str(post(url,headers=headers,data=data).text))['data']
     
-    def GroupInvite(group,friend):
+    def GroupInvite(self,group,friend):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
        }
         url='https://im.popoim.com/web/group/memberadd'
         data = {
             'gid':group,
             'members[]':friend
         }
         return loads(str(post(url,headers=headers,data=data).text))['data']
     
-    def GroupLeave(group):
+    def GroupLeave(self,group):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
        }
         url='https://im.popoim.com/web/group/leave'
         data = {
             'gid':group
         }
         return loads(str(post(url,headers=headers,data=data).text))['data']
         
-    def GroupDel(group):
+    def GroupDel(self,group):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
        }
         url='https://im.popoim.com/web/group/delete'
         data = {
             'gid':group
         }
         return loads(str(post(url,headers=headers,data=data).text))['data']
     
-    def RefuseApply(nid):
+    def RefuseApply(self,nid):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
        }
         url='https://im.popoim.com/web/friend/refuse'
         data = {
             'nid':nid
         }
         return loads(str(post(url,headers=headers,data=data).text))['data']
         
-    def Logout():
+    def Logout(self):
         headers = {
             'Origin':'https://im.popoim.com',
             'Host':'im.popoim.com',
             'Cookie':self.cookie,
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'X-Requested-With':'XMLHttpRequest'
        }
```

### Comparing `popobot-0.1/setup.py` & `popobot-0.2/setup.py`

 * *Files identical despite different names*

