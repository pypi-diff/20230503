# Comparing `tmp/mc_goods-1.1.0.tar.gz` & `tmp/mc_goods-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mc_goods-1.1.0.tar", last modified: Mon Mar 13 16:44:27 2023, max compression
+gzip compressed data, was "mc_goods-1.1.1.tar", last modified: Wed May  3 15:19:07 2023, max compression
```

## Comparing `mc_goods-1.1.0.tar` & `mc_goods-1.1.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:44:27.237847 mc_goods-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:44:27.217847 mc_goods-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:44:27.221847 mc_goods-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-13 16:44:17.000000 mc_goods-1.1.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-13 16:44:17.000000 mc_goods-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-13 16:44:17.000000 mc_goods-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-13 16:44:27.237847 mc_goods-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-13 16:44:17.000000 mc_goods-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:44:27.233847 mc_goods-1.1.0/mc_goods/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-13 16:44:27.000000 mc_goods-1.1.0/mc_goods/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:44:27.237847 mc_goods-1.1.0/mc_goods/boundaries/
--rw-r--r--   0 runner    (1001) docker     (123)    20203 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/cbofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/cbofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14612 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/ciofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/ciofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/creofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    30986 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/creofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/dbofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/dbofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/gfs_1_2deg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/gfs_1_4deg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/gfs_1deg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/gofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/gomofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/gomofs_2ds.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/gomofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/leofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/leofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23873 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/lmhofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/lmhofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/loofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/loofs_fvcom.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/lsofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/lsofs_fvcom.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/ngofs2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/ngofs2_2ds.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/ngofs2_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/nyofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/rtofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/rtofs_2d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/rtofs_ak.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/rtofs_east.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/rtofs_west.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/sfbofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/sfbofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/tbofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/tbofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/wcofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/wcofs_2ds.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/boundaries/wcofs_rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/cbofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/cbofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/ciofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/ciofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/creofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/creofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/dbofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/dbofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/gfs-1-2deg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/gfs-1-4deg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/gfs-1deg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/gofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/gomofs-2ds.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/gomofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/gomofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/leofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/leofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/lmhofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/lmhofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/loofs-fvcom.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/loofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/lsofs-fvcom.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/lsofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/ngofs2-2ds.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/ngofs2-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/ngofs2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/nyofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/rtofs-2d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/rtofs-ak.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/rtofs-east.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/rtofs-west.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/rtofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/sfbofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/sfbofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/tbofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/tbofs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/wcofs-2ds.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/wcofs-rgrid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-03-13 16:44:17.000000 mc_goods-1.1.0/mc_goods/wcofs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:44:27.233847 mc_goods-1.1.0/mc_goods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-13 16:44:27.000000 mc_goods-1.1.0/mc_goods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-13 16:44:27.000000 mc_goods-1.1.0/mc_goods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 16:44:27.000000 mc_goods-1.1.0/mc_goods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-13 16:44:27.000000 mc_goods-1.1.0/mc_goods.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-13 16:44:27.000000 mc_goods-1.1.0/mc_goods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-13 16:44:27.000000 mc_goods-1.1.0/mc_goods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-13 16:44:17.000000 mc_goods-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-13 16:44:27.241847 mc_goods-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-03-13 16:44:17.000000 mc_goods-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:19:07.686267 mc_goods-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:19:07.654266 mc_goods-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:19:07.658267 mc_goods-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-03 15:18:55.000000 mc_goods-1.1.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-03 15:18:55.000000 mc_goods-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 15:18:55.000000 mc_goods-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-03 15:19:07.686267 mc_goods-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-03 15:18:55.000000 mc_goods-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:19:07.670267 mc_goods-1.1.1/mc_goods/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 15:19:07.000000 mc_goods-1.1.1/mc_goods/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:19:07.686267 mc_goods-1.1.1/mc_goods/boundaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    20203 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/cbofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/cbofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14612 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/ciofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/ciofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/creofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    30986 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/creofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/dbofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/dbofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/gfs_1_2deg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/gfs_1_4deg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/gfs_1deg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/gofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/gomofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/gomofs_2ds.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/gomofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/leofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/leofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23873 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/lmhofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/lmhofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/loofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/loofs_fvcom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/lsofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/lsofs_fvcom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/ngofs2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/ngofs2_2ds.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/ngofs2_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/nyofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/rtofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/rtofs_2d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/rtofs_ak.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/rtofs_east.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/rtofs_west.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/sfbofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/sfbofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/tbofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/tbofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/wcofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/wcofs_2ds.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/boundaries/wcofs_rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/cbofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/cbofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/ciofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/ciofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/creofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/creofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/dbofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/dbofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/gfs-1-2deg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/gfs-1-4deg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/gfs-1deg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/gofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/gomofs-2ds.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/gomofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/gomofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/leofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/leofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/lmhofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/lmhofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/loofs-fvcom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/loofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/lsofs-fvcom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/lsofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/ngofs2-2ds.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/ngofs2-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/ngofs2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/nyofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/rtofs-2d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/rtofs-ak.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/rtofs-east.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/rtofs-west.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/rtofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/sfbofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/sfbofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/tbofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/tbofs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/wcofs-2ds.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/wcofs-rgrid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-05-03 15:18:55.000000 mc_goods-1.1.1/mc_goods/wcofs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:19:07.670267 mc_goods-1.1.1/mc_goods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-03 15:19:07.000000 mc_goods-1.1.1/mc_goods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-03 15:19:07.000000 mc_goods-1.1.1/mc_goods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:19:07.000000 mc_goods-1.1.1/mc_goods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-03 15:19:07.000000 mc_goods-1.1.1/mc_goods.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 15:19:07.000000 mc_goods-1.1.1/mc_goods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 15:19:07.000000 mc_goods-1.1.1/mc_goods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-03 15:18:55.000000 mc_goods-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-03 15:19:07.686267 mc_goods-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-03 15:18:55.000000 mc_goods-1.1.1/setup.py
```

### Comparing `mc_goods-1.1.0/.github/workflows/release.yaml` & `mc_goods-1.1.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/.gitignore` & `mc_goods-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/LICENSE.txt` & `mc_goods-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/PKG-INFO` & `mc_goods-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mc_goods
-Version: 1.1.0
+Version: 1.1.1
 Summary: model_catalogs catalogs for GOODS
 Home-page: https://github.com/axiom-data-science/mc-goods
 Author: Axiom Data Science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mc_goods-1.1.0/README.md` & `mc_goods-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/__init__.py` & `mc_goods-1.1.1/mc_goods/__init__.py`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/cbofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/cbofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/cbofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/cbofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/ciofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/ciofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/ciofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/ciofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/creofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/creofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/creofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/creofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/dbofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/dbofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/dbofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/dbofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/gomofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/gomofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/gomofs_2ds.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/gomofs_2ds.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/gomofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/gomofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/leofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/leofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/leofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/leofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/lmhofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/lmhofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/lmhofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/lmhofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/loofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/loofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/loofs_fvcom.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/loofs_fvcom.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/lsofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/lsofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/lsofs_fvcom.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/lsofs_fvcom.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/ngofs2.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/ngofs2.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/ngofs2_2ds.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/ngofs2_2ds.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/ngofs2_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/ngofs2_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/nyofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/nyofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/sfbofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/sfbofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/sfbofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/sfbofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/tbofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/tbofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/tbofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/tbofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/wcofs.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/wcofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/wcofs_2ds.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/wcofs_2ds.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/boundaries/wcofs_rgrid.yaml` & `mc_goods-1.1.1/mc_goods/boundaries/wcofs_rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/cbofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/cbofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/cbofs.yaml` & `mc_goods-1.1.1/mc_goods/cbofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/ciofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/ciofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/ciofs.yaml` & `mc_goods-1.1.1/mc_goods/ciofs.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   filetype: 'fields'
 
 sources:
   coops-forecast-agg:
     driver: opendap
     description: Aggregated 3D Cook Inlet model in ROMS from 7 days ago with 48 hour forecast.
     args:
+      chunks: {}
       drop_variables: ['ocean_time']
       engine: netcdf4
       urlpath: https://opendap.co-ops.nos.noaa.gov/thredds/dodsC/CIOFS/fmrc/Aggregated_7_day_CIOFS_Fields_Forecast_best.ncd
     metadata:
       overall_start_datetime: '7 days before present time'
       overall_end_datetime: '48 hours after present time'
       output_period_(hr): 1
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 Oceanographic_Products_and_Services_(CO-OPS) and the NOAA/National_Weather
 Service/National_Centers_for_Environmental_Prediction_(NCEP)_Central_Operations
 (NCO) using the Regional Ocean Modeling System (ROMS)
 . For detailed model information, visit the NOAA CO-OPS model_information_page.
 grid_dim_(xyz): [724,1044,30] grid_res_min_(km): 0.01 grid_res_max_(km): 3.5
 grid_type: 'curvilinear' alpha_shape: [5,5] # dd, alpha filetype: 'fields'
 sources: coops-forecast-agg: driver: opendap description: Aggregated 3D Cook
-Inlet model in ROMS from 7 days ago with 48 hour forecast. args:
+Inlet model in ROMS from 7 days ago with 48 hour forecast. args: chunks: {}
 drop_variables: ['ocean_time'] engine: netcdf4 urlpath: https://opendap.co-
 ops.nos.noaa.gov/thredds/dodsC/CIOFS/fmrc/
 Aggregated_7_day_CIOFS_Fields_Forecast_best.ncd metadata:
 overall_start_datetime: '7 days before present time' overall_end_datetime: '48
 hours after present time' output_period_(hr): 1 axis: T: time X: [xi_rho, xi_u,
 xi_v, xi_psi] Y: [eta_rho, eta_u, eta_v, eta_psi] Z: [s_rho, s_w]
 standard_names: angle: angle_of_rotation_from_east_to_x
```

