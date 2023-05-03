# Comparing `tmp/VodBot-1.1.5.tar.gz` & `tmp/VodBot-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VodBot-1.1.5.tar", last modified: Mon Apr 17 22:33:43 2023, max compression
+gzip compressed data, was "VodBot-1.1.6.tar", last modified: Wed May  3 01:39:47 2023, max compression
```

## Comparing `VodBot-1.1.5.tar` & `VodBot-1.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.595310 VodBot-1.1.5/
--rw-rw-rw-   0        0        0     1140 2022-12-17 05:25:09.000000 VodBot-1.1.5/LICENSE.md
--rw-rw-rw-   0        0        0     4208 2023-04-17 22:33:43.594800 VodBot-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3688 2023-02-01 04:16:24.000000 VodBot-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.551659 VodBot-1.1.5/VodBot.egg-info/
--rw-rw-rw-   0        0        0     4208 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      198 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 22:33:43.595310 VodBot-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-01-20 01:23:02.000000 VodBot-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.568876 VodBot-1.1.5/vodbot/
--rw-rw-rw-   0        0        0       47 2023-04-17 22:32:08.000000 VodBot-1.1.5/vodbot/__init__.py
--rw-rw-rw-   0        0        0     9038 2023-01-20 21:45:35.000000 VodBot-1.1.5/vodbot/__main__.py
--rw-rw-rw-   0        0        0     3843 2023-01-20 19:40:58.000000 VodBot-1.1.5/vodbot/cache.py
--rw-rw-rw-   0        0        0     7165 2023-01-30 04:24:10.000000 VodBot-1.1.5/vodbot/chatlog.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.589673 VodBot-1.1.5/vodbot/commands/
--rw-rw-rw-   0        0        0        0 2022-12-16 02:49:49.000000 VodBot-1.1.5/vodbot/commands/__init__.py
--rw-rw-rw-   0        0        0     3799 2023-01-29 07:37:06.000000 VodBot-1.1.5/vodbot/commands/export.py
--rw-rw-rw-   0        0        0     3433 2023-01-20 20:08:55.000000 VodBot-1.1.5/vodbot/commands/info.py
--rw-rw-rw-   0        0        0     1601 2023-01-21 05:15:39.000000 VodBot-1.1.5/vodbot/commands/init.py
--rw-rw-rw-   0        0        0     7901 2023-04-17 22:07:30.000000 VodBot-1.1.5/vodbot/commands/pull.py
--rw-rw-rw-   0        0        0    21509 2023-04-17 22:27:24.000000 VodBot-1.1.5/vodbot/commands/stage.py
--rw-rw-rw-   0        0        0    12980 2023-04-17 22:18:15.000000 VodBot-1.1.5/vodbot/commands/upload.py
--rw-rw-rw-   0        0        0    16412 2023-04-17 22:27:35.000000 VodBot-1.1.5/vodbot/config.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.593791 VodBot-1.1.5/vodbot/itd/
--rw-rw-rw-   0        0        0       68 2022-12-16 02:49:49.000000 VodBot-1.1.5/vodbot/itd/__init__.py
--rw-rw-rw-   0        0        0     3359 2023-04-17 22:07:30.000000 VodBot-1.1.5/vodbot/itd/download.py
--rw-rw-rw-   0        0        0     4374 2023-01-30 04:07:09.000000 VodBot-1.1.5/vodbot/itd/gql.py
--rw-rw-rw-   0        0        0     3298 2023-04-17 22:07:30.000000 VodBot-1.1.5/vodbot/itd/worker.py
--rw-rw-rw-   0        0        0     1213 2023-01-20 01:23:02.000000 VodBot-1.1.5/vodbot/printer.py
--rw-rw-rw-   0        0        0     5060 2023-01-28 02:09:38.000000 VodBot-1.1.5/vodbot/thumbnail.py
--rw-rw-rw-   0        0        0    10202 2023-01-30 04:19:30.000000 VodBot-1.1.5/vodbot/twitch.py
--rw-rw-rw-   0        0        0     4024 2023-01-28 02:09:38.000000 VodBot-1.1.5/vodbot/util.py
--rw-rw-rw-   0        0        0     3248 2023-01-29 07:28:46.000000 VodBot-1.1.5/vodbot/video.py
--rw-rw-rw-   0        0        0     6052 2023-01-20 01:23:02.000000 VodBot-1.1.5/vodbot/webhook.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:39:47.260429 VodBot-1.1.6/
+-rw-rw-rw-   0        0        0     1140 2022-12-17 05:25:09.000000 VodBot-1.1.6/LICENSE.md
+-rw-rw-rw-   0        0        0     4208 2023-05-03 01:39:47.260429 VodBot-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3688 2023-02-01 04:16:24.000000 VodBot-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 01:39:47.224837 VodBot-1.1.6/VodBot.egg-info/
+-rw-rw-rw-   0        0        0     4208 2023-05-03 01:39:47.000000 VodBot-1.1.6/VodBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-05-03 01:39:47.000000 VodBot-1.1.6/VodBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 01:39:47.000000 VodBot-1.1.6/VodBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-03 01:39:47.000000 VodBot-1.1.6/VodBot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      198 2023-05-03 01:39:47.000000 VodBot-1.1.6/VodBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 01:39:47.000000 VodBot-1.1.6/VodBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 01:39:47.261471 VodBot-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-01-20 01:23:02.000000 VodBot-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:39:47.237911 VodBot-1.1.6/vodbot/
+-rw-rw-rw-   0        0        0       47 2023-05-03 01:01:42.000000 VodBot-1.1.6/vodbot/__init__.py
+-rw-rw-rw-   0        0        0     9038 2023-01-20 21:45:35.000000 VodBot-1.1.6/vodbot/__main__.py
+-rw-rw-rw-   0        0        0     3843 2023-01-20 19:40:58.000000 VodBot-1.1.6/vodbot/cache.py
+-rw-rw-rw-   0        0        0     7165 2023-01-30 04:24:10.000000 VodBot-1.1.6/vodbot/chatlog.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:39:47.253798 VodBot-1.1.6/vodbot/commands/
+-rw-rw-rw-   0        0        0        0 2022-12-16 02:49:49.000000 VodBot-1.1.6/vodbot/commands/__init__.py
+-rw-rw-rw-   0        0        0     3799 2023-01-29 07:37:06.000000 VodBot-1.1.6/vodbot/commands/export.py
+-rw-rw-rw-   0        0        0     3460 2023-05-03 01:36:40.000000 VodBot-1.1.6/vodbot/commands/info.py
+-rw-rw-rw-   0        0        0     1601 2023-01-21 05:15:39.000000 VodBot-1.1.6/vodbot/commands/init.py
+-rw-rw-rw-   0        0        0     7901 2023-04-17 22:07:30.000000 VodBot-1.1.6/vodbot/commands/pull.py
+-rw-rw-rw-   0        0        0    21509 2023-04-17 22:27:24.000000 VodBot-1.1.6/vodbot/commands/stage.py
+-rw-rw-rw-   0        0        0    12978 2023-05-03 01:01:36.000000 VodBot-1.1.6/vodbot/commands/upload.py
+-rw-rw-rw-   0        0        0    16412 2023-04-17 22:27:35.000000 VodBot-1.1.6/vodbot/config.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:39:47.259420 VodBot-1.1.6/vodbot/itd/
+-rw-rw-rw-   0        0        0       68 2022-12-16 02:49:49.000000 VodBot-1.1.6/vodbot/itd/__init__.py
+-rw-rw-rw-   0        0        0     3372 2023-05-03 01:01:36.000000 VodBot-1.1.6/vodbot/itd/download.py
+-rw-rw-rw-   0        0        0     4576 2023-05-03 01:36:34.000000 VodBot-1.1.6/vodbot/itd/gql.py
+-rw-rw-rw-   0        0        0     3298 2023-04-17 22:07:30.000000 VodBot-1.1.6/vodbot/itd/worker.py
+-rw-rw-rw-   0        0        0     1213 2023-01-20 01:23:02.000000 VodBot-1.1.6/vodbot/printer.py
+-rw-rw-rw-   0        0        0     5060 2023-01-28 02:09:38.000000 VodBot-1.1.6/vodbot/thumbnail.py
+-rw-rw-rw-   0        0        0    10202 2023-01-30 04:19:30.000000 VodBot-1.1.6/vodbot/twitch.py
+-rw-rw-rw-   0        0        0     4024 2023-01-28 02:09:38.000000 VodBot-1.1.6/vodbot/util.py
+-rw-rw-rw-   0        0        0     3248 2023-01-29 07:28:46.000000 VodBot-1.1.6/vodbot/video.py
+-rw-rw-rw-   0        0        0     6052 2023-01-20 01:23:02.000000 VodBot-1.1.6/vodbot/webhook.py
```

### Comparing `VodBot-1.1.5/LICENSE.md` & `VodBot-1.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/PKG-INFO` & `VodBot-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VodBot
-Version: 1.1.5
+Version: 1.1.6
 Summary: Twitch VOD and Clip manager
 Home-page: https://github.com/FriendTeamInc/VodBot
 Author: Logan "NotQuiteApex" Hickok-Dickson
 Author-email: self@notquiteapex.net
 License: MIT
 Project-URL: Homepage, https://github.com/FriendTeamInc/VodBot
 Project-URL: Bug Tracker, https://github.com/FriendTeamInc/VodBot/issues
