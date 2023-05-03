# Comparing `tmp/autosrt-1.2.4.tar.gz` & `tmp/autosrt-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.2.4.tar", last modified: Sun Apr 30 23:47:31 2023, max compression
+gzip compressed data, was "autosrt-1.2.8.tar", last modified: Tue May  2 12:00:43 2023, max compression
```

## Comparing `autosrt-1.2.4.tar` & `autosrt-1.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 23:47:31.335685 autosrt-1.2.4/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.2.4/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-04-30 23:47:31.335685 autosrt-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 23:47:31.294480 autosrt-1.2.4/autosrt/
--rw-rw-rw-   0        0        0     9271 2023-04-30 23:38:40.000000 autosrt-1.2.4/autosrt/__init__.py
--rw-rw-rw-   0        0        0    32560 2023-04-30 13:27:29.000000 autosrt-1.2.4/autosrt/autosrt.py
-drwxrwxrwx   0        0        0        0 2023-04-30 23:47:31.310961 autosrt-1.2.4/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      137 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 23:47:30.000000 autosrt-1.2.4/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-30 23:47:31.337934 autosrt-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1583 2023-04-30 23:38:55.000000 autosrt-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 23:47:31.334189 autosrt-1.2.4/test/
--rw-rw-rw-   0        0        0     6874 2023-04-30 02:05:08.000000 autosrt-1.2.4/test/test1.py
--rw-rw-rw-   0        0        0     4087 2023-04-30 02:05:48.000000 autosrt-1.2.4/test/test2.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.670415 autosrt-1.2.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1087 2023-01-06 18:50:17.000000 autosrt-1.2.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-01-06 18:50:17.000000 autosrt-1.2.8/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 12:00:43.671018 autosrt-1.2.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5260 2023-04-30 04:22:31.000000 autosrt-1.2.8/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.662201 autosrt-1.2.8/autosrt/
+-rwxrwxrwx   0 root         (0) root         (0)     9271 2023-05-02 11:58:44.000000 autosrt-1.2.8/autosrt/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    33439 2023-05-02 10:41:14.000000 autosrt-1.2.8/autosrt/autosrt.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.667758 autosrt-1.2.8/autosrt.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1987 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      112 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-05-02 12:00:43.000000 autosrt-1.2.8/autosrt.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      136 2023-05-02 12:00:43.672433 autosrt-1.2.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1695 2023-05-02 12:00:07.000000 autosrt-1.2.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 12:00:43.669526 autosrt-1.2.8/test/
+-rwxrwxrwx   0 root         (0) root         (0)     6874 2023-04-30 02:05:08.000000 autosrt-1.2.8/test/test1.py
+-rwxrwxrwx   0 root         (0) root         (0)     4087 2023-04-30 02:05:48.000000 autosrt-1.2.8/test/test2.py
```

### Comparing `autosrt-1.2.4/LICENSE` & `autosrt-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.4/PKG-INFO` & `autosrt-1.2.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: autosrt
-Version: 1.2.4
-Summary: a utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: autosrt
+Version: 1.2.8
+Summary: a utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.2.4/README.md` & `autosrt-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.4/autosrt/__init__.py` & `autosrt-1.2.8/autosrt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in video/audio source_path", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired translation language code for the subtitles", default=None)
     parser.add_argument('-ll', '--list-languages', help="List all supported languages", action='store_true')
     parser.add_argument('-o', '--output', help="Output file path for subtitles (by default, subtitles are saved in the same directory and named with the source_path base name)")
     parser.add_argument('-F', '--format', help="Desired subtitle format", default="srt")
     parser.add_argument('-lf', '--list-formats', help="List all supported subtitle formats", action='store_true')
     parser.add_argument('-C', '--concurrency', help="Number of concurrent API requests to make", type=int, default=10)
-    parser.add_argument('-v', '--version', action='version', version='1.2.4')
+    parser.add_argument('-v', '--version', action='version', version='1.2.8')
 
     args = parser.parse_args()
 
     language = Language()
 
     if args.list_languages:
         print("List of supported languages:")
```

### Comparing `autosrt-1.2.4/autosrt/autosrt.py` & `autosrt-1.2.8/autosrt/autosrt.py`

 * *Files 2% similar despite different names*

```diff
@@ -666,89 +666,69 @@
 
         except Exception as e:
             print(e)
             return
 
 
 class SpeechRecognizer(object):
