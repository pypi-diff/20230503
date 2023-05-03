# Comparing `tmp/waifuim.py-4.2.0.tar.gz` & `tmp/waifuim.py-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waifuim.py-4.2.0.tar", last modified: Wed May  3 18:02:06 2023, max compression
+gzip compressed data, was "waifuim.py-4.2.2.tar", last modified: Tue Mar 21 19:18:51 2023, max compression
```

## Comparing `waifuim.py-4.2.0.tar` & `waifuim.py-4.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:02:06.569820 waifuim.py-4.2.0/
--rw-rw-rw-   0        0        0     1082 2022-12-10 05:08:58.000000 waifuim.py-4.2.0/LICENSE
--rw-rw-rw-   0        0        0     4215 2023-05-03 18:02:06.569820 waifuim.py-4.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3119 2023-03-09 15:27:43.000000 waifuim.py-4.2.0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-03 18:02:06.576878 waifuim.py-4.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1493 2022-12-10 05:08:58.000000 waifuim.py-4.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:02:06.536755 waifuim.py-4.2.0/waifuim/
--rw-rw-rw-   0        0        0     1252 2022-12-10 05:08:58.000000 waifuim.py-4.2.0/waifuim/__init__.py
--rw-rw-rw-   0        0        0    15485 2023-03-12 07:24:10.000000 waifuim.py-4.2.0/waifuim/aioclient.py
--rw-rw-rw-   0        0        0     1974 2022-12-10 05:08:58.000000 waifuim.py-4.2.0/waifuim/exceptions.py
--rw-rw-rw-   0        0        0     1134 2023-05-03 17:52:31.000000 waifuim.py-4.2.0/waifuim/moduleinfo.py
--rw-rw-rw-   0        0        0     1238 2023-05-03 17:57:29.000000 waifuim.py-4.2.0/waifuim/types.py
--rw-rw-rw-   0        0        0     1519 2022-12-10 05:08:58.000000 waifuim.py-4.2.0/waifuim/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:02:06.569820 waifuim.py-4.2.0/waifuim.py.egg-info/
--rw-rw-rw-   0        0        0     4215 2023-05-03 18:02:06.000000 waifuim.py-4.2.0/waifuim.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-03 18:02:06.000000 waifuim.py-4.2.0/waifuim.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:02:06.000000 waifuim.py-4.2.0/waifuim.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-03 18:02:06.000000 waifuim.py-4.2.0/waifuim.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 18:02:06.000000 waifuim.py-4.2.0/waifuim.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-21 19:18:50.994529 waifuim.py-4.2.2/
+-rw-rw-rw-   0        0        0     1082 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/LICENSE
+-rw-rw-rw-   0        0        0     4313 2023-03-21 19:18:50.994529 waifuim.py-4.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3240 2023-03-21 19:10:23.000000 waifuim.py-4.2.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-03-21 19:18:50.997520 waifuim.py-4.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1493 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-21 19:18:50.978572 waifuim.py-4.2.2/waifuim/
+-rw-rw-rw-   0        0        0     1252 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/waifuim/__init__.py
+-rw-rw-rw-   0        0        0    16582 2023-03-21 18:45:31.000000 waifuim.py-4.2.2/waifuim/aioclient.py
+-rw-rw-rw-   0        0        0     1974 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/waifuim/exceptions.py
+-rw-rw-rw-   0        0        0     1134 2023-03-21 18:42:55.000000 waifuim.py-4.2.2/waifuim/moduleinfo.py
+-rw-rw-rw-   0        0        0      801 2023-03-06 16:41:48.000000 waifuim.py-4.2.2/waifuim/types.py
+-rw-rw-rw-   0        0        0     1519 2022-04-11 11:41:39.000000 waifuim.py-4.2.2/waifuim/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-21 19:18:50.993532 waifuim.py-4.2.2/waifuim.py.egg-info/
+-rw-rw-rw-   0        0        0     4313 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-03-21 19:18:50.000000 waifuim.py-4.2.2/waifuim.py.egg-info/top_level.txt
```

### Comparing `waifuim.py-4.2.0/LICENSE` & `waifuim.py-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.0/PKG-INFO` & `waifuim.py-4.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: waifuim.py
-Version: 4.2.0
+Version: 4.2.2
 Summary: A Python wrapper for waifu.im API.
 Home-page: https://github.com/Waifu-im/waifuim.py
 Author: Buco
 Author-email: bucolo33fr@gmail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/Waifu-im/waifuim.py/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -69,14 +68,20 @@
     image = await wf.search()
     
     # Get an image by tags
     image = await wf.search(
         included_tags=['waifu','maid'],
         excluded_tags=['ero'],
     )