```

### Comparing `VodBot-1.1.5/README.md` & `VodBot-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/VodBot.egg-info/PKG-INFO` & `VodBot-1.1.6/VodBot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VodBot
-Version: 1.1.5
+Version: 1.1.6
 Summary: Twitch VOD and Clip manager
 Home-page: https://github.com/FriendTeamInc/VodBot
 Author: Logan "NotQuiteApex" Hickok-Dickson
 Author-email: self@notquiteapex.net
 License: MIT
 Project-URL: Homepage, https://github.com/FriendTeamInc/VodBot
 Project-URL: Bug Tracker, https://github.com/FriendTeamInc/VodBot/issues
```

### Comparing `VodBot-1.1.5/VodBot.egg-info/SOURCES.txt` & `VodBot-1.1.6/VodBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/setup.py` & `VodBot-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/__main__.py` & `VodBot-1.1.6/vodbot/__main__.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/cache.py` & `VodBot-1.1.6/vodbot/cache.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/chatlog.py` & `VodBot-1.1.6/vodbot/chatlog.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/commands/export.py` & `VodBot-1.1.6/vodbot/commands/export.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/commands/info.py` & `VodBot-1.1.6/vodbot/commands/info.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import re
 from vodbot.printer import cprint
 
 from vodbot import util
 from vodbot.itd import gql
 
 PATTERNS = {
+	"channel": [
+		r"^(?P<id>[a-zA-Z0-9][\w]{0,24})$",
+		r"^(https?://)?(www\.)?twitch\.tv/(?P<id>[a-zA-Z0-9][\w]{0,24})(\?.*)?$"
+	],
 	"vod": [
 		r"^(?P<id>\d+)?$",
 		r"^(https?://)?(www\.)?twitch.tv/videos/(?P<id>\d+)(\?.*)?$"
 	],
 	"clip": [
 		r"^(?P<id>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)$",
 		r"^(https?://)?(www\.)?twitch.tv/\w+/clip/(?P<id>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.*)?$",
 		r"^(https?://)?clips\.twitch.tv/(?P<id>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.*)?$"
 	],
-	"channel": [
-		r"^[a-zA-Z0-9][\w]{0,24}$",
-		r"^(https?://)?(www\.)?twitch\.tv/(?P<id>[a-zA-Z0-9][\w]{0,24})(\?.*)?$"
-	]
 }
 
 KEYTRANS = {
 	"vod": "VOD",
 	"clip": "Clip",
 	"channel": "Channel"
 }
