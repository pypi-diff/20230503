# Comparing `tmp/gn2pg_client-1.4.0.tar.gz` & `tmp/gn2pg_client-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gn2pg_client-1.4.0.tar", max compression
+gzip compressed data, was "gn2pg_client-1.5.0.tar", max compression
```

## Comparing `gn2pg_client-1.4.0.tar` & `gn2pg_client-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,33 @@
--rw-r--r--   0        0        0    34523 2023-02-08 23:50:04.385044 gn2pg_client-1.4.0/LICENSE
--rw-r--r--   0        0        0     7292 2023-02-08 23:50:04.385044 gn2pg_client-1.4.0/README.rst
--rw-r--r--   0        0        0     1059 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/__init__.py
--rw-r--r--   0        0        0     6977 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/api.py
--rw-r--r--   0        0        0    11087 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/check_conf.py
--rw-r--r--   0        0        0     1835 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/data/gn2pgconfig.toml
--rw-r--r--   0        0        0    78873 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/data/to_gnsynthese.sql
--rw-r--r--   0        0        0     8907 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/download.py
--rw-r--r--   0        0        0      241 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/env.py
--rw-r--r--   0        0        0     3968 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/helpers.py
--rw-r--r--   0        0        0     4100 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
--rw-r--r--   0        0        0     9305 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
--rwxr-xr-x   0        0        0     6063 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/main.py
--rw-r--r--   0        0        0      765 2023-02-08 23:50:04.389044 gn2pg_client-1.4.0/gn2pg/metadata.py
--rw-r--r--   0        0        0    20824 2023-02-08 23:50:04.393044 gn2pg_client-1.4.0/gn2pg/store_postgresql.py
--rw-r--r--   0        0        0     1387 2023-02-08 23:50:04.393044 gn2pg_client-1.4.0/gn2pg/utils.py
--rw-r--r--   0        0        0     2510 2023-02-08 23:50:04.393044 gn2pg_client-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     8622 1970-01-01 00:00:00.000000 gn2pg_client-1.4.0/setup.py
--rw-r--r--   0        0        0     8940 1970-01-01 00:00:00.000000 gn2pg_client-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-03 12:49:34.878197 gn2pg_client-1.5.0/LICENSE
+-rw-r--r--   0        0        0     7798 2023-05-03 12:49:34.878197 gn2pg_client-1.5.0/README.rst
+-rw-r--r--   0        0        0     1059 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/__init__.py
+-rw-r--r--   0        0        0     7124 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/api.py
+-rw-r--r--   0        0        0        0 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/__init__.py
+-rw-r--r--   0        0        0     1041 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/admin_views.py
+-rw-r--r--   0        0        0     1391 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/app.py
+-rw-r--r--   0        0        0     1942 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/config.py
+-rw-r--r--   0        0        0      456 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/database.py
+-rw-r--r--   0        0        0      240 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/env.py
+-rw-r--r--   0        0        0      202 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/index.py
+-rw-r--r--   0        0        0     1953 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/models.py
+-rw-r--r--   0        0        0      216 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/static/css/custom_flaks_admin.css
+-rw-r--r--   0        0        0    30240 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/static/img/src_gn2pg.png
+-rw-r--r--   0        0        0      185 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/app/templates/admin/master.html
+-rw-r--r--   0        0        0      353 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/app/templates/index.html
+-rw-r--r--   0        0        0        0 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/app/utils/__init__.py
+-rw-r--r--   0        0        0      582 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/app/utils/admin_views.py
+-rw-r--r--   0        0        0    11145 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/check_conf.py
+-rw-r--r--   0        0        0     1835 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/data/gn2pgconfig.toml
+-rw-r--r--   0        0        0    78873 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/data/to_gnsynthese.sql
+-rw-r--r--   0        0        0     8944 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/download.py
+-rw-r--r--   0        0        0      241 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/env.py
+-rw-r--r--   0        0        0     3968 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/helpers.py
+-rw-r--r--   0        0        0     4100 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
+-rw-r--r--   0        0        0    10575 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
+-rw-r--r--   0        0        0    10307 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~
+-rwxr-xr-x   0        0        0     6063 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/main.py
+-rw-r--r--   0        0        0      765 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/metadata.py
+-rw-r--r--   0        0        0    20834 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/store_postgresql.py
+-rw-r--r--   0        0        0     1387 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/utils.py
+-rw-r--r--   0        0        0     3169 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9874 1970-01-01 00:00:00.000000 gn2pg_client-1.5.0/PKG-INFO
```

### Comparing `gn2pg_client-1.4.0/LICENSE` & `gn2pg_client-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.4.0/README.rst` & `gn2pg_client-1.5.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 **************
  GN2PG Client
 **************
 
-.. image:: https://img.shields.io/badge/python-3.7+-yellowgreen
+.. image:: https://img.shields.io/badge/python-3.8+-yellowgreen
    :target: https://www.python.org/
 .. image:: https://img.shields.io/badge/PostgreSQL-10+-blue
    :target: https://www.postgresql.org/
 .. image:: https://img.shields.io/badge/packaging%20tool-poetry-important
    :target: https://python-poetry.org/
 .. image:: https://img.shields.io/badge/code%20style-black-black
    :target: https://github.com/psf/black
