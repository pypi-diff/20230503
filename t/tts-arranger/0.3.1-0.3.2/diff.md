# Comparing `tmp/tts_arranger-0.3.1.tar.gz` & `tmp/tts_arranger-0.3.2.tar.gz`

## Comparing `tts_arranger-0.3.1.tar` & `tts_arranger-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/requirements.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_abstract_writer.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_html_converter.py
--rw-r--r--   0        0        0    24605 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    17364 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/checkers_default.json
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/exclude_ids.json
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/examples/tts_project_example.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/examples/tts_simple_example.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/__init__.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/checker.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_abstract_reader.py
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_epub_reader.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_html_based_reader.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_html_reader.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_srt_reader.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_text_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/tests/reader_test.py
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/LICENSE
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/README.md
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 tts_arranger-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/requirements.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_abstract_writer.py
+-rw-r--r--   0        0        0    12647 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_html_converter.py
+-rw-r--r--   0        0        0    24594 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    17364 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/data/checkers_default.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/data/exclude_ids.json
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/examples/tts_project_example.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/examples/tts_simple_example.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_reader/__init__.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_reader/checker.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_abstract_reader.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_epub_reader.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_html_based_reader.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_html_reader.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_srt_reader.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_text_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/tests/reader_test.py
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/README.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 tts_arranger-0.3.2/PKG-INFO
```

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_abstract_writer.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_abstract_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_html_converter.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_html_converter.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,68 +6,84 @@
 from pathlib import Path
 from typing import Optional
 
 from tts_arranger.items.tts_item import TTS_Item  # type: ignore
 from tts_arranger.tts_writer import TTS_Chapter, TTS_Project  # type: ignore
 
 from tts_arranger.tts_reader.checker import (CHECK_SPEAKER_RESULT, CHECKER_SIGNAL, Checker,
-                     CheckerItemProperties, Condition, ConditionClass,
-                     ConditionID, ConditionName, Element)
+                                             CheckerItemProperties, Condition, ConditionClass,
+                                             ConditionID, ConditionName, Element)
 
 
 class CONVERSION_MODE(Enum):
     ITEMS = auto()
     PROJECT = auto()
 
 
 class TTS_HTML_Converter(HTMLParser):
     """
-    Class for converting HTML to a TTS_Project or list of TTS_Item objects.
+    Class for converting HTML to a TTS_Project or list of TTS_Item objects. Works on an internal project object that can be retrieved after loading all needed data is finished.
     """
     project: TTS_Project
 
-    def __init__(self, *, convert_charrefs: bool = True, checkers: Optional[list[Checker]] = None, default_properties=CheckerItemProperties(pause_after=250)) -> None:
+    def __init__(self, *, convert_charrefs: bool = True, default_properties=CheckerItemProperties(pause_after=250), custom_checkers: Optional[list[Checker]] = None, custom_checkers_files: Optional[list[str]] = None, ignore_default_checkers: bool = False) -> None:
         """
         Initializes a TTS_HTML_Converter object.
 
         :param convert_charrefs: A boolean indicating whether to replace HTML character references with their corresponding Unicode characters.
         :type convert_charrefs: bool
 
         :param checkers: An optional list of Checker objects to use for checking each HTML element.
         :type checkers: Optional[list[Checker]]
 
         :param default_properties: An optional CheckerItemProperties object that represents the default properties for all HTML elements.
         :type default_properties: CheckerItemProperties
         """
         super().__init__(convert_charrefs=convert_charrefs)
 
-        self.checkers: list[Checker] = checkers or []
-
         self.default_properties = default_properties
-
         self.last_signal = CHECKER_SIGNAL.NO_SIGNAL
 
+        # Initialize list with custom checkers so they have the highest priority
+        self.checkers: list[Checker] = custom_checkers or []
+
+        if custom_checkers:
+            print(f'{len(custom_checkers)} custom checker entries added.')
+
         self.checker_results_stack: list[tuple[CHECK_SPEAKER_RESULT, CHECKER_SIGNAL, Optional[CheckerItemProperties]]] = []
 
-        # Push default properties to stack to start with
+        # Add checkers from custom files
+        if custom_checkers_files:
+            for custom_checkers_file in custom_checkers_files:
+                self.add_checkers_from_json(custom_checkers_file)
+
+        # Finally add default checkers from data folder (lowest priority)
+        if not ignore_default_checkers:
+            source_dir = Path(__file__).resolve().parent.parent
+            base_path = os.path.dirname(__file__) if __file__ else str(source_dir)
+            default_file = os.path.join(base_path, 'data', 'checkers_default.json')
+
+            self.add_checkers_from_json(default_file)
+
+        # Push default starting properties to stack
         self.checker_results_stack.append((CHECK_SPEAKER_RESULT.NOT_MATCHED, CHECKER_SIGNAL.NO_SIGNAL, default_properties))
 
         self.project = TTS_Project()
-        self.current_item: TTS_Item | None = None
+        self.current_item: Optional[TTS_Item] = None
 
     def tag_to_element(self, name: str, attrs: list) -> Element:
         """
         Converts an HTML tag to an Element object.
 
         :param name: The name of the HTML tag.
         :type name: str
-        
+
         :param attrs: The attributes of the HTML tag.
         :type attrs: list
-        
+
         :return: An Element object representing the HTML tag.
         """
         elem = Element(name)
 
         for attr in attrs:
             match attr[0]:
                 case 'id':
@@ -78,20 +94,20 @@
 
     def handle_starttag(self, name: str, attrs: list) -> None:
         """
         Handles the start of an HTML tag.
 
         :param name: The name of the HTML tag.
         :type name: str
-        
+
         :param attrs: The attributes of the HTML tag.
         :type attrs: list
         """
-        # Ignore scripts
-        if name == 'script':
+        # Ignore script, style tags, etc.
+        if name in ['script', 'style', 'meta']:
             result = CHECK_SPEAKER_RESULT.MATCHED
             signal = CHECKER_SIGNAL.IGNORE
             properties = None
         else:
             result, signal, properties = copy.deepcopy(self._check_elem(self.tag_to_element(name, attrs), self.checkers))
 
             if result != CHECK_SPEAKER_RESULT.MATCHED:
@@ -234,137 +250,90 @@
                 return self.project
             case CONVERSION_MODE.ITEMS:
                 if self.project.tts_chapters:
                     return self.project.tts_chapters[-1].tts_items
 
         return None
 
-    def get_checkers_files(self, filename: str = '', default_filename: str = '', ignore_default: bool = False) -> list[str]:
+    def add_checkers_from_json(self, filename: str = '') -> None:
         """
-        Compiles a list of checkers files, sorted by priority, starting with the first file (if available), adding the default file (if available), and finally adding the library default file
+        Load and add checkers from a checkers JSON file.
 
         :param filename: Filename of the checkers file to load (in JSON format), defaults to ''
         :type filename: str, optional
 
-        :param default_filename: Filename of a fallback checkers file to load, defaults to ''
-        :type default_filename: str, optional
-
-        :param ignore_default: Defines if the library's default checkers file should be ignored, defaults to False
-        :type ignore_default: bool, optional
-
-        :return: List of checkers
-        :rtype: list[str]
-        """
-        files: list[str] = []
-
-        if os.path.exists(filename):
-            files.append(filename)
-
-        # Check for default file in the same path
-        if default_filename:
-            if os.path.exists(default_filename):
-                files.append(default_filename)
-
-        # Check for default file
-        if ignore_default:
-            return files
-        
-        source_dir = Path(__file__).resolve().parent.parent
-
-        base_path = os.path.dirname(__file__) if __file__ else str(source_dir)
-        default_file = os.path.join(base_path, 'data', 'checkers_default.json')
-        if os.path.exists(default_file):
-            files.append(default_file)
-            return files
-
-        raise FileNotFoundError(f'No checkers file or default file found.')
-
-    def add_checkers_from_json(self, filename: str = '', default_filename: str = '', ignore_default=False) -> None:
-        """
-        Load and add checkers from a list of checkers files.
-
-        :param filename: Filename of the checkers file to load (in JSON format), defaults to ''
-        :type filename: str, optional
-
-        :param default_filename: Filename of a fallback checkers file to load, defaults to ''
-        :type default_filename: str, optional
-
-        :param ignore_default: Defines if the library's default checkers file should be ignored, defaults to False
-        :type ignore_default: bool, optional
-
         :return: None
         """
-        for checker_file in self.get_checkers_files(filename, default_filename, ignore_default):
-            print(f'Loading checkers file "{checker_file}"')
+        print(f'Loading checkers file "{filename}"')
 
-            json_check_entries = []
+        json_check_entries = []
 
-            with open(checker_file, 'r') as file:
-                data = json.load(file)
+        with open(filename, 'r') as file:
+            data = json.load(file)
 
-                json_check_entries = data['check_entries']
+            json_check_entries = data['check_entries']
 
-            print(f'{len(json_check_entries)} checker entries found.')
-            for json_entry in json_check_entries:
+        for json_entry in json_check_entries:
 
-                # Access the conditions list for the entry
-                json_conditions = json_entry['conditions']
+            # Access the conditions list for the entry
+            json_conditions = json_entry['conditions']
 
-                conditions: list[Condition] = []
+            conditions: list[Condition] = []
 
-                for json_condition in json_conditions:
-                    # Access the name and arg properties of the condition
-                    name = json_condition['name']
-                    arg = json_condition['arg']
+            for json_condition in json_conditions:
+                # Access the name and arg properties of the condition
+                name = json_condition['name']
+                arg = json_condition['arg']
 
-                    condition: Condition | None = None
+                condition: Optional[Condition] = None
 
-                    match name:
-                        case 'Name':
-                            condition = ConditionName(arg)
-                        case 'Class':
-                            condition = ConditionClass(arg)
-                        case 'ID':
-                            condition = ConditionID(arg)
-                        case _:
-                            pass
+                match name:
+                    case 'Name':
+                        condition = ConditionName(arg)
+                    case 'Class':
+                        condition = ConditionClass(arg)
+                    case 'ID':
+                        condition = ConditionID(arg)
+                    case _:
+                        print(f'Unknown checker condition found: {name}')
 
-                    if condition:
-                        if condition.arg:
-                            conditions.append(condition)
+                if condition:
+                    if condition.arg:
+                        conditions.append(condition)
 
-                # Access the properties dictionary for the entry
-                json_properties = json_entry['properties']
+            # Access properties dictionary for entry
+            json_properties = json_entry['properties']
 
-                properties: Optional[CheckerItemProperties] = None
+            properties: Optional[CheckerItemProperties] = None
 
-                speaker_idx = 0
-                pause_after = 0
+            speaker_idx = 0
+            pause_after = 0
 
-                if 'speaker_idx' in json_properties:
-                    speaker_idx = int(json_properties['speaker_idx'])
-                if 'pause_after' in json_properties:
-                    pause_after = int(json_properties['pause_after'])
+            if 'speaker_idx' in json_properties:
+                speaker_idx = int(json_properties['speaker_idx'])
+            if 'pause_after' in json_properties:
+                pause_after = int(json_properties['pause_after'])
 
-                properties = CheckerItemProperties(speaker_idx, pause_after)
+            properties = CheckerItemProperties(speaker_idx, pause_after)
 
-                signal = CHECKER_SIGNAL.NO_SIGNAL
+            signal = CHECKER_SIGNAL.NO_SIGNAL
 
-                # Access the signals list for the entry
-                if 'signal' in json_entry:
-                    json_signal = json_entry['signal']
+            # Access signals list for entry
+            if 'signal' in json_entry:
+                json_signal = json_entry['signal']
 
-                    match json_signal:
-                        case 'NEW_CHAPTER':
-                            signal = CHECKER_SIGNAL.NEW_CHAPTER
-                        case 'IGNORE':
-                            signal = CHECKER_SIGNAL.IGNORE
-                        case _:
-                            pass
+                match json_signal:
+                    case 'NEW_CHAPTER':
+                        signal = CHECKER_SIGNAL.NEW_CHAPTER
+                    case 'IGNORE':
+                        signal = CHECKER_SIGNAL.IGNORE
+                    case _:
+                        print(f'Unknown checker signal found: {json_signal}')
 
-                self.checkers.append(Checker(conditions, properties, signal))
+            self.checkers.append(Checker(conditions, properties, signal))
+        print(f'{len(json_check_entries)} checkers entries added.')
 
     def get_project(self) -> TTS_Project:
         """
         Returns the finished TTS project.
         """
         return self.project
```

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_processor.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,21 +83,22 @@
         """
         Initializes the text-to-speech (TTS) system, downloads the specified models, and populates the speaker list.
 
         :return: None
         """
         log(LOG_TYPE.INFO, f'Initializing speech synthesizer.')
         models_dir = Path(TTS.__file__).resolve().parent / '.models.json'
