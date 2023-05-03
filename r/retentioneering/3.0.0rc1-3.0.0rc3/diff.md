# Comparing `tmp/retentioneering-3.0.0rc1.tar.gz` & `tmp/retentioneering-3.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retentioneering-3.0.0rc1.tar", max compression
+gzip compressed data, was "retentioneering-3.0.0rc3.tar", max compression
```

## Comparing `retentioneering-3.0.0rc1.tar` & `retentioneering-3.0.0rc3.tar`

### file list

```diff
@@ -1,128 +1,133 @@
--rw-r--r--   0        0        0     7341 2022-09-06 07:58:30.273796 retentioneering-3.0.0rc1/LICENSE
--rw-r--r--   0        0        0     1948 2023-04-25 09:10:37.994103 retentioneering-3.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      375 2023-04-19 10:56:29.220603 retentioneering-3.0.0rc1/retentioneering/__init__.py
--rw-r--r--   0        0        0       84 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc1/retentioneering/backend/__init__.py
--rw-r--r--   0        0        0      113 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc1/retentioneering/backend/callback/__init__.py
--rw-r--r--   0        0        0      490 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/backend/callback/list_dataprocessors.py
--rw-r--r--   0        0        0     5220 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/backend/callback/mock_list_dataprocessor.py
--rw-r--r--   0        0        0     1097 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc1/retentioneering/backend/jupiter_server.py
--rw-r--r--   0        0        0     5293 2023-04-03 06:56:53.875728 retentioneering-3.0.0rc1/retentioneering/backend/server_manager.py
--rw-r--r--   0        0        0      238 2023-04-25 12:22:39.634379 retentioneering-3.0.0rc1/retentioneering/backend/tracker/__init__.py
--rw-r--r--   0        0        0     1825 2023-04-25 10:18:51.331519 retentioneering-3.0.0rc1/retentioneering/backend/tracker/connector.py
--rw-r--r--   0        0        0     2250 2023-04-25 10:01:07.873883 retentioneering-3.0.0rc1/retentioneering/backend/tracker/hwid.py
--rw-r--r--   0        0        0     2875 2023-04-25 10:03:20.421185 retentioneering-3.0.0rc1/retentioneering/backend/tracker/tracker.py
--rw-r--r--   0        0        0     1162 2023-04-22 16:00:11.500677 retentioneering-3.0.0rc1/retentioneering/backend/tracker/tracking_info.py
--rw-r--r--   0        0        0       59 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc1/retentioneering/constants/__init__.py
--rw-r--r--   0        0        0      345 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc1/retentioneering/constants/constants.py
--rw-r--r--   0        0        0       42 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc1/retentioneering/data_processor/__init__.py
--rw-r--r--   0        0        0     2190 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc1/retentioneering/data_processor/data_processor.py
--rw-r--r--   0        0        0     1744 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc1/retentioneering/data_processor/registry.py
--rw-r--r--   0        0        0      843 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/__init__.py
--rw-r--r--   0        0        0     3887 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_negative_events.py
--rw-r--r--   0        0        0     3794 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_positive_events.py
--rw-r--r--   0        0        0     2449 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_start_end_events.py
--rw-r--r--   0        0        0     4781 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/collapse_loops.py
--rw-r--r--   0        0        0     3517 2023-04-21 10:45:45.328652 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/drop_paths.py
--rw-r--r--   0        0        0     2342 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/filter_events.py
--rw-r--r--   0        0        0     3332 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/group_events.py
--rw-r--r--   0        0        0     5454 2023-04-21 11:46:01.978908 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_cropped_paths.py
--rw-r--r--   0        0        0     4633 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_lost_users.py
--rw-r--r--   0        0        0     3186 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_new_users.py
--rw-r--r--   0        0        0     1760 2023-03-17 11:02:30.068802 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/rename.py
--rw-r--r--   0        0        0     8492 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/split_sessions.py
--rw-r--r--   0        0        0     6575 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/data_processors_lib/truncate_paths.py
--rw-r--r--   0        0        0       56 2023-01-16 14:26:06.544412 retentioneering-3.0.0rc1/retentioneering/datasets/__init__.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.544412 retentioneering-3.0.0rc1/retentioneering/datasets/data/__init__.py
--rw-r--r--   0        0        0  1903381 2023-01-16 14:26:06.551078 retentioneering-3.0.0rc1/retentioneering/datasets/data/ab_test_demo.csv
--rw-r--r--   0        0        0  1467900 2023-03-07 11:03:25.188171 retentioneering-3.0.0rc1/retentioneering/datasets/data/simple-onlineshop.csv
--rw-r--r--   0        0        0     1352 2023-03-07 11:03:25.188171 retentioneering-3.0.0rc1/retentioneering/datasets/load.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/edgelist/__init__.py
--rw-r--r--   0        0        0     4222 2023-04-21 11:46:51.235714 retentioneering-3.0.0rc1/retentioneering/edgelist/edgelist.py
--rw-r--r--   0        0        0      486 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/eventstream/__init__.py
--rw-r--r--   0        0        0    42818 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/eventstream.py
--rw-r--r--   0        0        0      792 2023-04-19 10:56:35.553951 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/__init__.py
--rw-r--r--   0        0        0     1431 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_negative_events_helper.py
--rw-r--r--   0        0        0     1430 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_positive_events_helper.py
--rw-r--r--   0        0        0     1084 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_start_end_events_helper.py
--rw-r--r--   0        0        0     1494 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/collapse_loops_helper.py
--rw-r--r--   0        0        0     1328 2023-04-25 09:09:49.820705 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/drop_paths_helper.py
--rw-r--r--   0        0        0     1194 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/filter_events_helper.py
--rw-r--r--   0        0        0     1511 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/group_events_helper.py
--rw-r--r--   0        0        0     1512 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_cropped_paths_helper.py
--rw-r--r--   0        0        0     1468 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_lost_users_helper.py
--rw-r--r--   0        0        0     1291 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_new_users_helper.py
--rw-r--r--   0        0        0      736 2023-04-25 09:09:49.824038 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/rename_helper.py
--rw-r--r--   0        0        0     1901 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/split_sessions_helper.py
--rw-r--r--   0        0        0     1758 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/truncate_paths_helper.py
--rw-r--r--   0        0        0     4157 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc1/retentioneering/eventstream/schema.py
--rw-r--r--   0        0        0     2389 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc1/retentioneering/eventstream/types.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/exceptions/__init__.py
--rw-r--r--   0        0        0       45 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/exceptions/base.py
--rw-r--r--   0        0        0     1242 2023-03-22 12:39:29.884664 retentioneering-3.0.0rc1/retentioneering/exceptions/server.py
--rw-r--r--   0        0        0      306 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/exceptions/widget.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/nodelist/__init__.py
--rw-r--r--   0        0        0     1071 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc1/retentioneering/nodelist/nodelist.py
--rw-r--r--   0        0        0       38 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/params_model/__init__.py
--rw-r--r--   0        0        0    11910 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/params_model/params_model.py
--rw-r--r--   0        0        0      952 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/params_model/registry.py
--rw-r--r--   0        0        0      105 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/__init__.py
--rw-r--r--   0        0        0     4223 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/nodes.py
--rw-r--r--   0        0        0    14182 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/preprocessing_graph.py
--rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/preprocessor/__init__.py
--rw-r--r--   0        0        0       65 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/templates/__init__.py
--rw-r--r--   0        0        0       45 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/__init__.py
--rw-r--r--   0        0        0     1704 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/preprocessing_graph.html
--rw-r--r--   0        0        0      736 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/show.py
--rw-r--r--   0        0        0       42 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/__init__.py
--rw-r--r--   0        0        0       22 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/body.html
--rw-r--r--   0        0        0      713 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/full.html
--rw-r--r--   0        0        0      894 2023-04-17 15:56:16.596442 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/init_template.py
--rw-r--r--   0        0        0     1507 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/inner_iframe.html
--rw-r--r--   0        0        0     1143 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/show.py
--rw-r--r--   0        0        0      382 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/__init__.py
--rw-r--r--   0        0        0       33 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_describe/__init__.py
--rw-r--r--   0        0        0     4543 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_describe/_describe.py
--rw-r--r--   0        0        0       46 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_describe_events/__init__.py
--rw-r--r--   0        0        0     4750 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_describe_events/_describe_events.py
--rw-r--r--   0        0        0       50 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_transition_matrix/__init__.py
--rw-r--r--   0        0        0     1319 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/_transition_matrix/_transition_matrix.py
--rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/clusters/__init__.py
--rw-r--r--   0        0        0    30782 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/tooling/clusters/clusters.py
--rw-r--r--   0        0        0     2039 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/clusters/segments.py
--rw-r--r--   0        0        0     3166 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/clusters/userlist.py
--rw-r--r--   0        0        0       29 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/cohorts/__init__.py
--rw-r--r--   0        0        0    13526 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/cohorts/cohorts.py
--rw-r--r--   0        0        0       39 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/constants/__init__.py
--rw-r--r--   0        0        0      240 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/constants/constants.py
--rw-r--r--   0        0        0       53 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc1/retentioneering/tooling/event_timestamp_hist/__init__.py
--rw-r--r--   0        0        0     6284 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py
--rw-r--r--   0        0        0       27 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/tooling/funnel/__init__.py
--rw-r--r--   0        0        0    12972 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/tooling/funnel/funnel.py
--rw-r--r--   0        0        0       43 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/mixins/__init__.py
--rw-r--r--   0        0        0     1516 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/mixins/ended_events.py
--rw-r--r--   0        0        0       71 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/stattests/__init__.py
--rw-r--r--   0        0        0      171 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc1/retentioneering/tooling/stattests/constants.py
--rw-r--r--   0        0        0    13243 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/tooling/stattests/stattests.py
--rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/tooling/step_matrix/__init__.py
--rw-r--r--   0        0        0    22300 2023-04-25 09:09:49.827372 retentioneering-3.0.0rc1/retentioneering/tooling/step_matrix/step_matrix.py
--rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/tooling/step_sankey/__init__.py
--rw-r--r--   0        0        0    25006 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/step_sankey/step_sankey.py
--rw-r--r--   0        0        0      110 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/timedelta_hist/__init__.py
--rw-r--r--   0        0        0      186 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/timedelta_hist/constants.py
--rw-r--r--   0        0        0    13342 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/timedelta_hist/timedelta_hist.py
--rw-r--r--   0        0        0       46 2023-04-03 06:56:53.882394 retentioneering-3.0.0rc1/retentioneering/tooling/transition_graph/__init__.py
--rw-r--r--   0        0        0    36518 2023-04-24 11:53:04.647152 retentioneering-3.0.0rc1/retentioneering/tooling/transition_graph/transition_graph.py
--rw-r--r--   0        0        0        0 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/typing/__init__.py
--rw-r--r--   0        0        0      171 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/tooling/typing/transition_graph/__init__.py
--rw-r--r--   0        0        0     1327 2023-04-03 06:56:53.882394 retentioneering-3.0.0rc1/retentioneering/tooling/typing/transition_graph/graph_types.py
--rw-r--r--   0        0        0       49 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/tooling/user_lifetime_hist/__init__.py
--rw-r--r--   0        0        0     7385 2023-04-22 16:00:17.282964 retentioneering-3.0.0rc1/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py
--rw-r--r--   0        0        0      458 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/utils/__init__.py
--rw-r--r--   0        0        0      122 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/utils/dict.py
--rw-r--r--   0        0        0      465 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/utils/list.py
--rw-r--r--   0        0        0      444 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc1/retentioneering/utils/pandas.py
--rw-r--r--   0        0        0      986 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/utils/registry.py
--rw-r--r--   0        0        0      269 2023-04-22 16:00:11.500677 retentioneering-3.0.0rc1/retentioneering/utils/singleton.py
--rw-r--r--   0        0        0       77 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc1/retentioneering/widget/__init__.py
--rw-r--r--   0        0        0     7265 2023-03-22 12:39:29.887997 retentioneering-3.0.0rc1/retentioneering/widget/widgets.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 retentioneering-3.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     7341 2022-09-06 07:58:30.273796 retentioneering-3.0.0rc3/LICENSE.md
+-rw-r--r--   0        0        0     6702 2023-05-03 14:22:21.309912 retentioneering-3.0.0rc3/README.md
+-rw-r--r--   0        0        0     3837 2023-05-03 14:25:06.940441 retentioneering-3.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      481 2023-05-03 07:44:34.838118 retentioneering-3.0.0rc3/retentioneering/__init__.py
+-rw-r--r--   0        0        0       25 2023-05-03 14:25:06.940441 retentioneering-3.0.0rc3/retentioneering/__version__.py
+-rw-r--r--   0        0        0       84 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc3/retentioneering/backend/__init__.py
+-rw-r--r--   0        0        0      113 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc3/retentioneering/backend/callback/__init__.py
+-rw-r--r--   0        0        0      490 2023-05-03 07:44:34.838118 retentioneering-3.0.0rc3/retentioneering/backend/callback/list_dataprocessors.py
+-rw-r--r--   0        0        0     5220 2023-05-03 07:44:34.838118 retentioneering-3.0.0rc3/retentioneering/backend/callback/mock_list_dataprocessor.py
+-rw-r--r--   0        0        0     1097 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc3/retentioneering/backend/jupiter_server.py
+-rw-r--r--   0        0        0     5293 2023-04-03 06:56:53.875728 retentioneering-3.0.0rc3/retentioneering/backend/server_manager.py
+-rw-r--r--   0        0        0      268 2023-05-03 07:44:34.838118 retentioneering-3.0.0rc3/retentioneering/backend/tracker/__init__.py
+-rw-r--r--   0        0        0     1872 2023-05-03 07:44:34.838118 retentioneering-3.0.0rc3/retentioneering/backend/tracker/connector.py
+-rw-r--r--   0        0        0     3994 2023-05-03 07:45:53.300634 retentioneering-3.0.0rc3/retentioneering/backend/tracker/tracker.py
+-rw-r--r--   0        0        0     1483 2023-05-03 07:44:34.841451 retentioneering-3.0.0rc3/retentioneering/backend/tracker/tracking_info.py
+-rw-r--r--   0        0        0       59 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc3/retentioneering/constants/__init__.py
+-rw-r--r--   0        0        0      345 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc3/retentioneering/constants/constants.py
+-rw-r--r--   0        0        0       42 2023-01-16 14:26:06.541078 retentioneering-3.0.0rc3/retentioneering/data_processor/__init__.py
+-rw-r--r--   0        0        0     2358 2023-05-03 07:44:34.841451 retentioneering-3.0.0rc3/retentioneering/data_processor/data_processor.py
+-rw-r--r--   0        0        0     1744 2023-03-07 11:03:25.184838 retentioneering-3.0.0rc3/retentioneering/data_processor/registry.py
+-rw-r--r--   0        0        0      843 2023-05-03 07:44:34.841451 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/__init__.py
+-rw-r--r--   0        0        0     4226 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/add_negative_events.py
+-rw-r--r--   0        0        0     4133 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/add_positive_events.py
+-rw-r--r--   0        0        0     2759 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/add_start_end_events.py
+-rw-r--r--   0        0        0     9279 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/collapse_loops.py
+-rw-r--r--   0        0        0     3838 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/drop_paths.py
+-rw-r--r--   0        0        0     2680 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/filter_events.py
+-rw-r--r--   0        0        0     3657 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/group_events.py
+-rw-r--r--   0        0        0     5793 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/label_cropped_paths.py
+-rw-r--r--   0        0        0     4966 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/label_lost_users.py
+-rw-r--r--   0        0        0     3517 2023-05-03 10:38:56.903565 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/label_new_users.py
+-rw-r--r--   0        0        0     1760 2023-03-17 11:02:30.068802 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/rename.py
+-rw-r--r--   0        0        0     8821 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/split_sessions.py
+-rw-r--r--   0        0        0     6904 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/data_processors_lib/truncate_paths.py
+-rw-r--r--   0        0        0       56 2023-01-16 14:26:06.544412 retentioneering-3.0.0rc3/retentioneering/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.544412 retentioneering-3.0.0rc3/retentioneering/datasets/data/__init__.py
+-rw-r--r--   0        0        0  1903381 2023-01-16 14:26:06.551078 retentioneering-3.0.0rc3/retentioneering/datasets/data/ab_test_demo.csv
+-rw-r--r--   0        0        0  1467900 2023-03-07 11:03:25.188171 retentioneering-3.0.0rc3/retentioneering/datasets/data/simple-onlineshop.csv
+-rw-r--r--   0        0        0     1352 2023-03-07 11:03:25.188171 retentioneering-3.0.0rc3/retentioneering/datasets/load.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/edgelist/__init__.py
+-rw-r--r--   0        0        0     4222 2023-04-21 11:46:51.235714 retentioneering-3.0.0rc3/retentioneering/edgelist/edgelist.py
+-rw-r--r--   0        0        0      486 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/eventstream/__init__.py
+-rw-r--r--   0        0        0    49413 2023-05-03 08:34:42.967807 retentioneering-3.0.0rc3/retentioneering/eventstream/eventstream.py
+-rw-r--r--   0        0        0      792 2023-05-03 07:44:34.841451 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/__init__.py
+-rw-r--r--   0        0        0     1711 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/add_negative_events_helper.py
+-rw-r--r--   0        0        0     1710 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/add_positive_events_helper.py
+-rw-r--r--   0        0        0     1312 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/add_start_end_events_helper.py
+-rw-r--r--   0        0        0     1772 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/collapse_loops_helper.py
+-rw-r--r--   0        0        0     1604 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/drop_paths_helper.py
+-rw-r--r--   0        0        0     1457 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/filter_events_helper.py
+-rw-r--r--   0        0        0     1813 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/group_events_helper.py
+-rw-r--r--   0        0        0     1803 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/label_cropped_paths_helper.py
+-rw-r--r--   0        0        0     1755 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/label_lost_users_helper.py
+-rw-r--r--   0        0        0     1554 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/label_new_users_helper.py
+-rw-r--r--   0        0        0      736 2023-05-03 07:44:34.841451 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/rename_helper.py
+-rw-r--r--   0        0        0     2212 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/split_sessions_helper.py
+-rw-r--r--   0        0        0     2163 2023-05-03 10:38:56.906898 retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/truncate_paths_helper.py
+-rw-r--r--   0        0        0     4157 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc3/retentioneering/eventstream/schema.py
+-rw-r--r--   0        0        0     2389 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc3/retentioneering/eventstream/types.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/exceptions/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/exceptions/base.py
+-rw-r--r--   0        0        0     1242 2023-03-22 12:39:29.884664 retentioneering-3.0.0rc3/retentioneering/exceptions/server.py
+-rw-r--r--   0        0        0      306 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/exceptions/widget.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/nodelist/__init__.py
+-rw-r--r--   0        0        0     1071 2023-04-03 06:56:53.879061 retentioneering-3.0.0rc3/retentioneering/nodelist/nodelist.py
+-rw-r--r--   0        0        0       38 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/params_model/__init__.py
+-rw-r--r--   0        0        0    11910 2023-05-03 07:44:34.841451 retentioneering-3.0.0rc3/retentioneering/params_model/params_model.py
+-rw-r--r--   0        0        0      952 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/params_model/registry.py
+-rw-r--r--   0        0        0      105 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/preprocessing_graph/__init__.py
+-rw-r--r--   0        0        0     4915 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/preprocessing_graph/nodes.py
+-rw-r--r--   0        0        0    14437 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/preprocessing_graph/preprocessing_graph.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/preprocessor/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/templates/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/templates/preprocessing_graph/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-03 10:39:03.936925 retentioneering-3.0.0rc3/retentioneering/templates/preprocessing_graph/preprocessing_graph.html
+-rw-r--r--   0        0        0      736 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/templates/preprocessing_graph/show.py
+-rw-r--r--   0        0        0       42 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/__init__.py
+-rw-r--r--   0        0        0       22 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/body.html
+-rw-r--r--   0        0        0      713 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/full.html
+-rw-r--r--   0        0        0      938 2023-05-03 10:04:24.091549 retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/init_template.py
+-rw-r--r--   0        0        0     1507 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/inner_iframe.html
+-rw-r--r--   0        0        0     1143 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/show.py
+-rw-r--r--   0        0        0      382 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/tooling/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/tooling/_describe/__init__.py
+-rw-r--r--   0        0        0     4699 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/_describe/_describe.py
+-rw-r--r--   0        0        0       46 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/tooling/_describe_events/__init__.py
+-rw-r--r--   0        0        0     4750 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/tooling/_describe_events/_describe_events.py
+-rw-r--r--   0        0        0       50 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/tooling/_transition_matrix/__init__.py
+-rw-r--r--   0        0        0     1319 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/tooling/_transition_matrix/_transition_matrix.py
+-rw-r--r--   0        0        0       31 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/tooling/clusters/__init__.py
+-rw-r--r--   0        0        0    33135 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/clusters/clusters.py
+-rw-r--r--   0        0        0     2039 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/tooling/clusters/segments.py
+-rw-r--r--   0        0        0     3166 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/tooling/clusters/userlist.py
+-rw-r--r--   0        0        0       29 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/tooling/cohorts/__init__.py
+-rw-r--r--   0        0        0    14680 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/cohorts/cohorts.py
+-rw-r--r--   0        0        0       39 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/tooling/constants/__init__.py
+-rw-r--r--   0        0        0      240 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/tooling/constants/constants.py
+-rw-r--r--   0        0        0       53 2023-01-16 14:26:06.557745 retentioneering-3.0.0rc3/retentioneering/tooling/event_timestamp_hist/__init__.py
+-rw-r--r--   0        0        0     7127 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py
+-rw-r--r--   0        0        0       27 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc3/retentioneering/tooling/funnel/__init__.py
+-rw-r--r--   0        0        0    13818 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/funnel/funnel.py
+-rw-r--r--   0        0        0       43 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/tooling/mixins/__init__.py
+-rw-r--r--   0        0        0     1516 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/tooling/mixins/ended_events.py
+-rw-r--r--   0        0        0       71 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/tooling/stattests/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-17 15:56:20.809770 retentioneering-3.0.0rc3/retentioneering/tooling/stattests/constants.py
+-rw-r--r--   0        0        0    14230 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/stattests/stattests.py
+-rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc3/retentioneering/tooling/step_matrix/__init__.py
+-rw-r--r--   0        0        0    23519 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/step_matrix/step_matrix.py
+-rw-r--r--   0        0        0       36 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc3/retentioneering/tooling/step_sankey/__init__.py
+-rw-r--r--   0        0        0    25874 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/step_sankey/step_sankey.py
+-rw-r--r--   0        0        0      110 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/tooling/timedelta_hist/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/tooling/timedelta_hist/constants.py
+-rw-r--r--   0        0        0    14302 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/timedelta_hist/timedelta_hist.py
+-rw-r--r--   0        0        0       46 2023-04-03 06:56:53.882394 retentioneering-3.0.0rc3/retentioneering/tooling/transition_graph/__init__.py
+-rw-r--r--   0        0        0    36866 2023-05-03 10:39:03.936925 retentioneering-3.0.0rc3/retentioneering/tooling/transition_graph/transition_graph.py
+-rw-r--r--   0        0        0        0 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/tooling/typing/__init__.py
+-rw-r--r--   0        0        0      171 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/tooling/typing/transition_graph/__init__.py
+-rw-r--r--   0        0        0     1327 2023-04-03 06:56:53.882394 retentioneering-3.0.0rc3/retentioneering/tooling/typing/transition_graph/graph_types.py
+-rw-r--r--   0        0        0       49 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc3/retentioneering/tooling/user_lifetime_hist/__init__.py
+-rw-r--r--   0        0        0     8218 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py
+-rw-r--r--   0        0        0      564 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/utils/__init__.py
+-rw-r--r--   0        0        0     3738 2023-05-03 08:34:42.967807 retentioneering-3.0.0rc3/retentioneering/utils/config.py
+-rw-r--r--   0        0        0     1518 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/utils/context_managers.py
+-rw-r--r--   0        0        0      122 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/utils/dict.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/utils/generator.py
+-rw-r--r--   0        0        0     2312 2023-05-03 10:04:24.091549 retentioneering-3.0.0rc3/retentioneering/utils/hwid.py
+-rw-r--r--   0        0        0      465 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc3/retentioneering/utils/list.py
+-rw-r--r--   0        0        0      444 2023-01-16 14:26:06.561078 retentioneering-3.0.0rc3/retentioneering/utils/pandas.py
+-rw-r--r--   0        0        0      986 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/utils/registry.py
+-rw-r--r--   0        0        0      293 2023-05-03 07:44:34.844784 retentioneering-3.0.0rc3/retentioneering/utils/singleton.py
+-rw-r--r--   0        0        0       77 2023-03-07 11:03:25.191505 retentioneering-3.0.0rc3/retentioneering/widget/__init__.py
+-rw-r--r--   0        0        0     7265 2023-03-22 12:39:29.887997 retentioneering-3.0.0rc3/retentioneering/widget/widgets.py
+-rw-r--r--   0        0        0     8331 1970-01-01 00:00:00.000000 retentioneering-3.0.0rc3/PKG-INFO
```

### Comparing `retentioneering-3.0.0rc1/LICENSE` & `retentioneering-3.0.0rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/backend/callback/mock_list_dataprocessor.py` & `retentioneering-3.0.0rc3/retentioneering/backend/callback/mock_list_dataprocessor.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/backend/jupiter_server.py` & `retentioneering-3.0.0rc3/retentioneering/backend/jupiter_server.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/backend/server_manager.py` & `retentioneering-3.0.0rc3/retentioneering/backend/server_manager.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/backend/tracker/connector.py` & `retentioneering-3.0.0rc3/retentioneering/backend/tracker/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,13 +48,14 @@
         except Exception:
             # supress any exceptions in tracking. Vladimir Makhanov
             return None
 
     def _prepare_data(self, data: TrackingInfo) -> dict:
         prepared_data = asdict(data)
         prepared_data["source"] = self.source
