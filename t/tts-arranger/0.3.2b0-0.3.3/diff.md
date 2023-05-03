# Comparing `tmp/tts_arranger-0.3.2b0.tar.gz` & `tmp/tts_arranger-0.3.3.tar.gz`

## Comparing `tts_arranger-0.3.2b0.tar` & `tts_arranger-0.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/requirements.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_abstract_writer.py
--rw-r--r--   0        0        0    12647 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_html_converter.py
--rw-r--r--   0        0        0    24620 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    17364 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/data/checkers_default.json
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/data/exclude_ids.json
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/examples/tts_project_example.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/examples/tts_simple_example.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/__init__.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/checker.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_abstract_reader.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_epub_reader.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_html_based_reader.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_html_reader.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_srt_reader.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_text_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/tests/reader_test.py
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/LICENSE
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/README.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/pyproject.toml
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 tts_arranger-0.3.2b0/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/requirements.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_abstract_writer.py
+-rw-r--r--   0        0        0    12647 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_html_converter.py
+-rw-r--r--   0        0        0    24620 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    17364 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/data/checkers_default.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/data/exclude_ids.json
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/examples/tts_project_example.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/examples/tts_simple_example.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_reader/__init__.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_reader/checker.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_abstract_reader.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_epub_reader.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_html_based_reader.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_html_reader.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_srt_reader.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_text_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/tests/reader_test.py
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/README.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 tts_arranger-0.3.3/PKG-INFO
```

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_abstract_writer.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_abstract_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_html_converter.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_html_converter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_processor.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_processor.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_simple_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_writer.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/data/checkers_default.json` & `tts_arranger-0.3.3/src/tts_arranger/data/checkers_default.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/examples/tts_project_example.py` & `tts_arranger-0.3.3/src/tts_arranger/examples/tts_project_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/examples/tts_simple_example.py` & `tts_arranger-0.3.3/src/tts_arranger/examples/tts_simple_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.3.3/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.3.3/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.3.3/src/tts_arranger/items/tts_project.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/checker.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_reader/checker.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_abstract_reader.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_abstract_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_epub_reader.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_epub_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_html_based_reader.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_html_based_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_html_reader.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_html_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_srt_reader.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_srt_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/tts_reader/tts_text_reader.py` & `tts_arranger-0.3.3/src/tts_arranger/tts_reader/tts_text_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/src/tts_arranger/utils/log.py` & `tts_arranger-0.3.3/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/tests/reader_test.py` & `tts_arranger-0.3.3/tests/reader_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/tests/tts_arranger_test.py` & `tts_arranger-0.3.3/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/LICENSE` & `tts_arranger-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.2b0/README.md` & `tts_arranger-0.3.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # TTS Arranger
 
-Library that simplifies arranging text items fragments with multiple speakers and processing them using coqui.ai TTS to write audio files. It also features helper classes for converting HTML (and thus EPUB files) into TTS projects, based of customizeable rules to read specific elements with different speakers, and define pauses after certain elements.
+Library that simplifies arranging text items fragments with multiple speakers, and processing them using [Coqui.ai TTS](https://github.com/coqui-ai/TTS) to write audio files, including chapter markers and metadata. It also features helper classes for converting HTML (and thus EPUB files) into TTS projects, based of customizeable rules to read specific elements with different speakers, and define pauses after certain elements.
+
+Install via pip: ``python -m pip install tts_arranger``
 
 ## Overview
 
 ### TTS project elements
-* TTS_Item, TTS_Chapter, TTS_Project
+* TTS_Item: basic building block containing text to synthesize, speaker index and length; is also used for pauses
+* TTS_Chapter: contains a list if TTS_Item objects, represents a chapter in the output audio file
+* TTS_Project: contains a list of chapters as well as metadata for the output file (like author, title, cover image)
 
 ### Writer Classes
 * TTS_Simple_Writer: Simple single-file writer, works with lists of TTS_Items directly
-* TTS_Writer: Designed for writing audiobooks with meta data and chapters, works on with TTS_Project
+* TTS_Writer: Designed for writing audiobooks with meta data and chapters, works with a TTS_Project object
 
 ### Reader Classes
 * TTS_Text_Reader: Reads and converts plain text into a TTS_Project instance 
 * TTS_HTML_Reader: Reads and converts HTML content into a TTS_Project instance
 * TTS_EPUB_Reader: Reads and converts an EPUB file into a TTS_Project instance
 * TTS_SRT_Reader: Reads and converts an SRT subtitle file into a TTS_Project instance *[not working due to timing bug at this point]*
```

### Comparing `tts_arranger-0.3.2b0/pyproject.toml` & `tts_arranger-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.3.2b"
+version = "0.3.3"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.3.2b0/PKG-INFO` & `tts_arranger-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.3.2b0
+Version: 0.3.3
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,24 +21,28 @@
 Requires-Dist: scipy>=1.9.0
 Requires-Dist: srt>=3.5.2
 Requires-Dist: tts>=0.13.3
 Description-Content-Type: text/markdown
 
 # TTS Arranger
 
-Library that simplifies arranging text items fragments with multiple speakers and processing them using coqui.ai TTS to write audio files. It also features helper classes for converting HTML (and thus EPUB files) into TTS projects, based of customizeable rules to read specific elements with different speakers, and define pauses after certain elements.
+Library that simplifies arranging text items fragments with multiple speakers, and processing them using [Coqui.ai TTS](https://github.com/coqui-ai/TTS) to write audio files, including chapter markers and metadata. It also features helper classes for converting HTML (and thus EPUB files) into TTS projects, based of customizeable rules to read specific elements with different speakers, and define pauses after certain elements.
+
+Install via pip: ``python -m pip install tts_arranger``
 
 ## Overview
 
 ### TTS project elements
-* TTS_Item, TTS_Chapter, TTS_Project
+* TTS_Item: basic building block containing text to synthesize, speaker index and length; is also used for pauses
+* TTS_Chapter: contains a list if TTS_Item objects, represents a chapter in the output audio file
+* TTS_Project: contains a list of chapters as well as metadata for the output file (like author, title, cover image)
 
 ### Writer Classes
 * TTS_Simple_Writer: Simple single-file writer, works with lists of TTS_Items directly
-* TTS_Writer: Designed for writing audiobooks with meta data and chapters, works on with TTS_Project
+* TTS_Writer: Designed for writing audiobooks with meta data and chapters, works with a TTS_Project object
 
 ### Reader Classes
 * TTS_Text_Reader: Reads and converts plain text into a TTS_Project instance 
 * TTS_HTML_Reader: Reads and converts HTML content into a TTS_Project instance
 * TTS_EPUB_Reader: Reads and converts an EPUB file into a TTS_Project instance
 * TTS_SRT_Reader: Reads and converts an SRT subtitle file into a TTS_Project instance *[not working due to timing bug at this point]*
```

