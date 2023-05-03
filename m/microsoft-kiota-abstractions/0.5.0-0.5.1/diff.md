# Comparing `tmp/microsoft-kiota-abstractions-0.5.0.tar.gz` & `tmp/microsoft-kiota-abstractions-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft-kiota-abstractions-0.5.0.tar", last modified: Fri Mar  3 20:33:56 2023, max compression
+gzip compressed data, was "microsoft-kiota-abstractions-0.5.1.tar", last modified: Wed May  3 10:16:24 2023, max compression
```

## Comparing `microsoft-kiota-abstractions-0.5.0.tar` & `microsoft-kiota-abstractions-0.5.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0       82 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1732 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2538 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/.gitignore
--rw-r--r--   0        0        0    15931 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/.pylintrc
--rw-r--r--   0        0        0      599 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/LICENSE
--rw-r--r--   0        0        0      285 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/Pipfile
--rw-r--r--   0        0        0    30112 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/Pipfile.lock
--rw-r--r--   0        0        0     2512 2023-03-03 20:33:53.175485 microsoft-kiota-abstractions-0.5.0/README.md
--rw-r--r--   0        0        0     2757 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/__init__.py
--rw-r--r--   0        0        0       23 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/_version.py
--rw-r--r--   0        0        0     3566 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/api_client_builder.py
--rw-r--r--   0        0        0      565 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/api_error.py
--rw-r--r--   0        0        0      346 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/__init__.py
--rw-r--r--   0        0        0      836 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/access_token_provider.py
--rw-r--r--   0        0        0     2175 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/allowed_hosts_validator.py
--rw-r--r--   0        0        0      607 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/anonymous_authentication_provider.py
--rw-r--r--   0        0        0      473 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/authentication_provider.py
--rw-r--r--   0        0        0     1231 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
--rw-r--r--   0        0        0      453 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/get_path_parameters.py
--rw-r--r--   0        0        0      529 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/method.py
--rw-r--r--   0        0        0      938 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/native_response_handler.py
--rw-r--r--   0        0        0     5164 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/request_adapter.py
--rw-r--r--   0        0        0     9062 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/request_information.py
--rw-r--r--   0        0        0      312 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/request_option.py
--rw-r--r--   0        0        0      965 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/response_handler.py
--rw-r--r--   0        0        0      632 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/__init__.py
--rw-r--r--   0        0        0      493 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/additional_data_holder.py
--rw-r--r--   0        0        0      961 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parsable.py
--rw-r--r--   0        0        0      642 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parsable_factory.py
--rw-r--r--   0        0        0     5793 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parse_node.py
--rw-r--r--   0        0        0      903 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parse_node_factory.py
--rw-r--r--   0        0        0     1972 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parse_node_factory_registry.py
--rw-r--r--   0        0        0     2424 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parse_node_proxy_factory.py
--rw-r--r--   0        0        0     9547 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/serialization_writer.py
--rw-r--r--   0        0        0      898 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/serialization_writer_factory.py
--rw-r--r--   0        0        0     2025 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/serialization_writer_factory_registry.py
--rw-r--r--   0        0        0     3132 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0      529 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/__init__.py
--rw-r--r--   0        0        0      398 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/backed_model.py
--rw-r--r--   0        0        0     3892 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/backing_store.py
--rw-r--r--   0        0        0      424 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/backing_store_factory.py
--rw-r--r--   0        0        0      237 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/backing_store_factory_singleton.py
--rw-r--r--   0        0        0     1166 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/backing_store_parse_node_factory.py
--rw-r--r--   0        0        0     1809 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0     4488 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/in_memory_backing_store.py
--rw-r--r--   0        0        0      380 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/in_memory_backing_store_factory.py
--rw-r--r--   0        0        0      899 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/kiota_abstractions/utils.py
--rw-r--r--   0        0        0     1268 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/tests/authentication/__init__.py
--rw-r--r--   0        0        0     1041 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/tests/authentication/test_base_bearer_token_authentication.py
--rw-r--r--   0        0        0      831 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0     5109 2023-03-03 20:33:53.179485 microsoft-kiota-abstractions-0.5.0/tests/test_request_information.py
--rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft-kiota-abstractions-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1732 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2538 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.gitignore
+-rw-r--r--   0        0        0    15931 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/.pylintrc
+-rw-r--r--   0        0        0      687 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/LICENSE
+-rw-r--r--   0        0        0      285 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/Pipfile
+-rw-r--r--   0        0        0    29636 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/Pipfile.lock
+-rw-r--r--   0        0        0     2512 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/README.md
+-rw-r--r--   0        0        0     2757 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/_version.py
+-rw-r--r--   0        0        0     3566 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/api_client_builder.py
+-rw-r--r--   0        0        0      962 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/api_error.py
+-rw-r--r--   0        0        0      346 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/__init__.py
+-rw-r--r--   0        0        0      836 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/access_token_provider.py
+-rw-r--r--   0        0        0     2175 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/allowed_hosts_validator.py
+-rw-r--r--   0        0        0      607 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/anonymous_authentication_provider.py
+-rw-r--r--   0        0        0      473 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/authentication_provider.py
+-rw-r--r--   0        0        0     1231 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
+-rw-r--r--   0        0        0      453 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/get_path_parameters.py
+-rw-r--r--   0        0        0      529 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/method.py
+-rw-r--r--   0        0        0      938 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/native_response_handler.py
+-rw-r--r--   0        0        0     5164 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_adapter.py
+-rw-r--r--   0        0        0     9048 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_information.py
+-rw-r--r--   0        0        0      312 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_option.py
+-rw-r--r--   0        0        0      965 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/response_handler.py
+-rw-r--r--   0        0        0      632 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/additional_data_holder.py
+-rw-r--r--   0        0        0      961 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parsable.py
+-rw-r--r--   0        0        0      642 2023-05-03 10:16:18.657619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parsable_factory.py
+-rw-r--r--   0        0        0     5793 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node.py
+-rw-r--r--   0        0        0      903 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_factory.py
+-rw-r--r--   0        0        0     1972 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_factory_registry.py
+-rw-r--r--   0        0        0     2424 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_proxy_factory.py
+-rw-r--r--   0        0        0     9547 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer.py
+-rw-r--r--   0        0        0      898 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_factory.py
+-rw-r--r--   0        0        0     2025 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_factory_registry.py
+-rw-r--r--   0        0        0     3132 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0      529 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/__init__.py
+-rw-r--r--   0        0        0      398 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backed_model.py
+-rw-r--r--   0        0        0     3892 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store.py
+-rw-r--r--   0        0        0      424 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_factory.py
+-rw-r--r--   0        0        0      237 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_factory_singleton.py
+-rw-r--r--   0        0        0     1166 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_parse_node_factory.py
+-rw-r--r--   0        0        0     1809 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0     4488 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/in_memory_backing_store.py
+-rw-r--r--   0        0        0      380 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/in_memory_backing_store_factory.py
+-rw-r--r--   0        0        0      899 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/kiota_abstractions/utils.py
+-rw-r--r--   0        0        0     1268 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/authentication/__init__.py
+-rw-r--r--   0        0        0     1041 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/authentication/test_base_bearer_token_authentication.py
+-rw-r--r--   0        0        0      831 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     5109 2023-05-03 10:16:18.661619 microsoft-kiota-abstractions-0.5.1/tests/test_request_information.py
+-rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft-kiota-abstractions-0.5.1/PKG-INFO
```

### Comparing `microsoft-kiota-abstractions-0.5.0/.github/workflows/auto-merge-dependabot.yml` & `microsoft-kiota-abstractions-0.5.1/.github/workflows/auto-merge-dependabot.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.3.6
+        uses: dependabot/fetch-metadata@v1.4.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft-kiota-abstractions-0.5.0/.github/workflows/ci.yml` & `microsoft-kiota-abstractions-0.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/.github/workflows/codeql-analysis.yml` & `microsoft-kiota-abstractions-0.5.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/.github/workflows/conflicting-pr-label.yml` & `microsoft-kiota-abstractions-0.5.1/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/.gitignore` & `microsoft-kiota-abstractions-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/.pylintrc` & `microsoft-kiota-abstractions-0.5.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/CHANGELOG.md` & `microsoft-kiota-abstractions-0.5.1/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.5.1] - 2023-04-29
+
+### Added
+
+- Adds the response headers to the APIError class.
+
 ## [0.5.0] - 2023-02-07
 
 ### Added
 
 - Added support for multi-valued request headers.
 
 ### Changed
