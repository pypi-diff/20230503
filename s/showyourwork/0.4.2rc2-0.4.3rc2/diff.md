# Comparing `tmp/showyourwork-0.4.2rc2.tar.gz` & `tmp/showyourwork-0.4.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showyourwork-0.4.2rc2.tar", last modified: Tue Jan 31 11:59:09 2023, max compression
+gzip compressed data, was "showyourwork-0.4.3rc2.tar", last modified: Wed May  3 12:48:03 2023, max compression
```

## Comparing `showyourwork-0.4.2rc2.tar` & `showyourwork-0.4.3rc2.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.616157 showyourwork-0.4.2rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-01-31 11:59:09.616157 showyourwork-0.4.2rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.576158 showyourwork-0.4.2rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.580158 showyourwork-0.4.2rc2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/actions_tab.png
--rw-r--r--   0 runner    (1001) docker     (123)   204092 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/article-abstract.png
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/badges.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.580158 showyourwork-0.4.2rc2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)   425530 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/default_ms.png
--rw-r--r--   0 runner    (1001) docker     (123)   540973 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/default_ms_with_figure.png
--rw-r--r--   0 runner    (1001) docker     (123)    43618 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   427880 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)   147093 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/workflow_permissions.png
--rw-r--r--   0 runner    (1001) docker     (123)    57574 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/_static/zenodo_dois.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.580158 showyourwork-0.4.2rc2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/api/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/attribution.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22625 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/faqs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/hacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/integration_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/latex.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/layout.rst
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/migrating.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/overleaf.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/projects.json
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/projects.rst.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/quickbuild.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/reproducibility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/snakefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/docs/zenodo.rst
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 11:59:09.616157 showyourwork-0.4.2rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.584158 showyourwork-0.4.2rc2/showyourwork/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-31 11:59:09.000000 showyourwork-0.4.2rc2/showyourwork/_showyourwork_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.588158 showyourwork-0.4.2rc2/showyourwork/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.588158 showyourwork-0.4.2rc2/showyourwork/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/commands/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/commands/run_snakemake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/commands/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/commands/tarball.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/commands/zenodo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.588158 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.592157 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.552158 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.592157 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build-pull-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/process-pull-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.592157 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/showyourwork.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.556158 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.592157 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/data/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.596157 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.596157 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/static/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.596157 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    37916 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aasjournal.bst
--rw-r--r--   0 runner    (1001) docker     (123)   238984 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aastex631.cls
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/bib.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.596157 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/figures/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/figures/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/ms.tex
--rw-r--r--   0 runner    (1001) docker     (123)    27604 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/orcid-ID.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.600157 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/output/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/showyourwork.sty
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/zenodo.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.600157 showyourwork-0.4.2rc2/showyourwork/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/exceptions/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/exceptions/latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/exceptions/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/exceptions/overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/exceptions/zenodo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/gitapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/subproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/tex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/userrules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.600157 showyourwork-0.4.2rc2/showyourwork/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/build.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.600157 showyourwork-0.4.2rc2/showyourwork/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/envs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/prep.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.600157 showyourwork-0.4.2rc2/showyourwork/workflow/report/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/report/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/report/workflow.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.560158 showyourwork-0.4.2rc2/showyourwork/workflow/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.600157 showyourwork-0.4.2rc2/showyourwork/workflow/resources/img/
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/img/article-thumb.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.604157 showyourwork-0.4.2rc2/showyourwork/workflow/resources/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/styles/build.tex
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/styles/preprocess.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.604157 showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/
--rw-r--r--   0 runner    (1001) docker     (123)   149938 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/lineno.sty
--rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/listofitems.tex
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/showyourwork-logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   689534 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/showyourwork-stamp.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/showyourwork.otf
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/xstring.sty
--rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/xstring.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.608157 showyourwork-0.4.2rc2/showyourwork/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/rules/arxiv.smk
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/rules/compile.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/rules/conda.smk
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/rules/dag.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/rules/figure.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/rules/preprocess.smk
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/rules/render_dag.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/rules/zenodo.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.612157 showyourwork-0.4.2rc2/showyourwork/workflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/scripts/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/scripts/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/scripts/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/scripts/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/scripts/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/workflow/scripts/render_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    38065 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/showyourwork/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.584158 showyourwork-0.4.2rc2/showyourwork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-01-31 11:59:09.000000 showyourwork-0.4.2rc2/showyourwork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-01-31 11:59:09.000000 showyourwork-0.4.2rc2/showyourwork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 11:59:09.000000 showyourwork-0.4.2rc2/showyourwork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-31 11:59:09.000000 showyourwork-0.4.2rc2/showyourwork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 11:59:09.000000 showyourwork-0.4.2rc2/showyourwork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-31 11:59:09.000000 showyourwork-0.4.2rc2/showyourwork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-31 11:59:09.000000 showyourwork-0.4.2rc2/showyourwork.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.564158 showyourwork-0.4.2rc2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.616157 showyourwork-0.4.2rc2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.616157 showyourwork-0.4.2rc2/tests/integration/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15997 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/helpers/temp_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.616157 showyourwork-0.4.2rc2/tests/integration/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/sandbox/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_cache_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_duplicate_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_letter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_missing_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_space_in_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/integration/test_zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 11:59:09.616157 showyourwork-0.4.2rc2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-31 11:58:59.000000 showyourwork-0.4.2rc2/tests/unit/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.571947 showyourwork-0.4.3rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.571947 showyourwork-0.4.3rc2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/actions_tab.png
+-rw-r--r--   0 runner    (1001) docker     (123)   204092 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/article-abstract.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/badges.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.571947 showyourwork-0.4.3rc2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)   425530 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/default_ms.png
+-rw-r--r--   0 runner    (1001) docker     (123)   540973 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/default_ms_with_figure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43618 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   427880 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)   147093 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/workflow_permissions.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57574 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/_static/zenodo_dois.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.571947 showyourwork-0.4.3rc2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/api/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/attribution.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24716 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/contributorguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25817 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/faqs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/hacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/integration_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/latex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/layout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/migrating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/overleaf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/projects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/projects.rst.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/quickbuild.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/reproducibility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/snakefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/docs/zenodo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork/_showyourwork_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/run_snakemake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/tarball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/commands/zenodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.563947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build-pull-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/process-pull-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/showyourwork.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.563947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    37916 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aasjournal.bst
+-rw-r--r--   0 runner    (1001) docker     (123)   238984 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aastex631.cls
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/bib.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/figures/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/ms.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    27604 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/orcid-ID.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/showyourwork.sty
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/zenodo.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/exceptions/zenodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/gitapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21277 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/userrules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/build.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.579947 showyourwork-0.4.3rc2/showyourwork/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/envs/render_dag.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/envs/tectonic.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/prep.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/report/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/report/workflow.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.567947 showyourwork-0.4.3rc2/showyourwork/workflow/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/resources/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/img/article-thumb.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/build.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/preprocess.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/
+-rw-r--r--   0 runner    (1001) docker     (123)   149938 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/lineno.sty
+-rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/listofitems.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork-logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   689534 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork-stamp.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork.otf
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/xstring.sty
+-rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/xstring.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/arxiv.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/common.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/compile.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/dag.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/figure.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/preprocess.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/render_dag.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/rules/zenodo.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.583947 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/compile_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/workflow/scripts/render_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38229 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/showyourwork/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.575947 showyourwork-0.4.3rc2/showyourwork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 12:48:03.000000 showyourwork-0.4.3rc2/showyourwork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.567947 showyourwork-0.4.3rc2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/tests/integration/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/helpers/temp_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/tests/integration/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/sandbox/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_cache_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_duplicate_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_letter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_missing_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_space_in_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/integration/test_zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:48:03.587947 showyourwork-0.4.3rc2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-03 12:47:50.000000 showyourwork-0.4.3rc2/tests/unit/test_overleaf_regex.py
```

### Comparing `showyourwork-0.4.2rc2/CITATION.cff` & `showyourwork-0.4.3rc2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/HISTORY.rst` & `showyourwork-0.4.3rc2/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 - For extended discussions about the above points, please see
   `this issue <https://github.com/showyourwork/showyourwork/issues/214>`__
   and the comments in
   `this PR <https://github.com/showyourwork/showyourwork/pull/217>`__ and
   `this PR <https://github.com/showyourwork/showyourwork/pull/221>`__.
 - ``showyourwork`` no longer has explicit non-python dependencies; packages
   like ``tectonic`` are specified within ``conda`` environments to specific rules,
-  so non-python dependency management is relagated to ``snakemake``.
+  so non-python dependency management is relegated to ``snakemake``.
 - Now enforcing strict channel provenance in ``environment.yml`` files.
 - Upgraded the pinned version of ``Snakemake`` to ``7.15.2``, which fixes
   several bugs and adds new features
   (such as `this one <https://github.com/showyourwork/showyourwork/issues/199>`__).
 - Removes ``showyourwork`` logo and abstract margin icon in favor of a
   ``showyourwork`` stamp in the upper right hand corner of the first page
   of the article. This approach is class-independent and fixes several issues
```

### Comparing `showyourwork-0.4.2rc2/LICENSE` & `showyourwork-0.4.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/PKG-INFO` & `showyourwork-0.4.3rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showyourwork
-Version: 0.4.2rc2
+Version: 0.4.3rc2
 Summary: A workflow for open-source scientific articles
 Home-page: https://github.com/showyourwork/showyourwork
 Author: Rodrigo Luger
 Author-email: rodluger@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: showyourwork Version: 0.4.2rc2 Summary: A workflow
+Metadata-Version: 2.1 Name: showyourwork Version: 0.4.3rc2 Summary: A workflow
 for open-source scientific articles Home-page: https://github.com/showyourwork/
 showyourwork Author: Rodrigo Luger Author-email: rodluger@gmail.com License:
 MIT Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
 Extra: tests License-File: LICENSE
                                 [showyourwork]
   [unit_tests] [local_integration_tests] [remote_integration_tests] [tests]
                            [sample_projects] [pypi]
```

### Comparing `showyourwork-0.4.2rc2/README.md` & `showyourwork-0.4.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/.gitignore` & `showyourwork-0.4.3rc2/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/Makefile` & `showyourwork-0.4.3rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/actions_tab.png` & `showyourwork-0.4.3rc2/docs/_static/actions_tab.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/article-abstract.png` & `showyourwork-0.4.3rc2/docs/_static/article-abstract.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/badges.png` & `showyourwork-0.4.3rc2/docs/_static/badges.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/css/custom.css` & `showyourwork-0.4.3rc2/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/default_ms.png` & `showyourwork-0.4.3rc2/docs/_static/default_ms.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/default_ms_with_figure.png` & `showyourwork-0.4.3rc2/docs/_static/default_ms_with_figure.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/logo.png` & `showyourwork-0.4.3rc2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/overview.png` & `showyourwork-0.4.3rc2/docs/_static/overview.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/workflow_permissions.png` & `showyourwork-0.4.3rc2/docs/_static/workflow_permissions.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/_static/zenodo_dois.png` & `showyourwork-0.4.3rc2/docs/_static/zenodo_dois.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/api.rst` & `showyourwork-0.4.3rc2/docs/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Developer API
 =============
 
 Welcome to the guts of |showyourwork|. The backend is fairly complicated given
-that ``showyourwork`` is not just a Python package: it is simultanteously a
+that ``showyourwork`` is not just a Python package: it is simultaneously a
 wrapper around Snakemake *and* a child process of Snakemake, as well as a command-line
 tool, a cookiecutter template, a GitHub Action, and a conda environment manager.
 The code is wrapped up into a pip-installable Python package, but users should
 never have to actually import ``showyourwork`` into their scripts. Users should
 only ever interact with the code via the command line interface, which spawns
 child processes that themselves import ``showyourwork``.
```

### Comparing `showyourwork-0.4.2rc2/docs/attribution.rst` & `showyourwork-0.4.3rc2/docs/attribution.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/cli.rst` & `showyourwork-0.4.3rc2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/conf.py` & `showyourwork-0.4.3rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/config.rst` & `showyourwork-0.4.3rc2/docs/config.rst`

 * *Files 6% similar despite different names*

```diff
@@ -437,14 +437,115 @@
 
 .. code-block:: yaml
 
   dependencies:
     src/tex/ms.tex:
         - src/tex/stylesheet.tex
 
+.. _config.margin_icons:
+
+``margin_icons``
+^^^^^^^^^^^^^^^^
+
+**Type:** ``mapping``
+
+**Description:** Define the color of the margin icons.
+
+**Required:** no
+
+**Example:**
+
+.. code-block:: yaml
+
+    margin_icons:
+        custom:
+            dataset: "0.5,0.2,0.6"
+
+.. _config.margin_icons.colors:
+
+``margin_icons.colors``
+^^^^^^^^^^^^^^^^^^^^^^^
+
+**Type:** ``mapping``
+
+**Description:** Allows custom colors to be set for the margin icons.
+
+**Required:** no
+
+.. _config.margin_icons.colors.cache:
+
+``margin_icons.colors.cache``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+**Type:** ``str``
+
+**Description:** A string describing the desired rgb values for colour the Zenodo cache margin icon.
+
+**Required:** no
+
+.. _config.margin_icons.colors.dataset:
+
+``margin_icons.colors.dataset``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+**Type:** ``str``
+
+**Description:** A string describing the desired rgb values for colour the Zenodo dataset margin icon.
+
+**Required:** no
+
+.. _config.margin_icons.colors.github:
+
+``margin_icons.colors.github``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+**Type:** ``str``
+
+**Description:** A string describing the desired rgb values for colour the github margin icon.
+
+**Required:** no
+
+.. _config.margin_icons.colors.sandbox:
+
+``margin_icons.colors.sandbox``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+**Type:** ``str``
+
+**Description:** A string describing the desired rgb values for colour the Zenodo Sandbox cache margin icon.
+
+**Required:** no
+
+.. _config.margin_icons.horizontal_offset:
+
+``margin_icons.horizontal_offset``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+**Type:** ``int``
+
+**Description:** This defines the horizontal offset to be used for all of the margin icons (this helps with positioning in two-column documents). Negative values will move the icons left and positive values move right.
+
+**Required:** no
+
+.. _config.margin_icons.monochrome:
+
+``margin_icons.monochrome``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+**Type:** ``bool``
+
+**Description:** Makes all margin_icons black, this will override any custom colors.
+
+**Required:** no
+
+.. code-block:: yaml
+
+    margin_icons:
+        monochrome: false
+
 
 .. _config.ms:
 
 ``ms_name``
 ^^^^^^^^^^^
 
 **Type:** ``str``
@@ -548,15 +649,15 @@
 
     https://www.overleaf.com/project/6262c032aae5421d6d945acf
 
 in this case, the id is ``6262c032aae5421d6d945acf``.
 
 .. warning::
 
-    Please read the :doc:`Overlaf <overleaf>` integration docs before
+    Please read the :doc:`Overleaf <overleaf>` integration docs before
     manually adding/changing this value, as you could risk losing
     changes to your local document or to your Overleaf document the
     next time you build!
 
 **Required:** no
 
 **Example:**
```

#### html2text {}

```diff
@@ -127,20 +127,48 @@
 dependencies: src/scripts/my_figure.py: - src/scripts/utils/helper_script.py
 You can also specify a dependency on a programmatically-generated file: ..
 code-block:: yaml dependencies: src/scripts/fibonacci.py: - src/data/
 fibonacci.dat provided ``data/fibonacci.dat`` is defined in a ``zenodo``
 deposit (see below) or instructions for generating it are provided in the
 ``Snakefile``. Finally, dependencies of the manuscript file are also allowed:
 .. code-block:: yaml dependencies: src/tex/ms.tex: - src/tex/stylesheet.tex ..