+
         self.manager = ModelManager(str(models_dir))
 
-        with contextlib.redirect_stdout(None):
-            (model_path, config_path, _), (vocoder_path, vocoder_config_path, _) = [
-                self.manager.download_model(m) if m else ('', '', '') for m in (self.model, self.vocoder)
-            ]
+        (model_path, config_path, _), (vocoder_path, vocoder_config_path, _) = [
+            self.manager.download_model(m) if m else ('', '', '') for m in (self.model, self.vocoder)
+        ]
 
+        with contextlib.redirect_stdout(None):
             self.synthesizer = Synthesizer(
                 tts_checkpoint=model_path,
                 tts_config_path=config_path,
                 vocoder_checkpoint=vocoder_path,
                 vocoder_config=vocoder_config_path if self.vocoder else '',
             )
```

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_simple_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_writer.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/data/checkers_default.json` & `tts_arranger-0.3.2/src/tts_arranger/data/checkers_default.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/examples/tts_project_example.py` & `tts_arranger-0.3.2/src/tts_arranger/examples/tts_project_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #!/usr/bin/python3
+import os
 from tts_arranger import TTS_Item, TTS_Chapter, TTS_Project, TTS_Writer
 
+user_dir = os.path.expanduser('~')
+
 preferred_speakers = ['p273', 'p330']
 
 # Advanced example using a TTS Project object for creating an audiobook with chapters and a title image, uses tts_models/en/vctk/vits by (default)
 
 items1 = []
 items1.append(TTS_Item('This is a test', 0))
 items1.append(TTS_Item('This is another test by a different speaker', 1))
@@ -20,15 +23,15 @@
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
 # Prepare the project file
 project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')  # Add a cover image
 
 # Finally synthesize and write the project as a m4b audiobook using our preferred speakers
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', preferred_speakers=preferred_speakers)
+writer = TTS_Writer(project, os.path.join(user_dir, 'tts_arranger_example_output/'), preferred_speakers=preferred_speakers)
 writer.synthesize_and_write(project.author + ' - ' + project.title)
 
 # German example using Thorsten voice (no multispeaker support), output as mp3, writing one mp3 file per chapter
 
 items1 = []
 items1.append(TTS_Item('Dies ist ein Test.'))
 items1.append(TTS_Item('Noch ein Test.'))
@@ -39,9 +42,10 @@
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
 chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
 
 project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
+writer = TTS_Writer(project, os.path.join(user_dir, 'tts_arranger_example_output/'),
+                    model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
 writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
```

