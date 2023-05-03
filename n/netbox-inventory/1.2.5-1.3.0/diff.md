# Comparing `tmp/netbox-inventory-1.2.5.tar.gz` & `tmp/netbox-inventory-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.2.5.tar", last modified: Wed Apr 26 11:31:54 2023, max compression
+gzip compressed data, was "netbox-inventory-1.3.0.tar", last modified: Wed May  3 08:04:19 2023, max compression
```

## Comparing `netbox-inventory-1.2.5.tar` & `netbox-inventory-1.3.0.tar`

### file list

```diff
@@ -1,110 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.524765 netbox-inventory-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-04-26 11:31:54.524765 netbox-inventory-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.476765 netbox-inventory-1.2.5/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.480765 netbox-inventory-1.2.5/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.488765 netbox-inventory-1.2.5/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/reassign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.492765 netbox-inventory-1.2.5/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.460765 netbox-inventory-1.2.5/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.500765 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_reassign.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.500765 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.504765 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.508765 netbox-inventory-1.2.5/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.512765 netbox-inventory-1.2.5/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.512765 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.516765 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.516765 netbox-inventory-1.2.5/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.516765 netbox-inventory-1.2.5/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.524765 netbox-inventory-1.2.5/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.480765 netbox-inventory-1.2.5/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-04-26 11:31:54.000000 netbox-inventory-1.2.5/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-26 11:31:54.000000 netbox-inventory-1.2.5/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:31:54.000000 netbox-inventory-1.2.5/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 11:31:54.000000 netbox-inventory-1.2.5/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:31:54.524765 netbox-inventory-1.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.881295 netbox-inventory-1.3.0/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.881295 netbox-inventory-1.3.0/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17795 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/reassign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.877294 netbox-inventory-1.3.0/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.881295 netbox-inventory-1.3.0/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-03 08:04:19.000000 netbox-inventory-1.3.0/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-03 08:04:19.000000 netbox-inventory-1.3.0/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:04:19.000000 netbox-inventory-1.3.0/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 08:04:19.000000 netbox-inventory-1.3.0/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/setup.cfg
```

### Comparing `netbox-inventory-1.2.5/LICENSE` & `netbox-inventory-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/PKG-INFO` & `netbox-inventory-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.2.5
+Version: 1.3.0
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -67,21 +67,22 @@
 
 With `asset_disable_editing_fields_for_tags` and `asset_disable_deletion_for_tags` you can prevent changes to specified asset data for assets that have certain tags attached. Changes are only prevented via web interface. API modifications are allowed.
 
 The idea is that an external system uses some assets stored in netbox_inventory, and you want to prevent accidental changes to data directly in NetBox web interface. Only that external system should modify the data.
 
 ## Compatibility
 
-This plugin requires netbox version 3.4.x to work. Older versions of the plugin
+This plugin requires netbox version 3.5.x to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |       3.3      |      1.1.x     |
 |       3.4      |      1.2.x     |
+|       3.5      |      1.3.x     |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
```

### Comparing `netbox-inventory-1.2.5/README.md` & `netbox-inventory-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,21 +52,22 @@
 
 With `asset_disable_editing_fields_for_tags` and `asset_disable_deletion_for_tags` you can prevent changes to specified asset data for assets that have certain tags attached. Changes are only prevented via web interface. API modifications are allowed.
 
 The idea is that an external system uses some assets stored in netbox_inventory, and you want to prevent accidental changes to data directly in NetBox web interface. Only that external system should modify the data.
 
 ## Compatibility
 
-This plugin requires netbox version 3.4.x to work. Older versions of the plugin
+This plugin requires netbox version 3.5.x to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |       3.3      |      1.1.x     |
 |       3.4      |      1.2.x     |
+|       3.5      |      1.3.x     |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/__init__.py` & `netbox-inventory-1.3.0/netbox_inventory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     name = 'netbox_inventory'
     verbose_name = 'NetBox Inventory'
     version = __version__
     description = 'Inventory asset management in NetBox'
     author = 'Matej Vadnjal'
     author_email = 'matej.vadnjal@arnes.si'
     base_url = 'inventory'
