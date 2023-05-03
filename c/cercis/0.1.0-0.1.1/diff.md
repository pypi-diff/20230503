# Comparing `tmp/cercis-0.1.0.tar.gz` & `tmp/cercis-0.1.1.tar.gz`

## Comparing `cercis-0.1.0.tar` & `cercis-0.1.1.tar`

### file list

```diff
@@ -1,286 +1,291 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.0/.coveragerc
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.0/.flake8
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.0/.gitattributes
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 cercis-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.0/.prettierrc.yaml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.0/CHANGES.md
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 cercis-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.0/Dockerfile
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 cercis-0.1.0/README.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cercis-0.1.0/SECURITY.md
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cercis-0.1.0/action.yml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.0/mypy.ini
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.0/test_requirements.txt
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.0/tox.ini
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/ISSUE_TEMPLATE/docs-issue.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/ISSUE_TEMPLATE/style_issue.md
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/workflows/fuzz.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/workflows/pypi_upload.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.0/.github/workflows/upload_binary.yml
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 cercis-0.1.0/action/main.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.0/autoload/black.vim
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.0/gallery/Dockerfile
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.0/gallery/README.md
--rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.0/gallery/gallery.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.0/plugin/black.vim
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/scripts/__init__.py
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.0/scripts/diff_shades_gha_helper.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.0/scripts/fuzz.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.0/scripts/make_width_table.py
--rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.0/scripts/migrate-black.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.0/src/_cercis_version.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blackd/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blackd/__main__.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blackd/middlewares.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/Grammar.txt
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/PatternGrammar.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/README
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/__init__.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pygram.py
--rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pytree.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pgen2/__init__.py
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pgen2/conv.py
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pgen2/driver.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pgen2/grammar.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pgen2/literals.py
--rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pgen2/parse.py
--rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pgen2/pgen.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pgen2/token.py
--rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 cercis-0.1.0/src/blib2to3/pgen2/tokenize.py
--rw-r--r--   0        0        0    47356 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/__main__.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/_width_table.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/brackets.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/cache.py
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/comments.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/concurrency.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/const.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/debug.py
--rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/files.py
--rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/handle_ipynb_magics.py
--rw-r--r--   0        0        0    60901 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/linegen.py
--rw-r--r--   0        0        0    36582 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/lines.py
--rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/mode.py
--rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/nodes.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/numerics.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/output.py
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/py.typed
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/report.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/rusty.py
--rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/strings.py
--rw-r--r--   0        0        0    91407 2020-02-02 00:00:00.000000 cercis-0.1.0/src/cercis/trans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/empty.toml
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/optional.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/test.toml
--rw-r--r--   0        0        0   100658 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/test_black.py
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/test_blackd.py
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/test_format.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/test_ipynb.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/test_no_ipynb.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/test_trans.py
--rw-r--r--   0        0        0     6959 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/util.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/conditional_expression.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/empty_pyproject.toml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/configurable_cases/func_def_extra_indent.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/configurable_cases/func_def_no_extra_indent.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/fast/pep_572_do_not_remove_parens.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/gitignore_used_on_multiple_sources/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/ignore_subfolders_gitignore_tests/a.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/.gitignore
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/b/dont_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/b/dont_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/b/exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/b/exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/include_exclude_tests/b/exclude/a.pyi
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/invalid_gitignore_tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/invalid_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/invalid_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/invalid_nested_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/invalid_nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/invalid_nested_gitignore_tests/a/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/invalid_nested_gitignore_tests/a/a.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/jupyter/non_python_notebook.ipynb
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/jupyter/notebook_empty_metadata.ipynb
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/jupyter/notebook_no_trailing_newline.ipynb
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/jupyter/notebook_trailing_newline.ipynb
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/jupyter/notebook_without_changes.ipynb
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/async_as_identifier.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/blackd_diff.diff
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/blackd_diff.py
--rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/debug_visitor.out
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/debug_visitor.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/decorators.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/docstring_no_string_normalization.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/force_py36.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/force_pyi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/invalid_header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/linelength6.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/long_strings_flag_disabled.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/missing_final_newline.diff
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/missing_final_newline.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/nested_class_stub.pyi
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/pattern_matching_invalid.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/power_op_newline.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/python2_detection.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/string_quotes.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/miscellaneous/stub.pyi
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/x.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/root/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/root/a.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/root/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/root/c.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/root/child/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/root/child/a.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/root/child/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/nested_gitignore_tests/root/child/c.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/async_stmts.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/cantfit.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/comments7.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/format_unicode_escape_seq.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/long_dict_values.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/long_strings.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/long_strings__east_asian_width.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/long_strings__edge_case.py
--rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/long_strings__regression.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/long_strings__type_annotations.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/multiline_strings.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/percent_precedence.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/prefer_rhs_split.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/return_annotation_brackets_string.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview/trailing_comma.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview_context_managers/targeting_py38.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview_context_managers/targeting_py39.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview_context_managers/auto_detect/features_3_10.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview_context_managers/auto_detect/features_3_11.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview_context_managers/auto_detect/features_3_8.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/preview_context_managers/auto_detect/features_3_9.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/project_metadata/both_pyproject.toml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/project_metadata/neither_pyproject.toml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/project_metadata/only_black_pyproject.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/project_metadata/only_metadata_pyproject.toml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_310/parenthesized_context_managers.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_310/pattern_matching_complex.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_310/pattern_matching_extras.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_310/pattern_matching_generic.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_310/pattern_matching_simple.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_310/pattern_matching_style.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_310/pep_572_py310.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_310/remove_newline_after_match.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_310/starred_for_target.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_311/pep_646.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_311/pep_654.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_311/pep_654_style.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_36/numeric_literals.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_36/numeric_literals_skip_underscores.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_37/python37.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_38/pep_570.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_38/pep_572.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_38/pep_572_remove_parens.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_38/python38.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_39/pep_572_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_39/python39.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/py_39/remove_with_brackets.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/attribute_access_on_number_literals.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/beginning_backslash.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/bracketmatch.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/class_blank_parentheses.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/class_methods_new_line.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/collections.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comment_after_escaped_newline.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comments.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comments2.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comments3.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comments4.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comments5.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comments6.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comments8.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comments9.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/comments_non_breaking_space.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/composition.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/composition_no_trailing_comma.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/docstring_preview.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/empty_lines.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/expression.diff
--rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/expression.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtonoff.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtonoff2.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtonoff3.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtonoff4.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtonoff5.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtpass_imports.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtskip.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtskip2.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtskip3.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtskip4.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtskip5.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtskip6.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtskip7.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fmtskip8.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/fstring.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/function.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/function2.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/function_trailing_comma.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/import_spacing.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/one_element_subscript.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/power_op_spacing.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/prefer_rhs_split_reformatted.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/remove_await_parens.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/remove_except_parens.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/remove_for_brackets.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/remove_newline_after_code_block_open.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/remove_parens.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/return_annotation_brackets.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/skip_magic_trailing_comma.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/slices.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/torture.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/trailing_comma_optional_parens1.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/trailing_comma_optional_parens2.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/trailing_comma_optional_parens3.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/trailing_commas_in_leading_parts.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/tricky_unicode_symbols.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/tupleassign.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/simple_cases/whitespace.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.0/tests/data/type_comments/type_comment_syntax_error.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.0/.gitignore
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 cercis-0.1.0/AUTHORS.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.0/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.0/LICENSE_ORIGINAL
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 cercis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 cercis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.1/.flake8
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.1/.gitattributes
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 cercis-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.1/.prettierrc.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 cercis-0.1.1/CHANGES.md
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 cercis-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.1/Dockerfile
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 cercis-0.1.1/README.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cercis-0.1.1/SECURITY.md
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cercis-0.1.1/action.yml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.1/mypy.ini
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.1/test_requirements.txt
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.1/tox.ini
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/docs-issue.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/style_issue.md
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/fuzz.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/upload_binary.yml
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 cercis-0.1.1/action/main.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.1/autoload/black.vim
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.1/gallery/Dockerfile
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.1/gallery/README.md
+-rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.1/gallery/gallery.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.1/plugin/black.vim
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/__init__.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/diff_shades_gha_helper.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/fuzz.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/make_width_table.py
+-rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/migrate-black.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.1/src/_cercis_version.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blackd/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blackd/__main__.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blackd/middlewares.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/Grammar.txt
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/PatternGrammar.txt
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/README
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/__init__.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pygram.py
+-rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pytree.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/__init__.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/conv.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/driver.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/grammar.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/literals.py
+-rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/parse.py
+-rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/pgen.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/token.py
+-rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/tokenize.py
+-rw-r--r--   0        0        0    47673 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/__main__.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/_width_table.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/brackets.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/cache.py
+-rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/comments.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/concurrency.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/const.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/debug.py
+-rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/files.py
+-rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/handle_ipynb_magics.py
+-rw-r--r--   0        0        0    61129 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/linegen.py
+-rw-r--r--   0        0        0    36582 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/lines.py
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/mode.py
+-rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/nodes.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/numerics.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/output.py
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/py.typed
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/report.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/rusty.py
+-rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/strings.py
+-rw-r--r--   0        0        0    91688 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/trans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/empty.toml
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/optional.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test.toml
+-rw-r--r--   0        0        0   100658 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_black.py
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_blackd.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_format.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_ipynb.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_no_ipynb.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_trans.py
+-rw-r--r--   0        0        0     6959 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/util.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/conditional_expression.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/empty_pyproject.toml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/func_def_extra_indent.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/func_def_no_extra_indent.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/docstring_preview.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/more_quotes.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/torture.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/fast/pep_572_do_not_remove_parens.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/ignore_subfolders_gitignore_tests/a.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/.gitignore
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/dont_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/exclude/a.pyi
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_gitignore_tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_nested_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_nested_gitignore_tests/a/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_nested_gitignore_tests/a/a.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/non_python_notebook.ipynb
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_empty_metadata.ipynb
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_no_trailing_newline.ipynb
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_trailing_newline.ipynb
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_without_changes.ipynb
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/async_as_identifier.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/blackd_diff.diff
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/blackd_diff.py
+-rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/debug_visitor.out
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/debug_visitor.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/decorators.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/docstring_no_string_normalization.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/force_py36.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/force_pyi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/invalid_header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/linelength6.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/long_strings_flag_disabled.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/missing_final_newline.diff
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/missing_final_newline.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/nested_class_stub.pyi
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/pattern_matching_invalid.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/power_op_newline.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/python2_detection.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/string_quotes.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/stub.pyi
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/x.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/a.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/child/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/child/a.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/child/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/child/c.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/async_stmts.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/cantfit.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/comments7.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/format_unicode_escape_seq.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_dict_values.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings__east_asian_width.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings__edge_case.py
+-rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings__regression.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings__type_annotations.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/multiline_strings.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/percent_precedence.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/prefer_rhs_split.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/return_annotation_brackets_string.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/trailing_comma.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/targeting_py38.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/targeting_py39.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_10.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_11.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_8.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_9.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/project_metadata/both_pyproject.toml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/project_metadata/neither_pyproject.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/project_metadata/only_black_pyproject.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/project_metadata/only_metadata_pyproject.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/parenthesized_context_managers.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_complex.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_extras.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_generic.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_simple.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_style.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pep_572_py310.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/remove_newline_after_match.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/starred_for_target.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_311/pep_646.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_311/pep_654.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_311/pep_654_style.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_36/numeric_literals.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_36/numeric_literals_skip_underscores.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_37/python37.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_38/pep_570.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_38/pep_572.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_38/pep_572_remove_parens.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_38/python38.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_39/pep_572_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_39/python39.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_39/remove_with_brackets.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/attribute_access_on_number_literals.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/beginning_backslash.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/bracketmatch.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/class_blank_parentheses.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/class_methods_new_line.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/collections.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comment_after_escaped_newline.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments2.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments3.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments4.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments5.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments6.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments8.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments9.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments_non_breaking_space.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/composition.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/composition_no_trailing_comma.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/docstring_preview.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/empty_lines.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/expression.diff
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/expression.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff2.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff3.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff4.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff5.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtpass_imports.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip2.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip3.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip4.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip5.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip6.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip7.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip8.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fstring.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/function.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/function2.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/function_trailing_comma.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/import_spacing.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/one_element_subscript.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/power_op_spacing.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/prefer_rhs_split_reformatted.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_await_parens.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_except_parens.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_for_brackets.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_newline_after_code_block_open.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_parens.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/return_annotation_brackets.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/skip_magic_trailing_comma.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/slices.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/torture.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens1.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens2.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens3.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/trailing_commas_in_leading_parts.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/tricky_unicode_symbols.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/tupleassign.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/whitespace.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/type_comments/type_comment_syntax_error.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.1/.gitignore
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 cercis-0.1.1/AUTHORS.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.1/LICENSE_ORIGINAL
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cercis-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 cercis-0.1.1/PKG-INFO
```

