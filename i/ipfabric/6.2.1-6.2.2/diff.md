# Comparing `tmp/ipfabric-6.2.1.tar.gz` & `tmp/ipfabric-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.2.1.tar", max compression
+gzip compressed data, was "ipfabric-6.2.2.tar", max compression
```

## Comparing `ipfabric-6.2.1.tar` & `ipfabric-6.2.2.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0     1790 2023-03-16 16:58:08.617128 ipfabric-6.2.1/ipfabric/__init__.py
--rw-r--r--   0        0        0    17096 2023-04-10 11:49:56.699072 ipfabric-6.2.1/ipfabric/api.py
--rw-r--r--   0        0        0     9229 2023-04-10 11:49:19.028096 ipfabric-6.2.1/ipfabric/client.py
--rw-r--r--   0        0        0      322 2023-02-08 21:33:38.498830 ipfabric-6.2.1/ipfabric/models/__init__.py
--rw-r--r--   0        0        0     6054 2023-03-14 15:20:54.722357 ipfabric-6.2.1/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2786 2023-03-14 15:45:17.816340 ipfabric-6.2.1/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0     2110 2023-02-09 13:14:16.640525 ipfabric-6.2.1/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     5669 2023-02-09 13:14:16.640525 ipfabric-6.2.1/ipfabric/models/jobs.py
--rw-r--r--   0        0        0    12119 2023-04-05 17:31:47.761633 ipfabric-6.2.1/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0    15036 2023-04-24 13:56:20.167261 ipfabric-6.2.1/ipfabric/models/table.py
--rw-r--r--   0        0        0     2830 2023-02-09 13:14:16.655535 ipfabric-6.2.1/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1156 2023-02-25 14:47:47.471307 ipfabric-6.2.1/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      488 2023-02-08 13:05:11.993384 ipfabric-6.2.1/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2173 2023-02-08 13:05:11.998383 ipfabric-6.2.1/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1002 2023-02-08 13:05:12.003471 ipfabric-6.2.1/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     7018 2023-02-25 14:47:47.471307 ipfabric-6.2.1/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      324 2023-02-08 13:05:12.011503 ipfabric-6.2.1/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0      843 2023-02-08 13:05:12.016497 ipfabric-6.2.1/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      470 2023-02-08 13:05:12.021499 ipfabric-6.2.1/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     5644 2023-02-08 13:05:12.027499 ipfabric-6.2.1/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2045 2023-02-25 14:47:47.482435 ipfabric-6.2.1/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     2783 2023-02-25 14:47:47.482435 ipfabric-6.2.1/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0      759 2023-02-08 13:05:12.031562 ipfabric-6.2.1/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      633 2023-02-08 13:05:12.031562 ipfabric-6.2.1/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     3529 2023-02-25 14:51:16.763228 ipfabric-6.2.1/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1231 2023-02-08 13:05:12.050282 ipfabric-6.2.1/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1078 2023-02-08 13:05:12.065065 ipfabric-6.2.1/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     4773 2023-02-25 14:51:16.794519 ipfabric-6.2.1/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2159 2023-02-08 13:05:12.078066 ipfabric-6.2.1/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      431 2023-02-08 13:05:12.083210 ipfabric-6.2.1/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2062 2023-02-08 13:05:12.088455 ipfabric-6.2.1/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2228 2023-02-08 13:05:12.092469 ipfabric-6.2.1/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0      856 2023-02-08 13:05:12.097528 ipfabric-6.2.1/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0      867 2023-02-08 13:05:12.097528 ipfabric-6.2.1/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.2.1/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3602 2023-02-09 20:02:01.172909 ipfabric-6.2.1/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     6187 2023-02-08 13:05:11.963806 ipfabric-6.2.1/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.2.1/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.2.1/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.2.1/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     1413 2023-01-31 20:32:11.592169 ipfabric-6.2.1/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     5247 2023-04-05 17:31:47.706534 ipfabric-6.2.1/ipfabric/settings/user_mgmt.py
--rw-r--r--   0        0        0     1875 2023-02-08 14:40:46.626939 ipfabric-6.2.1/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     6439 2023-02-09 20:02:01.204437 ipfabric-6.2.1/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.2.1/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     7876 2023-03-30 17:03:49.576728 ipfabric-6.2.1/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.2.1/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.1/ipfabric/tools/factory_defaults/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/__init__.py
--rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/dashboard.json
--rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/groups.json
--rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-03 16:42:03.278481 ipfabric-6.2.1/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     5784 2023-01-31 20:32:11.624088 ipfabric-6.2.1/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0     2519 2023-02-09 19:07:57.301096 ipfabric-6.2.1/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2396 2023-02-09 18:58:27.499064 ipfabric-6.2.1/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2573 2023-03-24 18:58:14.154592 ipfabric-6.2.1/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.2.1/LICENSE
--rw-r--r--   0        0        0     2014 2023-04-24 14:07:27.097697 ipfabric-6.2.1/pyproject.toml
--rw-r--r--   0        0        0     3705 2023-04-04 13:32:24.957368 ipfabric-6.2.1/README.md
--rw-r--r--   0        0        0     5234 1970-01-01 00:00:00.000000 ipfabric-6.2.1/setup.py
--rw-r--r--   0        0        0     5132 1970-01-01 00:00:00.000000 ipfabric-6.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1790 2023-05-02 13:05:28.009049 ipfabric-6.2.2/ipfabric/__init__.py
+-rw-r--r--   0        0        0    17332 2023-05-02 14:13:41.507070 ipfabric-6.2.2/ipfabric/api.py
+-rw-r--r--   0        0        0    10845 2023-05-02 15:08:19.059384 ipfabric-6.2.2/ipfabric/client.py
+-rw-r--r--   0        0        0      434 2023-04-28 15:05:01.483490 ipfabric-6.2.2/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0    14759 2023-04-28 15:24:56.152456 ipfabric-6.2.2/ipfabric/models/device.py
+-rw-r--r--   0        0        0     5842 2023-04-28 18:36:35.766072 ipfabric-6.2.2/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2786 2023-04-24 14:44:33.818272 ipfabric-6.2.2/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0     2092 2023-04-28 16:56:02.064091 ipfabric-6.2.2/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     5669 2023-04-24 14:44:33.819272 ipfabric-6.2.2/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0    12327 2023-05-02 12:02:38.016974 ipfabric-6.2.2/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0    19209 2023-04-28 18:36:35.782289 ipfabric-6.2.2/ipfabric/models/table.py
+-rw-r--r--   0        0        0     2830 2023-04-24 14:44:33.820322 ipfabric-6.2.2/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1156 2023-04-24 14:44:33.821325 ipfabric-6.2.2/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      488 2023-04-24 14:44:33.821325 ipfabric-6.2.2/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2173 2023-04-24 14:44:33.821325 ipfabric-6.2.2/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1002 2023-04-24 14:44:33.821325 ipfabric-6.2.2/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     7018 2023-04-24 14:44:33.822322 ipfabric-6.2.2/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      324 2023-04-24 14:44:33.822322 ipfabric-6.2.2/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0      843 2023-04-24 14:44:33.822322 ipfabric-6.2.2/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      470 2023-04-24 14:44:33.823320 ipfabric-6.2.2/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     5644 2023-04-24 14:44:33.823320 ipfabric-6.2.2/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2045 2023-04-24 14:44:33.823320 ipfabric-6.2.2/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     2783 2023-04-24 14:44:33.824322 ipfabric-6.2.2/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0      759 2023-04-24 14:44:33.824322 ipfabric-6.2.2/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      633 2023-04-24 14:44:33.825321 ipfabric-6.2.2/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     3529 2023-04-24 14:44:33.825321 ipfabric-6.2.2/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1231 2023-04-24 14:44:33.826320 ipfabric-6.2.2/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1078 2023-04-24 14:44:33.826320 ipfabric-6.2.2/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     4773 2023-04-24 14:44:33.827321 ipfabric-6.2.2/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2159 2023-04-24 14:44:33.827321 ipfabric-6.2.2/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      431 2023-04-24 14:44:33.827321 ipfabric-6.2.2/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2062 2023-04-24 14:44:33.828325 ipfabric-6.2.2/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2228 2023-04-24 14:44:33.828325 ipfabric-6.2.2/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0      856 2023-04-24 14:44:33.829324 ipfabric-6.2.2/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0      867 2023-04-24 14:44:33.829324 ipfabric-6.2.2/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.2.2/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3602 2023-04-24 14:44:33.835549 ipfabric-6.2.2/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     6187 2023-04-24 14:44:33.840110 ipfabric-6.2.2/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.2.2/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.2.2/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.2.2/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     1413 2023-04-24 14:44:33.844128 ipfabric-6.2.2/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     5247 2023-04-24 14:44:33.849107 ipfabric-6.2.2/ipfabric/settings/user_mgmt.py
+-rw-r--r--   0        0        0     1875 2023-04-24 14:44:33.866077 ipfabric-6.2.2/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     6439 2023-04-24 14:44:33.870769 ipfabric-6.2.2/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.2.2/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     7876 2023-04-24 14:44:33.876769 ipfabric-6.2.2/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.2.2/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.2/ipfabric/tools/factory_defaults/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v4/4/__init__.py
+-rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v4/4/dashboard.json
+-rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v4/4/groups.json
+-rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v4/4/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v4/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v5/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v5/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v5/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v5/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v5/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v6/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v6/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v6/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v6/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.2/ipfabric/tools/factory_defaults/v6/__init__.py
+-rw-r--r--   0        0        0     4511 2023-04-24 14:44:33.881459 ipfabric-6.2.2/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     5784 2023-04-24 14:44:33.886456 ipfabric-6.2.2/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0     2519 2023-04-24 14:44:33.891098 ipfabric-6.2.2/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2396 2023-04-24 14:44:33.895102 ipfabric-6.2.2/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2573 2023-04-24 14:44:33.902766 ipfabric-6.2.2/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.2.2/LICENSE
+-rw-r--r--   0        0        0     2054 2023-05-02 15:53:11.488078 ipfabric-6.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3705 2023-04-24 14:44:33.756295 ipfabric-6.2.2/README.md
+-rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 ipfabric-6.2.2/setup.py
+-rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 ipfabric-6.2.2/PKG-INFO
```

### Comparing `ipfabric-6.2.1/ipfabric/__init__.py` & `ipfabric-6.2.2/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/api.py` & `ipfabric-6.2.2/ipfabric/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,30 +142,35 @@
             self._login(auth, base_url=base_url, cookie_jar=cookie_jar)  # TODO: Keep only this in v7.0
 
         # Get Current User, by doing that we are also ensuring the token is valid
         self.user = self.get_user()
         self.snapshots = self.get_snapshots()
         # self.web_endpoints = self._web_endpoints(base_url)  # TODO When Implemented correctly.
         self._attribute_filters = None
