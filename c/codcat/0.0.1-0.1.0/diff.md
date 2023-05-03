# Comparing `tmp/codcat-0.0.1.tar.gz` & `tmp/codcat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codcat-0.0.1.tar", last modified: Fri Apr 14 12:00:26 2023, max compression
+gzip compressed data, was "codcat-0.1.0.tar", last modified: Wed May  3 16:23:12 2023, max compression
```

## Comparing `codcat-0.0.1.tar` & `codcat-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:00:26.313169 codcat-0.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1837 2023-04-14 12:00:11.000000 codcat-0.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-14 12:00:11.000000 codcat-0.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-04-14 12:00:11.000000 codcat-0.0.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    13829 2023-04-14 12:00:11.000000 codcat-0.0.1/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-04-14 12:00:11.000000 codcat-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3376 2023-04-14 12:00:26.313169 codcat-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2161 2023-04-14 12:00:11.000000 codcat-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:00:26.304168 codcat-0.0.1/codcat/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1617 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4188 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/downloader.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/manifest.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:00:26.307168 codcat-0.0.1/codcat/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6561 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/models/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:00:26.308169 codcat-0.0.1/codcat/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/utils/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/utils/tokenization.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-14 12:00:11.000000 codcat-0.0.1/codcat/utils/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:00:26.306168 codcat-0.0.1/codcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3376 2023-04-14 12:00:26.000000 codcat-0.0.1/codcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      822 2023-04-14 12:00:26.000000 codcat-0.0.1/codcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 12:00:26.000000 codcat-0.0.1/codcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-04-14 12:00:26.000000 codcat-0.0.1/codcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-14 12:00:26.000000 codcat-0.0.1/codcat.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-04-14 12:00:11.000000 codcat-0.0.1/codecov.yml
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-14 12:00:11.000000 codcat-0.0.1/commitlint.config.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:00:26.311169 codcat-0.0.1/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)   456701 2023-04-14 12:00:11.000000 codcat-0.0.1/notebooks/1-eda.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     7986 2023-04-14 12:00:11.000000 codcat-0.0.1/notebooks/2-preprocessing.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    25406 2023-04-14 12:00:11.000000 codcat-0.0.1/notebooks/3-bagofwords-tfidf.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   118786 2023-04-14 12:00:11.000000 codcat-0.0.1/notebooks/4-embeddings.ipynb
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 12:00:11.000000 codcat-0.0.1/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-04-14 12:00:11.000000 codcat-0.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-14 12:00:11.000000 codcat-0.0.1/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-14 12:00:11.000000 codcat-0.0.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-14 12:00:26.314169 codcat-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:00:26.313169 codcat-0.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 12:00:11.000000 codcat-0.0.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:00:26.313169 codcat-0.0.1/tests/resources/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-14 12:00:11.000000 codcat-0.0.1/tests/resources/test-manifest.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-04-14 12:00:11.000000 codcat-0.0.1/tests/test_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-04-14 12:00:11.000000 codcat-0.0.1/tests/test_estimator.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-14 12:00:11.000000 codcat-0.0.1/tests/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-04-14 12:00:11.000000 codcat-0.0.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.508141 codcat-0.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.483138 codcat-0.1.0/.dvc/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-03 16:22:58.000000 codcat-0.1.0/.dvc/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-03 16:22:58.000000 codcat-0.1.0/.dvcignore
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-05-03 16:22:58.000000 codcat-0.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-05-03 16:22:58.000000 codcat-0.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2023-05-03 16:22:58.000000 codcat-0.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    13829 2023-05-03 16:22:58.000000 codcat-0.1.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-03 16:22:58.000000 codcat-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-05-03 16:23:12.508141 codcat-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-05-03 16:22:58.000000 codcat-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.485139 codcat-0.1.0/codcat/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/manifest.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.488139 codcat-0.1.0/codcat/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7055 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/models/estimator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2888 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/pyg.py
+-rw-rw-rw-   0 root         (0) root         (0)     3828 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/tok.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.490139 codcat-0.1.0/codcat/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/utils/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/utils/tokenization.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-03 16:22:58.000000 codcat-0.1.0/codcat/utils/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.487139 codcat-0.1.0/codcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 16:23:12.000000 codcat-0.1.0/codcat.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-05-03 16:22:58.000000 codcat-0.1.0/codecov.yml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-03 16:22:58.000000 codcat-0.1.0/commitlint.config.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.492139 codcat-0.1.0/comparisons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2501 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/nn.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     6812 2023-05-03 16:22:58.000000 codcat-0.1.0/comparisons/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.493139 codcat-0.1.0/data/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-03 16:22:58.000000 codcat-0.1.0/data/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-03 16:22:58.000000 codcat-0.1.0/data/code-snippets.csv.dvc
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2023-05-03 16:22:58.000000 codcat-0.1.0/dvc.lock
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-05-03 16:22:58.000000 codcat-0.1.0/dvc.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.474138 codcat-0.1.0/eval/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.493139 codcat-0.1.0/eval/live/
+-rw-rw-rw-   0 root         (0) root         (0)     3121 2023-05-03 16:22:58.000000 codcat-0.1.0/eval/live/metrics.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.505141 codcat-0.1.0/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)   456701 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/1-eda.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7091 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/2-preprocessing.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    25406 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/3-bagofwords-tfidf.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   118990 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/4-embeddings.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     6980 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/5-sentence-transformers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     6000 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/6-code25-dataset.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    26980 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/7-code-tokenize.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)  1223000 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/8-final-evaluations.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50282 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/bigcode-datasets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17407 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/bigcode-training.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7557 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/eda-paper.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    39168 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/eval-loss.png
+-rw-rw-rw-   0 root         (0) root         (0)   249107 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/filtered-umap.png
+-rw-rw-rw-   0 root         (0) root         (0)   300932 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/full-umap.png
+-rw-rw-rw-   0 root         (0) root         (0)    47002 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/preprocessed-dataset-final-results.json
+-rw-rw-rw-   0 root         (0) root         (0)    79326 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/scc-smol-final-results.json
+-rw-rw-rw-   0 root         (0) root         (0)    79017 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/train-loss.png
+-rw-rw-rw-   0 root         (0) root         (0)   687147 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/umap-datasets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   159120 2023-05-03 16:22:58.000000 codcat-0.1.0/notebooks/wandbplot.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-03 16:22:58.000000 codcat-0.1.0/params.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-05-03 16:22:58.000000 codcat-0.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-03 16:22:58.000000 codcat-0.1.0/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-05-03 16:22:58.000000 codcat-0.1.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-03 16:23:12.509141 codcat-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.507141 codcat-0.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:23:12.508141 codcat-0.1.0/tests/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/resources/test-manifest.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/test_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/test_estimator.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-03 16:22:58.000000 codcat-0.1.0/tests/test_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-05-03 16:22:58.000000 codcat-0.1.0/tox.ini
```

### Comparing `codcat-0.0.1/.gitignore` & `codcat-0.1.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -128,7 +128,8 @@
 # Pyre type checker
 .pyre/
 
 .idea/
 .vscode/
 **/.DS_Store
 **/.pyc
