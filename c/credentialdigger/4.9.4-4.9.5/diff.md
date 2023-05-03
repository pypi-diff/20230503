# Comparing `tmp/credentialdigger-4.9.4-py3-none-any.whl.zip` & `tmp/credentialdigger-4.9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 78979 bytes, number of entries: 49
+Zip file size: 78975 bytes, number of entries: 49
 -rw-r--r--  2.0 unx      105 b- defN 21-May-26 09:14 credentialdigger/__init__.py
 -rw-r--r--  2.0 unx      137 b- defN 22-May-09 14:35 credentialdigger/__main__.py
--rw-r--r--  2.0 unx    55143 b- defN 22-Dec-09 10:14 credentialdigger/client.py
+-rw-r--r--  2.0 unx    55147 b- defN 23-Jan-18 13:21 credentialdigger/client.py
 -rw-r--r--  2.0 unx    18691 b- defN 22-Aug-08 09:44 credentialdigger/client_postgres.py
--rw-r--r--  2.0 unx    20128 b- defN 22-Aug-08 09:44 credentialdigger/client_sqlite.py
+-rw-r--r--  2.0 unx    20127 b- defN 23-Jan-18 13:21 credentialdigger/client_sqlite.py
 -rw-r--r--  2.0 unx     3924 b- defN 22-Jun-14 13:53 credentialdigger/snippet_similarity.py
 -rw-r--r--  2.0 unx        0 b- defN 21-May-26 09:14 credentialdigger/cli/__init__.py
 -rw-r--r--  2.0 unx     1992 b- defN 21-May-26 09:14 credentialdigger/cli/add_rules.py
 -rw-r--r--  2.0 unx     6171 b- defN 22-Aug-08 09:44 credentialdigger/cli/cli.py
 -rw-r--r--  2.0 unx     8953 b- defN 22-Sep-07 11:55 credentialdigger/cli/get_discoveries.py
 -rw-r--r--  2.0 unx     6616 b- defN 22-May-09 14:35 credentialdigger/cli/hook.py
 -rw-r--r--  2.0 unx     4897 b- defN 21-Oct-25 13:25 credentialdigger/cli/scan.py
@@ -38,14 +38,14 @@
 -rw-r--r--  2.0 unx     3808 b- defN 21-Jun-22 13:22 tests/integration_tests/test_git_file_scanner.py
 -rw-r--r--  2.0 unx     4150 b- defN 22-May-12 15:20 tests/integration_tests/test_git_scanner.py
 -rw-r--r--  2.0 unx        0 b- defN 21-May-26 09:14 tests/unit_tests/__init__.py
 -rw-r--r--  2.0 unx     4331 b- defN 21-May-26 09:14 tests/unit_tests/test_file_scanner.py
 -rw-r--r--  2.0 unx     2067 b- defN 22-Sep-05 13:20 tests/unit_tests/test_git_pr_scanner.py
 -rw-r--r--  2.0 unx     1398 b- defN 21-May-26 09:14 tests/unit_tests/test_git_scanner.py
 -rw-r--r--  2.0 unx     6064 b- defN 21-Oct-18 09:15 tests/unit_tests/test_scans.py
--rw-r--r--  2.0 unx    11402 b- defN 22-Dec-09 10:14 credentialdigger-4.9.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    12218 b- defN 22-Dec-09 10:14 credentialdigger-4.9.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-09 10:14 credentialdigger-4.9.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 22-Dec-09 10:14 credentialdigger-4.9.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 22-Dec-09 10:14 credentialdigger-4.9.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4535 b- defN 22-Dec-09 10:14 credentialdigger-4.9.4.dist-info/RECORD
-49 files, 265375 bytes uncompressed, 71595 bytes compressed:  73.0%
+-rw-r--r--  2.0 unx    11402 b- defN 23-Jan-18 13:21 credentialdigger-4.9.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12218 b- defN 23-Jan-18 13:21 credentialdigger-4.9.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-18 13:21 credentialdigger-4.9.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 23-Jan-18 13:21 credentialdigger-4.9.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jan-18 13:21 credentialdigger-4.9.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4535 b- defN 23-Jan-18 13:21 credentialdigger-4.9.5.dist-info/RECORD
+49 files, 265378 bytes uncompressed, 71591 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -123,26 +123,26 @@
 
 Filename: tests/unit_tests/test_git_scanner.py
 Comment: 
 
 Filename: tests/unit_tests/test_scans.py
 Comment: 
 