@@ -69,14 +69,15 @@
 	# run the query
 	resp = gql.gql_query(query=query).json()
 	resp = resp["data"]
 	if not any([resp.get("video"), resp.get("clip"), resp.get("user")]):
 		util.exit_prog(93, f"Could not query info on {cword} content from input.")
 	
 	# Read the data back and out to the terminal
+	# print(resp)
 	if ctype == "vod":
 		r = resp['video']
 		c = r['creator']
 		g = r['game']
 		cprint(f"#fGTitle: `{r['title']}`#r - ID: `{r['id']}`")
 		cprint(f"#fMBroadcaster: {c['displayName']} - {c['login']} ({c['id']})#r")
 		cprint(f"#fCPlaying: {g['name']} ({g['id']})#r")
@@ -95,10 +96,10 @@
 	elif ctype == "channel":
 		r = resp['user']
 		cprint(f"#fMBroadcaster: {r['displayName']} - {r['login']} (ID: `{r['id']}`)#r")
 		cprint(f"#fRDescription: {r['description']}#r")
 		cprint(f"#fYChannel Created At: {r['createdAt']}#r")
 		r = r['roles']
 		cprint(f"#fBRoles: Affiliate={r['isAffiliate']} - Partner={r['isPartner']}#r")
-		cprint(f"Site Roles: Staff={r['isStaff']} - GlobalMod={r['isGlobalMod']} - SiteAdmin={r['isSiteAdmin']}")
+		# cprint(f"Site Roles: Staff={r['isStaff']} - GlobalMod={r['isGlobalMod']} - SiteAdmin={r['isSiteAdmin']}")
 
 	# Done!
