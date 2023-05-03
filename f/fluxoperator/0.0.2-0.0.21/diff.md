# Comparing `tmp/fluxoperator-0.0.2.tar.gz` & `tmp/fluxoperator-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.2.tar", last modified: Mon Mar 20 22:55:37 2023, max compression
+gzip compressed data, was "fluxoperator-0.0.21.tar", last modified: Wed May  3 06:51:17 2023, max compression
```

## Comparing `fluxoperator-0.0.2.tar` & `fluxoperator-0.0.21.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-03-20 22:55:37.409297 fluxoperator-0.0.2/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2666 2023-03-20 22:55:37.409297 fluxoperator-0.0.2/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-03-20 22:55:37.401297 fluxoperator-0.0.2/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1906 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-03-20 22:55:37.401297 fluxoperator-0.0.2/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12899 2023-03-20 22:55:32.000000 fluxoperator-0.0.2/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-03-20 22:55:37.405297 fluxoperator-0.0.2/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1430 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6122 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5910 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23365 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5483 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13789 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4844 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-03-20 22:37:11.000000 fluxoperator-0.0.2/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-03-20 22:55:37.405297 fluxoperator-0.0.2/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-03-01 18:29:03.000000 fluxoperator-0.0.2/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-03-01 18:29:03.000000 fluxoperator-0.0.2/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5590 2023-03-15 02:58:30.000000 fluxoperator-0.0.2/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-03-20 22:55:37.401297 fluxoperator-0.0.2/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2666 2023-03-20 22:55:37.000000 fluxoperator-0.0.2/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1867 2023-03-20 22:55:37.000000 fluxoperator-0.0.2/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-03-20 22:55:37.000000 fluxoperator-0.0.2/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.2/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-03-20 22:55:37.000000 fluxoperator-0.0.2/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-03-20 22:55:37.000000 fluxoperator-0.0.2/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-03-20 22:55:37.409297 fluxoperator-0.0.2/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2152 2023-03-20 22:55:32.000000 fluxoperator-0.0.2/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-03-20 22:55:37.409297 fluxoperator-0.0.2/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-03-20 22:37:12.000000 fluxoperator-0.0.2/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4925 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-03-20 19:10:45.000000 fluxoperator-0.0.2/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2676 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1504 2023-03-20 19:10:45.000000 fluxoperator-0.0.2/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10360 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6188 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1364 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1334 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-03-04 00:15:06.000000 fluxoperator-0.0.2/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-03-20 19:10:45.000000 fluxoperator-0.0.2/test/test_security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.432146 fluxoperator-0.0.21/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2667 2023-05-03 06:51:17.432146 fluxoperator-0.0.21/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.420147 fluxoperator-0.0.21/fluxoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1906 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.420147 fluxoperator-0.0.21/fluxoperator/api/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/api/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/api_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13137 2023-05-02 21:28:30.000000 fluxoperator-0.0.21/fluxoperator/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/configuration.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/fluxoperator/decorator.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/fluxoperator/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/exceptions.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.428146 fluxoperator-0.0.21/fluxoperator/models/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1430 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-05-02 07:00:32.000000 fluxoperator-0.0.21/fluxoperator/models/commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-05-02 07:00:32.000000 fluxoperator-0.0.21/fluxoperator/models/container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-05-02 21:28:30.000000 fluxoperator-0.0.21/fluxoperator/models/logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    25818 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5483 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14746 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4844 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.428146 fluxoperator-0.0.21/fluxoperator/resource/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/fluxoperator/resource/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/fluxoperator/resource/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5653 2023-05-02 21:28:30.000000 fluxoperator-0.0.21/fluxoperator/resource/pods.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/rest.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.420147 fluxoperator-0.0.21/fluxoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2667 2023-05-03 06:51:16.000000 fluxoperator-0.0.21/fluxoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1867 2023-05-03 06:51:17.000000 fluxoperator-0.0.21/fluxoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-03 06:51:16.000000 fluxoperator-0.0.21/fluxoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.21/fluxoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-05-03 06:51:17.000000 fluxoperator-0.0.21/fluxoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-05-03 06:51:17.000000 fluxoperator-0.0.21/fluxoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-05-03 06:51:17.432146 fluxoperator-0.0.21/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-05-02 21:28:22.000000 fluxoperator-0.0.21/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.432146 fluxoperator-0.0.21/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/test/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4925 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2676 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1504 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10360 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6188 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1364 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1334 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.2/PKG-INFO` & `fluxoperator-0.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.2
+Version: 0.0.21
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.2/fluxoperator/__init__.py` & `fluxoperator-0.0.21/fluxoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/api_client.py` & `fluxoperator-0.0.21/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/client.py` & `fluxoperator-0.0.21/fluxoperator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,22 +137,23 @@
                 # There will be a few connection errors before everything is ready
                 except Exception:
                     pass
 
             print()
             yield url
 
