# Comparing `tmp/seqslabcli-3.2.0.post0.tar.gz` & `tmp/seqslabcli-3.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslabcli-3.2.0.post0.tar", last modified: Wed Apr 26 06:15:17 2023, max compression
+gzip compressed data, was "seqslabcli-3.2.0.post1.tar", last modified: Wed May  3 10:13:56 2023, max compression
```

## Comparing `seqslabcli-3.2.0.post0.tar` & `seqslabcli-3.2.0.post1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/seqslab/
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/seqslab/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/auth/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/auth/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/seqslab/drs/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/seqslab/drs/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    37716 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20396 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/aiocopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/drs/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40704 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/storage/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/drs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/utils/biomimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/organization/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/organization/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/organization/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/organization/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/role/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/role/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/role/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/runsheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/runsheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/runsheet/runsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/session_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/statusbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20679 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/register/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/template/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/template/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/usage_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/user/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/user/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/wes/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/wes/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/wes/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/wes/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/template/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/template/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/workspace/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.463189 seqslabcli-3.2.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-05-03 10:13:56.463189 seqslabcli-3.2.0.post1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/auth/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/auth/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/drs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/api/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37707 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/drs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20561 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/internal/aiocopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/drs/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40704 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/storage/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/drs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/utils/biomimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/drs/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/organization/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/organization/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/organization/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/organization/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/role/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/role/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/role/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/role/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/role/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.455188 seqslabcli-3.2.0.post1/python/seqslab/role/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/role/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/role/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/role/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/runsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/runsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/runsheet/runsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/session_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/statusbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/trs/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/trs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/trs/register/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/register/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/register/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/register/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/register/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/trs/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/resource/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/trs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/trs/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/usage_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/user/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/user/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/user/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/user/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/user/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/user/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/user/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/user/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/wes/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/wes/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/wes/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/wes/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/wes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/workspace/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/workspace/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/workspace/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/workspace/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.459189 seqslabcli-3.2.0.post1/python/seqslab/workspace/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/workspace/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/workspace/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/python/seqslab/workspace/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:56.463189 seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-05-03 10:13:56.000000 seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-03 10:13:56.000000 seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:13:56.000000 seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 10:13:56.000000 seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-03 10:13:56.000000 seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 10:13:56.000000 seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:13:56.000000 seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 10:13:56.463189 seqslabcli-3.2.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-03 10:13:42.000000 seqslabcli-3.2.0.post1/setup.py
```

### Comparing `seqslabcli-3.2.0.post0/LICENSE` & `seqslabcli-3.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/PKG-INFO` & `seqslabcli-3.2.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslabcli
-Version: 3.2.0.post0
+Version: 3.2.0.post1
 Summary: Seqslab CLI
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Jia-You Lin
 Author-email: jiayou.lin@atgenomix.com
 License: MIT license
 Description: <!-- PROJECT SHIELDS -->
         <!--
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslabcli Version: 3.2.0.post0 Summary: Seqslab
+Metadata-Version: 2.1 Name: seqslabcli Version: 3.2.0.post1 Summary: Seqslab
 CLI Home-page: https://github.com/AnomeGAP/seqslab-cli Author: Jia-You Lin
 Author-email: jiayou.lin@atgenomix.com License: MIT license Description:
 [Contributors][contributors-url] [Stargazers][stars-url] [Issues][issues-url]
 [License][license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     [Logo]
                  ***** Atgenomix SeqsLab V3 platform CLI *****
 Command Line Interface application in the Atgenomix SeqsLab platform, a cloud-
```

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/README.md` & `seqslabcli-3.2.0.post1/python/seqslab/README.md`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/__init__.py` & `seqslabcli-3.2.0.post1/python/seqslab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 name = "seqslab"
 
 __all__ = [
 
 ]
 
 
-__version__ = "3.2.0post"
+__version__ = "3.2.0post1"
 
 LOGGING = {
     "DIR_PATH": "/var/log/seqslab"
 }
```

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/auth/azuread.py` & `seqslabcli-3.2.0.post1/python/seqslab/auth/azuread.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/auth/commands.py` & `seqslabcli-3.2.0.post1/python/seqslab/auth/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/cli.py` & `seqslabcli-3.2.0.post1/python/seqslab/cli.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/context.py` & `seqslabcli-3.2.0.post1/python/seqslab/context.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/api/azure.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/api/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/api/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,16 +241,16 @@
             created_times.append(v.get('created_time'))
 
         folder_stdin = stdin[0].copy()
         folder_stdin['checksums'][0]['checksum_type'] = kwargs.get('checksum_type', "sha256")
         folder_stdin['checksums'][0]['checksum'] = kwargs.get('checksum', self.concat_checksum(checksums=checksums))
         folder_stdin['size'] = kwargs.get('size', self.sum_fsize(sizes=sizes))
         folder_stdin['created_time'] = kwargs.get('created_time', self.min_time(times=created_times))
-        folder_stdin['mime_type'] = kwargs.get('mime_type', "folder")
-        folder_stdin['file_type'] = kwargs.get('file_type', "folder")
+        folder_stdin['mime_type'] = kwargs.get('mime_type', "directory")
+        folder_stdin['file_type'] = kwargs.get('file_type', "directory")
         folder_stdin['description'] = kwargs.get('description', folder_stdin['description'])
         folder_stdin['aliases'] = kwargs.get('aliases', folder_stdin['aliases'])
         folder_stdin['metadata'] = json.loads(kwargs.get('metadata')) if "metadata" in kwargs else folder_stdin['metadata']
         folder_stdin['tags'] = kwargs.get('tags', folder_stdin['tags'])
         folder_stdin['id'] = kwargs.get('id', folder_stdin['id'])
         if "access_methods" in kwargs.keys():
             folder_stdin['access_methods'] = json.loads(kwargs.get('access_methods'))
```

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/api/common.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/api/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/api/template.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/api/template.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/commands.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,18 +357,18 @@
     @argument("workspace",
               type=str,
               positional=False,
               description="Specify the workspace based on the signed in account (required).", )
     @argument("type",
               type=str,
               positional=True,
-              description="If you want to register a file as a blob , please choose a file-blob. "
-                          "If you want to register a folder as a blob , please choose a folder-blob. "
-                          "(required)",
-              choices=['file-blob', 'folder-blob'])
+              description="If you want to register a file as a blob, please choose file-blob. "
+                          "If you want to register a directory as a blob, please choose dir-blob "
+                          "(required).",
+              choices=['file-blob', 'dir-blob'])
     @argument("name",
               type=str,
               description="Specify the name of the object that you want to register "
                           "(optional in stdin mode, otherwise required).", )
     @argument("file_type",
               type=str,
               description="Specify the file type of the object that you want to register "
```

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/internal/aiocopy.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/internal/aiocopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,16 +129,16 @@
     await asyncio.gather(*tasks, return_exceptions=True)
     return sha256_hash.hexdigest()
 
 
 def bio_filetype(filename: str) -> str:
     try:
         checker, file_extension = filename.split('.')[-2:]
-        if file_extension in ['gz', 'gzip']:
-            if checker in ['fastq', 'fq', 'fasta', 'fa', 'vcf', 'tar']:
+        if file_extension in ['gz', 'gzip', 'bai', 'fai', 'sa', 'amb', 'ann', 'bwt', 'pac']:
+            if checker in ['fastq', 'fq', 'fasta', 'fa', 'bam', 'vcf', 'tar']:
                 file_extension = '.'.join((checker, file_extension))
     except ValueError:
         file_extension = None
     return file_extension
 
 
 def argument_setting(files: list, **kwargs) -> tuple:
@@ -161,23 +161,25 @@
 
 
 async def result_setting(status: list, files: List[URL], resp_list: list,
                          checksum_bar: ProgressBarObject) -> List[dict]:
     def _create_copyresult(sent: int, resp: dict, mime_type: str, file_extension: str, checksum: str, type: str,
                            status: Literal["complete", "partial", "failed"]) -> dict:
         checksums = [CopyResult.checksum(checksum=checksum, type=type)]
+        name = os.path.basename(resp["dst"][0]).replace(f".{file_extension}", "")
         access_methods = [CopyResult.access_method(
             access_methods_type=resp["access_methods_type"][i] if resp.get("access_methods_type") else None,
             access_tier='hot', dst=dst, region=resp["region"]) for i, dst in enumerate(resp['dst'])]
         return CopyResult(
-            name=os.path.basename(resp["dst"][0]),
+            name=name,
             mime_type=mime_type,
             file_type=file_extension,
             created_time=resp["created_time"],
             size=sent,
+            aliases=[os.path.basename(resp["dst"][0])],
             access_methods=access_methods if status == "complete" else None,
             checksums=checksums if status == "complete" else None,
             status=status,
             exceptions=f"{resp.get('exceptions')}" if resp.get('exceptions') else None
         )._asdict()
 
     checksum_bar.print('result_setting: Create response json.')
```

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/internal/common.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/internal/utils.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/storage/azure.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/storage/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/storage/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/storage/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/utils/biomimetype.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/utils/biomimetype.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/drs/utils/progressbar.py` & `seqslabcli-3.2.0.post1/python/seqslab/drs/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/exceptions.py` & `seqslabcli-3.2.0.post1/python/seqslab/exceptions.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/organization/commands.py` & `seqslabcli-3.2.0.post1/python/seqslab/organization/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/organization/resource/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/organization/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/plugin.py` & `seqslabcli-3.2.0.post1/python/seqslab/plugin.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/role/commands.py` & `seqslabcli-3.2.0.post1/python/seqslab/role/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/role/internal/common.py` & `seqslabcli-3.2.0.post1/python/seqslab/role/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/role/resource/azure.py` & `seqslabcli-3.2.0.post1/python/seqslab/role/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/role/resource/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/role/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/runsheet/runsheet.py` & `seqslabcli-3.2.0.post1/python/seqslab/runsheet/runsheet.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/settings.py` & `seqslabcli-3.2.0.post1/python/seqslab/settings.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/statusbar.py` & `seqslabcli-3.2.0.post1/python/seqslab/statusbar.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/commands.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,18 @@
               description="Specify the aliases of the tool that you want to register (optional).", )
     @argument("checker_url",
               type=URL,
               description="Specify the URL of the checker tool that you want to register (optional).", )
     @argument("has_checker",
               type=bool,
               description="Specify whether or not this tool has a checker tool associated with it (optional).", )