@@ -14,14 +14,17 @@
    :target: https://opensource.org/licenses/AGPL-3.0
 .. image:: https://app.fossa.com/api/projects/git%2Bgithub.com%2Flpoaura%2FGN2PG.svg?type=shield
    :target: https://app.fossa.com/projects/git%2Bgithub.com%2Flpoaura%2FGN2PG?ref=badge_shield
 
 This project provides an import data from GeoNature_ instances to a PostgreSQL database (client side).
 Widely inspired from `ClientApiVN <https://framagit.org/lpo/Client_API_VN/>`_
 
+.. tip::
+
+    The minimum version of the source GeoNature instance required for the incremental update must be a version 2.12.0
 
 .. contents:: Topics
 
 .. image:: ./docs/source/_static/src_gn2pg.png
     :align: center
     :alt: Project logo
 
@@ -154,50 +157,66 @@
 
 .. code-block:: cron
 
     */30 * * * * /usr/bin/env bash -c "source <path to python environment>/bin/activate && gn2pg_cli --update <myconfigfile>" > /dev/null 2>&1
 
 
 Debug mode
-############
+##########
 
 Debug mode can be activated using ``--verbose`` CLI argument
 
 Logs
 ####
 
 Log files are stored in ``$HOME/.gn2pg/log`` directory.
 
-Import datas into GeoNature datas
-#################################
+Import datas into GeoNature database
+####################################
 
 Default script to auto populate GeoNature is called "to_gnsynthese".
 
 .. code-block:: bash
 
     gn2pg_cli --custom-script to_gnsynthese <myconfigfile>
 
 
 .. tip::
 
     You can also replacing synthese script by your own scripts, using file path instead of ``to_gnsynthese``.
 
 
+Dashboard
+=========
+
+A simple web dashboard can be run following `dashboard docs <./docs/dashboard.rst>`_.
+
+.. image:: ./docs/_static/home_gn2pg_dashboard.png
+    :align: center
+    :alt: Dashboard_Home
+
+
+
+.. image:: ./docs/_static/src_gn2pg_dashboard.png
+    :align: center
+    :alt: Dashboard_gn2pg_downloag_log
+
 Contributing
 ============
 
 All devs must be done in forks (see `GitHub doc <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`_).
 
 Pull requests must be pulled to `dev` branch.
 
 Install project and development requirements (require `poetry <https://python-poetry.org/>`_):
 
 .. code-block:: bash
 
-    poetry install
+    poetry install --with=docs --all-extras
+    poetry run pre-commit install
 
 Make your devs and pull requests.
 
 Test `gn2pg_cli` in dev mode by running this command:
 
 .. code-block:: bash
```

### Comparing `gn2pg_client-1.4.0/gn2pg/__init__.py` & `gn2pg_client-1.5.0/gn2pg/__init__.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.4.0/gn2pg/api.py` & `gn2pg_client-1.5.0/gn2pg/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - APIException    - General exception
 - HTTPError                  - HTTP protocol error
 
 """
 import json
 import logging
 import math
-from typing import Optional
+from typing import List, Optional
 from urllib.parse import urlencode
 
 import requests
 
 from gn2pg import _, __version__
 
 logger = logging.getLogger(__name__)
@@ -34,15 +34,21 @@
     """An HTTP error occurred."""
 
 
 class BaseAPI:
     """Top class, not for direct use.
     Provides internal and template methods to use GeoNature API."""
 
-    def __init__(self, config, controler, max_retry=None, max_requests=None):
+    def __init__(
+        self,
+        config,
+        controler,
+        max_retry: Optional[int] = None,
+        max_requests: Optional[int] = None,
+    ):
         self._config = config
         if max_retry is None:
             max_retry = config.max_retry
         if max_requests is None:
             max_requests = config.max_requests
         self._limits = {"max_retry": max_retry, "max_requests": max_requests}
         self._transfer_errors = 0
@@ -50,24 +56,21 @@
         self._ctrl = controler
         logger.debug(_("controler is %s"), self._ctrl)
         self._api_url = config.url + "/" * (not config.url.endswith("/")) + "api/"
 
         # init session
         self._session = requests.Session()
         self._session.headers = {"Content-Type": "application/json"}
-        auth_payload = json.dumps(
-            {
-                "login": config.user_name,
-                "password": config.user_password,
-                "id_application": config.id_application,
-            }
-        )
+        auth_payload = {
+            "login": config.user_name,
+            "password": config.user_password,
+        }
         login = self._session.post(
             self._api_url + "auth/login",
-            data=auth_payload,
+            json=auth_payload,
         )
         try:
             if login.status_code == 200:
                 logger.info(
                     "Successfully logged in into GeoNature named %s",
                     self._config.name,
                 )
@@ -89,15 +92,15 @@
         try:
             modules_list = self._session.get(self._api_url + "gn_commons/modules")
             logger.info(
                 _("Modules API status code is %s for url %s"),
                 modules_list.status_code,
                 modules_list.url,
             )
-            if modules_list.status_code == 200:
+            if modules_list.status_code == 200 and "login?next=" not in modules_list.url:
                 modules = json.loads(modules_list.content)
                 for item in modules:
                     if item["module_code"] == "EXPORTS":
                         self._export_api_path = item["module_path"]
                         logger.debug(_("Export api path is %s"), self._export_api_path)
                         break
             else:
@@ -123,19 +126,19 @@
 
     @property
     def http_status(self) -> int:
         """Return the latest HTTP status code."""
         return self._http_status
 
     @property
-    def controler(self) -> str:
+    def controler(self) -> Optional[str]:
         """Return the controler name."""
         return self._ctrl
 
-    def _url(self, kind: str = "data", params: dict = None) -> str:
+    def _url(self, kind: str = "data", params: Optional[dict] = None) -> Optional[str]:
         """Generate export API URL with QueryStrings if params.
 
         Args:
             params (dict, optional): dict of querystring parameters. Defaults to None.
 
         Returns:
             str: export API URL.
