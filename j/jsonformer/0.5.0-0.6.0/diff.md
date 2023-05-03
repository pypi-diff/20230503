# Comparing `tmp/jsonformer-0.5.0.tar.gz` & `tmp/jsonformer-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonformer-0.5.0.tar", max compression
+gzip compressed data, was "jsonformer-0.6.0.tar", max compression
```

## Comparing `jsonformer-0.5.0.tar` & `jsonformer-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2631 2023-05-01 19:27:44.428173 jsonformer-0.5.0/README.md
--rw-r--r--   0        0        0       85 2023-05-01 21:32:30.326739 jsonformer-0.5.0/jsonformer/__init__.py
--rw-r--r--   0        0        0     1037 2023-05-01 21:30:35.817333 jsonformer-0.5.0/jsonformer/example.py
--rw-r--r--   0        0        0      995 2023-05-01 17:24:41.244984 jsonformer-0.5.0/jsonformer/format.py
--rw-r--r--   0        0        0     1984 2023-05-01 17:24:41.245061 jsonformer-0.5.0/jsonformer/logits_processors.py
--rw-r--r--   0        0        0     6745 2023-05-01 18:48:35.415292 jsonformer-0.5.0/jsonformer/main.py
--rw-r--r--   0        0        0      498 2023-05-01 21:32:39.450479 jsonformer-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3286 1970-01-01 00:00:00.000000 jsonformer-0.5.0/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 jsonformer-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2672 2023-05-03 15:24:03.720613 jsonformer-0.6.0/README.md
+-rw-r--r--   0        0        0       85 2023-05-01 21:32:30.326739 jsonformer-0.6.0/jsonformer/__init__.py
+-rw-r--r--   0        0        0     1037 2023-05-01 21:30:35.817333 jsonformer-0.6.0/jsonformer/example.py
+-rw-r--r--   0        0        0      995 2023-05-01 17:24:41.244984 jsonformer-0.6.0/jsonformer/format.py
+-rw-r--r--   0        0        0     1984 2023-05-01 17:24:41.245061 jsonformer-0.6.0/jsonformer/logits_processors.py
+-rw-r--r--   0        0        0     6977 2023-05-03 15:24:18.507416 jsonformer-0.6.0/jsonformer/main.py
+-rw-r--r--   0        0        0      476 2023-05-03 15:25:28.274080 jsonformer-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3327 1970-01-01 00:00:00.000000 jsonformer-0.6.0/setup.py
+-rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 jsonformer-0.6.0/PKG-INFO
```

### Comparing `jsonformer-0.5.0/README.md` & `jsonformer-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.
 
-### Problem: Getting models to output structed JSON is hard
+### Problem: Getting models to output structured JSON is hard
 
 ### Solution: Only generate the content tokens and fill in the fixed tokens
 
 ![cover](img/cover4.png)
 
 Generating structured JSON from language models is a challenging task. The
 generated JSON must be syntactically correct, and it must conform to a schema
@@ -21,20 +21,21 @@
 - string
 - array
 - object
 
 ## Example
 
 ```python
+from jsonformer import Jsonformer
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 model = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")
 tokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")
 
-schema = {
+json_schema = {
     "type": "object",
     "properties": {
         "name": {"type": "string"},
         "age": {"type": "number"},
         "is_student": {"type": "boolean"},
         "courses": {
             "type": "array",
```

### Comparing `jsonformer-0.5.0/jsonformer/example.py` & `jsonformer-0.6.0/jsonformer/example.py`

 * *Files identical despite different names*

### Comparing `jsonformer-0.5.0/jsonformer/format.py` & `jsonformer-0.6.0/jsonformer/format.py`

 * *Files identical despite different names*

### Comparing `jsonformer-0.5.0/jsonformer/logits_processors.py` & `jsonformer-0.6.0/jsonformer/logits_processors.py`

 * *Files identical despite different names*

### Comparing `jsonformer-0.5.0/jsonformer/main.py` & `jsonformer-0.6.0/jsonformer/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,21 +118,30 @@
         self,
         schema: Dict[str, Any],
         obj: Union[Dict[str, Any], List[Any]],
         key: str | None = None,
     ) -> Any:
         schema_type = schema["type"]
         if schema_type == "number":
-            obj[key if key else -1] = self.generation_marker
+            if key:
+                obj[key] = self.generation_marker
+            else:
+                obj.append(self.generation_marker)
             return self.generate_number()
         elif schema_type == "boolean":
-            obj[key if key else -1] = self.generation_marker
+            if key:
+                obj[key] = self.generation_marker
+            else:
+                obj.append(self.generation_marker)
             return self.generate_boolean()
         elif schema_type == "string":
-            obj[key if key else -1] = self.generation_marker
+            if key:
+                obj[key] = self.generation_marker
+            else:
+                obj.append(self.generation_marker)
             return self.generate_string()
         elif schema_type == "array":
             new_array = []
             obj[key] = new_array
             return self.generate_array(schema["items"], new_array)
         elif schema_type == "object":
             new_obj = {}
@@ -153,17 +162,15 @@
             output = self.model.forward(input_tensor)
             logits = output.logits[0, -1]
 
             close_bracket_token_id = self.tokenizer.convert_tokens_to_ids("]")
             comma_token_id = self.tokenizer.convert_tokens_to_ids(", ")
             close_bracket_logits = logits[close_bracket_token_id]
             comma_logits = logits[comma_token_id]
-
         
-
             if close_bracket_logits > comma_logits:
                 break
 
         return obj
 
     def get_prompt(self):
         template = """{prompt}\nOutput result in the following JSON schema format:\n{schema}\nResult: {progress}"""
