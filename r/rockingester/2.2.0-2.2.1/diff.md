# Comparing `tmp/rockingester-2.2.0.tar.gz` & `tmp/rockingester-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockingester-2.2.0.tar", last modified: Tue May  2 08:58:16 2023, max compression
+gzip compressed data, was "rockingester-2.2.1.tar", last modified: Wed May  3 05:04:12 2023, max compression
```

## Comparing `rockingester-2.2.0.tar` & `rockingester-2.2.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-02 08:58:04.000000 rockingester-2.2.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-02 08:58:04.000000 rockingester-2.2.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.772846 rockingester-2.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-02 08:58:04.000000 rockingester-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-02 08:58:04.000000 rockingester-2.2.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-02 08:58:04.000000 rockingester-2.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 08:58:04.000000 rockingester-2.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-02 08:58:04.000000 rockingester-2.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-02 08:58:04.000000 rockingester-2.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 08:58:04.000000 rockingester-2.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 08:58:04.000000 rockingester-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-02 08:58:16.792846 rockingester-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-02 08:58:04.000000 rockingester-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-02 08:58:04.000000 rockingester-2.2.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.772846 rockingester-2.2.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-02 08:58:04.000000 rockingester-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 08:58:16.792846 rockingester-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.772846 rockingester-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/src/rockingester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/src/rockingester_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/direct_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/src/rockingester_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.934909 rockingester-2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.922909 rockingester-2.2.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-03 05:04:03.000000 rockingester-2.2.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-03 05:04:03.000000 rockingester-2.2.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-03 05:04:03.000000 rockingester-2.2.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-03 05:04:03.000000 rockingester-2.2.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 05:04:03.000000 rockingester-2.2.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-03 05:04:03.000000 rockingester-2.2.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 05:04:03.000000 rockingester-2.2.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 05:04:03.000000 rockingester-2.2.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 05:04:03.000000 rockingester-2.2.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-03 05:04:03.000000 rockingester-2.2.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-03 05:04:03.000000 rockingester-2.2.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-03 05:04:03.000000 rockingester-2.2.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.922909 rockingester-2.2.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-03 05:04:03.000000 rockingester-2.2.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 05:04:03.000000 rockingester-2.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-03 05:04:03.000000 rockingester-2.2.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-03 05:04:03.000000 rockingester-2.2.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-03 05:04:03.000000 rockingester-2.2.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-03 05:04:03.000000 rockingester-2.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-03 05:04:03.000000 rockingester-2.2.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-03 05:04:03.000000 rockingester-2.2.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-03 05:04:03.000000 rockingester-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-03 05:04:03.000000 rockingester-2.2.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 05:04:03.000000 rockingester-2.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 05:04:03.000000 rockingester-2.2.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 05:04:03.000000 rockingester-2.2.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 05:04:03.000000 rockingester-2.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-03 05:04:03.000000 rockingester-2.2.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 05:04:03.000000 rockingester-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-03 05:04:12.934909 rockingester-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-03 05:04:03.000000 rockingester-2.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-03 05:04:03.000000 rockingester-2.2.1/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.922909 rockingester-2.2.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.926909 rockingester-2.2.1/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.930909 rockingester-2.2.1/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.930909 rockingester-2.2.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 05:04:03.000000 rockingester-2.2.1/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-03 05:04:03.000000 rockingester-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 05:04:12.934909 rockingester-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.922909 rockingester-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.930909 rockingester-2.2.1/src/rockingester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-03 05:04:12.000000 rockingester-2.2.1/src/rockingester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-03 05:04:12.000000 rockingester-2.2.1/src/rockingester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:04:12.000000 rockingester-2.2.1/src/rockingester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-03 05:04:12.000000 rockingester-2.2.1/src/rockingester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-03 05:04:12.000000 rockingester-2.2.1/src/rockingester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-03 05:04:12.000000 rockingester-2.2.1/src/rockingester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.930909 rockingester-2.2.1/src/rockingester_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.930909 rockingester-2.2.1/src/rockingester_api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.930909 rockingester-2.2.1/src/rockingester_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.930909 rockingester-2.2.1/src/rockingester_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.930909 rockingester-2.2.1/src/rockingester_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 05:04:12.000000 rockingester-2.2.1/src/rockingester_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.934909 rockingester-2.2.1/src/rockingester_lib/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/collectors/direct_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.934909 rockingester-2.2.1/src/rockingester_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 05:04:03.000000 rockingester-2.2.1/src/rockingester_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.934909 rockingester-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:03.000000 rockingester-2.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 05:04:03.000000 rockingester-2.2.1/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:04:12.934909 rockingester-2.2.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-03 05:04:03.000000 rockingester-2.2.1/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-03 05:04:03.000000 rockingester-2.2.1/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-03 05:04:03.000000 rockingester-2.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-03 05:04:03.000000 rockingester-2.2.1/tests/test_collector.py
```

### Comparing `rockingester-2.2.0/.dae-devops/Makefile` & `rockingester-2.2.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.dae-devops/docs/conventions.rst` & `rockingester-2.2.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.dae-devops/docs/developing.rst` & `rockingester-2.2.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.dae-devops/docs/devops.rst` & `rockingester-2.2.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.dae-devops/docs/docs_structure.rst` & `rockingester-2.2.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.dae-devops/docs/installing.rst` & `rockingester-2.2.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.dae-devops/docs/testing.rst` & `rockingester-2.2.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.dae-devops/project.yaml` & `rockingester-2.2.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.devcontainer/Dockerfile` & `rockingester-2.2.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.devcontainer/devcontainer.json` & `rockingester-2.2.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.github/CONTRIBUTING.rst` & `rockingester-2.2.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.github/actions/install_requirements/action.yml` & `rockingester-2.2.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.github/dependabot.yml` & `rockingester-2.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.github/pages/make_switcher.py` & `rockingester-2.2.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.github/workflows/code.yml` & `rockingester-2.2.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.github/workflows/docs.yml` & `rockingester-2.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.github/workflows/docs_clean.yml` & `rockingester-2.2.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.github/workflows/linkcheck.yml` & `rockingester-2.2.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.gitignore` & `rockingester-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.gitlab-ci.yml` & `rockingester-2.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/.vscode/launch.json` & `rockingester-2.2.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/LICENSE` & `rockingester-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/PKG-INFO` & `rockingester-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.2.0
+Version: 2.2.1
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.2.0/README.rst` & `rockingester-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/configurations/development.yaml` & `rockingester-2.2.1/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/docs/conf.py` & `rockingester-2.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/docs/images/dls-favicon.ico` & `rockingester-2.2.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/docs/images/dls-logo.svg` & `rockingester-2.2.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/docs/index.rst` & `rockingester-2.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/docs/user/explanations/25-docs-structure.rst` & `rockingester-2.2.1/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/docs/user/index.rst` & `rockingester-2.2.1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/pyproject.toml` & `rockingester-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester.egg-info/PKG-INFO` & `rockingester-2.2.1/src/rockingester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.2.0
+Version: 2.2.1
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.2.0/src/rockingester.egg-info/SOURCES.txt` & `rockingester-2.2.1/src/rockingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_api/collectors/aiohttp.py` & `rockingester-2.2.1/src/rockingester_api/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_api/collectors/collectors.py` & `rockingester-2.2.1/src/rockingester_api/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_api/collectors/context.py` & `rockingester-2.2.1/src/rockingester_api/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_api/context_base.py` & `rockingester-2.2.1/src/rockingester_api/context_base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_api/exceptions.py` & `rockingester-2.2.1/src/rockingester_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_api/thing.py` & `rockingester-2.2.1/src/rockingester_api/thing.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_api/things.py` & `rockingester-2.2.1/src/rockingester_api/things.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_cli/main.py` & `rockingester-2.2.1/src/rockingester_cli/main.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_cli/subcommands/base.py` & `rockingester-2.2.1/src/rockingester_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_cli/subcommands/service.py` & `rockingester-2.2.1/src/rockingester_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_cli/version.py` & `rockingester-2.2.1/src/rockingester_cli/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_lib/__main__.py` & `rockingester-2.2.1/src/rockingester_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_lib/collectors/aiohttp.py` & `rockingester-2.2.1/src/rockingester_lib/collectors/aiohttp.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,16 +65,14 @@
             multiprocessing.current_process().name = "collector"
 
             self.activate_process_base()
 
         except Exception as exception:
             logger.exception("exception in collector process", exc_info=exception)
 