-_config.ms: ``ms_name`` ^^^^^^^^^^^ **Type:** ``str`` **Description:** The name
-of the main TeX manuscript (without the path or the extension). Change this if
-you'd prefer to name your manuscript something other than ``ms``. Note that you
-should still keep it in the ``src/tex`` directory. Note also that the compiled
-PDF file will have the same name (e.g., ``ms_name: article`` will compile
-``src/tex/article.tex`` and generate ``article.pdf`` in the repository root) .
+_config.margin_icons: ``margin_icons`` ^^^^^^^^^^^^^^^^ **Type:** ``mapping``
+**Description:** Define the color of the margin icons. **Required:** no
+**Example:** .. code-block:: yaml margin_icons: custom: dataset: "0.5,0.2,0.6"
+.. _config.margin_icons.colors: ``margin_icons.colors`` ^^^^^^^^^^^^^^^^^^^^^^^
+**Type:** ``mapping`` **Description:** Allows custom colors to be set for the
+margin icons. **Required:** no .. _config.margin_icons.colors.cache:
+``margin_icons.colors.cache`` ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ **Type:** ``str``
+**Description:** A string describing the desired rgb values for colour the
+Zenodo cache margin icon. **Required:** no ..
+_config.margin_icons.colors.dataset: ``margin_icons.colors.dataset``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ **Type:** ``str`` **Description:** A string
+describing the desired rgb values for colour the Zenodo dataset margin icon.
+**Required:** no .. _config.margin_icons.colors.github:
+``margin_icons.colors.github`` ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ **Type:** ``str``
+**Description:** A string describing the desired rgb values for colour the
+github margin icon. **Required:** no .. _config.margin_icons.colors.sandbox:
+``margin_icons.colors.sandbox`` ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ **Type:**
+``str`` **Description:** A string describing the desired rgb values for colour
+the Zenodo Sandbox cache margin icon. **Required:** no ..
+_config.margin_icons.horizontal_offset: ``margin_icons.horizontal_offset``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ **Type:** ``int`` **Description:** This
+defines the horizontal offset to be used for all of the margin icons (this
+helps with positioning in two-column documents). Negative values will move the
+icons left and positive values move right. **Required:** no ..
+_config.margin_icons.monochrome: ``margin_icons.monochrome``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^ **Type:** ``bool`` **Description:** Makes all
+margin_icons black, this will override any custom colors. **Required:** no ..
+code-block:: yaml margin_icons: monochrome: false .. _config.ms: ``ms_name``
+^^^^^^^^^^^ **Type:** ``str`` **Description:** The name of the main TeX
+manuscript (without the path or the extension). Change this if you'd prefer to
+name your manuscript something other than ``ms``. Note that you should still
+keep it in the ``src/tex`` directory. Note also that the compiled PDF file will
+have the same name (e.g., ``ms_name: article`` will compile ``src/tex/
+article.tex`` and generate ``article.pdf`` in the repository root) .
 **Required:** no **Default:** ``ms`` **Example:** .. code-block:: yaml ms_name:
 article .. _config.optimize_caching: ``optimize_caching`` ^^^^^^^^^^^^^^^^^^^^
 **Type:** ``bool`` **Description:** Optimize the workflow graph by removing
 unnecessary jobs upstream of cache hits? Can in some cases significantly reduce
 computation time; see `here
 github.com/showyourwork/showyourwork/issues/124>`__ for a detailed discussion.
 Snakemake does not do this optimization, so it is implemented as a patch on the
@@ -155,15 +183,15 @@
 **Description:** Commit and push Overleaf changes to the GitHub remote when
 running on GitHub Actions? **Default:** ``true`` **Required:** no **Example:**
 .. code-block:: yaml overleaf: gh_actions_sync: true .. _config.overleaf.id:
 ``overleaf.id`` ^^^^^^^^^^^^^^^ **Type:** ``str`` **Description:** The id of
 the Overleaf project to integrate with. This can be obtained from the URL of
 the project, e.g.: .. code-block:: bash https://www.overleaf.com/project/
 6262c032aae5421d6d945acf in this case, the id is ``6262c032aae5421d6d945acf``.
-.. warning:: Please read the :doc:`Overlaf ` integration docs before manually
+.. warning:: Please read the :doc:`Overleaf ` integration docs before manually
 adding/changing this value, as you could risk losing changes to your local
 document or to your Overleaf document the next time you build! **Required:** no
 **Example:** .. code-block:: yaml overleaf: id: 62150dd16134ef045f81d1c8 ..
 _config.overleaf.pull: ``overleaf.pull`` ^^^^^^^^^^^^^^^^^ **Type:** ``bool``
 **Description:** A list of files and/or folders to be pulled from the Overleaf
 project before every build. These should be files that are only ever modified
 on Overleaf, such as the TeX manuscript and other TeX files. Paths should be
```

### Comparing `showyourwork-0.4.2rc2/docs/faqs.rst` & `showyourwork-0.4.3rc2/docs/faqs.rst`

 * *Files 4% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 channel priorities on the ``conda`` side -- `see here <https://github.com/conda/conda/issues/11555>`__.
 For a longer discussion on issues and best practice recommendations related to the reproducibility
 of ``conda`` environments -- and a discussion of reproducibility of software in general --
 please check out :doc:`reproducibility`.
 
 
 Issues with ``datrie``
----------------------
+----------------------
 
 The ``datrie`` package, a dependency  of ``snakemake``, does not currently (as of
 the writing of these docs) have
 `wheels built for distributions of Python >= 3.9 <https://pypi.org/project/datrie/#files>`__.
 If you don't have a valid ``C/C++``
 compiler set up on your machine, the installation of this dependency might fail
 when running ``pip install showyourwork``. One workaround is to install ``datrie``
@@ -530,7 +530,47 @@
 
 This is a bug in ``showyourwork`` related to the fact that the default git branch on Overleaf
 projects is called ``master``, while the default branch on GitHub is called ``main``. This
 isn't an issue unless users don't have the correct credentials to access an Overleaf repository,
 in which case the ``git clone`` silently fails and no ``master`` branch is created.
 If you run into this error, delete or comment out the ``overleaf:`` section of the ``environment.yml``
 workflow config and re-run the workflow, or simply upgrade |showyourwork|.
+
+
+Debugging in |showyourwork|'s conda environment
+-----------------------------------------------
+
+Sometimes when debugging it can be helpful to bypass the ``showyourwork build`` command and
+run your code manually in the same environment |showyourwork| is using. To do that, you
+need to access the `conda environment <https://docs.conda.io/en/latest/>`_ that Snakemake
+creates.
+
+If conda is not your default package manager you may need to activate it using
+``conda activate``. Once activated, you can view the environments that exist on your
+computer using ``conda env list``. On a Unix machine, the output will look something like this:
+
+.. code-block:: text
+
+  base     /path/to/miniconda3
+           /path/to/my-article/.snakemake/conda/28e8667c7a3a18371030aff088ceb5c5_
+
+where "`/path/to/`" is often your home directory or wherever you installed Anaconda and cloned your article's repository.
+
+The environment for the |showyourwork| project is not given a name, but the path
+to the environment should be listed. The environment path will be something of the form:
+`the path to your article` + ``.snakemake/conda`` + `a long
+hexadecimal string (called a hash)`. In this example the environment path is
+``/path/to/my-article/.snakemake/conda/28e8667c7a3a18371030aff088ceb5c5_``.
+
+To activate the environment, copy and paste that full path and run ``conda activate <full path>``.
+For example:
+
+.. code-block:: text
+
+  conda activate /path/to/my-article/.snakemake/conda/28e8667c7a3a18371030aff088ceb5c5_
+
+Ideally there is only one environment per article that fits this format. If this isn't the
+case, we recommend selecting the most recent environment (lowest on the list).
+
+From this point, anything you run using the ``python`` command should use the same conda
+environment |showyourwork| is using behind the scenes. You can confirm this by running
+``which python`` and verifying that the path includes ``.snakemake/conda/``.
```

### Comparing `showyourwork-0.4.2rc2/docs/hacks.py` & `showyourwork-0.4.3rc2/docs/hacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 resp.headers["Link"]
                 .split(",")[1]
                 .split("per_page=1&page=")[1]
                 .split(">")[0]
             )
         else:
             commits = 0
-    except:
+    except Exception:
         commits = "N/A"
     return commits
 
 
 def get_date(repo, API_KEY):
     """
     Get the timestamp when a repo was last pushed to.
@@ -48,15 +48,15 @@
     req.add_header("Accept", "application/vnd.github.v3+json")
     req.add_header("Authorization", f"token {API_KEY}")
     req.add_header("User-Agent", "request")
     try:
         content = urlopen(req).read()
         content = json.loads(content)
         date = content["pushed_at"]
-    except:
+    except Exception:
         date = "??"
     return date
 
 
 def get_version(repo, API_KEY):
     """
     Get the showyourwork SHA or version from the config file.
@@ -71,15 +71,15 @@
         content = json.loads(content)
         branch = content.get("default_branch", "main")
         req = Request(
             f"https://raw.githubusercontent.com/{repo}/{branch}/showyourwork.yml"
         )
         content = urlopen(req).read()
         version = yaml.safe_load(content).get("version", "unknown")
-    except:
+    except Exception:
         version = "unknown"
     return version
 
 
 class RemoveSubmodulesHeading(StopIteration):
     pass
 
@@ -164,15 +164,15 @@
 url = "https://raw.githubusercontent.com/showyourwork/showyourwork-action/main/README.rst"
 try:
     r = requests.get(url, allow_redirects=True)
     content = r.content.decode()
     content = "The GitHub action\n=================\n\n" + "\n".join(
         content.split("\n")[10:]
     )
-except:
+except Exception:
     content = "The Github action\n=================\n\n"
     content += "Please visit `<https://github.com/showyourwork/showyourwork-action>`_."
     print("ERROR: Unable to generate `action.rst`.")
 with open("action.rst", "w") as f:
     f.write(content)
```

### Comparing `showyourwork-0.4.2rc2/docs/index.rst` & `showyourwork-0.4.3rc2/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -51,11 +51,12 @@
    latex
    zenodo
    overleaf
    logging
    migrating
    reproducibility
    faqs
+   contributorguide
    api/showyourwork
    changelog
    attribution
    projects
```

#### html2text {}

```diff
@@ -15,9 +15,9 @@
 github.com/showyourwork/showyourwork>`__. It is very much a work-in-progress,
 so please look over the `issues page
 github.com/showyourwork/showyourwork/issues>`__ if you think you've spotted a
 bug, and feel free to `raise a new issue
 github.com/showyourwork/showyourwork/issues/new>`__ if needed! Community
 contributions are also **most welcome**. Contents -------- .. toctree:: :
 maxdepth: 1 intro install quickstart cli layout config snakefile action latex
-zenodo overleaf logging migrating reproducibility faqs api/showyourwork
-changelog attribution projects
+zenodo overleaf logging migrating reproducibility faqs contributorguide api/
+showyourwork changelog attribution projects
```

### Comparing `showyourwork-0.4.2rc2/docs/install.rst` & `showyourwork-0.4.3rc2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/integration_tests.rst` & `showyourwork-0.4.3rc2/docs/integration_tests.rst`

 * *Files 2% similar despite different names*

```diff
@@ -99,20 +99,20 @@
 Note that several integration tests are marked with the ``remote`` mark (using ``pytest.mark``),
 which means they require push access to the ``showyourwork`` organization in order
 to test the entire workflow, including the ``showyourwork-action`` and the generation
 of the PDF when running on the remote.
 Each of these tests creates a temporary repository in the
 `github.com/showyourwork` organization with the same name as the test
 (but in ``snake_case`` instead of ``camelCase``); if a repository already exists,
-the test will force-push new commits to it, mimicing the behavior of a newly
+the test will force-push new commits to it, mimicking the behavior of a newly
 created repository.
 
 Remote tests are spawned from the `remote_integration_tests.yml`
 workflow in `.github/workflows` of the ``showyourwork/showyourwork`` repository
 on ``push`` events. These do not get run on forks, since they do not have
 write access to the ``showyourwork`` organization. This means pull request
 tests can only check unit tests and local integration tests. In order to run
 remote tests on pull requests, maintainers may label them with the ``safe to test``
-label, in which case the `remote_integration_tests.yml` worfklow is executed with the
+label, in which case the `remote_integration_tests.yml` workflow is executed with the
 ``pull_request_target`` trigger. Maintainers should carefully review the proposed
 changes to check for malicious code before marking PRs as ``safe to test``, since
 the workflow will have full write privileges to the organization!
```

### Comparing `showyourwork-0.4.2rc2/docs/intro.rst` & `showyourwork-0.4.3rc2/docs/intro.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 Introduction
 ============
 
 The |showyourwork| workflow is intended to help authors publish open source,
 replicable, and reproducible scientific articles. It ensures that the article
-PDF is always in sync with all of the scripts, code, and data used to generate it. It does this
-automatically—and seamlessly—with the help of the `Snakemake workflow management system <https://snakemake.readthedocs.io>`_,
-the `tectonic typesetting engine <https://tectonic-typesetting.github.io>`_, and
-`Github Actions CI <https://github.com/features/actions>`_.
+PDF is always in sync with all of the scripts, code, and data used to generate
+it.
+
+To achieve this, |showyourwork| represents all steps required to go from raw
+data to publication figures (and possibly even tables and macros) in a workflow
+file that can be used to reproduce all or part of the elements in a
+paper, potentially including any content that can be programmatically generated
+(e.g., numerical simulations, data reduction, fetching data from third-party
+releases, and plotting). It does this automatically—and seamlessly—with the
+help of the `Snakemake workflow management system
+<https://snakemake.readthedocs.io>`_, the `tectonic typesetting engine
+<https://tectonic-typesetting.github.io>`_, and `Github Actions CI
+<https://github.com/features/actions>`_.  Since |showyourwork| is built upon
+Snakemake, it can encompass arbitrarily complex workflows.
 
 .. raw:: html
 
     <div class="admonition note">
         <p class="admonition-title">The showyourwork philosophy</p>
         <p>Scientific papers should exist as GitHub repositories comprised of
         LaTeX files, figure scripts, rules to generate and/or access datasets, a platform/environment specification,
@@ -42,11 +52,13 @@
 .. include:: quickbuild.rst
 
 To get started with |showyourwork|, check out the :doc:`quickstart tutorial <quickstart>`.
 You should also read about
 the :doc:`showyourwork GitHub action <action>`, :doc:`LaTeX instructions <latex>`, and
 how to :doc:`build your article locally <cli>`.
 
+To take full advantage of |showyourwork|, it is worth learning about Snakemake and how to structure projects in a modular way to facilitate different levels of reproducibility. Some examples of this are provided in the :doc:`Snakefile <snakefile>` section.
+
 You should also spend some time browsing through the :doc:`FAQs page <faqs>`. Since |showyourwork|
 is itself a work in progress, new features are still being added frequently. If you spot a bug,
 have a question, or would like |showyourwork| to do something it doesn't currently support,
 please feel free to raise a `GitHub issue <https://github.com/showyourwork/showyourwork/issues>`_.
```

### Comparing `showyourwork-0.4.2rc2/docs/latex.rst` & `showyourwork-0.4.3rc2/docs/latex.rst`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 .. image:: _static/article-abstract.png
    :width: 100%
    :align: center
 
 When you execute your workflow, |showyourwork| dynamically embellishes the
 ``showyourwork.sty`` file with all of the metadata needed to annotate the PDF
 with the custom margin icons linking to the repository and the scripts that
-generated the invididual figures.
+generated the individual figures.
 
 While most users don't have to worry about how any of this works, it's important to
 keep in mind that this dynamically-generated style sheet redefines certain LaTeX commands under
 the hood, such as the ``abstract`` and ``figure`` environments and the
 ``includegraphics`` command. For instance, in order to include the
 margin icons next to the abstract, |showyourwork| simply patches the ``abstract``
 command to include a ``marginnote``. If you try to compile your PDF with a standard
```

### Comparing `showyourwork-0.4.2rc2/docs/layout.rst` & `showyourwork-0.4.3rc2/docs/layout.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/logging.rst` & `showyourwork-0.4.3rc2/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/migrating.rst` & `showyourwork-0.4.3rc2/docs/migrating.rst`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 9. Add a file called ``showyourwork.sty`` to ``src/tex``. You can copy it over from
    `the example repository <https://github.com/showyourwork/showyourwork-example/blob/main/src/tex/showyourwork.sty>`__.
    This is the new |showyourwork| LaTeX style file.
 
 10. Read about changes to the way |showyourwork| parses LaTeX at :doc:`latex`. The two big changes
     are that you must now explicitly import the ``showyourwork`` style file (see above) using
-    ``\usepackage{showyourwork}`` and that relationships beteween figure scripts and figure files
+    ``\usepackage{showyourwork}`` and that relationships between figure scripts and figure files
     are no longer inferred from the figure ``\label``. Instead, users should explicitly provide
     the path to the script (relative to ``src/scripts``) that generates figures inside a
     ``figure`` environment via the ``\script`` command. Edit your figure environments in your
     tex file accordingly; see :doc:`latex` for details, as there are a few other subtleties.
 
 11. Rename the ``src/figures`` directory to ``src/scripts``. This folder should still contain
     your figure scripts--just its naming convention in |showyourwork| changed. Hint: to preserve your
