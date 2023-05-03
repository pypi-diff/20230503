# Comparing `tmp/SoftLayer-6.1.6.tar.gz` & `tmp/SoftLayer-6.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SoftLayer-6.1.6.tar", last modified: Mon Mar 27 21:56:36 2023, max compression
+gzip compressed data, was "SoftLayer-6.1.7.tar", last modified: Wed May  3 21:38:24 2023, max compression
```

## Comparing `SoftLayer-6.1.6.tar` & `SoftLayer-6.1.7.tar`

### file list

```diff
@@ -1,650 +1,655 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.966558 SoftLayer-6.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-03-27 21:56:36.966558 SoftLayer-6.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.846556 SoftLayer-6.1.6/SoftLayer/
--rw-r--r--   0 runner    (1001) docker     (123)    22932 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/API.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.854556 SoftLayer-6.1.6/SoftLayer/CLI/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.854556 SoftLayer-6.1.6/SoftLayer/CLI/account/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/bandwidth_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/bandwidth_pools_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/billing_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/cancel_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/hook_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/hook_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/invoice_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/invoices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/item_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/account/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.858556 SoftLayer-6.1.6/SoftLayer/CLI/block/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.862556 SoftLayer-6.1.6/SoftLayer/CLI/block/access/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/access/authorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/access/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/access/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/access/revoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/duplicate_convert_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/lun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/modify.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/object_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/object_storage_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/object_storage_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/refresh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.862556 SoftLayer-6.1.6/SoftLayer/CLI/block/replication/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/replication/disaster_recovery_failover.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/replication/failback.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/replication/failover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/replication/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/replication/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/replication/partners.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/set_note.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.862556 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/get_notify_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/schedule_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/set_notify_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.866556 SoftLayer-6.1.6/SoftLayer/CLI/block/subnets/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/subnets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/subnets/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/subnets/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/block/subnets/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/call_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.866556 SoftLayer-6.1.6/SoftLayer/CLI/cdn/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/cdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/cdn/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/cdn/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/cdn/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/cdn/origin_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/cdn/origin_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/cdn/origin_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/cdn/purge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.866556 SoftLayer-6.1.6/SoftLayer/CLI/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/config/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/config/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.870556 SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/cancel_guests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/list_guests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.870556 SoftLayer-6.1.6/SoftLayer/CLI/dns/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/record_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/record_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/record_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/record_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/zone_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/zone_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/zone_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/zone_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/dns/zone_print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.870556 SoftLayer-6.1.6/SoftLayer/CLI/email/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/email/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/email/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/email/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.870556 SoftLayer-6.1.6/SoftLayer/CLI/event_log/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/event_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/event_log/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/event_log/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.874556 SoftLayer-6.1.6/SoftLayer/CLI/file/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.874556 SoftLayer-6.1.6/SoftLayer/CLI/file/access/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/access/authorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/access/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/access/revoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/duplicate_convert_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/modify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/refresh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.878556 SoftLayer-6.1.6/SoftLayer/CLI/file/replication/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/replication/disaster_recovery_failover.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/replication/failback.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/replication/failover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/replication/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/replication/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/replication/partners.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/set_note.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.878556 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/get_notify_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/schedule_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/set_notify_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.882557 SoftLayer-6.1.6/SoftLayer/CLI/firewall/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/firewall/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/firewall/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/firewall/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/firewall/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/firewall/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/firewall/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.882557 SoftLayer-6.1.6/SoftLayer/CLI/globalip/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/globalip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/globalip/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/globalip/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/globalip/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/globalip/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/globalip/unassign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.886556 SoftLayer-6.1.6/SoftLayer/CLI/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/authorize_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/cancel_reasons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/create_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/notification_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/notification_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/ready.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/reflash_firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/reload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/toggle_ipmi.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/update_firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/hardware/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.890556 SoftLayer-6.1.6/SoftLayer/CLI/image/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/share.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/image/share_deny.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.890556 SoftLayer-6.1.6/SoftLayer/CLI/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/licenses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/licenses/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/licenses/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/licenses/create_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.890556 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/layer7_policy_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/ns_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/ns_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/loadbal/pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.894557 SoftLayer-6.1.6/SoftLayer/CLI/nas/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/nas/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/nas/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.894557 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.894557 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/list_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/object_storage/list_endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.898557 SoftLayer-6.1.6/SoftLayer/CLI/order/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/category_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/item_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/package_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/package_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/place_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/preset_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/quote_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/quote_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/order/quote_save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.898557 SoftLayer-6.1.6/SoftLayer/CLI/report/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/report/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/report/dc_closures.py
--rw-r--r--   0 runner    (1001) docker     (123)    23126 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.898557 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.898557 SoftLayer-6.1.6/SoftLayer/CLI/sshkey/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/sshkey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/sshkey/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/sshkey/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/sshkey/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/sshkey/print.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/sshkey/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.902557 SoftLayer-6.1.6/SoftLayer/CLI/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ssl/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ssl/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ssl/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ssl/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ssl/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/storage_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.902557 SoftLayer-6.1.6/SoftLayer/CLI/subnet/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/clear_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/edit_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/subnet/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.906557 SoftLayer-6.1.6/SoftLayer/CLI/tags/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/tags/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/tags/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/tags/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/tags/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/tags/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/tags/taggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.906557 SoftLayer-6.1.6/SoftLayer/CLI/ticket/
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/attach.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/detach.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/ticket/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.910557 SoftLayer-6.1.6/SoftLayer/CLI/user/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/device_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/edit_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/edit_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/edit_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/grant_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/remove_access.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/vpn_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/user/vpn_subnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.914557 SoftLayer-6.1.6/SoftLayer/CLI/virt/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/authorize_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/cancel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.918557 SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/create_guest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/notification_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/notification_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/os_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.918557 SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/ready.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/reload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/virt/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.918557 SoftLayer-6.1.6/SoftLayer/CLI/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vlan/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vlan/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vlan/create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vlan/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vlan/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vlan/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.918557 SoftLayer-6.1.6/SoftLayer/CLI/vpn/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.922557 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.922557 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/subnet/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/subnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/subnet/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/subnet/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.922557 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/translation/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/translation/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/translation/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/translation/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/decoration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.938557 SoftLayer-6.1.6/SoftLayer/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/BluePages_Search.py
--rw-r--r--   0 runner    (1001) docker     (123)    43920 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Account.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Billing_Invoice_Item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Billing_Item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Billing_Order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Dns_Domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Dns_Domain_ResourceRecord.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Email_Subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Event_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Hardware_Server.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Location.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Location_Datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Health_Check_Type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Type.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service_Group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Cache_Purge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Firewall_Update_Request.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_LBaaS_HealthMonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Service_Vpn_Overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress_Global.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Subnet_Rwhois_Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Product_Order.py
--rw-r--r--   0 runner    (1001) docker     (123)    75145 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Product_Package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Provisioning_Hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Resource_Metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Scale_Group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Scale_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Security_Certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Security_Ssh_Key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Software_Component_Password.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Ticket_Subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Customer.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py
--rw-r--r--   0 runner    (1001) docker     (123)    29326 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_Host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup_Rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.946557 SoftLayer-6.1.6/SoftLayer/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/cdn.py
--rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/dedicated_host.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/ipsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    34611 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    32093 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/sshkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    26132 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    42319 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    18798 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    63471 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/vs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/vs_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/managers/vs_placement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.946557 SoftLayer-6.1.6/SoftLayer/shell/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/shell/cmd_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/shell/cmd_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/shell/cmd_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/shell/completer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/shell/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/shell/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.946557 SoftLayer-6.1.6/SoftLayer/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/testing/xmlrpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.946557 SoftLayer-6.1.6/SoftLayer/transports/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/transports/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/transports/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/transports/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/transports/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/transports/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/transports/xmlrpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/SoftLayer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.850556 SoftLayer-6.1.6/SoftLayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-03-27 21:56:36.000000 SoftLayer-6.1.6/SoftLayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21854 2023-03-27 21:56:36.000000 SoftLayer-6.1.6/SoftLayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:56:36.000000 SoftLayer-6.1.6/SoftLayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-27 21:56:36.000000 SoftLayer-6.1.6/SoftLayer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:56:36.000000 SoftLayer-6.1.6/SoftLayer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-27 21:56:36.000000 SoftLayer-6.1.6/SoftLayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 21:56:36.000000 SoftLayer-6.1.6/SoftLayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-27 21:56:36.970558 SoftLayer-6.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.846556 SoftLayer-6.1.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.950558 SoftLayer-6.1.6/tests/CLI/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/core_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/custom_types_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/environment_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/helper_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.958558 SoftLayer-6.1.6/tests/CLI/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/account_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    36346 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/block_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/call_api_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/cdn_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/config_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/dedicatedhost_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/dns_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/email_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/event_log_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/file_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/firewall_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/globalip_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/image_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    27405 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/ipsec_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/licenses_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/loadbal_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/nas_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/object_storage_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/order_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/report_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/search_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/securitygroup_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    44596 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/server_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/sshkey_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/ssl_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/subnet_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/summary_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/tag_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/ticket_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/user_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/vlan_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.958558 SoftLayer-6.1.6/tests/CLI/modules/vs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/vs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/vs/vs_capacity_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    32863 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/vs/vs_create_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/vs/vs_placement_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    43855 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/CLI/modules/vs/vs_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.966558 SoftLayer-6.1.6/tests/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/account_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    41784 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/block_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/cdn_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/dedicated_host_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/dns_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/email_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/event_log_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    34792 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/file_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/firewall_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    42708 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/hardware_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/image_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    16589 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/ipsec_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/loadbal_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/metadata_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    28050 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/network_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/object_storage_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    40125 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/ordering_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/search_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/sshkey_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/ssl_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/storage_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)   142912 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/storage_utils_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/tag_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/ticket_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/user_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.966558 SoftLayer-6.1.6/tests/managers/vs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/vs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/vs/vs_capacity_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/vs/vs_order_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/vs/vs_placement_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    45298 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/vs/vs_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/managers/vs/vs_waiting_for_ready_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:36.966558 SoftLayer-6.1.6/tests/transports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/transports/debug_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/transports/rest_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/transports/transport_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14582 2023-03-27 21:56:23.000000 SoftLayer-6.1.6/tests/transports/xmlrpc_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.328389 SoftLayer-6.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-05-03 21:38:24.328389 SoftLayer-6.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.256388 SoftLayer-6.1.7/SoftLayer/
+-rw-r--r--   0 runner    (1001) docker     (123)    22932 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/API.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.256388 SoftLayer-6.1.7/SoftLayer/CLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.260388 SoftLayer-6.1.7/SoftLayer/CLI/account/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/bandwidth_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/bandwidth_pools_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/billing_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/cancel_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/hook_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/hook_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/invoice_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/item_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/account/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.260388 SoftLayer-6.1.7/SoftLayer/CLI/block/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.264388 SoftLayer-6.1.7/SoftLayer/CLI/block/access/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/access/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/access/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/access/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/access/revoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/duplicate_convert_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/lun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/object_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/object_storage_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/object_storage_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/refresh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.264388 SoftLayer-6.1.7/SoftLayer/CLI/block/replication/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/replication/disaster_recovery_failover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/replication/failback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/replication/failover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/replication/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/replication/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/replication/partners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/set_note.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.264388 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/get_notify_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/schedule_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/set_notify_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.264388 SoftLayer-6.1.7/SoftLayer/CLI/block/subnets/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/subnets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/subnets/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/subnets/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/block/subnets/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/call_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.268388 SoftLayer-6.1.7/SoftLayer/CLI/cdn/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/origin_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/origin_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/origin_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/cdn/purge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.268388 SoftLayer-6.1.7/SoftLayer/CLI/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/config/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/config/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.268388 SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/cancel_guests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/list_guests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.268388 SoftLayer-6.1.7/SoftLayer/CLI/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/record_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/record_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/record_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/record_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/zone_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/zone_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/zone_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/zone_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/dns/zone_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.268388 SoftLayer-6.1.7/SoftLayer/CLI/email/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/email/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/email/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/email/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.268388 SoftLayer-6.1.7/SoftLayer/CLI/event_log/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/event_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/event_log/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/event_log/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.272388 SoftLayer-6.1.7/SoftLayer/CLI/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.272388 SoftLayer-6.1.7/SoftLayer/CLI/file/access/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/access/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/access/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/access/revoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/duplicate_convert_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/refresh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.272388 SoftLayer-6.1.7/SoftLayer/CLI/file/replication/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/replication/disaster_recovery_failover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/replication/failback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/replication/failover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/replication/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/replication/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/replication/partners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/set_note.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.276388 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/get_notify_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/schedule_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/set_notify_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.276388 SoftLayer-6.1.7/SoftLayer/CLI/firewall/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/firewall/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/firewall/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/firewall/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/firewall/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/firewall/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/firewall/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.276388 SoftLayer-6.1.7/SoftLayer/CLI/globalip/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/globalip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/globalip/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/globalip/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/globalip/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/globalip/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/globalip/unassign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.280388 SoftLayer-6.1.7/SoftLayer/CLI/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/authorize_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/cancel_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/create_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/notification_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/notification_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/ready.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/reflash_firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/toggle_ipmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/update_firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/hardware/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.280388 SoftLayer-6.1.7/SoftLayer/CLI/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/share.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/image/share_deny.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.280388 SoftLayer-6.1.7/SoftLayer/CLI/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/licenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/licenses/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/licenses/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/licenses/create_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.284388 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/layer7_policy_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/ns_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/ns_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/loadbal/pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.284388 SoftLayer-6.1.7/SoftLayer/CLI/nas/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/nas/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/nas/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.284388 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/cancel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.284388 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/list_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/object_storage/list_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.284388 SoftLayer-6.1.7/SoftLayer/CLI/order/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/category_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/item_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/package_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/package_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/place_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/preset_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/quote_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/quote_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/quote_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/order/quote_save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.284388 SoftLayer-6.1.7/SoftLayer/CLI/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/report/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/report/dc_closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.288388 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.288388 SoftLayer-6.1.7/SoftLayer/CLI/sshkey/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/sshkey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/sshkey/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/sshkey/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/sshkey/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/sshkey/print.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/sshkey/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.288388 SoftLayer-6.1.7/SoftLayer/CLI/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ssl/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ssl/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ssl/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ssl/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ssl/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/storage_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.288388 SoftLayer-6.1.7/SoftLayer/CLI/subnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/clear_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/edit_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/subnet/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.292389 SoftLayer-6.1.7/SoftLayer/CLI/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/tags/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/tags/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/tags/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/tags/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/tags/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/tags/taggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.292389 SoftLayer-6.1.7/SoftLayer/CLI/ticket/
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/detach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/ticket/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.292389 SoftLayer-6.1.7/SoftLayer/CLI/user/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/device_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/edit_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/edit_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/edit_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/grant_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/remove_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/vpn_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/vpn_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/user/vpn_subnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.296389 SoftLayer-6.1.7/SoftLayer/CLI/virt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/authorize_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/cancel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.296389 SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/create_guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/notification_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/notification_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/os_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.300389 SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/ready.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/virt/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.300389 SoftLayer-6.1.7/SoftLayer/CLI/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vlan/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vlan/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vlan/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vlan/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vlan/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vlan/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.300389 SoftLayer-6.1.7/SoftLayer/CLI/vpn/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.300389 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.300389 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/subnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/subnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/subnet/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/subnet/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.300389 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/translation/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/translation/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/translation/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/decoration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.312389 SoftLayer-6.1.7/SoftLayer/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/BluePages_Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44525 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Billing_Invoice_Item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Billing_Item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Billing_Order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Dns_Domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Dns_Domain_ResourceRecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Email_Subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Event_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Hardware_Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Location_Datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Health_Check_Type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service_Group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Cache_Purge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Firewall_Update_Request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_LBaaS_HealthMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Service_Vpn_Overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress_Global.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Subnet_Rwhois_Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Product_Order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75145 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Product_Package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Provisioning_Hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Resource_Metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Scale_Group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Scale_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Security_Certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Security_Ssh_Key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Software_Component_Password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Ticket_Subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29326 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_Host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup_Rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.316389 SoftLayer-6.1.7/SoftLayer/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/cdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/dedicated_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/ipsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34611 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32323 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/sshkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26132 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42319 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19064 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63471 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/vs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/vs_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/managers/vs_placement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.316389 SoftLayer-6.1.7/SoftLayer/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/shell/cmd_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/shell/cmd_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/shell/cmd_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/shell/completer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/shell/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/shell/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.316389 SoftLayer-6.1.7/SoftLayer/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/testing/xmlrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.320389 SoftLayer-6.1.7/SoftLayer/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/transports/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/transports/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/transports/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/transports/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/transports/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/transports/xmlrpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/SoftLayer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.256388 SoftLayer-6.1.7/SoftLayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-05-03 21:38:24.000000 SoftLayer-6.1.7/SoftLayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-05-03 21:38:24.000000 SoftLayer-6.1.7/SoftLayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:38:24.000000 SoftLayer-6.1.7/SoftLayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 21:38:24.000000 SoftLayer-6.1.7/SoftLayer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:38:24.000000 SoftLayer-6.1.7/SoftLayer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-03 21:38:24.000000 SoftLayer-6.1.7/SoftLayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 21:38:24.000000 SoftLayer-6.1.7/SoftLayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-03 21:38:24.332389 SoftLayer-6.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.252388 SoftLayer-6.1.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.320389 SoftLayer-6.1.7/tests/CLI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/core_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/custom_types_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/environment_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/helper_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.324389 SoftLayer-6.1.7/tests/CLI/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/account_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36346 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/block_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/call_api_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/cdn_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/dedicatedhost_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/dns_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/email_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/event_log_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/file_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/firewall_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/globalip_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/image_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27405 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/ipsec_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/licenses_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/loadbal_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/nas_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/object_storage_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23178 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/order_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/report_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/search_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/securitygroup_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44596 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/server_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/sshkey_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/ssl_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/subnet_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/summary_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/tag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/ticket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17921 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/user_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/vlan_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.324389 SoftLayer-6.1.7/tests/CLI/modules/vs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/vs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/vs/vs_capacity_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33579 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/vs/vs_create_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/vs/vs_placement_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43855 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/CLI/modules/vs/vs_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.328389 SoftLayer-6.1.7/tests/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/account_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41784 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/block_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/cdn_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/dedicated_host_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/dns_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/email_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/event_log_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34792 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/file_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/firewall_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42708 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/hardware_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/image_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16589 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/ipsec_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/loadbal_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/metadata_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28050 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/network_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/object_storage_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40279 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/ordering_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/search_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/sshkey_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/ssl_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/storage_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142912 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/storage_utils_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/tag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/ticket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/user_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.328389 SoftLayer-6.1.7/tests/managers/vs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/vs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/vs/vs_capacity_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/vs/vs_order_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/vs/vs_placement_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45298 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/vs/vs_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/managers/vs/vs_waiting_for_ready_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:24.328389 SoftLayer-6.1.7/tests/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/transports/debug_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/transports/rest_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/transports/transport_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14582 2023-05-03 21:38:15.000000 SoftLayer-6.1.7/tests/transports/xmlrpc_tests.py
```

### Comparing `SoftLayer-6.1.6/LICENSE` & `SoftLayer-6.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/PKG-INFO` & `SoftLayer-6.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SoftLayer
-Version: 6.1.6
+Version: 6.1.7
 Summary: A library for SoftLayer's API
 Home-page: http://github.com/softlayer/softlayer-python
 Author: SoftLayer, Inc., an IBM Company
 Author-email: SLDNDeveloperRelations@wwpdl.vnet.ibm.com
 License: MIT
 Keywords: softlayer,cloud,slcli
 Classifier: Environment :: Console
