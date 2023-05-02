# Comparing `tmp/pandasai-0.1.1.tar.gz` & `tmp/pandasai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.1.1.tar", max compression
+gzip compressed data, was "pandasai-0.2.0.tar", max compression
```

## Comparing `pandasai-0.1.1.tar` & `pandasai-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.1.1/LICENSE
--rw-r--r--   0        0        0     4082 2023-05-01 00:23:57.698037 pandasai-0.1.1/README.md
--rw-r--r--   0        0        0     4132 2023-04-30 23:39:11.591122 pandasai-0.1.1/pandasai/__init__.py
--rw-r--r--   0        0        0      512 2023-04-30 10:30:15.012968 pandasai-0.1.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.1.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1466 2023-04-30 23:41:22.772250 pandasai-0.1.1/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     2196 2023-04-30 23:43:44.275375 pandasai-0.1.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      439 2023-04-30 23:42:14.083716 pandasai-0.1.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1167 2023-04-30 10:29:36.204761 pandasai-0.1.1/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3296 2023-04-30 23:41:08.717617 pandasai-0.1.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0      635 2023-05-01 00:24:04.023587 pandasai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 pandasai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4396 2023-05-02 22:31:16.282339 pandasai-0.2.0/README.md
+-rw-r--r--   0        0        0     5966 2023-05-02 22:04:48.980512 pandasai-0.2.0/pandasai/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.0/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.0/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1466 2023-04-30 23:41:22.772250 pandasai-0.2.0/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     3128 2023-05-02 20:00:39.808930 pandasai-0.2.0/pandasai/llm/base.py
+-rw-r--r--   0        0        0      439 2023-04-30 23:42:14.083716 pandasai-0.2.0/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1167 2023-04-30 10:29:36.204761 pandasai-0.2.0/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3767 2023-05-02 20:00:39.809160 pandasai-0.2.0/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      657 2023-05-02 22:33:39.314750 pandasai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5164 1970-01-01 00:00:00.000000 pandasai-0.2.0/PKG-INFO
```

### Comparing `pandasai-0.1.1/LICENSE` & `pandasai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.1.1/README.md` & `pandasai-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 [![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai/month)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
 Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
 
 <!-- Add images/pandas-ai.png -->
+
 ![PandasAI](images/pandas-ai.png?raw=true)
 
 ## Demo
 
 Try out PandasAI in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
@@ -64,14 +65,25 @@
 
 The above code will return the following:
 
 ```
 14516000
 ```
 
+You can also ask PandasAI to draw a graph:
+
+```python
+pandas_ai.run(
+    df,
+    "Plot the histogram of countries showing for each the gpd, using different colors for each bar",
+)
+```
+
+![Chart](images/histogram-chart.png?raw=true)
+
 You can find more examples in the [examples](examples) directory.
 
 ## Environment Variables
 
 In order to set the API key for the LLM (Hugging Face Hub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
 
 ```bash
@@ -93,14 +105,15 @@
 ## License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
+For more information, please see the [contributing guidelines](CONTRIBUTING.md).
 
 ### Todo
 
 - [ ] Add support for more LLMs
 - [ ] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add unit tests
```

### Comparing `pandasai-0.1.1/pandasai/__init__.py` & `pandasai-0.2.0/pandasai/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,31 +11,49 @@
 
     _task_instruction: str = """
 There is a dataframe in pandas (python).
 The name of the dataframe is `df`.
 This is the result of `print(df.head({rows_to_display}))`:
 {df_head}.
 
-Return the python code (do not import anything) to get the answer to the following question:
+Return the python code (do not import anything) and make sure to prefix the python code with <startCode> exactly and suffix the code with <endCode> exactly 
+to get the answer to the following question :
 """
     _response_instruction: str = """
 Question: {question}
 Answer: {answer}
 
 Rewrite the answer to the question in a conversational way.
 """
+
+    _error_correct_instruction: str = """
+    For the task defined below:
+    {orig_task}
+    you generated this python code:
+    {code}
+    and this fails with the following error:
+    {error_returned}
+    Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error.
+    Make sure to prefix the python code with <startCode> exactly and suffix the code with <endCode> exactly.
+    """
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = True
     _enforce_privacy: bool = False
+    _max_retries: int = 3
+    _original_instruction_and_prompt = None
     last_code_generated: str = None
     code_output: str = None
 
     def __init__(
-        self, llm=None, conversational=True, verbose=False, enforce_privacy=False
+        self,
+        llm=None,
+        conversational=True,
+        verbose=False,
+        enforce_privacy=False,
     ):
         if llm is None:
             raise LLMNotFoundError(
                 "An LLM should be provided to instantiate a PandasAI instance"
             )
         self._llm = llm
         self._is_conversational_answer = conversational
@@ -70,46 +88,77 @@
         code = self._llm.generate_code(
             self._task_instruction.format(
                 df_head=data_frame.head(rows_to_display),
                 rows_to_display=rows_to_display,
             ),
             prompt,
         )
+        self._original_instruction_and_prompt = (
+            self._task_instruction.format(
+                df_head=data_frame.head(rows_to_display),
+                rows_to_display=rows_to_display,
+            )
+            + prompt
+        )
         self.last_code_generated = code
         self.log(
             f"""
 Code generated:
 ```
 {code}
 ```"""
         )
 
-        answer = self.run_code(code, data_frame)
+        answer = self.run_code(code, data_frame, False)
         self.code_output = answer
         self.log(f"Answer: {answer}")
 
         if is_conversational_answer is None:
             is_conversational_answer = self._is_conversational_answer
         if is_conversational_answer:
             answer = self.conversational_answer(prompt, code, answer)
             self.log(f"Conversational answer: {answer}")
         return answer
 
     def run_code(
-        self, code: str, df: pd.DataFrame  # pylint: disable=W0613 disable=C0103
+        self,
+        code: str,
+        df: pd.DataFrame,  # pylint: disable=W0613 disable=C0103
+        use_error_correction_framework: bool = False,
     ) -> str:
         # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
         """Run the code in the current context and return the result"""
 
         # Redirect standard output to a StringIO buffer
         output = io.StringIO()
         sys.stdout = output
 
         # Execute the code
-        exec(code)
+        if use_error_correction_framework:
+            count = 0
+            code_to_run = code
+            while count < self._max_retries:
+                try:
+                    exec(code_to_run)
+                    code = code_to_run
+                    break
+                except Exception as e:  # pylint: disable=W0718 disable=C0103
+                    count += 1
+                    error_correcting_instruction = (
+                        self._error_correct_instruction.format(
+                            orig_task=self._original_instruction_and_prompt,
+                            code=code,
+                            error_returned=e,
+                        )
+                    )
+                    code_to_run = self._llm.generate_code(
+                        error_correcting_instruction, ""
+                    )
+        else:
+            exec(code)
 
         # Restore standard output and get the captured output
         sys.stdout = sys.__stdout__
         captured_output = output.getvalue()
 
         # Evaluate the last line and return its value or the captured output
         lines = code.strip().split("\n")
```

### Comparing `pandasai-0.1.1/pandasai/llm/alpaca.py` & `pandasai-0.2.0/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.1.1/pandasai/llm/base.py` & `pandasai-0.2.0/pandasai/llm/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,35 +13,47 @@
 class LLM:
     """Base class to implement a new LLM."""
 
     last_prompt: str = None
 
     @property
     def type(self) -> str:
-        """Return type of llm."""
+        """
+        Return type of LLM.
+
+        Raises:
+            APIKeyNotFoundError: Type has not been implemented
+
+        Returns:
+            str: Type of LLM a string
+        """
         raise APIKeyNotFoundError("Type has not been implemented")
 
     def _remove_imports(self, code: str) -> str:
         tree = ast.parse(code)
         new_body = []
 
         for node in tree.body:
             if not isinstance(node, (ast.Import, ast.ImportFrom)):
                 new_body.append(node)
 
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree)
 
     def _polish_code(self, code: str) -> str:
-        """Polish the code:
-        - remove the leading "python" or "py"
-        - remove the imports
-        - remove trailing spaces and new lines
         """
+        Polish the code by removing the leading "python" or "py",  \
+        removing the imports and removing trailing spaces and new lines.
 
+        Args:
+            code (str): Code
+
+        Returns:
+            str: Polished code
+        """
         if re.match(r"^(python|py)", code):
             code = re.sub(r"^(python|py)", "", code)
         if re.match(r"^`.*`$", code):
             code = re.sub(r"^`(.*)`$", r"\1", code)
         self._remove_imports(code)
         code = code.strip()
         return code
@@ -50,27 +62,52 @@
         try:
             ast.parse(string)
             return True
         except SyntaxError:
             return False
 
     def _extract_code(self, response: str, separator: str = "```") -> str:
-        """Extract the code from the response"""
+        """
+        Extract the code from the response.
+
+        Args:
+            response (str): Response
+            separator (str, optional): Separator. Defaults to "```".
 
+        Raises:
+            NoCodeFoundError: No code found in the response
+
+        Returns:
+            str: Extracted code from the response
+        """
         code = response
         if len(response.split(separator)) > 1:
             code = response.split(separator)[1]
+        if re.match(r"<startCode>([\s\S]*?)<\/?endCode>", code):
+            code = re.findall(r"<startCode>([\s\S]*?)<\/?endCode>", code)[0]
         code = self._polish_code(code)
         if not self._is_python_code(code):
             raise NoCodeFoundError("No code found in the response")
 
         return code
 
-    def call(self, instruction: str, value: str) -> str:
-        """Execute the llm with the given prompt"""
+    def call(self, instruction: str, value: str) -> None:
+        """
+        Execute the LLM with given prompt.
+
+        Args:
+            instruction (str): Prompt
+            value (str): Value
 
+        Raises:
+            MethodNotImplementedError: Call method has not been implemented
+        """
         raise MethodNotImplementedError("Call method has not been implemented")
 
     def generate_code(self, instruction: str, prompt: str) -> str:
-        """Generate the code based on the instruction and the prompt"""
+        """
+        Generate the code based on the instruction and the given prompt.
 
+        Returns:
+            str: Code
+        """
         return self._extract_code(self.call(instruction, prompt))
```

### Comparing `pandasai-0.1.1/pandasai/llm/open_assistant.py` & `pandasai-0.2.0/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.1.1/pandasai/llm/openai.py` & `pandasai-0.2.0/pandasai/llm/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,23 @@
             "stop",
         ]
         for key, value in kwargs.items():
             if key in valid_params:
                 setattr(self, key, value)
 
     def completion(self, prompt: str) -> str:
-        """Query the completion API"""
+        """
+        Query the completation API
 
+        Args:
+            prompt (str): Prompt
+
+        Returns:
+            str: LLM response
+        """
         params = {
             "model": self.model,
             "prompt": prompt,
             "temperature": self.temperature,
             "max_tokens": self.max_tokens,
             "top_p": self.top_p,
             "frequency_penalty": self.frequency_penalty,
@@ -74,16 +81,23 @@
             params["stop"] = [self.stop]
 
         response = openai.Completion.create(**params)
 
         return response["choices"][0]["text"]
 
     def chat_completion(self, value: str) -> str:
-        """Query the chat completion API"""
+        """
+        Query the chat completion API
+
+        Args:
+            value (str): Prompt
 
+        Returns:
+            str: LLM response
+        """
         params = {
             "model": self.model,
             "temperature": self.temperature,
             "max_tokens": self.max_tokens,
             "top_p": self.top_p,
             "frequency_penalty": self.frequency_penalty,
             "presence_penalty": self.presence_penalty,
@@ -99,15 +113,27 @@
             params["stop"] = [self.stop]
 
         response = openai.ChatCompletion.create(**params)
 
         return response["choices"][0]["message"]["content"]
 
     def call(self, instruction: str, value: str) -> str:
-        """Call the openAI LLM"""
+        """
+        Call the OpenAI LLM.
+
+        Args:
+            instruction (str): Instruction to pass
+            value (str): Value to pass
+
+        Raises:
+            UnsupportedOpenAIModelError: Unsupported model
+
+        Returns:
+            str: Response
+        """
         self.last_prompt = str(instruction) + str(value)
 
         if self.model in self._supported_completion_models:
             response = self.completion(str(instruction) + str(value))
         elif self.model in self._supported_chat_models:
             response = self.chat_completion(str(instruction) + str(value))
         else:
```

### Comparing `pandasai-0.1.1/pyproject.toml` & `pandasai-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.1.1"
+version = "0.2.0"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 pandas = "^2.0.1"
 astor = "^0.8.1"
 openai = "^0.27.5"
+matplotlib = "^3.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 pylint = "^2.17.3"
 pytest = "^7.3.1"
```

### Comparing `pandasai-0.1.1/PKG-INFO` & `pandasai-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.1.1
+Version: 0.2.0
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PandasAI 🐼
 
@@ -22,14 +23,15 @@
 [![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai/month)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
 Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
 
 <!-- Add images/pandas-ai.png -->
+
 ![PandasAI](images/pandas-ai.png?raw=true)
 
 ## Demo
 
 Try out PandasAI in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
@@ -82,14 +84,25 @@
 
 The above code will return the following:
 
 ```
 14516000
 ```
 
+You can also ask PandasAI to draw a graph:
+
+```python
+pandas_ai.run(
+    df,
+    "Plot the histogram of countries showing for each the gpd, using different colors for each bar",
+)
+```
+
+![Chart](images/histogram-chart.png?raw=true)
+
 You can find more examples in the [examples](examples) directory.
 
 ## Environment Variables
 
 In order to set the API key for the LLM (Hugging Face Hub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
 
 ```bash
@@ -111,14 +124,15 @@
 ## License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
+For more information, please see the [contributing guidelines](CONTRIBUTING.md).
 
 ### Todo
 
 - [ ] Add support for more LLMs
 - [ ] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add unit tests
```

