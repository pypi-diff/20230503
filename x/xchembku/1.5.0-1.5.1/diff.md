# Comparing `tmp/xchembku-1.5.0.tar.gz` & `tmp/xchembku-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchembku-1.5.0.tar", last modified: Tue May  2 08:40:34 2023, max compression
+gzip compressed data, was "xchembku-1.5.1.tar", last modified: Wed May  3 05:00:35 2023, max compression
```

## Comparing `xchembku-1.5.0.tar` & `xchembku-1.5.1.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.407821 xchembku-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-02 08:40:24.000000 xchembku-1.5.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-02 08:40:24.000000 xchembku-1.5.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-02 08:40:24.000000 xchembku-1.5.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-02 08:40:24.000000 xchembku-1.5.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-02 08:40:24.000000 xchembku-1.5.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-02 08:40:24.000000 xchembku-1.5.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-02 08:40:24.000000 xchembku-1.5.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 08:40:24.000000 xchembku-1.5.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-02 08:40:24.000000 xchembku-1.5.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-02 08:40:24.000000 xchembku-1.5.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-02 08:40:24.000000 xchembku-1.5.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-02 08:40:24.000000 xchembku-1.5.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.391821 xchembku-1.5.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-02 08:40:24.000000 xchembku-1.5.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-02 08:40:24.000000 xchembku-1.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-02 08:40:24.000000 xchembku-1.5.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-02 08:40:24.000000 xchembku-1.5.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-02 08:40:24.000000 xchembku-1.5.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-02 08:40:24.000000 xchembku-1.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-02 08:40:24.000000 xchembku-1.5.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-02 08:40:24.000000 xchembku-1.5.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-02 08:40:24.000000 xchembku-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-02 08:40:24.000000 xchembku-1.5.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-02 08:40:24.000000 xchembku-1.5.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 08:40:24.000000 xchembku-1.5.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-02 08:40:24.000000 xchembku-1.5.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-02 08:40:24.000000 xchembku-1.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 08:40:24.000000 xchembku-1.5.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 08:40:24.000000 xchembku-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-02 08:40:34.407821 xchembku-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-02 08:40:24.000000 xchembku-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-02 08:40:24.000000 xchembku-1.5.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.391821 xchembku-1.5.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.395821 xchembku-1.5.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 08:40:24.000000 xchembku-1.5.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-02 08:40:24.000000 xchembku-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 08:40:34.407821 xchembku-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.391821 xchembku-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/src/xchembku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-02 08:40:34.000000 xchembku-1.5.0/src/xchembku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-02 08:40:34.000000 xchembku-1.5.0/src/xchembku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:40:34.000000 xchembku-1.5.0/src/xchembku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 08:40:34.000000 xchembku-1.5.0/src/xchembku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-02 08:40:34.000000 xchembku-1.5.0/src/xchembku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 08:40:34.000000 xchembku-1.5.0/src/xchembku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/src/xchembku_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/src/xchembku_api/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/crystal_plate_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/crystal_plate_objects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/crystal_plate_objects/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/src/xchembku_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/src/xchembku_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/src/xchembku_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/models/crystal_plate_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/models/crystal_plate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/models/crystal_well_autolocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/models/crystal_well_droplocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/models/crystal_well_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/models/crystal_well_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.399821 xchembku-1.5.0/src/xchembku_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.403821 xchembku-1.5.0/src/xchembku_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.403821 xchembku-1.5.0/src/xchembku_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 08:40:34.000000 xchembku-1.5.0/src/xchembku_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.403821 xchembku-1.5.0/src/xchembku_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/contexts/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.403821 xchembku-1.5.0/src/xchembku_lib/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/crystal_plate_objects/swiss3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.403821 xchembku-1.5.0/src/xchembku_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/databases/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.403821 xchembku-1.5.0/src/xchembku_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/direct_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-02 08:40:24.000000 xchembku-1.5.0/src/xchembku_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.403821 xchembku-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.407821 xchembku-1.5.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/configurations/direct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/test_crystal_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/test_crystal_well_autolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/test_crystal_well_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/test_soakdb3_crystal_well.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-02 08:40:24.000000 xchembku-1.5.0/tests/test_swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.402099 xchembku-1.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 05:00:25.000000 xchembku-1.5.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-03 05:00:25.000000 xchembku-1.5.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-03 05:00:25.000000 xchembku-1.5.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.386099 xchembku-1.5.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-03 05:00:25.000000 xchembku-1.5.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-03 05:00:25.000000 xchembku-1.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-03 05:00:25.000000 xchembku-1.5.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 05:00:25.000000 xchembku-1.5.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 05:00:25.000000 xchembku-1.5.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 05:00:25.000000 xchembku-1.5.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 05:00:25.000000 xchembku-1.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-03 05:00:25.000000 xchembku-1.5.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 05:00:25.000000 xchembku-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-03 05:00:35.402099 xchembku-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-03 05:00:25.000000 xchembku-1.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-03 05:00:25.000000 xchembku-1.5.1/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.386099 xchembku-1.5.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 05:00:25.000000 xchembku-1.5.1/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-03 05:00:25.000000 xchembku-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 05:00:35.402099 xchembku-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.390099 xchembku-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/src/xchembku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.394099 xchembku-1.5.1/src/xchembku_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_plate_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_plate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_autolocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_droplocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 05:00:35.000000 xchembku-1.5.1/src/xchembku_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/contexts/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.398099 xchembku-1.5.1/src/xchembku_lib/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.402099 xchembku-1.5.1/src/xchembku_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-03 05:00:25.000000 xchembku-1.5.1/src/xchembku_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.402099 xchembku-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:00:35.402099 xchembku-1.5.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/configurations/direct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_crystal_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_crystal_well_autolocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_crystal_well_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_soakdb3_crystal_well.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-03 05:00:25.000000 xchembku-1.5.1/tests/test_swiss3.py
```

### Comparing `xchembku-1.5.0/.dae-devops/Makefile` & `xchembku-1.5.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.dae-devops/docs/conventions.rst` & `xchembku-1.5.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.dae-devops/docs/developing.rst` & `xchembku-1.5.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.dae-devops/docs/devops.rst` & `xchembku-1.5.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.dae-devops/docs/docs_structure.rst` & `xchembku-1.5.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.dae-devops/docs/installing.rst` & `xchembku-1.5.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.dae-devops/docs/testing.rst` & `xchembku-1.5.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.dae-devops/project.yaml` & `xchembku-1.5.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.devcontainer/Dockerfile` & `xchembku-1.5.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.devcontainer/devcontainer.json` & `xchembku-1.5.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.github/CONTRIBUTING.rst` & `xchembku-1.5.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.github/actions/install_requirements/action.yml` & `xchembku-1.5.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.github/dependabot.yml` & `xchembku-1.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.github/pages/make_switcher.py` & `xchembku-1.5.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.github/workflows/code.yml` & `xchembku-1.5.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.github/workflows/docs.yml` & `xchembku-1.5.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.github/workflows/docs_clean.yml` & `xchembku-1.5.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.github/workflows/linkcheck.yml` & `xchembku-1.5.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.gitignore` & `xchembku-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.gitlab-ci.yml` & `xchembku-1.5.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/.vscode/launch.json` & `xchembku-1.5.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/LICENSE` & `xchembku-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/PKG-INFO` & `xchembku-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.5.0
+Version: 1.5.1
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.5.0/README.rst` & `xchembku-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/configurations/development.yaml` & `xchembku-1.5.1/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/docs/conf.py` & `xchembku-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/docs/images/dls-favicon.ico` & `xchembku-1.5.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/docs/images/dls-logo.svg` & `xchembku-1.5.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/docs/index.rst` & `xchembku-1.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/docs/user/explanations/25-docs-structure.rst` & `xchembku-1.5.1/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/docs/user/index.rst` & `xchembku-1.5.1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/pyproject.toml` & `xchembku-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku.egg-info/PKG-INFO` & `xchembku-1.5.1/src/xchembku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.5.0
+Version: 1.5.1
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.5.0/src/xchembku.egg-info/SOURCES.txt` & `xchembku-1.5.1/src/xchembku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/context_base.py` & `xchembku-1.5.1/src/xchembku_api/context_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/crystal_plate_objects/constants.py` & `xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/constants.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/crystal_plate_objects/interface.py` & `xchembku-1.5.1/src/xchembku_api/crystal_plate_objects/interface.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/datafaces/aiohttp.py` & `xchembku-1.5.1/src/xchembku_api/datafaces/aiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,28 +214,14 @@
             "originate_crystal_well_autolocations_serialized",
             records,
         )
 
         return None
 
     # ----------------------------------------------------------------------------------------
