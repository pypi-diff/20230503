# Comparing `tmp/dapla_toolbelt-1.6.2.tar.gz` & `tmp/dapla_toolbelt-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt-1.6.2.tar", max compression
+gzip compressed data, was "dapla_toolbelt-1.7.0.tar", max compression
```

## Comparing `dapla_toolbelt-1.6.2.tar` & `dapla_toolbelt-1.7.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1074 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/LICENSE
--rw-r--r--   0        0        0     6602 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/README.md
--rw-r--r--   0        0        0      401 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/__init__.py
--rw-r--r--   0        0        0     2900 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/auth.py
--rw-r--r--   0        0        0     1576 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/backports.py
--rw-r--r--   0        0        0     1537 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/collector.py
--rw-r--r--   0        0        0     4120 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/converter.py
--rw-r--r--   0        0        0     4185 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/doctor.py
--rw-r--r--   0        0        0     5074 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/files.py
--rw-r--r--   0        0        0     1861 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/gcs.py
--rw-r--r--   0        0        0     2864 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/guardian.py
--rw-r--r--   0        0        0     1140 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/jupyterhub.py
--rw-r--r--   0        0        0     4499 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/pandas.py
--rw-r--r--   0        0        0     6031 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/pubsub.py
--rw-r--r--   0        0        0        0 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/spark/__init__.py
--rw-r--r--   0        0        0      378 2023-02-24 08:09:02.791864 dapla_toolbelt-1.6.2/dapla/spark/sparkui.py
--rw-r--r--   0        0        0     3139 2023-02-24 08:09:02.795865 dapla_toolbelt-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     7802 1970-01-01 00:00:00.000000 dapla_toolbelt-1.6.2/setup.py
--rw-r--r--   0        0        0     7778 1970-01-01 00:00:00.000000 dapla_toolbelt-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/LICENSE
+-rw-r--r--   0        0        0     6602 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/README.md
+-rw-r--r--   0        0        0      401 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/__init__.py
+-rw-r--r--   0        0        0     2900 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/auth.py
+-rw-r--r--   0        0        0     1576 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/backports.py
+-rw-r--r--   0        0        0     1537 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/collector.py
+-rw-r--r--   0        0        0     4120 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/converter.py
+-rw-r--r--   0        0        0     4185 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/doctor.py
+-rw-r--r--   0        0        0     5550 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/files.py
+-rw-r--r--   0        0        0     1861 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/gcs.py
+-rw-r--r--   0        0        0     2887 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/guardian.py
+-rw-r--r--   0        0        0     1140 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/jupyterhub.py
+-rw-r--r--   0        0        0     4322 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/pandas.py
+-rw-r--r--   0        0        0     6031 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/pubsub.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/spark/__init__.py
+-rw-r--r--   0        0        0      378 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/spark/sparkui.py
+-rw-r--r--   0        0        0     3139 2023-05-03 19:08:12.173093 dapla_toolbelt-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7778 1970-01-01 00:00:00.000000 dapla_toolbelt-1.7.0/PKG-INFO
```

### Comparing `dapla_toolbelt-1.6.2/LICENSE` & `dapla_toolbelt-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.2/README.md` & `dapla_toolbelt-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.2/dapla/auth.py` & `dapla_toolbelt-1.7.0/dapla/auth.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.2/dapla/backports.py` & `dapla_toolbelt-1.7.0/dapla/backports.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.2/dapla/collector.py` & `dapla_toolbelt-1.7.0/dapla/collector.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.2/dapla/converter.py` & `dapla_toolbelt-1.7.0/dapla/converter.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.2/dapla/doctor.py` & `dapla_toolbelt-1.7.0/dapla/doctor.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.2/dapla/files.py` & `dapla_toolbelt-1.7.0/dapla/files.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import pandas as pd
 
 from .auth import AuthClient
 from .gcs import GCSFileSystem
 
+GS_URI_PREFIX = "gs://"
+
 
 class FileClient:
     @staticmethod
     def _ensure_gcs_uri_prefix(gcs_path):
         """
         GCS uri is the gcs file path prefixed with 'gs://'. Some operations require GCS uris,
         but we don't want the user to bother with knowing when to use the prefix,
         so we ensure its presence automatically where it is needed
         :param gcs_path:
         :return:
         """
