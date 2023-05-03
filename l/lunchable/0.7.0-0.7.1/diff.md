# Comparing `tmp/lunchable-0.7.0.tar.gz` & `tmp/lunchable-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunchable-0.7.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `lunchable-0.7.0.tar` & `lunchable-0.7.1.tar`

### file list

```diff
@@ -1,43 +1,136 @@
--rw-r--r--   0        0        0     1071 2023-04-23 04:32:09.089263 lunchable-0.7.0/LICENSE
--rw-r--r--   0        0        0     2215 2023-04-23 04:32:09.089263 lunchable-0.7.0/README.md
--rw-r--r--   0        0        0      537 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/__init__.py
--rw-r--r--   0        0        0       98 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/__main__.py
--rw-r--r--   0        0        0    13208 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_cli.py
--rw-r--r--   0        0        0      160 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_config/__init__.py
--rw-r--r--   0        0        0     4687 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_config/api_config.py
--rw-r--r--   0        0        0      379 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_config/file_config.py
--rw-r--r--   0        0        0     2216 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_config/logging_config.py
--rw-r--r--   0        0        0      147 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_version.py
--rw-r--r--   0        0        0      502 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/exceptions.py
--rw-r--r--   0        0        0      917 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/models/__init__.py
--rw-r--r--   0        0        0      322 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/models/_base.py
--rw-r--r--   0        0        0     6250 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/models/_core.py
--rw-r--r--   0        0        0     1895 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/models/_lunchmoney.py
--rw-r--r--   0        0        0     9126 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/assets.py
--rw-r--r--   0        0        0     6752 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/budgets.py
--rw-r--r--   0        0        0    15170 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/categories.py
--rw-r--r--   0        0        0     5188 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/crypto.py
--rw-r--r--   0        0        0     4626 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/plaid_accounts.py
--rw-r--r--   0        0        0     6857 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/recurring_expenses.py
--rw-r--r--   0        0        0     1271 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/tags.py
--rw-r--r--   0        0        0    32901 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/transactions.py
--rw-r--r--   0        0        0     1535 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/user.py
--rw-r--r--   0        0        0      220 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/__init__.py
--rw-r--r--   0        0        0      205 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/base/__init__.py
--rw-r--r--   0        0        0    12165 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/base/base_app.py
--rw-r--r--   0        0        0     1598 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/base/pandas_app.py
--rw-r--r--   0        0        0     2809 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/primelunch/README.md
--rw-r--r--   0        0        0       26 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/primelunch/__init__.py
--rw-r--r--   0        0        0    14911 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/primelunch/primelunch.py
--rw-r--r--   0        0        0     2104 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/pushlunch/README.md
--rw-r--r--   0        0        0      100 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/pushlunch/__init__.py
--rw-r--r--   0        0        0    11661 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/pushlunch/pushover.py
--rw-r--r--   0        0        0     1707 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/README.md
--rw-r--r--   0        0        0      230 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/__init__.py
--rw-r--r--   0        0        0      320 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/_config.py
--rw-r--r--   0        0        0      150 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/exceptions.py
--rw-r--r--   0        0        0    49243 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
--rw-r--r--   0        0        0      598 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/models.py
--rw-r--r--   0        0        0        0 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/py.typed
--rw-r--r--   0        0        0     1800 2023-04-23 04:32:09.093263 lunchable-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 lunchable-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 lunchable-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 lunchable-0.7.1/.releaserc.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 lunchable-0.7.1/Dockerfile
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 lunchable-0.7.1/docker-compose.yaml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/FUNDING.yaml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/labels.yaml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/release-drafter.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/matchers/python.json
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/workflows/docker.yaml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/workflows/labeler.yaml
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 lunchable-0.7.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/Makefile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/README.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/requirements.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/cli.md
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/cli.rst
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/conf.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/contributing.md
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/index.rst
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/lunchable.rst
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/plugins.rst
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/primelunch.md
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/pushlunch.rst
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/splitlunch.rst
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/usage.rst
+-rw-r--r--   0        0        0   124987 2020-02-02 00:00:00.000000 lunchable-0.7.1/docs/source/_static/lunchable.png
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/__main__.py
+-rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/_cli.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/_version.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/_config/__init__.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/_config/api_config.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/_config/file_config.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/_config/logging_config.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/_base.py
+-rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/_core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/_lunchmoney.py
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/assets.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/budgets.py
+-rw-r--r--   0        0        0    15170 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/categories.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/crypto.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/plaid_accounts.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/recurring_expenses.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/tags.py
+-rw-r--r--   0        0        0    32885 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/transactions.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/models/user.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/__init__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/base/__init__.py
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/base/base_app.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/base/pandas_app.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/primelunch/README.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/primelunch/__init__.py
+-rw-r--r--   0        0        0    14911 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/primelunch/primelunch.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/pushlunch/README.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/pushlunch/__init__.py
+-rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/pushlunch/pushover.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/splitlunch/README.md
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/splitlunch/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/splitlunch/_config.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/splitlunch/exceptions.py
+-rw-r--r--   0        0        0    49340 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lunchable-0.7.1/lunchable/plugins/splitlunch/models.py
+-rw-r--r--   0        0        0    68915 2020-02-02 00:00:00.000000 lunchable-0.7.1/requirements/dev.txt
+-rw-r--r--   0        0        0    18547 2020-02-02 00:00:00.000000 lunchable-0.7.1/requirements/prod.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/test_assets.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/test_budgets.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/test_categories.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/test_crypto.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/test_plaid_accounts.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/test_recurring_expenses.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/test_tags.py
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/test_transactions.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/test_user.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_add_to_category_group.yaml
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_create_and_delete_transaction_group.yaml
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_create_asset.yaml
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_create_category.yaml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_create_category_group.yaml
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_delete_budget.yaml
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_delete_category.yaml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_delete_category_force.yaml
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_assets.yaml
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_budgets.yaml
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_categories.yaml
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_category.yaml
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_crypto.yaml
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_plaid_accounts.yaml
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_recurring_expenses.yaml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_tags.yaml
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_transaction.yaml
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_transactions.yaml
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_get_user.yaml
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_insert_transactions.yaml
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_split_transaction.yaml
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_unsplit_transaction.yaml
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_update_asset.yaml
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_update_category.yaml
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_update_crypto.yaml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_update_transaction.yaml
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/models/cassettes/test_upsert_budget.yaml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/pushlunch/__init__.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/pushlunch/test_pushlunch.py
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/pushlunch/cassettes/test_post_transaction.yaml
+-rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/pushlunch/cassettes/test_send_notification.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/splitlunch/__init__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/splitlunch/test_splitwise.py
+-rw-r--r--   0        0        0    14089 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/splitlunch/cassettes/test_update_balance.yaml
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/splitlunch/data/splitwise_non_involved_expense.json
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/splitlunch/data/splitwise_non_involved_transfer.json
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/splitlunch/data/splitwise_non_user_paid_expense.json
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/splitlunch/data/splitwise_non_user_paid_transfer.json
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/splitlunch/data/splitwise_user_paid_expense.json
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 lunchable-0.7.1/tests/plugins/splitlunch/data/splitwise_user_paid_transfer.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 lunchable-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 lunchable-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 lunchable-0.7.1/README.md
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 lunchable-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 lunchable-0.7.1/PKG-INFO
```