-Filename: credentialdigger-4.9.4.dist-info/LICENSE
+Filename: credentialdigger-4.9.5.dist-info/LICENSE
 Comment: 
 
-Filename: credentialdigger-4.9.4.dist-info/METADATA
+Filename: credentialdigger-4.9.5.dist-info/METADATA
 Comment: 
 
-Filename: credentialdigger-4.9.4.dist-info/WHEEL
+Filename: credentialdigger-4.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: credentialdigger-4.9.4.dist-info/entry_points.txt
+Filename: credentialdigger-4.9.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: credentialdigger-4.9.4.dist-info/top_level.txt
+Filename: credentialdigger-4.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: credentialdigger-4.9.4.dist-info/RECORD
+Filename: credentialdigger-4.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## credentialdigger/client.py

```diff
@@ -1145,15 +1145,15 @@
         if self.add_repo(repo_url):
             # The repository is new, scan from the first commit
             from_timestamp = 0
             new_repo = True
         else:
             # Get the latest commit recorded on the db
             # `or` clause needed in case the previous scan attempt was broken
-            from_timestamp = self.get_repo(repo_url)['last_scan'] or 0
+            from_timestamp = self.get_repo(repo_url).get('last_scan') or 0
             new_repo = False
 
         # Force complete scan
         if force:
             logger.debug('Force complete scan')
             # Clean up discoveries and embeddings for this repo
             # embeddings must be deleted before discoveries since they
```

## credentialdigger/client_sqlite.py

```diff
@@ -123,15 +123,15 @@
             file_name=file_name,
             commit_id=commit_id,
             line_number=line_number,
             snippet=snippet,
             repo_url=repo_url,
             rule_id=rule_id,
             state=state,
-            query='INSERT INTO discoveries (file_name, commit_id, line_number, \
+            query='INSERT INTO discoveries (file_name, commit_id, line_number,\
             snippet, repo_url, rule_id, state) VALUES \
             (?, ?, ?, ?, ?, ?, ?)'
         )
 
     def add_discoveries(self, discoveries, repo_url):
         """ Bulk add new discoveries.
```

## Comparing `credentialdigger-4.9.4.dist-info/LICENSE` & `credentialdigger-4.9.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `credentialdigger-4.9.4.dist-info/METADATA` & `credentialdigger-4.9.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credentialdigger
-Version: 4.9.4
+Version: 4.9.5
 Summary: Credential Digger
 Home-page: https://github.com/SAP/credential-digger
 Author: SAP SE
 Maintainer: Marco Rosa, Slim Trabelsi
 Maintainer-email: marco.rosa@sap.com, slim.trabelsi@sap.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

## Comparing `credentialdigger-4.9.4.dist-info/RECORD` & `credentialdigger-4.9.5.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 credentialdigger/__init__.py,sha256=CniE5pjeQmJ52n92stfoVsZiiP91ywgd1i6zaIvBVpo,105
 credentialdigger/__main__.py,sha256=ooR_IQqvrdhFoflGGs_8HYZOW3wki9DY3m8fFG948RQ,137
-credentialdigger/client.py,sha256=8VAZfNfEgOqXQk3307wyjMJ-mzYEiFfgao6TiqVjJW8,55143
+credentialdigger/client.py,sha256=1H2sK6CLH441HJ8nam6yNDsiyHz5Ci5g-1t6Xz-KWIE,55147
 credentialdigger/client_postgres.py,sha256=mbwVi45aWSyjCDpEN_-j8che-m20bSPaMuM4XC5E8Ak,18691