-    min_version = '3.4.0'
+    min_version = '3.5.0'
     default_settings = {
         'top_level_menu': True,
         'used_status_name': 'used',
         'stored_status_name': 'stored',
         'sync_hardware_serial_asset_tag': False,
         'asset_import_create_purchase': False,
         'asset_import_create_device_type': False,
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/analyzers.py` & `netbox-inventory-1.3.0/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/api/nested_serializers.py` & `netbox-inventory-1.3.0/netbox_inventory/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/api/serializers.py` & `netbox-inventory-1.3.0/netbox_inventory/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/api/urls.py` & `netbox-inventory-1.3.0/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/api/views.py` & `netbox-inventory-1.3.0/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/filtersets.py` & `netbox-inventory-1.3.0/netbox_inventory/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/forms/assign.py` & `netbox-inventory-1.3.0/netbox_inventory/forms/assign.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from django import forms
 
 from dcim.models import Device, InventoryItem, Module, Site
 from netbox.forms import NetBoxModelForm
-from utilities.forms import APISelect, DynamicModelChoiceField
+from tenancy.models import Contact, Tenant
+from utilities.forms.fields import DynamicModelChoiceField
+from utilities.forms.widgets import APISelect
 from ..models import Asset
 
 __all__ = (
     'AssetDeviceAssignForm',
     'AssetModuleAssignForm',
     'AssetInventoryItemAssignForm',
 )
@@ -14,14 +16,26 @@
 
 class AssetAssignMixin(forms.Form):
     name = forms.CharField(
         required=False,
         label='Asset name',
         help_text=Asset._meta.get_field('name').help_text
     )
+    tenant = DynamicModelChoiceField(
+        queryset=Tenant.objects.all(),
+        selector=True,
+        required=False,
+        help_text=Asset._meta.get_field('tenant').help_text,
+    )
+    contact = DynamicModelChoiceField(
+        queryset=Contact.objects.all(),
+        selector=True,
+        required=False,
+        help_text=Asset._meta.get_field('contact').help_text,
+    )
     tags = None
 
     def _clean_hardware_type(self, kind):
         hardware_type = self.cleaned_data[f'{kind}_type']
         if getattr(self.instance, f'{kind}_type') != hardware_type:
             raise forms.ValidationError(f'You are not allowed to change {kind}_type')
         return hardware_type
@@ -67,15 +81,15 @@
             },
         )
     )
 
     fieldsets = (
         ('Asset', ('device_type', 'name')),
         ('Device', ('site', 'device')),
-        ('Tenancy', ('tenant', 'contact')),
+        ('Assigned to', ('tenant', 'contact')),
     )
 
     class Meta:
         model = Asset
         fields = ('device_type', 'name', 'site', 'device', 'tenant', 'contact')
         widgets = {'device_type': forms.HiddenInput()}
 
@@ -83,23 +97,17 @@
         return self._clean_hardware_type('device')
 
     def clean_device(self):
         return self._clean_hardware('device')
 
 
 class AssetModuleAssignForm(AssetAssignMixin, NetBoxModelForm):
-    site = DynamicModelChoiceField(
-        queryset=Site.objects.all(),
-        required=False,
-        initial_params={'devices': '$device'},
-    )
     device = DynamicModelChoiceField(
         queryset=Device.objects.all(),
-        query_params={'site_id': '$site'},
-        label='Device',
+        selector=True,
         required=False,
     )
     module = DynamicModelChoiceField(
         queryset=Module.objects.all(),
         query_params={'module_type_id': '$module_type', 'device_id': '$device'},
         label='Module',
         required=False,
@@ -110,44 +118,38 @@
                 'data-static-params': '[{"queryParam":"has_asset_assigned","queryValue":"false"}]',
             },
         )
     )
 
     fieldsets = (
         ('Asset', ('module_type', 'name')),
-        ('Module', ('site', 'device', 'module')),
+        ('Module', ('device', 'module',)),
         ('Tenancy', ('tenant', 'contact')),
     )
 
     class Meta:
         model = Asset