@@ -151,22 +154,23 @@
             url = url + "?" + urlencode(params)
         return url
 
     def page_list(
         self,
         params: dict,
         kind: str = "data",
-    ) -> Optional[list]:
+    ) -> Optional[List[str]]:
         """List offset pages to download data, based on API "total_filtered" and "limit" values
 
-        Args:
-            **kwargs : Keyword args to filter data from API (cf. swagger API doc)
-
-        Returns:
-            list: url page list
+        :param params: Querystrings
+        :type params: dict
+        :param kind: kind of data, defaults to "data"
+        :type kind: str, optional
+        :return: url page list
+        :rtype: Optional[List[str]]
         """
         # GET from API
         session = self._session
 
         # Check kind value
         if self._url(kind) is None:
             return None
@@ -217,9 +221,9 @@
             logger.critical(str(error))
             return None
 
 
 class DataAPI(BaseAPI):
     """Data API"""
 
-    def __init__(self, config, max_retry=None, max_requests=None):
+    def __init__(self, config, max_retry: int = None, max_requests: int = None):
         super().__init__(config, "data", max_retry, max_requests)
```

### Comparing `gn2pg_client-1.4.0/gn2pg/check_conf.py` & `gn2pg_client-1.5.0/gn2pg/check_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """TOML validation tools"""
 
 import logging
 from dataclasses import dataclass, field
 from typing import Any, Dict
+from typing import Optional as TypeOptional
 
 from schema import Optional, Schema
 from toml import load
 
 from gn2pg import _, __version__
 from gn2pg.env import ENVDIR
 from gn2pg.utils import coalesce_in_dict, simplify
@@ -72,15 +73,15 @@
 class Db:
     """Database connection settings"""
 
     host: str
     user: str
     password: str
     name: str
-    port: str = 5432
+    port: int = 5432
     schema_import: str = "gn2pg_import"
     querystring: dict = field(default_factory=dict)
 
 
 @dataclass
 class Source:
     """Source connection settings"""
@@ -89,15 +90,15 @@
     user_name: str
     user_password: str
     url: str
     export_id: int
     data_type: str
     id_application: int = 3
     enable: bool = True
-    last_action_date: str = None
+    last_action_date: TypeOptional[str] = None
     query_strings: dict = field(default_factory=dict)
 
 
 @dataclass
 class Tuning:
     """Tuning settings"""
 
@@ -109,15 +110,15 @@
     lru_maxsize: int = 32
     nb_threads: int = 1
 
 
 class Gn2PgSourceConf:
     """Source conf generator"""
 
-    def __init__(self, source: str, config: _ConfType) -> None:
+    def __init__(self, source: int, config: _ConfType) -> None:
         self._selected_source = source
         try:
             # Source configs
             self._source = Source(
                 name=config["source"][source]["name"],
                 user_name=config["source"][source]["user_name"],
                 user_password=config["source"][source]["user_password"],
@@ -160,15 +161,15 @@
                 )
 
         except Exception:  # pragma: no cover
             logger.exception(_("Error creating %s configuration"), source)
             raise
 
     @property
-    def source(self) -> str:
+    def source(self) -> int:
         """Return source list position, used to identify source configuration in config file.
 
         Returns:
             int: Return source list position
         """
         return self._selected_source
```

### Comparing `gn2pg_client-1.4.0/gn2pg/data/gn2pgconfig.toml` & `gn2pg_client-1.5.0/gn2pg/data/gn2pgconfig.toml`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.4.0/gn2pg/data/to_gnsynthese.sql` & `gn2pg_client-1.5.0/gn2pg/data/to_gnsynthese.sql`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.4.0/gn2pg/download.py` & `gn2pg_client-1.5.0/gn2pg/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 import logging
 from datetime import datetime
 from functools import partial
 from multiprocessing import Queue
 from multiprocessing.pool import ThreadPool
 from threading import Thread
