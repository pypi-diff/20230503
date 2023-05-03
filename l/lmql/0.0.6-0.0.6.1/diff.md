# Comparing `tmp/lmql-0.0.6.tar.gz` & `tmp/lmql-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.6.tar", last modified: Mon May  1 11:40:54 2023, max compression
+gzip compressed data, was "lmql-0.0.6.1.tar", last modified: Wed May  3 14:15:35 2023, max compression
```

## Comparing `lmql-0.0.6.tar` & `lmql-0.0.6.1.tar`

### file list

```diff
@@ -1,241 +1,249 @@
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.527314 lmql-0.0.6/.github/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.531314 lmql-0.0.6/.github/workflows/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1594 2023-05-01 11:40:25.000000 lmql-0.0.6/.github/workflows/lmql-web.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-01 11:40:25.000000 lmql-0.0.6/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6/MANIFEST.in
--rw-rw-r--   0 luca      (1000) luca      (1000)     4949 2023-05-01 11:40:54.571313 lmql-0.0.6/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     4520 2023-05-01 11:40:25.000000 lmql-0.0.6/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.6/TODO.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.531314 lmql-0.0.6/docs/
--rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/Makefile
--rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6/docs/RELEASE.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/make.bat
--rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_ext/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/_ext/lmql_snippets.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.527314 lmql-0.0.6/docs/source/_static/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_static/css/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-04-20 08:07:08.000000 lmql-0.0.6/docs/source/_static/css/lmql-docs.css
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_static/images/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/_static/images/lmql.svg
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_static/js/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/_static/js/lmql-playground.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_templates/
--rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/_templates/layout.html
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/blog/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-01 11:40:25.000000 lmql-0.0.6/docs/source/blog/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-01 11:40:25.000000 lmql-0.0.6/docs/source/blog/release-0.0.6.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6/docs/source/conf.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/dev-setup.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     2762 2023-04-30 16:34:02.000000 lmql-0.0.6/docs/source/index.rst
--rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/installation.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/language/constraints.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6/docs/source/language/decoders.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/language/functions.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     6564 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/language/models.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/language/overview.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/language/scripted_prompts.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/logo.png
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/docs/source/python/
--rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/python/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/python/langchain.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-04-30 16:34:02.000000 lmql-0.0.6/docs/source/python/llama_index.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/python/lmql.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-04-20 08:07:08.000000 lmql-0.0.6/docs/source/python/pandas.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-04-19 15:28:18.000000 lmql-0.0.6/docs/source/python/python.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/quickstart.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/docs/source/releases/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1078 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/releases/misc-snippets.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6/docs/source/releases/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/todo.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6/pyproject.toml
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:44:31.000000 lmql-0.0.6/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/scripts/
--rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6/scripts/activate-dev.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/scripts/conda/
--rw-rw-r--   0 luca      (1000) luca      (1000)      210 2023-04-19 15:28:18.000000 lmql-0.0.6/scripts/conda/requirements-no-gpu.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      344 2023-04-19 15:28:18.000000 lmql-0.0.6/scripts/conda/requirements.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6/scripts/pypi-release.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6/scripts/wheel.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      826 2023-05-01 11:40:54.571313 lmql-0.0.6/setup.cfg
--rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-03-14 15:27:49.000000 lmql-0.0.6/setup.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/src/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/src/lmql/
--rw-rw-r--   0 luca      (1000) luca      (1000)     7077 2023-04-30 16:34:02.000000 lmql-0.0.6/src/lmql/__init__.py
--rwxrwxr-x   0 luca      (1000) luca      (1000)     8087 2023-04-25 07:30:01.000000 lmql-0.0.6/src/lmql/cli.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/demo.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/http.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.543314 lmql-0.0.6/src/lmql/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/language/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21491 2023-04-30 16:34:02.000000 lmql-0.0.6/src/lmql/language/compiler.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/language/fragment_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/language/qstrings.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/language/validator.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.543314 lmql-0.0.6/src/lmql/model/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/model/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/model/async_generation_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/model/local_client.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18118 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/model/serve.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8413 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/model/served_model.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.543314 lmql-0.0.6/src/lmql/ops/
--rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ops/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ops/follow_map.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    39435 2023-04-30 16:34:02.000000 lmql-0.0.6/src/lmql/ops/ops.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21044 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ops/token_set.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.543314 lmql-0.0.6/src/lmql/runtime/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/runtime/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/runtime/bopenai/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/bopenai/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    27642 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/bopenai/batched_openai.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    17239 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/bopenai/openai_api.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/runtime/dclib/
--rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18631 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_array.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    26024 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_global.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21668 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_model.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_rewrite.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    30560 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_seq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    20722 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/decoders.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/dclib/trie_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/hf_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    34088 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/interpreter.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/runtime/interrupt.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/runtime/langchain.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6124 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/lmql_runtime.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/runtime/maiohttp.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/masks.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/runtime/model_registry.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/multi_head_interpretation.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    47425 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/openai_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/openai_secret.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2437 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/output_writer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/runtime/postprocessing/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/runtime/postprocessing/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/postprocessing/group_by.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/program_state.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/stats.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     9327 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/tokenizer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/tests/
--rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/tests/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     5188 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/expr_test_utils.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/tests/outdated/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/mask_product_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/monotonicity.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/one_of_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/sentences_op.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/starts_with_op_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/stops_at.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/str_in_str_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/test_multi_head.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/token_set_test.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/tests/system/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/tests/system/basic_use_cases.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      971 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/tail_token_set.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2481 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/test_sample_queries.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/ui/
--rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/ui/live/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/live/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/live/live.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3340 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ui/live/live.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/live/livelib.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/live/package.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/live/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.551313 lmql-0.0.6/src/lmql/ui/playground/
--rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/.dockerignore
--rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/.env
--rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/Dockerfile
--rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.551313 lmql-0.0.6/src/lmql/ui/playground/public/
--rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/_headers
--rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/favicon.ico
--rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/public/index.html
--rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/manifest.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.563313 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/
--rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/calc.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/chat.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/cot.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/hello.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/joke.json
--rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/kv.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/list.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/meta.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/translation.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/robots.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.563313 lmql-0.0.6/src/lmql/ui/playground/public/snippets/
--rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   252806 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/ref.py
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/run-in-docker.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.567313 lmql-0.0.6/src/lmql/ui/playground/src/
--rw-rw-r--   0 luca      (1000) luca      (1000)    69215 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ui/playground/src/App.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/App.test.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/Configuration.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/DataListView.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    21284 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ui/playground/src/DecoderGraph.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/DecodingTree.js
--rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/Embed.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/Explore.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/SharedState.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3868 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/State.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5763 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/browser_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/build_info.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.567313 lmql-0.0.6/src/lmql/ui/playground/src/editor/
--rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/editor/theme.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/explore.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/graph-layout.css
--rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/index.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/index.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/logo.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/queries.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/remote_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/reportWebVitals.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/screenshot.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/setupTests.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/spinner.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/tagged-model-result.js
--rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/src/lmql/ui/vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/.gitattributes
--rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/.gitignore
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/src/lmql/ui/vscode/.vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/.vscode/launch.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/.vscodeignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/vscode/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/vscode/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/language-configuration.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/vscode/lmql-vscode.png
--rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/vscode/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/src/lmql/ui/vscode/syntaxes/
--rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/src/lmql/utils/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/utils/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5384 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/utils/graph.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/utils/nputil.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      113 2023-05-01 11:40:49.000000 lmql-0.0.6/src/lmql/version.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/src/lmql.egg-info/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4949 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     6764 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/SOURCES.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/dependency_links.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/entry_points.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/requires.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/top_level.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.847245 lmql-0.0.6.1/.github/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.847245 lmql-0.0.6.1/.github/workflows/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1594 2023-05-01 11:40:25.000000 lmql-0.0.6.1/.github/workflows/lmql-web.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-01 11:40:25.000000 lmql-0.0.6.1/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.1/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6.1/MANIFEST.in
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4969 2023-05-03 14:15:35.871245 lmql-0.0.6.1/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4538 2023-05-03 11:12:24.000000 lmql-0.0.6.1/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.6.1/TODO.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/Makefile
+-rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6.1/docs/RELEASE.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/make.bat
+-rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_ext/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/_ext/lmql_snippets.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.847245 lmql-0.0.6.1/docs/source/_static/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_static/css/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-04-20 08:07:08.000000 lmql-0.0.6.1/docs/source/_static/css/lmql-docs.css
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_static/images/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/_static/images/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_static/js/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/_static/js/lmql-playground.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/_templates/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/_templates/layout.html
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/blog/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-01 11:40:25.000000 lmql-0.0.6.1/docs/source/blog/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-01 11:40:25.000000 lmql-0.0.6.1/docs/source/blog/release-0.0.6.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6.1/docs/source/conf.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/dev-setup.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2780 2023-05-02 15:32:22.000000 lmql-0.0.6.1/docs/source/index.rst
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-18 06:55:18.000000 lmql-0.0.6.1/docs/source/installation.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/language/constraints.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6.1/docs/source/language/decoders.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/language/functions.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8252 2023-05-02 15:32:22.000000 lmql-0.0.6.1/docs/source/language/models.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-04-18 06:55:18.000000 lmql-0.0.6.1/docs/source/language/overview.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-18 06:55:18.000000 lmql-0.0.6.1/docs/source/language/scripted_prompts.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/logo.png
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/python/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/python/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-04-18 06:55:18.000000 lmql-0.0.6.1/docs/source/python/langchain.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-04-30 16:34:02.000000 lmql-0.0.6.1/docs/source/python/llama_index.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/python/lmql.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7458 2023-05-02 15:32:22.000000 lmql-0.0.6.1/docs/source/python/output.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-04-20 08:07:08.000000 lmql-0.0.6.1/docs/source/python/pandas.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-04-19 15:28:18.000000 lmql-0.0.6.1/docs/source/python/python.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/source/quickstart.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/docs/source/releases/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2263 2023-05-02 15:32:22.000000 lmql-0.0.6.1/docs/source/releases/misc-snippets.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6.1/docs/source/releases/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6.1/docs/todo.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6.1/pyproject.toml
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:44:31.000000 lmql-0.0.6.1/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/scripts/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6.1/scripts/activate-dev.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/scripts/conda/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      210 2023-04-19 15:28:18.000000 lmql-0.0.6.1/scripts/conda/requirements-no-gpu.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      344 2023-04-19 15:28:18.000000 lmql-0.0.6.1/scripts/conda/requirements.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6.1/scripts/pypi-release.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6.1/scripts/wheel.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      828 2023-05-03 14:15:35.871245 lmql-0.0.6.1/setup.cfg
+-rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-03-14 15:27:49.000000 lmql-0.0.6.1/setup.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/src/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.851245 lmql-0.0.6.1/src/lmql/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5586 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/__init__.py
+-rwxrwxr-x   0 luca      (1000) luca      (1000)     7998 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/cli.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/demo.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/http.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/language/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21499 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/language/compiler.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/language/fragment_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/language/qstrings.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/language/validator.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/model/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/model/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/model/async_generation_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/model/local_client.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18118 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/model/serve.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8052 2023-05-02 15:48:30.000000 lmql-0.0.6.1/src/lmql/model/served_model.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/ops/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ops/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/ops/follow_map.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    39574 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/ops/ops.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21044 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/ops/token_set.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/output/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       57 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/output/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2313 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/output/http.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1889 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/output/sse.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2282 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/output/ws.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/runtime/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/runtime/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/runtime/bopenai/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/bopenai/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28384 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/runtime/bopenai/batched_openai.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    17221 2023-05-03 11:12:24.000000 lmql-0.0.6.1/src/lmql/runtime/bopenai/openai_api.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql/runtime/dclib/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18631 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_array.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    26433 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_global.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21721 2023-05-02 16:00:00.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_model.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_rewrite.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    30560 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_seq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20722 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/decoders.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/dclib/trie_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/hf_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    34019 2023-05-03 11:12:24.000000 lmql-0.0.6.1/src/lmql/runtime/interpreter.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/runtime/interrupt.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/runtime/langchain.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6367 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/runtime/lmql_runtime.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/runtime/maiohttp.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/masks.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/runtime/model_registry.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/multi_head_interpretation.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    42592 2023-05-03 11:12:24.000000 lmql-0.0.6.1/src/lmql/runtime/openai_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/openai_secret.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4042 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/runtime/output_writer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/runtime/postprocessing/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/runtime/postprocessing/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/postprocessing/group_by.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/program_state.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/runtime/stats.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9327 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/runtime/tokenizer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/tests/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/tests/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5188 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/expr_test_utils.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/tests/outdated/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/mask_product_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/monotonicity.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/one_of_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/sentences_op.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/starts_with_op_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/stops_at.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/str_in_str_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/test_multi_head.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/outdated/token_set_test.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/tests/system/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/tests/system/basic_use_cases.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      971 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/tail_token_set.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      788 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/tests/test_back2back_caching.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2481 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/tests/test_sample_queries.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/ui/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/ui/live/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/live/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/live/live.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3346 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/ui/live/live.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/live/livelib.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/live/package.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/live/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/ui/playground/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/.dockerignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/.env
+-rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/Dockerfile
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.859245 lmql-0.0.6.1/src/lmql/ui/playground/public/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/_headers
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/favicon.ico
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/index.html
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/manifest.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.867245 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/list.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/robots.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.867245 lmql-0.0.6.1/src/lmql/ui/playground/public/snippets/
+-rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   184008 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/ref.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/run-in-docker.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.867245 lmql-0.0.6.1/src/lmql/ui/playground/src/
+-rw-rw-r--   0 luca      (1000) luca      (1000)    69135 2023-05-03 14:14:45.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/App.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/App.test.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/Configuration.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/DataListView.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21319 2023-05-03 11:12:24.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/DecodingTree.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/Embed.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/Explore.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/SharedState.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3868 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/State.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5763 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/browser_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/build_info.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.867245 lmql-0.0.6.1/src/lmql/ui/playground/src/editor/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/editor/theme.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/explore.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/graph-layout.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/index.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/index.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/logo.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/queries.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/remote_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/screenshot.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/setupTests.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/spinner.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/playground/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/src/lmql/ui/vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/.gitattributes
+-rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/.gitignore
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/src/lmql/ui/vscode/.vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/.vscode/launch.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/.vscodeignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/vscode/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/vscode/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/language-configuration.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/vscode/lmql-vscode.png
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/ui/vscode/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.871245 lmql-0.0.6.1/src/lmql/utils/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.1/src/lmql/utils/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-02 15:32:22.000000 lmql-0.0.6.1/src/lmql/utils/docstring_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5384 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql/utils/graph.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-01 11:40:25.000000 lmql-0.0.6.1/src/lmql/utils/nputil.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-05-03 14:15:30.000000 lmql-0.0.6.1/src/lmql/version.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-03 14:15:35.855245 lmql-0.0.6.1/src/lmql.egg-info/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4969 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6969 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/SOURCES.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/dependency_links.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/entry_points.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/requires.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-05-03 14:15:35.000000 lmql-0.0.6.1/src/lmql.egg-info/top_level.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6.1/src/lmql.svg
```

### Comparing `lmql-0.0.6/.github/workflows/lmql-web.yml` & `lmql-0.0.6.1/.github/workflows/lmql-web.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/.gitignore` & `lmql-0.0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/LICENSE` & `lmql-0.0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/PKG-INFO` & `lmql-0.0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
     ·
     <a href="https://lmql.ai/playground">Playground IDE</a>
     ·
     <a href="https://github.com/eth-sri/lmql/issues">Report Bug</a>
     <br/>
     <br/>
     <a href="https://discord.gg/7eJP4fcyNT"><img src="https://img.shields.io/discord/1091288833997410414?style=plastic&logo=discord&color=blueviolet&logoColor=white" height=18/></a>