-        fields = ('module_type', 'name', 'site', 'device', 'module', 'tenant', 'contact')
+        fields = ('module_type', 'name', 'device', 'module', 'tenant', 'contact')
         widgets = {'module_type': forms.HiddenInput()}
 
     def clean_device(self):
         # prevents trying to set asset.device
         return None
 
     def clean_module_type(self):
         return self._clean_hardware_type('module')
 
     def clean_module(self):
         return self._clean_hardware('module')
 
 
 class AssetInventoryItemAssignForm(AssetAssignMixin, NetBoxModelForm):
-    site = DynamicModelChoiceField(
-        queryset=Site.objects.all(),
-        required=False,
-        initial_params={'devices': '$device'},
-    )
     device = DynamicModelChoiceField(
         queryset=Device.objects.all(),
-        query_params={'site_id': '$site'},
-        label='Device',
+        selector=True,
         required=False,
     )
     inventoryitem = DynamicModelChoiceField(
         queryset=InventoryItem.objects.all(),
         # we can't filter on inventoryitem_type because inventoryitem doesn't
         # have relation to inventoryitem_type
         query_params={'device_id': '$device'},
@@ -160,21 +162,21 @@
                 'data-static-params': '[{"queryParam":"has_asset_assigned","queryValue":"false"}]',
             },
         )
     )
 
     fieldsets = (
         ('Asset', ('inventoryitem_type', 'name')),
-        ('Inventory Item', ('site', 'device', 'inventoryitem')),
+        ('Inventory Item', ('device', 'inventoryitem')),
         ('Tenancy', ('tenant', 'contact')),
     )
 
     class Meta:
         model = Asset
-        fields = ('inventoryitem_type', 'name', 'site', 'device', 'inventoryitem', 'tenant', 'contact')
+        fields = ('inventoryitem_type', 'name', 'device', 'inventoryitem', 'tenant', 'contact')
         widgets = {'inventoryitem_type': forms.HiddenInput()}
 
     def clean_device(self):
         # prevents trying to set asset.device
         return None
 
     def clean_inventoryitem_type(self):
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/forms/bulk.py` & `netbox-inventory-1.3.0/netbox_inventory/forms/bulk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from django import forms
 from django.core.exceptions import ObjectDoesNotExist
 from django.utils.text import slugify
 
 from dcim.models import DeviceType, Manufacturer, ModuleType, Location, Site
 from netbox.forms import NetBoxModelBulkEditForm, NetBoxModelImportForm
