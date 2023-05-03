# Comparing `tmp/joes_giant_toolbox-0.2.21.tar.gz` & `tmp/joes_giant_toolbox-0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joes_giant_toolbox-0.2.21.tar", last modified: Wed May  3 10:49:17 2023, max compression
+gzip compressed data, was "joes_giant_toolbox-0.2.22.tar", last modified: Wed May  3 12:03:26 2023, max compression
```

## Comparing `joes_giant_toolbox-0.2.21.tar` & `joes_giant_toolbox-0.2.22.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 10:49:17.458943 joes_giant_toolbox-0.2.21/
--rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.2.21/LICENSE
--rw-r--r--   0 josephbolton   (501) staff       (20)    59255 2023-05-03 10:49:17.458768 joes_giant_toolbox-0.2.21/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)    17973 2023-05-03 09:24:44.000000 joes_giant_toolbox-0.2.21/README.md
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 10:49:17.442806 joes_giant_toolbox-0.2.21/joes_giant_toolbox/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/__init__.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 10:49:17.453568 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/__init__.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/ascii_density_histogram.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     9531 2023-04-30 11:40:27.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/compare_metric_to_prev_period.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     3441 2023-05-03 07:39:27.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/create_project_scope_doc.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/duckduckgo_search_multipage.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2453 2023-05-02 19:34:13.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/gcloud_vm_docker_template.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2261 2023-04-17 14:00:23.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/list_all_python_imports.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      878 2023-03-20 07:49:14.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      376 2023-04-23 20:15:27.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/manual_keyword_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2318 2023-04-19 11:00:23.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/print_progress_bar.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2117 2023-04-27 07:33:31.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/python_plotting_tutorials.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     8590 2023-05-03 10:45:09.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/regex_rules_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4608 2023-03-30 09:37:03.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/run_python_function_in_parallel.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    13692 2023-04-25 10:48:25.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/string_cleaner.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1536 2023-04-13 10:47:28.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/view_nested_dict_structure.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1805 2023-03-21 10:01:14.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      264 2023-04-17 12:16:19.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/convenience.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      413 2023-04-25 07:40:31.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/dataviz.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1300 2023-05-03 07:44:59.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/google_cloud.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 10:49:17.456461 joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/
--rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/ascii_barplot.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/query_wikipedia_api.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/recsys_data_simulator.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/proj_mgmt.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/sklearn.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      161 2023-04-26 19:46:54.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/stats.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      450 2023-05-03 07:44:37.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/text.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox/web.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 10:49:17.443517 joes_giant_toolbox-0.2.21/joes_giant_toolbox.egg-info/
--rw-r--r--   0 josephbolton   (501) staff       (20)    59255 2023-05-03 10:49:17.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)     2727 2023-05-03 10:49:17.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-05-03 10:49:17.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)      186 2023-05-03 10:49:17.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox.egg-info/requires.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-05-03 10:49:17.000000 joes_giant_toolbox-0.2.21/joes_giant_toolbox.egg-info/top_level.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)     1085 2023-05-03 10:41:19.000000 joes_giant_toolbox-0.2.21/pyproject.toml
--rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-05-03 10:49:17.458984 joes_giant_toolbox-0.2.21/setup.cfg
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 10:49:17.458320 joes_giant_toolbox-0.2.21/tests/
--rw-r--r--   0 josephbolton   (501) staff       (20)      557 2023-04-26 19:48:17.000000 joes_giant_toolbox-0.2.21/tests/test_conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      571 2023-04-25 09:26:34.000000 joes_giant_toolbox-0.2.21/tests/test_longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2617 2023-04-25 09:27:22.000000 joes_giant_toolbox-0.2.21/tests/test_make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     8681 2023-04-25 09:28:50.000000 joes_giant_toolbox-0.2.21/tests/test_rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4500 2023-04-25 09:29:06.000000 joes_giant_toolbox-0.2.21/tests/test_string_cleaner.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 12:03:26.754750 joes_giant_toolbox-0.2.22/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.2.22/LICENSE
+-rw-r--r--   0 josephbolton   (501) staff       (20)    59255 2023-05-03 12:03:26.754586 joes_giant_toolbox-0.2.22/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)    17973 2023-05-03 09:24:44.000000 joes_giant_toolbox-0.2.22/README.md
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 12:03:26.741045 joes_giant_toolbox-0.2.22/joes_giant_toolbox/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/__init__.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 12:03:26.751341 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/__init__.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/ascii_density_histogram.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     9531 2023-04-30 11:40:27.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/compare_metric_to_prev_period.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     3441 2023-05-03 07:39:27.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/create_project_scope_doc.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/duckduckgo_search_multipage.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2453 2023-05-02 19:34:13.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/gcloud_vm_docker_template.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2261 2023-04-17 14:00:23.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/list_all_python_imports.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      878 2023-03-20 07:49:14.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      376 2023-04-23 20:15:27.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/manual_keyword_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2318 2023-04-19 11:00:23.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/print_progress_bar.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2117 2023-04-27 07:33:31.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/python_plotting_tutorials.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     8677 2023-05-03 12:01:21.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/regex_rules_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4608 2023-03-30 09:37:03.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/run_python_function_in_parallel.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    13692 2023-04-25 10:48:25.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/string_cleaner.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1536 2023-04-13 10:47:28.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/view_nested_dict_structure.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1805 2023-03-21 10:01:14.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      264 2023-04-17 12:16:19.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/convenience.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      413 2023-04-25 07:40:31.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/dataviz.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1300 2023-05-03 07:44:59.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/google_cloud.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 12:03:26.752862 joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/ascii_barplot.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/query_wikipedia_api.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/recsys_data_simulator.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/proj_mgmt.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/sklearn.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      161 2023-04-26 19:46:54.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/stats.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      450 2023-05-03 07:44:37.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/text.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox/web.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 12:03:26.741752 joes_giant_toolbox-0.2.22/joes_giant_toolbox.egg-info/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    59255 2023-05-03 12:03:26.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2727 2023-05-03 12:03:26.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-05-03 12:03:26.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)      186 2023-05-03 12:03:26.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox.egg-info/requires.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-05-03 12:03:26.000000 joes_giant_toolbox-0.2.22/joes_giant_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1085 2023-05-03 12:03:00.000000 joes_giant_toolbox-0.2.22/pyproject.toml
+-rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-05-03 12:03:26.754785 joes_giant_toolbox-0.2.22/setup.cfg
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 12:03:26.754261 joes_giant_toolbox-0.2.22/tests/
+-rw-r--r--   0 josephbolton   (501) staff       (20)      557 2023-04-26 19:48:17.000000 joes_giant_toolbox-0.2.22/tests/test_conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      571 2023-04-25 09:26:34.000000 joes_giant_toolbox-0.2.22/tests/test_longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2617 2023-04-25 09:27:22.000000 joes_giant_toolbox-0.2.22/tests/test_make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     8681 2023-04-25 09:28:50.000000 joes_giant_toolbox-0.2.22/tests/test_rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4500 2023-04-25 09:29:06.000000 joes_giant_toolbox-0.2.22/tests/test_string_cleaner.py
```

### Comparing `joes_giant_toolbox-0.2.21/LICENSE` & `joes_giant_toolbox-0.2.22/LICENSE`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/PKG-INFO` & `joes_giant_toolbox-0.2.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joes_giant_toolbox
-Version: 0.2.21
+Version: 0.2.22
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `joes_giant_toolbox-0.2.21/README.md` & `joes_giant_toolbox-0.2.22/README.md`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/ascii_density_histogram.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/ascii_density_histogram.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/compare_metric_to_prev_period.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/compare_metric_to_prev_period.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/create_project_scope_doc.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/create_project_scope_doc.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/duckduckgo_search_multipage.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/duckduckgo_search_multipage.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/gcloud_vm_docker_template.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/gcloud_vm_docker_template.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/list_all_python_imports.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/list_all_python_imports.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/make_url_request.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/make_url_request.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/print_progress_bar.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/print_progress_bar.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/python_plotting_tutorials.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/python_plotting_tutorials.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/rapid_binary_classifier.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/rapid_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/regex_rules_classifier.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/regex_rules_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,18 @@
             Returns one of:
                 * A single predicted class label (if ties_handling in ["first","random"])
                 * A list of predicted class labels (if ties_handling=="all")
                 * None if no class label was awarded any points (i.e. no regex matches at all)
         """
         scores_dict: dict = self.__tally_label_scores(text_str)
         if max(scores_dict.values()) == 0:
-            return None
+            if ties_handling == "all":
+                return []
+            else:
+                return None
         elif ties_handling == "first":
             return max(scores_dict, key=scores_dict.get)
         elif ties_handling == "all":
             return [
                 k for k in scores_dict if scores_dict[k] == max(scores_dict.values())
             ]
         elif ties_handling == "random":
```

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/run_python_function_in_parallel.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/run_python_function_in_parallel.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/string_cleaner.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/string_cleaner.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/view_nested_dict_structure.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/view_nested_dict_structure.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/google_cloud.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/google_cloud.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/ascii_barplot.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/ascii_barplot.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/in_progress/recsys_data_simulator.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/in_progress/recsys_data_simulator.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox/web.py` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox/web.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox.egg-info/PKG-INFO` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joes-giant-toolbox
-Version: 0.2.21
+Version: 0.2.22
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `joes_giant_toolbox-0.2.21/joes_giant_toolbox.egg-info/SOURCES.txt` & `joes_giant_toolbox-0.2.22/joes_giant_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/pyproject.toml` & `joes_giant_toolbox-0.2.22/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "joes_giant_toolbox"
-version = "0.2.21"
+version = "0.2.22"
 description = "A large collection of general python functions and classes that I use in my daily work"
 readme = "README.md"
 authors = [{ name = "Joseph Bolton", email = "joseph.jazz.bolton@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `joes_giant_toolbox-0.2.21/tests/test_conjugate_prior_beta_binomial.py` & `joes_giant_toolbox-0.2.22/tests/test_conjugate_prior_beta_binomial.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/tests/test_longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.2.22/tests/test_longest_sentence_subsequence_plagiarism_detector.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/tests/test_make_url_request.py` & `joes_giant_toolbox-0.2.22/tests/test_make_url_request.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/tests/test_rapid_binary_classifier.py` & `joes_giant_toolbox-0.2.22/tests/test_rapid_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.21/tests/test_string_cleaner.py` & `joes_giant_toolbox-0.2.22/tests/test_string_cleaner.py`

 * *Files identical despite different names*