-from typing import Callable
+from typing import Callable, Optional
 
 from gn2pg import _, __version__
 from gn2pg.api import DataAPI
 
 logger = logging.getLogger(__name__)
 
 
@@ -106,15 +106,15 @@
                         response["total_len"],
                         perc_progress,
                         self._config.name,
                         self._api_instance.controler,
                     )
 
         # The Queue enables the report thread to get the progress from other threads
-        queue = Queue()
+        queue: Queue = Queue()
         # Initialize and start the report thread
         thread = Thread(target=report, args=[queue])
         thread.start()
         # Start the worker threads
         with ThreadPool(nb_threads) as thread:
             thread.map(partial(func, queue=queue), pages)
         # Will stop the report thread
@@ -200,15 +200,15 @@
         )
 
         self.launch_treads(nb_threads=self._config.nb_threads, func=self.download, pages=pages)
 
         # Log download timestamp to download.
         self._backend.increment_log(controler=self._api_instance.controler, last_ts=increment_ts)
 
-    def update(self, since: str = None, actions: list = None) -> None:
+    def update(self, since: Optional[str] = None, actions: Optional[list] = None) -> None:
         """[summary]
 
         Args:
             since (str): DateTime limit to update.
 
         Returns:
             [type]: [description]
```

### Comparing `gn2pg_client-1.4.0/gn2pg/helpers.py` & `gn2pg_client-1.5.0/gn2pg/helpers.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.4.0/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po` & `gn2pg_client-1.5.0/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.4.0/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po` & `gn2pg_client-1.5.0/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,77 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
-"POT-Creation-Date: 2023-02-07 21:56+0100\n"
+"POT-Creation-Date: 2023-04-18 22:47+0200\n"
 "PO-Revision-Date: 2023-02-07 21:16+0100\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 "X-Generator: Poedit 3.0.1\n"
 
-#: gn2pg/api.py:51
+#: gn2pg/api.py:57
 msgid "controler is %s"
 msgstr "Le controlleur est %s"
 
-#: gn2pg/api.py:96
+#: gn2pg/api.py:98
 msgid "Modules API status code is %s for url %s"
 msgstr "Le code d'état de l'API des modules est %s pour l'url %s"
 
+#: gn2pg/api.py:107
+msgid "Export api path is %s"
+msgstr ""
+
 #: gn2pg/api.py:111
 msgid "Get GeoNature modules failed with status code %s, cause: %s"
 msgstr ""
 "La récupération des modules GeoNature a échoué avec le code d'état %s, "
 "cause : %s"
 
-#: gn2pg/api.py:119
+#: gn2pg/api.py:117
 msgid "Find export module failed, %s"
 msgstr "La recherche du module d'exportation a échoué, %s"
 
-#: gn2pg/api.py:186
+#: gn2pg/api.py:184
 msgid "Defining page_list from %s with status code %s"
 msgstr "Définition de la page_list à partir de %s avec le code d'état %s"
 
-#: gn2pg/api.py:196
+#: gn2pg/api.py:194
 msgid "API %s contains %s data in %s page(s)"
 msgstr "API %s contient %s données dans %s page(s)"
 
-#: gn2pg/api.py:208
+#: gn2pg/api.py:202
 #, fuzzy
 msgid "No data available from from %s"
 msgstr "Aucune donnée disponible à partir de %s"
 
-#: gn2pg/api.py:222
+#: gn2pg/api.py:216
 msgid "Download page %s"
 msgstr "Téléchargement de la page %s"
 
-#: gn2pg/api.py:228
+#: gn2pg/api.py:222
 msgid "Download data from %s failed"
 msgstr "Le téléchargement des données depuis %s a échoué"
 
-#: gn2pg/check_conf.py:173
+#: gn2pg/app/app.py:23
+msgid "Home"
+msgstr "Accueil"
+
+#: gn2pg/app/config.py:28
+msgid "%s file doesn't exist. Check the filename at the path %s"
+msgstr "Le fichier %s n'existe pas. Vérifier le nom du fichier du chemin %s"
+
+#: gn2pg/check_conf.py:164
 msgid "Error creating %s configuration"
 msgstr "Erreur durant la création de la configuration %s"
 
 #: gn2pg/check_conf.py:353
 msgid "File %s does not exist"
 msgstr "Le fichier %s n'existe pas"
 
@@ -75,113 +87,117 @@
 msgid "Source \"%s\" identifier will be \"%s\""
 msgstr "L'identifiant de la source  \"%s\" sera \"%s\""
 
 #: gn2pg/check_conf.py:381
 msgid "Source #%s named \"%s\" (->%s) already used by another source"
 msgstr "Le nom de source #%s nommée \"%s\" (->%s) est déjà utilisé"
 
-#: gn2pg/check_conf.py:392
+#: gn2pg/check_conf.py:389
 msgid "Settings for %s are : %s"
 msgstr "Les paramètres de %s sont : %s"
 
-#: gn2pg/download.py:200
+#: gn2pg/download.py:157
+#, fuzzy
+msgid "No new deleted data from %s %s"
+msgstr "Pas de nouvelles données supprimées depuis %s %s"
+
+#: gn2pg/download.py:191
 msgid "Getting items from controler %s"
 msgstr "Récupération des éléments du contrôleur %s"
 
-#: gn2pg/download.py:204 gn2pg/download.py:250
+#: gn2pg/download.py:194 gn2pg/download.py:235
 msgid "QueryStrings %s"
 msgstr "Chaînes de requête %s"
 
-#: gn2pg/download.py:232
+#: gn2pg/download.py:217
 msgid "Updating items from controler %s"
 msgstr "Mise à jour des éléments du contrôleur %s"
 
-#: gn2pg/download.py:253
+#: gn2pg/download.py:238
 msgid "Getting new or update data from source %s since %s"
-msgstr ""
-"Obtention de données nouvelles ou mises à jour de la source %s depuis %s"
+msgstr "Obtention de données nouvelles ou mises à jour de la source %s depuis %s"
 
-#: gn2pg/download.py:271
+#: gn2pg/download.py:254
 msgid "Preparing data delete from source %s since %s"
 msgstr "Préparation de la suppression des données de la source %s depuis %s"
 
 #: gn2pg/helpers.py:37
 msgid "Conf directory %s created"
 msgstr "Dossier de configuration %s créée"
 
 #: gn2pg/helpers.py:38
 msgid "%s file already exists"
 msgstr "Le fichier %s existe déjà"
 
-#: gn2pg/helpers.py:44
+#: gn2pg/helpers.py:48
 msgid "File %s will be preserved"
 msgstr "Le fichier %s sera conservé"
 
-#: gn2pg/helpers.py:47
+#: gn2pg/helpers.py:51
 msgid "file %s will be overwritten"
 msgstr "Le fichier %s sera remplacé"
 
-#: gn2pg/helpers.py:49
+#: gn2pg/helpers.py:52
 #, fuzzy
 msgid "Creating TOML configuration file %s, from %s"
 msgstr "Chargement de la configuration TOML %s"
 
-#: gn2pg/helpers.py:52
+#: gn2pg/helpers.py:54
 msgid "Please edit %s before running the script"
 msgstr "Veuillez éditer %s avant d'éxécuter une autre action"
 
-#: gn2pg/helpers.py:73
+#: gn2pg/helpers.py:75
 msgid "%s => Starting download using controler %s"
 msgstr "%s => Démarrage du téléchargement à l'aide du contrôleur %s"
 
-#: gn2pg/helpers.py:79
+#: gn2pg/helpers.py:81
 msgid "%s => Ending download using controler %s"
 msgstr "%s => Fin du téléchargement en utilisant le contrôleur %s"
 
-#: gn2pg/helpers.py:91 gn2pg/helpers.py:133
+#: gn2pg/helpers.py:93 gn2pg/helpers.py:134
 msgid "Defining full download jobs"
 msgstr "Définition des tâches de téléchargement complet"
 
-#: gn2pg/helpers.py:94
+#: gn2pg/helpers.py:96
 msgid "Starting full download for source %s"
 msgstr "Démarrage du téléchargement complet de la source %s"
 
-#: gn2pg/helpers.py:98 gn2pg/helpers.py:139
+#: gn2pg/helpers.py:99 gn2pg/helpers.py:140
 msgid "Source %s is disabled"
 msgstr "La source %s est désactivée"
 
-#: gn2pg/helpers.py:108
+#: gn2pg/helpers.py:109
 msgid "config source name %s"
 msgstr "Le nom de la source de configuration est %s"
 
-#: gn2pg/helpers.py:109
+#: gn2pg/helpers.py:110
 msgid "controler %s"
 msgstr "Controlleur %s"
 
-#: gn2pg/helpers.py:113
+#: gn2pg/helpers.py:114
 msgid "%s => Starting updating using controler %s"
 msgstr "%s => Démarrage de la mise à jour à l'aide du contrôleur %s"
 
-#: gn2pg/helpers.py:119
+#: gn2pg/helpers.py:120
 msgid "%s => Ending updating using controler %s"
 msgstr "%s => Fin de la mise à jour à l'aide du contrôleur %s"
 
-#: gn2pg/helpers.py:136
+#: gn2pg/helpers.py:137
 msgid "Starting update download for source %s"
 msgstr "Démarrage du téléchargement de la mise à jour pour la source %s"
 
-#: gn2pg/main.py:37
+#: gn2pg/main.py:39
 msgid "Print version number"
 msgstr "Affichage du numéro de version"
 
-#: gn2pg/main.py:45
+#: gn2pg/main.py:47
 msgid "Increase output verbosity"
 msgstr "Augmenter la verbosité de la sortie"
 
-#: gn2pg/main.py:49
+#: gn2pg/main.py:50
 msgid "Reduce output verbosity"
 msgstr "Réduire la verbosité de la sortie"
 
 #: gn2pg/main.py:53
 msgid "Initialize the TOML configuration file"
 msgstr "Initialisation du fichier de configuration TOML"
 
@@ -200,116 +216,137 @@
 "of \"to_gnsynthese\""
 msgstr ""
 "Exécute un script SQL personnalisé dans la base de données, la valeur par "
 "défaut est \"to_gnsynthese\".\n"
 "        Vous pouvez également utiliser votre propre script en utilisant le "
 "chemin de fichier absolu à la place de \"to_gnsynthese\""
 
-#: gn2pg/main.py:77
+#: gn2pg/main.py:76
 msgid "Perform a full download"
 msgstr "Effectuer un téléchargement complet"
 
-#: gn2pg/main.py:81
+#: gn2pg/main.py:79
 msgid "Perform an incremental download"
 msgstr "Effectuer un téléchargement incrémentiel"
 
-#: gn2pg/main.py:139
+#: gn2pg/main.py:138
 msgid "%s, version %s"
 msgstr "%s, version %s"
 
-#: gn2pg/main.py:145
+#: gn2pg/main.py:144
 #, fuzzy
 msgid "Creating TOML configuration file"
 msgstr "Chargement de la configuration TOML %s"
 
-#: gn2pg/main.py:151
+#: gn2pg/main.py:150
 #, fuzzy
 msgid "Editing TOML configuration file"
 msgstr "Chargement de la configuration TOML %s"
 
-#: gn2pg/main.py:158
+#: gn2pg/main.py:156
 #, fuzzy
 msgid "Configuration file %s does not exist"
 msgstr "Le fichier %s n'existe pas"
 
-#: gn2pg/main.py:161
+#: gn2pg/main.py:158
 #, fuzzy
 msgid "Getting configuration data from %s"
 msgstr "Chargement de la configuration TOML %s"
 
-#: gn2pg/main.py:166
+#: gn2pg/main.py:162
 #, fuzzy
 msgid "Incorrect content in TOML configuration %s"
 msgstr "Contenu incorrect dans la configuration YAML %s : %s"
 
-#: gn2pg/main.py:172
+#: gn2pg/main.py:167
 msgid "config file have {len(cfg_source_list)} source(s) wich are : %s"
 msgstr ""
 
-#: gn2pg/main.py:179
+#: gn2pg/main.py:174
 #, fuzzy
 msgid "Create, if not exists, json tables"
 msgstr "Créer ou recréer des tables json"
 
-#: gn2pg/main.py:183
+#: gn2pg/main.py:178
 msgid "Execute custom script %s on db"
 msgstr "Exécution du script personnalisé %s sur la base de données"
 
-#: gn2pg/main.py:187
+#: gn2pg/main.py:182
 #, fuzzy
 msgid "Perform full action"
 msgstr "Effectuer un téléchargement complet"
 
-#: gn2pg/main.py:191
+#: gn2pg/main.py:186
 msgid "Perform update action"
 msgstr "Effectuer une action de mise à jour"
 
-#: gn2pg/store_postgresql.py:223
+#: gn2pg/store_postgresql.py:205
 #, fuzzy
 msgid "Connecting to %s database, to finalize creation"
 msgstr "Connexion à la base de données %s"
 
-#: gn2pg/store_postgresql.py:236 gn2pg/store_postgresql.py:247
+#: gn2pg/store_postgresql.py:218 gn2pg/store_postgresql.py:229
 msgid "Execute: %s"
 msgstr "Exécuter: %s"
 
-#: gn2pg/store_postgresql.py:252
+#: gn2pg/store_postgresql.py:233
 msgid "Schema %s owned by %s successfully created"
 msgstr "Le schéma %s appartenant à %s a été créé avec succès."
 
-#: gn2pg/store_postgresql.py:259
+#: gn2pg/store_postgresql.py:240
 msgid "Failed to create %s schema"
 msgstr "Échec de la création du schéma %s"
 
-#: gn2pg/store_postgresql.py:287
+#: gn2pg/store_postgresql.py:265
 msgid "Counting datas in database for all sources"
 msgstr "Comptage des données dans la base de données pour toutes les sources"
 
-#: gn2pg/store_postgresql.py:289 gn2pg/store_postgresql.py:361
+#: gn2pg/store_postgresql.py:267
 msgid "Connecting to database %s"
 msgstr "Connexion à la base de données %s"
 
-#: gn2pg/store_postgresql.py:312
+#: gn2pg/store_postgresql.py:287
 msgid "Start to execute %s script"
 msgstr "Lancement de l'exécution du script %s"
 
-#: gn2pg/store_postgresql.py:321
+#: gn2pg/store_postgresql.py:292
 msgid "You choosed to use internal to_gnsynthese.sql script in schema %s"
 msgstr ""
 "Vous avez choisi d'utiliser le script interne to_gnsynthese.sql dans le "
 "schéma %s"
 
-#: gn2pg/store_postgresql.py:328
+#: gn2pg/store_postgresql.py:297
 msgid "file %s exists, continue"
 msgstr "le fichier %s existe, continuer"
 
-#: gn2pg/store_postgresql.py:331
+#: gn2pg/store_postgresql.py:300
 msgid "file %s DO NOT EXISTS, exit"
 msgstr "le fichier %s N'EXISTE PAS, quitter"
 
-#: gn2pg/store_postgresql.py:344
+#: gn2pg/store_postgresql.py:310
 msgid "script %s successfully applied"
 msgstr "script %s appliqué avec succès"
 
-#: gn2pg/store_postgresql.py:386
+#: gn2pg/store_postgresql.py:342
 msgid "Entry into StorePostgresql"
 msgstr "Entrée dans StorePostgresql"
+
+#: gn2pg/store_postgresql.py:393
+msgid ""
+"One error occured for data from source %s with %s = %s. Error message is %s"
+msgstr ""
+
+#: gn2pg/store_postgresql.py:431
+#, fuzzy
+msgid "One error occurred for data from source %s with %s = %s"
+msgstr ""
+"Obtention de données nouvelles ou mises à jour de la source %s depuis %s"
+
+#: gn2pg/store_postgresql.py:437
+msgid ""
+"%s items have been stored in db from %s of source %s (%s error occurred)"
+msgstr ""
+
+#: gn2pg/store_postgresql.py:469
+#, fuzzy
+msgid "Deleting item with id %s from source %s (controler %s)"
+msgstr "Récupération des éléments du contrôleur %s"
```

### Comparing `gn2pg_client-1.4.0/gn2pg/main.py` & `gn2pg_client-1.5.0/gn2pg/main.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.4.0/gn2pg/metadata.py` & `gn2pg_client-1.5.0/gn2pg/metadata.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.4.0/gn2pg/store_postgresql.py` & `gn2pg_client-1.5.0/gn2pg/store_postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
         return del_count
 
     def download_log(
         self,
         controler: str,
         error_count: int = 0,
         http_status: int = 0,
-        comment: str = None,
+        comment: Optional[str] = None,
     ):
         """Write download log entries to database.
 
         Args:
             source (str): GeoNature source name.
             controler (str): Name of API controler.
             error_count (int, optional): Number of errors during download. Defaults to 0.