+/model.onnx
```

### Comparing `codcat-0.0.1/.gitlab-ci.yml` & `codcat-0.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/.pre-commit-config.yaml` & `codcat-0.1.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     hooks:
       - id: commitlint
         stages: [ commit-msg ]
         additional_dependencies: [ '@commitlint/config-conventional' ]
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
-      - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-toml
       - id: check-merge-conflict
       - id: check-yaml
       - id: debug-statements
```

### Comparing `codcat-0.0.1/.pylintrc` & `codcat-0.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/LICENSE` & `codcat-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/PKG-INFO` & `codcat-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codcat
-Version: 0.0.1
+Version: 0.1.0
 Summary: Code snippets language classification tool
 Author-email: Konstantin Templin <1qnbhd@gmail.com>
 Maintainer-email: Konstantin Templin <1qnbhd@gmail.com>
 License: MIT
 Project-URL: Repository, https://gitlab.com/codcat/codcat
 Keywords: code,snippets,classification,language,NLP,ML
 Classifier: Intended Audience :: Science/Research
@@ -62,7 +62,11 @@
 ```
 
 ### Output
 
 ```python
 ['python' 'c']
 ```
+
+## Authors
+
+- Templin Konstantin <1qnbhd@gmail.com>
```

### Comparing `codcat-0.0.1/README.md` & `codcat-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,7 +34,11 @@
 ```
 
 ### Output
 
 ```python
 ['python' 'c']
 ```
+
+## Authors
+
+- Templin Konstantin <1qnbhd@gmail.com>
```