-    def stream_output(self, filename, stdout=True):
+    def stream_output(self, filename, stdout=True, timestamps=False):
         """
         Stream output, optionally printing also to stdout.
         """
         return self.ctrl.stream_output(
             filename=filename,
             stdout=stdout,
             namespace=self.namespace,
+            timestamps=timestamps,
             name=self.name,
             pod=self.broker_pod,
         )
 
     @timed
     def delete(self):
         """
@@ -228,28 +229,29 @@
 
         self.c = client.Configuration.get_default_copy()
         self.c.assert_hostname = False
         client.Configuration.set_default(self.c)
         self._core_v1 = core_v1_api.CoreV1Api()
         return self._core_v1
 
-    def stream_output(self, filename, name=None, namespace=None, pod=None, stdout=True):
+    def stream_output(self, filename, name=None, namespace=None, pod=None, stdout=True, timestamps=False):
         """
         Stream output, optionally printing also to stdout.
         """
         namespace = namespace or self.namespace
         pod = pod or self.get_broker_pod(name=name, namespace=namespace).metadata.name
         watcher = watch.Watch()
 
         # Stream output to file (should we return output too?)
         with open(filename, "w") as fd:
             for line in watcher.stream(
                 self.core_v1.read_namespaced_pod_log,
                 name=pod,
                 namespace=namespace,
+                timestamps=timestamps,
                 follow=True,
             ):
                 # Lines end with /r and we need to strip and add a newline
                 fd.write(line.strip() + "\n")
                 if stdout:
                     print(line)
 
@@ -378,14 +380,18 @@
 
             for pod in pod_list.items:
                 logger.debug(f"{pod.metadata.name} is in phase {pod.status.phase}")
 
                 # Don't include the cert generator pod
                 if "cert-generator" in pod.metadata.name:
                     continue
+
+                # Ignore services pod
+                if pod.metadata.name.endswith('-services'):
+                    continue
                 if pod.status.phase not in states:
                     time.sleep(retry_seconds)
                 elif pod.status.phase not in ["Terminating", "Succeeded"]:
                     ready.add(pod.metadata.name)
 
         if not quiet:
             states = '" or "'.join(states)
```

### Comparing `fluxoperator-0.0.2/fluxoperator/configuration.py` & `fluxoperator-0.0.21/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/decorator.py` & `fluxoperator-0.0.21/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/exceptions.py` & `fluxoperator-0.0.21/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/__init__.py` & `fluxoperator-0.0.21/fluxoperator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/commands.py` & `fluxoperator-0.0.21/fluxoperator/models/logging_spec.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,154 +14,182 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from fluxoperator.configuration import Configuration
 
 
-class Commands(object):
+class LoggingSpec(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'post': 'str',
-        'pre': 'str',
-        'prefix': 'str',
-        'run_flux_as_root': 'bool'
+        'debug': 'bool',
+        'quiet': 'bool',
+        'strict': 'bool',
+        'timed': 'bool',
+        'zeromq': 'bool'
     }
 
     attribute_map = {
-        'post': 'post',
-        'pre': 'pre',
-        'prefix': 'prefix',
-        'run_flux_as_root': 'runFluxAsRoot'
+        'debug': 'debug',
+        'quiet': 'quiet',
+        'strict': 'strict',
+        'timed': 'timed',
+        'zeromq': 'zeromq'
     }
 
-    def __init__(self, post='', pre='', prefix='', run_flux_as_root=False, local_vars_configuration=None):  # noqa: E501
-        """Commands - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, debug=False, quiet=False, strict=True, timed=False, zeromq=False, local_vars_configuration=None):  # noqa: E501
+        """LoggingSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._post = None
-        self._pre = None
-        self._prefix = None
-        self._run_flux_as_root = None
+        self._debug = None
+        self._quiet = None
+        self._strict = None
+        self._timed = None
+        self._zeromq = None
         self.discriminator = None
 
-        if post is not None:
-            self.post = post
-        if pre is not None:
-            self.pre = pre
-        if prefix is not None:
-            self.prefix = prefix
-        if run_flux_as_root is not None:
-            self.run_flux_as_root = run_flux_as_root
+        if debug is not None:
+            self.debug = debug
+        if quiet is not None:
+            self.quiet = quiet
+        if strict is not None:
+            self.strict = strict
+        if timed is not None:
+            self.timed = timed
+        if zeromq is not None:
+            self.zeromq = zeromq
 
     @property
-    def post(self):
-        """Gets the post of this Commands.  # noqa: E501
+    def debug(self):
+        """Gets the debug of this LoggingSpec.  # noqa: E501
 
-        post command is run in the entrypoint when the broker exits / finishes  # noqa: E501
+        Debug mode adds extra verbosity to Flux  # noqa: E501
 
-        :return: The post of this Commands.  # noqa: E501
-        :rtype: str
+        :return: The debug of this LoggingSpec.  # noqa: E501
+        :rtype: bool
+        """
+        return self._debug
+
+    @debug.setter
+    def debug(self, debug):
+        """Sets the debug of this LoggingSpec.
+
+        Debug mode adds extra verbosity to Flux  # noqa: E501
+
+        :param debug: The debug of this LoggingSpec.  # noqa: E501
+        :type debug: bool
+        """
+
+        self._debug = debug
+
+    @property
+    def quiet(self):
+        """Gets the quiet of this LoggingSpec.  # noqa: E501
+
+        Quiet mode silences all output so the job only shows the test running  # noqa: E501
+
+        :return: The quiet of this LoggingSpec.  # noqa: E501
+        :rtype: bool
         """
