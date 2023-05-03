# Comparing `tmp/openai_forward-0.1.4.tar.gz` & `tmp/openai_forward-0.1.5.tar.gz`

## Comparing `openai_forward-0.1.4.tar` & `openai_forward-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/__main__.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/_base.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/app.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/config.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openai_forward-0.1.4/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.4/LICENSE
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 openai_forward-0.1.4/README.md
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 openai_forward-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 openai_forward-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/__main__.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/_base.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/app.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/config.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 openai_forward-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.5/LICENSE
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 openai_forward-0.1.5/README.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openai_forward-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 openai_forward-0.1.5/PKG-INFO
```

### Comparing `openai_forward-0.1.4/openai_forward/_base.py` & `openai_forward-0.1.5/openai_forward/_base.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.4/openai_forward/app.py` & `openai_forward-0.1.5/openai_forward/app.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.4/openai_forward/config.py` & `openai_forward-0.1.5/openai_forward/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from loguru import logger
 import orjson
 from sparrow import relp
 from typing import Union, List, Dict
 import sys
 import logging
 import os
+import time
+import pytz
 
 
 class InterceptHandler(logging.Handler):
     def emit(self, record):
         # Get corresponding Loguru level if it exists
         try:
             level = logger.level(record.levelname).name
@@ -19,23 +21,36 @@
         frame, depth = logging.currentframe(), 2
         while frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
         logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
 
-def setting_log(log_name, multi_process=True):
+def setting_log(log_name, multi_process=True, time_zone='Asia/Shanghai'):
+    # TODO 修复时区配置
+    if time_zone == "Asia/Shanghai":
+        import datetime
+        tz = pytz.timezone(time_zone)
+        loc_dt = tz.localize(datetime.datetime.now())
+        offset = loc_dt.utcoffset()
+        # tzname, offset = loc_dt.strftime("%Z::%z").split("::")
+        # offset = loc_dt.strftime("%z")
+        # os.environ['TZ'] = f"UTC-{offset}"
+        os.environ['TZ'] = f"UTC-8"
+        print(os.environ['TZ'])
+        time.tzset()
+
     logging.root.handlers = [InterceptHandler()]
     for name in logging.root.manager.loggerDict.keys():
         logging.getLogger(name).handlers = []
         logging.getLogger(name).propagate = True
     logger_config = {
         "handlers": [
             {"sink": sys.stdout},
-            {"sink": relp(f"../Log/{log_name}"), "enqueue": multi_process, "rotation": "100 MB"},
+            {"sink": f"./Log/{log_name}", "enqueue": multi_process, "rotation": "100 MB"},
         ],
     }
     logger.configure(**logger_config)
 
 
 def yaml_dump(data, filepath, rel_path=False, mode='w'):
     abs_path = relp(filepath, parents=1) if rel_path else filepath
@@ -80,9 +95,10 @@
 
 def str2list(s: str, sep=' '):
     if s:
         return [i.strip() for i in s.split(sep) if i.strip()]
     else:
         return []
 
+
 def env2list(env_name: str, sep=" "):
     return str2list(os.environ.get(env_name, "").strip(), sep=sep)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openai_forward-0.1.4/openai_forward/openai.py` & `openai_forward-0.1.5/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.4/openai_forward/content/chat.py` & `openai_forward-0.1.5/openai_forward/content/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import orjson
 from orjson import JSONDecodeError
 from loguru import logger
 from httpx._decoders import LineDecoder
 from pathlib import Path
 from sparrow import relp
 from typing import List, Dict
+import os
 
 decoder = LineDecoder()
 
 
 def _parse_iter_line_content(line: str):
     line = line[6:]
     try:
@@ -44,25 +45,26 @@
             target_info['content'] += _parse_iter_line_content(line)
         else:
             logger.warning(f"line not startswith data: {line}")
     return target_info
 
 
 class ChatSaver:
-    def __init__(self, max_chat_size=2000, save_interval=2):
+    def __init__(self, max_chat_size=2000, save_interval=2, _dir='./Log'):
         self._chat_list = []
         self._file_idx = 0
         self._save_interval = save_interval
         self._max_chat_file_size = max_chat_size
         self._cur_chat_file_size = 0
