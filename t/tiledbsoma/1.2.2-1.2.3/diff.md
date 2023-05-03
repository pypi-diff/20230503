# Comparing `tmp/tiledbsoma-1.2.2.tar.gz` & `tmp/tiledbsoma-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledbsoma-1.2.2.tar", last modified: Wed Apr 26 00:03:44 2023, max compression
+gzip compressed data, was "tiledbsoma-1.2.3.tar", last modified: Wed May  3 20:56:22 2023, max compression
```

## Comparing `tiledbsoma-1.2.2.tar` & `tiledbsoma-1.2.3.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-26 00:03:40.000000 tiledbsoma-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-04-26 00:03:40.000000 tiledbsoma-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-26 00:03:42.000000 tiledbsoma-1.2.2/RELEASE-VERSION
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-26 00:03:40.000000 tiledbsoma-1.2.2/dist_links/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     9437 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4058 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     4894 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     6323 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Superbuild.cmake
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/inputs/
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/reader.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/reader.uml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.878294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/span/
--rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/span/span.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     7148 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/producer_consumer_queue.h
--rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/status.h
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/thread_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.878294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/status.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6700 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.878294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/array_buffers.h
--rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/arrow_adapter.h
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/carrow.h
--rw-r--r--   0 runner    (1001) docker     (122)     7819 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/column_buffer.h
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/common.h
--rw-r--r--   0 runner    (1001) docker     (122)     2959 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/logger_public.h
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/managed_query.h
--rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/soma_array_reader.h
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/spdlog_with_R.h
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/stats.h
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/tiledbsoma
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/util.h
--rw-r--r--   0 runner    (1001) docker     (122)     1728 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/version.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.886294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/
--rw-r--r--   0 runner    (1001) docker     (122)     9518 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/cli.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7087 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/logger.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7934 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/logger.h
--rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    13037 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/soma_array_reader.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/stats.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/util.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/version.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.886294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6525 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (122)     7879 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_soma_array_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)     8829 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_soma_array_reader.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.886294 tiledbsoma-1.2.2/dist_links/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)     2811 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/bld
--rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/run-clang-format.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/show-versions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/update-tiledb-version.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.878294 tiledbsoma-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_arrow_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    26853 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     6993 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_common_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    33545 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6863 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_dense_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6712 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_general_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     2550 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_read_iters.py
--rw-r--r--   0 runner    (1001) docker     (122)    11747 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_sparse_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_tdb_handles.py
--rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_tiledb_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     9229 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_tiledb_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/eta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/experiment_query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/src/tiledbsoma/io/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/io/conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    53522 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/io/ingest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/src/tiledbsoma/options/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4049 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/options/_soma_tiledb_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/options/_tiledb_create_options.py
--rw-r--r--   0 runner    (1001) docker     (122)    26675 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/pytiledbsoma.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7781 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/query_condition.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-03 20:56:18.000000 tiledbsoma-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-03 20:56:18.000000 tiledbsoma-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-03 20:56:20.000000 tiledbsoma-1.2.3/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-05-03 20:56:18.000000 tiledbsoma-1.2.3/dist_links/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     6296 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Superbuild.cmake
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/inputs/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/reader.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/reader.uml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    10856 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/cli/cli.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.094111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/span/
+-rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/span/span.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     7148 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.094111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6700 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/
+-rw-r--r--   0 runner    (1001) docker     (122)     7122 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10172 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/managed_query.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14657 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15129 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/soma_array.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/logger_public.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.102111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/array_buffers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7272 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/carrow.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/column_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/logger.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7864 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/logger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/stats.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/stats.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/util.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/util.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/version.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/version.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.102111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_soma_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10346 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.102111 tiledbsoma-1.2.3/dist_links/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2811 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/bld
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/run-clang-format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/show-versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/update-tiledb-version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.094111 tiledbsoma-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_arrow_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26933 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7045 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_common_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33607 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6863 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_dense_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_general_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_read_iters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11735 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_sparse_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_tdb_handles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_tiledb_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_tiledb_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/eta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/experiment_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/src/tiledbsoma/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/io/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53795 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/io/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/src/tiledbsoma/options/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/options/_soma_tiledb_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/options/_tiledb_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/pytiledbsoma.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7781 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/query_condition.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/version.py
```

### Comparing `tiledbsoma-1.2.2/PKG-INFO` & `tiledbsoma-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.2.2/README.md` & `tiledbsoma-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/CMakeLists.txt` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,14 @@
 # so the option is forwarded to the non-superbuild
 if(TILEDBSOMA_BUILD_R)
   # Disable build targets when building for R
   set(TILEDBSOMA_BUILD_PYTHON OFF)
   set(TILEDBSOMA_BUILD_CLI OFF)
   set(TILEDBSOMA_ENABLE_TESTING OFF)
   set(TILEDBSOMA_BUILD_STATIC ON)
-
-  add_compile_options(-DR_BUILD)
 endif()
 
 # Enable compiler cache to speed up recompilation
 find_program(CCACHE_FOUND ccache)
 
 if(CCACHE_FOUND)
   set_property(GLOBAL PROPERTY RULE_LAUNCH_COMPILE ccache)
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/README.md` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 The [Makefile](../Makefile) automates common developer use cases and promotes sharing of consistent build flows.
 
 ```
 Usage: make rule [options]
 
 Rules:
   install [options]   Build C++ library and install python module
-  r-build [options]   Build C++ static library with "#define R_BUILD" for R
+  r-build [options]   Build C++ static library for R
   update              Incrementally build C++ library and update python module
   test                Run tests
   clean               Remove build artifacts
 
 Options:
   build=BUILD_TYPE    Cmake build type = Release|Debug|RelWithDebInfo|Coverage [Release]
   prefix=PREFIX       Install location [dist]
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
   set_target_properties(spdlog::spdlog PROPERTIES
           INTERFACE_INCLUDE_DIRECTORIES "${SPDLOG_INCLUDE_DIR}"
           )
   # If the target is defined we need to handle external fmt build types
 elseif(TARGET spdlog::spdlog)
   if (SPDLOG_FMT_EXTERNAL)
     # Since we are using header only we need to define this
-    add_definitions("-DSPDLOG_FMT_EXTERNAL=1")
+    # cf https://github.com/gabime/spdlog/wiki/0.-FAQ#how-to-use-external-fmt-library-instead-of-the-bundled
+    add_definitions("-DSPDLOG_FMT_EXTERNAL_HO=1")
     find_package(fmt REQUIRED)
     if (${fmt_FOUND})
       target_link_libraries(spdlog::spdlog INTERFACE fmt::fmt)
     endif()
   endif()
 endif()
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake`

 * *Files 11% similar despite different names*

```diff
@@ -54,28 +54,28 @@
     # loaded by the Python and R tiledbsoma packages. Those packages -also- use TileDB-Py and
     # TileDB-R, each of which links their own 'copy' of TileDB Embedded, whose version we don't
     # control here. Ideally the TileDB Embedded versions should match! The show_package_versions()
     # helper function in each package can help to diagnose any mismatch.
     # NB When updating the pinned URLs here, please also update in file apis/r/tools/get_tarball.R
     if(DOWNLOAD_TILEDB_PREBUILT)
         if (WIN32) # Windows
-          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.1/tiledb-windows-x86_64-2.15.1-432d4c2.zip")
-          SET(DOWNLOAD_SHA1 "7235a3bc0b5675ed83762a4290d99c6ff9db285f")
+          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-windows-x86_64-2.15.2-90f30eb.zip")
+          SET(DOWNLOAD_SHA1 "1adc1ffa3c6c0f637bcb68d3cd278b0bee597b9c")
         elseif(APPLE) # OSX
 
           if (CMAKE_OSX_ARCHITECTURES STREQUAL x86_64 OR CMAKE_SYSTEM_PROCESSOR MATCHES "(x86_64)|(AMD64|amd64)|(^i.86$)")
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.1/tiledb-macos-x86_64-2.15.1-432d4c2.tar.gz")
-            SET(DOWNLOAD_SHA1 "f5986f5a85912147e2b839e0968963df6c540688")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-x86_64-2.15.2-90f30eb.tar.gz")
+            SET(DOWNLOAD_SHA1 "616b9ab508d1233d3bc3d6a2a7b1c42c8098f38a")
           elseif (CMAKE_OSX_ARCHITECTURES STREQUAL arm64 OR CMAKE_SYSTEM_PROCESSOR MATCHES "^aarch64" OR CMAKE_SYSTEM_PROCESSOR MATCHES "^arm")
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.1/tiledb-macos-arm64-2.15.1-432d4c2.tar.gz")
-            SET(DOWNLOAD_SHA1 "6abb30f9dd7371d5a06a273008179bd57d691e36")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-arm64-2.15.2-90f30eb.tar.gz")
+            SET(DOWNLOAD_SHA1 "882eadcc256f95a5c91094407770799a8bd4e759")
           endif()
         else() # Linux
-          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.1/tiledb-linux-x86_64-2.15.1-432d4c2.tar.gz")
-          SET(DOWNLOAD_SHA1 "9b705af26007b193800f0382c343d421a8b59003")
+          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-linux-x86_64-2.15.2-90f30eb.tar.gz")
+          SET(DOWNLOAD_SHA1 "33ae11d507dc7bec82fbdfbd8e2b2e13cff16b89")
         endif()
 
         ExternalProject_Add(ep_tiledb
                 PREFIX "externals"
                 URL ${DOWNLOAD_URL}
                 URL_HASH SHA1=${DOWNLOAD_SHA1}
                 CONFIGURE_COMMAND ""
@@ -89,16 +89,16 @@
                 LOG_CONFIGURE FALSE
                 LOG_BUILD FALSE
                 LOG_INSTALL FALSE
                 )
     else() # Build from source
         ExternalProject_Add(ep_tiledb
           PREFIX "externals"
-          URL "https://github.com/TileDB-Inc/TileDB/archive/2.15.1.zip"
-          URL_HASH SHA1=8bb70f7534297b184d23b216b1097fdde40829df
+          URL "https://github.com/TileDB-Inc/TileDB/archive/2.15.2.zip"
+          URL_HASH SHA1=7443415b9f3081e87adaa638dea6e2d277fbb904
           DOWNLOAD_NAME "tiledb.zip"
           CMAKE_ARGS
             -DCMAKE_INSTALL_PREFIX=${EP_INSTALL_PREFIX}
             -DCMAKE_PREFIX_PATH=${EP_INSTALL_PREFIX}
             -DTILEDB_S3=${TILEDB_S3}
             -DTILEDB_AZURE=${TILEDB_AZURE}
             -DTILEDB_GCS=${TILEDB_GCS}
@@ -128,11 +128,11 @@
     list(APPEND FORWARD_EP_CMAKE_ARGS -DEP_TILEDB_BUILT=TRUE)
     list(APPEND EXTERNAL_PROJECTS ep_tiledb)
   else()
     message(FATAL_ERROR "Unable to find TileDB library.")
   endif()
 endif()
 
-if (EP_TILEDB_BUILT AND TARGET TileDB::tiledb_shared AND NOT TILEDBSOMA_BUILD_R)
+if (EP_TILEDB_BUILT AND TARGET TileDB::tiledb_shared)
   include(TileDBCommon)
   install_target_libs(TileDB::tiledb_shared)
 endif()
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Superbuild.cmake` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Superbuild.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
   -DTILEDB_SERIALIZATION=${TILEDB_SERIALIZATION}
   -DTILEDB_WERROR=${TILEDB_WERROR}
   -DTILEDB_VERBOSE=${TILEDB_VERBOSE}
   -DTileDB_DIR=${TileDB_DIR}
   -DSANITIZER=${SANITIZER}
   -DENABLE_ARROW_EXPORT=${ENABLE_ARROW_EXPORT}
   -DOVERRIDE_INSTALL_PREFIX=${OVERRIDE_INSTALL_PREFIX}
-  -DTILEDBSOMA_BUILD_R=${TILEDBSOMA_BUILD_R}
   -DTILEDBSOMA_BUILD_STATIC=${TILEDBSOMA_BUILD_STATIC}
   -DTILEDBSOMA_BUILD_CLI=${TILEDBSOMA_BUILD_CLI}
   -DTILEDBSOMA_ENABLE_TESTING=${TILEDBSOMA_ENABLE_TESTING}
   -DCMAKE_OSX_ARCHITECTURES=${CMAKE_OSX_ARCHITECTURES}
 )
 
 ############################################################
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/patches/spdlog.patch` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/patches/spdlog.patch`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/reader.svg` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/reader.svg`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/reader.uml` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/reader.uml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/.clang-format` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/.clang-format`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/span/span.hpp` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/span/span.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/producer_consumer_queue.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/status.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/thread_pool.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/status.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/thread_pool.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/array_buffers.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/array_buffers.h`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 #define ARRAY_BUFFERS_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <span/span.hpp>
 #include <tiledb/tiledb>
 
-#include "tiledbsoma/column_buffer.h"
-#include "tiledbsoma/common.h"
-#include "tiledbsoma/logger_public.h"
+#include "column_buffer.h"
+#include "common.h"
+#include "logger.h"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 class ArrayBuffers {
    public:
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/arrow_adapter.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/arrow_adapter.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #ifndef ARROW_ADAPTER_H
 #define ARROW_ADAPTER_H
 
-#include <tiledbsoma/tiledbsoma>
+#include <tiledb/tiledb>
+#include "../utils/column_buffer.h"
+#include "../utils/logger.h"
 #ifndef ARROW_SCHEMA_AND_ARRAY_DEFINED
 #include "carrow.h"
 #endif
 
 // https://arrow.apache.org/docs/format/CDataInterface.html
 // https://arrow.apache.org/docs/format/Columnar.html#buffer-listing-for-each-layout
 // https://arrow.apache.org/docs/format/CDataInterface.html#exporting-a-simple-int32-array
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/carrow.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/carrow.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/column_buffer.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/column_buffer.h`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 #define COLUMN_BUFFER_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <span/span.hpp>
 #include <tiledb/tiledb>
 
-#include "tiledbsoma/common.h"
-#include "tiledbsoma/logger_public.h"
+#include "common.h"
+#include "logger.h"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 /**
  * @brief Class to store data for a TileDB dimension or attribute.
@@ -69,16 +69,15 @@
     static std::shared_ptr<ColumnBuffer> create(
         std::shared_ptr<Array> array, std::string_view name);
 
     /**
      * @brief Convert a bytemap to a bitmap in place.
      *
      */