-from utilities.forms import (
-    add_blank_choice, ChoiceField, CommentField, CSVChoiceField,
-    CSVModelChoiceField, DynamicModelChoiceField
+from utilities.forms import add_blank_choice
+from utilities.forms.fields import (
+    ChoiceField, CommentField, CSVChoiceField, CSVModelChoiceField,
+    DynamicModelChoiceField
 )
 from tenancy.models import Contact, Tenant
 from ..choices import AssetStatusChoices, HardwareKindChoices
 from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from ..utils import get_plugin_setting
 
 __all__ = (
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/forms/bulk_add.py` & `netbox-inventory-1.3.0/netbox_inventory/forms/bulk_add.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/forms/filters.py` & `netbox-inventory-1.3.0/netbox_inventory/forms/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from cProfile import label
 from django import forms
 
 from dcim.models import Device, DeviceType, Manufacturer, ModuleType, Site, Location, Rack
 from netbox.forms import NetBoxModelFilterSetForm
-from utilities.forms import (
-    DatePicker, DynamicModelMultipleChoiceField, MultipleChoiceField,
-    StaticSelect, TagFilterField, BOOLEAN_WITH_BLANK_CHOICES
-)
+from utilities.forms import BOOLEAN_WITH_BLANK_CHOICES
+from utilities.forms.fields import DynamicModelMultipleChoiceField, MultipleChoiceField, TagFilterField
+from utilities.forms.widgets import DatePicker
 from tenancy.forms import ContactModelFilterForm
 from tenancy.models import Contact, Tenant
 from ..choices import HardwareKindChoices, AssetStatusChoices
 from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 
 
 __all__ = (
@@ -85,15 +83,15 @@
         queryset=InventoryItemGroup.objects.all(),
         required=False,
         label='Inventory Item Group',
     )
     is_assigned = forms.NullBooleanField(
         required=False,
         label='Is assigned to hardware',
-        widget=StaticSelect(
+        widget=forms.Select(
             choices=BOOLEAN_WITH_BLANK_CHOICES
         )
     )
     tenant_id = DynamicModelMultipleChoiceField(
         queryset=Tenant.objects.all(),
         required=False,
         null_option='None',
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/forms/models.py` & `netbox-inventory-1.3.0/netbox_inventory/forms/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dcim.models import DeviceType, Manufacturer, ModuleType, Location, Site
 from netbox.forms import NetBoxModelForm
 from netbox_inventory.choices import HardwareKindChoices
-from utilities.forms import CommentField, DatePicker, DynamicModelChoiceField, SlugField
+from utilities.forms.fields import CommentField, DynamicModelChoiceField, SlugField
+from utilities.forms.widgets import DatePicker
 from tenancy.models import Contact, Tenant
 from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from ..utils import get_tags_and_edit_protected_asset_fields
 
 __all__ = (
     'AssetForm',
     'SupplierForm',
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/forms/reassign.py` & `netbox-inventory-1.3.0/netbox_inventory/forms/reassign.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django import forms
 from django.core.exceptions import ValidationError
 
 from dcim.models import Device, InventoryItem, Module, Site, Location, Manufacturer
 from netbox.forms import NetBoxModelForm
-from utilities.forms import DynamicModelChoiceField, ChoiceField
+from utilities.forms.fields import DynamicModelChoiceField, ChoiceField
 from ..choices import AssetStatusChoices
 from ..models import Asset, InventoryItemType, InventoryItemGroup
 from ..utils import get_status_for
 
 
 __all__ = (
     'AssetDeviceReassignForm',
@@ -37,15 +37,15 @@
     tags = None
 
     class Meta:
         fields = ('storage_site', 'storage_location', 'assigned_asset', 'asset_status')
 
     def save(self, commit=True):
         # if existing assigned_asset, clear assignment before save
-        # handle snapshot for ald and new asset
+        # handle snapshot for old and new asset
         """
         Save this form's self.instance object if commit=True. Otherwise, add
         a save_m2m() method to the form which can be called after the instance
         is saved manually at a later time. Return the model instance.
         """
         if self.errors:
             raise ValueError(
@@ -56,16 +56,16 @@
                 )
             )
         if commit:
             self.instance.snapshot()
             if self.old_asset:
                 self.old_asset.status = self.cleaned_data['asset_status']
                 # if assigning another asset, don't clear data from device object
-                # will overwrite via net_asset.save later
-                # this is to avoind creating two changelog entries for device
+                # will overwrite via new_asset.save later
+                # this is to avoid creating two changelog entries for device
                 self.old_asset.save(clear_old_hw=not bool(self.new_asset))
             if self.new_asset:
                 self.new_asset.save()
         return self.instance
 
     def clean(self, *args, **kwargs):
         cleaned_data = super().clean(*args, **kwargs)
@@ -88,15 +88,15 @@
 
     def _clean_asset(self, asset, instance):
         # store old state of asset objects for changelog
         asset.snapshot()
         try:
             # update hardware assignment and validate data
             setattr(asset, asset.kind, instance)
-            asset.clean()
+            asset.full_clean(exclude=(asset.kind,))
         except ValidationError as e:
             # ValidationError raised for device or module field
             # "remap" to error for whole form 
             raise ValidationError(e.messages)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -107,14 +107,15 @@
             self.fields['asset_status'].widget = forms.HiddenInput()
 
 
 class AssetDeviceReassignForm(AssetReassignMixin, NetBoxModelForm):
     assigned_asset = DynamicModelChoiceField(
         queryset=Asset.objects.filter(device_type__isnull=False, device__isnull=True),
         required=False,
+        selector=True,
         query_params={
             'kind': 'device',
             'is_assigned': False,
             'device_type_id': '$device_type',
             'storage_site_id': '$storage_site',
             'storage_location_id': '$storage_location',
         },
@@ -136,14 +137,15 @@
         assigned_asset_field.queryset = Asset.objects.filter(device_type=self.instance.device_type, device__isnull=True)
 
 
 class AssetModuleReassignForm(AssetReassignMixin, NetBoxModelForm):
     assigned_asset = DynamicModelChoiceField(
         queryset=Asset.objects.filter(module_type__isnull=False, module__isnull=True),
         required=False,
+        selector=True,
         query_params={
             'kind': 'module',
             'is_assigned': False,
             'module_type_id': '$module_type',
             'storage_site_id': '$storage_site',
             'storage_location_id': '$storage_location',
         },
@@ -186,14 +188,15 @@
         },
         label='Inventory Item Type',
         help_text='Limit New Asset choices only to assets of this inventory item type',
     )
     assigned_asset = DynamicModelChoiceField(
         queryset=Asset.objects.filter(inventoryitem_type__isnull=False, inventoryitem__isnull=True),
         required=False,
+        selector=True,
         query_params={
             'kind': 'inventoryitem',
             'is_assigned': False,
             'storage_site_id': '$storage_site',
             'storage_location_id': '$storage_location',
             'manufacturer_id': '$manufacturer',
             'inventoryitem_type_id': '$inventoryitem_type',
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/migrations/0001_initial_prod.py` & `netbox-inventory-1.3.0/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox-inventory-1.3.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox-inventory-1.3.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/models.py` & `netbox-inventory-1.3.0/netbox_inventory/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/navigation.py` & `netbox-inventory-1.3.0/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/search.py` & `netbox-inventory-1.3.0/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/signals.py` & `netbox-inventory-1.3.0/netbox_inventory/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tables.py` & `netbox-inventory-1.3.0/netbox_inventory/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/template_content.py` & `netbox-inventory-1.3.0/netbox_inventory/template_content.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,18 +95,28 @@
 
 class TenantAssetInfo(PluginTemplateExtension):
     model = 'tenancy.tenant'
     def right_page(self):
         object = self.context.get('object')
         user = self.context['request'].user
         context = {
-            'asset_assigned_count': Asset.objects.restrict(user, 'view').filter(tenant=object).count(),
-            'asset_owned_count': Asset.objects.restrict(user, 'view').filter(owner=object).count(),
+            'asset_stats': [
+                {
+                    'label': 'Assigned',
+                    'filter_field': 'tenant_id',
+                    'count': Asset.objects.restrict(user, 'view').filter(tenant=object).count(),
+                },
+                {
+                    'label': 'Owned',
+                    'filter_field': 'owner_id',
+                    'count': Asset.objects.restrict(user, 'view').filter(owner=object).count(),
+                },
+            ],
         }
-        return self.render('netbox_inventory/inc/asset_tenant.html', extra_context=context)
+        return self.render('netbox_inventory/inc/asset_stats_counts.html', extra_context=context)
 
 
 class ContactAssetInfo(PluginTemplateExtension):
     model = 'tenancy.contact'
     def right_page(self):
         object = self.context.get('object')
         user = self.context['request'].user
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,62 @@
 {% extends "generic/bulk_import.html" %}
 
 {% load helpers %}
 {% load form_helpers %}
 
-{% block content %}
+{% block content-wrapper %}
 {{ block.super }}
 
-        <div class="row">
-            <div class="col col-md-12 col-lg-10 offset-lg-1">
-                <div class="row my-3">
-                    <div class="col col-md-12">
-                        <div class="card">
-                            <h5 class="card-header">
-                                Import settings
-                            </h5>
-                            <div class="card-body">
-                                <p>
-                                CSV import can automatically create objects related to each Asset being imported.
-                                This is controlled via plugin's <a href="https://github.com/ArnesSI/netbox-inventory#settings" target="_blank">settings</a>.
-                                If a related object is missing and is not allowed to be created autmatically, import will fail.
-                                </p>
-                                <p>
-                                Values bellow show your current config values.
-                                </p>
-                                <table class="table">
-                                    <tr>
-                                        <th>Object name</th>
-                                        <th>Created if missing?</th>
-                                        <th>Plugin setting name</th>
-                                    </tr>
-                                    <tr>
-                                        <td>Manufacturer & Device Type</td>
-                                        <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_device_type %}</td>
-                                        <td><code>asset_import_create_device_type</code></td>
-                                    </tr>
-                                    <tr>
-                                        <td>Manufacturer & Module Type</td>
-                                        <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_module_type %}</td>
-                                        <td><code>asset_import_create_module_type</code></td>
-                                    </tr>
-                                    <tr>
-                                        <td>Manufacturer & InventoryItem Type</td>
-                                        <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_inventoryitem_type %}</td>
-                                        <td><code>asset_import_create_inventoryitem_type</code></td>
-                                    </tr>
-                                    <tr>
-                                        <td>Supplier & Purchase</td>
-                                        <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_purchase %}</td>
-                                        <td><code>asset_import_create_purchase</code></td>
-                                    </tr>
-                                    <tr>
-                                        <td>Owner & Tenant</td>
-                                        <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_tenant %}</td>
-                                        <td><code>asset_import_create_tenant</code></td>
-                                    </tr>
-                                </table>
-                            </div>
-                        </div>
+    <div class="tab-content">
+        <div class="row my-3">
+            <div class="col col-md-12">
+                <div class="card">
+                    <h5 class="card-header">
+                        Import settings
+                    </h5>
+                    <div class="card-body">
+                        <p>
+                        CSV import can automatically create objects related to each Asset being imported.
+                        This is controlled via plugin's <a href="https://github.com/ArnesSI/netbox-inventory#settings" target="_blank">settings</a>.
+                        If a related object is missing and is not allowed to be created autmatically, import will fail.
+                        </p>
+                        <p>
+                        Values bellow show your current config values.
+                        </p>
+                        <table class="table">
+                            <tr>
+                                <th>Object name</th>
+                                <th>Created if missing?</th>
+                                <th>Plugin setting name</th>
+                            </tr>
+                            <tr>
+                                <td>Manufacturer & Device Type</td>
+                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_device_type %}</td>
+                                <td><code>asset_import_create_device_type</code></td>
+                            </tr>
+                            <tr>
+                                <td>Manufacturer & Module Type</td>
+                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_module_type %}</td>
+                                <td><code>asset_import_create_module_type</code></td>
+                            </tr>
+                            <tr>
+                                <td>Manufacturer & InventoryItem Type</td>
+                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_inventoryitem_type %}</td>
+                                <td><code>asset_import_create_inventoryitem_type</code></td>
+                            </tr>
+                            <tr>
+                                <td>Supplier & Purchase</td>
+                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_purchase %}</td>
+                                <td><code>asset_import_create_purchase</code></td>
+                            </tr>
+                            <tr>
+                                <td>Owner & Tenant</td>
+                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_tenant %}</td>
+                                <td><code>asset_import_create_tenant</code></td>
+                            </tr>
+                        </table>
                     </div>
                 </div>
             </div>
         </div>
