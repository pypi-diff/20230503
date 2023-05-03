# Comparing `tmp/curator-opensearch-0.0.7.tar.gz` & `tmp/curator-opensearch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curator-opensearch-0.0.7.tar", last modified: Thu Nov 10 11:44:06 2022, max compression
+gzip compressed data, was "curator-opensearch-0.0.9.tar", last modified: Fri Nov 25 13:31:38 2022, max compression
```

## Comparing `curator-opensearch-0.0.7.tar` & `curator-opensearch-0.0.9.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.646526 curator-opensearch-0.0.7/
--rw-rw-r--   0 boris     (1000) boris     (1000)     3790 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/CONTRIBUTING.md
--rw-rw-r--   0 boris     (1000) boris     (1000)     2338 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/CONTRIBUTORS
--rw-rw-r--   0 boris     (1000) boris     (1000)      832 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/Dockerfile
--rw-rw-r--   0 boris     (1000) boris     (1000)      598 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/LICENSE.txt
--rw-rw-r--   0 boris     (1000) boris     (1000)      484 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/MANIFEST.in
--rw-rw-r--   0 boris     (1000) boris     (1000)     4340 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/NOTICE
--rw-rw-r--   0 boris     (1000) boris     (1000)     3950 2022-11-10 11:44:06.646526 curator-opensearch-0.0.7/PKG-INFO
--rw-rw-r--   0 boris     (1000) boris     (1000)     3115 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/README.rst
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.626526 curator-opensearch-0.0.7/curator/
--rw-rw-r--   0 boris     (1000) boris     (1000)      396 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/__init__.py
--rw-rw-r--   0 boris     (1000) boris     (1000)       44 2022-11-10 10:43:55.000000 curator-opensearch-0.0.7/curator/_version.py
--rw-rw-r--   0 boris     (1000) boris     (1000)   108482 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/actions.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    10319 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli.py
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.630526 curator-opensearch-0.0.7/curator/cli_singletons/
--rw-rw-r--   0 boris     (1000) boris     (1000)        0 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/__init__.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1857 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/alias.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2268 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/allocation.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1467 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/close.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2719 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/delete.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1567 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/forcemerge.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1162 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/freeze.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     8944 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/object_class.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1186 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/open_indices.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1540 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/replicas.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     3822 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/restore.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2076 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/rollover.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     4454 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/show.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     4087 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/shrink.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2866 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/snapshot.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1168 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/unfreeze.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     5751 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/cli_singletons/utils.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2435 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/config_utils.py
--rwxrwxr-x   0 boris     (1000) boris     (1000)      298 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/curator_cli.py
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.630526 curator-opensearch-0.0.7/curator/defaults/
--rw-rw-r--   0 boris     (1000) boris     (1000)        0 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/defaults/__init__.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2368 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/defaults/client_defaults.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     7412 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/defaults/filter_elements.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     4816 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/defaults/filtertypes.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    11183 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/defaults/option_defaults.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     5275 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/defaults/settings.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1888 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/exceptions.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    60599 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/indexlist.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     4583 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/logtools.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     5437 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/repomgrcli.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     4134 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/singletons.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    23629 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/snapshotlist.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    85075 2022-11-10 10:42:06.000000 curator-opensearch-0.0.7/curator/utils.py
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.630526 curator-opensearch-0.0.7/curator/validators/
--rw-rw-r--   0 boris     (1000) boris     (1000)       55 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/validators/__init__.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1802 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/validators/actions.py
--rw-rw-r--   0 boris     (1000) boris     (1000)      277 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/validators/config_file.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1769 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/validators/filters.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     5935 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/validators/options.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2675 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/curator/validators/schemacheck.py
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.634526 curator-opensearch-0.0.7/curator_opensearch.egg-info/
--rw-rw-r--   0 boris     (1000) boris     (1000)     3950 2022-11-10 11:44:06.000000 curator-opensearch-0.0.7/curator_opensearch.egg-info/PKG-INFO
--rw-rw-r--   0 boris     (1000) boris     (1000)     4215 2022-11-10 11:44:06.000000 curator-opensearch-0.0.7/curator_opensearch.egg-info/SOURCES.txt
--rw-rw-r--   0 boris     (1000) boris     (1000)        1 2022-11-10 11:44:06.000000 curator-opensearch-0.0.7/curator_opensearch.egg-info/dependency_links.txt
--rw-rw-r--   0 boris     (1000) boris     (1000)      129 2022-11-10 11:44:06.000000 curator-opensearch-0.0.7/curator_opensearch.egg-info/entry_points.txt
--rw-rw-r--   0 boris     (1000) boris     (1000)      177 2022-11-10 11:44:06.000000 curator-opensearch-0.0.7/curator_opensearch.egg-info/requires.txt
--rw-rw-r--   0 boris     (1000) boris     (1000)        8 2022-11-10 11:44:06.000000 curator-opensearch-0.0.7/curator_opensearch.egg-info/top_level.txt
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.634526 curator-opensearch-0.0.7/docs/
--rw-rw-r--   0 boris     (1000) boris     (1000)    85455 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/Changelog.rst
--rw-rw-r--   0 boris     (1000) boris     (1000)     6790 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/Makefile
--rw-rw-r--   0 boris     (1000) boris     (1000)     1672 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/actionclasses.rst
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.638526 curator-opensearch-0.0.7/docs/asciidoc/
--rw-rw-r--   0 boris     (1000) boris     (1000)     5375 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/about.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)    36639 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/actions.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     8292 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/command-line.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)    16941 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/configuration.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)    22303 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/examples.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     8861 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/faq.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)    28009 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/filter_elements.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)    30139 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/filters.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     3186 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/ilm.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     1044 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/inc_datemath.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)      451 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/inc_filepath.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)      653 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/inc_filter_by_aliases.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)      972 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/inc_filter_chaining.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     1690 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/inc_kinds.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     1510 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/inc_sources.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)      505 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/inc_strftime_table.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     1355 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/inc_timestring_regex.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)      428 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/inc_unit_table.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)      932 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/index.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)    13176 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/installation.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)    84563 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/options.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     4782 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/security.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     1713 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/asciidoc/versions.asciidoc
--rw-rw-r--   0 boris     (1000) boris     (1000)     8959 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/conf.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2303 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/examples.rst
--rw-rw-r--   0 boris     (1000) boris     (1000)     1470 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/filters.rst
--rw-rw-r--   0 boris     (1000) boris     (1000)     3060 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/index.rst
--rw-rw-r--   0 boris     (1000) boris     (1000)      253 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/objectclasses.rst
--rw-rw-r--   0 boris     (1000) boris     (1000)      159 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/docs/utilities.rst
--rw-rw-r--   0 boris     (1000) boris     (1000)     1504 2022-11-10 11:44:06.646526 curator-opensearch-0.0.7/setup.cfg
--rw-rw-r--   0 boris     (1000) boris     (1000)     6224 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/setup.py
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.638526 curator-opensearch-0.0.7/test/
--rw-rw-r--   0 boris     (1000) boris     (1000)        0 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/__init__.py
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.642526 curator-opensearch-0.0.7/test/integration/
--rw-rw-r--   0 boris     (1000) boris     (1000)     7329 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/__init__.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    15915 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_alias.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    11924 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_allocation.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     9493 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_cli.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    12235 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_close.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1882 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_clusterrouting.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     5208 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_count_pattern.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     5585 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_create_index.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1638 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_datemath.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    24196 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_delete_indices.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     6335 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_delete_snapshots.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2924 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_envvars.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     5282 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_es_repo_mgr.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     3702 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_forcemerge.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     7424 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_freeze.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     4603 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_integrations.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     3290 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_open.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    18351 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_reindex.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     3071 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_replicas.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     7917 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_restore.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    16141 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_rollover.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    11340 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_shrink.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     6261 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_snapshot.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     5695 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/test_unfreeze.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    22373 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/integration/testvars.py
--rwxrwxr-x   0 boris     (1000) boris     (1000)      724 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/run_tests.py
-drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-10 11:44:06.646526 curator-opensearch-0.0.7/test/unit/
--rw-rw-r--   0 boris     (1000) boris     (1000)     1632 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/__init__.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     6962 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_alias.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     5334 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_allocation.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     4459 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_close.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2421 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_clusterrouting.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     1314 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_create_index.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     3926 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_delete_indices.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2708 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_delete_snapshots.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     4908 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_forcemerge.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     7297 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_indexsettings.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2555 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_open.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    10848 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_reindex.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     3666 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_replicas.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     8277 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_restore.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2438 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_rollover.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    10968 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_shrink.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    10417 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_action_snapshot.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    64235 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_class_index_list.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    24100 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_class_snapshot_list.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     2622 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_cli_methods.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    68556 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_utils.py
--rw-rw-r--   0 boris     (1000) boris     (1000)     7118 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/test_validators.py
--rw-rw-r--   0 boris     (1000) boris     (1000)    46149 2022-11-10 09:44:11.000000 curator-opensearch-0.0.7/test/unit/testvars.py
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.997720 curator-opensearch-0.0.9/
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3790 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/CONTRIBUTING.md
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2338 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/CONTRIBUTORS
+-rw-rw-r--   0 boris     (1000) boris     (1000)      832 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/Dockerfile
+-rw-rw-r--   0 boris     (1000) boris     (1000)      597 2022-11-10 19:36:50.000000 curator-opensearch-0.0.9/LICENSE
+-rw-rw-r--   0 boris     (1000) boris     (1000)      484 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/MANIFEST.in
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4340 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/NOTICE
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3946 2022-11-25 13:31:37.997720 curator-opensearch-0.0.9/PKG-INFO
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3115 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/README.rst
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.985720 curator-opensearch-0.0.9/curator/
+-rw-rw-r--   0 boris     (1000) boris     (1000)      396 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/__init__.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)       44 2022-11-25 13:31:17.000000 curator-opensearch-0.0.9/curator/_version.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)   108482 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/actions.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    10319 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli.py
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.989720 curator-opensearch-0.0.9/curator/cli_singletons/
+-rw-rw-r--   0 boris     (1000) boris     (1000)        0 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/__init__.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1857 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/alias.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2268 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/allocation.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1467 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/close.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2719 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/delete.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1567 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/forcemerge.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1162 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/freeze.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     8944 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/object_class.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1186 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/open_indices.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1540 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/replicas.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3822 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/restore.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2076 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/rollover.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4454 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/show.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4087 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/shrink.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2866 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/snapshot.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1168 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/unfreeze.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5751 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/cli_singletons/utils.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2435 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/config_utils.py
+-rwxrwxr-x   0 boris     (1000) boris     (1000)      298 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/curator_cli.py
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.989720 curator-opensearch-0.0.9/curator/defaults/
+-rw-rw-r--   0 boris     (1000) boris     (1000)        0 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/defaults/__init__.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2368 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/defaults/client_defaults.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     7412 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/defaults/filter_elements.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4816 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/defaults/filtertypes.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    11183 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/defaults/option_defaults.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5275 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/defaults/settings.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1888 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/exceptions.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    60599 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/indexlist.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4583 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/logtools.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5437 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/repomgrcli.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4134 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/singletons.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    23629 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/snapshotlist.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    85112 2022-11-25 13:26:18.000000 curator-opensearch-0.0.9/curator/utils.py
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.989720 curator-opensearch-0.0.9/curator/validators/
+-rw-rw-r--   0 boris     (1000) boris     (1000)       55 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/validators/__init__.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1802 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/validators/actions.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)      277 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/validators/config_file.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1769 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/validators/filters.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5935 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/validators/options.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2675 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/curator/validators/schemacheck.py
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.989720 curator-opensearch-0.0.9/curator_opensearch.egg-info/
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3946 2022-11-25 13:31:37.000000 curator-opensearch-0.0.9/curator_opensearch.egg-info/PKG-INFO
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4211 2022-11-25 13:31:37.000000 curator-opensearch-0.0.9/curator_opensearch.egg-info/SOURCES.txt
+-rw-rw-r--   0 boris     (1000) boris     (1000)        1 2022-11-25 13:31:37.000000 curator-opensearch-0.0.9/curator_opensearch.egg-info/dependency_links.txt
+-rw-rw-r--   0 boris     (1000) boris     (1000)      129 2022-11-25 13:31:37.000000 curator-opensearch-0.0.9/curator_opensearch.egg-info/entry_points.txt
+-rw-rw-r--   0 boris     (1000) boris     (1000)      177 2022-11-25 13:31:37.000000 curator-opensearch-0.0.9/curator_opensearch.egg-info/requires.txt
+-rw-rw-r--   0 boris     (1000) boris     (1000)        8 2022-11-25 13:31:37.000000 curator-opensearch-0.0.9/curator_opensearch.egg-info/top_level.txt
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.989720 curator-opensearch-0.0.9/docs/
+-rw-rw-r--   0 boris     (1000) boris     (1000)    85455 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/Changelog.rst
+-rw-rw-r--   0 boris     (1000) boris     (1000)     6790 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/Makefile
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1672 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/actionclasses.rst
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.993720 curator-opensearch-0.0.9/docs/asciidoc/
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5375 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/about.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)    36639 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/actions.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     8292 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/command-line.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)    16941 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/configuration.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)    22303 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/examples.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     8861 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/faq.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)    28009 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/filter_elements.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)    30139 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/filters.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3186 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/ilm.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1044 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/inc_datemath.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)      451 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/inc_filepath.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)      653 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/inc_filter_by_aliases.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)      972 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/inc_filter_chaining.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1690 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/inc_kinds.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1510 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/inc_sources.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)      505 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/inc_strftime_table.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1355 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/inc_timestring_regex.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)      428 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/inc_unit_table.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)      932 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/index.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)    13176 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/installation.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)    84563 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/options.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4782 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/security.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1713 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/asciidoc/versions.asciidoc
+-rw-rw-r--   0 boris     (1000) boris     (1000)     8959 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/conf.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2303 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/examples.rst
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1470 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/filters.rst
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3060 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/index.rst
+-rw-rw-r--   0 boris     (1000) boris     (1000)      253 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/objectclasses.rst
+-rw-rw-r--   0 boris     (1000) boris     (1000)      159 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/docs/utilities.rst
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1504 2022-11-25 13:31:38.001721 curator-opensearch-0.0.9/setup.cfg
+-rw-rw-r--   0 boris     (1000) boris     (1000)     6224 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/setup.py
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.993720 curator-opensearch-0.0.9/test/
+-rw-rw-r--   0 boris     (1000) boris     (1000)        0 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/__init__.py
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.997720 curator-opensearch-0.0.9/test/integration/
+-rw-rw-r--   0 boris     (1000) boris     (1000)     7329 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/__init__.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    15915 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_alias.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    11924 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_allocation.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     9493 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_cli.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    12235 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_close.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1882 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_clusterrouting.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5208 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_count_pattern.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5585 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_create_index.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1638 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_datemath.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    24196 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_delete_indices.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     6335 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_delete_snapshots.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2924 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_envvars.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5282 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_es_repo_mgr.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3702 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_forcemerge.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     7424 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_freeze.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4603 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_integrations.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3290 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_open.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    18351 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_reindex.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3071 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_replicas.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     7917 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_restore.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    16141 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_rollover.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    11340 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_shrink.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     6261 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_snapshot.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5695 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/test_unfreeze.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    22373 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/integration/testvars.py
+-rwxrwxr-x   0 boris     (1000) boris     (1000)      724 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/run_tests.py
+drwxrwxr-x   0 boris     (1000) boris     (1000)        0 2022-11-25 13:31:37.997720 curator-opensearch-0.0.9/test/unit/
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1632 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/__init__.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     6962 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_alias.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     5334 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_allocation.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4459 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_close.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2421 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_clusterrouting.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     1314 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_create_index.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3926 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_delete_indices.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2708 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_delete_snapshots.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     4908 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_forcemerge.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     7297 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_indexsettings.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2555 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_open.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    10848 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_reindex.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     3666 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_replicas.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     8277 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_restore.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2438 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_rollover.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    10968 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_shrink.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    10417 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_action_snapshot.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    64235 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_class_index_list.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    24100 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_class_snapshot_list.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     2622 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_cli_methods.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    68556 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_utils.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)     7118 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/test_validators.py
+-rw-rw-r--   0 boris     (1000) boris     (1000)    46149 2022-11-10 09:44:11.000000 curator-opensearch-0.0.9/test/unit/testvars.py
```

### Comparing `curator-opensearch-0.0.7/CONTRIBUTING.md` & `curator-opensearch-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/CONTRIBUTORS` & `curator-opensearch-0.0.9/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/Dockerfile` & `curator-opensearch-0.0.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/LICENSE.txt` & `curator-opensearch-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 
    http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