-        prepared_data["params"] = str(prepared_data["params"])
+        prepared_data["params"] = json.dumps(prepared_data["params"])
+        del prepared_data["event_time"]
         return prepared_data
 
     def send_message(self, data: TrackingInfo) -> None:
         prepared_data = self._prepare_data(data=data)
         self._post(prepared_data)
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/backend/tracker/hwid.py` & `retentioneering-3.0.0rc3/retentioneering/utils/hwid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # type: ignore
 # @FIXME: All code about subprocesses and uuids return either str or bytes or something else. Vladimir Makhanov.
-
+import os
 import platform
 import subprocess
 import uuid
 from collections import defaultdict
 
 UNDEFINED_PLATFORM_UUID = uuid.UUID("00000000-0000-0000-aaaa-eeeeeeeeeeee")
 UNDEFINED_WINDOWS_PLATFORM_UUID = uuid.UUID("00000000-0000-0000-aaaa-aaaaaaaaaaaa")
@@ -17,51 +17,57 @@
         current_machine_id = (
             str(subprocess.check_output("wmic csproduct get uuid", stderr=subprocess.DEVNULL), "utf-8")
             .split("\n")[1]
             .strip()
         )
         hwid = str(uuid.UUID(current_machine_id))
     except Exception:  # not sure if this is the right exception, but I don't know right one. Vladimir Makhanov.
-        hwid = str(UNDEFINED_WINDOWS_PLATFORM_UUID)
+        hwid = ""
     return hwid
 
 
 def get_linux_hwid() -> str:
     try:
-        hw = subprocess.check_output(["cat", "/etc/machine-id"], stderr=subprocess.DEVNULL)
-        hw = hw.decode().strip()
-        hwid = str(uuid.UUID(hw))
+        if os.access("/etc/machine-id", os.R_OK):
+            hw = subprocess.check_output(["cat", "/etc/machine-id"], stderr=subprocess.DEVNULL)
+            hw = hw.decode().strip()
+            hwid = str(uuid.UUID(hw))
+        else:
+            hwid = ""
     except Exception:  # not sure if this is the right exception, but I don't know right one. Vladimir Makhanov.
-        hwid = str(UNDEFINED_LINUX_PLATFORM_UUID)
+        hwid = ""
     return hwid
 
 
 def get_mac_hwid() -> str:
     try:
-        hw = subprocess.check_output(["cat", "/etc/machine-id"], stderr=subprocess.DEVNULL)
-        hw = hw.decode().strip()
-        hwid = str(uuid.UUID(hw))
+        if os.access("/etc/machine-id", os.R_OK):
+            hw = subprocess.check_output(["cat", "/etc/machine-id"], stderr=subprocess.DEVNULL)
+            hw = hw.decode().strip()
+            hwid = str(uuid.UUID(hw))
+        else:
+            hwid = ""
     except Exception:  # not sure if this is the right exception, but I don't know right one. Vladimir Makhanov.
-        hwid = str(UNDEFINED_MAC_PLATFORM_UUID)
+        hwid = ""
     return hwid
 
 
 def undefined_platform() -> str:
-    return str(UNDEFINED_PLATFORM_UUID)
+    return ""
 
 
 __platforms_HWID = defaultdict(default_factory=undefined_platform)
 __platforms_HWID["Windows"] = get_windows_hwid
 __platforms_HWID["Linux"] = get_linux_hwid
 __platforms_HWID["Darwin"] = get_mac_hwid
 
 
 def get_hwid() -> str:
     try:
         os_name = platform.system()
         hwid = __platforms_HWID[os_name]()
     except Exception as e:
-        hwid = UNDEFINED_PLATFORM_UUID
+        hwid = ""
     return hwid
 
 
 __all__ = ("get_hwid",)
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/backend/tracker/tracker.py` & `retentioneering-3.0.0rc3/retentioneering/backend/tracker/tracker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 import functools
+from datetime import datetime
 from typing import Any, Callable
 
+from retentioneering import RETE_CONFIG
+from retentioneering.utils.context_managers import simple_lock_context_manager
 from retentioneering.utils.singleton import Singleton
 
 from .connector import ConnectorProtocol
-from .hwid import get_hwid  # type: ignore
 from .tracking_info import TrackingInfo
 
 
 class Tracker(Singleton):
     connector: ConnectorProtocol
     enabled: bool = True
     _user_id: str | None = None
@@ -22,62 +24,91 @@
     @property
     def user_id(self) -> str:
         if self._user_id is None:
             self._user_id = self.__obtain_user_id()
         return self._user_id
 
     def __obtain_user_id(self) -> str:
-        return get_hwid()
+        return RETE_CONFIG.user.pk
 
-    def __clean_params(self, params: dict[str, Any], allowed_params: list[str] | None = None) -> dict[str, Any]:
+    def clear_params(self, params: dict[str, Any], allowed_params: list[str] | None = None) -> list[str]:
         if allowed_params is None:
             allowed_params = []
-        return {key: value for key, value in params.items() if key in allowed_params}
+        return [key for key in params.keys() if key in allowed_params]
 
     def _track_action(
-        self, called_function_params: dict[str, Any], event_name: str, event_custom_name: str, suffix: str
+        self,
+        called_function_params: list[str],
+        scope: str,
+        event_name: str,
+        event_custom_name: str,
+        event_value: str,
+        suffix: str,
+        event_time: datetime,
     ) -> None:
         if self.enabled:
             try:
-                _tracking_info_start = TrackingInfo(
-                    client_session_id=self.user_id,
-                    event_name=f"{event_name}_{suffix}",
-                    event_custom_name=event_custom_name,
+                tracking_info = TrackingInfo(
+                    user_id=self.user_id,
+                    event_name=event_name,
+                    event_custom_name=f"{event_custom_name}_{suffix}",
+                    event_value=event_value,
                     params=called_function_params,
+                    event_time=event_time,
+                    scope=scope,
                 )
-                self.connector.send_message(data=_tracking_info_start)
+                self.connector.send_message(data=tracking_info)
             except Exception:
                 # Maximum suppression. Vladimir Makhanov
                 pass
         else:
             pass
 
-    def track(self, tracking_info: dict[str, Any], allowed_params: list[str] | None = None) -> Callable:
+    def track(
+        self,
+        tracking_info: dict[str, Any],
+        scope: str,
+        event_value: str = "",
+        allowed_params: list[str] | None = None,
+    ) -> Callable:
         event_name = tracking_info["event_name"]
-        event_custom_name = tracking_info.get("event_custom_name", tracking_info["event_name"])
+        event_custom_name = tracking_info.get("event_custom_name", event_name)
 
         def tracker_decorator(func: Callable) -> Callable:
             @functools.wraps(func)
             def wrapper(*args: list[Any], **kwargs: dict[Any, Any]) -> Callable:
-                called_function_params = self.__clean_params(kwargs, allowed_params)
-
-                self._track_action(
-                    called_function_params=called_function_params,
-                    event_name=event_name,
-                    event_custom_name=event_custom_name,
-                    suffix="start",
-                )
-
-                res = func(*args, **kwargs)
-
-                self._track_action(
-                    called_function_params=called_function_params,
-                    event_name=event_name,
-                    event_custom_name=event_custom_name,
-                    suffix="end",
-                )
+                with simple_lock_context_manager as ctx:
+                    ctx.event_name = event_name
 
-                return res
+                    called_function_params = self.clear_params(kwargs, allowed_params)
+                    start_time = datetime.now()
+                    try:
+                        res = func(*args, **kwargs)
+                    except Exception as e:
+                        raise e
+
+                    end_time = datetime.now()
+
+                    if ctx.allow_action(event_name=event_name):
+                        self._track_action(
+                            called_function_params=called_function_params,
+                            scope=scope,
+                            event_name=event_name,
+                            event_custom_name=event_custom_name,
+                            event_value=event_value,
+                            event_time=start_time,
+                            suffix="start",
+                        )
+                        self._track_action(
+                            called_function_params=called_function_params,
+                            scope=scope,
+                            event_name=event_name,
+                            event_custom_name=event_custom_name,
+                            suffix="end",
+                            event_value=event_value,
+                            event_time=end_time,
+                        )
+                    return res
 
             return wrapper
 
         return tracker_decorator
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/backend/tracker/tracking_info.py` & `retentioneering-3.0.0rc3/retentioneering/backend/tracker/tracking_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 from __future__ import annotations
 
+import platform
 from dataclasses import dataclass
 from datetime import datetime
+from typing import Generator
+
+from retentioneering import __version__
+
+
+def get_index() -> Generator:
+    idx = 1
+    while True:
+        yield idx
+        idx += 1
+
+
+index = get_index()
 
 
 @dataclass
 class TrackingInfo:
-    client_session_id: str
+    user_id: str
     event_custom_name: str
     event_name: str
-    params: dict[str, str]
+    event_value: str
+    params: dict[str, str] | list[str]
+    scope: str
+    event_time: datetime
     # marketing_session_type_3_id: str # @FIXME: what is this? Vladimir Makhanov.
 
     event_date_local: str = ""
     # event_date_moscow: str    # @TODO: implement. Vladimir Makhanov
-    user_id: str = ""
     event_day_week: int = 0
     event_timestamp: int = 0
     event_timestamp_ms: int = 0
     source: str = "rete_transition_graph"
-    version: str = "3.0.0b2"
+    version: str = str(__version__)
+    os: str = platform.system()
+    index: int = 0
+    browser: str = ""
 
     def __post_init__(self) -> None:
-        current_time = datetime.now()
-        event_timestamp = current_time.timestamp()
-        tz_string = current_time.astimezone().tzname()
-        local_printable_date = current_time.strftime("%m/%d/%Y %H:%M:%S")
+        event_timestamp = self.event_time.timestamp()
+        tz_string = self.event_time.astimezone().tzname()
+        local_printable_date = self.event_time.strftime("%m/%d/%Y %H:%M:%S")
         self.event_date_local = f"{local_printable_date} GMT{tz_string}"
-        self.event_day_week = current_time.weekday()
+        self.event_day_week = self.event_time.weekday()
         self.event_timestamp = int(event_timestamp)
         self.event_timestamp_ms = int(event_timestamp * 1000)
-        self.user_id = f"{self.client_session_id}|none|none|none"
+        self.user_id = f"{self.user_id}|none|none|none"
+        self.index = next(index)
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processor/data_processor.py` & `retentioneering-3.0.0rc3/retentioneering/data_processor/data_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,7 +64,13 @@
 
     def to_dict(self) -> dict:
         data = {
             "values": self.params.dict(),
             "name": self.__class__.__name__,
         }
         return data
+
+    def copy(self) -> DataProcessor:
+        return self.__copy__()
+
+    def __copy__(self) -> DataProcessor:
+        return self.__class__(params=self.params.copy())
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processor/registry.py` & `retentioneering-3.0.0rc3/retentioneering/data_processor/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/__init__.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_negative_events.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/add_negative_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Callable, List
 
 import pandas as pd
 
+from retentioneering.backend.tracker import track
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.schema import EventstreamSchema
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfString, ReteFunction
 
 EventstreamFilter = Callable[[pd.DataFrame, EventstreamSchema], Any]
@@ -83,17 +84,27 @@
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
 
 
     """
 
     params: AddNegativeEventsParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="add_negative_events",
+        allowed_params=[],
+    )
     def __init__(self, params: AddNegativeEventsParams):
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="add_negative_events",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
 
         func = self.params.func
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_positive_events.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/add_positive_events.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Callable, List
 
 import pandas as pd
 
+from retentioneering.backend.tracker import track
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfString, ReteFunction
 
 
 def _default_func(eventstream: EventstreamType, targets: list[str]) -> pd.DataFrame:
@@ -78,17 +79,27 @@
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: AddPositiveEventsParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="add_positive_events",
+        allowed_params=[],
+    )
     def __init__(self, params: AddPositiveEventsParams):
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="add_positive_events",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
 
         func: Callable[[EventstreamType, list[str]], pd.DataFrame] = self.params.func
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/add_start_end_events.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/add_start_end_events.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import pandas as pd
 from pandas import DataFrame
 
+from retentioneering.backend.tracker import track
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 
 
 class AddStartEndEventsParams(ParamsModel):
     pass
@@ -33,17 +34,23 @@
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: AddStartEndEventsParams
 
+    @track(tracking_info={"event_name": "init"}, scope="add_start_end_events", allowed_params=[])  # type: ignore
     def __init__(self, params: AddStartEndEventsParams) -> None:
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="add_start_end_events",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         events: DataFrame = eventstream.to_dataframe(copy=True)
         user_col = eventstream.schema.user_id
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/drop_paths.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/drop_paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Optional, Tuple
 
 import numpy as np
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteTimeWidget
 
 
@@ -55,17 +56,27 @@
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: DropPathsParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="drop_paths",
+        allowed_params=[],
+    )
     def __init__(self, params: DropPathsParams):
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="drop_paths",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
 
         min_time, time_unit = None, None
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/filter_events.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/filter_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Callable
 
 import pandas as pd
-from pandas import DataFrame
+from pandas import DataFrame, Series
 
+from retentioneering.backend.tracker import track
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.schema import EventstreamSchema
 from retentioneering.eventstream.types import EventstreamSchemaType, EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteFunction
 
 
 class FilterEventsParams(ParamsModel):
     """
     A class with parameters for :py:class:`.FilterEvents` class.
 
     """
 
-    func: Callable[[DataFrame, EventstreamSchema], bool]
+    func: Callable[[DataFrame, EventstreamSchema], Series]
 
     _widgets = {
         "func": ReteFunction(),
     }
 
 
 class FilterEvents(DataProcessor):
@@ -29,36 +30,46 @@
 
     Parameters
     ----------
     func : Callable[[DataFrame, EventstreamSchema], bool]
         Custom function that returns boolean mask the same length as input ``eventstream``.
 
         - If ``True`` - the row will be left in the eventstream.
-        - If ``False`` - the row will be deleted from the eeventstream.
+        - If ``False`` - the row will be deleted from the eventstream.
 
     Returns
     -------
     Eventstream
         ``Eventstream`` with events that should be deleted from input ``eventstream``.
 
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
 
     """
 
     params: FilterEventsParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="filter_events",
+        allowed_params=[],
+    )
     def __init__(self, params: FilterEventsParams):
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="filter_events",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
-        func: Callable[[DataFrame, EventstreamSchemaType], bool] = self.params.func  # type: ignore
+        func: Callable[[DataFrame, EventstreamSchemaType], Series] = self.params.func  # type: ignore
         events: pd.DataFrame = eventstream.to_dataframe()
         mask = func(events, eventstream.schema)
         events_to_delete = events[~mask]
 
         with pd.option_context("mode.chained_assignment", None):
             events_to_delete["ref"] = events_to_delete[eventstream.schema.event_id]
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/group_events.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/group_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Callable, Optional
 
 import pandas as pd
 
+from retentioneering.backend.tracker import track
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamSchemaType, EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteFunction
 
 EventstreamFilter = Callable[[pd.DataFrame, EventstreamSchemaType], Any]
 
@@ -61,17 +62,27 @@
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: GroupEventsParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="group_events",
+        allowed_params=[],
+    )
     def __init__(self, params: GroupEventsParams) -> None:
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="group_events",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         event_name = self.params.event_name
         func: Callable = self.params.func
         event_type = self.params.event_type
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_cropped_paths.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/label_cropped_paths.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import Optional, Tuple
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteTimeWidget
 
 
@@ -73,17 +74,27 @@
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: LabelCroppedPathsParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="label_cropped_paths",
+        allowed_params=[],
+    )
     def __init__(self, params: LabelCroppedPathsParams):
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="label_cropped_paths",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         events: DataFrame = eventstream.to_dataframe(copy=True)
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
         type_col = eventstream.schema.event_type
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_lost_users.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/label_lost_users.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfInt, ReteTimeWidget
 
 
@@ -67,17 +68,27 @@
     Notes
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: LabelLostUsersParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="label_lost_users",
+        allowed_params=[],
+    )
     def __init__(self, params: LabelLostUsersParams):
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="label_lost_users",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/label_new_users.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/label_new_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import List, Literal, Union
 
 from pandas import DataFrame
 
+from retentioneering.backend.tracker import track
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ListOfIntNewUsers
 
 
 class LabelNewUsersParams(ParamsModel):
@@ -50,17 +51,27 @@
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
 
     """
 
     params: LabelNewUsersParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="label_new_users",
+        allowed_params=[],
+    )
     def __init__(self, params: LabelNewUsersParams):
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="label_new_users",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         events: DataFrame = eventstream.to_dataframe(copy=True)
         user_col = eventstream.schema.user_id
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/rename.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/rename.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/split_sessions.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/split_sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.schema import EventstreamSchema
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 from retentioneering.widget.widgets import ReteTimeWidget
 
@@ -101,17 +102,27 @@
     -----
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
 
     """
 
     params: SplitSessionsParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="split_sessions",
+        allowed_params=[],
+    )
     def __init__(self, params: SplitSessionsParams) -> None:
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="split_sessions",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
         type_col = eventstream.schema.event_type
         event_col = eventstream.schema.event_name
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/data_processors_lib/truncate_paths.py` & `retentioneering-3.0.0rc3/retentioneering/data_processors_lib/truncate_paths.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Literal, Optional
 
 import pandas as pd
 
+from retentioneering.backend.tracker import track
 from retentioneering.data_processor import DataProcessor
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.params_model import ParamsModel
 
 
 class TruncatePathsParams(ParamsModel):
     """
@@ -61,17 +62,27 @@
     path does not change.
 
     See :doc:`Data processors user guide</user_guides/dataprocessors>` for the details.
     """
 
     params: TruncatePathsParams
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="truncate_paths",
+        allowed_params=[],
+    )
     def __init__(self, params: TruncatePathsParams):
         super().__init__(params=params)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "apply"},
+        scope="truncate_paths",
+        allowed_params=[],
+    )
     def apply(self, eventstream: EventstreamType) -> EventstreamType:
         from retentioneering.eventstream.eventstream import Eventstream
 
         user_col = eventstream.schema.user_id
         time_col = eventstream.schema.event_timestamp
         event_col = eventstream.schema.event_name
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/datasets/data/ab_test_demo.csv` & `retentioneering-3.0.0rc3/retentioneering/datasets/data/ab_test_demo.csv`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/datasets/data/simple-onlineshop.csv` & `retentioneering-3.0.0rc3/retentioneering/datasets/data/simple-onlineshop.csv`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/datasets/load.py` & `retentioneering-3.0.0rc3/retentioneering/datasets/load.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/edgelist/edgelist.py` & `retentioneering-3.0.0rc3/retentioneering/edgelist/edgelist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/eventstream.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/eventstream.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,45 +156,56 @@
 
     """
 
     schema: EventstreamSchema
     index_order: IndexOrder
     relations: List[Relation]
     _preprocessing_graph: PreprocessingGraph | None = None
+    __clusters: Clusters | None = None
 
     __raw_data_schema: RawDataSchemaType
     __events: pd.DataFrame | pd.Series[Any]
-    __clusters: Clusters | None = None
-    __funnel: Funnel | None = None
-    __cohorts: Cohorts | None = None
-    __step_matrix: StepMatrix | None = None
-    __sankey: StepSankey | None = None
-    __stattests: StatTests | None = None
+    __funnel: Funnel
+    __cohorts: Cohorts
+    __step_matrix: StepMatrix
+    __sankey: StepSankey
+    __stattests: StatTests
     __transition_graph: TransitionGraph
-    __timedelta_hist: TimedeltaHist | None = None
-    __user_lifetime_hist: UserLifetimeHist | None = None
-    __event_timestamp_hist: EventTimestampHist | None = None
+    __timedelta_hist: TimedeltaHist
+    __user_lifetime_hist: UserLifetimeHist
+    __event_timestamp_hist: EventTimestampHist
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="eventstream",
+        allowed_params=[
+            "raw_data",
+            "raw_data_schema",
+            "schema",
+            "prepare",
+            "index_order",
+            "relations",
+            "user_sample_size",
+            "user_sample_seed",
+        ],
+    )
     def __init__(
         self,
         raw_data: pd.DataFrame | pd.Series[Any],
         raw_data_schema: RawDataSchema
         | RawDataSchemaType
         | dict[str, str | list[RawDataCustomColSchema]]
         | None = None,
         schema: EventstreamSchema | None = None,
         prepare: bool = True,
         index_order: Optional[IndexOrder] = None,
         relations: Optional[List[Relation]] = None,
         user_sample_size: Optional[int | float] = None,
         user_sample_seed: Optional[int] = None,
     ) -> None:
-        self.__clusters = None
-        self.__funnel = None
-
         self.schema = schema if schema else EventstreamSchema()
 
         if not raw_data_schema:
             raw_data_schema = RawDataSchema()
             if "event_type" in raw_data.columns:
                 raw_data_schema.event_type = "event_type"
         elif isinstance(raw_data_schema, dict):
@@ -212,14 +223,19 @@
         else:
             self.relations = relations
         self.__events = self.__prepare_events(raw_data) if prepare else raw_data
         self.__events = self.__required_cleanup(events=self.__events)
         self.index_events()
         self._preprocessing_graph = None
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "copy"},
+        scope="eventstream",
+        allowed_params=[],
+    )
     def copy(self) -> Eventstream:
         """
         Make a copy of current ``eventstream``.
 
         Returns
         -------
         Eventstream
@@ -230,14 +246,19 @@
             raw_data=self.__events.copy(),
             schema=self.schema.copy(),
             prepare=False,
             index_order=self.index_order.copy(),
             relations=self.relations.copy(),
         )
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "append_eventstream"},
+        scope="eventstream",
+        allowed_params=[],
+    )
     def append_eventstream(self, eventstream: Eventstream) -> None:  # type: ignore
         """
         Append ``eventstream`` with the same schema.
 
         Parameters
         ----------
         eventstream : Eventstream
@@ -253,53 +274,72 @@
         """
         if not self.schema.is_equal(eventstream.schema):
             raise ValueError("invalid schema: joined eventstream")
 
         curr_events = self.to_dataframe(raw_cols=True, show_deleted=True)
         new_events = eventstream.to_dataframe(raw_cols=True, show_deleted=True)
 
