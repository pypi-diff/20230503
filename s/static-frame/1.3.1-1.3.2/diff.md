# Comparing `tmp/static-frame-1.3.1.tar.gz` & `tmp/static-frame-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-1.3.1.tar", last modified: Fri Mar 31 04:03:00 2023, max compression
+gzip compressed data, was "static-frame-1.3.2.tar", last modified: Tue May  2 23:46:44 2023, max compression
```

## Comparing `static-frame-1.3.1.tar` & `static-frame-1.3.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-03-31 04:03:00.514375 static-frame-1.3.1/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.3.1/LICENSE.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.3.1/MANIFEST.in
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22827 2023-03-31 04:03:00.514375 static-frame-1.3.1/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23552 2023-03-31 02:54:43.000000 static-frame-1.3.1/README.rst
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.3.1/requirements-extras.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      362 2023-03-31 02:54:43.000000 static-frame-1.3.1/requirements-test.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       45 2023-03-31 02:54:43.000000 static-frame-1.3.1/requirements.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-03-31 04:03:00.514375 static-frame-1.3.1/setup.cfg
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.3.1/setup.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-03-31 04:03:00.482375 static-frame-1.3.1/static_frame/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7595 2023-03-31 02:56:07.000000 static-frame-1.3.1/static_frame/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/__main__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-03-31 04:03:00.494375 static-frame-1.3.1/static_frame/core/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.1/static_frame/core/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/assign.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3979 2023-03-31 02:54:43.000000 static-frame-1.3.1/static_frame/core/axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    70699 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.3.1/static_frame/core/display_html_datatables.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/display_visidata.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-03-28 16:03:56.000000 static-frame-1.3.1/static_frame/core/doc_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3524 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/exception.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   379746 2023-03-28 16:03:56.000000 static-frame-1.3.1/static_frame/core/frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    57244 2023-03-31 02:54:43.000000 static-frame-1.3.1/static_frame/core/index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21195 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   107621 2023-03-31 02:54:43.000000 static-frame-1.3.1/static_frame/core/index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/interface_meta.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24028 2023-03-31 02:54:43.000000 static-frame-1.3.1/static_frame/core/loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35539 2023-03-28 15:03:13.000000 static-frame-1.3.1/static_frame/core/node_dt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24034 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/node_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/node_hashlib.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31059 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/node_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-03-28 15:03:13.000000 static-frame-1.3.1/static_frame/core/node_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/node_selector.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/node_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/node_transpose.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10016 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/node_values.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/protocol_dfi_abc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-03-31 02:54:43.000000 static-frame-1.3.1/static_frame/core/quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   127657 2023-03-31 02:54:43.000000 static-frame-1.3.1/static_frame/core/series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/store_client_mixin.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/store_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14787 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   185086 2023-03-31 02:54:43.000000 static-frame-1.3.1/static_frame/core/type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   128557 2023-03-31 02:54:43.000000 static-frame-1.3.1/static_frame/core/util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/core/yarn.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.1/static_frame/py.typed
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-03-31 04:03:00.494375 static-frame-1.3.1/static_frame/test/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.1/static_frame/test/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/test_case.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-03-31 04:03:00.514375 static-frame-1.3.1/static_frame/test/unit/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.1/static_frame/test/unit/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35986 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_doc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   640212 2023-03-28 16:03:56.000000 static-frame-1.3.1/static_frame/test/unit/test_frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.3.1/static_frame/test/unit/test_frame_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    59285 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_frame_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_frame_join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_frame_via_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.3.1/static_frame/test/unit/test_frame_via_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    63780 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1394 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    41685 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   164808 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-03-28 16:03:56.000000 static-frame-1.3.1/static_frame/test/unit/test_interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    19542 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16278 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23360 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.3.1/static_frame/test/unit/test_platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    73785 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   242055 2023-03-28 16:03:56.000000 static-frame-1.3.1/static_frame/test/unit/test_series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_series_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14218 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   162493 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   116937 2023-03-31 02:54:43.000000 static-frame-1.3.1/static_frame/test/unit/test_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10382 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47630 2023-03-23 21:26:53.000000 static-frame-1.3.1/static_frame/test/unit/test_yarn.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-03-31 04:03:00.482375 static-frame-1.3.1/static_frame.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22827 2023-03-31 04:03:00.000000 static-frame-1.3.1/static_frame.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-03-31 04:03:00.000000 static-frame-1.3.1/static_frame.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-03-31 04:03:00.000000 static-frame-1.3.1/static_frame.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      199 2023-03-31 04:03:00.000000 static-frame-1.3.1/static_frame.egg-info/requires.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-03-31 04:03:00.000000 static-frame-1.3.1/static_frame.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.452348 static-frame-1.3.2/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.3.2/LICENSE.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.3.2/MANIFEST.in
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22827 2023-05-02 23:46:44.452348 static-frame-1.3.2/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23552 2023-05-02 20:45:20.000000 static-frame-1.3.2/README.rst
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.3.2/requirements-extras.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      362 2023-05-02 20:45:20.000000 static-frame-1.3.2/requirements-test.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       45 2023-05-02 20:45:20.000000 static-frame-1.3.2/requirements.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-02 23:46:44.452348 static-frame-1.3.2/setup.cfg
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.3.2/setup.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.432184 static-frame-1.3.2/static_frame/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7595 2023-05-02 20:42:21.000000 static-frame-1.3.2/static_frame/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/__main__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.444283 static-frame-1.3.2/static_frame/core/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/core/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/assign.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3979 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    70699 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/core/display_html_datatables.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/display_visidata.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/doc_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3524 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/exception.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   379745 2023-05-02 21:14:40.000000 static-frame-1.3.2/static_frame/core/frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    57244 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/core/index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21195 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/core/index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   107621 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/core/index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/interface_meta.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24028 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/core/loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35539 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/node_dt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24034 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_hashlib.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-04-24 22:32:18.000000 static-frame-1.3.2/static_frame/core/node_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/node_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_selector.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_transpose.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10016 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/node_values.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/protocol_dfi_abc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   127657 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/core/series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_client_mixin.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14787 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   185868 2023-05-02 21:14:40.000000 static-frame-1.3.2/static_frame/core/type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   128558 2023-05-02 21:14:40.000000 static-frame-1.3.2/static_frame/core/util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/core/yarn.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/py.typed
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.444283 static-frame-1.3.2/static_frame/test/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/test/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/test_case.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.452348 static-frame-1.3.2/static_frame/test/unit/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.3.2/static_frame/test/unit/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35986 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_doc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   640988 2023-05-02 21:14:40.000000 static-frame-1.3.2/static_frame/test/unit/test_frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-04-24 22:32:18.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.3.2/static_frame/test/unit/test_frame_via_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    63780 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1394 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    41685 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   164808 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/test/unit/test_interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    19542 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16278 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23360 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.3.2/static_frame/test/unit/test_platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    73785 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   242465 2023-04-24 22:32:18.000000 static-frame-1.3.2/static_frame/test/unit/test_series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_series_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14218 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   162493 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   116937 2023-04-19 18:21:25.000000 static-frame-1.3.2/static_frame/test/unit/test_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10382 2023-03-23 21:26:53.000000 static-frame-1.3.2/static_frame/test/unit/test_www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47630 2023-05-02 20:45:20.000000 static-frame-1.3.2/static_frame/test/unit/test_yarn.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-02 23:46:44.436217 static-frame-1.3.2/static_frame.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22827 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      199 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/requires.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-02 23:46:44.000000 static-frame-1.3.2/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-1.3.1/LICENSE.txt` & `static-frame-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/PKG-INFO` & `static-frame-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.3.1
+Version: 1.3.2
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -46,15 +46,15 @@
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
         - automap==0.6.2
