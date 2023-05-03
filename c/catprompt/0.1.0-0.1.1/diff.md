# Comparing `tmp/catprompt-0.1.0.tar.gz` & `tmp/catprompt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catprompt-0.1.0.tar", last modified: Fri Apr 28 11:19:20 2023, max compression
+gzip compressed data, was "catprompt-0.1.1.tar", last modified: Wed May  3 15:23:38 2023, max compression
```

## Comparing `catprompt-0.1.0.tar` & `catprompt-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-28 11:19:20.303316 catprompt-0.1.0/
--rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-15 09:03:27.000000 catprompt-0.1.0/LICENSE
--rw-r--r--   0 juanre     (501) staff       (20)     6900 2023-04-28 11:19:20.303215 catprompt-0.1.0/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)     5273 2023-04-28 11:18:41.000000 catprompt-0.1.0/README.md
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-28 11:19:20.302213 catprompt-0.1.0/catprompt/
--rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-15 09:03:27.000000 catprompt-0.1.0/catprompt/__init__.py
--rw-r--r--   0 juanre     (501) staff       (20)     4055 2023-04-28 11:16:44.000000 catprompt-0.1.0/catprompt/prompter.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-28 11:19:20.302839 catprompt-0.1.0/catprompt.egg-info/
--rw-r--r--   0 juanre     (501) staff       (20)     6900 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)      328 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/SOURCES.txt
--rw-r--r--   0 juanre     (501) staff       (20)        1 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/dependency_links.txt
--rw-r--r--   0 juanre     (501) staff       (20)       54 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/entry_points.txt
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/requires.txt
--rw-r--r--   0 juanre     (501) staff       (20)       10 2023-04-28 11:19:20.000000 catprompt-0.1.0/catprompt.egg-info/top_level.txt
--rw-r--r--   0 juanre     (501) staff       (20)      832 2023-04-28 11:18:09.000000 catprompt-0.1.0/pyproject.toml
--rw-r--r--   0 juanre     (501) staff       (20)       38 2023-04-28 11:19:20.303346 catprompt-0.1.0/setup.cfg
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 09:03:27.000000 catprompt-0.1.0/setup.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-28 11:19:20.303064 catprompt-0.1.0/test/
--rw-r--r--   0 juanre     (501) staff       (20)      796 2023-04-28 10:52:58.000000 catprompt-0.1.0/test/test_example.py
--rw-r--r--   0 juanre     (501) staff       (20)     3546 2023-04-24 11:39:03.000000 catprompt-0.1.0/test/test_prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-03 15:23:38.623459 catprompt-0.1.1/
+-rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-15 09:03:27.000000 catprompt-0.1.1/LICENSE
+-rw-r--r--   0 juanre     (501) staff       (20)     8875 2023-05-03 15:23:38.623254 catprompt-0.1.1/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)     7248 2023-05-03 15:18:22.000000 catprompt-0.1.1/README.md
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-03 15:23:38.622101 catprompt-0.1.1/catprompt/
+-rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-15 09:03:27.000000 catprompt-0.1.1/catprompt/__init__.py
+-rw-r--r--   0 juanre     (501) staff       (20)     7216 2023-05-03 14:28:16.000000 catprompt-0.1.1/catprompt/prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-03 15:23:38.622711 catprompt-0.1.1/catprompt.egg-info/
+-rw-r--r--   0 juanre     (501) staff       (20)     8875 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)      328 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 juanre     (501) staff       (20)        1 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       54 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/entry_points.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/requires.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       10 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/top_level.txt
+-rw-r--r--   0 juanre     (501) staff       (20)      832 2023-05-03 15:21:54.000000 catprompt-0.1.1/pyproject.toml
+-rw-r--r--   0 juanre     (501) staff       (20)       38 2023-05-03 15:23:38.623491 catprompt-0.1.1/setup.cfg
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 09:03:27.000000 catprompt-0.1.1/setup.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-03 15:23:38.623090 catprompt-0.1.1/test/
+-rw-r--r--   0 juanre     (501) staff       (20)      796 2023-04-28 10:52:58.000000 catprompt-0.1.1/test/test_example.py
+-rw-r--r--   0 juanre     (501) staff       (20)     3900 2023-05-03 14:03:45.000000 catprompt-0.1.1/test/test_prompter.py
```

### Comparing `catprompt-0.1.0/LICENSE` & `catprompt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `catprompt-0.1.0/PKG-INFO` & `catprompt-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: catprompt
-Version: 0.1.0
-Summary: Combine prompts for chatgpt.
-Author-email: Juan Reyero <juan@juanreyero.com>
-License: Copyright (c) 2018 The Python Packaging Authority
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
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # catprompt
 
 `catprompt` is a command-line tool that simplifies the process of combining prompts in different files for programming with ChatGPT. It allows users to define a system prompt along with several functionality-specific prompts, which may include files with code, into a single prompt. The prompt files can be part of the project and later be used as the seed for documentation.
 
 Using `catprompt` when developing a large program with ChatGPT offers several advantages:
 
 1. **System prompt consistency:** By having a central system prompt, you can ensure that essential information or context is consistently provided to ChatGPT across different parts of your project. This helps maintain uniformity and coherence in the responses generated by ChatGPT.
@@ -47,19 +14,51 @@
 
 5. **Documentation:** The prompt files can serve as a foundation for your project's documentation, making it easier to keep the documentation up-to-date and in sync with the code.
 
 ## Usage
 
 1. Install catprompt
 2. Create your prompt files
-3. Run catprompt with the main prompt file[s] as a command-line argument:
+3. Run catprompt with the main prompt file[s] as a command-line argument, along with any options:
+
+`catprompt [-r reverse_file] [-f flavor] path/to/prompt.txt [path/to/other-prompts.txt] [-c config_file]`
+
+4. Use the processed content from the clipboard in ChatGPT.
+
+### Options
+
+- `-c`, `--config`: Specify one or more configuration files containing private words and flavors (default: ~/.catprompt.ini and ./catprompt.ini).
+- `-r`, `--reverse`: Reverse the privatization from a given file and output the original content to stdout.
+- `-f`, `--flavor`: Use a flavor to prefix the output, extracted from the config file.
+
+## Configuration Files (ini files)
+
+Configuration files (`.ini` format) can be used to store private words and flavors. By default, catprompt looks for configuration files at `~/.catprompt.ini` and `./catprompt.ini`. You can specify other locations using the `-c` or `--config` option.
+
+### Private Words
+
+Private words are words that should be replaced with placeholders in the output. To define private words, create a section called `PrivateWords` and list them as a comma-separated string under the `list` key:
 
-`catprompt path/to/prompt.txt [path/to/other-prompts.txt]`
+```
+[PrivateWords]
+list = private_word_1, private_word_2, private_word_3
+```
+
+
+### Flavors
+
+Flavors are prefixes that can be added to the output. To define flavors, create a section called `Flavors` and list them as key-value pairs:
+
+```
+[Flavors]
+python = When programming in python follow the following rules, enclosed in ```:\n```\nAlways follow PEP-8 conventions.\n\nAlways prefer '' vs "" for strings. File names should be composed only with letters, numbers and dashes, not with underscores.\n\nThe first line of a python file is always # -*- coding: utf-8 -*-\n\nMake sure that the code formatting complies with PEP-8.\n\nUse pytest for tests.\n\nInput is from the command line whenever it makes sense. When the input is from the command line this is added at the end:\n\nif __name__ == '__main__':\n    main()\n\nand the functionality is implemented in main.
+javascript = Your setup for javascript programming.
+```
 
-4. Use the processed content from the clipboard
+You can use the `-f` or `--flavor` option to specify the desired flavor when running `catprompt`.
 
 ## Installation
 
 `pip install catprompt`
 
 or
 
@@ -70,15 +69,15 @@
 
 Make sure you have `pip` installed on your system. If not, you can find instructions on how to install pip here: https://pip.pypa.io/en/stable/installation/
 
 ## Prompt file format
 
 - Lines starting with `++` are ignored
 - Lines starting with `+=` should be followed by the name of a file to include. The file will be searched for in the directory of the original file, or in the working directory if not found there. The named file will be read, processed, and its content will replace the current line.
-- Lines starting with `+-` should be followed by the name of a file to include, and a description. The file will processed as above, and its content prefaced by a line saying "[description] follows delimited by +-----" and another line with just +-----, and followed by a line with +-----
+- Lines starting with `+-` should be followed by the name of a file to include, and a description. The file will processed as above, and its content prefaced by a line saying "[description] follows delimited by \`\`\` and another line with just \`\`\` and followed by a line with \`\`\`
 - Lines starting with `+#` will cause the current line and all following lines in the file being processed to be ignored
 - Segments of a file can be tagged by adding a line that contains :prompt:tag at the beginning, and :/prompt:tag at the end. Include them by adding [tag] after the file name.
 
 ### Example
 
 Let's consider the following example with three files:
 