+        self._log_dir = _dir
         self._init_chat_file()
 
     @property
     def chat_file(self):
-        return f"chat_{self._file_idx}.txt"
+        return os.path.join(self._log_dir, f"chat_{self._file_idx}.txt")
 
     def _init_chat_file(self):
         while Path(self.chat_file).exists():
             self._file_idx += 1
 
     def add_chat(self, chat_info: dict):
         logger.info(str(chat_info))
```

### Comparing `openai_forward-0.1.4/openai_forward/routers/schemas.py` & `openai_forward-0.1.5/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.4/.gitignore` & `openai_forward-0.1.5/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 run.sh
 ssl/
 chat.yaml
 chat_*.yaml
 
 .env.example
 Log/
+Log-caloi-top/
 dist/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `openai_forward-0.1.4/LICENSE` & `openai_forward-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.4/README.md` & `openai_forward-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.4/pyproject.toml` & `openai_forward-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,21 @@
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
 
 dependencies = [
     "loguru",
-    "sparrow-python>=0.1.1",
+    "sparrow-python>=0.1.2",
     "fastapi",
     "uvicorn",
     "orjson",
     "python-dotenv",
     "httpx",
+    "pytz"
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/beidongjiedeguang/openai-forward"
 Documentation = "https://github.com/beidongjiedeguang/openai-forward#openai-forward"
```

### Comparing `openai_forward-0.1.4/PKG-INFO` & `openai_forward-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.1.4
+Version: 0.1.5
 Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
@@ -14,15 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: fastapi
 Requires-Dist: httpx
 Requires-Dist: loguru
 Requires-Dist: orjson
 Requires-Dist: python-dotenv
-Requires-Dist: sparrow-python>=0.1.1
+Requires-Dist: pytz
+Requires-Dist: sparrow-python>=0.1.2
 Requires-Dist: uvicorn
 Provides-Extra: bard
 Requires-Dist: googlebard; extra == 'bard'
 Provides-Extra: chatgpt
 Requires-Dist: revchatgpt; extra == 'chatgpt'
 Provides-Extra: edge
 Requires-Dist: edgegpt; extra == 'edge'
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.1.4 Summary: ð Openai
+Metadata-Version: 2.1 Name: openai_forward Version: 0.1.5 Summary: ð Openai
 api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· streaming forward Project-URL:
 Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
 Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
 forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
 forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
 openai-forward Author-email: kunyuan
 gmail.com> License-File: LICENSE Keywords:
 chatgpt,fastapi,forward,openai,openai-api,openai-proxy,python,streaming-api
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6 Requires-Dist: fastapi Requires-Dist: httpx Requires-
 Dist: loguru Requires-Dist: orjson Requires-Dist: python-dotenv Requires-Dist:
-sparrow-python>=0.1.1 Requires-Dist: uvicorn Provides-Extra: bard Requires-
-Dist: googlebard; extra == 'bard' Provides-Extra: chatgpt Requires-Dist:
-revchatgpt; extra == 'chatgpt' Provides-Extra: edge Requires-Dist: edgegpt;
-extra == 'edge' Provides-Extra: ssl Requires-Dist: certbot; extra == 'ssl'
-Description-Content-Type: text/markdown [**ä¸­æ**](./README_ZH.md) |
-**English**
+pytz Requires-Dist: sparrow-python>=0.1.2 Requires-Dist: uvicorn Provides-
+Extra: bard Requires-Dist: googlebard; extra == 'bard' Provides-Extra: chatgpt
+Requires-Dist: revchatgpt; extra == 'chatgpt' Provides-Extra: edge Requires-
+Dist: edgegpt; extra == 'edge' Provides-Extra: ssl Requires-Dist: certbot;
+extra == 'ssl' Description-Content-Type: text/markdown [**ä¸­æ**](./
+README_ZH.md) | **English**
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                      image_size] [tests] [pypi_downloads]
```