```

### Comparing `microsoft-kiota-abstractions-0.5.0/LICENSE` & `microsoft-kiota-abstractions-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/Pipfile.lock` & `microsoft-kiota-abstractions-0.5.1/Pipfile.lock`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9557291666666666%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'b5e1af96431b5f676b23a3a2f5b2e5e24c17caee08b87924d61c85f9e9bf605e'}}",*

 * * "'develop'": "{'astroid': {'hashes': "*

 * *              "['sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347', "*

 * *              "'sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8'], "*

 * *              "'version': '==2.15.4'}, 'charset-normalizer': {'hashes': "*

 * *              "['sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6', "*

 * * […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "2f876971f1af2870de903243ad392917d92ea3fa3e6ed0f6ab2a67395970c29a"
+            "sha256": "b5e1af96431b5f676b23a3a2f5b2e5e24c17caee08b87924d61c85f9e9bf605e"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -22,145 +22,141 @@
             "index": "pypi",
             "version": "==4.1.1"
         }
     },
     "develop": {
         "astroid": {
             "hashes": [
-                "sha256:0e0e3709d64fbffd3037e4ff403580550f14471fd3eaae9fa11cc9a5c7901153",
-                "sha256:a3cf9f02c53dd259144a7e8f3ccd75d67c9a8c716ef183e0c1f291bc5d7bb3cf"
+                "sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347",
+                "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.14.2"
-        },
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
+            "version": "==2.15.4"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2022.12.7"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "version": "==3.0.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
+        },
+        "colorama": {
+            "hashes": [
+                "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
+                "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
+            ],
+            "markers": "sys_platform == 'win32'",
+            "version": "==0.4.6"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
                 "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.19"
         },
+        "exceptiongroup": {
+            "hashes": [
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==1.1.1"
+        },
         "flit": {
             "hashes": [
                 "sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c",
                 "sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937"
             ],
             "index": "pypi",
             "version": "==3.8.0"
@@ -245,147 +241,155 @@
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:0af4f0e20706aadf4e6f8f8dc5ab739089146b83fd53cb4a7e0e850ef3de0bb6",
-                "sha256:15b5a824b58c7c822c51bc66308e759243c32631896743f030daf449fe3677f3",
-                "sha256:17455cda53eeee0a4adb6371a21dd3dbf465897de82843751cf822605d152c8c",
-                "sha256:2013226d17f20468f34feddd6aae4635a55f79626549099354ce641bc7d40262",
-                "sha256:24189f23dc66f83b839bd1cce2dfc356020dfc9a8bae03978477b15be61b062e",
-                "sha256:27a0f74a298769d9fdc8498fcb4f2beb86f0564bcdb1a37b58cbbe78e55cf8c0",
-                "sha256:28cea5a6392bb43d266782983b5a4216c25544cd7d80be681a155ddcdafd152d",
-                "sha256:448de661536d270ce04f2d7dddaa49b2fdba6e3bd8a83212164d4174ff43aa65",
-                "sha256:48525aec92b47baed9b3380371ab8ab6e63a5aab317347dfe9e55e02aaad22e8",
-                "sha256:5bc8d6bd3b274dd3846597855d96d38d947aedba18776aa998a8d46fabdaed76",
-                "sha256:5deb252fd42a77add936b463033a59b8e48eb2eaec2976d76b6878d031933fe4",
-                "sha256:5f546ac34093c6ce33f6278f7c88f0f147a4849386d3bf3ae193702f4fe31407",
-                "sha256:5fdd63e4f50e3538617887e9aee91855368d9fc1dea30da743837b0df7373bc4",
-                "sha256:65b122a993d9c81ea0bfde7689b3365318a88bde952e4dfa1b3a8b4ac05d168b",
-                "sha256:71a808334d3f41ef011faa5a5cd8153606df5fc0b56de5b2e89566c8093a0c9a",
-                "sha256:920169f0184215eef19294fa86ea49ffd4635dedfdea2b57e45cb4ee85d5ccaf",
-                "sha256:93a85495fb13dc484251b4c1fd7a5ac370cd0d812bbfc3b39c1bafefe95275d5",
-                "sha256:a2948c40a7dd46c1c33765718936669dc1f628f134013b02ff5ac6c7ef6942bf",
-                "sha256:c6c2ccb7af7154673c591189c3687b013122c5a891bb5651eca3db8e6c6c55bd",
-                "sha256:c96b8a0c019fe29040d520d9257d8c8f122a7343a8307bf8d6d4a43f5c5bfcc8",
-                "sha256:d42a98e76070a365a1d1c220fcac8aa4ada12ae0db679cb4d910fabefc88b994",
-                "sha256:dbeb24514c4acbc78d205f85dd0e800f34062efcc1f4a4857c57e4b4b8712bff",
-                "sha256:e60d0b09f62ae97a94605c3f73fd952395286cf3e3b9e7b97f60b01ddfbbda88",
-                "sha256:e64f48c6176e243ad015e995de05af7f22bbe370dbb5b32bd6988438ec873919",
-                "sha256:e831662208055b006eef68392a768ff83596035ffd6d846786578ba1714ba8f6",
-                "sha256:eda5c8b9949ed411ff752b9a01adda31afe7eae1e53e946dbdf9db23865e66c4"
+                "sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521",
+                "sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140",
+                "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48",
+                "sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128",
+                "sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336",
+                "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a",
+                "sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41",
+                "sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f",
+                "sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e",
+                "sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8",
+                "sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238",
+                "sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119",
+                "sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb",
+                "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d",
+                "sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed",
+                "sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9",
+                "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e",
+                "sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a",
+                "sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5",
+                "sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950",
+                "sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937",
+                "sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394",
+                "sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6",
+                "sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602",
+                "sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1",
+                "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"
             ],
             "index": "pypi",
-            "version": "==1.0.1"
+            "version": "==1.2.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:13b08a53ed71021350c9e300d4ea8668438fb0046ab3937ac9a29913a1a1350a",
-                "sha256:accc3665857288317f32c7bebb5a8e482ba717b474f3fc1d18ca7f9214be0cef"
+                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
+                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.0"
+            "version": "==3.5.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:0decdf8dfe30298cd9f8d82e9a1542da464db47da60e03641631086671a03621",
-                "sha256:3e803be66e3a34c76b0aa1a3cf4714b538335e79bd69718d34fcf36d8fff2a2b"
+                "sha256:761907349e699f8afdcd56c4fe02f3021ab5b3a0fc26d19a9bfdc66c7d0d5cd5",
+                "sha256:a6cbb4c6e96eab4a3c7de7c6383c512478f58f88d95764507d84c899d656a89a"
             ],
             "index": "pypi",
-            "version": "==2.16.3"
+            "version": "==2.17.3"
         },
         "pytest": {
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
+                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
-            "version": "==7.2.1"
+            "version": "==7.3.1"
         },
         "pytest-asyncio": {
             "hashes": [
-                "sha256:83cbf01169ce3e8eb71c6c278ccb0574d1a7a3bb8eaaf5e50e0ad342afb33b36",
-                "sha256:f129998b209d04fcc65c96fc85c11e5316738358909a8399e93be553d7656442"
+                "sha256:2b38a496aef56f56b0e87557ec313e11e1ab9276fc3863f6a7be0f1d0e415e1b",
+                "sha256:f2b3366b7cd501a4056858bd39349d5af19742aed2d81660b7998b6341c7eb9c"
             ],
             "index": "pypi",
-            "version": "==0.20.3"
+            "version": "==0.21.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b",
+                "sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.29.0"
         },
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
             "version": "==0.10.2"
         },
+        "tomli": {
+            "hashes": [
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
+        },
         "tomli-w": {
             "hashes": [
                 "sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463",
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b",
-                "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.11.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.8"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "wrapt": {
             "hashes": [
                 "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
                 "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
                 "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
                 "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
@@ -457,20 +461,20 @@
                 "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
                 "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
                 "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
                 "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
                 "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
                 "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==1.15.0"
         },
         "yapf": {
             "hashes": [
-                "sha256:8fea849025584e486fd06d6ba2bed717f396080fd3cc236ba10cb97c4c51cf32",
-                "sha256:a3f5085d37ef7e3e004c4ba9f9b3e40c54ff1901cd111f05145ae313a7c67d1b"
+                "sha256:4c2b59bd5ffe46f3a7da48df87596877189148226ce267c16e8b44240e51578d",
+                "sha256:da62bdfea3df3673553351e6246abed26d9fe6780e548a5af9e70f6d2b4f5b9a"
             ],
             "index": "pypi",
-            "version": "==0.32.0"
+            "version": "==0.33.0"
         }
     }
 }
```