-{% endblock content %}
-
+    </div>
+{% endblock content-wrapper %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends "generic/bulk_import.html" %} {% load helpers %} {% load
-form_helpers %} {% block content %} {{ block.super }}
+form_helpers %} {% block content-wrapper %} {{ block.super }}
 ** Import settings **
 CSV import can automatically create objects related to each Asset being
 imported. This is controlled via plugin's settings. If a related object is
 missing and is not allowed to be created autmatically, import will fail.
 Values bellow show your current config values.
 Object name   Created if missing?                                                             Plugin setting name
 Manufacturer  {% checkmark                                                                    asset_import_create_device_type
@@ -14,8 +14,8 @@
 &             settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_inventoryitem_type asset_import_create_inventoryitem_type
 InventoryItem %}
 Type
 Supplier &    {% checkmark                                                                    asset_import_create_purchase
 Purchase      settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_purchase %}
 Owner &       {% checkmark                                                                    asset_import_create_tenant
 Tenant        settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_tenant %}
-{% endblock content %}
+{% endblock content-wrapper %}
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_edit.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_api.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_models.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views_create.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/custom.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,32 +7,33 @@
 class InventoryItemGroupTestCase(
     ModelViewTestCase,
     ViewTestCases.PrimaryObjectViewTestCase,
 ):
 
     model = InventoryItemGroup
 
