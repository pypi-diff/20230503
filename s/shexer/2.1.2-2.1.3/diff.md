# Comparing `tmp/shexer-2.1.2.tar.gz` & `tmp/shexer-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shexer-2.1.2.tar", last modified: Thu Apr 13 17:30:01 2023, max compression
+gzip compressed data, was "shexer-2.1.3.tar", last modified: Wed May  3 18:38:14 2023, max compression
```

## Comparing `shexer-2.1.2.tar` & `shexer-2.1.3.tar`

### file list

```diff
@@ -1,238 +1,239 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.958874 shexer-2.1.2/
--rw-rw-rw-   0        0        0    11558 2019-11-23 19:24:24.000000 shexer-2.1.2/LICENSE
--rw-rw-rw-   0        0        0    25803 2023-04-13 17:30:01.958874 shexer-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    24887 2023-04-06 19:41:11.000000 shexer-2.1.2/README.md
--rw-rw-rw-   0        0        0       86 2023-04-13 17:30:01.961871 shexer-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1392 2023-04-13 17:29:20.000000 shexer-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:29:59.985873 shexer-2.1.2/shexer/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/__init__.py
--rw-rw-rw-   0        0        0      644 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/consts.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.027882 shexer-2.1.2/shexer/core/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.111872 shexer-2.1.2/shexer/core/instances/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/__init__.py
--rw-rw-rw-   0        0        0      713 2021-10-25 09:34:37.000000 shexer-2.1.2/shexer/core/instances/abstract_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.190873 shexer-2.1.2/shexer/core/instances/annotators/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/annotators/__init__.py
--rw-rw-rw-   0        0        0      383 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/annotator_func.py
--rw-rw-rw-   0        0        0     1817 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/annotator_tracking_instances.py
--rw-rw-rw-   0        0        0     3198 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/annotators/base_annotator.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.297873 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/
--rw-rw-rw-   0        0        0        0 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/__init__.py
--rw-rw-rw-   0        0        0      688 2021-10-25 09:34:37.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
--rw-rw-rw-   0        0        0      592 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
--rw-rw-rw-   0        0        0      807 2021-01-14 17:50:11.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
--rw-rw-rw-   0        0        0     1793 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0      830 2021-10-25 09:34:37.000000 shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
--rw-rw-rw-   0        0        0     4260 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.309874 shexer-2.1.2/shexer/core/instances/mappings/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/mappings/__init__.py
--rw-rw-rw-   0        0        0     1081 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/mappings/shape_map_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.330873 shexer-2.1.2/shexer/core/instances/mix/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/mix/__init__.py
--rw-rw-rw-   0        0        0     2652 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/instances/mix/mixed_instance_tracker.py
--rw-rw-rw-   0        0        0       22 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/core/instances/pconsts.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.364914 shexer-2.1.2/shexer/core/profiling/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/profiling/__init__.py
--rw-rw-rw-   0        0        0     8614 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/profiling/class_profiler.py
--rw-rw-rw-   0        0        0      182 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/profiling/consts.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.431928 shexer-2.1.2/shexer/core/profiling/strategy/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/profiling/strategy/__init__.py
--rw-rw-rw-   0        0        0     6976 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
--rw-rw-rw-   0        0        0     1349 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/profiling/strategy/direct_features_strategy.py
--rw-rw-rw-   0        0        0     7395 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/profiling/strategy/include_reverse_features_strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.436872 shexer-2.1.2/shexer/core/shexing/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/shexing/__init__.py
--rw-rw-rw-   0        0        0     6110 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/class_shexer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.480914 shexer-2.1.2/shexer/core/shexing/strategy/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/core/shexing/strategy/__init__.py
--rw-rw-rw-   0        0        0    16882 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/abstract_shexing_strategy.py
--rw-rw-rw-   0        0        0     5685 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
--rw-rw-rw-   0        0        0     2804 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/direct_shexing_strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.530870 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/
--rw-rw-rw-   0        0        0        0 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
--rw-rw-rw-   0        0        0      118 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
--rw-rw-rw-   0        0        0     1088 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
--rw-rw-rw-   0        0        0      412 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.551875 shexer-2.1.2/shexer/io/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/__init__.py
--rw-rw-rw-   0        0        0      103 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/file.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.553876 shexer-2.1.2/shexer/io/graph/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.750869 shexer-2.1.2/shexer/io/graph/yielder/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/yielder/__init__.py
--rw-rw-rw-   0        0        0     1431 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/base_triples_yielder.py
--rw-rw-rw-   0        0        0    16303 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/big_ttl_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.775871 shexer-2.1.2/shexer/io/graph/yielder/filter/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/yielder/filter/__init__.py
--rw-rw-rw-   0        0        0      862 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
--rw-rw-rw-   0        0        0     1131 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
--rw-rw-rw-   0        0        0     1132 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multi_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     1757 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
--rw-rw-rw-   0        0        0     1166 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     2674 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/multifile_base_triples_yielder.py
--rw-rw-rw-   0        0        0     5686 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/nt_triples_yielder.py
--rw-rw-rw-   0        0        0     6817 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/rdflib_triple_yielder.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.806873 shexer-2.1.2/shexer/io/graph/yielder/remote/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/graph/yielder/remote/__init__.py
--rw-rw-rw-   0        0        0     3826 2023-04-03 18:35:42.000000 shexer-2.1.2/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
--rw-rw-rw-   0        0        0     4724 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.817871 shexer-2.1.2/shexer/io/json/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/json/__init__.py
--rw-rw-rw-   0        0        0      207 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/json/json_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.875872 shexer-2.1.2/shexer/io/line_reader/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/line_reader/__init__.py
--rw-rw-rw-   0        0        0      285 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/io/line_reader/file_line_reader.py
--rw-rw-rw-   0        0        0      332 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/line_reader/gz_line_reader.py
--rw-rw-rw-   0        0        0      260 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/line_reader/raw_string_line_reader.py
--rw-rw-rw-   0        0        0      353 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/io/line_reader/zip_file_line_reader.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.877873 shexer-2.1.2/shexer/io/profile/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.889871 shexer-2.1.2/shexer/io/profile/formater/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/profile/formater/__init__.py
--rw-rw-rw-   0        0        0      409 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/profile/formater/abstract_profile_serializer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.892879 shexer-2.1.2/shexer/io/shacl/
--rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/shacl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.913872 shexer-2.1.2/shexer/io/shacl/formater/
--rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/shacl/formater/__init__.py
--rw-rw-rw-   0        0        0    15833 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/io/shacl/formater/shacl_serializer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.934870 shexer-2.1.2/shexer/io/shape_map/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shape_map/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.961871 shexer-2.1.2/shexer/io/shape_map/label/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shape_map/label/__init__.py
--rw-rw-rw-   0        0        0     1410 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/io/shape_map/label/shape_map_label_parser.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.978913 shexer-2.1.2/shexer/io/shape_map/node_selector/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shape_map/node_selector/__init__.py
--rw-rw-rw-   0        0        0     6755 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/shape_map/node_selector/node_selector_parser.py
--rw-rw-rw-   0        0        0     4966 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shape_map/shape_map_parser.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.981871 shexer-2.1.2/shexer/io/shex/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.012871 shexer-2.1.2/shexer/io/shex/formater/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shex/formater/__init__.py
--rw-rw-rw-   0        0        0      244 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/io/shex/formater/consts.py
--rw-rw-rw-   0        0        0     7006 2023-04-07 09:41:11.000000 shexer-2.1.2/shexer/io/shex/formater/shex_serializer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.100872 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/__init__.py
--rw-rw-rw-   0        0        0     6083 2023-04-13 17:29:20.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
--rw-rw-rw-   0        0        0     2287 2023-02-03 19:09:46.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.161871 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/
--rw-rw-rw-   0        0        0        0 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
--rw-rw-rw-   0        0        0      383 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
--rw-rw-rw-   0        0        0      171 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
--rw-rw-rw-   0        0        0      887 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
--rw-rw-rw-   0        0        0     1278 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
--rw-rw-rw-   0        0        0     1500 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
--rw-rw-rw-   0        0        0     3211 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.182871 shexer-2.1.2/shexer/io/sparql/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/io/sparql/__init__.py
--rw-rw-rw-   0        0        0     4538 2022-07-15 19:02:46.000000 shexer-2.1.2/shexer/io/sparql/query.py
--rw-rw-rw-   0        0        0      469 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/io/wikidata.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.348910 shexer-2.1.2/shexer/model/
--rw-rw-rw-   0        0        0      552 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/IRI.py
--rw-rw-rw-   0        0        0      280 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/Literal.py
--rw-rw-rw-   0        0        0      810 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/model/Macro.py
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/__init__.py
--rw-rw-rw-   0        0        0      502 2021-10-04 17:33:25.000000 shexer-2.1.2/shexer/model/bnode.py
--rw-rw-rw-   0        0        0      100 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/const_elem_types.py
--rw-rw-rw-   0        0        0     1119 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/model/fixed_prop_choice_statement.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.437878 shexer-2.1.2/shexer/model/graph/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/graph/__init__.py
--rw-rw-rw-   0        0        0     6186 2022-07-15 19:02:46.000000 shexer-2.1.2/shexer/model/graph/abstract_sgraph.py
--rw-rw-rw-   0        0        0     7633 2023-04-04 10:53:17.000000 shexer-2.1.2/shexer/model/graph/endpoint_sgraph.py
--rw-rw-rw-   0        0        0     6201 2023-04-04 17:24:52.000000 shexer-2.1.2/shexer/model/graph/rdflib_sgraph.py
--rw-rw-rw-   0        0        0     4173 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/hierarchy_tree.py
--rw-rw-rw-   0        0        0     2527 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/node_selector.py
--rw-rw-rw-   0        0        0      427 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/property.py
--rw-rw-rw-   0        0        0     3361 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/model/shape.py
--rw-rw-rw-   0        0        0      858 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/model/shape_map.py
--rw-rw-rw-   0        0        0     2716 2023-02-02 16:28:05.000000 shexer-2.1.2/shexer/model/statement.py
--rw-rw-rw-   0        0        0    23678 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/shaper.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.583874 shexer-2.1.2/shexer/utils/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/__init__.py
--rw-rw-rw-   0        0        0      621 2022-08-11 11:37:45.000000 shexer-2.1.2/shexer/utils/compression.py
--rw-rw-rw-   0        0        0       94 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/dict.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.760872 shexer-2.1.2/shexer/utils/factories/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/factories/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/utils/factories/class_profiler_factory.py
--rw-rw-rw-   0        0        0     2226 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/utils/factories/class_shexer_factory.py
--rw-rw-rw-   0        0        0      728 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/factories/h_tree.py
--rw-rw-rw-   0        0        0    12215 2023-04-04 10:53:17.000000 shexer-2.1.2/shexer/utils/factories/instance_tracker_factory.py
--rw-rw-rw-   0        0        0      437 2021-10-03 10:32:18.000000 shexer-2.1.2/shexer/utils/factories/iri_factory.py
--rw-rw-rw-   0        0        0      286 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/utils/factories/remote_graph_factory.py
--rw-rw-rw-   0        0        0     1985 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/utils/factories/shape_map_factory.py
--rw-rw-rw-   0        0        0      616 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/factories/shape_map_parser_factory.py
--rw-rw-rw-   0        0        0     1723 2023-04-06 19:32:13.000000 shexer-2.1.2/shexer/utils/factories/shape_serializer_factory.py
--rw-rw-rw-   0        0        0    18627 2023-04-04 10:53:17.000000 shexer-2.1.2/shexer/utils/factories/triple_yielders_factory.py
--rw-rw-rw-   0        0        0      123 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/file.py
--rw-rw-rw-   0        0        0      397 2021-10-04 17:33:25.000000 shexer-2.1.2/shexer/utils/log.py
--rw-rw-rw-   0        0        0      803 2021-01-14 17:50:12.000000 shexer-2.1.2/shexer/utils/namespaces.py
--rw-rw-rw-   0        0        0      967 2019-11-23 19:24:28.000000 shexer-2.1.2/shexer/utils/obj_references.py
--rw-rw-rw-   0        0        0     2008 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/utils/shapes.py
--rw-rw-rw-   0        0        0     1397 2022-03-28 20:28:03.000000 shexer-2.1.2/shexer/utils/target_elements.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.789874 shexer-2.1.2/shexer/utils/translators/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.2/shexer/utils/translators/__init__.py
--rw-rw-rw-   0        0        0     2881 2021-04-26 09:52:52.000000 shexer-2.1.2/shexer/utils/translators/list_of_classes_to_shape_map.py
--rw-rw-rw-   0        0        0     3026 2023-04-03 15:39:42.000000 shexer-2.1.2/shexer/utils/triple_yielders.py
--rw-rw-rw-   0        0        0     5708 2023-04-13 17:29:20.000000 shexer-2.1.2/shexer/utils/uri.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:00.025872 shexer-2.1.2/shexer.egg-info/
--rw-rw-rw-   0        0        0    25803 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7785 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 17:29:58.000000 shexer-2.1.2/shexer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.899875 shexer-2.1.2/test/
--rw-rw-rw-   0        0        0        0 2021-01-14 17:50:12.000000 shexer-2.1.2/test/__init__.py
--rw-rw-rw-   0        0        0     1903 2021-11-20 10:36:36.000000 shexer-2.1.2/test/const.py
--rw-rw-rw-   0        0        0     8963 2023-04-03 18:35:42.000000 shexer-2.1.2/test/t_utils.py
--rw-rw-rw-   0        0        0     1488 2022-08-10 11:13:26.000000 shexer-2.1.2/test/test_all_classes_mode.py
--rw-rw-rw-   0        0        0     1525 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_allow_opt_cardinality.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.906875 shexer-2.1.2/test/test_bugs/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_bugs/__init__.py
--rw-rw-rw-   0        0        0      796 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_bugs/test_no_sharp_in_auto_shape_names.py
--rw-rw-rw-   0        0        0     1192 2023-04-13 17:29:20.000000 shexer-2.1.2/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
--rw-rw-rw-   0        0        0     9920 2022-08-11 11:37:45.000000 shexer-2.1.2/test/test_compression_mode.py
--rw-rw-rw-   0        0        0     2171 2023-02-02 16:28:05.000000 shexer-2.1.2/test/test_decimals.py
--rw-rw-rw-   0        0        0     5564 2023-04-03 18:13:21.000000 shexer-2.1.2/test/test_depth_for_building_subgraph.py
--rw-rw-rw-   0        0        0     3526 2023-04-13 15:42:15.000000 shexer-2.1.2/test/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0     1388 2023-02-02 16:28:05.000000 shexer-2.1.2/test/test_disable_comments.py
--rw-rw-rw-   0        0        0     2922 2023-04-04 10:53:17.000000 shexer-2.1.2/test/test_disable_endpoint_cache.py
--rw-rw-rw-   0        0        0     1491 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_disable_exact_cardinality.py
--rw-rw-rw-   0        0        0     2552 2023-04-03 18:35:42.000000 shexer-2.1.2/test/test_disable_or_statements.py
--rw-rw-rw-   0        0        0     3786 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_discard_and_compliant.py
--rw-rw-rw-   0        0        0     2090 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_file_target_classes.py
--rw-rw-rw-   0        0        0     1677 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_graph_file_input.py
--rw-rw-rw-   0        0        0     3456 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_graph_list_of_file_inputs.py
--rw-rw-rw-   0        0        0     1951 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_infer_numeric_types_for_untyped_literals.py
--rw-rw-rw-   0        0        0     7818 2023-02-02 16:28:05.000000 shexer-2.1.2/test/test_input_format.py
--rw-rw-rw-   0        0        0     3367 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_instances_file_input.py
--rw-rw-rw-   0        0        0     3852 2023-02-02 16:28:05.000000 shexer-2.1.2/test/test_instances_report.py
--rw-rw-rw-   0        0        0     3548 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_instantiation_property.py
--rw-rw-rw-   0        0        0     1964 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_inverse_paths.py
--rw-rw-rw-   0        0        0     3594 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_keep_less_specific.py
--rw-rw-rw-   0        0        0     4051 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_list_of_url_input.py
--rw-rw-rw-   0        0        0     4106 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_namespaces_dict.py
--rw-rw-rw-   0        0        0     2082 2023-04-13 17:23:12.000000 shexer-2.1.2/test/test_namespaces_to_ignore.py
--rw-rw-rw-   0        0        0     5000 2021-01-14 17:50:12.000000 shexer-2.1.2/test/test_raw_graph.py
--rw-rw-rw-   0        0        0     4300 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_raw_shape_map.py
--rw-rw-rw-   0        0        0     1711 2022-07-15 19:02:46.000000 shexer-2.1.2/test/test_rdflib_graph.py
--rw-rw-rw-   0        0        0     2930 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_remove_empty_sahpes.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.917874 shexer-2.1.2/test/test_shacl/
--rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.2/test/test_shacl/__init__.py
--rw-rw-rw-   0        0        0     2225 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shacl/test_annotation.py
--rw-rw-rw-   0        0        0     2242 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shacl/test_class_selection.py
--rw-rw-rw-   0        0        0     3291 2023-04-06 19:32:13.000000 shexer-2.1.2/test/test_shacl/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0      910 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_shacl/test_literal_types.py
--rw-rw-rw-   0        0        0     4313 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shape_map_file.py
--rw-rw-rw-   0        0        0     6086 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shape_map_format.py
--rw-rw-rw-   0        0        0     2307 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0     2889 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_shapes_namespaces.py
--rw-rw-rw-   0        0        0     2452 2022-03-28 20:28:03.000000 shexer-2.1.2/test/test_sort.py
--rw-rw-rw-   0        0        0     2058 2021-10-24 17:07:37.000000 shexer-2.1.2/test/test_target_classes.py
--rw-rw-rw-   0        0        0     3120 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_threshold.py
--rw-rw-rw-   0        0        0     2578 2023-04-03 18:13:27.000000 shexer-2.1.2/test/test_url_endpoint.py
--rw-rw-rw-   0        0        0     1867 2022-07-15 19:02:46.000000 shexer-2.1.2/test/test_url_graph.py
--rw-rw-rw-   0        0        0     1900 2021-10-03 10:32:18.000000 shexer-2.1.2/test/test_wikidata_annotation.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:30:01.956872 shexer-2.1.2/ws/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.2/ws/__init__.py
--rw-rw-rw-   0        0        0    19884 2022-03-28 20:28:03.000000 shexer-2.1.2/ws/shexer_rest.py
--rw-rw-rw-   0        0        0       28 2019-11-23 19:24:29.000000 shexer-2.1.2/ws/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.887637 shexer-2.1.3/
+-rw-rw-rw-   0        0        0    11558 2019-11-23 19:24:24.000000 shexer-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0    26626 2023-05-03 18:38:14.887958 shexer-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    25710 2023-05-03 18:36:37.000000 shexer-2.1.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-03 18:38:14.890637 shexer-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2023-05-03 18:37:15.000000 shexer-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.640580 shexer-2.1.3/shexer/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/__init__.py
+-rw-rw-rw-   0        0        0      644 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/consts.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.683448 shexer-2.1.3/shexer/core/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.757293 shexer-2.1.3/shexer/core/instances/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/__init__.py
+-rw-rw-rw-   0        0        0      713 2021-10-25 09:34:37.000000 shexer-2.1.3/shexer/core/instances/abstract_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.833421 shexer-2.1.3/shexer/core/instances/annotators/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/annotators/__init__.py
+-rw-rw-rw-   0        0        0      383 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/annotator_func.py
+-rw-rw-rw-   0        0        0     1817 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/annotator_tracking_instances.py
+-rw-rw-rw-   0        0        0     3198 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/annotators/base_annotator.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.926403 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/
+-rw-rw-rw-   0        0        0        0 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/__init__.py
+-rw-rw-rw-   0        0        0      688 2021-10-25 09:34:37.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
+-rw-rw-rw-   0        0        0      592 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
+-rw-rw-rw-   0        0        0      807 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
+-rw-rw-rw-   0        0        0     1793 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0      830 2021-10-25 09:34:37.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
+-rw-rw-rw-   0        0        0     4260 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/instance_tracker.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.938404 shexer-2.1.3/shexer/core/instances/mappings/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/mappings/__init__.py
+-rw-rw-rw-   0        0        0     1081 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/mappings/shape_map_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.958403 shexer-2.1.3/shexer/core/instances/mix/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/mix/__init__.py
+-rw-rw-rw-   0        0        0     2652 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/mix/mixed_instance_tracker.py
+-rw-rw-rw-   0        0        0       22 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/pconsts.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.020357 shexer-2.1.3/shexer/core/profiling/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/profiling/__init__.py
+-rw-rw-rw-   0        0        0     8614 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/profiling/class_profiler.py
+-rw-rw-rw-   0        0        0      182 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/profiling/consts.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.102592 shexer-2.1.3/shexer/core/profiling/strategy/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/profiling/strategy/__init__.py
+-rw-rw-rw-   0        0        0     6976 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
+-rw-rw-rw-   0        0        0     1349 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/profiling/strategy/direct_features_strategy.py
+-rw-rw-rw-   0        0        0     7395 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/profiling/strategy/include_reverse_features_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.107272 shexer-2.1.3/shexer/core/shexing/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/shexing/__init__.py
+-rw-rw-rw-   0        0        0     6191 2023-05-03 17:48:10.000000 shexer-2.1.3/shexer/core/shexing/class_shexer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.185346 shexer-2.1.3/shexer/core/shexing/strategy/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/shexing/strategy/__init__.py
+-rw-rw-rw-   0        0        0    17141 2023-05-03 17:48:10.000000 shexer-2.1.3/shexer/core/shexing/strategy/abstract_shexing_strategy.py
+-rw-rw-rw-   0        0        0     5685 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
+-rw-rw-rw-   0        0        0     2804 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/direct_shexing_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.227464 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/
+-rw-rw-rw-   0        0        0        0 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
+-rw-rw-rw-   0        0        0     1088 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
+-rw-rw-rw-   0        0        0      412 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.250502 shexer-2.1.3/shexer/io/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/__init__.py
+-rw-rw-rw-   0        0        0      103 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.252471 shexer-2.1.3/shexer/io/graph/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.529347 shexer-2.1.3/shexer/io/graph/yielder/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/yielder/__init__.py
+-rw-rw-rw-   0        0        0     1431 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/base_triples_yielder.py
+-rw-rw-rw-   0        0        0    16303 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/big_ttl_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.555857 shexer-2.1.3/shexer/io/graph/yielder/filter/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/yielder/filter/__init__.py
+-rw-rw-rw-   0        0        0      862 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
+-rw-rw-rw-   0        0        0     1131 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
+-rw-rw-rw-   0        0        0     1132 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multi_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     1757 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
+-rw-rw-rw-   0        0        0     1166 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     2674 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multifile_base_triples_yielder.py
+-rw-rw-rw-   0        0        0     5686 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     6817 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/rdflib_triple_yielder.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.592572 shexer-2.1.3/shexer/io/graph/yielder/remote/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/yielder/remote/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-04-03 18:35:42.000000 shexer-2.1.3/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
+-rw-rw-rw-   0        0        0     4724 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.607178 shexer-2.1.3/shexer/io/json/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/json/__init__.py
+-rw-rw-rw-   0        0        0      207 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/json/json_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.649582 shexer-2.1.3/shexer/io/line_reader/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/line_reader/__init__.py
+-rw-rw-rw-   0        0        0      285 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/io/line_reader/file_line_reader.py
+-rw-rw-rw-   0        0        0      332 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/line_reader/gz_line_reader.py
+-rw-rw-rw-   0        0        0      260 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/line_reader/raw_string_line_reader.py
+-rw-rw-rw-   0        0        0      353 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/line_reader/zip_file_line_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.652583 shexer-2.1.3/shexer/io/profile/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.664212 shexer-2.1.3/shexer/io/profile/formater/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/profile/formater/__init__.py
+-rw-rw-rw-   0        0        0      409 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/profile/formater/abstract_profile_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.666675 shexer-2.1.3/shexer/io/shacl/
+-rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/shacl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.689185 shexer-2.1.3/shexer/io/shacl/formater/
+-rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/shacl/formater/__init__.py
+-rw-rw-rw-   0        0        0    15833 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/io/shacl/formater/shacl_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.714186 shexer-2.1.3/shexer/io/shape_map/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shape_map/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.740196 shexer-2.1.3/shexer/io/shape_map/label/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shape_map/label/__init__.py
+-rw-rw-rw-   0        0        0     1410 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/io/shape_map/label/shape_map_label_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.775381 shexer-2.1.3/shexer/io/shape_map/node_selector/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shape_map/node_selector/__init__.py
+-rw-rw-rw-   0        0        0     6755 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/shape_map/node_selector/node_selector_parser.py
+-rw-rw-rw-   0        0        0     4966 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shape_map/shape_map_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.777197 shexer-2.1.3/shexer/io/shex/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.809260 shexer-2.1.3/shexer/io/shex/formater/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shex/formater/__init__.py
+-rw-rw-rw-   0        0        0      244 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/io/shex/formater/consts.py
+-rw-rw-rw-   0        0        0     7006 2023-04-07 09:41:11.000000 shexer-2.1.3/shexer/io/shex/formater/shex_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.947403 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/__init__.py
+-rw-rw-rw-   0        0        0     6083 2023-04-13 17:29:20.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
+-rw-rw-rw-   0        0        0     2287 2023-02-03 19:09:46.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.023201 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/
+-rw-rw-rw-   0        0        0        0 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
+-rw-rw-rw-   0        0        0      171 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
+-rw-rw-rw-   0        0        0      887 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
+-rw-rw-rw-   0        0        0     1278 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
+-rw-rw-rw-   0        0        0     1500 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
+-rw-rw-rw-   0        0        0     3211 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.051487 shexer-2.1.3/shexer/io/sparql/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/sparql/__init__.py
+-rw-rw-rw-   0        0        0     4538 2022-07-15 19:02:46.000000 shexer-2.1.3/shexer/io/sparql/query.py
+-rw-rw-rw-   0        0        0      469 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/wikidata.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.238240 shexer-2.1.3/shexer/model/
+-rw-rw-rw-   0        0        0      552 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/IRI.py
+-rw-rw-rw-   0        0        0      280 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/Literal.py
+-rw-rw-rw-   0        0        0      810 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/model/Macro.py
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/__init__.py
+-rw-rw-rw-   0        0        0      502 2021-10-04 17:33:25.000000 shexer-2.1.3/shexer/model/bnode.py
+-rw-rw-rw-   0        0        0      100 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/const_elem_types.py
+-rw-rw-rw-   0        0        0     1119 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/model/fixed_prop_choice_statement.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.310935 shexer-2.1.3/shexer/model/graph/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/graph/__init__.py
+-rw-rw-rw-   0        0        0     6186 2022-07-15 19:02:46.000000 shexer-2.1.3/shexer/model/graph/abstract_sgraph.py
+-rw-rw-rw-   0        0        0     7633 2023-04-04 10:53:17.000000 shexer-2.1.3/shexer/model/graph/endpoint_sgraph.py
+-rw-rw-rw-   0        0        0     6201 2023-04-04 17:24:52.000000 shexer-2.1.3/shexer/model/graph/rdflib_sgraph.py
+-rw-rw-rw-   0        0        0     4173 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/hierarchy_tree.py
+-rw-rw-rw-   0        0        0     2527 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/node_selector.py
+-rw-rw-rw-   0        0        0      427 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/property.py
+-rw-rw-rw-   0        0        0     3361 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/model/shape.py
+-rw-rw-rw-   0        0        0      858 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/shape_map.py
+-rw-rw-rw-   0        0        0     2716 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/model/statement.py
+-rw-rw-rw-   0        0        0    24509 2023-05-03 18:36:37.000000 shexer-2.1.3/shexer/shaper.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.492195 shexer-2.1.3/shexer/utils/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/__init__.py
+-rw-rw-rw-   0        0        0      621 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/utils/compression.py
+-rw-rw-rw-   0        0        0       94 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/dict.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.677481 shexer-2.1.3/shexer/utils/factories/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/factories/__init__.py
+-rw-rw-rw-   0        0        0     4300 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/utils/factories/class_profiler_factory.py
+-rw-rw-rw-   0        0        0     2322 2023-05-03 18:36:37.000000 shexer-2.1.3/shexer/utils/factories/class_shexer_factory.py
+-rw-rw-rw-   0        0        0      728 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/factories/h_tree.py
+-rw-rw-rw-   0        0        0    12215 2023-04-04 10:53:17.000000 shexer-2.1.3/shexer/utils/factories/instance_tracker_factory.py
+-rw-rw-rw-   0        0        0      437 2021-10-03 10:32:18.000000 shexer-2.1.3/shexer/utils/factories/iri_factory.py
+-rw-rw-rw-   0        0        0      286 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/utils/factories/remote_graph_factory.py
+-rw-rw-rw-   0        0        0     1985 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/utils/factories/shape_map_factory.py
+-rw-rw-rw-   0        0        0      616 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/factories/shape_map_parser_factory.py
+-rw-rw-rw-   0        0        0     1723 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/utils/factories/shape_serializer_factory.py
+-rw-rw-rw-   0        0        0    18627 2023-04-04 10:53:17.000000 shexer-2.1.3/shexer/utils/factories/triple_yielders_factory.py
+-rw-rw-rw-   0        0        0      123 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/file.py
+-rw-rw-rw-   0        0        0      397 2021-10-04 17:33:25.000000 shexer-2.1.3/shexer/utils/log.py
+-rw-rw-rw-   0        0        0      803 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/utils/namespaces.py
+-rw-rw-rw-   0        0        0      967 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/obj_references.py
+-rw-rw-rw-   0        0        0     2008 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/utils/shapes.py
+-rw-rw-rw-   0        0        0     1397 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/utils/target_elements.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.708407 shexer-2.1.3/shexer/utils/translators/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.3/shexer/utils/translators/__init__.py
+-rw-rw-rw-   0        0        0     2881 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/utils/translators/list_of_classes_to_shape_map.py
+-rw-rw-rw-   0        0        0     3026 2023-04-03 15:39:42.000000 shexer-2.1.3/shexer/utils/triple_yielders.py
+-rw-rw-rw-   0        0        0     5708 2023-04-13 17:29:20.000000 shexer-2.1.3/shexer/utils/uri.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.681762 shexer-2.1.3/shexer.egg-info/
+-rw-rw-rw-   0        0        0    26626 2023-05-03 18:38:10.000000 shexer-2.1.3/shexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7817 2023-05-03 18:38:11.000000 shexer-2.1.3/shexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:38:10.000000 shexer-2.1.3/shexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-03 18:38:10.000000 shexer-2.1.3/shexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-03 18:38:10.000000 shexer-2.1.3/shexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.829539 shexer-2.1.3/test/
+-rw-rw-rw-   0        0        0        0 2021-01-14 17:50:12.000000 shexer-2.1.3/test/__init__.py
+-rw-rw-rw-   0        0        0     1903 2021-11-20 10:36:36.000000 shexer-2.1.3/test/const.py
+-rw-rw-rw-   0        0        0     8963 2023-04-03 18:35:42.000000 shexer-2.1.3/test/t_utils.py
+-rw-rw-rw-   0        0        0     1488 2022-08-10 11:13:26.000000 shexer-2.1.3/test/test_all_classes_mode.py
+-rw-rw-rw-   0        0        0     1525 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_allow_opt_cardinality.py
+-rw-rw-rw-   0        0        0     3541 2023-05-03 18:36:37.000000 shexer-2.1.3/test/test_allow_redundant_or.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.836265 shexer-2.1.3/test/test_bugs/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_bugs/__init__.py
+-rw-rw-rw-   0        0        0      796 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_bugs/test_no_sharp_in_auto_shape_names.py
+-rw-rw-rw-   0        0        0     1192 2023-04-13 17:29:20.000000 shexer-2.1.3/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
+-rw-rw-rw-   0        0        0     9920 2022-08-11 11:37:45.000000 shexer-2.1.3/test/test_compression_mode.py
+-rw-rw-rw-   0        0        0     2171 2023-02-02 16:28:05.000000 shexer-2.1.3/test/test_decimals.py
+-rw-rw-rw-   0        0        0     5564 2023-04-03 18:13:21.000000 shexer-2.1.3/test/test_depth_for_building_subgraph.py
+-rw-rw-rw-   0        0        0     3526 2023-05-03 18:36:37.000000 shexer-2.1.3/test/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0     1388 2023-02-02 16:28:05.000000 shexer-2.1.3/test/test_disable_comments.py
+-rw-rw-rw-   0        0        0     2922 2023-04-04 10:53:17.000000 shexer-2.1.3/test/test_disable_endpoint_cache.py
+-rw-rw-rw-   0        0        0     1491 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_disable_exact_cardinality.py
+-rw-rw-rw-   0        0        0     2557 2023-05-03 18:36:37.000000 shexer-2.1.3/test/test_disable_or_statements.py
+-rw-rw-rw-   0        0        0     3786 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_discard_and_compliant.py
+-rw-rw-rw-   0        0        0     2090 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_file_target_classes.py
+-rw-rw-rw-   0        0        0     1677 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_graph_file_input.py
+-rw-rw-rw-   0        0        0     3456 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_graph_list_of_file_inputs.py
+-rw-rw-rw-   0        0        0     1951 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_infer_numeric_types_for_untyped_literals.py
+-rw-rw-rw-   0        0        0     7818 2023-02-02 16:28:05.000000 shexer-2.1.3/test/test_input_format.py
+-rw-rw-rw-   0        0        0     3367 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_instances_file_input.py
+-rw-rw-rw-   0        0        0     3852 2023-02-02 16:28:05.000000 shexer-2.1.3/test/test_instances_report.py
+-rw-rw-rw-   0        0        0     3548 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_instantiation_property.py
+-rw-rw-rw-   0        0        0     1964 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_inverse_paths.py
+-rw-rw-rw-   0        0        0     3594 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_keep_less_specific.py
+-rw-rw-rw-   0        0        0     4051 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_list_of_url_input.py
+-rw-rw-rw-   0        0        0     4106 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_namespaces_dict.py
+-rw-rw-rw-   0        0        0     2082 2023-04-13 17:23:12.000000 shexer-2.1.3/test/test_namespaces_to_ignore.py
+-rw-rw-rw-   0        0        0     5000 2021-01-14 17:50:12.000000 shexer-2.1.3/test/test_raw_graph.py
+-rw-rw-rw-   0        0        0     4300 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_raw_shape_map.py
+-rw-rw-rw-   0        0        0     1711 2022-07-15 19:02:46.000000 shexer-2.1.3/test/test_rdflib_graph.py
+-rw-rw-rw-   0        0        0     2930 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_remove_empty_sahpes.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.848264 shexer-2.1.3/test/test_shacl/
+-rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.3/test/test_shacl/__init__.py
+-rw-rw-rw-   0        0        0     2225 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shacl/test_annotation.py
+-rw-rw-rw-   0        0        0     2242 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shacl/test_class_selection.py
+-rw-rw-rw-   0        0        0     3291 2023-04-06 19:32:13.000000 shexer-2.1.3/test/test_shacl/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0      910 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_shacl/test_literal_types.py
+-rw-rw-rw-   0        0        0     4313 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shape_map_file.py
+-rw-rw-rw-   0        0        0     6086 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shape_map_format.py
+-rw-rw-rw-   0        0        0     2307 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0     2889 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shapes_namespaces.py
+-rw-rw-rw-   0        0        0     2452 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_sort.py
+-rw-rw-rw-   0        0        0     2058 2021-10-24 17:07:37.000000 shexer-2.1.3/test/test_target_classes.py
+-rw-rw-rw-   0        0        0     3120 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_threshold.py
+-rw-rw-rw-   0        0        0     2578 2023-04-03 18:13:27.000000 shexer-2.1.3/test/test_url_endpoint.py
+-rw-rw-rw-   0        0        0     1867 2022-07-15 19:02:46.000000 shexer-2.1.3/test/test_url_graph.py
+-rw-rw-rw-   0        0        0     1900 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_wikidata_annotation.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.885639 shexer-2.1.3/ws/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.3/ws/__init__.py
+-rw-rw-rw-   0        0        0    19884 2022-03-28 20:28:03.000000 shexer-2.1.3/ws/shexer_rest.py
+-rw-rw-rw-   0        0        0       28 2019-11-23 19:24:29.000000 shexer-2.1.3/ws/wsgi.py
```

### Comparing `shexer-2.1.2/LICENSE` & `shexer-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/PKG-INFO` & `shexer-2.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.1.2
+Version: 2.1.3
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.2.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.3.tar.gz
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -215,14 +215,15 @@
 * instantiation_property (default rdf:type): full URI (no prefixes) of the property linking instances and classes (ex: P31 in Wikidata's ontology)
 * namespaces_to_ignore (default None): list of namespaces of properties used in the target graph which are going to be ignored. For example, if you set namespaces_to_ignore to \[http://example.org/\], every triple whose predicate belongs to that namespace will not be computed. It just excludes properties whose name is a direct child of the namespace. For example, triples with <http:/example.org/foo> will be ignored, but triples with <http://example.org/anotherLevel/foo> will be computed.
 * infer_numeric_types_for_untyped_literals (default False): when it is set to True, if the parser finds a triple whose object in a number untyped (something like 56 instead of "56"^^xsd:int), it will accept it and consider it an int if it has decimals or a float if it does not. If it is set to False, triples like that will raise a parsing error.
 * discard_useles_constraints_with_positive_closure (default True): if it is set to True, when two constraints have been extracted with identical property and object, and one of them has '+' cardinality while the other one has a specific number of occurrences (example: {1}, {2}...), if they both have the same rate of compliance among the instances, the constraint with the '+' cardinality is discarded.
 * all_instances_are_compliant_mode (default True): when set to True, every inferred constraint which is not valid for all the instances of the class associated to the shape, then the cardinality of that constraint is changed to '\*' or '?'. With this, every instance conforms to the shape associated with its class. When it is set to False, no cardinality is changed, so there may be instances that do not conform to the inferred shape.
 * keep_less_specific (default True): when it is set to True, for a group of constraints with the same property and object but different cardinality, the one with less specific cardinality ('+') will be preserved, and the rest of constraints used to provide info in comments. When it is set to False, the preserved constraint will be the one with an integer as cardinality and the highest rate of conformance with the instances of the class.
 * disable_or_statements (default True): when set to False, sheXer tries to infer constraints with the operator oneOf (|) in case there are constraints with the same property but different object. By default, sheXer groups those constraint in a isngle one having the less general object possible. For instance, when the objects are different shapes, it merges the constraints a single one whose object is IRI.
+* allow_redundant_or (default False): when this is set to True, the example described for the disable_or_statements behaves differently. Let's say we have a set of candidate constraints whose property is the same but whose object differs: one have IRI, and two other have different shape labels (:A and :B). Whith allow_redundant_or=False, sheXer generates a single constraint with IRI and moves the information about the rest of discarded constraints with more specific objects to comments. However, with allow_redundant_or=True, the constraint generated will have a node constraint with a disjunction such as IRI OR @A OR @B. From the point of view of validation, as IRI subsumes :A and :B, this has no effect. However, some user whose extracted shapes are used to generate further products find this feature useful.   
 * allow_opt_cardinality (default True). When all-compliant mode is active, if there is a constraint which does not conform with every isntance but its maximun cardinality for any instance is {1}, it uses the optional cardinality (?). When set to False, it uses Kleene closure instead.
 * disable_opt_cardinality (dafault False). When set to True, it prevents any constraint to have a higher cardinality higher than one, even if every instance has that cardinality. For example, a constraint such as *ex:alias xsd:string {3}* will be changed to *ex:alias xsd:string +*.
 * shape_qualifiers_mode (default False). When it is set to True, it assumes a data model similar to Wikidata's one, where entity nodes are linked with qualifiers (BNodes) instead of the actual object meant by the triple. It is used to produce legible shapes for those special BNodes.
 * namespaces_for_qualifier_props (default None). Provide here a list of namespace in which the indirect properties used to link an entity with a qualifier node can be found. A reasonable configuration for Wikidata is namespaces_for_qualifier_props = \["http://www.wikidata.org/prop/"\] .
 * inverse_paths (default False). When it is set to True, sheXer will produce constraints with inverse_paths too. This is, constraints referring to triples in which the target node acst as object. Direct and inverse paths will be sorted in the final results w.r.t. their trutsworthiness score.
 * detect_minimal_iri (default False). When it is set to True, each shape will be associated with a regex pattern. That pattern expresses the initial part of the IRI that is common to every isntance used to extract a given shape. This pattern is only serialized when it is a "worthy" one (long enough, not just "http://", etc.).
```

### Comparing `shexer-2.1.2/README.md` & `shexer-2.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,15 @@
 * instantiation_property (default rdf:type): full URI (no prefixes) of the property linking instances and classes (ex: P31 in Wikidata's ontology)
 * namespaces_to_ignore (default None): list of namespaces of properties used in the target graph which are going to be ignored. For example, if you set namespaces_to_ignore to \[http://example.org/\], every triple whose predicate belongs to that namespace will not be computed. It just excludes properties whose name is a direct child of the namespace. For example, triples with <http:/example.org/foo> will be ignored, but triples with <http://example.org/anotherLevel/foo> will be computed.
 * infer_numeric_types_for_untyped_literals (default False): when it is set to True, if the parser finds a triple whose object in a number untyped (something like 56 instead of "56"^^xsd:int), it will accept it and consider it an int if it has decimals or a float if it does not. If it is set to False, triples like that will raise a parsing error.
 * discard_useles_constraints_with_positive_closure (default True): if it is set to True, when two constraints have been extracted with identical property and object, and one of them has '+' cardinality while the other one has a specific number of occurrences (example: {1}, {2}...), if they both have the same rate of compliance among the instances, the constraint with the '+' cardinality is discarded.
 * all_instances_are_compliant_mode (default True): when set to True, every inferred constraint which is not valid for all the instances of the class associated to the shape, then the cardinality of that constraint is changed to '\*' or '?'. With this, every instance conforms to the shape associated with its class. When it is set to False, no cardinality is changed, so there may be instances that do not conform to the inferred shape.
 * keep_less_specific (default True): when it is set to True, for a group of constraints with the same property and object but different cardinality, the one with less specific cardinality ('+') will be preserved, and the rest of constraints used to provide info in comments. When it is set to False, the preserved constraint will be the one with an integer as cardinality and the highest rate of conformance with the instances of the class.
 * disable_or_statements (default True): when set to False, sheXer tries to infer constraints with the operator oneOf (|) in case there are constraints with the same property but different object. By default, sheXer groups those constraint in a isngle one having the less general object possible. For instance, when the objects are different shapes, it merges the constraints a single one whose object is IRI.
+* allow_redundant_or (default False): when this is set to True, the example described for the disable_or_statements behaves differently. Let's say we have a set of candidate constraints whose property is the same but whose object differs: one have IRI, and two other have different shape labels (:A and :B). Whith allow_redundant_or=False, sheXer generates a single constraint with IRI and moves the information about the rest of discarded constraints with more specific objects to comments. However, with allow_redundant_or=True, the constraint generated will have a node constraint with a disjunction such as IRI OR @A OR @B. From the point of view of validation, as IRI subsumes :A and :B, this has no effect. However, some user whose extracted shapes are used to generate further products find this feature useful.   
 * allow_opt_cardinality (default True). When all-compliant mode is active, if there is a constraint which does not conform with every isntance but its maximun cardinality for any instance is {1}, it uses the optional cardinality (?). When set to False, it uses Kleene closure instead.
 * disable_opt_cardinality (dafault False). When set to True, it prevents any constraint to have a higher cardinality higher than one, even if every instance has that cardinality. For example, a constraint such as *ex:alias xsd:string {3}* will be changed to *ex:alias xsd:string +*.
 * shape_qualifiers_mode (default False). When it is set to True, it assumes a data model similar to Wikidata's one, where entity nodes are linked with qualifiers (BNodes) instead of the actual object meant by the triple. It is used to produce legible shapes for those special BNodes.
 * namespaces_for_qualifier_props (default None). Provide here a list of namespace in which the indirect properties used to link an entity with a qualifier node can be found. A reasonable configuration for Wikidata is namespaces_for_qualifier_props = \["http://www.wikidata.org/prop/"\] .
 * inverse_paths (default False). When it is set to True, sheXer will produce constraints with inverse_paths too. This is, constraints referring to triples in which the target node acst as object. Direct and inverse paths will be sorted in the final results w.r.t. their trutsworthiness score.
 * detect_minimal_iri (default False). When it is set to True, each shape will be associated with a regex pattern. That pattern expresses the initial part of the IRI that is common to every isntance used to extract a given shape. This pattern is only serialized when it is a "worthy" one (long enough, not just "http://", etc.).
```

### Comparing `shexer-2.1.2/setup.py` & `shexer-2.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def read(file_path):
 	with open(file_path, "r") as in_stream:
 		return in_stream.read()
 
 setup(
   name = 'shexer',
   packages = find_packages(exclude=["*.local_code.*"]), # this must be the same as the name above
-  version = '2.1.2',
+  version = '2.1.3',
   description = 'Automatic schema extraction for RDF graphs',
   author = 'Daniel Fernandez-Alvarez',
   author_email = 'danifdezalvarez@gmail.com',
   url = 'https://github.com/DaniFdezAlvarez/shexer',
-  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.1.2.tar.gz',
+  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.1.3.tar.gz',
   keywords = ['testing', 'shexer', 'shexerp3', "rdf", "shex", "shacl", "schema"],
   long_description = read('README.md'),
   long_description_content_type='text/markdown',
   classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `shexer-2.1.2/shexer/consts.py` & `shexer-2.1.3/shexer/consts.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/abstract_instance_tracker.py` & `shexer-2.1.3/shexer/core/instances/abstract_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/annotators/annotator_tracking_instances.py` & `shexer-2.1.3/shexer/core/instances/annotators/annotator_tracking_instances.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/annotators/base_annotator.py` & `shexer-2.1.3/shexer/core/instances/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py` & `shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py` & `shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py` & `shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py` & `shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py` & `shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/instance_tracker.py` & `shexer-2.1.3/shexer/core/instances/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/mappings/shape_map_instance_tracker.py` & `shexer-2.1.3/shexer/core/instances/mappings/shape_map_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/instances/mix/mixed_instance_tracker.py` & `shexer-2.1.3/shexer/core/instances/mix/mixed_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/profiling/class_profiler.py` & `shexer-2.1.3/shexer/core/profiling/class_profiler.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py` & `shexer-2.1.3/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/profiling/strategy/direct_features_strategy.py` & `shexer-2.1.3/shexer/core/profiling/strategy/direct_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/profiling/strategy/include_reverse_features_strategy.py` & `shexer-2.1.3/shexer/core/profiling/strategy/include_reverse_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/shexing/class_shexer.py` & `shexer-2.1.3/shexer/core/shexing/class_shexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                  remove_empty_shapes=True, original_target_classes=None, original_shape_map=None,
                  discard_useless_constraints_with_positive_closure=True, keep_less_specific=True,
                  all_compliant_mode=True, instantiation_property=RDF_TYPE, disable_or_statements=True,
                  disable_comments=False, namespaces_dict=None, tolerance_to_keep_similar_rules=0,
                  allow_opt_cardinality=True, disable_exact_cardinality=False,
                  shapes_namespace=SHAPES_DEFAULT_NAMESPACE, inverse_paths=False,
                  decimals=-1, instances_report_mode=RATIO_INSTANCES, detect_minimal_iri=False,
-                 class_min_iris_dict=None):
+                 class_min_iris_dict=None, allow_redundant_or=False):
         self._class_counts_dict = class_counts_dict
         self._class_profile_dict = class_profile_dict if class_profile_dict is not None else self._load_class_profile_dict_from_file(
             class_profile_json_file)
         self._class_min_iris_dict = class_min_iris_dict
 
         self._shapes_list = []
         self._remove_empty_shapes = remove_empty_shapes
@@ -36,14 +36,15 @@
         self._tolerance = tolerance_to_keep_similar_rules
         self._allow_opt_cardinality = allow_opt_cardinality
         self._disable_exact_cardinality = disable_exact_cardinality
         self._shapes_namespace = shapes_namespace
         self._decimals = decimals
         self._instances_report_mode = instances_report_mode
         self._detect_minimal_iri = detect_minimal_iri
+        self._allow_redundant_or = allow_redundant_or
 
         self._original_target_nodes = determine_original_target_nodes_if_needed(remove_empty_shapes=remove_empty_shapes,
                                                                                 original_target_classes=original_target_classes,
                                                                                 original_shape_map=original_shape_map,
                                                                                 shapes_namespace=shapes_namespace)
         self._strategy = DirectShexingStrategy(self) if not inverse_paths \
             else DirectAndInverseShexingStrategy(self)
```

### Comparing `shexer-2.1.2/shexer/core/shexing/strategy/abstract_shexing_strategy.py` & `shexer-2.1.3/shexer/core/shexing/strategy/abstract_shexing_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self._instantiation_property_str = self._class_shexer._instantiation_property_str
         self._keep_less_specific = self._class_shexer._keep_less_specific
         self._discard_useless_positive_closures = self._class_shexer._discard_useless_positive_closures
         self._tolerance = self._class_shexer._tolerance
         self._disable_or_statements = self._class_shexer._disable_or_statements
         self._all_compliant_mode = self._class_shexer._all_compliant_mode
         self._disable_exact_cardinality = self._class_shexer._disable_exact_cardinality
+        self._allow_redundant_or = self._class_shexer._allow_redundant_or
 
         self._strategy_min_iri = AnnotateMinIriStrategy(class_shexer._class_min_iris_dict) \
             if class_shexer._detect_minimal_iri \
             else IgnoreMinIriStrategy()
 
         self._statement_serializer_factory = StSerializerFactory(freq_mode=class_shexer._instances_report_mode,
                                                                  decimals=class_shexer._decimals,
@@ -199,15 +200,16 @@
                     for j in range(i + 1, len(candidate_statements)):
                         if self._statements_have_same_prop(a_statement,
                                                            candidate_statements[j]):
                             group_to_decide.append(candidate_statements[j])
                             already_visited.add(candidate_statements[j])
                     if len(group_to_decide) == 1:
                         result.append(a_statement)
-                    else:
+                    else:  # At this point, group_to_decide may contain a list of constraints with the same property and
+                           # different node constraint
                         if self._disable_or_statements:
                             for a_sentence in self._manage_group_to_decide_without_or(group_to_decide):
                                 result.append(a_sentence)
                         else:
                             for a_sentence in self._manage_group_to_decide_with_or(group_to_decide):
                                 result.append(a_sentence)
 
@@ -292,15 +294,15 @@
                 to_compose.append(a_statement)
             else:
                 result.append(a_statement)
         to_compose.sort(reverse=True, key=lambda x: x.probability)
         # target_probability = self._get_probability_of_IRI_statement_in_group(to_compose)
         iri_statement = self._get_IRI_statement_in_group(to_compose)
         was_removed_IRI = self._remove_IRI_statements_if_useles(to_compose)
-        if not was_removed_IRI:  # The IRI macro is still there
+        if not was_removed_IRI and not self._allow_redundant_or:  # The IRI macro is still there
             return [a_sentence for a_sentence in self._manage_group_to_decide_without_or(to_compose)] + result
         elif len(to_compose) > 1:  # There are some sentences to join in an OR and no IRI macro
             composed_statement = FixedPropChoiceStatement(
                 st_property=to_compose[0].st_property,
                 st_types=[a_statement.st_type for a_statement in to_compose],
                 cardinality=POSITIVE_CLOSURE,
                 probability=iri_statement.probability,
```

### Comparing `shexer-2.1.2/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py` & `shexer-2.1.3/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/shexing/strategy/direct_shexing_strategy.py` & `shexer-2.1.3/shexer/core/shexing/strategy/direct_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py` & `shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/base_triples_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/big_ttl_triples_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/big_ttl_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/multi_nt_triples_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/multi_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/multifile_base_triples_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/multifile_base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/nt_triples_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/rdflib_triple_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/graph/yielder/tsv_nt_triples_yielder.py` & `shexer-2.1.3/shexer/io/graph/yielder/tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shacl/formater/shacl_serializer.py` & `shexer-2.1.3/shexer/io/shacl/formater/shacl_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shape_map/label/shape_map_label_parser.py` & `shexer-2.1.3/shexer/io/shape_map/label/shape_map_label_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shape_map/node_selector/node_selector_parser.py` & `shexer-2.1.3/shexer/io/shape_map/node_selector/node_selector_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shape_map/shape_map_parser.py` & `shexer-2.1.3/shexer/io/shape_map/shape_map_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shex/formater/shex_serializer.py` & `shexer-2.1.3/shexer/io/shex/formater/shex_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py` & `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py` & `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py` & `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py` & `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py` & `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py` & `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/io/sparql/query.py` & `shexer-2.1.3/shexer/io/sparql/query.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/IRI.py` & `shexer-2.1.3/shexer/model/IRI.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/Macro.py` & `shexer-2.1.3/shexer/model/Macro.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/fixed_prop_choice_statement.py` & `shexer-2.1.3/shexer/model/fixed_prop_choice_statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/graph/abstract_sgraph.py` & `shexer-2.1.3/shexer/model/graph/abstract_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/graph/endpoint_sgraph.py` & `shexer-2.1.3/shexer/model/graph/endpoint_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/graph/rdflib_sgraph.py` & `shexer-2.1.3/shexer/model/graph/rdflib_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/hierarchy_tree.py` & `shexer-2.1.3/shexer/model/hierarchy_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/node_selector.py` & `shexer-2.1.3/shexer/model/node_selector.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/shape.py` & `shexer-2.1.3/shexer/model/shape.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/shape_map.py` & `shexer-2.1.3/shexer/model/shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/model/statement.py` & `shexer-2.1.3/shexer/model/statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/shaper.py` & `shexer-2.1.3/shexer/shaper.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
                  limit_remote_instances=-1,
                  wikidata_annotation=False,
                  inverse_paths=False,
                  compression_mode=None,
                  decimals=-1,
                  instances_report_mode=RATIO_INSTANCES,
                  disable_endpoint_cache=False,
-                 detect_minimal_iri=False
+                 detect_minimal_iri=False,
+                 allow_redundant_or=False
                  ):
         """
 
         :param target_classes:
         :param file_target_classes:
         :param input_format:
         :param instances_file_input:
@@ -98,14 +99,15 @@
         :param wikidata_annotation:
         :param inverse_paths:
         :param compression_mode:
         :param decimals:
         :param instances_report_mode:
         :param disable_endpoint_cache:
         :param detect_minimal_iri:
+        :param allow_redundant_or:
         """
 
         check_just_one_not_none((graph_file_input, "graph_file_input"),
                                 (graph_list_of_files_input, "graph_list_of_files_input"),
                                 (raw_graph, "raw_graph"),
                                 (url_graph_input, "url_input"),
                                 (list_of_url_input, "list_of_url_input"),
@@ -118,14 +120,17 @@
 
         self._check_target_classes(target_classes=target_classes,
                                    file_target_classes=file_target_classes,
                                    all_classes_mode=all_classes_mode,
                                    shape_map_raw=shape_map_raw,
                                    shape_map_file=shape_map_file)
 
+        self._check_or_config(or_disabled=disable_or_statements,
+                              enable_redundant=allow_redundant_or)
+
         #TODO ---> Param check of shape_map and graph_via_shape_map
 
         self._check_input_format(input_format)
 
         self._check_compression_mode(compression_mode, url_endpoint, url_graph_input, list_of_url_input)
 
         self._target_classes = target_classes
@@ -146,15 +151,16 @@
         self._keep_less_specific = keep_less_specific
         self._raw_graph = raw_graph
         self._all_classes_mode = all_classes_mode
         self._shape_map_file = shape_map_file
         self._shape_map_raw = shape_map_raw
         self._decimals = decimals
         self._instances_report_mode = instances_report_mode
-        self._disable_endpoint_cache=False
+        self._disable_endpoint_cache=disable_endpoint_cache
+        self._allow_redundant_or = allow_redundant_or
 
         self._remove_empty_shapes=remove_empty_shapes
         self._disable_comments = disable_comments
         self._disable_or_statements = disable_or_statements
         self._allow_opt_cardinality = allow_opt_cardinality
         self._disable_exact_cardinality = disable_exact_cardinality
         self._limit_remote_instances = limit_remote_instances
@@ -285,15 +291,16 @@
                                 allow_opt_cardinality=self._allow_opt_cardinality,
                                 disable_exact_cardinality=self._disable_exact_cardinality,
                                 shapes_namespace=self._shapes_namespace,
                                 inverse_paths=self._inverse_paths,
                                 decimals=self._decimals,
                                 instances_report_mode=self._instances_report_mode,
                                 detect_minimal_iri=self._detect_minimal_iri,
-                                class_min_iris=self._class_min_iris
+                                class_min_iris=self._class_min_iris,
+                                allow_redundant_or=self._allow_redundant_or
                                 )
 
     def _build_shapes_serializer(self, target_file, string_return, output_format):
         return get_shape_serializer(shapes_list=self._shape_list,
                                     target_file=target_file,
                                     string_return=string_return,
                                     namespaces_dict=self._namespaces_dict,
@@ -408,10 +415,17 @@
 
     @staticmethod
     def _check_output_format(output_format):
         if output_format not in [SHEXC, SHACL_TURTLE]:
             raise ValueError("Currently unsupported output format: " + output_format)
 
     @staticmethod
+    def _check_or_config(or_disabled, enable_redundant):
+        if or_disabled and enable_redundant:
+            raise ValueError("You are indicating that you'd like to have disjunction constraints including the macro "
+                             "IRI, but also that you do not want to have or constraints. Please, check your configuration"
+                             "of the disable_or_statements and allow_redundant_or paremeters")
+
+    @staticmethod
     def _check_aceptance_threshold(aceptance_threshold):
         if aceptance_threshold < 0 or aceptance_threshold > 1:
             raise ValueError("The acceptance threshold must be a value in [0,1]")
```

### Comparing `shexer-2.1.2/shexer/utils/compression.py` & `shexer-2.1.3/shexer/utils/compression.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/factories/class_profiler_factory.py` & `shexer-2.1.3/shexer/utils/factories/class_profiler_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/factories/class_shexer_factory.py` & `shexer-2.1.3/shexer/utils/factories/class_shexer_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,16 @@
                      allow_opt_cardinality=True,
                      disable_exact_cardinality=False,
                      shapes_namespace=SHAPES_DEFAULT_NAMESPACE,
                      inverse_paths=False,
                      decimals=-1,
                      instances_report_mode=RATIO_INSTANCES,
                      detect_minimal_iri=False,
-                     class_min_iris=None):
+                     class_min_iris=None,
+                     allow_redundant_or=False):
 
     return ClassShexer(
         class_counts_dict=class_counts,
         class_profile_dict=class_profile_dict,
         class_profile_json_file=None,
         remove_empty_shapes=remove_empty_shapes,
         original_target_classes=original_target_classes,
@@ -40,9 +41,10 @@
         allow_opt_cardinality=allow_opt_cardinality,
         disable_exact_cardinality=disable_exact_cardinality,
         shapes_namespace=shapes_namespace,
         inverse_paths=inverse_paths,
         instances_report_mode=instances_report_mode,
         decimals=decimals,
         detect_minimal_iri=detect_minimal_iri,
-        class_min_iris_dict=class_min_iris
+        class_min_iris_dict=class_min_iris,
+        allow_redundant_or=allow_redundant_or
     )
```

### Comparing `shexer-2.1.2/shexer/utils/factories/h_tree.py` & `shexer-2.1.3/shexer/utils/factories/h_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/factories/instance_tracker_factory.py` & `shexer-2.1.3/shexer/utils/factories/instance_tracker_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/factories/shape_map_factory.py` & `shexer-2.1.3/shexer/utils/factories/shape_map_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/factories/shape_map_parser_factory.py` & `shexer-2.1.3/shexer/utils/factories/shape_map_parser_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/factories/shape_serializer_factory.py` & `shexer-2.1.3/shexer/utils/factories/shape_serializer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/factories/triple_yielders_factory.py` & `shexer-2.1.3/shexer/utils/factories/triple_yielders_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/namespaces.py` & `shexer-2.1.3/shexer/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/obj_references.py` & `shexer-2.1.3/shexer/utils/obj_references.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/shapes.py` & `shexer-2.1.3/shexer/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/target_elements.py` & `shexer-2.1.3/shexer/utils/target_elements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/translators/list_of_classes_to_shape_map.py` & `shexer-2.1.3/shexer/utils/translators/list_of_classes_to_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/triple_yielders.py` & `shexer-2.1.3/shexer/utils/triple_yielders.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer/utils/uri.py` & `shexer-2.1.3/shexer/utils/uri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/shexer.egg-info/PKG-INFO` & `shexer-2.1.3/shexer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.1.2
+Version: 2.1.3
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.2.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.3.tar.gz
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -215,14 +215,15 @@
 * instantiation_property (default rdf:type): full URI (no prefixes) of the property linking instances and classes (ex: P31 in Wikidata's ontology)
 * namespaces_to_ignore (default None): list of namespaces of properties used in the target graph which are going to be ignored. For example, if you set namespaces_to_ignore to \[http://example.org/\], every triple whose predicate belongs to that namespace will not be computed. It just excludes properties whose name is a direct child of the namespace. For example, triples with <http:/example.org/foo> will be ignored, but triples with <http://example.org/anotherLevel/foo> will be computed.
 * infer_numeric_types_for_untyped_literals (default False): when it is set to True, if the parser finds a triple whose object in a number untyped (something like 56 instead of "56"^^xsd:int), it will accept it and consider it an int if it has decimals or a float if it does not. If it is set to False, triples like that will raise a parsing error.
 * discard_useles_constraints_with_positive_closure (default True): if it is set to True, when two constraints have been extracted with identical property and object, and one of them has '+' cardinality while the other one has a specific number of occurrences (example: {1}, {2}...), if they both have the same rate of compliance among the instances, the constraint with the '+' cardinality is discarded.
 * all_instances_are_compliant_mode (default True): when set to True, every inferred constraint which is not valid for all the instances of the class associated to the shape, then the cardinality of that constraint is changed to '\*' or '?'. With this, every instance conforms to the shape associated with its class. When it is set to False, no cardinality is changed, so there may be instances that do not conform to the inferred shape.
 * keep_less_specific (default True): when it is set to True, for a group of constraints with the same property and object but different cardinality, the one with less specific cardinality ('+') will be preserved, and the rest of constraints used to provide info in comments. When it is set to False, the preserved constraint will be the one with an integer as cardinality and the highest rate of conformance with the instances of the class.
 * disable_or_statements (default True): when set to False, sheXer tries to infer constraints with the operator oneOf (|) in case there are constraints with the same property but different object. By default, sheXer groups those constraint in a isngle one having the less general object possible. For instance, when the objects are different shapes, it merges the constraints a single one whose object is IRI.
+* allow_redundant_or (default False): when this is set to True, the example described for the disable_or_statements behaves differently. Let's say we have a set of candidate constraints whose property is the same but whose object differs: one have IRI, and two other have different shape labels (:A and :B). Whith allow_redundant_or=False, sheXer generates a single constraint with IRI and moves the information about the rest of discarded constraints with more specific objects to comments. However, with allow_redundant_or=True, the constraint generated will have a node constraint with a disjunction such as IRI OR @A OR @B. From the point of view of validation, as IRI subsumes :A and :B, this has no effect. However, some user whose extracted shapes are used to generate further products find this feature useful.   
 * allow_opt_cardinality (default True). When all-compliant mode is active, if there is a constraint which does not conform with every isntance but its maximun cardinality for any instance is {1}, it uses the optional cardinality (?). When set to False, it uses Kleene closure instead.
 * disable_opt_cardinality (dafault False). When set to True, it prevents any constraint to have a higher cardinality higher than one, even if every instance has that cardinality. For example, a constraint such as *ex:alias xsd:string {3}* will be changed to *ex:alias xsd:string +*.
 * shape_qualifiers_mode (default False). When it is set to True, it assumes a data model similar to Wikidata's one, where entity nodes are linked with qualifiers (BNodes) instead of the actual object meant by the triple. It is used to produce legible shapes for those special BNodes.
 * namespaces_for_qualifier_props (default None). Provide here a list of namespace in which the indirect properties used to link an entity with a qualifier node can be found. A reasonable configuration for Wikidata is namespaces_for_qualifier_props = \["http://www.wikidata.org/prop/"\] .
 * inverse_paths (default False). When it is set to True, sheXer will produce constraints with inverse_paths too. This is, constraints referring to triples in which the target node acst as object. Direct and inverse paths will be sorted in the final results w.r.t. their trutsworthiness score.
 * detect_minimal_iri (default False). When it is set to True, each shape will be associated with a regex pattern. That pattern expresses the initial part of the IRI that is common to every isntance used to extract a given shape. This pattern is only serialized when it is a "worthy" one (long enough, not just "http://", etc.).
```

### Comparing `shexer-2.1.2/shexer.egg-info/SOURCES.txt` & `shexer-2.1.3/shexer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 shexer/utils/translators/__init__.py
 shexer/utils/translators/list_of_classes_to_shape_map.py
 test/__init__.py
 test/const.py
 test/t_utils.py
 test/test_all_classes_mode.py
 test/test_allow_opt_cardinality.py
+test/test_allow_redundant_or.py
 test/test_compression_mode.py
 test/test_decimals.py
 test/test_depth_for_building_subgraph.py
 test/test_detect_minimal_iri.py
 test/test_disable_comments.py
 test/test_disable_endpoint_cache.py
 test/test_disable_exact_cardinality.py
```

### Comparing `shexer-2.1.2/test/const.py` & `shexer-2.1.3/test/const.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/t_utils.py` & `shexer-2.1.3/test/t_utils.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_all_classes_mode.py` & `shexer-2.1.3/test/test_all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_allow_opt_cardinality.py` & `shexer-2.1.3/test/test_allow_opt_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_bugs/test_no_sharp_in_auto_shape_names.py` & `shexer-2.1.3/test/test_bugs/test_no_sharp_in_auto_shape_names.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py` & `shexer-2.1.3/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_compression_mode.py` & `shexer-2.1.3/test/test_compression_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_decimals.py` & `shexer-2.1.3/test/test_decimals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_depth_for_building_subgraph.py` & `shexer-2.1.3/test/test_depth_for_building_subgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_detect_minimal_iri.py` & `shexer-2.1.3/test/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_disable_comments.py` & `shexer-2.1.3/test/test_disable_comments.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_disable_endpoint_cache.py` & `shexer-2.1.3/test/test_disable_endpoint_cache.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_disable_exact_cardinality.py` & `shexer-2.1.3/test/test_disable_exact_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_disable_or_statements.py` & `shexer-2.1.3/test/test_disable_or_statements.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from test.const import BASE_FILES, default_namespaces
 from test.t_utils import file_vs_str_tunned_comparison
 import os.path as pth
 from shexer.consts import TURTLE
 
 _BASE_DIR = BASE_FILES + "disable_or" + pth.sep
 
-class TestGraphFileInput(unittest.TestCase):
+class TestDisableOrStatements(unittest.TestCase):
 
     def test_or_enabled_choice_useful_IRI(self):
         shaper = Shaper(graph_file_input=_BASE_DIR + "g3_or_example.ttl",
                         namespaces_dict=default_namespaces(),
                         all_classes_mode=True,
                         input_format=TURTLE,
                         disable_comments=True,
```

### Comparing `shexer-2.1.2/test/test_discard_and_compliant.py` & `shexer-2.1.3/test/test_discard_and_compliant.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_file_target_classes.py` & `shexer-2.1.3/test/test_file_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_graph_file_input.py` & `shexer-2.1.3/test/test_graph_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_graph_list_of_file_inputs.py` & `shexer-2.1.3/test/test_graph_list_of_file_inputs.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_infer_numeric_types_for_untyped_literals.py` & `shexer-2.1.3/test/test_infer_numeric_types_for_untyped_literals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_input_format.py` & `shexer-2.1.3/test/test_input_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_instances_file_input.py` & `shexer-2.1.3/test/test_instances_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_instances_report.py` & `shexer-2.1.3/test/test_instances_report.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_instantiation_property.py` & `shexer-2.1.3/test/test_instantiation_property.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_inverse_paths.py` & `shexer-2.1.3/test/test_inverse_paths.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_keep_less_specific.py` & `shexer-2.1.3/test/test_keep_less_specific.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_list_of_url_input.py` & `shexer-2.1.3/test/test_list_of_url_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_namespaces_dict.py` & `shexer-2.1.3/test/test_namespaces_dict.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_namespaces_to_ignore.py` & `shexer-2.1.3/test/test_namespaces_to_ignore.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_raw_graph.py` & `shexer-2.1.3/test/test_raw_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_raw_shape_map.py` & `shexer-2.1.3/test/test_raw_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_rdflib_graph.py` & `shexer-2.1.3/test/test_rdflib_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_remove_empty_sahpes.py` & `shexer-2.1.3/test/test_remove_empty_sahpes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_shacl/test_annotation.py` & `shexer-2.1.3/test/test_shacl/test_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_shacl/test_class_selection.py` & `shexer-2.1.3/test/test_shacl/test_class_selection.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_shacl/test_detect_minimal_iri.py` & `shexer-2.1.3/test/test_shacl/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_shacl/test_literal_types.py` & `shexer-2.1.3/test/test_shacl/test_literal_types.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_shape_map_file.py` & `shexer-2.1.3/test/test_shape_map_file.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_shape_map_format.py` & `shexer-2.1.3/test/test_shape_map_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_shape_qualifiers_mode.py` & `shexer-2.1.3/test/test_shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_shapes_namespaces.py` & `shexer-2.1.3/test/test_shapes_namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_sort.py` & `shexer-2.1.3/test/test_sort.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_target_classes.py` & `shexer-2.1.3/test/test_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_threshold.py` & `shexer-2.1.3/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_url_endpoint.py` & `shexer-2.1.3/test/test_url_endpoint.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_url_graph.py` & `shexer-2.1.3/test/test_url_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/test/test_wikidata_annotation.py` & `shexer-2.1.3/test/test_wikidata_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.2/ws/shexer_rest.py` & `shexer-2.1.3/ws/shexer_rest.py`

 * *Files identical despite different names*