-limitations under the License.
+limitations under the License.
```

### Comparing `curator-opensearch-0.0.7/NOTICE` & `curator-opensearch-0.0.9/NOTICE`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/PKG-INFO` & `curator-opensearch-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: curator-opensearch
-Version: 0.0.7
+Version: 0.0.9
 Summary: Tending your Elasticsearch indices
 Home-page: https://github.com/uzhinskiy/curator-opensearch
-Download-URL: https://github.com/uzhinskiy/curator-opensearch/releases/tag/0.0.7
+Download-URL: https://github.com/uzhinskiy/curator-opensearch/releases/tag/0.0.9
 Author: Uzhinsky
 Author-email: lspci@mail.ru
 License: Apache License, Version 2.0
 Keywords: elasticsearch time-series indexed index-expiry
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE.txt
+License-File: LICENSE
 License-File: NOTICE
 
 .. _readme:
 
 
 Curator
 =======
```

### Comparing `curator-opensearch-0.0.7/README.rst` & `curator-opensearch-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/actions.py` & `curator-opensearch-0.0.9/curator/actions.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli.py` & `curator-opensearch-0.0.9/curator/cli.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/alias.py` & `curator-opensearch-0.0.9/curator/cli_singletons/alias.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/allocation.py` & `curator-opensearch-0.0.9/curator/cli_singletons/allocation.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/close.py` & `curator-opensearch-0.0.9/curator/cli_singletons/close.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/delete.py` & `curator-opensearch-0.0.9/curator/cli_singletons/delete.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/forcemerge.py` & `curator-opensearch-0.0.9/curator/cli_singletons/forcemerge.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/freeze.py` & `curator-opensearch-0.0.9/curator/cli_singletons/freeze.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/object_class.py` & `curator-opensearch-0.0.9/curator/cli_singletons/object_class.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/open_indices.py` & `curator-opensearch-0.0.9/curator/cli_singletons/open_indices.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/replicas.py` & `curator-opensearch-0.0.9/curator/cli_singletons/replicas.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/restore.py` & `curator-opensearch-0.0.9/curator/cli_singletons/restore.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/rollover.py` & `curator-opensearch-0.0.9/curator/cli_singletons/rollover.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/show.py` & `curator-opensearch-0.0.9/curator/cli_singletons/show.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/shrink.py` & `curator-opensearch-0.0.9/curator/cli_singletons/shrink.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/snapshot.py` & `curator-opensearch-0.0.9/curator/cli_singletons/snapshot.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/unfreeze.py` & `curator-opensearch-0.0.9/curator/cli_singletons/unfreeze.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/cli_singletons/utils.py` & `curator-opensearch-0.0.9/curator/cli_singletons/utils.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/config_utils.py` & `curator-opensearch-0.0.9/curator/config_utils.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/defaults/client_defaults.py` & `curator-opensearch-0.0.9/curator/defaults/client_defaults.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/defaults/filter_elements.py` & `curator-opensearch-0.0.9/curator/defaults/filter_elements.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/defaults/filtertypes.py` & `curator-opensearch-0.0.9/curator/defaults/filtertypes.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/defaults/option_defaults.py` & `curator-opensearch-0.0.9/curator/defaults/option_defaults.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/defaults/settings.py` & `curator-opensearch-0.0.9/curator/defaults/settings.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/exceptions.py` & `curator-opensearch-0.0.9/curator/exceptions.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/indexlist.py` & `curator-opensearch-0.0.9/curator/indexlist.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/logtools.py` & `curator-opensearch-0.0.9/curator/logtools.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/repomgrcli.py` & `curator-opensearch-0.0.9/curator/repomgrcli.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/singletons.py` & `curator-opensearch-0.0.9/curator/singletons.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/snapshotlist.py` & `curator-opensearch-0.0.9/curator/snapshotlist.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/utils.py` & `curator-opensearch-0.0.9/curator/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2124,11 +2124,11 @@
             if isinstance(value, dict):
                 iterdict(value)
             elif key == "http_auth":
                 if value is None:
                   mydict.update({"http_auth": None})
                 else: 
                   mydict.update({"http_auth": "REDACTED"})
