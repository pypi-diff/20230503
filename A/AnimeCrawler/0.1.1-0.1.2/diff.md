# Comparing `tmp/AnimeCrawler-0.1.1.tar.gz` & `tmp/AnimeCrawler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnimeCrawler-0.1.1.tar", last modified: Thu Apr 20 12:53:34 2023, max compression
+gzip compressed data, was "AnimeCrawler-0.1.2.tar", last modified: Wed May  3 03:36:47 2023, max compression
```

## Comparing `AnimeCrawler-0.1.1.tar` & `AnimeCrawler-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.212812 AnimeCrawler-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.093887 AnimeCrawler-0.1.1/AnimeCrawler/
--rw-rw-rw-   0        0        0      248 2023-04-18 15:03:38.000000 AnimeCrawler-0.1.1/AnimeCrawler/__init__.py
--rw-rw-rw-   0        0        0      311 2023-04-19 14:06:47.000000 AnimeCrawler-0.1.1/AnimeCrawler/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.167838 AnimeCrawler-0.1.1/AnimeCrawler/command/
--rw-rw-rw-   0        0        0       87 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/command/__init__.py
--rw-rw-rw-   0        0        0     3542 2023-04-20 12:45:39.000000 AnimeCrawler-0.1.1/AnimeCrawler/command/run.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.194822 AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/
--rw-rw-rw-   0        0        0      245 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/__init__.py
--rw-rw-rw-   0        0        0     2024 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/downloader.py
--rw-rw-rw-   0        0        0     3846 2023-04-19 13:04:13.000000 AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/spider.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.205821 AnimeCrawler-0.1.1/AnimeCrawler/utils/
--rw-rw-rw-   0        0        0      113 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/utils/__init__.py
--rw-rw-rw-   0        0        0      804 2023-04-17 15:39:52.000000 AnimeCrawler-0.1.1/AnimeCrawler/utils/decode.py
--rw-rw-rw-   0        0        0     2131 2023-04-19 13:15:05.000000 AnimeCrawler-0.1.1/AnimeCrawler/utils/file.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:53:34.147849 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/
--rw-rw-rw-   0        0        0     3411 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-20 12:53:33.000000 AnimeCrawler-0.1.1/AnimeCrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3411 2023-04-20 12:53:34.208814 AnimeCrawler-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2962 2023-04-20 12:31:36.000000 AnimeCrawler-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 12:53:34.213812 AnimeCrawler-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-04-20 12:52:40.000000 AnimeCrawler-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.215752 AnimeCrawler-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.136797 AnimeCrawler-0.1.2/AnimeCrawler/
+-rw-rw-rw-   0        0        0      353 2023-05-03 02:47:47.000000 AnimeCrawler-0.1.2/AnimeCrawler/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/__main__.py
+-rw-rw-rw-   0        0        0     2198 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/base_spider.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.185769 AnimeCrawler-0.1.2/AnimeCrawler/command/
+-rw-rw-rw-   0        0        0       76 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/command/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-05-03 03:12:56.000000 AnimeCrawler-0.1.2/AnimeCrawler/command/run.py
+-rw-rw-rw-   0        0        0      356 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/log.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.193771 AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/
+-rw-rw-rw-   0        0        0      256 2023-05-03 02:47:31.000000 AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/__init__.py
+-rw-rw-rw-   0        0        0     2286 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/downloader.py
+-rw-rw-rw-   0        0        0     4172 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/spider.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.211754 AnimeCrawler-0.1.2/AnimeCrawler/utils/
+-rw-rw-rw-   0        0        0      121 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/utils/decode.py
+-rw-rw-rw-   0        0        0     2154 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/utils/file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.179773 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/
+-rw-rw-rw-   0        0        0     3406 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3406 2023-05-03 03:36:47.213753 AnimeCrawler-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2957 2023-05-03 02:19:56.000000 AnimeCrawler-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 03:36:47.215752 AnimeCrawler-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-05-03 03:31:04.000000 AnimeCrawler-0.1.2/setup.py
```

### Comparing `AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/downloader.py` & `AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/downloader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 import asyncio
 
 import aiohttp
 import tqdm.asyncio
 