```

### Comparing `gn2pg_client-1.4.0/gn2pg/utils.py` & `gn2pg_client-1.5.0/gn2pg/utils.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.4.0/pyproject.toml` & `gn2pg_client-1.5.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,82 @@
 [tool.poetry]
 name = "gn2pg_client"
-packages = [
-    { include = "gn2pg" },
-]
-version = "1.4.0"
+packages = [{ include = "gn2pg" }]
+version = "1.5.0"
 description = "Import tool from GeoNature to a PostgreSQL database through Export module API (client side)"
 authors = ["lpofredc <frederic.cloitre@lpo.fr>"]
 maintainers = ["lpofredc <frederic.cloitre@lpo.fr>"]
 license = "AGPL-3.0-or-later"
 readme = "README.rst"
 homepage = "https://github.com/lpoaura/gn2gn_client/"
 keywords = ["GeoNature", "Export", "SINP", "opendata", "biodiversity"]
-classifiers= [
-        "Development Status :: 1 - Planning",
-        "Environment :: Console",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: GNU Affero General Public License v3",
-        "Natural Language :: French",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: Implementation :: PyPy",
-        "Topic :: Documentation",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: System :: Installation/Setup",
-        "Topic :: System :: Software Distribution",
-    ]
+classifiers = [
+    "Development Status :: 1 - Planning",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "Natural Language :: French",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "Topic :: Documentation",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: System :: Installation/Setup",
+    "Topic :: System :: Software Distribution",
+]
 
 [tool.poetry.scripts]
 gn2pg_cli = "gn2pg.main:run"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 requests = "^2.28.2"
 psycopg2-binary = "^2.9.5"
 coloredlogs = "^15.0.1"
 schema = "^0.7.5"
 toml = "^0.10.2"
 sqlalchemy = "^1.4.46"
