# Comparing `tmp/joes_giant_toolbox-0.1.0.tar.gz` & `tmp/joes_giant_toolbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joes_giant_toolbox-0.1.0.tar", last modified: Wed Apr 26 19:50:33 2023, max compression
+gzip compressed data, was "joes_giant_toolbox-0.2.0.tar", last modified: Wed May  3 07:45:58 2023, max compression
```

## Comparing `joes_giant_toolbox-0.1.0.tar` & `joes_giant_toolbox-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.809391 joes_giant_toolbox-0.1.0/
--rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.1.0/LICENSE
--rw-r--r--   0 josephbolton   (501) staff       (20)    58561 2023-04-26 19:50:33.809154 joes_giant_toolbox-0.1.0/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)    17280 2023-04-26 19:47:46.000000 joes_giant_toolbox-0.1.0/README.md
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.792653 joes_giant_toolbox-0.1.0/joes_giant_toolbox/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/__init__.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.803910 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/__init__.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/ascii_density_histogram.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/create_project_scope_doc.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/duckduckgo_search_multipage.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2261 2023-04-17 14:00:23.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/list_all_python_imports.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      878 2023-03-20 07:49:14.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      376 2023-04-23 20:15:27.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/manual_keyword_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2318 2023-04-19 11:00:23.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/print_progress_bar.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2098 2023-04-26 19:31:41.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/python_plotting_tutorials.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4608 2023-03-30 09:37:03.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/run_python_function_in_parallel.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    13692 2023-04-25 10:48:25.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/string_cleaner.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1536 2023-04-13 10:47:28.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/view_nested_dict_structure.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1805 2023-03-21 10:01:14.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      264 2023-04-17 12:16:19.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/convenience.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      413 2023-04-25 07:40:31.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/dataviz.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1150 2023-04-21 18:17:10.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/google_cloud.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.806525 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/
--rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/ascii_barplot.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/query_wikipedia_api.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/recsys_data_simulator.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/proj_mgmt.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/sklearn.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      161 2023-04-26 19:46:54.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/stats.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      246 2023-04-25 10:34:50.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/text.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/web.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.793753 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/
--rw-r--r--   0 josephbolton   (501) staff       (20)    58561 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)     2511 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)      186 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/requires.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/top_level.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)     1084 2023-04-26 19:49:36.000000 joes_giant_toolbox-0.1.0/pyproject.toml
--rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-04-26 19:50:33.809446 joes_giant_toolbox-0.1.0/setup.cfg
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.808561 joes_giant_toolbox-0.1.0/tests/
--rw-r--r--   0 josephbolton   (501) staff       (20)      557 2023-04-26 19:48:17.000000 joes_giant_toolbox-0.1.0/tests/test_conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      571 2023-04-25 09:26:34.000000 joes_giant_toolbox-0.1.0/tests/test_longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2617 2023-04-25 09:27:22.000000 joes_giant_toolbox-0.1.0/tests/test_make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     8681 2023-04-25 09:28:50.000000 joes_giant_toolbox-0.1.0/tests/test_rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4500 2023-04-25 09:29:06.000000 joes_giant_toolbox-0.1.0/tests/test_string_cleaner.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 07:45:58.685978 joes_giant_toolbox-0.2.0/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.2.0/LICENSE
+-rw-r--r--   0 josephbolton   (501) staff       (20)    59214 2023-05-03 07:45:58.685741 joes_giant_toolbox-0.2.0/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)    17933 2023-05-03 07:45:04.000000 joes_giant_toolbox-0.2.0/README.md
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 07:45:58.667156 joes_giant_toolbox-0.2.0/joes_giant_toolbox/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/__init__.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 07:45:58.680258 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/__init__.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/ascii_density_histogram.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     9531 2023-04-30 11:40:27.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/compare_metric_to_prev_period.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     3441 2023-05-03 07:39:27.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/create_project_scope_doc.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/duckduckgo_search_multipage.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2453 2023-05-02 19:34:13.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/gcloud_vm_docker_template.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2261 2023-04-17 14:00:23.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/list_all_python_imports.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      878 2023-03-20 07:49:14.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      376 2023-04-23 20:15:27.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/manual_keyword_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2318 2023-04-19 11:00:23.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/print_progress_bar.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2117 2023-04-27 07:33:31.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/python_plotting_tutorials.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     8380 2023-05-03 07:31:27.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/regex_rules_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4608 2023-03-30 09:37:03.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/run_python_function_in_parallel.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    13692 2023-04-25 10:48:25.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/string_cleaner.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1536 2023-04-13 10:47:28.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/view_nested_dict_structure.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1805 2023-03-21 10:01:14.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      264 2023-04-17 12:16:19.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/convenience.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      413 2023-04-25 07:40:31.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/dataviz.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1300 2023-05-03 07:44:59.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/google_cloud.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 07:45:58.683065 joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/ascii_barplot.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/query_wikipedia_api.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/recsys_data_simulator.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/proj_mgmt.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/sklearn.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      161 2023-04-26 19:46:54.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/stats.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      450 2023-05-03 07:44:37.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/text.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox/web.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 07:45:58.668205 joes_giant_toolbox-0.2.0/joes_giant_toolbox.egg-info/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    59214 2023-05-03 07:45:58.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2727 2023-05-03 07:45:58.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-05-03 07:45:58.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)      186 2023-05-03 07:45:58.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox.egg-info/requires.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-05-03 07:45:58.000000 joes_giant_toolbox-0.2.0/joes_giant_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1084 2023-05-03 07:45:26.000000 joes_giant_toolbox-0.2.0/pyproject.toml
+-rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-05-03 07:45:58.686035 joes_giant_toolbox-0.2.0/setup.cfg
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-03 07:45:58.685155 joes_giant_toolbox-0.2.0/tests/
+-rw-r--r--   0 josephbolton   (501) staff       (20)      557 2023-04-26 19:48:17.000000 joes_giant_toolbox-0.2.0/tests/test_conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      571 2023-04-25 09:26:34.000000 joes_giant_toolbox-0.2.0/tests/test_longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2617 2023-04-25 09:27:22.000000 joes_giant_toolbox-0.2.0/tests/test_make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     8681 2023-04-25 09:28:50.000000 joes_giant_toolbox-0.2.0/tests/test_rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4500 2023-04-25 09:29:06.000000 joes_giant_toolbox-0.2.0/tests/test_string_cleaner.py
```

### Comparing `joes_giant_toolbox-0.1.0/LICENSE` & `joes_giant_toolbox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/PKG-INFO` & `joes_giant_toolbox-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joes_giant_toolbox
-Version: 0.1.0
+Version: 0.2.0
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -758,27 +758,29 @@
 ..or you can just scroll through the master list:
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
+| create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
 | create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        | 
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | duckduckgo_search_multipage                       | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | make_url_request                                  | A convenience function for making API requests using the urllib library                                      |         3        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
+| RegexRulesClassifier | A multi-class text classifier using manual regex rules | 2
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 | scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | url_to_filename_to_url_mapper                     | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 | view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
@@ -825,25 +827,27 @@
 ```
 
 ```python
 import joes_giant_toolbox.google_cloud
 
 help(joes_giant_toolbox.google_cloud)
 
