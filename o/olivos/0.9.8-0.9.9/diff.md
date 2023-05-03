# Comparing `tmp/olivos-0.9.8.tar.gz` & `tmp/olivos-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/olivos-0.9.8.tar", last modified: Mon May  2 05:59:50 2022, max compression
+gzip compressed data, was "dist/olivos-0.9.9.tar", last modified: Tue Jun 14 02:47:09 2022, max compression
```

## Comparing `olivos-0.9.8.tar` & `olivos-0.9.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 05:59:50.790981 olivos-0.9.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 05:59:50.786981 olivos-0.9.8/OlivOS/
--rw-r--r--   0 root         (0) root         (0)    54854 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/API.py
--rw-r--r--   0 root         (0) root         (0)     1362 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5848 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/accountAPI.py
--rw-r--r--   0 root         (0) root         (0)    24308 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/bootAPI.py
--rw-r--r--   0 root         (0) root         (0)     7379 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/bootDataAPI.py
--rw-r--r--   0 root         (0) root         (0)     7919 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/contentAPI.py
--rw-r--r--   0 root         (0) root         (0)   360998 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/data.py
--rw-r--r--   0 root         (0) root         (0)    14482 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/diagnoseAPI.py
--rw-r--r--   0 root         (0) root         (0)    25012 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/dodoLinkSDK.py
--rw-r--r--   0 root         (0) root         (0)     4285 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/dodoLinkServerAPI.py
--rw-r--r--   0 root         (0) root         (0)     7343 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/dodoPollServerAPI.py
--rw-r--r--   0 root         (0) root         (0)    13327 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/dodoSDK.py
--rw-r--r--   0 root         (0) root         (0)     6272 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/dodobotEASDK.py
--rw-r--r--   0 root         (0) root         (0)     5130 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/dodobotEAServerAPI.py
--rw-r--r--   0 root         (0) root         (0)     4408 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/dodobotEATXAPI.py
--rw-r--r--   0 root         (0) root         (0)     6466 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/fanbookPollServerAPI.py
--rw-r--r--   0 root         (0) root         (0)    15892 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/fanbookSDK.py
--rw-r--r--   0 root         (0) root         (0)     3373 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/flaskServerAPI.py
--rw-r--r--   0 root         (0) root         (0)      496 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/hook.py
--rw-r--r--   0 root         (0) root         (0)     1124 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/infoAPI.py
--rw-r--r--   0 root         (0) root         (0)     7502 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/kaiheilaLinkServerAPI.py
--rw-r--r--   0 root         (0) root         (0)    25016 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/kaiheilaSDK.py
--rw-r--r--   0 root         (0) root         (0)     6468 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/libEXEModelAPI.py
--rw-r--r--   0 root         (0) root         (0)    34804 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/messageAPI.py
--rw-r--r--   0 root         (0) root         (0)     5327 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/metadataAPI.py
--rw-r--r--   0 root         (0) root         (0)    33179 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/multiLoginUIAPI.py
--rw-r--r--   0 root         (0) root         (0)     1279 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/multiprocessing_win.py
--rw-r--r--   0 root         (0) root         (0)    58527 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/onebotSDK.py
--rw-r--r--   0 root         (0) root         (0)    22888 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/pluginAPI.py
--rw-r--r--   0 root         (0) root         (0)     6517 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/qqGuildLinkServerAPI.py
--rw-r--r--   0 root         (0) root         (0)    21798 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/qqGuildSDK.py
--rw-r--r--   0 root         (0) root         (0)     3277 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/telegramPollServerAPI.py
--rw-r--r--   0 root         (0) root         (0)    31671 2022-05-02 05:59:49.000000 olivos-0.9.8/OlivOS/telegramSDK.py
--rw-r--r--   0 root         (0) root         (0)     7030 2022-05-02 05:59:50.790981 olivos-0.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5895 2022-05-02 05:59:49.000000 olivos-0.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 05:59:50.790981 olivos-0.9.8/olivos.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7030 2022-05-02 05:59:50.000000 olivos-0.9.8/olivos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      926 2022-05-02 05:59:50.000000 olivos-0.9.8/olivos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-02 05:59:50.000000 olivos-0.9.8/olivos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      125 2022-05-02 05:59:50.000000 olivos-0.9.8/olivos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-05-02 05:59:50.000000 olivos-0.9.8/olivos.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-02 05:59:50.790981 olivos-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1441 2022-05-02 05:59:49.000000 olivos-0.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 02:47:09.461255 olivos-0.9.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 02:47:09.457254 olivos-0.9.9/OlivOS/
+-rw-r--r--   0 root         (0) root         (0)    55816 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/API.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5848 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/accountAPI.py
+-rw-r--r--   0 root         (0) root         (0)    24308 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/bootAPI.py
+-rw-r--r--   0 root         (0) root         (0)     7379 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/bootDataAPI.py
+-rw-r--r--   0 root         (0) root         (0)     7919 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/contentAPI.py
+-rw-r--r--   0 root         (0) root         (0)   360998 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/data.py
+-rw-r--r--   0 root         (0) root         (0)    14482 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/diagnoseAPI.py
+-rw-r--r--   0 root         (0) root         (0)    25012 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/dodoLinkSDK.py
+-rw-r--r--   0 root         (0) root         (0)     4285 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/dodoLinkServerAPI.py
+-rw-r--r--   0 root         (0) root         (0)     7343 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/dodoPollServerAPI.py
+-rw-r--r--   0 root         (0) root         (0)    13327 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/dodoSDK.py
+-rw-r--r--   0 root         (0) root         (0)     6272 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/dodobotEASDK.py
+-rw-r--r--   0 root         (0) root         (0)     5130 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/dodobotEAServerAPI.py
+-rw-r--r--   0 root         (0) root         (0)     4408 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/dodobotEATXAPI.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/fanbookPollServerAPI.py
+-rw-r--r--   0 root         (0) root         (0)    15892 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/fanbookSDK.py
+-rw-r--r--   0 root         (0) root         (0)     3373 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/flaskServerAPI.py
+-rw-r--r--   0 root         (0) root         (0)      496 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/hook.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/infoAPI.py
+-rw-r--r--   0 root         (0) root         (0)     7502 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/kaiheilaLinkServerAPI.py
+-rw-r--r--   0 root         (0) root         (0)    25016 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/kaiheilaSDK.py
+-rw-r--r--   0 root         (0) root         (0)     6468 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/libEXEModelAPI.py
+-rw-r--r--   0 root         (0) root         (0)    34804 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/messageAPI.py
+-rw-r--r--   0 root         (0) root         (0)     5327 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/metadataAPI.py
+-rw-r--r--   0 root         (0) root         (0)    33224 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/multiLoginUIAPI.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/multiprocessing_win.py
+-rw-r--r--   0 root         (0) root         (0)    58641 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/onebotSDK.py
+-rw-r--r--   0 root         (0) root         (0)    22888 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/pluginAPI.py
+-rw-r--r--   0 root         (0) root         (0)     6517 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/qqGuildLinkServerAPI.py
+-rw-r--r--   0 root         (0) root         (0)    22363 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/qqGuildSDK.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/telegramPollServerAPI.py
+-rw-r--r--   0 root         (0) root         (0)    31671 2022-06-14 02:47:08.000000 olivos-0.9.9/OlivOS/telegramSDK.py
+-rw-r--r--   0 root         (0) root         (0)     7030 2022-06-14 02:47:09.461255 olivos-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5895 2022-06-14 02:47:08.000000 olivos-0.9.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 02:47:09.461255 olivos-0.9.9/olivos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7030 2022-06-14 02:47:09.000000 olivos-0.9.9/olivos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      926 2022-06-14 02:47:09.000000 olivos-0.9.9/olivos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-14 02:47:09.000000 olivos-0.9.9/olivos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2022-06-14 02:47:09.000000 olivos-0.9.9/olivos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2022-06-14 02:47:09.000000 olivos-0.9.9/olivos.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-14 02:47:09.461255 olivos-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1441 2022-06-14 02:47:08.000000 olivos-0.9.9/setup.py
```

### Comparing `olivos-0.9.8/OlivOS/API.py` & `olivos-0.9.9/OlivOS/API.py`

 * *Files 8% similar despite different names*

```diff
@@ -486,15 +486,15 @@
         if flag_log and self.log_func != None:
             self.log_func(2, str(enable) , [
                 ('%s|%s' % (self.platform['platform'], str(self.base_info['self_id'])), 'default'),
                 (self.plugin_info['name'], 'default'),
                 ('set_block', 'callback')
             ])
 
