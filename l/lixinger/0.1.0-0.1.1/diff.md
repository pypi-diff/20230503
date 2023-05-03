# Comparing `tmp/lixinger-0.1.0.tar.gz` & `tmp/lixinger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixinger-0.1.0.tar", last modified: Wed May  3 10:02:15 2023, max compression
+gzip compressed data, was "lixinger-0.1.1.tar", last modified: Wed May  3 10:12:07 2023, max compression
```

## Comparing `lixinger-0.1.0.tar` & `lixinger-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      559 2023-05-03 10:00:42.790787 lixinger-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.0/lixinger/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.0/lixinger/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.0/lixinger/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.0/lixinger/api/cn/company/__init__.py
--rw-r--r--   0        0        0     2096 2023-05-03 10:00:43.645184 lixinger-0.1.0/lixinger/api/cn/company/base.py
--rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.0/lixinger/api/cn/index/__init__.py
--rw-r--r--   0        0        0     1685 2023-05-03 09:59:49.921863 lixinger-0.1.0/lixinger/api/cn/index/fundamental.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.0/lixinger/api/hk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.0/lixinger/api/macro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.0/lixinger/api/us/__init__.py
--rw-r--r--   0        0        0     1540 2023-05-03 04:05:06.981904 lixinger-0.1.0/lixinger/config.py
--rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.0/lixinger/py.typed
--rw-r--r--   0        0        0      111 2023-05-03 09:44:20.482330 lixinger-0.1.0/lixinger/settings.toml
--rw-r--r--   0        0        0     1030 2023-05-03 09:26:05.615918 lixinger-0.1.0/lixinger/utils.py
--rw-r--r--   0        0        0      616 2023-05-03 10:02:15.882584 lixinger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.0/tests/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.0/tests/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.0/tests/api/cn/company/__init__.py
--rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.0/tests/api/cn/company/test_base.py
--rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.0/tests/api/cn/index/__init__.py
--rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.0/tests/api/cn/index/test_fundamental.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 lixinger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      705 2023-05-03 10:11:52.615764 lixinger-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.1/lixinger/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.1/lixinger/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.1/lixinger/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.1/lixinger/api/cn/company/__init__.py
+-rw-r--r--   0        0        0     2096 2023-05-03 10:00:43.645184 lixinger-0.1.1/lixinger/api/cn/company/base.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.1/lixinger/api/cn/index/__init__.py
+-rw-r--r--   0        0        0     1685 2023-05-03 09:59:49.921863 lixinger-0.1.1/lixinger/api/cn/index/fundamental.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.1/lixinger/api/hk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.1/lixinger/api/macro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.1/lixinger/api/us/__init__.py
+-rw-r--r--   0        0        0     1540 2023-05-03 04:05:06.981904 lixinger-0.1.1/lixinger/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.1/lixinger/py.typed
+-rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.1/lixinger/settings.toml
+-rw-r--r--   0        0        0     1030 2023-05-03 09:26:05.615918 lixinger-0.1.1/lixinger/utils.py
+-rw-r--r--   0        0        0      616 2023-05-03 10:12:07.486854 lixinger-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.1/tests/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.1/tests/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.1/tests/api/cn/company/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.1/tests/api/cn/company/test_base.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.1/tests/api/cn/index/__init__.py
+-rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.1/tests/api/cn/index/test_fundamental.py
+-rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 lixinger-0.1.1/PKG-INFO
```

### Comparing `lixinger-0.1.0/README.md` & `lixinger-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,16 +6,24 @@
 
 ```bash
 pip install lixinger
 ```
 
 ## 用法
 
+设置自己的 Token (配置文件路径: ~/.config/lixinger/settings.toml)
+
+```toml
+[default]
+token = "your token"
+```
+
+使用文档请参考 [理杏仁开放平台](https://www.lixinger.com/open/api/doc)
+
 ```python
-# 使用文档请参考 https://www.lixinger.com/open/api/doc
 from lixinger.api.cn.company.base import get_company
 
 # 获取股票详细信息
 company = get_company(stock_codes=["600519"])
 print(company)
 ```
```

### Comparing `lixinger-0.1.0/lixinger/api/cn/company/base.py` & `lixinger-0.1.1/lixinger/api/cn/company/base.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.0/lixinger/api/cn/index/fundamental.py` & `lixinger-0.1.1/lixinger/api/cn/index/fundamental.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.0/lixinger/config.py` & `lixinger-0.1.1/lixinger/config.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.0/lixinger/utils.py` & `lixinger-0.1.1/lixinger/utils.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.0/pyproject.toml` & `lixinger-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache/"
 addopts = "-s -p no:warnings"
 asyncio_mode = "auto"
 
 [project]
 name = "lixinger"
-version = "0.1.0"
+version = "0.1.1"
 description = "Lixinger SDK for Python (Unofficial)"
 authors = [
     { name = "Chaoying", email = "chaoying2022@gmail.com" },
 ]
 dependencies = [
     "pandera>=0.14.5",
     "pydantic>=1.10.7",
```

### Comparing `lixinger-0.1.0/PKG-INFO` & `lixinger-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lixinger
-Version: 0.1.0
+Version: 0.1.1
 Summary: Lixinger SDK for Python (Unofficial)
 Author-Email: Chaoying <chaoying2022@gmail.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: pandera>=0.14.5
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: requests>=2.29.0
@@ -19,16 +19,24 @@
 
 ```bash
 pip install lixinger
 ```
 
 ## 用法
 
+设置自己的 Token (配置文件路径: ~/.config/lixinger/settings.toml)
+
+```toml
+[default]
+token = "your token"
+```
+
+使用文档请参考 [理杏仁开放平台](https://www.lixinger.com/open/api/doc)
+
 ```python
-# 使用文档请参考 https://www.lixinger.com/open/api/doc
 from lixinger.api.cn.company.base import get_company
 
 # 获取股票详细信息
 company = get_company(stock_codes=["600519"])
 print(company)
 ```
```