### Comparing `cercis-0.1.0/.pre-commit-config.yaml` & `cercis-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.pre-commit-hooks.yaml` & `cercis-0.1.1/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/CHANGES.md` & `cercis-0.1.1/CHANGES.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Change Log
 
+## [0.1.1] - 2023-05-03
+
+### Added
+- A configurable option: `single-quote`, for formatting code into single quotes
+### Full changelog
+- https://github.com/jsh9/cercis/compare/0.1.0...0.1.1
+
+
 ## [0.1.0] - 2023-04-30
 
 This is the initial version that branches away from Black (commit:
 [e712e4](https://github.com/psf/black/commit/e712e48e06420d9240ce95c81acfcf6f11d14c83))
-
 ### Changed
-
 - The default indentation within a function definition (when line wrap happens) is now 8
   spaces. (Black's default is 4, which is
   [not PEP8-compatible](https://github.com/psf/black/issues/1127))
 - Updated README, because `cercis` now branches away from Black
-
 ### Added
-
 - A configurable option (`function-definition-extra-indent`) is added instead of
   enforcing 8 spaces for everyone
```

### Comparing `cercis-0.1.0/Dockerfile` & `cercis-0.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/action.yml` & `cercis-0.1.1/action.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/mypy.ini` & `cercis-0.1.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tox.ini` & `cercis-0.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/CODE_OF_CONDUCT.md` & `cercis-0.1.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `cercis-0.1.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/dependabot.yml` & `cercis-0.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `cercis-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/ISSUE_TEMPLATE/config.yml` & `cercis-0.1.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/ISSUE_TEMPLATE/docs-issue.md` & `cercis-0.1.1/.github/ISSUE_TEMPLATE/docs-issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `cercis-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/ISSUE_TEMPLATE/style_issue.md` & `cercis-0.1.1/.github/ISSUE_TEMPLATE/style_issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/workflows/docker.yml` & `cercis-0.1.1/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/workflows/fuzz.yml` & `cercis-0.1.1/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/workflows/lint.yml` & `cercis-0.1.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/workflows/python-package.yml` & `cercis-0.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/workflows/python-publish.yml` & `cercis-0.1.1/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
 
 # This workflow uses actions that are not certified by GitHub.
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
-name: Upload Python Package
+name: Publish package to PyPI
 
 on:
   release:
     types: [published]
 
 permissions:
   contents: read
```

### Comparing `cercis-0.1.0/.github/workflows/test.yml` & `cercis-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/.github/workflows/upload_binary.yml` & `cercis-0.1.1/.github/workflows/upload_binary.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/action/main.py` & `cercis-0.1.1/action/main.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/autoload/black.vim` & `cercis-0.1.1/autoload/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/gallery/README.md` & `cercis-0.1.1/gallery/README.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/gallery/gallery.py` & `cercis-0.1.1/gallery/gallery.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/plugin/black.vim` & `cercis-0.1.1/plugin/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/scripts/diff_shades_gha_helper.py` & `cercis-0.1.1/scripts/diff_shades_gha_helper.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/scripts/fuzz.py` & `cercis-0.1.1/scripts/fuzz.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/scripts/make_width_table.py` & `cercis-0.1.1/scripts/make_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/scripts/migrate-black.py` & `cercis-0.1.1/scripts/migrate-black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blackd/__init__.py` & `cercis-0.1.1/src/blackd/__init__.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blackd/middlewares.py` & `cercis-0.1.1/src/blackd/middlewares.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/Grammar.txt` & `cercis-0.1.1/src/blib2to3/Grammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/LICENSE` & `cercis-0.1.1/src/blib2to3/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/PatternGrammar.txt` & `cercis-0.1.1/src/blib2to3/PatternGrammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/README` & `cercis-0.1.1/src/blib2to3/README`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pygram.py` & `cercis-0.1.1/src/blib2to3/pygram.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pytree.py` & `cercis-0.1.1/src/blib2to3/pytree.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pgen2/conv.py` & `cercis-0.1.1/src/blib2to3/pgen2/conv.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pgen2/driver.py` & `cercis-0.1.1/src/blib2to3/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pgen2/grammar.py` & `cercis-0.1.1/src/blib2to3/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pgen2/literals.py` & `cercis-0.1.1/src/blib2to3/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pgen2/parse.py` & `cercis-0.1.1/src/blib2to3/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pgen2/pgen.py` & `cercis-0.1.1/src/blib2to3/pgen2/pgen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pgen2/token.py` & `cercis-0.1.1/src/blib2to3/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/blib2to3/pgen2/tokenize.py` & `cercis-0.1.1/src/blib2to3/pgen2/tokenize.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/__init__.py` & `cercis-0.1.1/src/cercis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from cercis.cache import Cache, get_cache_info, read_cache, write_cache
 from cercis.comments import normalize_fmt_off
 from cercis.const import (
     DEFAULT_EXCLUDES,
     DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     DEFAULT_INCLUDES,
     DEFAULT_LINE_LENGTH,
+    DEFAULT_SINGLE_QUOTE,
     STDIN_PLACEHOLDER,
 )
 from cercis.files import (
     find_project_root,
     find_pyproject_toml,
     find_user_pyproject_toml,
     gen_python_files,
@@ -118,15 +119,15 @@
 # Legacy name, left for integrations.
 FileMode = Mode
 
 
 def read_pyproject_toml(
         ctx: click.Context, param: click.Parameter, value: Optional[str]
 ) -> Optional[str]:
-    """Inject Black configuration from "pyproject.toml" into defaults in `ctx`.
+    """Inject Cercis configuration from "pyproject.toml" into defaults in `ctx`.
 
     Returns the path to a successfully found and read configuration file, None
     otherwise.
     """
     if not value:
         value = find_pyproject_toml(ctx.params.get("src", ()))
         if value is None:
@@ -221,23 +222,32 @@
     default=DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     help=(
         "If True, use 8 spaces as indent in function definition;"
         " otherwise, use 8 (Black's default)."
     ),
 )
 @click.option(
+    "-sq",
+    "--single-quote",
+    type=bool,
+    show_default=True,
+    default=DEFAULT_SINGLE_QUOTE,
+    help="If True, format code using single quotes; otherwise use double quotes.",
+)
+@click.option(
     "-t",
     "--target-version",
     type=click.Choice([v.name.lower() for v in TargetVersion]),
     callback=target_version_option_callback,
     multiple=True,
     help=(
-        "Python versions that should be supported by Black's output. By default, Black"
-        " will try to infer this from the project metadata in pyproject.toml. If this"
-        " does not yield conclusive results, Black will use per-file auto-detection."
+        "Python versions that should be supported by Cercis's output. By default,"
+        " Cercis will try to infer this from the project metadata in pyproject.toml."
+        " If this does not yield conclusive results, Cercis will use per-file"
+        " auto-detection."
     ),
 )
 @click.option(
     "--pyi",
     is_flag=True,
     help=(
         "Format all input files like typing stubs regardless of file extension (useful"
@@ -286,16 +296,16 @@
     hidden=True,
     help="(DEPRECATED and now included in --preview) Normalize string literals.",
 )
 @click.option(
     "--preview",
     is_flag=True,
     help=(
-        "Enable potentially disruptive style changes that may be added to Black's main"
-        " functionality in the next major release."
+        "Enable potentially disruptive style changes that may be added to"
+        " Cercis's main functionality in the next major release."
     ),
 )
 @click.option(
     "--check",
     is_flag=True,
     help=(
         "Don't write the files back, just return the status. Return code 0 means"
@@ -318,17 +328,17 @@
     is_flag=True,
     help="If --fast given, skip temporary sanity checks. [default: --safe]",
 )
 @click.option(
     "--required-version",
     type=str,
     help=(
-        "Require a specific version of Black to be running (useful for unifying results"
-        " across many environments e.g. with a pyproject.toml file). It can be"
-        " either a major version number or an exact version."
+        "Require a specific version of Cercis to be running (useful for unifying"
+        " results across many environments e.g. with a pyproject.toml file). It"
+        " can be either a major version number or an exact version."
     ),
 )
 @click.option(
     "--include",
     type=str,
     default=DEFAULT_INCLUDES,
     callback=validate_regex,
@@ -372,15 +382,15 @@
     ),
 )
 @click.option(
     "--stdin-filename",
     type=str,
     help=(
         "The name of the file when passing it through stdin. Useful to make "
-        "sure Black will respect --force-exclude option on some "
+        "sure Cercis will respect --force-exclude option on some "
         "editors that rely on using stdin."
     ),
 )
 @click.option(
     "-W",
     "--workers",
     type=click.IntRange(min=1),
@@ -437,14 +447,15 @@
 )
 @click.pass_context
 def main(  # noqa: C901
         ctx: click.Context,
         code: Optional[str],
         line_length: int,
         function_definition_extra_indent: bool,
+        single_quote: bool,
         target_version: List[TargetVersion],
         check: bool,
         diff: bool,
         color: bool,
         fast: bool,
         pyi: bool,
         ipynb: bool,
@@ -560,14 +571,15 @@
         skip_source_first_line=skip_source_first_line,
         string_normalization=not skip_string_normalization,
         magic_trailing_comma=not skip_magic_trailing_comma,
         experimental_string_processing=experimental_string_processing,
         preview=preview,
         python_cell_magics=set(python_cell_magics),
         function_definition_extra_indent=function_definition_extra_indent,
+        single_quote=single_quote,
     )
 
     if code is not None:
         # Run in quiet mode by default with -c; the extra output isn't useful.
         # You can still pass -v to get verbose output.
         quiet = True
 
@@ -1356,34 +1368,34 @@
     """Raise AssertionError if `src` and `dst` aren't equivalent."""
     try:
         src_ast = parse_ast(src)
     except Exception as exc:
         raise AssertionError(
             "cannot use --safe with this file; failed to parse source file AST: "
             f"{exc}\n"
-            "This could be caused by running Black with an older Python version "
+            "This could be caused by running Cercis with an older Python version "
             "that does not support new syntax used in your source file."
         ) from exc
 
     try:
         dst_ast = parse_ast(dst)
     except Exception as exc:
         log = dump_to_file("".join(traceback.format_tb(exc.__traceback__)), dst)
         raise AssertionError(
-            f"INTERNAL ERROR: Black produced invalid code: {exc}. "
+            f"INTERNAL ERROR: Cercis produced invalid code: {exc}. "
             "Please report a bug on https://github.com/psf/black/issues.  "
             f"This invalid output might be helpful: {log}"
         ) from None
 
     src_ast_str = "\n".join(stringify_ast(src_ast))
     dst_ast_str = "\n".join(stringify_ast(dst_ast))
     if src_ast_str != dst_ast_str:
         log = dump_to_file(diff(src_ast_str, dst_ast_str, "src", "dst"))
         raise AssertionError(
-            "INTERNAL ERROR: Black produced code that is not equivalent to the"
+            "INTERNAL ERROR: Cercis produced code that is not equivalent to the"
             " source.  Please report a bug on "
             f"https://github.com/psf/black/issues.  This diff might be helpful: {log}"
         ) from None
 
 
 def assert_stable(src: str, dst: str, mode: Mode) -> None:
     """Raise AssertionError if `dst` reformats differently the second time."""
@@ -1394,15 +1406,15 @@
     if dst != newdst:
         log = dump_to_file(
             str(mode),
             diff(src, dst, "source", "first pass"),
             diff(dst, newdst, "first pass", "second pass"),
         )
         raise AssertionError(
-            "INTERNAL ERROR: Black produced different code on the second pass of the"
+            "INTERNAL ERROR: Cercis produced different code on the second pass of the"
             " formatter.  Please report a bug on https://github.com/psf/black/issues."
             f"  This diff might be helpful: {log}"
         ) from None
 
 
 @contextmanager
 def nullcontext() -> Iterator[None]:
@@ -1416,15 +1428,15 @@
 def patch_click() -> None:
     """Make Click not crash on Python 3.6 with LANG=C.
 
     On certain misconfigured environments, Python 3 selects the ASCII encoding as the
     default which restricts paths that it can access during the lifetime of the
     application.  Click refuses to work in this scenario by raising a RuntimeError.
 
-    In case of Black the likelihood that non-ASCII characters are going to be used in
+    In case of Cercis the likelihood that non-ASCII characters are going to be used in
     file paths is minimal since it's Python source code.  Moreover, this crash was
     spurious on Python 3.7 thanks to PEP 538 and PEP 540.
     """
     modules: List[Any] = []
     try:
         from click import core
     except ImportError:
```

### Comparing `cercis-0.1.0/src/cercis/_width_table.py` & `cercis-0.1.1/src/cercis/_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/brackets.py` & `cercis-0.1.1/src/cercis/brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/cache.py` & `cercis-0.1.1/src/cercis/cache.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/comments.py` & `cercis-0.1.1/src/cercis/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/concurrency.py` & `cercis-0.1.1/src/cercis/concurrency.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/debug.py` & `cercis-0.1.1/src/cercis/debug.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/files.py` & `cercis-0.1.1/src/cercis/files.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/handle_ipynb_magics.py` & `cercis-0.1.1/src/cercis/handle_ipynb_magics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/linegen.py` & `cercis-0.1.1/src/cercis/linegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,18 @@
 
                     self.current_line.append(comment)
                     yield from self.line()
 
             normalize_prefix(node, inside_brackets=any_open_brackets)
             if self.mode.string_normalization and node.type == token.STRING:
                 node.value = normalize_string_prefix(node.value)
-                node.value = normalize_string_quotes(node.value)
+                node.value = normalize_string_quotes(
+                    node.value,
+                    single_quote=self.mode.single_quote,
+                )
             if node.type == token.NUMBER:
                 normalize_numeric_literal(node)
             if node.type not in WHITESPACE:
                 self.current_line.append(node)
         yield from super().visit_default(node)
 
     def visit_test(self, node: Node) -> Iterator[Line]:
@@ -391,15 +394,18 @@
                 docstring = normalize_string_prefix(leaf.value)
                 # visit_default() does handle string normalization for us, but
                 # since this method acts differently depending on quote style (ex.
                 # see padding logic below), there's a possibility for unstable
                 # formatting as visit_default() is called *after*. To avoid a
                 # situation where this function formats a docstring differently on
                 # the second pass, normalize it early.
-                docstring = normalize_string_quotes(docstring)
+                docstring = normalize_string_quotes(
+                    docstring,
+                    single_quote=self.mode.single_quote,
+                )
             else:
                 docstring = leaf.value
             prefix = get_string_prefix(docstring)
             docstring = docstring[len(prefix) :]  # Remove the prefix
             quote_char = docstring[0]
             # A natural way to remove the outer quotes is to do:
             #   docstring = docstring.strip(quote_char)
@@ -506,17 +512,19 @@
         yield line
         return
 
     line_str = line_to_string(line)
 
     ll = mode.line_length
     sn = mode.string_normalization
-    string_merge = StringMerger(ll, sn)
+    sq = mode.single_quote
+
+    string_merge = StringMerger(ll, sn, sq)
     string_paren_strip = StringParenStripper(ll, sn)
-    string_split = StringSplitter(ll, sn)
+    string_split = StringSplitter(ll, sn, sq)
     string_paren_wrap = StringParenWrapper(ll, sn)
 
     transformers: List[Transformer]
     if (
         not line.contains_uncollapsable_type_comments()
         and not line.should_split_rhs
         and not line.magic_trailing_comma
```

### Comparing `cercis-0.1.0/src/cercis/lines.py` & `cercis-0.1.1/src/cercis/lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/mode.py` & `cercis-0.1.1/src/cercis/mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 from warnings import warn
 
 if sys.version_info < (3, 8):
     from typing_extensions import Final
 else:
     from typing import Final
 
-from cercis.const import DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT, DEFAULT_LINE_LENGTH
+from cercis.const import (
+    DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
+    DEFAULT_LINE_LENGTH,
+    DEFAULT_SINGLE_QUOTE,
+)
 
 
 class TargetVersion(Enum):
     PY33 = 3
     PY34 = 4
     PY35 = 5
     PY36 = 6
@@ -181,14 +185,15 @@
     is_ipynb: bool = False
     skip_source_first_line: bool = False
     magic_trailing_comma: bool = True
     experimental_string_processing: bool = False
     python_cell_magics: Set[str] = field(default_factory=set)
     preview: bool = False
     function_definition_extra_indent: bool = DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT
+    single_quote: bool = DEFAULT_SINGLE_QUOTE
 
     def __post_init__(self) -> None:
         if self.experimental_string_processing:
             warn(
                 "`experimental string processing` has been included in `preview`"
                 " and deprecated. Use `preview` instead.",
                 Deprecated,
```

### Comparing `cercis-0.1.0/src/cercis/nodes.py` & `cercis-0.1.1/src/cercis/nodes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/numerics.py` & `cercis-0.1.1/src/cercis/numerics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/output.py` & `cercis-0.1.1/src/cercis/output.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/parsing.py` & `cercis-0.1.1/src/cercis/parsing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/report.py` & `cercis-0.1.1/src/cercis/report.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/rusty.py` & `cercis-0.1.1/src/cercis/rusty.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/src/cercis/strings.py` & `cercis-0.1.1/src/cercis/strings.py`

 * *Files 24% similar despite different names*

```diff
@@ -172,15 +172,97 @@
 # performance on a long list literal of strings by 5-9% since lru_cache's
 # caching overhead is much lower.
 @lru_cache(maxsize=64)
 def _cached_compile(pattern: str) -> Pattern[str]:
     return re.compile(pattern)
 
 
-def normalize_string_quotes(s: str) -> str:
+def normalize_string_quotes(s: str, single_quote: bool = True) -> str:
+    return convert_to_single_quotes(s) if single_quote else convert_to_double_quotes(s)
+
+
+def convert_to_single_quotes(s: str) -> str:
+    """Prefer single quotes but only if it doesn't cause more escaping.
+
+    Adds or removes backslashes as appropriate. Doesn't parse and fix
+    strings nested in f-strings.
+
+    (This function has lots of duplicated code fragments with
+    `convert_to_double_quotes()` below; we may think about de-duplicating
+    them in the future.)
+    """
+    value = s.lstrip(STRING_PREFIX_CHARS)
+    if value[:3] == '"""':
+        return s
+
+    elif value[:3] == "'''":
+        orig_quote = "'''"
+        new_quote = '"""'
+    elif value[0] == "'":
+        orig_quote = "'"
+        new_quote = '"'
+    else:
+        orig_quote = '"'
+        new_quote = "'"
+    first_quote_pos = s.find(orig_quote)
+    if first_quote_pos == -1:
+        return s  # There's an internal error
+
+    prefix = s[:first_quote_pos]
+    unescaped_new_quote = _cached_compile(rf"(([^\\]|^)(\\\\)*){new_quote}")
+    escaped_new_quote = _cached_compile(rf"([^\\]|^)\\((?:\\\\)*){new_quote}")
+    escaped_orig_quote = _cached_compile(rf"([^\\]|^)\\((?:\\\\)*){orig_quote}")
+    body = s[first_quote_pos + len(orig_quote) : -len(orig_quote)]
+    if "r" in prefix.casefold():
+        if unescaped_new_quote.search(body):
+            # There's at least one unescaped new_quote in this raw string
+            # so converting is impossible
+            return s
+
+        # Do not introduce or remove backslashes in raw strings
+        new_body = body
+    else:
+        # remove unnecessary escapes
+        new_body = sub_twice(escaped_new_quote, rf"\1\2{new_quote}", body)
+        if body != new_body:
+            # Consider the string without unnecessary escapes as the original
+            body = new_body
+            s = f"{prefix}{orig_quote}{body}{orig_quote}"
+        new_body = sub_twice(escaped_orig_quote, rf"\1\2{orig_quote}", new_body)
+        new_body = sub_twice(unescaped_new_quote, rf"\1\\{new_quote}", new_body)
+    if "f" in prefix.casefold():
+        matches = re.findall(
+            r"""
+            (?:(?<!\{)|^)\{  # start of the string or a non-{ followed by a single {
+                ([^{].*?)  # contents of the brackets except if begins with {{
+            \}(?:(?!\})|$)  # A } followed by end of the string or a non-}
+            """,
+            new_body,
+            re.VERBOSE,
+        )
+        for m in matches:
+            if "\\" in str(m):
+                # Do not introduce backslashes in interpolated expressions
+                return s
+
+    if new_quote == "'''" and new_body[-1:] == "'":
+        # edge case:
+        new_body = new_body[:-1] + "\\'"
+    orig_escape_count = body.count("\\")
+    new_escape_count = new_body.count("\\")
+    if new_escape_count > orig_escape_count:
+        return s  # Do not introduce more escaping
+
+    if new_escape_count == orig_escape_count and orig_quote == "'":
+        return s  # Prefer double quotes
+
+    return f"{prefix}{new_quote}{new_body}{new_quote}"
+
+
+def convert_to_double_quotes(s: str) -> str:
     """Prefer double quotes but only if it doesn't cause more escaping.
 
     Adds or removes backslashes as appropriate. Doesn't parse and fix
     strings nested in f-strings.
     """
     value = s.lstrip(STRING_PREFIX_CHARS)
     if value[:3] == '"""':
```

### Comparing `cercis-0.1.0/src/cercis/trans.py` & `cercis-0.1.1/src/cercis/trans.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,17 +192,23 @@
         as much as possible.
     """
 
     __name__: Final = "StringTransformer"
 
     # Ideally this would be a dataclass, but unfortunately mypyc breaks when used with
     # `abc.ABC`.
-    def __init__(self, line_length: int, normalize_strings: bool) -> None:
+    def __init__(
+            self,
+            line_length: int,
+            normalize_strings: bool,
+            single_quote: bool = True,
+    ) -> None:
         self.line_length = line_length
         self.normalize_strings = normalize_strings
+        self.single_quote = single_quote
 
     @abstractmethod
     def do_match(self, line: Line) -> TMatchResult:
         """
         Returns:
             * Ok(string_indices) such that for each index, `line.leaves[index]`
             is our target string if a match was able to be made. For
@@ -649,15 +655,18 @@
             next_str_idx += 1
 
         # Take a note on the index of the non-STRING leaf.
         non_string_idx = next_str_idx
 
         S_leaf = Leaf(token.STRING, S)
         if self.normalize_strings:
-            S_leaf.value = normalize_string_quotes(S_leaf.value)
+            S_leaf.value = normalize_string_quotes(
+                S_leaf.value,
+                single_quote=self.single_quote,
+            )
 
         # Fill the 'custom_splits' list with the appropriate CustomSplit objects.
         temp_string = S_leaf.value[len(prefix) + 1 : -1]
         for has_prefix in prefix_tracker:
             mark_idx = temp_string.find(BREAK_MARK)
             assert (
                 mark_idx >= 0
@@ -1754,15 +1763,18 @@
             if not is_valid_index(break_idx) or not passes_all_checks(break_idx):
                 return None
 
         return break_idx
 
     def _maybe_normalize_string_quotes(self, leaf: Leaf) -> None:
         if self.normalize_strings:
-            leaf.value = normalize_string_quotes(leaf.value)
+            leaf.value = normalize_string_quotes(
+                leaf.value,
+                single_quote=self.single_quote,
+            )
 
     def _normalize_f_string(self, string: str, prefix: str) -> str:
         """
         Pre-Conditions:
             * assert_is_leaf_string(@string)
 
         Returns:
```

### Comparing `cercis-0.1.0/tests/optional.py` & `cercis-0.1.1/tests/optional.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/test_black.py` & `cercis-0.1.1/tests/test_black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/test_blackd.py` & `cercis-0.1.1/tests/test_blackd.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/test_format.py` & `cercis-0.1.1/tests/test_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,7 +211,17 @@
         ("func_def_extra_indent.py", True),
         ("func_def_no_extra_indent.py", False),
     ],
 )
 def test_function_definition_extra_indent(filename: str, extra_indent: bool) -> None:
     mode = replace(DEFAULT_MODE, function_definition_extra_indent=extra_indent)
     check_file("configurable_cases", filename, mode)
+
+
+@pytest.mark.filterwarnings("ignore:invalid escape sequence.*:DeprecationWarning")
+@pytest.mark.parametrize(
+    "filename",
+    all_data_cases("configurable_cases/single_quote"),
+)
+def test_single_quote(filename: str) -> None:
+    mode = replace(DEFAULT_MODE, single_quote=True)
+    check_file("configurable_cases/single_quote", filename, mode)
```

### Comparing `cercis-0.1.0/tests/test_ipynb.py` & `cercis-0.1.1/tests/test_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/test_no_ipynb.py` & `cercis-0.1.1/tests/test_no_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/test_trans.py` & `cercis-0.1.1/tests/test_trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/util.py` & `cercis-0.1.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/conditional_expression.py` & `cercis-0.1.1/tests/data/conditional_expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/jupyter/notebook_no_trailing_newline.ipynb` & `cercis-0.1.1/tests/data/jupyter/notebook_no_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/jupyter/notebook_trailing_newline.ipynb` & `cercis-0.1.1/tests/data/jupyter/notebook_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/jupyter/notebook_without_changes.ipynb` & `cercis-0.1.1/tests/data/jupyter/notebook_without_changes.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/debug_visitor.out` & `cercis-0.1.1/tests/data/miscellaneous/debug_visitor.out`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/debug_visitor.py` & `cercis-0.1.1/tests/data/miscellaneous/debug_visitor.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/decorators.py` & `cercis-0.1.1/tests/data/miscellaneous/decorators.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/docstring_no_string_normalization.py` & `cercis-0.1.1/tests/data/miscellaneous/docstring_no_string_normalization.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff` & `cercis-0.1.1/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/force_py36.py` & `cercis-0.1.1/tests/data/miscellaneous/force_py36.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/force_pyi.py` & `cercis-0.1.1/tests/data/miscellaneous/force_pyi.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/long_strings_flag_disabled.py` & `cercis-0.1.1/tests/data/miscellaneous/long_strings_flag_disabled.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/python2_detection.py` & `cercis-0.1.1/tests/data/miscellaneous/python2_detection.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/string_quotes.py` & `cercis-0.1.1/tests/data/miscellaneous/string_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/miscellaneous/stub.pyi` & `cercis-0.1.1/tests/data/miscellaneous/stub.pyi`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/cantfit.py` & `cercis-0.1.1/tests/data/preview/cantfit.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/comments7.py` & `cercis-0.1.1/tests/data/preview/comments7.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/format_unicode_escape_seq.py` & `cercis-0.1.1/tests/data/preview/format_unicode_escape_seq.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/long_dict_values.py` & `cercis-0.1.1/tests/data/preview/long_dict_values.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/long_strings.py` & `cercis-0.1.1/tests/data/preview/long_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/long_strings__east_asian_width.py` & `cercis-0.1.1/tests/data/preview/long_strings__east_asian_width.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/long_strings__edge_case.py` & `cercis-0.1.1/tests/data/preview/long_strings__edge_case.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/long_strings__regression.py` & `cercis-0.1.1/tests/data/preview/long_strings__regression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/long_strings__type_annotations.py` & `cercis-0.1.1/tests/data/preview/long_strings__type_annotations.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/multiline_strings.py` & `cercis-0.1.1/tests/data/preview/multiline_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/prefer_rhs_split.py` & `cercis-0.1.1/tests/data/preview/prefer_rhs_split.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview/trailing_comma.py` & `cercis-0.1.1/tests/data/preview/trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview_context_managers/targeting_py38.py` & `cercis-0.1.1/tests/data/preview_context_managers/targeting_py38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview_context_managers/targeting_py39.py` & `cercis-0.1.1/tests/data/preview_context_managers/targeting_py39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview_context_managers/auto_detect/features_3_10.py` & `cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_10.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview_context_managers/auto_detect/features_3_11.py` & `cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_11.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview_context_managers/auto_detect/features_3_8.py` & `cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/preview_context_managers/auto_detect/features_3_9.py` & `cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_310/parenthesized_context_managers.py` & `cercis-0.1.1/tests/data/py_310/parenthesized_context_managers.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_310/pattern_matching_complex.py` & `cercis-0.1.1/tests/data/py_310/pattern_matching_complex.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_310/pattern_matching_extras.py` & `cercis-0.1.1/tests/data/py_310/pattern_matching_extras.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_310/pattern_matching_generic.py` & `cercis-0.1.1/tests/data/py_310/pattern_matching_generic.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_310/pattern_matching_simple.py` & `cercis-0.1.1/tests/data/py_310/pattern_matching_simple.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_310/pattern_matching_style.py` & `cercis-0.1.1/tests/data/py_310/pattern_matching_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_311/pep_646.py` & `cercis-0.1.1/tests/data/py_311/pep_646.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_311/pep_654.py` & `cercis-0.1.1/tests/data/py_311/pep_654.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_311/pep_654_style.py` & `cercis-0.1.1/tests/data/py_311/pep_654_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_36/numeric_literals.py` & `cercis-0.1.1/tests/data/py_36/numeric_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_37/python37.py` & `cercis-0.1.1/tests/data/py_37/python37.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_38/pep_570.py` & `cercis-0.1.1/tests/data/py_38/pep_570.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_38/pep_572.py` & `cercis-0.1.1/tests/data/py_38/pep_572.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_38/pep_572_remove_parens.py` & `cercis-0.1.1/tests/data/py_38/pep_572_remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_38/python38.py` & `cercis-0.1.1/tests/data/py_38/python38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_39/python39.py` & `cercis-0.1.1/tests/data/py_39/python39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/py_39/remove_with_brackets.py` & `cercis-0.1.1/tests/data/py_39/remove_with_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/attribute_access_on_number_literals.py` & `cercis-0.1.1/tests/data/simple_cases/attribute_access_on_number_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/class_blank_parentheses.py` & `cercis-0.1.1/tests/data/simple_cases/class_blank_parentheses.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/class_methods_new_line.py` & `cercis-0.1.1/tests/data/simple_cases/class_methods_new_line.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/collections.py` & `cercis-0.1.1/tests/data/simple_cases/collections.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/comments.py` & `cercis-0.1.1/tests/data/simple_cases/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/comments2.py` & `cercis-0.1.1/tests/data/simple_cases/comments2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/comments3.py` & `cercis-0.1.1/tests/data/simple_cases/comments3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/comments4.py` & `cercis-0.1.1/tests/data/simple_cases/comments4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/comments5.py` & `cercis-0.1.1/tests/data/simple_cases/comments5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/comments6.py` & `cercis-0.1.1/tests/data/simple_cases/comments6.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/comments9.py` & `cercis-0.1.1/tests/data/simple_cases/comments9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/comments_non_breaking_space.py` & `cercis-0.1.1/tests/data/simple_cases/comments_non_breaking_space.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/composition.py` & `cercis-0.1.1/tests/data/simple_cases/composition.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/composition_no_trailing_comma.py` & `cercis-0.1.1/tests/data/simple_cases/composition_no_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/docstring.py` & `cercis-0.1.1/tests/data/simple_cases/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/docstring_preview.py` & `cercis-0.1.1/tests/data/simple_cases/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/empty_lines.py` & `cercis-0.1.1/tests/data/simple_cases/empty_lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/expression.diff` & `cercis-0.1.1/tests/data/simple_cases/expression.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/expression.py` & `cercis-0.1.1/tests/data/simple_cases/expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/fmtonoff.py` & `cercis-0.1.1/tests/data/simple_cases/fmtonoff.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/fmtonoff2.py` & `cercis-0.1.1/tests/data/simple_cases/fmtonoff2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/fmtonoff5.py` & `cercis-0.1.1/tests/data/simple_cases/fmtonoff5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/fmtskip2.py` & `cercis-0.1.1/tests/data/simple_cases/fmtskip2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/fmtskip8.py` & `cercis-0.1.1/tests/data/simple_cases/fmtskip8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/fstring.py` & `cercis-0.1.1/tests/data/simple_cases/fstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/function.py` & `cercis-0.1.1/tests/data/simple_cases/function.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/function2.py` & `cercis-0.1.1/tests/data/simple_cases/function2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/function_trailing_comma.py` & `cercis-0.1.1/tests/data/simple_cases/function_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/import_spacing.py` & `cercis-0.1.1/tests/data/simple_cases/import_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/one_element_subscript.py` & `cercis-0.1.1/tests/data/simple_cases/one_element_subscript.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/power_op_spacing.py` & `cercis-0.1.1/tests/data/simple_cases/power_op_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/prefer_rhs_split_reformatted.py` & `cercis-0.1.1/tests/data/simple_cases/prefer_rhs_split_reformatted.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/remove_await_parens.py` & `cercis-0.1.1/tests/data/simple_cases/remove_await_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/remove_except_parens.py` & `cercis-0.1.1/tests/data/simple_cases/remove_except_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/remove_for_brackets.py` & `cercis-0.1.1/tests/data/simple_cases/remove_for_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/remove_newline_after_code_block_open.py` & `cercis-0.1.1/tests/data/simple_cases/remove_newline_after_code_block_open.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/remove_parens.py` & `cercis-0.1.1/tests/data/simple_cases/remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/return_annotation_brackets.py` & `cercis-0.1.1/tests/data/simple_cases/return_annotation_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/skip_magic_trailing_comma.py` & `cercis-0.1.1/tests/data/simple_cases/skip_magic_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/slices.py` & `cercis-0.1.1/tests/data/simple_cases/slices.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/string_prefixes.py` & `cercis-0.1.1/tests/data/simple_cases/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/torture.py` & `cercis-0.1.1/tests/data/simple_cases/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/trailing_comma_optional_parens1.py` & `cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/trailing_comma_optional_parens3.py` & `cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/tests/data/simple_cases/trailing_commas_in_leading_parts.py` & `cercis-0.1.1/tests/data/simple_cases/trailing_commas_in_leading_parts.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/AUTHORS.md` & `cercis-0.1.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/LICENSE` & `cercis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/LICENSE_ORIGINAL` & `cercis-0.1.1/LICENSE_ORIGINAL`

 * *Files identical despite different names*

### Comparing `cercis-0.1.0/pyproject.toml` & `cercis-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.cercis]
 line-length = 88
 function-definition-extra-indent = true
+single-quote = false
 target-version = ['py37', 'py38']
 include = '\.pyi?$'
 extend-exclude = '''
 /(
   # The following are specific to Black, you probably don't want those.
   | blib2to3
   | tests/data
@@ -28,15 +29,15 @@
 
 [build-system]
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cercis"
-version = "0.1.0"
+version = "0.1.1"
 description = "A more configurable Python code formatter"
 license = { text = "MIT" }
 requires-python = ">=3.7"
 authors = [
   { name = "Łukasz Langa", email = "lukasz@langa.pl" },
   { name = "jsh9", email = "" },
 ]
```