-    <a href="https://badge.fury.io/py/Lmql"><img src="https://badge.fury.io/py/Lmql.svg" alt="PyPI version" height=18></a>
+    <a href="https://badge.fury.io/py/Lmql"><img src="https://badge.fury.io/py/Lmql.svg?cacheSeconds=3600" alt="PyPI version" height=18></a>
   </p>
 </div>
 
 LMQL is a query language for large language models (LLMs). It facilitates LLM interaction by combining the benefits of natural language prompting with the expressiveness of Python. With only a few lines of LMQL code, users can express advanced, multi-part and tool-augmented LM queries, which then are optimized by the LMQL runtime to run efficiently as part of the LM decoding loop.
 
 ![lmql-overview](https://user-images.githubusercontent.com/17903049/222918379-84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.1 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.6/README.md` & `lmql-0.0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ·
     <a href="https://lmql.ai/playground">Playground IDE</a>
     ·
     <a href="https://github.com/eth-sri/lmql/issues">Report Bug</a>
     <br/>
     <br/>
     <a href="https://discord.gg/7eJP4fcyNT"><img src="https://img.shields.io/discord/1091288833997410414?style=plastic&logo=discord&color=blueviolet&logoColor=white" height=18/></a>
-    <a href="https://badge.fury.io/py/Lmql"><img src="https://badge.fury.io/py/Lmql.svg" alt="PyPI version" height=18></a>
+    <a href="https://badge.fury.io/py/Lmql"><img src="https://badge.fury.io/py/Lmql.svg?cacheSeconds=3600" alt="PyPI version" height=18></a>
   </p>
 </div>
 
 LMQL is a query language for large language models (LLMs). It facilitates LLM interaction by combining the benefits of natural language prompting with the expressiveness of Python. With only a few lines of LMQL code, users can express advanced, multi-part and tool-augmented LM queries, which then are optimized by the LMQL runtime to run efficiently as part of the LM decoding loop.
 
 ![lmql-overview](https://user-images.githubusercontent.com/17903049/222918379-84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
```

### Comparing `lmql-0.0.6/docs/Makefile` & `lmql-0.0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/make.bat` & `lmql-0.0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/_ext/lmql_snippets.py` & `lmql-0.0.6.1/docs/source/_ext/lmql_snippets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.6.1/docs/source/_static/css/lmql-docs.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/_static/images/lmql.svg` & `lmql-0.0.6.1/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.6.1/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/blog/release-0.0.5.md` & `lmql-0.0.6.1/docs/source/blog/release-0.0.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/blog/release-0.0.6.md` & `lmql-0.0.6.1/docs/source/blog/release-0.0.6.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/conf.py` & `lmql-0.0.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/dev-setup.md` & `lmql-0.0.6.1/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/index.rst` & `lmql-0.0.6.1/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -71,23 +71,24 @@
    
    language/overview.md
    language/scripted_prompts.md
    language/constraints.md
    language/decoders.md
    language/models.md
    language/functions.md
-   
+
 .. toctree::
     :maxdepth: 1
     :caption: 🔗 Python Integration
     
     python/python.ipynb
     python/langchain.ipynb
     python/llama_index.ipynb
     python/pandas.ipynb
+    python/output.md
    
 .. toctree::
     :maxdepth: 1
     :caption: 💬 Contribute
     
     dev-setup
     Discord <https://discord.gg/7eJP4fcyNT>
```

#### html2text {}

```diff
@@ -20,12 +20,12 @@
 ð¬_Discord_Server ð¥_Twitter âï¸_E-Mail
 Contents -------- .. toctree:: :maxdepth: 1 quickstart installation â¡ï¸
 Playground IDE
 lmql.ai/playground> .. toctree:: :maxdepth: 1 :caption: ð LMQL Language
 language/overview.md language/scripted_prompts.md language/constraints.md
 language/decoders.md language/models.md language/functions.md .. toctree:: :
 maxdepth: 1 :caption: ð Python Integration python/python.ipynb python/
-langchain.ipynb python/llama_index.ipynb python/pandas.ipynb .. toctree:: :
-maxdepth: 1 :caption: ð¬ Contribute dev-setup Discord
+langchain.ipynb python/llama_index.ipynb python/pandas.ipynb python/output.md
+.. toctree:: :maxdepth: 1 :caption: ð¬ Contribute dev-setup Discord
 discord.gg/7eJP4fcyNT> GitHub Issues
 github.com/eth-sri/lmql/issues> E-Mail
 lmql.ai>
```

### Comparing `lmql-0.0.6/docs/source/installation.md` & `lmql-0.0.6.1/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/language/constraints.md` & `lmql-0.0.6.1/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/language/decoders.md` & `lmql-0.0.6.1/docs/source/language/decoders.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/language/functions.md` & `lmql-0.0.6.1/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/language/models.md` & `lmql-0.0.6.1/docs/source/language/models.md`

 * *Files 23% similar despite different names*

```diff
@@ -14,35 +14,61 @@
 * `openai/text-curie-001`
 * `openai/text-babbage-001`
 * `openai/text-davinci-00[1-3]`
 
 * `openai/gpt-3.5-turbo` also available as `chatgpt`
 * `openai/gpt-4` also available as `gpt-4`
 
-### OpenAI API Limitations
-
-Unfortunately, the OpenAI API Completions and Chat API are severely limited in terms of token masking and the availability of the token distribution per predicted token. LMQL tries to leverage these APIs as much as possible, but there are some limitations that we have to work around and may affect users:
-
-* The **OpenAI Completion API limits the number of possible logit biases to 300**. This means, if your constraints induce token masks that are larger than 300 tokens, LMQL will automatically truncate the token mask to the first 300 tokens. This may lead to unexpected behavior, e.g., model performance may be worse than expected as the masks are truncated to be more restrictive than necessary. In cases where the 300 biases limit is exceeded, LMQL prints a warning message to the console, indicating that the logit biases were truncated.
-
-* The **OpenAI Completions API only provides the top-5 logprobs per predicted token**. This means that decoding algorithms that explore e.g. the top-n probabilities to make decisions like beam search, are limited to a branching factor of 5.
-
-* The **OpenAI Chat API does not provide any way to mask tokens or obtain the token distribution (ChatGPT, GPT-4)**. Simple constraints can still be enforced, as the LMQL runtime optimizes them to fit the OpenAI API. However, more complex constraints may not be enforceable. In these cases, LMQL will print a error message to the console. As a workaround users may then adjust their constraints to fit these API limitations or resort to post-processing and backtracking. Scripted prompting, intermediate instructions and simple constraints are still supported with Chat API models, nonetheless.
-
 ### Configuring OpenAI API Credentials
 
 If you want to use OpenAI models, you have to configure your API credentials. To do so you can either define the `OPENAI_API_KEY` environment variable or create a file `api.env` in the active working directory, with the following contents.
 
 ```
 openai-org: <org identifier>
 openai-secret: <api secret>
 ```
 
 For system-wide configuration, you can also create an `api.env` file at `$HOME/.lmql/api.env` or at the project root of your LMQL distribution (e.g. `src/` in a development copy).
 
+### Monitoring OpenAI API use
+
+When working with OpenAI models, it is important to keep track of your API usage. LMQL offers a couple of ways to see what is happening internally and how many API calls are being made.
+
+#### Playground
+
+In the playground in the bottom right of the query editor, you can see real-time query statistics, including no. of requests, tokens and estimated cost when using OpenAI models:
+
+<img src="https://user-images.githubusercontent.com/17903049/233836413-7e8ac978-4038-4b8e-a690-7090d8695513.png" height="50"/>
+
+This information is automatically updated as your query is being executed. If you want to see the same information in Python, you can use the following snippet.
+
+#### OpenAI Usage Statistics in Python
+
+To obtain the same information in Python, you can use the following snippet:
+
+```python
+from lmql.runtime.bopenai import get_stats
+print(get_stats())
+# OpenAI API Stats: 1 requests, 0 errors, 9 tokens, 1.0 average batch size
+```
+
+The `tokens` metric here refers to the number of tokens that were consumed and generated by the model.
+
+#### API Request Logging
+
+Additionally, you may be interested in seeing the actual API requests that are made in the background. To show these, there is a decoder option `chatty_openai=True`, which enables verbose logging and will print all OpenAI request payloads console, e.g. a query like this:
+
+```{lmql}
+name::chatty_openai
+argmax(chatty_openai=True) "Hello[WHO]" from "openai/text-ada-001" where STOPS_AT(WHO, "\n")
+
+model-output::
+Completion with {'model': 'text-ada-001', 'prompt': \[550256, 15496], 'max_tokens': 64, 'temperature': 0, 'logprobs': 5, 'user': 'lmql', 'stream': True, 'echo': True}
+```
+
 ### Configuring Speculative OpenAI API Use
 
 To integrate the OpenAI API with LMQL, we rely on speculative prediction, where LMQL applies token masking and stopping conditions less eagerly, to save API calls. 
 
 To achieve this, output is generated in chunks, where each chunk is verified to satisfy the constraints before generation continues. The chunk size can be configured by passing `openai_chunksize` parameter in the decoding clause like so:
 
 ```{lmql}
@@ -54,14 +80,24 @@
     "openai/text-ada-001"
 where
     STOPS_AT(COMPLETION, ".")
 ```
 
 By default, the chunk size is set to 32. This value is chosen based on the consideration, that a very large chunk size means that LMQL potentially has to discard many generated tokens (which is expensive), if a constraint is violated early on. However, if a query has few or only stopping phrase constraints, a larger chunk size may be beneficial for overall query cost. In general, if a query requires multiple long, uninterrupted sequences to be generated without imposing many constraints, a larger chunk size is recommended.
 
+
+### OpenAI API Limitations
+
+Unfortunately, the OpenAI API Completions and Chat API are severely limited in terms of token masking and the availability of the token distribution per predicted token. LMQL tries to leverage these APIs as much as possible, but there are some limitations that we have to work around and may affect users:
+
+* The **OpenAI Completion API limits the number of possible logit biases to 300**. This means, if your constraints induce token masks that are larger than 300 tokens, LMQL will automatically truncate the token mask to the first 300 tokens. This may lead to unexpected behavior, e.g., model performance may be worse than expected as the masks are truncated to be more restrictive than necessary. In cases where the 300 biases limit is exceeded, LMQL prints a warning message to the console, indicating that the logit biases were truncated.
+
+* The **OpenAI Completions API only provides the top-5 logprobs per predicted token**. This means that decoding algorithms that explore e.g. the top-n probabilities to make decisions like beam search, are limited to a branching factor of 5.
+
+* The **OpenAI Chat API does not provide any way to mask tokens or obtain the token distribution (ChatGPT, GPT-4)**. Simple constraints can still be enforced, as the LMQL runtime optimizes them to fit the OpenAI API. However, more complex constraints may not be enforceable. In these cases, LMQL will print a error message to the console. As a workaround users may then adjust their constraints to fit these API limitations or resort to post-processing and backtracking. Scripted prompting, intermediate instructions and simple constraints are still supported with Chat API models, nonetheless.
 ## 🤗 Transformers Models
 
 LMQL also support locally-hosted models via [🤗 Transformers](https://huggingface.co/transformers). This includes all models that are available via the [🤗 Transformers Model Hub](https://huggingface.co/models) and conform to the AutoModelForCausalLM API. Examples include `gpt2` or `facebook/opt-30B`.
 
 The API limitations mentioned above do not apply to locally-hosted models, as the LMQL runtime can leverage the full power of the 🤗 Transformers API and access the full token distribution, enforcing token masks of arbitrary size.
 
 ### Running LMQL with 🤗 Transformers
```

### Comparing `lmql-0.0.6/docs/source/language/overview.md` & `lmql-0.0.6.1/docs/source/language/overview.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/language/scripted_prompts.md` & `lmql-0.0.6.1/docs/source/language/scripted_prompts.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/lmql.svg` & `lmql-0.0.6.1/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/logo.png` & `lmql-0.0.6.1/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/python/langchain.ipynb` & `lmql-0.0.6.1/docs/source/python/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/python/llama_index.ipynb` & `lmql-0.0.6.1/docs/source/python/llama_index.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/python/lmql.txt` & `lmql-0.0.6.1/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/python/pandas.ipynb` & `lmql-0.0.6.1/docs/source/python/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/python/python.ipynb` & `lmql-0.0.6.1/docs/source/python/python.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/docs/source/quickstart.md` & `lmql-0.0.6.1/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/scripts/wheel.sh` & `lmql-0.0.6.1/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/setup.cfg` & `lmql-0.0.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.6
+version = 0.0.6.1
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.0.6/src/lmql/__init__.py` & `lmql-0.0.6.1/src/lmql/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 __license__ = "MIT"
 
 import os
 import tempfile
 
 import lmql.runtime.lmql_runtime as lmql_runtime
 import lmql.runtime.lmql_runtime as runtime_support
+from lmql.utils.docstring_parser import *
 from lmql.language.compiler import LMQLCompiler
 # re-export lmql runtime functions
 from lmql.runtime.lmql_runtime import (FunctionContext, LMQLInputVariableScope,
                                        LMQLQueryFunction, compiled_query, tag)
 from lmql.runtime.model_registry import LMQLModelRegistry
 from lmql.runtime.output_writer import headless, printing, silent, stream
 from lmql.runtime.interpreter import LMQLResult
@@ -106,72 +107,26 @@
         
 def _query_from_string(s):
     temp_lmql_file = tempfile.mktemp(suffix=".lmql")
     with open(temp_lmql_file, "w") as f:
         f.write(s)
     module = load(temp_lmql_file, autoconnect=True, output_writer=silent)
     return module.query
-        
-def _get_decorated_function_code(fct):
-    import ast
-    import inspect
-
-    source = ""
-
-    try:
-        source = inspect.getsource(fct)
-        tree = ast.parse(source)
-        docstring_element = tree.body[0].body[0].value
-        docstring = docstring_element.s
-        # get range of source that corresonds to the docstring
-        start = docstring_element.lineno
-        end = docstring_element.end_lineno
-        startcol = docstring_element.col_offset
-        endcol = docstring_element.end_col_offset
-        
-        # get source code of the function
-        source = source.splitlines()
-
-        # remove common indent
-        common_indent = None
-        lines = []
-        for line in source[start-1:end]:
-            if line.strip() == "" or line.strip() == '"""lmql' or line.strip() == "'''lmql":
-                lines.append(line)
-                continue
-            if common_indent is None:
-                common_indent = len(line) - len(line.lstrip())
-            else:
-                common_indent = min(common_indent, len(line) - len(line.lstrip()))
-            lines.append(line[common_indent:])
-        lines[0] = lines[0][startcol - common_indent:]
-        lines[-1] = lines[-1][:endcol]
-
-        source = "\n".join(lines)
-
-        quote_types = "'''" if source.endswith("'''") else '"""'
-        if source.lstrip().startswith(quote_types):
-            source = source.lstrip()[len(quote_types):]
-        assert source.endswith(quote_types), f"Docstring of @lmql.query function {fct.__name__} must be on the first line of the function, but is:\n {source}"
-        source = source[:-len(quote_types)].strip("\n")
-    except:
-        raise RuntimeError("Failed to parse docstring of query function as LMQL code:\n\n" + str(source))
-
-    return source
-
 
 def query(fct):
     import inspect
 
+    if type(fct) is LMQLQueryFunction: return fct
+
     # support for lmql.query(<query string>)
     if type(fct) is str: return _query_from_string(fct)
     
     calling_frame = inspect.stack()[1]
     scope = LMQLInputVariableScope(fct, calling_frame)
-    code = _get_decorated_function_code(fct)
+    code = get_decorated_function_code(fct)
 
     temp_lmql_file = tempfile.mktemp(suffix=".lmql")
     with open(temp_lmql_file, "w") as f:
         f.write(code)
     module = load(temp_lmql_file, autoconnect=True, output_writer=silent)
     
     assert inspect.iscoroutinefunction(fct), f"@lmql.query {fct.__name__} must be declared async."
@@ -190,8 +145,18 @@
     return module.query
 
 async def static_prompt(query_fct, *args, **kwargs):
     """
     Returns the static prompt prefix that is generated by the given query function up until the first variable.
     """
     res = await query_fct(*args, **kwargs, return_prompt_string=True)
-    return res[0]
+    return res[0]
+
+def main(query_fct):
+    """
+    Runs the provided query function in the main thread
+    and returns the result.
+
+    This call is blocking.
+    """
+    import asyncio
+    return asyncio.run(query_fct())
```

### Comparing `lmql-0.0.6/src/lmql/cli.py` & `lmql-0.0.6.1/src/lmql/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,16 @@
     parser.add_argument("--no-clear", action="store_true", dest="no_clear", help="don't clear inbetween printing results")
     parser.add_argument("--no-realtime", action="store_true", dest="no_realtime", help="don't print text as it's being generated")
     parser.add_argument("--time", action="store_true", dest="time", help="Time the query.")
 
     args = parser.parse_args(sys.argv[2:])
 
     absolute_path = os.path.abspath(args.lmql_file)
-    from lmql.runtime.output_writer import PrintingDebuggerOutputWriter
 
-    writer = PrintingDebuggerOutputWriter()
+    writer = lmql.printing
     writer.clear = not args.no_clear
     writer.print_output = not args.no_realtime
 
     if os.path.exists(absolute_path):
         results = asyncio.run(lmql.run_file(absolute_path, output_writer=writer))
     else:
         code = args.lmql_file
```

### Comparing `lmql-0.0.6/src/lmql/demo.py` & `lmql-0.0.6.1/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/http.py` & `lmql-0.0.6.1/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/language/compiler.py` & `lmql-0.0.6.1/src/lmql/language/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     def transform_node(self, expr, snf):
         if type(expr) is ast.BoolOp:
             if type(expr.op) is ast.And or type(expr.op) is ast.Or:
                 ops = expr.values
                 tops = [self.transform_node(op, snf) for op in ops]
                 tops_list = ",\n  ".join([t.strip() or "None" for t in tops])
                 
-                Op = "lmql.runtime_support.AndOp" if type(expr.op) is ast.And else "lmql.OrOp"
+                Op = f"{OPS_NAMESPACE}.AndOp" if type(expr.op) is ast.And else f"{OPS_NAMESPACE}.OrOp"
                 return snf.add(f"{Op}([\n  {tops_list}\n])")
         # elif type(expr) is ast.Call:
         #     tfunc = self.transform_node(expr.func, snf)
         #     targs = [self.transform_node(a, snf) for a in expr.args]
         #     targs_list = ", ".join(targs)
         #     return f"{tfunc}({targs_list})"
         elif type(expr) is ast.Name:
```

### Comparing `lmql-0.0.6/src/lmql/language/fragment_parser.py` & `lmql-0.0.6.1/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/language/qstrings.py` & `lmql-0.0.6.1/src/lmql/language/qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/language/validator.py` & `lmql-0.0.6.1/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/model/async_generation_utils.py` & `lmql-0.0.6.1/src/lmql/model/async_generation_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/model/local_client.py` & `lmql-0.0.6.1/src/lmql/model/local_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/model/serve.py` & `lmql-0.0.6.1/src/lmql/model/serve.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/model/served_model.py` & `lmql-0.0.6.1/src/lmql/model/served_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,25 +57,14 @@
                 "tokens": self.billable_tokens,
                 "model": self.model_identifier
             }
             if decoder_step is not None:
                 data["_step"] = decoder_step
             printer.report_model_stats(**data)
 
-    async def generate(self, input_ids=None, *args, **kwargs):
-        self.num_generate_calls += 1
-        
-        result = await super().generate(*args, input_ids=input_ids, **kwargs)
-        
-        if torch.is_tensor(result): ids = result
-        else: ids = result["sequences"]
-        self.billable_tokens += ids.numel()
-        
-        return result
-
     def create_result_processor_task_if_required(self):
         if self.result_process_running: 
             return
         
         loop = asyncio.get_event_loop()
         loop.create_task(self.result_processor())
         self.result_process_running = True
```

### Comparing `lmql-0.0.6/src/lmql/ops/follow_map.py` & `lmql-0.0.6.1/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ops/ops.py` & `lmql-0.0.6.1/src/lmql/ops/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -836,18 +836,14 @@
         var_op.diff_aware_read = True
         return super().execute_predecessors(trace, context)
     
     @property
     def variable(self):
         return self.predecessors[0]
 
-    @property
-    def stopping_phrase(self):
-        return self.predecessors[1]
-
     async def stopping_phrase_tokenized(self, tokenizer):
         if tokenizer in self._tokenized_stopping_phrase_cache:
             return self._tokenized_stopping_phrase_cache[tokenizer]
         else:
             result = (await tokenizer(self.stopping_phrase))
             self._tokenized_stopping_phrase_cache[tokenizer] = result
             return result
@@ -945,14 +941,18 @@
     def postprocess(self, operands, value):
         op2 = operands[1]
         matched_phrase_index = value.find(op2)
         if matched_phrase_index != -1:
             value = value[:matched_phrase_index]
 
         return postprocessed_rewrite(value), postprocessed_value(value)
+    
+    @property
+    def stopping_phrase(self):
+        return self.predecessors[1]
 
 class OpaqueLambdaOp(Node):
     def forward(self, *args, **kwargs):
         if any([a is None for a in args]): return None
         fct, *args = args
         return fct(*args)
     
@@ -1034,23 +1034,28 @@
 
 def execute_op_stops_at_only(op: Node, result=None):
     """
     Evaluates a Node and returns the list of defined StopAtOps for the query.
     """
     if result is None: result = []
 
-    if type(op) is StopAtOp:
+    if type(op) is StopBeforeOp:
         result.append(op)
     elif type(op) is AndOp:
         for p in op.predecessors:
             execute_op_stops_at_only(p, result=result)
     elif type(op) is OrOp:
-        # TODO: actually STOPS_AT in OR is not really supported yet
+        subresults = []
         for p in op.predecessors:
-            execute_op_stops_at_only(p, result=result)
+            subresult = []
+            execute_op_stops_at_only(p, result=subresult)
+            subresults.append(subresult)
+        # intersect subresults
+        result += list(set.intersection(*[set(r) for r in subresults]))
+
     else:
         # other ops are no-ops from a STOPS_AT perspective (cannot contain additional STOPS_AT ops)
         # TODO: what about not
         return []
     return result
 
 def execute_postprocess(op: Node, var_name: str, value: str, trace=None, context=None):
```

### Comparing `lmql-0.0.6/src/lmql/ops/token_set.py` & `lmql-0.0.6.1/src/lmql/ops/token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.6.1/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.6.1/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,26 +178,15 @@
 
                 for c in data["choices"]:
                     index = c["index"]
 
                     self.stats.tokens += len(c["logprobs"]["tokens"])
                     assert c is not None
                     self.slices[index].digest(c)
-                    
-                    if c["finish_reason"] == "stop":
-                        # "<|endoftext|>", "<|endoftext|>", 0.0
-                        self.slices[index].digest({
-                            "text": "<|endoftext|>",
-                            "logprobs": {
-                                "text_offset": [0],
-                                "token_logprobs": [0.0],
-                                "tokens": ["<|endoftext|>"],
-                                "top_logprobs": [{"<|endoftext|>": 0.0}]
-                            }
-                        })
+                    self.slices[index].finish_reason = c["finish_reason"]
                     
                     # logprobs.tokens, text, logprobs.token_logprobs
             for c in self.slices:
                 c.finish()
         except Exception as e:
             print("Failed with", e)
             for c in self.slices:
@@ -359,16 +348,15 @@
 
 class ResponseStreamSliceIterator:
     def __init__(self, slice):
         self.slice = slice
         self.retries = 0
         self.text = ""
         self.consumed_tokens = []
-
-        self.done = asyncio.Event()
+        self.n = 0
 
     async def recover(self):
         recovery_kwargs = self.slice.kwargs.copy()
         # reconstruct the prompt by tokenizing the consumed tokens
         if len(self.consumed_tokens) > 0:
             prompt = self.consumed_tokens
             recovery_kwargs["prompt"] = [t[0] for t in prompt]
@@ -406,44 +394,68 @@
         self.text = new_it.text
         self.consumed_tokens = new_it.consumed_tokens
         self.slice = new_slice
         # otherwise the chunking aligns with the old stream, so we return the next chunk
         return await self.__anext__()
 
     async def get_next(self):
-        if self.done.is_set(): 
+        if self.slice.done.is_set(): 
+            if self.n == 0:
+                return RecoveryAttempt(self.slice.kwargs, TimeoutError(), self.slice.maximum_retries)
             raise StopAsyncIteration
-        check_done_task = asyncio.create_task(self.done.wait())
+        check_done_task = asyncio.create_task(self.slice.done.wait())
         get_next_item_task = asyncio.create_task(self.slice.data_queue.get())
         done, pending = await asyncio.wait([get_next_item_task, check_done_task], 
             return_when=asyncio.FIRST_COMPLETED, timeout=2.0)
         
+
         if check_done_task in done:
             # this indicates the end of this response stream
             for t in pending: t.cancel()
+            if self.n == 0:
+                return RecoveryAttempt(self.slice.kwargs, TimeoutError(), self.slice.maximum_retries)
             raise StopAsyncIteration
         elif len(done) > 0:
             assert get_next_item_task in done, f"expected get_next_item_task to be done, but only {done} is done."
             # cancel self.done waiting task
             for t in pending: t.cancel()
             # return with new data chunk
+            self.n += 1
             return get_next_item_task.result()
         else:
+            for t in pending: t.cancel()
             # if after timeout this response has been fully consumed, we are done
-            if self.done.is_set():
+            if self.slice.done.is_set() and self.n > 0:
                 raise StopAsyncIteration
             # otherwise return a RecoveryAttempt for retrying this request
             return RecoveryAttempt(self.slice.kwargs, TimeoutError(), self.slice.maximum_retries)
 
     async def __anext__(self):
         try:
             data = await self.get_next()
             # None indicates end of stream
             if data is None:
-                raise StopAsyncIteration
+                if self.slice.done.is_set():
+                    raise StopAsyncIteration
+                else:
+                    if self.slice.finish_reason != "length":
+                        # return eos token as last item, if stream did not finish due to length
+                        data = {
+                            "text": "<|endoftext|>",
+                            "logprobs": {
+                                "text_offset": [0],
+                                "token_logprobs": [0.0],
+                                "tokens": ["<|endoftext|>"],
+                                "top_logprobs": [{"<|endoftext|>": 0.0}]
+                            }
+                        }
+                        self.slice.done.set()
+                    else:
+                        self.slice.done.set()
+                        raise StopAsyncIteration
             # exceptions that are queued are definitive (all retries failed)
             if isinstance(data, Exception): raise data
             # RecoveryAttempt indicates that the underlying stream errored out and we need to recover (still retries left)
             if isinstance(data, RecoveryAttempt):
                 if not self.slice.stream.scheduler.is_available():
                     # fail quietly, if parent scheduler is no longer available (results of this query will be discarded anyway)
                     raise StopAsyncIteration()
@@ -463,28 +475,31 @@
             self.consumed_tokens += data["logprobs"]["tokens"]
             self.text += data["text"]
 
             return data
         except asyncio.CancelledError:
             raise StopAsyncIteration
 
-
 class ResponseStreamSlice:
     def __init__(self, stream, kwargs, maximum_retries=3):
         self.stream: ResponseStream = stream
         self.kwargs = kwargs
         self.maximum_retries = maximum_retries
 
         self.data_queue = asyncio.Queue()
         self.failed = False
+        self.done = asyncio.Event()
+        self.finish_reason = None
+
+        self.itr = None
 
     def digest(self, data):
         assert not self.failed, f"digest called on failed slice"
         self.data_queue.put_nowait(data)
-    
+
     def finish(self):
         assert not self.failed, f"finish called on failed slice"
         self.data_queue.put_nowait(None)
 
     def error(self, error):
         assert not self.failed, f"error called on failed slice"
         self.failed = True
```

### Comparing `lmql-0.0.6/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.6.1/src/lmql/runtime/bopenai/openai_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,14 @@
                         
                         if is_done: break
                     
                 resp.close()
 
                 if current_chunk.strip() == "[DONE]":
                     return
-                
                 try:
                     last_message = json.loads(current_chunk.strip())
                     message = last_message.get("error", {}).get("message", "")
                     if "rate limit" in message.lower():
                         raise OpenAIRateLimitError(message + "local client capacity" + str(Capacity.reserved))
                     else:
                         raise OpenAIStreamError(last_message["error"]["message"] + " (after receiving " + str(n_chunks) + " chunks. Current chunk time: " + str(time.time() - last_chunk_time) + " Average chunk time: " + str(sum_chunk_times / max(1, n_chunks)) + ")", "Stream duration:", time.time() - stream_start)
@@ -336,15 +335,15 @@
                                 # last chunk may be incomplete
                                 break
                             complete_chunk = chunks[0].strip()
                             current_chunk = "data: ".join(chunks[1:])
 
                             if len(complete_chunk.strip()) == 0: 
                                 continue
-                            if complete_chunk == "[DONE]": 
+                            if complete_chunk == "[DONE]":
                                 return
                             
                             if n_chunks == 0:
                                 api_stats.times["first-chunk-latency"] = api_stats.times.get("first-chunk-latency", 0) + (time.time() - stream_start)
 
                             n_chunks += 1
                             sum_chunk_times += time.time() - last_chunk_time
```

### Comparing `lmql-0.0.6/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/dclib/dclib_cache.py` & `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,49 +31,55 @@
         mc.user_data_cache = {}
         mc.cache_lock = asyncio.Lock()
 
         mc.mask_cache = {}
         mc.show_speculative = show_speculative
         
         mc.input_id_key_offset = len(initial_prompt_ids) if initial_prompt_ids else 0
+        mc.initial_prompt_ids = initial_prompt_ids
         mc.cache["initial_prompt_ids"] = str(initial_prompt_ids) if initial_prompt_ids is not None else None
         mc.cache["model"] = delegate.model_identifier
     
         mc.calls = 0
         mc.hits = 0
 
         mc.cache_file = cache_file
 
         try:
             if cache_file is not None and os.path.exists(cache_file):
                 with open(cache_file, "rb") as f:
                     cache = pickle.load(f)
-                    if cache["initial_prompt_ids"] != str(initial_prompt_ids):
-                        print("warning: cache file is from a different query (revision). Its contents will be overwritten.")
-                    elif cache["model"] != delegate.model_identifier:
+                    if cache.get("model") != delegate.model_identifier:
                         print("warning: cache file is from a different model. Its contents will be overwritten.")
                     else:
-                        mc.cache = cache
+                        mc.cache = cache.get(str(initial_prompt_ids), {})
         except Exception as e:
             print("error: failed to load token cache from file", e)
             pass
 
         return mc
     
     def close(self):
         self.model.cache_delegate = None
         for ts in self.token_streams:
             ts.cancel()
         self.token_streams = []
 
     def save(self):
         if self.cache_file is not None:
+            if os.path.exists(self.cache_file):
+                with open(self.cache_file, "rb") as f:
+                    cache = pickle.load(f)
+            else:
+                cache = {}
+            cache[str(self.initial_prompt_ids)] = self.cache
+            cache["model"] = self.cache["model"]
             with open(self.cache_file, "wb") as f:
-                pickle.dump(self.cache, f)
-
+                pickle.dump(cache, f)
+    
     def base_key(self, ids, *args):
         if isinstance(ids, DecoderSequence):
             return self.base_key(ids.input_ids)
         return str(ids[self.input_id_key_offset:])
 
     async def get_mask(self, s: DecoderSequence, **kwargs):
         if s.id in self.mask_cache:
@@ -272,16 +278,16 @@
             results = []
             # put new results in cache
             for i, (s, key, c) in enumerate(zip(seqs, cache_keys, cached_tokens)):
                 if any(ct is None for ct in c):
                     r = next(non_cached_sample)
                     if any(ct is not None for ct in c):
                         mask = (await self.get_mask(s, **kwargs)).logits_mask[0]
-                        print("WARNING: some cache entries are None, but some are not", len([e for e in c if e is not None]), len(r.token))
-                        print([await s.text()])
+                        # print("WARNING: some cache entries are None, but some are not", len([e for e in c if e is not None]), len(r.token))
+                        # print([await s.text()])
                     results.append(r)
                     next_token_ids = ensure_iterable(r.token)
                     next_token_scores = ensure_iterable(r.logprob)
                     # cache each continuation separately
                     assert len(next_token_ids) <= len(key)
                     for i,ck in zip(range(len(next_token_ids)), key):
                         self.set_cache(ck, (next_token_ids[i], next_token_scores[i]))
@@ -478,31 +484,34 @@
                 sq = None
                 waiting_token_keys = []
 
                 async for (s, tokens, scores, edge_types, user_data) in itr():
                     if type(tokens) is int or len(tokens) == 1:
                         tokens = ensure_iterable(tokens)
                         scores = ensure_iterable(scores)
-                        if type(edge_types) is str:
+                        if type(edge_types) is str or edge_types is None:
                             edge_types = [edge_types]
                     else:
                         assert len(tokens) == len(scores) == len(edge_types), f"token_consumer: expected all lists to have the same length, but got {len(tokens)}, {len(scores)}, {len(edge_type)}"
                         # print("setting entries for", edge_types)
                     
                     waiting_token_keys = []
                     
                     async with self.cache_lock:
                         for token, score, edge_type in zip(tokens, scores, edge_types):
-                            assert type(edge_type) is str, "edge_types is {}".format(edge_types)
+                            assert type(edge_type) is str or edge_type is None, "edge_types is {}".format(edge_types)
+                            
                             if ids is None:
                                 ids = s.input_ids
                                 keys = await self.get_keys(s, edge_type, **self.model_args)
                                 sq = s
                             token_keys = [(self.base_key(ids), edge_type, *k[2:]) for k in keys]
                             token_keys += [(self.base_key(ids), str(token))]
+                            # filter out keys with edge_type=None
+                            token_keys = [k for k in token_keys if k[1] is not None]
 
                             # for tk in token_keys:
                             #     if tk in self.cache and type(self.cache[tk][0]) is not asyncio.Future:
                             #         print("token_consumer: token for {} from stream already in cache ({} streams): {}".format(tk, len(self.token_streams), self.cache[tk]))
 
                             self.set_cache(token_keys, (np.array(token).reshape(1), np.array(score).reshape(1)), user_data=user_data)
```

### Comparing `lmql-0.0.6/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
                     model = group[0].model
                     logits, raw = await model.logits(
                         [task.input_ids for task in group],
                         logits_mask=self.stack_logit_masks([task.logits_mask for task in group]),
                         **kwargs
                     )
                     for logits, raw, fut in zip(logits, raw, [task.result_fut for task in group]):
+                        if fut.cancelled(): continue
                         fut.set_result((logits, raw))
                     # print("batch of size", len(group), len(batch), self.logits_queue.qsize(), flush=True)
             except Exception as e:
                 import traceback
                 traceback.print_exc()
                 print("Exception in queue worker logits: ", e)
```

### Comparing `lmql-0.0.6/src/lmql/runtime/dclib/dclib_rewrite.py` & `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_rewrite.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.6.1/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.6.1/src/lmql/runtime/dclib/decoders.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/dclib/trie_cache.py` & `lmql-0.0.6.1/src/lmql/runtime/dclib/trie_cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/hf_integration.py` & `lmql-0.0.6.1/src/lmql/runtime/hf_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/interpreter.py` & `lmql-0.0.6.1/src/lmql/runtime/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,19 +131,17 @@
 class PromptInterpreter:
     """
     The PromptInterpreter is the main entry point for an LMQL query. It handles program execution, 
     token masking and scripted interaction during query execution.
     """
 
     def __init__(self, force_model=None) -> None:
-        assert force_model is None, "force_model is not supported in P2"
-        
         # model-specific components
-        self.model = None
-        self.model_identifier = None
+        self.model = force_model
+        self.model_identifier = force_model
         self.tokenizer: LMQLTokenizer = None
 
         # decoder configuration
         self.decoder = None
         self.decoder_kwargs = {}
         
         # extra interpreter flags passed via @lmql.query/@lmql.compiled_query
@@ -178,16 +176,17 @@
         self.extra_kwargs.update(kwargs)
 
     def set_decoder(self, method, **kwargs):
         self.decoder_kwargs = kwargs
         self.decoder_kwargs["decoder"] = method
 
     def set_model(self, model_name):
-        self.model = model_name
-        self.model_identifier = model_name
+        if self.model is None:
+            self.model = model_name
+            self.model_identifier = model_name
 
         client = LMQLModelRegistry.get(self.model)
 
         # setup the VocabularyMatcher to use the concrete vocabulary of the model
         VocabularyMatcher.init(client.get_tokenizer())
         
         # for OpenAI models we optimize for compact logit masks
@@ -452,15 +451,15 @@
         writer = CytoscapeGraphWriter(extra_data_provider=node_data)
         writer.write(self.where)
 
         return writer.graph.to_json(return_dict=True)
 
     async def debugger_output(self, state: PromptState, s: dc.DecoderSequence, valid, is_final, mask, stopping_phrases, program_variables, trace, text):
         if self.output_writer is not None:
-            self.output_writer.add_interpreter_head_state(state.variable, 0, state.prompt + text, self.where, trace, valid, is_final, mask, len(s.input_ids), program_variables)
+           await self.output_writer.add_interpreter_head_state(state.variable, 0, state.prompt + text, self.where, trace, valid, is_final, mask, len(s.input_ids), program_variables)
 
     async def where_processor(self, seqs, additional_logits_processor_mask, **kwargs):
         zipped_task_inputs = zip(seqs, additional_logits_processor_mask, range(len(seqs)))
         token_mask_tasks = [self.where_for_sequence(s, needs_masking, seqidx, **kwargs) for s,needs_masking, seqidx in zipped_task_inputs]
         results = [(mask, user_data) for mask, user_data in await asyncio.gather(*token_mask_tasks)]
         
         return TokenMask([r[0] for r in results], [r[1] for r in results])
@@ -737,16 +736,14 @@
                 has_deterministic_tail = False
                 while s.deterministic[upper-1] and upper >= 0:
                     upper -= 1
                     has_deterministic_tail = True
                 # +1 for the eos token
                 billable_tokens += upper + (1 if has_deterministic_tail else 0)
             
-            self.dcmodel.log_billable_tokens(billable_tokens)
-
             results = []
 
             for i,s in enumerate(result_sequences):
                 state = self.interpreter_state_from_user_data(s)
                 if state.query_head.result is not None:
                     results.append(state.query_head.result)
                 else:
@@ -763,15 +760,15 @@
         finally:
             # make sure token cache is saved if possible
             self.dcmodel.save()
             if hasattr(self.dcmodel, "close"):
                 self.dcmodel.close()
 
     def validate_args(self, decoder_args, decoder_fct):
-        INTERNAL_ARGS = ["decoder", "dcmodel", "modern_rewriter", "modern_logits_processor", "dclib_additional_logits_processor", "input_id_rewriter", "output_writer", "chatty_openai", "distribution_batch_size", "openai_chunksize", "step_budget", "stats", "performance_stats", "cache", "show_speculative"]
+        INTERNAL_ARGS = ["decoder", "dcmodel", "modern_rewriter", "modern_logits_processor", "dclib_additional_logits_processor", "input_id_rewriter", "output_writer", "chatty_openai", "distribution_batch_size", "openai_chunksize", "step_budget", "stats", "performance_stats", "cache", "show_speculative", "openai_nonstop"]
 
         # get all arg names and kwarg names of decoder function
         decoder_arg_names = inspect.getfullargspec(decoder_fct).args
         decoder_kwarg_names = inspect.getfullargspec(decoder_fct).kwonlyargs
         for k in decoder_args.keys():
             if k not in decoder_arg_names and k not in decoder_kwarg_names and k not in INTERNAL_ARGS:
                 raise ValueError("Unknown decoder argument: {}".format(k))
```

### Comparing `lmql-0.0.6/src/lmql/runtime/langchain.py` & `lmql-0.0.6.1/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.6.1/src/lmql/runtime/lmql_runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,23 +96,28 @@
         if self.function_context is None:
             return kwargs
         else:
             argnames = self.function_context.argnames
             args_of_query = self.function_context.args_of_query
             scope = self.function_context.scope
 
+        # do not consider kwargs that are already set
+        argnames = [a for a in argnames if a not in kwargs.keys()]
+
         assert len(args) == len(argnames), f"@lmql.query {self.fct.__name__} expects {len(argnames)} positional arguments, but got {len(args)}."
         captured_variables = set(args_of_query)
         for name, value in zip(argnames, args):
             if name in args_of_query:
                 kwargs[name] = value
                 captured_variables.remove(name)
-    
+
+        # resolve remaining unset args from scope
         for v in captured_variables:
-            kwargs[v] = scope.resolve(v)
+            if not v in kwargs:
+                kwargs[v] = scope.resolve(v)
         
         if "output_writer" in kwargs:
             self.output_writer = kwargs["output_writer"]
             del kwargs["output_writer"]
         else:
             self.output_writer = silent
 
@@ -124,18 +129,18 @@
         else:
             return super().__call__(*args, **kwargs)
 
     async def __acall__(self, *args, **kwargs):
         kwargs = self.make_kwargs(*args, **kwargs)
 
         interpreter = PromptInterpreter(force_model=self.model)
-        interpreter.set_extra_args(
-            output_writer = self.output_writer,
-            **kwargs
-        )
+        
+        if self.output_writer is not None:
+            kwargs["output_writer"] = self.output_writer
+        interpreter.set_extra_args(**kwargs)
 
         query_kwargs = {}
         for a in self.args:
             if a in kwargs.keys():
                 query_kwargs[a] = kwargs[a]
             else:
                 query_kwargs[a] = self.scope.resolve(a)
```

### Comparing `lmql-0.0.6/src/lmql/runtime/maiohttp.py` & `lmql-0.0.6.1/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/masks.py` & `lmql-0.0.6.1/src/lmql/runtime/masks.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/model_registry.py` & `lmql-0.0.6.1/src/lmql/runtime/model_registry.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.0.6.1/src/lmql/runtime/multi_head_interpretation.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/openai_integration.py` & `lmql-0.0.6.1/src/lmql/runtime/openai_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         self.output_writer = None
         if "output_writer" in kwargs:
             self.output_writer = kwargs["output_writer"]
         
         self.model_identifier = "openai/" + self.model.model_identifier
 
         self.model.chunk_size = kwargs.get("openai_chunksize", 64)
+        self.model.nostop = kwargs.get("openai_nonstop", False)
         self.num_billed_tokens = {}
         self.num_requests = 0
 
         self.stats = Stats("openai")
         openai.AsyncConfiguration.set_tokenizer(self.tokenize)
 
     def log_billable_tokens(self, n: int):
@@ -265,22 +266,24 @@
             if fixed_next_token == self.eos_token_id:
                 return CompletionResult(openai.response_buffer.singleton(token=fixed_next_token, token_logprob=0), completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
             else:
                 fixed_next_token = nputil.ensure_array(fixed_next_token, dtype=np.int64)
                 if noscore: logprob = 0.0
                 else: logprob = (await self.api_score(np.concatenate([input_ids, fixed_next_token.reshape(1)], axis=0), len(input_ids)))
                 return CompletionResult(openai.response_buffer.singleton(token=fixed_next_token, token_logprob=logprob), completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
-        elif len(completion_call.stopping_phrases) > 0:
+        else:
+            assert False, f"Internal openai API dispatcher returned an unknown completion mode {mode}"
+
+        if len(completion_call.stopping_phrases) > 0:
             if len(completion_call.stopping_phrases) > 4:
                 # same but blaming it more on OpenAI
                 print("warning: the number of stopping phrases that would need to be passed to the OpenAI API is greater than 4. Since the OpenAI API only supports up to 4 stopping phrases, the first 4 stopping phrases will be passed to the API. Other stopping phrases will also be enforced, but may lead to an increase in the number of tokens billed to the user.")
             # skip stopping phrases for more speculative execution
-            # kwargs.update({"stop": completion_call.stopping_phrases[:4]})
-        else:
-            assert False, f"Internal openai API dispatcher returned an unknown completion mode {mode}"
+            if not self.model.nostop:
+                kwargs.update({"stop": completion_call.stopping_phrases[:4]})
 
         # TODO: we are now overestimate the number of tokens billed to the user since we are not account for stopping phrases for the sake of streaming
         self.count_billed_tokens(input_ids.size + kwargs.get("max_tokens") * batch_size, self.model_identifier)
         
         if self.model_args.get("chatty_openai", False):
             args = kwargs.copy()
             args["prompt"] = str([await self.detokenize(kwargs["prompt"])])[2:-2]
@@ -292,75 +295,14 @@
         if len(tokens) > 0 and type(tokens[0]) is str:
             return [[t[0]] for t in await self.model.tokenize(tokens)]
         return tokens
     
     async def openai_cache_delegate(self, kwargs, tokens, scores):
         print(tokens, scores, self.cache_delegate)
 
-    async def _complete(self, completion_call: Union[CompletionCall, List[CompletionCall]], **kwargs):
-        if type(completion_call) is list:
-            input_ids = np.stack([c.input_ids for c in completion_call], axis=0)
-            assert input_ids.ndim == 2, f"_complete expects input_ids to be a 1D tensor per completion call, when multiple completion calls are passed, got {input_ids.ndim}D tensor."
-            # all other call parameters are assumed to be the same
-            batch_size = len(completion_call)
-            completion_call = completion_call[0]
-        else:
-            batch_size = 1
-            input_ids = completion_call.input_ids
-            assert input_ids.ndim == 1, f"_complete expects input_ids to be a 1D tensor when only one completion_call is passed, got {input_ids.ndim}D tensor."
-
-        temperature = completion_call.kwargs.get("temperature", 0.0)
-        logprobs = completion_call.kwargs.get("logprobs", 5)
-
-        kwargs = {
-            "model": self.model.model_identifier,
-            "prompt": input_ids.tolist()[0], # no more batching at this point
-            "max_tokens": self.model.chunk_size,
-            "temperature": temperature,
-            "logprobs": logprobs,
-            "user": "lmql",
-            "stream": True,
-        }
-
-        mode = completion_call.mode
-        
-        if mode == "*": # complete without mask
-            pass
-        elif mode == "complete": # complete with mask
-            logit_bias = completion_call.api_mask
-            kwargs.update({"logit_bias": logit_bias})
-        elif mode == "fixed": # complete with fixed token
-            fixed_next_token = completion_call.logit_mask_or_fixed_id # special return value case for prepare function
-            # TODO revisit this, what kind of probability do we want here (masked or unmasked/scored)
-            if fixed_next_token == self.eos_token_id:
-                return OpenAIModelOutputBuffer.fixed_output(fixed_next_token, 0)
-            else:
-                if not nputil.is_array(fixed_next_token): 
-                    fixed_next_token = np.array(fixed_next_token)
-                logprob = (await self.api_score(np.concatenate([input_ids, fixed_next_token.reshape(1)], axis=0), len(input_ids))).result
-                return OpenAIModelOutputBuffer.fixed_output(fixed_next_token, logprob)
-        elif len(completion_call.stopping_phrases) > 0:
-            if len(completion_call.stopping_phrases) > 4:
-                # same but blaming it more on OpenAI
-                print("warning: the number of stopping phrases that would need to be passed to the OpenAI API is greater than 4. Since the OpenAI API only supports up to 4 stopping phrases, the first 4 stopping phrases will be passed to the API. Other stopping phrases will also be enforced, but may lead to an increase in the number of tokens billed to the user.")
-            # kwargs.update({"stop": completion_call.stopping_phrases[:4]})
-        else:
-            assert False, f"Internal openai API dispatcher returned an unknown completion mode {mode}"
-
-        # TODO: we are now overestimate the number of tokens billed to the user since we are not account for stopping phrases for the sake of streaming
-        self.count_billed_tokens(input_ids.size + kwargs.get("max_tokens") * batch_size, self.model_identifier)
-        
-        if self.model_args.get("chatty_openai", False):
-            print("Completion with", kwargs)
-        
-        async def complete_op():
-            return openai_complete_create(**kwargs)
-        return await CompleteTask(complete_op, None, continuation_type=completion_call.continuation_type, 
-            logit_mask_or_fixed_id=completion_call.logit_mask_or_fixed_id).run(retries=3)
-
     def count_billed_tokens(self, n, model):
         if model not in self.num_billed_tokens.keys():
             self.num_billed_tokens[model] = 0
         self.num_billed_tokens[model] += n
         self.num_requests += 1
 
     async def completion_buffer(self, seqs, temperature=1, **kwargs):
@@ -403,14 +345,16 @@
                     None,
                 )
 
             completion_result = await self.async_complete(completion_call)
             # eagerly expand and cache full completion if a cache_delegate is available
             if self.cache_delegate is not None:
                 await self.expand_and_cache(s, completion_result, "top-1", logprobs=kwargs.get("logprobs", 1))
+            
+            assert not await completion_result.buffer.empty(), "Completion result is empty on arrival"
             return completion_result
 
         return await asyncio.gather(*[get_buffer(i, s) for i, s in enumerate(seqs)])
 
     async def expand_and_cache(self, s: DecoderSequence, completion_result: CompletionResult, edge_type, logprobs=1):
         async def token_stream():
             nonlocal edge_type, s, completion_result
@@ -442,14 +386,17 @@
                             scores = [score for _, score in topk_tokens]
                             edge_type = ["top-{}".format(i+1) for i in range(len(topk_tokens))]
                         
                         # future continuation
                         response_buffer = response_buffer[1:]
                         continuation = CompletionResult(response_buffer, completion_result.continuation_type, completion_result.logit_mask_or_fixed_id)
 
+                        if continuation.continuation_type is None:
+                            edge_type = None
+
                         user_data = {
                             "openai-continuations": {
                                 continuation.continuation_type: continuation
                             }
                         }
                         yield (s, tokens, scores, edge_type, user_data)
                     except IndexError:
@@ -874,14 +821,15 @@
             if at_end: break
         return self.current_len == 0
 
 class OptimisticChunkBasedOpenAIModel:
     def __init__(self, model_identifier, tokenizer):
         self.model_identifier = model_identifier.split("openai/",1)[1]
         self.chunk_size = 32
+        self.nostop = False
         self.tokenizer = tokenizer
 
         self.input_ids = []
         self.next_token_scores = []
         self.logits_mask = []
         
         self.buffer = []
@@ -916,47 +864,14 @@
             "stream": True,
             **kwargs
         }
 
         complete_op = lambda: openai_complete_create(**kwargs)
         return CompleteTask(complete_op, None, continuation_type=None).run(retries=3)
         
-
-    async def advance(self):
-        sequence_indices_to_extend_on = []
-        prompts_to_extend = []
-        for i, buffer in enumerate(self.buffer):
-            if await buffer.at_end():
-                sequence_indices_to_extend_on.append(i)
-                prompts_to_extend.append(self.input_ids[i])
-
-        if len(prompts_to_extend) > 0:
-            res = self._complete(np.stack(prompts_to_extend, axis=0))
-            response_buffer = OpenAIModelOutputBuffer(res, len(prompts_to_extend), self.tokenizer)
-            for i, seq_idx in enumerate(sequence_indices_to_extend_on):
-                self.buffer[seq_idx] = response_buffer.buffer(i)
-
-        # advance all self.input_ids by one token from buffer
-        next_tokens = []
-        for i, buffer in enumerate(self.buffer):
-            assert not await buffer.at_end(), f"openai model did not complete decoder head {i} further."
-            token, logprob = await buffer.pop()
-            next_tokens.append(token)
-            self.next_token_scores[i].append(logprob)
-
-        next_tokens = np.array(next_tokens, dtype=np.int64)
-        self.input_ids = np.concatenate([self.input_ids, next_tokens.unsqueeze(1)], axis=1)
-
-    def make_api_logits_mask(self, logits, invert):
-        if invert:
-            masked = (logits >= 0)
-        else:
-            masked = (logits < 0)
-        mask_value = 100 if invert else -100
-        return {int(idx): mask_value for idx in np.nonzero(masked)[0]}
     
     async def tokenize(self, text):
         return self.tokenizer(text)["input_ids"]
 
     async def __aenter__(self):
         self.previous_context_model = OptimisticChunkBasedOpenAIModel.context_model
```

### Comparing `lmql-0.0.6/src/lmql/runtime/openai_secret.py` & `lmql-0.0.6.1/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/output_writer.py` & `lmql-0.0.6.1/src/lmql/runtime/output_writer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,82 @@
 import os
 import termcolor
 
-class DebuggerOutputWriter:
+class BaseOutputWriter:
     def __init__(self, allows_input=True):
         self.allows_input = allows_input
 
     async def input(self, *args):
+        """
+        Handle user input with an input prompt of *args. This is invoked when a query asks for user input via `await input()`.
+
+        Returns:
+            str: The user input.
+        """
         if not self.allows_input:
             assert False, "current LMQL output writer does not allow input"
         return input(*args)
 
-    def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables): pass
-    def add_compiler_output(self, code): pass
+    async def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables): 
+        """
+        Called whenever the query interpreter progresses in a meaningful way (e.g. new token added, new variable added, variable updated, etc.).
+
+        Parameters:
+            variable (str): 
+                The name of the currently active variable.
+            head (int): 
+                The index of the current interpretation head (deprecated, will always be 0).
+            prompt (str): 
+                The full interaction trace/prompt of the query.
+            where (object): 
+                The AST representation of the queries validation condition.
+            trace (object): 
+                The evaluation trace of evaluating 'where' on the current program variables during generation.
+            is_valid (bool): 
+                Whether the current program variables satisfy the validation condition.
+            is_final (bool): 
+                Whether the value of 'valid' can be considered final (i.e. decoding more tokens will not change the value of 'valid').
+            mask (np.ndarray): 
+                Currently active token mask.
+            num_tokens (int): 
+                Number of tokens in the current 'prompt'.
+            program_variables (ProgramState): 
+                The current program state (lmql.runtime.program_state). E.g. program_variables.variable_values is a mapping of variable names to their current values.
+        """
+        pass
+    
+    def add_compiler_output(self, code): 
+        pass
 
