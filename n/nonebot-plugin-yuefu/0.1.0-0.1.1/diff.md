# Comparing `tmp/nonebot_plugin_yuefu-0.1.0.tar.gz` & `tmp/nonebot_plugin_yuefu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_yuefu-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_yuefu-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_yuefu-0.1.0.tar` & `nonebot_plugin_yuefu-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11558 2023-05-03 19:31:58.315599 nonebot_plugin_yuefu-0.1.0/LICENSE
--rw-r--r--   0        0        0     3162 2023-05-03 19:55:34.748396 nonebot_plugin_yuefu-0.1.0/nonebot_plugin_yuefu/__init__.py
--rw-r--r--   0        0        0      258 2023-05-03 19:38:56.720067 nonebot_plugin_yuefu-0.1.0/nonebot_plugin_yuefu/config.py
--rw-r--r--   0        0        0      416 2023-05-03 20:07:07.181431 nonebot_plugin_yuefu-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2379 2023-05-03 19:34:08.294443 nonebot_plugin_yuefu-0.1.0/README.md
--rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 nonebot_plugin_yuefu-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-05-03 19:31:58.315599 nonebot_plugin_yuefu-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3164 2023-05-03 20:25:08.333970 nonebot_plugin_yuefu-0.1.1/nonebot_plugin_yuefu/__init__.py
+-rw-r--r--   0        0        0      258 2023-05-03 19:38:56.720067 nonebot_plugin_yuefu-0.1.1/nonebot_plugin_yuefu/config.py
+-rw-r--r--   0        0        0      416 2023-05-03 20:25:15.497687 nonebot_plugin_yuefu-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2379 2023-05-03 19:34:08.294443 nonebot_plugin_yuefu-0.1.1/README.md
+-rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 nonebot_plugin_yuefu-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_yuefu-0.1.0/LICENSE` & `nonebot_plugin_yuefu-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_yuefu-0.1.0/nonebot_plugin_yuefu/__init__.py` & `nonebot_plugin_yuefu-0.1.1/nonebot_plugin_yuefu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nonebot import logger
 
 from .config import Config
 
 global_config = get_driver().config
 config = Config.parse_obj(global_config)
 
-voice = on_command("说", aliases={"语音"}, block=True, priority=4)
+voice = on_command("speak", aliases={"府说"}, block=True, priority=4)
 
 
 def speech_synthesis_to_wave_file(text: str):
     subscription_key = config.SPEECH_KEY
     region = config.SPEECH_REGION
     print(f'KEY：{subscription_key}, REGION:{region}')
```

### Comparing `nonebot_plugin_yuefu-0.1.0/README.md` & `nonebot_plugin_yuefu-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_yuefu-0.1.0/PKG-INFO` & `nonebot_plugin_yuefu-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-yuefu
-Version: 0.1.0
+Version: 0.1.1
 Summary: AI乐府Nonebot插件
 Author: Chengzhi
 Author-email: zmq175@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-yuefu Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-yuefu Version: 0.1.1 Summary:
 AIä¹åºNonebotæä»¶ Author: Chengzhi Author-email: zmq175@qq.com Requires-
 Python: >=3.9,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0) Requires-Dist: nonebot2
 (>=2.0.0b1,<3.0.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
```