-    form_data = {
-        'name': 'InventoryItemGroup',
-    }
-    csv_data = (
-        'name,comments',
-        'IIG4,a comment',
-        'IIG5,a comment',
-        'IIG6,a comment',
-    )
-
     @classmethod
     def setUpTestData(cls):
+        iig_parent = InventoryItemGroup.objects.create(name='parent group')
         iig1 = InventoryItemGroup.objects.create(name='IIG1')
         iig2 = InventoryItemGroup.objects.create(name='IIG2')
         iig3 = InventoryItemGroup.objects.create(name='IIG3')
 
+
+        cls.form_data = {
+            'name': 'InventoryItemGroup',
+        }
+        cls.csv_data = (
+            'name,comments',
+            'IIG4,a comment',
+            'IIG5,a comment',
+            'IIG6,a comment',
+        )
         cls.csv_update_data = (
             'id,name,parent',
-            f'{iig1.pk},IIG1_update,InventoryItemGroup',
-            f'{iig2.pk},IIG2_update,InventoryItemGroup',
-            f'{iig3.pk},IIG3_update,InventoryItemGroup',
+            f'{iig1.pk},IIG1_update,{iig_parent.name}',
+            f'{iig2.pk},IIG2_update,{iig_parent.name}',
+            f'{iig3.pk},IIG3_update,{iig_parent.name}',
         )
         cls.bulk_edit_data = {
             'comments': 'updated',
-        }
+        }
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/purchase/test_api.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/purchase/test_views.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/settings.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/supplier/test_api.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/supplier/test_views.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/tests/test_load.py` & `netbox-inventory-1.3.0/netbox_inventory/tests/test_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxDnsVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.2.5"
+        assert __version__ == "1.3.0"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/urls.py` & `netbox-inventory-1.3.0/netbox_inventory/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/utils.py` & `netbox-inventory-1.3.0/netbox_inventory/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/views/asset.py` & `netbox-inventory-1.3.0/netbox_inventory/views/asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,14 @@
                 return redirect(self.get_return_url(request, asset))
             return redirect(asset.get_absolute_url())
         return super().post(request, *args, **kwargs)
 
 
 class AssetBulkImportView(generic.BulkImportView):
     queryset = models.Asset.objects.all()