### Comparing `microsoft-kiota-abstractions-0.5.0/README.md` & `microsoft-kiota-abstractions-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/SECURITY.md` & `microsoft-kiota-abstractions-0.5.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/SUPPORT.md` & `microsoft-kiota-abstractions-0.5.1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/api_client_builder.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/access_token_provider.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/access_token_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/allowed_hosts_validator.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/allowed_hosts_validator.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/anonymous_authentication_provider.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/anonymous_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/method.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/method.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/native_response_handler.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/native_response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/request_adapter.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_adapter.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/request_information.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/request_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-from dataclasses import fields
+from dataclasses import dataclass, fields
 from datetime import date, datetime, time, timedelta
 from io import BytesIO
-from typing import TYPE_CHECKING, Any, Dict, Generic, List, Optional, Set, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, TypeVar, Union
 from uuid import UUID
 
 from uritemplate import URITemplate
 
 from .method import Method
 from .request_option import RequestOption
 from .serialization import Parsable, SerializationWriter
 
 if TYPE_CHECKING:
     from .request_adapter import RequestAdapter
 
 Url = str
 T = TypeVar("T", bound=Parsable)
-QueryParams = TypeVar('QueryParams')
 
 
-class RequestInformation(Generic[QueryParams]):
+@dataclass
+class QueryParams:
+    pass
+
+
+class RequestInformation():
     """This class represents an abstract HTTP request
     """
     RAW_URL_KEY = 'request-raw-url'
     BINARY_CONTENT_TYPE = 'application/octet-stream'
     CONTENT_TYPE_HEADER = 'Content-Type'
 
     def __init__(self) -> None:
```

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/response_handler.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/__init__.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parsable.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parsable.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parsable_factory.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parsable_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parse_node.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parse_node_factory.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parse_node_factory_registry.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/parse_node_proxy_factory.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/parse_node_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/serialization_writer.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/serialization_writer_factory.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/serialization_writer_factory_registry.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/serialization/serialization_writer_proxy_factory.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/serialization/serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/__init__.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/backing_store.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/backing_store_parse_node_factory.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/store/in_memory_backing_store.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/store/in_memory_backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/kiota_abstractions/utils.py` & `microsoft-kiota-abstractions-0.5.1/kiota_abstractions/utils.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/pyproject.toml` & `microsoft-kiota-abstractions-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/tests/authentication/test_base_bearer_token_authentication.py` & `microsoft-kiota-abstractions-0.5.1/tests/authentication/test_base_bearer_token_authentication.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/tests/conftest.py` & `microsoft-kiota-abstractions-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/tests/test_request_information.py` & `microsoft-kiota-abstractions-0.5.1/tests/test_request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-abstractions-0.5.0/PKG-INFO` & `microsoft-kiota-abstractions-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-abstractions
-Version: 0.5.0
+Version: 0.5.1
 Summary: Core abstractions for kiota generated libraries in Python
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