-
+flask = { version = "^2.2.3", optional = true }
+flask-sqlalchemy = { version = "^3.0.3", optional = true }
+flask-admin = { version = "^1.6.1", optional = true }
+gunicorn = { version = "^20.1.0", optional = true }
+python-decouple = { version = "^3.8", optional = true }
+python-dotenv = { version = "^1.0.0", optional = true }
+
+[tool.poetry.extras]
+dashboard = [
+    'flask',
+    'flask-sqlalchemy',
+    'flask-admin',
+    'gunicorn',
+    'python-decouple',
+    'python-dotenv',
+]
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 coverage = "^7.0.3"
 pylint = "^2.6.0"
 mypy = "^0.991"
 tox = "^4.2.3"
 isort = "^5.11.4"
-sphinx-rtd-theme = "^0.5.0"
 pre-commit = "^2.21.0"
 black = "^22.12.0"
 click = "^8.1.3"
+types-setuptools = "^67.2.0.0"
+no-implicit-optional = "^1.3"
+types-toml = "^0.10.8.3"
+types-requests = "^2.28.11.12"
 
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.1.0"
+sphinx = "^6.1.3"
+sphinx-rtd-theme = "^1.2.0"
+sphinxcontrib-napoleon = "^0.7"
 
 
 [tool.poetry.group.test.dependencies]
 sqlalchemy-utils = "^0.39.0"
 pytest = "^7.2.1"
 
 [tool.isort]
