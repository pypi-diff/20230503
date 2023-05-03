# Comparing `tmp/OWR-2.1.tar.gz` & `tmp/OWR-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-2.1.tar", last modified: Wed May  3 12:27:44 2023, max compression
+gzip compressed data, was "OWR-2.2.tar", last modified: Wed May  3 16:40:23 2023, max compression
```

## Comparing `OWR-2.1.tar` & `OWR-2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 12:27:44.766664 OWR-2.1/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-2.1/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 12:27:44.766664 OWR-2.1/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6495 2023-05-03 12:27:18.000000 OWR-2.1/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 12:27:44.766664 OWR-2.1/OWR/data/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      420 2023-05-01 12:40:20.000000 OWR-2.1/OWR/data/obscenity_words.json
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 12:27:44.766664 OWR-2.1/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 12:27:44.766664 OWR-2.1/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-2.1/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-03 12:27:44.766664 OWR-2.1/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      717 2023-05-03 12:27:30.000000 OWR-2.1/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 16:40:23.299534 OWR-2.2/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-2.2/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 16:40:23.299534 OWR-2.2/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6921 2023-05-03 16:39:31.000000 OWR-2.2/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 16:40:23.299534 OWR-2.2/OWR/data/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      420 2023-05-01 12:40:20.000000 OWR-2.2/OWR/data/obscenity_words.json
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 16:40:23.299534 OWR-2.2/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 16:40:23.000000 OWR-2.2/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-03 16:40:23.000000 OWR-2.2/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-03 16:40:23.000000 OWR-2.2/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-03 16:40:23.000000 OWR-2.2/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-03 16:40:23.000000 OWR-2.2/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 16:40:23.299534 OWR-2.2/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-2.2/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-03 16:40:23.299534 OWR-2.2/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      717 2023-05-03 16:40:07.000000 OWR-2.2/setup.py
```

### Comparing `OWR-2.1/LICENSE` & `OWR-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-2.1/OWR/__init__.py` & `OWR-2.2/OWR/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,16 @@
                     samples[i[0]:i[1]] = librosa.tone(600, length=i[1] - i[0], sr=16000)
                 else:
                     samples[i[0]:i[1]] = np.tile((librosa.tone(600, length=i[1] - i[0], sr=16000)),
                                                  (samples.ndim, 1)).transpose()
 
     def __init__(self):
         self.ASR = SpeechRecognitionModel("rmgaliullin/wav2vec2-based-obscenity-detector", letter_case='lowercase')
-        self.__phonetic_word_codes = self.__get_phonetic_for_words(os.path.split(inspect.getfile(self.__class__))[0]+'/data/obscenity_words.json')
+        self.__phonetic_word_codes = self.__get_phonetic_for_words(
+            os.path.split(inspect.getfile(self.__class__))[0] + '/data/obscenity_words.json')
         logger.info("Initialization of the model has been completed")
 
     def mute_words(self, audio_path: str, mode: str):
         audio_file = sf.SoundFile(audio_path)
         origin_samples = audio_file.read()
         origin_sr = audio_file.samplerate
         logger.info(
@@ -129,20 +130,30 @@
             is_valid = True
             for w in recognized_ow_indexes:
                 if not ((word[0] < w[0] and word[1] < w[0]) or (w[0] < word[0] and w[1] < word[0])):
                     is_valid = False
             if is_valid:
                 logger.info(f"Detected word: {sentence[word[0]:(word[1] + 1)]};  Probability: {p}")
                 recognized_ow_indexes.append(word)
-                ow_timestamps.append(
-                    (start_timestamps[word[0]] * (sample_rate // 1000) - (sample_rate // 1000),
-                     end_timestamps[word[1]] * (sample_rate // 1000) + (sample_rate // 1000)))
+                length = word[1] - word[0] + 1
+                start = start_timestamps[word[0]] * (sample_rate // 1000)
+                end = end_timestamps[word[1]] * (sample_rate // 1000)
+                letter_len = (end - start) // length
+                start -= 2 * letter_len
+                end += 2 * letter_len 
+                if start < 0:
+                    start = 0
+                if end > end_timestamps[-1] * (sample_rate // 1000):
+                    end = end_timestamps[-1] * (sample_rate // 1000)
+                ow_timestamps.append((start, end))
         return ow_timestamps
 
 
 if __name__ == "__main__":
     detector = ObscenityWordsRecognizer()
-    dir_path = os.path.join(os.getcwd(), "data", "audio")
-    file_name = "audio_03.wav"
+    dir_path = os.path.join(os.getcwd(), "data")
+    file_name = "AgADuykAAiQEkUoSL96illlSfCB5zPvoice.wav"
+    playsound(os.path.join(dir_path, file_name))
     a = detector.mute_words(os.path.join(dir_path, file_name), "b")
     print(a)
     playsound(os.path.join(dir_path, "result_" + file_name))
+
```

### Comparing `OWR-2.1/setup.py` & `OWR-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='2.1',
+    version='2.2',
     description='Obscene word recognition package',
     url='https://github.com/VladVslv/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
     package_data={'': ['data/obscenity_words.json']},
```