-        - arraykit==0.3.1
+        - arraykit==0.3.4
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
         - xarray>=0.13.0
```

### Comparing `static-frame-1.3.1/README.rst` & `static-frame-1.3.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 --------------
 
 Core StaticFrame requires the following:
 
 - Python>=3.7
 - NumPy>=1.18.5
 - automap==0.6.2
-- arraykit==0.3.1
+- arraykit==0.3.4
 
 For extended input and output, the following packages are required:
 
 - pandas>=0.24.2
 - xlsxwriter>=1.1.2
 - openpyxl>=3.0.9
 - xarray>=0.13.0
```

### Comparing `static-frame-1.3.1/setup.py` & `static-frame-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/__init__.py` & `static-frame-1.3.2/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,8 @@
 from static_frame.core.util import IndexSpecifier as IndexSpecifier
 from static_frame.core.util import KeyOrKeys as KeyOrKeys
 from static_frame.core.util import PathSpecifierOrFileLike as PathSpecifierOrFileLike
 from static_frame.core.util import SeriesInitializer as SeriesInitializer
 from static_frame.core.www import WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '1.3.1'
+__version__ = '1.3.2'
```

### Comparing `static-frame-1.3.1/static_frame/__main__.py` & `static-frame-1.3.2/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/archive_npy.py` & `static-frame-1.3.2/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/axis_map.py` & `static-frame-1.3.2/static_frame/core/axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/batch.py` & `static-frame-1.3.2/static_frame/core/batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/bus.py` & `static-frame-1.3.2/static_frame/core/bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/container.py` & `static-frame-1.3.2/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/container_util.py` & `static-frame-1.3.2/static_frame/core/container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/display.py` & `static-frame-1.3.2/static_frame/core/display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/display_color.py` & `static-frame-1.3.2/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/display_config.py` & `static-frame-1.3.2/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/display_html_datatables.py` & `static-frame-1.3.2/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/display_visidata.py` & `static-frame-1.3.2/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/doc_str.py` & `static-frame-1.3.2/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/exception.py` & `static-frame-1.3.2/static_frame/core/exception.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/fill_value_auto.py` & `static-frame-1.3.2/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/frame.py` & `static-frame-1.3.2/static_frame/core/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -5026,15 +5026,14 @@
             row_key: GetItemKeyType = None,
             column_key: GetItemKeyType = None,
             ) -> tp.Union['Frame', Series]:
         '''
         Extract Container based on iloc selection (indices have already mapped)
         '''
         blocks = self._blocks._extract(row_key=row_key, column_key=column_key)
