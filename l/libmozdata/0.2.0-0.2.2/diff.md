# Comparing `tmp/libmozdata-0.2.0.tar.gz` & `tmp/libmozdata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libmozdata-0.2.0.tar", last modified: Wed Apr  5 15:28:11 2023, max compression
+gzip compressed data, was "dist/libmozdata-0.2.2.tar", last modified: Wed May  3 18:20:38 2023, max compression
```

## Comparing `libmozdata-0.2.0.tar` & `libmozdata-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:28:11.000000 libmozdata-0.2.0/
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-05 15:28:11.000000 libmozdata-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-05 15:28:11.000000 libmozdata-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-05 15:28:11.000000 libmozdata-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-05 15:28:11.000000 libmozdata-0.2.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/
--rw-r--r--   0 root         (0) root         (0)     7695 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/BZInfo.py
--rw-r--r--   0 root         (0) root         (0)     1828 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/FXRevision.py
--rw-r--r--   0 root         (0) root         (0)     4268 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/FileStats.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/HGFileInfo.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38502 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/bugzilla.py
--rw-r--r--   0 root         (0) root         (0)     4042 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/buildhub.py
--rw-r--r--   0 root         (0) root         (0)     1800 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/config.py
--rw-r--r--   0 root         (0) root         (0)     7286 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/connection.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/fx_trains.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/handler.py
--rw-r--r--   0 root         (0) root         (0)    10234 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/hgmozilla.py
--rw-r--r--   0 root         (0) root         (0)     2423 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/lando.py
--rw-r--r--   0 root         (0) root         (0)    75057 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/modules.json
--rw-r--r--   0 root         (0) root         (0)     2781 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/modules.py
--rw-r--r--   0 root         (0) root         (0)    39379 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/patchanalysis.py
--rw-r--r--   0 root         (0) root         (0)    24085 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/phabricator.py
--rw-r--r--   0 root         (0) root         (0)     6327 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/redash.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/release_owners.py
--rw-r--r--   0 root         (0) root         (0)     8039 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/socorro.py
--rw-r--r--   0 root         (0) root         (0)     8653 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/utils.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/vcs_map.py
--rw-r--r--   0 root         (0) root         (0)     5014 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/versions.py
--rw-r--r--   0 root         (0) root         (0)     3581 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata/wiki_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      830 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-05 15:28:11.000000 libmozdata-0.2.0/libmozdata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-05 15:28:11.000000 libmozdata-0.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-04-05 15:28:11.000000 libmozdata-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1214 2023-04-05 15:28:11.000000 libmozdata-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:20:38.000000 libmozdata-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-03 18:20:38.000000 libmozdata-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-03 18:20:38.000000 libmozdata-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-03 18:20:38.000000 libmozdata-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-03 18:20:38.000000 libmozdata-0.2.2/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/
+-rw-r--r--   0 root         (0) root         (0)     7695 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/BZInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/FXRevision.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/FileStats.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/HGFileInfo.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38502 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/bugzilla.py
+-rw-r--r--   0 root         (0) root         (0)     4042 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/buildhub.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/config.py
+-rw-r--r--   0 root         (0) root         (0)     7286 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/connection.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/fx_trains.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/handler.py
+-rw-r--r--   0 root         (0) root         (0)    10234 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/hgmozilla.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/lando.py
+-rw-r--r--   0 root         (0) root         (0)    75057 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/modules.json
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/modules.py
+-rw-r--r--   0 root         (0) root         (0)    39379 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/patchanalysis.py
+-rw-r--r--   0 root         (0) root         (0)    24340 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/phabricator.py
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/redash.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/release_owners.py
+-rw-r--r--   0 root         (0) root         (0)     8039 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/socorro.py
+-rw-r--r--   0 root         (0) root         (0)     8653 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/vcs_map.py
+-rw-r--r--   0 root         (0) root         (0)     5014 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/versions.py
+-rw-r--r--   0 root         (0) root         (0)     3581 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata/wiki_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      830 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-03 18:20:38.000000 libmozdata-0.2.2/libmozdata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-03 18:20:38.000000 libmozdata-0.2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-03 18:20:38.000000 libmozdata-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-03 18:20:38.000000 libmozdata-0.2.2/setup.py
```

### Comparing `libmozdata-0.2.0/README.md` & `libmozdata-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/BZInfo.py` & `libmozdata-0.2.2/libmozdata/BZInfo.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/FXRevision.py` & `libmozdata-0.2.2/libmozdata/FXRevision.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/FileStats.py` & `libmozdata-0.2.2/libmozdata/FileStats.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/HGFileInfo.py` & `libmozdata-0.2.2/libmozdata/HGFileInfo.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/bugzilla.py` & `libmozdata-0.2.2/libmozdata/bugzilla.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/buildhub.py` & `libmozdata-0.2.2/libmozdata/buildhub.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/config.py` & `libmozdata-0.2.2/libmozdata/config.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/connection.py` & `libmozdata-0.2.2/libmozdata/connection.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/fx_trains.py` & `libmozdata-0.2.2/libmozdata/fx_trains.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/handler.py` & `libmozdata-0.2.2/libmozdata/handler.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/hgmozilla.py` & `libmozdata-0.2.2/libmozdata/hgmozilla.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/lando.py` & `libmozdata-0.2.2/libmozdata/lando.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # -*- coding: utf-8 -*-
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import requests
 