```

### Comparing `showyourwork-0.4.2rc2/docs/overleaf.rst` & `showyourwork-0.4.3rc2/docs/overleaf.rst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/projects.json` & `showyourwork-0.4.3rc2/docs/projects.json`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/projects.rst.jinja` & `showyourwork-0.4.3rc2/docs/projects.rst.jinja`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/docs/quickbuild.rst` & `showyourwork-0.4.3rc2/docs/quickbuild.rst`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         <br/>
 
    3. Build!
 
       .. code-block:: bash
 
-         showyourwork
+         showyourwork build
 
       .. raw:: html
 
          <pre>
          <span style="color:green;">Setting up the workflow...</span>
          <span style="color:green;">Generating the article PDF...</span>
          <span style="color:green;">Done!</span>
```

### Comparing `showyourwork-0.4.2rc2/docs/quickstart.rst` & `showyourwork-0.4.3rc2/docs/quickstart.rst`

 * *Files 3% similar despite different names*

```diff
@@ -116,15 +116,36 @@
 .. code-block:: bash
 
     showyourwork
 
 
 in the top level of your repository. The first time you run this, |showyourwork|
 will set up a new ``conda`` environment and install a bunch of packages, so it
-could take one or two minutes. The workflow will then build your article PDF,
+could take one or two minutes.
+
+
+.. note::
+
+    Be default, *showyourwork* will use the `conda` executable to create the
+    virtual environment.
+
+    At times this can prove to be very slow, depending on how many and which channels
+    are used (especially the very big `conda-forge`).
+
+    In order to make the environment creation faster, it is recommended to use the
+    `mamba <https://mamba.readthedocs.io/en/latest/index.html>`_ executable via
+    the associated option of the build command,
+
+    .. code-block:: bash
+
+        showyourwork build --conda-frontend=mamba
+
+    This feature is only available for `showyourwork >= v0.4.2`.
+
+The workflow will then build your article PDF,
 which by default is saved as ``ms.pdf`` in the top level of your repository:
 
 
 .. image:: _static/default_ms.png
    :width: 60%
    :align: center
```

#### html2text {}

```diff
@@ -53,16 +53,24 @@
 thing you might want to do is edit the main TeX file, which is located at
 ``src/tex/ms.tex``. Give it a custom title, edit the author name, and replace
 some of the Lorem Ipsum placeholder text with something informative. Then,
 compile the article PDF by running .. code-block:: bash showyourwork build or,
 as a shorthand, just .. code-block:: bash showyourwork in the top level of your
 repository. The first time you run this, |showyourwork| will set up a new
 ``conda`` environment and install a bunch of packages, so it could take one or
-two minutes. The workflow will then build your article PDF, which by default is
-saved as ``ms.pdf`` in the top level of your repository: .. image:: _static/
+two minutes. .. note:: Be default, *showyourwork* will use the `conda`
+executable to create the virtual environment. At times this can prove to be
+very slow, depending on how many and which channels are used (especially the
+very big `conda-forge`). In order to make the environment creation faster, it
+is recommended to use the `mamba
+mamba.readthedocs.io/en/latest/index.html>`_ executable via the associated
+option of the build command, .. code-block:: bash showyourwork build --conda-
+frontend=mamba This feature is only available for `showyourwork >= v0.4.2`. The
+workflow will then build your article PDF, which by default is saved as
+``ms.pdf`` in the top level of your repository: .. image:: _static/
 default_ms.png :width: 60% :align: center There's not much to see -- mostly
 placeholder text. One thing to note, though, is the blue GitHub icon in the
 right margin next to the abstract: this is a hyperlink pointing to your github
 repository (or, in this example, to ``github.com/rodluger/article``.) Let's
 turn this into a proper scientific article by adding a figure. In
 |showyourwork|, all figures should be programmatically generated, so we start
 by creating a script to generate the figure. For simplicity, let's create a
```

### Comparing `showyourwork-0.4.2rc2/docs/snakefile.rst` & `showyourwork-0.4.3rc2/docs/snakefile.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,27 @@
-The Snakefile
-=============
+Intro to Snakemake
+==================
+
+Under the hood, |showyourwork| is essentially a wrapper around Snakemake. The
+code builds the article PDF by parsing the ``showyourwork.yml`` config file and
+the ``ms.tex`` manuscript to build the computational graph for the workflow,
+identifying which scripts it needs to execute and which datasets it needs to
+download to produce all the figures in the article. If you poke around the
+API, you'll see that |showyourwork| defines several Snakemake rules to do
+these various tasks, then hands over full control to Snakemake.
 
-Overview
---------
+If your article consists only of text and figures that can be generated by
+running lightweight scripts, you probably don't need to worry about any of this.
+But for certain use cases, it can be convenient to extend or even override some
+of the |showyourwork| functionality by defining custom Snakemake rules.
+Below we discuss a few examples of this.
+
+
+The Snakefile
+-------------
 
 Every ``showyourwork`` article repository is instantiated with a blank Snakefile
 at the repository root. This file gets included at the start of the main (build) step of the
 workflow, and may thus be used to define custom rules or to run custom ``python``
 code during the workflow. Almost everything you need to know about Snakefiles can
 be found in the
 `Snakemake documentation <https://snakemake.readthedocs.io/en/stable/snakefiles/rules.html>`_,
@@ -73,32 +88,14 @@
 input files and parameters can be provided as *functions*, adding another
 layer of flexibility to your workflow. Rules can also be declared within
 for loops, if statements, etc. For the full list of features, please refer
 to the
 `Snakemake documentation <https://snakemake.readthedocs.io/en/stable/snakefiles/rules.html>`_.
 
 
-Integration with |showyourwork|
--------------------------------
-
-Under the hood, |showyourwork| is essentially a wrapper around Snakemake. The
-code builds the article PDF by parsing the ``showyourwork.yml`` config file and
-the ``ms.tex`` manuscript to build the computational graph for the workflow,
-identifying which scripts it needs to execute and which datasets it needs to
-download to produce all the figures in the article. If you poke around the
-API, you'll see that |showyourwork| defines several Snakemake rules to do
-these various tasks, then hands over full control to Snakemake.
-
-If your article consists only of text and figures that can be generated by
-running lightweight scripts, you probably don't need to worry about any of this.
-But for certain use cases, it can be convenient to extend or even override some
-of the |showyourwork| functionality by defining custom Snakemake rules.
-Below we discuss a few examples of this.
-
-
 Intermediate results
 --------------------
 
 An example usage of the Snakefile is discussed in the :doc:`zenodo` guide, where we show
 how to define a Snakemake rule to generate **intermediate results**. The idea here
 is that partitioning one's workflow into *pipeline* steps and *plotting* steps
 can make it easier for the author (and the interested reader) while writing or
@@ -195,7 +192,19 @@
 It is also possible to entirely override |showyourwork| rules. When ingesting
 user-defined rules from the Snakefile, the code automatically gives precedence
 to those rules over |showyourwork| rules (by setting a higher ``ruleorder`` for
 all user rules). This means that if there are two rules that can generate the
 same output, Snakemake will always favor the user-defined rule.
 You can take advantage of this to provide custom rules to build individual
 figures or even the article PDF itself.
+
+Using existing (data) files in a workflow by ignoring timestamps
+----------------------------------------------------------------
+
+When starting up a project or when in a rapid development phase, it can be useful to
+tell Snakemake to ignore changes to a file or timestamp when running the build. For
+example, you may have a slow rule to generate a data file from querying an external data
+archive and you just want to use a temporary subset of the data or existing copy of the
+data. Snakemake supports this with the ``ancient()`` command. See the `Snakemake
+documentation
+<https://snakemake.readthedocs.io/en/stable/snakefiles/rules.html#ignoring-timestamps>`_
+for more information about how to use this in a rule.
```

### Comparing `showyourwork-0.4.2rc2/docs/zenodo.rst` & `showyourwork-0.4.3rc2/docs/zenodo.rst`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 which has limited compute resources and a timeout of a few hours.
 
 The way |showyourwork| deals with these cases is to cache these lengthy
 computations on Zenodo or Zenodo Sandbox alongside a record of all the
 inputs that went into generating the cached output. If, on subsequent runs
 of the workflow, the inputs remain unchanged, |showyourwork| will simply
 download the cached results from Zenodo or Zenodo Sandbox, *maintaining the guarantee that
-the output you get follows determinstically from the given inputs*.
+the output you get follows deterministically from the given inputs*.
 
 Before we get into how this works and how to take advantage of it, let's
 discuss how to set up the integration by generating Zenodo and Zenodo Sandbox API tokens.
 
 
 Setting up Zenodo integration
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
```

### Comparing `showyourwork-0.4.2rc2/pyproject.toml` & `showyourwork-0.4.3rc2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=45", "setuptools_scm[toml]>=7.0.1"]
+requires = ["setuptools>=45.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "showyourwork/_showyourwork_version.py"
 write_to_template = '__version__ = "{version}"'
 
 [tool.black]
```

### Comparing `showyourwork-0.4.2rc2/setup.py` & `showyourwork-0.4.3rc2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,13 +35,10 @@
         ]
     },
     entry_points={
         "console_scripts": [
             "showyourwork=showyourwork.cli:entry_point",
         ]
     },
-    setup_requires=[
-        "setuptools_scm>=7.0.1",
-    ],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/cli/commands/build.py` & `showyourwork-0.4.3rc2/showyourwork/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cli/commands/cache.py` & `showyourwork-0.4.3rc2/showyourwork/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cli/commands/clean.py` & `showyourwork-0.4.3rc2/showyourwork/cli/commands/clean.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,9 +35,7 @@
                 file.unlink()
         for file in paths.user().data.rglob("*.*"):
             if file.name != ".gitignore":
                 file.unlink()
     if deep:
         if (paths.user().repo / ".snakemake").exists():
             shutil.rmtree(paths.user().repo / ".snakemake")
-        if paths.user().home_temp.exists():
-            shutil.rmtree(paths.user().home_temp)
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/cli/commands/preprocess.py` & `showyourwork-0.4.3rc2/showyourwork/cli/commands/preprocess.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cli/commands/run_snakemake.py` & `showyourwork-0.4.3rc2/showyourwork/cli/commands/run_snakemake.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cli/commands/setup.py` & `showyourwork-0.4.3rc2/showyourwork/cli/commands/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         ssh (bool): If True, use SSH to clone the repository. Otherwise, use HTTPS.
         action_spec (str or None): Showyourwork version passed to showyourwork-action in `.github/workflows/*.yml`
 
     """
     # Parse the slug
     user, repo = slug.split("/")
     if Path(repo).exists():
-
         # Check if it's an empty git repository
         def callback(code, stdout, stderr):
             if code != 0:
                 # `git log` errors if there are no commits;
                 # that's what we want
                 return
             else:
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/cli/commands/tarball.py` & `showyourwork-0.4.3rc2/showyourwork/cli/commands/tarball.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cli/commands/zenodo.py` & `showyourwork-0.4.3rc2/showyourwork/cli/commands/zenodo.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cli/main.py` & `showyourwork-0.4.3rc2/showyourwork/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,60 @@
 import os
 import re
 import shutil
+from collections import namedtuple
+from contextlib import contextmanager
 from textwrap import TextWrapper
 
 import click
 
-from .. import exceptions, git
+from .. import __version__, exceptions, git
 from . import commands
 
-# Store command & option metadata here so we can make `build`
-# the default subcommand in __init__.py
-DEFAULT_SUBCOMMAND = "build"
 SUBCOMMANDS = ["build", "cache", "clean", "setup", "tarball"]
 OPTIONS = ["-v", "--version", "--help"]
 
 
+# Common options:
+option_spec = namedtuple("option_spec", ["args", "kwargs"])
+cores_option = option_spec(
+    args=["-c", "--cores"],
+    kwargs=dict(
+        default="1",
+        help="Number of cores to use; passed to snakemake.",
+    ),
+)
+conda_frontend_option = option_spec(
+    args=["--conda-frontend"],
+    kwargs=dict(
+        default="conda",
+        help="The conda frontend to use; passed to snakemake.",
+    ),
+)
+project_option = option_spec(
+    args=["-p", "--project"],
+    kwargs=dict(
+        default=".",
+        help="The root folder of the showyourwork project.",
+    ),
+)
+branch_option = option_spec(
+    args=["-b", "--branch"],
+    kwargs=dict(
+        required=False,
+        default=None,
+        help="Branch whose deposit is to be deleted. Default is current branch.",
+    ),
+)
+
+
+def main_command(f):
+    return main.command(context_settings=dict(ignore_unknown_options=True))(f)
+
+
 def ensure_top_level():
     """Ensures we're running commands in the top level of a git repo.
 
     Raises:
         exceptions.ShowyourworkException: If not in the top level of a git repo.
     """
     root = os.path.realpath(git.get_repo_root())
@@ -29,29 +65,38 @@
             "from the top level of a git repository."
             "\n"
             "`showyourwork` by itself runs a document build. "
             "Did you mean to run `showyourwork setup`?"
         )
 
 
+@contextmanager
+def cwd_as(path):
+    """Temporarily change the current working directory to `path`."""
+    old_dir = os.getcwd()
+    os.chdir(path)
+    yield
+    os.chdir(old_dir)
+
+
 def echo(text="", **kwargs):
     """Print a message to the terminal with some custom formatting.
 
     Breaks long lines using ``TextWrapper`` and adds custom colors and
     indentation to code snippets and environment variables.
 
     This may just be the ugliest function I've ever written in my life.
 
     Args:
         text (str): The text to print.
         kwargs: Additional keyword arguments to pass to ``click.echo``.
     """
     try:
         terminal_size = shutil.get_terminal_size().columns
-    except:
+    except Exception:
         terminal_size = 80
     wrapper = TextWrapper(
         width=terminal_size,
         drop_whitespace=True,
         initial_indent="",
     )
     text = text.replace("\n", " ")
@@ -69,69 +114,63 @@
         text = text.replace("<BR>", "\n")
         if n == len(lines) - 1:
             if text.endswith("\n"):
                 text = text[:-1]
         click.echo(text, **kwargs)
 
 
-@click.group
+@click.group()
+@click.version_option(
+    __version__,
+    "--version",
+    "-v",
+    package_name="showyourwork",
+    message="%(version)s",
+)
 def main():
     """Easily build open-source, reproducible scientific articles."""
     pass
 
 
-@main.command(
-    context_settings=dict(
-        ignore_unknown_options=True,
-    )
-)
-@click.option(
-    "-c",
-    "--cores",
-    default="1",
-    help="Number of cores to use; passed to snakemake.",
-)
-@click.option(
-    "--conda-frontend",
-    default="conda",
-    help="The conda frontend to use; passed to snakemake.",
-)
+@main_command
+@click.option(*cores_option.args, **cores_option.kwargs)
+@click.option(*conda_frontend_option.args, **conda_frontend_option.kwargs)
+@click.option(*project_option.args, **project_option.kwargs)
 @click.argument("snakemake_args", nargs=-1, type=click.UNPROCESSED)
-def build(cores, conda_frontend, snakemake_args):
+def build(cores, conda_frontend, project, snakemake_args):
     """Build an article in the current working directory."""
-    ensure_top_level()
-    commands.preprocess(
-        snakemake_args=snakemake_args,
-        cores=cores,
-        conda_frontend=conda_frontend,
-    )
-    commands.build(
-        snakemake_args=snakemake_args,
-        cores=cores,
-        conda_frontend=conda_frontend,
-    )
+    with cwd_as(project):
+        ensure_top_level()
+        commands.preprocess(
+            snakemake_args=snakemake_args,
+            cores=cores,
+            conda_frontend=conda_frontend,
+        )
+        commands.build(
+            snakemake_args=snakemake_args,
+            cores=cores,
+            conda_frontend=conda_frontend,
+        )
 
 
 def validate_slug(context, param, slug):
     """Checks whether the repo slug was provided correctly."""
 
     def pause():
         if context.params.get("yes"):
             pass
         else:
             click.echo("\nPress any key to continue, or Ctrl+C to abort...")
             click.getchar()
             click.echo()
 
     if "/" in slug and len(slug.split("/")) == 2:
-
         user, repo = slug.split("/")
 
         if not context.params.get("quiet"):
-
             # Greeting
             echo(
                 f"""
                 Let's get you set up with a new repository. I'm going to create
                 a folder called ``{repo}`` in the current working directory. If
                 you haven't done this yet, please visit
                 ``https://github.com/new`` at this time and create an empty