-    async def originate_crystal_well_droplocations(
-        self, models: List[CrystalWellDroplocationModel]
-    ) -> None:
-        """"""
-
-        records: List[Dict] = [model.dict() for model in models]
-        await self.__send_protocolj(
-            "originate_crystal_well_droplocations_serialized",
-            records,
-        )
-
-        return None
-
-    # ----------------------------------------------------------------------------------------
     async def upsert_crystal_well_droplocations(
         self,
         models: List[CrystalWellDroplocationModel],
         only_fields: Optional[List[str]] = None,
         why: Optional[str] = None,
     ) -> None:
         """"""
```

### Comparing `xchembku-1.5.0/src/xchembku_api/datafaces/context.py` & `xchembku-1.5.1/src/xchembku_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/datafaces/datafaces.py` & `xchembku-1.5.1/src/xchembku_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/exceptions.py` & `xchembku-1.5.1/src/xchembku_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/models/crystal_plate_model.py` & `xchembku-1.5.1/src/xchembku_api/models/crystal_plate_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/models/crystal_well_autolocation_model.py` & `xchembku-1.5.1/src/xchembku_api/models/crystal_well_autolocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/models/crystal_well_droplocation_model.py` & `xchembku-1.5.1/src/xchembku_api/models/crystal_well_droplocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/models/crystal_well_model.py` & `xchembku-1.5.1/src/xchembku_api/models/crystal_well_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py` & `xchembku-1.5.1/src/xchembku_api/models/crystal_well_needing_droplocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_cli/main.py` & `xchembku-1.5.1/src/xchembku_cli/main.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_cli/subcommands/base.py` & `xchembku-1.5.1/src/xchembku_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_cli/subcommands/service.py` & `xchembku-1.5.1/src/xchembku_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_cli/version.py` & `xchembku-1.5.1/src/xchembku_cli/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/__main__.py` & `xchembku-1.5.1/src/xchembku_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/contexts/base.py` & `xchembku-1.5.1/src/xchembku_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py` & `xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from xchembku_api.exceptions import NotFound
 
 logger = logging.getLogger(__name__)
 
 
 class CrystalPlateObjects(Things):
     """
-    List of available databases.
+    List of available crystal plate object types.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, name=None):
         Things.__init__(self, name)
 
     # ----------------------------------------------------------------------------------------
@@ -37,25 +37,23 @@
             List[str]: names
         """
 
         return list(self.__treenode_names_to_thing_type.keys())
 
     # ----------------------------------------------------------------------------------------
     def build_object(self, specification) -> CrystalPlateInterface:
-        """
-        TODO: CrystalPlateObjects build_object method should return an interface.
-        """
+        """ """
 
         object_class = self.lookup_class(specification["type"])
 
         try:
             object_instance = object_class(specification)
         except Exception as exception:
             raise RuntimeError(
-                "unable to build database object for type %s" % object_class
+                "unable to build object for type %s" % object_class
             ) from exception
 
         return object_instance
 
     # ----------------------------------------------------------------------------------------
     def lookup_class(self, class_type):
         """
@@ -63,8 +61,8 @@
         """
 
         if class_type == ThingTypes.SWISS3:
             from xchembku_lib.crystal_plate_objects.swiss3 import Swiss3
 
             return Swiss3
 
-        raise NotFound("unable to get database class for type %s" % (class_type))
+        raise NotFound("unable to get class for type %s" % (class_type))
```

### Comparing `xchembku-1.5.0/src/xchembku_lib/crystal_plate_objects/swiss3.py` & `xchembku-1.5.1/src/xchembku_lib/crystal_plate_objects/swiss3.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/databases/database_definition.py` & `xchembku-1.5.1/src/xchembku_lib/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/databases/databases.py` & `xchembku-1.5.1/src/xchembku_lib/databases/databases.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/databases/normsql.py` & `xchembku-1.5.1/src/xchembku_lib/databases/normsql.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/databases/table_definitions.py` & `xchembku-1.5.1/src/xchembku_lib/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/aiohttp.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/context.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/datafaces.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/direct.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/direct.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/direct_base.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/direct_crystal_plates.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_plates.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,41 +18,14 @@
 upsert_lock = RLock()
 
 
 class DirectCrystalWellDroplocations(DirectBase):
     """ """
 
     # ----------------------------------------------------------------------------------------