@@ -122,26 +122,33 @@
 
 is equivalent to 
 
 .. code-block:: bash
 
   $ slcli -vvv --format=json vs list
 
+
 Getting Help
 ------------
 Bugs and feature requests about this library should have a `GitHub issue <https://github.com/softlayer/softlayer-python/issues>`_ opened about them. 
 
 Issues with the Softlayer API itself should be addressed by opening a ticket.
 
 
 Examples
 --------
 
 A curated list of examples on how to use this library can be found at `SLDN <https://softlayer.github.io/python/>`_
 
+Development
+-----------
+To get started working with this project please read the `CONTRIBUTING <https://github.com/softlayer/softlayer-python/blob/master/CONTRIBUTING.md>`_ document.
+
+You can quickly test local changes by running the './slcli' file, which will load the local softlayer-python code instead of the system's softlayer-python codebase.
+
 Debugging
 ---------
 To get the exact API call that this library makes, you can do the following.
 
 For the CLI, just use the -vvv option. If you are using the REST endpoint, this will print out a curl command that you can use, if using XML, this will print the minimal python code to make the request without the softlayer library.
 
 .. code-block:: bash
```

### Comparing `SoftLayer-6.1.6/README.rst` & `SoftLayer-6.1.7/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -94,26 +94,33 @@
 
 is equivalent to 
 
 .. code-block:: bash
 
   $ slcli -vvv --format=json vs list
 
+
 Getting Help
 ------------
 Bugs and feature requests about this library should have a `GitHub issue <https://github.com/softlayer/softlayer-python/issues>`_ opened about them. 
 
 Issues with the Softlayer API itself should be addressed by opening a ticket.
 
 
 Examples
 --------
 
 A curated list of examples on how to use this library can be found at `SLDN <https://softlayer.github.io/python/>`_
 
+Development
+-----------
+To get started working with this project please read the `CONTRIBUTING <https://github.com/softlayer/softlayer-python/blob/master/CONTRIBUTING.md>`_ document.
+
+You can quickly test local changes by running the './slcli' file, which will load the local softlayer-python code instead of the system's softlayer-python codebase.
+
 Debugging
 ---------
 To get the exact API call that this library makes, you can do the following.
 
 For the CLI, just use the -vvv option. If you are using the REST endpoint, this will print out a curl command that you can use, if using XML, this will print the minimal python code to make the request without the softlayer library.
 
 .. code-block:: bash
```

### Comparing `SoftLayer-6.1.6/SoftLayer/API.py` & `SoftLayer-6.1.7/SoftLayer/API.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/bandwidth_pools.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/bandwidth_pools.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/bandwidth_pools_detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/bandwidth_pools_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/billing_items.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/billing_items.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/cancel_item.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/cancel_item.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/event_detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/event_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/events.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/events.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/hook_create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/hook_create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/hook_delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/hook_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/hooks.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/hooks.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/invoice_detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/invoice_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/invoices.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/invoices.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/item_detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/item_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/licenses.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/licenses.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/account/summary.py` & `SoftLayer-6.1.7/SoftLayer/CLI/account/summary.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/access/authorize.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/access/authorize.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/access/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/access/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/access/password.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/access/password.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/access/revoke.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/access/revoke.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/convert.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/convert.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/count.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/count.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/detail.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,22 @@
     block_volume = block_manager.get_block_volume_details(block_volume_id)
     block_volume = utils.NestedDict(block_volume)
 
     table = formatting.KeyValueTable(['Name', 'Value'])
     table.align['Name'] = 'r'
     table.align['Value'] = 'l'
 
+    capacity = '0'
+    if block_volume['capacityGb'] != '':
+        capacity = "%iGB" % block_volume['capacityGb']
     storage_type = block_volume['storageType']['keyName'].split('_').pop(0)
     table.add_row(['ID', block_volume['id']])
     table.add_row(['Username', block_volume['username']])
     table.add_row(['Type', storage_type])