-class PrintingDebuggerOutputWriter:
+class PrintingOutputWriter:
     def __init__(self, clear=False):
         self.clear = clear
         self.print_output = True
 
     def add_decoder_state(*args, **kwargs): 
         pass
 
-    def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables):
+    async def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables):
         if head == 0:
             if self.clear:
                 os.system("clear")
             if self.print_output:
                 print(f"{prompt}\n\n valid={is_valid}, final={is_final}")
+    
     def add_compiler_output(self, code): pass
     
 class StreamingOutputWriter:
     def __init__(self, variable=None):
         self.variable = variable
-        
         self.last_value = None
     
     def add_decoder_state(*args, **kwargs): 
         pass
 
-    def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables):
+    async def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables):
         if head == 0:
             if self.variable is not None:
                 vars = self.variable
                 if type(vars) is not list:
                     vars = [vars]
                 
                 value = "\n".join(program_variables.variable_values.get(v, "").strip() for v in vars)
@@ -58,12 +92,11 @@
             
             os.system("clear")
             print(f"{prompt}\n", end="\r")
             
     def add_compiler_output(self, code): pass
 
 # ready to use output writer configurations
-
-silent = DebuggerOutputWriter()
-headless = DebuggerOutputWriter(allows_input=False)
+silent = BaseOutputWriter()
+headless = BaseOutputWriter(allows_input=False)
 stream = StreamingOutputWriter
