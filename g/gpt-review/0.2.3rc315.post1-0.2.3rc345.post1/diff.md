# Comparing `tmp/gpt-review-0.2.3rc315.post1.tar.gz` & `tmp/gpt-review-0.2.3rc345.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.2.3rc315.post1.tar", last modified: Wed May  3 06:38:52 2023, max compression
+gzip compressed data, was "gpt-review-0.2.3rc345.post1.tar", last modified: Wed May  3 20:10:34 2023, max compression
```

## Comparing `gpt-review-0.2.3rc315.post1.tar` & `gpt-review-0.2.3rc345.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      336 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2146 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     3879 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      898 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/LICENSE
--rw-r--r--   0        0        0     1617 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/README.md
--rw-r--r--   0        0        0     5206 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/action.yml
--rw-r--r--   0        0        0     8243 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/review.py
--rw-r--r--   0        0        0      364 2023-05-03 06:38:52.254541 gpt-review-0.2.3rc315.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    11461 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      464 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      413 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     1281 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/tests/conftest.py
--rw-r--r--   0        0        0     5554 2023-05-03 06:38:42.734279 gpt-review-0.2.3rc315.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 gpt-review-0.2.3rc315.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2116 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     3879 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      898 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/LICENSE
+-rw-r--r--   0        0        0     1617 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/README.md
+-rw-r--r--   0        0        0     5206 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/action.yml
+-rw-r--r--   0        0        0     8244 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/pyproject.toml
+-rw-r--r--   0        0        0    18646 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/review.py
+-rw-r--r--   0        0        0      364 2023-05-03 20:10:34.462782 gpt-review-0.2.3rc345.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    11455 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1312 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      464 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      413 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     1340 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/tests/conftest.py
+-rw-r--r--   0        0        0     5645 2023-05-03 20:10:27.158739 gpt-review-0.2.3rc345.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 gpt-review-0.2.3rc345.post1/PKG-INFO
```

### Comparing `gpt-review-0.2.3rc315.post1/.devcontainer/devcontainer.json` & `gpt-review-0.2.3rc345.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.2.3rc345.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/.github/dependabot.yml` & `gpt-review-0.2.3rc345.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/.github/pull_request_template.md` & `gpt-review-0.2.3rc345.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/.github/workflows/codeql.yml` & `gpt-review-0.2.3rc345.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.2.3rc345.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.2.3rc345.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -50,16 +50,17 @@
         with:
           python-version: 3.7
 
       - name: Install dependencies
         if: steps.tag_version.outputs.release_type
         run: |
           python -m pip install --upgrade pip
-          pip install setuptools wheel twine
-          python setup.py sdist bdist_wheel
+          python -m pip install flit
+
+          flit build
 
       - uses: "marvinpinto/action-automatic-releases@latest"
         if: steps.tag_version.outputs.release_type
         with:
           repo_token: "${{ secrets.GITHUB_TOKEN }}"
           draft: true
           automatic_release_tag: ${{ steps.tag_version.outputs.new_tag }}
```

### Comparing `gpt-review-0.2.3rc315.post1/.github/workflows/python.yml` & `gpt-review-0.2.3rc345.post1/.github/workflows/python.yml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         with:
           ref: ${{ github.event.pull_request.head.sha }}
       - uses: Azure/login@v1.4.6
         continue-on-error: true
         with:
           creds: ${{ secrets.AZURE_CREDENTIALS }}
       - name: ${{ matrix.tools }}
-        uses: microsoft/action-python@0.6.1
+        uses: microsoft/action-python@0.6.2
         with:
           ${{ matrix.tools }}: true
           args: ${{ matrix.args }}
           workdir: '.'
           testdir: 'tests'
           python_version: '3.11.3'
           flags: ${{ matrix.flags }}
```

### Comparing `gpt-review-0.2.3rc315.post1/.github/workflows/test-action.yml` & `gpt-review-0.2.3rc345.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/.gitignore` & `gpt-review-0.2.3rc345.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/.vscode/settings.json` & `gpt-review-0.2.3rc345.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/LICENSE` & `gpt-review-0.2.3rc345.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/README.md` & `gpt-review-0.2.3rc345.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/action.yml` & `gpt-review-0.2.3rc345.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/pyproject.toml` & `gpt-review-0.2.3rc345.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.10"
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
   'azure-identity',
   'azure-keyvault-secrets',
-  'llama-index<0.6.0',
+  'llama-index<=0.6.0',
   'httpx',
   'GitPython',
   'knack',
   'openai',
   'requests',
   "pyyaml",
 ]
```

### Comparing `gpt-review-0.2.3rc315.post1/review.py` & `gpt-review-0.2.3rc345.post1/review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/src/gpt_review/_ask.py` & `gpt-review-0.2.3rc345.post1/src/gpt_review/_ask.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import openai
 from azure.identity import DefaultAzureCredential
 from azure.keyvault.secrets import SecretClient
 from openai.error import RateLimitError
 from langchain.llms import AzureOpenAI
 from langchain.embeddings import OpenAIEmbeddings
 from llama_index import (
-    GPTSimpleVectorIndex,
+    GPTVectorStoreIndex,
     LangchainEmbedding,
     ServiceContext,
     LLMPredictor,
     SimpleDirectoryReader,
 )
 from llama_index.indices.base import BaseGPTIndex
 