-    def __init__(self, language="en", rate=44100, retries=3, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw"):
+    def __init__(self, language="en", rate=44100, retries=3, api_key="AIzaSyBOti4mM-6x9WDnZIjIeyEU21OpBXqWBgw", timeout=30):
         self.language = language
         self.rate = rate
         self.api_key = api_key
         self.retries = retries
+        self.timeout = timeout
 
     def __call__(self, data):
         try:
             for i in range(self.retries):
                 url = "http://www.google.com/speech-api/v2/recognize?client=chromium&lang={lang}&key={key}".format(lang=self.language, key=self.api_key)
-                headers = {"Content-Type": "audio/x-flac; rate=%d" % self.rate}
+                headers = {"Content-Type": "audio/x-flac rate=%d" % self.rate}
 
                 try:
-                    resp = requests.post(url, data=data, headers=headers)
+                    resp = requests.post(url, data=data, headers=headers, timeout=self.timeout)
                 except requests.exceptions.ConnectionError:
-                    continue
+                    try:
+                        resp = httpx.post(url, data=data, headers=headers, timeout=self.timeout)
+                    except httpx.exceptions.NetworkError:
+                        continue
 
                 for line in resp.content.decode('utf-8').split("\n"):
                     try:
                         line = json.loads(line)
                         line = line['result'][0]['alternative'][0]['transcript']
                         return line[:1].upper() + line[1:]
                     except:
                         # no result
                         continue
 
         except KeyboardInterrupt:
-            print("Cancelling transcription")
             return
 
         except Exception as e:
             print(e)
             return
 
 
 class SentenceTranslator(object):
-    @staticmethod
-    def GoogleTranslate(text, src, dst):
-        url = 'https://translate.googleapis.com/translate_a/'
-        params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
-        headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',}
-        try:
-            response = requests.get(url+params, headers=headers)
-            if response.status_code == 200:
-                response_json = response.json()[0]
-                length = len(response_json)
-                translation = ""
-                for i in range(length):
-                    translation = translation + response_json[i][0]
-                return translation
-            return
-
-        except KeyboardInterrupt:
-            print("Cancelling transcription")
-            return
-
-        except Exception as e:
-            print(e)
-            return
-
-    def __init__(self, src, dst, patience=-1):
+    def __init__(self, src, dst, patience=-1, timeout=30):
         self.src = src
         self.dst = dst
         self.patience = patience
+        self.timeout = timeout
 
     def __call__(self, sentence):
         try:
             translated_sentence = []
             # handle the special case: empty string.
             if not sentence:
                 return None
-            translated_sentence = self.GoogleTranslate(sentence, src=self.src, dst=self.dst)
+            translated_sentence = self.GoogleTranslate(sentence, src=self.src, dst=self.dst, timeout=self.timeout)
             fail_to_translate = translated_sentence[-1] == '\n'
             while fail_to_translate and patience:
-                translated_sentence = self.GoogleTranslate(translated_sentence, src=self.src, dst=self.dst).text
+                translated_sentence = self.GoogleTranslate(translated_sentence, src=self.src, dst=self.dst, timeout=self.timeout).text
                 if translated_sentence[-1] == '\n':
                     if patience == -1:
                         continue
                     patience -= 1
                 else:
                     fail_to_translate = False
 
@@ -756,14 +736,50 @@
 
         except KeyboardInterrupt:
             print("Cancelling transcription")
             return
 
         except Exception as e:
             print(e)
+            return
+
+    def GoogleTranslate(self, text, src, dst, timeout=30):
+        url = 'https://translate.googleapis.com/translate_a/'
+        params = 'single?client=gtx&sl='+src+'&tl='+dst+'&dt=t&q='+text;
+        headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)', 'Referer': 'https://translate.google.com',}
+
+        try:
+            response = requests.get(url+params, headers=headers, timeout=self.timeout)
+            if response.status_code == 200:
+                response_json = response.json()[0]
+                length = len(response_json)
+                translation = ""
+                for i in range(length):
+                    translation = translation + response_json[i][0]
+                return translation
+            return
+
+        except requests.exceptions.ConnectionError:
+            with httpx.Client() as client:
+                response = client.get(url+params, headers=headers, timeout=self.timeout)
+                if response.status_code == 200:
+                    response_json = response.json()[0]
+                    length = len(response_json)
+                    translation = ""
+                    for i in range(length):
+                        translation = translation + response_json[i][0]
+                    return translation
+                return
+
+        except KeyboardInterrupt:
+            print("Cancelling transcription")
+            return
+
+        except Exception as e:
+            print(e)
             return
 
 
 class SubtitleFormatter:
     supported_formats = ['srt', 'vtt', 'json', 'raw']
 
     def __init__(self, format_type):
```

### Comparing `autosrt-1.2.4/autosrt.egg-info/PKG-INFO` & `autosrt-1.2.8/autosrt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: autosrt
-Version: 1.2.4
-Summary: a utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: autosrt
+Version: 1.2.8
+Summary: a utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.2.4/test/test1.py` & `autosrt-1.2.8/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.4/test/test2.py` & `autosrt-1.2.8/test/test2.py`

 * *Files identical despite different names*