-    table.add_row(['Capacity (GB)', "%iGB" % block_volume['capacityGb']])
+    table.add_row(['Capacity (GB)', capacity])
     table.add_row(['LUN Id', "%s" % block_volume['lunId']])
 
     if block_volume.get('provisionedIops'):
         table.add_row(['IOPs', float(block_volume['provisionedIops'])])
 
     if block_volume.get('storageTierLevel'):
         table.add_row([
```

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/duplicate.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/duplicate.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/duplicate_convert_status.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/duplicate_convert_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/limit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/limit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/lun.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/lun.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/modify.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/modify.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/object_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/object_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/object_storage_detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/object_storage_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/object_storage_permission.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/object_storage_permission.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/options.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/order.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/refresh.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/refresh.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/replication/disaster_recovery_failover.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/replication/disaster_recovery_failover.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/replication/failback.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/replication/failback.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/replication/failover.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/replication/failover.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/replication/locations.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/replication/locations.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/replication/order.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/replication/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/replication/partners.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/replication/partners.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/set_note.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/set_note.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/disable.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/disable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/enable.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/enable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/get_notify_status.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/get_notify_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/order.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/restore.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/restore.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/schedule_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/schedule_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/snapshot/set_notify_status.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/snapshot/set_notify_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/subnets/assign.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/subnets/assign.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/subnets/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/subnets/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/block/subnets/remove.py` & `SoftLayer-6.1.7/SoftLayer/CLI/block/subnets/remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/call_api.py` & `SoftLayer-6.1.7/SoftLayer/CLI/call_api.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/cdn/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/cdn/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/cdn/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/cdn/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/cdn/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/cdn/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/cdn/origin_add.py` & `SoftLayer-6.1.7/SoftLayer/CLI/cdn/origin_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/cdn/origin_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/cdn/origin_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/cdn/origin_remove.py` & `SoftLayer-6.1.7/SoftLayer/CLI/cdn/origin_remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/cdn/purge.py` & `SoftLayer-6.1.7/SoftLayer/CLI/cdn/purge.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Purge cached files from all edge nodes."""
 # :license: MIT, see LICENSE for more details.
+import datetime
 
 import click
 
 import SoftLayer
 from SoftLayer.CLI import environment
 from SoftLayer.CLI import formatting
 
@@ -24,15 +25,16 @@
 
     manager = SoftLayer.CDNManager(env.client)
     result = manager.purge_content(unique_id, path)
 
     table = formatting.Table(['Date', 'Path', 'Saved', 'Status'])
 
     for data in result:
+        date = datetime.datetime.fromtimestamp(int(data['date']))
         table.add_row([
-            data['date'],
+            date,
             data['path'],
             data['saved'],
             data['status']
         ])
 
     env.fout(table)
```

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/columns.py` & `SoftLayer-6.1.7/SoftLayer/CLI/columns.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/command.py` & `SoftLayer-6.1.7/SoftLayer/CLI/command.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/config/__init__.py` & `SoftLayer-6.1.7/SoftLayer/CLI/config/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/config/setup.py` & `SoftLayer-6.1.7/SoftLayer/CLI/config/setup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/core.py` & `SoftLayer-6.1.7/SoftLayer/CLI/core.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/custom_types.py` & `SoftLayer-6.1.7/SoftLayer/CLI/custom_types.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/cancel_guests.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/cancel_guests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/create_options.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dedicatedhost/list_guests.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dedicatedhost/list_guests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dns/record_add.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dns/record_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dns/record_edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dns/record_edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dns/record_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dns/record_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dns/record_remove.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dns/record_remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dns/zone_delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dns/zone_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dns/zone_import.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dns/zone_import.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/dns/zone_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/dns/zone_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/email/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/email/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/email/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/email/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/email/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/email/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/environment.py` & `SoftLayer-6.1.7/SoftLayer/CLI/environment.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/event_log/get.py` & `SoftLayer-6.1.7/SoftLayer/CLI/event_log/get.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Get Event Logs."""
 # :license: MIT, see LICENSE for more details.
 
 import click
 
 import SoftLayer
 from SoftLayer.CLI import environment
-from SoftLayer.CLI import exceptions
+from SoftLayer import exceptions
 from SoftLayer import utils
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
 @click.option('--date-min', '-d',
               help='The earliest date we want to search for event logs in mm/dd/yyyy format.')
 @click.option('--date-max', '-D',
@@ -36,14 +36,15 @@
     columns = ['Event', 'Object', 'Type', 'Date', 'Username']
 
     event_mgr = SoftLayer.EventLogManager(env.client)
     user_mgr = SoftLayer.UserManager(env.client)
     request_filter = event_mgr.build_filter(date_min, date_max, obj_event, obj_id, obj_type, utc_offset)
     logs = event_mgr.get_event_logs(request_filter)
     log_time = "%Y-%m-%dT%H:%M:%S.%f%z"
+    # A list of IDs that we have looked up user information about.
     user_data = {}
 
     if metadata:
         columns.append('Metadata')
 
     row_count = 0
     click.secho(", ".join(columns))
@@ -55,17 +56,19 @@
         user = log['userType']
         label = log.get('label', '')
         if user == "CUSTOMER":
             username = user_data.get(log['userId'])
             if username is None:
                 try:
                     username = user_mgr.get_user(log['userId'], "mask[username]")['username']
-                    user_data[log['userId']] = username
+                # Some users might not be able to access information about this specific userId
                 except exceptions.SoftLayerAPIError:
                     username = log['userId']
+            # This keeps track of any users we asked the API about, so we can make fewer calls.
+            user_data[log['userId']] = username
             user = username
 
         if metadata:
             metadata_data = log['metaData'].strip("\n\t")
 
             click.secho("'{0}','{1}','{2}','{3}','{4}','{5}'".format(
                 log['eventName'],
```

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/event_log/types.py` & `SoftLayer-6.1.7/SoftLayer/CLI/event_log/types.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/exceptions.py` & `SoftLayer-6.1.7/SoftLayer/CLI/exceptions.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/access/authorize.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/access/authorize.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/access/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/access/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/access/revoke.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/access/revoke.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/convert.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/convert.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/count.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/count.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/detail.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 import SoftLayer
 from SoftLayer.CLI import environment
 from SoftLayer.CLI import formatting
 from SoftLayer.CLI import helpers
 from SoftLayer import utils
 
 
+def get_capacity(file_volume):
+    """Get the capacity Gb with validate the data"""
+    capacity = '0'
+    if file_volume['capacityGb'] != '':
+        capacity = "%iGB" % file_volume['capacityGb']
+    return capacity
+
+
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
 @click.argument('volume_id')
 @environment.pass_env
 def cli(env, volume_id):
     """Display details for a specified volume."""
     file_manager = SoftLayer.FileStorageManager(env.client)
     file_volume_id = helpers.resolve_id(file_manager.resolve_ids, volume_id, 'File Storage')
@@ -23,15 +31,15 @@
     table.align['Name'] = 'r'
     table.align['Value'] = 'l'
 
     storage_type = file_volume['storageType']['keyName'].split('_').pop(0)
     table.add_row(['ID', file_volume['id']])
     table.add_row(['Username', file_volume['username']])
     table.add_row(['Type', storage_type])
-    table.add_row(['Capacity (GB)', "%iGB" % file_volume['capacityGb']])
+    table.add_row(['Capacity (GB)', get_capacity(file_volume)])
 
     used_space = int(file_volume['bytesUsed']) \
         if file_volume['bytesUsed'] else 0
     if used_space < (1 << 10):
         table.add_row(['Used Space', "%dB" % used_space])
     elif used_space < (1 << 20):
         table.add_row(['Used Space', "%dKB" % (used_space / (1 << 10))])
```

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/duplicate.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/duplicate.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/duplicate_convert_status.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/duplicate_convert_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/limit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/limit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/modify.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/modify.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/options.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/order.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/refresh.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/refresh.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/replication/disaster_recovery_failover.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/replication/disaster_recovery_failover.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/replication/failback.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/replication/failback.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/replication/failover.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/replication/failover.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/replication/locations.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/replication/locations.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/replication/order.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/replication/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/replication/partners.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/replication/partners.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/set_note.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/set_note.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/disable.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/disable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/enable.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/enable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/get_notify_status.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/get_notify_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/order.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/restore.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/restore.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/schedule_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/schedule_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/file/snapshot/set_notify_status.py` & `SoftLayer-6.1.7/SoftLayer/CLI/file/snapshot/set_notify_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/firewall/add.py` & `SoftLayer-6.1.7/SoftLayer/CLI/firewall/add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/firewall/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/firewall/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/firewall/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/firewall/detail.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from SoftLayer.CLI import firewall
 from SoftLayer.CLI import formatting
 from SoftLayer import utils
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
 @click.argument('identifier')
-@click.option('--credentials', type=click.BOOL,
+@click.option('--password', is_flag=True,
               help="Display FortiGate username and FortiGate password to multi vlans.")
 @environment.pass_env
-def cli(env, identifier, credentials):
+def cli(env, identifier, password):
     """Detail firewall.
 
     EXAMPLES:
 
         slcli firewall detail vs:12345
 
         slcli firewall detail --credentials true multiVlan:456789
@@ -59,15 +59,15 @@
             table.add_row(['public ip', utils.lookup(_firewall, 'networkGateway', 'publicIpAddress', 'ipAddress')])
             table.add_row(['private ip', utils.lookup(_firewall, 'networkGateway', 'privateIpAddress', 'ipAddress')])
             table.add_row(['public  ipv6', utils.lookup(_firewall, 'networkGateway', 'publicIpv6Address', 'ipAddress')])
             table.add_row(['public vlan', utils.lookup(_firewall, 'networkGateway', 'publicVlan', 'vlanNumber')])
             table.add_row(['private vlan', utils.lookup(_firewall, 'networkGateway', 'privateVlan', 'vlanNumber')])
             table.add_row(['type', _firewall.get('firewallType')])
 
-            if credentials:
+            if password:
                 table.add_row(['fortiGate username', utils.lookup(_firewall, 'managementCredentials', 'username')])
                 table.add_row(['fortiGate password', utils.lookup(_firewall, 'managementCredentials', 'password')])
 
             rules = mgr.get_dedicated_fwl_rules(firewall_id)
             if len(rules) != 0:
                 table.add_row(['rules', get_rules_table(rules)])
             else:
```

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/firewall/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/firewall/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/firewall/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/firewall/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/firewall/monitoring.py` & `SoftLayer-6.1.7/SoftLayer/CLI/firewall/monitoring.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/formatting.py` & `SoftLayer-6.1.7/SoftLayer/CLI/formatting.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/globalip/assign.py` & `SoftLayer-6.1.7/SoftLayer/CLI/globalip/assign.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/globalip/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/globalip/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/globalip/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/globalip/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/globalip/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/globalip/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/globalip/unassign.py` & `SoftLayer-6.1.7/SoftLayer/CLI/globalip/unassign.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/authorize_storage.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/authorize_storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/bandwidth.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/bandwidth.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/billing.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/billing.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/cancel_reasons.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/cancel_reasons.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/create_credential.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/create_credential.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/create_options.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/credentials.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/credentials.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/dns.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/dns.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/monitoring.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/monitoring.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/notification_add.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/notification_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/notification_delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/notification_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/notifications.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/notifications.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/power.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/power.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/ready.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/ready.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/reflash_firmware.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/reflash_firmware.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/reload.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/reload.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/sensor.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/sensor.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/storage.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/toggle_ipmi.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/toggle_ipmi.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/update_firmware.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/update_firmware.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/hardware/upgrade.py` & `SoftLayer-6.1.7/SoftLayer/CLI/hardware/upgrade.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/helpers.py` & `SoftLayer-6.1.7/SoftLayer/CLI/helpers.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/image/__init__.py` & `SoftLayer-6.1.7/SoftLayer/CLI/image/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/image/datacenter.py` & `SoftLayer-6.1.7/SoftLayer/CLI/image/datacenter.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/image/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/image/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/image/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/image/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/image/export.py` & `SoftLayer-6.1.7/SoftLayer/CLI/image/export.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/image/import.py` & `SoftLayer-6.1.7/SoftLayer/CLI/image/import.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/image/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/image/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/image/share.py` & `SoftLayer-6.1.7/SoftLayer/CLI/image/share.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/image/share_deny.py` & `SoftLayer-6.1.7/SoftLayer/CLI/image/share_deny.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/licenses/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/licenses/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/licenses/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/licenses/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/licenses/create_options.py` & `SoftLayer-6.1.7/SoftLayer/CLI/licenses/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/loadbal/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/loadbal/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/loadbal/health.py` & `SoftLayer-6.1.7/SoftLayer/CLI/loadbal/health.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/loadbal/layer7_policy_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/loadbal/layer7_policy_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/loadbal/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/loadbal/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/loadbal/members.py` & `SoftLayer-6.1.7/SoftLayer/CLI/loadbal/members.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/loadbal/ns_detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/loadbal/ns_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/loadbal/ns_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/loadbal/ns_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/loadbal/order.py` & `SoftLayer-6.1.7/SoftLayer/CLI/loadbal/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/loadbal/pools.py` & `SoftLayer-6.1.7/SoftLayer/CLI/loadbal/pools.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/metadata.py` & `SoftLayer-6.1.7/SoftLayer/CLI/metadata.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/nas/credentials.py` & `SoftLayer-6.1.7/SoftLayer/CLI/nas/credentials.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/nas/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/nas/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/__init__.py` & `SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/limit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/limit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/object_storage/credential/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/object_storage/credential/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/object_storage/list_accounts.py` & `SoftLayer-6.1.7/SoftLayer/CLI/object_storage/list_accounts.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/object_storage/list_endpoints.py` & `SoftLayer-6.1.7/SoftLayer/CLI/object_storage/list_endpoints.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/category_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/category_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/item_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/item_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/lookup.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/lookup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/package_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/package_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/package_locations.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/package_locations.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/place.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/place.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/place_quote.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/place_quote.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/preset_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/preset_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/quote.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/quote.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/quote_detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/quote_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/quote_list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/quote_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/order/quote_save.py` & `SoftLayer-6.1.7/SoftLayer/CLI/order/quote_save.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/report/bandwidth.py` & `SoftLayer-6.1.7/SoftLayer/CLI/report/bandwidth.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/report/dc_closures.py` & `SoftLayer-6.1.7/SoftLayer/CLI/report/dc_closures.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/routes.py` & `SoftLayer-6.1.7/SoftLayer/CLI/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,16 @@
     ('cdn:detail', 'SoftLayer.CLI.cdn.detail:cli'),
     ('cdn:edit', 'SoftLayer.CLI.cdn.edit:cli'),
     ('cdn:list', 'SoftLayer.CLI.cdn.list:cli'),
     ('cdn:origin-add', 'SoftLayer.CLI.cdn.origin_add:cli'),
     ('cdn:origin-list', 'SoftLayer.CLI.cdn.origin_list:cli'),
     ('cdn:origin-remove', 'SoftLayer.CLI.cdn.origin_remove:cli'),
     ('cdn:purge', 'SoftLayer.CLI.cdn.purge:cli'),
+    ('cdn:delete', 'SoftLayer.CLI.cdn.delete:cli'),
+    ('cdn:create', 'SoftLayer.CLI.cdn.create:cli'),
 
     ('config', 'SoftLayer.CLI.config'),
     ('config:setup', 'SoftLayer.CLI.config.setup:cli'),
     ('config:show', 'SoftLayer.CLI.config.show:cli'),
     ('setup', 'SoftLayer.CLI.config.setup:cli'),
 
     ('dns', 'SoftLayer.CLI.dns'),
@@ -257,25 +259,27 @@
     ('licenses:cancel', 'SoftLayer.CLI.licenses.cancel:cli'),
 
     ('object-storage', 'SoftLayer.CLI.object_storage'),
 
     ('object-storage:accounts', 'SoftLayer.CLI.object_storage.list_accounts:cli'),
     ('object-storage:endpoints', 'SoftLayer.CLI.object_storage.list_endpoints:cli'),
     ('object-storage:credential', 'SoftLayer.CLI.object_storage.credential:cli'),
+    ('object-storage:cancel', 'SoftLayer.CLI.object_storage.cancel:cli'),
 
     ('order', 'SoftLayer.CLI.order'),
     ('order:category-list', 'SoftLayer.CLI.order.category_list:cli'),
     ('order:item-list', 'SoftLayer.CLI.order.item_list:cli'),
     ('order:package-list', 'SoftLayer.CLI.order.package_list:cli'),
     ('order:place', 'SoftLayer.CLI.order.place:cli'),
     ('order:preset-list', 'SoftLayer.CLI.order.preset_list:cli'),
     ('order:package-locations', 'SoftLayer.CLI.order.package_locations:cli'),
     ('order:place-quote', 'SoftLayer.CLI.order.place_quote:cli'),
     ('order:quote-list', 'SoftLayer.CLI.order.quote_list:cli'),
     ('order:quote-detail', 'SoftLayer.CLI.order.quote_detail:cli'),
+    ('order:quote-delete', 'SoftLayer.CLI.order.quote_delete:cli'),
     ('order:quote-save', 'SoftLayer.CLI.order.quote_save:cli'),
     ('order:quote', 'SoftLayer.CLI.order.quote:cli'),
     ('order:lookup', 'SoftLayer.CLI.order.lookup:cli'),
 
     ('hardware', 'SoftLayer.CLI.hardware'),
     ('hardware:bandwidth', 'SoftLayer.CLI.hardware.bandwidth:cli'),
     ('hardware:cancel', 'SoftLayer.CLI.hardware.cancel:cli'),
@@ -381,14 +385,15 @@
     ('user:create', 'SoftLayer.CLI.user.create:cli'),
     ('user:delete', 'SoftLayer.CLI.user.delete:cli'),
     ('user:device-access', 'SoftLayer.CLI.user.device_access:cli'),
     ('user:vpn-manual', 'SoftLayer.CLI.user.vpn_manual:cli'),
     ('user:vpn-subnet', 'SoftLayer.CLI.user.vpn_subnet:cli'),
     ('user:remove-access', 'SoftLayer.CLI.user.remove_access:cli'),
     ('user:grant-access', 'SoftLayer.CLI.user.grant_access:cli'),
+    ('user:vpn-password', 'SoftLayer.CLI.user.vpn_password:cli'),
 
     ('vlan', 'SoftLayer.CLI.vlan'),
     ('vlan:create', 'SoftLayer.CLI.vlan.create:cli'),
     ('vlan:create-options', 'SoftLayer.CLI.vlan.create_options:cli'),
     ('vlan:detail', 'SoftLayer.CLI.vlan.detail:cli'),
     ('vlan:edit', 'SoftLayer.CLI.vlan.edit:cli'),
     ('vlan:list', 'SoftLayer.CLI.vlan.list:cli'),
```

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/search.py` & `SoftLayer-6.1.7/SoftLayer/CLI/search.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/event_log.py` & `SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/event_log.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/interface.py` & `SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/interface.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/securitygroup/rule.py` & `SoftLayer-6.1.7/SoftLayer/CLI/securitygroup/rule.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/sshkey/add.py` & `SoftLayer-6.1.7/SoftLayer/CLI/sshkey/add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/sshkey/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/sshkey/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/sshkey/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/sshkey/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/sshkey/print.py` & `SoftLayer-6.1.7/SoftLayer/CLI/sshkey/print.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/sshkey/remove.py` & `SoftLayer-6.1.7/SoftLayer/CLI/sshkey/remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ssl/add.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ssl/add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ssl/download.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ssl/download.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ssl/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ssl/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ssl/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ssl/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ssl/remove.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ssl/remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/storage_utils.py` & `SoftLayer-6.1.7/SoftLayer/CLI/storage_utils.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/subnet/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/subnet/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/subnet/clear_route.py` & `SoftLayer-6.1.7/SoftLayer/CLI/subnet/clear_route.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/subnet/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/subnet/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/subnet/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/subnet/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/subnet/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/subnet/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/subnet/edit_ip.py` & `SoftLayer-6.1.7/SoftLayer/CLI/subnet/edit_ip.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/subnet/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/subnet/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/subnet/lookup.py` & `SoftLayer-6.1.7/SoftLayer/CLI/subnet/lookup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/subnet/route.py` & `SoftLayer-6.1.7/SoftLayer/CLI/subnet/route.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/summary.py` & `SoftLayer-6.1.7/SoftLayer/CLI/summary.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/tags/cleanup.py` & `SoftLayer-6.1.7/SoftLayer/CLI/tags/cleanup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/tags/delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/tags/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/tags/details.py` & `SoftLayer-6.1.7/SoftLayer/CLI/tags/details.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/tags/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/tags/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/tags/set.py` & `SoftLayer-6.1.7/SoftLayer/CLI/tags/set.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/tags/taggable.py` & `SoftLayer-6.1.7/SoftLayer/CLI/tags/taggable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/template.py` & `SoftLayer-6.1.7/SoftLayer/CLI/template.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/__init__.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/attach.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/attach.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/detach.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/detach.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/subjects.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/subjects.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/summary.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/summary.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/update.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/update.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/ticket/upload.py` & `SoftLayer-6.1.7/SoftLayer/CLI/ticket/upload.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/detail.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,17 +61,22 @@
 
     table = formatting.KeyValueTable(['Title', 'Basic Information'])
     table.align['Title'] = 'r'
     table.align['Basic Information'] = 'l'
 
     table.add_row(['Id', user.get('id', '-')])
     table.add_row(['Username', user.get('username', '-')])
-    if keys:
-        for key in user.get('apiAuthenticationKeys'):
+    keys_array = user.get('apiAuthenticationKeys')
+    if keys and len(keys_array) != 0:
+        for key in keys_array:
             table.add_row(['APIKEY', key.get('authenticationKey')])
+    elif keys_array is not None and len(keys_array) != 0:
+        table.add_row(['APIKEY', 'Yes'])
+    else:
+        table.add_row(['APIKEY', 'No'])
     table.add_row(['Name', "%s %s" % (user.get('firstName', '-'), user.get('lastName', '-'))])
     table.add_row(['Email', user.get('email')])
     table.add_row(['OpenID', user.get('openIdConnectUserName')])
     address = "%s %s %s %s %s %s" % (
         user.get('address1'), user.get('address2'), user.get('city'), user.get('state'),
         user.get('country'), user.get('postalCode'))
     table.add_row(['Address', address])
```

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/device_access.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/device_access.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/edit_details.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/edit_details.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/edit_notifications.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/edit_notifications.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/edit_permissions.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/edit_permissions.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/grant_access.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/grant_access.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/notifications.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/notifications.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/permissions.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/permissions.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/remove_access.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/remove_access.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/vpn_manual.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/vpn_manual.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/user/vpn_subnet.py` & `SoftLayer-6.1.7/SoftLayer/CLI/user/vpn_subnet.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/__init__.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/access.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/access.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/authorize_storage.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/authorize_storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/bandwidth.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/bandwidth.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/billing.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/billing.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/__init__.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/create_guest.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/create_guest.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/create_options.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/capacity/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/capacity/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/capture.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/capture.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/create_options.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/credentials.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/credentials.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/dns.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/dns.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/migrate.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/migrate.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/monitoring.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/monitoring.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/notification_add.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/notification_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/notification_delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/notification_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/notifications.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/notifications.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/os_available.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/os_available.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/__init__.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/create_options.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/delete.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/placementgroup/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/placementgroup/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/power.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/power.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/ready.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/ready.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/reload.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/reload.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/storage.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/upgrade.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/upgrade.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/virt/usage.py` & `SoftLayer-6.1.7/SoftLayer/CLI/virt/usage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vlan/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vlan/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vlan/create.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vlan/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vlan/create_options.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vlan/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vlan/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vlan/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vlan/edit.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vlan/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vlan/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vlan/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/cancel.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/configure.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/configure.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/detail.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/list.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/order.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/subnet/add.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/subnet/add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/subnet/remove.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/subnet/remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/translation/add.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/translation/add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/translation/remove.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/translation/remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/translation/update.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/translation/update.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/CLI/vpn/ipsec/update.py` & `SoftLayer-6.1.7/SoftLayer/CLI/vpn/ipsec/update.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/__init__.py` & `SoftLayer-6.1.7/SoftLayer/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/auth.py` & `SoftLayer-6.1.7/SoftLayer/auth.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/config.py` & `SoftLayer-6.1.7/SoftLayer/config.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/consts.py` & `SoftLayer-6.1.7/SoftLayer/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     SoftLayer.consts
     ~~~~~~~~~~~~~~~~
     Contains constants used throughout the library
 
     :license: MIT, see LICENSE for more details.
 """
-VERSION = 'v6.1.6'
+VERSION = 'v6.1.7'
 API_PUBLIC_ENDPOINT = 'https://api.softlayer.com/xmlrpc/v3.1/'
 API_PRIVATE_ENDPOINT = 'https://api.service.softlayer.com/xmlrpc/v3.1/'
 API_PUBLIC_ENDPOINT_REST = 'https://api.softlayer.com/rest/v3.1/'
 API_PRIVATE_ENDPOINT_REST = 'https://api.service.softlayer.com/rest/v3.1/'
 USER_AGENT = "softlayer-python/%s" % VERSION
 CONFIG_FILE = "~/.softlayer"
```

### Comparing `SoftLayer-6.1.6/SoftLayer/decoration.py` & `SoftLayer-6.1.7/SoftLayer/decoration.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/exceptions.py` & `SoftLayer-6.1.7/SoftLayer/exceptions.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Account.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1476,7 +1476,28 @@
     "uri": "http://test.com"
 },
     {
         "id": 123654,
         "name": "GettestProv12345",
         "uri": "http://test.com"
     }]