+
+    image = await wf.search(
+        excluded_tags=['maid'],
+        is_nsfw='null',
+        height="<=252"
+    )
     
     # Get sfw waifu images ordered by FAVORITES
     images = await wf.search(
         included_tags=['waifu'],
         is_nsfw='null',
         many=True,
         order_by='FAVORITES',
@@ -142,9 +147,7 @@
 )
 
 # ...
 ```
 
 ## License
 MIT Â© [Buco](https://github.com/Waifu-im/waifuim.py/blob/main/LICENSE)
-
-
```

### Comparing `waifuim.py-4.2.0/README.md` & `waifuim.py-4.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,20 @@
     image = await wf.search()
     
     # Get an image by tags
     image = await wf.search(
         included_tags=['waifu','maid'],
         excluded_tags=['ero'],
     )
+
+    image = await wf.search(
+        excluded_tags=['maid'],
+        is_nsfw='null',
+        height="<=252"
+    )
     
     # Get sfw waifu images ordered by FAVORITES
     images = await wf.search(
         included_tags=['waifu'],
         is_nsfw='null',
         many=True,
         order_by='FAVORITES',
```

### Comparing `waifuim.py-4.2.0/setup.py` & `waifuim.py-4.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.0/waifuim/__init__.py` & `waifuim.py-4.2.2/waifuim/__init__.py`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.0/waifuim/aioclient.py` & `waifuim.py-4.2.2/waifuim/aioclient.py`

 * *Files 11% similar despite different names*

```diff
@@ -125,14 +125,17 @@
             excluded_tags: List[str] = None,
             included_files: List[str] = None,
             excluded_files: List[str] = None,
             is_nsfw: Union[bool, str] = None,
             many: bool = None,
             order_by: str = None,
             orientation: str = None,
+            width: str = None,
+            height: str = None,
+            byte_size: str = None,
             gif: bool = None,
             full: str = None,
             token: str = None,
             raw: bool = False,
     ) -> Union[List[Image], Image, Dict]:
         """Gets a single or multiple images from the API.
         Kwargs:
@@ -140,14 +143,17 @@
             excluded_tags: The tag(s) that you want to exclude
             excluded_files: A list of files that you do not want to get.
             is_nsfw: If False is provided prevent the API to return nsfw files, else if True is provided force it to do
             so, if 'null' is provided it's random (Default fixed by the API, see the documentation).
             many: Get multiples images instead of a single one (see the api docs for the exact number).
             order_by: Order the images according to the value given (see the docs for the accepted values)
             orientation: Choose the images orientation according to the value given (see the docs for the accepted values)
+            width: Filter images by width (in pixels). Accepted operators: <=, >=, >, <, !=, =. e.g. >=2000
+            height: Filter images by height (in pixels). Accepted operators: <=, >=, >, <, !=, =. e.g. >=2000
+            byte_size: Filter images by byte size. Accepted operators: <=, >=, >, <, !=, =. e.g. >=2000
             gif: If False is provided prevent the API to return .gif files, else if True is provided force it to do so
             if nothing (or None) is provided then no filter is applied.
             full: Do not limit the result length (only for admins)
             raw : If True return the raw result.
         Returns:
             A single or a list of Image (find it in types.py).
         Raises:
@@ -157,14 +163,17 @@
                                      excluded_tags=excluded_tags,
                                      included_files=included_files,
                                      excluded_files=excluded_files,
                                      is_nsfw=is_nsfw,
                                      many=many,
                                      order_by=order_by,
                                      orientation=orientation,
+                                     width=width,
+                                     height=height,
+                                     byte_size=byte_size,
                                      gif=gif,
                                      full=full
                                      )
         headers = {}
         if full:
             if not token and not self.token:
                 raise NoToken(detail="the 'full' query string is only accessible to admins and needs a token")
@@ -182,17 +191,19 @@
             self,
             user_id: int = None,
             included_tags: List[str] = None,
             excluded_tags: List[str] = None,
             included_files: List[str] = None,
             excluded_files: List[str] = None,
             is_nsfw: Union[bool, str] = None,
-            many: bool = None,
             order_by: str = None,
             orientation: str = None,
+            width: str = None,
+            height: str = None,
+            byte_size: str = None,
             gif: bool = None,
             token: str = None,
             raw: bool = False,
     ) -> Union[List[Image], Dict]:
         """Get your favourite gallery.""
 
         Kwargs:
@@ -201,14 +212,17 @@
             excluded_tags: The tag(s) that you want to exclude
             excluded_files: A list of files that you do not want to get.
             is_nsfw: If False is provided prevent the API to return nsfw files, else if True is provided force it to do
             so, if 'null' is provided it's random (Default fixed by the API, see the documentation).
             many: Get multiples images instead of a single one (see the api docs for the exact number).
             order_by: Order the images according to the value given (see the docs for the accepted values)
             orientation: Choose the images orientation according to the value given (see the docs for the accepted values)
+            width: Filter images by width (in pixels). Accepted operators: <=, >=, >, <, !=, =. e.g. >=2000
+            height: Filter images by height (in pixels). Accepted operators: <=, >=, >, <, !=, =. e.g. >=2000
+            byte_size: Filter images by byte size. Accepted operators: <=, >=, >, <, !=, =. e.g. >=2000
             gif: If False is provided prevent the API to return .gif files, else if True is provided force it to do so
             if nothing (or None) is provided then no filter is applied.
             token: The token that will be use for this request only, this doesn't change the token passed in __init__.
             raw : If True return the raw result.
         Returns:
             A dictionary containing the json the API returned.
         Raises:
@@ -216,17 +230,19 @@
         """
         params = self._create_params(user_id=user_id,
                                      included_tags=included_tags,
                                      excluded_tags=excluded_tags,
                                      included_files=included_files,
                                      excluded_files=excluded_files,
                                      is_nsfw=is_nsfw,
-                                     many=many,
                                      order_by=order_by,
                                      orientation=orientation,
+                                     width=width,
+                                     height=height,
+                                     byte_size=byte_size,
                                      gif=gif,
                                      )
         headers = self._create_headers(**{'Authorization': f'Bearer {token if token else self.token}'})
 
         infos = await self._make_request(f"{APIBaseURL}fav", 'get', params=params, headers=headers)
         if raw:
             return infos
```

### Comparing `waifuim.py-4.2.0/waifuim/exceptions.py` & `waifuim.py-4.2.2/waifuim/exceptions.py`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.0/waifuim/moduleinfo.py` & `waifuim.py-4.2.2/waifuim/moduleinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE."""
 
 __author__ = 'Buco'
-__version__ = '4.2.0'
+__version__ = '4.2.2'
```

### Comparing `waifuim.py-4.2.0/waifuim/types.py` & `waifuim.py-4.2.2/waifuim/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,29 @@
 from dateutil.parser import parse
 
 
-class Artist:
-    """Represents an API Artist."""
-
-    def __init__(self, data):
-        for key, values in data.items():
-            setattr(self, key.lower(), values)
-
-    def __str__(self):
-        return self.name
-
-    def __eq__(self, other):
-        return isinstance(other, Artist) and self.artist_id == other.artist_id
-
-
 class Tag:
     """Represents an API tag."""
-
     def __init__(self, data):
         for key, values in data.items():
             setattr(self, key.lower(), values)
 
     def __str__(self):
         return self.name
 
     def __eq__(self, other):
         return isinstance(other, Tag) and self.tag_id == other.tag_id
 
 
 class Image:
     """Represents an API Image."""
-
     def __init__(self, data):
         for key, values in data.items():
             setattr(self, key.lower(), values)
-
         self.tags = [Tag(tag) for tag in self.tags]
-
-        if self.artist is not None:
-            self.artist = Artist(self.artist)
-
         self.uploaded_at = parse(self.uploaded_at)
 
     def __str__(self):
         return self.url
 
     def __eq__(self, other):
         return isinstance(other, Image) and self.image_id == other.image_id
```

### Comparing `waifuim.py-4.2.0/waifuim/utils.py` & `waifuim.py-4.2.2/waifuim/utils.py`

 * *Files identical despite different names*

### Comparing `waifuim.py-4.2.0/waifuim.py.egg-info/PKG-INFO` & `waifuim.py-4.2.2/waifuim.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: waifuim.py
-Version: 4.2.0
+Version: 4.2.2
 Summary: A Python wrapper for waifu.im API.
 Home-page: https://github.com/Waifu-im/waifuim.py
 Author: Buco
 Author-email: bucolo33fr@gmail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/Waifu-im/waifuim.py/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -69,14 +68,20 @@
     image = await wf.search()
     
     # Get an image by tags
     image = await wf.search(
         included_tags=['waifu','maid'],
         excluded_tags=['ero'],
     )
+
+    image = await wf.search(
+        excluded_tags=['maid'],
+        is_nsfw='null',
+        height="<=252"
+    )
     
     # Get sfw waifu images ordered by FAVORITES
     images = await wf.search(
         included_tags=['waifu'],
         is_nsfw='null',
         many=True,
         order_by='FAVORITES',
@@ -142,9 +147,7 @@
 )
 
 # ...
 ```
 
 ## License
 MIT Â© [Buco](https://github.com/Waifu-im/waifuim.py/blob/main/LICENSE)
-
-
```

