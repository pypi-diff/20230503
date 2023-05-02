# Comparing `tmp/TikTokLive-5.0.7.tar.gz` & `tmp/TikTokLive-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TikTokLive-5.0.7.tar", last modified: Sat Feb 25 05:36:20 2023, max compression
+gzip compressed data, was "TikTokLive-5.0.8.tar", last modified: Tue May  2 23:05:56 2023, max compression
```

## Comparing `TikTokLive-5.0.7.tar` & `TikTokLive-5.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 05:36:20.890053 TikTokLive-5.0.7/
--rw-rw-rw-   0        0        0     1089 2022-07-22 17:03:18.000000 TikTokLive-5.0.7/LICENSE
--rw-rw-rw-   0        0        0    29312 2023-02-25 05:36:20.889040 TikTokLive-5.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    28377 2023-02-23 05:22:11.000000 TikTokLive-5.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-02-25 05:36:20.794541 TikTokLive-5.0.7/TikTokLive/
--rw-rw-rw-   0        0        0       45 2022-07-22 17:03:18.000000 TikTokLive-5.0.7/TikTokLive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-25 05:36:20.840040 TikTokLive-5.0.7/TikTokLive/client/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:03:18.000000 TikTokLive-5.0.7/TikTokLive/client/__init__.py
--rw-rw-rw-   0        0        0    21431 2023-02-23 07:01:38.000000 TikTokLive-5.0.7/TikTokLive/client/base.py
--rw-rw-rw-   0        0        0     7544 2023-02-23 03:31:08.000000 TikTokLive-5.0.7/TikTokLive/client/client.py
--rw-rw-rw-   0        0        0     2081 2023-01-19 23:23:14.000000 TikTokLive-5.0.7/TikTokLive/client/config.py
--rw-rw-rw-   0        0        0     9897 2023-02-21 08:01:40.000000 TikTokLive-5.0.7/TikTokLive/client/httpx.py
--rw-rw-rw-   0        0        0     4894 2023-02-20 21:46:05.000000 TikTokLive-5.0.7/TikTokLive/client/wsclient.py
-drwxrwxrwx   0        0        0        0 2023-02-25 05:36:20.863040 TikTokLive-5.0.7/TikTokLive/proto/
--rw-rw-rw-   0        0        0       51 2022-07-22 17:03:18.000000 TikTokLive-5.0.7/TikTokLive/proto/__init__.py
--rw-rw-rw-   0        0        0    41517 2023-02-23 03:17:35.000000 TikTokLive-5.0.7/TikTokLive/proto/tiktok_schema_pb2.py
--rw-rw-rw-   0        0        0     3040 2023-02-23 04:40:40.000000 TikTokLive-5.0.7/TikTokLive/proto/utilities.py
-drwxrwxrwx   0        0        0        0 2023-02-25 05:36:20.888060 TikTokLive-5.0.7/TikTokLive/types/
--rw-rw-rw-   0        0        0       45 2022-07-22 17:03:18.000000 TikTokLive-5.0.7/TikTokLive/types/__init__.py
--rw-rw-rw-   0        0        0     3517 2023-02-21 07:53:35.000000 TikTokLive-5.0.7/TikTokLive/types/errors.py
--rw-rw-rw-   0        0        0    14837 2023-02-23 06:03:34.000000 TikTokLive-5.0.7/TikTokLive/types/events.py
--rw-rw-rw-   0        0        0    15255 2023-02-25 05:35:02.000000 TikTokLive-5.0.7/TikTokLive/types/objects.py
--rw-rw-rw-   0        0        0     1066 2023-02-21 07:43:33.000000 TikTokLive-5.0.7/TikTokLive/types/utilities.py
--rw-rw-rw-   0        0        0     1403 2023-02-20 20:58:20.000000 TikTokLive-5.0.7/TikTokLive/utilities.py
-drwxrwxrwx   0        0        0        0 2023-02-25 05:36:20.816799 TikTokLive-5.0.7/TikTokLive.egg-info/
--rw-rw-rw-   0        0        0    29312 2023-02-25 05:36:20.000000 TikTokLive-5.0.7/TikTokLive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      649 2023-02-25 05:36:20.000000 TikTokLive-5.0.7/TikTokLive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 05:36:20.000000 TikTokLive-5.0.7/TikTokLive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-02-25 05:36:20.000000 TikTokLive-5.0.7/TikTokLive.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-25 05:36:20.000000 TikTokLive-5.0.7/TikTokLive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-25 05:36:20.890053 TikTokLive-5.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1663 2023-02-25 05:35:42.000000 TikTokLive-5.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:05:56.211274 TikTokLive-5.0.8/
+-rw-rw-rw-   0        0        0     1089 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/LICENSE
+-rw-rw-rw-   0        0        0    31366 2023-05-02 23:05:56.210274 TikTokLive-5.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    30454 2023-05-02 22:57:01.000000 TikTokLive-5.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 23:05:56.173286 TikTokLive-5.0.8/TikTokLive/
+-rw-rw-rw-   0        0        0       45 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:05:56.202277 TikTokLive-5.0.8/TikTokLive/client/
+-rw-rw-rw-   0        0        0        0 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/client/__init__.py
+-rw-rw-rw-   0        0        0    21839 2023-04-30 21:26:16.000000 TikTokLive-5.0.8/TikTokLive/client/base.py
+-rw-rw-rw-   0        0        0     7645 2023-05-02 22:35:41.000000 TikTokLive-5.0.8/TikTokLive/client/client.py
+-rw-rw-rw-   0        0        0     2081 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/client/config.py
+-rw-rw-rw-   0        0        0    10340 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/client/httpx.py
+-rw-rw-rw-   0        0        0     4894 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/client/wsclient.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:05:56.204276 TikTokLive-5.0.8/TikTokLive/proto/
+-rw-rw-rw-   0        0        0       51 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/proto/__init__.py
+-rw-rw-rw-   0        0        0    19933 2023-05-02 22:32:03.000000 TikTokLive-5.0.8/TikTokLive/proto/tiktok_schema_pb2.py
+-rw-rw-rw-   0        0        0     3083 2023-05-02 21:10:35.000000 TikTokLive-5.0.8/TikTokLive/proto/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:05:56.209275 TikTokLive-5.0.8/TikTokLive/types/
+-rw-rw-rw-   0        0        0       45 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/types/__init__.py
+-rw-rw-rw-   0        0        0     3517 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/types/errors.py
+-rw-rw-rw-   0        0        0    16773 2023-05-02 22:35:41.000000 TikTokLive-5.0.8/TikTokLive/types/events.py
+-rw-rw-rw-   0        0        0    15652 2023-05-02 22:39:15.000000 TikTokLive-5.0.8/TikTokLive/types/objects.py
+-rw-rw-rw-   0        0        0     1066 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/types/utilities.py
+-rw-rw-rw-   0        0        0     1403 2023-04-30 20:16:28.000000 TikTokLive-5.0.8/TikTokLive/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:05:56.196284 TikTokLive-5.0.8/TikTokLive.egg-info/
+-rw-rw-rw-   0        0        0    31366 2023-05-02 23:05:56.000000 TikTokLive-5.0.8/TikTokLive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      649 2023-05-02 23:05:56.000000 TikTokLive-5.0.8/TikTokLive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 23:05:56.000000 TikTokLive-5.0.8/TikTokLive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-05-02 23:05:56.000000 TikTokLive-5.0.8/TikTokLive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-02 23:05:56.000000 TikTokLive-5.0.8/TikTokLive.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 23:05:56.211274 TikTokLive-5.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2023-05-02 22:39:39.000000 TikTokLive-5.0.8/setup.py
```

### Comparing `TikTokLive-5.0.7/LICENSE` & `TikTokLive-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TikTokLive-5.0.7/PKG-INFO` & `TikTokLive-5.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: TikTokLive
-Version: 5.0.7
-Summary: TikTok Live Connection Client
-Home-page: https://github.com/isaackogan/TikTokLive
-Author: Isaac Kogan
-Author-email: info@isaackogan.com
-License: MIT
-Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v5.0.7
-Keywords: tiktok,tiktok live,python3,api,unofficial
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 TikTokLive
 ==================
 A python library to connect to and read events from TikTok's LIVE service.
 
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/isaac-kogan-5a45b9193/ )
 [![HitCount](https://hits.dwyl.com/isaackogan/TikTokLive.svg?style=flat)](http://hits.dwyl.com/isaackogan/TikTokLive)
 ![Downloads](https://pepy.tech/badge/TikTokLive)
@@ -44,14 +20,22 @@
 by [@zerodytrash](https://github.com/zerodytrash/), but has since taken on its own identity as it has added more features & changed much of its core functionality.
 
 
 Join the [support discord](https://discord.gg/e2XwPNTBBr) and visit the `#support` channel for questions, contributions and ideas. Feel free to make pull requests with missing/new features, fixes, etc.
 
 > **UPDATE:**<br>Due to a change on the part of TikTok, versions prior to **v4.3.8** are no longer functional. If you are using an unsupported version, upgrade to the latest version using the `pip install TikTokLive --upgrade` command.
 
+## Other Languages
+
+TikTok LIVE is availible in several alternative languages with only slight differences between the versions:
+
+- **Node.JS:** https://github.com/zerodytrash/TikTok-Live-Connector
+- **Go:** https://github.com/Davincible/gotiktoklive
+- **C#/Unity:** https://github.com/frankvHoof93/TikTokLiveSharp
+
 ## Table of Contents
 
 **Primary Information**
 
 - [Documentation](https://isaackogan.github.io/TikTokLive/)
 - [Contributors](#contributors)
 - [License](#license)
@@ -107,46 +91,46 @@
 
 if __name__ == '__main__':
     # Run the client and block the main thread
     # await client.start() to run non-blocking
     client.run()
 ```
 
-For more examples, [see the examples folder](https://github.com/isaackogan/TikTok-Live-Connector/tree/master/examples) provided in the tree.
+For more examples, [see the examples folder](https://github.com/isaackogan/TikTokLive/tree/master/examples) provided in the tree.
 
 ## Params & Options
 
 To create a new `TikTokLiveClient` object the following parameter is required. You can optionally add configuration options to this via kwargs.
 
 `TikTokLiveClient(unique_id, **options)`
 
-| Param Name | Required | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-|------------|----------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| unique_id  | Yes      | The unique username of the broadcaster. You can find this name in the URL.<br>Example: `https://www.tiktok.com/@isaackogz` => `isaackogz`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-| **options  | No       | Here you can set the following optional connection properties. If you do not specify a value, the default value will be used.<br><br>`process_initial_data` (default: `True`) <br> Define if you want to process initial data upon connecting (e.g. first 1-10 messages from BEFORE you connected).<br><br>`fetch_room_info_on_connect` (default: `True`) <br> Define if you want to fetch all room information on start. If this option is enabled, connection to offline rooms will be prevented. If enabled, the connect result contains the room info via the `room_info` attribute. You can also manually retrieve the room info (even in an unconnected state) using the `retrieve_room_info()` method.<br><br>`enable_detailed_gifts` (default: `False`) <br> Define if you want to receive extended information about gifts like gift name, cost and images which you can retrieve via the `available_gifts` attribute. When enabled, the `details` attribute in a `Gift` object will be populated.<br><br>`ws_ping_interval` (default: `10.0`) <br> The interval between keepalive pings on the websocket connection (in seconds).<br><br>`ws_timeout` (default: `10.0`)<br>How long to wait before the websocket connection is considered timed out (in seconds).<br><br>`http_timeout` (default: `10.0`) <br> How long to wait before considering an HTTP request in the http client timed out (in seconds).<br><br>`http_headers` (default: `{}`) <br> Additional HTTP client headers to include when making requests to the Webcast API AND connecting to the websocket server.<br><br>`http_params` (default: `{}`) <br>Additional HTTP client parameters to include when making requests to the Webcast API AND connecting to the websocket.<br><br>`loop` (default: `None`)<br>Optionally supply your own asyncio event loop for usage by the client. When set to None, the client pulls the current active loop or creates a new one. This option is mostly useful for people trying to nest asyncio.<br/><br/>`trust_env` (default: `False`)<br/>Whether to trust environment variables that provide proxies in httpx requests<br/><br/>`proxies` (default: `None`)<br/>Enable proxied requests by turning on forwarding for the HTTP "proxies" argument. Websocket connections will NOT be proxied<br/><br/>`lang` (default: `en-US`)<br/>Change the language. Payloads *will* be in English, but front-end content will be in the desired language!<br/><br/>`sign_api_key` (default: `None`)<br/>Parameter to increase the amount of connections allowed to be made per minute via a Sign Server API key. If you need this, contact the project maintainer. |
+| Param Name | Required | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+|------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| unique_id  | Yes      | The unique username of the broadcaster. You can find this name in the URL.<br>Example: `https://www.tiktok.com/@isaackogz` => `isaackogz`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| **options  | No       | Here you can set the following optional connection properties. If you do not specify a value, the default value will be used.<br><br>`process_initial_data` (default: `True`) <br> Define if you want to process initial data upon connecting (e.g. first 1-10 messages from BEFORE you connected).<br><br>`fetch_room_info_on_connect` (default: `True`) <br> Define if you want to fetch all room information on start. If this option is enabled, connection to offline rooms will be prevented. If enabled, the connect result contains the room info via the `room_info` attribute. You can also manually retrieve the room info (even in an unconnected state) using the `retrieve_room_info()` method.<br><br>`enable_detailed_gifts` (default: `False`) <br> Define if you want to receive extended information about gifts like gift name, cost and images which you can retrieve via the `available_gifts` attribute. When enabled, the `details` attribute in a `Gift` object will be populated.<br><br>`ws_ping_interval` (default: `10.0`) <br> The interval between keepalive pings on the websocket connection (in seconds).<br><br>`ws_timeout` (default: `10.0`)<br>How long to wait before the websocket connection is considered timed out (in seconds).<br><br>`http_timeout` (default: `10.0`) <br> How long to wait before considering an HTTP request in the http client timed out (in seconds).<br><br>`http_headers` (default: `{}`) <br> Additional HTTP client headers to include when making requests to the Webcast API AND connecting to the websocket server.<br><br>`http_params` (default: `{}`) <br>Additional HTTP client parameters to include when making requests to the Webcast API AND connecting to the websocket.<br><br>`loop` (default: `None`)<br>Optionally supply your own asyncio event loop for usage by the client. When set to None, the client pulls the current active loop or creates a new one. This option is mostly useful for people trying to nest asyncio.<br/><br/>`trust_env` (default: `False`)<br/>Whether to trust environment variables that provide proxies in httpx requests<br/><br/>`proxies` (default: `None`)<br/>Enable proxied requests by turning on forwarding for the HTTP "proxies" argument. Websocket connections will NOT be proxied<br/><br/>`lang` (default: `en-US`)<br/>Change the language. Payloads *will* be in English, but front-end content will be in the desired language!<br/><br/>`sign_api_key` (default: `None`)<br/>Parameter to increase the amount of connections allowed to be made per minute via a Sign Server API key. If you need this, contact the project maintainer.<br/><br/>`ssl_context` (default: `None`)<br/>Providing an SSLContext object overrides the default context used in HTTP requests made to TikTok. This is useful if TikTok sends invalid SSL signatures, as you can provide a "no verify" context. |
 
 
 ## Methods
 
-A `TikTokLiveClient` object contains the following methods.
+A `TikTokLiveClient` object contains the following methods:
 
-| Method Name              | Description                                                                                                                                                                       |
-|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| run                      | Starts a connection to the live chat while blocking the main thread                                                                                                               |
-| start                    | (async) Connects to the live chat without blocking the main thread                                                                                                                |
-| stop                     | Turns off the connection to the live chat.                                                                                                                                        |
-| retrieve_room_info       | (async) Gets the current room info from TikTok API                                                                                                                                |
-| retrieve_available_gifts | (async) Retrieves a list of the available gifts for the room and adds it to the `extended_gift` attribute of the `Gift` object on the `gift` event, when enabled.                 |
-| add_listener             | Adds an *asynchronous* listener function (or, you can decorate a function with `@client.on("<event>")`) and takes two parameters, an event name and the payload, an AbstractEvent ||
-| download                 | Start downloading the livestream video for a given duration or until stopped via the `stop_download` method                                                                       |
-| stop_download            | Stop downloading the livestream video if currently downloading, otherwise throws an error                                                                                         |
+| Method Name              | Description                                                                                                                                                                                                                   |
+|--------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| run                      | Starts a connection to the live chat while blocking the main thread                                                                                                                                                           |
+| start                    | (async) Connects to the live chat without blocking the main thread                                                                                                                                                            |
+| stop                     | Turns off the connection to the live chat.                                                                                                                                                                                    |
+| retrieve_room_info       | (async) Gets the current room info from TikTok API                                                                                                                                                                            |
+| retrieve_available_gifts | (async) Retrieves a list of the available gifts for the room and adds it to the `extended_gift` attribute of the `Gift` object on the `gift` event, when enabled.                                                             |
+| add_listener             | Adds an *asynchronous* listener function (or, you can decorate a function with `@client.on("<event>")`) and takes two parameters, an event name and the payload, an AbstractEvent                                             ||
+| download                 | Start downloading the livestream video for a given duration or until stopped via the `stop_download` method. Supports the ability to add different flags, like `-c copy` which may reduce CPU usage by disabling transcoding. |
+| stop_download            | Stop downloading the livestream video if currently downloading, otherwise throws an error                                                                                                                                     |
 
 ## Attributes
 
-A `TikTokLiveClient` object contains the following attributes.
+A `TikTokLiveClient` object contains the following attributes:
 
 | Attribute Name  | Description                                                                                                                                  |
 |-----------------|----------------------------------------------------------------------------------------------------------------------------------------------|
 | room_id         | The Room ID of the livestream room the client is currently connected to                                                                      |
 | room_info       | Information about the given livestream room                                                                                                  |
 | unique_id       | The TikTok username of the person whose livestream the client is currently connected to (e.g. @charlidamelio)                                |
 | connected       | Whether the client is currently connected to a livestream                                                                                    |
@@ -261,15 +245,15 @@
 ### `more_share`
 
 Triggered when 5 or 10 users join from a viewer's share link.
 
 ```python
 @client.on("more_share")
 async def on_connect(event: MoreShareEvent):
-    print(f"More than {event.amount} users have joined from {user.unique_id}'s share link!")
+    print(f"More than {event.amount} users have joined from {event.user.unique_id}'s share link!")
 ```
 
 
 ### `viewer_update`
 
 Triggered every time the viewer count is updated. This event also updates the cached viewer count by default.
 
@@ -313,22 +297,32 @@
 
 ```python
 @client.on("envelope")
 async def on_connect(event: EnvelopeEvent):
     print(f"{event.treasure_box_user.unique_id} -> {event.treasure_box_data}")
 ```
 
-### `weekly_ranking`
+### `ranking_update`
+
+Triggered when a **stream** rank update is sent out. Can be `Weekly Ranking` or `Rising Star`!
 
-Triggered when a weekly ranking update is sent out.
+```python
+@client.on("ranking_update")
+async def on_connect(event: RankingUpdateEvent):
+    print(f"{event.user.unique_id} has the rank #{event.rank} for the {event.type} leaderboard.")
+```
+
+### `user_ranking_update`
 
+Triggered when a **user** rank update is sent out. Can be `Top Viewer`
+ status.
 ```python
-@client.on("weekly_ranking")
-async def on_connect(event: WeeklyRankingEvent):
-    print(f"{client.unique_id} has the rank #{event.data.rank} of all streamers!")
+@client.on("user_ranking_update")
+async def on_connect(event: UserRankingUpdateEvent):
+    print(f"{event.user.unique_id} just became a #{event.rank} top viewer!")
 ```
 
 ### `mic_battle_start`
 
 Triggered when a Mic Battle starts!
 
 ```python
@@ -422,9 +416,7 @@
 * **David Teather** - *TikTokLive Introduction Tutorial* - [davidteather](https://github.com/davidteather)
 
 See also the full list of [contributors](https://github.com/isaackogan/TikTokLive/contributors) who have participated in this project.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-
```

### Comparing `TikTokLive-5.0.7/README.md` & `TikTokLive-5.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: TikTokLive
+Version: 5.0.8
+Summary: TikTok Live Connection Client
+Home-page: https://github.com/isaackogan/TikTokLive
+Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v5.0.8
+Author: Isaac Kogan
+Author-email: info@isaackogan.com
+License: MIT
+Keywords: tiktok,tiktok live,python3,api,unofficial
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 TikTokLive
 ==================
 A python library to connect to and read events from TikTok's LIVE service.
 
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/isaac-kogan-5a45b9193/ )
 [![HitCount](https://hits.dwyl.com/isaackogan/TikTokLive.svg?style=flat)](http://hits.dwyl.com/isaackogan/TikTokLive)
 ![Downloads](https://pepy.tech/badge/TikTokLive)
@@ -20,14 +43,22 @@
 by [@zerodytrash](https://github.com/zerodytrash/), but has since taken on its own identity as it has added more features & changed much of its core functionality.
 
 
 Join the [support discord](https://discord.gg/e2XwPNTBBr) and visit the `#support` channel for questions, contributions and ideas. Feel free to make pull requests with missing/new features, fixes, etc.
 
 > **UPDATE:**<br>Due to a change on the part of TikTok, versions prior to **v4.3.8** are no longer functional. If you are using an unsupported version, upgrade to the latest version using the `pip install TikTokLive --upgrade` command.
 
+## Other Languages
+
+TikTok LIVE is availible in several alternative languages with only slight differences between the versions:
+
+- **Node.JS:** https://github.com/zerodytrash/TikTok-Live-Connector
+- **Go:** https://github.com/Davincible/gotiktoklive
+- **C#/Unity:** https://github.com/frankvHoof93/TikTokLiveSharp
+
 ## Table of Contents
 
 **Primary Information**
 
 - [Documentation](https://isaackogan.github.io/TikTokLive/)
 - [Contributors](#contributors)
 - [License](#license)
@@ -83,46 +114,46 @@
 
 if __name__ == '__main__':
     # Run the client and block the main thread
     # await client.start() to run non-blocking
     client.run()
 ```
 
-For more examples, [see the examples folder](https://github.com/isaackogan/TikTok-Live-Connector/tree/master/examples) provided in the tree.
+For more examples, [see the examples folder](https://github.com/isaackogan/TikTokLive/tree/master/examples) provided in the tree.
 
 ## Params & Options
 
 To create a new `TikTokLiveClient` object the following parameter is required. You can optionally add configuration options to this via kwargs.
 
 `TikTokLiveClient(unique_id, **options)`
 
-| Param Name | Required | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-|------------|----------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| unique_id  | Yes      | The unique username of the broadcaster. You can find this name in the URL.<br>Example: `https://www.tiktok.com/@isaackogz` => `isaackogz`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-| **options  | No       | Here you can set the following optional connection properties. If you do not specify a value, the default value will be used.<br><br>`process_initial_data` (default: `True`) <br> Define if you want to process initial data upon connecting (e.g. first 1-10 messages from BEFORE you connected).<br><br>`fetch_room_info_on_connect` (default: `True`) <br> Define if you want to fetch all room information on start. If this option is enabled, connection to offline rooms will be prevented. If enabled, the connect result contains the room info via the `room_info` attribute. You can also manually retrieve the room info (even in an unconnected state) using the `retrieve_room_info()` method.<br><br>`enable_detailed_gifts` (default: `False`) <br> Define if you want to receive extended information about gifts like gift name, cost and images which you can retrieve via the `available_gifts` attribute. When enabled, the `details` attribute in a `Gift` object will be populated.<br><br>`ws_ping_interval` (default: `10.0`) <br> The interval between keepalive pings on the websocket connection (in seconds).<br><br>`ws_timeout` (default: `10.0`)<br>How long to wait before the websocket connection is considered timed out (in seconds).<br><br>`http_timeout` (default: `10.0`) <br> How long to wait before considering an HTTP request in the http client timed out (in seconds).<br><br>`http_headers` (default: `{}`) <br> Additional HTTP client headers to include when making requests to the Webcast API AND connecting to the websocket server.<br><br>`http_params` (default: `{}`) <br>Additional HTTP client parameters to include when making requests to the Webcast API AND connecting to the websocket.<br><br>`loop` (default: `None`)<br>Optionally supply your own asyncio event loop for usage by the client. When set to None, the client pulls the current active loop or creates a new one. This option is mostly useful for people trying to nest asyncio.<br/><br/>`trust_env` (default: `False`)<br/>Whether to trust environment variables that provide proxies in httpx requests<br/><br/>`proxies` (default: `None`)<br/>Enable proxied requests by turning on forwarding for the HTTP "proxies" argument. Websocket connections will NOT be proxied<br/><br/>`lang` (default: `en-US`)<br/>Change the language. Payloads *will* be in English, but front-end content will be in the desired language!<br/><br/>`sign_api_key` (default: `None`)<br/>Parameter to increase the amount of connections allowed to be made per minute via a Sign Server API key. If you need this, contact the project maintainer. |
+| Param Name | Required | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+|------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| unique_id  | Yes      | The unique username of the broadcaster. You can find this name in the URL.<br>Example: `https://www.tiktok.com/@isaackogz` => `isaackogz`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| **options  | No       | Here you can set the following optional connection properties. If you do not specify a value, the default value will be used.<br><br>`process_initial_data` (default: `True`) <br> Define if you want to process initial data upon connecting (e.g. first 1-10 messages from BEFORE you connected).<br><br>`fetch_room_info_on_connect` (default: `True`) <br> Define if you want to fetch all room information on start. If this option is enabled, connection to offline rooms will be prevented. If enabled, the connect result contains the room info via the `room_info` attribute. You can also manually retrieve the room info (even in an unconnected state) using the `retrieve_room_info()` method.<br><br>`enable_detailed_gifts` (default: `False`) <br> Define if you want to receive extended information about gifts like gift name, cost and images which you can retrieve via the `available_gifts` attribute. When enabled, the `details` attribute in a `Gift` object will be populated.<br><br>`ws_ping_interval` (default: `10.0`) <br> The interval between keepalive pings on the websocket connection (in seconds).<br><br>`ws_timeout` (default: `10.0`)<br>How long to wait before the websocket connection is considered timed out (in seconds).<br><br>`http_timeout` (default: `10.0`) <br> How long to wait before considering an HTTP request in the http client timed out (in seconds).<br><br>`http_headers` (default: `{}`) <br> Additional HTTP client headers to include when making requests to the Webcast API AND connecting to the websocket server.<br><br>`http_params` (default: `{}`) <br>Additional HTTP client parameters to include when making requests to the Webcast API AND connecting to the websocket.<br><br>`loop` (default: `None`)<br>Optionally supply your own asyncio event loop for usage by the client. When set to None, the client pulls the current active loop or creates a new one. This option is mostly useful for people trying to nest asyncio.<br/><br/>`trust_env` (default: `False`)<br/>Whether to trust environment variables that provide proxies in httpx requests<br/><br/>`proxies` (default: `None`)<br/>Enable proxied requests by turning on forwarding for the HTTP "proxies" argument. Websocket connections will NOT be proxied<br/><br/>`lang` (default: `en-US`)<br/>Change the language. Payloads *will* be in English, but front-end content will be in the desired language!<br/><br/>`sign_api_key` (default: `None`)<br/>Parameter to increase the amount of connections allowed to be made per minute via a Sign Server API key. If you need this, contact the project maintainer.<br/><br/>`ssl_context` (default: `None`)<br/>Providing an SSLContext object overrides the default context used in HTTP requests made to TikTok. This is useful if TikTok sends invalid SSL signatures, as you can provide a "no verify" context. |
 
 
 ## Methods
 
-A `TikTokLiveClient` object contains the following methods.
+A `TikTokLiveClient` object contains the following methods:
 
-| Method Name              | Description                                                                                                                                                                       |
-|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| run                      | Starts a connection to the live chat while blocking the main thread                                                                                                               |
-| start                    | (async) Connects to the live chat without blocking the main thread                                                                                                                |
-| stop                     | Turns off the connection to the live chat.                                                                                                                                        |
-| retrieve_room_info       | (async) Gets the current room info from TikTok API                                                                                                                                |
-| retrieve_available_gifts | (async) Retrieves a list of the available gifts for the room and adds it to the `extended_gift` attribute of the `Gift` object on the `gift` event, when enabled.                 |
-| add_listener             | Adds an *asynchronous* listener function (or, you can decorate a function with `@client.on("<event>")`) and takes two parameters, an event name and the payload, an AbstractEvent ||
-| download                 | Start downloading the livestream video for a given duration or until stopped via the `stop_download` method                                                                       |
-| stop_download            | Stop downloading the livestream video if currently downloading, otherwise throws an error                                                                                         |
+| Method Name              | Description                                                                                                                                                                                                                   |
+|--------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| run                      | Starts a connection to the live chat while blocking the main thread                                                                                                                                                           |
+| start                    | (async) Connects to the live chat without blocking the main thread                                                                                                                                                            |
+| stop                     | Turns off the connection to the live chat.                                                                                                                                                                                    |
+| retrieve_room_info       | (async) Gets the current room info from TikTok API                                                                                                                                                                            |
+| retrieve_available_gifts | (async) Retrieves a list of the available gifts for the room and adds it to the `extended_gift` attribute of the `Gift` object on the `gift` event, when enabled.                                                             |
+| add_listener             | Adds an *asynchronous* listener function (or, you can decorate a function with `@client.on("<event>")`) and takes two parameters, an event name and the payload, an AbstractEvent                                             ||
+| download                 | Start downloading the livestream video for a given duration or until stopped via the `stop_download` method. Supports the ability to add different flags, like `-c copy` which may reduce CPU usage by disabling transcoding. |
+| stop_download            | Stop downloading the livestream video if currently downloading, otherwise throws an error                                                                                                                                     |
 
 ## Attributes
 
-A `TikTokLiveClient` object contains the following attributes.
+A `TikTokLiveClient` object contains the following attributes:
 
 | Attribute Name  | Description                                                                                                                                  |
 |-----------------|----------------------------------------------------------------------------------------------------------------------------------------------|
 | room_id         | The Room ID of the livestream room the client is currently connected to                                                                      |
 | room_info       | Information about the given livestream room                                                                                                  |
 | unique_id       | The TikTok username of the person whose livestream the client is currently connected to (e.g. @charlidamelio)                                |
 | connected       | Whether the client is currently connected to a livestream                                                                                    |
@@ -237,15 +268,15 @@
 ### `more_share`
 
 Triggered when 5 or 10 users join from a viewer's share link.
 
 ```python
 @client.on("more_share")
 async def on_connect(event: MoreShareEvent):
-    print(f"More than {event.amount} users have joined from {user.unique_id}'s share link!")
+    print(f"More than {event.amount} users have joined from {event.user.unique_id}'s share link!")
 ```
 
 
 ### `viewer_update`
 
 Triggered every time the viewer count is updated. This event also updates the cached viewer count by default.
 
@@ -289,22 +320,32 @@
 
 ```python
 @client.on("envelope")
 async def on_connect(event: EnvelopeEvent):
     print(f"{event.treasure_box_user.unique_id} -> {event.treasure_box_data}")
 ```
 
-### `weekly_ranking`
+### `ranking_update`
+
+Triggered when a **stream** rank update is sent out. Can be `Weekly Ranking` or `Rising Star`!
+
+```python
+@client.on("ranking_update")
+async def on_connect(event: RankingUpdateEvent):
+    print(f"{event.user.unique_id} has the rank #{event.rank} for the {event.type} leaderboard.")
+```
 
-Triggered when a weekly ranking update is sent out.
+### `user_ranking_update`
 
+Triggered when a **user** rank update is sent out. Can be `Top Viewer`
+ status.
 ```python
-@client.on("weekly_ranking")
-async def on_connect(event: WeeklyRankingEvent):
-    print(f"{client.unique_id} has the rank #{event.data.rank} of all streamers!")
+@client.on("user_ranking_update")
+async def on_connect(event: UserRankingUpdateEvent):
+    print(f"{event.user.unique_id} just became a #{event.rank} top viewer!")
 ```
 
 ### `mic_battle_start`
 
 Triggered when a Mic Battle starts!
 
 ```python
```

### Comparing `TikTokLive-5.0.7/TikTokLive/client/base.py` & `TikTokLive-5.0.8/TikTokLive/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import json
 import logging
 import os
 import signal
 from asyncio import AbstractEventLoop, Task
 from datetime import datetime
+from ssl import SSLContext
 from threading import Thread
 from typing import Optional, List, Dict, Set, Union
 
 import websockets
 from ffmpy import FFmpeg, FFRuntimeError
 
 from TikTokLive.client import config, wsclient
@@ -39,15 +40,16 @@
             ws_headers: Optional[dict] = None,
             process_initial_data: bool = True,
             enable_detailed_gifts: bool = False,
             trust_env: bool = False,
             proxies: Optional[Dict[str, str]] = None,
             lang: Optional[str] = "en-US",
             fetch_room_info_on_connect: bool = True,
-            sign_api_key: Optional[str] = None
+            sign_api_key: Optional[str] = None,
+            ssl_context: Optional[SSLContext] = None
     ):
         """
         Initialize the base client
 
         :param unique_id: The unique id of the creator to connect to.
         :param loop: Optionally supply your own asyncio loop.
         :param http_params: Additional HTTP client parameters to include when making requests to the Webcast API AND connecting to the websocket server.
@@ -58,26 +60,28 @@
         :param process_initial_data: Whether to process the initial data (including cached chats).
         :param enable_detailed_gifts: Whether to retrieve extended (detailed) gift info including its icon & other important things.
         :param trust_env: Whether to trust environment variables that provide proxies to be used in HTTP requests.
         :param proxies: Enable proxied requests by turning on forwarding for the HTTP "proxies" argument. Websocket connections will NOT be proxied.
         :param lang: Change the language. Payloads *will* be in English, but this will change stuff like the extended_gift Gift attribute to the desired language!
         :param fetch_room_info_on_connect: Whether to fetch room info on connect. If disabled, you might attempt to connect to a closed livestream.
         :param sign_api_key: Parameter to increase the amount of connections allowed to be made per minute via a Sign Server API key. If you need this, contact the project maintainer.
+        :param ssl_context: Add the option to modify the SSL context of the websocket connection request and httpx requests
         """
 
         # Event loop. On connect, this will be filled if None
         self.loop: Optional[AbstractEventLoop] = self.__get_event_loop(loop)
 
         # Managed Attributes
         self.__room_info: Optional[dict] = None
         self.__available_gifts: Dict[int, GiftDetailed] = dict()
         self.__unique_id: str = validate_and_normalize_unique_id(unique_id)
         self.__room_id: Optional[int] = None
         self.__connecting: bool = False
         self.__connected: bool = False
+        self.__ssl_context: Optional[SSLContext] = ssl_context
         self._ws_connection_task: Optional[Task] = None
 
         # Configured Attributes
         self._ws_headers: Optional[dict] = ws_headers or dict()
         self._ws_ping_interval: float = ws_ping_interval
         self._ws_timeout: float = ws_timeout
         self._process_initial_data: bool = process_initial_data
@@ -88,15 +92,16 @@
         self.http: TikTokHTTPClient = TikTokHTTPClient(
             loop=self.loop,
             headers=http_headers or dict(),
             timeout=http_timeout,
             proxies=proxies,
             trust_env=trust_env,
             params=self.__get_client_params(http_params or dict(), lang),
-            sign_api_key=sign_api_key
+            sign_api_key=sign_api_key,
+            ssl_context=self.__ssl_context
         )
 
         # Websocket Client for Webcast API
         self.websocket: Optional[WebcastWebsocketConnection] = None
 
         # FFMpeg client for video downloads
         self.ffmpeg: Optional[FFmpegWrapper] = None
@@ -128,15 +133,15 @@
             return loop
         else:
             try:
                 return asyncio.get_running_loop()
             except RuntimeError:
                 return asyncio.new_event_loop()
 
-    async def __fetch_room_id(self) -> Optional[int]:
+    async def _fetch_room_id(self) -> Optional[int]:
         """
         Fetch room ID of a given user
 
         :return: Their Room ID
         :raises: asyncio.TimeoutError
 
         """
@@ -146,15 +151,15 @@
             self.__room_id = int(get_room_id_from_main_page_html(html))
             self.http.params["room_id"] = str(self.__room_id)
             return self.__room_id
         except Exception as ex:
             await self._on_error(ex, FailedFetchRoomInfo("Failed to fetch room id from Webcast, see stacktrace for more info."))
             return None
 
-    async def __fetch_room_data(self) -> dict:
+    async def _fetch_room_data(self) -> dict:
         """
         Fetch the websocket URL from the Signing API
 
         :return: Initial Webcast response
 
         """
 
@@ -167,15 +172,15 @@
 
         # Add param if given
         if webcast_response.get("internalExt"):
             self.http.params["internal_ext"] = webcast_response["internalExt"]
 
         return webcast_response
 
-    async def __websocket_connect(self, webcast_response: Dict[str, Union[dict, str]]) -> None:
+    async def _websocket_connect(self, webcast_response: Dict[str, Union[dict, str]]) -> None:
         """
         Attempt to upgrade the connection to a websocket
 
         :param webcast_response: The initial webcast response including the wsParam and wsUrl items
         :return: The websocket, if one is produced
 
         """
@@ -271,44 +276,44 @@
         self.loop: AbstractEventLoop = self.__get_event_loop(self.loop)
         self.http.loop = self.loop
 
         # Set to already connecting
         self.__connecting = True
 
         # Get the Room ID, always
-        await self.__fetch_room_id()
+        await self._fetch_room_id()
 
         # Fetch room info when connecting
         if self._fetch_room_info_on_connect:
             await self.retrieve_room_info()
 
             # If offline
             if self.__room_info.get("status", 4) == 4:
                 raise LiveNotFound("The requested user is most likely offline.")
 
         # Get extended gift info
         if self._enable_detailed_gifts:
             await self.retrieve_available_gifts()
 
         # Make initial request to Webcast, connect to WebSocket server
-        webcast_response: Dict[str, Union[dict, str]] = await self.__fetch_room_data()
+        webcast_response: Dict[str, Union[dict, str]] = await self._fetch_room_data()
 
         if not webcast_response.get("cursor"):
             raise InitialCursorMissing("Missing cursor in initial fetch response.")
 
         # If a WebSocket is offered, upgrade
         if not (webcast_response.get("wsUrl") and webcast_response.get("wsParam")):
             raise WebsocketConnectionFailed("No websocket URL received from TikTok")
 
         # Process initial data if requested
         if self._process_initial_data:
             await self._handle_webcast_messages(webcast_response)
 
         # Blocks current async execution, CONNECTS TO WEBCAST
-        self._ws_connection_task = self.loop.create_task(self.__websocket_connect(webcast_response))
+        self._ws_connection_task = self.loop.create_task(self._websocket_connect(webcast_response))
 
     def _disconnect(self) -> None:
         """
         Set the disconnected status
 
         """
 
@@ -364,15 +369,15 @@
         """
         Run client while blocking main thread
 
         :return: None
 
         """
 
-        self.loop.run_until_complete(self._start())
+        self.loop.run_until_complete(self._start())  # TODO this is the reason the event loop stops. run until complete runs until the future ends, see docs
 
     async def retrieve_room_info(self) -> Optional[dict]:
         """
         Fetch room information from Webcast API
 
         :return: Room info dict
 
@@ -566,15 +571,15 @@
 
         return self.__connected
 
     @property
     def connecting(self) -> bool:
         """
         Whether the client is in the process of connecting
-        
+
         """
 
         return self.__connecting
 
     @property
     def available_gifts(self) -> Dict[int, GiftDetailed]:
         """
```

### Comparing `TikTokLive-5.0.7/TikTokLive/client/client.py` & `TikTokLive-5.0.8/TikTokLive/client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import traceback
 from typing import Optional, List
 
 from pyee import AsyncIOEventEmitter
 
 from .base import WebcastPushConnection
 from ..types import FailedParseMessage, TopViewer
-from ..types.events import AbstractEvent, ConnectEvent, DisconnectEvent, ViewerUpdateEvent, JoinEvent, LikeEvent, FollowEvent, ShareEvent, QuestionEvent, LiveEndEvent, \
-    IntroMessageEvent, EmoteEvent, MicBattleStartEvent, MicBattleUpdateEvent, MoreShareEvent, UnknownEvent, WeeklyRankingEvent, CommentEvent, GiftEvent
+from ..types.events import AbstractEvent, ConnectEvent, DisconnectEvent, ViewerUpdateEvent, JoinEvent, LikeEvent, \
+    FollowEvent, ShareEvent, QuestionEvent, LiveEndEvent, \
+    IntroMessageEvent, EmoteEvent, MicBattleStartEvent, MicBattleUpdateEvent, MoreShareEvent, UnknownEvent, \
+    CommentEvent, GiftEvent, RankingUpdateEvent, UserRankingUpdateEvent
 
 
 class TikTokLiveClient(WebcastPushConnection, AsyncIOEventEmitter):
     """
     TikTokLive Client responsible for emitting events asynchronously
 
     """
@@ -120,20 +122,20 @@
         for message in webcast_response.get("messages", list()):
             # Once we disconnect, stop parsing events
             if self.websocket is None:
                 break
 
             # Parse events & emit them
             try:
-                event: AbstractEvent = self.__parse_webcast_message(message)
+                event: AbstractEvent = self._parse_webcast_message(message)
                 self.emit(event.name, event)
             except Exception as ex:
                 await self._on_error(ex, FailedParseMessage("Failed parsing of a webcast message"))
 
-    def __parse_webcast_message(self, webcast_message: dict) -> Optional[AbstractEvent]:
+    def _parse_webcast_message(self, webcast_message: dict) -> Optional[AbstractEvent]:
         """
         Parse a webcast message into an event and return to the caller
 
         :param webcast_message: The message to parse
         :return: The parsed object of base-type AbstractEvent
 
         """
@@ -160,22 +162,22 @@
         mapping: Optional[AbstractEvent] = (
             {
                 "WebcastGiftMessage": GiftEvent,
                 "WebcastChatMessage": CommentEvent,
                 "WebcastRoomUserSeqMessage": ViewerUpdateEvent,
                 "WebcastMemberMessage": JoinEvent,
                 "WebcastLikeMessage": LikeEvent,
-                "WebcastRankUpdateMessage": WeeklyRankingEvent,
-                "WebcastHourlyRankMessage": WeeklyRankingEvent,
+                "WebcastRankUpdateMessage": RankingUpdateEvent,
+                "WebcastHourlyRankMessage": RankingUpdateEvent,
                 "WebcastQuestionNewMessage": QuestionEvent,
                 "WebcastLiveIntroMessage": IntroMessageEvent,
                 "WebcastEmoteChatMessage": EmoteEvent,
                 "WebcastLinkMicBattle": MicBattleStartEvent,
-                "WebcastLinkMicArmies": MicBattleUpdateEvent
-
+                "WebcastLinkMicArmies": MicBattleUpdateEvent,
+                "WebcastRankTextMessage": UserRankingUpdateEvent
             }.get(webcast_message.get('type'))
         )
 
         # Sometimes, we need to use the display_type attribute
         mapping: Optional[AbstractEvent] = mapping or (
             {
                 "pm_main_follow_message_viewer_2": FollowEvent,
```

### Comparing `TikTokLive-5.0.7/TikTokLive/client/config.py` & `TikTokLive-5.0.8/TikTokLive/client/config.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-5.0.7/TikTokLive/client/httpx.py` & `TikTokLive-5.0.8/TikTokLive/client/httpx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json as json_parse
 import urllib.parse
 from asyncio import AbstractEventLoop
 from http.cookies import SimpleCookie
+from ssl import SSLContext
 from typing import Dict, Optional
 
 import httpx
 from httpx import Cookies
 
 from TikTokLive.client import config
 from TikTokLive.proto.utilities import deserialize_message
@@ -25,35 +26,40 @@
             self,
             loop: AbstractEventLoop,
             headers: Optional[Dict[str, str]] = None,
             timeout: Optional[float] = None,
             proxies: Optional[Dict[str, str]] = None,
             trust_env: bool = True,
             params: Optional[Dict[str, str]] = dict(),
-            sign_api_key: Optional[str] = None
+            sign_api_key: Optional[str] = None,
+            ssl_context: Optional[SSLContext] = None
     ):
         """
         Initialize HTTP client for TikTok-related requests
 
+        :param loop: Asyncio event loop
         :param headers: Headers to use to make HTTP requests
         :param timeout: Timeout for HTTP requests
         :param proxies: Enable proxied requests by turning on forwarding for the HTTPX "proxies" argument
         :param trust_env: Whether to trust the environment when it comes to proxy usage
+        :param params: Client parameters to use in requests
         :param sign_api_key: API key to increase rate limits on the sign server API for bulk usage of the library
+        :param ssl_context: Add SSL context option, else True
 
         """
 
         self.loop: AbstractEventLoop = loop
         self.timeout: float = timeout or 10.0
         self.proxies: Optional[Dict[str, str]] = proxies
         self.headers: Dict[str, str] = {**config.DEFAULT_REQUEST_HEADERS, **(headers if isinstance(headers, dict) else dict())}
         self.params: dict = params if params else dict()
         self.sign_api_key: str = sign_api_key or ""
         self.trust_env: bool = trust_env
-        self.cookies = Cookies()
+        self.cookies: Cookies = Cookies()
+        self.ssl_context: Optional[SSLContext] = ssl_context if isinstance(ssl_context, SSLContext) else True
         TikTokHTTPClient._uuc += 1
 
     def __del__(self):
         """
         Internal utility method
         
         """
@@ -84,15 +90,15 @@
         :param params:  Parameters to include in the URL
         :return: The result of the request (a bytearray)
         :raises: httpx.TimeoutException
         """
 
         url: str = self.update_url(url, params or dict())
 
-        async with httpx.AsyncClient(trust_env=self.trust_env, proxies=self.proxies, cookies=self.cookies) as client:
+        async with httpx.AsyncClient(trust_env=self.trust_env, proxies=self.proxies, cookies=self.cookies, verify=self.ssl_context) as client:
             response: httpx.Response = await client.get(url, headers=self.headers, timeout=self.timeout)
 
         # If requesting the sign api
         if sign_api:
             # Rate Limit
             if response.status_code == 429:
                 raise SignatureRateLimitReached(
@@ -150,15 +156,15 @@
         :return: JSON Result
         :raises: httpx.TimeoutException
 
         """
 
         url: str = self.update_url(url, params or dict())
 
-        async with httpx.AsyncClient(trust_env=self.trust_env, proxies=self.proxies, cookies=self.cookies) as client:
+        async with httpx.AsyncClient(trust_env=self.trust_env, proxies=self.proxies, cookies=self.cookies, verify=self.ssl_context) as client:
             response: httpx.Response = await client.post(
                 url=url,
                 data=json,
                 headers=self.headers,
                 timeout=self.timeout
             )
 
@@ -258,15 +264,15 @@
         :param headers: Custom Headers
         :param json: JSON Payload as Dict
         :return: JSON Result
         :raises: httpx.TimeoutException
 
         """
 
-        async with httpx.AsyncClient(trust_env=self.trust_env, proxies=self.proxies, cookies=self.cookies) as client:
+        async with httpx.AsyncClient(trust_env=self.trust_env, proxies=self.proxies, cookies=self.cookies, verify=self.ssl_context) as client:
             response: httpx.Response = await client.post(
                 url=url,
                 data=json,
                 headers=headers,
                 timeout=self.timeout
             )
```

### Comparing `TikTokLive-5.0.7/TikTokLive/client/wsclient.py` & `TikTokLive-5.0.8/TikTokLive/client/wsclient.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-5.0.7/TikTokLive/proto/utilities.py` & `TikTokLive-5.0.8/TikTokLive/proto/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
                 "WebcastInRoomBannerMessage",
                 "SystemMessage",
                 "WebcastEmoteChatMessage",
                 "WebcastEnvelopeMessage",
                 "WebcastLiveIntroMessage",
                 "RoomMessage",
                 "WebcastRankUpdateMessage",
-                "WebcastHourlyRankMessage"
+                "WebcastHourlyRankMessage",
+                "WebcastRankTextMessage"
             ]:
                 continue
 
             _type = message.get("type")
             _schema = getattr(tiktok_schema, _type)()
             _schema.ParseFromString(message.get("binary"))
             _dict_data = protobuf_to_dict(_schema)
```

### Comparing `TikTokLive-5.0.7/TikTokLive/types/errors.py` & `TikTokLive-5.0.8/TikTokLive/types/errors.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-5.0.7/TikTokLive/types/events.py` & `TikTokLive-5.0.8/TikTokLive/types/events.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,561 +1,610 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from TikTokLive import TikTokLiveClient
-
-import base64
-from dataclasses import field
-from typing import Optional, List, Any, Dict, ClassVar
-
-from mashumaro import DataClassDictMixin, pass_through
-
-from TikTokLive.types import User, Gift, Emote, TreasureBoxData, ExtraRankData, LinkUser, BattleArmy, TopViewer, ChatImage
-from TikTokLive.types.utilities import LiveEvent, alias
-
-
-class AbstractEvent(DataClassDictMixin):
-    """
-    Abstract TikTok Live event from which to build on
-
-    """
-
-    name: ClassVar[str] = "event"
-    """The name of the TikTokLive event"""
-
-    def __init__(self):
-        """
-        Never run, this method is for type hinting the raw_data attribute
-
-        """
-
-        self.raw_data: Optional[dict] = dict()
-        """Raw event data as a dictionary in-case the dataclasses miss something"""
-
-    def _forward_client(self, client: TikTokLiveClient):
-        """
-        Forward the client to events where it is required
-
-        """
-
-        if hasattr(self, "user") and isinstance(self.user, User):
-            self.user.avatar._client = client
-            for badge in self.user.badges:
-                if badge.image:
-                    badge.image._client = client
-
-
-@LiveEvent("connect")
-class ConnectEvent(AbstractEvent):
-    """
-    Event that fires when the client connect to a livestream
-    
-    """
-
-
-@LiveEvent("disconnect")
-class DisconnectEvent(AbstractEvent):
-    """
-    Event that fires when the client disconnects from a livestream
-    
-    """
-
-
-@LiveEvent("like")
-class LikeEvent(AbstractEvent):
-    """
-    Event that fires when a user likes the livestream
-    
-    """
-
-    user: Optional[User] = None
-    """The user that liked the stream"""
-
-    likes: Optional[int] = None
-    """The number of likes sent in the payload (Max: 15)"""
-
-    total_likes: Optional[int] = None
-    """Total number of likes sent"""
-
-    display_type: Optional[str] = None
-    """Internal display type"""
-
-    label: Optional[str] = None
-    """Internal TikTok label"""
-
-
-@LiveEvent("join")
-class JoinEvent(AbstractEvent):
-    """
-    Event that fires when a user joins the livestream
-    
-    """
-
-    user: Optional[User] = None
-    """The user that joined the stream"""
-
-    display_type: Optional[str] = None
-    """The type of event"""
-
-    label: Optional[str] = None
-    """Label for event in live chat"""
-
-    total_viewers: Optional[int] = None
-    """Total number of viewers in the stream"""
-
-    action_id: Optional[int] = None
-    """Internal action ID from TikTok"""
-
-    @property
-    def through_share(self) -> bool:
-        """
-        Whether they joined through a link vs. the TikTok App
-
-        :return: Returns True if they joined through a share link
-
-        """
-        return self.display_type == "pm_mt_join_message_other_viewer"
-
-
-@LiveEvent("follow")
-class FollowEvent(AbstractEvent):
-    """
-    Event that fires when a user follows the livestream
-    
-    """
-
-    user: Optional[User] = None
-    """The user that followed the streamer"""
-
-    display_type: Optional[str] = None
-    """Internal TikTok display type"""
-
-    label: Optional[str] = None
-    """Internal TikTok label"""
-
-    total_followers: Optional[int] = None
-    """Total number of creator followers"""
-
-
-@LiveEvent("share")
-class ShareEvent(AbstractEvent):
-    """
-    Event that fires when a user shares the livestream
-
-    """
-
-    user: Optional[User] = None
-    """The user that shared the stream"""
-
-    display_type: Optional[str] = None
-    """Internal TikTok display type"""
-
-    label: Optional[str] = None
-    """Internal TikTok label"""
-
-
-@LiveEvent("more_share")
-class MoreShareEvent(ShareEvent):
-    """
-    Event that fires when a user shared the livestream to more than 5/10 users
-    e.g. "user123 has shared to more than 10 people!"
-
-    """
-
-    @property
-    def amount(self) -> Optional[int]:
-        """
-        The number of people that have joined the stream off the user
-
-        :return: The number of people that have joined
-
-        """
-
-        try:
-            return int(self.display_type.split("pm_mt_guidance_viewer_")[1].split("_share")[0])
-        except IndexError:
-            return None
-
-
-@LiveEvent("viewer_update")
-class ViewerUpdateEvent(AbstractEvent):
-    """
-    Event that fires when the viewer count & top viewers for the livestream updates
-    
-    """
-
-    viewer_count: Optional[int] = None
-    """The number of people viewing the stream currently"""
-
-    top_viewers: List[TopViewer] = field(default_factory=list)
-    """Top 10-20 viewers in the livestream by coins given"""
-
-
-@LiveEvent("comment")
-class CommentEvent(AbstractEvent):
-    """
-    Event that fires when someone comments on the livestream
-    
-    """
-
-    user: Optional[User] = None
-    """The user that sent the comment"""
-
-    comment: Optional[str] = None
-    """The UTF-8 text comment that was sent"""
-
-    mentions: List[User] = field(default_factory=list)
-    """List of people the comment mentions"""
-
-    images: List[ChatImage] = field(default_factory=list)
-    """List of chat images sent in a comment"""
-
-    language: Optional[str] = None
-    """Language the commenter uses"""
-
-
-@LiveEvent("live_end")
-class LiveEndEvent(AbstractEvent):
-    """
-    Event that fires when the livestream ends
-    
-    """
-
-
-@LiveEvent("gift")
-class GiftEvent(AbstractEvent):
-    """
-    Event that fires when a gift is received
-    
-    """
-
-    user: Optional[User] = None
-    """The user that sent the gift"""
-
-    gift: Optional[Gift] = None
-    """Object containing gift data"""
-
-    @classmethod
-    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
-        """
-        De-flatten the gift event (too much in the primary payload)
-
-        """
-
-        d["gift"] = d  # Move 'er up a bit
-        return d
-    
-    def _forward_client(self, client: TikTokLiveClient):
-        """
-        Forward the client to events where it is required
-
-        """
-
-        super()._forward_client(client)
-
-        if hasattr(self, "gift") and isinstance(self.gift, Gift):
-            if self.gift.info:
-                self.gift.info.image._client = client
-            if self.gift.detailed:
-                self.gift.detailed.icon._client = client
-
-
-@LiveEvent("question")
-class QuestionEvent(AbstractEvent):
-    """
-    Event that fires when someone asks a Q&A question
-    
-    """
-
-    @classmethod
-    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
-        """
-        Flatten the question event a bit
-
-        """
-
-        d = d.get("questionDetails")  # Get rid of empty container
-        return d
-
-    question: Optional[str] = None
-    """The question that was asked"""
-
-    user: Optional[User] = None
-    """User who asked the question"""
-
-
-@LiveEvent("emote")
-class EmoteEvent(AbstractEvent):
-    """
-    Event that fires when someone sends a subscriber emote
-    
-    """
-
-    def _forward_client(self, client: TikTokLiveClient):
-        """
-        Forward the client to events where it is required
-
-        """
-
-        super()._forward_client(client)
-
-        if hasattr(self, "emote") and isinstance(self.emote, Emote):
-            self.emote.image._client = client
-
-    user: Optional[User] = None
-    """Person who sent the emote message"""
-
-    emote: Optional[Emote] = None
-    """The emote the person sent"""
-
-
-@LiveEvent("envelope")
-class EnvelopeEvent(AbstractEvent):
-    """
-    Event that fire when someone sends an envelope (treasure box)
-    
-    """
-
-    @classmethod
-    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
-        """
-        Get rid of an obscene amount of nesting in the envelope event
-
-        """
-
-        # holy crap
-        user_3: List[dict] = d.get("treasureBoxUser", dict()).get("user2", dict()).get("user3", list())
-        d["treasureBoxUser"] = (user_3[0].get('user4', dict()).get('user', None)) if len(user_3) > 0 else None
-        return d
-
-    treasure_box_data: Optional[TreasureBoxData] = alias('treasureBoxData')
-    """Data about the enclosed Treasure Box in the envelope"""
-
-    treasure_box_user: Optional[User] = alias('treasureBoxUser')
-    """Data about the user that sent the treasure box"""
-
-
-@LiveEvent("weekly_ranking")
-class WeeklyRankingEvent(AbstractEvent):
-    """
-    Event that fires when the weekly rankings are updated
-
-    """
-
-    @classmethod
-    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
-        """
-        Pre-process weekly ranking event
-
-        """
-
-        ranks: Dict[str, Any] = d.get('data', dict()).get('rankings', dict())  # Do a little flattening
-
-        # Try to flatten rank data & convert to int
-        try:
-            ranks['rank'] = int(ranks.get('data', dict()).get('rank', None))
-        except:
-            pass
-
-        return ranks
-
-    type: Optional[str] = None
-    """Unknown"""
-
-    label: Optional[str] = None
-    """Internal TikTok Label"""
-
-    extra: Optional[ExtraRankData] = field(default_factory=ExtraRankData)
-    """Extra data relating to the UI, presumably"""
-
-    rank: Optional[int] = None
-    """The number for the user's TikTok ranking. If the rank is "None", the user is not in the top 99."""
-
-    @property
-    def top_99(self) -> bool:
-        """
-        Whether the user is in the top 99 of creators
-        """
-
-        return self.rank is not None
-
-
-@LiveEvent("intro_message")
-class IntroMessageEvent(AbstractEvent):
-    """
-    Event fires giving the current stream description when the stream is joined
-    Note: Only fires if "process_initial_data" is enabled and the streamer has an intro message configured
-
-    """
-
-    room_id: Optional[int] = None
-    """Room ID of the room we are in"""
-
-    message: Optional[str] = None
-    """The pinned intro message in the livestream"""
-
-    streamer: Optional[User] = None
-    """User payload of information about the streamer"""
-
-    language: Optional[str] = None
-    """Language of the creator's room"""
-
-
-@LiveEvent("mic_battle_start")
-class MicBattleStartEvent(AbstractEvent):
-    """
-    Event that fires when a Mic Battle starts
-
-    """
-
-    def _forward_client(self, client: TikTokLiveClient):
-        """
-        Forward the client to events where it is required
-
-        """
-
-        if hasattr(self, "battle_users") and isinstance(self.battle_users, list):
-            for user in self.battle_users:
-                if isinstance(user, LinkUser):
-                    user.avatar._client = client
-
-    @classmethod
-    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
-        """
-        Re-structure messy TikTok structuring for battles
-
-        """
-
-        # Flatten the nested TikTok structures into just a list of LinkUsers
-        battle_users: List[LinkUser] = []
-        for user_data in d.get('battleUsers', list()):
-            try:
-                battle_users.append(user_data["battleGroup"]["user"])
-            except KeyError:
-                continue
-
-        return {'battle_users': battle_users}
-
-    battle_users: List[LinkUser] = field(default_factory=list)
-    """Information about the users engaged in the Mic Battle"""
-
-
-@LiveEvent("mic_battle_update")
-class MicBattleUpdateEvent(AbstractEvent):
-    """
-    Triggered every time a battle participant receives points.
-    Contains the current status of the battle and the army that supported the group.
-
-    """
-
-    def _forward_client(self, client: TikTokLiveClient):
-        """
-        Forward the client to events where it is required
-
-        """
-
-        if hasattr(self, "battle_armies") and isinstance(self.battle_armies, list):
-            for army in self.battle_armies:
-                for user in army.participants:
-                    if isinstance(user, User):
-                        user.avatar._client = client
-
-    @classmethod
-    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
-        """
-        This event needs to be entirely custom-handled because it's a mess on TikTok's end
-
-        """
-
-        event_data: dict = {'battle_status': d.get('battleStatus')}
-        battle_armies: list = []
-
-        for battle_item in d.get('battleItems', list()):
-            for battle_group in battle_item.get('battleGroups', list()):
-                battle_armies.append({
-                    'host_user_id': battle_item.get('hostUserId'),
-                    'points': battle_group.get('points') or None,
-                    'participants': battle_group.get('users') or list()
-                })
-
-        event_data['battle_armies'] = battle_armies
-        return event_data
-
-    battle_status: Optional[int] = None
-    """The status of the current Battle. If battle_status=1, the battle is ongoing. If it's 2, the battle has ended."""
-
-    battle_armies: List[BattleArmy] = field(default_factory=list)
-    """Information about the users engaged in the Mic Battle"""
-
-    @property
-    def in_battle(self) -> bool:
-        """
-        Whether the users are currently in battle
-
-        """
-
-        return self.battle_status == 1
-
-    @property
-    def battle_finished(self) -> bool:
-        """
-        Whether the battle is currently finished
-
-        """
-
-        return self.battle_status == 2
-
-
-@LiveEvent("unknown")
-class UnknownEvent(AbstractEvent):
-    """
-    Event that fires when an event is received that is missing a handler
-
-    """
-
-    @classmethod
-    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
-        """
-        Give *some* structure for unknown events. We're not savages, here.
-
-        """
-
-        # Shallow copy of the data
-        copy: Dict[Any, Any] = d.copy()
-
-        # Remove from the original (will be in the new payload)
-        for key in ["type", "binary"]:
-            try:
-                del d[key]
-            except KeyError:
-                pass
-
-        # Build the new format
-        return (
-            {
-                "type": copy.get("type"),
-                "binary": copy.get("binary"),
-                "data": d or None
-            }
-        )
-
-    type: Optional[str] = None
-    """The type of message. This is the message's "official" name provided by TikTok"""
-
-    binary: Optional[bytes] = field(metadata={"serialization_strategy": pass_through}, default=None)
-    """Binary of the message if provided. This is useful if there is NO protobuf definition yet"""
-
-    data: Optional[Dict[Any, Any]] = None
-    """Data contained within the event. This is useful if the protobuf has been decoded but an event object has not been made."""
-
-    @property
-    def base64(self) -> Optional[bytes]:
-        """
-        Base64 version of message binary *if* binary is provided
-
-        Can be loaded into a decoder such as https://protobuf-decoder.netlify.app/.
-
-        """
-
-        return base64.b64encode(self.binary) if self.binary else None
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from TikTokLive import TikTokLiveClient
+
+import base64
+from dataclasses import field
+from typing import Optional, List, Any, Dict, ClassVar
+
+from mashumaro import DataClassDictMixin, pass_through
+
+from TikTokLive.types import User, Gift, Emote, TreasureBoxData, ExtraRankData, LinkUser, BattleArmy, TopViewer, \
+    ChatImage, ValueLabel
+from TikTokLive.types.utilities import LiveEvent, alias
+
+
+class AbstractEvent(DataClassDictMixin):
+    """
+    Abstract TikTok Live event from which to build on
+
+    """
+
+    name: ClassVar[str] = "event"
+    """The name of the TikTokLive event"""
+
+    def __init__(self):
+        """
+        Never run, this method is for type hinting the raw_data attribute
+
+        """
+
+        self.raw_data: Optional[dict] = dict()
+        """Raw event data as a dictionary in-case the dataclasses miss something"""
+
+    def _forward_client(self, client: TikTokLiveClient):
+        """
+        Forward the client to events where it is required
+
+        """
+
+        if hasattr(self, "user") and isinstance(self.user, User):
+            self.user.avatar._client = client
+            for badge in self.user.badges:
+                if badge.image:
+                    badge.image._client = client
+
+
+@LiveEvent("connect")
+class ConnectEvent(AbstractEvent):
+    """
+    Event that fires when the client connect to a livestream
+    
+    """
+
+
+@LiveEvent("disconnect")
+class DisconnectEvent(AbstractEvent):
+    """
+    Event that fires when the client disconnects from a livestream
+    
+    """
+
+
+@LiveEvent("like")
+class LikeEvent(AbstractEvent):
+    """
+    Event that fires when a user likes the livestream
+    
+    """
+
+    user: Optional[User] = None
+    """The user that liked the stream"""
+
+    likes: Optional[int] = None
+    """The number of likes sent in the payload (Max: 15)"""
+
+    total_likes: Optional[int] = None
+    """Total number of likes sent"""
+
+    display_type: Optional[str] = None
+    """Internal display type"""
+
+    label: Optional[str] = None
+    """Internal TikTok label"""
+
+
+@LiveEvent("join")
+class JoinEvent(AbstractEvent):
+    """
+    Event that fires when a user joins the livestream
+    
+    """
+
+    user: Optional[User] = None
+    """The user that joined the stream"""
+
+    display_type: Optional[str] = None
+    """The type of event"""
+
+    label: Optional[str] = None
+    """Label for event in live chat"""
+
+    total_viewers: Optional[int] = None
+    """Total number of viewers in the stream"""
+
+    action_id: Optional[int] = None
+    """Internal action ID from TikTok"""
+
+    @property
+    def through_share(self) -> bool:
+        """
+        Whether they joined through a link vs. the TikTok App
+
+        :return: Returns True if they joined through a share link
+
+        """
+        return self.display_type == "pm_mt_join_message_other_viewer"
+
+
+@LiveEvent("follow")
+class FollowEvent(AbstractEvent):
+    """
+    Event that fires when a user follows the livestream
+    
+    """
+
+    user: Optional[User] = None
+    """The user that followed the streamer"""
+
+    display_type: Optional[str] = None
+    """Internal TikTok display type"""
+
+    label: Optional[str] = None
+    """Internal TikTok label"""
+
+    total_followers: Optional[int] = None
+    """Total number of creator followers"""
+
+
+@LiveEvent("share")
+class ShareEvent(AbstractEvent):
+    """
+    Event that fires when a user shares the livestream
+
+    """
+
+    user: Optional[User] = None
+    """The user that shared the stream"""
+
+    display_type: Optional[str] = None
+    """Internal TikTok display type"""
+
+    label: Optional[str] = None
+    """Internal TikTok label"""
+
+
+@LiveEvent("more_share")
+class MoreShareEvent(ShareEvent):
+    """
+    Event that fires when a user shared the livestream to more than 5/10 users
+    e.g. "user123 has shared to more than 10 people!"
+
+    """
+
+    @property
+    def amount(self) -> Optional[int]:
+        """
+        The number of people that have joined the stream off the user
+
+        :return: The number of people that have joined
+
+        """
+
+        try:
+            return int(self.display_type.split("pm_mt_guidance_viewer_")[1].split("_share")[0])
+        except IndexError:
+            return None
+
+
+@LiveEvent("viewer_update")
+class ViewerUpdateEvent(AbstractEvent):
+    """
+    Event that fires when the viewer count & top viewers for the livestream updates
+    
+    """
+
+    viewer_count: Optional[int] = None
+    """The number of people viewing the stream currently"""
+
+    top_viewers: List[TopViewer] = field(default_factory=list)
+    """Top 10-20 viewers in the livestream by coins given"""
+
+
+@LiveEvent("comment")
+class CommentEvent(AbstractEvent):
+    """
+    Event that fires when someone comments on the livestream
+    
+    """
+
+    user: Optional[User] = None
+    """The user that sent the comment"""
+
+    comment: Optional[str] = None
+    """The UTF-8 text comment that was sent"""
+
+    mentions: List[User] = field(default_factory=list)
+    """List of people the comment mentions"""
+
+    images: List[ChatImage] = field(default_factory=list)
+    """List of chat images sent in a comment"""
+
+    language: Optional[str] = None
+    """Language the commenter uses"""
+
+
+@LiveEvent("live_end")
+class LiveEndEvent(AbstractEvent):
+    """
+    Event that fires when the livestream ends
+    
+    """
+
+
+@LiveEvent("gift")
+class GiftEvent(AbstractEvent):
+    """
+    Event that fires when a gift is received
+    
+    """
+
+    user: Optional[User] = None
+    """The user that sent the gift"""
+
+    gift: Optional[Gift] = None
+    """Object containing gift data"""
+
+    @classmethod
+    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
+        """
+        De-flatten the gift event (too much in the primary payload)
+
+        """
+
+        d["gift"] = d  # Move 'er up a bit
+        return d
+    
+    def _forward_client(self, client: TikTokLiveClient):
+        """
+        Forward the client to events where it is required
+
+        """
+
+        super()._forward_client(client)
+
+        if hasattr(self, "gift") and isinstance(self.gift, Gift):
+            if self.gift.info:
+                self.gift.info.image._client = client
+            if self.gift.detailed:
+                self.gift.detailed.icon._client = client
+
+
+@LiveEvent("question")
+class QuestionEvent(AbstractEvent):
+    """
+    Event that fires when someone asks a Q&A question
+    
+    """
+
+    @classmethod
+    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
+        """
+        Flatten the question event a bit
+
+        """
+
+        d = d.get("questionDetails")  # Get rid of empty container
+        return d
+
+    question: Optional[str] = None
+    """The question that was asked"""
+
+    user: Optional[User] = None
+    """User who asked the question"""
+
+
+@LiveEvent("emote")
+class EmoteEvent(AbstractEvent):
+    """
+    Event that fires when someone sends a subscriber emote
+    
+    """
+
+    def _forward_client(self, client: TikTokLiveClient):
+        """
+        Forward the client to events where it is required
+
+        """
+
+        super()._forward_client(client)
+
+        if hasattr(self, "emote") and isinstance(self.emote, Emote):
+            self.emote.image._client = client
+
+    user: Optional[User] = None
+    """Person who sent the emote message"""
+
+    emote: Optional[Emote] = None
+    """The emote the person sent"""
+
+
+@LiveEvent("envelope")
+class EnvelopeEvent(AbstractEvent):
+    """
+    Event that fire when someone sends an envelope (treasure box)
+    
+    """
+
+    @classmethod
+    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
+        """
+        Get rid of an obscene amount of nesting in the envelope event
+
+        """
+
+        # holy crap
+        user_3: List[dict] = d.get("treasureBoxUser", dict()).get("user2", dict()).get("user3", list())
+        d["treasureBoxUser"] = (user_3[0].get('user4', dict()).get('user', None)) if len(user_3) > 0 else None
+        return d
+
+    treasure_box_data: Optional[TreasureBoxData] = alias('treasureBoxData')
+    """Data about the enclosed Treasure Box in the envelope"""
+
+    treasure_box_user: Optional[User] = alias('treasureBoxUser')
+    """Data about the user that sent the treasure box"""
+
+
+@LiveEvent("user_ranking_update")
+class UserRankingUpdateEvent(AbstractEvent):
+    """
+    Event publishing that a user ranked up in some way
+    e.g. "{0:user} just became a top {1:string} viewer!"
+
+    """
+
+    @classmethod
+    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
+        """
+        Pre-process weekly ranking event
+
+        """
+
+        data: dict = d.get('details', dict())
+        details: List[dict] = data.get('details', list())
+
+        # Delete Duplicate Entry
+        try:
+            del data['details']
+        except KeyError:
+            pass
+
+        # Bring out user object
+        for detail in details:
+
+            # data1 = 11
+            if detail.get('user', dict()).get('user'):
+                data['user'] = detail['user']['user']
+
+            # data1 = 1
+            if detail.get('data1') == 1:
+                data['rank'] = detail.get('category')
+
+        return data
+
+    type: Optional[str] = None
+    """The type of update"""
+
+    label: Optional[str] = None
+    """Update message text label"""
+
+    user: Optional[User] = None
+    """User who is ranking up"""
+
+    rank: Optional[int] = None
+    """The rank of the user"""
+
+
+@LiveEvent("ranking_update")
+class RankingUpdateEvent(AbstractEvent):
+    """
+    Event firing containing updates to rank information. So far, this has been noted to include:
+    - Weekly Ranking
+    - Rising Stars
+    """
+
+    @classmethod
+    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
+        """
+        Pre-process weekly ranking event
+
+        """
+
+        rank: Dict[str, Any] = d.get('data', dict()).get('data', dict())  # Flatten
+
+        # Try to flatten rank data & convert to int to
+        try:
+            details: Optional[List] = rank.get('details', list())
+            if len(details) > 0:
+                rank['rank'] = int(details[0].get('value', None))
+        except:
+            pass
+
+        return rank
+
+    type: Optional[str] = None
+    """The type of rank update (e.g. Rising stars, etc.)"""
+
+    label: Optional[str] = None
+    """Internal TikTok Label"""
+
+    details: List[ValueLabel] = field(default_factory=list)
+    """The user's ranking details. This can be more than just weekly ranking!"""
+
+    extra: Optional[ExtraRankData] = field(default_factory=ExtraRankData)
+    """Extra data relating to the UI, presumably"""
+
+    rank: Optional[int] = None
+    """The number for the user's TikTok ranking. """
+
+
+@LiveEvent("intro_message")
+class IntroMessageEvent(AbstractEvent):
+    """
+    Event fires giving the current stream description when the stream is joined
+    Note: Only fires if "process_initial_data" is enabled and the streamer has an intro message configured
+
+    """
+
+    room_id: Optional[int] = None
+    """Room ID of the room we are in"""
+
+    message: Optional[str] = None
+    """The pinned intro message in the livestream"""
+
+    streamer: Optional[User] = None
+    """User payload of information about the streamer"""
+
+    language: Optional[str] = None
+    """Language of the creator's room"""
+
+
+@LiveEvent("mic_battle_start")
+class MicBattleStartEvent(AbstractEvent):
+    """
+    Event that fires when a Mic Battle starts
+
+    """
+
+    def _forward_client(self, client: TikTokLiveClient):
+        """
+        Forward the client to events where it is required
+
+        """
+
+        if hasattr(self, "battle_users") and isinstance(self.battle_users, list):
+            for user in self.battle_users:
+                if isinstance(user, LinkUser):
+                    user.avatar._client = client
+
+    @classmethod
+    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
+        """
+        Re-structure messy TikTok structuring for battles
+
+        """
+
+        # Flatten the nested TikTok structures into just a list of LinkUsers
+        battle_users: List[LinkUser] = []
+        for user_data in d.get('battleUsers', list()):
+            try:
+                battle_users.append(user_data["battleGroup"]["user"])
+            except KeyError:
+                continue
+
+        return {'battle_users': battle_users}
+
+    battle_users: List[LinkUser] = field(default_factory=list)
+    """Information about the users engaged in the Mic Battle"""
+
+
+@LiveEvent("mic_battle_update")
+class MicBattleUpdateEvent(AbstractEvent):
+    """
+    Triggered every time a battle participant receives points.
+    Contains the current status of the battle and the army that supported the group.
+
+    """
+
+    def _forward_client(self, client: TikTokLiveClient):
+        """
+        Forward the client to events where it is required
+
+        """
+
+        if hasattr(self, "battle_armies") and isinstance(self.battle_armies, list):
+            for army in self.battle_armies:
+                for user in army.participants:
+                    if isinstance(user, User):
+                        user.avatar._client = client
+
+    @classmethod
+    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
+        """
+        This event needs to be entirely custom-handled because it's a mess on TikTok's end
+
+        """
+
+        event_data: dict = {'battle_status': d.get('battleStatus')}
+        battle_armies: list = []
+
+        for battle_item in d.get('battleItems', list()):
+            for battle_group in battle_item.get('battleGroups', list()):
+                battle_armies.append({
+                    'host_user_id': battle_item.get('hostUserId'),
+                    'points': battle_group.get('points') or None,
+                    'participants': battle_group.get('users') or list()
+                })
+
+        event_data['battle_armies'] = battle_armies
+        return event_data
+
+    battle_status: Optional[int] = None
+    """The status of the current Battle. If battle_status=1, the battle is ongoing. If it's 2, the battle has ended."""
+
+    battle_armies: List[BattleArmy] = field(default_factory=list)
+    """Information about the users engaged in the Mic Battle"""
+
+    @property
+    def in_battle(self) -> bool:
+        """
+        Whether the users are currently in battle
+
+        """
+
+        return self.battle_status == 1
+
+    @property
+    def battle_finished(self) -> bool:
+        """
+        Whether the battle is currently finished
+
+        """
+
+        return self.battle_status == 2
+
+
+@LiveEvent("unknown")
+class UnknownEvent(AbstractEvent):
+    """
+    Event that fires when an event is received that is missing a handler
+
+    """
+
+    @classmethod
+    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
+        """
+        Give *some* structure for unknown events. We're not savages, here.
+
+        """
+
+        # Shallow copy of the data
+        copy: Dict[Any, Any] = d.copy()
+
+        # Remove from the original (will be in the new payload)
+        for key in ["type", "binary"]:
+            try:
+                del d[key]
+            except KeyError:
+                pass
+
+        # Build the new format
+        return (
+            {
+                "type": copy.get("type"),
+                "binary": copy.get("binary"),
+                "data": d or None
+            }
+        )
+
+    type: Optional[str] = None
+    """The type of message. This is the message's "official" name provided by TikTok"""
+
+    binary: Optional[bytes] = field(metadata={"serialization_strategy": pass_through}, default=None)
+    """Binary of the message if provided. This is useful if there is NO protobuf definition yet"""
+
+    data: Optional[Dict[Any, Any]] = None
+    """Data contained within the event. This is useful if the protobuf has been decoded but an event object has not been made."""
+
+    @property
+    def base64(self) -> Optional[bytes]:
+        """
+        Base64 version of message binary *if* binary is provided
+
+        Can be loaded into a decoder such as https://protobuf-decoder.netlify.app/.
+
+        """
+
+        return base64.b64encode(self.binary) if self.binary else None
```

### Comparing `TikTokLive-5.0.7/TikTokLive/types/objects.py` & `TikTokLive-5.0.8/TikTokLive/types/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,29 +158,35 @@
         :return: Search status
 
         """
 
         return any(badge_type == badge.badge_scene_type for badge in self.badges)
 
     @property
-    def is_following(self) -> bool:
+    def is_following(self) -> Optional[bool]:
         """
         Whether they are following the watched streamer
 
         """
 
+        if self.info.follow_role is None:
+            return None
+
         return (self.info.follow_role or 0) >= 1
 
     @property
-    def is_friend(self) -> bool:
+    def is_friend(self) -> Optional[bool]:
         """
         Whether they are a friend of the watched streamer
 
         """
 
+        if self.info.follow_role is None:
+            return None
+
         return (self.info.follow_role or 0) >= 2
 
     @property
     def is_new_gifter(self) -> bool:
         """
         Whether they are a new gifter in the streamer's stream
 
@@ -389,15 +395,15 @@
 
     id: Optional[int] = None
     """The Internal TikTok ID of the gift"""
 
     count: Optional[int] = alias("repeatCount", default=None)
     """Number of times the gift has repeated"""
 
-    is_repeating: Optional[int] = alias("repeatEnd", default=0)
+    repeat_end: Optional[int] = alias("repeatEnd", default=0)
     """Whether or not the repetition is over"""
 
     info: Optional[GiftInfo] = field(default_factory=GiftInfo)
     """Details about the specific Gift sent"""
 
     recipient: Optional[GiftRecipient] = field(default_factory=GiftRecipient)
     """Who received the gift (for streams with multiple users)"""
@@ -420,15 +426,15 @@
         """
         Whether the streak is over
         
         :return: True if currently streaking, False if not
 
         """
 
-        return bool(self.is_repeating)
+        return not bool(self.repeat_end)
 
 
 @dataclass()
 class EmoteImage(AbstractObject):
     """
     Container encapsulating the image URL for the Emote
 
@@ -561,14 +567,27 @@
     """The number of points the battle army has"""
 
     participants: List[User] = field(default_factory=list)
     """The users involved in the specific battle army"""
 
 
 @dataclass()
+class ValueLabel(AbstractObject):
+    """
+    Label containing a value
+
+    """
+
+    value: Optional[str] = None
+    data: Optional[int] = None
+    label: Optional[str] = None
+    label2: Optional[str] = None
+
+
+@dataclass()
 class FFmpegWrapper:
     """
     A wrapper for the FFmpeg Stream Download utility in the TikTokLive Package
 
     """
 
     runtime: Optional[str]
```

### Comparing `TikTokLive-5.0.7/TikTokLive/types/utilities.py` & `TikTokLive-5.0.8/TikTokLive/types/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-5.0.7/TikTokLive/utilities.py` & `TikTokLive-5.0.8/TikTokLive/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-5.0.7/TikTokLive.egg-info/PKG-INFO` & `TikTokLive-5.0.8/TikTokLive.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: TikTokLive
-Version: 5.0.7
+Version: 5.0.8
 Summary: TikTok Live Connection Client
 Home-page: https://github.com/isaackogan/TikTokLive
+Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v5.0.8
 Author: Isaac Kogan
 Author-email: info@isaackogan.com
 License: MIT
-Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v5.0.7
 Keywords: tiktok,tiktok live,python3,api,unofficial
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,14 +43,22 @@
 by [@zerodytrash](https://github.com/zerodytrash/), but has since taken on its own identity as it has added more features & changed much of its core functionality.
 
 
 Join the [support discord](https://discord.gg/e2XwPNTBBr) and visit the `#support` channel for questions, contributions and ideas. Feel free to make pull requests with missing/new features, fixes, etc.
 
 > **UPDATE:**<br>Due to a change on the part of TikTok, versions prior to **v4.3.8** are no longer functional. If you are using an unsupported version, upgrade to the latest version using the `pip install TikTokLive --upgrade` command.
 
+## Other Languages
+
+TikTok LIVE is availible in several alternative languages with only slight differences between the versions:
+
+- **Node.JS:** https://github.com/zerodytrash/TikTok-Live-Connector
+- **Go:** https://github.com/Davincible/gotiktoklive
+- **C#/Unity:** https://github.com/frankvHoof93/TikTokLiveSharp
+
 ## Table of Contents
 
 **Primary Information**
 
 - [Documentation](https://isaackogan.github.io/TikTokLive/)
 - [Contributors](#contributors)
 - [License](#license)
@@ -107,46 +114,46 @@
 
 if __name__ == '__main__':
     # Run the client and block the main thread
     # await client.start() to run non-blocking
     client.run()
 ```
 
-For more examples, [see the examples folder](https://github.com/isaackogan/TikTok-Live-Connector/tree/master/examples) provided in the tree.
+For more examples, [see the examples folder](https://github.com/isaackogan/TikTokLive/tree/master/examples) provided in the tree.
 
 ## Params & Options
 
 To create a new `TikTokLiveClient` object the following parameter is required. You can optionally add configuration options to this via kwargs.
 
 `TikTokLiveClient(unique_id, **options)`
 
-| Param Name | Required | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-|------------|----------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| unique_id  | Yes      | The unique username of the broadcaster. You can find this name in the URL.<br>Example: `https://www.tiktok.com/@isaackogz` => `isaackogz`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-| **options  | No       | Here you can set the following optional connection properties. If you do not specify a value, the default value will be used.<br><br>`process_initial_data` (default: `True`) <br> Define if you want to process initial data upon connecting (e.g. first 1-10 messages from BEFORE you connected).<br><br>`fetch_room_info_on_connect` (default: `True`) <br> Define if you want to fetch all room information on start. If this option is enabled, connection to offline rooms will be prevented. If enabled, the connect result contains the room info via the `room_info` attribute. You can also manually retrieve the room info (even in an unconnected state) using the `retrieve_room_info()` method.<br><br>`enable_detailed_gifts` (default: `False`) <br> Define if you want to receive extended information about gifts like gift name, cost and images which you can retrieve via the `available_gifts` attribute. When enabled, the `details` attribute in a `Gift` object will be populated.<br><br>`ws_ping_interval` (default: `10.0`) <br> The interval between keepalive pings on the websocket connection (in seconds).<br><br>`ws_timeout` (default: `10.0`)<br>How long to wait before the websocket connection is considered timed out (in seconds).<br><br>`http_timeout` (default: `10.0`) <br> How long to wait before considering an HTTP request in the http client timed out (in seconds).<br><br>`http_headers` (default: `{}`) <br> Additional HTTP client headers to include when making requests to the Webcast API AND connecting to the websocket server.<br><br>`http_params` (default: `{}`) <br>Additional HTTP client parameters to include when making requests to the Webcast API AND connecting to the websocket.<br><br>`loop` (default: `None`)<br>Optionally supply your own asyncio event loop for usage by the client. When set to None, the client pulls the current active loop or creates a new one. This option is mostly useful for people trying to nest asyncio.<br/><br/>`trust_env` (default: `False`)<br/>Whether to trust environment variables that provide proxies in httpx requests<br/><br/>`proxies` (default: `None`)<br/>Enable proxied requests by turning on forwarding for the HTTP "proxies" argument. Websocket connections will NOT be proxied<br/><br/>`lang` (default: `en-US`)<br/>Change the language. Payloads *will* be in English, but front-end content will be in the desired language!<br/><br/>`sign_api_key` (default: `None`)<br/>Parameter to increase the amount of connections allowed to be made per minute via a Sign Server API key. If you need this, contact the project maintainer. |
+| Param Name | Required | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+|------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| unique_id  | Yes      | The unique username of the broadcaster. You can find this name in the URL.<br>Example: `https://www.tiktok.com/@isaackogz` => `isaackogz`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| **options  | No       | Here you can set the following optional connection properties. If you do not specify a value, the default value will be used.<br><br>`process_initial_data` (default: `True`) <br> Define if you want to process initial data upon connecting (e.g. first 1-10 messages from BEFORE you connected).<br><br>`fetch_room_info_on_connect` (default: `True`) <br> Define if you want to fetch all room information on start. If this option is enabled, connection to offline rooms will be prevented. If enabled, the connect result contains the room info via the `room_info` attribute. You can also manually retrieve the room info (even in an unconnected state) using the `retrieve_room_info()` method.<br><br>`enable_detailed_gifts` (default: `False`) <br> Define if you want to receive extended information about gifts like gift name, cost and images which you can retrieve via the `available_gifts` attribute. When enabled, the `details` attribute in a `Gift` object will be populated.<br><br>`ws_ping_interval` (default: `10.0`) <br> The interval between keepalive pings on the websocket connection (in seconds).<br><br>`ws_timeout` (default: `10.0`)<br>How long to wait before the websocket connection is considered timed out (in seconds).<br><br>`http_timeout` (default: `10.0`) <br> How long to wait before considering an HTTP request in the http client timed out (in seconds).<br><br>`http_headers` (default: `{}`) <br> Additional HTTP client headers to include when making requests to the Webcast API AND connecting to the websocket server.<br><br>`http_params` (default: `{}`) <br>Additional HTTP client parameters to include when making requests to the Webcast API AND connecting to the websocket.<br><br>`loop` (default: `None`)<br>Optionally supply your own asyncio event loop for usage by the client. When set to None, the client pulls the current active loop or creates a new one. This option is mostly useful for people trying to nest asyncio.<br/><br/>`trust_env` (default: `False`)<br/>Whether to trust environment variables that provide proxies in httpx requests<br/><br/>`proxies` (default: `None`)<br/>Enable proxied requests by turning on forwarding for the HTTP "proxies" argument. Websocket connections will NOT be proxied<br/><br/>`lang` (default: `en-US`)<br/>Change the language. Payloads *will* be in English, but front-end content will be in the desired language!<br/><br/>`sign_api_key` (default: `None`)<br/>Parameter to increase the amount of connections allowed to be made per minute via a Sign Server API key. If you need this, contact the project maintainer.<br/><br/>`ssl_context` (default: `None`)<br/>Providing an SSLContext object overrides the default context used in HTTP requests made to TikTok. This is useful if TikTok sends invalid SSL signatures, as you can provide a "no verify" context. |
 
 
 ## Methods
 
-A `TikTokLiveClient` object contains the following methods.
+A `TikTokLiveClient` object contains the following methods:
 
-| Method Name              | Description                                                                                                                                                                       |
-|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| run                      | Starts a connection to the live chat while blocking the main thread                                                                                                               |
-| start                    | (async) Connects to the live chat without blocking the main thread                                                                                                                |
-| stop                     | Turns off the connection to the live chat.                                                                                                                                        |
-| retrieve_room_info       | (async) Gets the current room info from TikTok API                                                                                                                                |
-| retrieve_available_gifts | (async) Retrieves a list of the available gifts for the room and adds it to the `extended_gift` attribute of the `Gift` object on the `gift` event, when enabled.                 |
-| add_listener             | Adds an *asynchronous* listener function (or, you can decorate a function with `@client.on("<event>")`) and takes two parameters, an event name and the payload, an AbstractEvent ||
-| download                 | Start downloading the livestream video for a given duration or until stopped via the `stop_download` method                                                                       |
-| stop_download            | Stop downloading the livestream video if currently downloading, otherwise throws an error                                                                                         |
+| Method Name              | Description                                                                                                                                                                                                                   |
+|--------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| run                      | Starts a connection to the live chat while blocking the main thread                                                                                                                                                           |
+| start                    | (async) Connects to the live chat without blocking the main thread                                                                                                                                                            |
+| stop                     | Turns off the connection to the live chat.                                                                                                                                                                                    |
+| retrieve_room_info       | (async) Gets the current room info from TikTok API                                                                                                                                                                            |
+| retrieve_available_gifts | (async) Retrieves a list of the available gifts for the room and adds it to the `extended_gift` attribute of the `Gift` object on the `gift` event, when enabled.                                                             |
+| add_listener             | Adds an *asynchronous* listener function (or, you can decorate a function with `@client.on("<event>")`) and takes two parameters, an event name and the payload, an AbstractEvent                                             ||
+| download                 | Start downloading the livestream video for a given duration or until stopped via the `stop_download` method. Supports the ability to add different flags, like `-c copy` which may reduce CPU usage by disabling transcoding. |
+| stop_download            | Stop downloading the livestream video if currently downloading, otherwise throws an error                                                                                                                                     |
 
 ## Attributes
 
-A `TikTokLiveClient` object contains the following attributes.
+A `TikTokLiveClient` object contains the following attributes:
 
 | Attribute Name  | Description                                                                                                                                  |
 |-----------------|----------------------------------------------------------------------------------------------------------------------------------------------|
 | room_id         | The Room ID of the livestream room the client is currently connected to                                                                      |
 | room_info       | Information about the given livestream room                                                                                                  |
 | unique_id       | The TikTok username of the person whose livestream the client is currently connected to (e.g. @charlidamelio)                                |
 | connected       | Whether the client is currently connected to a livestream                                                                                    |
@@ -261,15 +268,15 @@
 ### `more_share`
 
 Triggered when 5 or 10 users join from a viewer's share link.
 
 ```python
 @client.on("more_share")
 async def on_connect(event: MoreShareEvent):
-    print(f"More than {event.amount} users have joined from {user.unique_id}'s share link!")
+    print(f"More than {event.amount} users have joined from {event.user.unique_id}'s share link!")
 ```
 
 
 ### `viewer_update`
 
 Triggered every time the viewer count is updated. This event also updates the cached viewer count by default.
 
@@ -313,22 +320,32 @@
 
 ```python
 @client.on("envelope")
 async def on_connect(event: EnvelopeEvent):
     print(f"{event.treasure_box_user.unique_id} -> {event.treasure_box_data}")
 ```
 
-### `weekly_ranking`
+### `ranking_update`
 
-Triggered when a weekly ranking update is sent out.
+Triggered when a **stream** rank update is sent out. Can be `Weekly Ranking` or `Rising Star`!
 
 ```python
-@client.on("weekly_ranking")
-async def on_connect(event: WeeklyRankingEvent):
-    print(f"{client.unique_id} has the rank #{event.data.rank} of all streamers!")
+@client.on("ranking_update")
+async def on_connect(event: RankingUpdateEvent):
+    print(f"{event.user.unique_id} has the rank #{event.rank} for the {event.type} leaderboard.")
+```
+
+### `user_ranking_update`
+
+Triggered when a **user** rank update is sent out. Can be `Top Viewer`
+ status.
+```python
+@client.on("user_ranking_update")
+async def on_connect(event: UserRankingUpdateEvent):
+    print(f"{event.user.unique_id} just became a #{event.rank} top viewer!")
 ```
 
 ### `mic_battle_start`
 
 Triggered when a Mic Battle starts!
 
 ```python
@@ -422,9 +439,7 @@
 * **David Teather** - *TikTokLive Introduction Tutorial* - [davidteather](https://github.com/davidteather)
 
 See also the full list of [contributors](https://github.com/isaackogan/TikTokLive/contributors) who have participated in this project.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-
```

### Comparing `TikTokLive-5.0.7/TikTokLive.egg-info/SOURCES.txt` & `TikTokLive-5.0.8/TikTokLive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TikTokLive-5.0.7/setup.py` & `TikTokLive-5.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 # PyPi upload Command
 # rm -r dist ; python setup.py sdist ; python -m twine upload dist/*
 
 setuptools.setup(
     name="TikTokLive",
     packages=setuptools.find_packages(),
-    version="5.0.7",
+    version="5.0.8",
     license="MIT",
     description="TikTok Live Connection Client",
     author="Isaac Kogan",
     author_email="info@isaackogan.com",
     url="https://github.com/isaackogan/TikTokLive",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    download_url="https://github.com/isaackogan/TikTokLive/releases/tag/v5.0.7",
+    download_url="https://github.com/isaackogan/TikTokLive/releases/tag/v5.0.8",
     keywords=["tiktok", "tiktok live", "python3", "api", "unofficial"],
     install_requires=[
         "httpx>=0.23.0",  # Make requests
         "protobuf3-to-dict>=0.1.5",  # Convert Protobuf to Dict
         "protobuf>=3.19.4",  # Decode Protobuf Messages
         "pyee>=9.0.4",  # Event Emitter
         "ffmpy>=0.3.0",  # Download streams
```

