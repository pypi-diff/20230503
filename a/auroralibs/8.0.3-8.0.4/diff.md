# Comparing `tmp/auroralibs-8.0.3.tar.gz` & `tmp/auroralibs-8.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auroralibs-8.0.3.tar", last modified: Wed May  3 12:26:52 2023, max compression
+gzip compressed data, was "auroralibs-8.0.4.tar", last modified: Wed May  3 13:17:38 2023, max compression
```

## Comparing `auroralibs-8.0.3.tar` & `auroralibs-8.0.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:26:52.478114 auroralibs-8.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:26:52.462113 auroralibs-8.0.3/Ayra/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2830 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:26:52.462113 auroralibs-8.0.3/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4655 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12387 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-05-03 12:26:31.000000 auroralibs-8.0.3/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:26:52.470114 auroralibs-8.0.3/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     1980 2023-04-30 08:20:27.000000 auroralibs-8.0.3/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:26:52.474114 auroralibs-8.0.3/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    19940 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17348 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28736 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:26:52.478114 auroralibs-8.0.3/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18388 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-04-30 02:37:34.000000 auroralibs-8.0.3/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-03 12:26:31.000000 auroralibs-8.0.3/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-04-30 02:37:34.000000 auroralibs-8.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3370 2023-05-03 12:26:52.478114 auroralibs-8.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2023-04-30 02:37:34.000000 auroralibs-8.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:26:52.478114 auroralibs-8.0.3/auroralibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3370 2023-05-03 12:26:52.000000 auroralibs-8.0.3/auroralibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1481 2023-05-03 12:26:52.000000 auroralibs-8.0.3/auroralibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:26:52.000000 auroralibs-8.0.3/auroralibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 12:26:52.000000 auroralibs-8.0.3/auroralibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-03 12:26:52.000000 auroralibs-8.0.3/auroralibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 12:26:52.478114 auroralibs-8.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1499 2023-04-30 02:42:13.000000 auroralibs-8.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:17:38.051725 auroralibs-8.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:17:38.043724 auroralibs-8.0.4/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:17:38.047724 auroralibs-8.0.4/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4656 2023-05-03 13:17:27.000000 auroralibs-8.0.4/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12387 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-05-03 12:26:31.000000 auroralibs-8.0.4/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:17:38.047724 auroralibs-8.0.4/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-04-30 08:20:27.000000 auroralibs-8.0.4/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:17:38.051725 auroralibs-8.0.4/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    19940 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17348 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28736 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:17:38.051725 auroralibs-8.0.4/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18388 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-30 02:37:34.000000 auroralibs-8.0.4/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-03 13:17:27.000000 auroralibs-8.0.4/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-04-30 02:37:34.000000 auroralibs-8.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3370 2023-05-03 13:17:38.051725 auroralibs-8.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-30 02:37:34.000000 auroralibs-8.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:17:38.051725 auroralibs-8.0.4/auroralibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3370 2023-05-03 13:17:37.000000 auroralibs-8.0.4/auroralibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-05-03 13:17:38.000000 auroralibs-8.0.4/auroralibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 13:17:37.000000 auroralibs-8.0.4/auroralibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 13:17:37.000000 auroralibs-8.0.4/auroralibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-03 13:17:37.000000 auroralibs-8.0.4/auroralibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 13:17:38.055725 auroralibs-8.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-04-30 02:42:13.000000 auroralibs-8.0.4/setup.py
```

### Comparing `auroralibs-8.0.3/Ayra/__init__.py` & `auroralibs-8.0.4/Ayra/__init__.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/__main__.py` & `auroralibs-8.0.4/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/_misc/__init__.py` & `auroralibs-8.0.4/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/_misc/_assistant.py` & `auroralibs-8.0.4/Ayra/_misc/_assistant.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 res = [
                     await event.builder.article(
                         title="ᴀʏʀᴀ ꭙ ᴜꜱᴇʀʙᴏᴛ",
                         url="https://t.me/Kamarsnow",
                         description="© Kynan",
                         text=MSG,
                         thumb=InputWebDocument(
-                            "https://graph.org/file/5e87b24315262edfb40db.jpg,
+                            "https://graph.org/file/5e87b24315262edfb40db.jpg",
                             0,
                             "image/jpeg",
                             [],
                         ),
                         buttons=IN_BTTS,
                     )
                 ]
