# Comparing `tmp/gpt-review-0.3.2rc350.post1.tar.gz` & `tmp/gpt-review-0.3.2rc354.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.3.2rc350.post1.tar", last modified: Wed May  3 20:20:34 2023, max compression
+gzip compressed data, was "gpt-review-0.3.2rc354.post1.tar", last modified: Wed May  3 21:25:26 2023, max compression
```

## Comparing `gpt-review-0.3.2rc350.post1.tar` & `gpt-review-0.3.2rc354.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      336 2023-05-03 20:20:27.673009 gpt-review-0.3.2rc350.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-03 20:20:27.673009 gpt-review-0.3.2rc350.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-03 20:20:27.673009 gpt-review-0.3.2rc350.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-03 20:20:27.673009 gpt-review-0.3.2rc350.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1393 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     3879 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      898 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/LICENSE
--rw-r--r--   0        0        0     1617 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/README.md
--rw-r--r--   0        0        0     5206 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/action.yml
--rw-r--r--   0        0        0     8252 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/review.py
--rw-r--r--   0        0        0      364 2023-05-03 20:20:34.521153 gpt-review-0.3.2rc350.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    11455 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      464 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      413 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     1340 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/tests/conftest.py
--rw-r--r--   0        0        0     5645 2023-05-03 20:20:27.677009 gpt-review-0.3.2rc350.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 gpt-review-0.3.2rc350.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1367 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     3879 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      898 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/LICENSE
+-rw-r--r--   0        0        0     1617 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/README.md
+-rw-r--r--   0        0        0     5206 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/action.yml
+-rw-r--r--   0        0        0     8252 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/pyproject.toml
+-rw-r--r--   0        0        0    18646 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/review.py
+-rw-r--r--   0        0        0      366 2023-05-03 21:25:26.402929 gpt-review-0.3.2rc354.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    11455 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1312 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      464 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      413 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     1340 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/tests/conftest.py
+-rw-r--r--   0        0        0     5645 2023-05-03 21:25:19.030848 gpt-review-0.3.2rc354.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 gpt-review-0.3.2rc354.post1/PKG-INFO
```

### Comparing `gpt-review-0.3.2rc350.post1/.devcontainer/devcontainer.json` & `gpt-review-0.3.2rc354.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.3.2rc354.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/.github/dependabot.yml` & `gpt-review-0.3.2rc354.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/.github/pull_request_template.md` & `gpt-review-0.3.2rc354.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/.github/workflows/codeql.yml` & `gpt-review-0.3.2rc354.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.3.2rc354.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.3.2rc354.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
           token: ${{ secrets.PAT }}
         
       - name: Bump version and push tag
         id: tag_version
         uses: mathieudutour/github-tag-action@v6.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
-          tag_prefix: "v"
           dry_run: true
           default_bump: false
 
       - name: Set Configurations
         if: steps.tag_version.outputs.release_type
         shell: bash
         env:
```

### Comparing `gpt-review-0.3.2rc350.post1/.github/workflows/python.yml` & `gpt-review-0.3.2rc354.post1/.github/workflows/python.yml`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         with:
           ref: ${{ github.event.pull_request.head.sha }}
       - uses: Azure/login@v1.4.6
         continue-on-error: true
         with:
           creds: ${{ secrets.AZURE_CREDENTIALS }}
       - name: ${{ matrix.tools }}
-        uses: microsoft/action-python@0.6.2
+        uses: microsoft/action-python@0.6.3
         with:
           ${{ matrix.tools }}: true
           args: ${{ matrix.args }}
           workdir: '.'
           testdir: 'tests'
           python_version: '3.11.3'
           flags: ${{ matrix.flags }}
@@ -75,37 +75,37 @@
         if: steps.tag_version.outputs.release_type && github.event_name == 'release'
         shell: bash
         env:
           VERSION: ${{ steps.tag_version.outputs.previous_version }}
         run: sed -ri 's/(__version__ = ")([0-9]+\.[0-9]+\.[0-9]+?.*)(")/\1'"$VERSION"'\3/' "src/gpt_review/__init__.py" || exit 1
 
       - name: Publish Snapshot to TestPyPi
-        uses: microsoft/action-python@0.4.0
+        uses: microsoft/action-python@0.6.3
         continue-on-error: true
         if: ${{ github.event_name == 'pull_request_target' }}
         with:
           pypi_publish: true
           pypi_password: ${{ secrets.TEST_PYPI_PASSWORD  }}
           pypi_repo: testpypi
           version_suffix: -post${{ github.run_number }}-dev${{ github.run_attempt }}
           workdir: '.'
           python_version: '3.11.3'
 
       - name: Publish RC to PyPi
-        uses: microsoft/action-python@0.4.0
+        uses: microsoft/action-python@0.6.3
         if: ${{ github.event_name == 'push' }}
         with:
           pypi_publish: true
           pypi_password: ${{ secrets.PYPI_PASSWORD }}
           version_suffix: -rc${{ github.run_number }}-post${{ github.run_attempt }}
           workdir: '.'
           python_version: '3.11.3'
 
       - name: Publish Release to PyPi
-        uses: microsoft/action-python@0.4.0
+        uses: microsoft/action-python@0.6.3
         if: ${{ github.event_name == 'release' }}
         with:
           pypi_publish: true
           pypi_password: ${{ secrets.PYPI_PASSWORD }}
           workdir: '.'
           python_version: '3.11.3'
```

### Comparing `gpt-review-0.3.2rc350.post1/.github/workflows/test-action.yml` & `gpt-review-0.3.2rc354.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/.gitignore` & `gpt-review-0.3.2rc354.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/.vscode/settings.json` & `gpt-review-0.3.2rc354.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/LICENSE` & `gpt-review-0.3.2rc354.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/README.md` & `gpt-review-0.3.2rc354.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/action.yml` & `gpt-review-0.3.2rc354.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/pyproject.toml` & `gpt-review-0.3.2rc354.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/review.py` & `gpt-review-0.3.2rc354.post1/review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/src/gpt_review/_ask.py` & `gpt-review-0.3.2rc354.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.3.2rc354.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/tests/conftest.py` & `gpt-review-0.3.2rc354.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/tests/test_gpt_cli.py` & `gpt-review-0.3.2rc354.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc350.post1/PKG-INFO` & `gpt-review-0.3.2rc354.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.3.2rc350.post1
+Version: 0.3.2rc354.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.3.2rc350.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.3.2rc354.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