@@ -199,15 +238,14 @@
                     """
                 )
             pause()
 
         return slug
 
     else:
-
         raise click.BadParameter("Must have the form `user/repo`.")
 
 
 @main.command()
 @click.argument("slug", callback=validate_slug, metavar="<user/repo>")
 @click.option(
     "-y",
@@ -261,143 +299,103 @@
     This command expects a single positional argument, `SLUG`, of the form
     `user/repo`, where `user` is the user's GitHub handle and `repo` is the
     name of the repository (and local directory) to create.
     """
     commands.setup(slug, cache, overleaf, ssh, action_spec)
 
 
-@main.command(
-    context_settings=dict(
-        ignore_unknown_options=True,
-    )
-)
-@click.option(
-    "-c",
-    "--cores",
-    default="1",
-    help="Number of cores to use; passed to snakemake.",
-)
-@click.option(
-    "--conda-frontend",
-    default="conda",
-    help="The conda frontend to use; passed to snakemake.",
-)
+@main_command
+@click.option(*cores_option.args, **cores_option.kwargs)
+@click.option(*conda_frontend_option.args, **conda_frontend_option.kwargs)
+@click.option(*project_option.args, **project_option.kwargs)
 @click.option(
     "-f",
     "--force",
     is_flag=True,
     help="Forcefully remove everything in the `src/tex/figures` and `src/data` directories.",
 )
 @click.option(
     "-d",
     "--deep",
     is_flag=True,
     help="Forcefully remove the `.snakemake` and `~/.showyourwork` directories.",
 )
 @click.argument("snakemake_args", nargs=-1, type=click.UNPROCESSED)
-def clean(cores, conda_frontend, force, deep, snakemake_args):
+def clean(cores, conda_frontend, project, force, deep, snakemake_args):
     """Clean the article build in the current working directory."""
-    ensure_top_level()
-    commands.clean(
-        force,
-        deep,
-        snakemake_args=snakemake_args,
-        cores=cores,
-        conda_frontend=conda_frontend,
-    )
+    with cwd_as(project):
+        ensure_top_level()
+        commands.clean(
+            force,
+            deep,
+            snakemake_args=snakemake_args,
+            cores=cores,
+            conda_frontend=conda_frontend,
+        )
 
 
-@main.command(
-    context_settings=dict(
-        ignore_unknown_options=True,
-    )
-)
-@click.option(
-    "-c",
-    "--cores",
-    default="1",
-    help="Number of cores to use; passed to snakemake.",
-)
-@click.option(
-    "--conda-frontend",
-    default="conda",
-    help="The conda frontend to use; passed to snakemake.",
-)
+@main_command
+@click.option(*cores_option.args, **cores_option.kwargs)
+@click.option(*conda_frontend_option.args, **conda_frontend_option.kwargs)
+@click.option(*project_option.args, **project_option.kwargs)
 @click.argument("snakemake_args", nargs=-1, type=click.UNPROCESSED)
-def tarball(cores, conda_frontend, snakemake_args):
+def tarball(cores, conda_frontend, project, snakemake_args):
     """Generate a tarball of the build in the current working directory."""
-    ensure_top_level()
-    commands.preprocess(
-        snakemake_args=snakemake_args,
-        cores=cores,
-        conda_frontend=conda_frontend,
-    )
-    commands.tarball(
-        snakemake_args=snakemake_args,
-        cores=cores,
-        conda_frontend=conda_frontend,
-    )
+    with cwd_as(project):
+        ensure_top_level()
+        commands.preprocess(
+            snakemake_args=snakemake_args,
+            cores=cores,
+            conda_frontend=conda_frontend,
+        )
+        commands.tarball(
+            snakemake_args=snakemake_args,
+            cores=cores,
+            conda_frontend=conda_frontend,
+        )
 
 
 @main.group()
 @click.pass_context
 def cache(ctx):
     """Caching-related operations."""
     pass
 
 
 @cache.command()
 @click.pass_context
-@click.option(
-    "-b",
-    "--branch",
-    required=False,
-    default=None,
-    help="Which branch to create the deposit for. Default is current branch.",
-)
+@click.option(*branch_option.args, **branch_option.kwargs)
 def create(ctx, branch):
     """
     Create a Zenodo Sandbox deposit draft for the given branch.
 
     Requires a Zenodo Sandbox API token provided as the
     environment variable and Github repository secret `SANDBOX_TOKEN`.
     """
     ensure_top_level()
     commands.zenodo_create(branch)
 
 
 @cache.command()
 @click.pass_context
-@click.option(
-    "-b",
-    "--branch",
-    required=False,
-    default=None,
-    help="Branch whose deposit is to be deleted. Default is current branch.",
-)
+@click.option(*branch_option.args, **branch_option.kwargs)
 def delete(ctx, branch):
     """
     Delete the latest draft of a Zenodo Sandbox deposit.
 
     Requires a Zenodo Sandbox API token provided as the
     environment variable and Github repository secret `SANDBOX_TOKEN`.
     """
     ensure_top_level()
     commands.zenodo_delete(branch)
 
 
 @cache.command()
 @click.pass_context
-@click.option(
-    "-b",
-    "--branch",
-    required=False,
-    default=None,
-    help="Branch whose deposit is to be frozen. Default is current branch.",
-)
+@click.option(*branch_option.args, **branch_option.kwargs)
 def freeze(ctx, branch):
     """
     Publishes the current Zenodo Sandbox deposit draft for the given branch
     to Zenodo Sandbox.
 
     Useful for preserving the current cache state even when changes are made
     to the rule inputs. Note that Zenodo Sandbox storage is temporary, so if
@@ -409,21 +407,15 @@
     """
     ensure_top_level()
     commands.zenodo_freeze(branch)
 
 
 @cache.command()
 @click.pass_context
-@click.option(
-    "-b",
-    "--branch",
-    required=False,
-    default=None,
-    help="Branch whose deposit is to be published. Default is current branch.",
-)
+@click.option(*branch_option.args, **branch_option.kwargs)
 def publish(ctx, branch):
     """
     Publishes the current Zenodo Sandbox deposit draft for the given branch
     to Zenodo for permanent, public storage. This action assigns a permanent,
     static DOI to the deposit, which cannot be deleted or undone.
 
     Requires a Zenodo API token provided as the environment variable
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/config.py` & `showyourwork-0.4.3rc2/showyourwork/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -236,15 +236,14 @@
 
     # During the preprocessing stage, we import user settings,
     # set defaults, and record additional internal settings.
     # These get recorded in a JSON file which is loaded as
     # the main config file in the build stage, so all these
     # settings are available in both stages.
     if Path(snakemake.workflow.workflow.main_snakefile).name == "prep.smk":
-
         #
         # -- User settings --
         #
 
         #: Showyourwork version
         config["version"] = config.get("version", None)
 
@@ -334,14 +333,40 @@
         config["stamp"]["url"]["enabled"] = config["stamp"]["url"].get(
             "enabled", False
         )
         config["stamp"]["url"]["maxlen"] = config["stamp"]["url"].get(
             "maxlen", 40
         )
 
+        #: Showyourwork margin_icon settings
+        config["margin_icons"] = as_dict(config.get("margin_icons", {}))
+        config["margin_icons"]["colors"] = as_dict(
+            config["margin_icons"].get("colors", {})
+        )
+        config["margin_icons"]["monochrome"] = config["margin_icons"].get(
+            "monochrome", False
+        )
+        config["margin_icons"]["colors"]["github"] = config["margin_icons"][
+            "colors"
+        ].get("github", "0.12,0.47,0.71")
+        config["margin_icons"]["colors"]["sandbox"] = config["margin_icons"][
+            "colors"
+        ].get("sandbox", "0.80,0.14,0.19")
+        config["margin_icons"]["colors"]["cache"] = config["margin_icons"][
+            "colors"
+        ].get("cache", "0.12,0.47,0.71")
+        config["margin_icons"]["colors"]["dataset"] = config["margin_icons"][
+            "colors"
+        ].get("dataset", "0.12,0.47,0.71")
+        offset = int(config["margin_icons"].get("horizontal_offset", 0))
+        if offset < 0:
+            config["margin_icons"]["horizontal_offset"] = r"\!" * abs(offset)
+        else:
+            config["margin_icons"]["horizontal_offset"] = "\," * offset
+
         #
         # -- Internal settings --
         #
 
         # Cache settings
         config["cache"] = config.get("cache", {})
 
@@ -352,21 +377,14 @@
         config["workflow_abspath"] = paths.showyourwork().workflow.as_posix()
 
         # TeX auxiliary files
         config["tex_files_in"] = [
             file.as_posix()
             for file in (paths.showyourwork().resources / "tex").glob("*")
         ]
-        config["tex_files_out"] = [
-            (
-                paths.user().tex.relative_to(paths.user().repo)
-                / Path(file).name
-            ).as_posix()
-            for file in config["tex_files_in"]
-        ]
 
         # The main tex file and the compiled pdf
         config["ms_tex"] = (
             paths.user().tex.relative_to(paths.user().repo)
             / (config["ms_name"] + ".tex")
         ).as_posix()
         config["ms_pdf"] = config["ms_name"] + ".pdf"
@@ -375,24 +393,16 @@
         config["config_json"] = (
             (paths.user().temp / "config.json")
             .relative_to(paths.user().repo)
             .as_posix()
         )
 
         # Paths to the TeX stylesheets
-        config["stylesheet"] = (
-            (paths.user().tex / "showyourwork.tex")
-            .relative_to(paths.user().repo)
-            .as_posix()
-        )
-        config["stylesheet_meta_file"] = (
-            (paths.user().tex / "showyourwork-metadata.tex")
-            .relative_to(paths.user().repo)
-            .as_posix()
-        )
+        config["stylesheet"] = "showyourwork.tex"
+        config["stylesheet_meta_file"] = "showyourwork-metadata.tex"
 
         # Script extensions
         config["script_extensions"] = list(config["scripts"].keys())
 
         # Overridden in the `preprocess` rule
         config["tree"] = {"figures": {}}
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build-pull-request.yml` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build-pull-request.yml`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build.yml` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/LICENSE` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/LICENSE`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/README.md` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/README.md`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/showyourwork.yml` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/showyourwork.yml`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/paths.py` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/scripts/paths.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aasjournal.bst` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aasjournal.bst`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aastex631.cls` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/aastex631.cls`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/bib.bib` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/bib.bib`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/ms.tex` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/ms.tex`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/orcid-ID.png` & `showyourwork-0.4.3rc2/showyourwork/cookiecutter-showyourwork/{{ cookiecutter.repo }}/src/tex/orcid-ID.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/exceptions/base.py` & `showyourwork-0.4.3rc2/showyourwork/exceptions/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,27 +33,27 @@
     The traceback gets logged to file, unless the logging level
     is `DEBUG`, in which case it also gets printed to the screen.
     """
     traceback.print_exception = redirect_exception
     sys.excepthook = custom_excepthook
     try:
         flag = paths.user().flags / "DISABLE_SNAKEMAKE_EXCEPTIONS"
-    except:
+    except Exception:
         pass
     else:
         flag.touch()
 
 
 def restore_trace():
     """Restore traceback printing to the screen."""
     traceback.print_exception = print_exception
     sys.excepthook = excepthook
     try:
         flag = paths.user().flags / "DISABLE_SNAKEMAKE_EXCEPTIONS"
-    except:
+    except Exception:
         pass
     else:
         if flag.exists():
             flag.unlink()
 
 
 class ShowyourworkException(Exception):
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/exceptions/latex.py` & `showyourwork-0.4.3rc2/showyourwork/exceptions/latex.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,35 +23,32 @@
                 if "Package: showyourwork" in line:
                     showyourwork_imported = True
                     break
             else:
                 showyourwork_imported = False
 
             if showyourwork_imported:
-
                 # Scan the log for an error message
                 for i, line in enumerate(tectonic_log[::-1]):
                     if line.startswith("!"):
                         message = "".join(tectonic_log[-i - 1 :])
                         break
                 else:
                     message = (
                         "An error occurred while compiling the manuscript."
                     )
                 message += f"\nFor more information, check out the log file:\n{logfile}."
             else:
-
                 # Admonish the user (:
                 message = (
                     r"Failed to compile manuscript. Perhaps you forgot to `\usepackage{showyourwork}`?"
                     f"\nFor more information, check out the log file:\n{logfile}"
                 )
 
         else:
-
             # No log to scan, so we're stuck with an uninformative message...
             message = "An error occurred while compiling the manuscript."
 
         super().__init__(message)
 
 
 class FigureFormatError(LaTeXException):
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/exceptions/other.py` & `showyourwork-0.4.3rc2/showyourwork/exceptions/other.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/exceptions/overleaf.py` & `showyourwork-0.4.3rc2/showyourwork/exceptions/overleaf.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/exceptions/zenodo.py` & `showyourwork-0.4.3rc2/showyourwork/exceptions/zenodo.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/git.py` & `showyourwork-0.4.3rc2/showyourwork/git.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/gitapi.py` & `showyourwork-0.4.3rc2/showyourwork/gitapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,14 @@
     )
 
     # Flatten the search criteria
     q = flatten_dict(q)
 
     # Return the first match
     for workflow_run in data["workflow_runs"]:
-
         # Flatten the response
         workflow_run = flatten_dict(workflow_run)
 
         # Check for matches
         for key, value in q.items():
             if workflow_run.get(key) != value:
                 break
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/logging.py` & `showyourwork-0.4.3rc2/showyourwork/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,35 +84,31 @@
     Sets up the logging if needed.
 
     """
     logger = logging.getLogger("showyourwork")
 
     # Add showyourwork stream & file handlers
     if not logger.handlers:
-
         # Root level
         logger.setLevel(logging.DEBUG)
 
         # Terminal: all messages
         stream_handler = ColorizingStreamHandler()
         stream_handler.setLevel(logging.INFO)
         logger.addHandler(stream_handler)
 
         try:
-
             LOGS = paths.user().logs
 
-        except:
-
+        except Exception:
             # Can't resolve path to logs; assume we're not
             # in a showyourwork/git repo and fail silently.
             pass
 
         else:
-
             # File: all showyourwork messages
             msg_file = LOGS / "showyourwork.log"
             file_handler = logging.FileHandler(msg_file)
             file_handler.setLevel(logging.DEBUG)
             logger.addHandler(file_handler)
 
     return logger
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/overleaf.py` & `showyourwork-0.4.3rc2/showyourwork/overleaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,40 @@
 
 from . import exceptions, logging, paths
 from .subproc import get_stdout
 
 OVERLEAF_BLANK_PROJECT_REGEX_TEMPLATE = r"[\n\r\s]+".join(
     [
         r"\\documentclass{article}",
-        r"\\usepackage\[utf8\]{inputenc}",
+        r"(\\usepackage{graphicx} % Required for inserting images)|(\\usepackage\[utf8\]{inputenc})",
         r"\\title{[^\n{}]+?}",
         r"\\author{[^\n{}]+?}",
         r"\\date{[^\n{}]+?}",
         r"\\begin{document}",
         r"\\maketitle",
         r"\\section{Introduction}",
         r"\\end{document}",
     ]
 )
 
 OVERLEAF_BLANK_PROJECT = r"""\documentclass{article}
-\usepackage[utf8]{inputenc}
+\usepackage{graphicx} % Required for inserting images
 
 \title{blank project}
-\author{Rodrigo Luger}
-\date{April 2022}
+\author{Dan Foreman-Mackey}
+\date{March 2023}
 
 \begin{document}
 
 \maketitle
 
 \section{Introduction}
 
-\end{document}"""
+\end{document}
+"""
 
 
 def check_for_rate_limit(code, stdout, stderr):
     """
     Callback function to check if we hit a rate limit on Overleaf.
 
     """
@@ -142,23 +143,26 @@
         ["git", "pull", url],
         cwd=str(paths.user(path=path).overleaf),
         secrets=[overleaf_email, overleaf_password],
         callback=callback,
     )
 
 
-def wipe_remote(project_id):
+def wipe_remote(project_id, tex=None):
     """
     Remove all files from the Overleaf project and start fresh as if it were a
     blank project.
 
     Args:
         project_id (str): The Overleaf project ID.
 
     """
+    if tex is None:
+        tex = OVERLEAF_BLANK_PROJECT
+
     with TemporaryDirectory() as cwd:
         get_stdout(["git", "init"], cwd=cwd)
         get_stdout(["git", "checkout", "-b", "master"], cwd=cwd)
         (
             overleaf_email,
             overleaf_password,
         ) = get_overleaf_credentials()