-            elif key == "password":
-                mydict.update({"password": "REDACTED"})
+            elif key in ["password", "aws_token", "aws_secret_key", "aws_key"]:
+                mydict.update({key: "REDACTED"})
         return mydict
     return iterdict(data)
```

### Comparing `curator-opensearch-0.0.7/curator/validators/actions.py` & `curator-opensearch-0.0.9/curator/validators/actions.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/validators/filters.py` & `curator-opensearch-0.0.9/curator/validators/filters.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/validators/options.py` & `curator-opensearch-0.0.9/curator/validators/options.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator/validators/schemacheck.py` & `curator-opensearch-0.0.9/curator/validators/schemacheck.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/curator_opensearch.egg-info/PKG-INFO` & `curator-opensearch-0.0.9/curator_opensearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: curator-opensearch
-Version: 0.0.7
+Version: 0.0.9
 Summary: Tending your Elasticsearch indices
 Home-page: https://github.com/uzhinskiy/curator-opensearch
-Download-URL: https://github.com/uzhinskiy/curator-opensearch/releases/tag/0.0.7
+Download-URL: https://github.com/uzhinskiy/curator-opensearch/releases/tag/0.0.9
 Author: Uzhinsky
 Author-email: lspci@mail.ru
 License: Apache License, Version 2.0
 Keywords: elasticsearch time-series indexed index-expiry
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE.txt
+License-File: LICENSE
 License-File: NOTICE
 
 .. _readme:
 
 
 Curator
 =======