-credentialdigger/client_sqlite.py,sha256=pCvSJ7fSi1HarUv1HPwFOUqY_7THT_OoAv7V4Wx7BCw,20128
+credentialdigger/client_sqlite.py,sha256=J84FxPTBW1lDr8AF29ip63wLmZoNrIVuViyxCdxYjNM,20127
 credentialdigger/snippet_similarity.py,sha256=VIvV4wSqEqajscX94CNDp0JgPLYc1VXg4ZOMyqIVCQg,3924
 credentialdigger/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 credentialdigger/cli/add_rules.py,sha256=N1GnEx41SEXboUSqwbodssxRLgyz71tzEa1IuTDXTlw,1992
 credentialdigger/cli/cli.py,sha256=u-The7pFPzHNC2sX1WnglQ9-wVcRKuywzlITMJT7lew,6171
 credentialdigger/cli/get_discoveries.py,sha256=sMwo6ZUxkdbRd-X1p93XY6gRB2Ul8API_KFyY2lqtrk,8953
 credentialdigger/cli/hook.py,sha256=lRbulV28jw2ElJuLZ0W7hjShEgMgUBqy-gdUxOsZXlU,6616
 credentialdigger/cli/scan.py,sha256=kw4yrbgruho-rCiDYAXi7U1eAbBHPBge2LcI3RU2zKw,4897
@@ -37,13 +37,13 @@
 tests/integration_tests/test_git_file_scanner.py,sha256=bzPZJohuG16bU-w1q2SGRpJyjCNj1TbJUggH_z6NDUQ,3808
 tests/integration_tests/test_git_scanner.py,sha256=PHmHmejx1HUMmMpwfJysFx4wEPplV5uEpOzh_vV7aw0,4150
 tests/unit_tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/unit_tests/test_file_scanner.py,sha256=ktaw-qliEgITgpVBy8Py15Gs9bGEKQrrhkkvUH1PwJk,4331
 tests/unit_tests/test_git_pr_scanner.py,sha256=i1QK1N0blRliOpQqa1xknFtXxeHzZupLYv7L6H4fQVs,2067
 tests/unit_tests/test_git_scanner.py,sha256=98gsen0nWsRqSAWPdvvWTWUCIAVSIR0kiOYO9QO5ytA,1398
 tests/unit_tests/test_scans.py,sha256=gfYcFsln0vF5a4gQO2vSmJWiIuYn77DsGvPhKq_Z5cM,6064
-credentialdigger-4.9.4.dist-info/LICENSE,sha256=2CGx06w_GrghZfOZU1OWszN8YZSbOgeIq80OwEtTC6Y,11402
-credentialdigger-4.9.4.dist-info/METADATA,sha256=tnfGqTGAr6HfIyfXarrB5tQoRJxIS67M5yBxPUN32Sk,12218
-credentialdigger-4.9.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-credentialdigger-4.9.4.dist-info/entry_points.txt,sha256=AyfBGgIx8_qNfexy3Zu3PCCWdVWgTVofT6WSG0XAHwg,68
-credentialdigger-4.9.4.dist-info/top_level.txt,sha256=RsokEyOc74o1CX86BpfkHzeGNj3alQkC5D8xjuegEVM,23
-credentialdigger-4.9.4.dist-info/RECORD,,
+credentialdigger-4.9.5.dist-info/LICENSE,sha256=2CGx06w_GrghZfOZU1OWszN8YZSbOgeIq80OwEtTC6Y,11402
+credentialdigger-4.9.5.dist-info/METADATA,sha256=x1XP1mstOm1K1X87sl4Y9jcZILm3Wj5ptRhVQmQh41A,12218
+credentialdigger-4.9.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+credentialdigger-4.9.5.dist-info/entry_points.txt,sha256=AyfBGgIx8_qNfexy3Zu3PCCWdVWgTVofT6WSG0XAHwg,68
+credentialdigger-4.9.5.dist-info/top_level.txt,sha256=RsokEyOc74o1CX86BpfkHzeGNj3alQkC5D8xjuegEVM,23
+credentialdigger-4.9.5.dist-info/RECORD,,
```