-        logger.debug(f"[PIDAL] {callsign(self)} is returning from activate_process")
-
     # ----------------------------------------------------------------------------------------
     def activate_thread(self, loop) -> None:
         """
         Activate the direct collector and web server in a new thread.
 
         Meant to be called from inside a newly created thread.
         """
@@ -92,31 +90,29 @@
     # ----------------------------------------------------------------------------------------
     async def activate_coro(self) -> None:
         """
         Activate the direct collector and web server in a two asyncio tasks.
         """
 
         try:
+            # Turn off noisy debug from the PIL library.
+            logging.getLogger("PIL").setLevel("INFO")
+
             # Build a local collector for our back-end.
             self.__direct_collector = Collectors().build_object(
                 self.specification()["type_specific_tbd"][
                     "direct_collector_specification"
                 ]
             )
 
-            logger.info("[COLSHUT] calling self.__direct_collector.activate()")
             # Get the local implementation started.
             await self.__direct_collector.activate()
 
-            # ----------------------------------------------
-            logger.info("[COLSHUT] calling BaseAiohttp.activate_coro_base(self)")
             await BaseAiohttp.activate_coro_base(self)
 
-            logger.info("[COLSHUT] returning")
-
         except Exception as exception:
             raise RuntimeError(
                 "exception while starting collector server"
             ) from exception
 
     # ----------------------------------------------------------------------------------------
     async def direct_shutdown(self) -> None:
```

### Comparing `rockingester-2.2.0/src/rockingester_lib/collectors/base.py` & `rockingester-2.2.1/src/rockingester_lib/collectors/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_lib/collectors/collectors.py` & `rockingester-2.2.1/src/rockingester_lib/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_lib/collectors/context.py` & `rockingester-2.2.1/src/rockingester_lib/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_lib/collectors/direct_poll.py` & `rockingester-2.2.1/src/rockingester_lib/collectors/direct_poll.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,17 +134,15 @@
             # Wait for the ticking to stop.
             await self.__tick_future
 
         # Forget we have an xchembku client reference.
         self.__xchembku = None
 
         if self.__xchembku_client_context is not None:
-            logger.debug(f"[ECHDON] {callsign(self)} exiting __xchembku_client_context")
             await self.__xchembku_client_context.aexit()
-            logger.debug(f"[ECHDON] {callsign(self)} exited __xchembku_client_context")
             self.__xchembku_client_context = None
 
     # ----------------------------------------------------------------------------------------
     async def tick(self) -> None:
         """
         A coro task which does periodic checking for new files in the directories.
 
@@ -209,21 +207,28 @@
         if not plates_directory.is_dir():
             return
 
         plate_names = [
             entry.name for entry in os.scandir(plates_directory) if entry.is_dir()
         ]
 
-        logger.info(
+        # Make sure we scrape the plate directories in barcode-order, which is the same as date order.
+        plate_names.sort()
+
+        logger.debug(
             f"[ROCKINGESTER POLL] found {len(plate_names)} plate directories in {plates_directory}"
         )
 
         for plate_name in plate_names:
             # We already handled this plate name?
             if plate_name in self.__handled_plate_names:
+                # logger.debug(
+                #     f"[ROCKINGESTER POLL] plate_barcode {plate_barcode}"
+                #     f" is already handled in this instance"
+                # )
                 continue
 
             # Get the plate's barcode from the directory name.
             plate_barcode = plate_name[0:4]
 
             # We have a specific list we want to process?
             if self.__ingest_only_barcodes is not None:
@@ -231,40 +236,51 @@
                     continue
 
             # Get the matching plate record from the database.
             crystal_plate_model = self.__crystal_plate_models_by_barcode.get(
                 plate_barcode
             )
 
-            # This plate is not in the database?
+            # This plate directory's barcode is not in the database?
             if crystal_plate_model is None:
+                # logger.debug(
+                #     f"[ROCKINGESTER POLL] plate_barcode {plate_barcode} is not in the database"
+                # )
                 continue
-
             try:
+                # Try to get the visit directory from the visit stored in the database's plate record.
                 visit_directory = Path(
                     get_xchem_directory(
                         self.__visits_directory, crystal_plate_model.visit
                     )
                 )
             # This is an improperly formatted visit name?
             except ValueError:
+                # logger.debug(
+                #     f"[ROCKINGESTER POLL] plate_barcode {plate_barcode}"
+                #     f" is in the database, but visit {crystal_plate_model.visit} is improperly formed"
+                # )
                 continue
             # This visit is not found on disk?
             except VisitNotFound:
+                # logger.debug(
+                #     f"[ROCKINGESTER POLL] plate_barcode {plate_barcode}"
+                #     f" is in the database, but cannot find visit directory in {self.__visits_directory}"
+                # )
                 continue
 
             # Scrape the directory when all image files have arrived.
-            await self.scrape_plate_directory_when_complete(
+            await self.scrape_plate_directory_if_complete(
                 plates_directory / plate_name,
                 crystal_plate_model,
                 visit_directory,
             )
 
     # ----------------------------------------------------------------------------------------
-    async def scrape_plate_directory_when_complete(
+    async def scrape_plate_directory_if_complete(
         self,
         plate_directory: Path,
         crystal_plate_model: CrystalPlateModel,
         visit_directory: Path,
     ) -> None:
         """
         Scrape a single directory looking for new files.