-    async def originate_crystal_well_droplocations_serialized(
-        self, records: List[Dict]
-    ) -> None:
-        # We are being given json, so parse it into models.
-        models = [CrystalWellDroplocationModel(**record) for record in records]
-
-        # Return the method doing the work.
-        return await self.originate_crystal_well_droplocations(models)
-
-    # ----------------------------------------------------------------------------------------
-    async def originate_crystal_well_droplocations(
-        self, models: List[CrystalWellDroplocationModel]
-    ) -> None:
-        """
-        Caller provides the records containing fields to be created.
-        """
-
-        # We're being given models, serialize them into dicts for the sql.
-        records = [model.dict() for model in models]
-
-        return await self.insert(
-            "crystal_well_droplocations",
-            records,
-            why="originate_crystal_well_droplocations",
-        )
-
-    # ----------------------------------------------------------------------------------------
     async def upsert_crystal_well_droplocations_serialized(
         self,
         records: List[Dict],
         only_fields: Optional[List[str]] = None,
         why=None,
     ) -> Dict:
         # We are being given json, so parse it into models.
@@ -127,14 +100,15 @@
             why = "upsert_crystal_well_droplocations"
 
         inserted_count = 0
         updated_count = 0
 
         # Loop over all the models to be upserted.
         for model in models:
+            # TODO: Reconsider the lock granularity in direct_crystal_well_droplocations.py.
             with upsert_lock:
                 model_dict = copy.deepcopy(model.dict())
 
                 # Find any existing record for this model object.
                 records = await self.query(
                     "SELECT * FROM crystal_well_droplocations WHERE crystal_well_uuid = ?",
                     subs=[model.crystal_well_uuid],
```

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/direct_crystal_wells.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_crystal_wells.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py` & `xchembku-1.5.1/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/src/xchembku_lib/version.py` & `xchembku-1.5.1/src/xchembku_lib/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/tests/base.py` & `xchembku-1.5.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/tests/configurations/direct.yaml` & `xchembku-1.5.1/tests/configurations/direct.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/tests/configurations/service.yaml` & `xchembku-1.5.1/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/tests/conftest.py` & `xchembku-1.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/tests/test_crystal_plate.py` & `xchembku-1.5.1/tests/test_crystal_plate.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/tests/test_crystal_well_autolocation.py` & `xchembku-1.5.1/tests/test_crystal_well_autolocation.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/tests/test_crystal_well_droplocation.py` & `xchembku-1.5.1/tests/test_crystal_well_droplocation.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/tests/test_soakdb3_crystal_well.py` & `xchembku-1.5.1/tests/test_soakdb3_crystal_well.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.5.0/tests/test_swiss3.py` & `xchembku-1.5.1/tests/test_swiss3.py`

 * *Files identical despite different names*