```

### Comparing `jsonformer-0.5.0/setup.py` & `jsonformer-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['termcolor>=2.3.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'jsonformer',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': '',
-    'long_description': '# Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.\n\n### Problem: Getting models to output structed JSON is hard\n\n### Solution: Only generate the content tokens and fill in the fixed tokens\n\n![cover](img/cover4.png)\n\nGenerating structured JSON from language models is a challenging task. The\ngenerated JSON must be syntactically correct, and it must conform to a schema\nthat specifies the structure of the JSON.\n\nCurrent approaches to this problem are brittle and error-prone. They rely on prompt engineering, fine-tuning, and post-processing, but they still fail to generate syntactically correct JSON in many cases.\n\nJsonformer is a new approach to this problem. In structured data, many tokens are fixed and predictable. Jsonformer is a wrapper around HuggingFace models that fills in the fixed tokens during the generation process, and only delegates the generation of content tokens to the language model. This makes it more efficient and bulletproof than existing approaches.\n\nThis currently supports a subset of JSON Schema. Below is a list of the supported schema types:\n\n- number\n- boolean\n- string\n- array\n- object\n\n## Example\n\n```python\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\nschema = {\n    "type": "object",\n    "properties": {\n        "name": {"type": "string"},\n        "age": {"type": "number"},\n        "is_student": {"type": "boolean"},\n        "courses": {\n            "type": "array",\n            "items": {"type": "string"}\n        }\n    }\n}\n\nprompt = "Generate a person\'s information based on the following schema:"\njsonformer = Jsonformer(model, tokenizer, json_schema, prompt)\ngenerated_data = jsonformer()\n\nprint(generated_data)\n```\n\n## Features\n\n- Bulletproof JSON generation: Jsonformer ensures that the generated JSON is always syntactically correct and conforms to the specified schema.\n- Efficiency: By generating only the content tokens and filling in the fixed tokens, Jsonformer is more efficient than generating a full JSON string and parsing it.\n- Flexible and extendable: Jsonformer is built on top of the HuggingFace transformers library, making it compatible with any model that supports the HuggingFace interface.\n\n## Installation\n\n```bash\npip install jsonformer\n```\n\n## License\n\nJsonformer is released under the MIT License. You are free to use, modify, and distribute this software for any purpose, commercial or non-commercial, as long as the original copyright and license notice are included.\n',
+    'long_description': '# Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.\n\n### Problem: Getting models to output structured JSON is hard\n\n### Solution: Only generate the content tokens and fill in the fixed tokens\n\n![cover](img/cover4.png)\n\nGenerating structured JSON from language models is a challenging task. The\ngenerated JSON must be syntactically correct, and it must conform to a schema\nthat specifies the structure of the JSON.\n\nCurrent approaches to this problem are brittle and error-prone. They rely on prompt engineering, fine-tuning, and post-processing, but they still fail to generate syntactically correct JSON in many cases.\n\nJsonformer is a new approach to this problem. In structured data, many tokens are fixed and predictable. Jsonformer is a wrapper around HuggingFace models that fills in the fixed tokens during the generation process, and only delegates the generation of content tokens to the language model. This makes it more efficient and bulletproof than existing approaches.\n\nThis currently supports a subset of JSON Schema. Below is a list of the supported schema types:\n\n- number\n- boolean\n- string\n- array\n- object\n\n## Example\n\n```python\nfrom jsonformer import Jsonformer\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\njson_schema = {\n    "type": "object",\n    "properties": {\n        "name": {"type": "string"},\n        "age": {"type": "number"},\n        "is_student": {"type": "boolean"},\n        "courses": {\n            "type": "array",\n            "items": {"type": "string"}\n        }\n    }\n}\n\nprompt = "Generate a person\'s information based on the following schema:"\njsonformer = Jsonformer(model, tokenizer, json_schema, prompt)\ngenerated_data = jsonformer()\n\nprint(generated_data)\n```\n\n## Features\n\n- Bulletproof JSON generation: Jsonformer ensures that the generated JSON is always syntactically correct and conforms to the specified schema.\n- Efficiency: By generating only the content tokens and filling in the fixed tokens, Jsonformer is more efficient than generating a full JSON string and parsing it.\n- Flexible and extendable: Jsonformer is built on top of the HuggingFace transformers library, making it compatible with any model that supports the HuggingFace interface.\n\n## Installation\n\n```bash\npip install jsonformer\n```\n\n## License\n\nJsonformer is released under the MIT License. You are free to use, modify, and distribute this software for any purpose, commercial or non-commercial, as long as the original copyright and license notice are included.\n',
     'author': '1rgs',
     'author_email': 'rgsduke@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `jsonformer-0.5.0/PKG-INFO` & `jsonformer-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: jsonformer
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: 1rgs
 Author-email: rgsduke@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.
 
-### Problem: Getting models to output structed JSON is hard
+### Problem: Getting models to output structured JSON is hard
 
 ### Solution: Only generate the content tokens and fill in the fixed tokens
 
 ![cover](img/cover4.png)
 
 Generating structured JSON from language models is a challenging task. The
 generated JSON must be syntactically correct, and it must conform to a schema
@@ -34,20 +36,21 @@
 - string
 - array
 - object
 
 ## Example
 
 ```python
+from jsonformer import Jsonformer
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 model = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")
 tokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")
 
-schema = {
+json_schema = {
     "type": "object",
     "properties": {
         "name": {"type": "string"},
         "age": {"type": "number"},
         "is_student": {"type": "boolean"},
         "courses": {
             "type": "array",
```