### Comparing `tts_arranger-0.3.1/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.3.2/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.3.2/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.3.2/src/tts_arranger/items/tts_project.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_reader/checker.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_reader/checker.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_abstract_reader.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_html_reader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,74 @@
-import os
-from abc import ABC
+
 from typing import Callable, Optional
 
-from .. import TTS_Item, TTS_Project, TTS_Writer  # type: ignore
+from bs4 import BeautifulSoup, PageElement  # type: ignore
 
+from tts_arranger.tts_reader.checker import Checker  # type: ignore
 
-class TTS_Abstract_Reader(ABC):
-    def __init__(self, preferred_speakers: Optional[list[str]] = None):
-        """
-        :param preferred_speakers: Optional list of preferred speakers to use instead of the models predefined speaker list  
-        :type preferred_speakers: Optional[list[str]]
-        """
+from .. import TTS_Project  # type: ignore
+from .tts_html_based_reader import TTS_HTML_Based_Reader  # type: ignore
 
-        self.preferred_speakers = preferred_speakers or []
-        self.project = TTS_Project()
 
-        self.title = ''
-        self.author = ''
+class TTS_HTML_Reader(TTS_HTML_Based_Reader):
+    """
+    Class for converting a HTML file into a TTS project.
+    """
 
-        self.output_format = 'm4b'
+    def __init__(self, preferred_speakers: Optional[list[str]] = None, ignore_default_checkers=False, custom_checkers: Optional[list[Checker]] = None):
+        super().__init__(preferred_speakers, custom_checkers, ignore_default_checkers=ignore_default_checkers)
 