+        self._no_loaded_snapshots = False
         self.snapshot_id = snapshot_id
         logger.debug(
             f"Successfully connected to '{self.base_url.host}' IPF version '{self.os_version}' "
             f"as user '{self.user.username}'"
         )
 
     @property
+    def _api_insuf_rights(self):
+        msg = f'API_INSUFFICIENT_RIGHTS for user "{self.user.username}" '
+        if self.user.token:
+            msg += f'token "{self.user.token.description}" '
+        return msg
+
+    @property
     def hostname(self):
         resp = self.get("/os/hostname")
         if resp.status_code == 200:
             return resp.json()["hostname"]
         elif resp.status_code == 403:
-            msg = f'API_INSUFFICIENT_RIGHTS for user "{self.user.username}" '
-            if self.user.token:
-                msg += f'token "{self.user.token.description}" '
-            logger.critical(msg + 'on GET "/os/hostname".')
+            logger.critical(self._api_insuf_rights + 'on GET "/os/hostname".')
             return None
         else:
             resp.raise_for_status()
 
     def _web_endpoints(self, base_url):
         resp = self.get(urljoin(base_url, "/api/oas/openapi-extended.json"))
         resp.raise_for_status()
@@ -269,14 +274,15 @@
             )
 
         return return_version, resp.json()["releaseVersion"]
 
     def update(self):
         """get all snapshots and assigns them to an attribute"""
         self.snapshots = self.get_snapshots()