-    def set_block(self, enable = True, flag_log = True, remote = False):
+    def set_block(self, enable: bool = True, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_block(enable, flag_log = True)
 
     def __message_router(self, message):
         tmp_message_obj = None
@@ -616,15 +616,15 @@
                 else:
                     self.log_func(2, 'Group(' + str(self.data.group_id) + '): ' + tmp_message_log, [
                         ('%s|%s' % (self.platform['platform'], str(self.base_info['self_id'])), 'default'),
                         (self.plugin_info['name'], 'default'),
                         ('reply', 'callback')
                     ])
 
-    def reply(self, message, flag_log = True, remote = False):
+    def reply(self, message, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__reply(message, flag_log = True)
 
 
     def __send(self, send_type, target_id, message, host_id = None, flag_log = True):
@@ -721,43 +721,43 @@
                 else:
                     self.log_func(2, 'Group(' + str(target_id) + '): ' + tmp_message_log, [
                         ('%s|%s' % (self.platform['platform'], str(self.base_info['self_id'])), 'default'),
                         (self.plugin_info['name'], 'default'),
                         ('send', 'callback')
                     ])
 
-    def send(self, send_type, target_id, message, host_id = None, flag_log = True, remote = False):
+    def send(self, send_type: str, target_id: 'str|int', message, host_id: 'str|int|None' = None, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__send(send_type, target_id, message, host_id = host_id, flag_log = True)
 
     @callbackLogger('delete_msg')
     def __delete_msg(self, message_id, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             OlivOS.onebotSDK.event_action.delete_msg(self, message_id)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def delete_msg(self, message_id, flag_log = True, remote = False):
+    def delete_msg(self, message_id: 'str|int', flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__delete_msg(message_id, flag_log = True)
 
     @callbackLogger('get_msg')
     def __get_msg(self, message_id, flag_log = True):
         res_data = None
         if self.platform['sdk'] == 'onebot':
             res_data = OlivOS.onebotSDK.event_action.get_msg(self, message_id)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
         return res_data
 
-    def get_msg(self, message_id, flag_log = True, remote = False):
+    def get_msg(self, message_id: 'str|int', flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_msg(message_id, flag_log = True)
         return res_data
 
@@ -765,193 +765,193 @@
     @callbackLogger('send_like')
     def __send_like(self, user_id, times, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             OlivOS.onebotSDK.event_action.send_like(self, user_id, times)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def send_like(self, user_id, times = 1, flag_log = True, remote = False):
+    def send_like(self, user_id: 'str|int', times: int = 1, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__send_like(user_id, times, flag_log = True)
 
 
     @callbackLogger('set_group_kick')
     def __set_group_kick(self, group_id, user_id, host_id, rehect_add_request, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_kick(self, group_id, user_id, rehect_add_request)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_kick(self, group_id, user_id, host_id = None, rehect_add_request = False, flag_log = True, remote = False):
+    def set_group_kick(self, group_id: 'str|int', user_id: 'str|int', host_id: 'str|int|None' = None, rehect_add_request: bool = False, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_kick(group_id, user_id, host_id, rehect_add_request, flag_log = True)
 
 
     @callbackLogger('set_group_ban')
     def __set_group_ban(self, group_id, user_id, host_id, duration, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_ban(self, group_id, user_id, duration)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_ban(self, group_id, user_id, host_id = None, duration = 1800, flag_log = True, remote = False):
+    def set_group_ban(self, group_id: 'str|int', user_id: 'str|int', host_id: 'str|int|None' = None, duration: int = 1800, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_ban(group_id, user_id, host_id, duration, flag_log = True)
 
 
     @callbackLogger('set_group_anonymous_ban')
     def __set_group_anonymous_ban(self, group_id, anonymous, anonymous_flag, host_id, duration, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_anonymous_ban(self, group_id, anonymous, anonymous_flag, duration)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_anonymous_ban(self, group_id, anonymous, anonymous_flag, host_id = None, duration = 1800, flag_log = True, remote = False):
+    def set_group_anonymous_ban(self, group_id: 'str|int', anonymous, anonymous_flag: str, host_id: 'str|int|None' = None, duration: int = 1800, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_anonymous_ban(group_id, anonymous, anonymous_flag, host_id, duration, flag_log = True)
 
 
     @callbackLogger('set_group_whole_ban')
     def __set_group_whole_ban(self, group_id, enable, host_id, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_whole_ban(self, group_id, enable)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_whole_ban(self, group_id, enable, host_id = None, flag_log = True, remote = False):
+    def set_group_whole_ban(self, group_id: 'str|int', enable: bool, host_id: 'str|int|None' = None, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_whole_ban(group_id, enable, host_id, flag_log = True)
 
 
     @callbackLogger('set_group_admin')
     def __set_group_admin(self, group_id, user_id, enable, host_id, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_admin(self, group_id, user_id, enable)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_admin(self, group_id, user_id, enable, host_id = None, flag_log = True, remote = False):
+    def set_group_admin(self, group_id: 'str|int', user_id: 'str|int', enable: bool, host_id: 'str|int|None' = None, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_admin(group_id, user_id, enable, host_id, flag_log = True)
 
 
     @callbackLogger('set_group_anonymous')
     def __set_group_anonymous(self, group_id, enable, host_id, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_anonymous(self, group_id, enable)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_anonymous(self, group_id, enable, host_id = None, flag_log = True, remote = False):
+    def set_group_anonymous(self, group_id: 'str|int', enable: bool, host_id: 'str|int' = None, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_anonymous(group_id, enable, host_id, flag_log = True)
 
 
     @callbackLogger('set_group_card')
     def __set_group_card(self, group_id, user_id, card, host_id, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_card(self, group_id, user_id, card)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_card(self, group_id, user_id, card, host_id = None, flag_log = True, remote = False):
+    def set_group_card(self, group_id: 'str|int', user_id: 'str|int', card, host_id: 'str|int|None' = None, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_card(group_id, user_id, card, host_id, flag_log = True)
 
 
     @callbackLogger('set_group_name')
     def __set_group_name(self, group_id, group_name, host_id, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_name(self, group_id, group_name)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_name(self, group_id, group_name, host_id = None, flag_log = True, remote = False):
+    def set_group_name(self, group_id: 'str|int', group_name: str, host_id: 'str|int|None' = None, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_name(group_id, group_name, host_id, flag_log = True)
 
 
     @callbackLogger('set_group_leave')
     def __set_group_leave(self, group_id, host_id, is_dismiss, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_leave(self, group_id, is_dismiss)
         elif self.platform['sdk'] == 'telegram_poll':
             OlivOS.telegramSDK.event_action.set_chat_leave(self, group_id, is_dismiss)
 
-    def set_group_leave(self, group_id, host_id = None, is_dismiss = False, flag_log = True, remote = False):
+    def set_group_leave(self, group_id: 'str|int', host_id: 'str|int|None' = None, is_dismiss: bool = False, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_leave(group_id, host_id, is_dismiss, flag_log = True)
 
 
     @callbackLogger('set_group_special_title')
     def __set_group_special_title(self, group_id, user_id, special_title, duration, host_id, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 OlivOS.onebotSDK.event_action.set_group_special_title(self, group_id, user_id, special_title, duration)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_special_title(self, group_id, user_id, special_title, duration, host_id = None, flag_log = True, remote = False):
+    def set_group_special_title(self, group_id: 'str|int', user_id: 'str|int', special_title: str, duration: int, host_id: 'str|int|None' = None, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_special_title(group_id, user_id, special_title, duration, host_id, flag_log = True)
 
 
     @callbackLogger('set_friend_add_request')
     def __set_friend_add_request(self, flag, approve, remark, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             OlivOS.onebotSDK.event_action.set_friend_add_request(self, flag, approve, remark)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_friend_add_request(self, flag, approve, remark, flag_log = True, remote = False):
+    def set_friend_add_request(self, flag: str, approve: bool, remark: str, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_friend_add_request(flag, approve, remark, flag_log = True)
 
 
     @callbackLogger('set_group_add_request')
     def __set_group_add_request(self, flag, sub_type, approve, reason, flag_log = True):
         if self.platform['sdk'] == 'onebot':
             OlivOS.onebotSDK.event_action.set_group_add_request(self, flag, sub_type, approve, reason)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
 
-    def set_group_add_request(self, flag, sub_type, approve, reason, flag_log = True, remote = False):
+    def set_group_add_request(self, flag: str, sub_type: str, approve: bool, reason: str, flag_log: bool = True, remote: bool = False):
         if remote:
             pass
         else:
             self.__set_group_add_request(flag, sub_type, approve, reason, flag_log = True)
 
 
     def __get_login_info(self, flag_log = True):
@@ -990,15 +990,15 @@
                     self.log_func(2, 'failed' , [
                         ('%s|%s' % (self.platform['platform'], str(self.base_info['self_id'])), 'default'),
                         (self.plugin_info['name'], 'default'),
                         ('get_login_info', 'callback')
                     ])
         return res_data
 
-    def get_login_info(self, flag_log = True, remote = False):
+    def get_login_info(self, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_login_info(flag_log = True)
         return res_data
 
@@ -1010,15 +1010,15 @@
             res_data = OlivOS.onebotSDK.event_action.get_stranger_info(self, user_id, no_cache)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
         elif self.platform['sdk'] == 'kaiheila_link':
             res_data = OlivOS.kaiheilaSDK.event_action.get_stranger_info(self, user_id)
         return res_data
 
-    def get_stranger_info(self, user_id, no_cache = False, flag_log = True, remote = False):
+    def get_stranger_info(self, user_id: 'str|int', no_cache: bool = False, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_stranger_info(user_id, no_cache, flag_log = True)
         return res_data
 
@@ -1028,15 +1028,15 @@
         res_data = None
         if self.platform['sdk'] == 'onebot':
             res_data = OlivOS.onebotSDK.event_action.get_friend_list(self)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
         return res_data
 
-    def get_friend_list(self, flag_log = True, remote = False):
+    def get_friend_list(self, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_friend_list(flag_log = True)
         return res_data
 
@@ -1047,15 +1047,15 @@
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 res_data = OlivOS.onebotSDK.event_action.get_group_info(self, group_id, no_cache)
         elif self.platform['sdk'] == 'telegram_poll':
             res_data = OlivOS.telegramSDK.event_action.get_group_info(self, group_id)
         return res_data
 
-    def get_group_info(self, group_id, host_id = None, no_cache = False, flag_log = True, remote = False):
+    def get_group_info(self, group_id: 'str|int', host_id: 'str|int|None' = None, no_cache: bool = False, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_group_info(group_id, host_id, no_cache, flag_log = True)
         return res_data
 
@@ -1065,15 +1065,15 @@
         res_data = None
         if self.platform['sdk'] == 'onebot':
             res_data = OlivOS.onebotSDK.event_action.get_group_list(self)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
         return res_data
 
-    def get_group_list(self, flag_log = True, remote = False):
+    def get_group_list(self, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_group_list(flag_log = True)
         return res_data
 
@@ -1088,15 +1088,15 @@
                 res_data = OlivOS.onebotSDK.event_action.get_guild_member_profile(self, host_id, user_id)
         elif self.platform['sdk'] == 'telegram_poll':
             res_data = OlivOS.telegramSDK.event_action.get_group_member_info(self, group_id, user_id)
         elif self.platform['sdk'] == 'kaiheila_link':
             res_data = OlivOS.kaiheilaSDK.event_action.get_group_member_info(self, host_id, user_id)
         return res_data
 
-    def get_group_member_info(self, group_id, user_id, host_id = None, no_cache = False, flag_log = True, remote = False):
+    def get_group_member_info(self, group_id: 'str|int', user_id: 'str|int', host_id: 'str|int|None' = None, no_cache: bool = False, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_group_member_info(group_id, user_id, host_id, no_cache, flag_log = True)
         return res_data
 
@@ -1107,15 +1107,15 @@
         if self.platform['sdk'] == 'onebot':
             if host_id == None:
                 res_data = OlivOS.onebotSDK.event_action.get_group_member_list(self, group_id)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
         return res_data
 
-    def get_group_member_list(self, group_id, host_id = None, flag_log = True, remote = False):
+    def get_group_member_list(self, group_id: 'str|int', host_id: 'str|int|None' = None, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_group_member_list(group_id, host_id, flag_log = True)
         return res_data
 
@@ -1125,15 +1125,15 @@
         res_data = None
         if self.platform['sdk'] == 'onebot':
             res_data = OlivOS.onebotSDK.event_action.can_send_image(self)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
         return res_data
 
-    def can_send_image(self, flag_log = True, remote = False):
+    def can_send_image(self, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__can_send_image(flag_log = True)
         return res_data
 
@@ -1143,15 +1143,15 @@
         res_data = None
         if self.platform['sdk'] == 'onebot':
             res_data = OlivOS.onebotSDK.event_action.can_send_record(self)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
         return res_data
 
-    def can_send_record(self, flag_log = True, remote = False):
+    def can_send_record(self, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__can_send_record(flag_log = True)
         return res_data
 
@@ -1161,15 +1161,15 @@
         res_data = None
         if self.platform['sdk'] == 'onebot':
             res_data = OlivOS.onebotSDK.event_action.get_status(self)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
         return res_data
 
-    def get_status(self, flag_log = True, remote = False):
+    def get_status(self, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_status(flag_log = True)
         return res_data
 
@@ -1179,15 +1179,15 @@
         res_data = None
         if self.platform['sdk'] == 'onebot':
             res_data = OlivOS.onebotSDK.event_action.get_version_info(self)
         elif self.platform['sdk'] == 'telegram_poll':
             pass
         return res_data
 
-    def get_version_info(self, flag_log = True, remote = False):
+    def get_version_info(self, flag_log: bool = True, remote: bool = False):
         res_data = None
         if remote:
             pass
         else:
             res_data = self.__get_version_info(flag_log = True)
         return res_data
```

### Comparing `olivos-0.9.8/OlivOS/__init__.py` & `olivos-0.9.9/OlivOS/__init__.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/accountAPI.py` & `olivos-0.9.9/OlivOS/accountAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/bootAPI.py` & `olivos-0.9.9/OlivOS/bootAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/bootDataAPI.py` & `olivos-0.9.9/OlivOS/bootDataAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/contentAPI.py` & `olivos-0.9.9/OlivOS/contentAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/data.py` & `olivos-0.9.9/OlivOS/data.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/diagnoseAPI.py` & `olivos-0.9.9/OlivOS/diagnoseAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/dodoLinkSDK.py` & `olivos-0.9.9/OlivOS/dodoLinkSDK.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/dodoLinkServerAPI.py` & `olivos-0.9.9/OlivOS/dodoLinkServerAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/dodoPollServerAPI.py` & `olivos-0.9.9/OlivOS/dodoPollServerAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/dodoSDK.py` & `olivos-0.9.9/OlivOS/dodoSDK.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/dodobotEASDK.py` & `olivos-0.9.9/OlivOS/dodobotEASDK.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/dodobotEAServerAPI.py` & `olivos-0.9.9/OlivOS/dodobotEAServerAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/dodobotEATXAPI.py` & `olivos-0.9.9/OlivOS/dodobotEATXAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/fanbookPollServerAPI.py` & `olivos-0.9.9/OlivOS/fanbookPollServerAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/fanbookSDK.py` & `olivos-0.9.9/OlivOS/fanbookSDK.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/flaskServerAPI.py` & `olivos-0.9.9/OlivOS/flaskServerAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/infoAPI.py` & `olivos-0.9.9/OlivOS/infoAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 @Copyright :   (C) 2020-2021, OlivOS-Team
 @Desc      :   None
 '''
 
 import OlivOS
 
 
-OlivOS_Version = '0.9.8'
-OlivOS_SVN = 95
+OlivOS_Version = '0.9.9'
+OlivOS_SVN = 96
 
 # Compatible    <= Plugin[compatible_svn]                 : Compatible
 # OldCompatible <= Plugin[compatible_svn] < Compatible    : OldCompatible Warn
 #                  Plugin[compatible_svn] < OldCompatible : NotCompatible Error & Skip
 OlivOS_SVN_Compatible = 95
 OlivOS_SVN_OldCompatible = -1
 OlivOS_compatible_svn_default = 0
```

### Comparing `olivos-0.9.8/OlivOS/kaiheilaLinkServerAPI.py` & `olivos-0.9.9/OlivOS/kaiheilaLinkServerAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/kaiheilaSDK.py` & `olivos-0.9.9/OlivOS/kaiheilaSDK.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/libEXEModelAPI.py` & `olivos-0.9.9/OlivOS/libEXEModelAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/messageAPI.py` & `olivos-0.9.9/OlivOS/messageAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/metadataAPI.py` & `olivos-0.9.9/OlivOS/metadataAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/multiLoginUIAPI.py` & `olivos-0.9.9/OlivOS/multiLoginUIAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,21 +292,23 @@
         ]
         self.UIData['edit_root_Combobox_dict']['platform_sdk_list']['fanbook'] = [
             'fanbook_poll'
         ]
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list'] = {}
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list']['qq'] = {}
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list']['qq']['onebot'] = [
-            'default',
             #'gocqhttp',
             #'gocqhttp_hide',
-            'gocqhttp_show'
+            'gocqhttp_show',
+            'default'
         ]
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list']['qqGuild'] = {}
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list']['qqGuild']['qqGuild_link'] = [
+            'private',
+            'public',
             'default'
         ]
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list']['kaiheila'] = {}
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list']['kaiheila']['kaiheila_link'] = [
             'default'
         ]
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list']['telegram'] = {}
@@ -326,16 +328,16 @@
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list']['fanbook'] = {}
         self.UIData['edit_root_Combobox_dict']['platform_sdk_model_list']['fanbook']['fanbook_poll'] = [
             'default',
             'private'
         ]
 
         self.UIData['edit_root_Combobox_Server_auto_list'] = [
-            'False',
-            'True'
+            'True',
+            'False'
         ]
 
         self.UIData['edit_root_Combobox_Server_type_list'] = [
             'post',
             'websocket'
         ]
```

### Comparing `olivos-0.9.8/OlivOS/multiprocessing_win.py` & `olivos-0.9.9/OlivOS/multiprocessing_win.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/onebotSDK.py` & `olivos-0.9.9/OlivOS/onebotSDK.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,17 @@
                 target_event.active = True
                 target_event.plugin_info['func_type'] = 'poke'
                 target_event.data = target_event.poke(
                     str(target_event.sdk_event.json['user_id']),
                     str(target_event.sdk_event.json['target_id'])
                 )
                 if 'group_id' in target_event.sdk_event.json:
-                    target_event.data.group_id = target_event.sdk_event.json['group_id']
+                    target_event.data.group_id = str(target_event.sdk_event.json['group_id'])
+                if target_event.data.group_id == '-1':
+                    target_event.data.group_id = None
             elif target_event.sdk_event.json['sub_type'] == 'lucky_king':
                 target_event.active = True
                 target_event.plugin_info['func_type'] = 'group_lucky_king'
                 target_event.data = target_event.group_lucky_king(
                     str(target_event.sdk_event.json['group_id']),
                     str(target_event.sdk_event.json['user_id']),
                     str(target_event.sdk_event.json['target_id'])
```

### Comparing `olivos-0.9.8/OlivOS/pluginAPI.py` & `olivos-0.9.9/OlivOS/pluginAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/qqGuildLinkServerAPI.py` & `olivos-0.9.9/OlivOS/qqGuildLinkServerAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/qqGuildSDK.py` & `olivos-0.9.9/OlivOS/qqGuildSDK.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,26 +39,29 @@
     'channel_id': '-1',
     'user_id': '-1'
 }
 
 sdkSubSelfInfo = {}
 
 class bot_info_T(object):
-    def __init__(self, id = -1, access_token = None):
+    def __init__(self, id = -1, access_token = None, model = 'private'):
         self.id = id
         self.access_token = access_token
+        self.model = model
         self.debug_mode = False
         self.debug_logger = None
 
 def get_SDK_bot_info_from_Plugin_bot_info(plugin_bot_info):
     res = bot_info_T(
         plugin_bot_info.id,
         plugin_bot_info.post_info.access_token
     )
     res.debug_mode = plugin_bot_info.debug_mode
+    if plugin_bot_info.platform['model'] == 'public':
+        res.model = 'public'
     return res
 
 def get_SDK_bot_info_from_Event(target_event):
     res = bot_info_T(
         target_event.bot_info.id,
         target_event.bot_info.post_info.access_token
     )
@@ -136,21 +139,24 @@
 
 class PAYLOAD(object):
     class rxPacket(payload_template):
         def __init__(self, data):
             payload_template.__init__(self, data, True)
 
     class sendIdentify(payload_template):
-        def __init__(self, bot_info, intents = (1 << 0 | 1 << 9 | 1 << 12 | 1 << 30)):
+        def __init__(self, bot_info, intents = (1 << 0 | 1 << 12 | 1 << 30)):
+            tmp_intents = intents
+            if bot_info.model == 'private':
+                tmp_intents |= (1 << 9)
             payload_template.__init__(self)
             self.data.op = 2
             try:
                 self.data.d = {
                     'token': 'Bot %s.%s' % (str(bot_info.id), bot_info.access_token),
-                    'intents': intents,
+                    'intents': tmp_intents,
                     'shard': [0,1],
                     'properties': {
                         'os': OlivOS.infoAPI.OlivOS_Header_UA
                     }
                 }
             except:
                 self.active = False
@@ -335,15 +341,18 @@
         api_msg_obj = API.getMe(tmp_bot_info)
         try:
             api_msg_obj.do_api('GET')
             api_res_json = json.loads(api_msg_obj.res)
             sdkSubSelfInfo[plugin_event_bot_hash] = api_res_json['id']
         except:
             pass
-    if target_event.sdk_event.payload.data.t == 'MESSAGE_CREATE':
+    if target_event.sdk_event.payload.data.t in [
+        'MESSAGE_CREATE',
+        'AT_MESSAGE_CREATE'
+    ]:
         message_obj = None
         message_para_list = []
         if 'content' in target_event.sdk_event.payload.data.d:
             if target_event.sdk_event.payload.data.d['content'] != '':
                 message_obj = OlivOS.messageAPI.Message_templet(
                     'qqGuild_string',
                     target_event.sdk_event.payload.data.d['content']
@@ -351,14 +360,19 @@
                 message_obj.mode_rx = target_event.plugin_info['message_mode_rx']
                 message_obj.data_raw = message_obj.data.copy()
             else:
                 message_obj = OlivOS.messageAPI.Message_templet(
                     'olivos_para',
                     []
                 )
+        else:
+            message_obj = OlivOS.messageAPI.Message_templet(
+                'olivos_para',
+                []
+            )
         if 'attachments' in target_event.sdk_event.payload.data.d:
             if type(target_event.sdk_event.payload.data.d['attachments']) == list:
                 for attachments_this in target_event.sdk_event.payload.data.d['attachments']:
                     if 'content_type' in attachments_this:
                         if attachments_this['content_type'].startswith('image'):
                             message_obj.data_raw.append(
                                 OlivOS.messageAPI.PARA.image(
@@ -421,14 +435,19 @@
                 message_obj.mode_rx = target_event.plugin_info['message_mode_rx']
                 message_obj.data_raw = message_obj.data.copy()
             else:
                 message_obj = OlivOS.messageAPI.Message_templet(
                     'olivos_para',
                     []
                 )
+        else:
+            message_obj = OlivOS.messageAPI.Message_templet(
+                'olivos_para',
+                []
+            )
         if 'attachments' in target_event.sdk_event.payload.data.d:
             if type(target_event.sdk_event.payload.data.d['attachments']) == list:
                 for attachments_this in target_event.sdk_event.payload.data.d['attachments']:
                     if 'content_type' in attachments_this:
                         if attachments_this['content_type'].startswith('image'):
                             message_obj.data_raw.append(
                                 OlivOS.messageAPI.PARA.image(
```

### Comparing `olivos-0.9.8/OlivOS/telegramPollServerAPI.py` & `olivos-0.9.9/OlivOS/telegramPollServerAPI.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/OlivOS/telegramSDK.py` & `olivos-0.9.9/OlivOS/telegramSDK.py`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/PKG-INFO` & `olivos-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olivos
-Version: 0.9.8
+Version: 0.9.9
 Summary: OlivOS - Witness Union
 Home-page: https://github.com/OlivOS-Team/OlivOS
 Author: OlivOS-Team
 Author-email: lunzhipenxil@gmail.com
 License: AGPLv3 License
 Description: <p align="center">
           <a href="#">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olivos Version: 0.9.8 Summary: OlivOS - Witness
+Metadata-Version: 2.1 Name: olivos Version: 0.9.9 Summary: OlivOS - Witness
 Union Home-page: https://github.com/OlivOS-Team/OlivOS Author: OlivOS-Team
 Author-email: lunzhipenxil@gmail.com License: AGPLv3 License Description:
  # OlivOS **éææ ¸å¿äº¤äºæ ** **Witness Union / è§è¯èå** [action]
                           [action] [PyPI] [Downloads]
                                ææ¡£ Â· ä¸è½½
 ## å¼å®¹ [![QQGuild](https://img.shields.io/badge/-QQGuild-EB1923?style=flat-
 square&logo=Tencent%20QQ&logoColor=white)](https://bot.q.qq.com/wiki/) [!
```

### Comparing `olivos-0.9.8/README.md` & `olivos-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/olivos.egg-info/PKG-INFO` & `olivos-0.9.9/olivos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olivos
-Version: 0.9.8
+Version: 0.9.9
 Summary: OlivOS - Witness Union
 Home-page: https://github.com/OlivOS-Team/OlivOS
 Author: OlivOS-Team
 Author-email: lunzhipenxil@gmail.com
 License: AGPLv3 License
 Description: <p align="center">
           <a href="#">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olivos Version: 0.9.8 Summary: OlivOS - Witness
+Metadata-Version: 2.1 Name: olivos Version: 0.9.9 Summary: OlivOS - Witness
 Union Home-page: https://github.com/OlivOS-Team/OlivOS Author: OlivOS-Team
 Author-email: lunzhipenxil@gmail.com License: AGPLv3 License Description:
  # OlivOS **éææ ¸å¿äº¤äºæ ** **Witness Union / è§è¯èå** [action]
                           [action] [PyPI] [Downloads]
                                ææ¡£ Â· ä¸è½½
 ## å¼å®¹ [![QQGuild](https://img.shields.io/badge/-QQGuild-EB1923?style=flat-
 square&logo=Tencent%20QQ&logoColor=white)](https://bot.q.qq.com/wiki/) [!
```

### Comparing `olivos-0.9.8/olivos.egg-info/SOURCES.txt` & `olivos-0.9.9/olivos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `olivos-0.9.8/setup.py` & `olivos-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import setuptools
 
 with open('README.md', 'r', encoding = 'utf-8') as f:
   long_description = f.read()
 
 setuptools.setup(name='olivos',
-    version='0.9.8',
+    version='0.9.9',
     description='OlivOS - Witness Union',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='OlivOS-Team',
     author_email='lunzhipenxil@gmail.com',
     url='https://github.com/OlivOS-Team/OlivOS',
     install_requires=[
```