-help(joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python)
-help(joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df)
-help(joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table)
+help( joes_giant_toolbox.google_cloud.create_gcloud_vm_docker_template ) 
+help( joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python )
+help( joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df )
+help( joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
+| create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
@@ -895,20 +899,22 @@
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 
 ## Text and Natural Language Processing
 ```python 
 import joes_giant_toolbox.text
 help( joes_giant_toolbox.text )
 help( joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector )
+help( joes_giant_toolbox.text.RegexRulesClassifier )
 help( joes_giant_toolbox.text.StringCleaner )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
+RegexRulesClassifier | A multi-class text classifier using manual regex rules | 2
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 
 # Run Unit Tests
 
 ```bash
 pip install pytest
 cd joes_giant_toolbox/tests
```

### Comparing `joes_giant_toolbox-0.1.0/README.md` & `joes_giant_toolbox-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,27 +66,29 @@
 ..or you can just scroll through the master list:
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
+| create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
 | create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        | 
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | duckduckgo_search_multipage                       | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | make_url_request                                  | A convenience function for making API requests using the urllib library                                      |         3        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
+| RegexRulesClassifier | A multi-class text classifier using manual regex rules | 2
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 | scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | url_to_filename_to_url_mapper                     | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 | view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
@@ -133,25 +135,27 @@
 ```
 
 ```python
 import joes_giant_toolbox.google_cloud
 
 help(joes_giant_toolbox.google_cloud)
 
-help(joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python)
-help(joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df)
-help(joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table)
+help( joes_giant_toolbox.google_cloud.create_gcloud_vm_docker_template ) 
+help( joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python )
+help( joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df )
+help( joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
+| create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
@@ -203,20 +207,22 @@
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 
 ## Text and Natural Language Processing
 ```python 
 import joes_giant_toolbox.text
 help( joes_giant_toolbox.text )
 help( joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector )
+help( joes_giant_toolbox.text.RegexRulesClassifier )
 help( joes_giant_toolbox.text.StringCleaner )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
+RegexRulesClassifier | A multi-class text classifier using manual regex rules | 2
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 
 # Run Unit Tests
 
 ```bash
 pip install pytest
 cd joes_giant_toolbox/tests
```

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/ascii_density_histogram.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/ascii_density_histogram.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/create_project_scope_doc.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/create_project_scope_doc.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/duckduckgo_search_multipage.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/duckduckgo_search_multipage.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/list_all_python_imports.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/list_all_python_imports.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/make_url_request.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/make_url_request.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/print_progress_bar.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/print_progress_bar.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/python_plotting_tutorials.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/python_plotting_tutorials.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         )
         axs[row_idx,col_idx].set_xlabel("x axis label")
         axs[row_idx,col_idx].set_ylabel("y axis label")
         axs[row_idx,col_idx].set_title(f"Axis [{row_idx},{col_idx}]")
 for ax in axs.flat:    # only keep the axis labels and axis ticks on the outer plots
     ax.label_outer()
 fig.suptitle("Global Plot Title")      
+fig.tight_layout()
 
 plt.show()
             """,
             "heatmap": """
 # https://seaborn.pydata.org/generated/seaborn.heatmap.html
 import numpy as np
 from matplotlib import pyplot as plt
```

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/rapid_binary_classifier.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/rapid_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/run_python_function_in_parallel.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/run_python_function_in_parallel.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/string_cleaner.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/string_cleaner.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/view_nested_dict_structure.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/view_nested_dict_structure.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/ascii_barplot.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/ascii_barplot.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/recsys_data_simulator.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/in_progress/recsys_data_simulator.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox/web.py` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox/web.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/PKG-INFO` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joes-giant-toolbox
-Version: 0.1.0
+Version: 0.2.0
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -758,27 +758,29 @@
 ..or you can just scroll through the master list:
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
+| create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
 | create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        | 
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | duckduckgo_search_multipage                       | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | make_url_request                                  | A convenience function for making API requests using the urllib library                                      |         3        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
+| RegexRulesClassifier | A multi-class text classifier using manual regex rules | 2
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 | scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | url_to_filename_to_url_mapper                     | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 | view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
@@ -825,25 +827,27 @@
 ```
 
 ```python
 import joes_giant_toolbox.google_cloud
 
 help(joes_giant_toolbox.google_cloud)
 
-help(joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python)
-help(joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df)
-help(joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket)
-help(joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table)
+help( joes_giant_toolbox.google_cloud.create_gcloud_vm_docker_template ) 
+help( joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python )
+help( joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df )
+help( joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket )
+help( joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
+| create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
@@ -895,20 +899,22 @@
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 
 ## Text and Natural Language Processing
 ```python 
 import joes_giant_toolbox.text
 help( joes_giant_toolbox.text )
 help( joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector )
+help( joes_giant_toolbox.text.RegexRulesClassifier )
 help( joes_giant_toolbox.text.StringCleaner )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
+RegexRulesClassifier | A multi-class text classifier using manual regex rules | 2
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 
 # Run Unit Tests
 
 ```bash
 pip install pytest
 cd joes_giant_toolbox/tests
```

### Comparing `joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/SOURCES.txt` & `joes_giant_toolbox-0.2.0/joes_giant_toolbox.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,29 +14,33 @@
 joes_giant_toolbox.egg-info/SOURCES.txt
 joes_giant_toolbox.egg-info/dependency_links.txt
 joes_giant_toolbox.egg-info/requires.txt
 joes_giant_toolbox.egg-info/top_level.txt
 joes_giant_toolbox/all/__init__.py
 joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
 joes_giant_toolbox/all/ascii_density_histogram.py
+joes_giant_toolbox/all/compare_metric_to_prev_period.py
 joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
+joes_giant_toolbox/all/create_gcloud_vm_docker_template.py
 joes_giant_toolbox/all/create_project_scope_doc.py
 joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
 joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
 joes_giant_toolbox/all/duckduckgo_search_multipage.py
+joes_giant_toolbox/all/gcloud_vm_docker_template.py
 joes_giant_toolbox/all/list_all_python_imports.py
 joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
 joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
 joes_giant_toolbox/all/make_url_request.py
 joes_giant_toolbox/all/manual_keyword_classifier.py
 joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
 joes_giant_toolbox/all/print_progress_bar.py
 joes_giant_toolbox/all/python_plotting_tutorials.py
 joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
 joes_giant_toolbox/all/rapid_binary_classifier.py
+joes_giant_toolbox/all/regex_rules_classifier.py
 joes_giant_toolbox/all/run_python_function_in_parallel.py
 joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
 joes_giant_toolbox/all/string_cleaner.py
 joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
 joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
 joes_giant_toolbox/all/view_nested_dict_structure.py
 joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
```

### Comparing `joes_giant_toolbox-0.1.0/pyproject.toml` & `joes_giant_toolbox-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "joes_giant_toolbox"
-version = "0.1.0"
+version = "0.2.0"
 description = "A large collection of general python functions and classes that I use in my daily work"
 readme = "README.md"
 authors = [{ name = "Joseph Bolton", email = "joseph.jazz.bolton@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `joes_giant_toolbox-0.1.0/tests/test_conjugate_prior_beta_binomial.py` & `joes_giant_toolbox-0.2.0/tests/test_conjugate_prior_beta_binomial.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/tests/test_longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.2.0/tests/test_longest_sentence_subsequence_plagiarism_detector.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/tests/test_make_url_request.py` & `joes_giant_toolbox-0.2.0/tests/test_make_url_request.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/tests/test_rapid_binary_classifier.py` & `joes_giant_toolbox-0.2.0/tests/test_rapid_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.1.0/tests/test_string_cleaner.py` & `joes_giant_toolbox-0.2.0/tests/test_string_cleaner.py`

 * *Files identical despite different names*