-    def get_output_filename(self) -> str:
+    def load(self, filename: str, callback: Optional[Callable[[float], None]] = None) -> None:
         """
-        Get the output filename.
+        Load an HTML file into the TTS_Project.
 
-        :return: The output filename.
-        :rtype: str
-        """
-        return self.project.author + ' - ' + self.project.title
+        :param content: The HTML string.
+        :type content: str
 
-    def _smart_truncate(self, content: str, length=100, suffix='…') -> str:
-        """
-        Shorten the given string without breaking words
-        """
-        if len(content) <= length:
-            return content
-        else:
-            return ' '.join(content[:length+1].split(' ')[0:-1]) + suffix
+        :param author: The author of the HTML file (will be used as the author of the audiobook).
+        :type author: str
 
-    def load(self, filename: str, callback: Optional[Callable[[float], None]] = None) -> None:
-        # Set filename as title
-        self.title = os.path.splitext(os.path.basename(filename))[0]
+        :param title: The title of the HTML file (will be used as the title of the audiobook).
+        :type title: str
 
-    def load_raw(self, content: str, author: str = '', title: str = '', callback: Optional[Callable[[float], None]] = None) -> None:
-        self.author = author or self.author
-        self.title = title or self.title
+        :param callback: An optional function that takes a float between 0 and 1 representing the progress of the loading process as its argument. This can be used to periodically check on the loading progress. Defaults to None if not provided.
+        :type callback: Optional[Callable[[float], None]]
+
+        :return: None
+        """
+        super().load(filename, callback)
+        with open(filename, 'r') as file:
+            self.load_raw(file.read())
 
-    def synthesize(self, output_filename: str, temp_dir_prefix='', callback: Optional[Callable[[float, TTS_Item], None]] = None) -> None:
+    def load_raw(self, content: str, author: str = '', title: str = '', callback: Optional[Callable[[float], None]] = None) -> None:
         """
-        Synthesize speech and write it to an audio file.
+        Load HTML content into the TTS_Project.
+
+        :param content: The HTML string.
+        :type content: str
 
-        :param filename: The name of the output audio file.
-        :type filename: str
+        :param author: The author of the HTML file (will be used as the author of the audiobook).
+        :type author: str
 
-        :param temp_dir_prefix: Prefix for the temporary directory used during synthesis.
-        :type temp_dir_prefix: str
+        :param title: The title of the HTML file (will be used as the title of the audiobook).
+        :type title: str
 
-        :param callback: A function that will be called repeatedly during synthesis to provide progress information and TTS items.
-        :type callback: Optional[Callable[[float, TTS_Item], None]]
+        :param callback: An optional function that takes a float between 0 and 1 representing the progress of the loading process as its argument. This can be used to periodically check on the loading progress. Defaults to None if not provided.
+        :type callback: Optional[Callable[[float], None]]
 
         :return: None
         """
+        super().load_raw(content, author, title, callback)
+
+        soup = BeautifulSoup(content, 'html.parser')
+
+        if isinstance(soup, PageElement):
+            project = self.html_converter.convert_from_html(str(soup))
 
-        path, full_name = os.path.split(output_filename)
-        filename, extension = os.path.splitext(full_name)
+            # Get titles from first chapter items
+            if isinstance(project, TTS_Project):
+                project.get_titles()
 
-        writer = TTS_Writer(self.project, path, self.output_format, preferred_speakers=self.preferred_speakers)
-        writer.synthesize_and_write(self.get_output_filename(), temp_dir_prefix, callback=callback, concat=False, optimize=True)
+            self.project.merge_from_project(project)
 
-    def get_project(self) -> TTS_Project:
-        return self.project
+        self.project.author = self.author
+        self.project.title = self.title
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_epub_reader.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_epub_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 from pathlib import Path
 from typing import Callable, Optional
 
 from bs4 import BeautifulSoup, PageElement  # type: ignore
 from dateutil.parser import parse  # type: ignore
 from ebooklib import ITEM_DOCUMENT, epub  # type: ignore
 
+from tts_arranger.tts_reader.checker import Checker  # type: ignore
+
 from .tts_html_based_reader import TTS_HTML_Based_Reader  # type: ignore
 
 
 class TTS_EPUB_Reader(TTS_HTML_Based_Reader):
     """
     Class for converting an EPUB file into a TTS project.
     """
 
-    def __init__(self, preferred_speakers: Optional[list[str]] = None, ignore_default_checkers=False):
+    def __init__(self, preferred_speakers: Optional[list[str]] = None, ignore_default_checkers=False, custom_checkers: Optional[list[Checker]] = None):
         """
         Initializes the reader
 
         :param preferred_speakers: Optional list of preferred speakers to use instead of the models predefined speaker list , defaults to None
         :type preferred_speakers: Optional[list[str]], optional
 