```

### Comparing `VodBot-1.1.5/vodbot/commands/init.py` & `VodBot-1.1.6/vodbot/commands/init.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/commands/pull.py` & `VodBot-1.1.6/vodbot/commands/pull.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/commands/stage.py` & `VodBot-1.1.6/vodbot/commands/stage.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/commands/upload.py` & `VodBot-1.1.6/vodbot/commands/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 	# create media file, upload in chunks
 	media_file = MediaFileUpload(str(tmpfile), chunksize=conf.upload.chunk_size, resumable=True)
 
 	# create upload request and execute
 	response_upload = service.videos().insert(
 		part="snippet,status",
 		body=request_body,
-		notifySubscribers=Config.upload.notify_subscribers,
+		notifySubscribers=conf.upload.notify_subscribers,
 		media_body=media_file
 	)
 
 	filesize = media_file.size()
 
 	cprint(f"#c#fCUploading stage video #r`#fM{stagedata.id}#r`: #fC0#fY%#r #d(0/{format_size(filesize)})...#r", end="\r")
 	uploaded = _upload_artifact(f"stage video #r`#fM{stagedata.id}#r`", response_upload, getting_video=True, filesize=filesize)
```

### Comparing `VodBot-1.1.5/vodbot/config.py` & `VodBot-1.1.6/vodbot/config.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/itd/download.py` & `VodBot-1.1.6/vodbot/itd/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 class JoiningFailed(Exception):
 	pass
 
 def get_playlist_uris(video_id: str, access_token: dict):
 	"""
 	Grabs the URI's for accessing each of the video chunks.
 	"""
-	url = f"http://usher.twitch.tv/vod/{video_id}"
+	url = f"http://usher.ttvnw.net/vod/{video_id}"
 
-	resp = requests.get(url, params={
+	resp = requests.get(url, timeout=5, params={
 		"nauth": access_token['value'],
 		"nauthsig": access_token['signature'],
 		"allow_source": "true",
 		"player": "twitchweb",
 	})
 	resp.raise_for_status()
 
@@ -114,8 +114,8 @@
 	# Get proper clip file URL
 	source_url = gql.get_clip_source(clip_slug)
 
 	# Download file to path
 	size, _ = worker.download_file(source_url, path, conf.pull.connection_retries, conf.pull.connection_timeout, conf.pull.chunk_size)
 
 	# Print progress
-	cprint(f"#fM#lClip#r `#fM{clip_slug}#r` ({clip_id}) #fB#l{format_size(size)}#r")
+	cprint(f"#fM#lClip#r `#fM{clip_slug}#r` ({clip_id}) #fB#l{format_size(size)}#r")
```

### Comparing `VodBot-1.1.5/vodbot/itd/gql.py` & `VodBot-1.1.6/vodbot/itd/gql.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,21 @@
 		creator {{ id login displayName }}
 }}  }}
 """
 # Single Clip query
 GET_CLIP_QUERY = """
 {{  clip(slug: "{clip_slug}") {{
 		videoQualities {{ frameRate quality sourceURL }}
+		id slug title
+		createdAt viewCount
+		durationSeconds url videoOffsetSeconds
+		video {{ id }}
+		game {{ id name }}
+		broadcaster {{ id displayName login }}
+		curator {{ id displayName login }}
 }}  }}
 """
 # Single Channel info query
 GET_CHANNEL_QUERY = """
 {{  user(login: "{channel_id}") {{
 		id login displayName
 		description createdAt
```

### Comparing `VodBot-1.1.5/vodbot/itd/worker.py` & `VodBot-1.1.6/vodbot/itd/worker.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/printer.py` & `VodBot-1.1.6/vodbot/printer.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/thumbnail.py` & `VodBot-1.1.6/vodbot/thumbnail.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/twitch.py` & `VodBot-1.1.6/vodbot/twitch.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/util.py` & `VodBot-1.1.6/vodbot/util.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/video.py` & `VodBot-1.1.6/vodbot/video.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.5/vodbot/webhook.py` & `VodBot-1.1.6/vodbot/webhook.py`

 * *Files identical despite different names*

