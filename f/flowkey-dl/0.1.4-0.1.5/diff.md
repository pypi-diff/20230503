# Comparing `tmp/flowkey_dl-0.1.4.tar.gz` & `tmp/flowkey_dl-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowkey_dl-0.1.4.tar", last modified: Mon Sep  5 09:18:12 2022, max compression
+gzip compressed data, was "flowkey_dl-0.1.5.tar", last modified: Wed May  3 15:04:58 2023, max compression
```

## Comparing `flowkey_dl-0.1.4.tar` & `flowkey_dl-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2022-09-05 09:18:12.415410 flowkey_dl-0.1.4/
--rw-rw----   0 lienhard  (2263) 42grp      (542)      310 2022-09-05 09:11:18.000000 flowkey_dl-0.1.4/CHANGELOG.md
--rw-rw----   0 lienhard  (2263) 42grp      (542)       66 2022-06-17 13:53:49.000000 flowkey_dl-0.1.4/MANIFEST.in
--rw-r-----   0 lienhard  (2263) 42grp      (542)     2222 2022-09-05 09:18:12.423410 flowkey_dl-0.1.4/PKG-INFO
--rwxr-x--x   0 lienhard  (2263) 42grp      (542)     1679 2022-06-17 15:12:09.000000 flowkey_dl-0.1.4/README.md
--rw-rw----   0 lienhard  (2263) 42grp      (542)        6 2022-09-05 09:09:05.000000 flowkey_dl-0.1.4/VERSION.txt
--rw-rw----   0 lienhard  (2263) 42grp      (542)      417 2022-06-17 14:03:17.000000 flowkey_dl-0.1.4/pyproject.toml
--rwxr-x--x   0 lienhard  (2263) 42grp      (542)       60 2022-06-17 13:34:26.000000 flowkey_dl-0.1.4/requirements.txt
--rw-rw----   0 lienhard  (2263) 42grp      (542)      981 2022-09-05 09:18:12.515410 flowkey_dl-0.1.4/setup.cfg
--rwxr-x--x   0 lienhard  (2263) 42grp      (542)       95 2022-06-17 14:04:40.000000 flowkey_dl-0.1.4/setup.py
-drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2022-09-05 09:18:11.142415 flowkey_dl-0.1.4/src/
-drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2022-09-05 09:18:11.973412 flowkey_dl-0.1.4/src/flowkey_dl/
--rwxr-x--x   0 lienhard  (2263) 42grp      (542)      471 2022-06-17 15:03:13.000000 flowkey_dl-0.1.4/src/flowkey_dl/__init__.py
--rwxrwx---   0 lienhard  (2263) 42grp      (542)     7275 2022-09-05 09:17:19.000000 flowkey_dl-0.1.4/src/flowkey_dl/flowkey_dl.py
--rw-r-----   0 lienhard  (2263) 42grp      (542)     1055 2022-09-05 08:46:42.000000 flowkey_dl-0.1.4/src/flowkey_dl/flowkey_dl_cli.py
--rwxr-x--x   0 lienhard  (2263) 42grp      (542)     9475 2022-09-05 09:07:58.000000 flowkey_dl-0.1.4/src/flowkey_dl/flowkey_dl_gui.py
-drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2022-09-05 09:18:12.374410 flowkey_dl-0.1.4/src/flowkey_dl.egg-info/
--rw-r-----   0 lienhard  (2263) 42grp      (542)     2222 2022-09-05 09:18:10.000000 flowkey_dl-0.1.4/src/flowkey_dl.egg-info/PKG-INFO
--rw-r-----   0 lienhard  (2263) 42grp      (542)      449 2022-09-05 09:18:11.000000 flowkey_dl-0.1.4/src/flowkey_dl.egg-info/SOURCES.txt
--rw-r-----   0 lienhard  (2263) 42grp      (542)        1 2022-09-05 09:18:10.000000 flowkey_dl-0.1.4/src/flowkey_dl.egg-info/dependency_links.txt
--rw-r-----   0 lienhard  (2263) 42grp      (542)      110 2022-09-05 09:18:10.000000 flowkey_dl-0.1.4/src/flowkey_dl.egg-info/entry_points.txt
--rw-r-----   0 lienhard  (2263) 42grp      (542)       60 2022-09-05 09:18:10.000000 flowkey_dl-0.1.4/src/flowkey_dl.egg-info/requires.txt
--rw-r-----   0 lienhard  (2263) 42grp      (542)       11 2022-09-05 09:18:11.000000 flowkey_dl-0.1.4/src/flowkey_dl.egg-info/top_level.txt
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-05-03 15:04:58.379023 flowkey_dl-0.1.5/
+-rw-rw----   0 lienhard  (2263) 42grp      (542)      400 2023-05-03 15:01:53.000000 flowkey_dl-0.1.5/CHANGELOG.md
+-rw-rw----   0 lienhard  (2263) 42grp      (542)       66 2022-06-17 13:53:49.000000 flowkey_dl-0.1.5/MANIFEST.in
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     2728 2023-05-03 15:04:58.388023 flowkey_dl-0.1.5/PKG-INFO
+-rwxr-x--x   0 lienhard  (2263) 42grp      (542)     2185 2023-05-03 14:41:21.000000 flowkey_dl-0.1.5/README.md
+-rw-rw----   0 lienhard  (2263) 42grp      (542)        6 2023-05-03 15:00:20.000000 flowkey_dl-0.1.5/VERSION.txt
+-rw-rw----   0 lienhard  (2263) 42grp      (542)      417 2022-06-17 14:03:17.000000 flowkey_dl-0.1.5/pyproject.toml
+-rwxr-x--x   0 lienhard  (2263) 42grp      (542)       60 2022-06-17 13:34:26.000000 flowkey_dl-0.1.5/requirements.txt
+-rw-rw----   0 lienhard  (2263) 42grp      (542)      981 2023-05-03 15:04:58.421023 flowkey_dl-0.1.5/setup.cfg
+-rwxr-x--x   0 lienhard  (2263) 42grp      (542)       95 2022-06-17 14:04:40.000000 flowkey_dl-0.1.5/setup.py
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-05-03 15:04:57.187027 flowkey_dl-0.1.5/src/
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-05-03 15:04:57.979024 flowkey_dl-0.1.5/src/flowkey_dl/
+-rwxr-x--x   0 lienhard  (2263) 42grp      (542)      471 2022-06-17 15:03:13.000000 flowkey_dl-0.1.5/src/flowkey_dl/__init__.py
+-rwxrwx---   0 lienhard  (2263) 42grp      (542)     7282 2023-05-03 15:04:37.000000 flowkey_dl-0.1.5/src/flowkey_dl/flowkey_dl.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     1055 2022-09-05 08:46:42.000000 flowkey_dl-0.1.5/src/flowkey_dl/flowkey_dl_cli.py
+-rwxr-x--x   0 lienhard  (2263) 42grp      (542)     9475 2022-09-05 09:07:58.000000 flowkey_dl-0.1.5/src/flowkey_dl/flowkey_dl_gui.py
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-05-03 15:04:58.330023 flowkey_dl-0.1.5/src/flowkey_dl.egg-info/
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     2728 2023-05-03 15:04:56.000000 flowkey_dl-0.1.5/src/flowkey_dl.egg-info/PKG-INFO
+-rw-r-----   0 lienhard  (2263) 42grp      (542)      449 2023-05-03 15:04:57.000000 flowkey_dl-0.1.5/src/flowkey_dl.egg-info/SOURCES.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)        1 2023-05-03 15:04:56.000000 flowkey_dl-0.1.5/src/flowkey_dl.egg-info/dependency_links.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)      110 2023-05-03 15:04:56.000000 flowkey_dl-0.1.5/src/flowkey_dl.egg-info/entry_points.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)       60 2023-05-03 15:04:56.000000 flowkey_dl-0.1.5/src/flowkey_dl.egg-info/requires.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)       11 2023-05-03 15:04:56.000000 flowkey_dl-0.1.5/src/flowkey_dl.egg-info/top_level.txt
```

### Comparing `flowkey_dl-0.1.4/PKG-INFO` & `flowkey_dl-0.1.5/src/flowkey_dl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flowkey_dl
-Version: 0.1.4
+Name: flowkey-dl
+Version: 0.1.5
 Summary: "A python app to download sheet music from flowkey and save it as pdf."
 Home-page: https://github.com/MatthiasLienhard/flowkey_dl
 Author: Matthias Lienhard
 Author-email: mali27048@gmail.com
 Project-URL: Bug Tracker, https://github.com/MatthiasLienhard/flowkey_dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -44,15 +44,18 @@
 In a terminal, run
 
 ```
 flowkey-dl
 
 ```
 
