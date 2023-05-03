# Comparing `tmp/marpdown-0.4.0.tar.gz` & `tmp/marpdown-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/marpdown-0.4.0.tar", last modified: Wed May  3 11:18:25 2023, max compression
+gzip compressed data, was "marpdown-0.5.0.tar", last modified: Wed May  3 11:56:26 2023, max compression
```

## Comparing `marpdown-0.4.0.tar` & `marpdown-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-03 11:18:25.000000 marpdown-0.4.0/
--rw-r--r--   0 leo       (1000) leo       (1000)     1066 2023-05-03 08:45:11.000000 marpdown-0.4.0/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      427 2023-05-03 11:18:25.000000 marpdown-0.4.0/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)       41 2023-05-03 08:45:11.000000 marpdown-0.4.0/README.md
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-03 11:18:25.000000 marpdown-0.4.0/marpdown/
--rw-r--r--   0 leo       (1000) leo       (1000)      116 2023-05-03 08:45:11.000000 marpdown-0.4.0/marpdown/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2943 2023-05-03 08:45:11.000000 marpdown-0.4.0/marpdown/css.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2462 2023-05-03 08:45:11.000000 marpdown-0.4.0/marpdown/ppt.py
--rw-r--r--   0 leo       (1000) leo       (1000)     3379 2023-05-03 11:15:29.000000 marpdown-0.4.0/marpdown/slide.py
--rw-r--r--   0 leo       (1000) leo       (1000)      240 2023-05-03 08:45:11.000000 marpdown-0.4.0/marpdown/utils.py
--rw-r--r--   0 leo       (1000) leo       (1000)      584 2023-05-03 08:45:11.000000 marpdown-0.4.0/marpdown/writer.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-03 11:18:25.000000 marpdown-0.4.0/marpdown.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      427 2023-05-03 11:18:24.000000 marpdown-0.4.0/marpdown.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      262 2023-05-03 11:18:25.000000 marpdown-0.4.0/marpdown.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-05-03 11:18:24.000000 marpdown-0.4.0/marpdown.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        9 2023-05-03 11:18:25.000000 marpdown-0.4.0/marpdown.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-05-03 11:18:25.000000 marpdown-0.4.0/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      605 2023-05-03 11:14:37.000000 marpdown-0.4.0/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-03 11:56:26.716434 marpdown-0.5.0/
+-rw-r--r--   0 leo       (1000) leo       (1000)     1066 2023-05-03 08:45:11.000000 marpdown-0.5.0/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      390 2023-05-03 11:56:26.716434 marpdown-0.5.0/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)       41 2023-05-03 08:45:11.000000 marpdown-0.5.0/README.md
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-03 11:56:26.712434 marpdown-0.5.0/marpdown/
+-rw-r--r--   0 leo       (1000) leo       (1000)      116 2023-05-03 08:45:11.000000 marpdown-0.5.0/marpdown/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2994 2023-05-03 11:31:06.000000 marpdown-0.5.0/marpdown/css.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2462 2023-05-03 08:45:11.000000 marpdown-0.5.0/marpdown/ppt.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     3380 2023-05-03 11:22:09.000000 marpdown-0.5.0/marpdown/slide.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      240 2023-05-03 08:45:11.000000 marpdown-0.5.0/marpdown/utils.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      584 2023-05-03 08:45:11.000000 marpdown-0.5.0/marpdown/writer.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-03 11:56:26.716434 marpdown-0.5.0/marpdown.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      390 2023-05-03 11:56:26.000000 marpdown-0.5.0/marpdown.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      262 2023-05-03 11:56:26.000000 marpdown-0.5.0/marpdown.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-05-03 11:56:26.000000 marpdown-0.5.0/marpdown.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        9 2023-05-03 11:56:26.000000 marpdown-0.5.0/marpdown.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-05-03 11:56:26.716434 marpdown-0.5.0/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      605 2023-05-03 11:55:41.000000 marpdown-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `marpdown-0.4.0/LICENSE` & `marpdown-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marpdown-0.4.0/marpdown/css.py` & `marpdown-0.5.0/marpdown/css.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,14 +122,17 @@
   color: black !important;
 }
 '''
 
 CARD = '''.card-container {
   display: flex;
   justify-content: center;
+  flex-wrap: wrap;
+  padding: 20px;
+  width: 100%;
 }
 
 .card {
   background-color: #cceeff;
   border-radius: 5px;
   padding: 20px;
   width: 250px;
```

### Comparing `marpdown-0.4.0/marpdown/ppt.py` & `marpdown-0.5.0/marpdown/ppt.py`

 * *Files identical despite different names*

### Comparing `marpdown-0.4.0/marpdown/slide.py` & `marpdown-0.5.0/marpdown/slide.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         super().__init__(content=self.__writer__.getValue(), backgroundImage=backgroundImage)
 
 class CardSlide(BaseSlide):
     def __init__(self, *, title: str,text:str, cards: list[tuple[str,list[str]]] ,backgroundImage: str = None):
         self.__writer__ = Writer()
         self.__writer__.append(f"# {title}")
         self.__writer__.append(text)
-        self.__writer__.append('<div class="card-container">')
+        self.__writer__.append(' <div class="card-container">')
         for card in cards:
             name,bulletpoints = card
             self.__writer__.append(f'''<div class="card">
     <h2>{name}</h2>
     <p>
       {utils.list_to_html_ul(bulletpoints)}
     </p>
```

### Comparing `marpdown-0.4.0/marpdown/writer.py` & `marpdown-0.5.0/marpdown/writer.py`

 * *Files identical despite different names*

### Comparing `marpdown-0.4.0/setup.py` & `marpdown-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [
 
 ]
 
 setup(
     name="marpdown",
-    version="0.4.0",
+    version="0.5.0",
     author="Tao Xiang",
     author_email="tao.xiang@tum.de",
     description="A package of RL algorithms",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/leoxiang66/marpdown",
     packages=find_packages(),
```