-    __attribute__((visibility("default"))) static void to_bitmap(
-        tcb::span<uint8_t> bytemap);
+    static void to_bitmap(tcb::span<uint8_t> bytemap);
 
     //===================================================================
     //= public non-static
     //===================================================================
 
     /**
      * @brief Construct a new ColumnBuffer object
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/common.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/logger_public.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/logger_public.h`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,15 @@
 
 #pragma once
 #ifndef TILEDB_LOGGER_PUBLIC_H
 #define TILEDB_LOGGER_PUBLIC_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
-#if !defined(R_BUILD)
 #include <spdlog/spdlog.h>
-#else
-#include "tiledbsoma/spdlog_with_R.h"
-#endif
 
 namespace tiledbsoma {
 
 /** Set log level for global logger and optionally set a logfile. */
 __attribute__((visibility("default"))) void LOG_CONFIG(
     const std::string& level, const std::string& logfile = "");
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/managed_query.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/managed_query.h`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 #define MANAGED_QUERY_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 #include <unordered_set>
 
 #include <tiledb/tiledb>
 
-#include "tiledbsoma/array_buffers.h"
-#include "tiledbsoma/column_buffer.h"
-#include "tiledbsoma/common.h"
+#include "utils/array_buffers.h"
+#include "utils/column_buffer.h"
+#include "utils/common.h"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 class ManagedQuery {
    public:
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/soma_array_reader.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/soma_array.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @file   soma_array_reader.h
+ * @file   soma_array.h
  *
  * @section LICENSE
  *
  * The MIT License
  *
  * @copyright Copyright (c) 2022 TileDB, Inc.
  *
@@ -23,114 +23,138 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- *   This declares the SOMAArrayReader
+ *   This declares the SOMAArray
  */
 
-#ifndef SOMA_ARRAY_READER
-#define SOMA_ARRAY_READER
+#ifndef SOMA_ARRAY
+#define SOMA_ARRAY
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <future>
 
 #include <tiledb/tiledb>
 
-#include "tiledbsoma/managed_query.h"
+#include "managed_query.h"
 
 namespace tiledbsoma {
 using namespace tiledb;
 
-class SOMAArrayReader {
+using MetadataValue =
+    std::tuple<std::string, tiledb_datatype_t, uint32_t, const void*>;
+enum MetadataInfo { key = 0, dtype, num, value };
+
+class SOMAArray {
    public:
     //===================================================================
     //= public static
     //===================================================================
 
     /**
-     * @brief Open an array at the specified URI and return SOMAArrayReader
+     * @brief Open an array at the specified URI and return SOMAArray
      * object.
      *
+     * @param mode TILEDB_READ or TILEDB_WRITE
      * @param uri URI of the array
      * @param name Name of the array
      * @param platform_config Config parameter dictionary
      * @param column_names Columns to read
      * @param batch_size Read batch size
      * @param result_order Read result order
-     * @return std::unique_ptr<SOMAArrayReader> SOMAArrayReader
+     * @return std::unique_ptr<SOMAArray> SOMAArray
      */
-    __attribute__((
-        visibility("default"))) static std::unique_ptr<SOMAArrayReader>
-    open(
+    static std::unique_ptr<SOMAArray> open(
+        tiledb_query_type_t mode,
         std::string_view uri,
         std::string_view name = "unnamed",
         std::map<std::string, std::string> platform_config = {},
         std::vector<std::string> column_names = {},
         std::string_view batch_size = "auto",
         std::string_view result_order = "auto",
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     /**
-     * @brief Open an array at the specified URI and return SOMAArrayReader
+     * @brief Open an array at the specified URI and return SOMAArray
      * object.
      *
+     * @param mode TILEDB_READ or TILEDB_WRITE
      * @param ctx TileDB context
      * @param uri URI of the array
      * @param name Name of the array
      * @param column_names Columns to read
      * @param batch_size Read batch size
      * @param result_order Read result order
-     * @return std::unique_ptr<SOMAArrayReader> SOMAArrayReader
+     * @return std::unique_ptr<SOMAArray> SOMAArray
      */
-    static std::unique_ptr<SOMAArrayReader> open(
+    static std::unique_ptr<SOMAArray> open(
+        tiledb_query_type_t mode,
         std::shared_ptr<Context> ctx,
         std::string_view uri,
         std::string_view name = "unnamed",
         std::vector<std::string> column_names = {},
         std::string_view batch_size = "auto",
         std::string_view result_order = "auto",
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     //===================================================================
     //= public non-static
     //===================================================================
     /**
-     * @brief Construct a new SOMAArrayReader object
+     * @brief Construct a new SOMAArray object
      *
+     * @param mode TILEDB_READ or TILEDB_WRITE
      * @param uri URI of the array
      * @param name name of the array
      * @param ctx TileDB context
+     * @param column_names Columns to read
+     * @param batch_size Batch size
+     * @param result_order Result order
+     * @param timestamp Timestamp
      */
-    SOMAArrayReader(
+    SOMAArray(
+        tiledb_query_type_t mode,
         std::string_view uri,
         std::string_view name,
         std::shared_ptr<Context> ctx,
         std::vector<std::string> column_names,
         std::string_view batch_size,
         std::string_view result_order,
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
-    SOMAArrayReader() = delete;
-    SOMAArrayReader(const SOMAArrayReader&) = delete;
-    SOMAArrayReader(SOMAArrayReader&&) = default;
-    ~SOMAArrayReader() = default;
+    SOMAArray() = delete;
+    SOMAArray(const SOMAArray&) = delete;
+    SOMAArray(SOMAArray&&) = default;
+    ~SOMAArray() = default;
+
+    /**
+     * Open the SOMAArray object.
+     */
+    void open(
+        tiledb_query_type_t mode,
+        std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
+
+    /**
+     * Closes the SOMAArray object.
+     */
+    void close();
 
     /**
-     * @brief Reset the state of this SOMAArrayReader object to prepare for a
+     * @brief Reset the state of this SOMAArray object to prepare for a
      * new query, while holding the array open.
      *
      * @param column_names
      * @param batch_size
      * @param result_order
      */
-    __attribute__((visibility("default"))) void reset(
+    void reset(
         std::vector<std::string> column_names = {},
         std::string_view batch_size = "auto",
         std::string_view result_order = "auto");
 
     /**
      * @brief Set the dimension slice using one point
      *
@@ -158,15 +182,15 @@
         const std::string& dim,
         const tcb::span<T> points,
         int partition_index,
         int partition_count) {
         // Validate partition inputs
         if (partition_index >= partition_count) {
             throw TileDBSOMAError(fmt::format(
-                "[SOMAArrayReader] partition_index ({}) must be < "
+                "[SOMAArray] partition_index ({}) must be < "
                 "partition_count "
                 "({})",
                 partition_index,
                 partition_count));
         }
 
         if (partition_count > 1) {
@@ -175,15 +199,15 @@
 
             // If this is the last partition, cover the rest of the points.
             if (partition_index == partition_count - 1) {
                 partition_size = points.size() - start;
             }
 
             LOG_DEBUG(fmt::format(
-                "[SOMAArrayReader] set_dim_points partitioning: sizeof(T)={} "
+                "[SOMAArray] set_dim_points partitioning: sizeof(T)={} "
                 "dim={} "
                 "index={} "
                 "count={} "
                 "range=[{}, {}] of {} points",
                 sizeof(T),
                 dim,
                 partition_index,
@@ -206,16 +230,16 @@
      *
      * @tparam T
      * @param dim
      * @param points
      */
     template <typename T>
     void set_dim_points(const std::string& dim, const std::vector<T>& points) {
-        LOG_DEBUG(fmt::format(
-            "[SOMAArrayReader] set_dim_points: sizeof(T)={}", sizeof(T)));
+        LOG_DEBUG(
+            fmt::format("[SOMAArray] set_dim_points: sizeof(T)={}", sizeof(T)));
         mq_->select_points(dim, points);
     }
 
     /**
      * @brief Set the dimension slice using multiple ranges
      *
      * @note Partitioning is not supported
@@ -253,33 +277,31 @@
         mq_->select_columns(names, if_not_empty);
     }
 
     /**
      * @brief Submit the query
      *
      */
-    __attribute__((visibility("default"))) void submit();
+    void submit();
 
     /**
      * @brief Read the next chunk of results from the query. If all results have
      * already been read, std::nullopt is returned.
      *
      * An example use model:
      *
-     *   auto reader = SOMAArrayReader::open(uri);
+     *   auto reader = SOMAArray::open(uri);
      *   reader->submit();
      *   while (auto batch = x_data->read_next()) {
      *       ...process batch ...
      *   }
      *
      * @return std::optional<std::shared_ptr<ArrayBuffers>>
      */
-    __attribute__((visibility("default")))
-    std::optional<std::shared_ptr<ArrayBuffers>>
-    read_next();
+    std::optional<std::shared_ptr<ArrayBuffers>> read_next();
 
     /**
      * @brief Check if the query is complete.
      *
      * If `query_status_only` is true, return true if the query status is
      * complete.
      *
@@ -316,15 +338,15 @@
     }
 
     /**
      * @brief Get the total number of unique cells in the array.
      *
      * @return uint64_t Total number of unique cells
      */
-    __attribute__((visibility("default"))) uint64_t nnz();
+    uint64_t nnz();
 
     /**
      * @brief Get the schema of the array.
      *
      * @return std::shared_ptr<ArraySchema> Schema
      */
     std::shared_ptr<ArraySchema> schema() {
@@ -333,45 +355,123 @@
 
     /**
      * @brief Get the capacity of each dimension.
      *
      * @return A vector with length equal to the number of dimensions; each
      * value in the vector is the capcity of each dimension.
      */
-    __attribute__((visibility("default"))) std::vector<int64_t> shape();
+    std::vector<int64_t> shape();
+
+    /**
+     * Set metadata key-value items to an open array. The array must
+     * opened in WRITE mode, otherwise the function will error out.
+     *
+     * @param key The key of the metadata item to be added. UTF-8 encodings
+     *     are acceptable.
+     * @param value_type The datatype of the value.
+     * @param value_num The value may consist of more than one items of the
+     *     same datatype. This argument indicates the number of items in the
+     *     value component of the metadata.
+     * @param value The metadata value in binary form.
+     *
+     * @note The writes will take effect only upon closing the array.
+     */
+    void set_metadata(
+        const std::string& key,
+        tiledb_datatype_t value_type,
+        uint32_t value_num,
+        const void* value);
+
+    /**
+     * Deletes a metadata key-value item from an open array. The array must
+     * be opened in WRITE mode, otherwise the function will error out.
+     *
+     * @param key The key of the metadata item to be deleted.
+     *
+     * @note The writes will take effect only upon closing the array.
+     *
+     * @note If the key does not exist, this will take no effect
+     *     (i.e., the function will not error out).
+     */
+    void delete_metadata(const std::string& key);
+
+    /**
+     * @brief Given a key, retrieve the associated value datatype, number of
+     * values, and value in binary form. The array must be opened in READ mode,
+     * otherwise the function will error out.
+     *
+     * The value may consist of more than one items of the same datatype. Keys
+     * that do not exist in the metadata will be return NULL for the value.
+     *
+     * @param key The key of the metadata item to be retrieved. UTF-8 encodings
+     *     are acceptable.
+     * @return MetadataValue (std::tuple<std::string, tiledb_datatype_t,
+     * uint32_t, const void*>)
+     */
+    MetadataValue get_metadata(const std::string& key) const;
+
+    /**
+     * @brief Given an index, retrieve the associated value datatype, number of
+     * values, and value in binary form. The array must be opened in READ mode,
+     * otherwise the function will error out.
+     *
+     * @param index The index used to get the metadata.
+     * @return MetadataValue (std::tuple<std::string, tiledb_datatype_t,
+     * uint32_t, const void*>)
+     */
+    MetadataValue get_metadata(uint64_t index) const;
+
+    /**
+     * Checks if key exists in metadata from an open array. The array must
+     * be opened in READ mode, otherwise the function will error out.
+     *
+     * @param key The key of the metadata item to be checked. UTF-8 encodings
+     *     are acceptable.
+     * @return true if the key exists, else false.
+     */
+    bool has_metadata(const std::string& key);
+
+    /**
+     * Returns then number of metadata items in an open array. The array must
+     * be opened in READ mode, otherwise the function will error out.
+     */
+    uint64_t metadata_num() const;
 
    private:
     //===================================================================
     //= private non-static
     //===================================================================
 
     // TileDB context
     std::shared_ptr<Context> ctx_;
 
-    // SOMAArrayReader URI
+    // SOMAArray URI
     std::string uri_;
 
     // Batch size
     std::string batch_size_;
 
     // Result order
     std::string result_order_;
 
     // Read timestamp range (start, end)
     std::optional<std::pair<uint64_t, uint64_t>> timestamp_;
 
     // Managed query for the array
     std::unique_ptr<ManagedQuery> mq_;
 
+    // Array associated with mq_
+    std::shared_ptr<Array> arr_;
+
     // True if this is the first call to read_next()
     bool first_read_next_ = true;
 
     // True if the query was submitted
     bool submitted_ = false;
 
     // Unoptimized method for computing nnz() (issue `count_cells` query)
     uint64_t nnz_slow();
 };
 
 }  // namespace tiledbsoma
 
-#endif  // SOMA_ARRAY_READER
+#endif  // SOMA_ARRAY
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/stats.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/stats.cc`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @file   stats.h
+ * @file   stats.cc
  *
  * @section LICENSE
  *
  * The MIT License
  *
  * @copyright Copyright (c) 2023 TileDB, Inc.
  *
@@ -23,27 +23,35 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- *   This declares the common functions in the API
+ * This file provides access to stats from libtiledbsoma's dependency on
+ * TileDB Embedded.
  */
 
-#ifndef TILEDBSOMA_STATS_H
-#define TILEDBSOMA_STATS_H
-
-#include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
-
-#include <string>
+#include "utils/stats.h"
+#include <tiledb/tiledb>
 
 namespace tiledbsoma::stats {
 
-__attribute__((visibility("default"))) void enable();
-__attribute__((visibility("default"))) void disable();
-__attribute__((visibility("default"))) void reset();
-__attribute__((visibility("default"))) std::string dump();
+void enable() {
+    tiledb::Stats::enable();
+}
+
+void disable() {
+    tiledb::Stats::disable();
+}
+
+void reset() {
+    tiledb::Stats::reset();
+}
+
+std::string dump() {
+    std::string stats;
+    tiledb::Stats::raw_dump(&stats);
+    return stats;
+}
 
 };  // namespace tiledbsoma::stats
-
-#endif  // TILEDBSOMA_STATS_H
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/tiledbsoma` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma`

 * *Files 20% similar despite different names*

