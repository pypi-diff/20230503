# Comparing `tmp/OWR-2.0.tar.gz` & `tmp/OWR-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-2.0.tar", last modified: Wed May  3 10:44:20 2023, max compression
+gzip compressed data, was "OWR-2.1.tar", last modified: Wed May  3 12:27:44 2023, max compression
```

## Comparing `OWR-2.0.tar` & `OWR-2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 10:44:20.668119 OWR-2.0/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-2.0/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 10:44:20.668119 OWR-2.0/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6425 2023-05-03 10:42:04.000000 OWR-2.0/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 10:44:20.668119 OWR-2.0/OWR/data/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      420 2023-05-01 12:40:20.000000 OWR-2.0/OWR/data/obscenity_words.json
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 10:44:20.668119 OWR-2.0/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 10:44:20.000000 OWR-2.0/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-03 10:44:20.000000 OWR-2.0/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-03 10:44:20.000000 OWR-2.0/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-03 10:44:20.000000 OWR-2.0/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-03 10:44:20.000000 OWR-2.0/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 10:44:20.668119 OWR-2.0/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-2.0/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-03 10:44:20.668119 OWR-2.0/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      717 2023-05-03 10:44:16.000000 OWR-2.0/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 12:27:44.766664 OWR-2.1/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-2.1/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 12:27:44.766664 OWR-2.1/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6495 2023-05-03 12:27:18.000000 OWR-2.1/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 12:27:44.766664 OWR-2.1/OWR/data/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      420 2023-05-01 12:40:20.000000 OWR-2.1/OWR/data/obscenity_words.json
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 12:27:44.766664 OWR-2.1/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-03 12:27:44.000000 OWR-2.1/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 12:27:44.766664 OWR-2.1/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-2.1/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-03 12:27:44.766664 OWR-2.1/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      717 2023-05-03 12:27:30.000000 OWR-2.1/setup.py
```

### Comparing `OWR-2.0/LICENSE` & `OWR-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-2.0/OWR/__init__.py` & `OWR-2.1/OWR/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                 else:
                     samples[i[0]:i[1]] = np.tile((librosa.tone(600, length=i[1] - i[0], sr=16000)),
                                                  (samples.ndim, 1)).transpose()
 
     def __init__(self):
         self.ASR = SpeechRecognitionModel("rmgaliullin/wav2vec2-based-obscenity-detector", letter_case='lowercase')
         self.__phonetic_word_codes = self.__get_phonetic_for_words(os.path.split(inspect.getfile(self.__class__))[0]+'/data/obscenity_words.json')
+        logger.info("Initialization of the model has been completed")
 
     def mute_words(self, audio_path: str, mode: str):
         audio_file = sf.SoundFile(audio_path)
         origin_samples = audio_file.read()
         origin_sr = audio_file.samplerate
         logger.info(
             f"Audio is loaded with {origin_sr} sample rate, {audio_file.channels} channels, type {audio_file.subtype}")
```

### Comparing `OWR-2.0/setup.py` & `OWR-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='2.0',
+    version='2.1',
     description='Obscene word recognition package',
     url='https://github.com/VladVslv/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
     package_data={'': ['data/obscenity_words.json']},
```