### Comparing `mc_goods-1.1.0/mc_goods/creofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/creofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/creofs.yaml` & `mc_goods-1.1.1/mc_goods/creofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/dbofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/dbofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/dbofs.yaml` & `mc_goods-1.1.1/mc_goods/dbofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/gfs-1-2deg.yaml` & `mc_goods-1.1.1/mc_goods/gfs-1-2deg.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/gfs-1-4deg.yaml` & `mc_goods-1.1.1/mc_goods/gfs-1-4deg.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/gfs-1deg.yaml` & `mc_goods-1.1.1/mc_goods/gfs-1deg.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/gofs.yaml` & `mc_goods-1.1.1/mc_goods/gofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/gomofs-2ds.yaml` & `mc_goods-1.1.1/mc_goods/gomofs-2ds.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/gomofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/gomofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/gomofs.yaml` & `mc_goods-1.1.1/mc_goods/gomofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/leofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/leofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/leofs.yaml` & `mc_goods-1.1.1/mc_goods/leofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/lmhofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/lmhofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/lmhofs.yaml` & `mc_goods-1.1.1/mc_goods/lmhofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/loofs-fvcom.yaml` & `mc_goods-1.1.1/mc_goods/loofs-fvcom.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/loofs.yaml` & `mc_goods-1.1.1/mc_goods/loofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/lsofs-fvcom.yaml` & `mc_goods-1.1.1/mc_goods/lsofs-fvcom.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/lsofs.yaml` & `mc_goods-1.1.1/mc_goods/lsofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/ngofs2-2ds.yaml` & `mc_goods-1.1.1/mc_goods/ngofs2-2ds.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/ngofs2-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/ngofs2-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/ngofs2.yaml` & `mc_goods-1.1.1/mc_goods/ngofs2.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/nyofs.yaml` & `mc_goods-1.1.1/mc_goods/nyofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/rtofs-2d.yaml` & `mc_goods-1.1.1/mc_goods/rtofs-2d.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/rtofs-ak.yaml` & `mc_goods-1.1.1/mc_goods/rtofs-ak.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/rtofs-east.yaml` & `mc_goods-1.1.1/mc_goods/rtofs-east.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/rtofs-west.yaml` & `mc_goods-1.1.1/mc_goods/rtofs-west.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/rtofs.yaml` & `mc_goods-1.1.1/mc_goods/rtofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/sfbofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/sfbofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/sfbofs.yaml` & `mc_goods-1.1.1/mc_goods/sfbofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/tbofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/tbofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/tbofs.yaml` & `mc_goods-1.1.1/mc_goods/tbofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/wcofs-2ds.yaml` & `mc_goods-1.1.1/mc_goods/wcofs-2ds.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/wcofs-rgrid.yaml` & `mc_goods-1.1.1/mc_goods/wcofs-rgrid.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods/wcofs.yaml` & `mc_goods-1.1.1/mc_goods/wcofs.yaml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods.egg-info/PKG-INFO` & `mc_goods-1.1.1/mc_goods.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mc-goods
-Version: 1.1.0
+Version: 1.1.1
 Summary: model_catalogs catalogs for GOODS
 Home-page: https://github.com/axiom-data-science/mc-goods
 Author: Axiom Data Science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mc_goods-1.1.0/mc_goods.egg-info/SOURCES.txt` & `mc_goods-1.1.1/mc_goods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/mc_goods.egg-info/entry_points.txt` & `mc_goods-1.1.1/mc_goods.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/pyproject.toml` & `mc_goods-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/setup.cfg` & `mc_goods-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mc_goods-1.1.0/setup.py` & `mc_goods-1.1.1/setup.py`

 * *Files identical despite different names*