+        self._no_loaded_snapshots = self.loaded_snapshots == dict()
 
     @property
     def loaded_snapshots(self) -> dict:
         """get only loaded snapshots"""
         return {k: v for k, v in self.snapshots.items() if v.loaded}
 
     @property
@@ -298,14 +304,15 @@
 
     @snapshot_id.setter
     def snapshot_id(self, snapshot_id):
         snapshot_id = snapshot_id or LAST_ID
         if not self.loaded_snapshots:
             logger.warning("No Snapshots are currently loaded.  Please load a snapshot before querying any data.")
             self._snapshot_id = None
+            self._no_loaded_snapshots = True
         elif snapshot_id not in self.snapshots:
             # Verify snapshot ID is valid
             raise ValueError(f"Incorrect Snapshot ID: '{snapshot_id}'")
         else:
             self._snapshot_id = self.snapshots[snapshot_id].snapshot_id
 
     def get_snapshot(self, snapshot_id: str):
```

### Comparing `ipfabric-6.2.1/ipfabric/client.py` & `ipfabric-6.2.2/ipfabric/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,24 @@
 import logging
 import re
 from json import loads
 from typing import Optional, Union, Dict, List, Any
 from urllib.parse import urlparse
 
+from httpx import HTTPStatusError
+
 from ipfabric.api import IPFabricAPI
 from ipfabric.models import Technology, Inventory, Jobs, Intent
 
 logger = logging.getLogger("ipfabric")
 
 RE_PATH = re.compile(r"^/?(api/)?v\d(\.\d)?/")
 RE_TABLE = re.compile(r"^tables/")
 
 
