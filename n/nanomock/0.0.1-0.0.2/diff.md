# Comparing `tmp/nanomock-0.0.1.tar.gz` & `tmp/nanomock-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomock-0.0.1.tar", last modified: Tue May  2 13:43:07 2023, max compression
+gzip compressed data, was "nanomock-0.0.2.tar", last modified: Wed May  3 09:31:35 2023, max compression
```

## Comparing `nanomock-0.0.1.tar` & `nanomock-0.0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 13:35:20.000000 nanomock-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2959 2023-05-02 13:43:07.332840 nanomock-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2743 2023-05-02 13:35:20.000000 nanomock-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.328840 nanomock-0.0.1/nanomock/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-02 09:54:26.000000 nanomock-0.0.1/nanomock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 11:22:58.000000 nanomock-0.0.1/nanomock/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:05.000000 nanomock-0.0.1/nanomock/internal/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-01 20:18:12.000000 nanomock-0.0.1/nanomock/internal/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-01 20:40:09.000000 nanomock-0.0.1/nanomock/internal/data/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:25.000000 nanomock-0.0.1/nanomock/internal/data/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-01 20:18:12.000000 nanomock-0.0.1/nanomock/internal/data/services/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-01 20:40:09.000000 nanomock-0.0.1/nanomock/internal/data/services/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/custom_Dockerfile
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/default_config-node.toml
--rw-r--r--   0 root         (0) root         (0)      298 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/default_config-node_voting-disabled.toml
--rw-r--r--   0 root         (0) root         (0)      220 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/default_config-rpc.toml
--rw-r--r--   0 root         (0) root         (0)     1822 2023-05-01 19:50:09.000000 nanomock-0.0.1/nanomock/internal/data/services/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/nanolooker/
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/nanolooker/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:55.000000 nanomock-0.0.1/nanomock/internal/data/services/nanolooker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/nanomonitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:59.000000 nanomock-0.0.1/nanomock/internal/data/services/nanomonitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/nanomonitor/default_config.php
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/nanoticker/
--rw-r--r--   0 root         (0) root         (0)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/nanoticker/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:02.000000 nanomock-0.0.1/nanomock/internal/data/services/nanoticker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      467 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/nanovotevisu/
--rw-r--r--   0 root         (0) root         (0)      768 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/nanovotevisu/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:05.000000 nanomock-0.0.1/nanomock/internal/data/services/nanovotevisu/__init__.py
--rw-r--r--   0 root         (0) root         (0)      504 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/promexporter/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/promexporter/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:14.000000 nanomock-0.0.1/nanomock/internal/data/services/promexporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/promexporter/default_docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.328840 nanomock-0.0.1/nanomock/internal/data/services/promexporter/grafana/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.328840 nanomock-0.0.1/nanomock/internal/data/services/promexporter/grafana/provisioning/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
--rw-r--r--   0 root         (0) root         (0)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
--rw-r--r--   0 root         (0) root         (0)      515 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/promexporter/prometheus.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/internal/data/services/tcpdump/
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/tcpdump/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:10.000000 nanomock-0.0.1/nanomock/internal/data/services/tcpdump/__init__.py
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-27 20:34:19.000000 nanomock-0.0.1/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.1/nanomock/internal/dependency_checker.py
--rw-r--r--   0 root         (0) root         (0)    26984 2023-05-02 13:32:24.000000 nanomock-0.0.1/nanomock/internal/nl_block_tools.py
--rw-r--r--   0 root         (0) root         (0)     6944 2023-05-02 13:32:24.000000 nanomock-0.0.1/nanomock/internal/nl_initialise.py
--rw-r--r--   0 root         (0) root         (0)     3599 2023-05-02 13:32:24.000000 nanomock-0.0.1/nanomock/internal/utils.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-05-02 13:34:05.000000 nanomock-0.0.1/nanomock/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.332840 nanomock-0.0.1/nanomock/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 15:36:50.000000 nanomock-0.0.1/nanomock/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.1/nanomock/modules/nl_nanolib.py
--rw-r--r--   0 root         (0) root         (0)    41310 2023-05-02 13:32:25.000000 nanomock-0.0.1/nanomock/modules/nl_parse_config.py
--rw-r--r--   0 root         (0) root         (0)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.1/nanomock/modules/nl_rpc.py
--rw-r--r--   0 root         (0) root         (0)    20325 2023-05-02 13:38:36.000000 nanomock-0.0.1/nanomock/nanomock_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:43:07.328840 nanomock-0.0.1/nanomock.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2959 2023-05-02 13:43:07.000000 nanomock-0.0.1/nanomock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2855 2023-05-02 13:43:07.000000 nanomock-0.0.1/nanomock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 13:43:07.000000 nanomock-0.0.1/nanomock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-02 13:43:07.000000 nanomock-0.0.1/nanomock.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-02 13:43:07.000000 nanomock-0.0.1/nanomock.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-02 13:43:07.000000 nanomock-0.0.1/nanomock.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 13:43:07.332840 nanomock-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-02 13:35:21.000000 nanomock-0.0.1/setup.py
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.808418 nanomock-0.0.2/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       44 2023-05-02 13:35:20.000000 nanomock-0.0.2/MANIFEST.in
+-rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)     2959 2023-05-03 09:31:35.808418 nanomock-0.0.2/PKG-INFO
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2743 2023-05-02 22:46:21.000000 nanomock-0.0.2/README.md
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       22 2023-05-03 09:31:09.000000 nanomock-0.0.2/nanomock/__init__.py
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-01 11:22:58.000000 nanomock-0.0.2/nanomock/internal/__init__.py
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/data/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-01 19:50:05.000000 nanomock-0.0.2/nanomock/internal/data/__init__.py
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/data/__pycache__/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      198 2023-05-01 20:18:12.000000 nanomock-0.0.2/nanomock/internal/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      168 2023-05-01 20:40:09.000000 nanomock-0.0.2/nanomock/internal/data/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/data/services/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-01 19:50:25.000000 nanomock-0.0.2/nanomock/internal/data/services/__init__.py
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/data/services/__pycache__/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      207 2023-05-01 20:18:12.000000 nanomock-0.0.2/nanomock/internal/data/services/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      177 2023-05-01 20:40:09.000000 nanomock-0.0.2/nanomock/internal/data/services/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      432 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/custom_Dockerfile
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      297 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/default_config-node.toml
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      298 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/default_config-node_voting-disabled.toml
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      220 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/default_config-rpc.toml
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1824 2023-05-03 07:50:15.000000 nanomock-0.0.2/nanomock/internal/data/services/default_docker-compose.yml
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/data/services/nanolooker/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      960 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/nanolooker/Dockerfile
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:41:55.000000 nanomock-0.0.2/nanomock/internal/data/services/nanolooker/__init__.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1213 2023-05-03 09:06:45.000000 nanomock-0.0.2/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/data/services/nanomonitor/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:41:59.000000 nanomock-0.0.2/nanomock/internal/data/services/nanomonitor/__init__.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      659 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/nanomonitor/default_config.php
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      354 2023-05-03 09:06:45.000000 nanomock-0.0.2/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/data/services/nanoticker/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/nanoticker/Dockerfile
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:02.000000 nanomock-0.0.2/nanomock/internal/data/services/nanoticker/__init__.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      468 2023-05-03 09:06:45.000000 nanomock-0.0.2/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.808418 nanomock-0.0.2/nanomock/internal/data/services/nanovotevisu/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      768 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/nanovotevisu/Dockerfile
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:05.000000 nanomock-0.0.2/nanomock/internal/data/services/nanovotevisu/__init__.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      505 2023-05-03 09:06:45.000000 nanomock-0.0.2/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      325 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.808418 nanomock-0.0.2/nanomock/internal/data/services/promexporter/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      323 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/promexporter/Dockerfile
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:14.000000 nanomock-0.0.2/nanomock/internal/data/services/promexporter/__init__.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1557 2023-05-03 09:09:15.000000 nanomock-0.0.2/nanomock/internal/data/services/promexporter/default_docker-compose.yml
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      422 2023-05-03 07:50:15.000000 nanomock-0.0.2/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/data/services/promexporter/grafana/
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock/internal/data/services/promexporter/grafana/provisioning/
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.808418 nanomock-0.0.2/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      132 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.808418 nanomock-0.0.2/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      515 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/promexporter/prometheus.yml
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.808418 nanomock-0.0.2/nanomock/internal/data/services/tcpdump/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      119 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/tcpdump/Dockerfile
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:10.000000 nanomock-0.0.2/nanomock/internal/data/services/tcpdump/__init__.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      223 2023-05-03 09:06:45.000000 nanomock-0.0.2/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      685 2023-04-27 20:34:19.000000 nanomock-0.0.2/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.2/nanomock/internal/dependency_checker.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    26984 2023-05-02 13:32:24.000000 nanomock-0.0.2/nanomock/internal/nl_block_tools.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     7682 2023-05-02 21:23:27.000000 nanomock-0.0.2/nanomock/internal/nl_initialise.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     4514 2023-05-03 09:19:59.000000 nanomock-0.0.2/nanomock/internal/utils.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1539 2023-05-02 22:39:42.000000 nanomock-0.0.2/nanomock/main.py
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.808418 nanomock-0.0.2/nanomock/modules/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-04-27 15:36:50.000000 nanomock-0.0.2/nanomock/modules/__init__.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.2/nanomock/modules/nl_nanolib.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    43584 2023-05-03 09:14:07.000000 nanomock-0.0.2/nanomock/modules/nl_parse_config.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.2/nanomock/modules/nl_rpc.py
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    19910 2023-05-03 07:07:28.000000 nanomock-0.0.2/nanomock/nanomock_manager.py
+drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 09:31:35.804418 nanomock-0.0.2/nanomock.egg-info/
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2959 2023-05-03 09:31:35.000000 nanomock-0.0.2/nanomock.egg-info/PKG-INFO
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2855 2023-05-03 09:31:35.000000 nanomock-0.0.2/nanomock.egg-info/SOURCES.txt
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        1 2023-05-03 09:31:35.000000 nanomock-0.0.2/nanomock.egg-info/dependency_links.txt
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       48 2023-05-03 09:31:35.000000 nanomock-0.0.2/nanomock.egg-info/entry_points.txt
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       54 2023-05-03 09:31:35.000000 nanomock-0.0.2/nanomock.egg-info/requires.txt
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        9 2023-05-03 09:31:35.000000 nanomock-0.0.2/nanomock.egg-info/top_level.txt
+-rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)       38 2023-05-03 09:31:35.808418 nanomock-0.0.2/setup.cfg
+-rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      784 2023-05-03 09:30:51.000000 nanomock-0.0.2/setup.py
```

### Comparing `nanomock-0.0.1/PKG-INFO` & `nanomock-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: nanomock
-Version: 0.0.1
-Summary: Create local dockerized nano-currency networks
-Home-page: https://github.com/gr0vity-dev/nanomock
-Author: gr0vity
-Description-Content-Type: text/markdown
-
 # nano-local
 
 A one click [nano-currency](https://nano.org) block-lattice environment on your local computer.
 This project aims to easily spin up an integration environment with multiple nano nodes.
 The local network is highly customizable.
 All configuration is done inside the config file : `nanonet/nl_config.toml`
 
@@ -21,15 +13,15 @@
 
 ## Quickstart :
 
 #### Install the library :
 
 To install the library you can
 - clone the respository and run `pip3 install .`
-- or run `pip3 install nanomock`to download teh latest version from PyPi
+- or run `pip3 install nanomock`to download the latest version from PyPi
 
 This gives you access to `nanomock {command}` command which will use `your_current_dir`as its entry point.
 
 #### Spin up a network :
 
 | Action            | Code                                              | Description  
 | :----------       |:---------------------------------------------     | -----
```

### Comparing `nanomock-0.0.1/README.md` & `nanomock-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: nanomock
+Version: 0.0.2
+Summary: Create local dockerized nano-currency networks
+Home-page: https://github.com/gr0vity-dev/nanomock
+Author: gr0vity
+Description-Content-Type: text/markdown
+
 # nano-local
 
 A one click [nano-currency](https://nano.org) block-lattice environment on your local computer.
 This project aims to easily spin up an integration environment with multiple nano nodes.
 The local network is highly customizable.
 All configuration is done inside the config file : `nanonet/nl_config.toml`
 
@@ -13,15 +21,15 @@
 
 ## Quickstart :
 
 #### Install the library :
 
 To install the library you can
 - clone the respository and run `pip3 install .`
-- or run `pip3 install nanomock`to download teh latest version from PyPi
+- or run `pip3 install nanomock`to download the latest version from PyPi
 
 This gives you access to `nanomock {command}` command which will use `your_current_dir`as its entry point.
 
 #### Spin up a network :
 
 | Action            | Code                                              | Description  
 | :----------       |:---------------------------------------------     | -----
```

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/default_docker-compose.yml` & `nanomock-0.0.2/nanomock/internal/data/services/default_docker-compose.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version: '3'
+version: '2.4'
 
 services:
 
   default_docker:
     image: nanocurrency/nano:V23.3
     user: "1000" #if your user is 1000 we can just run the container as is because because nano_docker_images use user 1000 too.
     container_name: ${default_docker}
```

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/nanolooker/Dockerfile` & `nanomock-0.0.2/nanomock/internal/data/services/nanolooker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/nanolooker/default_docker-compose.yml` & `nanomock-0.0.2/nanomock/internal/data/services/nanolooker/default_docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version : '3'
+version: '2.4'
 
 #when enable_nanolooker = true, this will be copied into the docker-compose file in nano_nodes
 services:
   nl_nanolooker_mongo:
     image: mongo:latest
     container_name: nanolooker_mongo
     restart: unless-stopped
```

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/nanomonitor/default_config.php` & `nanomock-0.0.2/nanomock/internal/data/services/nanomonitor/default_config.php`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/nanoticker/Dockerfile` & `nanomock-0.0.2/nanomock/internal/data/services/nanoticker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/nanovotevisu/Dockerfile` & `nanomock-0.0.2/nanomock/internal/data/services/nanovotevisu/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/promexporter/default_docker-compose.yml` & `nanomock-0.0.2/nanomock/internal/data/services/promexporter/default_docker-compose.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version: '3.8'
+version: '2.4'
 
 # networks:
 #   nl_prom_monitoring:
 #     driver: bridge
 #     name: nl_prom_monitoring
 
 services:
```

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json` & `nanomock-0.0.2/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml` & `nanomock-0.0.2/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/promexporter/prometheus.yml` & `nanomock-0.0.2/nanomock/internal/data/services/promexporter/prometheus.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json` & `nanomock-0.0.2/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/dependency_checker.py` & `nanomock-0.0.2/nanomock/internal/dependency_checker.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/nl_block_tools.py` & `nanomock-0.0.2/nanomock/internal/nl_block_tools.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/internal/nl_initialise.py` & `nanomock-0.0.2/nanomock/internal/nl_initialise.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from nanomock.modules.nl_rpc import NanoRpc
 from nanomock.modules.nl_nanolib import raw_high_precision_percent
 from nanomock.modules.nl_parse_config import ConfigParser
-import logging
+from nanomock.internal.utils import NanoLocalLogger
 
 
 class InitialBlocks:
 
-    def __init__(self, data_dir, rpc_url, logger=None):
+    def __init__(self, data_dir, rpc_url, logger: NanoLocalLogger = None):
         if logger is None:
-            logger = logging.getLogger(__name__)
-
+            logger = NanoLocalLogger.get_logger(__name__)
         self.logger = logger
         self.api = NanoRpc(rpc_url)
         self.config = ConfigParser(data_dir)
 
     def __epoch_link(self, epoch: int):
         message = f"epoch v{epoch} block"
         as_hex = bytearray(message, "ascii").hex()
@@ -26,68 +25,77 @@
         while e <= self.config.get_all()["epoch_count"]:
             link = self.__epoch_link(e)
             epoch_block = self.api.create_epoch_block(
                 link,
                 self.config.get_genesis_account_data()["private"],
                 self.config.get_genesis_account_data()["account"],
             )
-            self.logger.info("EPOCH {} sent by genesis : HASH {}".format(
-                e, epoch_block["hash"]))
+            self.logger.append_log(
+                "InitialBlocks", "INFO",
+                "EPOCH {} sent by genesis : HASH {}".format(
+                    e, epoch_block["hash"]))
             self.__log_active_difficulty()
             e += 1
         pass
 
     def __log_active_difficulty(self):
         diff = self.api.get_active_difficulty()
-        self.logger.info(
+        self.logger.append_log(
+            "InitialBlocks", "INFO",
             f'current_diff : [{diff["network_current"]}]  current_receive_diff: [{diff["network_receive_current"]}]'
         )
 
     def __publish_canary(self):
         fv_canary_send_block = self.api.create_send_block_pkey(
             self.config.get_genesis_account_data()["private"],
             self.config.get_canary_account_data()["account"], 1)
-        self.logger.info(
+        self.logger.append_log(
+            "InitialBlocks", "INFO",
             "SEND FINAL VOTES CANARY BLOCK FROM {} To {} : HASH {}".format(
                 self.config.get_genesis_account_data()["account"],
                 self.config.get_canary_account_data()["account"],
                 fv_canary_send_block["hash"]))
 
         fv_canary_open_block = self.api.create_open_block(
             self.config.get_canary_account_data()["account"],
             self.config.get_canary_account_data()["private"], 1,
             self.config.get_genesis_account_data()["account"],
             fv_canary_send_block["hash"])
-        self.logger.info("OPENED CANARY ACCOUNT {} : HASH {}".format(
-            self.config.get_canary_account_data()["account"],
-            fv_canary_open_block["hash"]))
+        self.logger.append_log(
+            "InitialBlocks", "INFO",
+            "OPENED CANARY ACCOUNT {} : HASH {}".format(
+                self.config.get_canary_account_data()["account"],
+                fv_canary_open_block["hash"]))
 
     def __send_to_burn(self):
         if "burn_amount" not in self.config.get_all():
             self.logger.debug("[burn_amount] is not set. exit send_to_burn()")
             return False
 
         genesis_balance = int(
             self.api.check_balance(self.config.get_genesis_account_data()
                                    ["account"])["balance_raw"])
         if int(self.config.get_all()["burn_amount"]) > genesis_balance:
-            self.logger.warning(
+            self.logger.append_log(
+                "InitialBlocks", "WARNING",
                 "[burn_amount] exceeds genesis balance. exit send_to_burn()")
             return False
 
         send_block = self.api.create_send_block_pkey(
             self.config.get_genesis_account_data()["private"],
             self.config.get_burn_account_data()["account"],
             self.config.get_all()["burn_amount"])
 
-        self.logger.info("SENT {:>40} FROM {} To {} : HASH {}".format(
-            send_block["amount_raw"],
-            self.config.get_genesis_account_data()["account"],
-            self.config.get_burn_account_data()["account"],
-            send_block["hash"]))
+        self.logger.append_log(
+            "InitialBlocks", "INFO",
+            "SENT {:>40} FROM {} To {} : HASH {}".format(
+                send_block["amount_raw"],
+                self.config.get_genesis_account_data()["account"],
+                self.config.get_burn_account_data()["account"],
+                send_block["hash"]))
 
     def __convert_weight_percentage_to_balance(self):
         genesis_balance = int(
             self.api.check_balance(
                 self.config.get_genesis_account_data()["account"],
                 include_only_confirmed=False)["balance_raw"])
         genesis_remaing = genesis_balance
@@ -98,21 +106,23 @@
                 continue  #skip genesis that was added as node
             if "vote_weight_percent" in node_conf:
                 node_conf["balance"] = raw_high_precision_percent(
                     genesis_balance, node_conf["vote_weight_percent"])
             node_conf["balance"] = int(node_conf["balance"])
 
             if genesis_remaing <= 0:
-                self.logger.warning(
+                self.logger.append_log(
+                    "InitialBlocks", "WARNING",
                     f'No Genesis funds remaining! Account [{node_conf["account_data"]["account"]}] will not be opened!'
                 )
                 #self.config["node_account_data"].remove(node_account_data)
                 continue
             if genesis_remaing < node_conf["balance"]:
-                self.logger.warning(
+                self.logger.append_log(
+                    "InitialBlocks", "WARNING",
                     f'Genesis remaining balance is too small! Send {genesis_remaing} instead of {node_conf["balance"]}.'
                 )
 
             self.config.set_node_balance(
                 node_conf["name"], min(node_conf["balance"], genesis_remaing))
             genesis_remaing = max(0, genesis_remaing - node_conf["balance"])
 
@@ -125,42 +135,48 @@
                 continue  #skip genesis that was added as node
             node_account_data = node_conf["account_data"]
 
             send_block = self.api.create_send_block_pkey(
                 self.config.get_genesis_account_data()["private"],
                 node_account_data["account"], node_conf["balance"])
 
-            self.logger.info("SENT {:>40} FROM {} To {} : HASH {}".format(
-                send_block["amount_raw"],
-                self.config.get_genesis_account_data()["account"],
-                node_account_data["account"], send_block["hash"]))
+            self.logger.append_log(
+                "InitialBlocks", "INFO",
+                "SENT {:>40} FROM {} To {} : HASH {}".format(
+                    send_block["amount_raw"],
+                    self.config.get_genesis_account_data()["account"],
+                    node_account_data["account"], send_block["hash"]))
 
             open_block = self.api.create_open_block(
                 node_account_data["account"], node_account_data["private"],
                 node_conf["balance"], node_account_data["account"],
                 send_block["hash"])
 
-            self.logger.info("OPENED PR ACCOUNT {} : HASH {}".format(
-                node_account_data["account"], open_block["hash"]))
+            self.logger.append_log(
+                "InitialBlocks", "INFO",
+                "OPENED PR ACCOUNT {} : HASH {}".format(
+                    node_account_data["account"], open_block["hash"]))
 
     def create_node_wallet(self,
                            rpc_url,
                            node_name,
                            private_key=None,
                            seed=None):
         api = NanoRpc(rpc_url)
 
         if private_key != None:
             wallet = api.wallet_create(None)["wallet"]
             account = api.wallet_add(wallet, private_key)["account"]
         if seed != None:
             wallet = api.wallet_create(seed)["wallet"]
             account = api.get_account_data(seed, 0)["account"]
-        self.logger.info(
+        self.logger.append_log(
+            "InitialBlocks", "INFO",
             f"WALLET {wallet} CREATED FOR {node_name} WITH ACCOUNT {account}")
 
     def publish_initial_blocks(self):
         self.__publish_epochs()
         self.__publish_canary()
         self.__send_to_burn()
         self.__convert_weight_percentage_to_balance()
         self.__send_vote_weigh()
+        return self.logger.pop("InitialBlocks")
```

### Comparing `nanomock-0.0.1/nanomock/internal/utils.py` & `nanomock-0.0.2/nanomock/internal/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,37 +5,52 @@
 from importlib.metadata import version, PackageNotFoundError
 from importlib import resources
 from pathlib import Path
 from typing import Tuple
 import tomli
 import oyaml as yaml
 import json
+import bitmath
 
 
 class NanoLocalLogger(logging.Logger):
 
     SUCCESS_LEVEL_NUM = 25
     logging.addLevelName(SUCCESS_LEVEL_NUM, "SUCCESS")
 
     def success(self, message, *args, **kws):
         self.log(self.SUCCESS_LEVEL_NUM, message, *args, **kws)
 
     @staticmethod
-    def get_logger(name: str):
+    def get_logger(name: str, handler=None):
         logger = NanoLocalLogger(name)
         logger.setLevel(logging.INFO)
-        handler = logging.StreamHandler()
-        handler.setFormatter(logging.Formatter('%(levelname)s: %(message)s'))
+
+        if handler is None:
+            handler = logging.StreamHandler()
+            handler.setFormatter(
+                logging.Formatter('%(levelname)s: %(message)s'))
+
         logger.addHandler(handler)
         return logger
 
+    LOG_STORE = {}
+
     def dynamic(self, log_level, message):
         log_level = getattr(logger, log_level, logging.INFO)
         logger.log(log_level, message)
 
+    def append_log(self, log_key, log_level, message):
+        self.LOG_STORE.setdefault(log_key, [])
+        self.LOG_STORE[log_key].append(message)
+        self.dynamic(log_level, message)
+
+    def pop(self, log_key):
+        return self.LOG_STORE.pop(log_key)
+
 
 logger = NanoLocalLogger.get_logger(__name__)
 
 
 def log_on_success(func: Callable) -> Callable:
 
     @functools.wraps(func)
@@ -113,8 +128,27 @@
             else:
                 # For read_file, the data is already in the correct format (list of lines)
                 return data.splitlines()
         else:
             # If not a packaged version, call the original read_method
             return read_method(self, path, *args, is_packaged=False, **kwargs)
 
-    return wrapper
+    return wrapper
+
+
+def find_device_for_path(path: str) -> str:
+    path = Path(path).resolve()
+    df_output = subprocess.check_output(['df', path],
+                                        universal_newlines=True).splitlines()
+
+    # The first line is the header, and the second line contains the information we need
+    device = df_output[1].split()[0]
+
+    return device
+
+
+def convert_to_bytes(size_string) -> int:
+    if str(size_string).isnumeric():
+        return int(size_string)
+
+    size = bitmath.parse_string(size_string)
+    return int(size.to_Byte())
```

### Comparing `nanomock-0.0.1/nanomock/main.py` & `nanomock-0.0.2/nanomock/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     if is_packaged_version():
         return Path.cwd()
     else:
         return Path.cwd() / 'nanomock'
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Docker Manager CLI')
+    parser = argparse.ArgumentParser(description='nanomock cli')
     parser.add_argument('command',
                         choices=[
                             'create', 'start', 'status', 'restart', 'init',
                             'stop', 'update', 'remove', 'reset', 'down',
                             'destroy', 'rpc'
                         ])
     parser.add_argument('--dir_path',
@@ -39,18 +39,12 @@
         '--payload',
         type=json.loads,
         help="JSON request payload (only required for rpc command)")
 
     args = parser.parse_args()
     manager = NanoLocalManager(args.dir_path, args.project_name)
 
-    if args.command == 'rpc':
-        if not args.payload:
-            parser.error(
-                "The --payload argument is required for the 'rpc' command.")
-        manager.execute_command(args.command, args.nodes, args.payload)
-    else:
-        manager.execute_command(args.command, args.nodes)
+    manager.execute_command(args.command, args.nodes, args.payload)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `nanomock-0.0.1/nanomock/modules/nl_nanolib.py` & `nanomock-0.0.2/nanomock/modules/nl_nanolib.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/modules/nl_parse_config.py` & `nanomock-0.0.2/nanomock/modules/nl_parse_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from nanolib import Block
 from extradict import NestedData
 from pathlib import Path
 from importlib import resources
 
 from nanomock.modules.nl_nanolib import NanoLibTools, raw_high_precision_multiply
 from nanomock.modules.nl_rpc import NanoRpc
-from nanomock.internal.utils import read_from_package_if_needed, is_packaged_version
+from nanomock.internal.utils import read_from_package_if_needed, is_packaged_version, find_device_for_path, convert_to_bytes
 
 
 def str2bool(v):
     return str(v).lower() in ("yes", "true", "t", "1")
 
 
 class ConfigReadWrite:
@@ -83,33 +83,35 @@
                       default_flow_style=False)
 
 
 class ConfigParser:
 
     preconfigured_peers = []
 
-    def __init__(self, app_dir):
+    def __init__(self, app_dir, config_file=None):
         self.enabled_services = []
-        self._set_path_variables(app_dir)
+        self._set_path_variables(app_dir, config_file)
         self.conf_rw = ConfigReadWrite(self.nl_config_path)
         self.nano_lib = NanoLibTools()
         self.config_dict = self.conf_rw.read_toml(self.nl_config_path)
         self.compose_dict = self.conf_rw.read_yaml(self.default_compose_path,
                                                    is_packaged=True)
         self.__config_dict_add_genesis_to_nodes()
         self.__config_dict_set_node_variables()  #modifies config_dict
         self.__config_dict_set_default_values()  #modifies config_dict
         self.__set_preconfigured_peers()
         self.__set_node_accounts()
         self.__set_balance_from_vote_weight()
         self.__set_special_account_data()
         #self.__set_docker_compose()
 
-    def _set_path_variables(self, app_dir):
+    def _set_path_variables(self, app_dir, config_file):
         user_app_dir = Path(app_dir).resolve()
+        if config_file is None:
+            config_file = "nl_config.toml"
 
         if is_packaged_version():
             self.services_dir = "nanomock.internal.data.services"
             self.default_compose_path = f"{self.services_dir}.default_docker-compose.yml"
             self.default_nanomonitor_config = f"{self.services_dir}.nanomonitor.default_config.php"
             self.default_nanomonitor_config = f"{self.services_dir}.nanovotevisu.default_docker-compose.yml"
         else:
@@ -120,15 +122,15 @@
                 self.services_dir) / "default_docker-compose.yml"
             self.default_nanomonitor_config = Path(
                 self.services_dir) / "nanomonitor" / "default_config.php"
             self.default_nanovotevisu_config = Path(
                 self.services_dir
             ) / "nanovotevisu" / "default_docker-compose.yml"
 
-        self.nl_config_path = user_app_dir / "nl_config.toml"
+        self.nl_config_path = user_app_dir / config_file
         self.nano_nodes_path = user_app_dir / "nano_nodes"
         self.nodes_dir = self.nano_nodes_path / "{node_name}"
         self.compose_out_path = self.nano_nodes_path / "docker-compose.yml"
         self.tcp_analyzer_path = Path("tcp_analyzer")
 
     def __set_node_accounts(self):
         available_supply = 340282366920938463463374607431768211455 - int(
@@ -839,69 +841,137 @@
         if key not in self.config_dict:
             return None
         return self.config_dict[key]
 
     def write_docker_compose(self):
         self.conf_rw.write_yaml(self.compose_out_path, self.compose_dict)
 
-    def get_docker_tag(self, node_name):
-        #takes the first non empty docker_tag.
+    def get_config_tag(self, tag, node_name, default):
+        #takes the first non empty tag.
         #First looks for the individual tag
         #then for the general tag
-        #last uses teh default nanocurrency/nano-beta:latest tag
-
-        individual_tag = self.get_representative_config(
-            "docker_tag", node_name)
-        general_tag = self.get_representative_config("docker_tag", None)
+        #last uses the default
+        individual_tag = self.get_representative_config(tag, node_name)
+        general_tag = self.get_representative_config(tag, None)
 
         if individual_tag["found"]:
             return individual_tag["value"]
         elif general_tag["found"]:
             return general_tag["value"]
         else:
-            return "nanocurrency/nano-beta:latest"
+            return default
 
-    def compose_add_node(self, node_name):
-        #Search for individual docker_tag, then individual executable, then shared docker-tag then shared-executable
+    def get_docker_tag(self, node_name):
+        self.get_config_tag(self, "docker_tag", node_name,
+                            "nanocurrency/nano-beta:latest")
 
-        user_id = str(os.getuid())
-        docker_tag = self.get_docker_tag(node_name)
+    def get_disk_defaults(self, disk_type):
+        disk_defaults = {
+            "NVME": {
+                "device_read_bps": "2000MB",
+                "device_write_bps": "1000MB",
+                "device_read_iops": "200000",
+                "device_write_iops": "200000",
+            },
+            "SSD": {
+                "device_read_bps": "400MB",
+                "device_write_bps": "300MB",
+                "device_read_iops": "50000",
+                "device_write_iops": "40000",
+            },
+            "HDD": {
+                "device_read_bps": "50MB",
+                "device_write_bps": "50MB",
+                "device_read_iops": "100",
+                "device_write_iops": "100",
+            },
+        }
+        return disk_defaults.get(disk_type.upper(), None)
 
-        if self.config_dict[
-                "tc_enable"]:  #installs iproute2 into the nano_node image
-            container = self.compose_add_container(node_name,
-                                                   "default_docker_custom")
-            container["user"] = user_id
-            container["build"]["args"][0] = f'NANO_IMAGE={docker_tag}'
-            container["build"]["args"][1] = f'UID={user_id}'
-            container["build"]["args"][
-                2] = f'TC_ENABLE={str(self.config_dict["tc_enable"]).upper()}'
-
-        elif user_id == "0":  #root
-            container = self.compose_add_container(node_name,
-                                                   "default_docker_root")
-            container["image"] = f"{docker_tag}"
+    def add_container_blkio_config(self, container, node_name):
+        blkio_config = {}
+        config_tags = [
+            "device_read_bps",
+            "device_write_bps",
+            "device_read_iops",
+            "device_write_iops",
+        ]
 
+        disk_type = self.get_config_tag("disk", node_name, None)
+        if disk_type:
+            disk_defaults = self.get_disk_defaults(disk_type)
+            if disk_defaults:
+                for tag in config_tags:
+                    rate = convert_to_bytes(disk_defaults[tag])
+                    blkio_config[tag] = [{
+                        "path":
+                        find_device_for_path(self.nl_config_path),
+                        "rate":
+                        rate
+                    }]
+        else:
+            for tag in config_tags:
+                rate = self.get_config_tag(tag, node_name, None)
+                if rate is not None:
+                    blkio_config[tag] = [{
+                        "path":
+                        find_device_for_path(self.nl_config_path),
+                        "rate":
+                        convert_to_bytes(rate)
+                    }]
+
+        if blkio_config:
+            container["blkio_config"] = blkio_config
+
+    def add_container_cpu_memory_config(self, container, node_name):
+        cpu = self.get_config_tag("cpu", node_name, None)
+        if cpu is not None:
+            container["cpus"] = float(cpu)
+
+        memory = self.get_config_tag("memory", node_name, None)
+        if memory is not None:
+            container["mem_limit"] = convert_to_bytes(memory)
+
+    def get_container_type(self, user_id):
+        if user_id == "0":
+            return "default_docker_root"
         elif user_id == "1000":
-            container = self.compose_add_container(node_name, "default_docker")
+            return "default_docker"
+        else:
+            return "default_docker_custom"
+
+    def set_container_image_or_build_args(self, container, user_id,
+                                          docker_tag):
+        if user_id in ["0", "1000"]:
             container["image"] = f"{docker_tag}"
+        else:
+            container["build"]["args"] = [
+                f'NANO_IMAGE={docker_tag}',
+                f'UID={user_id}',
+            ]
 
-            logging.warning(
-                "No docker_tag or nano_node_path specified. use [latest] (nanocurrency/nano-test:latest)"
-            )
+    def compose_add_node(self, node_name):
+        user_id = str(os.getuid())
+        docker_tag = self.get_config_tag("docker_tag", node_name,
+                                         "nanocurrency/nano-beta:latest")
 
-        else:  #non standart user
-            #we need to add the current user as user to the nano_node docker image
+        container_type = self.get_container_type(user_id)
+        container = self.compose_add_container(node_name, container_type)
 
-            container = self.compose_add_container(node_name,
-                                                   "default_docker_custom")
+        if user_id != "1000" or self.config_dict["tc_enable"]:
             container["user"] = user_id
-            #container["image"] = f"{docker_tag}"
-            container["build"]["args"][0] = f'NANO_IMAGE={docker_tag}'
-            container["build"]["args"][1] = f'UID={user_id}'
+
+        if self.config_dict["tc_enable"]:
+            container["build"]["args"].append(
+                f'TC_ENABLE={str(self.config_dict["tc_enable"]).upper()}')
+
+        self.set_container_image_or_build_args(container, user_id, docker_tag)
+        if container:
+            self.add_container_blkio_config(container, node_name)
+            self.add_container_cpu_memory_config(container, node_name)
 
     def compose_set_node_ports(self, node_name):
         node_config = self.get_node_config(node_name)
         self.compose_dict["services"][node_name]["ports"] = [
             f'{node_config["host_port_peer"]}:17075',
             f'{node_config["host_port_rpc"]}:17076',
             f'{node_config["host_port_ws"]}:17078'
```

### Comparing `nanomock-0.0.1/nanomock/modules/nl_rpc.py` & `nanomock-0.0.2/nanomock/modules/nl_rpc.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/nanomock/nanomock_manager.py` & `nanomock-0.0.2/nanomock/nanomock_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,55 +38,60 @@
         self.data_path = f"{self.nano_nodes_path}/{{node_name}}/NanoTest"
         self.config_node_path = f"{self.nano_nodes_path}/{{node_name}}/NanoTest/config-node.toml"
         self.config_rpc_path = f"{self.nano_nodes_path}/{{node_name}}/NanoTest/config-rpc.toml"
 
         os.makedirs(self.nano_nodes_path, exist_ok=True)
 
     def _initialize_command_mapping(self):
+        #(command_method , validation_method)
         return {
-            'create': self.create_docker_compose_file,
-            'start': self.start_containers,
-            'status': self.network_status,
-            'restart': self.restart_containers,
-            'reset': self.reset_nodes_data,
-            'init': self.init_nodes,
-            'stop': self.stop_containers,
-            'remove': self.remove_containers,
-            'down': self.remove_containers,
-            'destroy': lambda: self.destroy(remove_files=True),
-            'rpc': self.run_rpc
+            'create': (self.create_docker_compose_file, None),
+            'start': (self.start_containers, None),
+            'status': (self.network_status, None),
+            'restart': (self.restart_containers, None),
+            'reset': (self.reset_nodes_data, None),
+            'init': (self.init_nodes, None),
+            'stop': (self.stop_containers, None),
+            'remove': (self.remove_containers, None),
+            'down': (self.remove_containers, None),
+            'destroy': (lambda: self.destroy(remove_files=True), None),
+            'rpc': (self.run_rpc, self._rpc_validator)
         }
 
-    def subprocess_capture_raise(self, cmd, shell=True, cwd=None, increment=0):
+    def _subprocess_capture_raise(self,
+                                  cmd,
+                                  shell=True,
+                                  cwd=None,
+                                  increment=0):
         #Capture output to stdout or raise CalledProcessError if the command returns a non-zero exit code
         try:
             result = subprocess.run(cmd,
                                     shell=shell,
                                     check=True,
                                     capture_output=True,
                                     text=True,
                                     cwd=cwd)
 
             #print(str.join(" ", [str(e) for e in cmd]))
             return result
         except subprocess.CalledProcessError as e:
-            response = self.auto_heal(e, cmd, shell, cwd, increment)
+            response = self.auto_heal(e, shell, cwd, increment)
             return response
 
     def _run_docker_compose_command(self,
                                     command,
                                     nodes: Optional[List[str]] = None):
         base_command = [
             "docker-compose", "-f", self.compose_yml_path, "-p",
             self.project_name
         ]
         base_command.extend(command)
         if nodes: base_command.extend(nodes)
 
-        return self.subprocess_capture_raise(base_command, shell=False)
+        return self._subprocess_capture_raise(base_command, shell=False)
 
     def _get_default(self, config_name):
         """ Load config with default values"""
         #minimal node config if no file is provided in the nl_config.toml
         if config_name == "config_node":
             default_config_path = os.path.join(self.services_dir,
                                                "default_config-node.toml")
@@ -161,15 +166,15 @@
         self._generate_config_rpc_file(node_name)
         self._generate_nanomonitor_config_file(node_name)
 
     def _online_containers(self, node_names: List[str]) -> List[str]:
         online_containers = []
         for container in node_names:
             cmd = f"docker ps |grep {container}$ | wc -l"
-            res = self.subprocess_capture_raise(cmd)
+            res = self._subprocess_capture_raise(cmd)
             online = int(res.stdout.strip())
 
             if online == 1:
                 online_containers.append(container)
 
         return online_containers
 
@@ -318,14 +323,20 @@
     def create_docker_compose_file(self):
         self._prepare_nodes()
         self._generate_docker_compose_env_file()
         self._generate_docker_compose_yml_file()
         logger.success(
             f"Docker Compose file created at {self.compose_yml_path}")
 
+    def _rpc_validator(self, nodes=None, payload=None):
+        if not payload:
+            raise ValueError(
+                "The --payload argument is required for the 'rpc' command.")
+        return nodes, payload
+
     @log_on_success
     def run_rpc(self, payload=None, nodes=None):
         responses = []
         if nodes is None:
             nodes = self.conf_p.get_nodes_name()
 
         for node in nodes:
@@ -356,24 +367,24 @@
 
     @log_on_success
     def init_nodes(self):
         self.init_wallets()
         init_blocks = InitialBlocks(self.dir_path,
                                     self.conf_p.get_nodes_rpc()[0],
                                     logger=logger)
-        init_blocks.publish_initial_blocks()
+        return init_blocks.publish_initial_blocks()
 
     @log_on_success
     def reset_nodes_data(self, nodes: Optional[List[str]] = None):
         self.stop_containers(nodes)
         nodes_to_process = nodes or ['.']
         for node in nodes_to_process:
             node_path = f'{self.nano_nodes_path}/{node}' if nodes else self.nano_nodes_path
             cmd = 'rm -f $(find . -name "*.ldb")'
-            self.subprocess_capture_raise(cmd, node_path)
+            self._subprocess_capture_raise(cmd, node_path)
 
     def init_containers(self):
         self.create_docker_compose_file()
         self.build_containers()
 
     @log_on_success
     def restart_containers(self, nodes: Optional[List[str]] = None):
@@ -411,15 +422,14 @@
         self._run_docker_compose_command(["pull"])
         # Remove containers and networks
         self.remove_containers()
         self.build_containers()
 
     def auto_heal(self,
                   error: subprocess.CalledProcessError,
-                  cmd,
                   cmd_shell,
                   cmd_cwd,
                   increment=0):
         if increment >= 10:
             raise (error)
 
         stderr = error.stderr
@@ -436,93 +446,65 @@
                 continue
 
             logger.warning(
                 f"Retry attempt {increment}... {error_key}: \n {stderr}")
 
             if heal_func(error_msg, stderr):
                 increment += 1
-                return self.subprocess_capture_raise(cmd,
-                                                     cmd_shell,
-                                                     cmd_cwd,
-                                                     increment=increment)
+                return self._subprocess_capture_raise(error.cmd,
+                                                      cmd_shell,
+                                                      cmd_cwd,
+                                                      increment=increment)
 
+        raise ValueError(error.stderr)
         raise (error)
 
     def _heal_address_in_use(self, error_msg, stderr):
         container_name = re.search(r"{} (\w+)".format(error_msg),
                                    stderr).group(1)
-        self.subprocess_capture_raise(
-            f"docker stop {container_name} && sleep 5 && docker start {container_name}",
+        self._subprocess_capture_raise(
+            f"docker stop -t 0 {container_name} && sleep 5 && docker start {container_name}",
             shell=True)
         return True
 
     def _heal_docker_in_use(self, error_msg, stderr):
         pattern = r'{} "/([^"]+)"'.format(error_msg)
         match = re.search(pattern, stderr)
         if match:
             container_name = match.group(1)
-            self.subprocess_capture_raise(
-                f"docker stop {container_name} && docker rm {container_name} && sleep 5",
+            self._subprocess_capture_raise(
+                f"docker stop -t 0 {container_name} && docker rm {container_name} && sleep 5",
                 shell=True)
             return True
         return False
 
-    # def auto_heal(self,
-    #               error: subprocess.CalledProcessError,
-    #               cmd,
-    #               increment=0):
-    #     if increment >= 3: raise (error)
-
-    #     stderr = error.stderr
-    #     healable_errors = {
-    #         "address_in_use":
-    #         "programming external connectivity on endpoint",
-    #         "docker_in_use":
-    #         "Error response from daemon: Conflict. The container name"
-    #     }
-
-    #     for error_key, error_msg in healable_errors.items():
-    #         if error_msg not in stderr: continue
-    #         logger.warn(
-    #             f"Retry attempt {increment}... {error_key}: \n {stderr}")
-
-    #         retry = False
-
-    #         if error_key == "address_in_use":
-    #             container_name = re.search(r"{} (\w+)".format(error_msg),
-    #                                        stderr).group(1)
-    #             self.subprocess_capture_raise(
-    #                 f"docker stop {container_name} && sleep 5 && docker start {container_name}",
-    #                 shell=True)
-    #             retry = True
-
-    #         if error_key == "docker_in_use":
-    #             pattern = r'{} "/([^"]+)"'.format(error_msg)
-    #             match = re.search(pattern, stderr)
-    #             if match:
-    #                 container_name = match.group(1)
-    #                 self.subprocess_capture_raise(
-    #                     f"docker stop {container_name} && docker rm {container_name} && sleep 5",
-    #                     shell=True)
-    #                 retry = True
-
-    #         if retry:
-    #             increment = increment + 1
-    #             return self.subprocess_capture_raise(cmd, increment=increment)
-
-    #     raise (error)
+    def _filter_args(self, func, **kwargs):
+        sig = inspect.signature(func)
+        filtered_args = {
+            k: v
+            for k, v in kwargs.items() if k in sig.parameters
+        }
+        return filtered_args
 
     def execute_command(self, command, nodes=None, payload=None):
         if command not in self.command_mapping:
             raise ValueError(f"Invalid command: {command}")
 
-        func = self.command_mapping[command]
-        if command == 'rpc':
-            func(payload=payload, nodes=nodes)
-        elif nodes:
-            func(nodes=nodes)
+        command_func, validator_func = self.command_mapping[command]
+
+        if validator_func is not None:
+            filtered_validator_args = self._filter_args(validator_func,
+                                                        nodes=nodes,
+                                                        payload=payload)
+            validated_nodes, validated_payload = validator_func(
+                **filtered_validator_args)
         else:
-            func()
+            validated_nodes, validated_payload = nodes, payload
+
+        filtered_command_args = self._filter_args(command_func,
+                                                  nodes=validated_nodes,
+                                                  payload=validated_payload)
+        command_func(**filtered_command_args)
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `nanomock-0.0.1/nanomock.egg-info/PKG-INFO` & `nanomock-0.0.2/nanomock.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomock
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create local dockerized nano-currency networks
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 # nano-local
 
@@ -21,15 +21,15 @@
 
 ## Quickstart :
 
 #### Install the library :
 
 To install the library you can
 - clone the respository and run `pip3 install .`
-- or run `pip3 install nanomock`to download teh latest version from PyPi
+- or run `pip3 install nanomock`to download the latest version from PyPi
 
 This gives you access to `nanomock {command}` command which will use `your_current_dir`as its entry point.
 
 #### Spin up a network :
 
 | Action            | Code                                              | Description  
 | :----------       |:---------------------------------------------     | -----
```

### Comparing `nanomock-0.0.1/nanomock.egg-info/SOURCES.txt` & `nanomock-0.0.2/nanomock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.1/setup.py` & `nanomock-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="nanomock",
-      version="0.0.1",
+      version="0.0.2",
       author="gr0vity",
       description="Create local dockerized nano-currency networks",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/gr0vity-dev/nanomock",
       packages=find_packages(exclude=["unit_tests"]),
       include_package_data=True,
```

