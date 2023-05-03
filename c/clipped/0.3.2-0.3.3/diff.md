# Comparing `tmp/clipped-0.3.2.tar.gz` & `tmp/clipped-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.3.2.tar", last modified: Mon May  1 21:11:19 2023, max compression
+gzip compressed data, was "clipped-0.3.3.tar", last modified: Wed May  3 11:51:45 2023, max compression
```

## Comparing `clipped-0.3.2.tar` & `clipped-0.3.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-01 21:11:19.441573 clipped-0.3.2/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-05-01 21:10:00.000000 clipped-0.3.2/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-05-01 21:11:19.441669 clipped-0.3.2/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-01 21:11:19.429200 clipped-0.3.2/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-01 21:11:19.431784 clipped-0.3.2/clipped/config/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)       91 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/constants.py
--rw-r--r--   0 mourad     (501) staff       (20)      312 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/contexts.py
--rw-r--r--   0 mourad     (501) staff       (20)       40 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/exceptions.py
--rw-r--r--   0 mourad     (501) staff       (20)     8943 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/manager.py
--rw-r--r--   0 mourad     (501) staff       (20)     6138 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/parser.py
--rw-r--r--   0 mourad     (501) staff       (20)      527 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/patch_strategy.py
--rw-r--r--   0 mourad     (501) staff       (20)     4047 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/reader.py
--rw-r--r--   0 mourad     (501) staff       (20)    15121 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/schema.py
--rw-r--r--   0 mourad     (501) staff       (20)     8892 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/config/spec.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-01 21:11:19.432646 clipped-0.3.2/clipped/decorators/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/decorators/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/decorators/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/decorators/deprecation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/decorators/memoization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/decorators/signals.py
--rw-r--r--   0 mourad     (501) staff       (20)     6256 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/py.typed
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-01 21:11:19.435114 clipped-0.3.2/clipped/types/
--rw-r--r--   0 mourad     (501) staff       (20)     3914 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/docker_image.py
--rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/email.py
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)      698 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      158 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/numbers.py
--rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/ref_or_obj.py
--rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)      965 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/uri.py
--rw-r--r--   0 mourad     (501) staff       (20)      688 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/uuids.py
--rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/types/wasb.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-01 21:11:19.441415 clipped-0.3.2/clipped/utils/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1655 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/assertions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/bools.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/click.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/csv.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/dates.py
--rw-r--r--   0 mourad     (501) staff       (20)     3358 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/dicts.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/enums.py
--rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/git.py
--rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/http.py
--rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      420 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/json.py
--rw-r--r--   0 mourad     (501) staff       (20)     1163 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/logging.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/np.py
--rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/paths.py
--rw-r--r--   0 mourad     (501) staff       (20)      674 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/requests.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/responses.py
--rw-r--r--   0 mourad     (501) staff       (20)      595 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/tz.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/units.py
--rw-r--r--   0 mourad     (501) staff       (20)      282 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/urls.py
--rw-r--r--   0 mourad     (501) staff       (20)      614 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/workers.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-05-01 21:10:00.000000 clipped-0.3.2/clipped/utils/yaml.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-01 21:11:19.429976 clipped-0.3.2/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-05-01 21:11:19.000000 clipped-0.3.2/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1901 2023-05-01 21:11:19.000000 clipped-0.3.2/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-05-01 21:11:19.000000 clipped-0.3.2/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-05-01 21:11:19.000000 clipped-0.3.2/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-05-01 21:11:19.442179 clipped-0.3.2/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-05-01 21:10:00.000000 clipped-0.3.2/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-03 11:51:45.991539 clipped-0.3.3/
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-05-03 11:50:51.000000 clipped-0.3.3/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-05-03 11:51:45.991644 clipped-0.3.3/PKG-INFO
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-03 11:51:45.979050 clipped-0.3.3/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-03 11:51:45.981785 clipped-0.3.3/clipped/config/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)       91 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/constants.py
+-rw-r--r--   0 mourad     (501) staff       (20)      312 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/contexts.py
+-rw-r--r--   0 mourad     (501) staff       (20)       40 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/exceptions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8943 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/manager.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6138 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/parser.py
+-rw-r--r--   0 mourad     (501) staff       (20)      527 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/patch_strategy.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4047 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/reader.py
+-rw-r--r--   0 mourad     (501) staff       (20)    15121 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8892 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/config/spec.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-03 11:51:45.982718 clipped-0.3.3/clipped/decorators/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/decorators/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/decorators/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4313 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/decorators/deprecation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/decorators/memoization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/decorators/signals.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6256 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/py.typed
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-03 11:51:45.984891 clipped-0.3.3/clipped/types/
+-rw-r--r--   0 mourad     (501) staff       (20)     3914 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/docker_image.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/email.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)      698 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      158 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/numbers.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/ref_or_obj.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)      965 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/uri.py
+-rw-r--r--   0 mourad     (501) staff       (20)      688 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/uuids.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/types/wasb.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-03 11:51:45.991382 clipped-0.3.3/clipped/utils/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1655 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/assertions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/bools.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/click.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/csv.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/dates.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3358 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/dicts.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/enums.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/git.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/http.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      420 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/json.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1163 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/logging.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/np.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/paths.py
+-rw-r--r--   0 mourad     (501) staff       (20)      674 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/requests.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/responses.py
+-rw-r--r--   0 mourad     (501) staff       (20)      595 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      676 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/tz.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/units.py
+-rw-r--r--   0 mourad     (501) staff       (20)      282 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/urls.py
+-rw-r--r--   0 mourad     (501) staff       (20)      614 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/workers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-05-03 11:50:51.000000 clipped-0.3.3/clipped/utils/yaml.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-03 11:51:45.979994 clipped-0.3.3/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-05-03 11:51:45.000000 clipped-0.3.3/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1901 2023-05-03 11:51:45.000000 clipped-0.3.3/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-05-03 11:51:45.000000 clipped-0.3.3/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-05-03 11:51:45.000000 clipped-0.3.3/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-05-03 11:51:45.992163 clipped-0.3.3/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-05-03 11:50:51.000000 clipped-0.3.3/setup.py
```

### Comparing `clipped-0.3.2/PKG-INFO` & `clipped-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.3.2
+Version: 0.3.3
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.3.2 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.3.3 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.3.2/clipped/config/manager.py` & `clipped-0.3.3/clipped/config/manager.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/config/parser.py` & `clipped-0.3.3/clipped/config/parser.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/config/patch_strategy.py` & `clipped-0.3.3/clipped/config/patch_strategy.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/config/reader.py` & `clipped-0.3.3/clipped/config/reader.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/config/schema.py` & `clipped-0.3.3/clipped/config/schema.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/config/spec.py` & `clipped-0.3.3/clipped/config/spec.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/decorators/cached_property.py` & `clipped-0.3.3/clipped/decorators/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/decorators/deprecation.py` & `clipped-0.3.3/clipped/decorators/deprecation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import functools
-import warnings
+import logging
 
 from typing import Optional, Tuple
 
 from clipped.utils.versions import compare_versions
 
 
 class DeprecatedWarning(DeprecationWarning):