-        curr_deleted_events = curr_events[curr_events[DELETE_COL_NAME] == True]
-        new_deleted_events = new_events[new_events[DELETE_COL_NAME] == True]
-        deleted_events = pd.concat([curr_deleted_events, new_deleted_events])
-        deleted_events = deleted_events.drop_duplicates(subset=[self.schema.event_id])
-
         merged_events = pd.merge(
             curr_events,
             new_events,
             left_on=self.schema.event_id,
             right_on=self.schema.event_id,
             how="outer",
             indicator=True,
         )
 
-        left_events = merged_events[(merged_events["_merge"] == "left_only") | (merged_events["_merge"] == "both")]
+        left_delete_col = f"{DELETE_COL_NAME}_x"
+        right_delete_col = f"{DELETE_COL_NAME}_y"
+
+        merged_events[left_delete_col] = merged_events[left_delete_col].astype("bool")
+        merged_events[right_delete_col] = merged_events[right_delete_col].astype("bool")
+
+        left_events = merged_events[(merged_events["_merge"] == "left_only")]
+        both_events = merged_events[(merged_events["_merge"] == "both")]
         right_events = merged_events[(merged_events["_merge"] == "right_only")]
 
+        both_events_deleted = both_events[both_events[left_delete_col] & both_events[right_delete_col]].copy()
+        both_events_deleted_left = both_events[both_events[left_delete_col] & ~both_events[right_delete_col]].copy()
+        both_events_deleted_right = both_events[~both_events[left_delete_col] & both_events[right_delete_col]].copy()
+        both_events_not_deleted = both_events[~both_events[left_delete_col] & ~both_events[right_delete_col]].copy()
+
+        right_events = pd.concat([right_events, both_events_deleted_left, both_events_not_deleted])
+        left_events = pd.concat([left_events, both_events_deleted_right])
+
         left_raw_cols = self._get_raw_cols()
         right_raw_cols = eventstream._get_raw_cols()
         cols = self.schema.get_cols()
 
         result_left_part = pd.DataFrame()
         result_right_part = pd.DataFrame()
+        result_both_part = pd.DataFrame()
 
-        for col in cols:
-            result_left_part[col] = get_merged_col(df=left_events, colname=col, suffix="_x")
-            result_right_part[col] = get_merged_col(df=right_events, colname=col, suffix="_y")
-
-        for col in left_raw_cols:
-            result_left_part[col] = get_merged_col(df=left_events, colname=col, suffix="_x")
-
-        for col in right_raw_cols:
-            result_right_part[col] = get_merged_col(df=right_events, colname=col, suffix="_y")
-
-        result_left_part[DELETE_COL_NAME] = get_merged_col(df=left_events, colname=DELETE_COL_NAME, suffix="_x")
-        result_right_part[DELETE_COL_NAME] = get_merged_col(df=right_events, colname=DELETE_COL_NAME, suffix="_y")
+        with warnings.catch_warnings():
+            # disable warning for pydantic schema Callable type
+            warnings.simplefilter(action="ignore", category=FutureWarning)
+
+            for col in cols:
+                result_left_part[col] = get_merged_col(df=left_events, colname=col, suffix="_x")
+                result_both_part[col] = get_merged_col(df=both_events_deleted, colname=col, suffix="_x")
+                result_right_part[col] = get_merged_col(df=right_events, colname=col, suffix="_y")
+
+            for col in left_raw_cols:
+                result_both_part[col] = get_merged_col(df=both_events_deleted, colname=col, suffix="_x")
+                result_left_part[col] = get_merged_col(df=left_events, colname=col, suffix="_x")
+
+            for col in right_raw_cols:
+                result_right_part[col] = get_merged_col(df=right_events, colname=col, suffix="_y")
+
+            result_left_part[DELETE_COL_NAME] = get_merged_col(df=left_events, colname=DELETE_COL_NAME, suffix="_x")
+            result_both_part[DELETE_COL_NAME] = get_merged_col(
+                df=both_events_deleted, colname=DELETE_COL_NAME, suffix="_x"
+            )
+            result_right_part[DELETE_COL_NAME] = get_merged_col(df=right_events, colname=DELETE_COL_NAME, suffix="_y")
 
-        self.__events = pd.concat([result_left_part, result_right_part])
-        self._soft_delete(deleted_events)
+        self.__events = pd.concat([result_left_part, result_both_part, result_right_part])
         self.index_events()
 
     def _join_eventstream(self, eventstream: Eventstream) -> None:  # type: ignore
         if not self.schema.is_equal(eventstream.schema):
             raise ValueError("invalid schema: joined eventstream")
 
         relation_i = find_index(
@@ -325,49 +365,52 @@
             right_on=relation_col_name,
             how="outer",
             indicator=True,
         )
 
         left_id_colname = f"{self.schema.event_id}_y"
 
-        both_events = merged_events[(merged_events["_merge"] == "both")]
         left_events = merged_events[(merged_events["_merge"] == "left_only")]
-        right_events = merged_events[
-            (merged_events["_merge"] == "both") | (merged_events[left_id_colname].isin(not_related_events_ids))
-        ]
+        both_events = merged_events[(merged_events["_merge"] == "both")]
+        right_events = merged_events[(merged_events[left_id_colname].isin(not_related_events_ids))]
 
         left_raw_cols = self._get_raw_cols()
         right_raw_cols = eventstream._get_raw_cols()
         cols = self._get_both_cols(eventstream)
 
         result_left_part = pd.DataFrame()
         result_right_part = pd.DataFrame()
-        result_deleted_events = pd.DataFrame()
+        result_both_part = pd.DataFrame()
 
         for col in cols:
             result_left_part[col] = get_merged_col(df=left_events, colname=col, suffix="_x")
-            result_deleted_events[col] = get_merged_col(df=both_events, colname=col, suffix="_x")
             result_right_part[col] = get_merged_col(df=right_events, colname=col, suffix="_y")
+            result_both_part[col] = get_merged_col(df=both_events, colname=col, suffix="_y")
 
         for col in left_raw_cols:
+            result_both_part[col] = get_merged_col(df=both_events, colname=col, suffix="_x")
             result_left_part[col] = get_merged_col(df=left_events, colname=col, suffix="_x")
-            result_deleted_events[col] = get_merged_col(df=both_events, colname=col, suffix="_x")
 
         for col in right_raw_cols:
             result_right_part[col] = get_merged_col(df=right_events, colname=col, suffix="_y")
 
         result_left_part[DELETE_COL_NAME] = get_merged_col(df=left_events, colname=DELETE_COL_NAME, suffix="_x")
 
-        result_deleted_events[DELETE_COL_NAME] = True
-
-        left_delete_col = f"{DELETE_COL_NAME}_x"
         right_delete_col = f"{DELETE_COL_NAME}_y"
-        result_right_part[DELETE_COL_NAME] = right_events[left_delete_col] | right_events[right_delete_col]
+        result_right_part[DELETE_COL_NAME] = right_events[right_delete_col]
+        result_both_part[DELETE_COL_NAME] = both_events[right_delete_col]
+
+        result_both_part[self.schema.event_id] = get_merged_col(
+            df=both_events, colname=self.schema.event_id, suffix="_x"
+        )
+        with warnings.catch_warnings():
+            # disable warning for pydantic schema Callable type
+            warnings.simplefilter(action="ignore", category=FutureWarning)
+            self.__events = pd.concat([result_left_part, result_right_part, result_both_part])
 
-        self.__events = pd.concat([result_left_part, result_right_part, result_deleted_events])
         self.__events[self.schema.user_id] = self.__events[self.schema.user_id].astype(user_id_type)
 
         self.schema.custom_cols = self._get_both_custom_cols(eventstream)
         self.index_events()
 
     def _get_both_custom_cols(self, eventstream: Eventstream) -> list[str]:
         self_custom_cols = set(self.schema.custom_cols)
@@ -407,14 +450,19 @@
         if show_deleted:
             cols.append(DELETE_COL_NAME)
 
         events = self.__events if show_deleted else self.__get_not_deleted_events()
         view = pd.DataFrame(events, columns=cols, copy=copy)
         return view
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "index_events"},
+        scope="eventstream",
+        allowed_params=[],
+    )
     def index_events(self) -> None:
         """
         Sort and index eventstream using DEFAULT_INDEX_ORDER.
 
         Returns
         -------
         None
@@ -443,14 +491,19 @@
         cols = self.__events.columns
         relation_cols: list[str] = []
         for col in cols:
             if col.startswith("ref_"):  # type: ignore
                 relation_cols.append(col)  # type: ignore
         return relation_cols
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "add_custom_col"},
+        scope="eventstream",
+        allowed_params=["name", "data"],
+    )
     def add_custom_col(self, name: str, data: pd.Series[Any] | None) -> None:
         """
         Add custom column to an existing ``eventstream``.
 
         Parameters
         ----------
         name : str
@@ -608,14 +661,27 @@
             return raw_data
         if user_sample_seed is not None:
             np.random.seed(user_sample_seed)
         sample_users = np.random.choice(unique_users, sample_size, replace=False)
         raw_data_sampled = raw_data.loc[raw_data[user_col_name].isin(sample_users), :]  # type: ignore
         return raw_data_sampled
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="funnel",
+        event_value="plot",
+        allowed_params=[
+            "stages",
+            "stage_names",
+            "funnel_type",
+            "segments",
+            "segment_names",
+            "show_plot",
+        ],
+    )
     def funnel(
         self,
         stages: list[str],
         stage_names: list[str] | None = None,
         funnel_type: Literal["open", "closed", "hybrid"] = "closed",
         segments: Collection[Collection[int]] | None = None,
         segment_names: list[str] | None = None,
@@ -663,14 +729,31 @@
         --------
         .Clusters
         """
         if self.__clusters is None:
             self.__clusters = Clusters(eventstream=self)
         return self.__clusters
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="step_matrix",
+        event_value="plot",
+        allowed_params=[
+            "max_steps",
+            "weight_col",
+            "precision",
+            "targets",
+            "accumulated",
+            "sorting",
+            "threshold",
+            "centered",
+            "groups",
+            "show_plot",
+        ],
+    )
     def step_matrix(
         self,
         max_steps: int = 20,
         weight_col: str | None = None,
         precision: int = 2,
         targets: list[str] | str | None = None,
         accumulated: Literal["both", "only"] | None = None,
@@ -709,14 +792,29 @@
             centered=centered,
             groups=groups,
         )
         if show_plot:
             self.__step_matrix.plot()
         return self.__step_matrix
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="step_sankey",
+        event_value="plot",
+        allowed_params=[
+            "max_steps",
+            "threshold",
+            "sorting",
+            "targets",
+            "autosize",
+            "width",
+            "height",
+            "show_plot",
+        ],
+    )
     def step_sankey(
         self,
         max_steps: int = 10,
         threshold: int | float = 0.05,
         sorting: list | None = None,
         targets: list[str] | str | None = None,
         autosize: bool = True,
@@ -744,14 +842,30 @@
 
         self.__sankey.fit(max_steps=max_steps, threshold=threshold, sorting=sorting, targets=targets)
         if show_plot:
             figure = self.__sankey.plot(autosize=autosize, width=width, height=height)
             figure.show()
         return self.__sankey
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="cohorts",
+        event_value="heatmap",
+        allowed_params=[
+            "cohort_start_unit",
+            "cohort_period",
+            "average",
+            "cut_bottom",
+            "cut_right",
+            "cut_diagonal",
+            "width",
+            "height",
+            "show_plot",
+        ],
+    )
     def cohorts(
         self,
         cohort_start_unit: DATETIME_UNITS,
         cohort_period: Tuple[int, DATETIME_UNITS],
         average: bool = True,
         cut_bottom: int = 0,
         cut_right: int = 0,
@@ -786,14 +900,26 @@
             cut_right=cut_right,
             cut_diagonal=cut_diagonal,
         )
         if show_plot:
             self.__cohorts.heatmap(width=width, height=height)
         return self.__cohorts
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="stattests",
+        event_value="display_results",
+        allowed_params=[
+            "test",
+            "groups",
+            "func",
+            "group_names",
+            "alpha",
+        ],
+    )
     def stattests(
         self,
         test: STATTEST_NAMES,
         groups: Tuple[list[str | int], list[str | int]],
         func: Callable,
         group_names: Tuple[str, str] = ("group_1", "group_2"),
         alpha: float = 0.05,
@@ -812,14 +938,34 @@
             A ``StatTest`` class instance fitted to the given parameters.
         """
         self.__stattests = StatTests(eventstream=self)
         self.__stattests.fit(groups=groups, func=func, test=test, group_names=group_names, alpha=alpha)
         self.__stattests.display_results()
         return self.__stattests
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="timedelta_hist",
+        event_value="plot",
+        allowed_params=[
+            "raw_events_only",
+            "event_pair",
+            "adjacent_events_only",
+            "weight_col",
+            "time_agg",
+            "timedelta_unit",
+            "log_scale",
+            "lower_cutoff_quantile",
+            "upper_cutoff_quantile",
+            "bins",
+            "width",
+            "height",
+            "show_plot",
+        ],
+    )
     def timedelta_hist(
         self,
         raw_events_only: bool = False,
         event_pair: list[str | Literal[EVENTSTREAM_GLOBAL_EVENTS]] | None = None,
         adjacent_events_only: bool = True,
         weight_col: str | None = None,
         time_agg: AGGREGATION_NAMES | None = None,
@@ -870,14 +1016,29 @@
             self.__timedelta_hist.plot(
                 width=width,
                 height=height,
             )
 
         return self.__timedelta_hist
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="user_lifetime_hist",
+        event_value="plot",
+        allowed_params=[
+            "timedelta_unit",
+            "log_scale",
+            "lower_cutoff_quantile",
+            "upper_cutoff_quantile",
+            "bins",
+            "width",
+            "height",
+            "show_plot",
+        ],
+    )
     def user_lifetime_hist(
         self,
         timedelta_unit: DATETIME_UNITS = "s",
         log_scale: bool | tuple[bool, bool] | None = None,
         lower_cutoff_quantile: float | None = None,
         upper_cutoff_quantile: float | None = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
@@ -913,14 +1074,29 @@
             upper_cutoff_quantile=upper_cutoff_quantile,
             bins=bins,
         )
         if show_plot:
             self.__user_lifetime_hist.plot(width=width, height=height)
         return self.__user_lifetime_hist
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="event_timestamp_hist",
+        event_value="plot",
+        allowed_params=[
+            "event_list",
+            "raw_events_only",
+            "lower_cutoff_quantile",
+            "upper_cutoff_quantile",
+            "bins",
+            "width",
+            "height",
+            "show_plot",
+        ],
+    )
     def event_timestamp_hist(
         self,
         event_list: list[str] | None = None,
         raw_events_only: bool = False,
         lower_cutoff_quantile: float | None = None,
         upper_cutoff_quantile: float | None = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
@@ -956,14 +1132,23 @@
             upper_cutoff_quantile=upper_cutoff_quantile,
             bins=bins,
         )
         if show_plot:
             self.__event_timestamp_hist.plot(width=width, height=height)
         return self.__event_timestamp_hist
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="describe",
+        event_value="_values",
+        allowed_params=[
+            "session_col",
+            "raw_events_only",
+        ],
+    )
     def describe(self, session_col: str = "session_id", raw_events_only: bool = False) -> pd.DataFrame:
         """
         Display general eventstream information. If ``session_col`` is present in eventstream, also
         output session statistics.
 
         Parameters
         ----------
@@ -997,14 +1182,24 @@
         See :ref:`Eventstream user guide<eventstream_describe>` for the details.
 
 
         """
         describer = _Describe(eventstream=self, session_col=session_col, raw_events_only=raw_events_only)
         return describer._values()
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="describe_events",
+        event_value="_values",
+        allowed_params=[
+            "session_col",
+            "raw_events_only",
+            "event_list",
+        ],
+    )
     def describe_events(
         self, session_col: str = "session_id", raw_events_only: bool = False, event_list: list[str] | None = None
     ) -> pd.DataFrame:
         """
         Display general information on eventstream events. If ``session_col`` is present in eventstream, also
         output session statistics.
 
@@ -1069,39 +1264,46 @@
         """
         describer = _DescribeEvents(
             eventstream=self, session_col=session_col, event_list=event_list, raw_events_only=raw_events_only
         )
         return describer._values()
 
     @track(  # type: ignore
-        tracking_info={"event_name": "transition_graph", "event_custom_name": "transition_graph_helper"},
+        tracking_info={"event_name": "helper"},
+        scope="transition_graph",
+        event_value="plot",
         allowed_params=[
             "edges_norm_type",
             "targets",
             "nodes_threshold",
             "edges_threshold",
             "nodes_weight_col",
             "edges_weight_col",
             "custom_weight_cols",
             "width",
             "height",
+            "show_weights",
+            "show_percents",
+            "show_nodes_names",
+            "show_all_edges_for_targets",
+            "show_nodes_without_links",
         ],
     )
     def transition_graph(
         self,
         edges_norm_type: NormType = None,
         nodes_norm_type: NormType = None,
         targets: MutableMapping[str, str | None] | None = None,
         nodes_threshold: Threshold | None = None,
         edges_threshold: Threshold | None = None,
         nodes_weight_col: str | None = None,
         edges_weight_col: str | None = None,
         custom_weight_cols: list[str] | None = None,
         width: int = 960,
-        height: int = 900,
+        height: int = 600,
         show_weights: bool = True,
         show_percents: bool = False,
         show_nodes_names: bool = True,
         show_all_edges_for_targets: bool = True,
         show_nodes_without_links: bool = False,
     ) -> TransitionGraph:
         """
@@ -1133,26 +1335,50 @@
             show_percents=show_percents,
             show_nodes_names=show_nodes_names,
             show_all_edges_for_targets=show_all_edges_for_targets,
             show_nodes_without_links=show_nodes_without_links,
         )
         return self.__transition_graph
 
-    def preprocessing_graph(self) -> PreprocessingGraph:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="preprocessing_graph",
+        event_value="display",
+        allowed_params=[
+            "width",
+            "height",
+        ],
+    )
+    def preprocessing_graph(self, width: int = 960, height: int = 600) -> PreprocessingGraph:
         """
         Display the preprocessing GUI tool.