+
+getUpgradeRequests = [{
+    "createDate": "2023-03-01T19:39:51-06:00",
+    "id": 3237486,
+    "maintenanceStartTimeUtc": "2023-03-01T19:39:51-06:00",
+    "modifyDate": "2023-03-01T19:39:53-06:00",
+    "orderId": 103127604,
+    "statusId": 3,
+    "ticketId": 152510472,
+    "userId": 167758
+},
+    {
+        "createDate": "2023-02-27T19:41:26-06:00",
+        "id": 3229998,
+        "maintenanceStartTimeUtc": "2023-02-27T19:41:26-06:00",
+        "modifyDate": "2023-02-27T19:41:29-06:00",
+        "orderId": 103029352,
+        "statusId": 3,
+        "ticketId": 152452042,
+        "userId": 167758
+    }]
```

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Billing_Item.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Billing_Item.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Billing_Order.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Billing_Order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,7 +100,8 @@
                 'setupFee': '0',
             }
         ]
     }
 }
 
 saveQuote = getObject
+deleteQuote = getObject
```

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Dns_Domain.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Dns_Domain.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Event_Log.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Event_Log.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Hardware.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Hardware.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Hardware_Server.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Hardware_Server.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Pod.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Pod.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Storage.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Subnet.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Subnet.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Vlan.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Vlan.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Product_Order.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Product_Order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Product_Package.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Product_Package.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Scale_Group.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Scale_Group.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Scale_Policy.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Scale_Policy.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Search.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Search.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Security_Certificate.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Security_Certificate.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Tag.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Tag.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Ticket.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Ticket.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Customer.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Customer.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 updateVpnUser = True
 removeDedicatedHostAccess = True
 removeHardwareAccess = True
 removeVirtualGuestAccess = True
 addDedicatedHostAccess = True
 addHardwareAccess = True
 addVirtualGuestAccess = True