-        gs_uri_prefix = "gs://"
-        if not gcs_path.startswith(gs_uri_prefix):
-            gcs_path = f"{gs_uri_prefix}{gcs_path}"
+        if not gcs_path.startswith(GS_URI_PREFIX):
+            gcs_path = f"{GS_URI_PREFIX}{gcs_path}"
+        return gcs_path
+
+    @staticmethod
+    def _remove_gcs_uri_prefix(gcs_path):
+        """Remove the 'gs://' prefix from a GCS uri
+        :param gcs_path:
+        :return:
+        """
+        if gcs_path.startswith(GS_URI_PREFIX):
+            gcs_path = gcs_path[len(GS_URI_PREFIX) :]
         return gcs_path
 
     @staticmethod
     def get_gcs_file_system(**kwargs):
         """
         Return a pythonic file-system for Google Cloud Storage - initialized with a personal Google Identity token.
         See https://gcsfs.readthedocs.io/en/latest for usage
@@ -43,80 +54,102 @@
         Get string content of file from gcs
         :param gcs_path: path or paths to the file(s) you want to get the contents of
         :return: utf-8 decoded string content of the given file
         """
         return FileClient.get_gcs_file_system().cat(gcs_path).decode("utf-8")
 
     @staticmethod
-    def gcs_open(gcs_path, mode='r'):
+    def gcs_open(gcs_path, mode="r"):
         """
         Open a file in GCS, works like regular python open()
         :param gcs_path:
         :param mode:
         :return:
         """
-        return FileClient.get_gcs_file_system().open(FileClient._ensure_gcs_uri_prefix(gcs_path), mode)
+        return FileClient.get_gcs_file_system().open(
+            FileClient._ensure_gcs_uri_prefix(gcs_path), mode
+        )
 
     @staticmethod
     def load_csv_to_pandas(gcs_path, **kwargs):
         """
         Reads a csv file from google cloud storage into a Pandas data frame
         :param gcs_path: of the file, starting with the bucket name
         :return: a Pandas data frame
         """
-        return pd.read_csv(FileClient._ensure_gcs_uri_prefix(gcs_path),
-                           storage_options={"token": AuthClient.fetch_google_credentials()}, **kwargs)
+        return pd.read_csv(
+            FileClient._ensure_gcs_uri_prefix(gcs_path),
+            storage_options={"token": AuthClient.fetch_google_credentials()},
+            **kwargs,
+        )
 
     @staticmethod
     def load_json_to_pandas(gcs_path, **kwargs):
         """
         Reads a json file from google cloud storage into a Pandas data frame
         :param gcs_path: of the file, starting with the bucket name
         :return: a Pandas data frame
         """
-        return pd.read_json(FileClient._ensure_gcs_uri_prefix(gcs_path),
-                            storage_options={"token": AuthClient.fetch_google_credentials()}, **kwargs)
+        return pd.read_json(
+            FileClient._ensure_gcs_uri_prefix(gcs_path),
+            storage_options={"token": AuthClient.fetch_google_credentials()},
+            **kwargs,
+        )
 
     @staticmethod
     def load_xml_to_pandas(gcs_path, **kwargs):
         """
         Reads an xml file from google cloud storage into a Pandas data frame
         :param gcs_path: of the file, starting with the bucket name
         :return: a Pandas data frame
         """
-        return pd.read_xml(FileClient._ensure_gcs_uri_prefix(gcs_path),
-                           storage_options={"token": AuthClient.fetch_google_credentials()}, **kwargs)
+        return pd.read_xml(
+            FileClient._ensure_gcs_uri_prefix(gcs_path),
+            storage_options={"token": AuthClient.fetch_google_credentials()},
+            **kwargs,
+        )
 
     @staticmethod
     def save_pandas_to_csv(df: pd.DataFrame, gcs_path, index=False, **kwargs):
         """
         Write the contents of a Pandas data frame to a csv file in a bucket
         :param df: the Pandas data frame to persist as csv
         :param gcs_path: target path, starting with the bucket name and ending with the file name
         :param index: True if you want to write the pandas index to the file
         :return:
         """