-        return self._post
+        return self._quiet
 
-    @post.setter
-    def post(self, post):
-        """Sets the post of this Commands.
+    @quiet.setter
+    def quiet(self, quiet):
+        """Sets the quiet of this LoggingSpec.
 
-        post command is run in the entrypoint when the broker exits / finishes  # noqa: E501
+        Quiet mode silences all output so the job only shows the test running  # noqa: E501
 
-        :param post: The post of this Commands.  # noqa: E501
-        :type post: str
+        :param quiet: The quiet of this LoggingSpec.  # noqa: E501
+        :type quiet: bool
         """
 
-        self._post = post
+        self._quiet = quiet
 
     @property
-    def pre(self):
-        """Gets the pre of this Commands.  # noqa: E501
+    def strict(self):
+        """Gets the strict of this LoggingSpec.  # noqa: E501
 
-        pre command is run after global PreCommand, before anything else  # noqa: E501
+        Strict mode ensures any failure will not continue in the job entrypoint  # noqa: E501
 
-        :return: The pre of this Commands.  # noqa: E501
-        :rtype: str
+        :return: The strict of this LoggingSpec.  # noqa: E501
+        :rtype: bool
         """
-        return self._pre
+        return self._strict
 
-    @pre.setter
-    def pre(self, pre):
-        """Sets the pre of this Commands.
+    @strict.setter
+    def strict(self, strict):
+        """Sets the strict of this LoggingSpec.
 
-        pre command is run after global PreCommand, before anything else  # noqa: E501
+        Strict mode ensures any failure will not continue in the job entrypoint  # noqa: E501
 
-        :param pre: The pre of this Commands.  # noqa: E501
-        :type pre: str
+        :param strict: The strict of this LoggingSpec.  # noqa: E501
+        :type strict: bool
         """
 
-        self._pre = pre
+        self._strict = strict
 
     @property
-    def prefix(self):
-        """Gets the prefix of this Commands.  # noqa: E501
+    def timed(self):
+        """Gets the timed of this LoggingSpec.  # noqa: E501
 
-        Prefix to flux start / submit / broker Typically used for a wrapper command to mount, etc.  # noqa: E501
+        Timed mode adds timing to Flux commands  # noqa: E501
 
-        :return: The prefix of this Commands.  # noqa: E501
-        :rtype: str
+        :return: The timed of this LoggingSpec.  # noqa: E501
+        :rtype: bool
         """
-        return self._prefix
+        return self._timed
 
-    @prefix.setter
-    def prefix(self, prefix):
-        """Sets the prefix of this Commands.
+    @timed.setter
+    def timed(self, timed):
+        """Sets the timed of this LoggingSpec.
 
-        Prefix to flux start / submit / broker Typically used for a wrapper command to mount, etc.  # noqa: E501
+        Timed mode adds timing to Flux commands  # noqa: E501
 
-        :param prefix: The prefix of this Commands.  # noqa: E501
-        :type prefix: str
+        :param timed: The timed of this LoggingSpec.  # noqa: E501
+        :type timed: bool
         """
 
-        self._prefix = prefix
+        self._timed = timed
 
     @property
-    def run_flux_as_root(self):
-        """Gets the run_flux_as_root of this Commands.  # noqa: E501
+    def zeromq(self):
+        """Gets the zeromq of this LoggingSpec.  # noqa: E501
 
-        Run flux start as root - required for some storage binds  # noqa: E501
+        Enable Zeromq logging  # noqa: E501
 
-        :return: The run_flux_as_root of this Commands.  # noqa: E501
+        :return: The zeromq of this LoggingSpec.  # noqa: E501
         :rtype: bool
         """
-        return self._run_flux_as_root
+        return self._zeromq
 
-    @run_flux_as_root.setter
-    def run_flux_as_root(self, run_flux_as_root):
-        """Sets the run_flux_as_root of this Commands.
+    @zeromq.setter
+    def zeromq(self, zeromq):
+        """Sets the zeromq of this LoggingSpec.
 
-        Run flux start as root - required for some storage binds  # noqa: E501
+        Enable Zeromq logging  # noqa: E501
 
