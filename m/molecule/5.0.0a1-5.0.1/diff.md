# Comparing `tmp/molecule-5.0.0a1.tar.gz` & `tmp/molecule-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-5.0.0a1.tar", last modified: Wed Apr 19 17:52:07 2023, max compression
+gzip compressed data, was "molecule-5.0.1.tar", last modified: Wed May  3 13:49:22 2023, max compression
```

## Comparing `molecule-5.0.0a1.tar` & `molecule-5.0.1.tar`

### file list

```diff
@@ -1,422 +1,430 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.041295 molecule-5.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.965293 molecule-5.0.0a1/.config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.965293 molecule-5.0.0a1/.config/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.config/molecule/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.config/molecule.spec
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.969293 molecule-5.0.0a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.969293 molecule-5.0.0a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/patchback.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.969293 molecule-5.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.npmrc
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.969293 molecule-5.0.0a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-19 17:51:46.000000 molecule-5.0.0a1/DCO_1_1.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-19 17:51:46.000000 molecule-5.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 17:51:46.000000 molecule-5.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-19 17:52:07.041295 molecule-5.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-19 17:51:46.000000 molecule-5.0.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-19 17:51:47.000000 molecule-5.0.0a1/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-19 17:51:47.000000 molecule-5.0.0a1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-19 17:51:47.000000 molecule-5.0.0a1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.973293 molecule-5.0.0a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.933292 molecule-5.0.0a1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.973293 molecule-5.0.0a1/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/_static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   143898 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/_static/images/logo_big.png
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/ci.md
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/getting-started.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.973293 molecule-5.0.0a1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-19 17:51:47.000000 molecule-5.0.0a1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-19 17:51:47.000000 molecule-5.0.0a1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.973293 molecule-5.0.0a1/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-19 17:51:47.000000 molecule-5.0.0a1/playbooks/snap-pre-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-19 17:51:47.000000 molecule-5.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-19 17:51:47.000000 molecule-5.0.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 17:51:47.000000 molecule-5.0.0a1/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:52:07.041295 molecule-5.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.977293 molecule-5.0.0a1/snap/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 17:51:47.000000 molecule-5.0.0a1/snap/snapcraft.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.981293 molecule-5.0.0a1/src/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/command/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/idempotence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/command/init/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/side_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/data/driver.json
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/data/molecule.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/driver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/driver/delegated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/model/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/model/schema_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/platforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/provisioner/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34238 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/functional/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/invalid_role_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/invalid_role_template/bad_format/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/invalid_role_template/bad_format/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/invalid_role_template/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/test/resources/playbooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/invalid/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/valid/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/templates/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/hosts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.957293 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.021294 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.021294 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.021294 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.021294 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.025295 molecule-5.0.0a1/src/molecule/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.029295 molecule-5.0.0a1/src/molecule/test/unit/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.029295 molecule-5.0.0a1/src/molecule/test/unit/command/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/init/test_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/init/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_idempotence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_side_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/cookiecutter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/cookiecutter/test_molecule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/driver/test_delegated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/lint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/lint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/model/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_dependency_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_driver_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_platforms_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_provisioner_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_scenario_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_verifier_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.037295 molecule-5.0.0a1/src/molecule/test/unit/provisioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25691 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_scenarios_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.037295 molecule-5.0.0a1/src/molecule/test/unit/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/verifier/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/verifier/test_testinfra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.037295 molecule-5.0.0a1/src/molecule/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/verifier/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/verifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/verifier/testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.981293 molecule-5.0.0a1/src/molecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.041295 molecule-5.0.0a1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/get-version.sh
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/opts.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/smoketest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/test-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/update-version.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.603660 molecule-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 13:49:06.000000 molecule-5.0.1/.ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-03 13:49:06.000000 molecule-5.0.1/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.515658 molecule-5.0.1/.config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.515658 molecule-5.0.1/.config/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 13:49:06.000000 molecule-5.0.1/.config/molecule/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-03 13:49:06.000000 molecule-5.0.1/.config/molecule.spec
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 13:49:06.000000 molecule-5.0.1/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-03 13:49:06.000000 molecule-5.0.1/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-03 13:49:06.000000 molecule-5.0.1/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 13:49:06.000000 molecule-5.0.1/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-03 13:49:06.000000 molecule-5.0.1/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 13:49:06.000000 molecule-5.0.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-03 13:49:06.000000 molecule-5.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.515658 molecule-5.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.519658 molecule-5.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/patchback.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.519658 molecule-5.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/workflows/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-03 13:49:06.000000 molecule-5.0.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-03 13:49:06.000000 molecule-5.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 13:49:06.000000 molecule-5.0.1/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 13:49:06.000000 molecule-5.0.1/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-03 13:49:06.000000 molecule-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 13:49:06.000000 molecule-5.0.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.519658 molecule-5.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 13:49:06.000000 molecule-5.0.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-03 13:49:06.000000 molecule-5.0.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-03 13:49:06.000000 molecule-5.0.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-03 13:49:06.000000 molecule-5.0.1/DCO_1_1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-03 13:49:06.000000 molecule-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 13:49:06.000000 molecule-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-03 13:49:22.603660 molecule-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-03 13:49:06.000000 molecule-5.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-03 13:49:06.000000 molecule-5.0.1/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 13:49:06.000000 molecule-5.0.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-03 13:49:06.000000 molecule-5.0.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.523658 molecule-5.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.483657 molecule-5.0.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.523658 molecule-5.0.1/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/_static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   143898 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/_static/images/logo_big.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/ci.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12910 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/google04e29a42ae6e6cbc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.523658 molecule-5.0.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-03 13:49:06.000000 molecule-5.0.1/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-03 13:49:06.000000 molecule-5.0.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-03 13:49:06.000000 molecule-5.0.1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.523658 molecule-5.0.1/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-03 13:49:06.000000 molecule-5.0.1/playbooks/snap-pre-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-03 13:49:06.000000 molecule-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-03 13:49:06.000000 molecule-5.0.1/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:49:22.603660 molecule-5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.523658 molecule-5.0.1/snap/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-03 13:49:06.000000 molecule-5.0.1/snap/snapcraft.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.483657 molecule-5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.531659 molecule-5.0.1/src/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 13:49:22.000000 molecule-5.0.1/src/molecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.535658 molecule-5.0.1/src/molecule/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/idempotence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.539659 molecule-5.0.1/src/molecule/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/init/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/init/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/init/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/init/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/command/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.487657 molecule-5.0.1/src/molecule/cookiecutter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.539659 molecule-5.0.1/src/molecule/cookiecutter/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/molecule/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.539659 molecule-5.0.1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.487657 molecule-5.0.1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.539659 molecule-5.0.1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.487657 molecule-5.0.1/src/molecule/cookiecutter/scenario/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.487657 molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.539659 molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.487657 molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.539659 molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.487657 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.539659 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/ansible/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.487657 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.539659 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.539659 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/testinfra/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.487657 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.487657 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.543659 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.543659 molecule-5.0.1/src/molecule/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/data/driver.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/data/molecule.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.543659 molecule-5.0.1/src/molecule/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.543659 molecule-5.0.1/src/molecule/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/dependency/ansible_galaxy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/dependency/ansible_galaxy/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/dependency/ansible_galaxy/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/dependency/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.547659 molecule-5.0.1/src/molecule/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/driver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/driver/delegated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.547659 molecule-5.0.1/src/molecule/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/model/schema_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/platforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.547659 molecule-5.0.1/src/molecule/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34235 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/provisioner/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/provisioner/ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/provisioner/ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/provisioner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.547659 molecule-5.0.1/src/molecule/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.547659 molecule-5.0.1/src/molecule/test/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/functional/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/invalid_role_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/invalid_role_template/bad_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/invalid_role_template/bad_format/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/invalid_role_template/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.491657 molecule-5.0.1/src/molecule/test/resources/playbooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/playbooks/delegated/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/playbooks/delegated/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/playbooks/delegated/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.491657 molecule-5.0.1/src/molecule/test/resources/playbooks/delegated/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.491657 molecule-5.0.1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.491657 molecule-5.0.1/src/molecule/test/resources/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.491657 molecule-5.0.1/src/molecule/test/resources/roles/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/roles/molecule/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/roles/molecule/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/roles/molecule/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/roles/molecule/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/sample-collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/sample-collection/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.491657 molecule-5.0.1/src/molecule/test/resources/sample-collection/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/sample-collection/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.491657 molecule-5.0.1/src/molecule/test/resources/sample-collection/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.495657 molecule-5.0.1/src/molecule/test/resources/sample-collection/roles/get_rich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.495657 molecule-5.0.1/src/molecule/test/resources/schema_instance_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.551659 molecule-5.0.1/src/molecule/test/resources/schema_instance_files/invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.555659 molecule-5.0.1/src/molecule/test/resources/schema_instance_files/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.555659 molecule-5.0.1/src/molecule/test/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/templates/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.555659 molecule-5.0.1/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.555659 molecule-5.0.1/src/molecule/test/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.495657 molecule-5.0.1/src/molecule/test/scenarios/cleanup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.495657 molecule-5.0.1/src/molecule/test/scenarios/cleanup/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.555659 molecule-5.0.1/src/molecule/test/scenarios/cleanup/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.555659 molecule-5.0.1/src/molecule/test/scenarios/cleanup/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.495657 molecule-5.0.1/src/molecule/test/scenarios/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.495657 molecule-5.0.1/src/molecule/test/scenarios/dependency/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.555659 molecule-5.0.1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.555659 molecule-5.0.1/src/molecule/test/scenarios/dependency/molecule/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.499657 molecule-5.0.1/src/molecule/test/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.495657 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.559659 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.495657 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.559659 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.499657 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.559659 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.499657 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.559659 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.559659 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.499657 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.559659 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.563659 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/host_vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.563659 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/hosts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.499657 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.563659 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.499657 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.563659 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.499657 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.563659 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.563659 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.499657 molecule-5.0.1/src/molecule/test/scenarios/idempotence/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.499657 molecule-5.0.1/src/molecule/test/scenarios/idempotence/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.563659 molecule-5.0.1/src/molecule/test/scenarios/idempotence/molecule/raises/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.563659 molecule-5.0.1/src/molecule/test/scenarios/idempotence/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/idempotence/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.503658 molecule-5.0.1/src/molecule/test/scenarios/interpolation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.503658 molecule-5.0.1/src/molecule/test/scenarios/interpolation/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.563659 molecule-5.0.1/src/molecule/test/scenarios/interpolation/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.503658 molecule-5.0.1/src/molecule/test/scenarios/overrride_driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.503658 molecule-5.0.1/src/molecule/test/scenarios/overrride_driver/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.567659 molecule-5.0.1/src/molecule/test/scenarios/overrride_driver/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.503658 molecule-5.0.1/src/molecule/test/scenarios/side_effect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.503658 molecule-5.0.1/src/molecule/test/scenarios/side_effect/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.567659 molecule-5.0.1/src/molecule/test/scenarios/side_effect/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.567659 molecule-5.0.1/src/molecule/test/scenarios/side_effect/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.503658 molecule-5.0.1/src/molecule/test/scenarios/test_destroy_strategy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.503658 molecule-5.0.1/src/molecule/test/scenarios/test_destroy_strategy/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.571659 molecule-5.0.1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.571659 molecule-5.0.1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.571659 molecule-5.0.1/src/molecule/test/scenarios/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.503658 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.571659 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.571659 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.575660 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.571659 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.571659 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.579660 molecule-5.0.1/src/molecule/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.587660 molecule-5.0.1/src/molecule/test/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.587660 molecule-5.0.1/src/molecule/test/unit/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/init/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/init/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_idempotence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/command/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.587660 molecule-5.0.1/src/molecule/test/unit/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/cookiecutter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/cookiecutter/test_molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.591660 molecule-5.0.1/src/molecule/test/unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.591660 molecule-5.0.1/src/molecule/test/unit/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/dependency/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.591660 molecule-5.0.1/src/molecule/test/unit/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/driver/test_delegated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.591660 molecule-5.0.1/src/molecule/test/unit/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/lint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.591660 molecule-5.0.1/src/molecule/test/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.595660 molecule-5.0.1/src/molecule/test/unit/model/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/v2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/v2/test_dependency_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/v2/test_driver_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/v2/test_platforms_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/v2/test_provisioner_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/v2/test_scenario_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/v2/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/model/v2/test_verifier_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.599660 molecule-5.0.1/src/molecule/test/unit/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25691 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/provisioner/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/provisioner/test_ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/provisioner/test_ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_scenarios_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.599660 molecule-5.0.1/src/molecule/test/unit/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/verifier/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/test/unit/verifier/test_testinfra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.599660 molecule-5.0.1/src/molecule/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/verifier/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/verifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-03 13:49:06.000000 molecule-5.0.1/src/molecule/verifier/testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.531659 molecule-5.0.1/src/molecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-03 13:49:22.000000 molecule-5.0.1/src/molecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-03 13:49:22.000000 molecule-5.0.1/src/molecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:49:22.000000 molecule-5.0.1/src/molecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 13:49:22.000000 molecule-5.0.1/src/molecule.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-03 13:49:22.000000 molecule-5.0.1/src/molecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 13:49:22.000000 molecule-5.0.1/src/molecule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:49:22.603660 molecule-5.0.1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-05-03 13:49:06.000000 molecule-5.0.1/tools/get-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:49:06.000000 molecule-5.0.1/tools/opts.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-05-03 13:49:06.000000 molecule-5.0.1/tools/smoketest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-03 13:49:06.000000 molecule-5.0.1/tools/test-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-05-03 13:49:06.000000 molecule-5.0.1/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-03 13:49:06.000000 molecule-5.0.1/tox.ini
```

### Comparing `molecule-5.0.0a1/.config/molecule.spec` & `molecule-5.0.1/.config/molecule.spec`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/.gitattributes` & `molecule-5.0.1/.gitattributes`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md` & `molecule-5.0.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/.github/ISSUE_TEMPLATE/config.yml` & `molecule-5.0.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/.github/dependabot.yml` & `molecule-5.0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/.github/workflows/release.yml` & `molecule-5.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/.github/workflows/tox.yml` & `molecule-5.0.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/.packit.yaml` & `molecule-5.0.1/.packit.yaml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/.pre-commit-config.yaml` & `molecule-5.0.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,18 @@
           (?x)^(
             src/molecule/cookiecutter/.*|
             src/molecule/test/resources/templates/.*|
           )$
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
-  - repo: https://github.com/PyCQA/doc8
-    rev: "v1.1.1"
-    hooks:
-      - id: doc8
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
     rev: v4.4.0