### Comparing `lunchable-0.7.0/LICENSE` & `lunchable-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/README.md` & `lunchable-0.7.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 [![Lunchable Version](https://img.shields.io/pypi/v/lunchable?color=blue&label=lunchable)](https://github.com/juftin/lunchable)
 [![PyPI](https://img.shields.io/pypi/pyversions/lunchable)](https://pypi.python.org/pypi/lunchable/)
 [![Docker Image Version](https://img.shields.io/docker/v/juftin/lunchable?color=blue&label=docker&logo=docker)](https://hub.docker.com/r/juftin/lunchable)
 [![Testing Status](https://github.com/juftin/lunchable/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/juftin/lunchable/actions/workflows/tests.yaml?query=branch%3Amain)
 [![GitHub License](https://img.shields.io/github/license/juftin/lunchable?color=blue&label=License)](https://github.com/juftin/lunchable/blob/main/LICENSE)
 
 **lunchable** is a Python Client for the [Lunch Money Developer API](https://lunchmoney.dev). It's
-built on top of [pydantic](https://github.com/samuelcolvin/pydantic), it offers an *intuitive* API,
-a *simple* CLI, complete coverage of all endpoints, and *plugins* to other external services.
+built on top of [pydantic](https://github.com/samuelcolvin/pydantic), it offers an _intuitive_ API,
+a _simple_ CLI, complete coverage of all endpoints, and _plugins_ to other external services.
 
 ### Installation
 
 ```shell
 pip install lunchable
 ```
 
@@ -41,17 +41,19 @@
 ```shell
 export LUNCHMONEY_ACCESS_TOKEN="xxxxxxxxxxx"
 lunchable transactions get --limit 5
 lunchable http -X GET https://dev.lunchmoney.app/v1/assets
 ```
 
 ### Check out the [**Docs**](https://juftin.com/lunchable/)
+
 ### Looking to contribute? See the [Contributing Guide](docs/source/contributing.md)
+
 ### See the [Changelog](https://github.com/juftin/lunchable/releases)
 
+---
 
---------------
---------------
+---
 
 <br/>
 
 [<p align="center" ><img src="https://raw.githubusercontent.com/juftin/juftin/main/static/juftin.png" width="60" height="60"  alt="juftin logo"> </p>](https://github.com/juftin)
```

#### html2text {}

```diff
@@ -8,23 +8,23 @@
 (https://hub.docker.com/r/juftin/lunchable) [![Testing Status](https://
 github.com/juftin/lunchable/actions/workflows/tests.yaml/
 badge.svg?branch=main)](https://github.com/juftin/lunchable/actions/workflows/
 tests.yaml?query=branch%3Amain) [![GitHub License](https://img.shields.io/
 github/license/juftin/lunchable?color=blue&label=License)](https://github.com/
 juftin/lunchable/blob/main/LICENSE) **lunchable** is a Python Client for the
 [Lunch Money Developer API](https://lunchmoney.dev). It's built on top of
-[pydantic](https://github.com/samuelcolvin/pydantic), it offers an *intuitive*
-API, a *simple* CLI, complete coverage of all endpoints, and *plugins* to other
+[pydantic](https://github.com/samuelcolvin/pydantic), it offers an _intuitive_
+API, a _simple_ CLI, complete coverage of all endpoints, and _plugins_ to other
 external services. ### Installation ```shell pip install lunchable ``` ###
 Usage ```python from typing import Any, Dict, List from lunchable import
 LunchMoney from lunchable.models import TransactionObject lunch = LunchMoney
 (access_token="xxxxxxxxxxx") transactions: List[TransactionObject] =
 lunch.get_transactions() first_transaction: TransactionObject = transactions[0]
 transaction_as_dict: Dict[str, Any] = first_transaction.dict() ``` ```shell
 export LUNCHMONEY_ACCESS_TOKEN="xxxxxxxxxxx" lunchable transactions get --limit
 5 lunchable http -X GET https://dev.lunchmoney.app/v1/assets ``` ### Check out
 the [**Docs**](https://juftin.com/lunchable/) ### Looking to contribute? See
 the [Contributing Guide](docs/source/contributing.md) ### See the [Changelog]
-(https://github.com/juftin/lunchable/releases) -------------- --------------
+(https://github.com/juftin/lunchable/releases) --- ---
 [
                                  [juftin logo]
 ](https://github.com/juftin)
```

### Comparing `lunchable-0.7.0/lunchable/__init__.py` & `lunchable-0.7.1/lunchable/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/_cli.py` & `lunchable-0.7.1/lunchable/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Lunchmoney CLI
 """
 
 import datetime
 import logging
+import sys
 from json import JSONDecodeError
 from typing import Any, Dict, Optional, Union
 
 import click
 import requests
 from pydantic.json import pydantic_encoder
 from rich import print, print_json, traceback
@@ -414,15 +415,15 @@
         data=data,
     )
     try:
         resp.raise_for_status()
     except requests.HTTPError:
         logger.error(resp)
         print(resp.text)
-        exit(1)
+        sys.exit(1)
     try:
         response = resp.json()
     except JSONDecodeError:
         response = resp.text
     print_json(data=response, default=pydantic_encoder)
```

### Comparing `lunchable-0.7.0/lunchable/_config/api_config.py` & `lunchable-0.7.1/lunchable/_config/api_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,16 +145,16 @@
         fragment: str
             Fragment identifier
         Returns
         -------
         url: str
             Compiled URL
         """
-        url_components = dict(
-            scheme=scheme,
-            netloc=netloc,
-            path=path,
-            params=params,
-            query=query,
-            fragment=fragment,
-        )
+        url_components = {
+            "scheme": scheme,
+            "netloc": netloc,
+            "path": path,
+            "params": params,
+            "query": query,
+            "fragment": fragment,
+        }
         return parse.urlunparse(components=tuple(url_components.values()))
```

### Comparing `lunchable-0.7.0/lunchable/_config/logging_config.py` & `lunchable-0.7.1/lunchable/_config/logging_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/models/__init__.py` & `lunchable-0.7.1/lunchable/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/models/_core.py` & `lunchable-0.7.1/lunchable/models/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     def _make_request(
         self,
         method: str,
         url_path: Union[List[Union[str, int]], str, int],
         params: Optional[Dict[str, Any]] = None,
         payload: Optional[Any] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> Any:
         """
         Make a Request to the API
 
         Parameters
         ----------
         method: str
@@ -119,15 +119,15 @@
                 method=method, url=url, params=params, data=payload, **kwargs
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as he:
             logger.exception(he)
             # noinspection PyUnboundLocalVariable
             logger.error(response.text)
-            raise LunchMoneyHTTPError(he)
+            raise LunchMoneyHTTPError(he) from he
         returned_data = loads(response.content)
         if isinstance(returned_data, dict) and any(
             ["error" in returned_data.keys(), "errors" in returned_data.keys()]
         ):
             try:
                 errors = returned_data["error"]
             except KeyError:
@@ -139,15 +139,15 @@
     def make_http_request(
         self,
         method: str,
         url: str,
         params: Optional[Any] = None,
         data: Optional[Any] = None,
         json: Optional[Any] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> requests.Response:
         """
         Make a HTTP Request
 
         This is a simple method :class:`.LunchMoney` exposes to make HTTP requests. It
         has the benefit of using an existing `requests.Session` as well as as out of the box
         auth headers that are used to connect to the Lunch Money Developer API.
```

### Comparing `lunchable-0.7.0/lunchable/models/_lunchmoney.py` & `lunchable-0.7.1/lunchable/models/_lunchmoney.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/models/assets.py` & `lunchable-0.7.1/lunchable/models/assets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/models/budgets.py` & `lunchable-0.7.1/lunchable/models/budgets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/models/categories.py` & `lunchable-0.7.1/lunchable/models/categories.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/models/crypto.py` & `lunchable-0.7.1/lunchable/models/crypto.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/models/plaid_accounts.py` & `lunchable-0.7.1/lunchable/models/plaid_accounts.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/models/recurring_expenses.py` & `lunchable-0.7.1/lunchable/models/recurring_expenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         months”, then that recurring expense will not show up in the results for this month.
 
         Parameters
         ----------
         start_date : Optional[datetime.date]
             Date to search. By default will return the first day of the current month
         debit_as_negative: bool
-            Pass in true if you’d like expenses to be returned as negative amounts and credits as
+            Pass in true if you'd like expenses to be returned as negative amounts and credits as
             positive amounts.
 
         Returns
         -------
         List[RecurringExpensesObject]
         """
         if start_date is None:
```

### Comparing `lunchable-0.7.0/lunchable/models/tags.py` & `lunchable-0.7.1/lunchable/models/tags.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/models/transactions.py` & `lunchable-0.7.1/lunchable/models/transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,19 +245,19 @@
     _parent_id_description = """
     Exists if this is a split transaction. Denotes the transaction ID of the original
     transaction. Note that the parent transaction is not returned in this call.
     """
     _is_group_description = """
     True if this transaction represents a group of transactions. If so, amount
     and currency represent the totalled amount of transactions bearing this
-    transaction’s id as their group_id. Amount is calculated based on the
-    user’s primary currency.
+    transaction's id as their group_id. Amount is calculated based on the
+    user's primary currency.
     """
     _group_id_description = """
-    Exists if this transaction is part of a group. Denotes the parent’s transaction ID
+    Exists if this transaction is part of a group. Denotes the parent's transaction ID
     """
     _external_id_description = """
     User-defined external ID for any manually-entered or imported transaction.
     External ID cannot be accessed or changed for Plaid-imported transactions.
     External ID must be unique by asset_id. Max 75 characters.
     """
     _original_name_description = """
@@ -486,18 +486,18 @@
             Sets the offset for the records returned
         limit: Optional[int]
             Sets the maximum number of records to return. Note: The server will not
             respond with any indication that there are more records to be returned.
             Please check the response length to determine if you should make another
             call with an offset to fetch more transactions.
         debit_as_negative: Optional[bool]
-            Pass in true if you’d like expenses to be returned as negative amounts and
+            Pass in true if you'd like expenses to be returned as negative amounts and
             credits as positive amounts. Defaults to false.
         pending: Optional[bool]
-            Pass in true if you’d like to include imported transactions with a pending status.
+            Pass in true if you'd like to include imported transactions with a pending status.
         params: Optional[dict]
             Additional Query String Params
 
         Returns
         -------
         List[TransactionObject]
             A list of transactions
@@ -684,15 +684,15 @@
 
         Parameters
         ----------
         transactions: ListOrSingleTransactionTypeObject
             Transactions to insert. Either a single TransactionInsertObject object or
             a list of them
         apply_rules: bool
-            If true, will apply account’s existing rules to the inserted transactions.
+            If true, will apply account's existing rules to the inserted transactions.
             Defaults to false.
         skip_duplicates: bool
             If true, the system will automatically dedupe based on transaction date,
             payee and amount. Note that deduping by external_id will occur regardless
             of this flag.
         check_for_recurring: bool
             if true, will check new transactions for occurrences of new monthly expenses.
@@ -717,15 +717,15 @@
             lunch = LunchMoney(access_token="xxxxxxx")
 
             new_transaction = TransactionInsertObject(payee="Example Restaurant",
                                                       amount=120.00,
                                                       notes="Saturday Dinner")
             new_transaction_ids = lunch.insert_transactions(transactions=new_transaction)
         """
-        insert_objects = list()
+        insert_objects = []
         if not isinstance(transactions, list):
             transactions = [transactions]
         for item in transactions:
             if isinstance(item, TransactionObject):
                 insert_objects.append(item.get_insert_object())
             elif isinstance(item, TransactionInsertObject):
                 insert_objects.append(item)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lunchable-0.7.0/lunchable/models/user.py` & `lunchable-0.7.1/lunchable/models/user.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/plugins/base/base_app.py` & `lunchable-0.7.1/lunchable/plugins/base/base_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,22 +340,20 @@
         """
 
     @property
     def __builtin_data_models__(self) -> List[LunchableDataModel]:
         """
         Which Data Should this app get
         """
-        return super().__builtin_data_models__ + [
+        return [
+            *super().__builtin_data_models__,
             LunchableDataModel(
                 model=TransactionObject,
                 function=self.lunch.get_transactions,
-                kwargs={
-                    "start_date": self.start_date,
-                    "end_date": self.end_date,
-                },
+                kwargs={"start_date": self.start_date, "end_date": self.end_date},
             ),
         ]
 
     def refresh_transactions(
         self,
         start_date: Optional[datetime.date] = None,
         end_date: Optional[datetime.date] = None,
```

### Comparing `lunchable-0.7.0/lunchable/plugins/base/pandas_app.py` & `lunchable-0.7.1/lunchable/plugins/base/pandas_app.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/plugins/primelunch/README.md` & `lunchable-0.7.1/lunchable/plugins/primelunch/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,27 @@
         <img src=https://upload.wikimedia.org/wikipedia/commons/d/de/Amazon_icon.png
             width="35%" alt="lunchable">
         <img src=https://i.imgur.com/FyKDsG3.png
             width="60%" alt="lunchable">
     </p>
 </div>
 
---------
+---
 
 `PrimeLunch` is a command line tool that supports updating Amazon transaction notes with the items from
 Amazon itself. This tool uses CSVs generated by the
 [Amazon Order History Reporter](https://chrome.google.com/webstore/detail/amazon-order-history-repo/mgkilgclilajckgnedgjgnfdokkgnibi)
 plugin on Chrome. Once you've gathered your transactions, export them as a CSV and scan them with the tool.
 You'll be asked which transactions you'd like to update.
 
 <div>
     <img src=https://i.imgur.com/C5IcOQl.png>
 </div>
 
---------
+---
 
 The plugin uses the dollar amounts on the CSV export to match Amazon transactions in LunchMoney.
 When a matching dollar amount is found, `PrimeLunch` compares the date window between the transactions
 to determine if they're really a match.
 
 We're using
 the [Amazon Order History Reporter](https://chrome.google.com/webstore/detail/amazon-order-history-repo/mgkilgclilajckgnedgjgnfdokkgnibi)
```

### Comparing `lunchable-0.7.0/lunchable/plugins/primelunch/primelunch.py` & `lunchable-0.7.1/lunchable/plugins/primelunch/primelunch.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/plugins/pushlunch/README.md` & `lunchable-0.7.1/lunchable/plugins/pushlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/plugins/pushlunch/pushover.py` & `lunchable-0.7.1/lunchable/plugins/pushlunch/pushover.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,21 +67,21 @@
         token = app_token or b64decode(_courtesy_token).decode("utf-8")
         user_key = user_key or getenv("PUSHOVER_USER_KEY", None)
         if user_key in [None, ""]:
             raise PushLunchError(
                 "You must provide a Pushover User Key or define it with "
                 "a `PUSHOVER_USER_KEY` environment variable"
             )
-        self._params = dict(user=user_key, token=token)
+        self._params = {"user": user_key, "token": token}
         self.lunchable = lunchable_client or LunchMoney(
             access_token=lunchmoney_access_token
         )
         self.asset_mapping = self._get_assets()
         self.category_mapping = self._get_categories()
-        self.notified_transactions: List[int] = list()
+        self.notified_transactions: List[int] = []
 
     def send_notification(
         self,
         message: str,
         attachment: Optional[object] = None,
         device: Optional[str] = None,
         title: Optional[str] = None,
@@ -125,26 +125,26 @@
             Pass 1 if message contains HTML contents
 
         Returns
         -------
         requests.Response
         """
         html_param = 1 if html not in [None, False] else None
-        params_dict = dict(
-            message=message,
-            attachment=attachment,
-            device=device,
-            title=title,
-            url=url,
-            url_title=url_title,
-            priority=priority,
-            sound=sound,
-            timestamp=timestamp,
-            html=html_param,
-        )
+        params_dict = {
+            "message": message,
+            "attachment": attachment,
+            "device": device,
+            "title": title,
+            "url": url,
+            "url_title": url_title,
+            "priority": priority,
+            "sound": sound,
+            "timestamp": timestamp,
+            "html": html_param,
+        }
         params: Dict[str, Any] = {
             key: value for key, value in params_dict.items() if value is not None
         }
         params.update(self._params)
         response = self.session.post(url=self.pushover_endpoint, params=params)
         response.raise_for_status()
         return response
@@ -215,15 +215,15 @@
         Returns
         -------
         Dict[int, str]
         """
         manual_assets = self.lunchable.get_assets()
         plaid_account = self.lunchable.get_plaid_accounts()
         assets = [*manual_assets, *plaid_account]
-        asset_mapping = dict()
+        asset_mapping = {}
         for account in assets:
             if isinstance(account, AssetsObject):
                 if account.display_name is None:
                     name = account.name
                 else:
                     name = account.display_name
                 asset_mapping[account.id] = name
@@ -236,15 +236,15 @@
         Get Mapping Of Category ID -> Category Name
 
         Returns
         -------
         Dict[int, str]
         """
         categories = self.lunchable.get_categories()
-        category_mapping = dict()
+        category_mapping = {}
         for category in categories:
             category_mapping[category.id] = category.name
         return category_mapping
 
     @classmethod
     def _format_float(cls, amount: float) -> str:
         """
@@ -307,15 +307,15 @@
             logger.warning(
                 "Check interval cannot be less than 5 minutes. Defaulting to 5."
             )
             interval = 5
         if continuous is True:
             logger.info("Continuous Notifications Enabled. Beginning PushLunch.")
 
-        uncleared_transactions = list()
+        uncleared_transactions = []
         continuous_search = True
 
         while continuous_search is True:
             found_transactions = len(self.notified_transactions)
             uncleared_transactions += self._get_uncleared_transactions()
             for transaction in uncleared_transactions:
                 self.post_transaction(transaction=transaction)
```

### Comparing `lunchable-0.7.0/lunchable/plugins/splitlunch/README.md` & `lunchable-0.7.1/lunchable/plugins/splitlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py` & `lunchable-0.7.1/lunchable/plugins/splitlunch/lunchmoney_splitwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     from dateutil.tz import tzlocal
 except ImportError as ie:
     logger.exception(ie)
     _pip_extra_error = (
         "Looks like you don't have the Splitwise plugin installed: "
         f"`pip install {__application__}[splitlunch]`"
     )
-    raise LunchMoneyImportError(_pip_extra_error)
+    raise LunchMoneyImportError(_pip_extra_error) from ie
 
 
 def _get_splitwise_impact(
     expense: splitwise.Expense, current_user_id: int
 ) -> Tuple[float, bool]:
     """
     Get the Financial Impact of a Splitwise Transaction
@@ -230,18 +230,18 @@
 
         Returns
         -------
         Tuple[float]
         """
         try:
             assert amount == round(amount, 2)
-        except AssertionError:
+        except AssertionError as ae:
             raise SplitLunchError(
                 f"{amount} caused an error, you must provide a real " "spending amount."
-            )
+            ) from ae
         equal_shares = round(amount, 2) / splits
         remainder_dollars = floor(equal_shares)
         remainder_cents = floor((equal_shares - remainder_dollars) * 100) / 100
         remainder_left = round(
             (equal_shares - remainder_dollars - remainder_cents) * splits * 100, 0
         )
         owed_amount = remainder_dollars + remainder_cents
@@ -312,16 +312,16 @@
         new_expense.addUser(user=primary_user)
         new_expense.addUser(user=financial_partner)
         # SUBMIT THE EXPENSE AND GET THE RESPONSE
         expense_response: splitwise.Expense
         expense_response, expense_errors = self.createExpense(expense=new_expense)
         try:
             assert expense_errors is None
-        except AssertionError:
-            raise SplitLunchError(expense_errors["base"][0])
+        except AssertionError as ae:
+            raise SplitLunchError(expense_errors["base"][0]) from ae
         logger.info("Expense Created: %s", expense_response.id)
         message = f"Created via SplitLunch: {datetime.datetime.now()}"
         self.createComment(expense_id=expense_response.id, content=message)
         pydantic_response = self.splitwise_to_pydantic(expense=expense_response)
         return pydantic_response
 
     def create_expense_on_behalf_of_partner(
@@ -364,16 +364,16 @@
         new_expense.addUser(user=primary_user)
         new_expense.addUser(user=financial_partner)
         # SUBMIT THE EXPENSE AND GET THE RESPONSE
         expense_response: splitwise.Expense
         expense_response, expense_errors = self.createExpense(expense=new_expense)
         try:
             assert expense_errors is None
-        except AssertionError:
-            raise SplitLunchError(expense_errors["base"][0])
+        except AssertionError as ae:
+            raise SplitLunchError(expense_errors["base"][0]) from ae
         logger.info("Expense Created: %s", expense_response.id)
         message = f"Created via SplitLunch: {datetime.datetime.now()}"
         self.createComment(expense_id=expense_response.id, content=message)
         pydantic_response = self.splitwise_to_pydantic(expense=expense_response)
         return pydantic_response
 
     def get_friend(
@@ -477,17 +477,19 @@
         """
         if consumer_key is None:
             consumer_key = getenv("SPLITWISE_CONSUMER_KEY")
         if consumer_secret is None:
             consumer_secret = getenv("SPLITWISE_CONSUMER_SECRET")
         if api_key is None:
             api_key = getenv("SPLITWISE_API_KEY", None)
-        init_kwargs = dict(
-            consumer_key=consumer_key, consumer_secret=consumer_secret, api_key=api_key
-        )
+        init_kwargs = {
+            "consumer_key": consumer_key,
+            "consumer_secret": consumer_secret,
+            "api_key": api_key,
+        }
         if consumer_key is None or consumer_secret is None or api_key is None:
             error_message = (
                 dedent(
                     """
             You must set your Splitwise credentials explicitly or by assigning
             the `SPLITWISE_CONSUMER_KEY`, `SPLITWISE_CONSUMER_SECRET`, and the
             `SPLITWISE_API_KEY`environment variables
@@ -541,15 +543,15 @@
         Splitwise account asset object
 
         Returns
         -------
         AssetsObject
         """
         assets = self.lunchable.get_assets()
-        splitwise_assets = list()
+        splitwise_assets = []
         for asset in assets:
             if (
                 asset.institution_name is not None
                 and "splitwise" in asset.institution_name.lower()
             ):
                 splitwise_assets.append(asset)
         if len(splitwise_assets) == 0:
@@ -571,15 +573,15 @@
         category
 
         Returns
         -------
         CategoriesObject
         """
         categories = self.lunchable.get_categories()
-        reimbursement_list = list()
+        reimbursement_list = []
         for category in categories:
             if "reimbursement" == category.name.strip().lower():
                 reimbursement_list.append(category)
         if len(reimbursement_list) != 1:
             return None
         return reimbursement_list[0]
 
@@ -776,15 +778,15 @@
         Split all transactions with the `SplitLunch` tag in half. One of these
         new splits will be recategorized to `Reimbursement`. Both new splits will receive
         the `Splitwise` tag without any preexisting tags.
         """
         if self.reimbursement_category is None:
             self._raise_category_reimbursement_error()
             raise ValueError("ReimbursementCategory")
-        split_transaction_ids = list()
+        split_transaction_ids = []
         tagged_objects = self.get_splitlunch_tagged_transactions()
         for transaction in tagged_objects:
             # Split the Original Amount
             amount_1, amount_2 = self.split_a_transaction(amount=transaction.amount)
             # Generate the First Split
             split_object = TransactionSplitObject(
                 date=transaction.date,
@@ -850,15 +852,15 @@
         List[Dict[str, Any]]
         """
         self._raise_financial_partner_error()
         if self.reimbursement_category is None:
             self._raise_category_reimbursement_error()
             raise ValueError("ReimbursementCategory")
         tagged_objects = self.get_splitlunch_import_tagged_transactions()
-        update_responses = list()
+        update_responses = []
         for transaction in tagged_objects:
             # Split the Original Amount
             description = str(transaction.payee)
             if transaction.notes is not None:
                 description = f"{transaction.payee} - {transaction.notes}"
             new_transaction = self.create_self_paid_expense(
                 amount=transaction.amount, description=description
@@ -882,24 +884,24 @@
                 f"Transaction split by Splitwise: {transaction.amount} -> "
                 f"({split_object.amount}, {reimbursement_object.amount})"
             )
             update_response = self.lunchable.update_transaction(
                 transaction_id=transaction.id,
                 split=[split_object, reimbursement_object],
             )
-            formatted_update_response = dict(
-                original_id=transaction.id,
-                payee=transaction.payee,
-                amount=transaction.amount,
-                reimbursement_amount=reimbursement_object.amount,
-                notes=transaction.notes,
-                splitwise_id=new_transaction.splitwise_id,
-                updated=update_response["updated"],
-                split=update_response["split"],
-            )
+            formatted_update_response = {
+                "original_id": transaction.id,
+                "payee": transaction.payee,
+                "amount": transaction.amount,
+                "reimbursement_amount": reimbursement_object.amount,
+                "notes": transaction.notes,
+                "splitwise_id": new_transaction.splitwise_id,
+                "updated": update_response["updated"],
+                "split": update_response["split"],
+            }
             update_responses.append(formatted_update_response)
             # Tag each of the new transactions generated
             for split_transaction_id in update_response["split"]:
                 update_tags = transaction.tags or []
                 tags = [
                     tag.name
                     for tag in update_tags
@@ -933,15 +935,15 @@
             Defaults to False which
         """
         self._raise_financial_partner_error()
         if self.reimbursement_category is None:
             self._raise_category_reimbursement_error()
             raise ValueError("ReimbursementCategory")
         tagged_objects = self.get_splitlunch_direct_import_tagged_transactions()
-        update_responses = list()
+        update_responses = []
         for transaction in tagged_objects:
             # Split the Original Amount
             description = str(transaction.payee)
             if transaction.notes is not None:
                 description = f"{transaction.payee} - {transaction.notes}"
             new_transaction = self.create_expense_on_behalf_of_partner(
                 amount=transaction.amount, description=description
@@ -960,24 +962,24 @@
                 tags.append(self.splitwise_tag.name)
             update = TransactionUpdateObject(
                 category_id=self.reimbursement_category.id, tags=tags, notes=notes
             )
             response = self.lunchable.update_transaction(
                 transaction_id=transaction.id, transaction=update
             )
-            formatted_update_response = dict(
-                original_id=transaction.id,
-                payee=transaction.payee,
-                amount=transaction.amount,
-                reimbursement_amount=transaction.amount,
-                notes=transaction.notes,
-                splitwise_id=new_transaction.splitwise_id,
-                updated=response["updated"],
-                split=None,
-            )
+            formatted_update_response = {
+                "original_id": transaction.id,
+                "payee": transaction.payee,
+                "amount": transaction.amount,
+                "reimbursement_amount": transaction.amount,
+                "notes": transaction.notes,
+                "splitwise_id": new_transaction.splitwise_id,
+                "updated": response["updated"],
+                "split": None,
+            }
             update_responses.append(formatted_update_response)
         return update_responses
 
     def splitwise_to_lunchmoney(
         self,
         expenses: List[SplitLunchExpense],
         allow_self_paid: bool = False,
@@ -1061,15 +1063,15 @@
         ----------
         expenses: List[SplitLunchExpense]
 
         Returns
         -------
         List[SplitLunchExpense]
         """
-        filtered_expenses = list()
+        filtered_expenses = []
         for splitwise_transaction in expenses:
             if all(
                 [
                     splitwise_transaction.deleted is False,
                     splitwise_transaction.financial_impact != 0.00,
                     allow_self_paid or (splitwise_transaction.self_paid is False),
                     allow_payments or (splitwise_transaction.payment is False),
@@ -1227,19 +1229,19 @@
         self.splitwise_to_lunchmoney(
             expenses=new_transactions,
             allow_self_paid=allow_self_paid,
             allow_payments=allow_payments,
         )
         splitwise_asset = self.update_splitwise_balance()
         self.handle_deleted_transactions(deleted_transactions=deleted_transactions)
-        return dict(
-            balance=splitwise_asset.balance,
-            new=new_transactions,
-            deleted=deleted_transactions,
-        )
+        return {
+            "balance": splitwise_asset.balance,
+            "new": new_transactions,
+            "deleted": deleted_transactions,
+        }
 
     def handle_deleted_transactions(
         self,
         deleted_transactions: List[TransactionObject],
     ) -> List[Dict[str, Any]]:
         """
         Update Transactions That Exist in Splitwise, but have been deleted in Splitwise
@@ -1248,15 +1250,15 @@
         ----------
         deleted_transactions: List[TransactionObject]
 
         Returns
         -------
         List[Dict[str, Any]]
         """
-        updated_transactions = list()
+        updated_transactions = []
         for transaction in deleted_transactions:
             update = self.lunchable.update_transaction(
                 transaction_id=transaction.id,
                 transaction=TransactionUpdateObject(
                     amount=0.00,
                     payee=self._deleted_payee,
                     notes=f"{transaction.payee} || {transaction.amount} || {transaction.notes}",
```

### Comparing `lunchable-0.7.0/lunchable/plugins/splitlunch/models.py` & `lunchable-0.7.1/lunchable/plugins/splitlunch/models.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.7.0/PKG-INFO` & `lunchable-0.7.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: lunchable
-Version: 0.7.0
+Version: 0.7.1
 Summary: A simple Python SDK around the Lunch Money Developer API
-Home-page: https://github.com/juftin/lunchable
-License: MIT
-Author: Justin Flannery
-Author-email: juftin@juftin.com
-Requires-Python: >=3.7.1,<4.0
+Project-URL: Changelog, https://github.com/juftin/lunchable/releases
+Project-URL: Discussions, https://github.com/juftin/lunchable/discussions
+Project-URL: Docker, https://hub.docker.com/r/juftin/lunchable
+Project-URL: Documentation, https://github.com/juftin/lunchable#readme
+Project-URL: Issues, https://github.com/juftin/lunchable/issues
+Project-URL: Source, https://github.com/juftin/lunchable
+Author-email: Justin Flannery <justin.flannery@juftin.com>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: api-client,lunchmoney,pydantic,python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Requires-Python: <4,>=3.7.1
+Requires-Dist: click>=8.0.1
+Requires-Dist: pydantic<2.0.0,>=1.2.0
+Requires-Dist: requests<3.0.0,>=2.0.0
+Requires-Dist: rich>=10.0.0
 Provides-Extra: all
+Requires-Dist: pandas<2.0.0,>=1.3.0; extra == 'all'
+Requires-Dist: python-dateutil~=2.8.2; extra == 'all'
+Requires-Dist: splitwise<3.0.0,>=2.3.0; extra == 'all'
 Provides-Extra: apps
+Requires-Dist: pandas<2.0.0,>=1.3.0; extra == 'apps'
 Provides-Extra: primelunch
+Requires-Dist: pandas<2.0.0,>=1.3.0; extra == 'primelunch'
 Provides-Extra: splitlunch
-Requires-Dist: click (>=8.0.1)
-Requires-Dist: pandas (>=1.3,<2.0) ; extra == "all" or extra == "apps" or extra == "primelunch"
-Requires-Dist: pydantic (>=1.2.0,<2.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) ; extra == "all" or extra == "splitlunch"
-Requires-Dist: requests (>=2,<3)
-Requires-Dist: rich (>=10.0.0)
-Requires-Dist: splitwise (>=2.3.0) ; extra == "all" or extra == "splitlunch"
-Project-URL: Bug Tracker, https://github.com/juftin/lunchable/issues
-Project-URL: Changelog, https://github.com/juftin/lunchable/releases
-Project-URL: Documentation, https://juftin.github.io/lunchable
-Project-URL: Discussions, https://github.com/juftin/lunchable/discussions
-Project-URL: Lunch Money API Docs, https://lunchmoney.dev
-Project-URL: Repository, https://github.com/juftin/lunchable
+Requires-Dist: python-dateutil~=2.8.2; extra == 'splitlunch'
+Requires-Dist: splitwise<3.0.0,>=2.3.0; extra == 'splitlunch'
 Description-Content-Type: text/markdown
 
 # lunchable
 
 <div align="center">
 <a href="https://github.com/juftin/lunchable">
   <img src=https://i.imgur.com/FyKDsG3.png
@@ -51,16 +51,16 @@
 [![Lunchable Version](https://img.shields.io/pypi/v/lunchable?color=blue&label=lunchable)](https://github.com/juftin/lunchable)
 [![PyPI](https://img.shields.io/pypi/pyversions/lunchable)](https://pypi.python.org/pypi/lunchable/)
 [![Docker Image Version](https://img.shields.io/docker/v/juftin/lunchable?color=blue&label=docker&logo=docker)](https://hub.docker.com/r/juftin/lunchable)
 [![Testing Status](https://github.com/juftin/lunchable/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/juftin/lunchable/actions/workflows/tests.yaml?query=branch%3Amain)
 [![GitHub License](https://img.shields.io/github/license/juftin/lunchable?color=blue&label=License)](https://github.com/juftin/lunchable/blob/main/LICENSE)
 
 **lunchable** is a Python Client for the [Lunch Money Developer API](https://lunchmoney.dev). It's
-built on top of [pydantic](https://github.com/samuelcolvin/pydantic), it offers an *intuitive* API,
-a *simple* CLI, complete coverage of all endpoints, and *plugins* to other external services.
+built on top of [pydantic](https://github.com/samuelcolvin/pydantic), it offers an _intuitive_ API,
+a _simple_ CLI, complete coverage of all endpoints, and _plugins_ to other external services.
 
 ### Installation
 
 ```shell
 pip install lunchable
 ```
 
@@ -82,18 +82,19 @@
 ```shell
 export LUNCHMONEY_ACCESS_TOKEN="xxxxxxxxxxx"
 lunchable transactions get --limit 5
 lunchable http -X GET https://dev.lunchmoney.app/v1/assets
 ```
 
 ### Check out the [**Docs**](https://juftin.com/lunchable/)
+
 ### Looking to contribute? See the [Contributing Guide](docs/source/contributing.md)
+
 ### See the [Changelog](https://github.com/juftin/lunchable/releases)
 
+---
 
---------------
---------------
+---
 
 <br/>
 
 [<p align="center" ><img src="https://raw.githubusercontent.com/juftin/juftin/main/static/juftin.png" width="60" height="60"  alt="juftin logo"> </p>](https://github.com/juftin)
-
```

#### html2text {}

```diff
@@ -1,54 +1,54 @@
-Metadata-Version: 2.1 Name: lunchable Version: 0.7.0 Summary: A simple Python
-SDK around the Lunch Money Developer API Home-page: https://github.com/juftin/
-lunchable License: MIT Author: Justin Flannery Author-email: juftin@juftin.com
-Requires-Python: >=3.7.1,<4.0 Classifier: Development Status :: 5 - Production/
-Stable Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: all Provides-Extra: apps Provides-Extra: primelunch Provides-
-Extra: splitlunch Requires-Dist: click (>=8.0.1) Requires-Dist: pandas
-(>=1.3,<2.0) ; extra == "all" or extra == "apps" or extra == "primelunch"
-Requires-Dist: pydantic (>=1.2.0,<2.0.0) Requires-Dist: python-dateutil
-(>=2.8.2,<3.0.0) ; extra == "all" or extra == "splitlunch" Requires-Dist:
-requests (>=2,<3) Requires-Dist: rich (>=10.0.0) Requires-Dist: splitwise
-(>=2.3.0) ; extra == "all" or extra == "splitlunch" Project-URL: Bug Tracker,
-https://github.com/juftin/lunchable/issues Project-URL: Changelog, https://
-github.com/juftin/lunchable/releases Project-URL: Documentation, https://
-juftin.github.io/lunchable Project-URL: Discussions, https://github.com/juftin/
-lunchable/discussions Project-URL: Lunch Money API Docs, https://lunchmoney.dev
-Project-URL: Repository, https://github.com/juftin/lunchable Description-
-Content-Type: text/markdown # lunchable
+Metadata-Version: 2.1 Name: lunchable Version: 0.7.1 Summary: A simple Python
+SDK around the Lunch Money Developer API Project-URL: Changelog, https://
+github.com/juftin/lunchable/releases Project-URL: Discussions, https://
+github.com/juftin/lunchable/discussions Project-URL: Docker, https://
+hub.docker.com/r/juftin/lunchable Project-URL: Documentation, https://
+github.com/juftin/lunchable#readme Project-URL: Issues, https://github.com/
+juftin/lunchable/issues Project-URL: Source, https://github.com/juftin/
+lunchable Author-email: Justin Flannery
+flannery@juftin.com> License-Expression: MIT License-File: LICENSE Keywords:
+api-client,lunchmoney,pydantic,python Classifier: Development Status :: 5 -
+Production/Stable Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: <4,>=3.7.1 Requires-
+Dist: click>=8.0.1 Requires-Dist: pydantic<2.0.0,>=1.2.0 Requires-Dist:
+requests<3.0.0,>=2.0.0 Requires-Dist: rich>=10.0.0 Provides-Extra: all
+Requires-Dist: pandas<2.0.0,>=1.3.0; extra == 'all' Requires-Dist: python-
+dateutil~=2.8.2; extra == 'all' Requires-Dist: splitwise<3.0.0,>=2.3.0; extra
+== 'all' Provides-Extra: apps Requires-Dist: pandas<2.0.0,>=1.3.0; extra ==
+'apps' Provides-Extra: primelunch Requires-Dist: pandas<2.0.0,>=1.3.0; extra ==
+'primelunch' Provides-Extra: splitlunch Requires-Dist: python-dateutil~=2.8.2;
+extra == 'splitlunch' Requires-Dist: splitwise<3.0.0,>=2.3.0; extra ==
+'splitlunch' Description-Content-Type: text/markdown # lunchable
                                   [lunchable]
 [![Lunchable Version](https://img.shields.io/pypi/v/
 lunchable?color=blue&label=lunchable)](https://github.com/juftin/lunchable) [!
 [PyPI](https://img.shields.io/pypi/pyversions/lunchable)](https://
 pypi.python.org/pypi/lunchable/) [![Docker Image Version](https://
 img.shields.io/docker/v/juftin/lunchable?color=blue&label=docker&logo=docker)]
 (https://hub.docker.com/r/juftin/lunchable) [![Testing Status](https://
 github.com/juftin/lunchable/actions/workflows/tests.yaml/
 badge.svg?branch=main)](https://github.com/juftin/lunchable/actions/workflows/
 tests.yaml?query=branch%3Amain) [![GitHub License](https://img.shields.io/
 github/license/juftin/lunchable?color=blue&label=License)](https://github.com/
 juftin/lunchable/blob/main/LICENSE) **lunchable** is a Python Client for the
 [Lunch Money Developer API](https://lunchmoney.dev). It's built on top of
-[pydantic](https://github.com/samuelcolvin/pydantic), it offers an *intuitive*
-API, a *simple* CLI, complete coverage of all endpoints, and *plugins* to other
+[pydantic](https://github.com/samuelcolvin/pydantic), it offers an _intuitive_
+API, a _simple_ CLI, complete coverage of all endpoints, and _plugins_ to other
 external services. ### Installation ```shell pip install lunchable ``` ###
 Usage ```python from typing import Any, Dict, List from lunchable import
 LunchMoney from lunchable.models import TransactionObject lunch = LunchMoney
 (access_token="xxxxxxxxxxx") transactions: List[TransactionObject] =
 lunch.get_transactions() first_transaction: TransactionObject = transactions[0]
 transaction_as_dict: Dict[str, Any] = first_transaction.dict() ``` ```shell
 export LUNCHMONEY_ACCESS_TOKEN="xxxxxxxxxxx" lunchable transactions get --limit
 5 lunchable http -X GET https://dev.lunchmoney.app/v1/assets ``` ### Check out
 the [**Docs**](https://juftin.com/lunchable/) ### Looking to contribute? See
 the [Contributing Guide](docs/source/contributing.md) ### See the [Changelog]
-(https://github.com/juftin/lunchable/releases) -------------- --------------
+(https://github.com/juftin/lunchable/releases) --- ---
 [
                                  [juftin logo]
 ](https://github.com/juftin)
```