-def check_format(func):
-    """
-    Checks to make sure api/v1/ is not in the URL and converts filters from json str to dict
-    """
-
-    def wrapper(self, url, *args, **kwargs):
-        if "filters" in kwargs and isinstance(kwargs["filters"], str):
-            kwargs["filters"] = loads(kwargs["filters"])
-        path = urlparse(url or kwargs["url"]).path
-        r = RE_PATH.search(path)
-        url = path[r.end():] if r else path  # fmt: skip
-        url = url[1:] if url[0] == "/" else url
-        return func(self, url, *args, **kwargs)
-
-    return wrapper
-
-
 class IPFClient(IPFabricAPI):
     def __init__(
         self,
         base_url: Optional[str] = None,
         api_version: Optional[str] = None,
         snapshot_id: Optional[str] = None,
         auth: Optional[Any] = None,
@@ -43,29 +28,84 @@
         """Initializes the IP Fabric Client
 
         Args:
             base_url: IP Fabric instance provided in 'base_url' parameter, or the 'IPF_URL' environment variable
             api_version: [Optional] Version of IP Fabric API
             auth: API token, tuple (username, password), or custom Auth to pass to httpx
             snapshot_id: IP Fabric snapshot ID to use by default for database actions - defaults to '$last'
-            unloaded: True to load metadata from unloaded snapshots
             **kwargs: Keyword args to pass to httpx
         """
         super().__init__(
-            base_url=base_url, api_version=api_version, auth=auth, snapshot_id=snapshot_id, unloaded=unloaded, **kwargs
+            base_url=base_url,
+            api_version=api_version,
+            auth=auth,
+            snapshot_id=snapshot_id,
+            unloaded=unloaded,
+            **kwargs,
         )
-        self.inventory = Inventory(client=self)
-        self.intent = Intent(client=self)  # check no snapshot
-        self.api_to_web = {intent.api_endpoint: intent.web_endpoint for intent in self.intent.intent_checks}
         self.technology = Technology(client=self)
         self.jobs = Jobs(client=self)
+        self._devices = list()
+
+    @property
+    def snapshot_id(self):
+        """get snapshot Id"""
+        return self._snapshot_id
+
+    @snapshot_id.setter
+    def snapshot_id(self, snapshot_id):
+        super(self.__class__, self.__class__).snapshot_id.fset(self, snapshot_id)
+        self.intent = Intent(client=self)
+        self.api_to_web = {intent.api_endpoint: intent.web_endpoint for intent in self.intent.intent_checks}
+        self.inventory = Inventory(client=self)
+
+    @property
+    def devices(self):
+        """get devices"""
+        if not self._devices:
+            logger.info("Devices not loaded, loading devices.")
+            self._devices = self.load_devices()
+        return self._devices
+
+    @devices.setter
+    def devices(self, devices):
+        self._devices = devices
+
+    def load_devices(self, device_filters: dict = None, device_attr_filters: dict = None):
+        if self._no_loaded_snapshots:
+            logger.warning("No loaded snapshots, cannot load devices.")
+        else:
+            if not device_attr_filters and self.attribute_filters:
+                logger.warning(
+                    f"Global `attribute_filters` is set; only pulling devices matching:\n{self.attribute_filters}."
+                )
+            try:
+                self.devices = self.inventory.devices.all(
+                    as_model=True, filters=device_filters, attr_filters=device_attr_filters
+                )
+                return self.devices
+            except HTTPStatusError:
+                logger.warning(self._api_insuf_rights + 'on POST "/tables/inventory/devices". Will not load Devices.')
+        return list()
+
+    @staticmethod
+    def _check_url(url):
+        path = urlparse(url).path
+        r = RE_PATH.search(path)
+        url = path[r.end():] if r else path  # fmt: skip
+        url = url[1:] if url[0] == "/" else url
+        return url
 
-    def _check_payload(self, url, payload, snapshot, filters, reports, sort, attr_filters):
-        if not snapshot:
-            payload.pop("snapshot", None)
+    def _check_url_payload(self, url, snapshot_id, snapshot, filters, reports, sort, attr_filters):
+        url = self._check_url(url)
+        payload = dict()
+        if filters and isinstance(filters, str):
+            filters = loads(filters)
+        if snapshot:
+            payload["snapshot"] = snapshot_id
         if filters:
             payload["filters"] = filters
         if isinstance(reports, (str, list)):
             payload["reports"] = reports
         elif reports is True and "/" + url in self.api_to_web:
             payload["reports"] = self.api_to_web["/" + url]
         elif reports is True and "/" + url not in self.api_to_web:
@@ -74,17 +114,16 @@
                 f"Table may not have any Intent Checks, please manually verify and enter to reports.\n"
                 f"Returning results without Intent Rules."
             )
         if sort:
             payload["sort"] = sort
         if RE_TABLE.match(url) and (attr_filters or self.attribute_filters):
             payload["attributeFilters"] = attr_filters or self.attribute_filters
-        return payload
+        return url, payload
 