-        :param run_flux_as_root: The run_flux_as_root of this Commands.  # noqa: E501
-        :type run_flux_as_root: bool
+        :param zeromq: The zeromq of this LoggingSpec.  # noqa: E501
+        :type zeromq: bool
         """
 
-        self._run_flux_as_root = run_flux_as_root
+        self._zeromq = zeromq
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -197,18 +225,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Commands):
+        if not isinstance(other, LoggingSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Commands):
+        if not isinstance(other, LoggingSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fluxoperator-0.0.2/fluxoperator/models/container_resources.py` & `fluxoperator-0.0.21/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/container_volume.py` & `fluxoperator-0.0.21/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/flux_restful.py` & `fluxoperator-0.0.21/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/flux_user.py` & `fluxoperator-0.0.21/fluxoperator/models/flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/life_cycle.py` & `fluxoperator-0.0.21/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/logging_spec.py` & `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_existing_volume.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,154 +14,124 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from fluxoperator.configuration import Configuration
 
 
-class LoggingSpec(object):
+class MiniClusterExistingVolume(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'debug': 'bool',
-        'quiet': 'bool',
-        'strict': 'bool',
-        'timed': 'bool'
+        'claim_name': 'str',
+        'path': 'str',
+        'read_only': 'bool'
     }
 
     attribute_map = {
-        'debug': 'debug',
-        'quiet': 'quiet',
-        'strict': 'strict',
-        'timed': 'timed'
+        'claim_name': 'claimName',
+        'path': 'path',
+        'read_only': 'readOnly'
     }
 
-    def __init__(self, debug=False, quiet=False, strict=True, timed=False, local_vars_configuration=None):  # noqa: E501
-        """LoggingSpec - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, claim_name='', path='', read_only=False, local_vars_configuration=None):  # noqa: E501
+        """MiniClusterExistingVolume - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._debug = None
-        self._quiet = None
-        self._strict = None
-        self._timed = None
+        self._claim_name = None
+        self._path = None
+        self._read_only = None
         self.discriminator = None
 
-        if debug is not None:
-            self.debug = debug
-        if quiet is not None:
-            self.quiet = quiet
-        if strict is not None:
-            self.strict = strict
-        if timed is not None:
-            self.timed = timed
+        self.claim_name = claim_name
+        self.path = path
+        if read_only is not None:
+            self.read_only = read_only
 
     @property
-    def debug(self):
-        """Gets the debug of this LoggingSpec.  # noqa: E501
+    def claim_name(self):
+        """Gets the claim_name of this MiniClusterExistingVolume.  # noqa: E501
 
-        Debug mode adds extra verbosity to Flux  # noqa: E501
 
-        :return: The debug of this LoggingSpec.  # noqa: E501
-        :rtype: bool
+        :return: The claim_name of this MiniClusterExistingVolume.  # noqa: E501
+        :rtype: str
         """
-        return self._debug
+        return self._claim_name
 
-    @debug.setter
-    def debug(self, debug):
-        """Sets the debug of this LoggingSpec.
+    @claim_name.setter
+    def claim_name(self, claim_name):
+        """Sets the claim_name of this MiniClusterExistingVolume.
 
-        Debug mode adds extra verbosity to Flux  # noqa: E501
 
-        :param debug: The debug of this LoggingSpec.  # noqa: E501
-        :type debug: bool
+        :param claim_name: The claim_name of this MiniClusterExistingVolume.  # noqa: E501
+        :type claim_name: str
         """
+        if self.local_vars_configuration.client_side_validation and claim_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `claim_name`, must not be `None`")  # noqa: E501
 
-        self._debug = debug
+        self._claim_name = claim_name
 
     @property
-    def quiet(self):
-        """Gets the quiet of this LoggingSpec.  # noqa: E501
-
-        Quiet mode silences all output so the job only shows the test running  # noqa: E501
+    def path(self):
+        """Gets the path of this MiniClusterExistingVolume.  # noqa: E501
 
-        :return: The quiet of this LoggingSpec.  # noqa: E501
-        :rtype: bool
-        """
-        return self._quiet
+        Path and claim name are always required  # noqa: E501
 
-    @quiet.setter
-    def quiet(self, quiet):
-        """Sets the quiet of this LoggingSpec.
-
-        Quiet mode silences all output so the job only shows the test running  # noqa: E501
-
-        :param quiet: The quiet of this LoggingSpec.  # noqa: E501
-        :type quiet: bool
-        """
-
-        self._quiet = quiet
-
-    @property
-    def strict(self):
-        """Gets the strict of this LoggingSpec.  # noqa: E501
-
-        Strict mode ensures any failure will not continue in the job entrypoint  # noqa: E501
-
-        :return: The strict of this LoggingSpec.  # noqa: E501
-        :rtype: bool
+        :return: The path of this MiniClusterExistingVolume.  # noqa: E501
+        :rtype: str
         """
-        return self._strict
+        return self._path
 
-    @strict.setter
-    def strict(self, strict):
-        """Sets the strict of this LoggingSpec.
+    @path.setter
+    def path(self, path):
+        """Sets the path of this MiniClusterExistingVolume.
 
-        Strict mode ensures any failure will not continue in the job entrypoint  # noqa: E501
+        Path and claim name are always required  # noqa: E501
 