+    @argument("organization",
+              type=str,
+              description="Specify the organization of the tool that you want to register (optional)."
+              )
     def tool(self, name: str, **kwargs) -> int:
         """
                 Register TRS tool object.
         """
         tool_id = self._tool(tool_name=name, **kwargs)
         if isinstance(tool_id, int):
             return tool_id
@@ -301,16 +305,16 @@
     @argument("output",
               type=str,
               description="Specify the output filename of execs.json in relation to the working directory. "
                           "(optional, default = execs.json)")
     @argument("config_import",
               type=List[str],
               positional=False,
-              description="Specify one or more sub-workflow execs.json files to config operator pipeline configs  "
-                          "(optional).", )
+              description="Specify one or more subworkflow execution files (execs.json) to configure "
+                          "operator pipeline settings (optional).", )
     def execs(self, working_dir: str, inputs: str, main_wdl: str,
               output: str = "working_dir + execs.json", config_import: List[str] = []) -> int:
         """
             Create SeqsLab execs.json file.
         """
         if not os.path.isdir(working_dir):
             cprint(f"{working_dir} does not exist or is not a directory", "red")
```

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/internal/utils.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/register/azure.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/register/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/register/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/register/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
                            files=files) as response:
             if response.status_code not in [requests.codes.created]:
                 raise requests.HTTPError(f"{response.status_code}: {repr(response.text)}")
             return workflow_url.split('?')[0]
 
     def tool(self, tool_name: str, **kwargs):
         data = get_template("tool").create(
+            organization=kwargs.get('organization'),
             toolclass_name=kwargs.get('toolclass_name'),
             toolclass_description=kwargs.get('toolclass_description'),
             tool_name=tool_name,
             description=kwargs.get("description"),
             aliases=kwargs.get("aliases", []),
             checker_url=kwargs.get("checker_url"),
             has_checker=kwargs.get('has_checker'),
```

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/register/common.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/register/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/register/template.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/register/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         self.trs = trs_api
 
     def create(self, **kwargs) -> dict or list:
         assert self.trs in ['tool', 'toolversion', 'toolfile'], f"No such trs api"
         if self.trs == "tool":
             try:
                 return Template.tool(
+                    organization=kwargs.get("organization", None),
                     toolclass_name=kwargs.get("toolclass_name", None),
                     toolclass_description=kwargs.get("toolclass_description", None),
                     name=kwargs.get("tool_name", None),
                     description=kwargs.get("description", None),
                     aliases=kwargs.get("aliases", []),
                     checker_url=kwargs.get("checker_url", None),
                     has_checker=kwargs.get("has_checker", None),
@@ -103,20 +104,22 @@
             try:
                 return Template.toolfile(toolfile_json=kwargs.get("toolfile_json", []))
             except Exception as error:
                 raise error
 
     @staticmethod
     def tool(toolclass_name: str, toolclass_description: str, name: str, description: str, aliases: list,
-             checker_url: str, has_checker: bool, id: str) -> dict:
+             checker_url: str, has_checker: bool, id: str, organization: str) -> dict:
         try:
             assert name is not None, f"Enter a valid tool_name"
             tool = {
                 "name": name
             }