-    table = tables.AssetTable
     model_form = forms.AssetImportForm
     template_name = 'netbox_inventory/asset_bulk_import.html'
 
 
 class AssetBulkEditView(generic.BulkEditView):
     queryset = models.Asset.objects.all()
     filterset = filtersets.AssetFilterSet
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/views/asset_assign.py` & `netbox-inventory-1.3.0/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/views/asset_create.py` & `netbox-inventory-1.3.0/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/views/asset_reassign.py` & `netbox-inventory-1.3.0/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory/views/inventoryitem_group.py` & `netbox-inventory-1.3.0/netbox_inventory/views/inventoryitem_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,15 @@
 
 
 class InventoryItemGroupDeleteView(generic.ObjectDeleteView):
     queryset = models.InventoryItemGroup.objects.all()
 
 
 class InventoryItemGroupBulkImportView(generic.BulkImportView):
-    queryset = models.InventoryItemGroup.objects.all()   
-    table = tables.InventoryItemGroupTable 
+    queryset = models.InventoryItemGroup.objects.all()
     model_form = forms.InventoryItemGroupImportForm
 
 
 class InventoryItemGroupBulkEditView(generic.BulkEditView):
     queryset = models.InventoryItemGroup.objects.all()
     filterset = filtersets.InventoryItemGroupFilterSet
     table = tables.InventoryItemGroupTable
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/views/inventoryitem_type.py` & `netbox-inventory-1.3.0/netbox_inventory/views/inventoryitem_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 
 
 class InventoryItemTypeDeleteView(generic.ObjectDeleteView):
     queryset = models.InventoryItemType.objects.all()
 
 
 class InventoryItemTypeBulkImportView(generic.BulkImportView):