@@ -41,29 +41,29 @@
 
     Returns:
         Dict[str, str]: The response.
     """
     documents = SimpleDirectoryReader(input_files=files).load_data()
     index = _document_indexer(documents)
 
-    return index.query(question).response  # type: ignore
+    return index.as_query_engine().query(question).response  # type: ignore
 
 
 def _document_indexer(documents) -> BaseGPTIndex:
     """
     Create a document indexer.
 
     Deployment names include: "gpt-35-turbo", "text-davinci-003"
 
     Args:
         documents (List[Document]): The documents to index.
         azure (bool): Whether to use Azure OpenAI.
 
     Returns:
-        GPTSimpleVectorIndex: The document indexer.
+        GPTVectorStoreIndex: The document indexer.
     """
     _load_azure_openai_context()
 
     llm = AzureGPT35Turbo(  # type: ignore
         deployment_name="gpt-35-turbo",
         model_kwargs={
             "api_key": openai.api_key,
@@ -73,25 +73,24 @@
         },
         max_retries=10,
     )
     llm_predictor = LLMPredictor(llm=llm)
 
     embedding_llm = LangchainEmbedding(
         OpenAIEmbeddings(
-            document_model_name="text-embedding-ada-002",
-            query_model_name="text-embedding-ada-002",
+            model="text-embedding-ada-002",
         ),  # type: ignore
         embed_batch_size=1,
     )
 
     service_context = ServiceContext.from_defaults(
         llm_predictor=llm_predictor,
         embed_model=embedding_llm,
     )
-    return GPTSimpleVectorIndex.from_documents(documents, service_context=service_context)
+    return GPTVectorStoreIndex.from_documents(documents, service_context=service_context)
 
 
 class AzureGPT35Turbo(AzureOpenAI):
     """Azure OpenAI Chat API."""
 
     @property
     @override
@@ -324,8 +323,9 @@
             )
             args.argument(
                 "files",
                 type=str,
                 help="Ask question about a file. Can be used multiple times.",
                 default=None,
                 action="append",
+                options_list=("--files", "-f"),
             )
```

### Comparing `gpt-review-0.2.3rc315.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.2.3rc345.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3rc315.post1/tests/conftest.py` & `gpt-review-0.2.3rc345.post1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,17 @@
             self.response = "test"
 
     class MockIndex:
         def query(self, question: str) -> MockQueryResponse:
             assert isinstance(question, str)
             return MockQueryResponse()
 
+        def as_query_engine(self):
+            return self
+
     def mock_create(
         engine,
         messages,
         temperature,
         max_tokens,
         top_p,
         frequency_penalty,
@@ -36,8 +39,8 @@
     ) -> MockResponse:
         return MockResponse()
 
     def from_documents(documents, service_context=None) -> MockIndex:
         return MockIndex()
 
     monkeypatch.setattr("openai.ChatCompletion.create", mock_create)
-    monkeypatch.setattr("llama_index.GPTSimpleVectorIndex.from_documents", from_documents)
+    monkeypatch.setattr("llama_index.GPTVectorStoreIndex.from_documents", from_documents)
```

### Comparing `gpt-review-0.2.3rc315.post1/tests/test_gpt_cli.py` & `gpt-review-0.2.3rc345.post1/tests/test_gpt_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     CLICase(
         f"ask how are you --fast --max-tokens={C.MAX_TOKENS_DEFAULT} --temperature {C.TEMPERATURE_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"
     ),
     CLICase(
         f"""ask how are you --fast --max-tokens {C.MAX_TOKENS_DEFAULT} --top-p {C.TOP_P_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"""
     ),
     CLICase("ask --files review.py --files review.py what programming language is this code written in?"),
+    CLICase("ask --fast -f review.py what programming language is this code written in?"),
 ]
 
 ARGS = ROOT_COMMANDS + ASK_COMMANDS
 
 
 @pytest.mark.parametrize("command", ARGS)
 @pytest.mark.cli
```

### Comparing `gpt-review-0.2.3rc315.post1/PKG-INFO` & `gpt-review-0.2.3rc345.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.2.3rc315.post1
+Version: 0.2.3rc345.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: azure-identity
 Requires-Dist: azure-keyvault-secrets
-Requires-Dist: llama-index<0.6.0
+Requires-Dist: llama-index<=0.6.0
 Requires-Dist: httpx
 Requires-Dist: GitPython
 Requires-Dist: knack
 Requires-Dist: openai
 Requires-Dist: requests
 Requires-Dist: pyyaml
 Requires-Dist: bandit[toml]==1.7.5 ; extra == "test"
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3rc315.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3rc345.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Requires-Dist: azure-identity Requires-Dist: azure-keyvault-
-secrets Requires-Dist: llama-index<0.6.0 Requires-Dist: httpx Requires-Dist:
+secrets Requires-Dist: llama-index<=0.6.0 Requires-Dist: httpx Requires-Dist:
 GitPython Requires-Dist: knack Requires-Dist: openai Requires-Dist: requests
 Requires-Dist: pyyaml Requires-Dist: bandit[toml]==1.7.5 ; extra == "test"
 Requires-Dist: black==23.3.0 ; extra == "test" Requires-Dist: check-
 manifest==0.49 ; extra == "test" Requires-Dist: flake8-bugbear==23.3.23 ; extra
 == "test" Requires-Dist: flake8-docstrings ; extra == "test" Requires-Dist:
 flake8-formatter_junit_xml ; extra == "test" Requires-Dist: flake8 ; extra ==
 "test" Requires-Dist: flake8-pyproject ; extra == "test" Requires-Dist: pre-
```