-printing = PrintingDebuggerOutputWriter(clear=True)
+printing = PrintingOutputWriter(clear=True)
```

### Comparing `lmql-0.0.6/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.0.6.1/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/program_state.py` & `lmql-0.0.6.1/src/lmql/runtime/program_state.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/stats.py` & `lmql-0.0.6.1/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/runtime/tokenizer.py` & `lmql-0.0.6.1/src/lmql/runtime/tokenizer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/expr_test_utils.py` & `lmql-0.0.6.1/src/lmql/tests/expr_test_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/outdated/mask_product_test.py` & `lmql-0.0.6.1/src/lmql/tests/outdated/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/outdated/monotonicity.py` & `lmql-0.0.6.1/src/lmql/tests/outdated/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/outdated/one_of_tests.py` & `lmql-0.0.6.1/src/lmql/tests/outdated/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/outdated/sentences_op.py` & `lmql-0.0.6.1/src/lmql/tests/outdated/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/outdated/starts_with_op_test.py` & `lmql-0.0.6.1/src/lmql/tests/outdated/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/outdated/stops_at.py` & `lmql-0.0.6.1/src/lmql/tests/outdated/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/outdated/str_in_str_tests.py` & `lmql-0.0.6.1/src/lmql/tests/outdated/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/outdated/test_multi_head.py` & `lmql-0.0.6.1/src/lmql/tests/outdated/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/outdated/token_set_test.py` & `lmql-0.0.6.1/src/lmql/tests/outdated/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.6.1/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/tail_token_set.py` & `lmql-0.0.6.1/src/lmql/tests/tail_token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/tests/test_sample_queries.py` & `lmql-0.0.6.1/src/lmql/tests/test_sample_queries.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/live/live.js` & `lmql-0.0.6.1/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/live/live.py` & `lmql-0.0.6.1/src/lmql/ui/live/live.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def report_model_stats(self, **kwargs):
         add_debugger_output("openai-token-count", kwargs)
         
     async def input(self, *args):
         add_debugger_output("stdin-request", {})
         return await LiveApp.ainput(*args, web=self.web)
 
