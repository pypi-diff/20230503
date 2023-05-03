# Comparing `tmp/hdsr_fewspy-1.6.tar.gz` & `tmp/hdsr_fewspy-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_fewspy-1.6.tar", last modified: Tue May  2 18:39:18 2023, max compression
+gzip compressed data, was "dist\hdsr_fewspy-1.7.tar", last modified: Wed May  3 12:26:15 2023, max compression
```

## Comparing `hdsr_fewspy-1.6.tar` & `hdsr_fewspy-1.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/
--rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.6/LICENSE.txt
--rw-rw-rw-   0        0        0    22748 2023-05-02 18:39:19.000000 hdsr_fewspy-1.6/PKG-INFO
--rw-rw-rw-   0        0        0    21872 2023-05-02 16:32:08.000000 hdsr_fewspy-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/
--rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/__init__.py
--rw-rw-rw-   0        0        0    14082 2023-05-02 18:30:36.000000 hdsr_fewspy-1.6/hdsr_fewspy/api.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/
--rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/__init__.py
--rw-rw-rw-   0        0        0     7535 2023-05-02 15:42:12.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/base.py
--rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_filters.py
--rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_locations.py
--rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_parameters.py
--rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_qualifiers.py
--rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_samples.py
--rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/__init__.py
--rw-rw-rw-   0        0        0     9475 2023-05-02 15:54:18.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/base.py
--rw-rw-rw-   0        0        0     6091 2023-05-02 15:54:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
--rw-rw-rw-   0        0        0     2895 2023-05-02 15:54:31.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/choices.py
--rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/custom_types.py
--rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/github.py
--rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/paths.py
--rw-rw-rw-   0        0        0     6246 2023-05-02 18:32:13.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/pi_settings.py
--rw-rw-rw-   0        0        0      911 2023-05-02 16:23:52.000000 hdsr_fewspy-1.6/hdsr_fewspy/constants/request_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/__init__.py
--rw-rw-rw-   0        0        0     5955 2023-05-02 10:29:19.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/download.py
--rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/json_to_df_timeseries.py
--rw-rw-rw-   0        0        0     1812 2023-05-02 11:23:01.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/manager.py
--rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/utils.py
--rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/converters/xml_to_python_obj.py
--rw-rw-rw-   0        0        0     4570 2023-05-02 16:27:51.000000 hdsr_fewspy-1.6/hdsr_fewspy/date_frequency.py
--rw-rw-rw-   0        0        0      681 2023-05-02 10:03:04.000000 hdsr_fewspy-1.6/hdsr_fewspy/exceptions.py
--rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/permissions.py
--rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.6/hdsr_fewspy/retry_session.py
--rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/secrets.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1837 2023-05-02 18:38:33.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/fixtures_requests.py
--rw-rw-rw-   0        0        0      713 2023-05-02 12:17:38.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_filters.py
--rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_locations.py
--rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_parameters.py
--rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_qualifiers.py
--rw-rw-rw-   0        0        0    11741 2023-05-02 15:44:49.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
--rw-rw-rw-   0        0        0     7674 2023-05-02 16:25:46.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
--rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
--rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:39:17.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/
--rw-rw-rw-   0        0        0    22748 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-02 16:32:28.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 18:39:14.000000 hdsr_fewspy-1.6/hdsr_fewspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.6/pyproject.toml
--rw-rw-rw-   0        0        0      439 2023-05-02 18:39:19.000000 hdsr_fewspy-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-05-02 18:38:09.000000 hdsr_fewspy-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    23177 2023-05-03 12:26:16.000000 hdsr_fewspy-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    22301 2023-05-03 12:24:46.000000 hdsr_fewspy-1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/
+-rw-rw-rw-   0        0        0      462 2023-05-03 11:03:03.000000 hdsr_fewspy-1.7/hdsr_fewspy/__init__.py
+-rw-rw-rw-   0        0        0    14458 2023-05-03 11:28:19.000000 hdsr_fewspy-1.7/hdsr_fewspy/api.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/
+-rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/__init__.py
+-rw-rw-rw-   0        0        0     7535 2023-05-02 15:42:12.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/base.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_filters.py
+-rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_locations.py
+-rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_parameters.py
+-rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_qualifiers.py
+-rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_samples.py
+-rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/__init__.py
+-rw-rw-rw-   0        0        0     9475 2023-05-02 15:54:18.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/base.py
+-rw-rw-rw-   0        0        0     6091 2023-05-02 15:54:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
+-rw-rw-rw-   0        0        0     2895 2023-05-02 15:54:31.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
+-rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/choices.py
+-rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/custom_types.py
+-rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/github.py
+-rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/paths.py
+-rw-rw-rw-   0        0        0     6246 2023-05-02 18:32:13.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/pi_settings.py
+-rw-rw-rw-   0        0        0      911 2023-05-02 16:23:52.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/request_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/__init__.py
+-rw-rw-rw-   0        0        0     5955 2023-05-02 10:29:19.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/download.py
+-rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/json_to_df_timeseries.py
+-rw-rw-rw-   0        0        0     1812 2023-05-02 11:23:01.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/manager.py
+-rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/utils.py
+-rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/xml_to_python_obj.py
+-rw-rw-rw-   0        0        0     4570 2023-05-02 16:27:51.000000 hdsr_fewspy-1.7/hdsr_fewspy/date_frequency.py
+-rw-rw-rw-   0        0        0      681 2023-05-02 10:03:04.000000 hdsr_fewspy-1.7/hdsr_fewspy/exceptions.py
+-rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/permissions.py
+-rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.7/hdsr_fewspy/retry_session.py
+-rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/secrets.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1837 2023-05-02 18:38:33.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/fixtures_requests.py
+-rw-rw-rw-   0        0        0      713 2023-05-02 12:17:38.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_filters.py
+-rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_locations.py
+-rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_parameters.py
+-rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_qualifiers.py
+-rw-rw-rw-   0        0        0    11741 2023-05-02 15:44:49.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
+-rw-rw-rw-   0        0        0     7743 2023-05-03 11:53:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
+-rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
+-rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/
+-rw-rw-rw-   0        0        0    23177 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-05-03 12:26:16.000000 hdsr_fewspy-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-03 12:18:21.000000 hdsr_fewspy-1.7/setup.py
```

### Comparing `hdsr_fewspy-1.6/LICENSE.txt` & `hdsr_fewspy-1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/PKG-INFO` & `hdsr_fewspy-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr_fewspy
-Version: 1.6
+Version: 1.7
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.6.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.7.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -71,112 +71,110 @@
 2. Only once per project: install hdsr_fewspy dependency:
 ```
 pip install hdsr-fewspy (or 'conda install hdsr-fewspy -channel hdsr-mid')
 ```
 3. Run imports and instantiate a hdsr_fewspy API: 
 ```
 from datetime import datetime
-from hdsr_fewspy import Api, PiSettings, OutputChoices
-import geopandas as gpd  # comes with hdsr_fewspy
-import pandas as pd  # comes with hdsr_fewspy
-
-# option 1: 
-# Instantiate API using default settings:
-api = Api()  
-
-# option 2
-# Instantiate API using custom settings:
-custom_settings = PiSettings(
+import hdsr_fewspy
+from hdsr_fewspy import Api, PiSettings, OutputChoices, github_pi_setting_defaults, TimeZoneChoices
+
+# option 1 Instantiate API using default settings:
+api = hdsr_fewspy.Api()  
+
+# option 2 Instantiate API using custom settings:
+custom_settings = hdsr_fewspy.PiSettings(
    settings_name="does not matter blabla",            
    document_version=1.25",
    ssl_verify=True,
    domain="localhost",
    port="8080",
    service="FewsWebServices",
    filter_id="INTERNAL-API",
    module_instance_ids="WerkFilter",
-   time_zone=0.0,
+   time_zone=hdsr_fewspy.TimeZoneChoices.eu_amsterdam,  # = 1.0 (only affects get_time_series dataframe and csv)
 )
-api = Api(pi_settings=custom_settings)
-
-# option 3.
-# If you want to download responses to file, then you need to specify a output_directory_root.
-# Note: the files will be downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/
-api = Api(output_directory_root=<path_to_a_dir>)
+api = hdsr_fewspy.Api(pi_settings=custom_settings)
+# or use a default custom setting:
+sa_default_pi_settings = hdsr_fewspy.github_pi_setting_defaults.get_pi_settings(settings_name="standalone")
+api = hdsr_fewspy.Api(pi_settings=sa_default_pi_settings)
+
+# option 3: Instantiate API with download directory
+# If you want to download responses to file, then you need to specify an output_directory_root. The files will be 
+downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/<here_your_files_will_be_downloaded>
+api = hdsr_fewspy.Api(output_directory_root=<path_to_a_dir>)
 ```
 
 ###### Examples 9 different API calls (using api option 3 from above)
 1. get_parameters
 ```
-df = api.get_parameters(output_choice=OutputChoices.pandas_dataframe_in_memory)
+df = api.get_parameters(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory)
 
 # id       name                                parameter_type unit display_unit uses_datum parameter_group  
 # ---------------------------------------------------------------------------------------------------------                                                                                                                                 
 # BG.b.0   Oppervlaktebegroeiing [%] - noneq   instantaneous  %    %            False      Begroeiingsgraad   
 # BG.fd.0  Flab en draadwieren [%] - noneq     instantaneous  %    %            False      Begroeiingsgraad   
 # BG.ka.0  Algen-/kroosbedekking [%] - noneq   instantaneous  %    %            False      Begroeiingsgraad  
 # ...etc...
 ```
 2. get_filters
 ```
-response = api.get_filters(output_choice=OutputChoices.json_response_in_memory)
+response = api.get_filters(output_choice=hdsr_fewspy.OutputChoices.json_response_in_memory)
 response.json() 
 
 # {
 # "version": "1.25",
 # "filters": [
 #     {
 #         "id": "INTERNAL-API",
 #         "name": "INTERNAL-API",
 #         "child": [{"id": "INTERNAL-API.RUWMET", "name": "Ruwe metingen (punt)"
 # ...etc...
 ```
 3. get_locations
 ```
-gdf = get_locations(output_choice=OutputChoices.pandas_dataframe_in_memory, show_attributes=True)
+gdf = get_locations(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory, show_attributes=True)
 
 # location_id description          short_name          lat               lon                x        y        z   parent_location_id geometry                      attributes
 # -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------                                                  
 # beg_062     BEGROEIINGSMEETPUNT  beg_062-LR_13_xruim 52.58907339700342 5.1718081593021505 140251.0 460118.0 0.0 NaN                POINT (140251.000 460118.000) [{'name': 'LOC_NAME', 'type': 'text', 'id': 'LOC_NAME', 'value': 'beg_062 ...etc...]
 # beg_084     BEGROEIINGSMEETPUNT  beg_084-LR_17_xruim 52.06261306007392 5.12600382893812   137088.0 452734.0 0.0 NaN                POINT (137088.000 452734.000) [{'name': 'LOC_NAME', 'type': 'text', 'id': 'LOC_NAME', 'value': 'beg_084 ...etc...]
 # beg_102     BEGROEIINGSMEETPUNT  beg_102-KR_9_xruim  52.07249358678008 5.215531005948442  143230.0 453815.0 0.0 NaN                POINT (143230.000 453815.000) [{'name': 'LOC_NAME', 'type': 'text', 'id': 'LOC_NAME', 'value': 'beg_102 ...etc...]
 # ...etc...
 ```
 4. get_qualifiers
 ```
-df = fixture_api_sa_no_download_dir.get_qualifiers(output_choice=OutputChoices.pandas_dataframe_in_memory)
+df = fixture_api_sa_no_download_dir.get_qualifiers(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory)
     
 # id      name               group_id
 # -----------------------------------
 # ergkrap erg krap (max 10%) None
 # krap    krap (max 30%)     None
 # normaal normaal (max 50%)  None
 # ruim    ruim (max 70%)     None
 # ...etc...
 ```
 
 5. get_timezone_id
 ```
-response = api.get_timezone_id(output_choice=OutputChoices.json_response_in_memory)
+response = api.get_timezone_id(output_choice=hdsr_fewspy.OutputChoices.json_response_in_memory)
 
 # verify response
 assert response.text == "GMT"
 assert TimeZoneChoices.get_tz_float(value=response.text) == TimeZoneChoices.gmt == 0.0
 ```
 6. get_samples
 ```
 # Not yet implemented
 ```
 7. get_time_series_single
 ```
-# Single means: use max 1 location_id and/or parameter_id and/or qualifier_id.
-# One large call can result in multiple small calls and therefore multiple responses.
-
-# If your output_choice is json/xml in memory, then you get a list with >=1 responses. 
-# Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
+# Single means: use max 1 location_id and/or parameter_id and/or qualifier_id. One large call can result in multiple 
+# small calls and therefore multiple responses. If your output_choice is json/xml in memory, then you get a list with 
+# >=1 responses. Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
 
 responses = api.get_time_series_single(
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_response_in_memory,
@@ -207,35 +205,33 @@
 #         <event date="2012-01-01" time="00:15:00" value="-0.35" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="00:45:00" value="-0.36" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:30:00" value="-0.37" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:31:17" value="-0.38" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="03:15:00" value="-0.39" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         ...etc..
 
-# If your output_choice is dataframe, then all responses are collected in one dataframe. 
-# Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
+# If your output_choice is dataframe, then all responses are collected in one dataframe. Arguments 'flag_threshold' 
+# and 'drop_missing_values' do have effect.
 
 df = api.get_time_series_single(
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     drop_missing_values = True,
     flag_threshold = 6,  # all flags 6 and higher are removed from dataframe
     output_choice = OutputChoices.pandas_dataframe_in_memory,
 )
 ```
 8. get_time_series_multi 
 ```
-# Multi means: use >=1 location_id and/or parameter_id and/or qualifier_id.
-# The api call below results in 4 unique location_parameter_qualifier comibinations: OW433001_hg0, OW433001_hgd, OW433002_hg0, OW433002_hgd
-# Per unique combination we do >=1 requests which therefore results in >=1 responses.
-
-# If output_choice is xml/json to file, then each response results in a file. 
-# Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
+# Multi means: use >=1 location_id and/or parameter_id and/or qualifier_id. The api call below results in 4 unique 
+# location_parameter_qualifier comibinations: OW433001_hg0, OW433001_hgd, OW433002_hg0, OW433002_hgd. Per unique 
+# combination we do >=1 requests which therefore result in >=1 responses. If output_choice is xml/json to file, then 
+# each response results in a file. Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
 
 list_with_donwloaded_csv_filepaths = api.get_time_series_multi(
     location_ids = ["OW433001", "OW433002"]
     parameter_ids = ["H.G.0", "H.G.d"],
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_file_in_download_dir,
@@ -243,16 +239,16 @@
 
 print(list_with_donwloaded_csv_filepaths)
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433001_hg0_20120101t000000z_20120102t000000z_0.json
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_0.json
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_1.json
 
 
-# If output_choice is csv to file, then all responses per unique combi are grouped in one csv file. 
-# Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
+# If output_choice is csv to file, then all responses per unique combi are grouped in one csv file. Arguments 
+# 'flag_threshold' and 'drop_missing_values' do have effect.
   
 list_with_donwloaded_csv_filepaths = api.get_time_series_multi(
     location_ids = ["OW433001", "OW433002"]
     parameter_ids = ["H.G.0", "H.G.d"],
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.csv_file_in_download_dir,
@@ -326,21 +322,21 @@
 
 ### Releases
 [Release history][releases]
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (May 2nd 2023)
+### Test Coverage (May 3rd 2023)
 ```
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
-hdsr_fewspy\__init__.py                                               8      0   100%
-hdsr_fewspy\api.py                                                   99     11    89%
+hdsr_fewspy\__init__.py                                              10      0   100%
+hdsr_fewspy\api.py                                                  107     16    85%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
@@ -349,29 +345,29 @@
 hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           73      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          35      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