```

### Comparing `auroralibs-8.0.3/Ayra/_misc/_decorators.py` & `auroralibs-8.0.4/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/_misc/_supporter.py` & `auroralibs-8.0.4/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/_misc/_wrappers.py` & `auroralibs-8.0.4/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/configs.py` & `auroralibs-8.0.4/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/__init__.py` & `auroralibs-8.0.4/Ayra/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/afk_db.py` & `auroralibs-8.0.4/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/antiflood_db.py` & `auroralibs-8.0.4/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/asst_fns.py` & `auroralibs-8.0.4/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/asstcmd_db.py` & `auroralibs-8.0.4/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/autoban_db.py` & `auroralibs-8.0.4/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/blacklist_db.py` & `auroralibs-8.0.4/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/botchat_db.py` & `auroralibs-8.0.4/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/broadcast_db.py` & `auroralibs-8.0.4/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/ch_db.py` & `auroralibs-8.0.4/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/dnd_db.py` & `auroralibs-8.0.4/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/echo_db.py` & `auroralibs-8.0.4/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/filestore_db.py` & `auroralibs-8.0.4/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/filter_db.py` & `auroralibs-8.0.4/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/forcesub_db.py` & `auroralibs-8.0.4/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/gban_mute_db.py` & `auroralibs-8.0.4/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/gcast_blacklist_db.py` & `auroralibs-8.0.4/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/greetings_db.py` & `auroralibs-8.0.4/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/logusers_db.py` & `auroralibs-8.0.4/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/mute_db.py` & `auroralibs-8.0.4/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/night_db.py` & `auroralibs-8.0.4/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/notes_db.py` & `auroralibs-8.0.4/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/nsfw_db.py` & `auroralibs-8.0.4/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/pmpermit_db.py` & `auroralibs-8.0.4/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/snips_db.py` & `auroralibs-8.0.4/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/vc_sudos.py` & `auroralibs-8.0.4/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/dB/warn_db.py` & `auroralibs-8.0.4/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/FastTelethon.py` & `auroralibs-8.0.4/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/__init__.py` & `auroralibs-8.0.4/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/admins.py` & `auroralibs-8.0.4/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/executor.py` & `auroralibs-8.0.4/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/gDrive.py` & `auroralibs-8.0.4/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/google_image.py` & `auroralibs-8.0.4/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/helper.py` & `auroralibs-8.0.4/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/info.py` & `auroralibs-8.0.4/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/misc.py` & `auroralibs-8.0.4/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/tools.py` & `auroralibs-8.0.4/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/fns/ytdl.py` & `auroralibs-8.0.4/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/kynan.py` & `auroralibs-8.0.4/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/loader.py` & `auroralibs-8.0.4/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/startup/BaseClient.py` & `auroralibs-8.0.4/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/startup/__init__.py` & `auroralibs-8.0.4/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/startup/_database.py` & `auroralibs-8.0.4/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/startup/_extra.py` & `auroralibs-8.0.4/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/startup/connections.py` & `auroralibs-8.0.4/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/startup/funcs.py` & `auroralibs-8.0.4/Ayra/startup/funcs.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/startup/loader.py` & `auroralibs-8.0.4/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/Ayra/startup/utils.py` & `auroralibs-8.0.4/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/LICENSE` & `auroralibs-8.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/PKG-INFO` & `auroralibs-8.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auroralibs
-Version: 8.0.3
+Version: 8.0.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `auroralibs-8.0.3/README.md` & `auroralibs-8.0.4/README.md`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/auroralibs.egg-info/PKG-INFO` & `auroralibs-8.0.4/auroralibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auroralibs
-Version: 8.0.3
+Version: 8.0.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `auroralibs-8.0.3/auroralibs.egg-info/SOURCES.txt` & `auroralibs-8.0.4/auroralibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auroralibs-8.0.3/setup.py` & `auroralibs-8.0.4/setup.py`

 * *Files identical despite different names*