-
         if blocks.__class__ is not TypeBlocks:
             return blocks # type: ignore # reduced to an element
 
         index: IndexBase
         own_index = True # the extracted Frame can always own this index
         row_key_is_slice = row_key.__class__ is slice
         if row_key is None or (row_key_is_slice and row_key == NULL_SLICE):
```

### Comparing `static-frame-1.3.1/static_frame/core/hloc.py` & `static-frame-1.3.2/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/index.py` & `static-frame-1.3.2/static_frame/core/index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/index_auto.py` & `static-frame-1.3.2/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/index_base.py` & `static-frame-1.3.2/static_frame/core/index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/index_correspondence.py` & `static-frame-1.3.2/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/index_datetime.py` & `static-frame-1.3.2/static_frame/core/index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/index_hierarchy.py` & `static-frame-1.3.2/static_frame/core/index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-1.3.2/static_frame/core/index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/interface.py` & `static-frame-1.3.2/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/interface_meta.py` & `static-frame-1.3.2/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/join.py` & `static-frame-1.3.2/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/loc_map.py` & `static-frame-1.3.2/static_frame/core/loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/memory_measure.py` & `static-frame-1.3.2/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/node_dt.py` & `static-frame-1.3.2/static_frame/core/node_dt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/node_fill_value.py` & `static-frame-1.3.2/static_frame/core/node_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/node_hashlib.py` & `static-frame-1.3.2/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/node_iter.py` & `static-frame-1.3.2/static_frame/core/node_iter.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,16 @@
 
     @doc_inject(selector='apply')
     def apply(self,
             func: AnyCallable,
             *,
             dtype: DtypeSpecifier = None,
             name: NameType = None,
-            index_constructor: tp.Optional[IndexConstructor]= None,
+            index_constructor: tp.Optional[IndexConstructor] = None,
+            columns_constructor: tp.Optional[IndexConstructor] = None,
             ) -> FrameOrSeries:
         '''
         {doc} Returns a new container.
 
         Args:
             {func}
             {dtype}
@@ -215,21 +216,34 @@
             raise RuntimeError('use map_fill(), map_any(), or map_all() for applying a mapping type')
 
         if IterNodeApplyType.is_items(self._apply_type):
             apply_func = self.apply_iter_items
         else:
             apply_func = self.apply_iter
 
+        if self._apply_type is IterNodeApplyType.FRAME_ELEMENTS:
+            # can always pass columns_constructor
+            return self._apply_constructor(
+                    apply_func(func),
+                    dtype=dtype,
+                    name=name,
+                    index_constructor=index_constructor,
+                    columns_constructor=columns_constructor,
+                    )
+
+        if columns_constructor is not None:
+            raise RuntimeError('Cannot use `columns_constructor` in this type of apply.')
         return self._apply_constructor(
                 apply_func(func),
                 dtype=dtype,
                 name=name,
                 index_constructor=index_constructor,
                 )
 
+
     @doc_inject(selector='apply')
     def apply_pool(self,
             func: AnyCallable,
             *,
             dtype: DtypeSpecifier = None,
             name: NameType = None,
             index_constructor: tp.Optional[IndexConstructor]= None,
@@ -625,30 +639,40 @@
     def to_frame_from_elements(self,
             items: tp.Iterable[tp.Tuple[
                     tp.Tuple[tp.Hashable, tp.Hashable], tp.Any]],
             *,
             dtype: DtypeSpecifier = None,
             name: NameType = None,
             index_constructor: tp.Optional[IndexConstructor]= None,
+            columns_constructor: tp.Optional[IndexConstructor]= None,
             axis: int = 0,
             ) -> 'Frame':
+        # NOTE: this is only called from `Frame` to produce a new `Frame`
+
         from static_frame.core.frame import Frame
 
-        index_constructor = (self._container._index.from_labels
-                if index_constructor is None else index_constructor)
+        if index_constructor is not None:
+            index = index_constructor(self._container._index)
+        else:
+            index = self._container._index
+
+        assert isinstance(self._container, Frame) # mypy
+
+        if columns_constructor is not None:
+            columns = columns_constructor(self._container._columns)
+        else:
+            columns = self._container._columns
 
-        assert isinstance(self._container, Frame)
         return self._container.__class__.from_element_items(
                 items,
-                index=self._container._index,
-                columns=self._container._columns,
+                index=index,
+                columns=columns,
                 axis=axis,
                 own_index=True,
-                index_constructor=index_constructor,
-                columns_constructor=self._container._columns.from_labels,
+                own_columns=True,
                 name=name,
                 )
 
     def to_index_from_labels(self,
             values: tp.Iterator[tp.Hashable], #pylint: disable=function-redefined
             dtype: DtypeSpecifier = None,
             name: NameType = None,
```

### Comparing `static-frame-1.3.1/static_frame/core/node_re.py` & `static-frame-1.3.2/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/node_selector.py` & `static-frame-1.3.2/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/node_str.py` & `static-frame-1.3.2/static_frame/core/node_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/node_transpose.py` & `static-frame-1.3.2/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/node_values.py` & `static-frame-1.3.2/static_frame/core/node_values.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/pivot.py` & `static-frame-1.3.2/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/platform.py` & `static-frame-1.3.2/static_frame/core/platform.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/protocol_dfi.py` & `static-frame-1.3.2/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/protocol_dfi_abc.py` & `static-frame-1.3.2/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/quilt.py` & `static-frame-1.3.2/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/rank.py` & `static-frame-1.3.2/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/series.py` & `static-frame-1.3.2/static_frame/core/series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/store.py` & `static-frame-1.3.2/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/store_client_mixin.py` & `static-frame-1.3.2/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/store_config.py` & `static-frame-1.3.2/static_frame/core/store_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/store_filter.py` & `static-frame-1.3.2/static_frame/core/store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/store_hdf5.py` & `static-frame-1.3.2/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/store_sqlite.py` & `static-frame-1.3.2/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/store_xlsx.py` & `static-frame-1.3.2/static_frame/core/store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/store_zip.py` & `static-frame-1.3.2/static_frame/core/store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/style_config.py` & `static-frame-1.3.2/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/type_blocks.py` & `static-frame-1.3.2/static_frame/core/type_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -2780,52 +2780,59 @@
                 ):
             if self._shape[1] == 0:
                 yield EMPTY_ARRAY.reshape(self._shape)[row_key]
             elif row_key_null: # when column_key is full
                 yield from self._blocks
             else:
                 for b in self._blocks:
-                    # selection work for both 1D and 2D
-                    block_sliced = b[row_key] # PERF: most time from line profiler
-                    if block_sliced.__class__ is np.ndarray:
-                        if single_row and block_sliced.ndim == 1:
-                            block_sliced = block_sliced.reshape(1, block_sliced.shape[0])
+                    # selection works for both 1D (to an element) and 2D (two a 1D array)
+                    b_row = b[row_key] # PERF: most time from line profiler
+                    if b_row.__class__ is np.ndarray:
+                        if single_row and b_row.ndim == 1:
+                            # reshaping preserves writeable status
+                            b_row = b_row.reshape(1, b_row.shape[0])
+                        yield b_row
                     else: # wrap element back into an array
-                        block_sliced = np.array((block_sliced,), dtype=b.dtype)
-                    yield block_sliced
+                        # If `row_key`` selects a non-array, we have selected an element; if b is an object dtype, we might have selected a list or other iterable that, if naively given to an array constructor, gets "flattened" into arrays. Thus, we create an empty and assign
+                        b_fill = np.empty(1, dtype=b.dtype)
+                        b_fill[0] = b_row
+                        b_fill.flags.writeable = False
+                        yield b_fill
         else:
             # convert column_key into a series of block slices; we have to do this as we stride blocks; do not have to convert row_key as can use directly per block slice
             for block_idx, slc in self._key_to_block_slices(column_key): # PERF: most time from line profiler
                 b = self._blocks[block_idx]
                 if b.ndim == 1: # given 1D array, our row key is all we need
                     if row_key_null:
-                        block_sliced = b
+                        b_sliced = b
                     else:
-                        block_sliced = b[row_key] # PERF: slow from line profiler
+                        b_sliced = b[row_key] # PERF: slow from line profiler
                 else: # given 2D, use row key and column slice
                     if row_key_null:
-                        block_sliced = b[NULL_SLICE, slc]
+                        b_sliced = b[NULL_SLICE, slc]
                     else:
-                        block_sliced = b[row_key, slc]
+                        b_sliced = b[row_key, slc]
 
                 # optionally, apply additional selection, reshaping, or adjustments to what we got out of the block
-                if block_sliced.__class__ is np.ndarray:
+                if b_sliced.__class__ is np.ndarray:
                     # if we have a single row and the thing we sliced is 1d, we need to rotate it
-                    if single_row and block_sliced.ndim == 1:
-                        block_sliced = block_sliced.reshape(1, block_sliced.shape[0])
+                    if single_row and b_sliced.ndim == 1:
+                        b_sliced = b_sliced.reshape(1, b_sliced.shape[0])
                     # if we have a single column as 2d, unpack it; however, we have to make sure this is not a single row in a 2d, which would go to element.
-                    elif (block_sliced.ndim == 2
-                            and block_sliced.shape[1] == 1
+                    elif (b_sliced.ndim == 2
+                            and b_sliced.shape[1] == 1
                             and not single_row):
-                        block_sliced = block_sliced[NULL_SLICE, 0]
-                else: # a single element, wrap back up in array
-                    # NOTE: this is faster than using np.full(1, block_sliced, dtype=dtype)
-                    block_sliced = np.array((block_sliced,), dtype=b.dtype)
-                yield block_sliced
-
+                        b_sliced = b_sliced[NULL_SLICE, 0]
+                    b_sliced.flags.writeable = False
+                    yield b_sliced
+                else: # a single element, wrap back up in array; assignment handles special cases with lists in object dtypes correctly
+                    b_fill = np.empty(1, dtype=b.dtype)
+                    b_fill[0] = b_sliced
+                    b_fill.flags.writeable = False
+                    yield b_fill
 
     def _extract_array(self,
             row_key: tp.Optional[GetItemKeyTypeCompound] = None,
             column_key: tp.Optional[GetItemKeyTypeCompound] = None
             ) -> np.ndarray:
         '''Alternative extractor that returns just an ndarray, concatenating blocks as necessary. Used by internal clients that need to process row/column with an array.
 
