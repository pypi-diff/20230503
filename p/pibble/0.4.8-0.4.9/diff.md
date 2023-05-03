# Comparing `tmp/pibble-0.4.8.tar.gz` & `tmp/pibble-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibble-0.4.8.tar", last modified: Sun Apr 30 19:53:27 2023, max compression
+gzip compressed data, was "pibble-0.4.9.tar", last modified: Mon May  1 00:10:08 2023, max compression
```

## Comparing `pibble-0.4.8.tar` & `pibble-0.4.9.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.674868 pibble-0.4.8/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6435 2023-04-30 19:53:27.674868 pibble-0.4.8/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5960 2023-04-30 19:53:27.000000 pibble-0.4.8/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.662869 pibble-0.4.8/pibble/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8891 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.662869 pibble-0.4.8/pibble/api/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3287 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.662869 pibble-0.4.8/pibble/api/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.662869 pibble-0.4.8/pibble/api/client/apachethrift/
--rw-------   0 benjamin  (1000) benjamin  (1000)     6189 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/apachethrift/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1326 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.662869 pibble-0.4.8/pibble/api/client/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    14182 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/file/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9703 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/file/hdfs.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12462 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/file/local.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    19644 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4126 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/client/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4698 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16829 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2330 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/client/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11322 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4770 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10558 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6564 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/soap.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7325 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/webservice/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/client/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/configuration.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6084 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/exceptions.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/helpers/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/helpers/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15593 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/helpers/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    20508 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/helpers/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24123 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/helpers/googlerpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13134 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/helpers/store.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13916 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/helpers/wrappers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/meta/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/meta/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9353 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/meta/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2958 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/meta/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/middleware/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/middleware/apachethrift/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/apachethrift/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/apachethrift/screening.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/middleware/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3112 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/database/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/middleware/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      438 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/file/temp.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/middleware/googlerpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/googlerpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/googlerpc/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/googlerpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/googlerpc/metadata.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3027 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/middleware/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/middleware/webservice/authentication/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/authentication/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/authentication/basic.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/authentication/bearer.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13466 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/authentication/digest.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/authentication/header.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    17694 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/authentication/oauth.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3248 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/limit.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/middleware/webservice/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/protocol/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/protocol/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19471 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/protocol/apachethrift.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2443 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1983 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.666868 pibble-0.4.8/pibble/api/server/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15450 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5445 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/api/server/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2377 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7264 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/awslambda.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    41732 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15507 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/handler.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3182 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/api/server/webservice/mixin/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/mixin/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      718 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/mixin/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      987 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/api/server/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4212 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6486 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11970 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16833 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/soap.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/api/server/webservice/template/
--rw-------   0 benjamin  (1000) benjamin  (1000)     9667 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/template/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9195 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/template/extensions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9364 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/api/server/webservice/template/loader.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7772 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/database/dedupe.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10216 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/database/engine.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/database/exceptions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    26389 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/database/orm.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2667 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/database/util.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/cms/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/cms/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/database/interface.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/database/menu.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/database/view.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/cms/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6382 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2998 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/server/extension.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      350 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/cms/server/mixin.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/dam/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/dam/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/dam/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/dam/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/dam/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/dam/database/files.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/dam/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/dam/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/dam/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/rest/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/rest/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/rest/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/rest/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/rest/database/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/rest/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/rest/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15691 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/rest/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7707 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/rest/server/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/session/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/session/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/session/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/session/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/session/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/session/database/session.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/session/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/session/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5026 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/session/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/user/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.670868 pibble-0.4.8/pibble/ext/user/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/client/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      963 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.674868 pibble-0.4.8/pibble/ext/user/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/database/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/database/notification.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/database/permission.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/database/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.674868 pibble-0.4.8/pibble/ext/user/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24981 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/ext/user/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.674868 pibble-0.4.8/pibble/hooks/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/hooks/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5971 2023-04-30 19:53:26.000000 pibble-0.4.8/pibble/hooks/aws.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.674868 pibble-0.4.8/pibble/media/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:26.000000 pibble-0.4.8/pibble/media/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10231 2023-04-30 19:53:26.000000 pibble-0.4.8/pibble/media/thumbnail.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.674868 pibble-0.4.8/pibble/resources/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/resources/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10649 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/resources/retriever.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2693 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/setup.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.674868 pibble-0.4.8/pibble/util/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/util/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8375 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/util/encryption.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16134 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/util/files.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    32731 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/util/helpers.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/util/imaging.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/util/log.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1610 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/util/numeric.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    26217 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/util/strings.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.674868 pibble-0.4.8/pibble/web/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/web/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble/web/scraper.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 19:53:27.662869 pibble-0.4.8/pibble.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6435 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5413 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1872 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-04-30 19:53:27.000000 pibble-0.4.8/pibble.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-04-30 19:53:27.674868 pibble-0.4.8/setup.cfg
--rw-------   0 benjamin  (1000) benjamin  (1000)     2693 2023-04-30 19:53:27.000000 pibble-0.4.8/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.989380 pibble-0.4.9/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6435 2023-05-01 00:10:08.989380 pibble-0.4.9/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5960 2023-05-01 00:10:08.000000 pibble-0.4.9/README.md
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.973380 pibble-0.4.9/pibble/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8891 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.973380 pibble-0.4.9/pibble/api/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3287 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.973380 pibble-0.4.9/pibble/api/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/client/apachethrift/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6189 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/apachethrift/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1326 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/client/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    14182 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9703 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/hdfs.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12462 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/local.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    19644 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4126 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/client/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4698 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16829 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2330 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/client/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11322 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4770 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10558 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6564 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/soap.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7325 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/webservice/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/client/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/configuration.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6085 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/exceptions.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/helpers/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15593 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    20508 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24123 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/googlerpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13134 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/store.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13916 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/helpers/wrappers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/meta/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/meta/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9353 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/meta/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2958 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/meta/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/apachethrift/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/apachethrift/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/apachethrift/screening.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3112 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/database/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      438 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/file/temp.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/googlerpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/googlerpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/googlerpc/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/googlerpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/googlerpc/metadata.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3027 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.977380 pibble-0.4.9/pibble/api/middleware/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/middleware/webservice/authentication/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/basic.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/bearer.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13466 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/digest.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/header.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17694 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/authentication/oauth.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3248 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/limit.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/middleware/webservice/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/protocol/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/protocol/__init__.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19471 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/protocol/apachethrift.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2443 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1983 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15450 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5445 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2377 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7264 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/awslambda.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    41732 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15532 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/handler.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3182 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/webservice/mixin/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/mixin/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      718 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/mixin/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      987 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4212 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6486 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11970 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16833 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/soap.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/api/server/webservice/template/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9667 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/template/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9195 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/template/extensions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9764 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/api/server/webservice/template/loader.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7772 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/dedupe.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10216 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/engine.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/exceptions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    26389 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/orm.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2667 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/database/util.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/ext/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.981380 pibble-0.4.9/pibble/ext/cms/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/cms/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/interface.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/menu.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/database/view.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/cms/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6382 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2998 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/server/extension.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      350 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/cms/server/mixin.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/dam/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/dam/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/database/files.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/dam/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/dam/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/rest/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/rest/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/database/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/rest/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15691 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7707 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/rest/server/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/session/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/session/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/database/session.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/session/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5026 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/session/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/user/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/user/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/client/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      963 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/user/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/notification.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/permission.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/database/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/ext/user/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24969 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/ext/user/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/hooks/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/hooks/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5971 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/hooks/aws.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/media/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/media/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10234 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/media/thumbnail.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.985380 pibble-0.4.9/pibble/resources/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/resources/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10649 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/resources/retriever.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.989380 pibble-0.4.9/pibble/util/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8375 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/encryption.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16134 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/files.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    32731 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/helpers.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/imaging.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/log.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1610 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/numeric.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    27059 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/util/strings.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.989380 pibble-0.4.9/pibble/web/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/web/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble/web/scraper.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-01 00:10:08.973380 pibble-0.4.9/pibble.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6435 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5413 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1872 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-01 00:10:08.000000 pibble-0.4.9/pibble.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-01 00:10:08.989380 pibble-0.4.9/setup.cfg
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-01 00:10:08.000000 pibble-0.4.9/setup.py
```

### Comparing `pibble-0.4.8/PKG-INFO` & `pibble-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.4.8
+Version: 0.4.9
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.4.8/README.md` & `pibble-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/__main__.py` & `pibble-0.4.9/pibble/__main__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/base.py` & `pibble-0.4.9/pibble/api/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/apachethrift/__init__.py` & `pibble-0.4.9/pibble/api/client/apachethrift/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/apachethrift/wrapper.py` & `pibble-0.4.9/pibble/api/client/apachethrift/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/base.py` & `pibble-0.4.9/pibble/api/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/file/base.py` & `pibble-0.4.9/pibble/api/client/file/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/file/ftp.py` & `pibble-0.4.9/pibble/api/client/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/file/hdfs.py` & `pibble-0.4.9/pibble/api/client/file/hdfs.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/file/local.py` & `pibble-0.4.9/pibble/api/client/file/local.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/file/sftp.py` & `pibble-0.4.9/pibble/api/client/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/googlerpc.py` & `pibble-0.4.9/pibble/api/client/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/webservice/apachethrift.py` & `pibble-0.4.9/pibble/api/client/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/webservice/base.py` & `pibble-0.4.9/pibble/api/client/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/webservice/jsonapi.py` & `pibble-0.4.9/pibble/api/client/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/webservice/rpc/base.py` & `pibble-0.4.9/pibble/api/client/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/webservice/rpc/jsonrpc.py` & `pibble-0.4.9/pibble/api/client/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/webservice/rpc/xmlrpc.py` & `pibble-0.4.9/pibble/api/client/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/webservice/soap.py` & `pibble-0.4.9/pibble/api/client/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/webservice/wrapper.py` & `pibble-0.4.9/pibble/api/client/webservice/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/client/wrapper.py` & `pibble-0.4.9/pibble/api/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/configuration.py` & `pibble-0.4.9/pibble/api/configuration.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/exceptions.py` & `pibble-0.4.9/pibble/api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pibble.util.helpers import qualify
 
 try:
     from thrift.Thrift import TApplicationException
 except ImportError:
     TApplicationException: Type = Exception  # type: ignore[no-redef]
 