+updateVpnPassword = True
 
 getHardware = [{
         "domain": "testedit.com",
         "fullyQualifiedDomainName": "test.testedit.com",
         "hardwareStatusId": 5,
         "hostname": "test",
         "id": 1403539,
```

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_Host.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_Host.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py` & `SoftLayer-6.1.7/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/__init__.py` & `SoftLayer-6.1.7/SoftLayer/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/account.py` & `SoftLayer-6.1.7/SoftLayer/managers/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,7 +412,11 @@
         """Delete a provisioning script
 
         param: identifier provisioning script identifier
 
         Returns: boolean
         """
         return self.client.call("SoftLayer_Provisioning_Hook", "deleteObject", id=identifier)
+
+    def get_account_upgrade_orders(self, limit=100):
+        """Gets upgrade order list"""
+        return self.client.call('SoftLayer_Account', 'getUpgradeRequests', limit=limit)
```

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/block.py` & `SoftLayer-6.1.7/SoftLayer/managers/block.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/cdn.py` & `SoftLayer-6.1.7/SoftLayer/managers/cdn.py`

 * *Files 16% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     def purge_content(self, unique_id, path):
         """Purges a URL or path from the CDN.
 
         :param str unique_id: The unique ID associated with the CDN.
         :param str path: A string of url or path that should be purged.
         :returns: A Container_Network_CdnMarketplace_Configuration_Cache_Purge array object
         """
-
+        path = f"/{path}"
         return self.cdn_purge.createPurge(unique_id, path)
 
     def get_usage_metrics(self, unique_id, history=30, frequency="aggregate"):
         """Retrieves the cdn usage metrics.
 
         It uses the 'days' argument if start_date and end_date are None.
 
@@ -265,7 +265,75 @@
         """
         if 'description' not in cache:
             raise SoftLayer.SoftLayerError('Please add a description to be able to update the'
                                            ' cache.')
         cache_result = '%s: %s' % (cache_type, cache['description'])
 
         return cache_result
+
+    def delete_cdn(self, unique_id):
+        """Delete CDN domain mapping for a particular customer.
+
+        :param str unique_id: The unique ID associated with the CDN.
+        :returns: The cdn that is being deleted.
+        """
+
+        return self.cdn_configuration.deleteDomainMapping(unique_id)
+
+    def create_cdn(self, hostname=None, origin=None, origin_type=None, http=None, https=None, bucket_name=None,
+                   cname=None, header=None, path=None, ssl=None):
+        """Create CDN domain mapping for a particular customer.
+
+        :param str hostname: The unique ID associated with the CDN.
+        :param str origin: ip address or hostname if origin_type=server, API endpoint for
+                           your S3 object storage if origin_type=storage
+        :param str origin_type: it can be 'server' or 'storage' types.
+        :param int http: http port
+        :param int https: https port
+        :param str bucket_name: name of the available resource
+        :param str cname: globally unique subdomain
+        :param str header: the edge server uses the host header to communicate with the origin.
+                            It defaults to hostname. (optional)
+        :param str path: relative path to the domain provided, e.g. "/articles/video"
+        :param str ssl: ssl certificate
+        :returns: The cdn that is being created.
+        """
+        types = {'server': 'HOST_SERVER', 'storage': 'OBJECT_STORAGE'}
+        ssl_certificate = {'wilcard': 'WILDCARD_CERT', 'dvSan': 'SHARED_SAN_CERT'}
+
+        new_origin = {
+            'domain': hostname,
+            'origin': origin,
+            'originType': types.get(origin_type),
+            'vendorName': 'akamai',
+        }
+
+        protocol = ''
+        if http:
+            protocol = 'HTTP'
+            new_origin['httpPort'] = http
+        if https:
+            protocol = 'HTTPS'
+            new_origin['httpsPort'] = https
+            new_origin['certificateType'] = ssl_certificate.get(ssl)
+        if http and https:
+            protocol = 'HTTP_AND_HTTPS'
+
+        new_origin['protocol'] = protocol
+
+        if types.get(origin_type) == 'OBJECT_STORAGE':
+            new_origin['bucketName'] = bucket_name
+            new_origin['header'] = header
+
+        if cname:
+            new_origin['cname'] = cname + '.cdn.appdomain.cloud'
+
+        if header:
+            new_origin['header'] = header
+
+        if path:
+            new_origin['path'] = '/' + path
+
+        origin = self.cdn_configuration.createDomainMapping(new_origin)
+
+        # The method createOriginPath() returns an array but there is only 1 object
+        return origin[0]
```

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/dedicated_host.py` & `SoftLayer-6.1.7/SoftLayer/managers/dedicated_host.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/dns.py` & `SoftLayer-6.1.7/SoftLayer/managers/dns.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/email.py` & `SoftLayer-6.1.7/SoftLayer/managers/email.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/event_log.py` & `SoftLayer-6.1.7/SoftLayer/managers/event_log.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/file.py` & `SoftLayer-6.1.7/SoftLayer/managers/file.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/firewall.py` & `SoftLayer-6.1.7/SoftLayer/managers/firewall.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/hardware.py` & `SoftLayer-6.1.7/SoftLayer/managers/hardware.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/image.py` & `SoftLayer-6.1.7/SoftLayer/managers/image.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/ipsec.py` & `SoftLayer-6.1.7/SoftLayer/managers/ipsec.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/license.py` & `SoftLayer-6.1.7/SoftLayer/managers/license.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/licenses.py` & `SoftLayer-6.1.7/SoftLayer/managers/licenses.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/load_balancer.py` & `SoftLayer-6.1.7/SoftLayer/managers/load_balancer.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/metadata.py` & `SoftLayer-6.1.7/SoftLayer/managers/metadata.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/network.py` & `SoftLayer-6.1.7/SoftLayer/managers/network.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/object_storage.py` & `SoftLayer-6.1.7/SoftLayer/managers/object_storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/ordering.py` & `SoftLayer-6.1.7/SoftLayer/managers/ordering.py`

 * *Files 1% similar despite different names*

```diff
@@ -733,7 +733,15 @@
 
         :param int package_id: The package for which to get the items.
         """
         _filter = ''
         if location:
             _filter = {"regions": {"location": {"location": {"name": {"operation": location}}}}}
         return self.client.call('SoftLayer_Product_Package', 'getRegions', id=package_id, filter=_filter)
+
+    def delete_quote(self, quote_id):
+        """Delete the quote of an order.
+
+        :param quote_id: ID number of target quote
+        """
+
+        return self.client['SoftLayer_Billing_Order_Quote'].deleteQuote(id=quote_id)
```

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/search.py` & `SoftLayer-6.1.7/SoftLayer/managers/search.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/sshkey.py` & `SoftLayer-6.1.7/SoftLayer/managers/sshkey.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/ssl.py` & `SoftLayer-6.1.7/SoftLayer/managers/ssl.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/storage.py` & `SoftLayer-6.1.7/SoftLayer/managers/storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/storage_utils.py` & `SoftLayer-6.1.7/SoftLayer/managers/storage_utils.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/tags.py` & `SoftLayer-6.1.7/SoftLayer/managers/tags.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/ticket.py` & `SoftLayer-6.1.7/SoftLayer/managers/ticket.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/user.py` & `SoftLayer-6.1.7/SoftLayer/managers/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,13 +472,23 @@
         """User virtual guest list.
 
         :param int user_id:
         :return: List virtual guest relate to user
         """
         return self.user_service.getVirtualGuests(id=user_id)
 
+    def update_vpn_password(self, user_id, password):
+        """Update a user's VPN password.
+
+        :param int user_id:
+        :param string password:
+
+        :returns: true
+        """
+        return self.user_service.updateVpnPassword(password, id=user_id)
+
 
 def _keyname_search(haystack, needle):
     for item in haystack:
         if item.get('keyName') == needle:
             return True
     return False
```

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/vs.py` & `SoftLayer-6.1.7/SoftLayer/managers/vs.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/vs_capacity.py` & `SoftLayer-6.1.7/SoftLayer/managers/vs_capacity.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/managers/vs_placement.py` & `SoftLayer-6.1.7/SoftLayer/managers/vs_placement.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/shell/cmd_help.py` & `SoftLayer-6.1.7/SoftLayer/shell/cmd_help.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/shell/completer.py` & `SoftLayer-6.1.7/SoftLayer/shell/completer.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/shell/core.py` & `SoftLayer-6.1.7/SoftLayer/shell/core.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/testing/__init__.py` & `SoftLayer-6.1.7/SoftLayer/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/testing/xmlrpc.py` & `SoftLayer-6.1.7/SoftLayer/testing/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/transports/__init__.py` & `SoftLayer-6.1.7/SoftLayer/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/transports/debug.py` & `SoftLayer-6.1.7/SoftLayer/transports/debug.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/transports/fixture.py` & `SoftLayer-6.1.7/SoftLayer/transports/fixture.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/transports/rest.py` & `SoftLayer-6.1.7/SoftLayer/transports/rest.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/transports/timing.py` & `SoftLayer-6.1.7/SoftLayer/transports/timing.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/transports/transport.py` & `SoftLayer-6.1.7/SoftLayer/transports/transport.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/transports/xmlrpc.py` & `SoftLayer-6.1.7/SoftLayer/transports/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer/utils.py` & `SoftLayer-6.1.7/SoftLayer/utils.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/SoftLayer.egg-info/PKG-INFO` & `SoftLayer-6.1.7/SoftLayer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SoftLayer
-Version: 6.1.6
+Version: 6.1.7
 Summary: A library for SoftLayer's API
 Home-page: http://github.com/softlayer/softlayer-python
 Author: SoftLayer, Inc., an IBM Company
 Author-email: SLDNDeveloperRelations@wwpdl.vnet.ibm.com
 License: MIT
 Keywords: softlayer,cloud,slcli
 Classifier: Environment :: Console
@@ -122,26 +122,33 @@
 
 is equivalent to 
 
 .. code-block:: bash
 
   $ slcli -vvv --format=json vs list
 
+
 Getting Help
 ------------
 Bugs and feature requests about this library should have a `GitHub issue <https://github.com/softlayer/softlayer-python/issues>`_ opened about them. 
 
 Issues with the Softlayer API itself should be addressed by opening a ticket.
 
 
 Examples
 --------
 
 A curated list of examples on how to use this library can be found at `SLDN <https://softlayer.github.io/python/>`_
 
+Development
+-----------
+To get started working with this project please read the `CONTRIBUTING <https://github.com/softlayer/softlayer-python/blob/master/CONTRIBUTING.md>`_ document.
+
+You can quickly test local changes by running the './slcli' file, which will load the local softlayer-python code instead of the system's softlayer-python codebase.
+
 Debugging
 ---------
 To get the exact API call that this library makes, you can do the following.
 
 For the CLI, just use the -vvv option. If you are using the REST endpoint, this will print out a curl command that you can use, if using XML, this will print the minimal python code to make the request without the softlayer library.
 
 .. code-block:: bash
```

### Comparing `SoftLayer-6.1.6/SoftLayer.egg-info/SOURCES.txt` & `SoftLayer-6.1.7/SoftLayer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,16 @@
 SoftLayer/CLI/block/snapshot/schedule_list.py
 SoftLayer/CLI/block/snapshot/set_notify_status.py
 SoftLayer/CLI/block/subnets/__init__.py
 SoftLayer/CLI/block/subnets/assign.py
 SoftLayer/CLI/block/subnets/list.py
 SoftLayer/CLI/block/subnets/remove.py
 SoftLayer/CLI/cdn/__init__.py
+SoftLayer/CLI/cdn/create.py
+SoftLayer/CLI/cdn/delete.py
 SoftLayer/CLI/cdn/detail.py
 SoftLayer/CLI/cdn/edit.py
 SoftLayer/CLI/cdn/list.py
 SoftLayer/CLI/cdn/origin_add.py
 SoftLayer/CLI/cdn/origin_list.py
 SoftLayer/CLI/cdn/origin_remove.py
 SoftLayer/CLI/cdn/purge.py
@@ -233,14 +235,15 @@
 SoftLayer/CLI/loadbal/ns_list.py
 SoftLayer/CLI/loadbal/order.py
 SoftLayer/CLI/loadbal/pools.py
 SoftLayer/CLI/nas/__init__.py
 SoftLayer/CLI/nas/credentials.py
 SoftLayer/CLI/nas/list.py
 SoftLayer/CLI/object_storage/__init__.py
+SoftLayer/CLI/object_storage/cancel.py
 SoftLayer/CLI/object_storage/list_accounts.py
 SoftLayer/CLI/object_storage/list_endpoints.py
 SoftLayer/CLI/object_storage/credential/__init__.py
 SoftLayer/CLI/object_storage/credential/create.py
 SoftLayer/CLI/object_storage/credential/delete.py
 SoftLayer/CLI/object_storage/credential/limit.py
 SoftLayer/CLI/object_storage/credential/list.py
@@ -250,14 +253,15 @@
 SoftLayer/CLI/order/lookup.py
 SoftLayer/CLI/order/package_list.py
 SoftLayer/CLI/order/package_locations.py
 SoftLayer/CLI/order/place.py
 SoftLayer/CLI/order/place_quote.py
 SoftLayer/CLI/order/preset_list.py
 SoftLayer/CLI/order/quote.py
+SoftLayer/CLI/order/quote_delete.py
 SoftLayer/CLI/order/quote_detail.py
 SoftLayer/CLI/order/quote_list.py
 SoftLayer/CLI/order/quote_save.py
 SoftLayer/CLI/report/__init__.py
 SoftLayer/CLI/report/bandwidth.py
 SoftLayer/CLI/report/dc_closures.py
 SoftLayer/CLI/securitygroup/__init__.py
@@ -318,14 +322,15 @@
 SoftLayer/CLI/user/edit_permissions.py
 SoftLayer/CLI/user/grant_access.py
 SoftLayer/CLI/user/list.py
 SoftLayer/CLI/user/notifications.py
 SoftLayer/CLI/user/permissions.py
 SoftLayer/CLI/user/remove_access.py
 SoftLayer/CLI/user/vpn_manual.py
+SoftLayer/CLI/user/vpn_password.py
 SoftLayer/CLI/user/vpn_subnet.py
 SoftLayer/CLI/virt/__init__.py
 SoftLayer/CLI/virt/access.py
 SoftLayer/CLI/virt/authorize_storage.py
 SoftLayer/CLI/virt/bandwidth.py
 SoftLayer/CLI/virt/billing.py
 SoftLayer/CLI/virt/cancel.py
```

### Comparing `SoftLayer-6.1.6/setup.py` & `SoftLayer-6.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with codecs.open('README.rst', 'r', 'utf-8') as readme_file:
         LONG_DESCRIPTION = readme_file.read()
 else:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name='SoftLayer',
-    version='6.1.6',
+    version='6.1.7',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
     author='SoftLayer, Inc., an IBM Company',
     author_email='SLDNDeveloperRelations@wwpdl.vnet.ibm.com',
     packages=find_packages(exclude=['tests']),
     license='MIT',
@@ -36,15 +36,15 @@
     install_requires=[
         'prettytable >= 2.5.0',
         'click >= 8.0.4',
         'requests >= 2.20.0',
         'prompt_toolkit >= 2',
         'pygments >= 2.0.0',
         'urllib3 >= 1.24',
-        'rich == 13.3.2'
+        'rich == 13.3.5'
     ],
     keywords=['softlayer', 'cloud', 'slcli'],
     classifiers=[
         'Environment :: Console',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
```

### Comparing `SoftLayer-6.1.6/tests/CLI/core_tests.py` & `SoftLayer-6.1.7/tests/CLI/core_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/custom_types_tests.py` & `SoftLayer-6.1.7/tests/CLI/custom_types_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/environment_tests.py` & `SoftLayer-6.1.7/tests/CLI/environment_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/helper_tests.py` & `SoftLayer-6.1.7/tests/CLI/helper_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/account_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/account_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,7 +170,12 @@
         self.assert_no_fail(result)
         self.assert_called_with('SoftLayer_Provisioning_Hook', 'createObject')
 
     def test_delete_provisioning_hook(self):
         result = self.run_command(['account', 'hook-delete', '123456'])
         self.assert_no_fail(result)
         self.assert_called_with('SoftLayer_Provisioning_Hook', 'deleteObject')
+
+    def test_order_upgrade(self):
+        result = self.run_command(['account', 'orders', '--upgrades'])
+        self.assert_no_fail(result)
+        self.assert_called_with('SoftLayer_Account', 'getUpgradeRequests')
```

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/block_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/block_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/call_api_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/call_api_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/cdn_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/sshkey_tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,125 +1,130 @@
 """
-    SoftLayer.tests.CLI.modules.cdn_tests
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    SoftLayer.tests.CLI.modules.sshkey_tests
+    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     :license: MIT, see LICENSE for more details.
 """
-import datetime
 import json
+import os.path
+import sys
+import tempfile
+
 from unittest import mock as mock
 
 from SoftLayer.CLI import exceptions
 from SoftLayer import testing
 
 
-class CdnTests(testing.TestCase):
-
-    def test_list_accounts(self):
-        result = self.run_command(['cdn', 'list'])
+class SshKeyTests(testing.TestCase):
+    def test_add_without_key_errors(self):
+        result = self.run_command(['sshkey', 'add', 'key1'])
 
-        self.assert_no_fail(result)
-        self.assertEqual(json.loads(result.output),
-                         [{'cname': 'cdnakauuiet7s6u6.cdnedge.bluemix.net',
-                           'domain': 'test.example.com',
-                           'origin': '1.1.1.1',
-                           'status': 'CNAME_CONFIGURATION',
-                           'unique_id': '11223344',
-                           'vendor': 'akamai'}]
-                         )
-
-    @mock.patch('SoftLayer.utils.days_to_datetime')
-    def test_detail_account(self, mock_now):
-        mock_now.return_value = datetime.datetime(2020, 1, 1)
-        result = self.run_command(['cdn', 'detail', '--history=30', '1245'])
-
-        self.assert_no_fail(result)
-        api_results = json.loads(result.output)
-        self.assertEqual(api_results['hit_ratio'], '2.0 %')
-        self.assertEqual(api_results['total_bandwidth'], '1.0 GB')
-        self.assertEqual(api_results['total_hits'], 3)
-        self.assertEqual(api_results['hostname'], 'test.example.com')
-        self.assertEqual(api_results['protocol'], 'HTTP')
+        self.assertEqual(result.exit_code, 2)
+        self.assertIsInstance(result.exception, exceptions.ArgumentError)
 
-    def test_purge_content(self):
-        result = self.run_command(['cdn', 'purge', '1234',
-                                   '/article/file.txt'])
+    def test_add_with_key_file_and_key_argument_errors(self):
+        path = os.path.join(testing.FIXTURE_PATH, 'id_rsa.pub')
+        result = self.run_command(['sshkey', 'add', 'key1',
+                                   '--key=some_key',
+                                   '--in-file=%s' % path])
 
-        self.assert_no_fail(result)
+        self.assertEqual(result.exit_code, 2)
+        self.assertIsInstance(result.exception, exceptions.ArgumentError)
 
-    def test_list_origins(self):
-        result = self.run_command(['cdn', 'origin-list', '1234'])
+    def test_add_by_option(self):
+        service = self.client['Security_Ssh_Key']
+        mock_key = service.getObject()['key']
+
+        result = self.run_command(['sshkey', 'add', 'key1',
+                                   '--key=%s' % mock_key,
+                                   '--note=my key'])
 
         self.assert_no_fail(result)
-        self.assertEqual(json.loads(result.output), [{'HTTP Port': 80,
-                                                      'Origin': '10.10.10.1',
-                                                      'Path': '/example',
-                                                      'Status': 'RUNNING'},
-                                                     {'HTTP Port': 80,
-                                                      'Origin': '10.10.10.1',
-                                                      'Path': '/example1',
-                                                      'Status': 'RUNNING'}])
-
-    def test_add_origin_server(self):
-        result = self.run_command(
-            ['cdn', 'origin-add', '-t', 'server', '-H=test.example.com', '-p', 80, '-o', 'web', '-c=include-all',
-             '1234', '10.10.10.1', '/example/videos2'])
+        self.assertEqual(json.loads(result.output),
+                         "SSH key added: aa:bb:cc:dd")
+        self.assert_called_with('SoftLayer_Security_Ssh_Key', 'createObject',
+                                args=({'notes': 'my key',
+                                       'key': mock_key,
+                                       'label': 'key1'},))
 
-        self.assert_no_fail(result)
+    def test_add_by_file(self):
+        path = os.path.join(testing.FIXTURE_PATH, 'id_rsa.pub')
 
-    def test_add_origin_storage(self):
-        result = self.run_command(['cdn', 'origin-add', '-t', 'storage', '-b=test-bucket', '-H=test.example.com',
-                                   '-p', 80, '-o', 'web', '-c=include-all', '1234', '10.10.10.1', '/example/videos2'])
+        result = self.run_command(['sshkey', 'add', 'key1',
+                                   '--in-file=%s' % path])
 
         self.assert_no_fail(result)
-
-    def test_add_origin_without_storage(self):
-        result = self.run_command(['cdn', 'origin-add', '-t', 'storage', '-H=test.example.com', '-p', 80,
-                                   '-o', 'web', '-c=include-all', '1234', '10.10.10.1', '/example/videos2'])
+        self.assertEqual(json.loads(result.output),
+                         "SSH key added: aa:bb:cc:dd")
+        service = self.client['Security_Ssh_Key']
+        mock_key = service.getObject()['key']
+        self.assert_called_with('SoftLayer_Security_Ssh_Key', 'createObject',
+                                args=({'notes': None,
+                                       'key': mock_key,
+                                       'label': 'key1'},))
+
+    def test_remove_key(self):
+        result = self.run_command(['--really', 'sshkey', 'remove', '1234'])
+
+        self.assert_no_fail(result)
+        self.assert_called_with('SoftLayer_Security_Ssh_Key', 'deleteObject',
+                                identifier=1234)
+
+    @mock.patch('SoftLayer.CLI.formatting.no_going_back')
+    def test_remove_key_fail(self, ngb_mock):
+        ngb_mock.return_value = False
+        result = self.run_command(['sshkey', 'remove', '1234'])
 
         self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.ArgumentError)
 
-    def test_add_origin_storage_with_file_extensions(self):
-        result = self.run_command(
-            ['cdn', 'origin-add', '-t', 'storage', '-b=test-bucket', '-e', 'jpg', '-H=test.example.com', '-p', 80,
-             '-o', 'web', '-c=include-all', '1234', '10.10.10.1', '/example/videos2'])
+    def test_edit_key(self):
+        result = self.run_command(['sshkey', 'edit', '1234',
+                                   '--label=key1', '--note=my key'])
+
+        self.assert_no_fail(result)
+        self.assert_called_with('SoftLayer_Security_Ssh_Key', 'editObject',
+                                args=({'notes': 'my key',
+                                       'label': 'key1'},),
+                                identifier=1234)
+
+    def test_edit_key_fail(self):
+        fixture = self.set_mock('SoftLayer_Security_Ssh_Key', 'editObject')
+        fixture.return_value = False
 
-        self.assert_no_fail(result)
+        result = self.run_command(['sshkey', 'edit', '1234',
+                                   '--label=key1', '--note=my key'])
 
-    def test_remove_origin(self):
-        result = self.run_command(['cdn', 'origin-remove', '1234',
-                                   '/example1'])
+        self.assertEqual(result.exit_code, 2)
 
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, "Origin with path /example1 has been deleted\n")
+    def test_list_keys(self):
+        result = self.run_command(['sshkey', 'list'])
 
-    def test_edit_header(self):
-        result = self.run_command(['cdn', 'edit', 'test.example.com', '--header=www.test.com'])
         self.assert_no_fail(result)
-        header_result = json.loads(result.output)
-        self.assertEqual('www.test.com', header_result['Header'])
+        self.assertEqual(json.loads(result.output),
+                         [{'notes': '-',
+                           'fingerprint': None,
+                           'id': '100',
+                           'label': 'Test 1'},
+                          {'notes': 'my key',
+                           'fingerprint': None,
+                           'id': '101',
+                           'label': 'Test 2'}])
 
-    def test_edit_http_port(self):
-        result = self.run_command(['cdn', 'edit', 'test.example.com', '--http-port=83'])
-        self.assert_no_fail(result)
-        header_result = json.loads(result.output)
-        self.assertEqual(83, header_result['Http Port'])
+    def test_print_key(self):
+        result = self.run_command(['sshkey', 'print', '1234'])
 
-    def test_edit_respect_headers(self):
-        result = self.run_command(['cdn', 'edit', 'test.example.com', '--respect-headers=1'])
         self.assert_no_fail(result)
-        header_result = json.loads(result.output)
-        self.assertEqual(True, header_result['Respect Headers'])
+        self.assertEqual(json.loads(result.output),
+                         {'id': 1234, 'label': 'label', 'notes': 'notes'})
 
-    def test_edit_cache(self):
-        result = self.run_command(['cdn', 'edit', 'test.example.com', '--cache', 'include-specified',
-                                   '--cache', 'test'])
-        self.assert_no_fail(result)
-        header_result = json.loads(result.output)
-        self.assertEqual('include: test', header_result['Cache key optimization'])
+    def test_print_key_file(self):
+        if (sys.platform.startswith("win")):
+            self.skipTest("Test doesn't work in Windows")
+        with tempfile.NamedTemporaryFile() as sshkey_file:
+            service = self.client['Security_Ssh_Key']
+            mock_key = service.getObject()['key']
+            result = self.run_command(['sshkey', 'print', '1234',
+                                       '--out-file=%s' % sshkey_file.name])
 
-    def test_edit_cache_by_uniqueId(self):
-        result = self.run_command(['cdn', 'edit', '11223344', '--cache', 'include-specified', '--cache', 'test'])
-        self.assert_no_fail(result)
-        header_result = json.loads(result.output)
-        self.assertEqual('include: test', header_result['Cache key optimization'])
+            self.assert_no_fail(result)
+            self.assertEqual(mock_key, sshkey_file.read().decode("utf-8"))
```

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/config_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/config_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/dedicatedhost_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/dedicatedhost_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/dns_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/dns_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/email_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/email_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/event_log_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/event_log_tests.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     SoftLayer.tests.CLI.modules.event_log_tests
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     :license: MIT, see LICENSE for more details.
 """
 
 import json
 
+from SoftLayer import SoftLayerAPIError
 from SoftLayer import testing
 
 
 class EventLogTests(testing.TestCase):
 
     def test_get_event_log_with_metadata(self):
         result = self.run_command(['event-log', 'get', '--metadata'])
@@ -87,7 +88,20 @@
         self.assertEqual(expected, json.loads(result.output))
 
     def test_get_unlimited_events(self):
         result = self.run_command(['event-log', 'get', '-l -1'])
         self.assert_no_fail(result)
         self.assert_called_with('SoftLayer_Event_Log', 'getAllObjects')
         self.assertEqual(8, result.output.count("\n"))
+
+    def test_issues1905(self):
+        """https://github.com/softlayer/softlayer-python/issues/1905"""
+        getUser = self.set_mock('SoftLayer_User_Customer', 'getObject')
+        getUser.side_effect = SoftLayerAPIError(
+            "SoftLayer_Exception_PermissionDenied",
+            "You do not have permission to access this user")
+        result = self.run_command(['event-log', 'get', '-l -1'])
+        self.assert_no_fail(result)
+        self.assert_called_with('SoftLayer_Event_Log', 'getAllObjects')
+        self.assert_called_with('SoftLayer_User_Customer', 'getObject', identifier=400)
+        user_calls = self.calls('SoftLayer_User_Customer', 'getObject')
+        self.assertEqual(1, len(user_calls))
```

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/file_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/file_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/firewall_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/firewall_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                                      'dest': 'any on server:80-800',
                                      'dest_mask': '255.255.255.255',
                                      'protocol': 'tcp',
                                      'src_ip': '0.0.0.0',
                                      'src_mask': '0.0.0.0'}]})
 
     def test_detail_multi_vlan_firewall(self):
-        result = self.run_command(['firewall', 'detail', 'multiVlan:1234', '--credentials', 'true'])
+        result = self.run_command(['firewall', 'detail', 'multiVlan:1234', '--password'])
         self.assert_no_fail(result)
         json_result = json.loads(result.output)
         self.assertEqual(json_result['rules'][0]['action'], 'permit')
         self.assertEqual(json.loads(result.output),
                          {'name': 'testFirewall',
                           'datacenter': 'Amsterdam 1',
                           'public ip': '67.228.206.245',
```

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/globalip_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/globalip_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/image_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/image_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/ipsec_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/ipsec_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/licenses_test.py` & `SoftLayer-6.1.7/tests/CLI/modules/licenses_test.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/loadbal_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/loadbal_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/nas_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/nas_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/object_storage_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/object_storage_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,7 +116,17 @@
         self.assert_no_fail(result)
 
     @mock.patch('SoftLayer.CLI.helpers.resolve_id')
     def test_list_credential_by_username(self, resolve_id_mock):
         resolve_id_mock.return_value = 100
         result = self.run_command(['object-storage', 'credential', 'list', 'test'])
         self.assert_no_fail(result)
+
+    def test_object_storage_cancel(self):
+        result = self.run_command([
+            '--really', 'object-storage', 'cancel', '1234'])
+
+        self.assert_no_fail(result)
+        self.assertEqual('Object storage with id 1234 has been marked'
+                         ' for cancellation\n', result.output)
+        self.assert_called_with('SoftLayer_Billing_Item', 'cancelItem',
+                                args=(False, True, None))
```

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/order_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/order_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,19 @@
     def test_order_lookup(self):
         result = self.run_command(['order', 'lookup', '12345'])
         self.assert_no_fail(result)
         self.assert_called_with('SoftLayer_Billing_Order', 'getObject', identifier='12345')
         self.assertIn('Ordered By', result.output)
         self.assertIn('Initial Invoice', result.output)
 
+    def test_quote_delete(self):
+        result = self.run_command(['order', 'quote-delete', '12345'])
+        self.assert_no_fail(result)
+        self.assert_called_with('SoftLayer_Billing_Order_Quote', 'deleteQuote', identifier='12345')
+
 
 def _get_all_packages():
     package_type = {'keyName': 'BARE_METAL_CPU'}
     all_packages = [
         {'id': 1, 'name': 'package1', 'keyName': 'PACKAGE1', 'type': package_type, 'isActive': 1},
         {'id': 2, 'name': 'package2', 'keyName': 'PACKAGE2', 'type': package_type, 'isActive': 1},
         {'id': 3, 'name': 'package2', 'keyName': 'PACKAGE2', 'type': package_type, 'isActive': 0}
```

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/report_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/report_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/securitygroup_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/securitygroup_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/server_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/server_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/ssl_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/ssl_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/subnet_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/subnet_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/summary_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/summary_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/tag_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/tag_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/ticket_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/ticket_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/user_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/user_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,7 +374,16 @@
         result = self.run_command(['user', 'remove-access', '123456', '--dedicated', '369852'])
         self.assert_no_fail(result)
 
     def test_remove_without_device(self):
         result = self.run_command(['user', 'remove-access', '123456'])
         self.assertEqual(2, result.exit_code)
         self.assertIn('A device option is required.', result.exception.message)
+
+    def test_update_vpn_password(self):
+        result = self.run_command(['user', 'vpn-password', '123456', '--password', 'Mypassword1.'])
+        self.assert_no_fail(result)
+
+    def test_remove_without_password(self):
+        result = self.run_command(['user', 'vpn-password', '123456'])
+        self.assertEqual(2, result.exit_code)
+        self.assertIn("Missing option '--password'", result.output)
```

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/vlan_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/vlan_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/vs/vs_capacity_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/vs/vs_capacity_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/vs/vs_create_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/vs/vs_create_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,36 +65,36 @@
                                    '--tag=dev',
                                    '--tag=green'])
 
         self.assert_no_fail(result)
         self.assertIn('"guid": "1a2b3c-1701"', result.output)
         self.assert_called_with('SoftLayer_Product_Order', 'placeOrder')
         args = ({
-            'startCpus': 2,
-            'maxMemory': 1024,
-            'hostname': 'host',
-            'domain': 'example.com',
-            'localDiskFlag': True,
-            'hourlyBillingFlag': True,
-            'supplementalCreateObjectOptions': {'bootMode': None},
-            'operatingSystemReferenceCode': 'UBUNTU_LATEST',
-            'datacenter': {'name': 'dal05'},
-            'primaryBackendNetworkComponent': {
-                'networkVlan': {
-                    'id': 577940,
-                    'primarySubnet': {'id': 478700}
-                }
-            },
-            'primaryNetworkComponent': {
-                'networkVlan': {
-                    'id': 1639255,
-                    'primarySubnet': {'id': 297614}
-                }
-            }
-        },)
+                    'startCpus': 2,
+                    'maxMemory': 1024,
+                    'hostname': 'host',
+                    'domain': 'example.com',
+                    'localDiskFlag': True,
+                    'hourlyBillingFlag': True,
+                    'supplementalCreateObjectOptions': {'bootMode': None},
+                    'operatingSystemReferenceCode': 'UBUNTU_LATEST',
+                    'datacenter': {'name': 'dal05'},
+                    'primaryBackendNetworkComponent': {
+                        'networkVlan': {
+                            'id': 577940,
+                            'primarySubnet': {'id': 478700}
+                        }
+                    },
+                    'primaryNetworkComponent': {
+                        'networkVlan': {
+                            'id': 1639255,
+                            'primarySubnet': {'id': 297614}
+                        }
+                    }
+                },)
 
         self.assert_called_with('SoftLayer_Virtual_Guest', 'generateOrderTemplate', args=args)
 
     @mock.patch('SoftLayer.CLI.formatting.confirm')
     def test_create_by_router(self, confirm_mock):
         confirm_mock.return_value = True
 
@@ -110,34 +110,34 @@
                                    '--router-public=1639255',
                                    '--tag=dev',
                                    '--tag=green'])
 
         self.assert_no_fail(result)
         self.assert_called_with('SoftLayer_Product_Order', 'placeOrder')
         args = ({
-            'startCpus': 2,
-            'maxMemory': 1024,
-            'hostname': 'host',
-            'domain': 'example.com',
-            'localDiskFlag': True,
-            'hourlyBillingFlag': True,
-            'supplementalCreateObjectOptions': {'bootMode': None},
-            'operatingSystemReferenceCode': 'UBUNTU_LATEST',
-            'datacenter': {'name': 'dal05'},
-            'primaryBackendNetworkComponent': {
+                    'startCpus': 2,
+                    'maxMemory': 1024,
+                    'hostname': 'host',
+                    'domain': 'example.com',
+                    'localDiskFlag': True,
+                    'hourlyBillingFlag': True,
+                    'supplementalCreateObjectOptions': {'bootMode': None},
+                    'operatingSystemReferenceCode': 'UBUNTU_LATEST',
+                    'datacenter': {'name': 'dal05'},
+                    'primaryBackendNetworkComponent': {
                         'router': {
                             'id': 577940
                         }
-            },
-            'primaryNetworkComponent': {
-                'router': {
-                    'id': 1639255
-                }
-            }
-        },)
+                    },
+                    'primaryNetworkComponent': {
+                        'router': {
+                            'id': 1639255
+                        }
+                    }
+                },)
 
         self.assert_called_with('SoftLayer_Virtual_Guest', 'generateOrderTemplate', args=args)
 
     @mock.patch('SoftLayer.CLI.formatting.confirm')
     def test_create_with_wait_ready(self, confirm_mock):
         mock = self.set_mock('SoftLayer_Virtual_Guest', 'getObject')
         mock.return_value = {
@@ -212,25 +212,25 @@
                                    '--network=100',
                                    '--billing=hourly',
                                    '--datacenter=dal05'])
 
         self.assert_no_fail(result)
         self.assertIn('"guid": "1a2b3c-1701"', result.output)
         args = ({
-            'startCpus': 2,
-            'maxMemory': 1024,
-            'hostname': 'host',
-            'domain': 'example.com',
-            'localDiskFlag': True,
-            'hourlyBillingFlag': True,
-            'supplementalCreateObjectOptions': {'bootMode': None},
-            'blockDeviceTemplateGroup': {'globalIdentifier': 'aaaa1111bbbb2222'},
-            'datacenter': {'name': 'dal05'},
-            'networkComponents': [{'maxSpeed': 100}]
-        },)
+                    'startCpus': 2,
+                    'maxMemory': 1024,
+                    'hostname': 'host',
+                    'domain': 'example.com',
+                    'localDiskFlag': True,
+                    'hourlyBillingFlag': True,
+                    'supplementalCreateObjectOptions': {'bootMode': None},
+                    'blockDeviceTemplateGroup': {'globalIdentifier': 'aaaa1111bbbb2222'},
+                    'datacenter': {'name': 'dal05'},
+                    'networkComponents': [{'maxSpeed': 100}]
+                },)
 
         self.assert_called_with('SoftLayer_Virtual_Guest', 'generateOrderTemplate', args=args)
         self.assert_called_with('SoftLayer_Product_Order', 'placeOrder')
 
     @mock.patch('SoftLayer.CLI.formatting.confirm')
     def test_create_with_flavor(self, confirm_mock):
         confirm_mock.return_value = True
@@ -341,26 +341,26 @@
         # Argument testing Example
         order_call = self.calls('SoftLayer_Product_Order', 'placeOrder')
         order_args = getattr(order_call[0], 'args')[0]
         self.assertEqual(123, order_args['hostId'])
 
         self.assert_called_with('SoftLayer_Product_Order', 'placeOrder')
         template_args = ({
-            'startCpus': 2,
-            'maxMemory': 1024,
-            'hostname': 'host',
-            'domain': 'example.com',
-            'localDiskFlag': True,
-            'hourlyBillingFlag': True,
-            'supplementalCreateObjectOptions': {'bootMode': None},
-            'dedicatedHost': {'id': 123},
-            'operatingSystemReferenceCode': 'UBUNTU_LATEST',
-            'datacenter': {'name': 'dal05'},
-            'networkComponents': [{'maxSpeed': 100}]
-        },)
+                             'startCpus': 2,
+                             'maxMemory': 1024,
+                             'hostname': 'host',
+                             'domain': 'example.com',
+                             'localDiskFlag': True,
+                             'hourlyBillingFlag': True,
+                             'supplementalCreateObjectOptions': {'bootMode': None},
+                             'dedicatedHost': {'id': 123},
+                             'operatingSystemReferenceCode': 'UBUNTU_LATEST',
+                             'datacenter': {'name': 'dal05'},
+                             'networkComponents': [{'maxSpeed': 100}]
+                         },)
 
         self.assert_called_with('SoftLayer_Virtual_Guest', 'generateOrderTemplate', args=template_args)
 
     @mock.patch('SoftLayer.CLI.formatting.confirm')
     def test_create_like(self, confirm_mock):
         mock = self.set_mock('SoftLayer_Virtual_Guest', 'getObject')
         mock.return_value = {
@@ -629,30 +629,29 @@
                                    '--domain', 'TESTING', '--flavor', 'B1_2X8X25',
                                    '--datacenter', 'TEST00', '--os', 'UBUNTU_LATEST', '--ipv6'])
 
         self.assert_no_fail(result)
         self.assertEqual(result.exit_code, 0)
         self.assert_called_with('SoftLayer_Product_Order', 'verifyOrder')
         args = ({
-            'startCpus': None,
-            'maxMemory': None,
-            'hostname': 'TEST',
-            'domain': 'TESTING',
-            'localDiskFlag': None,
-            'hourlyBillingFlag': True,
-            'supplementalCreateObjectOptions': {
-                'bootMode': None,
-                'flavorKeyName': 'B1_2X8X25'
-            },
-            'operatingSystemReferenceCode': 'UBUNTU_LATEST',
-            'datacenter': {
-                'name': 'TEST00'
-            }
-        },
-        )
+                    'startCpus': None,
+                    'maxMemory': None,
+                    'hostname': 'TEST',
+                    'domain': 'TESTING',
+                    'localDiskFlag': None,
+                    'hourlyBillingFlag': True,
+                    'supplementalCreateObjectOptions': {
+                        'bootMode': None,
+                        'flavorKeyName': 'B1_2X8X25'
+                    },
+                    'operatingSystemReferenceCode': 'UBUNTU_LATEST',
+                    'datacenter': {
+                        'name': 'TEST00'
+                    }
+                },)
         self.assert_called_with('SoftLayer_Virtual_Guest', 'generateOrderTemplate', args=args)
         self.assertEqual([], self.calls('SoftLayer_Virtual_Guest', 'setTags'))
 
     @mock.patch('SoftLayer.CLI.formatting.confirm')
     def test_create_with_ipv6_no_test(self, confirm_mock):
         confirm_mock.return_value = True
         amock = self.set_mock('SoftLayer_Product_Package', 'getItems')
@@ -689,15 +688,15 @@
         result = self.run_command(['vs', 'create', '--hostname', 'TEST',
                                    '--domain', 'TESTING', '--flavor', 'B1_2X8X25',
                                    '--datacenter', 'TEST00', '--os', 'UBUNTU_LATEST'])
 
         self.assertEqual(result.exit_code, 2)
 
     def test_create_vs_export(self):
-        if(sys.platform.startswith("win")):
+        if (sys.platform.startswith("win")):
             self.skipTest("Test doesn't work in Windows")
         with tempfile.NamedTemporaryFile() as config_file:
             result = self.run_command(['vs', 'create', '--hostname', 'TEST', '--export', config_file.name,
                                        '--domain', 'TESTING', '--flavor', 'B1_2X8X25',
                                        '--datacenter', 'TEST00', '--os', 'UBUNTU_LATEST'])
             self.assert_no_fail(result)
             self.assertIn('Successfully exported options to a template file.', result.output)
```

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/vs/vs_placement_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/vs/vs_placement_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/CLI/modules/vs/vs_tests.py` & `SoftLayer-6.1.7/tests/CLI/modules/vs/vs_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/account_tests.py` & `SoftLayer-6.1.7/tests/managers/account_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,7 +184,11 @@
     def test_create_provisioning_scripts(self):
         self.manager.create_provisioning('testslcli', 'http://slclitest.com')
         self.assert_called_with('SoftLayer_Provisioning_Hook', 'createObject')
 
     def test_delete_provisioning_scripts(self):
         self.manager.delete_provisioning(123456)
         self.assert_called_with("SoftLayer_Provisioning_Hook", "deleteObject")
+
+    def test_get_upgrades_orders(self):
+        self.manager.get_account_upgrade_orders()
+        self.assert_called_with("SoftLayer_Account", "getUpgradeRequests")
```

### Comparing `SoftLayer-6.1.6/tests/managers/block_tests.py` & `SoftLayer-6.1.7/tests/managers/block_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/cdn_tests.py` & `SoftLayer-6.1.7/tests/managers/cdn_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         args = ("12345",
                 "/example1")
         self.assert_called_with('SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path',
                                 'deleteOriginPath',
                                 args=args)
 
     def test_purge_content(self):
-        self.cdn_client.purge_content("12345", "/example1")
+        self.cdn_client.purge_content("12345", "example1")
 
         args = ("12345",
                 "/example1")
         self.assert_called_with('SoftLayer_Network_CdnMarketplace_Configuration_Cache_Purge',
                                 'createPurge',
                                 args=args)
 
@@ -146,7 +146,30 @@
         hostname = 'test.example.com'
         result = self.cdn_client._get_ids_from_hostname(hostname)
         expected_result = fixtures.SoftLayer_Network_CdnMarketplace_Configuration_Mapping.listDomainMappings
         self.assertEqual(expected_result[0]['uniqueId'], result[0])
         self.assert_called_with(
             'SoftLayer_Network_CdnMarketplace_Configuration_Mapping',
             'listDomainMappings',)
+
+    def test_delete_cdn(self):
+        uniqueId = "123465"
+        self.cdn_client.delete_cdn(uniqueId)
+
+        args = (uniqueId,)
+
+        self.assert_called_with('SoftLayer_Network_CdnMarketplace_Configuration_Mapping',
+                                'deleteDomainMapping',
+                                args=args)
+
+    def test_create_cdn(self):
+        hostname = "test.com"
+        origin = "123.123.123.123"
+        origin_type = "server"
+        http = 80
+        newCdn = ({"domain": hostname, "origin": origin, "originType": "HOST_SERVER",
+                  "vendorName": "akamai", "httpPort": http, "protocol": "HTTP"},)
+        self.cdn_client.create_cdn(hostname, origin, origin_type, http)
+
+        self.assert_called_with('SoftLayer_Network_CdnMarketplace_Configuration_Mapping',
+                                'createDomainMapping',
+                                args=newCdn)
```

### Comparing `SoftLayer-6.1.6/tests/managers/dedicated_host_tests.py` & `SoftLayer-6.1.7/tests/managers/dedicated_host_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/dns_tests.py` & `SoftLayer-6.1.7/tests/managers/dns_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/email_tests.py` & `SoftLayer-6.1.7/tests/managers/email_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/event_log_tests.py` & `SoftLayer-6.1.7/tests/managers/event_log_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/file_tests.py` & `SoftLayer-6.1.7/tests/managers/file_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/firewall_tests.py` & `SoftLayer-6.1.7/tests/managers/firewall_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/hardware_tests.py` & `SoftLayer-6.1.7/tests/managers/hardware_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/image_tests.py` & `SoftLayer-6.1.7/tests/managers/image_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/ipsec_tests.py` & `SoftLayer-6.1.7/tests/managers/ipsec_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/loadbal_tests.py` & `SoftLayer-6.1.7/tests/managers/loadbal_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/metadata_tests.py` & `SoftLayer-6.1.7/tests/managers/metadata_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/network_tests.py` & `SoftLayer-6.1.7/tests/managers/network_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/object_storage_tests.py` & `SoftLayer-6.1.7/tests/managers/object_storage_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/ordering_tests.py` & `SoftLayer-6.1.7/tests/managers/ordering_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -897,7 +897,11 @@
     def test_get_items(self):
         self.ordering.get_items(123)
         self.assert_called_with('SoftLayer_Product_Package', 'getItems')
 
     def test_get_regions(self):
         self.ordering.get_regions(123)
         self.assert_called_with('SoftLayer_Product_Package', 'getRegions')
+
+    def test_delete_quote(self):
+        self.ordering.delete_quote(123)
+        self.assert_called_with('SoftLayer_Billing_Order_Quote', 'deleteQuote')
```

### Comparing `SoftLayer-6.1.6/tests/managers/search_tests.py` & `SoftLayer-6.1.7/tests/managers/search_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/sshkey_tests.py` & `SoftLayer-6.1.7/tests/managers/sshkey_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/ssl_tests.py` & `SoftLayer-6.1.7/tests/managers/ssl_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/storage_generic_tests.py` & `SoftLayer-6.1.7/tests/managers/storage_generic_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/storage_utils_tests.py` & `SoftLayer-6.1.7/tests/managers/storage_utils_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/tag_tests.py` & `SoftLayer-6.1.7/tests/managers/tag_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/ticket_tests.py` & `SoftLayer-6.1.7/tests/managers/ticket_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/user_tests.py` & `SoftLayer-6.1.7/tests/managers/user_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,7 +326,11 @@
     def test_remove_virtual(self):
         self.manager.remove_virtual_access(123456, 369852)
         self.assert_called_with('SoftLayer_User_Customer', 'removeVirtualGuestAccess')
 
     def test_remove_dedicated(self):
         self.manager.remove_dedicated_access(123456, 369852)
         self.assert_called_with('SoftLayer_User_Customer', 'removeDedicatedHostAccess')
+
+    def test_update_vpn_password(self):
+        self.manager.update_vpn_password(123456, "Mypassword1.")
+        self.assert_called_with('SoftLayer_User_Customer', 'updateVpnPassword')
```

### Comparing `SoftLayer-6.1.6/tests/managers/vs/vs_capacity_tests.py` & `SoftLayer-6.1.7/tests/managers/vs/vs_capacity_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/vs/vs_order_tests.py` & `SoftLayer-6.1.7/tests/managers/vs/vs_order_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/vs/vs_placement_tests.py` & `SoftLayer-6.1.7/tests/managers/vs/vs_placement_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/vs/vs_tests.py` & `SoftLayer-6.1.7/tests/managers/vs/vs_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/managers/vs/vs_waiting_for_ready_tests.py` & `SoftLayer-6.1.7/tests/managers/vs/vs_waiting_for_ready_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/transports/debug_tests.py` & `SoftLayer-6.1.7/tests/transports/debug_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/transports/rest_tests.py` & `SoftLayer-6.1.7/tests/transports/rest_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/transports/transport_tests.py` & `SoftLayer-6.1.7/tests/transports/transport_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.6/tests/transports/xmlrpc_tests.py` & `SoftLayer-6.1.7/tests/transports/xmlrpc_tests.py`

 * *Files identical despite different names*