@@ -53,28 +45,28 @@
     rev: v1.30.0
     hooks:
       - id: yamllint
         files: \.(yaml|yml)$
         types: [file, yaml]
         entry: yamllint --strict
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.261"
+    rev: "v0.0.262"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: []
         entry: mypy src/
         pass_filenames: false
         additional_dependencies:
-          - ansible-compat>=2.2.0
+          - ansible-compat>=2.2.0,<4.0.0
           - click>=8.0.1
           - enrich>=1.2.7
           - importlib-metadata>=4.6.1
           - jinja2
           - packaging
           - rich
           - ruamel.yaml>=0.17.10
@@ -85,27 +77,40 @@
   - repo: https://github.com/pycqa/pylint
     rev: v3.0.0a6
     hooks:
       - id: pylint
         args:
           - --output-format=colorized
         additional_dependencies:
-          - ansible-compat>=2.2.0
+          - ansible-compat>=2.2.0,<4.0.0
           - click
           - click-help-colors
           - cookiecutter
           - enrich>=1.2.7
           - filelock
           - jsonschema
           - pexpect
           - testinfra
   - repo: https://github.com/jazzband/pip-tools
     rev: 6.13.0
     hooks:
       - id: pip-compile
-        entry: pip-compile -q --resolver=backtracking --strip-extras --no-annotate --output-file=requirements.txt tools/opts.txt pyproject.toml --extra docs --extra test --extra lint
-        files: ^(pyproject\.toml|requirements.txt|constraints\.txt)$
+        entry: pip-compile -q --resolver=backtracking --strip-extras --no-annotate --output-file=.config/requirements.txt pyproject.toml --extra docs --extra test
+        files: ^(pyproject\.toml|\.config\/.*)$
       - id: pip-compile
         name: pip-compile-upgrade
-        entry: pip-compile -q  --resolver=backtracking --strip-extras -q --upgrade --no-annotate --output-file=requirements.txt tools/opts.txt pyproject.toml --extra docs --extra test --extra lint
-        files: ^(pyproject\.toml|requirements.txt|constraints\.txt)$
+        alias: up
+        entry: pip-compile -q  --resolver=backtracking --strip-extras -q --upgrade --no-annotate --output-file=.config/requirements.txt pyproject.toml --extra docs --extra test
+        files: ^(pyproject\.toml|\.config\/.*)$
+        stages: [manual]
+      - id: pip-compile
+        name: lock
+        alias: lock
+        always_run: true
+        entry: pip-compile --upgrade --resolver=backtracking --no-annotate --output-file=.config/requirements-lock.txt pyproject.toml --strip-extras --unsafe-package ruamel-yaml-clib
+        files: ^.config\/requirements.*$
+        language: python
+        language_version: "3.9" # minimal we support officially
+        pass_filenames: false
         stages: [manual]