+from . import config
+
 
 class LandoWarnings(object):
     """
     Encapsulates lando warning calls
     """
 
     def __init__(self, api_url, api_key):
         self.api_url = f"{api_url}/diff_warnings"
         self.api_key = api_key
+        self.USER_AGENT = config.get("User-Agent", "name", "libmozdata")
 
     def del_warnings(self, warnings):
         """
         Deletes warnings from Lando based on a json warnings list
         """
         for warning in warnings:
             warning_id = warning["id"]
 
             response = requests.delete(
                 f"{self.api_url}/{warning_id}",
-                headers={"X-Phabricator-API-Key": self.api_key},
+                headers={
+                    "X-Phabricator-API-Key": self.api_key,
+                    "User-Agent": self.USER_AGENT,
+                },
             )
 
             if response.status_code != 200:
                 raise Exception(f"Failed to delete warning with ID {warning_id}!")
 
     def add_warning(self, warning, revision_id, diff_id):
         """
@@ -38,15 +44,18 @@
             self.api_url,
             json={
                 "revision_id": revision_id,
                 "diff_id": diff_id,
                 "group": "LINT",
                 "data": {"message": warning},
             },
-            headers={"X-Phabricator-API-Key": self.api_key},
+            headers={
+                "X-Phabricator-API-Key": self.api_key,
+                "User-Agent": self.USER_AGENT,
+            },
         )
         if response.status_code != 201:
             raise Exception(
                 f"Failed to add warnings for revision_id {revision_id} and diff_id {diff_id}!"
             )
 
     def get_warnings(self, revision_id, diff_id):
@@ -56,15 +65,18 @@
         response = requests.get(
             self.api_url,
             params={
                 "revision_id": revision_id,
                 "diff_id": diff_id,
                 "group": "LINT",
             },
-            headers={"X-Phabricator-API-Key": self.api_key},
+            headers={
+                "X-Phabricator-API-Key": self.api_key,
+                "User-Agent": self.USER_AGENT,
+            },
         )
         if response.status_code != 200:
             raise Exception(
                 f"Failed to get warnings for revision_id {revision_id} and diff_id {diff_id}!"
             )
 
         return response.json()
```

### Comparing `libmozdata-0.2.0/libmozdata/modules.json` & `libmozdata-0.2.2/libmozdata/modules.json`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/modules.py` & `libmozdata-0.2.2/libmozdata/modules.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/patchanalysis.py` & `libmozdata-0.2.2/libmozdata/patchanalysis.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/phabricator.py` & `libmozdata-0.2.2/libmozdata/phabricator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import json
 import logging
 from urllib.parse import urlencode, urlparse
 
 import hglib
 import requests
 
+from . import config
+
 HGMO_JSON_REV_URL_TEMPLATE = "https://hg.mozilla.org/mozilla-central/json-rev/{}"
 MOZILLA_PHABRICATOR_PROD = "https://phabricator.services.mozilla.com/api/"
 
 PhabricatorPatch = collections.namedtuple(
     "PhabricatorPatch", "id, phid, patch, base_revision, commits"
 )
 
@@ -211,27 +213,32 @@
 
 class PhabricatorAPI(object):
     """
     Phabricator Rest API client
     """
 
     def __init__(self, api_key, url=MOZILLA_PHABRICATOR_PROD):
+        self.USER_AGENT = config.get("User-Agent", "name", "libmozdata")
         self.api_key = api_key
         self.url = url
         assert self.url.endswith("/api/"), "Phabricator API must end with /api/"
 
         # Test authentication
         self.user = self.request("user.whoami")
         logger.info("Authenticated on {} as {}".format(self.url, self.user["realName"]))
 
     @property
     def hostname(self):
         parts = urlparse(self.url)
         return parts.netloc
 
+    def get_header(self):
+        """Get the header to use each query"""
+        return {"User-Agent": self.USER_AGENT}
+
     def search_diffs(
         self,
         diff_phid=None,
         diff_id=None,
         revision_phid=None,
         output_cursor=False,
         **params
@@ -658,14 +665,15 @@
         """
         # Add api token to payload
         payload["__conduit__"] = {"token": self.api_key}
 
         # Run POST request on api
         response = requests.post(
             self.url + path,
+            headers=self.get_header(),
             data=urlencode({"params": json.dumps(payload), "output": "json"}),
         )
         response.raise_for_status()
 
         # Check response
         data = response.json()
         assert "error_code" in data