### Comparing `codcat-0.0.1/codcat/downloader.py` & `codcat-0.1.0/codcat/downloader.py`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/codcat/models/estimator.py` & `codcat-0.1.0/codcat/models/estimator.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,47 @@
 from typing import (
     Callable,
     List,
 )
 
 import numpy as np
 import onnxruntime as rt
+from lightgbm import LGBMClassifier
 from nltk import TweetTokenizer
-from skl2onnx import to_onnx
+from onnxmltools.convert.lightgbm.operator_converters.LightGbm import (
+    convert_lightgbm,
+)
+from skl2onnx import (
+    to_onnx,
+    update_registered_converter,
+)
 from skl2onnx.common.data_types import StringTensorType
+from skl2onnx.common.shape_calculator import (
+    calculate_linear_classifier_output_shapes,
+)
 from sklearn.utils.validation import check_is_fitted
 
 from codcat.utils.types import PathLike
 
 __all__ = [
     "Estimator",
     "SklearnEstimator",
 ]
 
 
 _DEFAULT_TOKENIZER = TweetTokenizer().tokenize
 
+update_registered_converter(
+    LGBMClassifier,
+    "LightGbmLGBMClassifier",
+    calculate_linear_classifier_output_shapes,
+    convert_lightgbm,
+    options={"nocl": [True, False], "zipmap": [True, False, "columns"]},
+)
+
 
 # noinspection PyPep8Naming
 class Estimator(metaclass=ABCMeta):
     """Abstract base class for Estimators."""
 
     @classmethod
     @abstractmethod
```

### Comparing `codcat-0.0.1/codcat/utils/dataset.py` & `codcat-0.1.0/codcat/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/codcat/utils/tokenization.py` & `codcat-0.1.0/codcat/utils/tokenization.py`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/codcat.egg-info/PKG-INFO` & `codcat-0.1.0/codcat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codcat
-Version: 0.0.1
+Version: 0.1.0
 Summary: Code snippets language classification tool
 Author-email: Konstantin Templin <1qnbhd@gmail.com>
 Maintainer-email: Konstantin Templin <1qnbhd@gmail.com>
 License: MIT
 Project-URL: Repository, https://gitlab.com/codcat/codcat
 Keywords: code,snippets,classification,language,NLP,ML
 Classifier: Intended Audience :: Science/Research
@@ -62,7 +62,11 @@
 ```
 
 ### Output
 
 ```python
 ['python' 'c']
 ```
+
+## Authors
+
+- Templin Konstantin <1qnbhd@gmail.com>
```

### Comparing `codcat-0.0.1/notebooks/1-eda.ipynb` & `codcat-0.1.0/notebooks/1-eda.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/notebooks/2-preprocessing.ipynb` & `codcat-0.1.0/notebooks/2-preprocessing.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9936755952380952%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(6, 'For now we will choose `TweetTokenizer`, in the future "*

 * *            "we will describe the preprocessing with `code_tokenize` (tree-sitter) packets.')], "*

 * *            'delete: [10, 8, 7, 6, 5]}}, delete: [2]}'}*