-    @check_format
     def fetch(
         self,
         url,
         columns: Optional[List] = None,
         filters: Optional[Union[dict, str]] = None,
         limit: Optional[int] = 1000,
         start: Optional[int] = 0,
@@ -107,25 +146,22 @@
             sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
             attr_filters: Optional dictionary to apply an Attribute filter
             snapshot: Set to False for some tables like management endpoints.
 
         Returns:
             list: List of Dictionary objects.
         """
-        payload = dict(
-            columns=columns or self.get_columns(url),
-            pagination=dict(start=start, limit=limit),
-            snapshot=snapshot_id or self.snapshot_id,
-        )
-        payload = self._check_payload(url, payload, snapshot, filters, reports, sort, attr_filters)
+        snapshot_id = snapshot_id or self.snapshot_id
+        url, payload = self._check_url_payload(url, snapshot_id, snapshot, filters, reports, sort, attr_filters)
+        payload["columns"] = columns or self.get_columns(url, snapshot=snapshot)
+        payload["pagination"] = dict(start=start, limit=limit)
         res = self.post(url, json=payload)
         res.raise_for_status()
         return res.json()["data"]
 
-    @check_format
     def fetch_all(
         self,
         url: str,
         columns: Optional[List] = None,
         filters: Optional[Union[dict, str]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
@@ -144,77 +180,80 @@
             sort: Optional dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
             attr_filters: Optional dictionary to apply an Attribute filter
             snapshot: Set to False for some tables like management endpoints.
 
         Returns:
             list: List of Dictionary objects.
         """
-        payload = dict(columns=columns or self.get_columns(url), snapshot=snapshot_id or self.snapshot_id)
-        payload = self._check_payload(url, payload, snapshot, filters, reports, sort, attr_filters)
+        snapshot_id = snapshot_id or self.snapshot_id
+        url, payload = self._check_url_payload(url, snapshot_id, snapshot, filters, reports, sort, attr_filters)
+        payload["columns"] = columns or self.get_columns(url, snapshot=snapshot)
         return self._ipf_pager(url, payload)
 
-    @check_format
     def query(self, url: str, payload: Union[str, dict], get_all: bool = True) -> list:
         """Submits a query, does no formatting on the parameters.  Use for copy/pasting from the webpage.
 
         Args:
             url: Example: https://demo1.ipfabric.io/api/v1/tables/vlan/device-summary or tables/vlan/device-summary
             payload: Dictionary to submit in POST or can be JSON string (i.e. read from file).
             get_all: Default use pager to get all results and ignore pagination information in the payload
 
-
         Returns:
             list: List of Dictionary objects.
         """
+        url = self._check_url(url)
         if isinstance(payload, str):
             payload = loads(payload)
         if get_all:
             return self._ipf_pager(url, payload)
         else:
             res = self.post(url, json=payload)
             res.raise_for_status()
             return res.json()["data"]
 
-    def _get_columns(self, url: str):
+    def _get_columns(self, url: str):  # TODO: Remove in v7
         logger.warning("""Use of _get_columns will be deprecated in a future release, please use get_columns""")
-        return self.get_columns(url)
+        return self.get_columns(url=url)
 
-    def get_columns(self, url: str):
+    def get_columns(self, url: str, snapshot: bool = True) -> List[str]:
         """Submits malformed payload and extracts column names from it
 
         Args:
             url: API url to post
+            snapshot: Set to False for some tables like management endpoints.
 
         Returns:
             list: List of column names
         """
-        r = self.post(url, json=dict(snapshot=self.snapshot_id, columns=["*"]))
+        url, payload = self._check_url_payload(url, self.snapshot_id, snapshot, None, None, None, None)
+        payload["columns"] = ["*"]
+        r = self.post(url, json=payload)
         if r.status_code == 422:
             msg = r.json()["errors"][0]["message"]
             return [x.strip() for x in re.match(r"\".*\".*\[(.*)]$", msg).group(1).split(",")]
         else:
             r.raise_for_status()
 
-    @check_format
     def get_count(
         self,
         url: str,
         filters: Optional[Union[dict, str]] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         snapshot_id: Optional[str] = None,
         snapshot: bool = True,
     ) -> int:
         """Get a total number of rows
         Args:
-            url: Full URL to post to
+            url: API URL to post to
             filters: Optional dictionary of filters
             attr_filters: Optional dictionary of attribute filters
             snapshot_id: Optional snapshot_id to override default
             snapshot: Set to False for some tables like management endpoints.
         Returns:
             int: a count of rows
         """
-        payload = dict(columns=["id"], pagination=dict(limit=1, start=0), snapshot=snapshot_id or self.snapshot_id)
-        payload = self._check_payload(url, payload, snapshot, filters, None, None, attr_filters)
+        snapshot_id = snapshot_id or self.snapshot_id
+        url, payload = self._check_url_payload(url, snapshot_id, snapshot, filters, None, None, attr_filters)
+        payload.update({"columns": ["id"], "pagination": {"limit": 1, "start": 0}})
         res = self.post(url, json=payload)
         res.raise_for_status()
         return res.json()["_meta"]["count"]
```

### Comparing `ipfabric-6.2.1/ipfabric/models/intent.py` & `ipfabric-6.2.2/ipfabric/models/intent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import logging
 from typing import Any, Union, List
 
+from httpx import HTTPStatusError
+
 from .intent_check import Group, IntentCheck
 
 logger = logging.getLogger("ipfabric")
 COLOR_DICT = dict(nan=-1, green=0, blue=10, amber=20, red=30)
 
 
 class Intent:
     def __init__(self, client):
         self.client: Any = client
         self.snapshot_id: str = self.client.snapshot_id
         self.intent_checks: List[IntentCheck] = self.get_intent_checks() if self.snapshot_id else list()
         self.groups: List[Group] = self.get_groups() if self.snapshot_id else list()
 
     def get_intent_checks(self, snapshot_id: str = None) -> list:
-        """Gets all intent checks and returns a list of them.  You can also:
+        """Gets all intent checks and returns a list of them.
 
-        Examples:
-            >>> from ipfabric import IPFabric
-            >>> ipf = IPFabric()
-            >>> ipf.load_intent()  # Loads the intents to intent_checks
-            >>> print(len(ipf.intent.intent_checks))
         Args:
         snapshot_id: Optional snapshot ID to get different data
 
         Returns:
             list: List of intent checks
         """
         snapshot = self.client.snapshots[snapshot_id] if snapshot_id else self.client.snapshots[self.snapshot_id]
@@ -33,16 +30,20 @@
             raise ValueError(f"Snapshot {snapshot.snapshot_id} is not loaded; cannot pull Intent Rules.")
         if snapshot.disabled_intent_verification is True:
             raise ValueError(
                 f"Snapshot {snapshot.snapshot_id} has Intent Verification computation disabled; "
                 f"cannot pull Intent Rules."
             )
         res = self.client.get("reports", params=dict(snapshot=snapshot.snapshot_id))
-        res.raise_for_status()
-        return [IntentCheck(**check) for check in res.json()]
+        try:
+            res.raise_for_status()
+            return [IntentCheck(**check) for check in res.json()]
+        except HTTPStatusError:
+            logger.warning(self.client._api_insuf_rights + 'on GET "/reports". Will not load Intents.')
+            return list()
 
     def load_intent(self, snapshot_id: str = None):
         """Loads intent checks into the class.
 
         Args:
             snapshot_id: Uses a different Snapshot ID then client
         """
@@ -53,51 +54,43 @@
     def get_groups(self) -> list:
         """
 
         Returns:
             list: list of groups
         """
         res = self.client.get("reports/groups")
-        res.raise_for_status()
-        return [Group(**group) for group in res.json()]
+        try:
+            res.raise_for_status()
+            return [Group(**group) for group in res.json()]
+        except HTTPStatusError:
+            logger.warning(self.client._api_insuf_rights + 'on GET "/reports/groups". Will not load Intent Groups.')
+            return list()
 
     @property
     def custom(self):
-        if not self.intent_checks:
-            self.load_intent()
         return [c for c in self.intent_checks if c.custom]
 
     @property
     def builtin(self):
-        if not self.intent_checks:
-            self.load_intent()
         return [c for c in self.intent_checks if not c.custom]
 
     @property
     def intent_by_id(self):
-        if not self.intent_checks:
-            self.load_intent()
         return {c.intent_id: c for c in self.intent_checks}
 
     @property
     def intent_by_name(self):
-        if not self.intent_checks:
-            self.load_intent()
         return {c.name: c for c in self.intent_checks}
 
     @property
     def group_by_id(self):
-        if not self.groups:
-            self.load_intent()
         return {g.group_id: g for g in self.groups}
 
     @property
     def group_by_name(self):
-        if not self.groups:
-            self.load_intent()
         return {g.name: g for g in self.groups}
 
     def get_results(self, intent: IntentCheck, color: Union[str, int], snapshot_id: str = None) -> list:
         """Get the outcome of an Intent Check by a specific color
 
         Args:
             intent: an IntentCheck, please see the Intent Check Model
```

### Comparing `ipfabric-6.2.1/ipfabric/models/intent_check.py` & `ipfabric-6.2.2/ipfabric/models/intent_check.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/inventory.py` & `ipfabric-6.2.2/ipfabric/models/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any
 
 from pydantic import BaseModel
 
-from .table import Table
+from .table import Table, DeviceTable
 
 logger = logging.getLogger("ipfabric")
 
 IGNORE_COLUMNS = {"id"}
 
 
 class Inventory(BaseModel):
@@ -21,15 +21,15 @@
 
     @property
     def vendors(self):
         return Table(client=self.client, endpoint="tables/inventory/summary/vendors")
 
     @property
     def devices(self):
-        return Table(client=self.client, endpoint="tables/inventory/devices")
+        return DeviceTable(client=self.client)
 
     @property
     def models(self):
         return Table(client=self.client, endpoint="tables/inventory/summary/models")
 
     @property
     def os_version_consistency(self):
```

### Comparing `ipfabric-6.2.1/ipfabric/models/jobs.py` & `ipfabric-6.2.2/ipfabric/models/jobs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/snapshot.py` & `ipfabric-6.2.2/ipfabric/models/snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     "userCount",
 ]
 
 
 def snapshot_upload(ipf: IPFClient, filename: str):
     data = {"file": (Path(filename).name, open(filename, "rb"), "application/x-tar")}
     resp = ipf.post("snapshots/upload", files=data)