+
+        Parameters
+        ----------
+        width : int, default 960
+            Width of plot in pixels.
+        height : int, default 600
+            Height of plot in pixels.
+
+        Returns
+        -------
+        PreprocessingGraph
+            Rendered preprocessing graph.
         """
         if self._preprocessing_graph is None:
             self._preprocessing_graph = PreprocessingGraph(source_stream=self)
-        self._preprocessing_graph.display()
+        self._preprocessing_graph.display(width=width, height=height)
+
         return self._preprocessing_graph
 
     @track(  # type: ignore
-        tracking_info={"event_name": "transition_matrix", "event_custom_name": "transition_matrix_helper"},
+        tracking_info={"event_name": "helper"},
         allowed_params=["weight_col", "norm_type"],
+        scope="transition_matrix",
+        event_value="_values",
     )
     def transition_matrix(self, weight_col: str | None = None, norm_type: NormType = None) -> pd.DataFrame:
         """
         Get transition weights as a matrix for each unique pair of events. The calculation logic is the same
         that is used for edge weights calculation of transition graph.
 
         Parameters
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/__init__.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_negative_events_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/add_negative_events_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 from __future__ import annotations
 
 from typing import Callable, List, Optional
 
+from retentioneering.backend.tracker import track
+
 from ..types import EventstreamType
 
 
 class AddNegativeEventsHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="add_negative_events",
+        event_value="combine",
+        allowed_params=[
+            "targets",
+            "func",
+        ],
+    )
     def add_negative_events(self, targets: List[str], func: Optional[Callable] = None) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates new synthetic
         events in paths of all users having the specified events - ``negative_target_RAW_EVENT_NAME``.
 
         Parameters
         ----------
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_positive_events_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/add_positive_events_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 from __future__ import annotations
 
 from typing import Callable, List, Optional
 
+from retentioneering.backend.tracker import track
+
 from ..types import EventstreamType
 
 
 class AddPositiveEventsHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="add_negative_events",
+        event_value="combine",
+        allowed_params=[
+            "targets",
+            "func",
+        ],
+    )
     def add_positive_events(self, targets: List[str], func: Optional[Callable] = None) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates new synthetic
         events in paths of all users having the specified events - ``positive_target_RAW_EVENT_NAME``.
 
         Parameters
         ----------
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/add_start_end_events_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/add_start_end_events_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from __future__ import annotations
 
+from retentioneering.backend.tracker import track
+
 from ..types import EventstreamType
 
 
 class AddStartEndEventsHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="add_negative_events",
+        event_value="combine",
+        allowed_params=[],
+    )
     def add_start_end_events(self) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates
         two synthetic events in each user's path: ``path_start`` and ``path_end``.
 
         Returns
         -------
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/collapse_loops_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/collapse_loops_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 from __future__ import annotations
 
 from typing import Literal, Union
 
+from retentioneering.backend.tracker import track
+
 from ..types import EventstreamType
 
 
 class CollapseLoopsHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="collapse_loops",
+        event_value="combine",
+        allowed_params=[
+            "suffix",
+            "time_agg",
+        ],
+    )
     def collapse_loops(
         self,
         suffix: Union[Literal["loop", "count"], None] = None,
-        time_agg: Literal["max", "min", "mean"] = "max",
+        time_agg: Literal["max", "min", "mean"] = "min",
     ) -> EventstreamType:
         """
         A method of ``Eventstream`` class that finds ``loops`` and creates new synthetic events
         in paths of all users having such sequences.
 
         A ``loop`` - is a sequence of repetitive events.
         For example *"event1 -> event1"*
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/drop_paths_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/drop_paths_helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 from __future__ import annotations
 
 from typing import Tuple
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 
 from ..types import EventstreamType
 
 
 class DropPathsHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="drop_paths",
+        event_value="combine",
+        allowed_params=[
+            "min_steps",
+            "min_time",
+        ],
+    )
     def drop_paths(
         self, min_steps: int | None = None, min_time: Tuple[float, DATETIME_UNITS] | None = None
     ) -> EventstreamType:
         """
         A method of ``Eventstream`` class that deletes users' paths that are shorter than the specified
         number of events or cut_off.
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/filter_events_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/filter_events_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 from __future__ import annotations
 
-from typing import Any, Callable
+from typing import Callable
 
-from pandas import DataFrame
+from pandas import DataFrame, Series
+
+from retentioneering.backend.tracker import track
 
 from ..types import EventstreamSchemaType, EventstreamType
 
 
 class FilterEventsHelperMixin:
-    def filter_events(self, func: Callable[[DataFrame, EventstreamSchemaType], Any]) -> EventstreamType:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="add_negative_events",
+        event_value="combine",
+        allowed_params=[
+            "func",
+        ],
+    )
+    def filter_events(self, func: Callable[[DataFrame, EventstreamSchemaType], Series]) -> EventstreamType:
         """
         A method of ``Eventstream`` class that filters input ``eventstream`` based on custom conditions.
 
         Parameters
         ----------
         See parameters description
             :py:class:`.FilterEvents`
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_cropped_paths_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/label_cropped_paths_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 from __future__ import annotations
 
 from typing import Optional, Tuple
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 
 from ..types import EventstreamType
 
 
 class LabelCroppedPathsHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="label_cropped_paths",
+        event_value="combine",
+        allowed_params=[
+            "left_cutoff",
+            "right_cutoff",
+        ],
+    )
     def label_cropped_paths(
         self,
         left_cutoff: Optional[Tuple[float, DATETIME_UNITS]],
         right_cutoff: Optional[Tuple[float, DATETIME_UNITS]],
     ) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates new synthetic event(s) for each user based
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_lost_users_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/label_lost_users_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 from __future__ import annotations
 
 from typing import List, Optional, Tuple
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 
 from ..types import EventstreamType
 
 
 class LabelLostUsersHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="label_lost_users",
+        event_value="combine",
+        allowed_params=[
+            "timeout",
+            "lost_users_list",
+        ],
+    )
     def label_lost_users(
         self, timeout: Optional[Tuple[float, DATETIME_UNITS]] = None, lost_users_list: Optional[List[int]] = None
     ) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates one
         of the synthetic events in each user's path: ``lost_user`` or ``absent_user`` .
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/label_new_users_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/label_new_users_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 from __future__ import annotations
 
 from typing import List, Literal, Union
 
+from retentioneering.backend.tracker import track
+
 from ..types import EventstreamType
 
 
 class LabelNewUsersHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="label_new_users",
+        event_value="combine",
+        allowed_params=[
+            "new_users_list",
+        ],
+    )
     def label_new_users(self, new_users_list: Union[List[int], Literal["all"]]) -> EventstreamType:
         """
         A method of ``Eventstream`` class that creates one
         of the synthetic events in each user's path: ``new_user`` or ``existing_user`` .
 
         Parameters
         ----------
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/rename_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/rename_helper.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/split_sessions_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/split_sessions_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 from __future__ import annotations
 
 from typing import Optional, Tuple
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 
 from ..types import EventstreamType
 
 
 class SplitSessionsHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="split_sessions",
+        event_value="combine",
+        allowed_params=[
+            "timeout",
+            "session_col",
+            "mark_truncated",
+        ],
+    )
     def split_sessions(
         self,
         timeout: Tuple[float, DATETIME_UNITS],
         session_col: str = "session_id",
         mark_truncated: Optional[bool] = False,
     ) -> EventstreamType:
         """
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/helpers/truncate_paths_helper.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/helpers/truncate_paths_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 from __future__ import annotations
 
 from typing import Literal, Optional
 
+from retentioneering.backend.tracker import track
+
 from ..types import EventstreamType
 
 
 class TruncatePathsHelperMixin:
+    @track(  # type: ignore
+        tracking_info={"event_name": "helper"},
+        scope="truncate_paths",
+        event_value="combine",
+        allowed_params=[
+            "drop_before",
+            "drop_after",
+            "occurrence_before",
+            "occurrence_after",
+            "shift_before",
+            "shift_after",
+        ],
+    )
     def truncate_paths(
         self,
         drop_before: Optional[str] = None,
         drop_after: Optional[str] = None,
         occurrence_before: Literal["first", "last"] = "first",
         occurrence_after: Literal["first", "last"] = "first",
         shift_before: int = 0,
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/schema.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/schema.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/eventstream/types.py` & `retentioneering-3.0.0rc3/retentioneering/eventstream/types.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/exceptions/server.py` & `retentioneering-3.0.0rc3/retentioneering/exceptions/server.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/nodelist/nodelist.py` & `retentioneering-3.0.0rc3/retentioneering/nodelist/nodelist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/params_model/params_model.py` & `retentioneering-3.0.0rc3/retentioneering/params_model/params_model.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/params_model/registry.py` & `retentioneering-3.0.0rc3/retentioneering/params_model/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/nodes.py` & `retentioneering-3.0.0rc3/retentioneering/preprocessing_graph/nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,24 +29,36 @@
         if self.description:
             data["description"] = self.description
 
         if processor := getattr(self, "processor", None):
             data["processor"] = processor.to_dict()
         return data
 
+    def copy(self) -> BaseNode:
+        return BaseNode()
+
 
 class SourceNode(BaseNode):
     events: EventstreamType
     description: Optional[str]
 
     def __init__(self, source: EventstreamType, description: Optional[str] = None) -> None:
         super().__init__()
         self.events = source
         self.description = description
 
+    def __copy__(self) -> SourceNode:
+        return SourceNode(
+            source=self.events.copy(),
+            description=self.description,
+        )
+
+    def copy(self) -> SourceNode:
+        return self.__copy__()
+
 
 class EventsNode(BaseNode):
     """
     Class for regular nodes of a PreprocessingGraph.
 
     Notes
     -----
@@ -69,14 +81,23 @@
         self.processor = processor
         self.events = None
         self.description = description
 
     def calc_events(self, parent: EventstreamType) -> None:
         self.events = self.processor.apply(parent)
 
+    def __copy__(self) -> EventsNode:
+        return EventsNode(
+            processor=self.processor.copy(),
+            description=self.description,
+        )
+
+    def copy(self) -> EventsNode:
+        return self.__copy__()
+
 
 class MergeNode(BaseNode):
     """
     Class for merging nodes of a PreprocessingGraph.
 
     Notes
     -----
@@ -94,14 +115,22 @@
     description: Optional[str]
 
     def __init__(self, description: Optional[str] = None) -> None:
         super().__init__()
         self.events = None
         self.description = description
 
+    def __copy__(self) -> MergeNode:
+        return MergeNode(
+            description=self.description,
+        )
+
+    def copy(self) -> MergeNode:
+        return self.__copy__()
+
 
 Node = Union[SourceNode, EventsNode, MergeNode]
 nodes = {
     "MergeNode": MergeNode,
     "EventsNode": EventsNode,
     "SourceNode": SourceNode,
 }
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/preprocessing_graph/preprocessing_graph.py` & `retentioneering-3.0.0rc3/retentioneering/preprocessing_graph/preprocessing_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,18 +210,28 @@
             raise ValueError("node already exists!")
 
     def __validate_not_found(self, nodes: List[Node]) -> None:
         for node in nodes:
             if node not in self._ngraph.nodes:
                 raise ValueError("node not found!")
 
-    def display(self, width: int = 960, height: int = 900) -> DisplayHandle:
+    def display(self, width: int = 960, height: int = 600) -> DisplayHandle:
         """
         Show constructed ``PreprocessingGraph``.
 
