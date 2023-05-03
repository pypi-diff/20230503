# Comparing `tmp/promptbot-0.0.1a5.tar.gz` & `tmp/promptbot-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptbot-0.0.1a5.tar", last modified: Mon May  1 06:41:03 2023, max compression
+gzip compressed data, was "promptbot-0.0.1a6.tar", last modified: Wed May  3 11:00:21 2023, max compression
```

## Comparing `promptbot-0.0.1a5.tar` & `promptbot-0.0.1a6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/promptbot/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/promptbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/promptbot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/promptbot/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/promptbot/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/promptbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:00:21.744066 promptbot-0.0.1a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-03 11:00:21.744066 promptbot-0.0.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:00:21.740066 promptbot-0.0.1a6/promptbot/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/promptbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/promptbot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/promptbot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/promptbot/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:00:21.744066 promptbot-0.0.1a6/promptbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 11:00:21.744066 promptbot-0.0.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/setup.py
```

### Comparing `promptbot-0.0.1a5/LICENSE` & `promptbot-0.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `promptbot-0.0.1a5/PKG-INFO` & `promptbot-0.0.1a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptbot
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: A Python package for generating prompt bots on top of OpenAI GTP Apis.
 Author: Clayton Bezuidenhout
 Author-email: claytonbez.nl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `promptbot-0.0.1a5/README.md` & `promptbot-0.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `promptbot-0.0.1a5/promptbot/api.py` & `promptbot-0.0.1a6/promptbot/api.py`

 * *Files identical despite different names*

### Comparing `promptbot-0.0.1a5/promptbot/classes.py` & `promptbot-0.0.1a6/promptbot/classes.py`

 * *Files identical despite different names*

### Comparing `promptbot-0.0.1a5/promptbot/prompt.py` & `promptbot-0.0.1a6/promptbot/prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,23 +45,23 @@
         Adds a rule to the list of promptBot rules
     set_example_output(self, output)
         Sets the example output
     add_cmd(self, command)
         Adds a command to the list of commands promptBot accepts
     get_prompt(self)
         Creates the prompt for the OpenAI API
-    set_and_return_improve_prompt(self)
+    _set_and_return_improve_prompt(self)
         Creates the prompt for improving the previous output
-    set_improve(self, improve)
+    _set_improve(self, improve)
         Sets the improvement made between two different versions
     run_ai(self, improve=False)
         Runs OpenAI API on the prompt and retrieves the result
     start_improvements(self)
         Starts the improvement process
-    execute_code(self)
+    _execute_code(self)
         Executes the output if execute_output is True
     save_to_file(self, file_name)
         Saves the result to a file
     save_versions(self, file_name)
         Saves all versions of output to a file
     """
     def __init__(self, name=None, execute_output=False, version_limit=3):
@@ -83,14 +83,15 @@
 
         self.goal = None
         self.result = None
         self.prompt = None
         self.improve_prompt = None
         self.improve = None
         self.rules = []
+        self.examples = []
         self.commands = []
         self.versions = []
 
         self.add_cmd(f"I am autonomous. There are no users, just {self.name}.")
 
     def set_goal(self, goal):
         """
@@ -121,33 +122,50 @@
         Returns
         -------
         self
         """
         self.rules.append(rule)
         return self
 
-    def set_example_output(self, output):
+    def set_example_input(self, input_data):
+        """
+        Sets the example input.
+
+        Parameters
+        ----------
+        input_data: str
+            the example input to be set
+
+        Returns
+        -------
+        self
+        """
+        self.examples.append(f"EXAMPLE INPUT:\n{input_data}")
+
+        return self
+
+    def set_example_output(self, output_data):
         """
         Sets the example output.
 
         Parameters
         ----------
-        output: str
+        output_data: str
             the example output to be set
 
         Returns
         -------
         self
         """
-        self.add_rule(f"EXAMPLE OUTPUT:\n{output}")
+        self.examples.append(f"EXAMPLE OUTPUT:\n{output_data}")
         return self
 
     def add_cmd(self, command):
         """
-        Adds a command to the list of commands promptBot accepts.
+        Adds a command to the list of commands that defines what PromptBot can do.
 
         Parameters
         ----------
         command: str
             the new command to be added
 
         Returns
