# Comparing `tmp/lexikos-0.0.1b0.tar.gz` & `tmp/lexikos-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikos-0.0.1b0.tar", last modified: Fri Apr 21 13:38:28 2023, max compression
+gzip compressed data, was "lexikos-0.0.1rc0.tar", last modified: Wed May  3 04:15:15 2023, max compression
```

## Comparing `lexikos-0.0.1b0.tar` & `lexikos-0.0.1rc0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-04-21 13:38:28.926989 lexikos-0.0.1b0/
--rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1b0/LICENSE
--rw-r--r--   0 mac        (502) staff       (20)       16 2023-04-21 13:04:42.000000 lexikos-0.0.1b0/MANIFEST.in
--rw-r--r--   0 mac        (502) staff       (20)    24399 2023-04-21 13:38:28.927230 lexikos-0.0.1b0/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)    10676 2023-04-21 13:37:48.000000 lexikos-0.0.1b0/README.md
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-04-21 13:38:28.911099 lexikos-0.0.1b0/lexikos/
--rw-r--r--   0 mac        (502) staff       (20)       75 2023-04-21 13:37:16.000000 lexikos-0.0.1b0/lexikos/__init__.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-04-21 13:38:28.908610 lexikos-0.0.1b0/lexikos/dict/
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-04-21 13:38:28.912755 lexikos-0.0.1b0/lexikos/dict/cmudict-ipa/
--rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1b0/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-04-21 13:38:28.926633 lexikos-0.0.1b0/lexikos/dict/wikipron/
--rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_au_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_us_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)     2172 2023-04-21 13:36:22.000000 lexikos-0.0.1b0/lexikos/lexicon.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-04-21 13:38:28.912414 lexikos-0.0.1b0/lexikos.egg-info/
--rw-r--r--   0 mac        (502) staff       (20)    24399 2023-04-21 13:38:28.000000 lexikos-0.0.1b0/lexikos.egg-info/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)      584 2023-04-21 13:38:28.000000 lexikos-0.0.1b0/lexikos.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (502) staff       (20)        1 2023-04-21 13:38:28.000000 lexikos-0.0.1b0/lexikos.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (502) staff       (20)        8 2023-04-21 13:38:28.000000 lexikos-0.0.1b0/lexikos.egg-info/top_level.txt
--rw-r--r--   0 mac        (502) staff       (20)      819 2023-04-21 13:37:22.000000 lexikos-0.0.1b0/pyproject.toml
--rw-r--r--   0 mac        (502) staff       (20)      113 2023-04-21 13:38:28.927902 lexikos-0.0.1b0/setup.cfg
--rw-r--r--   0 mac        (502) staff       (20)      964 2023-04-21 13:31:07.000000 lexikos-0.0.1b0/setup.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.481010 lexikos-0.0.1rc0/
+-rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc0/LICENSE
+-rw-r--r--   0 mac        (502) staff       (20)       16 2023-04-21 13:04:42.000000 lexikos-0.0.1rc0/MANIFEST.in
+-rw-r--r--   0 mac        (502) staff       (20)    26127 2023-05-03 04:15:15.481446 lexikos-0.0.1rc0/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)    12403 2023-05-03 04:06:40.000000 lexikos-0.0.1rc0/README.md
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.425787 lexikos-0.0.1rc0/lexikos/
+-rw-r--r--   0 mac        (502) staff       (20)       75 2023-05-03 04:09:34.000000 lexikos-0.0.1rc0/lexikos/__init__.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.423361 lexikos-0.0.1rc0/lexikos/dict/
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.428685 lexikos-0.0.1rc0/lexikos/dict/cmudict-ipa/
+-rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc0/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.479429 lexikos-0.0.1rc0/lexikos/dict/wikipron/
+-rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_au_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_in_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_us_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     2172 2023-05-03 04:02:24.000000 lexikos-0.0.1rc0/lexikos/lexicon.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.428199 lexikos-0.0.1rc0/lexikos.egg-info/
+-rw-r--r--   0 mac        (502) staff       (20)    26127 2023-05-03 04:15:15.000000 lexikos-0.0.1rc0/lexikos.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)      851 2023-05-03 04:15:15.000000 lexikos-0.0.1rc0/lexikos.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (502) staff       (20)        1 2023-05-03 04:15:15.000000 lexikos-0.0.1rc0/lexikos.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (502) staff       (20)        8 2023-05-03 04:15:15.000000 lexikos-0.0.1rc0/lexikos.egg-info/top_level.txt
+-rw-r--r--   0 mac        (502) staff       (20)      819 2023-05-03 04:09:32.000000 lexikos-0.0.1rc0/pyproject.toml
+-rw-r--r--   0 mac        (502) staff       (20)      113 2023-05-03 04:15:15.482369 lexikos-0.0.1rc0/setup.cfg
+-rw-r--r--   0 mac        (502) staff       (20)      964 2023-04-21 13:31:07.000000 lexikos-0.0.1rc0/setup.py
```

### Comparing `lexikos-0.0.1b0/LICENSE` & `lexikos-0.0.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/PKG-INFO` & `lexikos-0.0.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1b0
+Version: 0.0.1rc0
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -221,25 +221,40 @@
 
 A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 
 <p align="center">
     <img src="https://github.com/bookbot-hive/lexikos/raw/main/assets/lexikos.png" alt="logo" width="300"/>
 </p>
 