-        df.to_csv(FileClient._ensure_gcs_uri_prefix(gcs_path),
-                  storage_options={"token": AuthClient.fetch_google_credentials()}, index=index, **kwargs)
+        df.to_csv(
+            FileClient._ensure_gcs_uri_prefix(gcs_path),
+            storage_options={"token": AuthClient.fetch_google_credentials()},
+            index=index,
+            **kwargs,
+        )
 
     @staticmethod
     def save_pandas_to_json(df: pd.DataFrame, gcs_path, **kwargs):
         """
         Write the contents of a Pandas data frame to a json file in a bucket
         :param df: the Pandas data frame to persist as json
         :param gcs_path: target path, starting with the bucket name and ending with the file name
         :return:
         """
-        df.to_json(FileClient._ensure_gcs_uri_prefix(gcs_path),
-                   storage_options={"token": AuthClient.fetch_google_credentials()}, **kwargs)
+        df.to_json(
+            FileClient._ensure_gcs_uri_prefix(gcs_path),
+            storage_options={"token": AuthClient.fetch_google_credentials()},
+            **kwargs,
+        )
 
     @staticmethod
     def save_pandas_to_xml(df: pd.DataFrame, gcs_path, index=False, **kwargs):
         """
         Write the contents of a Pandas data frame to an xml file in a bucket
         :param df: the Pandas data frame to persist as xml
         :param gcs_path: target path, starting with the bucket name and ending with the file name
         :param index: True if you want to write the pandas index to the file
         :return:
         """
-        df.to_xml(FileClient._ensure_gcs_uri_prefix(gcs_path),
-                  storage_options={"token": AuthClient.fetch_google_credentials()}, index=index, **kwargs)
+        df.to_xml(
+            FileClient._ensure_gcs_uri_prefix(gcs_path),
+            storage_options={"token": AuthClient.fetch_google_credentials()},
+            index=index,
+            **kwargs,
+        )
```

### Comparing `dapla_toolbelt-1.6.2/dapla/gcs.py` & `dapla_toolbelt-1.7.0/dapla/gcs.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.2/dapla/guardian.py` & `dapla_toolbelt-1.7.0/dapla/guardian.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 from .auth import AuthClient
 
 
 class GuardianClient:
     @staticmethod
     def call_api(api_endpoint_url: str, maskinporten_client_id: str, scopes: str,
-                 guardian_endpoint_url: str = 'https://guardian.dapla.ssb.no/maskinporten/access-token',
+                 guardian_endpoint_url: str = 'http://maskinporten-guardian.dapla.svc.cluster.local/maskinporten/access-token',
                  keycloak_token: str = None) -> Any:
         """
         Call an external API using the maskinporten guardian
         :param api_endpoint_url: URL to the target API
         :param maskinporten_client_id: the Maskinporten client id
         :param scopes: the Maskinporten scopes
         :param guardian_endpoint_url: URL to the Maskinporten Guardian
```

### Comparing `dapla_toolbelt-1.6.2/dapla/jupyterhub.py` & `dapla_toolbelt-1.7.0/dapla/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.2/dapla/pandas.py` & `dapla_toolbelt-1.7.0/dapla/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,26 @@
         methods like read_json, read_csv, etc.
     :param columns: If not None, only these columns will be read
     :return: a pandas dataframe
 
     Other arguments are passed through to the to_pandas method.
     """
     if file_format == "parquet":
-        import warnings
         import pyarrow.parquet as pq
 
         fs = FileClient.get_gcs_file_system()
 
-        # Suppress warning for use of legacy dataset
-        with warnings.catch_warnings():
-            warnings.simplefilter(action="ignore", category=FutureWarning)
-            parquet_ds = pq.ParquetDataset(
-                # use_legacy_dataset as workaround for https://github.com/apache/arrow/issues/30481
-                gcs_path,
-                filesystem=fs,
-                use_legacy_dataset=True,
-            )
+        # Workaround for https://github.com/apache/arrow/issues/30481
+        gcs_path = FileClient._remove_gcs_uri_prefix(gcs_path)
+
+        parquet_ds = pq.ParquetDataset(
+            gcs_path,
+            filesystem=fs,
+            use_legacy_dataset=False,
+        )
         return parquet_ds.read_pandas(columns=columns).to_pandas(
             split_blocks=False, self_destruct=True, **kwargs
         )
     elif file_format == "json":
         return read_json(gcs_path, storage_options=get_storage_options(), **kwargs)
     elif file_format == "csv":
         return read_csv(gcs_path, storage_options=get_storage_options(), **kwargs)
