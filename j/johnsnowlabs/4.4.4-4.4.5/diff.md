# Comparing `tmp/johnsnowlabs-4.4.4.tar.gz` & `tmp/johnsnowlabs-4.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs-4.4.4.tar", last modified: Wed Apr 26 21:10:43 2023, max compression
+gzip compressed data, was "johnsnowlabs-4.4.5.tar", last modified: Wed May  3 11:42:03 2023, max compression
```

## Comparing `johnsnowlabs-4.4.4.tar` & `johnsnowlabs-4.4.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.697373 johnsnowlabs-4.4.4/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.4/LICENSE
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.4/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.4/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.4/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-04-13 00:38:10.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-04-26 14:33:09.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8828 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.4/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.4/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4526 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.4/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-4.4.4/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.4/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.4/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2201 2023-04-26 21:09:24.000000 johnsnowlabs-4.4.4/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4253 2023-04-26 21:00:41.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8019 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 14:39:50.000000 johnsnowlabs-4.4.4/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.4/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.4/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:10:43.693373 johnsnowlabs-4.4.4/johnsnowlabs.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-04-26 21:10:43.000000 johnsnowlabs-4.4.4/johnsnowlabs.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-04-26 21:10:43.000000 johnsnowlabs-4.4.4/johnsnowlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-04-26 21:10:43.000000 johnsnowlabs-4.4.4/johnsnowlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-04-26 21:10:43.000000 johnsnowlabs-4.4.4/johnsnowlabs.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-04-26 21:10:43.000000 johnsnowlabs-4.4.4/johnsnowlabs.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-04-26 21:10:43.697373 johnsnowlabs-4.4.4/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2054 2023-04-26 21:10:35.000000 johnsnowlabs-4.4.4/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.5/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.5/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-04-13 00:38:10.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-04-26 21:13:04.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8828 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4526 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-4.4.5/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2201 2023-05-03 11:36:35.000000 johnsnowlabs-4.4.5/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4253 2023-04-26 21:13:04.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8019 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs-4.4.5/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.5/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.5/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-03 11:42:03.535852 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-05-03 11:42:03.000000 johnsnowlabs-4.4.5/johnsnowlabs.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-03 11:42:03.539852 johnsnowlabs-4.4.5/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2054 2023-04-26 21:10:35.000000 johnsnowlabs-4.4.5/setup.py
```

### Comparing `johnsnowlabs-4.4.4/LICENSE` & `johnsnowlabs-4.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/PKG-INFO` & `johnsnowlabs-4.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 4.4.4
+Version: 4.4.5
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-4.4.4/README.md` & `johnsnowlabs-4.4.5/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/__init__.py` & `johnsnowlabs-4.4.5/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs-4.4.5/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs-4.4.5/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/finance.py` & `johnsnowlabs-4.4.5/johnsnowlabs/finance.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/legal.py` & `johnsnowlabs-4.4.5/johnsnowlabs/legal.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/medical.py` & `johnsnowlabs-4.4.5/johnsnowlabs/medical.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/nlp.py` & `johnsnowlabs-4.4.5/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs-4.4.5/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs-4.4.5/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs-4.4.5/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs-4.4.5/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/settings.py` & `johnsnowlabs-4.4.5/johnsnowlabs/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from johnsnowlabs.utils.env_utils import (
     is_running_in_databricks,
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
-raw_version_jsl_lib = "4.4.4"
+raw_version_jsl_lib = "4.4.5"
 raw_version_nlp = "4.4.1"
 raw_version_nlu = "4.2.0"
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
-raw_version_medical = "4.4.0"
-raw_version_secret_medical = "4.4.0"
+raw_version_medical = "4.4.1"
+raw_version_secret_medical = "4.4.1"
 
 raw_version_secret_ocr = "4.4.0"
 raw_version_ocr = "4.4.0"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
 
 json_indent = 4
```

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/enums.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/functional.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/py_process.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs-4.4.5/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs/visual.py` & `johnsnowlabs-4.4.5/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs.egg-info/PKG-INFO` & `johnsnowlabs-4.4.5/johnsnowlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 4.4.4
+Version: 4.4.5
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-4.4.4/johnsnowlabs.egg-info/SOURCES.txt` & `johnsnowlabs-4.4.5/johnsnowlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.4/setup.py` & `johnsnowlabs-4.4.5/setup.py`

 * *Files identical despite different names*