+
 class ApacheThriftError(TApplicationException):
     """
     An exception wrapping around TApplicationExceptions, to pass up to the thrift server layer.
 
     :param cause Exception: The exception to wrap.
     """
```

### Comparing `pibble-0.4.8/pibble/api/helpers/apachethrift.py` & `pibble-0.4.9/pibble/api/helpers/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/helpers/authentication.py` & `pibble-0.4.9/pibble/api/helpers/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/helpers/googlerpc.py` & `pibble-0.4.9/pibble/api/helpers/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/helpers/store.py` & `pibble-0.4.9/pibble/api/helpers/store.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/helpers/wrappers.py` & `pibble-0.4.9/pibble/api/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/meta/base.py` & `pibble-0.4.9/pibble/api/meta/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/meta/helpers.py` & `pibble-0.4.9/pibble/api/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/apachethrift/base.py` & `pibble-0.4.9/pibble/api/middleware/apachethrift/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/apachethrift/screening.py` & `pibble-0.4.9/pibble/api/middleware/apachethrift/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/database/orm.py` & `pibble-0.4.9/pibble/api/middleware/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/googlerpc/authentication.py` & `pibble-0.4.9/pibble/api/middleware/googlerpc/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/googlerpc/base.py` & `pibble-0.4.9/pibble/api/middleware/googlerpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/googlerpc/metadata.py` & `pibble-0.4.9/pibble/api/middleware/googlerpc/metadata.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/screening.py` & `pibble-0.4.9/pibble/api/middleware/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/webservice/authentication/basic.py` & `pibble-0.4.9/pibble/api/middleware/webservice/authentication/basic.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/webservice/authentication/bearer.py` & `pibble-0.4.9/pibble/api/middleware/webservice/authentication/bearer.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/webservice/authentication/digest.py` & `pibble-0.4.9/pibble/api/middleware/webservice/authentication/digest.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/webservice/authentication/header.py` & `pibble-0.4.9/pibble/api/middleware/webservice/authentication/header.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/webservice/authentication/oauth.py` & `pibble-0.4.9/pibble/api/middleware/webservice/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/webservice/base.py` & `pibble-0.4.9/pibble/api/middleware/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/webservice/limit.py` & `pibble-0.4.9/pibble/api/middleware/webservice/limit.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/middleware/webservice/screening.py` & `pibble-0.4.9/pibble/api/middleware/webservice/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/protocol/apachethrift.py` & `pibble-0.4.9/pibble/api/protocol/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/apachethrift.py` & `pibble-0.4.9/pibble/api/server/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/base.py` & `pibble-0.4.9/pibble/api/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/file/ftp.py` & `pibble-0.4.9/pibble/api/server/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/file/sftp.py` & `pibble-0.4.9/pibble/api/server/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/googlerpc.py` & `pibble-0.4.9/pibble/api/server/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/apachethrift.py` & `pibble-0.4.9/pibble/api/server/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/awslambda.py` & `pibble-0.4.9/pibble/api/server/webservice/awslambda.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/base.py` & `pibble-0.4.9/pibble/api/server/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/handler.py` & `pibble-0.4.9/pibble/api/server/webservice/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,18 @@
         self.cache_response = cache_response
 
     def bind(self, **kwargs: Any) -> WebServiceAPIBoundHandler:
         return WebServiceAPIBoundHandler(self, **kwargs)
 
     def __repr__(self) -> str:
         return "{0} {1}: {2}{3}".format(
-            ", ".join(self.methods), self.pattern, self.function.__name__,
-            "" if not self.reverse else ", reverse: {0}".format(self.reverse)
+            ", ".join(self.methods),
+            self.pattern,
+            self.function.__name__,
+            "" if not self.reverse else ", reverse: {0}".format(self.reverse),
         )
 
     def __call__(
         self,
         server: APIServerBase,
         request: Request,
         response: Response,
```

### Comparing `pibble-0.4.8/pibble/api/server/webservice/jsonapi.py` & `pibble-0.4.9/pibble/api/server/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/mixin/base.py` & `pibble-0.4.9/pibble/api/server/webservice/mixin/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/orm.py` & `pibble-0.4.9/pibble/api/server/webservice/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/rpc/base.py` & `pibble-0.4.9/pibble/api/server/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/rpc/jsonrpc.py` & `pibble-0.4.9/pibble/api/server/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/rpc/xmlrpc.py` & `pibble-0.4.9/pibble/api/server/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/soap.py` & `pibble-0.4.9/pibble/api/server/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/template/__init__.py` & `pibble-0.4.9/pibble/api/server/webservice/template/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/template/extensions.py` & `pibble-0.4.9/pibble/api/server/webservice/template/extensions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/api/server/webservice/template/loader.py` & `pibble-0.4.9/pibble/api/server/webservice/template/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,36 +151,52 @@
         for extension in extensions:
             extension = type(
                 "{0}Extension".format(extension.__name__), (extension,), lambdas
             )
 
             if issubclass(extension, TestExtensionBase):
                 if extension in self.tests:
-                    logger.debug("Tried to extend template loader with duplicate test {0}".format(extension))
+                    logger.debug(
+                        "Tried to extend template loader with duplicate test {0}".format(
+                            extension
+                        )
+                    )
                     return
                 logger.debug("Template loader adding test {0}".format(extension))
                 self.tests.append(extension)
                 extension.assign(self.environment)
             elif issubclass(extension, FilterExtensionBase):
                 if extension in self.filters:
-                    logger.debug("Tried to extend template loader with duplicate filter {0}".format(extension))
+                    logger.debug(
+                        "Tried to extend template loader with duplicate filter {0}".format(
+                            extension
+                        )
+                    )
                     return
                 logger.debug("Template loader adding filter {0}".format(extension))
                 self.filters.append(extension)
                 extension.assign(self.environment)
             elif issubclass(extension, FunctionExtensionBase):
                 if extension in self.functions:
-                    logger.debug("Tried to extend template loader with duplicate function {0}".format(extension))
+                    logger.debug(
+                        "Tried to extend template loader with duplicate function {0}".format(
+                            extension
+                        )
+                    )
                     return
                 logger.debug("Template loader adding function {0}".format(extension))
                 self.functions.append(extension)
                 extension.assign(self.environment)
             elif issubclass(extension, Extension):
                 if extension in self.extensions:
-                    logger.debug("Tried to extend template loader with duplicate extension {0}".format(extension))
+                    logger.debug(
+                        "Tried to extend template loader with duplicate extension {0}".format(
+                            extension
+                        )
+                    )
                     return
                 logger.debug("Template loader adding extension {0}".format(extension))
                 self.extensions.append(extension)
                 self.environment.add_extension(extension)
             else:
                 raise ConfigurationError(
                     "Extension does not extend either a base or assignable Jinja2 extension."
```

### Comparing `pibble-0.4.8/pibble/database/dedupe.py` & `pibble-0.4.9/pibble/database/dedupe.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/database/engine.py` & `pibble-0.4.9/pibble/database/engine.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/database/orm.py` & `pibble-0.4.9/pibble/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/database/util.py` & `pibble-0.4.9/pibble/database/util.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/cms/database/__init__.py` & `pibble-0.4.9/pibble/ext/cms/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/cms/database/interface.py` & `pibble-0.4.9/pibble/ext/cms/database/interface.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/cms/database/menu.py` & `pibble-0.4.9/pibble/ext/cms/database/menu.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/cms/database/view.py` & `pibble-0.4.9/pibble/ext/cms/database/view.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/cms/server/base.py` & `pibble-0.4.9/pibble/ext/cms/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/cms/server/extension.py` & `pibble-0.4.9/pibble/ext/cms/server/extension.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/dam/database/files.py` & `pibble-0.4.9/pibble/ext/dam/database/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/rest/server/base.py` & `pibble-0.4.9/pibble/ext/rest/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/rest/server/user.py` & `pibble-0.4.9/pibble/ext/rest/server/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/session/database/session.py` & `pibble-0.4.9/pibble/ext/session/database/session.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/session/server/base.py` & `pibble-0.4.9/pibble/ext/session/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/user/client/base.py` & `pibble-0.4.9/pibble/ext/user/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/user/database/__init__.py` & `pibble-0.4.9/pibble/ext/user/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/user/database/authentication.py` & `pibble-0.4.9/pibble/ext/user/database/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/user/database/notification.py` & `pibble-0.4.9/pibble/ext/user/database/notification.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/user/database/permission.py` & `pibble-0.4.9/pibble/ext/user/database/permission.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/user/database/user.py` & `pibble-0.4.9/pibble/ext/user/database/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/ext/user/server/base.py` & `pibble-0.4.9/pibble/ext/user/server/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,35 +544,36 @@
         """
         user = (
             self.database.query(self.orm.User)
             .filter(self.orm.User.id == 0)
             .one_or_none()
         )
         if not user:
-            user = self.orm.User(id = 0, email = "noauth", superuser = True)
+            user = self.orm.User(id=0, email="noauth", superuser=True)
             self.database.add(user)
             self.database.commit()
 
         token = self.orm.AuthenticationToken(
             access_token=get_uuid(),
             refresh_token=get_uuid(),
             token_type=self.token_type,
-            user_id=user.id
+            user_id=user.id,
         )
-        
+
         user.last_login = datetime.datetime.now()
 
         self.database.add(token)
         self.database.commit()
 
         return token
 
 
 handlers = UserExtensionHandlerRegistry()
 
+
 class UserExtensionServer(UserExtensionServerBase):
     """
     This base class defines default handlers, if desired.
     """
 
     @classmethod
     def get_handlers(cls) -> UserExtensionHandlerRegistry:
```

### Comparing `pibble-0.4.8/pibble/hooks/aws.py` & `pibble-0.4.9/pibble/hooks/aws.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/media/thumbnail.py` & `pibble-0.4.9/pibble/media/thumbnail.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,15 @@
             )
             return ThumbnailBuilder(
                 os.path.join(tempfiles.directory, output_file)
             ).build(output, width, height)
 
     def _build_browser(self, output: str, width: int, height: int) -> Image.Image:
         from pibble.web.scraper import WebScraper
+
         logger.debug(f"Building browser thumbnail from {self.filename} to {output}")
         tempfiles = TempfileContext()
         with tempfiles as generator:
             screenshot = tempfiles.touch("screenshot.png")
             with WebScraper(1920, 1080) as scraper:
                 if not has_protocol_regex.match(self.filename):
                     path = "file://{0}".format(os.path.abspath(self.filename))
@@ -257,26 +258,28 @@
                 scraper.get(path)
                 scraper.save_screenshot(screenshot)
                 return ThumbnailBuilder(screenshot).build(output, width, height)
 
     def _build_pdf(self, output: str, width: int, height: int) -> Image.Image:
         logger.debug(f"Building PDF thumbnail from {self.filename} to {output}")
         from pdf2image import convert_from_path
+
         tempfiles = TempfileContext()
         with tempfiles as generator:
             images_from_path = convert_from_path(
                 self.filename, output_folder=tempfiles.directory
             )
             page_1 = images_from_path[0]
             page_1.thumbnail((width, height))
             page_1.save(output)
         return page_1
 
     def _build_psd(self, output: str, width: int, height: int) -> Image.Image:
         from psd_tools import PSDImage
+
         logger.debug(f"Building PSD thumbnail from {self.filename} to {output}")
         psd = PSDImage.open(self.filename)
         image = psd.composite()
         image.thumbnail((width, height))
         image.save(output)
         return image
```

### Comparing `pibble-0.4.8/pibble/resources/retriever.py` & `pibble-0.4.9/pibble/resources/retriever.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/setup.py` & `pibble-0.4.9/pibble/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "4"
-version_patch = "8"
+version_patch = "9"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
@@ -58,15 +58,15 @@
         "types-protobuf>=4.22,<5.0",
         "types-paramiko>=3.0,<4.0",
         "types-oauthlib>=3.2,<4.0",
         "types-openpyxl==3.0.0",
         "types-urllib3<1.27",
         "importchecker>=2.0,<3.0",
         "black>=23.3,<24.0",
-        "twine>=4.0,<5.0"
+        "twine>=4.0,<5.0",
     ],
 }
 
 extras_require["all"] = [
     package for package_list in extras_require.values() for package in package_list
 ]
```

### Comparing `pibble-0.4.8/pibble/util/encryption.py` & `pibble-0.4.9/pibble/util/encryption.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/util/files.py` & `pibble-0.4.9/pibble/util/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/util/helpers.py` & `pibble-0.4.9/pibble/util/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/util/imaging.py` & `pibble-0.4.9/pibble/util/imaging.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/util/log.py` & `pibble-0.4.9/pibble/util/log.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/util/numeric.py` & `pibble-0.4.9/pibble/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble/util/strings.py` & `pibble-0.4.9/pibble/util/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import io
 import sys
+import base64
 import string
 import hashlib
 
 import email.parser
 
 from re import compile, sub, split
 from typing import Any, TypedDict, Optional, Union, Tuple, cast
 from random import choice, shuffle
 from uuid import uuid4, UUID
 from json import dumps, loads, JSONDecodeError
 from numpy import nan, isnan
 from datetime import datetime, date, time
 from chardet import detect
 from urllib.parse import unquote
+from PIL import Image
 
 from pibble.util.log import logger
 
 EMPTY_CASE = compile(r"^$")
 LOWER_CASE = compile(r"^[a-z0-9]+$")
 UPPER_CASE = compile(r"^[A-Z0-9]+$")
 SNAKE_CASE = compile(r"^[A-Za-z0-9]+(_[A-Za-z0-9]+)+$")
@@ -49,14 +51,34 @@
     try:
         loaded = loads(to_parse)
         return [FlexibleStringer.parse(i) for i in loaded]
     except JSONDecodeError:
         return to_parse
 
 
+def serialize_image(image: Image.Image, **kwargs: Any) -> str:
+    """
+    Serializes an image to a base64 Data URI.
+    """
+    image_byte_io = io.BytesIO()
+    image.save(image_byte_io, format="PNG")
+    image_bytestring = base64.b64encode(image_byte_io.getvalue()).decode("utf-8")
+    return f"data:image/png;base64,{image_bytestring}"
+
+
+def deserialize_image(image_string: str, **kwargs: Any) -> Image.Image:
+    """
+    Deserializes an image from a base64 Data URI.
+    """
+    image_bytestring = image_string.split(",")[1]
+    logger.debug(image_bytestring)
+    image_bytes = base64.b64decode(image_bytestring)
+    return Image.open(io.BytesIO(image_bytes))
+
+
 class FlexibleStringer:
     """
     A class that takes a string and attempts to parse it into an object by matching
     it with a regular expression, and vice-versa.
 
     >>> from pibble.util.strings import FlexibleStringer
     >>> from datetime import datetime
@@ -76,14 +98,15 @@
     '2018-01-01T00:00:00'
 
     :param parameter str: The string to attempt to parse.
     :returns object: Either the parameter itself, or the parsed version of it.
     """
 
     PARSE_FORMATS = {
+        compile(r"^data:image/.+;base64,.+$"): lambda p: deserialize_image(p),
         compile(r"^[0-9\,]+$"): lambda p: int(p.replace(",", "")),
         compile(r"^[0-9\,]+\.[0-9\,]+$"): lambda p: float(p.replace(",", "")),
         compile(r"^(null|Null|NULL|none|None|NONE)$"): lambda p: None,
         compile(
             r"^(y|Y|yes|Yes|YES|t|T|true|True|TRUE|n|N|no|No|NO|f|F|false|False|FALSE)$"
         ): lambda p: p.lower()
         in ["t", "true", "y", "yes"],
@@ -137,14 +160,15 @@
             r"^\d{4}-\d{1,2}-\d{1,2}\ \d{1,2}:\d{1,2}:\d{1,2}\.\d+$"
         ): lambda p: datetime.strptime(p, "%Y-%m-%d %H:%M:%S.%f"),
         compile(r"^\{.*\}$"): lambda p: try_json_dict_parse(p),
         compile(r"^\[.*\]$"): lambda p: try_json_list_parse(p),
     }
 
     SERIALIZE_FORMATS = {
+        Image.Image: lambda p, **k: serialize_image(p, **k),
         nan: lambda p, **k: "null",
         type(None): lambda p, **k: "null",
         str: lambda p, **k: p,
         bytes: lambda p, **k: decode(p),
         datetime: lambda p, **k: p.isoformat(),
         date: lambda p, **k: p.isoformat(),
         time: lambda p, **k: p.isoformat(),
```

### Comparing `pibble-0.4.8/pibble/web/scraper.py` & `pibble-0.4.9/pibble/web/scraper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble.egg-info/PKG-INFO` & `pibble-0.4.9/pibble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.4.8
+Version: 0.4.9
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.4.8/pibble.egg-info/SOURCES.txt` & `pibble-0.4.9/pibble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/pibble.egg-info/requires.txt` & `pibble-0.4.9/pibble.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.4.8/setup.py` & `pibble-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "4"
-version_patch = "8"
+version_patch = "9"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
@@ -58,15 +58,15 @@
         "types-protobuf>=4.22,<5.0",
         "types-paramiko>=3.0,<4.0",
         "types-oauthlib>=3.2,<4.0",
         "types-openpyxl==3.0.0",
         "types-urllib3<1.27",
         "importchecker>=2.0,<3.0",
         "black>=23.3,<24.0",
-        "twine>=4.0,<5.0"
+        "twine>=4.0,<5.0",
     ],
 }
 
 extras_require["all"] = [
     package for package_list in extras_require.values() for package in package_list
 ]
```