+        additional_dependencies:
+          - pip>=22.3.1
```

### Comparing `molecule-5.0.0a1/.vscode/settings.json` & `molecule-5.0.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/.yamllint` & `molecule-5.0.1/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/DCO_1_1.md` & `molecule-5.0.1/DCO_1_1.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/LICENSE` & `molecule-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/PKG-INFO` & `molecule-5.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 5.0.0a1
+Version: 5.0.1
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
@@ -12,30 +12,31 @@
 Keywords: ansible,roles,testing,molecule
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: lint
 Provides-Extra: test
+Provides-Extra: lock
 License-File: LICENSE
 
 # About Ansible Molecule
 
 [![PyPI Package](https://img.shields.io/pypi/v/molecule)](https://pypi.org/project/molecule/)
 [![Documentation Status](https://readthedocs.org/projects/molecule/badge/?version=latest)](https://molecule.readthedocs.io/en/latest/)
 [![image](https://github.com/ansible-community/molecule/workflows/tox/badge.svg)](https://github.com/ansible-community/molecule/actions)
```

### Comparing `molecule-5.0.0a1/README.md` & `molecule-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/bindep.txt` & `molecule-5.0.1/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/conftest.py` & `molecule-5.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/_static/images/favicon.ico` & `molecule-5.0.1/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/_static/images/logo.png` & `molecule-5.0.1/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/_static/images/logo_big.png` & `molecule-5.0.1/docs/_static/images/logo_big.png`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/ci.md` & `molecule-5.0.1/docs/ci.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/configuration.md` & `molecule-5.0.1/docs/configuration.md`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 ::: molecule.provisioner.ansible.Ansible
 
 ## Scenario
 
 Molecule treats scenarios as a first-class citizens, with a top-level
 configuration syntax.
 
-A scenario allows Molecule test a role in a particular way, this is a \
+A scenario allows Molecule to test a role in a particular way, this is a
 fundamental change from Molecule v1.
 
 A scenario is a self-contained directory containing everything necessary
 for testing the role in a particular way. The default scenario is named
 `default`, and every role should contain a default scenario.
 
 Unless mentioned explicitly, the scenario name will be the directory name
```

### Comparing `molecule-5.0.0a1/docs/contributing.md` & `molecule-5.0.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/examples.md` & `molecule-5.0.1/docs/examples.md`

 * *Files 2% similar despite different names*

```diff
@@ -275,17 +275,30 @@
 ```
 
 ## Monolith Repo
 
 Molecule is generally used to test roles in isolation. However, it can
 also test roles from a monolith repo.
 
-> \$ tree monolith-repo -L 3 \--prune monolith-repo ├── library │   └──
-> foo.py ├── plugins │   └── filters │   └── foo.py └── roles ├── bar
-> │   └── README.md ├── baz │   └── README.md └── foo └── README.md
+```bash
+$ tree monolith-repo -L 3 --prune
+monolith-repo
+ ├── library
+ │   └── foo.py
+ ├── plugins
+ │   └── filters
+ │       └── foo.py
+ └── roles
+     ├── bar
+     │   └── README.md
+     ├── baz
+     │   └── README.md
+     └── foo
+         └── README.md
+```
 
 The role initialized with Molecule (baz in this case) would simply
 reference the dependent roles via it's `converge.yml` or meta
 dependencies.
 
 Molecule can test complex scenarios leveraging this technique.
```

### Comparing `molecule-5.0.0a1/docs/faq.md` & `molecule-5.0.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/getting-started.md` & `molecule-5.0.1/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/images/favicon.ico` & `molecule-5.0.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/images/logo.png` & `molecule-5.0.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/images/logo.svg` & `molecule-5.0.1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/index.md` & `molecule-5.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/installation.md` & `molecule-5.0.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/docs/usage.md` & `molecule-5.0.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/mkdocs.yml` & `molecule-5.0.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/mypy.ini` & `molecule-5.0.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/playbooks/snap-pre-run.yaml` & `molecule-5.0.1/playbooks/snap-pre-run.yaml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/pyproject.toml` & `molecule-5.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,53 @@
 [build-system]
 requires = [
-  "setuptools >= 61.0", # PEP-621
-  "setuptools_scm[toml] >= 7.0.0",
+  "setuptools >= 63.0.0", # required by pyproject+setuptools_scm integration
+  "setuptools_scm[toml] >= 7.0.5", # required for "no-local-version" scheme
+
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 # https://peps.python.org/pep-0621/#readme
 requires-python = ">=3.9"
-dynamic = ["version"]
+dynamic = ["version", "dependencies", "optional-dependencies"]
 name = "molecule"
 description = "Molecule aids in the development and testing of Ansible roles"
 readme = "README.md"
 authors = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
 maintainers = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
 license = { text = "MIT" }
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
+  "Operating System :: MacOS",
+  "Operating System :: POSIX",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python",
   "Topic :: System :: Systems Administration",
   "Topic :: Software Development :: Bug Tracking",
   "Topic :: Software Development :: Quality Assurance",
   "Topic :: Software Development :: Testing",
   "Topic :: Utilities",
 ]
 keywords = ["ansible", "roles", "testing", "molecule"]
-dependencies = [
-  "ansible-compat >= 2.2.0",
-  "ansible-core >= 2.12.10",
-  "click >= 8.0, < 9",
-  "click-help-colors >= 0.9",
-  "cookiecutter >= 1.7.3", # dependency issues in older versions
-  "enrich >= 1.2.7",
-  "jsonschema >= 4.9.1",
-  "Jinja2 >= 2.11.3",
-  "packaging",
-  "pluggy >= 0.7.1, < 2.0",
-  "PyYAML >= 5.1",
-  "rich >= 9.5.1",
-]
 
 [project.urls]
 homepage = "https://github.com/ansible-community/molecule"
 documentation = "https://molecule.readthedocs.io/"
 repository = "https://github.com/ansible-community/molecule"
 changelog = "https://github.com/ansible-community/molecule/releases"
 
-[project.optional-dependencies]
-docs = [
-  "argparse-manpage",
-  "cairosvg",
-  "markdown-include",
-  "mkdocs",
-  "mkdocs-git-revision-date-localized-plugin",
-  "mkdocs-material",
-  "mkdocs-material-extensions",
-  "mkdocs-multirepo-plugin",
-  "mkdocstrings[python]",
-  "pillow",
-  "pymdown-extensions",
-]
-lint = [
-  "check-jsonschema >= 0.20.0",
-  "flake8 >= 6.0.0",
-  "jsonschema >= 4.17.3",
-  "pre-commit >= 2.21.0",
-  "yamllint >= 1.28.0",
-]
-test = [
-  # Do not include ansible or any package that would drag ansible in here
-  # We want to assure test extra provides tools to test molecule and its
-  # related tools/plugins but w/o ansible, which can be installed separated.
-  "ansible-lint >= 6.12.1",
-  "ansi2html >= 1.8.0",
-  "coverage >= 7.0.3",
-  "filelock >= 3.9.0",
-  "pexpect >= 4.8.0, < 5",
-  "pytest-mock >= 3.10.0",
-  "pytest-plus >= 0.4.0",
-  "pytest-testinfra >= 7.0.0",
-  "pytest-xdist >= 3.1.0",
-  "pytest >= 7.2.0",
-]
-
 [project.scripts]
 molecule = "molecule.__main__:main"
 
 [project.entry-points."molecule.driver"]
 delegated = "molecule.driver.delegated:Delegated"
 
 [project.entry-points."molecule.verifier"]
@@ -113,26 +64,14 @@
 
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
 omit = ["test/*"]
 fail_under = 88
 skip_covered = true
 
-# skip_empty = true
-[tool.doc8]
-# see https://github.com/PyCQA/doc8/issues/75
-ignore-path = [
-  ".eggs",
-  ".tox",
-  "requirements.txt",
-  "build",
-  "molecule.egg-info",
-  "src/molecule.egg-info",
-]
-
 [tool.black]
 skip-string-normalization = false
 
 [tool.isort]
 profile = "black"
 known_first_party = "molecule"
 
@@ -140,47 +79,33 @@
 disable = [
   # TODO(ssbarnea): remove temporary skips adding during initial adoption:
   "abstract-method",
   "arguments-differ",
   "broad-except",
   "consider-merging-isinstance",
   # We will clean this up in a dedicated refactoring commit
-  "consider-using-in",
   "dangerous-default-value",
   "duplicate-code",
   "fixme",
-  "implicit-str-concat",
   "import-outside-toplevel",
-  "inconsistent-return-statements",
   "invalid-name",
   "line-too-long",
-  "logging-format-interpolation",
-  "logging-not-lazy",
   "missing-function-docstring",
   "missing-module-docstring",
-  "no-else-raise",
-  "no-else-return",
   "no-member",
   "no-self-argument",
   "no-value-for-parameter",
   "not-callable",
   "protected-access",
-  "raise-missing-from",
   "redefined-builtin",
   "redefined-outer-name",
-  "subprocess-run-check",
-  "super-init-not-called",
-  "super-with-arguments",
   "too-few-public-methods",
   "too-many-ancestors",
   "too-many-arguments",
   "too-many-public-methods",
-  "unidiomatic-typecheck",
-  "unnecessary-comprehension",
-  "unnecessary-lambda",
   # Next rule was added because we cannot adjust the open calls during minor
   # releases since there is no guarantee that this will not break existing
   # scenarios (right now, we have no idea what encoding files that molecule
   # wrote to disk have).
   "unspecified-encoding",
   "unused-argument",
   "unused-import",
@@ -221,49 +146,57 @@
   "ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning",
   # ignore::UserWarning
 
 ]
 
 [tool.ruff]
 ignore = [
+  # Disabled on purpose:
   "E501", # we use black
-  # temporary disabled until we fix them:
+  "FBT", # Boolean positional value in function call
+  # Temporary disabled until we fix them:
   "A",
-  "ANN",
+  "ANN", # Annotations
   "ARG",
   "B",
   "BLE001",
   "C901",
   "D",
   "E741",
   "EM",
-  "EXE",
-  "FBT",
   "INP",
-  "ISC",
   "N",
   "PGH",
-  "PLC",
   "PLR",
   "PLW",
   "PT",
   "PTH",
   "RET",
-  "S",
   "SIM",
   "SLF",
   "T",
   "TRY",
 ]
 select = ["ALL"]
 target-version = "py39"
 # Same as Black.
 line-length = 88
 
 [tool.ruff.flake8-pytest-style]
 parametrize-values-type = "tuple"
 
 [tool.ruff.isort]
-known-first-party = ["ansiblelint"]
+known-first-party = ["molecule"]
+
+[tool.ruff.per-file-ignores]
+"src/molecule/test/**.py" = ["S"]
+"src/molecule/*/\\{\\{*/**.py" = ["S"]
+
+[tool.setuptools.dynamic]
+optional-dependencies.docs = { file = [".config/requirements-docs.txt"] }
+optional-dependencies.test = { file = [".config/requirements-test.txt"] }
+optional-dependencies.lock = { file = [".config/requirements-lock.txt"] }
+dependencies = { file = [".config/requirements.in"] }
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
+write_to = "src/molecule/_version.py"
```

### Comparing `molecule-5.0.0a1/requirements.txt` & `molecule-5.0.1/.config/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,117 +1,107 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=docs --extra=lint --extra=test --no-annotate --output-file=requirements.txt --resolver=backtracking --strip-extras pyproject.toml tools/opts.txt
+#    pip-compile --extra=docs --extra=test --no-annotate --output-file=.config/requirements.txt --resolver=backtracking --strip-extras pyproject.toml
 #
 ansi2html==1.8.0
 ansible-compat==3.0.2
 ansible-core==2.14.4
 ansible-lint==6.14.6
-argparse-manpage==4.1
 arrow==1.2.3
-asyncio==3.4.3
 attrs==23.1.0
-babel==2.12.1
+beautifulsoup4==4.12.1
 binaryornot==0.4.4
 black==23.3.0
 bracex==2.3.post1
-cairocffi==1.5.1
+cairocffi==1.5.0
 cairosvg==2.7.0
 certifi==2022.12.7
 cffi==1.15.1
-cfgv==3.3.1
 chardet==5.1.0
 charset-normalizer==3.1.0
 check-jsonschema==0.22.0
 click==8.1.3
 click-help-colors==0.9.1
 colorama==0.4.6
 cookiecutter==2.1.1
 coverage==7.2.3
 cryptography==40.0.2
+csscompressor==0.9.5
 cssselect2==0.7.0
-dacite==1.8.0
 defusedxml==0.7.1
-distlib==0.3.6
-distro==1.8.0
 enrich==1.2.7
 exceptiongroup==1.1.1
 execnet==1.9.0
 filelock==3.12.0
-flake8==6.0.0
 ghp-import==2.1.0
-gitdb==4.0.10
-gitpython==3.1.31
-griffe==0.27.1
-identify==2.5.22
+griffe==0.26.0
+htmlmin2==0.1.13
 idna==3.4
-importlib-metadata==6.5.0
+importlib-metadata==6.1.0
 iniconfig==2.0.0
 jinja2==3.1.2
 jinja2-time==0.2.0
+jsmin==3.0.1
 jsonschema==4.17.3
 markdown==3.3.7
+markdown-exec==1.4.0
 markdown-include==0.8.1
 markdown-it-py==2.2.0
 markupsafe==2.1.2
-mccabe==0.7.0
 mdurl==0.1.2
 mergedeep==1.3.4
 mkdocs==1.4.2
+mkdocs-ansible==0.1.4
 mkdocs-autorefs==0.4.1
-mkdocs-git-revision-date-localized-plugin==1.2.0
-mkdocs-material==9.1.6
+mkdocs-gen-files==0.4.0
+mkdocs-htmlproofer-plugin==0.11.0
+mkdocs-material==9.1.5
 mkdocs-material-extensions==1.1.1
-mkdocs-multirepo-plugin==0.6.1
+mkdocs-minify-plugin==0.6.4
+mkdocs-monorepo-plugin==1.0.4
 mkdocstrings==0.21.2
 mkdocstrings-python==0.9.0
 mypy-extensions==1.0.0
-nodeenv==1.7.0
-packaging==23.1
+packaging==23.0
 pathspec==0.11.1
 pexpect==4.8.0
 pillow==9.5.0
+pipdeptree==2.7.0
 platformdirs==3.2.0
 pluggy==1.0.0
-pre-commit==3.2.2
 ptyprocess==0.7.0
-pycodestyle==2.10.0
 pycparser==2.21
-pyflakes==3.0.1
-pygments==2.15.1
-pymdown-extensions==9.11
+pygments==2.14.0
+pymdown-extensions==9.10
 pyrsistent==0.19.3
 pytest==7.3.1
 pytest-mock==3.10.0
 pytest-plus==0.4.0
 pytest-testinfra==7.0.0
 pytest-xdist==3.2.1
 python-dateutil==2.8.2
 python-slugify==8.0.1
-pytz==2023.3
 pyyaml==6.0
 pyyaml-env-tag==0.1
 regex==2023.3.23
 requests==2.28.2
 resolvelib==0.8.1
 rich==13.3.4
 ruamel-yaml==0.17.21
 ruamel-yaml-clib==0.2.7
 six==1.16.0
-smmap==5.0.0
+soupsieve==2.4
 subprocess-tee==0.4.1
 text-unidecode==1.3
 tinycss2==1.2.1
 tomli==2.0.1
 typing-extensions==4.5.0
-typing-inspect==0.8.0
 urllib3==1.26.15
-virtualenv==20.21.0
 watchdog==3.0.0
 wcmatch==8.4.1
 webencodings==0.5.1
 yamllint==1.30.0
 zipp==3.15.0
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `molecule-5.0.0a1/snap/snapcraft.yaml` & `molecule-5.0.1/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/__init__.py` & `molecule-5.0.1/src/molecule/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,12 +15,14 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Molecule version information."""
+try:
+    from ._version import __version__, version  # type: ignore
+except ImportError:  # pragma: no cover
+    __version__ = "0.1.dev1"
+    version = __version__
 
-
-from importlib.metadata import version
-
-__version__ = version("molecule")
+__all__ = ("__version__", "version")
```

### Comparing `molecule-5.0.0a1/src/molecule/__main__.py` & `molecule-5.0.1/src/molecule/__main__.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/api.py` & `molecule-5.0.1/src/molecule/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,15 @@
     foo.boo
     """
 
     def __getitem__(self, i):
         """Implement indexing."""
         if isinstance(i, int):
             return super().__getitem__(i)
-        else:
-            return self.__dict__[i]
+        return self.__dict__[i]
 
     def get(self, key, default):
         return self.__dict__.get(key, default)
 
     def append(self, item) -> None:
         self.__dict__[str(item)] = item
         super().append(item)
```

### Comparing `molecule-5.0.0a1/src/molecule/command/__init__.py` & `molecule-5.0.1/src/molecule/command/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/base.py` & `molecule-5.0.1/src/molecule/command/base.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/check.py` & `molecule-5.0.1/src/molecule/command/check.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/cleanup.py` & `molecule-5.0.1/src/molecule/command/cleanup.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/converge.py` & `molecule-5.0.1/src/molecule/command/converge.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/create.py` & `molecule-5.0.1/src/molecule/command/create.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/dependency.py` & `molecule-5.0.1/src/molecule/command/dependency.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/destroy.py` & `molecule-5.0.1/src/molecule/command/destroy.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/drivers.py` & `molecule-5.0.1/src/molecule/command/drivers.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/idempotence.py` & `molecule-5.0.1/src/molecule/command/idempotence.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/init/base.py` & `molecule-5.0.1/src/molecule/command/init/base.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/init/init.py` & `molecule-5.0.1/src/molecule/command/init/init.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/init/role.py` & `molecule-5.0.1/src/molecule/command/init/role.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/init/scenario.py` & `molecule-5.0.1/src/molecule/command/init/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     # if role name was not mentioned we assume that current directory is the
     # one hosting the role and determining the role name.
     if not value:
         value = os.path.basename(os.getcwd())
 
     role_directory = os.path.join(os.pardir, value)
     if not os.path.exists(role_directory):
-        msg = f"The role '{value}' not found. " "Please choose the proper role name."
+        msg = f"The role '{value}' not found. Please choose the proper role name."
         util.sysexit_with_message(msg)
     return value
 
 
 def _default_scenario_exists(ctx, param, value: str):  # pragma: no cover
     if value == command_base.MOLECULE_DEFAULT_SCENARIO_NAME:
         return value
```

### Comparing `molecule-5.0.0a1/src/molecule/command/list.py` & `molecule-5.0.1/src/molecule/command/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     statuses = []
     s = scenarios.Scenarios(base.get_configs(args, command_args), scenario_name)
     for scenario in s:
         statuses.extend(base.execute_subcommand(scenario.config, subcommand))
 
     headers = [text.title(name) for name in Status._fields]
-    if format == "simple" or format == "plain":
+    if format in ["simple", "plain"]:
         table_format = format  # "simple"
 
         if format == "plain":
             headers = []
             table_format = format
         _print_tabulate_data(headers, statuses, table_format)
     else:
```

### Comparing `molecule-5.0.0a1/src/molecule/command/login.py` & `molecule-5.0.1/src/molecule/command/login.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,22 +87,24 @@
                     f"Available hosts:\n{host_list}"
                 )
                 util.sysexit_with_message(msg)
 
         return match[0]
 
     def _get_login(self, hostname):  # pragma: no cover
+        # ruff: noqa: S605,S607
         lines, columns = os.popen("stty size", "r").read().split()
         login_options = self._config.driver.login_options(hostname)
         login_options["columns"] = columns
         login_options["lines"] = lines
         login_cmd = self._config.driver.login_cmd_template.format(**login_options)
 
         cmd = shlex.split(f"/usr/bin/env {login_cmd}")
-        subprocess.run(cmd)
+        # ruff: noqa: S603
+        subprocess.run(cmd, check=False)
 
 
 @base.click_command_ex()
 @click.pass_context
 @click.option("--host", "-h", help="Host to access.")
 @click.option(
     "--scenario-name",
```

### Comparing `molecule-5.0.0a1/src/molecule/command/matrix.py` & `molecule-5.0.1/src/molecule/command/matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/prepare.py` & `molecule-5.0.1/src/molecule/command/prepare.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/reset.py` & `molecule-5.0.1/src/molecule/command/reset.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/side_effect.py` & `molecule-5.0.1/src/molecule/command/side_effect.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/syntax.py` & `molecule-5.0.1/src/molecule/command/syntax.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/command/test.py` & `molecule-5.0.1/src/molecule/command/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     default=False,
     help="Test all scenarios. Default is False.",
 )
 @click.option(
     "--destroy",
     type=click.Choice(["always", "never"]),
     default="always",
-    help=("The destroy strategy used at the conclusion of a " "Molecule run (always)."),
+    help=("The destroy strategy used at the conclusion of a Molecule run (always)."),
 )
 @click.option(
     "--parallel/--no-parallel",
     default=MOLECULE_PARALLEL,
     help="Enable or disable parallel mode. Default is disabled.",
 )
 @click.argument("ansible_args", nargs=-1, type=click.UNPROCESSED)
```

### Comparing `molecule-5.0.0a1/src/molecule/command/verify.py` & `molecule-5.0.1/src/molecule/command/verify.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/config.py` & `molecule-5.0.1/src/molecule/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,16 +122,15 @@
 
     @property
     def ansible_collections_path(self):
         """Return collection path variable for current version of Ansible."""
         # https://github.com/ansible/ansible/pull/70007
         if self.runtime.version >= Version("2.10.0.dev0"):
             return "ANSIBLE_COLLECTIONS_PATH"
-        else:
-            return "ANSIBLE_COLLECTIONS_PATHS"
+        return "ANSIBLE_COLLECTIONS_PATHS"
 
     @property
     def config_file(self):
         return os.path.join(self.scenario.ephemeral_directory, MOLECULE_FILE)
 
     @property
     def is_parallel(self):
@@ -170,16 +169,17 @@
         return molecule_directory(self.project_directory)
 
     @cached_property
     def dependency(self):
         dependency_name = self.config["dependency"]["name"]
         if dependency_name == "galaxy":
             return ansible_galaxy.AnsibleGalaxy(self)
-        elif dependency_name == "shell":
+        if dependency_name == "shell":
             return shell.Shell(self)
+        return None
 
     @cached_property
     def driver(self):
         driver_name = self._get_driver_name()
         driver = None
 
         driver = api.drivers(config=self)[driver_name]
@@ -232,18 +232,20 @@
         # look at state file for molecule.yml date modified and warn if they do not match
         if self.molecule_file and os.path.isfile(self.molecule_file):
             modTime = os.path.getmtime(self.molecule_file)
             if myState.molecule_yml_date_modified is None:
                 myState.change_state("molecule_yml_date_modified", modTime)
             elif myState.molecule_yml_date_modified != modTime:
                 LOG.warning(
-                    f"The scenario config file ('{self.molecule_file}') has been modified since the scenario was created. "
-                    + "If recent changes are important, reset the scenario with 'molecule destroy' to clean up created items or "
-                    + "'molecule reset' to clear current configuration.",
+                    "The scenario config file ('%s') has been modified since the scenario was created. "
+                    "If recent changes are important, reset the scenario with 'molecule destroy' to clean up created items or "
+                    "'molecule reset' to clear current configuration.",
+                    self.molecule_file,
                 )
+
         return state.State(self)
 
     @cached_property
     def verifier(self):
         return api.verifiers(self).get(self.config["verifier"]["name"], None)
 
     def _get_driver_name(self):
```

### Comparing `molecule-5.0.0a1/src/molecule/console.py` & `molecule-5.0.1/src/molecule/console.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/.yamllint` & `molecule-5.0.1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-5.0.1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py` & `molecule-5.0.1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/data/driver.json` & `molecule-5.0.1/src/molecule/data/driver.json`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/data/molecule.json` & `molecule-5.0.1/src/molecule/data/molecule.json`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/__init__.py` & `molecule-5.0.1/src/molecule/dependency/ansible_galaxy/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/base.py` & `molecule-5.0.1/src/molecule/dependency/ansible_galaxy/base.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/collections.py` & `molecule-5.0.1/src/molecule/dependency/ansible_galaxy/collections.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/roles.py` & `molecule-5.0.1/src/molecule/dependency/ansible_galaxy/roles.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/dependency/base.py` & `molecule-5.0.1/src/molecule/dependency/base.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/dependency/shell.py` & `molecule-5.0.1/src/molecule/dependency/shell.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/driver/base.py` & `molecule-5.0.1/src/molecule/driver/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Base Driver Module."""
 
 import inspect
 import os
 from abc import ABCMeta, abstractmethod
+from importlib.metadata import version
 
 import molecule
 from molecule.status import Status
 
 
 class Driver:
     """Driver Class."""
@@ -37,15 +38,15 @@
 
         :param config: An instance of a Molecule config.
         :returns: None
         """
         self._config = config
         self._path = os.path.abspath(os.path.dirname(inspect.getfile(self.__class__)))
         self.module = self.__module__.split(".", maxsplit=1)[0]
-        self.version = molecule.version(self.module)
+        self.version = version(self.module)
 
     @property
     @abstractmethod
     def name(self) -> str:  # pragma: no cover
         """Name of the driver and returns a string.
 
         :returns: str
@@ -266,14 +267,17 @@
             "playbooks",
             step + ".yml",
         )
         if os.path.isfile(p):
             return p
         return None
 
+    def schema_file(self):
+        return None
+
     def modules_dir(self):
         """Return path to ansible modules included with driver."""
         p = os.path.join(self._path, "modules")
         if os.path.isdir(p):
             return p
         return None
```

### Comparing `molecule-5.0.0a1/src/molecule/driver/delegated.py` & `molecule-5.0.1/src/molecule/driver/delegated.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Delegated Driver Module."""
 
 import logging
+import os
 
 from molecule import util
 from molecule.api import Driver
+from molecule.data import __file__ as data_module
 
 LOG = logging.getLogger(__name__)
 
 
 class Delegated(Driver):
     r"""The class responsible for managing delegated instances.
 
@@ -249,7 +251,10 @@
         return next(
             item for item in instance_config_dict if item["instance"] == instance_name
         )
 
     def sanity_checks(self):
         # Note(decentral1se): Cannot implement driver specifics are unknown
         pass
+
+    def schema_file(self):
+        return os.path.join(os.path.dirname(data_module), "driver.json")
```

### Comparing `molecule-5.0.0a1/src/molecule/interpolation.py` & `molecule-5.0.1/src/molecule/interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.templater = templater
         self.mapping = mapping
 
     def interpolate(self, string: str, keep_string=None) -> str:
         try:
             return self.templater(string).substitute(self.mapping, keep_string)  # type: ignore
         except ValueError as e:
-            raise InvalidInterpolation(string, e)
+            raise InvalidInterpolation(string, e) from e
 
 
 class TemplateWithDefaults(string.Template):
     """TemplateWithDefaults Class."""
 
     idpattern = r"[_a-z][_a-z0-9]*(?::?-[^}]+)?"
```

### Comparing `molecule-5.0.0a1/src/molecule/logger.py` & `molecule-5.0.1/src/molecule/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
 @cache
 def get_section_loggers() -> Iterable[Callable]:
     """Return a list of section wrappers to be added."""
     default_section_loggers = [section_logger]
     if not os.getenv("CI"):
         return default_section_loggers
-    elif os.getenv("GITHUB_ACTIONS"):
+    if os.getenv("GITHUB_ACTIONS"):
         return [github_actions_groups, *default_section_loggers]
-    elif os.getenv("GITLAB_CI"):
+    if os.getenv("GITLAB_CI"):
         return [gitlab_ci_sections, *default_section_loggers]
-    elif os.getenv("TRAVIS"):
+    if os.getenv("TRAVIS"):
         return [travis_ci_folds, *default_section_loggers]
     # CI is set but no extra section_loggers apply.
     return default_section_loggers
```

### Comparing `molecule-5.0.0a1/src/molecule/model/schema_v3.py` & `molecule-5.0.1/src/molecule/model/schema_v3.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,50 +15,46 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Schema v3 Validation Module."""
 
-import importlib.resources as pkg_resources
 import json
 import logging
 import os
 
 from jsonschema import validate as jsonschema_validate
 from jsonschema.exceptions import ValidationError
 
+from molecule import api
 from molecule.data import __file__ as data_module
 
 LOG = logging.getLogger(__name__)
 
 
 def validate(c):
     """Perform schema validation."""
     result = []
     schemas = []
 
     schema_files = [os.path.dirname(data_module) + "/molecule.json"]
     driver_name = c["driver"]["name"]
+
     driver_schema_file = None
+    if driver_name in api.drivers():
+        driver_schema_file = api.drivers()[driver_name].schema_file()
 
-    if driver_name == "delegated":
-        driver_schema_file = os.path.dirname(data_module) + "/driver.json"
+    if driver_schema_file is None:
+        msg = f"Driver {driver_name} does not provide a schema."
+        LOG.warning(msg)
+    elif not os.path.exists(driver_schema_file):
+        msg = f"Schema {driver_schema_file} for driver {driver_name} not found."
+        LOG.warning(msg)
     else:
-        try:
-            with pkg_resources.path(f"molecule_{driver_name}", "driver.json") as p:
-                driver_schema_file = p.as_posix()
-        except FileNotFoundError:
-            msg = f"No schema found in {driver_name} driver."
-            LOG.warning(msg)
-        except ModuleNotFoundError:
-            msg = f"{driver_name} driver is not installed."
-            LOG.warning(msg)
-
-    if driver_schema_file:
         schema_files.append(driver_schema_file)
 
     for schema_file in schema_files:
         with open(schema_file, encoding="utf-8") as f:
             schema = json.load(f)
         schemas.append(schema)
```

### Comparing `molecule-5.0.0a1/src/molecule/platforms.py` & `molecule-5.0.1/src/molecule/platforms.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/provisioner/ansible.py` & `molecule-5.0.1/src/molecule/provisioner/ansible.py`

 * *Files 0% similar despite different names*

```diff
@@ -943,15 +943,15 @@
 
     def _verify_inventory(self):
         """Verify the inventory is valid and returns None.
 
         :return: None
         """
         if not self.inventory:
-            msg = "Instances missing from the 'platform' " "section of molecule.yml."
+            msg = "Instances missing from the 'platform' section of molecule.yml."
             util.sysexit_with_message(msg)
 
     def _get_config_template(self):
         """Return a config template string.
 
         :return: str
         """
```

### Comparing `molecule-5.0.0a1/src/molecule/provisioner/ansible_playbook.py` & `molecule-5.0.1/src/molecule/provisioner/ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/provisioner/ansible_playbooks.py` & `molecule-5.0.1/src/molecule/provisioner/ansible_playbooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,34 +81,35 @@
         c = self._config.config
         driver_dict = c["provisioner"]["playbooks"].get(self._config.driver.name)
 
         playbook = c["provisioner"]["playbooks"][section]
         if driver_dict:
             try:
                 playbook = driver_dict[section]
-            except Exception:
-                pass
+            except Exception as exc:
+                LOG.exception(exc)
         if playbook is not None:
             playbook = self._config.provisioner.abs_path(playbook)
             playbook = self._normalize_playbook(playbook)
 
             if os.path.exists(playbook):
                 return playbook
-            elif os.path.exists(self._get_bundled_driver_playbook(section)):
+            if os.path.exists(self._get_bundled_driver_playbook(section)):
                 return self._get_bundled_driver_playbook(section)
-            elif section not in [
+            if section not in [
                 # these playbooks can be considered optional
                 "prepare",
                 "create",
                 "destroy",
                 "cleanup",
                 "side_effect",
                 "verify",
             ]:
                 return playbook
+        return None
 
     def _get_bundled_driver_playbook(self, section):
         path = self._config.driver.get_playbook(section)
         if path:
             return path
 
         path = os.path.join(
```

### Comparing `molecule-5.0.0a1/src/molecule/provisioner/base.py` & `molecule-5.0.1/src/molecule/provisioner/base.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/scenario.py` & `molecule-5.0.1/src/molecule/scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,15 @@
     def name(self):
         return self.config.config["scenario"]["name"]
 
     @property
     def directory(self):
         if self.config.molecule_file:
             return os.path.dirname(self.config.molecule_file)
-        else:
-            return os.getcwd()
+        return os.getcwd()
 
     @property
     def ephemeral_directory(self):
         path = os.getenv("MOLECULE_EPHEMERAL_DIRECTORY", None)
         if not path:
             project_directory = os.path.basename(self.config.project_directory)
```

### Comparing `molecule-5.0.0a1/src/molecule/scenarios.py` & `molecule-5.0.1/src/molecule/scenarios.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,26 +117,24 @@
                     'action-1',
                 ],
             },
         }
 
         :returns: dict
         """
-        return dict(
-            {
-                scenario.name: {
-                    "check": scenario.check_sequence,
-                    "cleanup": scenario.cleanup_sequence,
-                    "converge": scenario.converge_sequence,
-                    "create": scenario.create_sequence,
-                    "dependency": scenario.dependency_sequence,
-                    "destroy": scenario.destroy_sequence,
-                    "idempotence": scenario.idempotence_sequence,
-                    "prepare": scenario.prepare_sequence,
-                    "side_effect": scenario.side_effect_sequence,
-                    "syntax": scenario.syntax_sequence,
-                    "test": scenario.test_sequence,
-                    "verify": scenario.verify_sequence,
-                }
-                for scenario in self.all
-            },
-        )
+        return {
+            scenario.name: {
+                "check": scenario.check_sequence,
+                "cleanup": scenario.cleanup_sequence,
+                "converge": scenario.converge_sequence,
+                "create": scenario.create_sequence,
+                "dependency": scenario.dependency_sequence,
+                "destroy": scenario.destroy_sequence,
+                "idempotence": scenario.idempotence_sequence,
+                "prepare": scenario.prepare_sequence,
+                "side_effect": scenario.side_effect_sequence,
+                "syntax": scenario.syntax_sequence,
+                "test": scenario.test_sequence,
+                "verify": scenario.verify_sequence,
+            }
+            for scenario in self.all
+        }
```

### Comparing `molecule-5.0.0a1/src/molecule/shell.py` & `molecule-5.0.1/src/molecule/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,20 +58,21 @@
 
     v = packaging.version.Version(molecule.__version__)
     color = "bright_yellow" if v.is_prerelease else "green"
     msg = f"molecule [{color}]{v}[/] using python [repr.number]{sys.version_info[0]}.{sys.version_info[1]}[/] \n"
 
     msg += f"    [repr.attrib_name]ansible[/][dim]:[/][repr.number]{app.runtime.version}[/]"
     for driver in drivers():
-        msg += f"\n    [repr.attrib_name]{str(driver)}[/][dim]:[/][repr.number]{driver.version}[/][dim] from {driver.module}[/]"
+        msg += f"\n    [repr.attrib_name]{str(driver)}[/][dim]:[/][repr.number]{driver.version}[/][dim] from {driver.module}"
         if driver.required_collections:
             msg += " requiring collections:"
             for name, version in driver.required_collections.items():
-                msg += f" {name}>={version}"
-    console.print(msg)
+                msg += f" [repr.attrib_name]{name}[/]>=[repr.number]{version}[/]"
+        msg += "[/]"
+    console.print(msg, highlight=False)
 
     ctx.exit()
 
 
 @click_group_ex()  # type: ignore
 @click.option(
     "--debug/--no-debug",
@@ -101,15 +102,15 @@
         f"in user home. ({LOCAL_CONFIG})."
     ),
 )
 @click.option(
     "--env-file",
     "-e",
     default=ENV_FILE,
-    help=("The file to read variables from when rendering molecule.yml. " "(.env.yml)"),
+    help=("The file to read variables from when rendering molecule.yml. (.env.yml)"),
 )
 @click.option(
     "--version",
     is_flag=True,
     callback=print_version,
     expose_value=False,
     is_eager=True,
```

### Comparing `molecule-5.0.0a1/src/molecule/state.py` & `molecule-5.0.1/src/molecule/state.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/status.py` & `molecule-5.0.1/src/molecule/status.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/conftest.py` & `molecule-5.0.1/src/molecule/test/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/functional/.ansible-lint` & `molecule-5.0.1/src/molecule/test/functional/.ansible-lint`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/functional/conftest.py` & `molecule-5.0.1/src/molecule/test/functional/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,25 +44,25 @@
 # it failed, see https://bugzilla.redhat.com/show_bug.cgi?id=1759713
 MIN_PODMAN_VERSION = "1.5.1"
 
 
 @pytest.fixture(scope="session", autouse=True)
 def require_installed_package():
     try:
-        molecule.version("molecule")
+        molecule.__version__
     except Exception as e:
         pytest.fail(f"Functional tests require molecule package to be installed: {e}")
 
 
 def _env_vars_exposed(env_vars, env=os.environ):
     """Check if environment variables are exposed and populated."""
     for env_var in env_vars:
         if env_var not in os.environ:
             return False
-        return os.environ[env_var] != ""
+        return bool(os.environ[env_var])
     return None
 
 
 @pytest.fixture()
 def with_scenario(request, scenario_to_test, driver_name, scenario_name, skip_test):
     scenario_directory = os.path.join(
         os.path.dirname(util.abs_path(__file__)),
@@ -236,15 +236,20 @@
     return shutil.which("VBoxManage")
 
 
 @cache
 def supports_docker() -> bool:
     docker = get_docker_executable()
     if docker:
-        result = subprocess.run([docker, "info"], stdout=PIPE, text=True)
+        result = subprocess.run(
+            [docker, "info"],
+            stdout=PIPE,
+            text=True,
+            check=True,
+        )  # Explicitly set check=True
         if result.returncode != 0:
             LOG.error(
                 "Error %s returned from `docker info`: %s",
                 result.returncode,
                 result.stdout,
             )
             return False
```

### Comparing `molecule-5.0.0a1/src/molecule/test/functional/test_command.py` & `molecule-5.0.1/src/molecule/test/functional/test_command.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/valid/molecule.yml` & `molecule-5.0.1/src/molecule/test/resources/schema_instance_files/valid/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml` & `molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml` & `molecule-5.0.1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py` & `molecule-5.0.1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/conftest.py` & `molecule-5.0.1/src/molecule/test/unit/command/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/init/test_role.py` & `molecule-5.0.1/src/molecule/test/unit/command/init/test_role.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/init/test_scenario.py` & `molecule-5.0.1/src/molecule/test/unit/command/init/test_scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     _instance.execute()
 
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
     assert e.value.code == 1
 
-    msg = "The directory molecule/test-scenario exists. " "Cannot create new scenario."
+    msg = "The directory molecule/test-scenario exists. Cannot create new scenario."
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_execute_with_invalid_driver(
     temp_dir,
     _instance,
     _command_args,
```

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_base.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         f"{cache_dir}/roles:"
         f"{home}/.ansible/roles:"
         f"/usr/share/ansible/roles:"
         f"/etc/ansible/roles",
     )
 
     assert runtime_collections_path.startswith(
-        f"{cache_dir}/collections:" f"{home}/.ansible/collections",
+        f"{cache_dir}/collections:{home}/.ansible/collections",
     )
 
     assert provisioner_roles_path.startswith(f"{cache_dir}/roles")
 
     assert provisioner_collections_path.startswith(f"{cache_dir}/collections")
```

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_check.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_check.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_cleanup.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_converge.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_converge.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_create.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_create.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_dependency.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_dependency.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_destroy.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_destroy.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_idempotence.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_idempotence.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_list.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_list.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_login.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_login.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_matrix.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_prepare.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_prepare.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_side_effect.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_side_effect.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_syntax.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_syntax.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_test.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_test.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/command/test_verify.py` & `molecule-5.0.1/src/molecule/test/unit/command/test_verify.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/conftest.py` & `molecule-5.0.1/src/molecule/test/unit/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import copy
-import functools
 import os
 import shutil
 from collections.abc import Generator
 from pathlib import Path
 from subprocess import CompletedProcess
 from typing import Any
 from uuid import uuid4
@@ -105,15 +104,19 @@
         _molecule_driver_section_data,
         _molecule_platforms_section_data,
         _molecule_provisioner_section_data,
         _molecule_scenario_section_data,
         _molecule_verifier_section_data,
     ]
 
-    return functools.reduce(lambda x, y: util.merge_dicts(x, y), fixtures)
+    merged_dict = {}
+    for fixture in fixtures:
+        merged_dict.update(fixture)
+
+    return merged_dict
 
 
 @pytest.fixture()
 def molecule_directory_fixture(temp_dir):
     return molecule_directory()
```

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/cookiecutter/test_molecule.py` & `molecule-5.0.1/src/molecule/test/unit/cookiecutter/test_molecule.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py` & `molecule-5.0.1/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py` & `molecule-5.0.1/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from molecule import config
 from molecule.dependency.ansible_galaxy import roles
 
 
 @pytest.fixture()
 def _patched_ansible_galaxy_has_requirements_file(mocker):
     m = mocker.patch(
-        "molecule.dependency.ansible_galaxy.roles." "Roles._has_requirements_file",
+        "molecule.dependency.ansible_galaxy.roles.Roles._has_requirements_file",
     )
     m.return_value = True
 
     return m
 
 
 @pytest.fixture()
```

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/dependency/test_shell.py` & `molecule-5.0.1/src/molecule/test/unit/dependency/test_shell.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/driver/test_delegated.py` & `molecule-5.0.1/src/molecule/test/unit/driver/test_delegated.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/model/v2/conftest.py` & `molecule-5.0.1/src/molecule/test/unit/model/v2/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_dependency_section.py` & `molecule-5.0.1/src/molecule/test/unit/model/v2/test_dependency_section.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_driver_section.py` & `molecule-5.0.1/src/molecule/test/unit/model/v2/test_driver_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
     ],
     indirect=True,
 )
 def test_driver_has_errors(_config):
     base_error_msg = "is not one of ['azure', 'ec2', 'delegated', 'docker', 'containers', 'openstack', 'podman', 'vagrant', 'digitalocean', 'gce', 'libvirt', 'lxd', 'molecule-*', 'molecule_*', 'custom-*', 'custom_*']"
 
     driver_name = str(_config["driver"]["name"])
-    if type(_config["driver"]["name"]) is str:
+    if isinstance(_config["driver"]["name"], str):
         # add single quotes for string
-        driver_name = f"'{driver_name}'"
+        driver_name = f"'{_config['driver']['name']}'"
 
     error_msg = [" ".join((driver_name, base_error_msg))]
     assert error_msg == schema_v3.validate(_config)
 
 
 @pytest.fixture()
 def _model_driver_provider_name_nullable_section_data():
```

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_platforms_section.py` & `molecule-5.0.1/src/molecule/test/unit/model/v2/test_platforms_section.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_provisioner_section.py` & `molecule-5.0.1/src/molecule/test/unit/model/v2/test_provisioner_section.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_scenario_section.py` & `molecule-5.0.1/src/molecule/test/unit/model/v2/test_scenario_section.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_schema.py` & `molecule-5.0.1/src/molecule/test/unit/model/v2/test_schema.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_verifier_section.py` & `molecule-5.0.1/src/molecule/test/unit/model/v2/test_verifier_section.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible.py` & `molecule-5.0.1/src/molecule/test/unit/provisioner/test_ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible_playbook.py` & `molecule-5.0.1/src/molecule/test/unit/provisioner/test_ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible_playbooks.py` & `molecule-5.0.1/src/molecule/test/unit/provisioner/test_ansible_playbooks.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_api.py` & `molecule-5.0.1/src/molecule/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_config.py` & `molecule-5.0.1/src/molecule/test/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_interpolation.py` & `molecule-5.0.1/src/molecule/test/unit/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_logger.py` & `molecule-5.0.1/src/molecule/test/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_platforms.py` & `molecule-5.0.1/src/molecule/test/unit/test_platforms.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_scenario.py` & `molecule-5.0.1/src/molecule/test/unit/test_scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_scenarios.py` & `molecule-5.0.1/src/molecule/test/unit/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_scenarios_ordered.py` & `molecule-5.0.1/src/molecule/test/unit/test_scenarios_ordered.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_shell.py` & `molecule-5.0.1/src/molecule/test/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_state.py` & `molecule-5.0.1/src/molecule/test/unit/test_state.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_status.py` & `molecule-5.0.1/src/molecule/test/unit/test_status.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_text.py` & `molecule-5.0.1/src/molecule/test/unit/test_text.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/test_util.py` & `molecule-5.0.1/src/molecule/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/verifier/test_ansible.py` & `molecule-5.0.1/src/molecule/test/unit/verifier/test_ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/test/unit/verifier/test_testinfra.py` & `molecule-5.0.1/src/molecule/test/unit/verifier/test_testinfra.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/text.py` & `molecule-5.0.1/src/molecule/text.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/util.py` & `molecule-5.0.1/src/molecule/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     """
     args = []
     if cmd.__class__.__name__ == "Command":
         raise RuntimeError(
             "Molecule 3.2.0 dropped use of sh library, update plugin code to use new API. "
             "See https://github.com/ansible-community/molecule/issues/2678",
         )
-    elif cmd.__class__.__name__ == "BakedCommand":
+    if cmd.__class__.__name__ == "BakedCommand":
         env = dict(cmd.env, **env) if cmd.env and env else cmd.env or env
         args = cmd.cmd
     else:
         args = cmd
 
     if debug:
         print_environment_vars(env)
@@ -171,15 +171,15 @@
                 filename = os.path.join(root, basename)
 
                 yield filename
 
 
 def render_template(template, **kwargs):
     """Render a jinaj2 template."""
-    t = jinja2.Environment()
+    t = jinja2.Environment(autoescape=True)
     t = t.from_string(template)
 
     return t.render(kwargs)
 
 
 def write_file(filename: str, content: str, header: Optional[str] = None) -> None:
     """Write a file with the given filename and content and returns None.
@@ -375,15 +375,15 @@
 
     normalized_value = value
     if isinstance(value, (str, bytes)):
         normalized_value = str(value).lower().strip()
 
     if normalized_value in BOOLEANS_TRUE:
         return True
-    elif normalized_value in BOOLEANS_FALSE or not strict:
+    if normalized_value in BOOLEANS_FALSE or not strict:
         return False
 
     raise TypeError(
         f"The value '{value!s}' is not a valid boolean.  Valid booleans include: {', '.join(repr(i) for i in BOOLEANS)!s}",
     )
```

### Comparing `molecule-5.0.0a1/src/molecule/verifier/ansible.py` & `molecule-5.0.1/src/molecule/verifier/ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/verifier/base.py` & `molecule-5.0.1/src/molecule/verifier/base.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/src/molecule/verifier/testinfra.py` & `molecule-5.0.1/src/molecule/verifier/testinfra.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,25 +199,24 @@
                         os.path.join(self._config.scenario.directory, arg),
                         "test_*.py",
                         followlinks=True,
                     ),
                 )
                 tests.extend(args_tests)
             return sorted(tests)
-        else:
-            return sorted(
-                list(
-                    util.os_walk(
-                        self.directory,
-                        "test_*.py",
-                        followlinks=True,
-                    ),
-                )
-                + self.additional_files_or_dirs,
+        return sorted(
+            list(
+                util.os_walk(
+                    self.directory,
+                    "test_*.py",
+                    followlinks=True,
+                ),
             )
+            + self.additional_files_or_dirs,
+        )
 
     def schema(self):
         return {
             "verifier": {
                 "type": "dict",
                 "schema": {"name": {"type": "string", "allowed": ["testinfra"]}},
             },
```

### Comparing `molecule-5.0.0a1/src/molecule.egg-info/PKG-INFO` & `molecule-5.0.1/src/molecule.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 5.0.0a1
+Version: 5.0.1
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
@@ -12,30 +12,31 @@
 Keywords: ansible,roles,testing,molecule
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: lint
 Provides-Extra: test
+Provides-Extra: lock
 License-File: LICENSE
 
 # About Ansible Molecule
 
 [![PyPI Package](https://img.shields.io/pypi/v/molecule)](https://pypi.org/project/molecule/)
 [![Documentation Status](https://readthedocs.org/projects/molecule/badge/?version=latest)](https://molecule.readthedocs.io/en/latest/)
 [![image](https://github.com/ansible-community/molecule/workflows/tox/badge.svg)](https://github.com/ansible-community/molecule/actions)
```

### Comparing `molecule-5.0.0a1/src/molecule.egg-info/SOURCES.txt` & `molecule-5.0.1/src/molecule.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,52 +14,60 @@
 README.md
 bindep.txt
 codecov.yml
 conftest.py
 mkdocs.yml
 mypy.ini
 pyproject.toml
-requirements.txt
 runtime.txt
 tox.ini
 .config/molecule.spec
+.config/requirements-docs.txt
+.config/requirements-lock.txt
+.config/requirements-test.txt
+.config/requirements.in
+.config/requirements.txt
 .config/molecule/config.yml
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/dependabot.yml
 .github/patchback.yml
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/security_bug_report.md
 .github/workflows/ack.yml
 .github/workflows/push.yml
+.github/workflows/redirects.yml
 .github/workflows/release.yml
 .github/workflows/tox.yml
 .vscode/extensions.json
 .vscode/settings.json
 docs/ci.md
 docs/configuration.md
 docs/contributing.md
 docs/examples.md
 docs/faq.md
 docs/getting-started.md
+docs/google04e29a42ae6e6cbc.html
 docs/index.md
 docs/installation.md
+docs/redirects.yml
 docs/usage.md
 docs/_static/images/favicon.ico
 docs/_static/images/logo.png
 docs/_static/images/logo_big.png
 docs/images/favicon.ico
 docs/images/logo.png
 docs/images/logo.svg
 playbooks/snap-pre-run.yaml
 snap/snapcraft.yaml
 src/molecule/__init__.py
 src/molecule/__main__.py
+src/molecule/_version.py
 src/molecule/api.py
 src/molecule/app.py
 src/molecule/config.py
 src/molecule/console.py
 src/molecule/constants.py
 src/molecule/interpolation.py
 src/molecule/logger.py
```

### Comparing `molecule-5.0.0a1/tools/test-setup.sh` & `molecule-5.0.1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a1/tox.ini` & `molecule-5.0.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -35,32 +35,27 @@
     ANSIBLE_CONFIG={toxinidir}/.ansible.cfg
     ANSIBLE_DISPLAY_FAILED_STDERR=1
     ANSIBLE_NOCOWS=1
     ANSIBLE_VERBOSITY=1
     COVERAGE_FILE={env:COVERAGE_FILE:{toxworkdir}/.coverage.{envname}}
     COVERAGE_PROCESS_START={toxinidir}/pyproject.toml
     MOLECULE_NO_LOG=0
-    PIP_CONSTRAINT = {toxinidir}/requirements.txt
+    PIP_CONSTRAINT = {toxinidir}/.config/requirements.txt
     devel: PIP_CONSTRAINT=/dev/null
     PIP_DISABLE_PIP_VERSION_CHECK=1
     PYTHONDONTWRITEBYTECODE=1
     PYTHONUNBUFFERED=1
     # Temporare remove "-n auto" as it seems to break coverage on this project.
     _EXTRAS=-l
 deps =
-    # py,py{39,310,311,312}: --editable .[docker,lint,podman,test,windows]
     devel: git+https://github.com/ansible/ansible#egg=ansible-core
     # pytest-molecule not used but we want to check that it does not conflict
     devel: git+https://github.com/ansible-community/pytest-molecule#egg=pytest-molecule
 extras =
-    docker
-    lint
-    podman
     test
-    windows
 commands =
     ansibledevel: ansible-galaxy install git+https://github.com/ansible-collections/community.general.git
     # failsafe as pip may install incompatible dependencies
     pip check
     # failsafe for preventing changes that may break pytest collection
     sh -c "PYTEST_ADDOPTS= python -m pytest -p no:cov --collect-only >>/dev/null"
     sh -c "rm -f .tox/.coverage.*"
@@ -94,14 +89,18 @@
 description = Bump all test dependencies
 skip_install = true
 deps = {[testenv:lint]deps}
 setenv = {[testenv:lint]setenv}
 commands =
   # manual hook calls the optional pip-compile-upgrade hook after pip-compile
   {[testenv:lint]commands} --hook-stage manual pip-compile
+  # Update pre-commit hooks
+  -pre-commit autoupdate
+  # We fail if files are modified at the end
+  git diff --exit-code
 
 [testenv:docs]
 description = Build documentation
 passenv = *
 usedevelop = true
 commands =
     mkdocs build --strict
```