-        :param strict: The strict of this LoggingSpec.  # noqa: E501
-        :type strict: bool
+        :param path: The path of this MiniClusterExistingVolume.  # noqa: E501
+        :type path: str
         """
+        if self.local_vars_configuration.client_side_validation and path is None:  # noqa: E501
+            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
-        self._strict = strict
+        self._path = path
 
     @property
-    def timed(self):
-        """Gets the timed of this LoggingSpec.  # noqa: E501
+    def read_only(self):
+        """Gets the read_only of this MiniClusterExistingVolume.  # noqa: E501
 
-        Timed mode adds timing to Flux commands  # noqa: E501
 
-        :return: The timed of this LoggingSpec.  # noqa: E501
+        :return: The read_only of this MiniClusterExistingVolume.  # noqa: E501
         :rtype: bool
         """
-        return self._timed
+        return self._read_only
 
-    @timed.setter
-    def timed(self, timed):
-        """Sets the timed of this LoggingSpec.
+    @read_only.setter
+    def read_only(self, read_only):
+        """Sets the read_only of this MiniClusterExistingVolume.
 
-        Timed mode adds timing to Flux commands  # noqa: E501
 
-        :param timed: The timed of this LoggingSpec.  # noqa: E501
-        :type timed: bool
+        :param read_only: The read_only of this MiniClusterExistingVolume.  # noqa: E501
+        :type read_only: bool
         """
 
-        self._timed = timed
+        self._read_only = read_only
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -197,18 +167,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LoggingSpec):
+        if not isinstance(other, MiniClusterExistingVolume):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LoggingSpec):
+        if not isinstance(other, MiniClusterExistingVolume):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fluxoperator-0.0.2/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.0.21/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,93 +29,106 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'batch': 'bool',
+        'batch_raw': 'bool',
         'command': 'str',
         'commands': 'Commands',
         'cores': 'int',
         'diagnostics': 'bool',
         'environment': 'dict(str, str)',
         'existing_volumes': 'dict(str, MiniClusterExistingVolume)',
         'flux_log_level': 'int',
         'flux_option_flags': 'str',
         'flux_user': 'FluxUser',
         'image': 'str',
         'image_pull_secret': 'str',
         'launcher': 'bool',
         'life_cycle': 'LifeCycle',
+        'logs': 'str',
         'name': 'str',
         'ports': 'list[int]',
         'pre_command': 'str',
         'pull_always': 'bool',
         'resources': 'ContainerResources',
         'run_flux': 'bool',
         'security_context': 'SecurityContext',
         'volumes': 'dict(str, ContainerVolume)',
         'working_dir': 'str'
     }
 
     attribute_map = {
+        'batch': 'batch',
+        'batch_raw': 'batchRaw',
         'command': 'command',
         'commands': 'commands',
         'cores': 'cores',
         'diagnostics': 'diagnostics',
         'environment': 'environment',
         'existing_volumes': 'existingVolumes',
         'flux_log_level': 'fluxLogLevel',
         'flux_option_flags': 'fluxOptionFlags',
         'flux_user': 'fluxUser',
         'image': 'image',
         'image_pull_secret': 'imagePullSecret',
         'launcher': 'launcher',
         'life_cycle': 'lifeCycle',
+        'logs': 'logs',
         'name': 'name',
         'ports': 'ports',
         'pre_command': 'preCommand',
         'pull_always': 'pullAlways',
         'resources': 'resources',
         'run_flux': 'runFlux',
         'security_context': 'securityContext',
         'volumes': 'volumes',
         'working_dir': 'workingDir'
     }
 
-    def __init__(self, command='', commands=None, cores=0, diagnostics=False, environment=None, existing_volumes=None, flux_log_level=6, flux_option_flags='', flux_user=None, image='ghcr.io/rse-ops/accounting:app-latest', image_pull_secret='', launcher=False, life_cycle=None, name='', ports=None, pre_command='', pull_always=False, resources=None, run_flux=False, security_context=None, volumes=None, working_dir='', local_vars_configuration=None):  # noqa: E501
+    def __init__(self, batch=False, batch_raw=False, command='', commands=None, cores=0, diagnostics=False, environment=None, existing_volumes=None, flux_log_level=6, flux_option_flags='', flux_user=None, image='ghcr.io/rse-ops/accounting:app-latest', image_pull_secret='', launcher=False, life_cycle=None, logs='', name='', ports=None, pre_command='', pull_always=False, resources=None, run_flux=False, security_context=None, volumes=None, working_dir='', local_vars_configuration=None):  # noqa: E501
         """MiniClusterContainer - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._batch = None
+        self._batch_raw = None
         self._command = None
         self._commands = None
         self._cores = None
         self._diagnostics = None
         self._environment = None
         self._existing_volumes = None
         self._flux_log_level = None
         self._flux_option_flags = None
         self._flux_user = None
         self._image = None
         self._image_pull_secret = None
         self._launcher = None
         self._life_cycle = None