@@ -169,15 +173,15 @@
         get_stdout(
             ["git", "pull", url],
             cwd=cwd,
             secrets=[overleaf_email, overleaf_password],
         )
         get_stdout(["git", "rm", "-r", "*"], cwd=cwd)
         with open(Path(cwd) / "main.tex", "w") as f:
-            print(OVERLEAF_BLANK_PROJECT, file=f)
+            print(tex, file=f)
         get_stdout(["git", "add", "main.tex"], cwd=cwd)
 
         def callback(code, stdout, stderr):
             if code != 0:
                 if (
                     "Your branch is up to date" in stdout + stderr
                     or "nothing to commit" in stdout + stderr
@@ -239,32 +243,32 @@
             # by comparing it to the blank project regex template
             with open(files[0], "r") as f:
                 contents = f.read()
             if re.match(OVERLEAF_BLANK_PROJECT_REGEX_TEMPLATE, contents):
                 pass
             else:
                 raise Exception()
-    except:
+    except Exception:
         raise exceptions.OverleafError(
             "Overleaf repository not empty! "
             "Refusing to rewrite files on remote."
         )
     else:
         # Delete the file
         files[0].unlink()
         get_stdout(
             ["git", "add", files[0].name],
             cwd=str(paths.user(path=path).overleaf),
         )
 
     # Copy over all files in the `tex` directory
     for file in paths.user(path=path).tex.glob("*"):
-
         # Copy it to the local version of the repo
         file = Path(file).resolve()
+        logger.info(file)
         remote_file = paths.user(path=path).overleaf / file.relative_to(
             paths.user(path=path).tex
         )
         if file.is_dir():
             if remote_file.exists():
                 shutil.rmtree(remote_file)
             shutil.copytree(file, remote_file)
@@ -275,14 +279,15 @@
         get_stdout(
             [
                 "git",
                 "add",
                 remote_file.relative_to(paths.user(path=path).overleaf),
             ],
             cwd=str(paths.user(path=path).overleaf),
+            callback=lambda *_: None,
         )
 
     # Commit callback
     def callback(code, stdout, stderr):
         if stdout:
             logger.debug(stdout)
         if code != 0:
@@ -346,15 +351,14 @@
         # Not fatal!
         exceptions.restore_trace()
         return
 
     # Process each file
     skip = []
     for file in files:
-
         # Copy it to the local version of the repo
         if not Path(file).exists():
             skip.append(file)
             continue
         file = Path(file).resolve()
         remote_file = paths.user(path=path).overleaf / file.relative_to(
             paths.user(path=path).tex
@@ -576,15 +580,15 @@
             else:
                 if (
                     "Your branch is up to date" in stdout + stderr
                     or "nothing to commit" in stdout + stderr
                     or "nothing added to commit" in stdout + stderr
                 ):
                     logger.warning(
-                        f"No Overleaf changes to commit to the repo."
+                        "No Overleaf changes to commit to the repo."
                     )
                 else:
                     raise exceptions.CalledProcessError(stdout + "\n" + stderr)
 
         get_stdout(
             [
                 "git",
@@ -597,9 +601,8 @@
                 "[showyourwork] overleaf sync",
             ],
             cwd=paths.user(path=path).repo,
             callback=callback,
         )
 
         if push_changes:
-
             get_stdout(["git", "push"], cwd=paths.user(path=path).repo)
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/patches.py` & `showyourwork-0.4.3rc2/showyourwork/patches.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
     # Get the showyourwork logger
     logger = get_logger()
 
     # The instance we'll patch
     output_file_cache = snakemake.workflow.workflow.output_file_cache
 
     if output_file_cache is not None:
-
         # Instantiate our interfaces
         if zenodo_doi is not None:
             zenodo = Zenodo(zenodo_doi)
         else:
             zenodo = None
         if sandbox_doi is not None:
             sandbox = Zenodo(sandbox_doi)
@@ -231,15 +230,14 @@
 
         def store(self, job):
             # Call the original method
             result = _store(job)
 
             # GitHub Actions runs should never update the cache
             if not snakemake.workflow.config.get("github_actions"):
-
                 # See note in `fetch()` about tarballs
                 if job.output[0].is_directory:
                     tarball = True
                 else:
                     tarball = False
 
                 for (
@@ -303,40 +301,37 @@
         snakemake_logger.logger.addHandler(
             snakemake_logger.custom_stream_handler
         )
 
     # Custom Snakemake file handler
     if not hasattr(snakemake_logger, "custom_file_handler"):
         try:
-
             LOGS = paths.user().logs
 
-        except:
-
+        except Exception:
             # Can't resolve path to logs; assume we're not
             # in a showyourwork/git repo and fail silently.
             pass
 
         else:
-
             snakemake_logger.custom_file_handler = logging.FileHandler(
                 paths.user().logs / "snakemake.log"
             )
             snakemake_logger.custom_file_handler.setLevel(logging.DEBUG)
             snakemake_logger.logger.addHandler(
                 snakemake_logger.custom_file_handler
             )
 
     # Suppress Snakemake exceptions if we caught them on the
     # showyourwork side
     def job_error(self, **msg):
         msg["level"] = "job_error"
         try:
             FLAGS = paths.user().flags
-        except:
+        except Exception:
             self.handler(msg)
         else:
             if (FLAGS / "DISABLE_SNAKEMAKE_EXCEPTIONS").exists():
                 for handler in snakemake_logger.logger.handlers:
                     if not isinstance(handler, logging.FileHandler):
                         handler.setLevel(logging.CRITICAL)
             else:
@@ -444,15 +439,15 @@
     # Check for a local cache hit
     try:
         if cache.exists(job):
             logger.debug(f"Local cache exists for job {job.name}.")
             return True
         else:
             pass
-    except:
+    except Exception:
         # Job is not cacheable (no output files or multiple output files)
         logger.debug(f"Job {job.name} is not cacheable.")
         return False
 
     # Check if a remote cache exists
     branch = snakemake.workflow.config["git_branch"]
     zenodo_doi = snakemake.workflow.config["cache"][branch]["zenodo"]
@@ -506,18 +501,16 @@
 
     # Nodes we can skip
     nodes = set(cached_jobs)
 
     # Loop until there are no changes to the graph
     new_nodes = True
     while new_nodes:
-
         new_nodes = set()
         for node in nodes:
-
             # Find all parents that are in `nodes`
             parents = set()
             for file in node.input:
                 try:
                     parents |= set(dag.file2jobs(file)).difference(nodes)
                 except snakemake.exceptions.MissingRuleException:
                     # Not all files have producers
@@ -549,33 +542,30 @@
     See the full discussion about this feature
     `here <https://github.com/showyourwork/showyourwork/issues/124>`__.
 
     """
     logger = get_logger()
 
     if snakemake.workflow.workflow.output_file_cache is not None:
-
         # Get list of jobs we can skip
         skippable_jobs = get_skippable_jobs(dag)
         logger.debug(
             "Skipping the following jobs because of downstream cache hits:"
         )
         logger.debug("    " + " ".join([job.name for job in skippable_jobs]))
 
         # Patch the Snakemake method that executes jobs
         scheduler = snakemake.workflow.workflow.scheduler
         for executor in scheduler._executor, scheduler._local_executor:
             if executor:
-
                 # Original method
                 _cached_or_run = executor.cached_or_run
 
                 # Intercept jobs we don't need to run
                 def wrapper(self, job, run_func, *args):
-
                     if job in skippable_jobs:
                         # Instead of running this job, we create empty temp
                         # outputs to trick Snakemake & keep going
                         for output in job.output:
                             if not output.exists:
                                 logger.warning(
                                     f"Skipping job {job.name} because "
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/paths.py` & `showyourwork-0.4.3rc2/showyourwork/paths.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/subproc.py` & `showyourwork-0.4.3rc2/showyourwork/subproc.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/userrules.py` & `showyourwork-0.4.3rc2/showyourwork/userrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     if cache_sandbox_doi and get_run_type == "build":
         get_logger().warn(
             f"Zenodo cache not yet published for this repository."
         )
 
     # Process each user rule
     for ur in user_rules:
-
         # Set its order > all showyourwork rules
         for sr in syw_rules:
             snakemake.workflow.workflow.ruleorder(ur.name, sr.name)
 
         # Add a message if it doesn't have one
         if not ur.message:
             ur.message = f"Running user rule {ur.name}..."
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/build.smk` & `showyourwork-0.4.3rc2/showyourwork/workflow/build.smk`

 * *Files 1% similar despite different names*

```diff
@@ -54,21 +54,21 @@
     # deleted; these are the rules we actually call from the Makefile
     rule syw__arxiv_entrypoint:
         input:
             "arxiv.tar.gz"
 
 
     # Include all other rules
+    include: "rules/common.smk"
     include: "rules/dag.smk"
     include: "rules/arxiv.smk"
     include: "rules/compile.smk"
     include: "rules/zenodo.smk"
     include: "rules/figure.smk"
     include: "rules/render_dag.smk"
-    include: "rules/conda.smk"
 
     # Resolve ambiguities in rule order
     ruleorder: syw__compile > syw__arxiv
 
 
     # Include custom rules defined by the user
     include: (paths.user().repo / "Snakefile").as_posix()
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/prep.smk` & `showyourwork-0.4.3rc2/showyourwork/workflow/prep.smk`

 * *Files 7% similar despite different names*

```diff
@@ -46,17 +46,16 @@
 # Hack to make the configfile generation the default rule
 rule syw__main:
     input:
         config["config_json"]
 
 
 # Include all other rules
+include: "rules/common.smk"
 include: "rules/preprocess.smk"
-include: "rules/conda.smk"
-
 
 onstart:
 
 
     # Overleaf sync: pull in changes
     if run_type == "preprocess" and get_repo_branch() == "main":
         overleaf.pull_files(
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/resources/img/article-thumb.png` & `showyourwork-0.4.3rc2/showyourwork/workflow/resources/img/article-thumb.png`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/resources/styles/build.tex` & `showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/build.tex`

 * *Files 20% similar despite different names*

```diff
@@ -51,22 +51,17 @@
 \newcommand\script[1]{}
 
 % Showyourwork logo
 \newcommand{\showyourwork}{%
   \smash{\raisebox{-1.4ex}{\includegraphics[width=7.3em]{showyourwork-logo.pdf}}}\xspace%
 }
 
-% Define custom colors
-\definecolor{sywRed}{rgb}{0.80,0.14,0.19}
+% Define custom stamp colors
 \definecolor{sywStampRed}{rgb}{0.80,0.45,0.45}
 \definecolor{sywStampLightRed}{rgb}{0.90,0.74,0.74}
-\definecolor{sywOrange}{rgb}{1.0,0.65,0.0}
-\definecolor{sywYellow}{rgb}{1.0,0.88,0.30}
-\definecolor{sywBlue}{rgb}{0.12,0.47,0.71}
-\definecolor{sywGreen}{rgb}{0.13,0.53,0.23}
 
 % Generate the stamp on the first page
 \ifAddStamp
   % No-op offsets. Override these for, e.g.,
   % specific documentclasses that require a
   % different default stamp position.
   \newcommand{\syw@stampXOffset}{0.00}
@@ -128,87 +123,70 @@
 \newcommand\GitHubSHA{\syw@sha}
 \newcommand\GitHubIcon{\faGithub\xspace}
 
 % Figure script icon
 \newcommand\syw@Script[1]{%
   \raisebox{0pt}[6pt][0pt]{%
     \href{\syw@url/blob/\syw@sha/\usevalue{#1}}{%
-      \color{sywBlue}\faGithub%
+      \color{github-icon}\faGithub%
     }%
   }%
 }
 
 % Figure dataset icon
 \newcommand\syw@DatasetOne[1]{%
   \raisebox{0pt}[6pt][6pt]{%
     \href{\usevalue{#1}}{%
-      \color{sywBlue}\faDatabase%
+      \color{dataset-icon}\faDatabase%
     }%
   }%
 }
 
 % Figure dataset icon
 \newcommand\syw@DatasetTwo[1]{%
   \raisebox{0pt}[6pt][6pt]{%
     \href{\usevalue{#1}}{%
-      \color{sywBlue}\faDatabase%
+      \color{dataset-icon}\faDatabase%
     }%
   }%
 }
 
 % Figure dataset icon
 \newcommand\syw@DatasetThree[1]{%
   \raisebox{0pt}[6pt][6pt]{%
     \href{\usevalue{#1}}{%
-      \color{sywBlue}\faDatabase%
+      \color{dataset-icon}\faDatabase%
     }%
   }%
 }
 
 % Figure cache icon
 \newcommand\syw@Cache[1]{%
   \raisebox{0pt}[6pt][6pt]{%
     \IfSubStr*{\usevalue{#1}}{sandbox}{%
       \href{\usevalue{#1}}{%
-        \color{sywRed}\faRecycle%
+        \color{sandbox-icon}\faRecycle%
       }%
     }{%
       \href{\usevalue{#1}}{%
-        \color{sywBlue}\faRecycle%
+        \color{cache-icon}\faRecycle%
       }%
     }%
   }%
 }
 
 % Variable script icon: links to a line in the Snakefile
 \newcommand\syw@Variable[1]{%
   \raisebox{0pt}[6pt][0pt]{%
     \href{\syw@url/blob/\syw@sha/\usevalue{#1}}{%
-      \color{sywBlue}\faGithub%
+      \color{github-icon}\faGithub%
     }%
   }%
 }
 
-% Hack `showkeys' to show margin links for figures and variables
-% See https://tex.stackexchange.com/a/580553
-\renewcommand\showkeyslabelformat[1]{%
-  \normalfont%
-  \setstackgap{S}{0pt}
-  \Shortstack[c]{
-    \IfEq*{\usevalue{#1_cache}}{KEYNOTFOUND}{}{\syw@Cache{#1_cache}}
-    \IfEq*{\usevalue{#1_datasetThree}}{KEYNOTFOUND}{}{\syw@DatasetThree{#1_datasetThree}}
-    \IfEq*{\usevalue{#1_datasetTwo}}{KEYNOTFOUND}{}{\syw@DatasetTwo{#1_datasetTwo}}
-    \IfEq*{\usevalue{#1_datasetOne}}{KEYNOTFOUND}{}{\syw@DatasetOne{#1_datasetOne}}
-    \IfEq*{\usevalue{#1_script}}{KEYNOTFOUND}{}{\syw@Script{#1_script}}
-  }
-  % Link to the line in the Snakefile that generates a given variable
-  % in the texfile
-  \IfEq*{\usevalue{#1_rule}}{KEYNOTFOUND}{}{\syw@Variable{#1_rule}}
-}
-
 % Set the graphics path for all figures
 \graphicspath{{./}{./figures/}}
 
 % Alias of \input for syw-controlled files
 \newcommand\variable[1]{%
-  \input{#1}\label{#1}\unskip%
+  \input{#1}\unskip\label{#1}\unskip%
 }
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/resources/styles/preprocess.tex` & `showyourwork-0.4.3rc2/showyourwork/workflow/resources/styles/preprocess.tex`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/lineno.sty` & `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/lineno.sty`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/listofitems.tex` & `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/listofitems.tex`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/showyourwork-logo.pdf` & `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork-logo.pdf`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/showyourwork-stamp.pdf` & `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork-stamp.pdf`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/showyourwork.otf` & `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/showyourwork.otf`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/resources/tex/xstring.tex` & `showyourwork-0.4.3rc2/showyourwork/workflow/resources/tex/xstring.tex`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/rules/arxiv.smk` & `showyourwork-0.4.3rc2/showyourwork/workflow/rules/render_dag.smk`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 """
-Defines the rule ``syw__arxiv`` to generate a tarball for arXiv submission.
+Defines the rule ``syw__render_dag`` to render the article DAG.
 
-Runs the script :doc:`arxiv` to generate the tarball ``arxiv.tar.gz``.
+Runs the script :doc:`render_dag` to generate ``dag.pdf``.
 
 """
 from showyourwork import paths
 
+# All figure output files
+figures = config["tree"]["figures"].keys()
 
 rule:
     """
-    Generate a tarball for arXiv submission.
+    Render the article DAG.
 
     """
     name:
-        "syw__arxiv"
+        "syw__render_dag"
     message:
-        "Generating the arXiv tarball..."
+        "Rendering the article DAG..."
     input:
         config["ms_tex"],
         config["dependencies"][config["ms_tex"]],
         WORKFLOW_GRAPH,
-        "showyourwork.yml",
-        paths.user().flags / "SYW__CONDA"
+        "showyourwork.yml"
     output:
-        "arxiv.tar.gz",
-        config["ms_pdf"],
-        temp(config["tex_files_out"]),
-        temp(config["stylesheet"]),
-        temp(config["stylesheet_meta_file"]),
-        directory(paths.user().compile.as_posix())
+       "dag.pdf"
+    conda:
+        (paths.showyourwork().envs / "render_dag.yml").as_posix()
+    params:
+        repo=paths.user().repo,
+        flags=paths.user().flags,
+        data=paths.user().data,
+        scripts=paths.user().scripts,
+        figures=paths.user().figures,
+        tex=paths.user().tex,
+        compile=paths.user().compile,
+        preprocess=paths.user().preprocess,
+        resources=paths.showyourwork().resources,
     script:
-        "../scripts/arxiv.py"
+        "../scripts/render_dag.py"
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/rules/dag.smk` & `showyourwork-0.4.3rc2/showyourwork/workflow/rules/dag.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/rules/figure.smk` & `showyourwork-0.4.3rc2/showyourwork/workflow/rules/figure.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/rules/zenodo.smk` & `showyourwork-0.4.3rc2/showyourwork/workflow/rules/zenodo.smk`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/scripts/arxiv.py` & `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/arxiv.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,36 +5,29 @@
 
 """
 import tarfile
 
 from showyourwork import paths
 
 if __name__ == "__main__":
-
     # Snakemake config (available automagically)
     config = snakemake.config  # type:ignore
 
-    # Hack to run the `pdf.py` script
-    script = __file__.replace("arxiv.py", "pdf.py")
-    with open(script, "r") as f:
-        script = f.read()
-    exec(script)
-
     # File names to exclude
-    ms_name = snakemake.config["ms_name"]
+    ms_name = config["ms_name"]
     exclude = [
         ".gitignore",
         f"{ms_name}.pdf",
         f"{ms_name}.aux",
         f"{ms_name}.blg",
         f"{ms_name}.log",
         f"{ms_name}.out",
+        f"{ms_name}.fls",
+        f"{ms_name}.synctex.gz",
+        f"{ms_name}.fdb_latexmk",
     ]
 
     # Tar up everything in the src/tex directory
     with tarfile.open("arxiv.tar.gz", "w:gz") as tarball:
-        for file in paths.user().tex.rglob("*"):
-            if not file.is_dir() and not file.name in exclude:
-                tarball.add(file, arcname=file.relative_to(paths.user().tex))
         for file in paths.user().compile.rglob("*"):
             if file.name not in exclude:
                 tarball.add(file, arcname=file.name)
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/scripts/download.py` & `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import subprocess
 
 from showyourwork import exceptions
 from showyourwork.logging import get_logger
 from showyourwork.zenodo import Zenodo
 
 if __name__ == "__main__":
-
     # Snakemake config (available automagically)
     config = snakemake.config  # type:ignore
 
     # Get params
     doi = snakemake.params["doi"]
     remote_file = snakemake.params["remote_file"]
     output = snakemake.output[0]
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/scripts/extract.py` & `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,62 +8,50 @@
 from pathlib import Path
 from zipfile import ZipFile
 
 from showyourwork import exceptions
 from showyourwork.logging import get_logger
 
 if __name__ == "__main__":
-
     # Snakemake config (available automagically)
     config = snakemake.config  # type:ignore
 
     # Initialize the logger
     logger = get_logger()
 
     # Input/output file names
     zipfile = Path(snakemake.input[0])
     extracted_file = Path(snakemake.output[0])
     compressed_file = snakemake.params["compressed_file"]
 
     # Tar balls
     if zipfile.name.endswith(".tar") or zipfile.name.endswith(".tar.gz"):
-
         # Open the tarball
         with tarfile.open(zipfile) as f:
-
             # Extract into a temp folder
             with tempfile.TemporaryDirectory() as TEMP:
-
                 try:
-
                     f.extract(compressed_file, TEMP)
 
                 except Exception as e:
-
                     raise exceptions.TarballExtractionError(str(e))
 
                 # Move it to target destination
                 shutil.move(Path(TEMP) / compressed_file, extracted_file)
 
     # Zip files
     elif zipfile.name.endswith(".zip"):
-
         # Open the tarball
         with ZipFile(zipfile, "r") as f:
-
             # Extract into a temp folder
             with tempfile.TemporaryDirectory() as TEMP:
-
                 try:
-
                     f.extract(compressed_file, TEMP)
 
                 except Exception as e:
-
                     raise exceptions.TarballExtractionError(str(e))
 
                 # Move it to target destination
                 shutil.move(Path(TEMP) / compressed_file, extracted_file)
 
     else:
-
         raise exceptions.NotImplementedError("Unsupported archive file type.")
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/scripts/preprocess.py` & `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import re
 from collections.abc import MutableMapping
 from pathlib import Path
 from xml.etree.ElementTree import parse as ParseXMLTree
 
 from showyourwork import exceptions, paths, zenodo
 from showyourwork.config import get_upstream_dependencies
-from showyourwork.tex import compile_tex
 from showyourwork.zenodo import Zenodo, get_dataset_urls
 
 
 def flatten_dataset_contents(d, parent_key="", default_path=None):
     """
     Flatten the ``contents`` dictionary of a dataset entry, filling
     in default mappings and removing zipfile extensions from the target path.
@@ -77,15 +76,14 @@
     """
     Parse the ``datasets`` keys in the config file and populate entries with
     custom metadata.
 
     """
 
     for doi, entry in config["datasets"].items():
-
         # Parse the DOI to get the Zenodo ID
         deposit = Zenodo(doi)
 
         # Require that this is a static *version* ID
         entry["id_type"] = deposit.get_id_type()
         if entry["id_type"] != "version":
             if entry["id_type"] == "concept":
@@ -110,15 +108,14 @@
             entry.get("contents", {}), default_path=entry["destination"]
         )
 
         # Handle files inside zipfiles, tarballs, etc.
         entry["zip_files"] = {}
         tmp_path = deposit.path().relative_to(paths.user().repo)
         for source in list(contents.keys()):
-
             # Ensure the target is not a list
             target = contents[source]
             if type(target) is list:
                 raise exceptions.ZenodoContentsError(
                     "Error parsing the config. "
                     "The `contents` field of a Zenodo deposit must be "
                     "provided as a mapping, not as a list."
@@ -169,23 +166,21 @@
                     caption_labels[0].text
                 )
             )
 
     # The label must always come after the figure caption
     # Any marginicons must always come before the label
     if len(captions):
-
         # Index of last caption
         for caption_idx, element in enumerate(elements[::-1]):
             if element.tag == "CAPTION":
                 break
         caption_idx = len(elements) - 1 - caption_idx
 
         if len(labels):
-
             # Index of first label
             for label_idx, element in enumerate(elements):
                 if element.tag == "LABEL":
                     break
 
             if label_idx < caption_idx:
                 raise exceptions.FigureFormatError(
@@ -219,36 +214,22 @@
         raise exceptions.FigureFormatError(
             "A figure defines a script but has no label: `{}`".format(
                 ", ".join(script.text for script in scripts)
             )
         )
 
 
-def get_xml_tree():
+def get_xml_tree(xmlfile):
     """Compiles the TeX file to generate the XML tree.
 
     Returns:
         xml.etree.ElementTree.ElementTree: The XML tree.
     """
 
-    # Parameters
-    xmlfile = paths.user().preprocess / "showyourwork.xml"
-
-    # Build the paper to get the XML file
-    compile_tex(
-        config,
-        args=[
-            "-r",
-            "0",
-        ],
-        output_dir=paths.user().preprocess,
-        stylesheet=paths.showyourwork().resources
-        / "styles"
-        / "preprocess.tex",
-    )
+    xmlfile = Path(xmlfile)
 
     # Add <HTML></HTML> tags to the XML file
     if xmlfile.exists():
         with open(xmlfile, "r") as f:
             contents = f.read()
     else:
         raise exceptions.MissingXMLFile(
@@ -259,41 +240,40 @@
     with open(xmlfile, "w") as f:
         print(contents, file=f)
 
     # Load the XML tree
     return ParseXMLTree(paths.user().preprocess / "showyourwork.xml").getroot()
 
 
-def get_json_tree():
+def get_json_tree(xmlfile):
     """Builds a dictionary containing mappings between input and output files.
 
     Returns:
         dict: The JSON dependency tree for the article.
     """
     # Get the XML article tree
-    xml_tree = get_xml_tree()
+    xml_tree = get_xml_tree(xmlfile)
 
     # Parse the \graphicspath command
     # Note that if there are multiple graphicspath calls, only the first one
     # is read. Same for multiple directories within a graphicspath call.
     try:
         graphicspath = xml_tree.findall("GRAPHICSPATH")
         if len(graphicspath) == 0:
             graphicspath = Path(".")
         else:
             graphicspath = re.findall("\{(.*?)\}", graphicspath[-1].text)[0]
             graphicspath = Path(graphicspath)
-    except:
+    except Exception:
         raise exceptions.GraphicsPathError()
 
     # Parse labeled graphics inside `figure` environments
     figures = {}
     unlabeled_graphics = []
     for figure in xml_tree.findall("FIGURE"):
-
         # Ensure the figure environment conforms to the standard
         check_figure_format(figure)
 
         # Find all graphics included in this figure environment
         graphics = [
             str(
                 (paths.user().tex / graphicspath / graphic.text)
@@ -312,28 +292,26 @@
                 for graphic in graphics
             ]
         )
 
         # Get the figure \label, if it exists
         labels = figure.findall("LABEL")
         if len(labels):
-
             # We already checked that there's only one label above
             label = labels[0].text
 
         else:
-
             # Treat these as free-floating graphics
             unlabeled_graphics.extend(graphics)
             continue
 
         # Get the figure \script, if it exists
         scripts = figure.findall("SCRIPT")
+        extra_dependencies = []
         if len(scripts) and scripts[0].text is not None:
-
             # The user provided an argument to \script{}, which we assume
             # is the name of the script relative to the figure scripts
             # directory
             script = str(
                 (paths.user().scripts / scripts[0].text).relative_to(
                     paths.user().repo
                 )
@@ -355,42 +333,42 @@
                     "Can't determine how to execute the figure "
                     f"script {scripts[0].text}. Please provide instructions "
                     "on how to execute scripts with this extension in the "
                     "config file."
                 )
 
         else:
-
             # No script provided
             script = None
 
             # If all the figures in this environment exist in the
             # static directory, set up the command to copy them over
             if static:
-                srcs = " ".join(
-                    [
-                        str(
-                            (
-                                paths.user().static / Path(graphic).name
-                            ).relative_to(paths.user().repo)
+                srcs = [
+                    str(
+                        (paths.user().static / Path(graphic).name).relative_to(
+                            paths.user().repo
                         )
-                        for graphic in graphics
-                    ]
-                )
+                    )
+                    for graphic in graphics
+                ]
+                extra_dependencies = srcs
                 dest = paths.user().figures.relative_to(paths.user().repo)
-                command = f"cp {srcs} {dest}"
+                command = f"cp {' '.join(srcs)} {dest}"
 
             else:
-
                 # We don't know how to generate this figure at this time.
                 # Hopefully the user specified a custom Snakemake rule!
                 command = None
 
         # Collect user-defined dependencies
         dependencies = config["dependencies"].get(script, [])
+        if isinstance(dependencies, str):
+            dependencies = [dependencies]
+        dependencies += list(extra_dependencies)
 
         # Same, but recursing all the way up the graph
         # (i.e., including dependendencies of dependencies, and so forth)
         upstream = get_upstream_dependencies(script, config["dependencies"])
 
         # If any of the upstream dependencies exist in a Zenodo deposit, infer
         # their URLs so we can add margin links to the PDF
@@ -463,31 +441,29 @@
         "dependencies": [],
         "command": None,
         "static": False,
     }
 
     # Add entries to the tree: static figures
     # (copy them over from the static folder)
-    srcs = " ".join(
-        [
-            str(
-                (paths.user().static / Path(graphic).name).relative_to(
-                    paths.user().repo
-                )
+    srcs = [
+        str(
+            (paths.user().static / Path(graphic).name).relative_to(
+                paths.user().repo
             )
-            for graphic in free_floating_static
-        ]
-    )
+        )
+        for graphic in free_floating_static
+    ]
     dest = paths.user().figures.relative_to(paths.user().repo)
     figures["free-floating-static"] = {
         "script": None,
         "graphics": free_floating_static,
         "datasets": [],
-        "dependencies": [],
-        "command": f"cp {srcs} {dest}",
+        "dependencies": srcs,
+        "command": f"cp {' '.join(srcs)} {dest}",
         "static": True,
     }
 
     # Parse files included using the \input statement;
     # these will be made explicit dependencies of the build
     files = [
         str(
@@ -501,23 +477,22 @@
     # The full tree (someday we'll have equations in here, too)
     tree = {"figures": figures, "files": files}
 
     return tree
 
 
 if __name__ == "__main__":
-
     # Snakemake config (available automagically)
     config = snakemake.config  # type:ignore
 
     # Parse the `datasets` key in the config
     parse_datasets()
 
     # Get the article tree
-    config["tree"] = get_json_tree()
+    config["tree"] = get_json_tree(snakemake.input[0])
 
     # Make all of the graphics dependencies of the article
     config["dependencies"][config["ms_tex"]] = config["dependencies"].get(
         config["ms_tex"], []
     )
     for figure_name in config["tree"]["figures"]:
         graphics = config["tree"]["figures"][figure_name]["graphics"]
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/workflow/scripts/render_dag.py` & `showyourwork-0.4.3rc2/showyourwork/workflow/scripts/render_dag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 """
 Generates a directed acyclic graph (DAG) of the build process.
 
 """
+import subprocess
 from pathlib import Path
 
 import graphviz
 
-from showyourwork import paths
-from showyourwork.subproc import get_stdout
-from showyourwork.zenodo import get_dataset_dois
-
-# Activate the showyourwork conda environment
-conda_activate = open(paths.user().flags / "SYW__CONDA", "r").read()
-
 
 def is_relative_to(path, other):
     """
     Local implementation of `pathlib.Path.is_relative_to` (for python < 3.9).
 
     """
     try:
@@ -40,37 +34,66 @@
 def convert_to_png(file):
     """
     Convert a file to a PNG thumbnail w/ a border and return its aspect ratio.
 
     On error, returns None.
     """
     try:
-
-        aspect = float(
-            get_stdout(
-                f'{conda_activate} convert "{file}" -format "%[fx:w/h]" info:',
-                shell=True,
-            )
+        result = subprocess.run(
+            f'convert "{file}" -format "%[fx:w/h]" info:',
+            shell=True,
+            stdout=subprocess.PIPE,
         )
+        assert result.returncode == 0
+        aspect = float(result.stdout.decode())
         width = aspect * 500
-        get_stdout(
-            f"{conda_activate} convert -resize {width}x500 -background white -alpha remove "
+        result = subprocess.run(
+            f"convert -resize {width}x500 -background white -alpha remove "
             f'-bordercolor black -border 15 "{file}" "{file}.png"',
             shell=True,
         )
+        assert result.returncode == 0
+
     except Exception:
         return None
     else:
         return aspect
 
 
-if __name__ == "__main__":
+def get_dataset_dois(files, datasets):
+    """
+    Local version of this function copied from `showyourwork/zenodo.py`
 
+    """
+    result = []
+    for doi in datasets:
+        for file in files:
+            if file in datasets[doi]["contents"].values():
+                result.append(doi)
+            else:
+                for zip_file in datasets[doi]["zip_files"]:
+                    if file in datasets[doi]["zip_files"][zip_file].values():
+                        result.append(doi)
+                        break
+    return list(set(result))
+
+
+def should_ignore(ignore, path):
+    path = Path(path).resolve()
+    for pattern in ignore:
+        pattern = Path(pattern).resolve()
+        if path == pattern or is_relative_to(path, pattern):
+            return True
+    return False
+
+
+if __name__ == "__main__":
     # Snakemake config (available automagically)
     config = snakemake.config  # type:ignore
+    params = snakemake.params  # type:ignore
 
     # User settings
     node_attr = config["dag"]["node_attr"]
     graph_attr = config["dag"]["graph_attr"]
     engine = config["dag"]["engine"]
     group_by_type = config["dag"]["group_by_type"]
 
@@ -98,67 +121,76 @@
         node_attr=node_attr,
         graph_attr=graph_attr,
         engine=engine,
     )
 
     # Collect all dependency information
     deps = config["dag_dependencies"]
-    prefix = str(paths.user().repo / "x")[:-1]
+    prefix = str(params.repo / "x")[:-1]
     dependencies = {}
     for f, d in deps.items():
         dependencies[removeprefix(f, prefix)] = [
             removeprefix(file, prefix) for file in d
         ]
 
     # Ignore temporary & showyourwork files
-    ignore = config["tex_files_out"] + [
-        config["stylesheet"],
-        config["stylesheet_meta_file"],
-        str((paths.user().flags / "SYW__DAG").relative_to(paths.user().repo)),
-        str(
-            (paths.user().flags / "SYW__CONDA").relative_to(paths.user().repo)
-        ),
-        str(paths.user().compile.relative_to(paths.user().repo)),
+    ignore = list(config["tex_files_in"]) + [
+        params.resources,
+        params.flags,
+        params.preprocess,
+        params.compile,
         "dag.pdf",
         "showyourwork.yml",
         "zenodo.yml",
     ]
 
     # Ignore user-specified patterns
     user_ignore = []
     for pat in config["dag"]["ignore_files"]:
-        file_list = list(Path(paths.user().repo).glob(pat))
-        file_list = [
-            str(file.relative_to(paths.user().repo)) for file in file_list
-        ]
+        file_list = list(Path(params.repo).glob(pat))
+        file_list = [str(file.relative_to(params.repo)) for file in file_list]
         user_ignore.extend(file_list)
     ignore.extend(user_ignore)
 
+    # Remove ignored files from dependency tree
+    tree = {}
+    for file, parents in dependencies.items():
+        if should_ignore(ignore, file):
+            continue
+        tree[file] = set()
+        for parent in parents:
+            todo = [parent]
+            while len(todo):
+                query = todo.pop()
+                if should_ignore(ignore, query):
+                    todo += dependencies.get(query, [])
+                else:
+                    tree[file] |= {query}
+
     # Assemble all files
     files = []
-    for file in dependencies:
+    for file, parents in tree.items():
         files.append(file)
-        files.extend(dependencies[file])
+        files.extend(parents)
     files = list(set(files))
-    files = [file for file in files if file not in ignore]
 
     # Group into different types
     datasets = []
     scripts = []
     texfiles = []
     figures = []
     others = []
     for file in files:
-        if is_relative_to(Path(file).absolute(), paths.user().data):
+        if is_relative_to(Path(file).absolute(), params.data):
             datasets.append(file)
-        elif is_relative_to(Path(file).absolute(), paths.user().scripts):
+        elif is_relative_to(Path(file).absolute(), params.scripts):
             scripts.append(file)
-        elif is_relative_to(Path(file).absolute(), paths.user().figures):
+        elif is_relative_to(Path(file).absolute(), params.figures):
             figures.append(file)
-        elif is_relative_to(Path(file).absolute(), paths.user().tex):
+        elif is_relative_to(Path(file).absolute(), params.tex):
             texfiles.append(file)
         elif file == config["ms_pdf"]:
             pass
         else:
             others.append(file)
 
     # Get permalink for file
@@ -314,54 +346,53 @@
             fillcolor=colors["article"],
             style="filled",
             label="ms.pdf",
         )
         c.node(
             config["ms_pdf"],
             label="",
-            image=str(
-                paths.showyourwork().resources / "img" / "article-thumb.png"
-            ),
+            image=str(params.resources / "img" / "article-thumb.png"),
             penwidth="0",
             fixedsize="true",
             imagescale="false",
             width="1.15",
             height="1.5",
             color="black" if group_by_type else colors["article"],
             style="filled",
             fillcolor="white",
         )
 
     # Add the edges
     for file in files:
-        for dependency in dependencies.get(file, []):
+        for dependency in tree.get(file, []):
             if dependency not in ignore:
                 dot.edge(dependency, file, color=colors["edge"])
 
                 # Cache
                 if dependency in config["cached_deps"]:
                     dot.edge(
                         cache, dependency, color=colors["edge"], style="dashed"
                     )
                 if file in config["cached_deps"]:
                     dot.edge(
                         dependency, cache, color=colors["edge"], style="dashed"
                     )
 
     # Save the graph
-    dot.save(directory=paths.user().repo)
+    dot.save(directory=params.repo)
 
     # Render the PDF
-    get_stdout(
-        f"{conda_activate} dot -Tpdf dag.gv > dag.pdf",
+    result = subprocess.run(
+        "dot -Tpdf dag.gv > dag.pdf",
         shell=True,
-        cwd=paths.user().repo,
+        cwd=params.repo,
     )
+    assert result.returncode == 0
 
     # Remove temporary files
     for figure in figures:
         pngfile = Path(f"{figure}.png")
         if pngfile.exists():
             pngfile.unlink()
-    gvfile = paths.user().repo / "dag.gv"
+    gvfile = params.repo / "dag.gv"
     if gvfile.exists():
         gvfile.unlink()
```

### Comparing `showyourwork-0.4.2rc2/showyourwork/zenodo.py` & `showyourwork-0.4.3rc2/showyourwork/zenodo.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,29 +117,27 @@
                 (e.g., "zenodo" or "sandbox").
             kwargs: Forwarded to ``Zenodo._create``.
 
         """
 
         # Parse input
         if str(doi_or_service).lower() in services.keys():
-
             # Create a new draft on the given service
             service = services[doi_or_service]
             self.doi_prefix = service["doi_prefix"]
             self.url = service["url"]
             self.token_name = service["token_name"]
             self.access_token = self._get_access_token()
             self.path = service["path"]
             self.service = service["name"]
             self.doi = self._create(**kwargs)
             self.deposit_id = self.doi.split(self.doi_prefix)[1]
             self.user_is_owner = True
 
         else:
-
             # Parse the DOI
             self.doi = doi_or_service
             try:
                 for service in services.values():
                     if self.doi.startswith(service["doi_prefix"]):
                         self.doi_prefix = service["doi_prefix"]
                         self.deposit_id = self.doi.split(self.doi_prefix)[1]
@@ -177,39 +175,35 @@
 
         Caches the result locally.
 
         """
         cache_file = self.path() / f"{self.deposit_id}" / "id_type.txt"
 
         if cache_file.exists():
-
             # Restore from cache
             with open(cache_file, "r") as f:
                 id_type = f.readline().replace("\n", "")
 
         else:
-
             # Try to find a published record (no authentication needed)
             try:
                 r = requests.get(
                     f"https://{self.url}/api/records/{self.deposit_id}"
                 )
                 data = r.json()
             except Exception as e:
                 r = None
                 data = {"status": "", "message": str(e)}
 
             if (r is None) or (r.status_code > 204):
-
                 # Either is private or doesn't exist.
                 # In any event, don't cache it, as this could change.
                 return "unknown"
 
             else:
-
                 # This is a public record
                 if int(self.deposit_id) == int(data["conceptrecid"]):
                     id_type = "concept"
                 elif int(self.deposit_id) == int(data["id"]):
                     id_type = "version"
                 else:
                     id_type = "unknown"
@@ -290,15 +284,14 @@
         )
         if cache_file_true.exists():
             return True
         if cache_file_false.exists():
             return False
 
         if self.access_token:
-
             logger.debug(f"Testing if user is authenticated for {self.doi}...")
 
             # Search for both concept and version DOIs
             r = requests.get(
                 f"https://{self.url}/api/deposit/depositions",
                 params={
                     "q": f"recid:{self.deposit_id} conceptrecid:{self.deposit_id}",
@@ -398,15 +391,15 @@
                     "--upload-file",
                     str(file_to_upload),
                     "--request",
                     "PUT",
                     f"{bucket_url}/{rule_name}?access_token={self.access_token}",
                 ]
             )
-        except:
+        except Exception:
             raise exceptions.ZenodoUploadError()
 
         # Delete the tarball if we created it
         if tarball:
             file_to_upload.unlink()
 
         # Update the provenance
@@ -449,24 +442,22 @@
         )
 
         # Look for a match
         logger.debug(
             f"Searching for file `{rule_name}` with hash `{file.name}`..."
         )
         for entry in data:
-
             logger.debug(
                 f"Inspecting candidate file `{entry['filename']}` with hash `{rule_hashes.get(rule_name, None)}`..."
             )
 
             if (
                 entry["filename"] == rule_name
                 and rule_hashes.get(rule_name, None) == file.name
             ):
-
                 # Download it
                 logger.debug(f"File name and hash both match.")
                 if not dry_run:
                     logger.debug("Downloading...")
                     url = entry["links"]["download"]
                     progress_bar = (
                         ["--progress-bar"]
@@ -480,36 +471,34 @@
                                 "-f",
                                 f"{url}?access_token={self.access_token}",
                                 *progress_bar,
                                 "--output",
                                 str(file),
                             ]
                         )
-                    except:
+                    except Exception:
                         raise exceptions.ZenodoDownloadError()
 
                     # If it's a directory tarball, extract it
                     if tarball:
                         os.rename(file, f"{file}.tar.gz")
                         with tarfile.open(f"{file}.tar.gz") as tb:
                             tb.extractall(file)
                         Path(f"{file}.tar.gz").unlink()
 
                 return
 
             elif entry["filename"] == rule_name:
-
                 # We're done with this deposit
                 logger.debug(
                     f"File {rule_name} found, but it has the wrong hash. Skipping..."
                 )
                 break
 
             else:
-
                 # Keep looking in this deposit for a file with the right name
                 logger.debug(
                     f"Cache miss for file {entry['filename']}. Skipping..."
                 )
 
         # This is caught in the enclosing scope and treated as a cache miss
         raise exceptions.FileNotFoundOnZenodo(rule_name)
@@ -534,15 +523,14 @@
 
         # Look for a match
         for entry in record["files"]:
             if (
                 entry["key"] == rule_name
                 and rule_hashes.get(rule_name, None) == file.name
             ):
-
                 # Download it
                 logger.debug(f"File name and hash both match.")
                 if not dry_run:
                     logger.debug("Downloading...")
                     url = entry["links"]["self"]
                     progress_bar = (
                         ["--progress-bar"]
@@ -565,15 +553,14 @@
                         with tarfile.open(f"{file}.tar.gz") as tb:
                             tb.extractall(file)
                         Path(f"{file}.tar.gz").unlink()
 
                 return
 
             elif entry["key"] == rule_name:
-
                 logger.debug(
                     f"File {rule_name} found, but it has the wrong hash. Skipping..."
                 )
                 break
 
         # This is caught in the enclosing scope and treated as a cache miss
         raise exceptions.FileNotFoundOnZenodo(rule_name)
@@ -601,15 +588,15 @@
         )
         try:
             for data in r.json():
                 if not data["submitted"]:
                     break
             else:
                 raise Exception
-        except:
+        except Exception:
             raise exceptions.ZenodoRecordNotFound(self.deposit_id)
         version_id = data["id"]
         parse_request(
             requests.delete(
                 f"https://{self.url}/api/deposit/depositions/{version_id}",
                 params={
                     "access_token": self.access_token,
@@ -641,15 +628,15 @@
         )
         try:
             for data in r.json():
                 if not data["submitted"]:
                     break
             else:
                 raise Exception
-        except:
+        except Exception:
             raise exceptions.ZenodoRecordNotFound(self.deposit_id)
         version_id = data["id"]
         parse_request(
             requests.post(
                 f"https://{self.url}/api/deposit/depositions/{version_id}/actions/publish",
                 params={
                     "access_token": self.access_token,
@@ -684,15 +671,15 @@
                 "all_versions": 1,
                 "access_token": self.access_token,
             },
         )
         if r.status_code <= 204:
             try:
                 data = r.json()
-            except:
+            except Exception:
                 data = []
             if len(data):
                 data = data[0]
                 draft_url = data.get("links", {}).get("latest_draft", None)
                 if draft_url:
                     r = requests.get(
                         draft_url,
@@ -717,42 +704,42 @@
                             return
                     else:
                         logger.debug(
                             f"Something went wrong accessing {draft_url}."
                         )
                         try:
                             data = r.json()
-                        except:
+                        except Exception:
                             pass
                         else:
                             logger.debug(data["message"])
             else:
                 logger.debug(
                     f"Failed to access {self.service} deposit with DOI {self.doi}."
                 )
         else:
             logger.debug(
                 f"Failed to access {self.service} deposit with DOI {self.doi}."
             )
             try:
                 data = r.json()
-            except:
+            except Exception:
                 pass
             else:
                 logger.debug(data["message"])
 
         # Check for a published record
         logger.debug(
             f"Attempting to access {self.service} record with DOI {self.doi}..."
         )
         r = requests.get(f"https://{self.url}/api/records/{concept_id}")
         if r.status_code > 204:
             try:
                 data = r.json()
-            except:
+            except Exception:
                 data = {}
             if "PID is not registered" in data.get("message", ""):
                 # There is no published record with this id
                 pass
             else:
                 # Something unexpected happened
                 raise exceptions.ZenodoError(
@@ -772,15 +759,15 @@
                     "access_token": self.access_token,
                     "all_versions": 1,
                 },
             )
             if r.status_code <= 204:
                 try:
                     records = r.json().get("hits", {}).get("hits", [])
-                except:
+                except Exception:
                     records = []
                     logger.debug(
                         f"File {rule_name} not found in record with DOI {self.doi}."
                     )
                 for record in records[::-1]:
                     try:
                         self.download_file_from_record(
@@ -797,15 +784,15 @@
                         )
                     else:
                         return
             else:
                 # Something unexpected happened
                 try:
                     data = r.json()
-                except:
+                except Exception:
                     data = {}
                 raise exceptions.ZenodoError(
                     status=data.get("status", "unknown"),
                     message=data.get(
                         "message",
                         f"An error occurred while accessing {self.service}.",
                     ),
@@ -836,46 +823,44 @@
         )
         if r.status_code > 204:
             logger.warning(
                 f"{self.service} authentication failed. Unable to upload cache for rule {rule_name}."
             )
             try:
                 data = r.json()
-            except:
+            except Exception:
                 pass
             else:
                 logger.debug(data["message"])
             return
 
         try:
             data = r.json()
-        except:
+        except Exception:
             data = []
         if len(data):
             data = data[0]
         else:
             logger.warning(
                 f"{self.service} authentication failed. Unable to upload cache for rule {rule_name}."
             )
             return
         draft_url = data.get("links", {}).get("latest_draft", None)
         if not draft_url and not data["submitted"]:
             draft_url = data["links"]["self"]
         if draft_url:
-
             # Draft exists
             draft = parse_request(
                 requests.get(
                     draft_url,
                     params={"access_token": self.access_token},
                 )
             )
 
         else:
-
             # Create a new draft
             data = parse_request(
                 requests.post(
                     f"https://{self.url}/api/deposit/depositions/{data['id']}/actions/newversion",
                     params={"access_token": self.access_token},
                 )
             )
@@ -906,15 +891,15 @@
                 "all_versions": 1,
                 "access_token": self.access_token,
             },
         )
         if r.status_code <= 204:
             try:
                 data = r.json()
-            except:
+            except Exception:
                 raise exceptions.ZenodoError(
                     message=f"Error accessing latest draft for DOI {self.doi}."
                 )
 
             # Look for a draft
             if len(data):
                 data = data[0]
@@ -926,15 +911,15 @@
                 if not draft_url:
                     r = requests.post(
                         f"https://{self.url}/api/deposit/depositions/{data['id']}/actions/newversion",
                         params={"access_token": self.access_token},
                     )
                     try:
                         data = r.json()
-                    except:
+                    except Exception:
                         raise exceptions.ZenodoError(
                             message=f"Error accessing latest draft for DOI {self.doi}."
                         )
                     draft_url = data["links"]["latest_draft"]
 
                 # Grab the draft
                 r = requests.get(
@@ -984,15 +969,15 @@
                         f"{url}?access_token={self.access_token}",
                         "--progress-bar",
                         "--output",
                         entry["filename"],
                     ],
                     cwd=cache_folder,
                 )
-            except:
+            except Exception:
                 raise exceptions.ZenodoDownloadError()
 
         # Return path to cache folder
         return cache_folder
 
     @require_access_token
     def copy_draft(self, target_doi_or_service, **kwargs):
@@ -1019,15 +1004,15 @@
                 "all_versions": 1,
                 "access_token": target_deposit.access_token,
             },
         )
         if r.status_code <= 204:
             try:
                 data = r.json()
-            except:
+            except Exception:
                 raise exceptions.ZenodoError(
                     message=f"Error accessing latest draft for DOI {target_deposit.doi}."
                 )
 
             # Look for a draft
             if len(data):
                 data = data[0]
@@ -1039,15 +1024,15 @@
                 if not draft_url:
                     r = requests.post(
                         f"https://{target_deposit.url}/api/deposit/depositions/{data['id']}/actions/newversion",
                         params={"access_token": target_deposit.access_token},
                     )
                     try:
                         data = r.json()
-                    except:
+                    except Exception:
                         raise exceptions.ZenodoError(
                             message=f"Error accessing latest draft for DOI {target_deposit.doi}."
                         )
                     draft_url = data["links"]["latest_draft"]
 
                 # Grab the draft
                 r = requests.get(
@@ -1092,15 +1077,14 @@
                 headers={"Content-Type": "application/json"},
             )
         )
 
         # Upload files
         logger.info(f"Uploading files to {target_deposit.doi}...")
         for file in cache_folder.glob("*"):
-
             if file.name == ".metadata.json":
                 continue
 
             try:
                 res = subprocess.run(
                     [
                         "curl",
@@ -1112,13 +1096,13 @@
                         file.name,
                         "--request",
                         "PUT",
                         f"{bucket_url}/{file.name}?access_token={target_deposit.access_token}",
                     ],
                     cwd=cache_folder,
                 )
-            except:
+            except Exception:
                 raise exceptions.ZenodoUploadError()
 
         # We're done
         logger.info(f"Successfully copied {self.doi} to {target_deposit.doi}.")
         return target_deposit.doi
```

### Comparing `showyourwork-0.4.2rc2/showyourwork.egg-info/PKG-INFO` & `showyourwork-0.4.3rc2/showyourwork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showyourwork
-Version: 0.4.2rc2
+Version: 0.4.3rc2
 Summary: A workflow for open-source scientific articles
 Home-page: https://github.com/showyourwork/showyourwork
 Author: Rodrigo Luger
 Author-email: rodluger@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: showyourwork Version: 0.4.2rc2 Summary: A workflow
+Metadata-Version: 2.1 Name: showyourwork Version: 0.4.3rc2 Summary: A workflow
 for open-source scientific articles Home-page: https://github.com/showyourwork/
 showyourwork Author: Rodrigo Luger Author-email: rodluger@gmail.com License:
 MIT Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
 Extra: tests License-File: LICENSE
                                 [showyourwork]
   [unit_tests] [local_integration_tests] [remote_integration_tests] [tests]
                            [sample_projects] [pypi]
```

### Comparing `showyourwork-0.4.2rc2/showyourwork.egg-info/SOURCES.txt` & `showyourwork-0.4.3rc2/showyourwork.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 docs/Makefile
 docs/api.rst
 docs/attribution.rst
 docs/changelog.rst
 docs/cli.rst
 docs/conf.py
 docs/config.rst
+docs/contributorguide.rst
 docs/environment.yml
 docs/faqs.rst
 docs/hacks.py
 docs/index.rst
 docs/install.rst
 docs/integration_tests.rst
 docs/intro.rst
@@ -51,15 +52,14 @@
 showyourwork/git.py
 showyourwork/gitapi.py
 showyourwork/logging.py
 showyourwork/overleaf.py
 showyourwork/patches.py
 showyourwork/paths.py
 showyourwork/subproc.py
-showyourwork/tex.py
 showyourwork/userrules.py
 showyourwork/zenodo.py
 showyourwork.egg-info/PKG-INFO
 showyourwork.egg-info/SOURCES.txt
 showyourwork.egg-info/dependency_links.txt
 showyourwork.egg-info/entry_points.txt
 showyourwork.egg-info/not-zip-safe
@@ -107,40 +107,40 @@
 showyourwork/exceptions/github.py
 showyourwork/exceptions/latex.py
 showyourwork/exceptions/other.py
 showyourwork/exceptions/overleaf.py
 showyourwork/exceptions/zenodo.py
 showyourwork/workflow/build.smk
 showyourwork/workflow/prep.smk
-showyourwork/workflow/envs/environment.yml
+showyourwork/workflow/envs/render_dag.yml
+showyourwork/workflow/envs/tectonic.yml
 showyourwork/workflow/report/preprocess.rst
 showyourwork/workflow/report/workflow.rst
 showyourwork/workflow/resources/img/article-thumb.png
 showyourwork/workflow/resources/styles/build.tex
 showyourwork/workflow/resources/styles/preprocess.tex
 showyourwork/workflow/resources/tex/lineno.sty
 showyourwork/workflow/resources/tex/listofitems.tex
 showyourwork/workflow/resources/tex/showyourwork-logo.pdf
 showyourwork/workflow/resources/tex/showyourwork-stamp.pdf
 showyourwork/workflow/resources/tex/showyourwork.otf
 showyourwork/workflow/resources/tex/xstring.sty
 showyourwork/workflow/resources/tex/xstring.tex
 showyourwork/workflow/rules/arxiv.smk
+showyourwork/workflow/rules/common.smk
 showyourwork/workflow/rules/compile.smk
-showyourwork/workflow/rules/conda.smk
 showyourwork/workflow/rules/dag.smk
 showyourwork/workflow/rules/figure.smk
 showyourwork/workflow/rules/preprocess.smk
 showyourwork/workflow/rules/render_dag.smk
 showyourwork/workflow/rules/zenodo.smk
 showyourwork/workflow/scripts/arxiv.py
-showyourwork/workflow/scripts/conda.py
+showyourwork/workflow/scripts/compile_setup.py
 showyourwork/workflow/scripts/download.py
 showyourwork/workflow/scripts/extract.py
-showyourwork/workflow/scripts/pdf.py
 showyourwork/workflow/scripts/preprocess.py
 showyourwork/workflow/scripts/render_dag.py
 tests/integration/conftest.py
 tests/integration/test_cache.py
 tests/integration/test_cache_optim.py
 tests/integration/test_default.py
 tests/integration/test_duplicate_graphics.py
@@ -151,8 +151,8 @@
 tests/integration/test_pr.py
 tests/integration/test_space_in_path.py
 tests/integration/test_variable.py
 tests/integration/test_zenodo.py
 tests/integration/helpers/__init__.py
 tests/integration/helpers/temp_repo.py
 tests/integration/sandbox/.gitignore
-tests/unit/test_placeholder.py
+tests/unit/test_overleaf_regex.py
```

### Comparing `showyourwork-0.4.2rc2/tests/integration/conftest.py` & `showyourwork-0.4.3rc2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/tests/integration/helpers/temp_repo.py` & `showyourwork-0.4.3rc2/tests/integration/helpers/temp_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     def cwd(self):
         return self.root_path / self.repo
 
     def startup(self):
         """Subclass me to run things at startup."""
         pass
 
-    def teardown(self):
-        """Subclass me to run things at teardown."""
+    def finish(self):
+        """Subclass me to run things after finishing."""
         pass
 
     def customize(self):
         """Subclass me to customize the repo."""
         pass
 
     def check_build(self):
@@ -211,15 +211,19 @@
         print(
             f"[{self.repo}] Waiting {self.action_wait} seconds for workflow "
             f"to finish (1/{self.action_max_tries})..."
         )
         await asyncio.sleep(self.action_wait)
         status = "unknown"
         for n in range(self.action_max_tries):
-            (status, conclusion, url,) = gitapi.get_workflow_run_status(
+            (
+                status,
+                conclusion,
+                url,
+            ) = gitapi.get_workflow_run_status(
                 self.repo,
                 org="showyourwork",
                 q={"event": "push", "head_sha": head_sha},
             )
             if status == "completed":
                 if conclusion == "success":
                     print(f"[{self.repo}] Workflow completed successfully.")
@@ -277,15 +281,14 @@
         """
         Test functionality by creating a new repo, customizing it,
         pushing it to GitHub, and awaiting the article build action to
         complete.
 
         """
         try:
-
             # Disable screen logging info from showyourwork
             self.disable_logging()
 
             # Always run this first
             self.startup()
 
             # Set up the repo
@@ -303,35 +306,33 @@
             # Run local checks
             self.check_build()
 
             # Delete local repo (only on success)
             self.delete_local()
 
         finally:
-
             # Always delete the Zenodo deposit (if created)
             self.delete_zenodo()
 
             # Always run this last
-            self.teardown()
+            self.finish()
 
     @pytest.mark.remote
     @pytest.mark.asyncio_cooperative
     async def test_remote(self):
         """
         Test functionality by creating a new repo, customizing it,
         pushing it to GitHub, and awaiting the article build action to
         complete.
 
         """
         if self.local_build_only:
             return
 
         try:
-
             # Disable screen logging info from showyourwork
             self.disable_logging()
 
             # Always run this first
             self.startup()
 
             # Create the repo on GitHub
@@ -361,20 +362,19 @@
             if self.delete_remote_on_success:
                 self.delete_remote()
 
             # Delete local repo (only on success)
             self.delete_local()
 
         finally:
-
             # Always delete the Zenodo deposit (if created)
             self.delete_zenodo()
 
             # Always run this last
-            self.teardown()
+            self.finish()
 
 
 class ShowyourworkRepositoryActions:
     def add_figure_environment(self, add_script=True, label="fig:test_figure"):
         """Adds a figure environment to the TeX file that includes `test_figure.pdf`."""
         ms = self.cwd / "src" / "tex" / "ms.tex"
         with open(ms, "r") as f:
```

### Comparing `showyourwork-0.4.2rc2/tests/integration/test_cache.py` & `showyourwork-0.4.3rc2/tests/integration/test_cache.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/tests/integration/test_cache_optim.py` & `showyourwork-0.4.3rc2/tests/integration/test_cache_optim.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/tests/integration/test_latex.py` & `showyourwork-0.4.3rc2/tests/integration/test_latex.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/tests/integration/test_letter.py` & `showyourwork-0.4.3rc2/tests/integration/test_letter.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/tests/integration/test_missing_inputs.py` & `showyourwork-0.4.3rc2/tests/integration/test_missing_inputs.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/tests/integration/test_overleaf.py` & `showyourwork-0.4.3rc2/tests/integration/test_overleaf.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 class TestOverleaf(
     TemporaryShowyourworkRepository, ShowyourworkRepositoryActions
 ):
     """Test a repo that integrates with an Overleaf project."""
 
     # No need to test this on CI
     local_build_only = True
-    overleaf_id = "6262c032aae5421d6d945acf"
+    overleaf_id = "6409f16f438b5fb7c4dfa837"
 
-    # Overeleaf rate limit error re-try settings
+    # Overleaf rate limit error re-try settings
     auth_retries = 1
     auth_sleep = 60
 
     def startup(self):
         """Wipe the Overleaf remote to start fresh."""
         for n in range(self.auth_retries):
             try:
                 overleaf.wipe_remote(self.overleaf_id)
             except exceptions.OverleafRateLimitExceeded:
                 get_logger().warn(
-                    f"Overleaf authentication failed. Re-trying in {self.auth_sleep} seconds..."
+                    "Overleaf authentication failed. "
+                    f"Re-trying in {self.auth_sleep} seconds..."
                 )
                 time.sleep(self.auth_sleep)
             else:
                 break
 
     def customize(self):
         """Customize the build to test all Overleaf functionality."""
@@ -59,15 +60,16 @@
                 overleaf.push_files(
                     [self.cwd / "src" / "tex" / "ms.tex"],
                     self.overleaf_id,
                     path=self.cwd,
                 )
             except exceptions.OverleafRateLimitExceeded:
                 get_logger().warn(
-                    f"Overleaf authentication failed. Re-trying in {self.auth_sleep} seconds..."
+                    "Overleaf authentication failed. "
+                    f"Re-trying in {self.auth_sleep} seconds..."
                 )
                 time.sleep(self.auth_sleep)
             else:
                 break
 
         get_stdout("git checkout -- src/tex/ms.tex", shell=True, cwd=self.cwd)
 
@@ -101,15 +103,16 @@
                     [figure],
                     self.overleaf_id,
                     path=self.cwd,
                     error_if_missing=True,
                 )
             except exceptions.OverleafRateLimitExceeded:
                 get_logger().warn(
-                    f"Overleaf authentication failed. Re-trying in {self.auth_sleep} seconds..."
+                    "Overleaf authentication failed. "
+                    f"Re-trying in {self.auth_sleep} seconds..."
                 )
                 time.sleep(self.auth_sleep)
             else:
                 break
 
         # Check that an exception is raised if we try to overwrite a file
         # with uncommitted changes
@@ -124,18 +127,19 @@
                     [ms],
                     self.overleaf_id,
                     path=self.cwd,
                     error_if_local_changes=True,
                 )
             except exceptions.OverleafRateLimitExceeded:
                 get_logger().warn(
-                    f"Overleaf authentication failed. Re-trying in {self.auth_sleep} seconds..."
+                    f"Overleaf authentication failed. "
+                    f"Re-trying in {self.auth_sleep} seconds..."
                 )
                 time.sleep(self.auth_sleep)
-            except exceptions.OverleafError as e:
+            except exceptions.OverleafError:
                 break
             else:
                 raise Exception("Failed to raise exception!")
 
         # Commit the changes and check that the exception is still raised
         get_stdout(
             f"git add -f {ms} && git commit -m 'changing ms.tex locally'",
@@ -148,37 +152,39 @@
                     [ms],
                     self.overleaf_id,
                     path=self.cwd,
                     error_if_local_changes=True,
                 )
             except exceptions.OverleafRateLimitExceeded:
                 get_logger().warn(
-                    f"Overleaf authentication failed. Re-trying in {self.auth_sleep} seconds..."
+                    "Overleaf authentication failed. "
+                    f"Re-trying in {self.auth_sleep} seconds..."
                 )
                 time.sleep(self.auth_sleep)
-            except exceptions.OverleafError as e:
+            except exceptions.OverleafError:
                 break
             else:
                 raise Exception("Failed to raise exception!")
 
         # Amend the commit message with the magical `[showyourwork]` label
         # and check that the merge works
         get_stdout(
-            f"git commit --amend -m '[showyourwork] changing ms.tex locally'",
+            "git commit --amend -m '[showyourwork] changing ms.tex locally'",
             cwd=self.cwd,
             shell=True,
         )
         for n in range(self.auth_retries):
             try:
                 overleaf.pull_files(
                     [ms],
                     self.overleaf_id,
                     path=self.cwd,
                     error_if_local_changes=True,
                 )
             except exceptions.OverleafRateLimitExceeded:
                 get_logger().warn(
-                    f"Overleaf authentication failed. Re-trying in {self.auth_sleep} seconds..."
+                    "Overleaf authentication failed. "
+                    f"Re-trying in {self.auth_sleep} seconds..."
                 )
                 time.sleep(self.auth_sleep)
             else:
                 break
```

### Comparing `showyourwork-0.4.2rc2/tests/integration/test_pr.py` & `showyourwork-0.4.3rc2/tests/integration/test_pr.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,19 +106,22 @@
         print(
             f"[{self.repo}] Waiting {self.action_wait} seconds for PR workflow "
             f"to finish (1/{self.action_max_tries})..."
         )
         await asyncio.sleep(self.action_wait)
         status = "unknown"
         for n in range(self.action_max_tries):
-
             # Note that we're querying `workflow_run` actions, specifically
             # to catch the `process-pull-request` action and check that the bot
             # has posted a comment to the PR with the link to the PDF and the diff.
-            (status, conclusion, url,) = gitapi.get_workflow_run_status(
+            (
+                status,
+                conclusion,
+                url,
+            ) = gitapi.get_workflow_run_status(
                 self.repo,
                 org="showyourwork",
                 q={
                     "event": "workflow_run",
                     "head_sha": head_sha,
                 },
             )
@@ -158,15 +161,15 @@
         for comment in data:
             if comment["user"]["login"] == "github-actions[bot]":
                 comment = comment["body"]
                 try:
                     diff_url = re.search(
                         r"\[PDF with highlighted changes\]\((.*?)\)", comment
                     ).groups()[0]
-                except:
+                except Exception:
                     raise Exception(
                         "Bot did not post the link to the PDF diff."
                     )
                 else:
                     break
         else:
             raise Exception("Cannot find bot comment on PR.")
```

### Comparing `showyourwork-0.4.2rc2/tests/integration/test_variable.py` & `showyourwork-0.4.3rc2/tests/integration/test_variable.py`

 * *Files identical despite different names*

### Comparing `showyourwork-0.4.2rc2/tests/integration/test_zenodo.py` & `showyourwork-0.4.3rc2/tests/integration/test_zenodo.py`

 * *Files identical despite different names*