-        :param ignore_default_checkers: Defines if the default checkers should be ignored and only, defaults to False
+        :param ignore_default_checkers: Defines if the default checkers should be ignored, defaults to False
         :type ignore_default_checkers: bool, optional
         """
-        super().__init__(preferred_speakers, ignore_default_checkers)
+        super().__init__(preferred_speakers, custom_checkers, ignore_default_checkers=ignore_default_checkers)
 
     def get_chapter_title(self, toc: list, href: str) -> str:
         """
         Get the title of the chapter from the table of contents and href.
 
         :param toc: The table of contents.
         :type toc: list
```

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_html_based_reader.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_html_based_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,31 +7,28 @@
 
 
 class TTS_HTML_Based_Reader(TTS_Abstract_Reader):
     """
     Base class for converting an EPUB file into a TTS project.
     """
 
-    def __init__(self, preferred_speakers: Optional[list[str]] = None, ignore_default_checkers=False):
+    def __init__(self, preferred_speakers: Optional[list[str]] = None, custom_checkers: Optional[list[Checker]] = None, custom_checkers_files: Optional[list[str]] = None, ignore_default_checkers=False):
         """
         :param preferred_speakers: Optional list of preferred speakers to use instead of the models predefined speaker list  
         :type preferred_speakers: Optional[list[str]]
         """
         super().__init__(preferred_speakers)
 
         self.current_properties: list[CheckerItemProperties] = []
         self.default_properties = CheckerItemProperties(0, 250)
         self.last_signal = CHECKER_SIGNAL.NO_SIGNAL
         self.current_chapter: Optional[TTS_Chapter] = None
-        self.checkers: list[Checker]
 
-        # Setup converter with default checkers
-        self.html_converter = TTS_HTML_Converter()
-        self.html_converter.add_checkers_from_json(ignore_default=ignore_default_checkers)
-
-    def initialize_checkers(self, default_properties: Optional[CheckerItemProperties] = None, checker_config_file='', checkers: Optional[list[Checker]] = None, ignore_default=False):
-        self.default_properties = default_properties or self.default_properties
-        self.current_properties.append(self.default_properties)
-
-        self.checkers = checkers or []
-        self.html_converter = TTS_HTML_Converter(checkers=self.checkers)
-        self.html_converter.add_checkers_from_json(checker_config_file, ignore_default=ignore_default)
+        self.html_converter = TTS_HTML_Converter(custom_checkers=custom_checkers, custom_checkers_files=custom_checkers_files, ignore_default_checkers=ignore_default_checkers)
+
+    # def initialize_checkers(self, default_properties: Optional[CheckerItemProperties] = None, checker_config_file='', checkers: Optional[list[Checker]] = None, ignore_default=False):
+    #     self.default_properties = default_properties or self.default_properties
+    #     self.current_properties.append(self.default_properties)
+
+    #     self.checkers = checkers or []
+    #     self.html_converter = TTS_HTML_Converter(checkers=self.checkers)
+    #     self.html_converter.add_checkers_from_json(checker_config_file, ignore_default=ignore_default)
```

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_srt_reader.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_srt_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/tts_reader/tts_text_reader.py` & `tts_arranger-0.3.2/src/tts_arranger/tts_reader/tts_text_reader.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/src/tts_arranger/utils/log.py` & `tts_arranger-0.3.2/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/tests/reader_test.py` & `tts_arranger-0.3.2/tests/reader_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
         checkers: list[Checker] = []
 
         checkers.append(Checker([ConditionName('p'), ConditionClass('bla')], CheckerItemProperties(1, 800)))
         checkers.append(Checker([ConditionName('i')], CheckerItemProperties(2, 500)))
         checkers.append(Checker([ConditionName('b')], CheckerItemProperties(3, 1000)))
 
-        reader = TTS_HTML_Reader()
-        reader.initialize_checkers(checkers=checkers)
+        reader = TTS_HTML_Reader(custom_checkers=checkers)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         self.assertEqual(items[0].speaker_idx, 1)
         self.assertEqual(items[0].text, 'test1 ')
         self.assertEqual(items[1].text, 'test2')