+    if resp.status_code == 400:
+        if resp.json()["code"] == "API_SNAPSHOT_CONFLICT":
+            logger.warning(f"SNAPSHOT ID {resp.json()['data']['snapshot']} already uploaded")
+            return
     resp.raise_for_status()
     return resp.json()
 
 
 class Error(BaseModel):
     error_type: str = Field(alias="errorType")
     count: int
```

### Comparing `ipfabric-6.2.1/ipfabric/models/table.py` & `ipfabric-6.2.2/ipfabric/models/table.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import logging
 from typing import Optional, Dict, List, Any, Union
 
 import deepdiff
+from httpx import HTTPStatusError
 from pydantic import BaseModel
 
+from ipfabric.models import Devices
+from ipfabric.settings import Attributes
+
 logger = logging.getLogger("ipfabric")
 
 IGNORE_COLUMNS = {"id"}
 
 
 class BaseTable(BaseModel):
     """model for table data"""
@@ -136,15 +140,15 @@
         self,
         columns: list = None,
         filters: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
-    ):
+    ) -> list:
         """Gets all data from corresponding endpoint
 
         Args:
             columns: Optional columns to return, default is all
             filters: Optional filters
             attr_filters: dict: Optional dictionary of Attribute filters
             snapshot_id: Optional snapshot ID to override class
@@ -371,7 +375,109 @@
             hashed_data_compare[hashed_str]
             for hashed_str in hashed_data_compare.keys()
             if hashed_str not in hashed_data.keys()
         ]
         return_dict["added"] = added
         return_dict["removed"] = removed
         return return_dict
+
+
+class DeviceTable(Table):
+    """model for Device Table data"""
+
+    endpoint = "tables/inventory/devices"
+
+    def _as_model(self, devices, as_model):
+        try:
+            attributes = Attributes(client=self.client, snapshot_id=self.client.snapshot_id).all()
+        except HTTPStatusError:
+            logger.warning(
+                self.client._api_insuf_rights
+                + 'on POST "/tables/snapshot-attributes". Cannot load Attributes in Devices.'
+            )
+            attributes = None
+        try:
+            blob_keys = self.client.fetch_all("/tables/management/configuration/saved", columns=["sn", "blobKey"])
+        except HTTPStatusError:
+            logger.warning(
+                self.client._api_insuf_rights + 'on POST "/tables/management/configuration/saved". '
+                "You will not be able to pull device config from Device model."
+            )
+            blob_keys = None
+        if as_model:
+            devices = Devices(
+                snapshot_id=self.client.snapshot_id, devices=devices, attributes=attributes, blob_keys=blob_keys
+            )
+        return devices
+
+    def fetch(
+        self,
+        columns: list = None,
+        filters: Optional[dict] = None,
+        attr_filters: Optional[Dict[str, List[str]]] = None,
+        snapshot_id: Optional[str] = None,
+        reports: Optional[Union[bool, list, str]] = False,
+        sort: Optional[dict] = None,
+        limit: Optional[int] = 1000,
+        start: Optional[int] = 0,
+        as_model: Optional[bool] = False,
+    ) -> Union[list, Devices]:
+        """Gets all data from corresponding endpoint
+
+        Args:
+            columns: Optional columns to return, default is all
+            filters: Optional filters'
+            attr_filters: dict: Optional dictionary of Attribute filters
+            snapshot_id: Optional snapshot ID to override class
+            reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
+            sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
+            limit: Default to 1,000 rows
+            start: Starts at 0
+            as_model: bool: Default False, if True returns Devices model
+
+        Returns:
+            list: List of Dictionaries
+        """
+        devices = super(DeviceTable, self).fetch(
+            columns=columns,
+            filters=filters,
+            attr_filters=attr_filters,
+            snapshot_id=snapshot_id,
+            reports=reports,
+            sort=sort,
+            limit=limit,
+            start=start,
+        )
+        return self._as_model(devices, as_model)
+
+    def all(
+        self,
+        columns: list = None,
+        filters: Optional[dict] = None,
+        attr_filters: Optional[Dict[str, List[str]]] = None,
+        snapshot_id: Optional[str] = None,
+        reports: Optional[Union[bool, list, str]] = False,
+        sort: Optional[dict] = None,
+        as_model: Optional[bool] = False,
+    ) -> Union[list, Devices]:
+        """Gets all data from corresponding endpoint
+
+        Args:
+            columns: Optional columns to return, default is all
+            filters: Optional filters
+            attr_filters: dict: Optional dictionary of Attribute filters
+            snapshot_id: Optional snapshot ID to override class
+            reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
+            sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
+            as_model: bool: Default False, if True returns Devices model
+        Returns:
+            list: List of Dictionaries
+        """
+        devices = super(DeviceTable, self).all(
+            columns=columns,
+            filters=filters,
+            attr_filters=attr_filters,
+            snapshot_id=snapshot_id,
+            reports=reports,
+            sort=sort,
+        )
+        return self._as_model(devices, as_model)
```

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/__init__.py` & `ipfabric-6.2.2/ipfabric/models/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/addressing.py` & `ipfabric-6.2.2/ipfabric/models/technology/addressing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/dhcp.py` & `ipfabric-6.2.2/ipfabric/models/technology/dhcp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/fhrp.py` & `ipfabric-6.2.2/ipfabric/models/technology/fhrp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/interfaces.py` & `ipfabric-6.2.2/ipfabric/models/technology/interfaces.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.2.2/ipfabric/models/technology/load_balancing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/management.py` & `ipfabric-6.2.2/ipfabric/models/technology/management.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/mpls.py` & `ipfabric-6.2.2/ipfabric/models/technology/mpls.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/multicast.py` & `ipfabric-6.2.2/ipfabric/models/technology/multicast.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/neighbors.py` & `ipfabric-6.2.2/ipfabric/models/technology/neighbors.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/oam.py` & `ipfabric-6.2.2/ipfabric/models/technology/oam.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/platforms.py` & `ipfabric-6.2.2/ipfabric/models/technology/platforms.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/port_channels.py` & `ipfabric-6.2.2/ipfabric/models/technology/port_channels.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/qos.py` & `ipfabric-6.2.2/ipfabric/models/technology/qos.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/routing.py` & `ipfabric-6.2.2/ipfabric/models/technology/routing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/sdn.py` & `ipfabric-6.2.2/ipfabric/models/technology/sdn.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/security.py` & `ipfabric-6.2.2/ipfabric/models/technology/security.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/stp.py` & `ipfabric-6.2.2/ipfabric/models/technology/stp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/vlans.py` & `ipfabric-6.2.2/ipfabric/models/technology/vlans.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/models/technology/wireless.py` & `ipfabric-6.2.2/ipfabric/models/technology/wireless.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/__init__.py` & `ipfabric-6.2.2/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/api_tokens.py` & `ipfabric-6.2.2/ipfabric/settings/api_tokens.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/attributes.py` & `ipfabric-6.2.2/ipfabric/settings/attributes.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/authentication.py` & `ipfabric-6.2.2/ipfabric/settings/authentication.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/discovery.py` & `ipfabric-6.2.2/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/seeds.py` & `ipfabric-6.2.2/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/site_separation.py` & `ipfabric-6.2.2/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/user_mgmt.py` & `ipfabric-6.2.2/ipfabric/settings/user_mgmt.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/vendor_api.py` & `ipfabric-6.2.2/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.2.2/ipfabric/settings/vendor_api_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/configuration.py` & `ipfabric-6.2.2/ipfabric/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/discovery_history.py` & `ipfabric-6.2.2/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/dashboard.json` & `ipfabric-6.2.2/ipfabric/tools/factory_defaults/v4/4/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/groups.json` & `ipfabric-6.2.2/ipfabric/tools/factory_defaults/v4/4/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/intents.json` & `ipfabric-6.2.2/ipfabric/tools/factory_defaults/v4/4/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/dashboard.json` & `ipfabric-6.2.2/ipfabric/tools/factory_defaults/v5/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/groups.json` & `ipfabric-6.2.2/ipfabric/tools/factory_defaults/v5/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/intents.json` & `ipfabric-6.2.2/ipfabric/tools/factory_defaults/v5/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/dashboard.json` & `ipfabric-6.2.2/ipfabric/tools/factory_defaults/v6/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/groups.json` & `ipfabric-6.2.2/ipfabric/tools/factory_defaults/v6/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/intents.json` & `ipfabric-6.2.2/ipfabric/tools/factory_defaults/v6/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/nist.py` & `ipfabric-6.2.2/ipfabric/tools/nist.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/restore_intents.py` & `ipfabric-6.2.2/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/shared.py` & `ipfabric-6.2.2/ipfabric/tools/shared.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.2.2/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.2.2/ipfabric/tools/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/LICENSE` & `ipfabric-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/pyproject.toml` & `ipfabric-6.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.2.1"
+version = "v6.2.2"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
@@ -27,14 +27,15 @@
 pandas = {version = "^1.3.0", optional = true}
 openpyxl = {version = "^3.0.9", optional = true}
 tabulate = {version = ">=0.8.9,<0.10.0",  optional = true}
 python-json-logger = {version = "^2.0.4",  optional = true}
 macaddress = "~2.0.2"
 pyyaml = {version = "^6.0", optional = true}
 deepdiff = "^6.2.2"
+case-insensitive-dictionary = "^0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
 black = "^22.12"
```

### Comparing `ipfabric-6.2.1/README.md` & `ipfabric-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.1/setup.py` & `ipfabric-6.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
  'ipfabric.tools.factory_defaults.v6',
  'ipfabric.tools.factory_defaults.v6.0']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['deepdiff>=6.2.2,<7.0.0',
+['case-insensitive-dictionary>=0.2.1,<0.3.0',
+ 'deepdiff>=6.2.2,<7.0.0',
  'httpx>=0.23.2,<0.24.0',
  'macaddress>=2.0.2,<2.1.0',
  'pydantic>=1.10.4,<2.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'python-dotenv>=0.21,<0.22',
  'pytz>=2023.3,<2024.0']
 
@@ -32,15 +33,15 @@
               'openpyxl>=3.0.9,<4.0.0',
               'tabulate>=0.8.9,<0.10.0',
               'python-json-logger>=2.0.4,<3.0.0',
               'pyyaml>=6.0,<7.0']}
 
 setup_kwargs = {
     'name': 'ipfabric',
-    'version': '6.2.1',
+    'version': '6.2.2',
     'description': 'Python package for interacting with IP Fabric',
     'long_description': '# IP Fabric \n\nIPFabric is a Python module for connecting to and communicating against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation. \n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- Python 3.7 support will be removed.\n- The use of `token=\'<TOKEN>\'` or `username=\'<USER>\', password=\'<PASS>\'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth=\'TOKEN\')`\n  - User/Pass: `IPFClient(auth=(\'USER\', \'PASS\'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API\'s are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK\'s match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric\n```\n\n## Introduction\n\nPlease take a look at [API Programmability - Part 1: The Basics](https://ipfabric.io/blog/api-programmability-part-1/)\nfor instructions on creating an API token.\n\nMost of the methods and features can be located in [Examples](examples) to show how to use this package. \nAnother great introduction to this package can be found at [API Programmability - Part 2: Python](https://ipfabric.io/blog/api-programmability-python/)\n\n## Diagrams\n\nDiagramming in IP Fabric version v4.3 and above has been moved to it\'s own package.\n\nDiagramming will move back to this project in v7.0\n\n```\npip install ipfabric-diagrams\n```\n\n## Authentication\n### Username/Password\nSupply in client:\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=(\'user\', \'pass\'))\n```\n\n### Token\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=\'token\')\n```\n\n### Environment \nThe easiest way to use this package is with a `.env` file.  You can copy the sample and edit it with your environment variables. \n\n```commandline\ncp sample.env .env\n```\n\nThis contains the following variables which can also be set as environment variables instead of a .env file.\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_TOKEN=TOKEN\nIPF_VERIFY=true\n```\n\nOr if using Username/Password:\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_USERNAME=USER\nIPF_PASSWORD=PASS\n```\n\n## Development\n\n### Poetry Installation\n\nIPFabric uses [Poetry](https://pypi.org/project/poetry/) to make setting up a virtual environment with all dependencies\ninstalled quick and easy.\n\nInstall poetry globally:\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo run examples, install extras:\n```\npoetry install ipfabric -E examples\n```\n\n### Test and Build\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric\npoetry update\n```\n',
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric',
```

### Comparing `ipfabric-6.2.1/PKG-INFO` & `ipfabric-6.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.2.1
+Version: 6.2.2
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: examples
+Requires-Dist: case-insensitive-dictionary (>=0.2.1,<0.3.0)
 Requires-Dist: deepdiff (>=6.2.2,<7.0.0)
 Requires-Dist: httpx (>=0.23.2,<0.24.0)
 Requires-Dist: macaddress (>=2.0.2,<2.1.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0) ; extra == "examples"
 Requires-Dist: pandas (>=1.3.0,<2.0.0) ; extra == "examples"
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
```