```diff
@@ -29,18 +29,27 @@
  *
  * This is the main import header for the C++ API
  */
 
 #ifndef __TILEDBSOMA__
 #define __TILEDBSOMA__
 
-#include <tiledbsoma/array_buffers.h>
-#include <tiledbsoma/arrow_adapter.h>
-#include <tiledbsoma/column_buffer.h>
-#include <tiledbsoma/common.h>
+// TODO Uncomment after finishing Python and R bindings
+// #include "soma_collection.h"
+// #include "soma_dataframe.h"
+// #include "soma_dense_ndarray.h"
+// #include "soma_experiment.h"
+// #include "soma_measurement.h"
+// #include "soma_object.h"
+// #include "soma_sparse_ndarray.h"
+
+#include <utils/arrow_adapter.h>
 #include <tiledbsoma/logger_public.h>
-#include <tiledbsoma/managed_query.h>
-#include <tiledbsoma/soma_array_reader.h>
-#include <tiledbsoma/stats.h>
-#include <tiledbsoma/version.h>
+#include <utils/array_buffers.h>
+#include <utils/column_buffer.h>
+#include <utils/common.h>
+#include <utils/stats.h>
+#include <utils/version.h>
+#include <soma/managed_query.h>
+#include <soma/soma_array.h>
 
 #endif
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/util.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/util.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,17 @@
  *
  * This file defines the utility functions
  */
 
 #ifndef UTIL_H
 #define UTIL_H
 
-#include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
-
 #include <regex>
-#include <tiledbsoma/tiledbsoma>
+#include <span/span.hpp>
+#include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 namespace tiledbsoma::util {
 
 using VarlenBufferPair =
     std::pair<std::vector<std::byte>, std::vector<uint64_t>>;
 
 template <typename T>
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/version.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/version.h`

 * *Files 15% similar despite different names*

```diff
@@ -35,14 +35,13 @@
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <string>
 
 namespace tiledbsoma::version {
 
-__attribute__((visibility("default"))) std::string as_string();
-__attribute__((visibility("default"))) std::tuple<int, int, int>
-embedded_version_triple();
+std::string as_string();
+std::tuple<int, int, int> embedded_version_triple();
 
 };  // namespace tiledbsoma::version
 
 #endif  // TILEDBSOMA_VERSION_H
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/CMakeLists.txt` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 message(STATUS "Starting TileDB-SOMA build.")
 
 set(TILEDBSOMA_INSTALL_TARGETS "")
 
 # ###########################################################
 # Find required dependencies
 # See ../cmake/Modules/*.cmake for provenance/version info
-############################################################
-
+# ###########################################################
 find_package(TileDB_EP REQUIRED)
 find_package(Spdlog_EP REQUIRED)
 
 # ###########################################################
 # Get source commit hash
 # ###########################################################
 find_package(Git REQUIRED)
@@ -40,25 +39,25 @@
 
 message(STATUS "Building with commit hash ${BUILD_COMMIT_HASH}")
 
 # ###########################################################
 # Common object library
 # ###########################################################
 add_library(TILEDB_SOMA_OBJECTS OBJECT
-  ${CMAKE_CURRENT_SOURCE_DIR}/column_buffer.cc
-  ${CMAKE_CURRENT_SOURCE_DIR}/logger.cc
-  ${CMAKE_CURRENT_SOURCE_DIR}/managed_query.cc
-  ${CMAKE_CURRENT_SOURCE_DIR}/soma_array_reader.cc
-  ${CMAKE_CURRENT_SOURCE_DIR}/stats.cc
-  ${CMAKE_CURRENT_SOURCE_DIR}/util.cc
-  ${CMAKE_CURRENT_SOURCE_DIR}/version.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/managed_query.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_array.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/column_buffer.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/logger.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/stats.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/util.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/version.cc
 
   # TODO: uncomment when thread_pool is enabled
-  # ${CMAKE_CURRENT_SOURCE_DIR}/../external/src/thread_pool/thread_pool.cc
-  # ${CMAKE_CURRENT_SOURCE_DIR}/../external/src/thread_pool/status.cc
+  # ${CMAKE_CURRENT_SOURCE_DIR}/external/src/thread_pool/thread_pool.cc
+  # ${CMAKE_CURRENT_SOURCE_DIR}/external/src/thread_pool/status.cc
 )
 
 message(STATUS "Building TileDB without deprecation warnings")
 target_compile_definitions(TILEDB_SOMA_OBJECTS PRIVATE
   -DBUILD_COMMIT_HASH="${BUILD_COMMIT_HASH}"
   -DTILEDB_DEPRECATED=
 )
@@ -68,16 +67,15 @@
 )
 
 set_property(TARGET TILEDB_SOMA_OBJECTS PROPERTY POSITION_INDEPENDENT_CODE ON)
 
 target_include_directories(TILEDB_SOMA_OBJECTS
   PRIVATE
   ${CMAKE_CURRENT_SOURCE_DIR}
-  ${CMAKE_CURRENT_SOURCE_DIR}/../include
-  ${CMAKE_CURRENT_SOURCE_DIR}/../external/include
+  ${CMAKE_CURRENT_SOURCE_DIR}/external/include
   $<TARGET_PROPERTY:TileDB::tiledb_shared,INTERFACE_INCLUDE_DIRECTORIES>
   $<TARGET_PROPERTY:spdlog::spdlog,INTERFACE_INCLUDE_DIRECTORIES>
   ${pybind11_INCLUDE_DIRS}
 )
 
 # ###########################################################
 # Compile options/definitions
@@ -150,23 +148,60 @@
     target_link_libraries(tiledbsoma
       INTERFACE
       -fsanitize=${SANITIZER}
     )
   endif()
 endif()
 
-# Install header files and preserve directory structure
+# Install header files 
 # target_sources FILE_SET is preferred with cmake>=3.23