+        self._logs = None
         self._name = None
         self._ports = None
         self._pre_command = None
         self._pull_always = None
         self._resources = None
         self._run_flux = None
         self._security_context = None
         self._volumes = None
         self._working_dir = None
         self.discriminator = None
 
+        if batch is not None:
+            self.batch = batch
+        if batch_raw is not None:
+            self.batch_raw = batch_raw
         if command is not None:
             self.command = command
         if commands is not None:
             self.commands = commands
         if cores is not None:
             self.cores = cores
         if diagnostics is not None:
@@ -134,14 +147,16 @@
             self.image = image
         if image_pull_secret is not None:
             self.image_pull_secret = image_pull_secret
         if launcher is not None:
             self.launcher = launcher
         if life_cycle is not None:
             self.life_cycle = life_cycle
+        if logs is not None:
+            self.logs = logs
         if name is not None:
             self.name = name
         if ports is not None:
             self.ports = ports
         if pre_command is not None:
             self.pre_command = pre_command
         if pull_always is not None:
@@ -154,14 +169,60 @@
             self.security_context = security_context
         if volumes is not None:
             self.volumes = volumes
         if working_dir is not None:
             self.working_dir = working_dir
 
     @property
+    def batch(self):
+        """Gets the batch of this MiniClusterContainer.  # noqa: E501
+
+        Indicate that the command is a batch job that will be written to a file to submit  # noqa: E501
+
+        :return: The batch of this MiniClusterContainer.  # noqa: E501
+        :rtype: bool
+        """
+        return self._batch
+
+    @batch.setter
+    def batch(self, batch):
+        """Sets the batch of this MiniClusterContainer.
+
+        Indicate that the command is a batch job that will be written to a file to submit  # noqa: E501
+
+        :param batch: The batch of this MiniClusterContainer.  # noqa: E501
+        :type batch: bool
+        """
+
+        self._batch = batch
+
+    @property
+    def batch_raw(self):
+        """Gets the batch_raw of this MiniClusterContainer.  # noqa: E501
+
+        Don't wrap batch commands in flux submit (provide custom logic myself)  # noqa: E501
+
+        :return: The batch_raw of this MiniClusterContainer.  # noqa: E501
+        :rtype: bool
+        """
+        return self._batch_raw
+
+    @batch_raw.setter
+    def batch_raw(self, batch_raw):
+        """Sets the batch_raw of this MiniClusterContainer.
+
+        Don't wrap batch commands in flux submit (provide custom logic myself)  # noqa: E501
+
+        :param batch_raw: The batch_raw of this MiniClusterContainer.  # noqa: E501
+        :type batch_raw: bool
+        """
+
+        self._batch_raw = batch_raw
+
+    @property
     def command(self):
         """Gets the command of this MiniClusterContainer.  # noqa: E501
 
         Single user executable to provide to flux start  # noqa: E501
 
         :return: The command of this MiniClusterContainer.  # noqa: E501
         :rtype: str
@@ -447,14 +508,37 @@
         :param life_cycle: The life_cycle of this MiniClusterContainer.  # noqa: E501
         :type life_cycle: LifeCycle
         """
 
         self._life_cycle = life_cycle
 
     @property
+    def logs(self):
+        """Gets the logs of this MiniClusterContainer.  # noqa: E501
+
+        Log output directory  # noqa: E501
+
+        :return: The logs of this MiniClusterContainer.  # noqa: E501
+        :rtype: str
+        """
+        return self._logs
+
+    @logs.setter
+    def logs(self, logs):
+        """Sets the logs of this MiniClusterContainer.
+
+        Log output directory  # noqa: E501
+
+        :param logs: The logs of this MiniClusterContainer.  # noqa: E501
+        :type logs: str
+        """
+
+        self._logs = logs
+
+    @property
     def name(self):
         """Gets the name of this MiniClusterContainer.  # noqa: E501
 
         Container name is only required for non flux runners  # noqa: E501
 
         :return: The name of this MiniClusterContainer.  # noqa: E501
         :rtype: str
```

### Comparing `fluxoperator-0.0.2/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_user.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,124 +14,97 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from fluxoperator.configuration import Configuration
 
 
-class MiniClusterExistingVolume(object):
+class MiniClusterUser(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'claim_name': 'str',
-        'path': 'str',
-        'read_only': 'bool'
+        'name': 'str',
+        'password': 'str'
     }
 
     attribute_map = {
-        'claim_name': 'claimName',
-        'path': 'path',
-        'read_only': 'readOnly'
+        'name': 'name',
+        'password': 'password'
     }
 
-    def __init__(self, claim_name='', path='', read_only=False, local_vars_configuration=None):  # noqa: E501
-        """MiniClusterExistingVolume - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name='', password='', local_vars_configuration=None):  # noqa: E501
+        """MiniClusterUser - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._claim_name = None
-        self._path = None
-        self._read_only = None
+        self._name = None
+        self._password = None
         self.discriminator = None
 
-        self.claim_name = claim_name
-        self.path = path
-        if read_only is not None:
-            self.read_only = read_only
+        self.name = name
+        if password is not None:
+            self.password = password
 
     @property
-    def claim_name(self):
-        """Gets the claim_name of this MiniClusterExistingVolume.  # noqa: E501
+    def name(self):
+        """Gets the name of this MiniClusterUser.  # noqa: E501
 
+        If a user is defined, the username is required  # noqa: E501
 
-        :return: The claim_name of this MiniClusterExistingVolume.  # noqa: E501
+        :return: The name of this MiniClusterUser.  # noqa: E501
         :rtype: str
         """