@@ -2834,18 +2841,26 @@
         # identifying column_key as integer, then we only access one block, and can return directly without iterating over blocks
         if isinstance(column_key, INT_TYPES):
             block_idx, column = self._index[column_key]
             b = self._blocks[block_idx]
             if b.ndim == 1:
                 if row_key is None:
                     return b
-                return b[row_key]
+                array = b[row_key]
+                if array.__class__ is np.ndarray:
+                    array.flags.writeable = False
+                return array
+
             if row_key is None:
                 return b[NULL_SLICE, column]
-            return b[row_key, column]
+
+            array = b[row_key, column]
+            if array.__class__ is np.ndarray:
+                array.flags.writeable = False
+            return array
 
         # figure out shape from keys so as to not accumulate?
         blocks = []
         rows = 0
         columns = 0
         for b in self._slice_blocks( # a generator
                 row_key=row_key,
```

### Comparing `static-frame-1.3.1/static_frame/core/util.py` & `static-frame-1.3.2/static_frame/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 InexactTypes = tp.Union[float, complex, np.inexact]
 NUMERIC_TYPES = (int, float, complex, np.number)
 
 BOOL_TYPES = (bool, np.bool_)
 DICTLIKE_TYPES = (abc.Set, dict, FrozenAutoMap)
 
 
-# iterables that cannot be used in NP array constructors; asumes that dictlike types have already been identified
+# iterables that cannot be used in NP array constructors; assumes that dictlike types have already been identified
 INVALID_ITERABLE_FOR_ARRAY = (abc.ValuesView, abc.KeysView)
 NON_STR_TYPES = {int, float, bool}
 
 # integers above this value will occassionally, once coerced to a float (64 or 128) in an NP array, will not match a hash lookup as a key in a dictionary; an NP array of int or object will work
 INT_MAX_COERCIBLE_TO_FLOAT = 1_000_000_000_000_000
 
 # for getitem / loc selection
```

### Comparing `static-frame-1.3.1/static_frame/core/www.py` & `static-frame-1.3.2/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/core/yarn.py` & `static-frame-1.3.2/static_frame/core/yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/test_case.py` & `static-frame-1.3.2/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_archive_npy.py` & `static-frame-1.3.2/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_axis_map.py` & `static-frame-1.3.2/static_frame/test/unit/test_axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_batch.py` & `static-frame-1.3.2/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_bus.py` & `static-frame-1.3.2/static_frame/test/unit/test_bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_container.py` & `static-frame-1.3.2/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_container_util.py` & `static-frame-1.3.2/static_frame/test/unit/test_container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_display.py` & `static-frame-1.3.2/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_display_color.py` & `static-frame-1.3.2/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_doc.py` & `static-frame-1.3.2/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-1.3.2/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_frame.py` & `static-frame-1.3.2/static_frame/test/unit/test_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -2679,14 +2679,35 @@
 
         post2 = f.loc[HLoc[:, f['mass'] > 1]]
 
         self.assertEqual(post2.to_pairs(0),
                 (('mass', ((('lepton', 'tau'), 1.777), (('quark', 'charm'), 1.3))), ('charge', ((('lepton', 'tau'), -1.0), (('quark', 'charm'), 0.666))))
                 )
 
+    def test_frame_loc_l(self) -> None:
+        f1 = Frame.from_records((('a', [1, 2]), ('b', [3, 4])))
+        s1 = f1.loc[0]
+        self.assertEqual(s1.values.tolist(), ['a', [1, 2]])
+
+
+        f3 = Frame.from_records(
+                (('a', [1, 2], [10, 20]), ('b', [3, 4], [30, 40])),
+                consolidate_blocks=True)
+        self.assertEqual(f3.shape, (2, 3))
+        self.assertEqual(f3.consolidate.status['shape'].values.tolist(), [(2,), (2, 2)])
+
+        s2 = f3.loc[1]
+        self.assertEqual(s2.values.tolist(), ['b', [3, 4], [30, 40]])
+
+    def test_frame_loc_m(self) -> None:
+        f1 = Frame.from_records((('a', [1, 2], [10, 20]), ('b', [3, 4], [30, 40])))
+        s1 = f1.loc[0, 1:]
+        self.assertEqual(s1.values.tolist(), [[1, 2], [10, 20]])
+
+
     #---------------------------------------------------------------------------
 
     def test_frame_items_a(self) -> None:
 
         records = (
                 (1, 2, 'a', False, True),
                 (30, 50, 'b', True, False))
```

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_frame_he.py` & `static-frame-1.3.2/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_frame_iter.py` & `static-frame-1.3.2/static_frame/test/unit/test_frame_iter.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import static_frame as sf
 from static_frame import Frame
 from static_frame import FrameGO
 from static_frame import HLoc
 from static_frame import IndexDate
 from static_frame import IndexHierarchy
+from static_frame import IndexYear
 from static_frame import Series
 from static_frame import TypeBlocks
 from static_frame.core.exception import AxisInvalid
 from static_frame.test.test_case import TestCase
 
 nan = np.nan
 
@@ -454,14 +455,35 @@
 
         mapping = {x: x*3 for x in range(3)}
         f2 = f1.iter_element(axis=1).map_fill(mapping, fill_value=-1)
         self.assertEqual(f2.to_pairs(),
             ((0, ((0, 0), (1, -1), (2, -1))), (1, ((0, 3), (1, -1), (2, -1))), (2, ((0, 6), (1, -1), (2, -1))))
             )
 
+    def test_frame_iter_element_g1(self) -> None:
+        f1 = Frame(np.arange(9).reshape(3, 3)).rename(index='a', columns='b')
+        f2 = f1.iter_element().apply(str)
+        self.assertEqual(f1.columns.name, f2.columns.name)
+        self.assertEqual(f1.index.name, f2.index.name)
+
+    def test_frame_iter_element_g2(self) -> None:
+        f1 = Frame(np.arange(9).reshape(3, 3), columns=('2021', '1943', '1523')).rename(index='a', columns='b')
+        f2 = f1.iter_element().apply(str, columns_constructor=IndexYear)
+        self.assertIs(f2.columns.__class__, IndexYear)
+        self.assertIs(f2.columns.name, 'b')
+        self.assertEqual(f1.shape, f2.shape)
+
+    def test_frame_iter_element_g3(self) -> None:
+        f1 = Frame(np.arange(9).reshape(3, 3), index=('2021', '1943', '1523')).rename(index='a', columns='b')
+        f2 = f1.iter_element().apply(str, index_constructor=IndexYear)
+        self.assertIs(f2.index.__class__, IndexYear)
+        self.assertIs(f2.index.name, 'a')
+        self.assertEqual(f1.shape, f2.shape)
+
+
     #---------------------------------------------------------------------------
 
     def test_frame_iter_group_a(self) -> None:
         columns = tuple('pqrst')
         index = tuple('zxwy')
         records = (('A', 1, 'a', False, False),
                    ('A', 2, 'b', True, False),
```

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_frame_join.py` & `static-frame-1.3.2/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-1.3.2/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_frame_via_re.py` & `static-frame-1.3.2/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_hloc.py` & `static-frame-1.3.2/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_index.py` & `static-frame-1.3.2/static_frame/test/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_index_auto.py` & `static-frame-1.3.2/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_index_base.py` & `static-frame-1.3.2/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_index_correspondence.py` & `static-frame-1.3.2/static_frame/test/unit/test_index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_index_datetime.py` & `static-frame-1.3.2/static_frame/test/unit/test_index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-1.3.2/static_frame/test/unit/test_index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-1.3.2/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_interface.py` & `static-frame-1.3.2/static_frame/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_loc_map.py` & `static-frame-1.3.2/static_frame/test/unit/test_loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_memory_measure.py` & `static-frame-1.3.2/static_frame/test/unit/test_memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-1.3.2/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_pivot.py` & `static-frame-1.3.2/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-1.3.2/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_quilt.py` & `static-frame-1.3.2/static_frame/test/unit/test_quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_rank.py` & `static-frame-1.3.2/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_series.py` & `static-frame-1.3.2/static_frame/test/unit/test_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1918,27 +1918,38 @@
                 (('a', 0), ('b', 0), ('c', 150), ('d', 0), ('e', 0)))
 
         post3 = tuple(s1.iter_element_items().map_all_iter_items(
                 {(k, v): v * 10 for k, v in s1.items()}))
         self.assertEqual(post3,
                 (('a', 100), ('b', 30), ('c', 150), ('d', 210), ('e', 280)))
 