```

### Comparing `curator-opensearch-0.0.7/curator_opensearch.egg-info/SOURCES.txt` & `curator-opensearch-0.0.9/curator_opensearch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 CONTRIBUTING.md
 CONTRIBUTORS
 Dockerfile
-LICENSE.txt
+LICENSE
 MANIFEST.in
 NOTICE
 README.rst
 setup.cfg
 setup.py
 curator/__init__.py
 curator/_version.py
```

### Comparing `curator-opensearch-0.0.7/docs/Changelog.rst` & `curator-opensearch-0.0.9/docs/Changelog.rst`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/Makefile` & `curator-opensearch-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/actionclasses.rst` & `curator-opensearch-0.0.9/docs/actionclasses.rst`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/about.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/about.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/actions.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/actions.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/command-line.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/command-line.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/configuration.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/configuration.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/examples.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/examples.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/faq.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/faq.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/filter_elements.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/filter_elements.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/filters.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/filters.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/ilm.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/ilm.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/inc_datemath.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/inc_datemath.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/inc_filter_by_aliases.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/inc_filter_by_aliases.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/inc_filter_chaining.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/inc_filter_chaining.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/inc_kinds.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/inc_kinds.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/inc_sources.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/inc_sources.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/inc_timestring_regex.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/inc_timestring_regex.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/index.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/index.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/installation.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/installation.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/options.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/options.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/security.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/security.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/asciidoc/versions.asciidoc` & `curator-opensearch-0.0.9/docs/asciidoc/versions.asciidoc`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/conf.py` & `curator-opensearch-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/examples.rst` & `curator-opensearch-0.0.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/filters.rst` & `curator-opensearch-0.0.9/docs/filters.rst`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/docs/index.rst` & `curator-opensearch-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/setup.cfg` & `curator-opensearch-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/setup.py` & `curator-opensearch-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/__init__.py` & `curator-opensearch-0.0.9/test/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_alias.py` & `curator-opensearch-0.0.9/test/integration/test_alias.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_allocation.py` & `curator-opensearch-0.0.9/test/integration/test_allocation.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_cli.py` & `curator-opensearch-0.0.9/test/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_close.py` & `curator-opensearch-0.0.9/test/integration/test_close.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_clusterrouting.py` & `curator-opensearch-0.0.9/test/integration/test_clusterrouting.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_count_pattern.py` & `curator-opensearch-0.0.9/test/integration/test_count_pattern.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_create_index.py` & `curator-opensearch-0.0.9/test/integration/test_create_index.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_datemath.py` & `curator-opensearch-0.0.9/test/integration/test_datemath.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_delete_indices.py` & `curator-opensearch-0.0.9/test/integration/test_delete_indices.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_delete_snapshots.py` & `curator-opensearch-0.0.9/test/integration/test_delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_envvars.py` & `curator-opensearch-0.0.9/test/integration/test_envvars.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_es_repo_mgr.py` & `curator-opensearch-0.0.9/test/integration/test_es_repo_mgr.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_forcemerge.py` & `curator-opensearch-0.0.9/test/integration/test_forcemerge.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_freeze.py` & `curator-opensearch-0.0.9/test/integration/test_freeze.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_integrations.py` & `curator-opensearch-0.0.9/test/integration/test_integrations.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_open.py` & `curator-opensearch-0.0.9/test/integration/test_open.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_reindex.py` & `curator-opensearch-0.0.9/test/integration/test_reindex.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_replicas.py` & `curator-opensearch-0.0.9/test/integration/test_replicas.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_restore.py` & `curator-opensearch-0.0.9/test/integration/test_restore.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_rollover.py` & `curator-opensearch-0.0.9/test/integration/test_rollover.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_shrink.py` & `curator-opensearch-0.0.9/test/integration/test_shrink.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_snapshot.py` & `curator-opensearch-0.0.9/test/integration/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/test_unfreeze.py` & `curator-opensearch-0.0.9/test/integration/test_unfreeze.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/integration/testvars.py` & `curator-opensearch-0.0.9/test/integration/testvars.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/run_tests.py` & `curator-opensearch-0.0.9/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/__init__.py` & `curator-opensearch-0.0.9/test/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_alias.py` & `curator-opensearch-0.0.9/test/unit/test_action_alias.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_allocation.py` & `curator-opensearch-0.0.9/test/unit/test_action_allocation.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_close.py` & `curator-opensearch-0.0.9/test/unit/test_action_close.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_clusterrouting.py` & `curator-opensearch-0.0.9/test/unit/test_action_clusterrouting.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_create_index.py` & `curator-opensearch-0.0.9/test/unit/test_action_create_index.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_delete_indices.py` & `curator-opensearch-0.0.9/test/unit/test_action_delete_indices.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_delete_snapshots.py` & `curator-opensearch-0.0.9/test/unit/test_action_delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_forcemerge.py` & `curator-opensearch-0.0.9/test/unit/test_action_forcemerge.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_indexsettings.py` & `curator-opensearch-0.0.9/test/unit/test_action_indexsettings.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_open.py` & `curator-opensearch-0.0.9/test/unit/test_action_open.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_reindex.py` & `curator-opensearch-0.0.9/test/unit/test_action_reindex.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_replicas.py` & `curator-opensearch-0.0.9/test/unit/test_action_replicas.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_restore.py` & `curator-opensearch-0.0.9/test/unit/test_action_restore.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_rollover.py` & `curator-opensearch-0.0.9/test/unit/test_action_rollover.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_shrink.py` & `curator-opensearch-0.0.9/test/unit/test_action_shrink.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_action_snapshot.py` & `curator-opensearch-0.0.9/test/unit/test_action_snapshot.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_class_index_list.py` & `curator-opensearch-0.0.9/test/unit/test_class_index_list.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_class_snapshot_list.py` & `curator-opensearch-0.0.9/test/unit/test_class_snapshot_list.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_cli_methods.py` & `curator-opensearch-0.0.9/test/unit/test_cli_methods.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_utils.py` & `curator-opensearch-0.0.9/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/test_validators.py` & `curator-opensearch-0.0.9/test/unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `curator-opensearch-0.0.7/test/unit/testvars.py` & `curator-opensearch-0.0.9/test/unit/testvars.py`

 * *Files identical despite different names*