-Go to flowkey.com, select a song or lesson and right click on the sheet track at the bottom of the page. Select "Copy image adress" and paste this url (e.g. https://flowkeycdn.com/sheets/XXXX/150/0.png) into the url filed of the app. Click on "load" and the sheet is downloaded and aranged. If you enter title and author, it gets added to the sheet. Optionally adjust layout, scale and font size and select measures (e.g. 1,3,5-10 would select only measures 1, 3 and 5 to 10). Click save to save the sheet as pdf.
+~~Go to flowkey.com, select a song or lesson and right click on the sheet track at the bottom of the page.~~
+Flowkey made it harder to get the url of the underlying images, simply right click does not work anymore. It should still work when looking in the browsers cache. With google-chrome browser, you find it by clicking on the three dots in the top right -> more tools -> developer tools, then on the "sources" tab. Here you should find flowkeycdn.com with a folder /sheets, with all the songs from the last session. Click right on the first image (0.png) and then 'copy link location'. There is probably similar ways in other browsers.
+
+Paste this url (e.g. https://flowkeycdn.com/sheets/XXXX/300/0.png) into the url filed of the app. Click on "load" and the sheet is downloaded and aranged. If you enter title and author, it gets added to the sheet. Optionally adjust layout, scale and font size and select measures (e.g. 1,3,5-10 would select only measures 1, 3 and 5 to 10). Click save to save the sheet as pdf.
 
 If the font size does not change, you probably do not have the fonts installed. Try installing either FreeMono or arial as ttf.
 
 ### CLI:
 
 To start the command line interface run
```

#### html2text {}

```diff
@@ -1,30 +1,36 @@
-Metadata-Version: 2.1 Name: flowkey_dl Version: 0.1.4 Summary: "A python app to
+Metadata-Version: 2.1 Name: flowkey-dl Version: 0.1.5 Summary: "A python app to
 download sheet music from flowkey and save it as pdf." Home-page: https://
 github.com/MatthiasLienhard/flowkey_dl Author: Matthias Lienhard Author-email:
 mali27048@gmail.com Project-URL: Bug Tracker, https://github.com/
 MatthiasLienhard/flowkey_dl/issues Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown # flowkey_dl A python app to download sheet music from flowkey and
 save it as pdf. ## installation This is a python3 app, that can be installed
 with pip: ``` python3 -m pip install flowkey_dl ``` To get the latest dev
 version from git, clone the repository and install from the folder. ``` git
 clone https://github.com/MatthiasLienhard/flowkey_dl.git cd flowkey_dl python3
 -m pip install . ``` The gui of the app depends on tkinter which should be
 included with all standard Python distributions. If you get import errors, try
 installing it manually, e.g. in linux with ``` sudo apt-get install python3-tk
-``` ## usage: ### GUI: In a terminal, run ``` flowkey-dl ``` Go to flowkey.com,
-select a song or lesson and right click on the sheet track at the bottom of the
-page. Select "Copy image adress" and paste this url (e.g. https://
-flowkeycdn.com/sheets/XXXX/150/0.png) into the url filed of the app. Click on
-"load" and the sheet is downloaded and aranged. If you enter title and author,
-it gets added to the sheet. Optionally adjust layout, scale and font size and
-select measures (e.g. 1,3,5-10 would select only measures 1, 3 and 5 to 10).
-Click save to save the sheet as pdf. If the font size does not change, you
-probably do not have the fonts installed. Try installing either FreeMono or
-arial as ttf. ### CLI: To start the command line interface run ```bash flowkey-
-dl-cli  [] [-t
+``` ## usage: ### GUI: In a terminal, run ``` flowkey-dl ``` ~~Go to
+flowkey.com, select a song or lesson and right click on the sheet track at the
+bottom of the page.~~ Flowkey made it harder to get the url of the underlying
+images, simply right click does not work anymore. It should still work when
+looking in the browsers cache. With google-chrome browser, you find it by
+clicking on the three dots in the top right -> more tools -> developer tools,
+then on the "sources" tab. Here you should find flowkeycdn.com with a folder /
+sheets, with all the songs from the last session. Click right on the first
+image (0.png) and then 'copy link location'. There is probably similar ways in
+other browsers. Paste this url (e.g. https://flowkeycdn.com/sheets/XXXX/300/
+0.png) into the url filed of the app. Click on "load" and the sheet is
+downloaded and aranged. If you enter title and author, it gets added to the
+sheet. Optionally adjust layout, scale and font size and select measures (e.g.
+1,3,5-10 would select only measures 1, 3 and 5 to 10). Click save to save the
+sheet as pdf. If the font size does not change, you probably do not have the
+fonts installed. Try installing either FreeMono or arial as ttf. ### CLI: To
+start the command line interface run ```bash flowkey-dl-cli  [] [-t
 ] ``` This will download the sheet music for the provided flowkey url and
 export it in pdf format. The base url refers to the url from flowkey as
 described above (e.g. https://flowkeycdn.com/sheets/XXXX/<...>) and is
 required.
```

### Comparing `flowkey_dl-0.1.4/README.md` & `flowkey_dl-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,18 @@
 In a terminal, run
 
 ```
 flowkey-dl
 
 ```
 
-Go to flowkey.com, select a song or lesson and right click on the sheet track at the bottom of the page. Select "Copy image adress" and paste this url (e.g. https://flowkeycdn.com/sheets/XXXX/150/0.png) into the url filed of the app. Click on "load" and the sheet is downloaded and aranged. If you enter title and author, it gets added to the sheet. Optionally adjust layout, scale and font size and select measures (e.g. 1,3,5-10 would select only measures 1, 3 and 5 to 10). Click save to save the sheet as pdf.
+~~Go to flowkey.com, select a song or lesson and right click on the sheet track at the bottom of the page.~~
+Flowkey made it harder to get the url of the underlying images, simply right click does not work anymore. It should still work when looking in the browsers cache. With google-chrome browser, you find it by clicking on the three dots in the top right -> more tools -> developer tools, then on the "sources" tab. Here you should find flowkeycdn.com with a folder /sheets, with all the songs from the last session. Click right on the first image (0.png) and then 'copy link location'. There is probably similar ways in other browsers.
+
+Paste this url (e.g. https://flowkeycdn.com/sheets/XXXX/300/0.png) into the url filed of the app. Click on "load" and the sheet is downloaded and aranged. If you enter title and author, it gets added to the sheet. Optionally adjust layout, scale and font size and select measures (e.g. 1,3,5-10 would select only measures 1, 3 and 5 to 10). Click save to save the sheet as pdf.
 
 If the font size does not change, you probably do not have the fonts installed. Try installing either FreeMono or arial as ttf.
 
 ### CLI:
 
 To start the command line interface run
```

#### html2text {}

```diff
@@ -2,21 +2,28 @@
 pdf. ## installation This is a python3 app, that can be installed with pip: ```
 python3 -m pip install flowkey_dl ``` To get the latest dev version from git,
 clone the repository and install from the folder. ``` git clone https://
 github.com/MatthiasLienhard/flowkey_dl.git cd flowkey_dl python3 -m pip install
 . ``` The gui of the app depends on tkinter which should be included with all
 standard Python distributions. If you get import errors, try installing it
 manually, e.g. in linux with ``` sudo apt-get install python3-tk ``` ## usage:
-### GUI: In a terminal, run ``` flowkey-dl ``` Go to flowkey.com, select a song
-or lesson and right click on the sheet track at the bottom of the page. Select
-"Copy image adress" and paste this url (e.g. https://flowkeycdn.com/sheets/
-XXXX/150/0.png) into the url filed of the app. Click on "load" and the sheet is
-downloaded and aranged. If you enter title and author, it gets added to the
-sheet. Optionally adjust layout, scale and font size and select measures (e.g.
-1,3,5-10 would select only measures 1, 3 and 5 to 10). Click save to save the
-sheet as pdf. If the font size does not change, you probably do not have the
-fonts installed. Try installing either FreeMono or arial as ttf. ### CLI: To
-start the command line interface run ```bash flowkey-dl-cli  [] [-t
+### GUI: In a terminal, run ``` flowkey-dl ``` ~~Go to flowkey.com, select a
+song or lesson and right click on the sheet track at the bottom of the page.~~
+Flowkey made it harder to get the url of the underlying images, simply right
+click does not work anymore. It should still work when looking in the browsers
+cache. With google-chrome browser, you find it by clicking on the three dots in
+the top right -> more tools -> developer tools, then on the "sources" tab. Here
+you should find flowkeycdn.com with a folder /sheets, with all the songs from
+the last session. Click right on the first image (0.png) and then 'copy link
+location'. There is probably similar ways in other browsers. Paste this url
+(e.g. https://flowkeycdn.com/sheets/XXXX/300/0.png) into the url filed of the
+app. Click on "load" and the sheet is downloaded and aranged. If you enter
+title and author, it gets added to the sheet. Optionally adjust layout, scale
+and font size and select measures (e.g. 1,3,5-10 would select only measures 1,
+3 and 5 to 10). Click save to save the sheet as pdf. If the font size does not
+change, you probably do not have the fonts installed. Try installing either
+FreeMono or arial as ttf. ### CLI: To start the command line interface run
+```bash flowkey-dl-cli  [] [-t
 ] ``` This will download the sheet music for the provided flowkey url and
 export it in pdf format. The base url refers to the url from flowkey as
 described above (e.g. https://flowkeycdn.com/sheets/XXXX/<...>) and is
 required.
```

### Comparing `flowkey_dl-0.1.4/setup.cfg` & `flowkey_dl-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `flowkey_dl-0.1.4/src/flowkey_dl/flowkey_dl.py` & `flowkey_dl-0.1.5/src/flowkey_dl/flowkey_dl.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     imgs = list()
     i = 0
     while True:
         # im = imageio.imread(url.format(i))
         r = requests.get(url.format(i))
         if r.content[-6:-1] == b"Error":
             break
-        patch = next(iter(imageio.get_reader(r.content, ".png")))
+        patch = imageio.imread(r.content, format='png', pilmode="RGBA")
         print(f"loaded patch {i} with shape {patch.shape}")
         if len(patch.shape) == 3 and patch.shape[2] == 4:  # rgba
             imgs.append(255 - patch[:, :, 3])
         elif len(patch.shape) == 2:  # bw
             imgs.append(patch)
         else:
             print(f"patch {i} looks strange, " +
-                  "ignoring: {patch} \nshape: {patch.shape}")
+                  f"ignoring: {patch} \nshape: {patch.shape}")
         i += 1
     print(f"downloaded {len(imgs)} patches form {url}")
     # print([i.shape for i in imgs])
 
     return np.hstack(imgs), None, None
```

### Comparing `flowkey_dl-0.1.4/src/flowkey_dl/flowkey_dl_cli.py` & `flowkey_dl-0.1.5/src/flowkey_dl/flowkey_dl_cli.py`

 * *Files identical despite different names*

### Comparing `flowkey_dl-0.1.4/src/flowkey_dl/flowkey_dl_gui.py` & `flowkey_dl-0.1.5/src/flowkey_dl/flowkey_dl_gui.py`

 * *Files identical despite different names*

### Comparing `flowkey_dl-0.1.4/src/flowkey_dl.egg-info/PKG-INFO` & `flowkey_dl-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flowkey-dl
-Version: 0.1.4
+Name: flowkey_dl
+Version: 0.1.5
 Summary: "A python app to download sheet music from flowkey and save it as pdf."
 Home-page: https://github.com/MatthiasLienhard/flowkey_dl
 Author: Matthias Lienhard
 Author-email: mali27048@gmail.com
 Project-URL: Bug Tracker, https://github.com/MatthiasLienhard/flowkey_dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -44,15 +44,18 @@
 In a terminal, run
 
 ```
 flowkey-dl
 
 ```
 
-Go to flowkey.com, select a song or lesson and right click on the sheet track at the bottom of the page. Select "Copy image adress" and paste this url (e.g. https://flowkeycdn.com/sheets/XXXX/150/0.png) into the url filed of the app. Click on "load" and the sheet is downloaded and aranged. If you enter title and author, it gets added to the sheet. Optionally adjust layout, scale and font size and select measures (e.g. 1,3,5-10 would select only measures 1, 3 and 5 to 10). Click save to save the sheet as pdf.
+~~Go to flowkey.com, select a song or lesson and right click on the sheet track at the bottom of the page.~~
+Flowkey made it harder to get the url of the underlying images, simply right click does not work anymore. It should still work when looking in the browsers cache. With google-chrome browser, you find it by clicking on the three dots in the top right -> more tools -> developer tools, then on the "sources" tab. Here you should find flowkeycdn.com with a folder /sheets, with all the songs from the last session. Click right on the first image (0.png) and then 'copy link location'. There is probably similar ways in other browsers.
+
+Paste this url (e.g. https://flowkeycdn.com/sheets/XXXX/300/0.png) into the url filed of the app. Click on "load" and the sheet is downloaded and aranged. If you enter title and author, it gets added to the sheet. Optionally adjust layout, scale and font size and select measures (e.g. 1,3,5-10 would select only measures 1, 3 and 5 to 10). Click save to save the sheet as pdf.
 
 If the font size does not change, you probably do not have the fonts installed. Try installing either FreeMono or arial as ttf.
 
 ### CLI:
 
 To start the command line interface run
```

#### html2text {}

```diff
@@ -1,30 +1,36 @@
-Metadata-Version: 2.1 Name: flowkey-dl Version: 0.1.4 Summary: "A python app to
+Metadata-Version: 2.1 Name: flowkey_dl Version: 0.1.5 Summary: "A python app to
 download sheet music from flowkey and save it as pdf." Home-page: https://
 github.com/MatthiasLienhard/flowkey_dl Author: Matthias Lienhard Author-email:
 mali27048@gmail.com Project-URL: Bug Tracker, https://github.com/
 MatthiasLienhard/flowkey_dl/issues Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown # flowkey_dl A python app to download sheet music from flowkey and
 save it as pdf. ## installation This is a python3 app, that can be installed
 with pip: ``` python3 -m pip install flowkey_dl ``` To get the latest dev
 version from git, clone the repository and install from the folder. ``` git
 clone https://github.com/MatthiasLienhard/flowkey_dl.git cd flowkey_dl python3
 -m pip install . ``` The gui of the app depends on tkinter which should be
 included with all standard Python distributions. If you get import errors, try
 installing it manually, e.g. in linux with ``` sudo apt-get install python3-tk
-``` ## usage: ### GUI: In a terminal, run ``` flowkey-dl ``` Go to flowkey.com,
-select a song or lesson and right click on the sheet track at the bottom of the
-page. Select "Copy image adress" and paste this url (e.g. https://
-flowkeycdn.com/sheets/XXXX/150/0.png) into the url filed of the app. Click on
-"load" and the sheet is downloaded and aranged. If you enter title and author,
-it gets added to the sheet. Optionally adjust layout, scale and font size and
-select measures (e.g. 1,3,5-10 would select only measures 1, 3 and 5 to 10).
-Click save to save the sheet as pdf. If the font size does not change, you
-probably do not have the fonts installed. Try installing either FreeMono or
-arial as ttf. ### CLI: To start the command line interface run ```bash flowkey-
-dl-cli  [] [-t
+``` ## usage: ### GUI: In a terminal, run ``` flowkey-dl ``` ~~Go to
+flowkey.com, select a song or lesson and right click on the sheet track at the
+bottom of the page.~~ Flowkey made it harder to get the url of the underlying
+images, simply right click does not work anymore. It should still work when
+looking in the browsers cache. With google-chrome browser, you find it by
+clicking on the three dots in the top right -> more tools -> developer tools,
+then on the "sources" tab. Here you should find flowkeycdn.com with a folder /
+sheets, with all the songs from the last session. Click right on the first
+image (0.png) and then 'copy link location'. There is probably similar ways in
+other browsers. Paste this url (e.g. https://flowkeycdn.com/sheets/XXXX/300/
+0.png) into the url filed of the app. Click on "load" and the sheet is
+downloaded and aranged. If you enter title and author, it gets added to the
+sheet. Optionally adjust layout, scale and font size and select measures (e.g.
+1,3,5-10 would select only measures 1, 3 and 5 to 10). Click save to save the
+sheet as pdf. If the font size does not change, you probably do not have the
+fonts installed. Try installing either FreeMono or arial as ttf. ### CLI: To
+start the command line interface run ```bash flowkey-dl-cli  [] [-t
 ] ``` This will download the sheet music for the provided flowkey url and
 export it in pdf format. The base url refers to the url from flowkey as
 described above (e.g. https://flowkeycdn.com/sheets/XXXX/<...>) and is
 required.
```