+from AnimeCrawler.log import get_logger
 from AnimeCrawler.utils import write
 
 
 class Downloader:
     session = None
-
-    def __init__(self, urls):
-        self.urls = urls
+    logger = get_logger('Downloader')
 
     @property
-    def current_sesion(self):
+    def current_session(self):
         if not self.session:
             self.session = aiohttp.ClientSession(
-                connector=aiohttp.TCPConnector(limit=40, verify_ssl=False)
+                connector = aiohttp.TCPConnector(verify_ssl=False)
             )
+            self.logger.debug('创建了session')
         return self.session
 
+    @property
+    def set_url(self, urls):
+        return urls
+
+    @set_url.setter
+    def set_url(self, urls):
+        self.urls = urls
+
+    async def close_session(self):
+        await self.current_session.close()
+
     async def get_ts_file(
         self,
+        session: aiohttp.ClientSession,
         title: str,
         url: str,
         error_times: int = 1,
     ):
-        resp = await self.current_sesion.get(
+        resp = await session.get(
             url=url,
             headers={'User-Agent': 'Mozilla/5.0', ' Transfer-Encoding': 'chunked'},
         )
         try:
             text = await resp.content.read()
+            await asyncio.sleep(0)
             return (text, title)
         except aiohttp.ClientPayloadError as e:  # 报错时重新下载
             if error_times == 3:
                 raise Warning(f'下载{title}.ts时发生错误') from e
             print(f'下载{title}.ts时发生错误，正在重试第{error_times}次')
-            return await self.get_ts_file(title, url, error_times + 1)
+            return await self.get_ts_file(session, title, url, error_times + 1)
         except Exception as e:
-            print(f'下载{title}.ts时发生{e}')
-            await asyncio.sleep(0)
+            raise ValueError(f'下载{title}.ts时，{e}') from e
         finally:
             resp.close()
 
-    async def close_session(self):
-        if self.session:
-            await self.session.close()
-
     async def download_ts_files(self, path, episodes):
         tasks = [
-            self.get_ts_file(str(index).zfill(4), url)
+            self.get_ts_file(self.current_session, str(index).zfill(4), url)
             for index, url in enumerate(self.urls)
         ]
-        for task in tqdm.asyncio.tqdm.as_completed(tasks, desc=f"正在下载第{episodes}集视频"):
+        for task in tqdm.asyncio.tqdm.as_completed(
+            tasks, desc=f"正在下载第{episodes}集视频", delay=3
+        ):
             result = await task
             text_1, title = (
                 (b'error', 'error') if result is None else result
             )  # result为空时返回'error'
             await write(path, text_1, title, suffix='ts', mode='wb')
-        await self.close_session()
```

### Comparing `AnimeCrawler-0.1.1/AnimeCrawler/mhyyy/spider.py` & `AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 from pathlib import Path
 
-from ruia import Item, Response, Spider, TextField
+from ruia import Item, Response, TextField
 
+from AnimeCrawler.base_spider import BaseSpider
+from AnimeCrawler.log import get_logger
 from AnimeCrawler.utils import (
     base64_decode,
     folder_path,
     get_video_path,
     merge_ts2mp4,
     unescape,
     write,
@@ -19,42 +21,43 @@
     target_item = TextField(xpath_select='//div[@class="player-box-main"]')
     profile = TextField(xpath_select='//div/script[@type="text/javascript"]')
     episodes = None
     _base_m3u8_url = None
     mixed_m3u8_url = None
 
 
-class AnimeSpider(Spider):
+class AnimeSpider(BaseSpider):
     _base_ts_url = None
     _mixed_m3u8 = None
+    downloader = Downloader()
     headers = {'User-Agent': 'Mozilla/5.0'}
 
     @classmethod
-    def init(cls, anime_title: str, start_urls: str, del_ts: bool = False):
+    def init(cls, anime_title: str, urls: str, del_ts: bool = False):
         '''初始化爬虫
 
         Args:
             anime_title (str): 动漫标题，用于取文件夹的名称，利于管理动漫
-            start_urls (str): 第一页的网址
+            urls (str): 第一页的网址
 
         Returns:
             cls: 为了链式调用返回了cls
         '''
-        cls.start_urls = [start_urls]
+        cls.domain = cls.get_domain(cls, urls)
+        cls.start_urls = [cls.get_path(cls, urls)]
+        cls.PATH = folder_path(Path(get_video_path()) / anime_title)
         cls.del_ts = del_ts
-        video_path = Path(get_video_path()) / anime_title  # 在项目目录下存储
-        cls.PATH = folder_path(video_path)
-        return cls
+        return super().init()
 
     async def _mixed_m3u8_url_parse(self, index_m3u8_url: str, item: AnimeItem) -> None:
         resp = await self.request(index_m3u8_url).fetch()
         text = await resp.text()
         if self._mixed_m3u8 is None:
             self._mixed_m3u8 = text.split('\n')[-1]
-        item.mixed_m3u8_url = item._base_m3u8_url + self._mixed_m3u8
+        item.mixed_m3u8_url = await self.urljoin(item._base_m3u8_url, self._mixed_m3u8)
 
     def _parse_mixed_m3u8(self, item: AnimeItem):
         '''解析mixed.m3u8文件，获得ts文件下载地址
 
         Returns:
             str：ts_url
         '''
@@ -63,16 +66,16 @@
             for i in fp:
                 if '#' not in i:
                     yield base_ts_file + i
 
     async def have_next_page(self, link_next: str):
         # 当有下一页时
         link_next = link_next.replace('\\', '')
-        return self.request(
-            'https://www.mhyyy.com' + link_next,
+        return await self.follow(
+            await self.urljoin(self.domain, link_next),
             callback=self.parse,
             headers=self.headers,
         )
 
     async def parse(self, response: Response):
         async for item in AnimeItem.get_items(html=await response.text()):
             profile = item.profile
@@ -91,17 +94,22 @@
             yield item
 
     async def process_item(self, item: AnimeItem):
         resp = await self.request(item.mixed_m3u8_url, headers=self.headers).fetch()
         text = await resp.text()
         episodes = item.episodes
         folder_path = self.PATH / f'{episodes}'
-        print('\033[0;32;40m写入mixed.m3u8\033[0m')
+        self.logger.info('\033[0;32;40m写入mixed.m3u8\033[0m')
         await write(folder_path, text, 'mixed', 'm3u8', 'w+')
         urls = self._parse_mixed_m3u8(item)
-        await Downloader(urls).download_ts_files(folder_path, episodes)
+        self.downloader.set_url = urls
+        await self.downloader.download_ts_files(folder_path, episodes)
         self.logger.info(f"正在把第 {episodes} 集的ts文件转码成 mp4")
         await merge_ts2mp4(folder_path, episodes, self.del_ts)
 
+    async def stop(self, _signal):
+        await self.downloader.close_session()
+        return await super().stop(_signal)
+
 
 if __name__ == '__main__':
     AnimeSpider.init('魔女之旅', ['https://www.mhyyy.com/play/166269-1-1.html']).start()
```

### Comparing `AnimeCrawler-0.1.1/AnimeCrawler/utils/decode.py` & `AnimeCrawler-0.1.2/AnimeCrawler/utils/decode.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,34 @@
 import html
 import re
 import urllib.parse
 from base64 import b64decode
 
 
+def is_url(string: str):
+    '''解析是否为url
+
+    Args:
+        string (str): 要解析的字符串
+
+    Returns:
+        bool: 用于判断
+    '''
+    pattern = re.compile(
+        r'^(?:http|ftp)s?://'  # http:// or https://
+        r'(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|'  # domain...
+        r'localhost|'  # localhost...
+        r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'  # ...or ip
+        r'(?::\d+)?'  # optional port
+        r'(?:/?|[/?]\S+)$',
+        re.IGNORECASE,
+    )
+    return bool(re.search(pattern, string))
+
+
 def base64_decode(string: str) -> str:
     '''对base64.b64decode()的包装
 
     Arguments:
         string -- 要解码的字符串
 
     Returns:
```

### Comparing `AnimeCrawler-0.1.1/AnimeCrawler/utils/file.py` & `AnimeCrawler-0.1.2/AnimeCrawler/utils/file.py`

 * *Files 18% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 async def merge_ts2mp4(folder_path: Path, episodes: int = None, del_ts: bool = False):
     '''将ts文件合并成mp4
 
     Args:
         folder_path (Path): 文件夹路径，里面应有ts文件
         episodes (int): 动漫集数. Defaults to None.
     '''
-    print(del_ts)
     for file_path in folder_path.iterdir():
         if file_path.suffix == '.ts':
-            with open(file_path, 'rb') as f1:
-                with open(folder_path / f"第{episodes}集.mp4", 'ab') as f2:
-                    f2.write(f1.read())
+            async with aiofiles.open(file_path, 'rb') as f1:
+                async with aiofiles.open(folder_path / f"第{episodes}集.mp4", 'ab') as f2:
+                    await f2.write(await f1.read())
             if del_ts:
                 file_path.unlink()
```

### Comparing `AnimeCrawler-0.1.1/AnimeCrawler.egg-info/PKG-INFO` & `AnimeCrawler-0.1.2/AnimeCrawler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.1.1
+Version: 0.1.2
 Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,16 +28,16 @@
 
 这是一款在Windows平台下基于轻量级框架<code>[**Ruia**](https://github.com/howie6879/ruia)</code>、专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持**命令行输入**，立志成为最实用，最轻量的动漫管理及下载助手
 
 ## ❓如何使用
 1. 首先来到[这里](https://www.python.org/downloads)下载Python解释器, 要求Python3.8及以上版本，安装即可
 2. 然后，打开命令提示符，输入 <code>pip install AnimeCrawler</code>
 3. 其次，来到[这个网站](https://www.mhyyy.com/),搜索您喜欢的动漫，点击播放页，将第一页的url复制一下
-4. 最后，打开命令提示符，输入 <code>python -m AnimeCrawler "动漫名称" "url"</code> 回车就可以下载啦
-    - 输入 <code>python -m AnimeCrawler -h</code> 会有详细的说明
+4. 最后，打开命令提示符，输入 <code>AnimeCrawler download -t "动漫名称" -u "url"</code> 回车就可以下载啦
+    - 输入 <code>AnimeCrawler -h</code> 会有详细的说明
 > 下载后的文件在您的视频文件夹里
 
 如果您想体验最新的功能，请转到dev分支~
 
 ## 🚀我想帮忙
 十分感谢您有这个想法。这个项目仍在青涩年华，总会有一些跌跌撞撞的时候，也许您的举手之劳，能造就更好的它
```

### Comparing `AnimeCrawler-0.1.1/AnimeCrawler.egg-info/SOURCES.txt` & `AnimeCrawler-0.1.2/AnimeCrawler.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 setup.py
 AnimeCrawler/__init__.py
 AnimeCrawler/__main__.py
+AnimeCrawler/base_spider.py
+AnimeCrawler/log.py
 AnimeCrawler.egg-info/PKG-INFO
 AnimeCrawler.egg-info/SOURCES.txt
 AnimeCrawler.egg-info/dependency_links.txt
 AnimeCrawler.egg-info/entry_points.txt
 AnimeCrawler.egg-info/requires.txt
 AnimeCrawler.egg-info/top_level.txt
 AnimeCrawler/command/__init__.py
```

### Comparing `AnimeCrawler-0.1.1/LICENSE` & `AnimeCrawler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.1.1/PKG-INFO` & `AnimeCrawler-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.1.1
+Version: 0.1.2
 Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,16 +28,16 @@
 
 这是一款在Windows平台下基于轻量级框架<code>[**Ruia**](https://github.com/howie6879/ruia)</code>、专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持**命令行输入**，立志成为最实用，最轻量的动漫管理及下载助手
 
 ## ❓如何使用
 1. 首先来到[这里](https://www.python.org/downloads)下载Python解释器, 要求Python3.8及以上版本，安装即可
 2. 然后，打开命令提示符，输入 <code>pip install AnimeCrawler</code>
 3. 其次，来到[这个网站](https://www.mhyyy.com/),搜索您喜欢的动漫，点击播放页，将第一页的url复制一下
-4. 最后，打开命令提示符，输入 <code>python -m AnimeCrawler "动漫名称" "url"</code> 回车就可以下载啦
-    - 输入 <code>python -m AnimeCrawler -h</code> 会有详细的说明
+4. 最后，打开命令提示符，输入 <code>AnimeCrawler download -t "动漫名称" -u "url"</code> 回车就可以下载啦
+    - 输入 <code>AnimeCrawler -h</code> 会有详细的说明
 > 下载后的文件在您的视频文件夹里
 
 如果您想体验最新的功能，请转到dev分支~
 
 ## 🚀我想帮忙
 十分感谢您有这个想法。这个项目仍在青涩年华，总会有一些跌跌撞撞的时候，也许您的举手之劳，能造就更好的它
```

### Comparing `AnimeCrawler-0.1.1/README.md` & `AnimeCrawler-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 这是一款在Windows平台下基于轻量级框架<code>[**Ruia**](https://github.com/howie6879/ruia)</code>、专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持**命令行输入**，立志成为最实用，最轻量的动漫管理及下载助手
 
 ## ❓如何使用
 1. 首先来到[这里](https://www.python.org/downloads)下载Python解释器, 要求Python3.8及以上版本，安装即可
 2. 然后，打开命令提示符，输入 <code>pip install AnimeCrawler</code>
 3. 其次，来到[这个网站](https://www.mhyyy.com/),搜索您喜欢的动漫，点击播放页，将第一页的url复制一下
-4. 最后，打开命令提示符，输入 <code>python -m AnimeCrawler "动漫名称" "url"</code> 回车就可以下载啦
-    - 输入 <code>python -m AnimeCrawler -h</code> 会有详细的说明
+4. 最后，打开命令提示符，输入 <code>AnimeCrawler download -t "动漫名称" -u "url"</code> 回车就可以下载啦
+    - 输入 <code>AnimeCrawler -h</code> 会有详细的说明
 > 下载后的文件在您的视频文件夹里
 
 如果您想体验最新的功能，请转到dev分支~
 
 ## 🚀我想帮忙
 十分感谢您有这个想法。这个项目仍在青涩年华，总会有一些跌跌撞撞的时候，也许您的举手之劳，能造就更好的它
```

### Comparing `AnimeCrawler-0.1.1/setup.py` & `AnimeCrawler-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AnimeCrawler",
-    version="v0.1.1",
+    version="v0.1.2",
     author="Senvlin",
     author_email="2994515402@qq.com",
     description="一个可免费下载动漫的爬虫",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Senvlin/AnimeCrawler",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=[
-        'ruia',
-        'tqdm',
-        'aiofiles',
-    ],
+    install_requires=['ruia', 'tqdm', 'aiofiles', 'aiohttp'],
     entry_points={
         'console_scripts': [
             'animecrawler = AnimeCrawler.command.run:main',
         ],
     },
     python_requires='>=3.8',
 )
```

