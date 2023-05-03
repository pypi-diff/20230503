# Comparing `tmp/netbox_plugin_dns-0.18.0b1.tar.gz` & `tmp/netbox_plugin_dns-0.18.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_dns-0.18.0b1.tar", max compression
+gzip compressed data, was "netbox_plugin_dns-0.18.0b5.tar", max compression
```

## Comparing `netbox_plugin_dns-0.18.0b1.tar` & `netbox_plugin_dns-0.18.0b5.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     1076 2022-07-17 16:18:33.855780 netbox_plugin_dns-0.18.0b1/LICENSE
--rw-r--r--   0        0        0     3096 2023-05-02 21:38:03.057221 netbox_plugin_dns-0.18.0b1/README.md
--rw-r--r--   0        0        0      909 2023-05-02 21:38:24.559937 netbox_plugin_dns-0.18.0b1/netbox_dns/__init__.py
--rw-r--r--   0        0        0      512 2022-07-17 16:18:33.872788 netbox_plugin_dns-0.18.0b1/netbox_dns/admin.py
--rw-r--r--   0        0        0     1951 2023-04-02 13:35:16.802838 netbox_plugin_dns-0.18.0b1/netbox_dns/api/nested_serializers.py
--rw-r--r--   0        0        0     4555 2022-12-22 08:12:50.669592 netbox_plugin_dns-0.18.0b1/netbox_dns/api/serializers.py
--rw-r--r--   0        0        0      441 2022-07-17 16:18:33.873476 netbox_plugin_dns-0.18.0b1/netbox_dns/api/urls.py
--rw-r--r--   0        0        0     3060 2022-07-17 16:18:33.873678 netbox_plugin_dns-0.18.0b1/netbox_dns/api/views.py
--rw-r--r--   0        0        0      151 2022-10-24 11:40:31.264932 netbox_plugin_dns-0.18.0b1/netbox_dns/apps.py
--rw-r--r--   0        0        0       46 2022-12-22 08:12:55.785535 netbox_plugin_dns-0.18.0b1/netbox_dns/fields/__init__.py
--rw-r--r--   0        0        0     1530 2022-12-22 08:12:55.785726 netbox_plugin_dns-0.18.0b1/netbox_dns/fields/address.py
--rw-r--r--   0        0        0     3023 2022-12-22 08:12:55.785924 netbox_plugin_dns-0.18.0b1/netbox_dns/fields/network.py
--rw-r--r--   0        0        0       88 2022-07-17 16:18:33.873956 netbox_plugin_dns-0.18.0b1/netbox_dns/filters/__init__.py
--rwxr-xr-x   0        0        0      596 2022-07-17 16:18:33.874098 netbox_plugin_dns-0.18.0b1/netbox_dns/filters/nameserver.py
--rwxr-xr-x   0        0        0     1609 2022-08-18 09:11:58.958786 netbox_plugin_dns-0.18.0b1/netbox_dns/filters/record.py
--rw-r--r--   0        0        0      572 2022-07-17 16:18:33.874580 netbox_plugin_dns-0.18.0b1/netbox_dns/filters/view.py
--rwxr-xr-x   0        0        0     1179 2022-10-24 11:43:44.507516 netbox_plugin_dns-0.18.0b1/netbox_dns/filters/zone.py
--rw-r--r--   0        0        0       88 2022-07-17 16:18:33.874949 netbox_plugin_dns-0.18.0b1/netbox_dns/forms/__init__.py
--rwxr-xr-x   0        0        0     1308 2023-05-02 21:38:03.058431 netbox_plugin_dns-0.18.0b1/netbox_dns/forms/nameserver.py
--rwxr-xr-x   0        0        0     5083 2023-05-02 21:38:03.059309 netbox_plugin_dns-0.18.0b1/netbox_dns/forms/record.py
--rw-r--r--   0        0        0      961 2023-05-02 21:38:03.060131 netbox_plugin_dns-0.18.0b1/netbox_dns/forms/view.py
--rwxr-xr-x   0        0        0    14198 2023-05-02 21:38:03.060860 netbox_plugin_dns-0.18.0b1/netbox_dns/forms/zone.py
--rw-r--r--   0        0        0      604 2022-12-22 08:12:55.788382 netbox_plugin_dns-0.18.0b1/netbox_dns/graphql/__init__.py
--rw-r--r--   0        0        0      527 2022-07-17 16:18:33.876024 netbox_plugin_dns-0.18.0b1/netbox_dns/graphql/nameserver.py
--rw-r--r--   0        0        0      487 2022-07-17 16:18:33.876212 netbox_plugin_dns-0.18.0b1/netbox_dns/graphql/record.py
--rw-r--r--   0        0        0      221 2022-07-17 16:18:33.876372 netbox_plugin_dns-0.18.0b1/netbox_dns/graphql/schema.py
--rw-r--r--   0        0        0      467 2022-07-17 16:18:33.876520 netbox_plugin_dns-0.18.0b1/netbox_dns/graphql/view.py
--rw-r--r--   0        0        0      467 2022-07-17 16:18:33.876631 netbox_plugin_dns-0.18.0b1/netbox_dns/graphql/zone.py
--rw-r--r--   0        0        0     6035 2023-04-02 13:35:16.805068 netbox_plugin_dns-0.18.0b1/netbox_dns/management/commands/cleanup_database.py
--rw-r--r--   0        0        0      661 2022-07-17 16:18:33.877004 netbox_plugin_dns-0.18.0b1/netbox_dns/management/commands/update_soa.py
--rw-r--r--   0        0        0     4153 2023-04-02 13:35:16.805325 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0001_initial.py
--rw-r--r--   0        0        0    11513 2023-04-02 13:35:16.805620 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
--rw-r--r--   0        0        0      437 2023-04-02 13:35:16.805791 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0002_zone_default_ttl.py
--rw-r--r--   0        0        0     3716 2023-04-02 13:35:16.806012 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0003_soa_managed_records.py
--rw-r--r--   0        0        0     2287 2022-12-22 08:12:55.789196 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py
--rw-r--r--   0        0        0     1156 2023-04-02 13:35:16.806287 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0005_update_ns_records.py
--rw-r--r--   0        0        0      861 2023-04-02 13:35:16.806490 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0006_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      399 2023-04-02 13:35:16.806721 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0007_alter_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      527 2023-04-02 13:35:16.807012 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0008_zone_status_names.py
--rw-r--r--   0        0        0     2176 2023-04-02 13:35:16.807205 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0009_netbox32.py
--rw-r--r--   0        0        0     1543 2022-07-17 16:18:33.878802 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0010_update_soa_records.py
--rw-r--r--   0        0        0     2201 2023-04-02 13:35:16.807512 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0011_add_view_model.py
--rw-r--r--   0        0        0      402 2023-04-02 13:35:16.807776 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0012_adjust_zone_and_record.py
--rw-r--r--   0        0        0      733 2023-04-02 13:35:16.808038 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py
--rw-r--r--   0        0        0      428 2023-04-02 13:35:16.808282 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0014_add_view_description.py
--rw-r--r--   0        0        0      393 2023-04-02 13:35:16.808474 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0015_add_record_status.py
--rw-r--r--   0        0        0     1053 2023-04-02 13:35:16.808701 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0016_cleanup_ptr_records.py
--rw-r--r--   0        0        0      405 2023-04-02 13:35:16.808982 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0017_alter_record_ttl.py
--rw-r--r--   0        0        0     1553 2023-04-02 13:35:16.809193 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0018_zone_arpa_network.py
--rw-r--r--   0        0        0      433 2023-04-02 13:35:16.809450 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0019_update_ns_ttl.py
--rw-r--r--   0        0        0     1260 2023-04-02 13:35:16.809723 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0020_netbox_3_4.py
--rw-r--r--   0        0        0     3304 2023-04-02 13:35:16.809999 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0021_record_ip_address.py
--rw-r--r--   0        0        0      891 2023-04-02 13:35:16.810254 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0022_search.py
--rw-r--r--   0        0        0        0 2022-07-17 16:18:33.879155 netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/__init__.py
--rw-r--r--   0        0        0    28247 2023-04-02 13:35:16.810736 netbox_plugin_dns-0.18.0b1/netbox_dns/models.py
--rw-r--r--   0        0        0     3158 2022-12-22 08:12:55.791521 netbox_plugin_dns-0.18.0b1/netbox_dns/navigation.py
--rw-r--r--   0        0        0       88 2022-07-17 16:18:33.879860 netbox_plugin_dns-0.18.0b1/netbox_dns/tables/__init__.py
--rw-r--r--   0        0        0      701 2023-04-02 13:35:16.811050 netbox_plugin_dns-0.18.0b1/netbox_dns/tables/nameserver.py
--rw-r--r--   0        0        0     3064 2023-04-02 13:35:16.811382 netbox_plugin_dns-0.18.0b1/netbox_dns/tables/record.py
--rw-r--r--   0        0        0      325 2022-07-28 12:40:17.148541 netbox_plugin_dns-0.18.0b1/netbox_dns/tables/view.py
--rw-r--r--   0        0        0     1660 2023-04-02 13:35:16.811669 netbox_plugin_dns-0.18.0b1/netbox_dns/tables/zone.py
--rw-r--r--   0        0        0     1980 2022-12-22 08:12:55.792723 netbox_plugin_dns-0.18.0b1/netbox_dns/template_content.py
--rw-r--r--   0        0        0     1192 2023-04-02 13:34:21.822417 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/nameserver.html
--rw-r--r--   0        0        0       89 2022-12-22 08:12:55.793857 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/record/managed.html
--rw-r--r--   0        0        0      378 2022-12-22 08:12:55.794103 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/record/related.html
--rw-r--r--   0        0        0     4136 2023-04-02 13:35:16.812028 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/record.html
--rw-r--r--   0        0        0      919 2022-12-22 08:12:55.794573 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/view.html
--rw-r--r--   0        0        0      460 2022-12-22 08:12:55.795482 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/zone/base.html
--rw-r--r--   0        0        0     2139 2022-12-22 08:12:55.795809 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/zone/child.html
--rw-r--r--   0        0        0      492 2022-12-22 08:12:55.796064 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/zone/managed_record.html
--rw-r--r--   0        0        0     2186 2022-12-22 08:12:55.796573 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/zone/record.html
--rw-r--r--   0        0        0      215 2022-12-22 08:12:55.797323 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/zone/related.html
--rw-r--r--   0        0        0     5480 2023-04-02 13:34:21.822729 netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/zone.html
--rw-r--r--   0        0        0        0 2022-07-17 16:18:33.882509 netbox_plugin_dns-0.18.0b1/netbox_dns/templatetags/__init__.py
--rw-r--r--   0        0        0      271 2022-07-17 16:18:33.882686 netbox_plugin_dns-0.18.0b1/netbox_dns/templatetags/view_helpers.py
--rw-r--r--   0        0        0     5202 2022-12-22 08:12:55.801975 netbox_plugin_dns-0.18.0b1/netbox_dns/urls.py
--rw-r--r--   0        0        0     1537 2023-04-02 13:35:16.816079 netbox_plugin_dns-0.18.0b1/netbox_dns/utilities.py
--rw-r--r--   0        0        0     1969 2023-04-02 13:35:16.816370 netbox_plugin_dns-0.18.0b1/netbox_dns/validators.py
--rw-r--r--   0        0        0       88 2022-07-17 16:18:33.886884 netbox_plugin_dns-0.18.0b1/netbox_dns/views/__init__.py
--rw-r--r--   0        0        0     2991 2023-04-02 13:35:16.816747 netbox_plugin_dns-0.18.0b1/netbox_dns/views/nameserver.py
--rw-r--r--   0        0        0     2554 2023-04-02 13:35:16.817070 netbox_plugin_dns-0.18.0b1/netbox_dns/views/record.py
--rw-r--r--   0        0        0     1895 2022-12-22 08:12:55.803351 netbox_plugin_dns-0.18.0b1/netbox_dns/views/view.py
--rw-r--r--   0        0        0     3600 2023-04-02 13:35:16.817363 netbox_plugin_dns-0.18.0b1/netbox_dns/views/zone.py
--rw-r--r--   0        0        0      698 2023-05-02 21:54:53.816806 netbox_plugin_dns-0.18.0b1/pyproject.toml
--rw-r--r--   0        0        0     3884 1970-01-01 00:00:00.000000 netbox_plugin_dns-0.18.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-03 10:39:22.373572 netbox_plugin_dns-0.18.0b5/LICENSE
+-rw-r--r--   0        0        0     3096 2023-05-03 10:39:22.373572 netbox_plugin_dns-0.18.0b5/README.md
+-rw-r--r--   0        0        0      909 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/admin.py
+-rw-r--r--   0        0        0     1951 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/api/nested_serializers.py
+-rw-r--r--   0        0        0     4555 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/api/serializers.py
+-rw-r--r--   0        0        0      441 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/api/urls.py
+-rw-r--r--   0        0        0     3060 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/api/views.py
+-rw-r--r--   0        0        0      151 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/apps.py
+-rw-r--r--   0        0        0       46 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/fields/__init__.py
+-rw-r--r--   0        0        0     1530 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/fields/address.py
+-rw-r--r--   0        0        0     3023 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/fields/network.py
+-rw-r--r--   0        0        0       88 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/filters/__init__.py
+-rwxr-xr-x   0        0        0      596 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/filters/nameserver.py
+-rwxr-xr-x   0        0        0     1609 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/filters/record.py
+-rw-r--r--   0        0        0      572 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/filters/view.py
+-rwxr-xr-x   0        0        0     1179 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/filters/zone.py
+-rw-r--r--   0        0        0       88 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/forms/__init__.py
+-rwxr-xr-x   0        0        0     1308 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/forms/nameserver.py
+-rwxr-xr-x   0        0        0     5083 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/forms/record.py
+-rw-r--r--   0        0        0      961 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/forms/view.py
+-rwxr-xr-x   0        0        0    14198 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/forms/zone.py
+-rw-r--r--   0        0        0      604 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/graphql/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/graphql/nameserver.py
+-rw-r--r--   0        0        0      487 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/graphql/record.py
+-rw-r--r--   0        0        0      221 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/graphql/schema.py
+-rw-r--r--   0        0        0      467 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/graphql/view.py
+-rw-r--r--   0        0        0      467 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/graphql/zone.py
+-rw-r--r--   0        0        0     6035 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/management/commands/cleanup_database.py
+-rw-r--r--   0        0        0      661 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/management/commands/update_soa.py
+-rw-r--r--   0        0        0     4153 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0001_initial.py
+-rw-r--r--   0        0        0    11513 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
+-rw-r--r--   0        0        0      437 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0002_zone_default_ttl.py
+-rw-r--r--   0        0        0     3716 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0003_soa_managed_records.py
+-rw-r--r--   0        0        0     2287 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py
+-rw-r--r--   0        0        0     1156 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0005_update_ns_records.py
+-rw-r--r--   0        0        0      861 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0006_zone_soa_serial_auto.py
+-rw-r--r--   0        0        0      399 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0007_alter_zone_soa_serial_auto.py
+-rw-r--r--   0        0        0      527 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0008_zone_status_names.py
+-rw-r--r--   0        0        0     2176 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0009_netbox32.py
+-rw-r--r--   0        0        0     1543 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0010_update_soa_records.py
+-rw-r--r--   0        0        0     2201 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0011_add_view_model.py
+-rw-r--r--   0        0        0      402 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0012_adjust_zone_and_record.py
+-rw-r--r--   0        0        0      733 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py
+-rw-r--r--   0        0        0      428 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0014_add_view_description.py
+-rw-r--r--   0        0        0      393 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0015_add_record_status.py
+-rw-r--r--   0        0        0     1053 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0016_cleanup_ptr_records.py
+-rw-r--r--   0        0        0      405 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0017_alter_record_ttl.py
+-rw-r--r--   0        0        0     1553 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0018_zone_arpa_network.py
+-rw-r--r--   0        0        0      433 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0019_update_ns_ttl.py
+-rw-r--r--   0        0        0     1260 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0020_netbox_3_4.py
+-rw-r--r--   0        0        0     3304 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0021_record_ip_address.py
+-rw-r--r--   0        0        0      891 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0022_search.py
+-rw-r--r--   0        0        0        0 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/__init__.py
+-rw-r--r--   0        0        0    28247 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/models.py
+-rw-r--r--   0        0        0     3158 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/navigation.py
+-rw-r--r--   0        0        0       88 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/tables/__init__.py
+-rw-r--r--   0        0        0      701 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/tables/nameserver.py
+-rw-r--r--   0        0        0     3064 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/tables/record.py
+-rw-r--r--   0        0        0      325 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/tables/view.py
+-rw-r--r--   0        0        0     1660 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/tables/zone.py
+-rw-r--r--   0        0        0     1980 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/template_content.py
+-rw-r--r--   0        0        0     1192 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/nameserver.html
+-rw-r--r--   0        0        0       89 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/record/managed.html
+-rw-r--r--   0        0        0      378 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/record/related.html
+-rw-r--r--   0        0        0     4136 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/record.html
+-rw-r--r--   0        0        0      919 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/view.html
+-rw-r--r--   0        0        0      460 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/zone/base.html
+-rw-r--r--   0        0        0     2139 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/zone/child.html
+-rw-r--r--   0        0        0      492 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/zone/managed_record.html
+-rw-r--r--   0        0        0     2186 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/zone/record.html
+-rw-r--r--   0        0        0      215 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/zone/related.html
+-rw-r--r--   0        0        0     5480 2023-05-03 10:39:22.397573 netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/zone.html
+-rw-r--r--   0        0        0        0 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/templatetags/__init__.py
+-rw-r--r--   0        0        0      271 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/templatetags/view_helpers.py
+-rw-r--r--   0        0        0     5202 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/urls.py
+-rw-r--r--   0        0        0     1537 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/utilities.py
+-rw-r--r--   0        0        0     1969 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/validators.py
+-rw-r--r--   0        0        0       88 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/views/__init__.py
+-rw-r--r--   0        0        0     2991 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/views/nameserver.py
+-rw-r--r--   0        0        0     2554 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/views/record.py
+-rw-r--r--   0        0        0     1895 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/views/view.py
+-rw-r--r--   0        0        0     3600 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/netbox_dns/views/zone.py
+-rw-r--r--   0        0        0      696 2023-05-03 10:39:22.401573 netbox_plugin_dns-0.18.0b5/pyproject.toml
+-rw-r--r--   0        0        0     3880 1970-01-01 00:00:00.000000 netbox_plugin_dns-0.18.0b5/PKG-INFO
```

### Comparing `netbox_plugin_dns-0.18.0b1/LICENSE` & `netbox_plugin_dns-0.18.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/README.md` & `netbox_plugin_dns-0.18.0b5/README.md`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/__init__.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from extras.plugins import PluginConfig
 
-__version__ = "0.18.0-beta1"
+__version__ = "0.18.0-beta5"
 
 
 class DNSConfig(PluginConfig):
     name = "netbox_dns"
     verbose_name = "Netbox DNS"
     description = "Netbox DNS"
     min_version = "3.5"
```

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/admin.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/api/nested_serializers.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/api/serializers.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/api/views.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/fields/address.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/fields/address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/fields/network.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/fields/network.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/filters/nameserver.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/filters/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/filters/record.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/filters/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/filters/view.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/filters/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/filters/zone.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/filters/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/forms/nameserver.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/forms/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/forms/record.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/forms/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/forms/view.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/forms/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/forms/zone.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/forms/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/graphql/__init__.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/graphql/nameserver.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/graphql/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/management/commands/cleanup_database.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/management/commands/cleanup_database.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/management/commands/update_soa.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/management/commands/update_soa.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0001_initial.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0003_soa_managed_records.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0003_soa_managed_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0005_update_ns_records.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0005_update_ns_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0006_zone_soa_serial_auto.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0006_zone_soa_serial_auto.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0008_zone_status_names.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0008_zone_status_names.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0009_netbox32.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0009_netbox32.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0010_update_soa_records.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0010_update_soa_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0011_add_view_model.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0011_add_view_model.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0016_cleanup_ptr_records.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0016_cleanup_ptr_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0018_zone_arpa_network.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0018_zone_arpa_network.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0020_netbox_3_4.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0020_netbox_3_4.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0021_record_ip_address.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0021_record_ip_address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/migrations/0022_search.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/migrations/0022_search.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/models.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/models.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/navigation.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/tables/nameserver.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/tables/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/tables/record.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/tables/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/tables/zone.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/tables/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/template_content.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/nameserver.html` & `netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/nameserver.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/record.html` & `netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/view.html` & `netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/view.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/zone/child.html` & `netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/zone/child.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/zone/record.html` & `netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/zone/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/templates/netbox_dns/zone.html` & `netbox_plugin_dns-0.18.0b5/netbox_dns/templates/netbox_dns/zone.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/urls.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/utilities.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/utilities.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/validators.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/validators.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/views/nameserver.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/views/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/views/record.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/views/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/views/view.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/views/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/netbox_dns/views/zone.py` & `netbox_plugin_dns-0.18.0b5/netbox_dns/views/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.18.0b1/PKG-INFO` & `netbox_plugin_dns-0.18.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-dns
-Version: 0.18.0b1
-Summary: Netbox DNS is a netbox plugin for managing DNS inventory
+Version: 0.18.0b5
+Summary: Netbox DNS is a NetBox plugin for managing DNS data.
 Home-page: https://github.com/peteeckel/netbox-plugin-dns
 License: MIT
 Keywords: netbox,netbox-plugin,dns
 Author: Peter Eckel
 Author-email: pe-netbox-dns@hindenburgring.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 0.18.0b1 Summary: Netbox
-DNS is a netbox plugin for managing DNS inventory Home-page: https://
-github.com/peteeckel/netbox-plugin-dns License: MIT Keywords: netbox,netbox-
-plugin,dns Author: Peter Eckel Author-email: pe-netbox-dns@hindenburgring.com
-Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
+Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 0.18.0b5 Summary: Netbox
+DNS is a NetBox plugin for managing DNS data. Home-page: https://github.com/
+peteeckel/netbox-plugin-dns License: MIT Keywords: netbox,netbox-plugin,dns
+Author: Peter Eckel Author-email: pe-netbox-dns@hindenburgring.com Requires-
+Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: dnspython (>=2.2.1,<3.0.0) Project-
 URL: Repository, https://github.com/peteeckel/netbox-plugin-dns Description-
 Content-Type: text/markdown
                            ****** NetBox DNS ******
```