+        Parameters
+        ----------
+        width : int, default 960
+            Width of plot in pixels.
+        height : int, default 600
+            Height of plot in pixels.
+
+        Returns
+        -------
+            Rendered preprocessing graph.
         """
         if not self.__server_manager:
             self.__server_manager = ServerManager()
 
         if not self.__server:
             self.__server = self.__server_manager.create_server()
             self.__server.register_action("list-dataprocessor-mock", list_dataprocessor_mock)
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/preprocessing_graph.html` & `retentioneering-3.0.0rc3/retentioneering/templates/preprocessing_graph/preprocessing_graph.html`

 * *Files 22% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     iframe.contentWindow.__HEIGHT__ = height
 
     const fDocument = iframe.contentDocument
     const container = fDocument.createElement("div")
     container.id = "root"
 
     const script = fDocument.createElement("script")
-    script.src = "https://static.server.retentioneering.com/viztools/preprocessing-graph/v3/preprocessing-graph.umd.js?block={{block_id}}"
+    script.src = "https://static.server.retentioneering.com/package/@rete/preprocessing-graph/version/1/dist/preprocessing-graph.umd.js?block={{block_id}}"
     script.type = "text/javascript"
 
     const link = fDocument.createElement("link")
     link.rel = "stylesheet"
-    link.href = "https://static.server.retentioneering.com/viztools/preprocessing-graph/v3/style.css?block={{block_id}}"
+    link.href = "https://static.server.retentioneering.com/package/@rete/preprocessing-graph/version/1/dist/style.css?block={{block_id}}"
 
     const font1 = fDocument.createElement("link")
     font1.rel = "stylesheet"
     font1.href = "https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap"
 
     const font2 = fDocument.createElement("link")
     font2.rel = "stylesheet"
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/templates/preprocessing_graph/show.py` & `retentioneering-3.0.0rc3/retentioneering/templates/preprocessing_graph/show.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/full.html` & `retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/full.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/init_template.py` & `retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/init_template.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,10 +15,11 @@
     selectedLinksWeightForThresholds: '{selected_links_weight_for_thresholds}',
     showWeights: {show_weights},
     showPercents: {show_percents},
     showNodesNames: {show_nodes_names},
     showAllEdgesForTargets: {show_all_edges_for_targets},
     showNodesWithoutLinks: {show_nodes_without_links},
     useLayoutDump: Boolean({layout_dump}),
-    weightTemplate: {weight_template}
+    weightTemplate: {weight_template},
+    trackingHWID: '{tracking_hardware_id}'
 }})
 """
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/inner_iframe.html` & `retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/inner_iframe.html`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/templates/transition_graph/show.py` & `retentioneering-3.0.0rc3/retentioneering/templates/transition_graph/show.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/_describe/_describe.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/_describe/_describe.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,16 +68,17 @@
 
     def _output_df_construction(
         self, values_overall: list[timedelta64 | int | float], values_time_events: list[timedelta64 | int | float]
     ) -> pd.DataFrame:
         overall_index = pd.MultiIndex.from_product(self.overall_stats, names=self.INDEX_NAMES)
         time_events_index = pd.MultiIndex.from_product(self.time_events_stats, names=self.INDEX_NAMES)
 
-        df_overall = pd.DataFrame(data=values_overall, index=overall_index, columns=self.OUT_COLS)
-        df_time_events = pd.DataFrame(data=values_time_events, index=time_events_index, columns=self.OUT_COLS)
+        # TODO внезапно в старом коде появилась ошибка типов, разобраться
+        df_overall = pd.DataFrame(data=values_overall, index=overall_index, columns=self.OUT_COLS)  # type: ignore
+        df_time_events = pd.DataFrame(data=values_time_events, index=time_events_index, columns=self.OUT_COLS)  # type: ignore
 
         return pd.concat([df_overall, df_time_events])
 
     def _values(self) -> pd.DataFrame:
         max_time = self.df[self.time_col].max()
         min_time = self.df[self.time_col].min()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/_describe_events/_describe_events.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/_describe_events/_describe_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/_transition_matrix/_transition_matrix.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/_transition_matrix/_transition_matrix.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/clusters/clusters.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/clusters/clusters.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from matplotlib import axes, rcParams
 from numpy import ndarray
 from sklearn.cluster import KMeans
 from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
 from sklearn.manifold import TSNE
 from sklearn.mixture import GaussianMixture
 
+from retentioneering.backend.tracker import track
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.clusters.segments import Segments
 
 FeatureType = Literal["tfidf", "count", "frequency", "binary", "time", "time_fraction", "markov"]
 SklearnFeatureType = Literal["count", "frequency", "tfidf", "binary"]
 NgramRange = Tuple[int, int]
 Method = Literal["kmeans", "gmm"]
@@ -39,14 +40,19 @@
     .Eventstream.clusters : Call Clusters tool as an eventstream method.
 
     Notes
     -----
     See :doc:`Clusters user guide</user_guides/clusters>` for the details.
     """
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="clusters",
+        allowed_params=[],
+    )
     def __init__(self, eventstream: EventstreamType):
         self.__eventstream: EventstreamType = eventstream
         self.user_col = eventstream.schema.user_id
         self.event_col = eventstream.schema.event_name
         self.time_col = eventstream.schema.event_timestamp
         self.event_index_col = eventstream.schema.event_index
 
@@ -58,20 +64,25 @@
         self._method: Method | None = None
         self._n_clusters: int | None = None
         self._user_clusters: pd.Series | None = None
         self._X: pd.DataFrame | None = None
 
     # public API
 
-    def fit(
-        self,
-        method: Method,
-        n_clusters: int,
-        X: pd.DataFrame,
-    ) -> Clusters:
+    @track(  # type: ignore
+        tracking_info={"event_name": "fit"},
+        scope="clusters",
+        allowed_params=[
+            "method",
+            "n_clusters",
+            "X",
+            "random_state",
+        ],
+    )
+    def fit(self, method: Method, n_clusters: int, X: pd.DataFrame, random_state: int | None = None) -> Clusters:
         """
         Prepare features and compute clusters for the input eventstream data.
 
         Parameters
         ----------
         method : {"kmeans", "gmm"}
             - ``kmeans`` stands for the classic K-means algorithm.
@@ -79,35 +90,49 @@
             - ``gmm`` stands for Gaussian mixture model. See details in :sklearn_gmm:`sklearn documentation<>`.
 
         n_clusters : int
             The expected number of clusters to be passed to a clustering algorithm.
         X : pd.DataFrame
             ``pd.DataFrame`` representing a custom vectorization of the user paths. The index corresponds to user_ids,
             the columns are vectorized values of the path. See :py:func:`extract_features`.
+        random_state : int, optional
+            Use an int to make the randomness deterministic. Calling ``fit`` multiple times with the same
+            ``random_state`` leads to the same clustering results.
 
         Returns
         -------
         Clusters
             A fitted ``Clusters`` instance.
         """
 
         self._method, self._n_clusters, self._X = self.__validate_input(method, n_clusters, X)
 
-        self.__cluster_result = self._prepare_clusters()
+        self.__cluster_result = self._prepare_clusters(random_state=random_state)
         self._user_clusters = self.__cluster_result.copy()
 
         self.__segments = Segments(
             eventstream=self.__eventstream,
             segments_df=self.__cluster_result.to_frame("segment").reset_index(),
         )
 
         self.__is_fitted = True
 
         return self
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "diff"},
+        scope="clusters",
+        allowed_params=[
+            "cluster_id1",
+            "cluster_id2",
+            "top_n_events",
+            "weight_col",
+            "targets",
+        ],
+    )
     def diff(
         self,
         cluster_id1: int | str,
         cluster_id2: int | str | None = None,
         top_n_events: int = 8,
         weight_col: str | None = None,
         targets: list[str] | None = None,
@@ -208,14 +233,21 @@
             target_pos=target_separator_position,
             targets=targets,
             cl2=cluster_id2,
         )
 
         return figure
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "plot"},
+        scope="clusters",
+        allowed_params=[
+            "targets",
+        ],
+    )
     def plot(self, targets: list[str] | list[list[str]] | None = None) -> go.Figure:
         """
         Plot a bar plot illustrating the cluster sizes and the conversion rates of
         the ``target`` events within the clusters. Should be used after :py:func:`fit` or :py:func:`set_clusters`.
 
         Parameters
         ----------
@@ -230,14 +262,19 @@
         return self._cluster_bar(
             clusters=self.__cluster_result.values,  # type: ignore
             target=cast(List[List[bool]], targets_bool),  # @TODO: fix types. Vladimir Makhanov
             target_names=target_names,
         )
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "user_clusters"},
+        scope="clusters",
+        allowed_params=[],
+    )
     def user_clusters(self) -> pd.Series | None:
         """
 
         Returns
         -------
         pd.Series
             ``user_id -> cluster_id`` mapping representing as ``pd.Series``. The index corresponds to
@@ -245,14 +282,19 @@
         """
         if not self.__is_fitted:
             raise RuntimeError("Clusters are not defined. Consider to run 'fit()' or `set_clusters()` methods.")
 
         return self.__cluster_result
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "cluster_mapping"},
+        scope="clusters",
+        allowed_params=[],
+    )
     def cluster_mapping(self) -> dict:
         """
         Return calculated before ``cluster_id -> list[user_ids]`` mapping.
 
         Returns
         -------
         dict
@@ -263,21 +305,33 @@
 
         df = self.__cluster_result.to_frame("cluster_id").reset_index()
         user_col, cluster_col = df.columns
         cluster_map = df.groupby(cluster_col)[user_col].apply(list)  # type: ignore
         return cluster_map.to_dict()
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "params"},
+        scope="clusters",
+        allowed_params=[],
+    )
     def params(self) -> dict:
         """
         Returns the parameters used for the last fitting.
 
         """
         return {"method": self._method, "n_clusters": self._n_clusters, "X": self._X}
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "set_clusters"},
+        scope="clusters",
+        allowed_params=[
+            "user_clusters",
+        ],
+    )
     def set_clusters(self, user_clusters: pd.Series) -> Clusters:
         """
         Set custom user-cluster mapping.
 
         Parameters
         ----------
         user_clusters : pd.Series
@@ -292,14 +346,19 @@
         self._user_clusters = user_clusters
         self.__cluster_result = user_clusters.copy()
         self._n_clusters = user_clusters.nunique()
         self._method = None
         self.__is_fitted = True
         return self
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "filter_cluster"},
+        scope="clusters",
+        allowed_params=["cluster_id"],
+    )
     def filter_cluster(self, cluster_id: int | str) -> EventstreamType:
         """
         Truncate the eventstream, leaving the trajectories of the users who belong to the selected cluster.
         Should be used after :py:func:`fit` or :py:func:`set_clusters`.
 
         Parameters
         ----------
@@ -330,14 +389,22 @@
         es = Eventstream(
             raw_data=df,
             raw_data_schema=eventstream.schema.to_raw_data_schema(),
             schema=eventstream.schema.copy(),
         )
         return es
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "extract_features"},
+        scope="clusters",
+        allowed_params=[
+            "feature_type",
+            "ngram_range",
+        ],
+    )
     def extract_features(self, feature_type: FeatureType, ngram_range: NgramRange | None = None) -> pd.DataFrame:
         """
         Calculate vectorized user paths.
 
         Parameters
         ----------
         feature_type : {"tfidf", "count", "frequency", "binary", "markov", "time", "time_fraction"}
@@ -396,14 +463,23 @@
                 )
 
         if vec_data is not None:
             vec_data.columns = [f"{col}_{feature_type}" for col in vec_data.columns]  # type: ignore
 
         return cast(pd.DataFrame, vec_data)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "projection"},
+        scope="clusters",
+        allowed_params=[
+            "method",
+            "targets",
+            "color_type",
+        ],
+    )
     def projection(
         self,
         method: PlotProjectionMethod = "tsne",
         targets: list[str] | None = None,
         color_type: Literal["targets", "clusters"] = "clusters",
         **kwargs: Any,
     ) -> go.Figure:
@@ -501,23 +577,23 @@
         if not isinstance(X, pd.DataFrame):  # type: ignore
             raise ValueError("X is not a DataFrame!")
         if np.all(np.all(X.dtypes == "float") and X.isna().sum().sum() != 0):
             raise ValueError("X is wrong formatted! NaN should be replaced with 0 and all dtypes must be float!")
 
         return _method, _n_clusters, X
 
-    def _prepare_clusters(self) -> pd.Series:
+    def _prepare_clusters(self, random_state: int | None) -> pd.Series:
         user_clusters = pd.Series(dtype=np.int64)
 
         features = self._X.copy()  # type: ignore
         if self._n_clusters is not None:
             if self._method == "kmeans":
-                cluster_result = self._kmeans(features=features, n_clusters=self._n_clusters)
+                cluster_result = self._kmeans(features=features, n_clusters=self._n_clusters, random_state=random_state)
             elif self._method == "gmm":
-                cluster_result = self._gmm(features=features, n_clusters=self._n_clusters)
+                cluster_result = self._gmm(features=features, n_clusters=self._n_clusters, random_state=random_state)
             else:
                 raise ValueError("Unknown method: %s" % self._method)
 
             user_clusters = pd.Series(cluster_result, index=features.index)
 
         return user_clusters
 
@@ -687,21 +763,21 @@
         ymin, ymax = bar.get_ylim()
         if ymax > 1:
             bar.set_ylim(ymin, 1.05)
 
         return bar
 
     @staticmethod
-    def _kmeans(features: pd.DataFrame, n_clusters: int = 8, random_state: int = 0) -> np.ndarray:
+    def _kmeans(features: pd.DataFrame, random_state: int | None, n_clusters: int = 8) -> np.ndarray:
         km = KMeans(random_state=random_state, n_clusters=n_clusters)
         cl = km.fit_predict(features.values)
         return cl
 
     @staticmethod
-    def _gmm(features: pd.DataFrame, n_clusters: int = 8, random_state: int = 0) -> np.ndarray:
+    def _gmm(features: pd.DataFrame, random_state: int | None, n_clusters: int = 8) -> np.ndarray:
         km = GaussianMixture(random_state=random_state, n_components=n_clusters)
         cl = km.fit_predict(features.values)
         return cl
 
     def _prepare_targets(self, targets: list[str] | list[list[str]] | None) -> tuple[list[str], list[ndarray]]:
         events = self.__eventstream.to_dataframe()
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/clusters/segments.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/clusters/segments.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/clusters/userlist.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/clusters/userlist.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/cohorts/cohorts.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/cohorts/cohorts.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS, DATETIME_UNITS_LIST
 from retentioneering.eventstream.types import EventstreamType
 
 # @TODO Подумать над сокращением списка поддерживаемых типов для когорт? dpanina
 
 
 class Cohorts:
@@ -45,14 +46,19 @@
 
     average: bool
     cut_bottom: int
     cut_right: int
     cut_diagonal: int
     _cohort_matrix_result: pd.DataFrame
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="cohorts",
+        allowed_params=[],
+    )
     def __init__(self, eventstream: EventstreamType):
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
 
         self._cohort_matrix_result = pd.DataFrame()
@@ -112,14 +118,26 @@
         df: pd.DataFrame, cut_bottom: int = 0, cut_right: int = 0, cut_diagonal: int = 0
     ) -> pd.DataFrame:
         for row in df.index:
             df.loc[row, max(0, df.loc[row].notna()[::-1].idxmax() + 1 - cut_diagonal) :] = None  # type: ignore
 
         return df.iloc[: len(df) - cut_bottom, : len(df.columns) - cut_right]
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "fit"},
+        scope="cohorts",
+        allowed_params=[
+            "cohort_start_unit",
+            "cohort_period",
+            "average",
+            "cut_bottom",
+            "cut_right",
+            "cut_diagonal",
+        ],
+    )
     def fit(
         self,
         cohort_start_unit: DATETIME_UNITS,
         cohort_period: Tuple[int, DATETIME_UNITS],
         average: bool = True,
         cut_bottom: int = 0,
         cut_right: int = 0,
@@ -226,14 +244,22 @@
         )
         user_retention.index = user_retention.index.astype(str)
         if self.average:
             user_retention.loc["Average"] = user_retention.mean()
 
         self._cohort_matrix_result = user_retention
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "heatmap"},
+        scope="cohorts",
+        allowed_params=[
+            "width",
+            "height",
+        ],
+    )
     def heatmap(self, width: float = 5.0, height: float = 5.0) -> matplotlib.axes.Axes:
         """
         Builds a heatmap based on the calculated cohort matrix values.
         Should be used after :py:func:`fit`.
 
         Parameters
         ----------
@@ -250,14 +276,23 @@
 
         df = self._cohort_matrix_result
         figsize = (width, height)
         figure, ax = plt.subplots(figsize=figsize)
         sns.heatmap(df, annot=True, fmt=".1%", linewidths=1, linecolor="gray", ax=ax)
         return ax
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "lineplot"},
+        scope="cohorts",
+        allowed_params=[
+            "plot_type",
+            "width",
+            "height",
+        ],
+    )
     def lineplot(
         self, plot_type: Literal["cohorts", "average", "all"] = "cohorts", width: float = 7.0, height: float = 5.0
     ) -> matplotlib.axes.Axes:
         """
         Create a chart representing each cohort dynamics over time.
         Should be used after :py:func:`fit`.
 
@@ -298,27 +333,37 @@
 
         ax.legend(loc="upper left", bbox_to_anchor=(1, 1))
         ax.set_xlabel("Period from the start of observation")
         ax.set_ylabel("Share of active users")
         return ax
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "values"},
+        scope="cohorts",
+        allowed_params=[],
+    )
     def values(self) -> pd.DataFrame:
         """
         Returns a pd.DataFrame representing the calculated cohort matrix values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
         pd.DataFrame
 
         """
         return self._cohort_matrix_result
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "params"},
+        scope="cohorts",
+        allowed_params=[],
+    )
     def params(self) -> dict[str, DATETIME_UNITS | tuple | bool | int | None]:
         """
         Returns the parameters used for the last fitting.
         Should be used after :py:func:`fit`.
 
         """
         return {
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/event_timestamp_hist/event_timestamp_hist.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
+from retentioneering.backend.tracker import track
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.constants import BINS_ESTIMATORS
 
 
 class EventTimestampHist:
     """
     Plot the distribution of events over time. Can be useful for detecting
@@ -39,14 +40,19 @@
     event_list: list[str] | None
     lower_cutoff_quantile: float | None
     upper_cutoff_quantile: float | None
     bins: int | Literal[BINS_ESTIMATORS]
     bins_to_show: np.ndarray
     values_to_plot: np.ndarray
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="event_timestamp_hist",
+        allowed_params=[],
+    )
     def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
 
         self.bins_to_show = np.array([])
@@ -75,14 +81,25 @@
 
         if lower_cutoff_quantile is not None and upper_cutoff_quantile is not None:
             if lower_cutoff_quantile > upper_cutoff_quantile:
                 warnings.warn("lower_cutoff_quantile exceeds upper_cutoff_quantile; no data passed to the histogram")
 
         return upper_cutoff_quantile, lower_cutoff_quantile
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "fit"},
+        scope="event_timestamp_hist",
+        allowed_params=[
+            "raw_events_only",
+            "event_list",
+            "lower_cutoff_quantile",
+            "upper_cutoff_quantile",
+            "bins",
+        ],
+    )
     def fit(
         self,
         raw_events_only: bool = False,
         event_list: list[str] | None = None,
         lower_cutoff_quantile: float | None = None,
         upper_cutoff_quantile: float | None = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
@@ -136,27 +153,40 @@
         if len(values_to_plot) == 0:
             bins_to_show = np.array([])
 
         self.bins_to_show = bins_to_show  # type: ignore
         self.values_to_plot = values_to_plot  # type: ignore
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "values"},
+        scope="event_timestamp_hist",
+        allowed_params=[],
+    )
     def values(self) -> tuple[np.ndarray, np.ndarray]:
         """
 
         Returns
         -------
         tuple(np.ndarray, np.ndarray)
 
             1. The first array contains the values for histogram.
             2. The first array contains the bin edges.
 
         """
         return self.values_to_plot, self.bins_to_show
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "plot"},
+        scope="event_timestamp_hist",
+        allowed_params=[
+            "width",
+            "height",
+        ],
+    )
     def plot(self, width: float = 6.0, height: float = 4.5) -> matplotlib.axes.Axesne:
         """
         Create a sns.histplot based on the calculated values.
 
         Parameters
         ----------
         width : float, default 6.0
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/funnel/funnel.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/funnel/funnel.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections.abc import Collection
 from typing import Any, Literal
 
 import pandas as pd
 import plotly.graph_objects as go
 from pandas.core.common import flatten
 
+from retentioneering.backend.tracker import track
 from retentioneering.eventstream.types import EventstreamType
 
 FunnelTypes = Literal["open", "closed", "hybrid"]
 
 
 class Funnel:
     """
@@ -41,14 +42,19 @@
     stages: list[str]
     stage_names: list[str] | None
     funnel_type: FunnelTypes
     segments: Collection[Collection[int]] | None
     segment_names: list[str] | None
     __res_dict: dict[str, dict]
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="funnel",
+        allowed_params=[],
+    )
     def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.__res_dict = {}
 
@@ -196,14 +202,25 @@
                 )
                 df.drop(columns="min_date", inplace=True)
             else:
                 df = df.drop(df[~df[self.user_col].isin(user_stage)].index.tolist())
 
         return vals, df
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "fit"},
+        scope="funnel",
+        allowed_params=[
+            "stages",
+            "stage_names",
+            "funnel_type",
+            "segments",
+            "segment_names",
+        ],
+    )
     def fit(
         self,
         stages: list[str],
         stage_names: list[str] | None = None,
         funnel_type: FunnelTypes = "closed",
         segments: Collection[Collection[int]] | None = None,
         segment_names: list[str] | None = None,
@@ -262,14 +279,19 @@
                 data=data,
                 stages=self.stages,
                 segments=self.segments,
                 segment_names=self.segment_names,
                 stage_names=self.stage_names,
             )
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "plot"},
+        scope="funnel",
+        allowed_params=[],
+    )
     def plot(self) -> go.Figure:
         """
         Create a funnel plot based on the calculated funnel values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
@@ -278,14 +300,19 @@
         """
         result_dict = self.__res_dict
         data = self._calculate_plot_data(plot_params=result_dict)
         figure = self._plot_stacked_funnel(data=data)
         return figure
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "values"},
+        scope="funnel",
+        allowed_params=[],
+    )
     def values(self) -> pd.DataFrame:
         """
         Returns a pd.DataFrame representing the calculated funnel values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
@@ -313,14 +340,19 @@
             result_list.append(result_)
 
         result_df = pd.concat(result_list).set_index(["segment_name", "stages"])
 
         return result_df
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "params"},
+        scope="funnel",
+        allowed_params=[],
+    )
     def params(self) -> dict:
         """
         Returns the parameters used for the last fitting.
 
         """
 
         return {
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/mixins/ended_events.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/mixins/ended_events.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/stattests/stattests.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/stattests/stattests.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import plotly.graph_objects as go
 import seaborn as sns
 from scipy.stats import chi2_contingency, fisher_exact, ks_2samp, mannwhitneyu
 from scipy.stats.contingency import crosstab
 from statsmodels.stats.power import TTestIndPower
 from statsmodels.stats.weightstats import ttest_ind, ztest
 
+from retentioneering.backend.tracker import track
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.stattests.constants import STATTEST_NAMES
 
 
 def _effect_size_cohend(sample1: list, sample2: list) -> float:
     """
     Calculate an effect size value using Cohen’s D measure (difference between two means).
@@ -96,14 +97,19 @@
     g2_data: list[str | int]
 
     is_fitted: bool
     output_template_numerical = "{0} (mean ± SD): {1:.3f} ± {2:.3f}, n = {3}"
     output_template_categorical = "{0} (size): n = {1}"
     p_val, power, label_min, label_max = 0.0, 0.0, "", ""
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="stattests",
+        allowed_params=[],
+    )
     def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
 
         self.g1_data = list()
@@ -182,14 +188,25 @@
         else:
             p_val = p_val_rev
             power = power_rev
             label_max = self.group_names[1]
             label_min = self.group_names[0]
         return p_val, power, label_max, label_min
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "fit"},
+        scope="stattests",
+        allowed_params=[
+            "test",
+            "groups",
+            "func",
+            "group_names",
+            "alpha",
+        ],
+    )
     def fit(
         self,
         test: STATTEST_NAMES,
         groups: Tuple[list[str | int], list[str | int]],
         func: Callable,
         group_names: Tuple[str, str] = ("group_1", "group_2"),
         alpha: float = 0.05,
@@ -230,14 +247,19 @@
         self.group_names = group_names
         self.alpha = alpha
 
         self.g1_data, self.g2_data = self._get_group_values()
         self.p_val, self.power, self.label_min, self.label_max = self._get_sorted_test_results()
         self.is_fitted = True
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "plot"},
+        scope="stattests",
+        allowed_params=[],
+    )
     def plot(self) -> Tuple[go.Figure, str]:
         """
         Plots a barplot comparing the metric values between two groups.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
@@ -247,14 +269,19 @@
         data2 = pd.DataFrame(data={"data": self.g2_data, "groups": self.group_names[1]})
         combined_stats = pd.concat([data1, data2]).reset_index()
         compare_plot = sns.displot(data=combined_stats, x="data", hue="groups", multiple="dodge")
         compare_plot.set(xlabel=None)
         return compare_plot
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "values"},
+        scope="stattests",
+        allowed_params=[],
+    )
     def values(self) -> dict:
         """
         Returns the comprehensive results of the comparison between the two groups.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
@@ -287,14 +314,19 @@
                 "group_two_size": len(self.g2_data),
                 "p_val": self.p_val,
             }
         else:
             raise ValueError("Wrong test passed")
         return res_dict
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "display_results"},
+        scope="stattests",
+        allowed_params=[],
+    )
     def display_results(self) -> None:
         if not self.is_fitted:
             raise ValueError("The StatTests instance needs to be fitted before displaying results")
         values = self.values
         if self.test in ["ztest", "ttest", "mannwhitneyu", "ks_2samp"]:
             print(
                 self.output_template_numerical.format(
@@ -316,14 +348,19 @@
             print(self.output_template_categorical.format(values["group_one_name"], values["group_one_size"]))
             print(self.output_template_categorical.format(values["group_two_name"], values["group_two_size"]))
             print("Group difference test with p-value: {:.5f}".format(values["p_val"]))
         else:
             raise ValueError("Wrong test passed")
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "params"},
+        scope="stattests",
+        allowed_params=[],
+    )
     def params(self) -> dict:
         """
         Returns the parameters used for the last fitting.
         Should be used after :py:func:`fit`.
 
         """
         return {
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/step_matrix/step_matrix.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/step_matrix/step_matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dataclasses import dataclass
 from typing import Literal, Tuple
 
 import matplotlib
 import pandas as pd
 import seaborn as sns
 
+from retentioneering.backend.tracker import track
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.mixins.ended_events import EndedEventsMixin
 
 
 @dataclass
 class CenteredParams:
     event: str
@@ -60,18 +61,35 @@
     groups: Tuple[list, list] | None = None
 
     __result_data: pd.DataFrame
     __result_targets: pd.DataFrame | None
     _fraction_title: str | None
     _targets_list: list[list[str]] | None
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="step_matrix",
+        allowed_params=[
+            "max_steps",
+            "weight_col",
+            "precision",
+            "targets",
+            "accumulated",
+            "sorting",
+            "threshold",
+            "centered",
+            "groups",
+        ],
+    )
     def __init__(
         self,
         eventstream: EventstreamType,
     ) -> None:
+        super().__init__()
+
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.event_index_col = self.__eventstream.schema.event_index
 
         self.__result_data = pd.DataFrame()
@@ -328,14 +346,29 @@
             if self.centered is not None:
                 centered_position = self.centered.left_gap
                 axs.vlines(
                     [centered_position - 0.02, centered_position + 0.98], *axs.get_ylim(), colors="Black", linewidth=0.7
                 )
         return axs
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "fit"},
+        scope="step_matrix",
+        allowed_params=[
+            "max_steps",
+            "weight_col",
+            "precision",
+            "targets",
+            "accumulated",
+            "sorting",
+            "threshold",
+            "centered",
+            "groups",
+        ],
+    )
     def fit(
         self,
         max_steps: int = 20,
         weight_col: str | None = None,
         precision: int = 2,
         targets: list[str] | str | None = None,
         accumulated: Literal["both", "only"] | None = None,
@@ -489,42 +522,57 @@
                 piv_targets.columns = [f"{int(i) - window - 1}" for i in piv_targets.columns]  # type: ignore
 
         self.__result_data = piv
         self.__result_targets = piv_targets
         self._fraction_title = fraction_title
         self._targets_list = targets_plot
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "plot"},
+        scope="step_matrix",
+        allowed_params=[],
+    )
     def plot(self) -> matplotlib.axes.Axes:
         """
         Create a heatmap plot based on the calculated step matrix values.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
         matplotlib.axes.Axes
 
         """
         axes = self._render_plot(self.__result_data, self.__result_targets, self._targets_list, self._fraction_title)
         return axes
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "values"},
+        scope="step_matrix",
+        allowed_params=[],
+    )
     def values(self) -> tuple[pd.DataFrame, pd.DataFrame | None]:
         """
         Returns the calculated step matrix as a pd.DataFrame.
         Should be used after :py:func:`fit`.
 
         Returns
         -------
         tuple[pd.DataFrame, pd.DataFrame | None]
             1. Stands for the step matrix.
             2. Stands for a separate step matrix related for target events only.
         """
         return self.__result_data, self.__result_targets
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "params"},
+        scope="step_matrix",
+        allowed_params=[],
+    )
     def params(self) -> dict:
         """
         Returns the parameters used for the last fitting.
         Should be used after :py:func:`fit`.
 
         """
         return {
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/step_sankey/step_sankey.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/step_sankey/step_sankey.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Dict
 
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 import seaborn as sns
 
+from retentioneering.backend.tracker import track
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.mixins.ended_events import EndedEventsMixin
 
 
 class StepSankey(EndedEventsMixin):
     """
     A class for the visualization of user paths in stepwise manner using Sankey diagram.
@@ -32,23 +33,24 @@
 
     """
 
     max_steps: int
     threshold: int | float
     sorting: list | None
     targets: list[str] | str | None
-    autosize: bool
-    width: int | None
-    height: int | None
 
     data_grp_nodes: pd.DataFrame
     data: pd.DataFrame
     data_grp_links: pd.DataFrame
     data_for_plot: dict
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="step_sankey",
+    )
     def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.event_index_col = self.__eventstream.schema.event_index
 
@@ -257,15 +259,22 @@
         data = data.loc[data["step"] <= self.max_steps, :]
 
         # TODO: Do we really need to replace NA values?
         # NOTE skip mean calculating error
         data["time_to_next"].fillna(data["time_to_next"].min(), inplace=True)
         return data
 
-    def _render_plot(self, data_for_plot: dict, data_grp_nodes: pd.DataFrame) -> go.Figure:
+    def _render_plot(
+        self,
+        data_for_plot: dict,
+        data_grp_nodes: pd.DataFrame,
+        autosize: bool = True,
+        width: int | None = None,
+        height: int | None = None,
+    ) -> go.Figure:
         # NOTE fill lists for plot
         targets = []
         sources = []
         values = []
         time_to_next = []
         for source_key in data_for_plot["links_dict"].keys():
             for target_key, target_value in data_for_plot["links_dict"][source_key].items():
@@ -311,17 +320,15 @@
                         label=time_to_next,
                         hovertemplate="%{value} unique users went from %{source.label} to %{target.label}.<br />"
                         + "<br />It took them %{label} in average.<extra></extra>",
                     ),
                 )
             ]
         )
-        fig.update_layout(
-            font=dict(size=15), plot_bgcolor="white", autosize=self.autosize, width=self.width, height=self.height
-        )
+        fig.update_layout(font=dict(size=15), plot_bgcolor="white", autosize=autosize, width=width, height=height)
 
         return fig
 
     def _get_links(
         self, data: pd.DataFrame, data_for_plot: dict, data_grp_nodes: pd.DataFrame
     ) -> tuple[dict, pd.DataFrame]:
         # NOTE create links aggregated dataframe
@@ -502,14 +509,24 @@
         grouped = data.groupby(self.user_col)
         data["next_event"] = grouped[self.event_col].shift(-1)
         data["next_timestamp"] = grouped[self.time_col].shift(-1)
         data["time_to_next"] = data["next_timestamp"] - data[self.time_col]
         data = data.drop("next_timestamp", axis=1)
         return data
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "fit"},
+        scope="step_sankey",
+        allowed_params=[
+            "max_steps",
+            "threshold",
+            "sorting",
+            "targets",
+        ],
+    )
     def fit(
         self,
         max_steps: int = 10,
         threshold: int | float = 0.05,
         sorting: list | None = None,
         targets: list[str] | str | None = None,
     ) -> None:
@@ -553,14 +570,23 @@
         self.sorting = sorting
         self.targets = targets
 
         self.data = self._prepare_data(data)
         data_for_plot, self.data_grp_nodes = self._get_nodes(self.data)
         self.data_for_plot, self.data_grp_links = self._get_links(self.data, data_for_plot, self.data_grp_nodes)
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "plot"},
+        scope="step_sankey",
+        allowed_params=[
+            "autosize",
+            "width",
+            "height",
+        ],
+    )
     def plot(self, autosize: bool = True, width: int | None = None, height: int | None = None) -> go.Figure:
         """
         Create a Sankey interactive plot based on the calculated values.
         Should be used after :py:func:`fit`.
 
         Parameters
         ----------
@@ -573,21 +599,29 @@
 
         Returns
         -------
         plotly.graph_objects.Figure
 
         """
 
-        self.autosize = autosize
-        self.width = width
-        self.height = height
-        figure = self._render_plot(self.data_for_plot, self.data_grp_nodes)
+        figure = self._render_plot(
+            data_for_plot=self.data_for_plot,
+            data_grp_nodes=self.data_grp_nodes,
+            autosize=autosize,
+            width=width,
+            height=height,
+        )
         return figure
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "values"},
+        scope="step_sankey",
+        allowed_params=[],
+    )
     def values(self) -> tuple[pd.DataFrame, pd.DataFrame]:
         """
         Returns two pd.DataFrames which the Sankey diagram is based on.
 
         Should be used after :py:func:`fit`.
 
         Returns
@@ -596,22 +630,24 @@
             1. Contains the nodes of the diagram.
             2. Contains the edges of the diagram.
 
         """
         return self.data_grp_nodes, self.data_grp_links
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "params"},
+        scope="step_sankey",
+        allowed_params=[],
+    )
     def params(self) -> dict:
         """
         Returns the parameters used for the last fitting.
         Should be used after :py:func:`fit`.
 
         """
         return {
             "max_steps": self.max_steps,
             "threshold": self.threshold,
             "sorting": self.sorting,
             "targets": self.targets,
-            "autosize": self.autosize,
-            "width": self.width,
-            "height": self.height,
         }
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/timedelta_hist/timedelta_hist.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/timedelta_hist/timedelta_hist.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.constants import BINS_ESTIMATORS
 from retentioneering.tooling.timedelta_hist.constants import (
     AGGREGATION_NAMES,
     EVENTSTREAM_GLOBAL_EVENTS,
 )
@@ -61,14 +62,19 @@
     log_scale: bool | tuple[bool, bool] | None
     lower_cutoff_quantile: float | None
     upper_cutoff_quantile: float | None
     bins: int | Literal[BINS_ESTIMATORS]
     bins_to_show: np.ndarray
     values_to_plot: np.ndarray
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="timedelta_hist",
+        allowed_params=[],
+    )
     def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
         self.type_col = self.__eventstream.schema.event_type
         self.bins_to_show = np.array([])
@@ -140,14 +146,30 @@
             else:
                 log_scale = log_scale
         else:
             log_scale = (False, False)
 
         return log_scale, upper_cutoff_quantile, lower_cutoff_quantile
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "fit"},
+        scope="timedelta_hist",
+        allowed_params=[
+            "raw_events_only",
+            "event_pair",
+            "adjacent_events_only",
+            "weight_col",
+            "time_agg",
+            "timedelta_unit",
+            "log_scale",
+            "lower_cutoff_quantile",
+            "upper_cutoff_quantile",
+            "bins",
+        ],
+    )
     def fit(
         self,
         raw_events_only: bool = False,
         event_pair: Optional[list[str | EVENTSTREAM_GLOBAL_EVENTS]] = None,
         adjacent_events_only: bool = True,
         weight_col: str | None = None,
         time_agg: Optional[AGGREGATION_NAMES] = None,
@@ -260,26 +282,39 @@
             bins_to_show = np.histogram_bin_edges(values_to_plot, bins=self.bins)
         if len(values_to_plot) == 0:
             bins_to_show = np.array([])
         self.bins_to_show = bins_to_show
         self.values_to_plot = values_to_plot  # type: ignore
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "values"},
+        scope="timedelta_hist",
+        allowed_params=[],
+    )
     def values(self) -> tuple[np.ndarray, np.ndarray]:
         """
 
         Returns
         -------
         tuple(np.ndarray, np.ndarray)
 
             1. The first array contains the values for histogram.
             2. The first array contains the bin edges.
         """
         return self.values_to_plot, self.bins_to_show
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "plot"},
+        scope="timedelta_hist",
+        allowed_params=[
+            "width",
+            "height",
+        ],
+    )
     def plot(self, width: float = 6.0, height: float = 4.5) -> matplotlib.axes.Axes:
         """
         Create a sns.histplot based on the calculated values.
 
         Parameters
         ----------
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/transition_graph/transition_graph.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/transition_graph/transition_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import warnings
 from typing import Any, Dict, List, MutableMapping, MutableSequence, Union, cast
 
 import networkx as nx
 import pandas as pd
 from IPython.core.display import HTML, display
 
+from retentioneering import RETE_CONFIG
 from retentioneering.backend import ServerManager
 from retentioneering.backend.tracker import track
 from retentioneering.edgelist import Edgelist
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.nodelist import Nodelist
 from retentioneering.templates.transition_graph import TransitionGraphRenderer
 from retentioneering.tooling.typing.transition_graph import (
@@ -89,15 +90,16 @@
         else:
             if not all(map(lambda x: x is None or 0 <= x <= 1, value.values())):
                 raise ValueError(f"For normalization type {norm_type} all thresholds must be between 0 and 1 or None")
 
         return True
 
     @track(  # type: ignore
-        tracking_info={"event_name": "transition_graph", "event_custom_name": "transition_graph_init"},
+        tracking_info={"event_name": "init"},
+        scope="transition_graph",
     )
     def __init__(
         self,
         eventstream: EventstreamType,  # graph: dict,  # preprocessed graph
     ) -> None:
         from retentioneering.eventstream.eventstream import Eventstream
 
@@ -549,141 +551,149 @@
     def generateId(size: int = 6, chars: str = string.ascii_uppercase + string.digits) -> str:
         return "el" + "".join(random.choice(chars) for _ in range(size))
 
     def _edges_norm_type_to_json_value(self, edges_norm_type: NormType) -> str:
         return "none" if edges_norm_type is None else str(edges_norm_type).lower()
 
     @track(  # type: ignore
-        tracking_info={"event_name": "transition_graph", "event_custom_name": "transition_graph_plot_graph"},
+        tracking_info={"event_name": "plot"},
+        scope="transition_graph",
         allowed_params=[
             "edges_norm_type",
             "targets",
             "nodes_threshold",
             "edges_threshold",
             "nodes_weight_col",
             "edges_weight_col",
             "custom_weight_cols",
+            "width",
+            "height",
+            "show_weights",
+            "show_percents",
+            "show_nodes_names",
+            "show_all_edges_for_targets",
+            "show_nodes_without_links",
         ],
     )
     def plot(
         self,
         targets: MutableMapping[str, str | None] | None = None,
         edges_norm_type: NormType | None = None,
         nodes_threshold: Threshold | None = None,
         nodes_norm_type: NormType | None = None,
         edges_threshold: Threshold | None = None,
         nodes_weight_col: str | None = None,
         edges_weight_col: str | None = None,
         custom_weight_cols: list[str] | None = None,
         width: int = 960,
-        height: int = 900,
+        height: int = 600,
         show_weights: bool = True,
         show_percents: bool = False,
         show_nodes_names: bool = True,
         show_all_edges_for_targets: bool = True,
         show_nodes_without_links: bool = False,
     ) -> None:
         """
         Create interactive transition graph visualization with callback to sourcing eventstream.
 
         Parameters
         ----------
-        edges_norm_type: {"full", "node", None}, default None
+        edges_norm_type : {"full", "node", None}, default None
             Type of normalization that is used to calculate weights for graph edges.
             Based on ``edges_weight_col`` parameter the weight values are calculated.
 
             - If ``None``, normalization is not used, the absolute values are taken.
             - If ``full``, normalization across the whole eventstream.
             - If ``node``, normalization across each node (or outgoing transitions from each node).
 
             See :ref:`Transition graph user guide <transition_graph_weights>` for the details.
 
-        nodes_norm_type: {"full", "node", None}, default None
+        nodes_norm_type : {"full", "node", None}, default None
             Currently not implemented. Always None.
 
-        edges_weight_col: str, optional
+        edges_weight_col : str, optional
             A column name from the :py:class:`.EventstreamSchema` which values will control the final
             edges' weights and displayed width as well.
 
             For each edge is calculated:
 
             - If ``None`` or ``event_id`` - the number of transitions.
             - If ``user_id`` - the number of unique users.
             - If ``session_id`` - the number of unique sessions.
             - If ``custom_col`` - the number of unique values in selected column.
 
             See :ref:`Transition graph user guide <transition_graph_weights>` for the details.
 
-        edges_threshold: dict, optional
+        edges_threshold : dict, optional
             Threshold mapping that defines the minimal weights for edges displayed on the canvas.
 
             - Keys should be of type str and contain the weight column names (the values from the
               :py:class:`.EventstreamSchema`).
             - Values of the dict are the thresholds for the edges that will be displayed.
 
             Support multiple weighting columns. In that case, logical OR will be applied.
             Edges with value less than at least one of thresholds will be hidden.
             Example: {'event_id': 100, user_id: 50}.
 
             See :ref:`Transition graph user guide<transition_graph_thresholds>` for the details.
 
-        nodes_weight_col: str, optional
+        nodes_weight_col : str, optional
             A column name from the :py:class:`.EventstreamSchema` which values control the final
             nodes' weights and displayed diameter as well.
 
             For each node is calculated:
 
             - If ``None`` or ``event_id`` - the number of events.
             - If ``user_id`` - the number of unique users.
             - If ``session_id`` - the number of unique sessions.
             - If ``custom_col`` - the number of unique values in selected column.
 
             See :ref:`Transition graph user guide <transition_graph_weights>` for the details.
 
-        nodes_threshold: dict, optional
+        nodes_threshold : dict, optional
             Threshold mapping that defines the minimal weights for nodes displayed on the canvas.
 
             - Keys should be of type str and contain the weight column names (the values from the
               :py:class:`.EventstreamSchema`).
             - Values of the dict are the thresholds for the nodes that will be displayed.
               They should be of type int or float.
 
             Support multiple weighting columns. In that case, logical OR will be applied.
             Nodes with value less than at least one of thresholds will be hidden.
             Example: {'event_id': 100, user_id: 50}.
 
             See :ref:`Transition graph user guide<transition_graph_thresholds>` for the details.
 
-        targets: dict, optional
+        targets : dict, optional
             Events mapping that defines which nodes and edges should be colored for better visualization.
 
             - Possible keys: "positive" (green), "negative" (red), "source" (orange).
             - Possible values: list of events of a given type.
 
             See :ref:`Transition graph user guide<transition_graph_targets>` for the details.
 
-        custom_weight_cols: list of str, optional
+        custom_weight_cols : list of str, optional
             Custom columns from the :py:class:`.EventstreamSchema` that can be selected in ``edges_weight_col``
             and ``nodes_weight_col`` parameters. If ``session_col=session_id`` exists,
             it is added by default to this list.
-        width: int, default 960
+        width : int, default 960
             Width of plot in pixels.
-        height: int, default 960
+        height : int, default 600
             Height of plot in pixels.
-        show_weights: bool, default True
+        show_weights : bool, default True
             Hide/display the edge weight labels. By default, weights are shown.
-        show_percents: bool, default False
+        show_percents : bool, default False
             Display edge weights as percents. Available only if an edge normalization type is chosen.
             By default, weights are displayed in fractions.
-        show_nodes_names: bool, default True
+        show_nodes_names : bool, default True
             Hide/display the node names. By default, names are shown.
-        show_all_edges_for_targets: bool, default True
+        show_all_edges_for_targets : bool, default True
             This displaying option allows to ignore the threshold filters and always display
             any edge connected to a target node. By default, all such edges are shown.
-        show_nodes_without_links: bool, default False
+        show_nodes_without_links : bool, default False
             Setting a threshold filter might remove all the edges connected to a node.
             Such isolated nodes might be considered as useless. This displaying option
             hides them in the canvas as well.
         @TODO: add show_edge_info_on_hover Ticket: https://retentioneering.atlassian.net/browse/PLAT-776. dpanina.
 
         Returns
         -------
@@ -759,21 +769,22 @@
                 show_percents=self._get_option("show_percents", settings),
                 show_nodes_names=self._get_option("show_nodes_names", settings),
                 show_all_edges_for_targets=self._get_option("show_all_edges_for_targets", settings),
                 show_nodes_without_links=self._get_option("show_nodes_without_links", settings),
                 nodes_threshold=self._to_js_val(norm_nodes_threshold),
                 links_threshold=self._to_js_val(norm_links_threshold),
                 weight_template="undefined",
+                tracking_hardware_id=RETE_CONFIG.user.pk,
             )
         )
 
         graph_body = self.render.body()
 
         graph_script_src = (
-            "https://static.server.retentioneering.com/viztools/transition-graph/v3/transition-graph.umd.js?id="
+            "https://static.server.retentioneering.com/package/@rete/transition-graph/version/1/dist/transition-graph.umd.js?id="
             + self.generateId()
         )
 
         init_graph_template = self.render.init(
             **dict(
                 server_id=self.server.pk,
                 env=self.env,
@@ -792,14 +803,15 @@
                 show_percents="<%= show_percents %>",
                 show_nodes_names="<%= show_nodes_names %>",
                 show_all_edges_for_targets="<%= show_all_edges_for_targets %>",
                 show_nodes_without_links="<%= show_nodes_without_links %>",
                 nodes_threshold="<%= nodes_threshold %>",
                 links_threshold="<%= links_threshold %>",
                 weight_template="undefined",
+                tracking_hardware_id=RETE_CONFIG.user.pk,
             )
         )
 
         html_template = self.render.full(
             **dict(
                 content=self.render.inner_iframe(
                     **dict(
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/typing/transition_graph/graph_types.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/typing/transition_graph/graph_types.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py` & `retentioneering-3.0.0rc3/retentioneering/tooling/user_lifetime_hist/user_lifetime_hist.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
+from retentioneering.backend.tracker import track
 from retentioneering.constants import DATETIME_UNITS
 from retentioneering.eventstream.types import EventstreamType
 from retentioneering.tooling.constants import BINS_ESTIMATORS
 
 
 class UserLifetimeHist:
     """
@@ -44,14 +45,19 @@
     log_scale: bool | tuple[bool, bool] | None
     lower_cutoff_quantile: float | None
     upper_cutoff_quantile: float | None
     bins: int | Literal[BINS_ESTIMATORS]
     bins_to_show: np.ndarray
     values_to_plot: np.ndarray
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "init"},
+        scope="user_lifetime_hist",
+        allowed_params=[],
+    )
     def __init__(self, eventstream: EventstreamType) -> None:
         self.__eventstream = eventstream
         self.user_col = self.__eventstream.schema.user_id
         self.event_col = self.__eventstream.schema.event_name
         self.time_col = self.__eventstream.schema.event_timestamp
 
         self.bins_to_show = np.array([])
@@ -89,14 +95,25 @@
             else:
                 log_scale = log_scale
         else:
             log_scale = (False, False)
 
         return log_scale, upper_cutoff_quantile, lower_cutoff_quantile
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "fit"},
+        scope="user_lifetime_hist",
+        allowed_params=[
+            "timedelta_unit",
+            "log_scale",
+            "lower_cutoff_quantile",
+            "upper_cutoff_quantile",
+            "bins",
+        ],
+    )
     def fit(
         self,
         timedelta_unit: DATETIME_UNITS = "s",
         log_scale: bool | tuple[bool, bool] | None = None,
         lower_cutoff_quantile: float | None = None,
         upper_cutoff_quantile: float | None = None,
         bins: int | Literal[BINS_ESTIMATORS] = 20,
@@ -151,26 +168,39 @@
         if len(values_to_plot) == 0:
             bins_to_show = np.array([])
 
         self.bins_to_show = bins_to_show
         self.values_to_plot = values_to_plot  # type: ignore
 
     @property
+    @track(  # type: ignore
+        tracking_info={"event_name": "values"},
+        scope="user_lifetime_hist",
+        allowed_params=[],
+    )
     def values(self) -> tuple[np.ndarray, np.ndarray]:
         """
 
         Returns
         -------
         tuple(np.ndarray, np.ndarray)
             1. The first array contains the values for histogram.
             2. The first array contains the bin edges.
 
         """
         return self.values_to_plot, self.bins_to_show
 
+    @track(  # type: ignore
+        tracking_info={"event_name": "plot"},
+        scope="user_lifetime_hist",
+        allowed_params=[
+            "width",
+            "height",
+        ],
+    )
     def plot(self, width: float = 6.0, height: float = 4.5) -> matplotlib.axes.Axes:
         """
         Create a sns.histplot based on the calculated values.
 
         Parameters
         ----------
         width : float, default 6.0
```

### Comparing `retentioneering-3.0.0rc1/retentioneering/utils/registry.py` & `retentioneering-3.0.0rc3/retentioneering/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retentioneering-3.0.0rc1/retentioneering/widget/widgets.py` & `retentioneering-3.0.0rc3/retentioneering/widget/widgets.py`

 * *Files identical despite different names*