-hdsr_fewspy\constants\pi_settings.py                                 80      7    91%
+hdsr_fewspy\constants\pi_settings.py                                 78      7    91%
 hdsr_fewspy\constants\request_settings.py                            12      0   100%
 hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
 hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
 hdsr_fewspy\exceptions.py                                            16      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1518    188    88%
+TOTAL                                                              1526    193    87%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.6/README.md` & `hdsr_fewspy-1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,112 +49,110 @@
 2. Only once per project: install hdsr_fewspy dependency:
 ```
 pip install hdsr-fewspy (or 'conda install hdsr-fewspy -channel hdsr-mid')
 ```
 3. Run imports and instantiate a hdsr_fewspy API: 
 ```
 from datetime import datetime
-from hdsr_fewspy import Api, PiSettings, OutputChoices
-import geopandas as gpd  # comes with hdsr_fewspy
-import pandas as pd  # comes with hdsr_fewspy
-
-# option 1: 
-# Instantiate API using default settings:
-api = Api()  
-
-# option 2
-# Instantiate API using custom settings:
-custom_settings = PiSettings(
+import hdsr_fewspy
+from hdsr_fewspy import Api, PiSettings, OutputChoices, github_pi_setting_defaults, TimeZoneChoices
+
+# option 1 Instantiate API using default settings:
+api = hdsr_fewspy.Api()  
+
+# option 2 Instantiate API using custom settings:
+custom_settings = hdsr_fewspy.PiSettings(
    settings_name="does not matter blabla",            
    document_version=1.25",
    ssl_verify=True,
    domain="localhost",
    port="8080",
    service="FewsWebServices",
    filter_id="INTERNAL-API",
    module_instance_ids="WerkFilter",
-   time_zone=0.0,
+   time_zone=hdsr_fewspy.TimeZoneChoices.eu_amsterdam,  # = 1.0 (only affects get_time_series dataframe and csv)
 )
-api = Api(pi_settings=custom_settings)
-
-# option 3.
-# If you want to download responses to file, then you need to specify a output_directory_root.
-# Note: the files will be downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/
-api = Api(output_directory_root=<path_to_a_dir>)
+api = hdsr_fewspy.Api(pi_settings=custom_settings)
+# or use a default custom setting:
+sa_default_pi_settings = hdsr_fewspy.github_pi_setting_defaults.get_pi_settings(settings_name="standalone")
+api = hdsr_fewspy.Api(pi_settings=sa_default_pi_settings)
+
+# option 3: Instantiate API with download directory
+# If you want to download responses to file, then you need to specify an output_directory_root. The files will be 
+downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/<here_your_files_will_be_downloaded>
+api = hdsr_fewspy.Api(output_directory_root=<path_to_a_dir>)
 ```
 
 ###### Examples 9 different API calls (using api option 3 from above)
 1. get_parameters
 ```
-df = api.get_parameters(output_choice=OutputChoices.pandas_dataframe_in_memory)
+df = api.get_parameters(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory)
 
 # id       name                                parameter_type unit display_unit uses_datum parameter_group  
 # ---------------------------------------------------------------------------------------------------------                                                                                                                                 
 # BG.b.0   Oppervlaktebegroeiing [%] - noneq   instantaneous  %    %            False      Begroeiingsgraad   
 # BG.fd.0  Flab en draadwieren [%] - noneq     instantaneous  %    %            False      Begroeiingsgraad   
 # BG.ka.0  Algen-/kroosbedekking [%] - noneq   instantaneous  %    %            False      Begroeiingsgraad  
 # ...etc...
 ```
 2. get_filters
 ```
-response = api.get_filters(output_choice=OutputChoices.json_response_in_memory)
+response = api.get_filters(output_choice=hdsr_fewspy.OutputChoices.json_response_in_memory)
 response.json() 
 
 # {
 # "version": "1.25",
 # "filters": [
 #     {
 #         "id": "INTERNAL-API",
 #         "name": "INTERNAL-API",
 #         "child": [{"id": "INTERNAL-API.RUWMET", "name": "Ruwe metingen (punt)"
 # ...etc...
 ```
 3. get_locations
 ```
-gdf = get_locations(output_choice=OutputChoices.pandas_dataframe_in_memory, show_attributes=True)
+gdf = get_locations(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory, show_attributes=True)
 
 # location_id description          short_name          lat               lon                x        y        z   parent_location_id geometry                      attributes
 # -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------                                                  
 # beg_062     BEGROEIINGSMEETPUNT  beg_062-LR_13_xruim 52.58907339700342 5.1718081593021505 140251.0 460118.0 0.0 NaN                POINT (140251.000 460118.000) [{'name': 'LOC_NAME', 'type': 'text', 'id': 'LOC_NAME', 'value': 'beg_062 ...etc...]
 # beg_084     BEGROEIINGSMEETPUNT  beg_084-LR_17_xruim 52.06261306007392 5.12600382893812   137088.0 452734.0 0.0 NaN                POINT (137088.000 452734.000) [{'name': 'LOC_NAME', 'type': 'text', 'id': 'LOC_NAME', 'value': 'beg_084 ...etc...]
 # beg_102     BEGROEIINGSMEETPUNT  beg_102-KR_9_xruim  52.07249358678008 5.215531005948442  143230.0 453815.0 0.0 NaN                POINT (143230.000 453815.000) [{'name': 'LOC_NAME', 'type': 'text', 'id': 'LOC_NAME', 'value': 'beg_102 ...etc...]
 # ...etc...
 ```
 4. get_qualifiers
 ```
-df = fixture_api_sa_no_download_dir.get_qualifiers(output_choice=OutputChoices.pandas_dataframe_in_memory)
+df = fixture_api_sa_no_download_dir.get_qualifiers(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory)
     
 # id      name               group_id
 # -----------------------------------
 # ergkrap erg krap (max 10%) None
 # krap    krap (max 30%)     None
 # normaal normaal (max 50%)  None
 # ruim    ruim (max 70%)     None
 # ...etc...
 ```
 
 5. get_timezone_id
 ```
-response = api.get_timezone_id(output_choice=OutputChoices.json_response_in_memory)
+response = api.get_timezone_id(output_choice=hdsr_fewspy.OutputChoices.json_response_in_memory)
 
 # verify response
 assert response.text == "GMT"
 assert TimeZoneChoices.get_tz_float(value=response.text) == TimeZoneChoices.gmt == 0.0
 ```
 6. get_samples
 ```
 # Not yet implemented
 ```
 7. get_time_series_single
 ```
-# Single means: use max 1 location_id and/or parameter_id and/or qualifier_id.
-# One large call can result in multiple small calls and therefore multiple responses.
-
-# If your output_choice is json/xml in memory, then you get a list with >=1 responses. 
-# Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
+# Single means: use max 1 location_id and/or parameter_id and/or qualifier_id. One large call can result in multiple 
+# small calls and therefore multiple responses. If your output_choice is json/xml in memory, then you get a list with 
+# >=1 responses. Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
 
 responses = api.get_time_series_single(
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_response_in_memory,
@@ -185,35 +183,33 @@
 #         <event date="2012-01-01" time="00:15:00" value="-0.35" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="00:45:00" value="-0.36" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:30:00" value="-0.37" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:31:17" value="-0.38" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="03:15:00" value="-0.39" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         ...etc..
 
-# If your output_choice is dataframe, then all responses are collected in one dataframe. 
-# Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
+# If your output_choice is dataframe, then all responses are collected in one dataframe. Arguments 'flag_threshold' 
+# and 'drop_missing_values' do have effect.
 
 df = api.get_time_series_single(
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     drop_missing_values = True,
     flag_threshold = 6,  # all flags 6 and higher are removed from dataframe
     output_choice = OutputChoices.pandas_dataframe_in_memory,
 )
 ```
 8. get_time_series_multi 
 ```
-# Multi means: use >=1 location_id and/or parameter_id and/or qualifier_id.
-# The api call below results in 4 unique location_parameter_qualifier comibinations: OW433001_hg0, OW433001_hgd, OW433002_hg0, OW433002_hgd
-# Per unique combination we do >=1 requests which therefore results in >=1 responses.
-
-# If output_choice is xml/json to file, then each response results in a file. 
-# Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
+# Multi means: use >=1 location_id and/or parameter_id and/or qualifier_id. The api call below results in 4 unique 
+# location_parameter_qualifier comibinations: OW433001_hg0, OW433001_hgd, OW433002_hg0, OW433002_hgd. Per unique 
+# combination we do >=1 requests which therefore result in >=1 responses. If output_choice is xml/json to file, then 
+# each response results in a file. Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
 
 list_with_donwloaded_csv_filepaths = api.get_time_series_multi(
     location_ids = ["OW433001", "OW433002"]
     parameter_ids = ["H.G.0", "H.G.d"],
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_file_in_download_dir,
@@ -221,16 +217,16 @@
 
 print(list_with_donwloaded_csv_filepaths)
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433001_hg0_20120101t000000z_20120102t000000z_0.json
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_0.json
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_1.json
 
 
-# If output_choice is csv to file, then all responses per unique combi are grouped in one csv file. 
-# Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
+# If output_choice is csv to file, then all responses per unique combi are grouped in one csv file. Arguments 
+# 'flag_threshold' and 'drop_missing_values' do have effect.
   
 list_with_donwloaded_csv_filepaths = api.get_time_series_multi(
     location_ids = ["OW433001", "OW433002"]
     parameter_ids = ["H.G.0", "H.G.d"],
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.csv_file_in_download_dir,
@@ -304,21 +300,21 @@
 
 ### Releases
 [Release history][releases]
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (May 2nd 2023)
+### Test Coverage (May 3rd 2023)
 ```
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
-hdsr_fewspy\__init__.py                                               8      0   100%
-hdsr_fewspy\api.py                                                   99     11    89%
+hdsr_fewspy\__init__.py                                              10      0   100%
+hdsr_fewspy\api.py                                                  107     16    85%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
@@ -327,29 +323,29 @@
 hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           73      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          35      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