-install(DIRECTORY
-  ${CMAKE_CURRENT_SOURCE_DIR}/../external/include/span
-  ${CMAKE_CURRENT_SOURCE_DIR}/../external/include/thread_pool
-  ${CMAKE_CURRENT_SOURCE_DIR}/../include/tiledbsoma
-  TYPE INCLUDE
+# TODO Uncomment after finishing Python and R bindings
+# set(TILEDB_SOMA_PUBLIC_HEADERS
+#   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/tiledbsoma
+#   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_collection.h
+#   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_dataframe.h
+#   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_dense_ndarray.h
+#   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_experiment.h
+#   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_measurement.h
+#   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_object.h
+#   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_sparse_ndarray.h
+#   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/logger_public.h
+# )
+
+install(FILES 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/managed_query.h
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_array.h 
+  DESTINATION "include/soma"
+)
+
+install(FILES 
+  ${CMAKE_CURRENT_SOURCE_DIR}/tiledbsoma/logger_public.h
+  ${CMAKE_CURRENT_SOURCE_DIR}/tiledbsoma/tiledbsoma
+  DESTINATION "include/tiledbsoma"
+)
+
+install(FILES
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/array_buffers.h  
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/arrow_adapter.h  
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/carrow.h  
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/column_buffer.h  
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/common.h  
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/logger.h  
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/stats.h  
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/util.h  
+  ${CMAKE_CURRENT_SOURCE_DIR}/utils/version.h
+  DESTINATION "include/utils"
 )
 
+install(FILES 
+  ${CMAKE_CURRENT_SOURCE_DIR}/external/include/span/span.hpp
+  DESTINATION "include/span"
+)
+
+
 # ###########################################################
 # API symbol exports
 # ###########################################################
 include(GenerateExportHeader)
 
 # Generates the file 'tiledbsoma_export.h' suitable for the current compiler.
 generate_export_header(TILEDB_SOMA_OBJECTS
@@ -180,28 +215,33 @@
 set(TILEDB_SOMA_EXPORT_HEADER "${CMAKE_CURRENT_BINARY_DIR}/tiledbsoma_export.h")
 set(TILEDB_SOMA_EXPORT_HEADER "${TILEDB_SOMA_EXPORT_HEADER}" PARENT_SCOPE)
 
 # Set related compiler settings
 target_compile_definitions(TILEDB_SOMA_OBJECTS PRIVATE -DTILEDB_SOMA_OBJECTS_EXPORTS)
 target_include_directories(TILEDB_SOMA_OBJECTS PRIVATE ${CMAKE_CURRENT_BINARY_DIR})
 
+# Add the generated header to the public headers list
+list(APPEND TILEDB_SOMA_PUBLIC_HEADERS
+  "${TILEDB_SOMA_EXPORT_HEADER}"
+)
+
 # Add public headers, which are the ones that get installed.
 if(NOT TILEDBSOMA_BUILD_STATIC)
   set_target_properties(tiledbsoma
     PROPERTIES
-    PUBLIC_HEADER "${TILEDB_SOMA_EXPORT_HEADER}"
+    PUBLIC_HEADER "${TILEDB_SOMA_PUBLIC_HEADERS}"
   )
 endif()
 
 # ###########################################################
 # CLI executable target
 # ###########################################################
 if(TILEDBSOMA_BUILD_CLI)
   add_executable(tiledbsoma-cli
-    ${CMAKE_CURRENT_SOURCE_DIR}/cli.cc
+    ${CMAKE_CURRENT_SOURCE_DIR}/cli/cli.cc
     $<TARGET_OBJECTS:TILEDB_SOMA_OBJECTS>
   )
 
   list(APPEND TILEDBSOMA_INSTALL_TARGETS tiledbsoma-cli)
 
   set_target_properties(tiledbsoma-cli PROPERTIES OUTPUT_NAME tdbsoma)
 
@@ -225,16 +265,15 @@
   if(NOT APPLE AND NOT WIN32)
     target_link_libraries(tiledbsoma-cli PRIVATE pthread)
   endif()
 
   target_include_directories(tiledbsoma-cli
     PRIVATE
     ${CMAKE_CURRENT_SOURCE_DIR}
-    ${CMAKE_CURRENT_SOURCE_DIR}/../include
-    ${CMAKE_CURRENT_SOURCE_DIR}/../external/include
+    ${CMAKE_CURRENT_SOURCE_DIR}/external/include
     ${TILEDB_SOMA_EXPORT_HEADER_DIR}
     ${pybind11_INCLUDE_DIRS}
   )
 endif()
 
 # ###########################################################
 # Installation
@@ -252,35 +291,34 @@
 set(TARGETS_EXPORT_NAME "TileDBSomaTargets")
 
 # Path to generated cmake file
 set(PROJECT_CONFIG "${CMAKE_CURRENT_BINARY_DIR}/TileDBSomaConfig.cmake")
 
 # Generate 'TileDBConfig.cmake'
 # This process requires these variables to be defined at this point:
-#   * TARGETS_EXPORT_NAME
-#   * PROJECT_NAME
-#   * TILEDB_STATIC_DEP_STRING
+# * TARGETS_EXPORT_NAME
+# * PROJECT_NAME
+# * TILEDB_STATIC_DEP_STRING
 configure_package_config_file(
   "${TILEDBSOMA_CMAKE_INPUTS_DIR}/Config.cmake.in"
   "${PROJECT_CONFIG}"
   INSTALL_DESTINATION "${CONFIG_INSTALL_DIR}"
 )
 
 # Install config file to <prefix>/lib/cmake/tiledbsoma/TileDBSomaConfig.cmake
 install(
   FILES "${PROJECT_CONFIG}"
   DESTINATION "${CONFIG_INSTALL_DIR}"
 )
 
-
 # Set rpath so the TileDB-SOMA dynamic dependencies can be located.
-if (NOT WIN32 AND NOT TILEDBSOMA_BUILD_STATIC)
+if(NOT WIN32 AND NOT TILEDBSOMA_BUILD_STATIC)
   set_target_properties(tiledbsoma
     PROPERTIES
-      INSTALL_RPATH "${CMAKE_INSTALL_PREFIX}/${CMAKE_INSTALL_LIBDIR}"
+    INSTALL_RPATH "${CMAKE_INSTALL_PREFIX}/${CMAKE_INSTALL_LIBDIR}"
   )
 endif()
 
 if(TILEDBSOMA_BUILD_CLI)
   set_target_properties(tiledbsoma-cli PROPERTIES INSTALL_RPATH ${CMAKE_INSTALL_PREFIX}/${CMAKE_INSTALL_LIBDIR})
 endif()
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/cli.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/cli/cli.cc`

 * *Files 10% similar despite different names*

```diff
@@ -26,45 +26,46 @@
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
  * This file is currently a sandbox for C++ API experiments
  */
 
-#include <tiledbsoma/tiledbsoma>
+#include "soma/soma_array.h"
+#include "utils/arrow_adapter.h"
 
 using namespace tiledbsoma;
 
 // [[Rcpp::export]]
 void test_sdf(const std::string& uri) {
     std::map<std::string, std::string> config;
     // Control buffer sizes, similar to tiledb-py
     // config["soma.init_buffer_bytes"] = "4294967296";
 
     // Control core memory usage
     // config["sm.mem.total_budget"] = "1118388608";
 
     // Read all values from the obs array
-    auto obs = SOMAArrayReader::open(uri + "/obs", "obs");
+    auto obs = SOMAArray::open(TILEDB_READ, uri + "/obs", "obs");
     obs->submit();
     auto obs_data = obs->read_next();
 
     // Read all values from the var array
-    auto var = SOMAArrayReader::open(uri + "/ms/RNA/var", "var");
+    auto var = SOMAArray::open(TILEDB_READ, uri + "/ms/RNA/var", "var");
     var->submit();
     auto var_data = var->read_next();
 
     // Check if obs and var reads are complete
     if (obs->results_complete() && var->results_complete()) {
         LOG_INFO("var and obs queries are complete");
     }
 
     // Read all values from the X/data array
-    auto x_data = SOMAArrayReader::open(
-        uri + "/ms/RNA/X/data", "X/data", config);
+    auto x_data = SOMAArray::open(
+        TILEDB_READ, uri + "/ms/RNA/X/data", "X/data", config);
     x_data->submit();
 
     int batches = 0;
     int total_num_rows = 0;
 
     // Handle incomplete queries
     while (auto batch = x_data->read_next()) {
@@ -75,23 +76,21 @@
     LOG_INFO(fmt::format("X/data rows = {}", total_num_rows));
     LOG_INFO(fmt::format("  batches = {}", batches));
 }
 
 namespace tdbs = tiledbsoma;
 void test_arrow(const std::string& uri) {
     const std::vector<std::string>& colnames{"n_counts", "n_genes", "louvain"};
-    auto obs = tdbs::SOMAArrayReader::open(uri, "", {}, colnames);
+    auto obs = tdbs::SOMAArray::open(TILEDB_READ, uri, "", {}, colnames);
     obs->submit();
     // Getting next batch:  std::optional<std::shared_ptr<ArrayBuffers>>
     auto obs_data = obs->read_next();
     if (!obs->results_complete()) {
         tdbs::LOG_WARN(fmt::format("Read of '{}' incomplete", uri));
-#if !defined(R_BUILD)
         exit(-1);
-#endif
     }
     tdbs::LOG_INFO(fmt::format(
         "Read complete with {} obs and {} cols",
         obs_data->get()->num_rows(),
         obs_data->get()->names().size()));
     std::vector<std::string> names = obs_data->get()->names();
     for (auto nm : names) {
@@ -102,15 +101,14 @@
             "Accessing '{}', retrieved '{}', n_children {}",
             nm,
             schema->name,
             schema->n_children));
     }
 }
 
-#if !defined(R_BUILD)
 int main(int argc, char** argv) {
     LOG_CONFIG("debug");
 
     if (argc < 2) {
         printf("Run with CI test SOMA:\n\n");
         printf("  %s test/soco/pbmc3k_processed\n", argv[0]);
         return 0;
@@ -122,8 +120,7 @@
     } catch (const std::exception& e) {
         printf("%s\n", e.what());
         return 1;
     }
 
     return 0;
 };
-#endif
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/column_buffer.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/column_buffer.cc`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,18 @@
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
  * This file defines the a ColumBuffer class.
  */
 
-#include "tiledbsoma/column_buffer.h"
-#include "tiledbsoma/array_buffers.h"
-#include "tiledbsoma/common.h"
-#include "tiledbsoma/logger_public.h"
+#include "column_buffer.h"
+#include "array_buffers.h"
+#include "common.h"
+#include "logger.h"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 //===================================================================
 //= public static
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/logger.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/logger.cc`

 * *Files 1% similar despite different names*

```diff
@@ -57,21 +57,16 @@
 /* ********************************* */
 /*     CONSTRUCTORS & DESTRUCTORS    */
 /* ********************************* */
 
 Logger::Logger() {
     logger_ = spdlog::get(CONSOLE_LOGGER);
     if (logger_ == nullptr) {
-#if !defined(R_BUILD)
         logger_ = spdlog::stdout_color_mt(CONSOLE_LOGGER);
-#else
-        logger_ = spdlog::r_sink_mt(CONSOLE_LOGGER);
-        spdlog::set_default_logger(logger_);
-#endif
-#if !defined(R_BUILD) && !defined(_WIN32)
+#if !defined(_WIN32)
         // change color of critical messages
         auto console_sink = static_cast<spdlog::sinks::stdout_color_sink_mt*>(
             logger_->sinks().back().get());
         console_sink->set_color(
             spdlog::level::critical, console_sink->red_bold);
 #endif
     }
@@ -223,17 +218,15 @@
 void LOG_ERROR(const std::string& msg) {
     global_logger().error(msg.c_str());
 }
 
 /** Logs a critical error and exits with a non-zero status. */
 void LOG_FATAL(const std::string& msg) {
     global_logger().critical(msg.c_str());
-#if !defined(R_BUILD)
     exit(1);
-#endif
 }
 
 /** Convert TileDB timestamp (in ms) to human readable timestamp. */
 std::string asc_timestamp(uint64_t timestamp_ms) {
     auto time_sec = static_cast<time_t>(timestamp_ms) / 1000;
     std::string time_str = asctime(gmtime(&time_sec));
     time_str.pop_back();  // remove newline
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/logger.h` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/logger.h`

 * *Files 1% similar despite different names*

```diff
@@ -47,19 +47,15 @@
  * creating an additional external dependency.
  */
 
 #pragma once
 #ifndef TILEDB_LOGGER_H
 #define TILEDB_LOGGER_H
 
-#if !defined(R_BUILD)
 #include <spdlog/spdlog.h>
-#else
-#include "tiledbsoma/spdlog_with_R.h"
-#endif
 
 namespace tiledbsoma {
 
 /** Definition of class Logger. */
 class Logger {
    public:
     /* ********************************* */
@@ -244,10 +240,10 @@
 
 }  // namespace tiledbsoma
 
 /** Convert TileDB timestamp (in ms) to human readable timestamp. */
 std::string asc_timestamp(uint64_t timestamp_ms);
 
 // Also include the public logger functions here.
-#include "tiledbsoma/logger_public.h"
+#include "../tiledbsoma/logger_public.h"
 
 #endif  // TILEDB_LOGGER_H
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/managed_query.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/managed_query.cc`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
  * This file defines the performing TileDB queries.
  */
 
-#include "tiledbsoma/managed_query.h"
-#include "tiledbsoma/common.h"
+#include "soma/managed_query.h"
 #include "tiledbsoma/logger_public.h"
+#include "utils/common.h"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 //===================================================================
 //= public non-static
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/soma_array_reader.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/soma_array.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @file   soma_array_reader.cc
+ * @file   soma_array.cc
  *
  * @section LICENSE
  *
  * The MIT License
  *
  * @copyright Copyright (c) 2022 TileDB, Inc.
  *
@@ -23,114 +23,144 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- *   This file defines the SOMAArrayReader class.
+ *   This file defines the SOMAArray class.
  */
 
-#include "tiledbsoma/soma_array_reader.h"
-#include "tiledbsoma/logger_public.h"
-#include "tiledbsoma/util.h"
+#include "soma_array.h"
+#include "../tiledbsoma/logger_public.h"
+#include "../utils/util.h"
 
 namespace tiledbsoma {
 using namespace tiledb;
 
 //===================================================================
 //= public static
 //===================================================================
 
-std::unique_ptr<SOMAArrayReader> SOMAArrayReader::open(
+std::unique_ptr<SOMAArray> SOMAArray::open(
+    tiledb_query_type_t mode,
     std::string_view uri,
     std::string_view name,
     std::map<std::string, std::string> platform_config,
     std::vector<std::string> column_names,
     std::string_view batch_size,
     std::string_view result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
-    return std::make_unique<SOMAArrayReader>(
+    return std::make_unique<SOMAArray>(
+        mode,
         uri,
         name,
         std::make_shared<Context>(Config(platform_config)),
         column_names,
         batch_size,
         result_order,
         timestamp);
 }
 
-std::unique_ptr<SOMAArrayReader> SOMAArrayReader::open(
+std::unique_ptr<SOMAArray> SOMAArray::open(
+    tiledb_query_type_t mode,
     std::shared_ptr<Context> ctx,
     std::string_view uri,
     std::string_view name,
     std::vector<std::string> column_names,
     std::string_view batch_size,
     std::string_view result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
-    return std::make_unique<SOMAArrayReader>(
-        uri, name, ctx, column_names, batch_size, result_order, timestamp);
+    return std::make_unique<SOMAArray>(
+        mode,
+        uri,
+        name,
+        ctx,
+        column_names,
+        batch_size,
+        result_order,
+        timestamp);
 }
 
 //===================================================================
 //= public non-static
 //===================================================================
 
-SOMAArrayReader::SOMAArrayReader(
+SOMAArray::SOMAArray(
+    tiledb_query_type_t mode,
     std::string_view uri,
     std::string_view name,
     std::shared_ptr<Context> ctx,
     std::vector<std::string> column_names,
     std::string_view batch_size,
     std::string_view result_order,
     std::optional<std::pair<uint64_t, uint64_t>> timestamp)
     : ctx_(ctx)
     , uri_(util::rstrip_uri(uri))
     , timestamp_(timestamp) {
     // Validate parameters
     try {
-        LOG_DEBUG(fmt::format("[SOMAArrayReader] opening array '{}'", uri_));
-        auto array = std::make_shared<Array>(*ctx_, uri_, TILEDB_READ);
+        LOG_DEBUG(fmt::format("[SOMAArray] opening array '{}'", uri_));
+        arr_ = std::make_shared<Array>(*ctx_, uri_, mode);
         if (timestamp) {
             if (timestamp->first > timestamp->second) {
                 throw std::invalid_argument("timestamp start > end");
             }
-            array->set_open_timestamp_start(timestamp->first);
-            array->set_open_timestamp_end(timestamp->second);
-            array->reopen();
+            arr_->set_open_timestamp_start(timestamp->first);
+            arr_->set_open_timestamp_end(timestamp->second);
+            arr_->close();
+            arr_->open(mode);
         }
-        mq_ = std::make_unique<ManagedQuery>(array, name);
+        mq_ = std::make_unique<ManagedQuery>(arr_, name);
         LOG_DEBUG(
-            fmt::format("timestamp_start = {}", array->open_timestamp_start()));
+            fmt::format("timestamp_start = {}", arr_->open_timestamp_start()));
         LOG_DEBUG(
-            fmt::format("timestamp_end = {}", array->open_timestamp_end()));
+            fmt::format("timestamp_end = {}", arr_->open_timestamp_end()));
     } catch (const std::exception& e) {
         throw TileDBSOMAError(
             fmt::format("Error opening array: '{}'\n  {}", uri_, e.what()));
     }
 
     reset(column_names, batch_size, result_order);
 }
 
-void SOMAArrayReader::reset(
+void SOMAArray::open(
+    tiledb_query_type_t mode,
+    std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
+    arr_->open(mode);
+    if (timestamp) {
+        if (timestamp->first > timestamp->second) {
+            throw std::invalid_argument("timestamp start > end");
+        }
+        arr_->set_open_timestamp_start(timestamp->first);
+        arr_->set_open_timestamp_end(timestamp->second);
+        arr_->close();
+        arr_->open(mode);
+    }
+}
+
+void SOMAArray::close() {
+    arr_->close();
+}
+
+void SOMAArray::reset(
     std::vector<std::string> column_names,
     std::string_view batch_size,
     std::string_view result_order) {
     // Reset managed query
     mq_->reset();
 
     if (!column_names.empty()) {
         mq_->select_columns(column_names);
     }
 
     batch_size_ = batch_size;
 
     result_order_ = "auto";
-    if (result_order !=
-        "auto") {  // default "auto" is set in soma_array_reader.h
+    if (result_order != "auto") {  // default "auto" is set in soma_array.h
         tiledb_layout_t layout;
         if (result_order == "row-major") {
             layout = TILEDB_ROW_MAJOR;
         } else if (result_order == "column-major") {
             layout = TILEDB_COL_MAJOR;
         } else {
             throw TileDBSOMAError(
@@ -140,24 +170,24 @@
         result_order_ = result_order;
     }
 
     first_read_next_ = true;
     submitted_ = false;
 }
 
-void SOMAArrayReader::submit() {
+void SOMAArray::submit() {
     // Submit the query
     mq_->submit();
     submitted_ = true;
 }
 
-std::optional<std::shared_ptr<ArrayBuffers>> SOMAArrayReader::read_next() {
+std::optional<std::shared_ptr<ArrayBuffers>> SOMAArray::read_next() {
     if (!submitted_) {
         throw TileDBSOMAError(
-            "[SOMAArrayReader] submit must be called before read_next");
+            "[SOMAArray] submit must be called before read_next");
     }
 
     // Always return results from the first call to read_next()
     if (first_read_next_) {
         first_read_next_ = false;
         return mq_->results();
     }
@@ -170,27 +200,26 @@
     // Submit the query
     mq_->submit();
 
     // Return the results, possibly incomplete
     return mq_->results();
 }
 
-uint64_t SOMAArrayReader::nnz() {
+uint64_t SOMAArray::nnz() {
     // Verify array is sparse
     if (mq_->schema()->array_type() != TILEDB_SPARSE) {
         throw TileDBSOMAError(
-            "[SOMAArrayReader] nnz is only supported for sparse arrays");
+            "[SOMAArray] nnz is only supported for sparse arrays");
     }
 
     // Load fragment info
     FragmentInfo fragment_info(*ctx_, uri_);
     fragment_info.load();
 
-    LOG_DEBUG(
-        fmt::format("[SOMAArrayReader] Fragment info for array '{}'", uri_));
+    LOG_DEBUG(fmt::format("[SOMAArray] Fragment info for array '{}'", uri_));
     if (LOG_DEBUG_ENABLED()) {
         fragment_info.dump();
     }
 
     // Find the subset of fragments contained within the read timestamp range
     // [if any]
     std::vector<uint32_t> relevant_fragments;
@@ -243,29 +272,29 @@
         // TODO[perf]: Reading fragment info is not supported on TileDB Cloud
         // yet, but reading one fragment at a time will be slow. Is there
         // another way?
         total_cell_num += fragment_info.cell_num(relevant_fragments[i]);
         fragment_info.get_non_empty_domain(
             relevant_fragments[i], 0, &non_empty_domains[i]);
         LOG_DEBUG(fmt::format(
-            "[SOMAArrayReader] fragment {} non-empty domain = [{}, {}]",
+            "[SOMAArray] fragment {} non-empty domain = [{}, {}]",
             i,
             non_empty_domains[i][0],
             non_empty_domains[i][1]));
     }
 
     // Sort non-empty domains by the start of their ranges
     std::sort(non_empty_domains.begin(), non_empty_domains.end());
 
     // After sorting, if the end of a non-empty domain is >= the beginning of
     // the next non-empty domain, there is an overlap
     bool overlap = false;
     for (uint32_t i = 0; i < fragment_count - 1; i++) {
         LOG_DEBUG(fmt::format(
-            "[SOMAArrayReader] Checking {} < {}",
+            "[SOMAArray] Checking {} < {}",
             non_empty_domains[i][1],
             non_empty_domains[i + 1][0]));
         if (non_empty_domains[i][1] >= non_empty_domains[i + 1][0]) {
             overlap = true;
             break;
         }
     }
@@ -274,20 +303,21 @@
     if (!overlap) {
         return total_cell_num;
     }
     // Found relevant fragments with overlap, count cells
     return nnz_slow();
 }
 
-uint64_t SOMAArrayReader::nnz_slow() {
+uint64_t SOMAArray::nnz_slow() {
     LOG_DEBUG(
-        "[SOMAArrayReader] nnz() found consolidated or overlapping fragments, "
+        "[SOMAArray] nnz() found consolidated or overlapping fragments, "
         "counting cells...");
 
-    auto sr = SOMAArrayReader::open(
+    auto sr = SOMAArray::open(
+        TILEDB_READ,
         ctx_,
         uri_,
         "count_cells",
         {mq_->schema()->domain().dimension(0).name()},
         batch_size_,
         result_order_,
         timestamp_);
@@ -297,15 +327,15 @@
     while (auto batch = sr->read_next()) {
         total_cell_num += (*batch)->num_rows();
     }
 
     return total_cell_num;
 }
 
-std::vector<int64_t> SOMAArrayReader::shape() {
+std::vector<int64_t> SOMAArray::shape() {
     std::vector<int64_t> result;
     auto dimensions = this->schema().get()->domain().dimensions();
 
     for (const auto& dim : dimensions) {
         switch (dim.type()) {
             case TILEDB_UINT8:
                 result.push_back(
@@ -372,8 +402,47 @@
             default:
                 throw TileDBSOMAError("Dimension must be integer type.");
         }
     }
 
     return result;
 }
+
+void SOMAArray::set_metadata(
+    const std::string& key,
+    tiledb_datatype_t value_type,
+    uint32_t value_num,
+    const void* value) {
+    arr_->put_metadata(key, value_type, value_num, value);
+}
+
+void SOMAArray::delete_metadata(const std::string& key) {
+    arr_->delete_metadata(key);
+}
+
+MetadataValue SOMAArray::get_metadata(const std::string& key) const {
+    tiledb_datatype_t value_type;
+    uint32_t value_num;
+    const void* value;
+    arr_->get_metadata(key, &value_type, &value_num, &value);
+    return MetadataValue(key, value_type, value_num, value);
+}
+
+MetadataValue SOMAArray::get_metadata(uint64_t index) const {
+    std::string key;
+    tiledb_datatype_t value_type;
+    uint32_t value_num;
+    const void* value;
+    arr_->get_metadata_from_index(index, &key, &value_type, &value_num, &value);
+    return MetadataValue(key, value_type, value_num, value);
+}
+
+bool SOMAArray::has_metadata(const std::string& key) {
+    tiledb_datatype_t value_type;
+    return arr_->has_metadata(key, &value_type);
+}
+
+uint64_t SOMAArray::metadata_num() const {
+    return arr_->metadata_num();
+}
+
 }  // namespace tiledbsoma
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/stats.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/util.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
- * @file   stats.cc
+ * @file   util.cc
  *
  * @section LICENSE
  *
  * The MIT License
  *
- * @copyright Copyright (c) 2023 TileDB, Inc.
+ * @copyright Copyright (c) 2022 TileDB, Inc.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
@@ -23,35 +23,55 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- * This file provides access to stats from libtiledbsoma's dependency on
- * TileDB Embedded.
+ * This file defines utilities.
  */
 
-#include "tiledbsoma/stats.h"
-#include <tiledb/tiledb>
+#include "utils/util.h"
+#include <cstring>
 
-namespace tiledbsoma::stats {
+namespace tiledbsoma::util {
 
-void enable() {
-    tiledb::Stats::enable();
-}
+template <typename T>
+VarlenBufferPair to_varlen_buffers(std::vector<T> data, bool arrow) {
+    size_t nbytes = 0;
+    for (auto& elem : data) {
+        nbytes += elem.size();
+    }
+
+    std::vector<std::byte> result(nbytes);
+    std::vector<uint64_t> offsets(data.size() + 1);
+    size_t offset = 0;
+    size_t idx = 0;
+
+    for (auto& elem : data) {
+        std::memcpy(result.data() + offset, elem.data(), elem.size());
+        offsets[idx++] = offset;
+
+        offset += elem.size();
+    }
+    offsets[idx] = offset;
+
+    // Remove extra arrow offset when creating buffers for TileDB write
+    if (!arrow) {
+        offsets.pop_back();
+    }
 
-void disable() {
-    tiledb::Stats::disable();
+    return {result, offsets};
 }
 
-void reset() {
-    tiledb::Stats::reset();
+template VarlenBufferPair to_varlen_buffers(
+    std::vector<std::string>, bool arrow);
+
+bool is_tiledb_uri(std::string_view uri) {
+    return uri.find("tiledb://") == 0;
 }
 
-std::string dump() {
-    std::string stats;
-    tiledb::Stats::raw_dump(&stats);
-    return stats;
+std::string rstrip_uri(std::string_view uri) {
+    return std::regex_replace(std::string(uri), std::regex("/+$"), "");
 }
 
-};  // namespace tiledbsoma::stats
+};  // namespace tiledbsoma::util
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/version.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/version.cc`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,17 @@
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
  * This exposes the version of the TileDB Embedded library in use.
  */
 
-#include "tiledbsoma/version.h"
+#include "version.h"
 #include <tiledb/tiledb>
-#include "tiledbsoma/logger_public.h"
-
+#include "logger.h"
 namespace tiledbsoma::version {
 
 std::string as_string() {
     int major, minor, patch;
     tiledb_version(&major, &minor, &patch);
     return fmt::format("libtiledb={}.{}.{}", major, minor, patch);
 }
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/CMakeLists.txt` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,29 @@
 
 find_package(Catch_EP REQUIRED)
 
 add_executable(unit_soma EXCLUDE_FROM_ALL
     $<TARGET_OBJECTS:TILEDB_SOMA_OBJECTS>
     unit_column_buffer.cc
     unit_managed_query.cc
-    unit_soma_array_reader.cc
+    unit_soma_array.cc
 # TODO: uncomment when thread_pool is enabled
 #    unit_thread_pool.cc
 )
 
 target_link_libraries(unit_soma
   PRIVATE
     Catch2::Catch2WithMain
     TileDB::tiledb_shared
 )
 
 target_include_directories(unit_soma
   PRIVATE
     ${CMAKE_CURRENT_SOURCE_DIR}/../src
-    ${CMAKE_CURRENT_SOURCE_DIR}/../include
-    ${CMAKE_CURRENT_SOURCE_DIR}/../external/include
+    ${CMAKE_CURRENT_SOURCE_DIR}/../src/external/include
     ${pybind11_INCLUDE_DIRS}
     $<TARGET_PROPERTY:spdlog::spdlog,INTERFACE_INCLUDE_DIRECTORIES>
 )
 
 target_compile_definitions(unit_soma PRIVATE CATCH_CONFIG_MAIN)
 
 # Allow deprecated function for writing to an array with a timestamp
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_query_condition.py` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_query_condition.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 SOMA_URI = f"{TEST_DIR}/../../test/soco/pbmc3k_processed"
 
 if VERBOSE:
     clib.config_logging("debug")
 
 
 def pandas_query(uri, condition):
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
     sr.submit()
     arrow_table = sr.read_next()
     assert sr.results_complete()
 
     return arrow_table.to_pandas().query(condition)
 
 
 def soma_query(uri, condition):
     qc = QueryCondition(condition)
     schema = tiledb.open(uri).schema
 
-    sr = clib.SOMAArrayReader(uri, query_condition=qc, schema=schema)
+    sr = clib.SOMAArray(uri, query_condition=qc, schema=schema)
     sr.submit()
     arrow_table = sr.read_next()
     assert sr.results_complete()
 
     return arrow_table
 
 
@@ -108,15 +108,15 @@
 def test_query_condition_select_columns():
     uri = os.path.join(SOMA_URI, "obs")
     condition = "percent_mito > 0.02"
 
     qc = QueryCondition(condition)
     schema = tiledb.open(uri).schema
 
-    sr = clib.SOMAArrayReader(
+    sr = clib.SOMAArray(
         uri, query_condition=qc, schema=schema, column_names=["n_genes"]
     )
     sr.submit()
     arrow_table = sr.read_next()
 
     assert sr.results_complete()
     assert arrow_table.num_rows == 1332
@@ -126,15 +126,15 @@
 def test_query_condition_all_columns():
     uri = os.path.join(SOMA_URI, "obs")
     condition = "percent_mito > 0.02"
 
     qc = QueryCondition(condition)
     schema = tiledb.open(uri).schema
 
-    sr = clib.SOMAArrayReader(uri, query_condition=qc, schema=schema)
+    sr = clib.SOMAArray(uri, query_condition=qc, schema=schema)
     sr.submit()
     arrow_table = sr.read_next()
 
     assert sr.results_complete()
     assert arrow_table.num_rows == 1332
     assert arrow_table.num_columns == 7
 
@@ -142,15 +142,15 @@
 def test_query_condition_reset():
     uri = os.path.join(SOMA_URI, "obs")
     condition = "percent_mito > 0.02"
 
     qc = QueryCondition(condition)
     schema = tiledb.open(uri).schema
 
-    sr = clib.SOMAArrayReader(uri, query_condition=qc, schema=schema)
+    sr = clib.SOMAArray(uri, query_condition=qc, schema=schema)
     sr.submit()
     arrow_table = sr.read_next()
 
     assert sr.results_complete()
     assert arrow_table.num_rows == 1332
     assert arrow_table.num_columns == 7
 
@@ -224,14 +224,14 @@
     schema = tiledb.open(uri).schema
 
     # TODO: these raise the wrong error - it should be SOMAError. Change the test
     # when https://github.com/single-cell-data/TileDB-SOMA/issues/783 is fixed
     #
     with pytest.raises(RuntimeError):
         qc = QueryCondition(malformed_condition)
-        sr = clib.SOMAArrayReader(uri, query_condition=qc, schema=schema)
+        sr = clib.SOMAArray(uri, query_condition=qc, schema=schema)
         sr.submit()
         sr.read_next()
 
 
 if __name__ == "__main__":
     test_query_condition_select_columns()
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_simple.py` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_soma_array_reader.py` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_soma_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,48 +11,48 @@
 TEST_DIR = os.path.dirname(__file__)
 SOMA_URI = f"{TEST_DIR}/../../test/soco/pbmc3k_processed"
 
 if VERBOSE:
     clib.config_logging("debug")
 
 
-def test_soma_array_reader_obs():
+def test_soma_array_obs():
     """Read all values from obs array into an arrow table."""
 
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
     sr.submit()
     arrow_table = sr.read_next()
 
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_rows == 2638
 
 
-def test_soma_array_reader_var():
+def test_soma_array_var():
     """Read all values from var array into an arrow table."""
 
     name = "var"
     uri = os.path.join(SOMA_URI, "ms/RNA", name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
     sr.submit()
     arrow_table = sr.read_next()
 
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_rows == 1838
 
 
-def test_soma_array_reader_var_x_data():
+def test_soma_array_var_x_data():
     """Read all values from x/data array into an arrow table."""
 
     name = "X/data"
     uri = os.path.join(SOMA_URI, "ms/RNA", name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
     sr.submit()
 
     # iterate read batches until all results have been processed
     total_num_rows = 0
     # The := "walrus" operator is really the appropriate thing here, but alas, is not
     # supported in Python 3.7 which we do wish to preserve compatibility with.
     # while arrow_table := sr.read_next():
@@ -63,77 +63,77 @@
         total_num_rows += arrow_table.num_rows
 
     # test that all results are not present in the arrow table (incomplete queries)
     assert not sr.results_complete()
     assert total_num_rows == 4848644
 
 
-def test_soma_array_reader_dim_points():
+def test_soma_array_dim_points():
     """Read scalar dimension slice from obs array into an arrow table."""
 
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
 
     obs_id_points = list(range(0, 100, 2))
 
     sr.set_dim_points_int64("soma_joinid", obs_id_points)
 
     sr.submit()
     arrow_table = sr.read_next()
 
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_rows == len(obs_id_points)
 
 
-def test_soma_array_reader_empty_dim_points():
+def test_soma_array_empty_dim_points():
     """Read scalar dimension slice from obs array into an arrow table."""
 
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
 
     obs_id_points = []
 
     sr.set_dim_points_int64("soma_joinid", obs_id_points)
 
     sr.submit()
     arrow_table = sr.read_next()
 
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_rows == len(obs_id_points)
 
 
-def test_soma_array_reader_dim_points_arrow_array():
+def test_soma_array_dim_points_arrow_array():
     """Read scalar dimension slice from obs array into an arrow table."""
 
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
 
     obs_id_points = pa.array([0, 2, 4, 6, 8])
 
     sr.set_dim_points_arrow("soma_joinid", obs_id_points)
 
     sr.submit()
     arrow_table = sr.read_next()
 
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_rows == len(obs_id_points)
 
 
-def test_soma_array_reader_dim_ranges():
+def test_soma_array_dim_ranges():
     """Read range dimension slice from obs array into an arrow table."""
 
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
 
     obs_id_ranges = [
         [1000, 1004],
         [2000, 2004],
     ]
 
     sr.set_dim_ranges_int64("soma_joinid", obs_id_ranges)
@@ -142,20 +142,20 @@
     arrow_table = sr.read_next()
 
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_rows == 10
 
 
-def test_soma_array_reader_dim_mixed():
+def test_soma_array_dim_mixed():
     """Read scalar and range dimension slice from obs array into an arrow table."""
 
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
 
     obs_id_points = list(range(0, 100, 2))
 
     obs_id_ranges = [
         [1000, 1004],
         [2000, 2004],
     ]
@@ -167,22 +167,22 @@
     arrow_table = sr.read_next()
 
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_rows == 60
 
 
-def test_soma_array_reader_obs_slice_x():
+def test_soma_array_obs_slice_x():
     """Read X/data sliced by obs."""
 
     # read obs
     # ---------------------------------------------------------------1
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
 
     obs_id_points = list(range(0, 100, 2))
 
     obs_id_ranges = [
         [1000, 1004],
         [2000, 2004],
     ]
@@ -197,15 +197,15 @@
     assert sr.results_complete()
     assert obs.num_rows == 60
 
     # read X/data
     # ---------------------------------------------------------------1
     name = "X/data"
     uri = os.path.join(SOMA_URI, "ms/RNA", name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
 
     # slice X/data read with obs.soma_joinid column
     sr.set_dim_points_arrow("soma_dim_0", obs.column("soma_joinid"))
     sr.submit()
 
     # iterate read batches until all results have been processed
     total_num_rows = 0
@@ -217,45 +217,45 @@
         if not x_data:
             break
         total_num_rows += x_data.num_rows
 
     assert total_num_rows == 110280
 
 
-def test_soma_array_reader_column_names():
+def test_soma_array_column_names():
     """Read specified column names of obs array into an arrow table."""
 
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri, column_names=["soma_joinid", "louvain"])
+    sr = clib.SOMAArray(uri, column_names=["soma_joinid", "louvain"])
 
     sr.submit()
     arrow_table = sr.read_next()
 
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_columns == 2
 
 
 def test_nnz():
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri)
+    sr = clib.SOMAArray(uri)
 
     total_cell_count = sr.nnz()
 
     assert total_cell_count == 2638
 
 
-def test_soma_array_reader_reset():
-    """Submit a query with a SOMAArrayReader object, reset the SOMAArrayReader, and submit another query."""
+def test_soma_array_reset():
+    """Submit a query with a SOMAArray object, reset the SOMAArray, and submit another query."""
 
     name = "obs"
     uri = os.path.join(SOMA_URI, name)
-    sr = clib.SOMAArrayReader(uri, column_names=["soma_joinid", "louvain"])
+    sr = clib.SOMAArray(uri, column_names=["soma_joinid", "louvain"])
 
     sr.submit()
     arrow_table = sr.read_next()
 
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_columns == 2
@@ -273,8 +273,8 @@
     # test that all results are present in the arrow table (no incomplete queries)
     assert sr.results_complete()
     assert arrow_table.num_columns == 7
     assert arrow_table.num_rows == 5
 
 
 if __name__ == "__main__":
-    test_soma_array_reader_obs_slice_x()
+    test_soma_array_obs_slice_x()
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_column_buffer.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_managed_query.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_managed_query.cc`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 #include <catch2/matchers/catch_matchers_floating_point.hpp>
 #include <catch2/matchers/catch_matchers_predicate.hpp>
 #include <catch2/matchers/catch_matchers_string.hpp>
 #include <catch2/matchers/catch_matchers_templated.hpp>
 #include <catch2/matchers/catch_matchers_vector.hpp>
 #include <random>
 
-#include <tiledbsoma/util.h>
 #include <tiledb/tiledb>
 #include <tiledbsoma/tiledbsoma>
+#include "utils/util.h"
 
 using namespace tiledb;
 using namespace tiledbsoma;
 using namespace Catch::Matchers;
 
 #ifndef TILEDBSOMA_SOURCE_ROOT
 #define TILEDBSOMA_SOURCE_ROOT "not_defined"
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_soma_array_reader.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_soma_array.cc`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @file   unit_soma_array_reader.cc
+ * @file   unit_soma_array.cc
  *
  * @section LICENSE
  *
  * The MIT License
  *
  * @copyright Copyright (c) 2022 TileDB, Inc.
  *
@@ -23,32 +23,32 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- * This file manages unit tests for the SOMAArrayReader class
+ * This file manages unit tests for the SOMAArray class
  */
 
 #include <catch2/catch_template_test_macros.hpp>
 #include <catch2/catch_test_macros.hpp>
 #include <catch2/generators/catch_generators_all.hpp>
 #include <catch2/matchers/catch_matchers_exception.hpp>
 #include <catch2/matchers/catch_matchers_floating_point.hpp>
 #include <catch2/matchers/catch_matchers_predicate.hpp>
 #include <catch2/matchers/catch_matchers_string.hpp>
 #include <catch2/matchers/catch_matchers_templated.hpp>
 #include <catch2/matchers/catch_matchers_vector.hpp>
 #include <numeric>
 #include <random>
 
-#include <tiledbsoma/util.h>
 #include <tiledb/tiledb>
 #include <tiledbsoma/tiledbsoma>
+#include "utils/util.h"
 
 using namespace tiledb;
 using namespace tiledbsoma;
 using namespace Catch::Matchers;
 
 #ifndef TILEDBSOMA_SOURCE_ROOT
 #define TILEDBSOMA_SOURCE_ROOT "not_defined"
@@ -145,15 +145,15 @@
     }
 
     return {uri, nnz};
 }
 
 };  // namespace
 
-TEST_CASE("SOMAArrayReader: nnz") {
+TEST_CASE("SOMAArray: nnz") {
     auto num_fragments = GENERATE(1, 10);
     auto overlap = GENERATE(false, true);
     auto allow_duplicates = GENERATE(false, true);
     int num_cells_per_fragment = 128;
 
     SECTION(fmt::format(
         " - fragments={}, overlap={}, allow_duplicates={}",
@@ -170,26 +170,26 @@
             num_cells_per_fragment,
             num_fragments,
             overlap,
             allow_duplicates,
             10);
 
         // Get total cell num
-        auto sr = SOMAArrayReader::open(ctx, uri);
+        auto sr = SOMAArray::open(TILEDB_READ, ctx, uri);
 
         uint64_t nnz = sr->nnz();
         REQUIRE(nnz == expected_nnz);
 
         std::vector<int64_t> shape = sr->shape();
         REQUIRE(shape.size() == 1);
         REQUIRE(shape[0] == std::numeric_limits<int64_t>::max());
     }
 }
 
-TEST_CASE("SOMAArrayReader: nnz with timestamp") {
+TEST_CASE("SOMAArray: nnz with timestamp") {
     auto num_fragments = GENERATE(1, 10);
     auto overlap = GENERATE(false, true);
     auto allow_duplicates = GENERATE(false, true);
     int num_cells_per_fragment = 128;
 
     SECTION(fmt::format(
         " - fragments={}, overlap={}, allow_duplicates={}",
@@ -219,23 +219,23 @@
             overlap,
             allow_duplicates,
             20,
             true);
 
         // Get total cell num at timestamp (0, 15)
         std::pair<uint64_t, uint64_t> timestamp{0, 15};
-        auto sr = SOMAArrayReader::open(
-            ctx, uri, "nnz", {}, "auto", "auto", timestamp);
+        auto sr = SOMAArray::open(
+            TILEDB_READ, ctx, uri, "nnz", {}, "auto", "auto", timestamp);
 
         uint64_t nnz = sr->nnz();
         REQUIRE(nnz == expected_nnz);
     }
 }
 
-TEST_CASE("SOMAArrayReader: nnz with consolidation") {
+TEST_CASE("SOMAArray: nnz with consolidation") {
     auto num_fragments = GENERATE(1, 10);
     auto overlap = GENERATE(false, true);
     auto allow_duplicates = GENERATE(false, true);
     auto vacuum = GENERATE(false, true);
     int num_cells_per_fragment = 128;
 
     SECTION(fmt::format(
@@ -273,18 +273,65 @@
         // Consolidate and optionally vacuum
         Array::consolidate(*ctx, uri);
         if (vacuum) {
             Array::vacuum(*ctx, uri);
         }
 
         // Get total cell num
-        auto sr = SOMAArrayReader::open(ctx, uri, "nnz", {}, "auto", "auto");
+        auto sr = SOMAArray::open(
+            TILEDB_READ, ctx, uri, "nnz", {}, "auto", "auto");
 
         uint64_t nnz = sr->nnz();
         if (allow_duplicates) {
             // Since we wrote twice
             REQUIRE(nnz == 2 * expected_nnz);
         } else {
             REQUIRE(nnz == expected_nnz);
         }
     }
 }
+
+TEST_CASE("SOMAArray: metadata") {
+    auto ctx = std::make_shared<Context>();
+
+    std::string base_uri = "mem://unit-test-array";
+    const auto& [uri, expected_nnz] = create_array(base_uri, *ctx);
+
+    auto sr = SOMAArray::open(
+        TILEDB_WRITE,
+        ctx,
+        uri,
+        "metadata_test",
+        {},
+        "auto",
+        "auto",
+        std::pair<uint64_t, uint64_t>(1, 1));
+    int32_t val = 100;
+    sr->set_metadata("md", TILEDB_INT32, 1, &val);
+    sr->close();
+
+    sr->open(TILEDB_READ, std::pair<uint64_t, uint64_t>(1, 1));
+    REQUIRE(sr->has_metadata("md") == true);
+    REQUIRE(sr->metadata_num() == 1);
+
+    auto mdval = sr->get_metadata(0);
+    REQUIRE(std::get<MetadataInfo::key>(mdval) == "md");
+    REQUIRE(std::get<MetadataInfo::dtype>(mdval) == TILEDB_INT32);
+    REQUIRE(std::get<MetadataInfo::num>(mdval) == 1);
+    REQUIRE(*((const int32_t*)std::get<MetadataInfo::value>(mdval)) == 100);
+
+    mdval = sr->get_metadata("md");
+    REQUIRE(std::get<MetadataInfo::key>(mdval) == "md");
+    REQUIRE(std::get<MetadataInfo::dtype>(mdval) == TILEDB_INT32);
+    REQUIRE(std::get<MetadataInfo::num>(mdval) == 1);
+    REQUIRE(*((const int32_t*)std::get<MetadataInfo::value>(mdval)) == 100);
+    sr->close();
+
+    sr->open(TILEDB_WRITE, std::pair<uint64_t, uint64_t>(2, 2));
+    sr->delete_metadata("md");
+    sr->close();
+
+    sr->open(TILEDB_READ, std::pair<uint64_t, uint64_t>(3, 3));
+    REQUIRE(sr->has_metadata("md") == false);
+    REQUIRE(sr->metadata_num() == 0);
+    sr->close();
+}
```

### Comparing `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_thread_pool.cc` & `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/scripts/bld` & `tiledbsoma-1.2.3/dist_links/scripts/bld`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/scripts/run-clang-format.sh` & `tiledbsoma-1.2.3/dist_links/scripts/run-clang-format.sh`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/scripts/show-versions.py` & `tiledbsoma-1.2.3/dist_links/scripts/show-versions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/dist_links/scripts/update-tiledb-version.py` & `tiledbsoma-1.2.3/dist_links/scripts/update-tiledb-version.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/setup.py` & `tiledbsoma-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,16 +284,16 @@
         "numba==0.56.4; python_version<'3.11'",
         "numba==0.57.0rc1; python_version=='3.11'",
         "numpy>=1.18,<1.24",
         "pandas",
         "pyarrow>=9.0.0",
         "scanpy>=1.9.2",
         "scipy",
-        "somacore==1.0.1",
-        "tiledb==0.21.*",
+        "somacore==1.0.2",
+        "tiledb~=0.21.3",
         "typing-extensions",  # Note "-" even though `import typing_extensions`
     ],
     extras_require={
         "dev": [
             "black",
             "ruff",
             "pytest",
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/__init__.py` & `tiledbsoma-1.2.3/src/tiledbsoma/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_arrow_types.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_arrow_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_collection.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from ._dense_nd_array import DenseNDArray
 from ._exception import SOMAError, is_does_not_exist_error
 from ._sparse_nd_array import SparseNDArray
 from ._tiledb_object import AnyTileDBObject, TileDBObject
 from ._types import OpenTimestamp
 from ._util import is_relative_uri, make_relative_path, uri_joinpath
 from .options import SOMATileDBContext
+from .options._soma_tiledb_context import _validate_soma_tiledb_context
 
 # A collection can hold any sub-type of TileDBObject
 CollectionElementType = TypeVar("CollectionElementType", bound=AnyTileDBObject)
 _TDBO = TypeVar("_TDBO", bound=AnyTileDBObject)
 _Coll = TypeVar("_Coll", bound="CollectionBase[AnyTileDBObject]")
 _NDArr = TypeVar("_NDArr", bound=NDArray)
 
@@ -103,15 +104,15 @@
         Raises:
             TileDBError:
                 If unable to create the underlying object.
 
         Lifecycle:
             Experimental.
         """
-        context = context or SOMATileDBContext()
+        context = _validate_soma_tiledb_context(context)
         tiledb.group_create(uri=uri, ctx=context.tiledb_ctx)
         handle = cls._wrapper_type.open(uri, "w", context, tiledb_timestamp)
         cls._set_create_metadata(handle)
         return cls(
             handle,
             _dont_call_this_use_create_or_open_instead="tiledbsoma-internal-code",
         )
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_common_nd_array.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_common_nd_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 import tiledb
 from somacore import options
 from typing_extensions import Self
 
 from . import _arrow_types, _util
 from ._tiledb_array import TileDBArray
 from ._types import OpenTimestamp
-from .options._soma_tiledb_context import SOMATileDBContext
+from .options._soma_tiledb_context import (
+    SOMATileDBContext,
+    _validate_soma_tiledb_context,
+)
 from .options._tiledb_create_options import TileDBCreateOptions
 
 
 class NDArray(TileDBArray, somacore.NDArray):
     """Abstract base for the common behaviors of both kinds of NDArray."""
 
     __slots__ = ()
@@ -80,15 +83,15 @@
         # Implementor note: we carefully say "maximum possible int64 size" rather than 2**63-1. The
         # reason that the latter, while temptingly simple, is actually untrue is that tiledb core
         # requires that the capacity, when rounded up to an exact multiple of the extent, needs to
         # be representable as a signed 64-bit integer.  So in particular when a unit test (or anyone
         # else) sets extent to a not-power-of-two number like 999 or 1000 then the create fails if
         # the upper limit is exactly 2**63-1.
 
-        context = context or SOMATileDBContext()
+        context = _validate_soma_tiledb_context(context)
         schema = cls._build_tiledb_schema(
             type,
             shape,
             TileDBCreateOptions.from_platform_config(platform_config),
             context,
             is_sparse=cls.is_sparse,
         )
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_dataframe.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from . import pytiledbsoma as clib
 from ._constants import SOMA_JOINID
 from ._query_condition import QueryCondition
 from ._read_iters import TableReadIter
 from ._tiledb_array import TileDBArray
 from ._types import NPFloating, NPInteger, OpenTimestamp, Slice, is_slice_of
 from .options import SOMATileDBContext
+from .options._soma_tiledb_context import _validate_soma_tiledb_context
 from .options._tiledb_create_options import TileDBCreateOptions
 
 _UNBATCHED = options.BatchSize()
 
 
 class DataFrame(TileDBArray, somacore.DataFrame):
     """:class:`DataFrame` is a multi-column table with a user-defined schema. The
@@ -195,15 +196,15 @@
                soma_joinid col1
             0            0    a
             1            1    b
 
         Lifecycle:
             Experimental.
         """
-        context = context or SOMATileDBContext()
+        context = _validate_soma_tiledb_context(context)
         schema = _canonicalize_schema(schema, index_column_names)
         tdb_schema = _build_tiledb_schema(
             schema,
             index_column_names,
             domain,
             TileDBCreateOptions.from_platform_config(platform_config),
             context,
@@ -400,15 +401,15 @@
         dim_cols_list = [dim_cols_map[name] for name in self.index_column_names]
         dim_cols_tuple = tuple(dim_cols_list)
         self._handle.writer[dim_cols_tuple] = attr_cols_map
 
         return self
 
     def _set_reader_coord(
-        self, sr: clib.SOMAArrayReader, dim_idx: int, dim: tiledb.Dim, coord: object
+        self, sr: clib.SOMAArray, dim_idx: int, dim: tiledb.Dim, coord: object
     ) -> bool:
 
         if coord is None:
             return True  # No constraint; select all in this dimension
 
         if isinstance(coord, (str, bytes)):
             sr.set_dim_points_string_or_bytes(dim.name, [coord])
@@ -472,15 +473,15 @@
         if super()._set_reader_coord(sr, dim_idx, dim, coord):
             return True
 
         return False
 
     def _set_reader_coord_by_py_seq_or_np_array(
         self,
-        sr: clib.SOMAArrayReader,
+        sr: clib.SOMAArray,
         dim_idx: int,
         dim: tiledb.Dim,
         coord: object,
     ) -> bool:
         if isinstance(coord, np.ndarray):
             if coord.ndim != 1:
                 raise ValueError(
@@ -538,15 +539,15 @@
             raise ValueError(
                 f"unhandled type {dim.dtype} for index column named {dim.name}"
             )
 
         return True
 
     def _set_reader_coord_by_numeric_slice(
-        self, sr: clib.SOMAArrayReader, dim_idx: int, dim: tiledb.Dim, coord: Slice[Any]
+        self, sr: clib.SOMAArray, dim_idx: int, dim: tiledb.Dim, coord: Slice[Any]
     ) -> bool:
 
         try:
             lo_hi = _util.slice_to_numeric_range(coord, dim.domain)
         except _util.NonNumericDimensionError:
             return False  # We only handle numeric dimensions here.
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_dense_nd_array.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_dense_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_exception.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_exception.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_experiment.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_experiment.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,26 +21,46 @@
     CollectionBase[AnyTileDBObject],
     experiment.Experiment[  # type: ignore[type-var]
         DataFrame,
         Collection[Measurement],
         AnyTileDBObject,
     ],
 ):
-    """An :class:`Experiment` represents a single-cell experiment. It is
-    a container class that has observations and measurements.
+    """A collection subtype that combines observations and measurements
+    from an individual experiment.
+
+    In single cell biology, this can represent multiple modes of measurement
+    across a single collection of cells (i.e., a "multimodal dataset").
+    Within an experiment, a set of measurements on a single set of variables
+    (i.e., features) is represented as a :class:`Measurement`.
 
     Attributes:
         obs (DataFrame):
             Primary annotations on the observation axis. The contents of the
             ``soma_joinid`` column define the observation index domain,
             AKA ``obs_id``. All observations for the Experiment must be
             defined in this dataframe.
         ms (Collection):
             A collection of named measurements.
 
+    Example:
+        >>> import tiledbsoma
+        >>> with tiledbsoma.open("/path/to/experiment") as exp:
+        ...     # While users can interact directly with an Experiment's fields:
+        ...     obs_df = exp.obs
+        ...
+        ...     # the primary use case is to run queries on the experiment data.
+        ...     q = exp.query(
+        ...         "mtdna",
+        ...         obs_query=tiledbsoma.AxisQuery(value_filter="tissue == 'lung'"),
+        ...         var_query=tiledbsoma.AxisQuery(coords=(slice(50, 100),)),
+        ...     )
+        ...     query_obs = q.obs().concat().to_pandas()
+        ...     query_var = q.var().concat().to_pandas()
+
     Lifecycle:
         Experimental.
     """
 
     __slots__ = ()
 
     _subclass_constrained_soma_types = {
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_factory.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     SOMA_ENCODING_VERSION_METADATA_KEY,
     SOMA_OBJECT_TYPE_METADATA_KEY,
 )
 from ._exception import SOMAError
 from ._funcs import typeguard_ignore
 from ._types import OpenTimestamp
 from .options import SOMATileDBContext
+from .options._soma_tiledb_context import _validate_soma_tiledb_context
 
 _Obj = TypeVar("_Obj", bound="_tiledb_object.AnyTileDBObject")
 _Wrapper = TypeVar("_Wrapper", bound=_tdb_handles.AnyWrapper)
 
 
 @overload
 def open(
@@ -105,15 +106,15 @@
             recognizable type name or value.
         ValueError:
             If the user-provided ``mode`` is invalid.
 
     Lifecycle:
         Experimental.
     """
-    context = context or SOMATileDBContext()
+    context = _validate_soma_tiledb_context(context)
     obj = _open_internal(_tdb_handles.open, uri, mode, context, tiledb_timestamp)
     try:
         if soma_type:
             if isinstance(soma_type, str):
                 soma_type_name = soma_type
             elif issubclass(soma_type, somacore.SOMAObject):
                 soma_type_name = soma_type.soma_type
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_funcs.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_funcs.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_general_utilities.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_general_utilities.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_measurement.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_measurement.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,50 @@
 # Copyright (c) 2021-2023 TileDB, Inc.
 #
 # Licensed under the MIT License.
 
 """Implementation of a SOMA Measurement.
 """
 
+from typing import Union
+
 from somacore import measurement
 
 from ._collection import Collection, CollectionBase
-from ._common_nd_array import NDArray
 from ._dataframe import DataFrame
 from ._dense_nd_array import DenseNDArray
 from ._sparse_nd_array import SparseNDArray
 from ._tiledb_object import AnyTileDBObject
 
 
 class Measurement(
     CollectionBase[AnyTileDBObject],
     measurement.Measurement[  # type: ignore[type-var]
         DataFrame,
-        Collection[NDArray],
+        Collection[
+            Union[SparseNDArray, DenseNDArray]
+        ],  # not just `NDArray` since that has no common `read`
         Collection[DenseNDArray],
         Collection[SparseNDArray],
         AnyTileDBObject,
     ],
 ):
-    """A :class:`Measurement` is a sub-element of a :class:`Experiment`, and is otherwise
-    a specialized :class:`Collection` with pre-defined fields.
+    """A set of observations defined by a dataframe, with measurements.
+
+    This is a common set of annotated variables (defined by the ``var``
+    dataframe) for which values (e.g., measurements or calculations) are stored
+    in sparse and dense ND arrays.
+
+    The observables are inherited from the parent ``Experiment``'s
+    ``obs`` dataframe. The ``soma_joinid`` of these observables (``obsid``),
+    along with those of the measurement's ``var`` dataframe (``varid``),
+    are the indices for all the other matrices stored in the measurement.
+
+    In most cases, users interact with a measurement via querying the experiment
+    which contains it, rather than directly accessing its fields.
 
     Attributes:
         var (DataFrame):
             Primary annotations on the variable axis, for variables in this measurement
             (i.e., annotates columns of ``X``). The contents of the ``soma_joinid`` column
             define the variable index domain, AKA var_id. All variables for this measurement
             must be defined in this dataframe.
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_query_condition.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_read_iters.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_read_iters.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from ._types import NTuple
 
 
 class TableReadIter(somacore.ReadIter[pa.Table]):
     """Iterator over `Arrow Table <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_ elements"""
 
-    def __init__(self, sr: clib.SOMAArrayReader):
+    def __init__(self, sr: clib.SOMAArray):
         self.sr = sr
 
     def __next__(self) -> pa.Table:
         arrow_table = self.sr.read_next()
         if arrow_table is None:
             raise StopIteration
 
@@ -38,15 +38,15 @@
 
 RT = TypeVar("RT")
 
 
 class SparseTensorReadIterBase(somacore.ReadIter[RT], metaclass=abc.ABCMeta):
     """Private implementation class"""
 
-    def __init__(self, sr: clib.SOMAArrayReader, shape: NTuple):
+    def __init__(self, sr: clib.SOMAArray, shape: NTuple):
         self.sr = sr
         self.shape = shape
 
     @abc.abstractmethod
     def _from_table(self, arrow_table: pa.Table) -> RT:
         raise NotImplementedError()
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_sparse_nd_array.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_sparse_nd_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             return self
 
         raise TypeError(
             f"Unsupported Arrow type or non-arrow type for values argument: {type(values)}"
         )
 
     def _set_reader_coord(
-        self, sr: clib.SOMAArrayReader, dim_idx: int, dim: tiledb.Dim, coord: object
+        self, sr: clib.SOMAArray, dim_idx: int, dim: tiledb.Dim, coord: object
     ) -> bool:
         if super()._set_reader_coord(sr, dim_idx, dim, coord):
             return True
         if isinstance(coord, Sequence):
             if dim.dtype == np.int64:
                 sr.set_dim_points_int64(dim.name, coord)
                 return True
@@ -285,15 +285,15 @@
     See also:
         somacore.data.SparseRead
 
     Lifecycle:
         Experimental.
     """
 
-    def __init__(self, sr: clib.SOMAArrayReader, shape: NTuple):
+    def __init__(self, sr: clib.SOMAArray, shape: NTuple):
         """
         Lifecycle:
             Experimental.
         """
         self.sr = sr
         self.shape = shape
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_tdb_handles.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_tdb_handles.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_tiledb_array.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_tiledb_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,39 +92,37 @@
     def _soma_reader(
         self,
         *,
         schema: Optional[tiledb.ArraySchema] = None,
         column_names: Optional[Sequence[str]] = None,
         query_condition: Optional[tiledb.QueryCondition] = None,
         result_order: Optional[ResultOrderStr] = None,
-    ) -> clib.SOMAArrayReader:
-        """Constructs a C++ SOMAArrayReader using appropriate context/config/etc."""
+    ) -> clib.SOMAArray:
+        """Constructs a C++ SOMAArray using appropriate context/config/etc."""
         # Leave empty arguments out of kwargs to allow C++ constructor defaults to apply, as
         # they're not all wrapped in std::optional<>.
         kwargs: Dict[str, object] = {}
         if schema:
             kwargs["schema"] = schema
         if column_names:
             kwargs["column_names"] = column_names
         if query_condition:
             kwargs["query_condition"] = query_condition
         if result_order:
             result_order_str = ResultOrder(result_order).value
             kwargs["result_order"] = result_order_str
-        return clib.SOMAArrayReader(
+        return clib.SOMAArray(
             self.uri,
             name=f"{self} reader",
             platform_config=self._ctx.config().dict(),
             timestamp=(0, self.tiledb_timestamp_ms),
             **kwargs,
         )
 
-    def _set_reader_coords(
-        self, sr: clib.SOMAArrayReader, coords: Sequence[object]
-    ) -> None:
+    def _set_reader_coords(self, sr: clib.SOMAArray, coords: Sequence[object]) -> None:
         """Parses the given coords and sets them on the SOMA Reader."""
         if not is_nonstringy_sequence(coords):
             raise TypeError(
                 f"coords type {type(coords)} must be a regular sequence,"
                 " not str or bytes"
             )
         schema = self._handle.schema
@@ -138,15 +136,15 @@
             if not self._set_reader_coord(sr, i, dim, coord):
                 raise TypeError(
                     f"coord type {type(coord)} for dimension {dim.name}"
                     f" (slot {i}) unsupported"
                 )
 
     def _set_reader_coord(
-        self, sr: clib.SOMAArrayReader, dim_idx: int, dim: tiledb.Dim, coord: object
+        self, sr: clib.SOMAArray, dim_idx: int, dim: tiledb.Dim, coord: object
     ) -> bool:
         """Parses a single coordinate entry.
 
         The base implementation parses the most fundamental types shared by all
         TileDB Array types; subclasses can implement their own readers that
         handle types not recognized here.
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_tiledb_object.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_tiledb_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from typing_extensions import Self
 
 from . import _constants, _tdb_handles
 from ._exception import SOMAError
 from ._types import OpenTimestamp
 from ._util import check_type, ms_to_datetime
 from .options import SOMATileDBContext
+from .options._soma_tiledb_context import _validate_soma_tiledb_context
 
 _WrapperType_co = TypeVar(
     "_WrapperType_co", bound=_tdb_handles.AnyWrapper, covariant=True
 )
 """The type of handle on a backend object that we have.
 
 Covariant because ``_handle`` is read-only.
@@ -75,15 +76,15 @@
             ValueError:
                 If the user-provided ``mode`` is invalid.
 
         Lifecycle:
             Experimental.
         """
         del platform_config  # unused
-        context = context or SOMATileDBContext()
+        context = _validate_soma_tiledb_context(context)
         handle = cls._wrapper_type.open(uri, mode, context, tiledb_timestamp)
         return cls(
             handle,
             _dont_call_this_use_create_or_open_instead="tiledbsoma-internal-code",
         )
 
     def __init__(
@@ -248,15 +249,15 @@
             >>> tiledbsoma.SparseNDArray.exists("./a_dataframe")
             False
 
         Lifecycle:
             Experimental.
         """
         check_type("uri", uri, (str,))
-        context = context or SOMATileDBContext()
+        context = _validate_soma_tiledb_context(context)
         try:
             with cls._wrapper_type.open(uri, "r", context, tiledb_timestamp) as hdl:
                 md_type = hdl.metadata.get(_constants.SOMA_OBJECT_TYPE_METADATA_KEY)
                 if not isinstance(md_type, str):
                     return False
                 return md_type.lower() == cls.soma_type.lower()
         except (SOMAError, tiledb.cc.TileDBError):
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_types.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/_util.py` & `tiledbsoma-1.2.3/src/tiledbsoma/_util.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/eta.py` & `tiledbsoma-1.2.3/src/tiledbsoma/eta.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/experiment_query.py` & `tiledbsoma-1.2.3/src/tiledbsoma/experiment_query.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/io/conversions.py` & `tiledbsoma-1.2.3/src/tiledbsoma/io/conversions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/io/ingest.py` & `tiledbsoma-1.2.3/src/tiledbsoma/io/ingest.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from .._exception import DoesNotExistError, SOMAError
 from .._funcs import typeguard_ignore
 from .._tdb_handles import RawHandle
 from .._tiledb_array import TileDBArray
 from .._tiledb_object import AnyTileDBObject, TileDBObject
 from .._types import INGEST_MODES, IngestMode, NPNDArray, Path
 from ..options import SOMATileDBContext
+from ..options._soma_tiledb_context import _validate_soma_tiledb_context
 from ..options._tiledb_create_options import TileDBCreateOptions
 from . import conversions
 
 SparseMatrix = Union[sp.csr_matrix, sp.csc_matrix, SparseDataset]
 DenseMatrix = Union[NPNDArray, h5py.Dataset]
 Matrix = Union[DenseMatrix, SparseMatrix]
 _NDArr = TypeVar("_NDArr", bound=NDArray)
@@ -114,15 +115,17 @@
     """
     if ingest_mode not in INGEST_MODES:
         raise SOMAError(
             f'expected ingest_mode to be one of {INGEST_MODES}; got "{ingest_mode}"'
         )
 
     if isinstance(input_path, ad.AnnData):
-        raise TypeError("Input path is an AnnData object -- did you want from_anndata?")
+        raise TypeError("input path is an AnnData object -- did you want from_anndata?")
+
+    context = _validate_soma_tiledb_context(context)
 
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  Experiment.from_h5ad {input_path}")
 
     logging.log_io(None, f"START  READING {input_path}")
 
     anndata = ad.read_h5ad(input_path, backed="r")
@@ -198,14 +201,16 @@
         )
 
     if not isinstance(anndata, ad.AnnData):
         raise TypeError(
             "Second argument is not an AnnData object -- did you want from_h5ad?"
         )
 
+    context = _validate_soma_tiledb_context(context)
+
     # Without _at least_ an index, there is nothing to indicate the dimension indices.
     if anndata.obs.index.empty or anndata.var.index.empty:
         raise NotImplementedError("Empty AnnData.obs or AnnData.var unsupported.")
 
     s = _util.get_start_stamp()
     logging.log_io(None, "START  DECATEGORICALIZING")
 
@@ -1377,15 +1382,16 @@
     obsm = {}
     if "obsm" in measurement:
         for key in measurement.obsm.keys():
             shape = measurement.obsm[key].shape
             if len(shape) != 2:
                 raise ValueError(f"expected shape == 2; got {shape}")
             if isinstance(measurement.obsm[key], DenseNDArray):
-                matrix = measurement.obsm[key].read().to_numpy()
+                obj = cast(DenseNDArray, measurement.obsm[key])
+                matrix = obj.read().to_numpy()
                 # The spelling ``sp.csr_array`` is more idiomatic but doesn't exist until Python 3.8
                 obsm[key] = matrix
             else:
                 # obsp is nobs x nobs.
                 # obsm is nobs x some number -- number of PCA components, etc.
                 matrix = measurement.obsm[key].read().tables().concat().to_pandas()
                 nobs_times_width, coo_column_count = matrix.shape
@@ -1404,15 +1410,16 @@
     varm = {}
     if "varm" in measurement:
         for key in measurement.varm.keys():
             shape = measurement.varm[key].shape
             if len(shape) != 2:
                 raise ValueError(f"expected shape == 2; got {shape}")
             if isinstance(measurement.varm[key], DenseNDArray):
-                matrix = measurement.varm[key].read().to_numpy()
+                obj = cast(DenseNDArray, measurement.varm[key])
+                matrix = obj.read().to_numpy()
                 # The spelling ``sp.csr_array`` is more idiomatic but doesn't exist until Python 3.8
                 varm[key] = matrix
             else:
                 # varp is nvar x nvar.
                 # varm is nvar x some number -- number of PCs, etc.
                 matrix = measurement.varm[key].read().tables().concat().to_pandas()
                 nvar_times_width, coo_column_count = matrix.shape
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/logging.py` & `tiledbsoma-1.2.3/src/tiledbsoma/logging.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/options/_soma_tiledb_context.py` & `tiledbsoma-1.2.3/src/tiledbsoma/options/_soma_tiledb_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -108,7 +108,29 @@
     def _open_timestamp_ms(self, in_timestamp: Optional[OpenTimestamp]) -> int:
         """Returns the real timestamp that should be used to open an object."""
         if in_timestamp is not None:
             return to_timestamp_ms(in_timestamp)
         if self.timestamp_ms is not None:
             return self.timestamp_ms
         return int(time.time() * 1000)
+
+
+def _validate_soma_tiledb_context(context: Any) -> SOMATileDBContext:
+    """Returns the argument, as long as it's a ``SOMATileDBContext``, or a new
+    one if the argument is ``None``. While we already have static type-checking,
+    a few things are extra-important to have runtime validation on.  Since it's
+    easy for users to pass a ``tiledb.Ctx`` when a ``SOMATileDBContext`` is
+    expected, we should offer a helpful redirect when they do.
+    """
+
+    if context is None:
+        return SOMATileDBContext()
+
+    if isinstance(context, tiledb.Ctx):
+        raise TypeError(
+            "context is a tiledb.Ctx, not a SOMATileDBContext -- please wrap it in tiledbsoma.SOMATileDBContext(...)"
+        )
+
+    if not isinstance(context, SOMATileDBContext):
+        raise TypeError("context is not a SOMATileDBContext")
+
+    return context
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/options/_tiledb_create_options.py` & `tiledbsoma-1.2.3/src/tiledbsoma/options/_tiledb_create_options.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/pytiledbsoma.cc` & `tiledbsoma-1.2.3/src/tiledbsoma/pytiledbsoma.cc`

 * *Files 13% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         []() {
             py::print(tiledbsoma::version::as_string());
             std::string stats = tiledbsoma::stats::dump();
             py::print(stats);
         },
         "Print TileDB internal statistics. Lifecycle: experimental.");
 
-    py::class_<SOMAArrayReader>(m, "SOMAArrayReader")
+    py::class_<SOMAArray>(m, "SOMAArray")
         .def(
             py::init(
                 [](std::string_view uri,
                    std::string_view name,
                    std::optional<std::vector<std::string>> column_names_in,
                    py::object py_query_condition,
                    py::object py_schema,
@@ -176,15 +176,16 @@
                                  .get();
                     }
 
                     // Release python GIL after we're done accessing python
                     // objects
                     py::gil_scoped_release release;
 
-                    auto reader = SOMAArrayReader::open(
+                    auto reader = SOMAArray::open(
+                        TILEDB_READ,
                         uri,
                         name,
                         platform_config,
                         column_names,
                         batch_size,
                         result_order,
                         timestamp);
@@ -205,15 +206,15 @@
             "batch_size"_a = "auto",
             "result_order"_a = "auto",
             "platform_config"_a = py::dict(),
             "timestamp"_a = py::none())
 
         .def(
             "reset",
-            [](SOMAArrayReader& reader,
+            [](SOMAArray& reader,
                std::optional<std::vector<std::string>> column_names_in,
                py::object py_query_condition,
                py::object py_schema,
                std::string_view batch_size,
                std::string_view result_order) {
                 // Handle optional args
                 std::vector<std::string> column_names;
@@ -250,15 +251,15 @@
                              .ptr()
                              .get();
                 }
 
                 // Release python GIL after we're done accessing python objects
                 py::gil_scoped_release release;
 
-                // Reset state of the existing SOMAArrayReader object
+                // Reset state of the existing SOMAArray object
                 reader.reset(column_names, batch_size, result_order);
 
                 // Set query condition if present
                 if (qc) {
                     reader.set_condition(*qc);
                 }
             },
@@ -270,15 +271,15 @@
             "result_order"_a = "auto")
 
         // After this are short functions expected to be invoked when the coords
         // are Python list/tuple, or NumPy arrays.  Arrow arrays are in this
         // long if-else-if function.
         .def(
             "set_dim_points_arrow",
-            [](SOMAArrayReader& reader,
+            [](SOMAArray& reader,
                const std::string& dim,
                py::object py_arrow_array,
                int partition_index,
                int partition_count) {
                 // Create a list of array chunks
                 py::list array_chunks;
                 if (py::hasattr(py_arrow_array, "chunks")) {
@@ -455,77 +456,77 @@
         // Experiments have shown that when both float32 and float64 are
         // implemented with overloaded names to be differentiated solely by
         // type, pybind11 uses the _first found_. Therefore it is necessary for
         // us to no longer use common overloaded names.
 
         .def(
             "set_dim_points_string_or_bytes",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<std::string>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_float64",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<double>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_float32",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<float>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_int64",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<int64_t>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_int32",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<int32_t>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_int16",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<int16_t>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_int8",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<int8_t>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_uint64",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<uint64_t>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_uint32",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<uint32_t>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_uint16",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<uint16_t>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         .def(
             "set_dim_points_uint8",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&, const std::vector<uint8_t>&)>(
-                &SOMAArrayReader::set_dim_points))
+                &SOMAArray::set_dim_points))
 
         // In an initial version of this file we had `set_dim_ranges` relying
         // solely on type-overloading. This worked since we supported only int
         // and string indices. In a subsequent version we are now supporting
         // various NumPy/PyArrow types including float32, float64, int8, uint16,
         // etc. It is an unfortunate fact that pybind11 does _not_ successfully
         // disambiguate between float32 and float64, or between int8 and int64,
@@ -534,99 +535,99 @@
         // Experiments have shown that when both float32 and float64 are
         // implemented with overloaded names to be differentiated solely by
         // type, pybind11 uses the _first found_. Therefore it is necessary for
         // us to no longer use common overloaded names.
 
         .def(
             "set_dim_ranges_string_or_bytes",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<std::string, std::string>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_int64",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<int64_t, int64_t>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_int32",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<int32_t, int32_t>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_int16",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<int16_t, int16_t>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_int8",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<int8_t, int8_t>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_uint64",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<uint64_t, uint64_t>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_uint32",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<uint32_t, uint32_t>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_uint16",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<uint16_t, uint16_t>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_uint8",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<uint8_t, uint8_t>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_float64",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<double, double>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "set_dim_ranges_float32",
-            static_cast<void (SOMAArrayReader::*)(
+            static_cast<void (SOMAArray::*)(
                 const std::string&,
                 const std::vector<std::pair<float, float>>&)>(
-                &SOMAArrayReader::set_dim_ranges))
+                &SOMAArray::set_dim_ranges))
 
         .def(
             "submit",
-            &SOMAArrayReader::submit,
+            &SOMAArray::submit,
             py::call_guard<py::gil_scoped_release>())
 
-        .def("results_complete", &SOMAArrayReader::results_complete)
+        .def("results_complete", &SOMAArray::results_complete)
 
         .def(
             "read_next",
-            [](SOMAArrayReader& reader) -> std::optional<py::object> {
+            [](SOMAArray& reader) -> std::optional<py::object> {
                 // Release python GIL before reading data
                 py::gil_scoped_release release;
 
                 // Try to read more data
                 auto buffers = reader.read_next();
 
                 // If more data was read, convert it to an arrow table and
@@ -637,12 +638,12 @@
                     return to_table(*buffers);
                 }
 
                 // No data was read, the query is complete, return nullopt
                 return std::nullopt;
             })
 
-        .def("nnz", &SOMAArrayReader::nnz, py::call_guard<py::gil_scoped_release>())
+        .def("nnz", &SOMAArray::nnz, py::call_guard<py::gil_scoped_release>())
 
-        .def_property_readonly("shape", &SOMAArrayReader::shape);
+        .def_property_readonly("shape", &SOMAArray::shape);
 }
 }  // namespace tiledbsoma
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma/query_condition.cc` & `tiledbsoma-1.2.3/src/tiledbsoma/query_condition.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma.egg-info/PKG-INFO` & `tiledbsoma-1.2.3/src/tiledbsoma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.2.2/src/tiledbsoma.egg-info/SOURCES.txt` & `tiledbsoma-1.2.3/src/tiledbsoma.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,51 +16,50 @@
 dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
 dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
 dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
 dist_links/libtiledbsoma/cmake/patches/spdlog.patch
 dist_links/libtiledbsoma/doc/README.md
 dist_links/libtiledbsoma/doc/reader.svg
 dist_links/libtiledbsoma/doc/reader.uml
-dist_links/libtiledbsoma/external/.clang-format
-dist_links/libtiledbsoma/external/include/span/span.hpp
-dist_links/libtiledbsoma/external/include/thread_pool/producer_consumer_queue.h
-dist_links/libtiledbsoma/external/include/thread_pool/status.h
-dist_links/libtiledbsoma/external/include/thread_pool/thread_pool.h
-dist_links/libtiledbsoma/external/src/thread_pool/status.cc
-dist_links/libtiledbsoma/external/src/thread_pool/thread_pool.cc
-dist_links/libtiledbsoma/include/tiledbsoma/array_buffers.h
-dist_links/libtiledbsoma/include/tiledbsoma/arrow_adapter.h
-dist_links/libtiledbsoma/include/tiledbsoma/carrow.h
-dist_links/libtiledbsoma/include/tiledbsoma/column_buffer.h
-dist_links/libtiledbsoma/include/tiledbsoma/common.h
-dist_links/libtiledbsoma/include/tiledbsoma/logger_public.h
-dist_links/libtiledbsoma/include/tiledbsoma/managed_query.h
-dist_links/libtiledbsoma/include/tiledbsoma/soma_array_reader.h
-dist_links/libtiledbsoma/include/tiledbsoma/spdlog_with_R.h
-dist_links/libtiledbsoma/include/tiledbsoma/stats.h
-dist_links/libtiledbsoma/include/tiledbsoma/tiledbsoma
-dist_links/libtiledbsoma/include/tiledbsoma/util.h
-dist_links/libtiledbsoma/include/tiledbsoma/version.h
 dist_links/libtiledbsoma/src/CMakeLists.txt
-dist_links/libtiledbsoma/src/cli.cc
-dist_links/libtiledbsoma/src/column_buffer.cc
-dist_links/libtiledbsoma/src/logger.cc
-dist_links/libtiledbsoma/src/logger.h
-dist_links/libtiledbsoma/src/managed_query.cc
-dist_links/libtiledbsoma/src/soma_array_reader.cc
-dist_links/libtiledbsoma/src/stats.cc
-dist_links/libtiledbsoma/src/util.cc
-dist_links/libtiledbsoma/src/version.cc
+dist_links/libtiledbsoma/src/cli/cli.cc
+dist_links/libtiledbsoma/src/external/.clang-format
+dist_links/libtiledbsoma/src/external/include/span/span.hpp
+dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
+dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
+dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
+dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
+dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+dist_links/libtiledbsoma/src/soma/managed_query.cc
+dist_links/libtiledbsoma/src/soma/managed_query.h
+dist_links/libtiledbsoma/src/soma/soma_array.cc
+dist_links/libtiledbsoma/src/soma/soma_array.h
+dist_links/libtiledbsoma/src/tiledbsoma/logger_public.h
+dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
+dist_links/libtiledbsoma/src/utils/array_buffers.h
+dist_links/libtiledbsoma/src/utils/arrow_adapter.h
+dist_links/libtiledbsoma/src/utils/carrow.h
+dist_links/libtiledbsoma/src/utils/column_buffer.cc
+dist_links/libtiledbsoma/src/utils/column_buffer.h
+dist_links/libtiledbsoma/src/utils/common.h
+dist_links/libtiledbsoma/src/utils/logger.cc
+dist_links/libtiledbsoma/src/utils/logger.h
+dist_links/libtiledbsoma/src/utils/stats.cc
+dist_links/libtiledbsoma/src/utils/stats.h
+dist_links/libtiledbsoma/src/utils/util.cc
+dist_links/libtiledbsoma/src/utils/util.h
+dist_links/libtiledbsoma/src/utils/version.cc
+dist_links/libtiledbsoma/src/utils/version.h
 dist_links/libtiledbsoma/test/CMakeLists.txt
 dist_links/libtiledbsoma/test/test_query_condition.py
 dist_links/libtiledbsoma/test/test_simple.py
-dist_links/libtiledbsoma/test/test_soma_array_reader.py
+dist_links/libtiledbsoma/test/test_soma_array.py
 dist_links/libtiledbsoma/test/unit_column_buffer.cc
 dist_links/libtiledbsoma/test/unit_managed_query.cc
-dist_links/libtiledbsoma/test/unit_soma_array_reader.cc
+dist_links/libtiledbsoma/test/unit_soma_array.cc
 dist_links/libtiledbsoma/test/unit_thread_pool.cc
 dist_links/scripts/README.md
 dist_links/scripts/bld
 dist_links/scripts/run-clang-format.sh
 dist_links/scripts/show-versions.py
 dist_links/scripts/update-tiledb-version.py
 src/tiledbsoma/__init__.py
```

### Comparing `tiledbsoma-1.2.2/version.py` & `tiledbsoma-1.2.3/version.py`

 * *Files identical despite different names*