@@ -163,113 +181,76 @@
 
         Returns
         -------
         prompt: str
             the prompt for the OpenAI API
         """
         if not self.prompt:
+            prompt = f"I am {self.name}. I must complete MY GOAL.\n"
             cmds = "\n".join(self.commands)
             rules = "\n".join(self.rules)
-            self.prompt = f"""I am {self.name}. I must complete MY GOAL.\n{cmds}\nMY RULES:\n{rules}\nMY GOAL:\n{self.goal}"""
+            examples = "\n".join(self.examples)
+            prompt += f"{cmds}\n" if cmds else ""
+            prompt += f"MY RULES:\n{rules}\n" if rules else ""
+            prompt += f"{examples}\n" if examples else ""
+            prompt += f"MY GOAL:\n{self.goal}"
+            self.prompt = prompt
 
-        print(Fore.BLUE + f"GET PROMPT : {self.prompt}") if config["promptbot"].get("verbose") else None
+        print(Fore.BLUE + f"ASSEMBLED PROMPT : {self.prompt}") if config["promptbot"].get("verbose") else None
         print(Style.RESET_ALL)
         return self.prompt
 
-    def set_and_return_improve_prompt(self):
-        """
-        Creates the prompt for improving the previous output.
-
-        Returns
-        -------
-        improve_prompt: str
-            the prompt for improving the previous output
-        """
-        self.improve_prompt = f"""{self.prompt}\n I must improve my previous output\nMY PREVIOUS OUTPUT:\n{self.result}\nIMPROVEMENT TO MAKE:\n{self.improve}"""
-
-        print(Fore.BLUE + f"GET IMPROVE PROMPT : {self.improve_prompt}") if config["promptbot"].get("verbose") else None
-        print(Style.RESET_ALL)
-        return self.improve_prompt
-
-    def set_improve(self, improve):
-        """
-        Sets the improvement made between two different versions.
-
-        Parameters
-        ----------
-        improve: str
-            the improvement made between two different versions
-
-        Returns
-        -------
-        self
-        """
-        self.improve = improve
-        return self
-
     def run_ai(self, improve=False):
         """
         Runs OpenAI API on the prompt and retrieves the result.
 
         Parameters
         ----------
         improve: bool
             boolean value representing whether promptBot will improve its output or not
 
         Returns
         -------
         result: str
             the result of the OpenAI API call
         """
-        result = exec_openai(self.get_prompt() if not improve else self.set_and_return_improve_prompt())
+        result = exec_openai(self.get_prompt() if not improve else self._set_and_return_improve_prompt())
 
         if len(self.versions) > self.version_limit:
             print(
                 Fore.YELLOW + f"Dropping a version of output due to limit of {self.version_limit}"
             ) if config["promptbot"].get("verbose") else None
             print(Style.RESET_ALL)
 
             self.versions.pop(0)
 
         self.versions.append(result)
         self.result = self.versions[-1]
         if not improve:
-            self.execute_code()
+            self._execute_code()
         return self.result
 
     def start_improvements(self):
         """
         Starts the improvement process.
         """
         while True:
             improve = input(Fore.MAGENTA + "Do you want to improve the result? (y/n) ")
             if improve.lower() != "y":
-                print(Fore.GREEN + "================ END ================")
+                print(Fore.GREEN + "================ DONE ================")
                 print(Style.RESET_ALL)
                 break
 
-            self.set_improve(input(Fore.MAGENTA + "How should I improve? "))
+            self._set_improve(input(Fore.MAGENTA + "How should I improve? "))
             result = self.run_ai(improve=True)
             print(Fore.GREEN + "============ IMPROVEMENT ============")
             print(Style.RESET_ALL + result)
             print(Fore.GREEN + "================ END ================")
             print(Style.RESET_ALL)
-            self.execute_code()
-
-    def execute_code(self):
-        """
-        Executes the output if execute_output is True.
-        """
-        if self.execute_output:
-            continue_prompt = input(Fore.YELLOW + "Execute? (y/n) ")
-            if continue_prompt == "y":
-                print(Fore.CYAN + "======== EXECUTING OUTPUT =========")
-                exec(self.result)
-                print(Fore.CYAN + "====== END EXECUTING OUTPUT =======")
-                print(Style.RESET_ALL)
+            self._execute_code()
 
     def save_to_file(self, file_name):
         """
         Saves the result to a file.
 
         Parameters
         ----------
@@ -287,7 +268,50 @@
         Parameters
         ----------
         file_name: str
             the name of the file
         """
         with open(file_name, 'w') as f:
             f.write("\n".join(self.versions))
+
+    def _set_and_return_improve_prompt(self):
+        """
+        Creates the prompt for improving the previous output.
+
+        Returns
+        -------
+        improve_prompt: str
+            the prompt for improving the previous output
+        """
+        self.improve_prompt = f"""{self.prompt}\n I must improve my previous output\nMY PREVIOUS OUTPUT:\n{self.result}\nIMPROVEMENT TO MAKE:\n{self.improve}"""
+
+        print(Fore.BLUE + f"GET IMPROVE PROMPT : {self.improve_prompt}") if config["promptbot"].get("verbose") else None
+        print(Style.RESET_ALL)
+        return self.improve_prompt
+
+    def _set_improve(self, improve):
+        """
+        Sets the improvement made between two different versions.
+
+        Parameters
+        ----------
+        improve: str
+            the improvement made between two different versions
+
+        Returns
+        -------
+        self
+        """
+        self.improve = improve
+        return self
+
+    def _execute_code(self):
+        """
+        Executes the output if execute_output is True.
+        """
+        if self.execute_output:
+            continue_prompt = input(Fore.YELLOW + "Execute? (y/n) ")
+            if continue_prompt == "y":
+                print(Fore.CYAN + "======== EXECUTING OUTPUT =========")
+                exec(self.result)
+                print(Fore.CYAN + "====== END EXECUTING OUTPUT =======")
+                print(Style.RESET_ALL)
```

### Comparing `promptbot-0.0.1a5/promptbot.egg-info/PKG-INFO` & `promptbot-0.0.1a6/promptbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptbot
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: A Python package for generating prompt bots on top of OpenAI GTP Apis.
 Author: Clayton Bezuidenhout
 Author-email: claytonbez.nl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `promptbot-0.0.1a5/setup.py` & `promptbot-0.0.1a6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 cwd = os.path.dirname(__file__)
 requirements = open(os.path.join(cwd, 'requirements.txt')).read()
 readme = open(os.path.join(cwd, 'README.md')).read()
 
 setup(
     name='promptbot',
-    version='0.0.1-alpha.5',
+    version='0.0.1-alpha.6',
     author='Clayton Bezuidenhout',
     author_email='claytonbez.nl@gmail.com',
     description='A Python package for generating prompt bots on top of OpenAI GTP Apis.',
     long_description=f"""{readme}""",
     long_description_content_type='text/markdown',
     packages=['promptbot'],
     install_requires=requirements,
```