-hdsr_fewspy\constants\pi_settings.py                                 80      7    91%
+hdsr_fewspy\constants\pi_settings.py                                 78      7    91%
 hdsr_fewspy\constants\request_settings.py                            12      0   100%
 hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
 hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
 hdsr_fewspy\exceptions.py                                            16      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1518    188    88%
+TOTAL                                                              1526    193    87%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,54 +37,61 @@
 
     def __init__(
         self,
         pi_settings: PiSettings = None,
         output_directory_root: Union[str, Path] = None,
     ):
         self.permissions = Permissions()
-        self.output_dir = self._get_output_dir(output_directory_root=output_directory_root)
-        self.pi_settings = self._validate_pi_settings(pi_settings=pi_settings)
+        self.output_dir = self.__get_output_dir(output_directory_root=output_directory_root)
+        self.pi_settings = self.__validate_pi_settings(pi_settings=pi_settings)
         self.request_settings: RequestSettings = get_default_request_settings()
         self.retry_backoff_session = RetryBackoffSession(
             _request_settings=self.request_settings,
             pi_settings=self.pi_settings,
             output_dir=self.output_dir,
         )
-        self._ensure_service_is_running()
+        self.__ensure_service_is_running()
 
     @staticmethod
-    def _get_output_dir(output_directory_root: Union[str, Path] = None) -> Optional[Path]:
+    def __get_output_dir(output_directory_root: Union[str, Path] = None) -> Optional[Path]:
         if output_directory_root is None:
             return None
         # check 1
         output_directory_root = Path(output_directory_root)
         assert output_directory_root.is_dir(), f"output_directory_root {output_directory_root} must exist"
         # check 2
         is_dir_writable = os.access(path=output_directory_root.as_posix(), mode=os.W_OK)
         assert is_dir_writable, f"output_directory_root {output_directory_root} must be writable"
         # create subdir
         output_dir = output_directory_root / f"hdsr_fewspy_{datetime.now().strftime('%Y%m%d_%H%M%S')}"
         return output_dir
 
