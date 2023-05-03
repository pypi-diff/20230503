# Comparing `tmp/SpotifyPictureHelper-0.1.0.tar.gz` & `tmp/SpotifyPictureHelper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpotifyPictureHelper-0.1.0.tar", last modified: Sun Mar 26 03:16:06 2023, max compression
+gzip compressed data, was "SpotifyPictureHelper-0.2.0.tar", last modified: Wed May  3 04:04:44 2023, max compression
```

## Comparing `SpotifyPictureHelper-0.1.0.tar` & `SpotifyPictureHelper-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-03-26 03:16:06.015122 SpotifyPictureHelper-0.1.0/
--rw-r--r--   0 daisyye    (501) staff       (20)      588 2023-03-26 01:55:08.000000 SpotifyPictureHelper-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 daisyye    (501) staff       (20)    11357 2023-02-17 19:38:03.000000 SpotifyPictureHelper-0.1.0/LICENSE
--rw-r--r--   0 daisyye    (501) staff       (20)      380 2023-03-26 03:13:44.000000 SpotifyPictureHelper-0.1.0/MANIFEST.in
--rw-r--r--   0 daisyye    (501) staff       (20)     1136 2023-03-10 21:58:56.000000 SpotifyPictureHelper-0.1.0/Makefile
--rw-r--r--   0 daisyye    (501) staff       (20)      336 2023-03-26 03:16:06.015381 SpotifyPictureHelper-0.1.0/PKG-INFO
--rw-r--r--   0 daisyye    (501) staff       (20)     1937 2023-03-26 03:13:44.000000 SpotifyPictureHelper-0.1.0/README.md
-drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-03-26 03:16:06.002028 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/
--rw-r--r--   0 daisyye    (501) staff       (20)        0 2023-03-10 21:51:02.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/__init__.py
--rw-r--r--   0 daisyye    (501) staff       (20)       22 2023-03-10 21:50:19.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/_version.py
--rw-r--r--   0 daisyye    (501) staff       (20)     4568 2023-03-10 21:55:56.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/main.py
-drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-03-26 03:16:06.014381 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/tests/
--rw-r--r--   0 daisyye    (501) staff       (20)   269272 2023-03-10 21:36:53.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/tests/fakeArtist.html
--rw-r--r--   0 daisyye    (501) staff       (20)   307980 2023-03-10 21:12:24.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/tests/fakePlaylist.html
--rw-r--r--   0 daisyye    (501) staff       (20)    59842 2023-03-10 20:43:38.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/tests/fakeUser.html
--rw-r--r--   0 daisyye    (501) staff       (20)     3951 2023-03-10 21:50:19.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/tests/test_all.py
-drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-03-26 03:16:06.005826 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper.egg-info/
--rw-r--r--   0 daisyye    (501) staff       (20)      336 2023-03-26 03:16:05.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper.egg-info/PKG-INFO
--rw-r--r--   0 daisyye    (501) staff       (20)      660 2023-03-26 03:16:05.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper.egg-info/SOURCES.txt
--rw-r--r--   0 daisyye    (501) staff       (20)        1 2023-03-26 03:16:05.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper.egg-info/dependency_links.txt
--rw-r--r--   0 daisyye    (501) staff       (20)       64 2023-03-26 03:16:05.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper.egg-info/entry_points.txt
--rw-r--r--   0 daisyye    (501) staff       (20)        1 2023-03-26 03:16:05.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper.egg-info/not-zip-safe
--rw-r--r--   0 daisyye    (501) staff       (20)      119 2023-03-26 03:16:05.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper.egg-info/requires.txt
--rw-r--r--   0 daisyye    (501) staff       (20)       21 2023-03-26 03:16:05.000000 SpotifyPictureHelper-0.1.0/SpotifyPictureHelper.egg-info/top_level.txt
--rw-r--r--   0 daisyye    (501) staff       (20)     1405 2023-03-26 03:13:44.000000 SpotifyPictureHelper-0.1.0/pyproject.toml
--rw-r--r--   0 daisyye    (501) staff       (20)      721 2023-03-26 03:16:06.016691 SpotifyPictureHelper-0.1.0/setup.cfg
--rw-r--r--   0 daisyye    (501) staff       (20)       38 2023-03-10 21:50:19.000000 SpotifyPictureHelper-0.1.0/setup.py
+drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-03 04:04:44.377290 SpotifyPictureHelper-0.2.0/
+-rw-r--r--   0 daisyye    (501) staff       (20)      588 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 daisyye    (501) staff       (20)    11357 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/LICENSE
+-rw-r--r--   0 daisyye    (501) staff       (20)      380 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/MANIFEST.in
+-rw-r--r--   0 daisyye    (501) staff       (20)     1136 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/Makefile
+-rw-r--r--   0 daisyye    (501) staff       (20)      336 2023-05-03 04:04:44.377493 SpotifyPictureHelper-0.2.0/PKG-INFO
+-rw-r--r--   0 daisyye    (501) staff       (20)     4718 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/README.md
+drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-03 04:04:44.358539 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/
+-rw-r--r--   0 daisyye    (501) staff       (20)        0 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/__init__.py
+-rw-r--r--   0 daisyye    (501) staff       (20)       22 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/_version.py
+-rw-r--r--   0 daisyye    (501) staff       (20)    10051 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/main.py
+drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-03 04:04:44.376468 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/
+-rw-r--r--   0 daisyye    (501) staff       (20)    17435 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/blackWhite.png
+-rw-r--r--   0 daisyye    (501) staff       (20)   269272 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakeArtist.html
+-rw-r--r--   0 daisyye    (501) staff       (20)   307980 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakePlaylist.html
+-rw-r--r--   0 daisyye    (501) staff       (20)    59842 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakeUser.html
+-rw-r--r--   0 daisyye    (501) staff       (20)     1541 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/overlay.png
+-rw-r--r--   0 daisyye    (501) staff       (20)    14988 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/test2.png
+-rw-r--r--   0 daisyye    (501) staff       (20)     7458 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/test_all.py
+drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-03 04:04:44.362295 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/
+-rw-r--r--   0 daisyye    (501) staff       (20)      336 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/PKG-INFO
+-rw-r--r--   0 daisyye    (501) staff       (20)      778 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)        1 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)       64 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/entry_points.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)        1 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/not-zip-safe
+-rw-r--r--   0 daisyye    (501) staff       (20)      119 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/requires.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)       21 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/top_level.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)     1431 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/pyproject.toml
+-rw-r--r--   0 daisyye    (501) staff       (20)      721 2023-05-03 04:04:44.378330 SpotifyPictureHelper-0.2.0/setup.cfg
+-rw-r--r--   0 daisyye    (501) staff       (20)       38 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/setup.py
```

### Comparing `SpotifyPictureHelper-0.1.0/CONTRIBUTING.md` & `SpotifyPictureHelper-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.1.0/LICENSE` & `SpotifyPictureHelper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.1.0/Makefile` & `SpotifyPictureHelper-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/tests/fakeArtist.html` & `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakeArtist.html`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/tests/fakePlaylist.html` & `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakePlaylist.html`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.1.0/SpotifyPictureHelper/tests/fakeUser.html` & `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakeUser.html`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.1.0/SpotifyPictureHelper.egg-info/SOURCES.txt` & `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,11 +12,14 @@
 SpotifyPictureHelper.egg-info/PKG-INFO
 SpotifyPictureHelper.egg-info/SOURCES.txt
 SpotifyPictureHelper.egg-info/dependency_links.txt
 SpotifyPictureHelper.egg-info/entry_points.txt
 SpotifyPictureHelper.egg-info/not-zip-safe
 SpotifyPictureHelper.egg-info/requires.txt
 SpotifyPictureHelper.egg-info/top_level.txt
+SpotifyPictureHelper/tests/blackWhite.png
 SpotifyPictureHelper/tests/fakeArtist.html
 SpotifyPictureHelper/tests/fakePlaylist.html
 SpotifyPictureHelper/tests/fakeUser.html
+SpotifyPictureHelper/tests/overlay.png
+SpotifyPictureHelper/tests/test2.png
 SpotifyPictureHelper/tests/test_all.py
```

### Comparing `SpotifyPictureHelper-0.1.0/pyproject.toml` & `SpotifyPictureHelper-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "SpotifyPictureHelper"
 authors = [{name = "Daisy Ye", email = "daisyye20010730@gmail.com"}]
 description="A python library that helps with the analysis of Spotify pictures."
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 requires-python = ">=3.7"
 
-dependencies = ['requests','bs4']
+dependencies = ['requests','bs4', 'numpy', 'opencv-python']
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

### Comparing `SpotifyPictureHelper-0.1.0/setup.cfg` & `SpotifyPictureHelper-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SpotifyPictureHelper
-version = v0.1.0
+version = v0.2.0
 author = Daisy ye
 author_email = daisyye20010730@gmail.com
 description = A python library that helps with the analysis of Spotify pictures.
 
 [options]
 zip_safe = False
 include_package_data = True
```

