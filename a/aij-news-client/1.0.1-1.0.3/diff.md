# Comparing `tmp/aij-news-client-1.0.1.tar.gz` & `tmp/aij-news-client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-news-client-1.0.1.tar", last modified: Tue May  2 23:25:40 2023, max compression
+gzip compressed data, was "aij-news-client-1.0.3.tar", last modified: Tue May  2 23:31:25 2023, max compression
```

## Comparing `aij-news-client-1.0.1.tar` & `aij-news-client-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-client-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4302 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-client-1.0.1/README.md
--rw-rw-rw-   0        0        0     6292 2023-05-02 23:25:28.000000 aij-news-client-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/src/aij_news_client.egg-info/
--rw-rw-rw-   0        0        0     4302 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/src/aij_news_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/src/aij_news_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/src/aij_news_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/src/aij_news_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      130 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/src/aij_news_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/src/aij_news_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 23:25:42.000000 aij-news-client-1.0.1/src/news_client/
--rw-rw-rw-   0        0        0     6506 2023-05-02 23:24:38.000000 aij-news-client-1.0.1/src/news_client/__init__.py
--rw-rw-rw-   0        0        0      832 2023-05-02 22:32:04.000000 aij-news-client-1.0.1/src/news_client/news_consumer.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-client-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-client-1.0.3/README.md
+-rw-rw-rw-   0        0        0     6292 2023-05-02 23:31:14.000000 aij-news-client-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/src/aij_news_client.egg-info/
+-rw-rw-rw-   0        0        0     4302 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/src/aij_news_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/src/aij_news_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/src/aij_news_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/src/aij_news_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/src/aij_news_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/src/aij_news_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 23:31:26.000000 aij-news-client-1.0.3/src/news_client/
+-rw-rw-rw-   0        0        0     6373 2023-05-02 23:30:08.000000 aij-news-client-1.0.3/src/news_client/__init__.py
+-rw-rw-rw-   0        0        0      832 2023-05-02 22:32:04.000000 aij-news-client-1.0.3/src/news_client/news_consumer.py
```

### Comparing `aij-news-client-1.0.1/LICENSE.txt` & `aij-news-client-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-news-client-1.0.1/PKG-INFO` & `aij-news-client-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-client
-Version: 1.0.1
+Version: 1.0.3
 Summary: AI Journalist News Client package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-client-1.0.1/README.md` & `aij-news-client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aij-news-client-1.0.1/pyproject.toml` & `aij-news-client-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-news-client"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.1"
+version = "1.0.3"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist News Client package"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -140,15 +140,15 @@
 "Funding" = "https://donate.pypi.org"
 "Say Thanks!" = "http://saythanks.io/to/aij"
 "Source" = "https://github.com/codesapienbe/aij-news-client"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
-aijnp = "news_client:main"
+aijnc = "news_client:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = { "db" = ["*.dat"] }
```

### Comparing `aij-news-client-1.0.1/src/aij_news_client.egg-info/PKG-INFO` & `aij-news-client-1.0.3/src/aij_news_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-client
-Version: 1.0.1
+Version: 1.0.3
 Summary: AI Journalist News Client package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-client-1.0.1/src/news_client/__init__.py` & `aij-news-client-1.0.3/src/news_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from news_client.console_client import NewsConsumer
 import cv2
 import mediapipe as mp
 import screeninfo
 import time
 
 articles = []
-headings = []
+headings = None
 
 def callback(self, ch, method, properties, body):
     """
     This method prints the articles.
     """
 
     _response = body.decode('utf-8')
@@ -22,15 +22,15 @@
         f"=============================\n"
     )
 
     # self.temp_data.append(_response)
     articles.append(_response)
     _response = _response.split(" ")
     _headings = _response[0]
-    headings.append(_headings)
+    headings += _headings
 
 
 def main():
     """
     The main function to run the server and publish the news articles to the RabbitMQ queue
     """
     consumer = NewsConsumer(os.environ['AIJ_NEWS_PUBLISHER_HOST'] or 'localhost', callback)
@@ -103,15 +103,15 @@
             cv2.rectangle(image, (0, image.shape[0] - box_height), (image.shape[1], image.shape[0]), (255, 255, 255), 2)
 
             if results.multi_hand_landmarks:
                 for hand_landmarks in results.multi_hand_landmarks:
 
                     # if left hand is raised then move the text to the left
                     if hand_landmarks.landmark[mp_hands.HandLandmark.WRIST].x < 0.2 and len(results.multi_hand_landmarks) == 1:
-                        self.temp_data.titles = self.temp_data.titles[1:] + self.temp_data.titles[0]
+                        headings = headings[1:] + headings[0]
                         direction = 0
                         font_size = 12
                         color = standard_text_color
                         box_height = 50
 
                     # if right hand is raised then move the text to the right
                     elif hand_landmarks.landmark[mp_hands.HandLandmark.WRIST].x > 0.8 and len(results.multi_hand_landmarks) == 1:
@@ -129,20 +129,20 @@
             else:
                 # if no hands are detected then move the text to the left
                 font_size = 12
                 color = standard_text_color
                 box_height = 50
 
             if direction == 0:
-                self.temp_data.titles = self.temp_data.titles[1:] + self.temp_data.titles[0]
+                headings = headings[1:] + headings[0]
             elif direction == 1:
-                self.temp_data.titles = self.temp_data.titles[-1] + self.temp_data.titles[:-1]
+                headings = headings[-1] + headings[:-1]
 
             # draw the text in the bottom left corner with a 2px border in black color. Get the font size from the variable font_size
-            cv2.putText(image, self.temp_data.titles, (10, image.shape[0] - 10), cv2.FONT_HERSHEY_SIMPLEX, font_size / 12, color, 2, cv2.LINE_AA)
+            cv2.putText(image, headings, (10, image.shape[0] - 10), cv2.FONT_HERSHEY_SIMPLEX, font_size / 12, color, 2, cv2.LINE_AA)
 
             # draw another text at the right top corner to show the current time of the day in 24h format (HH:MM:SS) and in white color with a 1px border in black color. Change to font-size to 14pt with bold style
             cv2.putText(image, datetime.datetime.now().strftime("%H:%M:%S"), (image.shape[1] - 100, 20), cv2.FONT_HERSHEY_SIMPLEX, 1, (255, 255, 255), 2, cv2.LINE_AA)
 
             # put a logo in the top left corner
             logo = cv2.imread('news/logo.png')
```

### Comparing `aij-news-client-1.0.1/src/news_client/news_consumer.py` & `aij-news-client-1.0.3/src/news_client/news_consumer.py`

 * *Files identical despite different names*