```

### Comparing `libmozdata-0.2.0/libmozdata/redash.py` & `libmozdata-0.2.2/libmozdata/redash.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/release_owners.py` & `libmozdata-0.2.2/libmozdata/release_owners.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,32 +44,34 @@
         table = parser.get_tables()[0]
         if [
             "Firefox Version",
             "Owner",
             "Secondary",
             "Engineering REO",
             "Release Duty",
+            "QA Owner",
             "Corresponding ESR",
             "Release Date",
         ] != table[0]:
             raise InvalidWiki("Column headers are wrong")
 
         _OWNERS = []
         for row in table[1:]:
             try:
                 # sometimes the date is 2019-XX-XX (when the date is not known)
-                release_date = utils.get_date_ymd(row[6])
+                release_date = utils.get_date_ymd(row[7])
             except (AssertionError, ValueError):
                 continue
 
             _OWNERS.append(
                 {
                     "version": get_versions(row[0])[0][0],
                     "owner": row[1],
                     "secondary": row[2],
                     "engineering reo": row[3],
                     "release duty": _get_list_people(row[4]),
-                    "corresponding esr": row[5],
+                    "qa owner": row[5],
+                    "corresponding esr": row[6],
                     "release date": release_date,
                 }
             )
         return _OWNERS
```

### Comparing `libmozdata-0.2.0/libmozdata/socorro.py` & `libmozdata-0.2.2/libmozdata/socorro.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/utils.py` & `libmozdata-0.2.2/libmozdata/utils.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/vcs_map.py` & `libmozdata-0.2.2/libmozdata/vcs_map.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/versions.py` & `libmozdata-0.2.2/libmozdata/versions.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata/wiki_parser.py` & `libmozdata-0.2.2/libmozdata/wiki_parser.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/libmozdata.egg-info/SOURCES.txt` & `libmozdata-0.2.2/libmozdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.0/setup.py` & `libmozdata-0.2.2/setup.py`

 * *Files identical despite different names*