-    queryset = models.InventoryItemType.objects.all()   
-    table = tables.InventoryItemTypeTable 
+    queryset = models.InventoryItemType.objects.all()
     model_form = forms.InventoryItemTypeImportForm
 
 
 class InventoryItemTypeBulkEditView(generic.BulkEditView):
     queryset = models.InventoryItemType.objects.all()
     filterset = filtersets.InventoryItemTypeFilterSet
     table = tables.InventoryItemTypeTable
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/views/purchase.py` & `netbox-inventory-1.3.0/netbox_inventory/views/purchase.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,16 +45,15 @@
 
 
 class PurchaseDeleteView(generic.ObjectDeleteView):
     queryset = models.Purchase.objects.all()
 
 
 class PurchaseBulkImportView(generic.BulkImportView):
-    queryset = models.Purchase.objects.all()   
-    table = tables.PurchaseTable 
+    queryset = models.Purchase.objects.all()
     model_form = forms.PurchaseImportForm
 
 
 class PurchaseBulkEditView(generic.BulkEditView):
     queryset = models.Purchase.objects.all()
     filterset = filtersets.PurchaseFilterSet
     table = tables.PurchaseTable
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/views/supplier.py` & `netbox-inventory-1.3.0/netbox_inventory/views/supplier.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,15 @@
 
 
 class SupplierDeleteView(generic.ObjectDeleteView):
     queryset = models.Supplier.objects.all()
 
 
 class SupplierBulkImportView(generic.BulkImportView):
-    queryset = models.Supplier.objects.all()   
-    table = tables.SupplierTable 
+    queryset = models.Supplier.objects.all()
     model_form = forms.SupplierImportForm
 
 
 class SupplierBulkEditView(generic.BulkEditView):
     queryset = models.Supplier.objects.all()
     filterset = filtersets.SupplierFilterSet
     table = tables.SupplierTable
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory/views/tabs.py` & `netbox-inventory-1.3.0/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.5/netbox_inventory.egg-info/PKG-INFO` & `netbox-inventory-1.3.0/netbox_inventory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.2.5
+Version: 1.3.0
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -67,21 +67,22 @@
 
 With `asset_disable_editing_fields_for_tags` and `asset_disable_deletion_for_tags` you can prevent changes to specified asset data for assets that have certain tags attached. Changes are only prevented via web interface. API modifications are allowed.
 
 The idea is that an external system uses some assets stored in netbox_inventory, and you want to prevent accidental changes to data directly in NetBox web interface. Only that external system should modify the data.
 
 ## Compatibility
 
-This plugin requires netbox version 3.4.x to work. Older versions of the plugin
+This plugin requires netbox version 3.5.x to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |       3.3      |      1.1.x     |
 |       3.4      |      1.2.x     |
+|       3.5      |      1.3.x     |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
```

### Comparing `netbox-inventory-1.2.5/netbox_inventory.egg-info/SOURCES.txt` & `netbox-inventory-1.3.0/netbox_inventory.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
 netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
 netbox_inventory/templates/netbox_inventory/purchase.html
 netbox_inventory/templates/netbox_inventory/supplier.html
 netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
 netbox_inventory/templates/netbox_inventory/inc/asset_info.html
 netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
-netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html
 netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
 netbox_inventory/tests/__init__.py
 netbox_inventory/tests/custom.py
```

### Comparing `netbox-inventory-1.2.5/pyproject.toml` & `netbox-inventory-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.2.5"
+version = "1.3.0"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