-    def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables):
+    async def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables):
         from lmql.utils.graph import CytoscapeGraphWriter
         
         def node_data(op):
             follow_map = "<follow_map output not supported>"
 
             result = "-"
             if trace is not None and op in trace:
```

### Comparing `lmql-0.0.6/src/lmql/ui/live/livelib.py` & `lmql-0.0.6.1/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/live/yarn.lock` & `lmql-0.0.6.1/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/README.md` & `lmql-0.0.6.1/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/package.json` & `lmql-0.0.6.1/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.6.1/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/index.html` & `lmql-0.0.6.1/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.6.1/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.0.6.1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.6.1/src/lmql/ui/playground/src/App.jsx`

 * *Files 0% similar despite different names*

```diff
@@ -808,19 +808,14 @@
     color: white;
     background-color: #333;
     opacity: 1.0;
     border-radius: 2pt;
     margin-left: 2pt;
   }
 
-  div .variable:hover {
-    position: relative;
-    transform: scale(1.1);
-  }
-
   div .badge {
     padding: 1.0pt 4pt;
     border-radius: 2pt;
     font-size: 0.9em;
     background-color: rgba(0, 0, 0, 0.5);
     position:relative; 
     top: -0.05em;
```

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.0.6.1/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -294,14 +294,15 @@
                 style: {
                     // light blue
                     'background-color': 'rgb(249, 209, 248)',
                     'background-opacity': 0.7,
                     'color': 'white',
                     'border-color': 'red',
                     'border-width': '0px',
+                    'opacity': 0.4
                 }
             }, {
                 selector: 'node.inactive',
                 style: {
                     'opacity': 0.5
                 }
             },
```

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.6.1/src/lmql/ui/playground/src/Explore.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/State.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.6.1/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.6.1/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.6.1/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.6.1/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/index.css` & `lmql-0.0.6.1/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.6.1/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/queries.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.0.6.1/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.6.1/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.6.1/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.6.1/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.6.1/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.6.1/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.6.1/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.0.6.1/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/vscode/package.json` & `lmql-0.0.6.1/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.6.1/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/utils/graph.py` & `lmql-0.0.6.1/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql/utils/nputil.py` & `lmql-0.0.6.1/src/lmql/utils/nputil.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6/src/lmql.egg-info/PKG-INFO` & `lmql-0.0.6.1/src/lmql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
     ·
     <a href="https://lmql.ai/playground">Playground IDE</a>
     ·
     <a href="https://github.com/eth-sri/lmql/issues">Report Bug</a>
     <br/>
     <br/>
     <a href="https://discord.gg/7eJP4fcyNT"><img src="https://img.shields.io/discord/1091288833997410414?style=plastic&logo=discord&color=blueviolet&logoColor=white" height=18/></a>
-    <a href="https://badge.fury.io/py/Lmql"><img src="https://badge.fury.io/py/Lmql.svg" alt="PyPI version" height=18></a>
+    <a href="https://badge.fury.io/py/Lmql"><img src="https://badge.fury.io/py/Lmql.svg?cacheSeconds=3600" alt="PyPI version" height=18></a>
   </p>
 </div>
 
 LMQL is a query language for large language models (LLMs). It facilitates LLM interaction by combining the benefits of natural language prompting with the expressiveness of Python. With only a few lines of LMQL code, users can express advanced, multi-part and tool-augmented LM queries, which then are optimized by the LMQL runtime to run efficiently as part of the LM decoding loop.
 
 ![lmql-overview](https://user-images.githubusercontent.com/17903049/222918379-84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.6 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6.1 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
```

### Comparing `lmql-0.0.6/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.6.1/src/lmql.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 docs/source/language/models.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
 docs/source/python/.gitignore
 docs/source/python/langchain.ipynb
 docs/source/python/llama_index.ipynb
 docs/source/python/lmql.txt
+docs/source/python/output.ipynb
 docs/source/python/pandas.ipynb
 docs/source/python/python.ipynb
 docs/source/releases/misc-snippets.md
 docs/source/releases/release-0.0.5.md
 scripts/activate-dev.sh
 scripts/pypi-release.sh
 scripts/wheel.sh
@@ -68,14 +69,18 @@
 src/lmql/model/local_client.py
 src/lmql/model/serve.py
 src/lmql/model/served_model.py
 src/lmql/ops/__init__.py
 src/lmql/ops/follow_map.py
 src/lmql/ops/ops.py
 src/lmql/ops/token_set.py
+src/lmql/output/__init__.py
+src/lmql/output/http.py
+src/lmql/output/sse.py
+src/lmql/output/ws.py
 src/lmql/runtime/__init__.py
 src/lmql/runtime/hf_integration.py
 src/lmql/runtime/interpreter.py
 src/lmql/runtime/interrupt.py
 src/lmql/runtime/langchain.py
 src/lmql/runtime/lmql_runtime.py
 src/lmql/runtime/maiohttp.py
@@ -102,14 +107,15 @@
 src/lmql/runtime/dclib/trie_cache.py
 src/lmql/runtime/postprocessing/__init__.py
 src/lmql/runtime/postprocessing/conditional_prob.py
 src/lmql/runtime/postprocessing/group_by.py
 src/lmql/tests/README.md
 src/lmql/tests/expr_test_utils.py
 src/lmql/tests/tail_token_set.py
+src/lmql/tests/test_back2back_caching.py
 src/lmql/tests/test_sample_queries.py
 src/lmql/tests/outdated/mask_product_test.py
 src/lmql/tests/outdated/monotonicity.py
 src/lmql/tests/outdated/one_of_tests.py
 src/lmql/tests/outdated/sentences_op.py
 src/lmql/tests/outdated/starts_with_op_test.py
 src/lmql/tests/outdated/stops_at.py
@@ -190,9 +196,10 @@
 src/lmql/ui/vscode/lmql-vscode.png
 src/lmql/ui/vscode/package.json
 src/lmql/ui/vscode/.vscode/launch.json
 src/lmql/ui/vscode/syntaxes/lmql.qstring.json
 src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
 src/lmql/ui/vscode/syntaxes/pylmql.json
 src/lmql/utils/__init__.py
+src/lmql/utils/docstring_parser.py
 src/lmql/utils/graph.py
 src/lmql/utils/nputil.py
```

### Comparing `lmql-0.0.6/src/lmql.svg` & `lmql-0.0.6.1/src/lmql.svg`

 * *Files identical despite different names*