@@ -83,15 +83,15 @@
 
         message = get_deprecation_warning_message(
             deprecation_version=deprecation_version,
             latest_version=latest_version,
             current_logic=current_logic,
             new_logic=new_logic,
         )
-        warnings.warn(cls(message, details), category=DeprecationWarning, stacklevel=2)
+        logging.warning(cls(message, details))
 
 
 def deprecated(
     deprecation_version: Optional[str] = None,
     latest_version: Optional[str] = None,
     current_version: Optional[str] = None,
     current_logic: Optional[str] = None,
```

### Comparing `clipped-0.3.2/clipped/decorators/memoization.py` & `clipped-0.3.3/clipped/decorators/memoization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/decorators/signals.py` & `clipped-0.3.3/clipped/decorators/signals.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/formatting.py` & `clipped-0.3.3/clipped/formatting.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/manager_interface.py` & `clipped-0.3.3/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/__init__.py` & `clipped-0.3.3/clipped/types/__init__.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/docker_image.py` & `clipped-0.3.3/clipped/types/docker_image.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/email.py` & `clipped-0.3.3/clipped/types/email.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/gcs.py` & `clipped-0.3.3/clipped/types/gcs.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/lists.py` & `clipped-0.3.3/clipped/types/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/ref_or_obj.py` & `clipped-0.3.3/clipped/types/ref_or_obj.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/s3.py` & `clipped-0.3.3/clipped/types/s3.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/strings.py` & `clipped-0.3.3/clipped/types/strings.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/uri.py` & `clipped-0.3.3/clipped/types/uri.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/uuids.py` & `clipped-0.3.3/clipped/types/uuids.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/types/wasb.py` & `clipped-0.3.3/clipped/types/wasb.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/assertions.py` & `clipped-0.3.3/clipped/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/bools.py` & `clipped-0.3.3/clipped/utils/bools.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/cmd.py` & `clipped-0.3.3/clipped/utils/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/coroutine.py` & `clipped-0.3.3/clipped/utils/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/csv.py` & `clipped-0.3.3/clipped/utils/csv.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/dates.py` & `clipped-0.3.3/clipped/utils/dates.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/dicts.py` & `clipped-0.3.3/clipped/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/enums.py` & `clipped-0.3.3/clipped/utils/enums.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/env.py` & `clipped-0.3.3/clipped/utils/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/git.py` & `clipped-0.3.3/clipped/utils/git.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/hashing.py` & `clipped-0.3.3/clipped/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/http.py` & `clipped-0.3.3/clipped/utils/http.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/humanize.py` & `clipped-0.3.3/clipped/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/imports.py` & `clipped-0.3.3/clipped/utils/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/indentation.py` & `clipped-0.3.3/clipped/utils/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/lists.py` & `clipped-0.3.3/clipped/utils/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/np.py` & `clipped-0.3.3/clipped/utils/np.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/paths.py` & `clipped-0.3.3/clipped/utils/paths.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/query_params.py` & `clipped-0.3.3/clipped/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/requests.py` & `clipped-0.3.3/clipped/utils/requests.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/responses.py` & `clipped-0.3.3/clipped/utils/responses.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/sanitizers.py` & `clipped-0.3.3/clipped/utils/sanitizers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/serialization.py` & `clipped-0.3.3/clipped/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/strings.py` & `clipped-0.3.3/clipped/utils/strings.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/tz.py` & `clipped-0.3.3/clipped/utils/tz.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/units.py` & `clipped-0.3.3/clipped/utils/units.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/validation.py` & `clipped-0.3.3/clipped/utils/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/versions.py` & `clipped-0.3.3/clipped/utils/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/workers.py` & `clipped-0.3.3/clipped/utils/workers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped/utils/yaml.py` & `clipped-0.3.3/clipped/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/clipped.egg-info/PKG-INFO` & `clipped-0.3.3/clipped.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.3.2
+Version: 0.3.3
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.3.2 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.3.3 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.3.2/clipped.egg-info/SOURCES.txt` & `clipped-0.3.3/clipped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/setup.cfg` & `clipped-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `clipped-0.3.2/setup.py` & `clipped-0.3.3/setup.py`

 * *Files identical despite different names*