@@ -40,16 +39,15 @@
     def test2(self):
         html = '<body><html><sup class="endnote">1</sup>2</html></body>'
 
         checkers = []
 
         checkers.append(Checker([ConditionName('sup'), ConditionClass('endnote')], None, CHECKER_SIGNAL.IGNORE))
 
-        reader = TTS_HTML_Reader()
-        reader.initialize_checkers(checkers=checkers)
+        reader = TTS_HTML_Reader(custom_checkers=checkers)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize()
@@ -58,16 +56,15 @@
         self.assertEqual(items[0].text, '2')
 
     def test3(self):
         html = '<body id="itest" class="ctest"><html><p>1 <i>2</i> 3</p></html></body>'
 
         checkers = []
 
-        reader = TTS_HTML_Reader()
-        reader.initialize_checkers(checkers=checkers)
+        reader = TTS_HTML_Reader(custom_checkers=checkers)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize()
@@ -79,16 +76,15 @@
 
         html = '<body><html><p>1<i>2</i>3</p><p>4</p><p>5</p></html></body>'
 
         checkers = []
 
         checkers.append(Checker([ConditionName('p')], CheckerItemProperties(0, 800)))
 
-        reader = TTS_HTML_Reader()
-        reader.initialize_checkers(checkers=checkers)
+        reader = TTS_HTML_Reader(custom_checkers=checkers)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize()
@@ -103,16 +99,15 @@
 
     def test_merge_items2a(self):
         html = """<p id="b">a <em>b</em></div>"""
         checkers = []
 
         checkers.append(Checker([ConditionID('b')], CheckerItemProperties(1, 800)))
 
-        reader = TTS_HTML_Reader()
-        reader.initialize_checkers(checkers=checkers)
+        reader = TTS_HTML_Reader(custom_checkers=checkers)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize()
@@ -124,16 +119,15 @@
     def test_merge_items2(self):
         html = """<div class="c"><p id="a">a <a href="">b</a>. c.</p><p id="b">a <em>b</em>, c — d <a href="">e</a> f — g.</p><p id="c">a <a href="">b</a> c. d. e.</p></div>"""
         checkers = []
 
         checkers.append(Checker([ConditionID('b')], CheckerItemProperties(1, 800)))
         checkers.append(Checker([ConditionName('p')], CheckerItemProperties(0, 800)))
 
-        reader = TTS_HTML_Reader()
-        reader.initialize_checkers(checkers=checkers, ignore_default=True)
+        reader = TTS_HTML_Reader(custom_checkers=checkers, ignore_default_checkers=True)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize()
@@ -147,16 +141,15 @@
 
     def test_merge_items3(self):
         html = """<div style="text-align: justify;">Released 1992 for <b>Macintosh</b> <br></div>"""
         checkers = []
 
         checkers.append(Checker([ConditionName('br')], CheckerItemProperties(0, 800)))
 
-        reader = TTS_HTML_Reader()
-        reader.initialize_checkers(checkers=checkers)
+        reader = TTS_HTML_Reader(custom_checkers=checkers)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize()
@@ -167,16 +160,15 @@
     def test_merge_items4(self):
         html = """<span>1</span><span>2</span>"""
 
         checkers = []
 
         checkers.append(Checker([ConditionName('span')], CheckerItemProperties()))
 
-        reader = TTS_HTML_Reader(ignore_default_checkers=True)
-        reader.initialize_checkers(checkers=checkers, ignore_default=True)
+        reader = TTS_HTML_Reader(custom_checkers=checkers, ignore_default_checkers=True)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize()
@@ -187,66 +179,83 @@
     def test_merge_items5(self):
         html = """<span>1</span><span>2</span>"""
 
         checkers = []
 
         checkers.append(Checker([ConditionName('span')], CheckerItemProperties()))
 
-        reader = TTS_HTML_Reader(ignore_default_checkers=True)
-        reader.initialize_checkers(checkers=checkers, ignore_default=True)
+        reader = TTS_HTML_Reader(custom_checkers=checkers, ignore_default_checkers=True)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize()
         items = project.tts_chapters[0].tts_items
 
         self.assertEqual(items[0].text, '12')
         # self.assertEqual(items[1].text, '2')
 
-    def test_merge_items6(self):
-        # html = """<p>a <a href="">b</a>:<strong> </strong>c </p>"""
-        html = """<p id="2AaPJu">For more than two decades, the American Lung Association (ALA) has <a href="https://www.lung.org/research/sota">posed a simple question</a>:<strong> </strong>Is air pollution in the United States getting better or worse? </p>"""
+    # def test_merge_items6(self):
+    #     # html = """<p>a <a href="">b</a>:<strong> </strong>c </p>"""
+    #     html = """<p id="2AaPJu">For more than two decades, the American Lung Association (ALA) has <a href="https://www.lung.org/research/sota">posed a simple question</a>:<strong> </strong>Is air pollution in the United States getting better or worse? </p>"""
 
-        checkers = []
+    #     checkers = []
 
-        # checkers.append(Checker([ConditionName('span')], CheckerItemProperties()))
+    #     # checkers.append(Checker([ConditionName('span')], CheckerItemProperties()))
 