```

### Comparing `dapla_toolbelt-1.6.2/dapla/pubsub.py` & `dapla_toolbelt-1.7.0/dapla/pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,10 +162,10 @@
         source_name (str): The name of source that should process the files.
     """
 
     project_name = _extract_project_name(project_id)
 
     bucket_suffix = "-data-kilde"
     bucket_id = f"ssb-{project_name}{bucket_suffix}"
-    topic_id = f"{source_name}-update"
+    topic_id = f"update-{source_name}"
 
     _publish_gcs_objects_to_pubsub(project_id, bucket_id, folder_prefix, topic_id)
```

### Comparing `dapla_toolbelt-1.6.2/pyproject.toml` & `dapla_toolbelt-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt"
-version = "1.6.2"
+version = "1.7.0"
 description = "Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called Dapla"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt"
 
 classifiers = [
```

### Comparing `dapla_toolbelt-1.6.2/setup.py` & `dapla_toolbelt-1.7.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,197 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dapla-toolbelt
+Version: 1.7.0
+Summary: Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called Dapla
+Home-page: https://github.com/statisticsnorway/dapla-toolbelt
+License: MIT
+Author: Statistics Norway
+Author-email: stat-dev@ssb.no
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Typed
+Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
+Requires-Dist: gcsfs (>=2022.7.1)
+Requires-Dist: google-cloud-pubsub (>=2.14.1,<3.0.0)
+Requires-Dist: google-cloud-storage (>=2.7.0,<3.0.0)
+Requires-Dist: ipython (>=8.10.0,<9.0.0)
+Requires-Dist: jupyterhub (>=3.0.0,<4.0.0)
+Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Requires-Dist: pandas (>=1.4.2)
+Requires-Dist: pyarrow (>=8.0.0)
+Requires-Dist: pydantic (>=1.9.1)
+Requires-Dist: requests (>=2.27.1)
+Project-URL: Repository, https://github.com/statisticsnorway/dapla-toolbelt
+Description-Content-Type: text/markdown
 
-packages = \
-['dapla', 'dapla.spark']
+# dapla-toolbelt
 
-package_data = \
-{'': ['*']}
+Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called 
+`Dapla`. It contains support for authenticated access to Google Services such as Google Cloud Storage (GCS) and custom
+Dapla services such as [Maskinporten Guardian](https://github.com/statisticsnorway/maskinporten-guardian). The 
+authentication process is based on the [TokenExchangeAuthenticator](https://github.com/statisticsnorway/jupyterhub-extensions/tree/main/TokenExchangeAuthenticator)
+for Jupyterhub.
 
-install_requires = \
-['PyJWT>=2.6.0,<3.0.0',
- 'gcsfs>=2022.7.1',
- 'google-cloud-pubsub>=2.14.1,<3.0.0',
- 'google-cloud-storage>=2.7.0,<3.0.0',
- 'ipython>=8.10.0,<9.0.0',
- 'jupyterhub>=3.0.0,<4.0.0',
- 'lxml>=4.9.1,<5.0.0',
- 'pandas>=1.4.2',
- 'pyarrow>=8.0.0',
- 'pydantic>=1.9.1',
- 'requests>=2.27.1']
-
-setup_kwargs = {
-    'name': 'dapla-toolbelt',
-    'version': '1.6.2',
-    'description': "Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called Dapla",
-    'long_description': '# dapla-toolbelt\n\nPython module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway\'s data platform called \n`Dapla`. It contains support for authenticated access to Google Services such as Google Cloud Storage (GCS) and custom\nDapla services such as [Maskinporten Guardian](https://github.com/statisticsnorway/maskinporten-guardian). The \nauthentication process is based on the [TokenExchangeAuthenticator](https://github.com/statisticsnorway/jupyterhub-extensions/tree/main/TokenExchangeAuthenticator)\nfor Jupyterhub.\n\n[![PyPI version](https://img.shields.io/pypi/v/dapla-toolbelt.svg)](https://pypi.python.org/pypi/dapla-toolbelt/)\n![Unit tests](https://github.com/statisticsnorway/dapla-toolbelt/actions/workflows/unit-tests.yml/badge.svg) \n![Code coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/bjornandre/73205f2f30335801fa2819c31b3ecf79/raw/pytest-coverage-badge-dapla-toolbelt.json) \n![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)\n[![License](https://img.shields.io/pypi/l/dapla-toolbelt.svg)](https://pypi.python.org/pypi/dapla-toolbelt/)\n\nThese operations are supported:\n* List contents of a bucket\n* Open a file in GCS\n* Copy a file from GCS into local\n* Load a file (CSV, JSON or XML) from GCS into a pandas dataframe\n* Save contents of a data frame into a file (CSV, JSON, XML) in GCS\n\nWhen the user gives the path to a resource, they do not need to give the GCS uri, only the path. \nThis just means users don\'t have to prefix a path with "gs://". \nIt is implicitly understood that all resources accessed with this tool are located in GCS, \nwith the first level of the path being a GCS bucket name.\n\n## Installation\n\n`pip install dapla-toolbelt`\n\n## Usage Examples\n\n``` python\nfrom dapla import FileClient\nfrom dapla import GuardianClient\nimport pandas as pd\n\n# Load data using the Maskinporten Guardian client\nresponse = GuardianClient.call_api("https://data.udir.no/api/kag", "88ace991-7871-4ccc-aaec-8fb6d78ed04e", "udir:datatilssb")\ndata_json = response.json()\n\nraw_data_df = pd.DataFrame(data_json)  # create pandas data frame from json\nraw_data_df.head()  # show first rows of data frame\n\nFileClient.ls("bucket-name/folder")  # list contents of given folder\n\n# Save data into different formats\npath_base = "bucket-name/folder/raw_data"\nFileClient.save_pandas_to_json(raw_data_df, f"{path_base}.json")  # generate json from data frame, and save to given path\nFileClient.save_pandas_to_csv(raw_data_df, f"{path_base}.csv")  # generate csv from data frame, and save to given path\nFileClient.save_pandas_to_xml(raw_data_df, f"{path_base}.xml")  # generate xml from data frame, and save to given path\n\nFileClient.cat(f"{path_base}.json")  # print contents of file\n\n# Load data from different formats\n# All these data frames should contain the same data:\ndf = FileClient.load_json_to_pandas(f"{path_base}.json")  # read json from path and load into pandas data frame\ndf.head()  # show first rows of data frame\ndf = FileClient.load_csv_to_pandas(f"{path_base}.csv")  # read csv from path and load into pandas data frame\ndf.head()  # show first rows of data frame\ndf = FileClient.load_xml_to_pandas(f"{path_base}.xml")  # read xml from path and load into pandas data frame\ndf.head()  # show first rows of data frame\n\n```\n\n## Development\n\n### Prerequisites\n\n- Python >3.8 (3.10 is preferred)\n- Poetry, install via `curl -sSL https://install.python-poetry.org | python3 -`\n\nYou can also execute `make` in the project folder to see available `make` commands.\n\n### Dependency Management\n\nPoetry is used for dependency management. [Poe the Poet](https://github.com/nat-n/poethepoet) is used for running poe tasks within poetry\'s virtualenv. \nUpon cloning this project first install necessary dependencies, then run the tests to verify everything is working.\n\n#### Install all dependencies\n\n```shell\npoetry install\n```\n\n### Add dependencies\n\n#### Main\n\n```shell\npoetry add <python package name>\n```\n\n#### Dev\n\n```shell\npoetry add --group dev <python package name>\n```\n\n### Run tests\n\n```shell\npoetry run poe test\n```\n\n### Run project locally in Jupyter\n\nTo run the project locally in Jupyter run:\n\n```shell\npoetry run poe jupyter\n```\n\nA Jupyter instance should open in your browser. Open and run the cells in the `demo.ipynb` file.\n\n### Bumping version\n\nUse `make` to bump the *patch*, *minor* version or *major* version before creating a pull request to the `main` GIT branch.\nOr run a poe task like this:\n\n```shell\npoetry run poe bump-patch-version\n```\n\nYou can use either `bump-version-patch`, `bump-version-minor`, or `bump-version-major`.\nBumping must be done with a clean git working space, and automatically commits with the new version number.\n\nThen just run `git push origin --tags` to push the changes and trigger the release process.\n\n### Building and releasing\n\nBefore merging your changes into the `main` branch, make sure you have bumped the version like outlined above.\n\nAn automatic release process will build *dapla-toolbelt* upon pull request-creation, merges, and direct commits to the\n`main` GIT branch. It will also release a new version of the package to **pypi.org** automatically when a commit is \ntagged, for example by a GitHub release.\n\n### Building and releasing manually\n\nRun `make build` to build a wheel and a source distribution.\n\nRun `make release-validate` to do all that AND validate it for release.\n\nRun this (replacing <SEMVER> with your current version number) to check the contents of your wheel:\n`tar tzf dist/dapla-toolbelt-<SEMVER>.tar.gz`\n\n#### Test release\n\nYou have to bump the version of the package (see documentation on "Bumping version" above) before releasing, \nbecause even test.pypi.org does not allow re-releases of a previously released version.\n\nRun the following command in order to build, validate, and test package publication by uploading to TestPyPI:\n`make release-test`\n\nYou will have to manually enter a username and password for a user registered to [test.pypi.org](https://test.pypi.org) \nin order for this to work.\n\n#### Production release\n\n**NB: A manual production release should only be done as a last resort**, if the regular CI/CD pipeline \ndoes not work, and it\'s necessary to release regardless.\n\nYou have to bump the version of the package (see documentation on "Bumping version" above) to something \ndifferent from the last release before releasing.\n\nIn order to publish a new version of the package to PyPI for real, run `make release`. \nAuthenticate by manually entering your [pypi.org](https://pypi.org) username and password. \n',
-    'author': 'Statistics Norway',
-    'author_email': 'stat-dev@ssb.no',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/statisticsnorway/dapla-toolbelt',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+[![PyPI version](https://img.shields.io/pypi/v/dapla-toolbelt.svg)](https://pypi.python.org/pypi/dapla-toolbelt/)
+![Unit tests](https://github.com/statisticsnorway/dapla-toolbelt/actions/workflows/unit-tests.yml/badge.svg) 
+![Code coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/bjornandre/73205f2f30335801fa2819c31b3ecf79/raw/pytest-coverage-badge-dapla-toolbelt.json) 
+![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
+[![License](https://img.shields.io/pypi/l/dapla-toolbelt.svg)](https://pypi.python.org/pypi/dapla-toolbelt/)
 
+These operations are supported:
+* List contents of a bucket
+* Open a file in GCS
+* Copy a file from GCS into local
+* Load a file (CSV, JSON or XML) from GCS into a pandas dataframe
+* Save contents of a data frame into a file (CSV, JSON, XML) in GCS
+
+When the user gives the path to a resource, they do not need to give the GCS uri, only the path. 
+This just means users don't have to prefix a path with "gs://". 
+It is implicitly understood that all resources accessed with this tool are located in GCS, 
+with the first level of the path being a GCS bucket name.
+
+## Installation
+
+`pip install dapla-toolbelt`
+
+## Usage Examples
+
+``` python
+from dapla import FileClient
+from dapla import GuardianClient
+import pandas as pd
+
+# Load data using the Maskinporten Guardian client
+response = GuardianClient.call_api("https://data.udir.no/api/kag", "88ace991-7871-4ccc-aaec-8fb6d78ed04e", "udir:datatilssb")
+data_json = response.json()
+
+raw_data_df = pd.DataFrame(data_json)  # create pandas data frame from json
+raw_data_df.head()  # show first rows of data frame
+
+FileClient.ls("bucket-name/folder")  # list contents of given folder
+
+# Save data into different formats
+path_base = "bucket-name/folder/raw_data"
+FileClient.save_pandas_to_json(raw_data_df, f"{path_base}.json")  # generate json from data frame, and save to given path
+FileClient.save_pandas_to_csv(raw_data_df, f"{path_base}.csv")  # generate csv from data frame, and save to given path
+FileClient.save_pandas_to_xml(raw_data_df, f"{path_base}.xml")  # generate xml from data frame, and save to given path
+
+FileClient.cat(f"{path_base}.json")  # print contents of file
+
+# Load data from different formats
+# All these data frames should contain the same data:
+df = FileClient.load_json_to_pandas(f"{path_base}.json")  # read json from path and load into pandas data frame
+df.head()  # show first rows of data frame
+df = FileClient.load_csv_to_pandas(f"{path_base}.csv")  # read csv from path and load into pandas data frame
+df.head()  # show first rows of data frame
+df = FileClient.load_xml_to_pandas(f"{path_base}.xml")  # read xml from path and load into pandas data frame
+df.head()  # show first rows of data frame
+
+```
+
+## Development
+
+### Prerequisites
+
+- Python >3.8 (3.10 is preferred)
+- Poetry, install via `curl -sSL https://install.python-poetry.org | python3 -`
+
+You can also execute `make` in the project folder to see available `make` commands.
+
+### Dependency Management
+
+Poetry is used for dependency management. [Poe the Poet](https://github.com/nat-n/poethepoet) is used for running poe tasks within poetry's virtualenv. 
+Upon cloning this project first install necessary dependencies, then run the tests to verify everything is working.
+
+#### Install all dependencies
+
+```shell
+poetry install
+```
+
+### Add dependencies
+
+#### Main
+
+```shell
+poetry add <python package name>
+```
+
+#### Dev
+
+```shell
+poetry add --group dev <python package name>
+```
+
+### Run tests
+
+```shell
+poetry run poe test
+```
+
+### Run project locally in Jupyter
+
+To run the project locally in Jupyter run:
+
+```shell
+poetry run poe jupyter
+```
+
+A Jupyter instance should open in your browser. Open and run the cells in the `demo.ipynb` file.
+
+### Bumping version
+
+Use `make` to bump the *patch*, *minor* version or *major* version before creating a pull request to the `main` GIT branch.
+Or run a poe task like this:
+
+```shell
+poetry run poe bump-patch-version
+```
+
+You can use either `bump-version-patch`, `bump-version-minor`, or `bump-version-major`.
+Bumping must be done with a clean git working space, and automatically commits with the new version number.
+
+Then just run `git push origin --tags` to push the changes and trigger the release process.
+
+### Building and releasing
+
+Before merging your changes into the `main` branch, make sure you have bumped the version like outlined above.
+
+An automatic release process will build *dapla-toolbelt* upon pull request-creation, merges, and direct commits to the
+`main` GIT branch. It will also release a new version of the package to **pypi.org** automatically when a commit is 
+tagged, for example by a GitHub release.
+
+### Building and releasing manually
+
+Run `make build` to build a wheel and a source distribution.
+
+Run `make release-validate` to do all that AND validate it for release.
+
+Run this (replacing <SEMVER> with your current version number) to check the contents of your wheel:
+`tar tzf dist/dapla-toolbelt-<SEMVER>.tar.gz`
+
+#### Test release
+
+You have to bump the version of the package (see documentation on "Bumping version" above) before releasing, 
+because even test.pypi.org does not allow re-releases of a previously released version.
+
+Run the following command in order to build, validate, and test package publication by uploading to TestPyPI:
+`make release-test`
+
+You will have to manually enter a username and password for a user registered to [test.pypi.org](https://test.pypi.org) 
+in order for this to work.
+
+#### Production release
+
+**NB: A manual production release should only be done as a last resort**, if the regular CI/CD pipeline 
+does not work, and it's necessary to release regardless.
+
+You have to bump the version of the package (see documentation on "Bumping version" above) to something 
+different from the last release before releasing.
+
+In order to publish a new version of the package to PyPI for real, run `make release`. 
+Authenticate by manually entering your [pypi.org](https://pypi.org) username and password. 
 
-setup(**setup_kwargs)
```