@@ -275,21 +291,25 @@
         """
 
         # Name of the destination directory where we will permanently store ingested well image files.
         target = (
             visit_directory / self.__visit_plates_subdirectory / plate_directory.name
         )
 
-        # We have already put this plate directory into the visit directory and presumably also the database?
+        # We have already put this plate directory into the visit directory?
+        # This shouldn't really happen except when someone has been fiddling with the database.
+        # TODO: Have a way to rebuild rockingest after database wipe, but images have already been copied to the visit.
         if target.is_dir():
-            # Remember we "handled" this one.
-            self.__handled_plate_names.append(plate_directory.stem)
+            # Presumably this is done, so no error but log it.
+            # logger.debug(
+            #     f"[ROCKINGESTER POLL] plate_barcode {plate_directory.name} is apparently already copied to {target}"
+            # )
             return
 
-        # This is the first time we have scraped a directory for this plate?
+        # This is the first time we have scraped a directory for this plate record in the database?
         if crystal_plate_model.rockminer_collected_stem is None:
             # Update the path stem in the crystal plate record.
             # TODO: Consider if important to report/record same barcodes on different rockmaker directories.
             crystal_plate_model.rockminer_collected_stem = plate_directory.stem
             await self.__xchembku.upsert_crystal_plates(
                 [crystal_plate_model], "update rockminer_collected_stem"
             )
@@ -323,14 +343,15 @@
                 target,
             )
 
             # Append well model to the list of all wells on the plate.
             crystal_well_models.append(crystal_well_model)
 
         # Here we create or update the crystal well records into xchembku.
+        # TODO: Make sure that direct_poll does not double-create crystal well records if scrape is re-run with a different filename path.
         await self.__xchembku.upsert_crystal_wells(crystal_well_models)
 
         # Copy scraped directory to visit, replacing what might already be there.
         # TODO: Handle case where we upsert the crystal_well record but then unable to copy image file.
         shutil.copytree(
             plate_directory,
             target,
@@ -359,15 +380,15 @@
         """
 
         input_well_filename = plate_directory / subwell_name
         ingested_well_filename = target / subwell_name
 
         # Stems are like "9acx_01A_1".
         # Convert the stem into a position as shown in soakdb3.
-        position = crystal_plate_object.normalize_subwell_name(subwell_name)
+        position = crystal_plate_object.normalize_subwell_name(Path(subwell_name).stem)
 
         error = None
         try:
             image = Image.open(input_well_filename)
             width, height = image.size
         except Exception as exception:
             error = str(exception)
```

### Comparing `rockingester-2.2.0/src/rockingester_lib/contexts/base.py` & `rockingester-2.2.1/src/rockingester_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_lib/exceptions.py` & `rockingester-2.2.1/src/rockingester_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/src/rockingester_lib/version.py` & `rockingester-2.2.1/src/rockingester_lib/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/tests/base.py` & `rockingester-2.2.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/tests/configurations/direct_poll.yaml` & `rockingester-2.2.1/tests/configurations/direct_poll.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/tests/configurations/service.yaml` & `rockingester-2.2.1/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/tests/conftest.py` & `rockingester-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.0/tests/test_collector.py` & `rockingester-2.2.1/tests/test_collector.py`

 * *Files identical despite different names*

