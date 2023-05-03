# Comparing `tmp/hugchat-0.0.5.1.tar.gz` & `tmp/hugchat-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.5.1.tar", last modified: Mon May  1 18:00:57 2023, max compression
+gzip compressed data, was "hugchat-0.0.5.2.tar", last modified: Wed May  3 15:57:41 2023, max compression
```

## Comparing `hugchat-0.0.5.1.tar` & `hugchat-0.0.5.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1690 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      670 2023-05-01 00:33:11.000000 hugchat-0.0.5.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1407 2023-05-01 18:00:50.000000 hugchat-0.0.5.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 18:00:57.585077 hugchat-0.0.5.1/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4696 2023-05-01 17:58:33.000000 hugchat-0.0.5.1/src/hugchat/hugchat.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1690 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      223 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:57:41.375097 hugchat-0.0.5.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2826 2023-05-03 15:57:41.375097 hugchat-0.0.5.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1806 2023-05-03 15:54:22.000000 hugchat-0.0.5.2/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-03 15:57:41.375097 hugchat-0.0.5.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1407 2023-05-03 15:55:47.000000 hugchat-0.0.5.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:57:41.371097 hugchat-0.0.5.2/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:57:41.371097 hugchat-0.0.5.2/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.2/src/hugchat/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.2/src/hugchat/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6265 2023-05-03 15:54:22.000000 hugchat-0.0.5.2/src/hugchat/hugchat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:57:41.371097 hugchat-0.0.5.2/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2826 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.5.1/LICENSE` & `hugchat-0.0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.5.1/setup.py` & `hugchat-0.0.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.5.1",
+    version="0.0.5.2",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