-    def test_series_iter_element_d(self) -> None:
+    def test_series_iter_element_d1(self) -> None:
 
         s1 = Series((10, 3, 15, 21),
                 index=('2021', '1564', '1876', '2067'),
                 )
         post = s1.iter_element().apply(
                 lambda x: x*2,
                 index_constructor=IndexYear,
                 )
         self.assertTrue(
                 (post.index.values == np.array(['2021', '1564', '1876', '2067'], dtype='datetime64[Y]')).all()
                 )
 
+    def test_series_iter_element_d2(self) -> None:
+        s1 = Series((10, 3, 15, 21),
+                index=('2021', '1564', '1876', '2067'),
+                )
+        # cannot use columns_constructor on Series
+        with self.assertRaises(RuntimeError):
+            _ = s1.iter_element().apply(
+                    lambda x: x*2,
+                    columns_constructor=IndexYear,
+                    )
+
     #---------------------------------------------------------------------------
 
     def test_series_iter_element_map_any_a(self) -> None:
 
         s1 = Series((10, 3, 15, 21, 28),
                 index=('a', 'b', 'c', 'd', 'e'),
                 dtype=object)
```

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_series_he.py` & `static-frame-1.3.2/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_store.py` & `static-frame-1.3.2/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_store_filter.py` & `static-frame-1.3.2/static_frame/test/unit/test_store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_store_hdf5.py` & `static-frame-1.3.2/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_store_sqlite.py` & `static-frame-1.3.2/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_store_xlsx.py` & `static-frame-1.3.2/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_store_zip.py` & `static-frame-1.3.2/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_style_config.py` & `static-frame-1.3.2/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_type_blocks.py` & `static-frame-1.3.2/static_frame/test/unit/test_type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_util.py` & `static-frame-1.3.2/static_frame/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_www.py` & `static-frame-1.3.2/static_frame/test/unit/test_www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame/test/unit/test_yarn.py` & `static-frame-1.3.2/static_frame/test/unit/test_yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.3.1/static_frame.egg-info/PKG-INFO` & `static-frame-1.3.2/static_frame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.3.1
+Version: 1.3.2
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -46,15 +46,15 @@
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
         - automap==0.6.2
-        - arraykit==0.3.1
+        - arraykit==0.3.4
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
         - xarray>=0.13.0
```

### Comparing `static-frame-1.3.1/static_frame.egg-info/SOURCES.txt` & `static-frame-1.3.2/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

