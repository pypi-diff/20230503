# Comparing `tmp/discord-ext-pager-1.0.1.tar.gz` & `tmp/discord-ext-pager-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ext-pager-1.0.1.tar", last modified: Sat Apr 22 22:39:59 2023, max compression
+gzip compressed data, was "discord-ext-pager-1.0.2.tar", last modified: Wed May  3 03:01:41 2023, max compression
```

## Comparing `discord-ext-pager-1.0.1.tar` & `discord-ext-pager-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.754344 discord-ext-pager-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-22 22:39:47.000000 discord-ext-pager-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-22 22:39:59.754344 discord-ext-pager-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-22 22:39:47.000000 discord-ext-pager-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-22 22:39:47.000000 discord-ext-pager-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 22:39:59.754344 discord-ext-pager-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.750344 discord-ext-pager-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.750344 discord-ext-pager-1.0.1/src/discord/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.750344 discord-ext-pager-1.0.1/src/discord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.750344 discord-ext-pager-1.0.1/src/discord/ext/pager/
--rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-04-22 22:39:47.000000 discord-ext-pager-1.0.1/src/discord/ext/pager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:39:59.754344 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 22:39:59.000000 discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:01:41.837136 discord-ext-pager-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-03 03:01:29.000000 discord-ext-pager-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-03 03:01:41.837136 discord-ext-pager-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-03 03:01:29.000000 discord-ext-pager-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-03 03:01:29.000000 discord-ext-pager-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 03:01:41.837136 discord-ext-pager-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:01:41.837136 discord-ext-pager-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:01:41.837136 discord-ext-pager-1.0.2/src/discord/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:01:41.837136 discord-ext-pager-1.0.2/src/discord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:01:41.837136 discord-ext-pager-1.0.2/src/discord/ext/pager/
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-05-03 03:01:29.000000 discord-ext-pager-1.0.2/src/discord/ext/pager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:01:41.837136 discord-ext-pager-1.0.2/src/discord_ext_pager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-03 03:01:41.000000 discord-ext-pager-1.0.2/src/discord_ext_pager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 03:01:41.000000 discord-ext-pager-1.0.2/src/discord_ext_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 03:01:41.000000 discord-ext-pager-1.0.2/src/discord_ext_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 03:01:41.000000 discord-ext-pager-1.0.2/src/discord_ext_pager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 03:01:41.000000 discord-ext-pager-1.0.2/src/discord_ext_pager.egg-info/top_level.txt
```

### Comparing `discord-ext-pager-1.0.1/LICENSE` & `discord-ext-pager-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.0.1/PKG-INFO` & `discord-ext-pager-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.0.1
+Version: 1.0.2
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
```

### Comparing `discord-ext-pager-1.0.1/README.md` & `discord-ext-pager-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.0.1/pyproject.toml` & `discord-ext-pager-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.0.1/src/discord/ext/pager/__init__.py` & `discord-ext-pager-1.0.2/src/discord/ext/pager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Union,
     cast,
 )
 
 import discord
 from typing_extensions import TypeAlias
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 __all__ = (
     "PageOption",
     "PageSource",
     "ListPageSource",
     "AsyncIteratorPageSource",
     "TimeoutAction",
@@ -474,15 +474,16 @@
     )
     async def stop_button(
         self,
         interaction: discord.Interaction,
         button: discord.ui.Button,
     ) -> None:
         self.stop()
-        await interaction.message.delete()  # type: ignore  # message is not None
+        await interaction.response.defer()
+        await interaction.delete_original_response()
 
     @discord.ui.button(
         emoji="\N{LEFTWARDS ARROW WITH HOOK}",
         style=discord.ButtonStyle.blurple,
         row=2,
     )
     async def back_button(
```

### Comparing `discord-ext-pager-1.0.1/src/discord_ext_pager.egg-info/PKG-INFO` & `discord-ext-pager-1.0.2/src/discord_ext_pager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.0.1
+Version: 1.0.2
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
```