-        reader = TTS_HTML_Reader()
-        reader.initialize_checkers(checkers=checkers)
-        reader.load_raw(html)
+    #     reader = TTS_HTML_Reader(custom_checkers=checkers)
+    #     reader.load_raw(html)
 
-        items = reader.project.tts_chapters[0].tts_items
+    #     items = reader.project.tts_chapters[0].tts_items
 
-        project = TTS_Project()
-        project.tts_chapters.append(TTS_Chapter(items))
-        project.optimize()
-        items = project.tts_chapters[0].tts_items
+    #     project = TTS_Project()
+    #     project.tts_chapters.append(TTS_Chapter(items))
+    #     project.optimize()
+    #     items = project.tts_chapters[0].tts_items
 
-        # p = TTS_Processor()
-        # items = p.preprocess_items(items)
-        reader.project = project
-        reader.synthesize('/tmp/test.mp3')
+    #     # p = TTS_Processor()
+    #     # items = p.preprocess_items(items)
+    #     # reader.project = project
+    #     # reader.synthesize('/tmp/test.mp3')
 
-        self.assertEqual(items[0].text, 'a')
-        # self.assertEqual(items[1].text, '2')
+    #     self.assertEqual(items[0].text, 'a')
+    #     # self.assertEqual(items[1].text, '2')
+
+    # def test_merge_items7(self):
+    #     html = """<div>a. <b>b</b>. c. <i>d: </i><b>e</b>.</div>"""
+
+    #     checkers = []
+
+    #     checkers.append(Checker([ConditionName('b')], CheckerItemProperties(speaker_idx=1)))
+    #     checkers.append(Checker([ConditionName('i')], CheckerItemProperties(speaker_idx=1)))
+
+    #     reader = TTS_HTML_Reader(custom_checkers=checkers, ignore_default_checkers=True)
+    #     reader.load_raw(html)
+
+    #     items = reader.project.tts_chapters[0].tts_items
+
+    #     project = TTS_Project()
+    #     project.tts_chapters.append(TTS_Chapter(items))
+    #     project.optimize()
+    #     items = project.tts_chapters[0].tts_items
+
+    #     self.assertEqual(items[0].text, '12')
 
     def test_nested_tags(self):
         # html = """<p>a <a href="">b</a>:<strong> </strong>c </p>"""
         html = """<blockquote><p>test</p></blockquote>"""
 
         checkers = []
 
         checkers.append(Checker([ConditionName('p')], CheckerItemProperties(0)))
         checkers.append(Checker([ConditionName('blockquote')], CheckerItemProperties(1)))
 
-        reader = TTS_HTML_Reader()
-        reader.initialize_checkers(checkers=checkers, ignore_default=True)
+        reader = TTS_HTML_Reader(custom_checkers=checkers, ignore_default_checkers=True)
         reader.load_raw(html)
 
         items = reader.project.tts_chapters[0].tts_items
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize()
@@ -277,16 +286,15 @@
 
             urllib.request.urlretrieve('https://epubtest.org/books/Fundamental-Accessibility-Tests-Basic-Functionality-v1.0.0.epub', file_path)
 
             checkers = []
 
             checkers.append(Checker([ConditionName('h1')], CheckerItemProperties(1, 800)))
 
-            reader = TTS_EPUB_Reader(preferred_speakers)
-            reader.initialize_checkers(checkers=checkers)
+            reader = TTS_EPUB_Reader(preferred_speakers, custom_checkers=checkers)
             reader.load(file_path)
             reader.get_project().optimize()
 
             items = reader.get_project().tts_chapters[0].tts_items
 
             self.assertEqual(items[0].text, 'Table of Contents')
             self.assertEqual(items[0].speaker_idx, 1)
```

### Comparing `tts_arranger-0.3.1/tests/tts_arranger_test.py` & `tts_arranger-0.3.2/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/LICENSE` & `tts_arranger-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.3.1/README.md` & `tts_arranger-0.3.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -17,32 +17,40 @@
 * TTS_EPUB_Reader: Reads and converts an EPUB file into a TTS_Project instance
 * TTS_SRT_Reader: Reads and converts an SRT subtitle file into a TTS_Project instance *[not working due to timing bug at this point]*
 
 ### Helper Classes
 * TTS_Processor: Takes a TTS_Item, synthesizes and writes it to a file, also takes care of preprocessing the text input and post processing the audio output
 * TTS_HTML_Converter: Parses HTML content into a TTS_Project (mainly used by TTS_HTML_Reader and TTS_EPUB_Reader)
 
