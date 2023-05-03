# Comparing `tmp/emoji-generator-0.3.tar.gz` & `tmp/emoji-generator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emoji-generator-0.3.tar", last modified: Wed May  3 11:56:51 2023, max compression
+gzip compressed data, was "emoji-generator-0.4.tar", last modified: Wed May  3 12:11:23 2023, max compression
```

## Comparing `emoji-generator-0.3.tar` & `emoji-generator-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        0 2023-05-03 11:56:51.289557 emoji-generator-0.3/
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)      235 2023-05-03 11:56:51.289557 emoji-generator-0.3/PKG-INFO
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)     1197 2023-05-03 11:56:44.000000 emoji-generator-0.3/README.md
-drwxrwxr-x   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        0 2023-05-03 11:56:51.285557 emoji-generator-0.3/emoji_generator/
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        0 2023-05-03 10:48:49.000000 emoji-generator-0.3/emoji_generator/__init__.py
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)   275846 2023-05-03 11:50:09.000000 emoji-generator-0.3/emoji_generator/random_emoji.py
-drwxrwxr-x   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        0 2023-05-03 11:56:51.285557 emoji-generator-0.3/emoji_generator.egg-info/
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)      235 2023-05-03 11:56:51.000000 emoji-generator-0.3/emoji_generator.egg-info/PKG-INFO
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)      234 2023-05-03 11:56:51.000000 emoji-generator-0.3/emoji_generator.egg-info/SOURCES.txt
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        1 2023-05-03 11:56:51.000000 emoji-generator-0.3/emoji_generator.egg-info/dependency_links.txt
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)       16 2023-05-03 11:56:51.000000 emoji-generator-0.3/emoji_generator.egg-info/top_level.txt
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)       38 2023-05-03 11:56:51.289557 emoji-generator-0.3/setup.cfg
--rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)      291 2023-05-03 11:46:08.000000 emoji-generator-0.3/setup.py
+drwxrwxr-x   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        0 2023-05-03 12:11:23.839014 emoji-generator-0.4/
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)     1464 2023-05-03 12:11:23.835014 emoji-generator-0.4/PKG-INFO
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)     1197 2023-05-03 11:56:44.000000 emoji-generator-0.4/README.md
+drwxrwxr-x   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        0 2023-05-03 12:11:23.831014 emoji-generator-0.4/emoji_generator/
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        0 2023-05-03 10:48:49.000000 emoji-generator-0.4/emoji_generator/__init__.py
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)   275846 2023-05-03 11:50:09.000000 emoji-generator-0.4/emoji_generator/random_emoji.py
+drwxrwxr-x   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        0 2023-05-03 12:11:23.835014 emoji-generator-0.4/emoji_generator.egg-info/
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)     1464 2023-05-03 12:11:23.000000 emoji-generator-0.4/emoji_generator.egg-info/PKG-INFO
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)      234 2023-05-03 12:11:23.000000 emoji-generator-0.4/emoji_generator.egg-info/SOURCES.txt
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)        1 2023-05-03 12:11:23.000000 emoji-generator-0.4/emoji_generator.egg-info/dependency_links.txt
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)       16 2023-05-03 12:11:23.000000 emoji-generator-0.4/emoji_generator.egg-info/top_level.txt
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)       38 2023-05-03 12:11:23.839014 emoji-generator-0.4/setup.cfg
+-rw-rw-r--   0 dhanunjayavarmak  (1001) dhanunjayavarmak  (1001)      450 2023-05-03 12:11:07.000000 emoji-generator-0.4/setup.py
```

### Comparing `emoji-generator-0.3/README.md` & `emoji-generator-0.4/README.md`

 * *Files identical despite different names*

### Comparing `emoji-generator-0.3/emoji_generator/random_emoji.py` & `emoji-generator-0.4/emoji_generator/random_emoji.py`

 * *Files identical despite different names*