-        return self._claim_name
+        return self._name
 
-    @claim_name.setter
-    def claim_name(self, claim_name):
-        """Sets the claim_name of this MiniClusterExistingVolume.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this MiniClusterUser.
 
+        If a user is defined, the username is required  # noqa: E501
 
-        :param claim_name: The claim_name of this MiniClusterExistingVolume.  # noqa: E501
-        :type claim_name: str
+        :param name: The name of this MiniClusterUser.  # noqa: E501
+        :type name: str
         """
-        if self.local_vars_configuration.client_side_validation and claim_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `claim_name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._claim_name = claim_name
+        self._name = name
 
     @property
-    def path(self):
-        """Gets the path of this MiniClusterExistingVolume.  # noqa: E501
+    def password(self):
+        """Gets the password of this MiniClusterUser.  # noqa: E501
 
-        Path and claim name are always required  # noqa: E501
 
-        :return: The path of this MiniClusterExistingVolume.  # noqa: E501
+        :return: The password of this MiniClusterUser.  # noqa: E501
         :rtype: str
         """
-        return self._path
+        return self._password
 
-    @path.setter
-    def path(self, path):
-        """Sets the path of this MiniClusterExistingVolume.
+    @password.setter
+    def password(self, password):
+        """Sets the password of this MiniClusterUser.
 
-        Path and claim name are always required  # noqa: E501
 
-        :param path: The path of this MiniClusterExistingVolume.  # noqa: E501
-        :type path: str
+        :param password: The password of this MiniClusterUser.  # noqa: E501
+        :type password: str
         """
-        if self.local_vars_configuration.client_side_validation and path is None:  # noqa: E501
-            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
-        self._path = path
-
-    @property
-    def read_only(self):
-        """Gets the read_only of this MiniClusterExistingVolume.  # noqa: E501
-
-
-        :return: The read_only of this MiniClusterExistingVolume.  # noqa: E501
-        :rtype: bool
-        """
-        return self._read_only
-
-    @read_only.setter
-    def read_only(self, read_only):
-        """Sets the read_only of this MiniClusterExistingVolume.
-
-
-        :param read_only: The read_only of this MiniClusterExistingVolume.  # noqa: E501
-        :type read_only: bool
-        """
-
-        self._read_only = read_only
+        self._password = password
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -167,18 +140,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MiniClusterExistingVolume):
+        if not isinstance(other, MiniClusterUser):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MiniClusterExistingVolume):
+        if not isinstance(other, MiniClusterUser):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fluxoperator-0.0.2/fluxoperator/models/mini_cluster_list.py` & `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         'containers': 'list[MiniClusterContainer]',
         'deadline_seconds': 'int',
         'flux_restful': 'FluxRestful',
         'interactive': 'bool',
         'job_labels': 'dict(str, str)',
         'logging': 'LoggingSpec',
         'pod': 'PodSpec',
+        'services': 'list[MiniClusterContainer]',
         'size': 'int',
         'tasks': 'int',
         'users': 'list[MiniClusterUser]',
         'volumes': 'dict(str, MiniClusterVolume)'
     }
 
     attribute_map = {
@@ -54,35 +55,37 @@
         'containers': 'containers',
         'deadline_seconds': 'deadlineSeconds',
         'flux_restful': 'fluxRestful',
         'interactive': 'interactive',
         'job_labels': 'jobLabels',
         'logging': 'logging',
         'pod': 'pod',
+        'services': 'services',
         'size': 'size',
         'tasks': 'tasks',
         'users': 'users',
         'volumes': 'volumes'
     }
 
-    def __init__(self, archive=None, cleanup=False, containers=None, deadline_seconds=31500000, flux_restful=None, interactive=False, job_labels=None, logging=None, pod=None, size=1, tasks=1, users=None, volumes=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, archive=None, cleanup=False, containers=None, deadline_seconds=31500000, flux_restful=None, interactive=False, job_labels=None, logging=None, pod=None, services=None, size=1, tasks=1, users=None, volumes=None, local_vars_configuration=None):  # noqa: E501
         """MiniClusterSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._archive = None
         self._cleanup = None
         self._containers = None
         self._deadline_seconds = None
         self._flux_restful = None
         self._interactive = None
         self._job_labels = None
         self._logging = None
         self._pod = None
+        self._services = None
         self._size = None
         self._tasks = None
         self._users = None
         self._volumes = None
         self.discriminator = None
 
         if archive is not None:
@@ -98,14 +101,16 @@
             self.interactive = interactive
         if job_labels is not None:
             self.job_labels = job_labels
         if logging is not None:
             self.logging = logging
         if pod is not None:
             self.pod = pod
+        if services is not None:
+            self.services = services
         if size is not None:
             self.size = size
         if tasks is not None:
             self.tasks = tasks
         if users is not None:
             self.users = users
         if volumes is not None:
@@ -309,14 +314,37 @@
         :param pod: The pod of this MiniClusterSpec.  # noqa: E501
         :type pod: PodSpec
         """
 
         self._pod = pod
 
     @property
+    def services(self):
+        """Gets the services of this MiniClusterSpec.  # noqa: E501
+
+        Services are one or more service containers to bring up alongside the MiniCluster.  # noqa: E501
+
+        :return: The services of this MiniClusterSpec.  # noqa: E501
+        :rtype: list[MiniClusterContainer]
+        """
+        return self._services
+
+    @services.setter
+    def services(self, services):
+        """Sets the services of this MiniClusterSpec.
+
+        Services are one or more service containers to bring up alongside the MiniCluster.  # noqa: E501
+
+        :param services: The services of this MiniClusterSpec.  # noqa: E501
+        :type services: list[MiniClusterContainer]
+        """
+
+        self._services = services
+
+    @property
     def size(self):
         """Gets the size of this MiniClusterSpec.  # noqa: E501
 
         Size (number of job pods to run, size of minicluster in pods)  # noqa: E501
 
         :return: The size of this MiniClusterSpec.  # noqa: E501
         :rtype: int
```