+## Requirements
+* ffmpeg, espeak-ng
+* for required Python packages see requirements.txt
+
 ## Examples
 
 ```python
-from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
-                          TTS_Simple_Writer, TTS_Writer)
+import os
+
+from tts_arranger import TTS_Item, TTS_Simple_Writer
+
+# Simple example using Simple Writer (using a simple list of TTS items), uses tts_models/en/vctk/vits by (default)
 
-# Simple example using Simple Writer (using a simple list of TTS items)
+user_dir = os.path.expanduser('~')
 
 tts_items = []
 
 preferred_speakers = ['p273', 'p330']
 
-tts_items.append(TTS_Item('This is a test', 1))
+tts_items.append(TTS_Item('This is a test', 0))  # Uses preferred speaker #0
 tts_items.append(TTS_Item(length=2000))  # Insert pause
-tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 0, length=10000))
+tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 1, length=10000)) # Uses preferred speaker #1 and sets minimum length
 
+# Create writer using our item list and prefered speakers and synthesize and save as mp3 audio
 simple_writer = TTS_Simple_Writer(tts_items, preferred_speakers)
-simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test.mp3')
+simple_writer.synthesize_and_write(os.path.join(user_dir, 'tts_arranger_example_output/test.mp3'))
 
 # English example using tts_models/en/vctk/vits (with multispeaker support)
 
 items1 = []
 items1.append(TTS_Item('This is a test:', 0))
 items1.append(TTS_Item('This is another test:', 1))
 
@@ -55,15 +63,15 @@
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
 project = TTS_Project(chapter, 'Project Title', 'Project Subtitle', author='Some Author')
 
 # Add a cover image
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', preferred_speakers=preferred_speakers)
+writer = TTS_Writer(project, os.path.join(user_dir, 'tts_arranger_example_output/'), preferred_speakers=preferred_speakers)
 writer.synthesize_and_write(project.author + ' - ' + project.title)
 
 # German example using Thorsten voice (no multispeaker support)
 
 items1 = []
 items1.append(TTS_Item('Dies ist ein Test:', speaker_idx=0))
 items1.append(TTS_Item('Noch ein Test:',  speaker_idx=1))
@@ -74,10 +82,10 @@
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
 chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
 
 project = TTS_Project(chapter, 'Projektname', 'Projekt-Untertitel', author='Ein Autor', lang_code='de')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
+writer = TTS_Writer(project, os.path.join(user_dir, 'tts_arranger_example_output/'), model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
 writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
 ```
```

### Comparing `tts_arranger-0.3.1/pyproject.toml` & `tts_arranger-0.3.2/pyproject.toml`

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
-version = "0.3.1"
+version = "0.3.2"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.3.1/PKG-INFO` & `tts_arranger-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.3.1
+Version: 0.3.2
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,32 +42,40 @@
 * TTS_EPUB_Reader: Reads and converts an EPUB file into a TTS_Project instance
 * TTS_SRT_Reader: Reads and converts an SRT subtitle file into a TTS_Project instance *[not working due to timing bug at this point]*
 
 ### Helper Classes
 * TTS_Processor: Takes a TTS_Item, synthesizes and writes it to a file, also takes care of preprocessing the text input and post processing the audio output
 * TTS_HTML_Converter: Parses HTML content into a TTS_Project (mainly used by TTS_HTML_Reader and TTS_EPUB_Reader)
 
+## Requirements
+* ffmpeg, espeak-ng
+* for required Python packages see requirements.txt
+
 ## Examples
 
 ```python
-from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
-                          TTS_Simple_Writer, TTS_Writer)
+import os
+
+from tts_arranger import TTS_Item, TTS_Simple_Writer
+
+# Simple example using Simple Writer (using a simple list of TTS items), uses tts_models/en/vctk/vits by (default)
 
-# Simple example using Simple Writer (using a simple list of TTS items)
+user_dir = os.path.expanduser('~')
 
 tts_items = []
 
 preferred_speakers = ['p273', 'p330']
 
-tts_items.append(TTS_Item('This is a test', 1))
+tts_items.append(TTS_Item('This is a test', 0))  # Uses preferred speaker #0
 tts_items.append(TTS_Item(length=2000))  # Insert pause
-tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 0, length=10000))
+tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 1, length=10000)) # Uses preferred speaker #1 and sets minimum length
 
+# Create writer using our item list and prefered speakers and synthesize and save as mp3 audio
 simple_writer = TTS_Simple_Writer(tts_items, preferred_speakers)
-simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test.mp3')
+simple_writer.synthesize_and_write(os.path.join(user_dir, 'tts_arranger_example_output/test.mp3'))
 
 # English example using tts_models/en/vctk/vits (with multispeaker support)
 
 items1 = []
 items1.append(TTS_Item('This is a test:', 0))
 items1.append(TTS_Item('This is another test:', 1))
 
@@ -80,15 +88,15 @@
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
 project = TTS_Project(chapter, 'Project Title', 'Project Subtitle', author='Some Author')
 
 # Add a cover image
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', preferred_speakers=preferred_speakers)
+writer = TTS_Writer(project, os.path.join(user_dir, 'tts_arranger_example_output/'), preferred_speakers=preferred_speakers)
 writer.synthesize_and_write(project.author + ' - ' + project.title)
 
 # German example using Thorsten voice (no multispeaker support)
 
 items1 = []
 items1.append(TTS_Item('Dies ist ein Test:', speaker_idx=0))
 items1.append(TTS_Item('Noch ein Test:',  speaker_idx=1))
@@ -99,10 +107,10 @@
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
 chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
 
 project = TTS_Project(chapter, 'Projektname', 'Projekt-Untertitel', author='Ein Autor', lang_code='de')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
+writer = TTS_Writer(project, os.path.join(user_dir, 'tts_arranger_example_output/'), model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
 writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
 ```
```