@@ -127,36 +126,36 @@
 ```
 
 When running `catprompt main-prompt.txt`, the processed content will be:
 
 ```
 This is the main prompt.
 This is the sub-prompt 1.
-The snippet of code follows delimited by +-----
-+-----
+The snippet of code follows delimited by \`\`\`
+\`\`\`
 def example_function_1():
     return "F1"
 # :prompt:tag-1
 def example_function_2():
     return "F2"
 # :/prompt:tag-1
 def example_function_3():
     return "F3"
 # :prompt:tag-1
 def example_function_4():
     return "F4"
 # :/prompt:tag-1
-+-----
-The snippet of code limited to tag-1 follows delimited by +-----
-+-----
+\`\`\`
+The snippet of code limited to tag-1 follows delimited by \`\`\`
+\`\`\`
 def example_function_2():
     return "F2"
 def example_function_4():
     return "F4"
-+-----
+\`\`\`
 This is the end of the main prompt.
 ```
 
 This processed content will be copied to your clipboard, ready for use with ChatGPT.
 
 ## Use cases
```

### Comparing `catprompt-0.1.0/pyproject.toml` & `catprompt-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "catprompt"
-version = "0.1.0"
+version = "0.1.1"
 description = "Combine prompts for chatgpt."
 readme = "README.md"
 authors = [
     { name = "Juan Reyero", email="juan@juanreyero.com" }
 ]
 requires-python = ">=3.8"
 license = { file="LICENSE" }
```

### Comparing `catprompt-0.1.0/test/test_example.py` & `catprompt-0.1.1/test/test_example.py`

 * *Files identical despite different names*

### Comparing `catprompt-0.1.0/test/test_prompter.py` & `catprompt-0.1.1/test/test_prompter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import os
 from pathlib import Path
-from catprompt.prompter import process_and_copy_to_clipboard
+from catprompt.prompter import process_and_copy_to_clipboard, replace_private_words
 import clipboard
 
 
 def test_process_file():
     # Prepare test data
     test_data_dir = Path(__file__).parent / "data"
     input_file = test_data_dir / "input.txt"
@@ -92,7 +92,17 @@
     # Run process_and_copy_to_clipboard
     processed_content = process_and_copy_to_clipboard(input_file)
 
     # Compare the processed content with the expected output
     with expected_output_file.open() as f:
         expected_output = f.read().rstrip()
     assert processed_content == expected_output
+
+
+def test_replace_private_words():
+    content = "This is a test with some privateWord1 and privateWord2."
+    private_words = ["privateWord1", "privateWord2"]
+
+    expected_output = "This is a test with some private0 and private1."
+    output = replace_private_words(content, private_words)
+
+    assert output == expected_output
```

