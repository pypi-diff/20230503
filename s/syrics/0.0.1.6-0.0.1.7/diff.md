# Comparing `tmp/syrics-0.0.1.6.tar.gz` & `tmp/syrics-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syrics-0.0.1.6.tar", last modified: Sun Mar 12 05:12:11 2023, max compression
+gzip compressed data, was "syrics-0.0.1.7.tar", last modified: Wed May  3 19:34:51 2023, max compression
```

## Comparing `syrics-0.0.1.6.tar` & `syrics-0.0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 05:12:11.794137 syrics-0.0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-03-12 05:11:57.000000 syrics-0.0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-12 05:12:11.794137 syrics-0.0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-03-12 05:11:57.000000 syrics-0.0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-12 05:12:11.794137 syrics-0.0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-12 05:11:57.000000 syrics-0.0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 05:12:11.794137 syrics-0.0.1.6/syrics/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-12 05:11:57.000000 syrics-0.0.1.6/syrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-03-12 05:11:57.000000 syrics-0.0.1.6/syrics/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-12 05:11:57.000000 syrics-0.0.1.6/syrics/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7232 2023-03-12 05:11:57.000000 syrics-0.0.1.6/syrics/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-12 05:11:57.000000 syrics-0.0.1.6/syrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 05:12:11.794137 syrics-0.0.1.6/syrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-12 05:12:11.000000 syrics-0.0.1.6/syrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-12 05:12:11.000000 syrics-0.0.1.6/syrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 05:12:11.000000 syrics-0.0.1.6/syrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-12 05:12:11.000000 syrics-0.0.1.6/syrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-12 05:12:11.000000 syrics-0.0.1.6/syrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-12 05:12:11.000000 syrics-0.0.1.6/syrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:34:51.156920 syrics-0.0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-05-03 19:34:34.000000 syrics-0.0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-03 19:34:51.156920 syrics-0.0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-03 19:34:34.000000 syrics-0.0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 19:34:51.156920 syrics-0.0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-03 19:34:34.000000 syrics-0.0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:34:51.156920 syrics-0.0.1.7/syrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:34:34.000000 syrics-0.0.1.7/syrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-03 19:34:34.000000 syrics-0.0.1.7/syrics/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-03 19:34:34.000000 syrics-0.0.1.7/syrics/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7376 2023-05-03 19:34:34.000000 syrics-0.0.1.7/syrics/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 19:34:34.000000 syrics-0.0.1.7/syrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:34:51.156920 syrics-0.0.1.7/syrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-03 19:34:51.000000 syrics-0.0.1.7/syrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-03 19:34:51.000000 syrics-0.0.1.7/syrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:34:51.000000 syrics-0.0.1.7/syrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 19:34:51.000000 syrics-0.0.1.7/syrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 19:34:51.000000 syrics-0.0.1.7/syrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 19:34:51.000000 syrics-0.0.1.7/syrics.egg-info/top_level.txt
```

### Comparing `syrics-0.0.1.6/LICENSE` & `syrics-0.0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `syrics-0.0.1.6/PKG-INFO` & `syrics-0.0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syrics
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: A command line tool to fetch lyrics from spotify and save it to lrc file. It can fetch both synced and unsynced lyrics from spotify. 
 Home-page: https://github.com/akashrchandran/syrics
 Author: Akash R Chandran
 Author-email: chandranrakash@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `syrics-0.0.1.6/README.md` & `syrics-0.0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `syrics-0.0.1.6/setup.py` & `syrics-0.0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "spotipy",
     "tqdm",
     "tinytag",
 ]
 
 setup(
     name=pkg_name,
-    version="0.0.1.6",
+    version="0.0.1.7",
     author="Akash R Chandran",
     author_email="chandranrakash@gmail.com",
     description="A command line tool to fetch lyrics from spotify and save it to lrc file. It can fetch both synced and unsynced lyrics from spotify. ",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/akashrchandran/syrics",
     install_requires=requirements,
```

### Comparing `syrics-0.0.1.6/syrics/api.py` & `syrics-0.0.1.7/syrics/api.py`

 * *Files identical despite different names*

### Comparing `syrics-0.0.1.6/syrics/cli.py` & `syrics-0.0.1.7/syrics/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,33 +37,29 @@
 parser.add_argument("URL",
                     metavar="URL",
                     nargs="?",
                     help=("url of song, album or playlist from spotify."),
                     )
 
 
-def parse_cmd(config):
+def parse_cmd():
     args = parser.parse_args()
-    if args.directory:
-        config['download_path'] = args.directory
-    if args.force:
-        config['force_download'] = args.force
     if args.user in ['current', 'current-playing']:
         args.URL = 'current'
     elif args.user in ['play', 'playlist']:
         args.URL = 'play'
     elif args.user in ['album']:
         args.URL = 'album'
     if args.config == 'edit':
         create_config()
     elif args.config in ["reset", "r"]:
         create_config(config_exists = False)
     elif args.config in ["open", "o"]:
         open_config()
-    return args.URL
+    return args.URL, args.directory, args.force
 
 def input_taker(config, key, question, string = True):
     print(question)
     print(f"[SAVED]: {str(config[key])[:50]}")
     if ans := input():
         config[key] = ans if string else bool(int(ans))
```

### Comparing `syrics-0.0.1.6/syrics/core.py` & `syrics-0.0.1.7/syrics/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,21 +135,23 @@
                     save_lyrics(format_lrc(lyrics_json, track[0]), path=file_name)
             else:
                 unable.append(tag.title)
     return unable
 
 def initial_checks():
     global client, cmd_url, config
+    cmd_url, directory, force = parse_cmd()
     CONFIG_FILE = check_config()
     try:
         with open(CONFIG_FILE) as f:
             config = json.load(f)
     except Exception as e:
         raise CorruptedConfig("Config file seems corrupted, run syrics -c reset") from e
-    cmd_url = parse_cmd(config)
+    config['download_path'] = directory or config['download_path']
+    config['force_download'] = force or config['force_download']
     client = Spotify(config['sp_dc'])
     if cmd_url == 'current':
         cmd_url = client.get_current_song( )['item']['external_urls']['spotify']
     elif cmd_url == 'play':
         cmd_url = client.select_user_playlist()['external_urls']['spotify']
     elif cmd_url == 'album':
         cmd_url = client.select_user_album()['external_urls']['spotify']
```

### Comparing `syrics-0.0.1.6/syrics.egg-info/PKG-INFO` & `syrics-0.0.1.7/syrics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syrics
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: A command line tool to fetch lyrics from spotify and save it to lrc file. It can fetch both synced and unsynced lyrics from spotify. 
 Home-page: https://github.com/akashrchandran/syrics
 Author: Akash R Chandran
 Author-email: chandranrakash@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