+## Install Lexikos
+
+Install from PyPI
+
+```sh
+pip install lexikos
+```
+
+Editable install from Source
+
+```sh
+git clone https://github.com/bookbot-hive/lexikos.git
+pip install -e lexikos
+```
+
 ## Usage
 
 ```py
 >>> from lexikos import Lexicon
 >>> lexicon = Lexicon()
 >>> print(lexicon["added"])
-{'ˈæ d ə d', 'a d ɪ d', 'æ d ɪ d', 'a d ə d', 'æ ɾ ə d', 'ˈa d ə d', 'æ d ə d', 'ˈæ d ɪ d', 'ˈa d ɪ d', 'ˈæ ɾ ɪ d', 'æ ɾ ɪ d', 'ˈæ ɾ ə d'}
+{'ˈæ ɾ ɪ d', 'æ ɾ ɪ d', 'ˈæ d ɪ d', 'a d ɪ d', 'a d ə d', 'ˈæ ɾ ə d', 'ˈæ d ə d', 'æ d ɪ d', 'æ ɾ ə d', 'æ d ə d', 'ˈa d ɪ d', 'ˈa d ə d'}
 >>> print(lexicon["runner"])
-{'ɹ ʌ n ɚ', 'ˈr ʌ n ɝ', 'ɹ ʌ n ə'}
+{'ɹ ʌ n ə', 'ɹ ʌ n ɚ', 'ˈr ʌ n ɝ'}
 >>> print(lexicon["water"])
-{'w ɑ ɾ ɚ', 'ˈw oː t ə', 'w ɑ t ə ɹ', 'w ɔ ɾ ɚ', 'ˈw oː ɾ ə', 'w ɔː t ə', 'ˈw ɔ t ɝ', 'w ɔ t ə ɹ'}
+{'ˈw oː t ə', 'w ɔ t ə ɹ', 'ˈw ɑ t ə ɹ', 'w ɑ ɾ ɚ', 'ˈw ɔ t ɝ', 'ˈw ɑ ɾ ɚ', 'ˈʋ ɔ ʈ ə r', 'ˈʋ aː ʈ ə r ɯ', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ', 'ˈw aː ʈ ə r ɯ', 'ˈw ɔ ʈ ə r', 'ˈw oː ɾ ə', 'w ɔː t ə'}
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
 | Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
@@ -267,14 +282,36 @@
 ### English `(en-AU)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
 | -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
 | en-AU (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
 | en-AU (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
 
+### English `(en-CA)`
+
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
+| en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  |           |
+| en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |           |
+
+### English `(en-NZ)`
+
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
+| en-NZ (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_broad.tsv)  |           |
+| en-NZ (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_narrow.tsv) |           |
+
+### English `(en-IN)`
+
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
+| en-IN (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_broad.tsv)  |           |
+| en-IN (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_narrow.tsv) |           |
+
+
 ## Training G2P Model
 
 We modified the sequence-to-sequence training script of [🤗 HuggingFace](https://github.com/huggingface/transformers/blob/main/examples/pytorch/translation/run_translation.py) for the purpose of training G2P models. Refer to their [installation requirements](https://github.com/huggingface/transformers/tree/main/examples/pytorch/translation) for more details.
 
 Training a new G2P model generally follow this recipe:
 
 ```diff
@@ -368,19 +405,19 @@
 | Language Family        | Code                              | Region                                                | Corpus | G2P Model |
 | ---------------------- | --------------------------------- | ----------------------------------------------------- | :----: | :-------: |
 | African English        | en-ZA                             | South Africa                                          |        |           |
 | Australian English     | en-AU                             | Australia                                             |   ✅    |     ✅     |
 | East Asian English     | en-CN, en-HK, en-JP, en-KR, en-TW | China, Hong Kong, Japan, South Korea, Taiwan          |        |           |
 | European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |        |           |
 | Mexican English        | en-MX                             | Mexico                                                |        |           |
-| New Zealand English    | en-NZ                             | New Zealand                                           |        |           |
-| North American         | en-CA, en-US                      | Canada, United States                                 |        |           |
+| New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |           |
+| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |           |
 | Middle Eastern English | en-EG, en-IL                      | Egypt, Israel                                         |        |           |
 | Southeast Asian        | en-TH, en-ID, en-MY, en-PH, en-SG | Thailand, Indonesia, Malaysia, Philippines, Singapore |        |           |
-| South Asian English    | en-IN                             | India                                                 |        |           |
+| South Asian English    | en-IN                             | India                                                 |   ✅    |           |
   
 ## Resources
 
 - [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P)
 - [Microsoft CNTK](https://github.com/microsoft/CNTK/tree/master)
 - [CMU Pronouncing Dictionary - IPA](https://github.com/menelik3/cmudict-ipa)
 - [Wikipron](https://github.com/CUNY-CL/wikipron/tree/master)
@@ -403,15 +440,15 @@
     publisher = "European Language Resources Association",
     pages = "4223--4228",
 }
 ```
 
 ```bibtex
 @misc{zhu2022byt5,
-      title={ByT5 model for massively multilingual grapheme-to-phoneme conversion}, 
-      author={Jian Zhu and Cong Zhang and David Jurgens},
-      year={2022},
-      eprint={2204.03067},
-      archivePrefix={arXiv},
-      primaryClass={cs.CL}
+    title={ByT5 model for massively multilingual grapheme-to-phoneme conversion}, 
+    author={Jian Zhu and Cong Zhang and David Jurgens},
+    year={2022},
+    eprint={2204.03067},
+    archivePrefix={arXiv},
+    primaryClass={cs.CL}
 }
 ```
```

### Comparing `lexikos-0.0.1b0/README.md` & `lexikos-0.0.1rc0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,40 @@
 
 A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 
 <p align="center">
     <img src="https://github.com/bookbot-hive/lexikos/raw/main/assets/lexikos.png" alt="logo" width="300"/>
 </p>
 
+## Install Lexikos
+
+Install from PyPI
+
+```sh
+pip install lexikos
+```
+
+Editable install from Source
+
+```sh
+git clone https://github.com/bookbot-hive/lexikos.git
+pip install -e lexikos
+```
+
 ## Usage
 
 ```py
 >>> from lexikos import Lexicon
 >>> lexicon = Lexicon()
 >>> print(lexicon["added"])
-{'ˈæ d ə d', 'a d ɪ d', 'æ d ɪ d', 'a d ə d', 'æ ɾ ə d', 'ˈa d ə d', 'æ d ə d', 'ˈæ d ɪ d', 'ˈa d ɪ d', 'ˈæ ɾ ɪ d', 'æ ɾ ɪ d', 'ˈæ ɾ ə d'}
+{'ˈæ ɾ ɪ d', 'æ ɾ ɪ d', 'ˈæ d ɪ d', 'a d ɪ d', 'a d ə d', 'ˈæ ɾ ə d', 'ˈæ d ə d', 'æ d ɪ d', 'æ ɾ ə d', 'æ d ə d', 'ˈa d ɪ d', 'ˈa d ə d'}
 >>> print(lexicon["runner"])
-{'ɹ ʌ n ɚ', 'ˈr ʌ n ɝ', 'ɹ ʌ n ə'}
+{'ɹ ʌ n ə', 'ɹ ʌ n ɚ', 'ˈr ʌ n ɝ'}
 >>> print(lexicon["water"])
-{'w ɑ ɾ ɚ', 'ˈw oː t ə', 'w ɑ t ə ɹ', 'w ɔ ɾ ɚ', 'ˈw oː ɾ ə', 'w ɔː t ə', 'ˈw ɔ t ɝ', 'w ɔ t ə ɹ'}
+{'ˈw oː t ə', 'w ɔ t ə ɹ', 'ˈw ɑ t ə ɹ', 'w ɑ ɾ ɚ', 'ˈw ɔ t ɝ', 'ˈw ɑ ɾ ɚ', 'ˈʋ ɔ ʈ ə r', 'ˈʋ aː ʈ ə r ɯ', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ', 'ˈw aː ʈ ə r ɯ', 'ˈw ɔ ʈ ə r', 'ˈw oː ɾ ə', 'w ɔː t ə'}
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
 | Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
@@ -48,14 +63,36 @@
 ### English `(en-AU)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
 | -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
 | en-AU (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
 | en-AU (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
 
+### English `(en-CA)`
+
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
+| en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  |           |
+| en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |           |
+
+### English `(en-NZ)`
+
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
+| en-NZ (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_broad.tsv)  |           |
+| en-NZ (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_narrow.tsv) |           |
+
+### English `(en-IN)`
+
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
+| en-IN (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_broad.tsv)  |           |
+| en-IN (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_narrow.tsv) |           |
+
+
 ## Training G2P Model
 
 We modified the sequence-to-sequence training script of [🤗 HuggingFace](https://github.com/huggingface/transformers/blob/main/examples/pytorch/translation/run_translation.py) for the purpose of training G2P models. Refer to their [installation requirements](https://github.com/huggingface/transformers/tree/main/examples/pytorch/translation) for more details.
 
 Training a new G2P model generally follow this recipe:
 
 ```diff
@@ -149,19 +186,19 @@
 | Language Family        | Code                              | Region                                                | Corpus | G2P Model |
 | ---------------------- | --------------------------------- | ----------------------------------------------------- | :----: | :-------: |
 | African English        | en-ZA                             | South Africa                                          |        |           |
 | Australian English     | en-AU                             | Australia                                             |   ✅    |     ✅     |
 | East Asian English     | en-CN, en-HK, en-JP, en-KR, en-TW | China, Hong Kong, Japan, South Korea, Taiwan          |        |           |
 | European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |        |           |
 | Mexican English        | en-MX                             | Mexico                                                |        |           |
-| New Zealand English    | en-NZ                             | New Zealand                                           |        |           |
-| North American         | en-CA, en-US                      | Canada, United States                                 |        |           |
+| New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |           |
+| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |           |
 | Middle Eastern English | en-EG, en-IL                      | Egypt, Israel                                         |        |           |
 | Southeast Asian        | en-TH, en-ID, en-MY, en-PH, en-SG | Thailand, Indonesia, Malaysia, Philippines, Singapore |        |           |
-| South Asian English    | en-IN                             | India                                                 |        |           |
+| South Asian English    | en-IN                             | India                                                 |   ✅    |           |
   
 ## Resources
 
 - [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P)
 - [Microsoft CNTK](https://github.com/microsoft/CNTK/tree/master)
 - [CMU Pronouncing Dictionary - IPA](https://github.com/menelik3/cmudict-ipa)
 - [Wikipron](https://github.com/CUNY-CL/wikipron/tree/master)
@@ -184,15 +221,15 @@
     publisher = "European Language Resources Association",
     pages = "4223--4228",
 }
 ```
 
 ```bibtex
 @misc{zhu2022byt5,
-      title={ByT5 model for massively multilingual grapheme-to-phoneme conversion}, 
-      author={Jian Zhu and Cong Zhang and David Jurgens},
-      year={2022},
-      eprint={2204.03067},
-      archivePrefix={arXiv},
-      primaryClass={cs.CL}
+    title={ByT5 model for massively multilingual grapheme-to-phoneme conversion}, 
+    author={Jian Zhu and Cong Zhang and David Jurgens},
+    year={2022},
+    eprint={2204.03067},
+    archivePrefix={arXiv},
+    primaryClass={cs.CL}
 }
 ```
```

### Comparing `lexikos-0.0.1b0/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv` & `lexikos-0.0.1rc0/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn.tsv` & `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_au_broad.tsv` & `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_au_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_au_narrow.tsv` & `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_au_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_uk_broad.tsv` & `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_uk_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv` & `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_us_broad.tsv` & `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_us_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/lexikos/dict/wikipron/eng_latn_us_narrow.tsv` & `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_us_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/lexikos/lexicon.py` & `lexikos-0.0.1rc0/lexikos/lexicon.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1b0/lexikos.egg-info/PKG-INFO` & `lexikos-0.0.1rc0/lexikos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1b0
+Version: 0.0.1rc0
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -221,25 +221,40 @@
 
 A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 
 <p align="center">
     <img src="https://github.com/bookbot-hive/lexikos/raw/main/assets/lexikos.png" alt="logo" width="300"/>
 </p>
 
+## Install Lexikos
+
+Install from PyPI
+
+```sh
+pip install lexikos
+```
+
+Editable install from Source
+
+```sh
+git clone https://github.com/bookbot-hive/lexikos.git
+pip install -e lexikos
+```
+
 ## Usage
 
 ```py
 >>> from lexikos import Lexicon
 >>> lexicon = Lexicon()
 >>> print(lexicon["added"])
-{'ˈæ d ə d', 'a d ɪ d', 'æ d ɪ d', 'a d ə d', 'æ ɾ ə d', 'ˈa d ə d', 'æ d ə d', 'ˈæ d ɪ d', 'ˈa d ɪ d', 'ˈæ ɾ ɪ d', 'æ ɾ ɪ d', 'ˈæ ɾ ə d'}
+{'ˈæ ɾ ɪ d', 'æ ɾ ɪ d', 'ˈæ d ɪ d', 'a d ɪ d', 'a d ə d', 'ˈæ ɾ ə d', 'ˈæ d ə d', 'æ d ɪ d', 'æ ɾ ə d', 'æ d ə d', 'ˈa d ɪ d', 'ˈa d ə d'}
 >>> print(lexicon["runner"])
-{'ɹ ʌ n ɚ', 'ˈr ʌ n ɝ', 'ɹ ʌ n ə'}
+{'ɹ ʌ n ə', 'ɹ ʌ n ɚ', 'ˈr ʌ n ɝ'}
 >>> print(lexicon["water"])
-{'w ɑ ɾ ɚ', 'ˈw oː t ə', 'w ɑ t ə ɹ', 'w ɔ ɾ ɚ', 'ˈw oː ɾ ə', 'w ɔː t ə', 'ˈw ɔ t ɝ', 'w ɔ t ə ɹ'}
+{'ˈw oː t ə', 'w ɔ t ə ɹ', 'ˈw ɑ t ə ɹ', 'w ɑ ɾ ɚ', 'ˈw ɔ t ɝ', 'ˈw ɑ ɾ ɚ', 'ˈʋ ɔ ʈ ə r', 'ˈʋ aː ʈ ə r ɯ', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ', 'ˈw aː ʈ ə r ɯ', 'ˈw ɔ ʈ ə r', 'ˈw oː ɾ ə', 'w ɔː t ə'}
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
 | Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
@@ -267,14 +282,36 @@
 ### English `(en-AU)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
 | -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
 | en-AU (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
 | en-AU (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
 
+### English `(en-CA)`
+
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
+| en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  |           |
+| en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |           |
+
+### English `(en-NZ)`
+
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
+| en-NZ (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_broad.tsv)  |           |
+| en-NZ (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_narrow.tsv) |           |
+
+### English `(en-IN)`
+
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
+| en-IN (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_broad.tsv)  |           |
+| en-IN (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_narrow.tsv) |           |
+
+
 ## Training G2P Model
 
 We modified the sequence-to-sequence training script of [🤗 HuggingFace](https://github.com/huggingface/transformers/blob/main/examples/pytorch/translation/run_translation.py) for the purpose of training G2P models. Refer to their [installation requirements](https://github.com/huggingface/transformers/tree/main/examples/pytorch/translation) for more details.
 
 Training a new G2P model generally follow this recipe:
 
 ```diff
@@ -368,19 +405,19 @@
 | Language Family        | Code                              | Region                                                | Corpus | G2P Model |
 | ---------------------- | --------------------------------- | ----------------------------------------------------- | :----: | :-------: |
 | African English        | en-ZA                             | South Africa                                          |        |           |
 | Australian English     | en-AU                             | Australia                                             |   ✅    |     ✅     |
 | East Asian English     | en-CN, en-HK, en-JP, en-KR, en-TW | China, Hong Kong, Japan, South Korea, Taiwan          |        |           |
 | European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |        |           |
 | Mexican English        | en-MX                             | Mexico                                                |        |           |
-| New Zealand English    | en-NZ                             | New Zealand                                           |        |           |
-| North American         | en-CA, en-US                      | Canada, United States                                 |        |           |
+| New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |           |
+| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |           |
 | Middle Eastern English | en-EG, en-IL                      | Egypt, Israel                                         |        |           |
 | Southeast Asian        | en-TH, en-ID, en-MY, en-PH, en-SG | Thailand, Indonesia, Malaysia, Philippines, Singapore |        |           |
-| South Asian English    | en-IN                             | India                                                 |        |           |
+| South Asian English    | en-IN                             | India                                                 |   ✅    |           |
   
 ## Resources
 
 - [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P)
 - [Microsoft CNTK](https://github.com/microsoft/CNTK/tree/master)
 - [CMU Pronouncing Dictionary - IPA](https://github.com/menelik3/cmudict-ipa)
 - [Wikipron](https://github.com/CUNY-CL/wikipron/tree/master)
@@ -403,15 +440,15 @@
     publisher = "European Language Resources Association",
     pages = "4223--4228",
 }
 ```
 
 ```bibtex
 @misc{zhu2022byt5,
-      title={ByT5 model for massively multilingual grapheme-to-phoneme conversion}, 
-      author={Jian Zhu and Cong Zhang and David Jurgens},
-      year={2022},
-      eprint={2204.03067},
-      archivePrefix={arXiv},
-      primaryClass={cs.CL}
+    title={ByT5 model for massively multilingual grapheme-to-phoneme conversion}, 
+    author={Jian Zhu and Cong Zhang and David Jurgens},
+    year={2022},
+    eprint={2204.03067},
+    archivePrefix={arXiv},
+    primaryClass={cs.CL}
 }
 ```
```

### Comparing `lexikos-0.0.1b0/lexikos.egg-info/SOURCES.txt` & `lexikos-0.0.1rc0/lexikos.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,11 +10,17 @@
 lexikos.egg-info/SOURCES.txt
 lexikos.egg-info/dependency_links.txt
 lexikos.egg-info/top_level.txt
 lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
 lexikos/dict/wikipron/eng_latn.tsv
 lexikos/dict/wikipron/eng_latn_au_broad.tsv
 lexikos/dict/wikipron/eng_latn_au_narrow.tsv
+lexikos/dict/wikipron/eng_latn_ca_broad.tsv
+lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
+lexikos/dict/wikipron/eng_latn_in_broad.tsv
+lexikos/dict/wikipron/eng_latn_in_narrow.tsv
+lexikos/dict/wikipron/eng_latn_nz_broad.tsv
+lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
 lexikos/dict/wikipron/eng_latn_uk_broad.tsv
 lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
 lexikos/dict/wikipron/eng_latn_us_broad.tsv
 lexikos/dict/wikipron/eng_latn_us_narrow.tsv
```

### Comparing `lexikos-0.0.1b0/pyproject.toml` & `lexikos-0.0.1rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexikos"
-version = "0.0.1b"
+version = "0.0.1c"
 description = "A collection of pronunciation dictionaries and neural grapheme-to-phoneme models."
 readme = "README.md"
 authors = [{ name="w11wo", email="wilson@bookbotkids.com" }, { name="anantoj", email="gg.ananto@gmail.com" }, { name="DavidSamuell", email="davidsamuel.7878@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `lexikos-0.0.1b0/setup.py` & `lexikos-0.0.1rc0/setup.py`

 * *Files identical despite different names*