### Comparing `fluxoperator-0.0.2/fluxoperator/models/mini_cluster_status.py` & `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/pod_spec.py` & `fluxoperator-0.0.21/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/models/security_context.py` & `fluxoperator-0.0.21/fluxoperator/models/security_context.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/resource/network.py` & `fluxoperator-0.0.21/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator/resource/pods.py` & `fluxoperator-0.0.21/fluxoperator/resource/pods.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 _objects = ["logging", "volumes", "resources", "flux_restful", "container", "resources"]
 
 
 def _get_logging_spec(logging):
     """
     Return models.Logging
     """
-    logging_defaults = {"debug": False, "quiet": False, "strict": True, "timed": False}
+    logging_defaults = {
+        "debug": False,
+        "quiet": False,
+        "strict": True,
+        "timed": False,
+        "zeromq": False,
+    }
 
     for k, v in (logging or {}).items():
         if k in logging_defaults and v in [True, False]:
             logging_defaults[k] = v
 
     return models.LoggingSpec(**logging_defaults)
 
@@ -45,15 +51,14 @@
     for k in models.MiniClusterContainer.attribute_map:
         if k in container and k not in _objects:
             container_kwargs[k] = container[k]
         elif k in container and k == "volumes":
             container_kwargs[k] = _get_container_volumes(container[k])
         elif k in container and k == "resources":
             container_kwargs["resources"] = _get_container_resources_spec(container[k])
-
     return models.MiniClusterContainer(**container_kwargs)
 
 
 def _get_container_resources_spec(resources):
     """
     Get container resources spec.
     """
```

### Comparing `fluxoperator-0.0.2/fluxoperator/rest.py` & `fluxoperator-0.0.21/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.0.21/fluxoperator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.2
+Version: 0.0.21
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.2/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.0.21/fluxoperator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/setup.py` & `fluxoperator-0.0.21/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.2",
+        version="0.0.21",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.2/test/test_commands.py` & `fluxoperator-0.0.21/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_container_resources.py` & `fluxoperator-0.0.21/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_container_volume.py` & `fluxoperator-0.0.21/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_flux_restful.py` & `fluxoperator-0.0.21/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_flux_user.py` & `fluxoperator-0.0.21/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_life_cycle.py` & `fluxoperator-0.0.21/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_logging_spec.py` & `fluxoperator-0.0.21/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_mini_cluster.py` & `fluxoperator-0.0.21/test/test_mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_mini_cluster_archive.py` & `fluxoperator-0.0.21/test/test_mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_mini_cluster_container.py` & `fluxoperator-0.0.21/test/test_mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.0.21/test/test_mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_mini_cluster_list.py` & `fluxoperator-0.0.21/test/test_mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_mini_cluster_spec.py` & `fluxoperator-0.0.21/test/test_mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_mini_cluster_status.py` & `fluxoperator-0.0.21/test/test_mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_mini_cluster_user.py` & `fluxoperator-0.0.21/test/test_mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_mini_cluster_volume.py` & `fluxoperator-0.0.21/test/test_mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_pod_spec.py` & `fluxoperator-0.0.21/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.2/test/test_security_context.py` & `fluxoperator-0.0.21/test/test_security_context.py`

 * *Files identical despite different names*