-    def _ensure_service_is_running(self) -> None:
-        # check endpoint with smallest response (=timezonid)
-        response = self.get_timezone_id(output_choice=OutputChoices.json_response_in_memory)
-        if response.ok:
-            logger.info("PiWebService is running")
-            return
+    def __log_not_running_service(self, err: Exception = None, response: ResponseType = None) -> None:
+        error = f"{response.text}, {err}" if response else str(err)
         msg = (
-            f"Piwebservice is not running, err={response.text}. Ensure that you can visit the test page "
-            f"{self.pi_settings.test_url}"
+            f"Piwebservice is not running, Ensure that you can visit the test page '{self.pi_settings.test_url}', "
+            f"err={error}"
         )
         if self.pi_settings.domain == "localhost":
             msg += ". Please make sure FEWS SA webservice is running and start embedded tomcat server via F12 key."
             raise exceptions.StandAloneFewsWebServiceNotRunningError(msg)
         raise exceptions.FewsWebServiceNotRunningError(msg)
 
-    def _validate_pi_settings(self, pi_settings: PiSettings = None) -> PiSettings:
+    def __ensure_service_is_running(self) -> None:
+        """Just request endpoint with smallest response (=timezonid)."""
+        try:
+            response = self.get_timezone_id(output_choice=OutputChoices.json_response_in_memory)
+            if response.ok:
+                logger.info("PiWebService is running")
+                return
+            self.__log_not_running_service(err=None, response=response)
+        except Exception as err:
+            self.__log_not_running_service(err=err, response=None)
+
+    def __validate_pi_settings(self, pi_settings: PiSettings = None) -> PiSettings:
         if not pi_settings:
             pi_settings = github_pi_setting_defaults.get_pi_settings(settings_name="production")
         if not isinstance(pi_settings, PiSettings):
             raise AssertionError("pi_settings must be a PiSettings, see README.ml example how to create one")
         mapper = {
             # setting: (used, allowed)
             "domain": (pi_settings.domain, self.permissions.allowed_domain),
@@ -325,16 +332,15 @@
 # TODO: Ciska geen interesse in:
 #  --------------------------------
 #  get_qualifiers
 
 # TODO: check of properties goed meekomen in get_timeseries in PI_JSON (in PI_XML gaat het goed) -> Ciska:" bij
 #  EFICS werkt niet helemaal lekker. bij get_samples gaat het helemaal fout"
 
-# TODO: potentieel van grote naar kleine belasting (retry-backoff nodig): get_samples, get_timeseries,
+# TODO: van potentieel grote naar kleine request belasting: get_samples, get_timeseries,
 #  get_qualifiers (25 groepen * 100k regels per groep), get_parameters (4000), get_locations (300)
 
 # TODO: use onlyHeader=True kan voor get_timeseries en get_samples (beide hebben ook start + eind).
 #  Echter, get_qualifiers heeft dat niet. FEWS-WIS response is snel (<1sec). FEWS-EFICS duurt lang (8 sec)
-#  get_lcoations duurt 7 sec.
-#  Voorstel Ciska: alleen func get_timeseries + get_samples via PiWebService. De andere request disabelen:
-#  logger.info('Stuur ciska.overbeek@hdsr.nl een mailtje of dat lijstje mag, dan krijg je er ook nog meer info bij)
-#  die lijstjes worden 2 a 3 per jaar script + handmatig ge-update.
+#  get_lcoations duurt 7 sec. Voorstel Ciska: alleen func get_timeseries + get_samples via PiWebService. De andere
+#  request disabelen: logger.info('Stuur ciska.overbeek@hdsr.nl een mailtje of dat lijstje mag, dan krijg je er ook
+#  nog meer info bij) die lijstjes worden 2 a 3 per jaar script + handmatig ge-update...
```

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/__init__.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/base.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_filters.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_locations.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_parameters.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_qualifiers.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_samples.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_samples.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/get_timezone_id.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/base.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_single.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_single.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py` & `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/constants/choices.py` & `hdsr_fewspy-1.7/hdsr_fewspy/constants/choices.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/constants/paths.py` & `hdsr_fewspy-1.7/hdsr_fewspy/constants/paths.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/constants/pi_settings.py` & `hdsr_fewspy-1.7/hdsr_fewspy/constants/pi_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/constants/request_settings.py` & `hdsr_fewspy-1.7/hdsr_fewspy/constants/request_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/converters/download.py` & `hdsr_fewspy-1.7/hdsr_fewspy/converters/download.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/converters/json_to_df_timeseries.py` & `hdsr_fewspy-1.7/hdsr_fewspy/converters/json_to_df_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/converters/manager.py` & `hdsr_fewspy-1.7/hdsr_fewspy/converters/manager.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/converters/utils.py` & `hdsr_fewspy-1.7/hdsr_fewspy/converters/utils.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/converters/xml_to_python_obj.py` & `hdsr_fewspy-1.7/hdsr_fewspy/converters/xml_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/date_frequency.py` & `hdsr_fewspy-1.7/hdsr_fewspy/date_frequency.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/exceptions.py` & `hdsr_fewspy-1.7/hdsr_fewspy/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/permissions.py` & `hdsr_fewspy-1.7/hdsr_fewspy/permissions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/retry_session.py` & `hdsr_fewspy-1.7/hdsr_fewspy/retry_session.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/secrets.py` & `hdsr_fewspy-1.7/hdsr_fewspy/secrets.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/fixtures.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/fixtures_requests.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/fixtures_requests.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_filters.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_locations.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_parameters.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_qualifiers.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_single.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_single.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.json_response_in_memory,
     )
     assert len(responses) == 11
     assert api.request_settings.default_request_period == pd.Timedelta(days=56)
-    assert api.request_settings.updated_request_period == pd.Timedelta(days=283, hours=12)
+    assert api.request_settings.updated_request_period == pd.Timedelta(days=270, hours=7, minutes=13, seconds=52)
 
 
 def test_sa_single_ts_long_ok_xml_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
     request_data = fixtures_requests.RequestTimeSeriesSingleLong
 
     responses = api.get_time_series_single(
@@ -154,24 +154,24 @@
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_response_in_memory,
     )
     assert len(responses) == 11
     assert api.request_settings.default_request_period == pd.Timedelta(days=56)
-    assert api.request_settings.updated_request_period == pd.Timedelta(days=283, hours=12)
+    assert api.request_settings.updated_request_period == pd.Timedelta(days=270, hours=7, minutes=13, seconds=52)
 
 
 def test_sa_single_ts_long_ok_df_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
     request_data = fixtures_requests.RequestTimeSeriesSingleLong
 
     df_found = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.pandas_dataframe_in_memory,
     )
-    assert len(df_found) == 199255
+    assert len(df_found) == 199251
     assert api.request_settings.default_request_period == pd.Timedelta(days=56)
-    assert api.request_settings.updated_request_period == pd.Timedelta(days=283, hours=12)
+    assert api.request_settings.updated_request_period == pd.Timedelta(days=270, hours=7, minutes=13, seconds=52)
```

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy/tests/test_sa_timezone_id.py` & `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy.egg-info/PKG-INFO` & `hdsr_fewspy-1.7/hdsr_fewspy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr-fewspy
-Version: 1.6
+Version: 1.7
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.6.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.7.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -71,112 +71,110 @@
 2. Only once per project: install hdsr_fewspy dependency:
 ```
 pip install hdsr-fewspy (or 'conda install hdsr-fewspy -channel hdsr-mid')
 ```
 3. Run imports and instantiate a hdsr_fewspy API: 
 ```
 from datetime import datetime
-from hdsr_fewspy import Api, PiSettings, OutputChoices
-import geopandas as gpd  # comes with hdsr_fewspy
-import pandas as pd  # comes with hdsr_fewspy
-
-# option 1: 
-# Instantiate API using default settings:
-api = Api()  
-
-# option 2
-# Instantiate API using custom settings:
-custom_settings = PiSettings(
+import hdsr_fewspy
+from hdsr_fewspy import Api, PiSettings, OutputChoices, github_pi_setting_defaults, TimeZoneChoices
+
+# option 1 Instantiate API using default settings:
+api = hdsr_fewspy.Api()  
+
+# option 2 Instantiate API using custom settings:
+custom_settings = hdsr_fewspy.PiSettings(
    settings_name="does not matter blabla",            
    document_version=1.25",
    ssl_verify=True,
    domain="localhost",
    port="8080",
    service="FewsWebServices",
    filter_id="INTERNAL-API",
    module_instance_ids="WerkFilter",
-   time_zone=0.0,
+   time_zone=hdsr_fewspy.TimeZoneChoices.eu_amsterdam,  # = 1.0 (only affects get_time_series dataframe and csv)
 )
-api = Api(pi_settings=custom_settings)
-
-# option 3.
-# If you want to download responses to file, then you need to specify a output_directory_root.
-# Note: the files will be downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/
-api = Api(output_directory_root=<path_to_a_dir>)
+api = hdsr_fewspy.Api(pi_settings=custom_settings)
+# or use a default custom setting:
+sa_default_pi_settings = hdsr_fewspy.github_pi_setting_defaults.get_pi_settings(settings_name="standalone")
+api = hdsr_fewspy.Api(pi_settings=sa_default_pi_settings)
+
+# option 3: Instantiate API with download directory
+# If you want to download responses to file, then you need to specify an output_directory_root. The files will be 
+downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/<here_your_files_will_be_downloaded>
+api = hdsr_fewspy.Api(output_directory_root=<path_to_a_dir>)
 ```
 
 ###### Examples 9 different API calls (using api option 3 from above)
 1. get_parameters
 ```
-df = api.get_parameters(output_choice=OutputChoices.pandas_dataframe_in_memory)
+df = api.get_parameters(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory)
 
 # id       name                                parameter_type unit display_unit uses_datum parameter_group  
 # ---------------------------------------------------------------------------------------------------------                                                                                                                                 
 # BG.b.0   Oppervlaktebegroeiing [%] - noneq   instantaneous  %    %            False      Begroeiingsgraad   
 # BG.fd.0  Flab en draadwieren [%] - noneq     instantaneous  %    %            False      Begroeiingsgraad   
 # BG.ka.0  Algen-/kroosbedekking [%] - noneq   instantaneous  %    %            False      Begroeiingsgraad  
 # ...etc...
 ```
 2. get_filters
 ```
-response = api.get_filters(output_choice=OutputChoices.json_response_in_memory)
+response = api.get_filters(output_choice=hdsr_fewspy.OutputChoices.json_response_in_memory)
 response.json() 
 
 # {
 # "version": "1.25",
 # "filters": [
 #     {
 #         "id": "INTERNAL-API",
 #         "name": "INTERNAL-API",
 #         "child": [{"id": "INTERNAL-API.RUWMET", "name": "Ruwe metingen (punt)"
 # ...etc...
 ```
 3. get_locations
 ```
-gdf = get_locations(output_choice=OutputChoices.pandas_dataframe_in_memory, show_attributes=True)
+gdf = get_locations(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory, show_attributes=True)
 
 # location_id description          short_name          lat               lon                x        y        z   parent_location_id geometry                      attributes
 # -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------                                                  
 # beg_062     BEGROEIINGSMEETPUNT  beg_062-LR_13_xruim 52.58907339700342 5.1718081593021505 140251.0 460118.0 0.0 NaN                POINT (140251.000 460118.000) [{'name': 'LOC_NAME', 'type': 'text', 'id': 'LOC_NAME', 'value': 'beg_062 ...etc...]
 # beg_084     BEGROEIINGSMEETPUNT  beg_084-LR_17_xruim 52.06261306007392 5.12600382893812   137088.0 452734.0 0.0 NaN                POINT (137088.000 452734.000) [{'name': 'LOC_NAME', 'type': 'text', 'id': 'LOC_NAME', 'value': 'beg_084 ...etc...]
 # beg_102     BEGROEIINGSMEETPUNT  beg_102-KR_9_xruim  52.07249358678008 5.215531005948442  143230.0 453815.0 0.0 NaN                POINT (143230.000 453815.000) [{'name': 'LOC_NAME', 'type': 'text', 'id': 'LOC_NAME', 'value': 'beg_102 ...etc...]
 # ...etc...
 ```
 4. get_qualifiers
 ```
-df = fixture_api_sa_no_download_dir.get_qualifiers(output_choice=OutputChoices.pandas_dataframe_in_memory)
+df = fixture_api_sa_no_download_dir.get_qualifiers(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory)
     
 # id      name               group_id
 # -----------------------------------
 # ergkrap erg krap (max 10%) None
 # krap    krap (max 30%)     None
 # normaal normaal (max 50%)  None
 # ruim    ruim (max 70%)     None
 # ...etc...
 ```
 
 5. get_timezone_id
 ```
-response = api.get_timezone_id(output_choice=OutputChoices.json_response_in_memory)
+response = api.get_timezone_id(output_choice=hdsr_fewspy.OutputChoices.json_response_in_memory)
 
 # verify response
 assert response.text == "GMT"
 assert TimeZoneChoices.get_tz_float(value=response.text) == TimeZoneChoices.gmt == 0.0
 ```
 6. get_samples
 ```
 # Not yet implemented
 ```
 7. get_time_series_single
 ```
-# Single means: use max 1 location_id and/or parameter_id and/or qualifier_id.
-# One large call can result in multiple small calls and therefore multiple responses.
-
-# If your output_choice is json/xml in memory, then you get a list with >=1 responses. 
-# Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
+# Single means: use max 1 location_id and/or parameter_id and/or qualifier_id. One large call can result in multiple 
+# small calls and therefore multiple responses. If your output_choice is json/xml in memory, then you get a list with 
+# >=1 responses. Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
 
 responses = api.get_time_series_single(
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_response_in_memory,
@@ -207,35 +205,33 @@
 #         <event date="2012-01-01" time="00:15:00" value="-0.35" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="00:45:00" value="-0.36" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:30:00" value="-0.37" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:31:17" value="-0.38" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="03:15:00" value="-0.39" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         ...etc..
 
-# If your output_choice is dataframe, then all responses are collected in one dataframe. 
-# Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
+# If your output_choice is dataframe, then all responses are collected in one dataframe. Arguments 'flag_threshold' 
+# and 'drop_missing_values' do have effect.
 
 df = api.get_time_series_single(
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     drop_missing_values = True,
     flag_threshold = 6,  # all flags 6 and higher are removed from dataframe
     output_choice = OutputChoices.pandas_dataframe_in_memory,
 )
 ```
 8. get_time_series_multi 
 ```
-# Multi means: use >=1 location_id and/or parameter_id and/or qualifier_id.
-# The api call below results in 4 unique location_parameter_qualifier comibinations: OW433001_hg0, OW433001_hgd, OW433002_hg0, OW433002_hgd
-# Per unique combination we do >=1 requests which therefore results in >=1 responses.
-
-# If output_choice is xml/json to file, then each response results in a file. 
-# Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
+# Multi means: use >=1 location_id and/or parameter_id and/or qualifier_id. The api call below results in 4 unique 
+# location_parameter_qualifier comibinations: OW433001_hg0, OW433001_hgd, OW433002_hg0, OW433002_hgd. Per unique 
+# combination we do >=1 requests which therefore result in >=1 responses. If output_choice is xml/json to file, then 
+# each response results in a file. Arguments 'flag_threshold' and 'drop_missing_values' have no effect.  
 
 list_with_donwloaded_csv_filepaths = api.get_time_series_multi(
     location_ids = ["OW433001", "OW433002"]
     parameter_ids = ["H.G.0", "H.G.d"],
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_file_in_download_dir,
@@ -243,16 +239,16 @@
 
 print(list_with_donwloaded_csv_filepaths)
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433001_hg0_20120101t000000z_20120102t000000z_0.json
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_0.json
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_1.json
 
 
-# If output_choice is csv to file, then all responses per unique combi are grouped in one csv file. 
-# Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
+# If output_choice is csv to file, then all responses per unique combi are grouped in one csv file. Arguments 
+# 'flag_threshold' and 'drop_missing_values' do have effect.
   
 list_with_donwloaded_csv_filepaths = api.get_time_series_multi(
     location_ids = ["OW433001", "OW433002"]
     parameter_ids = ["H.G.0", "H.G.d"],
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.csv_file_in_download_dir,
@@ -326,21 +322,21 @@
 
 ### Releases
 [Release history][releases]
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (May 2nd 2023)
+### Test Coverage (May 3rd 2023)
 ```
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
-hdsr_fewspy\__init__.py                                               8      0   100%
-hdsr_fewspy\api.py                                                   99     11    89%
+hdsr_fewspy\__init__.py                                              10      0   100%
+hdsr_fewspy\api.py                                                  107     16    85%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
@@ -349,29 +345,29 @@
 hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           73      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          35      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
-hdsr_fewspy\constants\pi_settings.py                                 80      7    91%
+hdsr_fewspy\constants\pi_settings.py                                 78      7    91%
 hdsr_fewspy\constants\request_settings.py                            12      0   100%
 hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
 hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
 hdsr_fewspy\exceptions.py                                            16      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1518    188    88%
+TOTAL                                                              1526    193    87%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.6/hdsr_fewspy.egg-info/SOURCES.txt` & `hdsr_fewspy-1.7/hdsr_fewspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/pyproject.toml` & `hdsr_fewspy-1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.6/setup.py` & `hdsr_fewspy-1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.6"
+version = "1.7"
 
 install_requires = [
     "requests",
     "geopandas",
     "pandas",
     "hdsr-pygithub",
     "pathlib",
```