+            if organization:
+                tool['organization'] = organization
             if toolclass_name or toolclass_description:
                 tool["toolclass"] = Base.toolclass(name=toolclass_name, description=toolclass_description)
             if description:
                 tool["description"] = description
             if aliases:
                 tool["aliases"] = aliases
             if has_checker:
```

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/resource/azure.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/resource/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/resource/common.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/resource/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/template/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/trs/template/template.py` & `seqslabcli-3.2.0.post1/python/seqslab/trs/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/usage_logger.py` & `seqslabcli-3.2.0.post1/python/seqslab/usage_logger.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/user/commands.py` & `seqslabcli-3.2.0.post1/python/seqslab/user/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/user/internal/common.py` & `seqslabcli-3.2.0.post1/python/seqslab/user/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/user/resource/azure.py` & `seqslabcli-3.2.0.post1/python/seqslab/user/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/user/resource/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/user/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/wes/commands.py` & `seqslabcli-3.2.0.post1/python/seqslab/wes/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/wes/internal/common.py` & `seqslabcli-3.2.0.post1/python/seqslab/wes/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/wes/resource/azure.py` & `seqslabcli-3.2.0.post1/python/seqslab/wes/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/wes/resource/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/wes/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/wes/template/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/wes/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/wes/template/template.py` & `seqslabcli-3.2.0.post1/python/seqslab/wes/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/wes/utils.py` & `seqslabcli-3.2.0.post1/python/seqslab/wes/utils.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/workspace/commands.py` & `seqslabcli-3.2.0.post1/python/seqslab/workspace/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/workspace/internal/common.py` & `seqslabcli-3.2.0.post1/python/seqslab/workspace/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/azure.py` & `seqslabcli-3.2.0.post1/python/seqslab/workspace/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/base.py` & `seqslabcli-3.2.0.post1/python/seqslab/workspace/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/PKG-INFO` & `seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslabcli
-Version: 3.2.0.post0
+Version: 3.2.0.post1
 Summary: Seqslab CLI
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Jia-You Lin
 Author-email: jiayou.lin@atgenomix.com
 License: MIT license
 Description: <!-- PROJECT SHIELDS -->
         <!--
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslabcli Version: 3.2.0.post0 Summary: Seqslab
+Metadata-Version: 2.1 Name: seqslabcli Version: 3.2.0.post1 Summary: Seqslab
 CLI Home-page: https://github.com/AnomeGAP/seqslab-cli Author: Jia-You Lin
 Author-email: jiayou.lin@atgenomix.com License: MIT license Description:
 [Contributors][contributors-url] [Stargazers][stars-url] [Issues][issues-url]
 [License][license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     [Logo]
                  ***** Atgenomix SeqsLab V3 platform CLI *****
 Command Line Interface application in the Atgenomix SeqsLab platform, a cloud-
```

### Comparing `seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/SOURCES.txt` & `seqslabcli-3.2.0.post1/python/seqslabcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0.post0/setup.py` & `seqslabcli-3.2.0.post1/setup.py`

 * *Files identical despite different names*