@@ -93,11 +111,16 @@
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 99
 disable = """
     too-many-arguments,
     too-many-instance-attributes,
     too-few-public-methods
 """
+good-names=["i","j" ,"k","ex","Run","_","db"]
+
+
+[tool.mypy]
+ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gn2pg_client-1.4.0/PKG-INFO` & `gn2pg_client-1.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gn2pg-client
-Version: 1.4.0
+Version: 1.5.0
 Summary: Import tool from GeoNature to a PostgreSQL database through Export module API (client side)
 Home-page: https://github.com/lpoaura/gn2gn_client/
 License: AGPL-3.0-or-later
 Keywords: GeoNature,Export,SINP,opendata,biodiversity
 Author: lpofredc
 Author-email: frederic.cloitre@lpo.fr
 Maintainer: lpofredc
@@ -23,27 +23,34 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Software Distribution
+Provides-Extra: dashboard
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
+Requires-Dist: flask (>=2.2.3,<3.0.0) ; extra == "dashboard"
+Requires-Dist: flask-admin (>=1.6.1,<2.0.0) ; extra == "dashboard"
+Requires-Dist: flask-sqlalchemy (>=3.0.3,<4.0.0) ; extra == "dashboard"
+Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "dashboard"
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
+Requires-Dist: python-decouple (>=3.8,<4.0) ; extra == "dashboard"
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) ; extra == "dashboard"
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
 Requires-Dist: sqlalchemy (>=1.4.46,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/x-rst
 
 **************
  GN2PG Client
 **************
 
-.. image:: https://img.shields.io/badge/python-3.7+-yellowgreen
+.. image:: https://img.shields.io/badge/python-3.8+-yellowgreen
    :target: https://www.python.org/
 .. image:: https://img.shields.io/badge/PostgreSQL-10+-blue
    :target: https://www.postgresql.org/
 .. image:: https://img.shields.io/badge/packaging%20tool-poetry-important
    :target: https://python-poetry.org/
 .. image:: https://img.shields.io/badge/code%20style-black-black
    :target: https://github.com/psf/black
@@ -51,14 +58,17 @@
    :target: https://opensource.org/licenses/AGPL-3.0
 .. image:: https://app.fossa.com/api/projects/git%2Bgithub.com%2Flpoaura%2FGN2PG.svg?type=shield
    :target: https://app.fossa.com/projects/git%2Bgithub.com%2Flpoaura%2FGN2PG?ref=badge_shield
 
 This project provides an import data from GeoNature_ instances to a PostgreSQL database (client side).
 Widely inspired from `ClientApiVN <https://framagit.org/lpo/Client_API_VN/>`_
 
+.. tip::
+
+    The minimum version of the source GeoNature instance required for the incremental update must be a version 2.12.0
 
 .. contents:: Topics
 
 .. image:: ./docs/source/_static/src_gn2pg.png
     :align: center
     :alt: Project logo
 
@@ -191,50 +201,66 @@
 
 .. code-block:: cron
 
     */30 * * * * /usr/bin/env bash -c "source <path to python environment>/bin/activate && gn2pg_cli --update <myconfigfile>" > /dev/null 2>&1
 
 
 Debug mode
-############
+##########
 
 Debug mode can be activated using ``--verbose`` CLI argument
 
 Logs
 ####
 
 Log files are stored in ``$HOME/.gn2pg/log`` directory.
 
-Import datas into GeoNature datas
-#################################
+Import datas into GeoNature database
+####################################
 
 Default script to auto populate GeoNature is called "to_gnsynthese".
 
 .. code-block:: bash
 
     gn2pg_cli --custom-script to_gnsynthese <myconfigfile>
 
 
 .. tip::
 
     You can also replacing synthese script by your own scripts, using file path instead of ``to_gnsynthese``.
 
 
+Dashboard
+=========
+
+A simple web dashboard can be run following `dashboard docs <./docs/dashboard.rst>`_.
+
+.. image:: ./docs/_static/home_gn2pg_dashboard.png
+    :align: center
+    :alt: Dashboard_Home
+
+
+
+.. image:: ./docs/_static/src_gn2pg_dashboard.png
+    :align: center
+    :alt: Dashboard_gn2pg_downloag_log
+
 Contributing
 ============
 
 All devs must be done in forks (see `GitHub doc <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`_).
 
 Pull requests must be pulled to `dev` branch.
 
 Install project and development requirements (require `poetry <https://python-poetry.org/>`_):
 
 .. code-block:: bash
 
-    poetry install
+    poetry install --with=docs --all-extras
+    poetry run pre-commit install
 
 Make your devs and pull requests.
 
 Test `gn2pg_cli` in dev mode by running this command:
 
 .. code-block:: bash
```