```diff
@@ -15,30 +15,15 @@
             "source": [
                 "Source code preprocessing has several features:\n",
                 "\n",
                 "1) Each language has its own grammar.\n",
                 "When working with source code, lexemes are usually individual words or code elements, such as variable names, function names, and operator names.\n",
                 "2) Source code preprocessing also requires certain steps that are unique to code, such as removing code comments, handling variable declarations and imports, and dealing with the peculiarities of coding languages.\n",
                 "\n",
-                "Preprocessing was done with `code_tokenize` package, `pygments`, `TweetTokenizer`, `NLTKWordTokenizer`.\n",
-                "\n",
-                "The `code_tokenize` package works best if we know the language in which we are tokenizing the source code. It also allows us to remove comments, literals and other characters. However, this method cannot be used on inference. `Pygments`, on the other hand, often offers the wrong lexical analyzer. \n",
-                "\n",
-                "For the final choice, `TweetTokenizer` was chosen based on extrinsic evaluation performance."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "057e6028-9595-490c-9d53-674db6910c92",
-            "metadata": {},
-            "source": [
-                "The `code_tokenize` package was selected to tokenize the source code during the training phase. It is based on the `tree-sitter` package, which has tokenizers for a large number of programming languages and more.\n",
-                "\n",
-                "- `code_tokenize`: https://github.com/cedricrupb/code_tokenize\n",
-                "- `tree-sitter`: https://tree-sitter.github.io/tree-sitter/"
+                "For now we will choose `TweetTokenizer`, in the future we will describe the preprocessing with `code_tokenize` (tree-sitter) packets."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "9f75909f-d27e-4aa2-bf47-be152a50f2f5",
             "metadata": {},
```

### Comparing `codcat-0.0.1/notebooks/3-bagofwords-tfidf.ipynb` & `codcat-0.1.0/notebooks/3-bagofwords-tfidf.ipynb`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/notebooks/4-embeddings.ipynb` & `codcat-0.1.0/notebooks/4-embeddings.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953993055555556%*

 * *Differences: {"'cells'": "{8: {'outputs': {0: {'data': {'text/plain': ['(12589201, 22772280)']}}}}, 18: "*

 * *            "{'execution_count': 7, 'outputs': {0: {'data': {'text/plain': ['(12586232, "*

 * *            "22772280)']}, 'execution_count': 7}}}, insert: [(19, OrderedDict([('cell_type', "*

 * *            "'code'), ('execution_count', 8), ('id', 'a8f19929-bf9e-4b10-ac17-a98ab2f9d6d3'), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            '["fst.save(\'fasttext-embeddings.bin\')"])]))]}'}*

```diff
@@ -87,15 +87,15 @@
             "execution_count": 6,
             "id": "2cb28f72-d05d-46b0-bb34-aa0175f8faba",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(12588237, 22772280)"
+                            "(12589201, 22772280)"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -247,37 +247,47 @@
             "source": [
                 "preds = clf.predict(X_test_embeddings)\n",
                 "print(classification_report(y_test, preds))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 7,
             "id": "2b19cc68-2fff-4c76-9877-b5a465fff7d4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(12588497, 22772280)"
+                            "(12586232, 22772280)"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fst = FastText(window=3, workers=16, sg=1, negative=5)\n",
                 "fst.build_vocab(corpus_iterable=train['code'].values)\n",
                 "fst.train(corpus_iterable=train['code'].values,  total_examples=train.shape[0], epochs=10)"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": 8,
+            "id": "a8f19929-bf9e-4b10-ac17-a98ab2f9d6d3",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "fst.save('fasttext-embeddings.bin')"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 18,
             "id": "846eecc5-51ce-4065-bb27-c82e66242f77",
             "metadata": {},
             "outputs": [],
             "source": [
                 "X_train_embeddings = get_emb_matrix(train['code'], fst)\n",
                 "X_test_embeddings = get_emb_matrix(test['code'], fst)"
```

### Comparing `codcat-0.0.1/pyproject.toml` & `codcat-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/tests/test_downloader.py` & `codcat-0.1.0/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/tests/test_estimator.py` & `codcat-0.1.0/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `codcat-0.0.1/tox.ini` & `codcat-0.1.0/tox.ini`

 * *Files identical despite different names*

