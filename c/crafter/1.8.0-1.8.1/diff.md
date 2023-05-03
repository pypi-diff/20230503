# Comparing `tmp/crafter-1.8.0.tar.gz` & `tmp/crafter-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crafter-1.8.0.tar", last modified: Thu Feb 10 15:54:13 2022, max compression
+gzip compressed data, was "crafter-1.8.1.tar", last modified: Wed May  3 19:32:11 2023, max compression
```

## Comparing `crafter-1.8.0.tar` & `crafter-1.8.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 danijar  (322066) primarygroup (89939)        0 2022-02-10 15:54:13.979712 crafter-1.8.0/
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1058 2021-12-23 00:21:20.000000 crafter-1.8.0/LICENSE
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     4962 2022-02-10 15:54:13.979241 crafter-1.8.0/PKG-INFO
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     4423 2022-02-10 15:52:45.000000 crafter-1.8.0/README.md
-drwxr-xr-x   0 danijar  (322066) primarygroup (89939)        0 2022-02-10 15:54:13.938180 crafter-1.8.0/crafter/
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      381 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/__init__.py
-drwxr-xr-x   0 danijar  (322066) primarygroup (89939)        0 2022-02-10 15:54:13.978578 crafter-1.8.0/crafter/assets/
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1827 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/1.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1501 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/2.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1559 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/3.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1533 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/4.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1518 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/5.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1567 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/6.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1538 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/7.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1506 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/8.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1535 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/9.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1825 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/arrow-down.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1731 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/arrow-left.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1752 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/arrow-right.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1833 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/arrow-up.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      866 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/coal.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1983 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/cow.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     5735 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/debug-2.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     5762 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/debug-3.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     5761 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/debug.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      839 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/diamond.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2492 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/drink.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2213 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/energy.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2449 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/fence.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2292 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/food.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      910 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/furnace.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      691 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/grass.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2721 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/health.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1048 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/iron.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2354 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/iron_pickaxe.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2390 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/iron_sword.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2130 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/lava.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      755 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/leaves.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      745 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/log.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     7488 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/path.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2154 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/plant-ripe.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2511 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/plant-young.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2080 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/plant.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     6186 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/player-down.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     6195 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/player-left.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     6212 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/player-right.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     6590 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/player-sleep.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     6144 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/player-up.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      813 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/player.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      729 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/sand.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1817 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/sapling.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     5993 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/skeleton.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     7242 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/stone.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2345 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/stone_pickaxe.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2429 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/stone_sword.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      885 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/table.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     7782 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/tree.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2127 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/unknown.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2198 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/water.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1577 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/wood.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2045 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/wood_pickaxe.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2453 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/wood_sword.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2089 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/assets/zombie.png
--rw-r--r--   0 danijar  (322066) primarygroup (89939)      182 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/constants.py
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2632 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/data.yaml
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     8734 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/engine.py
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     6474 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/env.py
--rw-r--r--   0 danijar  (322066) primarygroup (89939)    11408 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/objects.py
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     5272 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/recorder.py
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     4449 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/run_gui.py
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1494 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/run_random.py
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1199 2021-12-23 00:21:20.000000 crafter-1.8.0/crafter/run_terrain.py
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     2966 2022-02-10 15:52:01.000000 crafter-1.8.0/crafter/worldgen.py
-drwxr-xr-x   0 danijar  (322066) primarygroup (89939)        0 2022-02-10 15:54:13.941939 crafter-1.8.0/crafter.egg-info/
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     4962 2022-02-10 15:54:13.000000 crafter-1.8.0/crafter.egg-info/PKG-INFO
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1899 2022-02-10 15:54:13.000000 crafter-1.8.0/crafter.egg-info/SOURCES.txt
--rw-r--r--   0 danijar  (322066) primarygroup (89939)        1 2022-02-10 15:54:13.000000 crafter-1.8.0/crafter.egg-info/dependency_links.txt
--rw-r--r--   0 danijar  (322066) primarygroup (89939)       50 2022-02-10 15:54:13.000000 crafter-1.8.0/crafter.egg-info/entry_points.txt
--rw-r--r--   0 danijar  (322066) primarygroup (89939)       65 2022-02-10 15:54:13.000000 crafter-1.8.0/crafter.egg-info/requires.txt
--rw-r--r--   0 danijar  (322066) primarygroup (89939)        8 2022-02-10 15:54:13.000000 crafter-1.8.0/crafter.egg-info/top_level.txt
--rw-r--r--   0 danijar  (322066) primarygroup (89939)       38 2022-02-10 15:54:13.980015 crafter-1.8.0/setup.cfg
--rw-r--r--   0 danijar  (322066) primarygroup (89939)     1049 2022-02-10 15:53:41.000000 crafter-1.8.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-03 19:32:11.283193 crafter-1.8.1/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2022-12-12 13:23:53.000000 crafter-1.8.1/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4925 2023-05-03 19:32:11.283193 crafter-1.8.1/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4423 2022-12-12 13:23:53.000000 crafter-1.8.1/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-03 19:32:11.279193 crafter-1.8.1/crafter/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      381 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/__init__.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-03 19:32:11.283193 crafter-1.8.1/crafter/assets/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1827 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/1.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1501 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/2.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1559 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/3.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1533 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/4.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1518 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/5.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1567 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/6.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1538 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/7.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1506 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/8.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1535 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/9.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1825 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/arrow-down.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1731 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/arrow-left.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1752 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/arrow-right.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1833 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/arrow-up.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      866 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/coal.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1983 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/cow.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5735 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/debug-2.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5762 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/debug-3.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5761 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/debug.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      839 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/diamond.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2492 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/drink.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2213 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/energy.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2449 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/fence.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2292 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/food.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      910 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/furnace.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      691 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/grass.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2721 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/health.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1048 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/iron.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2354 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/iron_pickaxe.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2390 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/iron_sword.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2130 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/lava.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      755 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/leaves.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      745 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/log.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7488 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/path.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2154 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/plant-ripe.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2511 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/plant-young.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2080 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/plant.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6186 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/player-down.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6195 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/player-left.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6212 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/player-right.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6590 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/player-sleep.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6144 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/player-up.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      813 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/player.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      729 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/sand.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1817 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/sapling.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5993 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/skeleton.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7242 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/stone.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2345 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/stone_pickaxe.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2429 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/stone_sword.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      885 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/table.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7782 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/tree.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2127 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/unknown.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/water.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1577 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/wood.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2045 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/wood_pickaxe.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2453 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/wood_sword.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2089 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/assets/zombie.png
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      182 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/constants.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2632 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/data.yaml
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     8734 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/engine.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6474 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/env.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    11408 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/objects.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5272 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/recorder.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4449 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/run_gui.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1494 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/run_random.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1199 2022-12-12 13:23:53.000000 crafter-1.8.1/crafter/run_terrain.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2963 2023-05-03 19:30:46.000000 crafter-1.8.1/crafter/worldgen.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-03 19:32:11.279193 crafter-1.8.1/crafter.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4925 2023-05-03 19:32:11.000000 crafter-1.8.1/crafter.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1899 2023-05-03 19:32:11.000000 crafter-1.8.1/crafter.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-05-03 19:32:11.000000 crafter-1.8.1/crafter.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       49 2023-05-03 19:32:11.000000 crafter-1.8.1/crafter.egg-info/entry_points.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-05-03 19:32:11.000000 crafter-1.8.1/crafter.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2023-05-03 19:32:11.000000 crafter-1.8.1/crafter.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-05-03 19:32:11.283193 crafter-1.8.1/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      898 2023-05-03 19:31:38.000000 crafter-1.8.1/setup.py
```

### Comparing `crafter-1.8.0/LICENSE` & `crafter-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/PKG-INFO` & `crafter-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: crafter
-Version: 1.8.0
+Version: 1.8.1
 Summary: Open world survival game for reinforcement learning.
 Home-page: http://github.com/danijar/crafter
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: gui
@@ -145,9 +143,7 @@
 <img src="https://github.com/danijar/crafter/raw/main/media/scores.png" width="400"/>
 
 ## Questions
 
 Please [open an issue][issues] on Github.
 
 [issues]: https://github.com/danijar/crafter/issues
-
-
```

### Comparing `crafter-1.8.0/README.md` & `crafter-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/1.png` & `crafter-1.8.1/crafter/assets/1.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/2.png` & `crafter-1.8.1/crafter/assets/2.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/3.png` & `crafter-1.8.1/crafter/assets/3.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/4.png` & `crafter-1.8.1/crafter/assets/4.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/5.png` & `crafter-1.8.1/crafter/assets/5.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/6.png` & `crafter-1.8.1/crafter/assets/6.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/7.png` & `crafter-1.8.1/crafter/assets/7.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/8.png` & `crafter-1.8.1/crafter/assets/8.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/9.png` & `crafter-1.8.1/crafter/assets/9.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/arrow-down.png` & `crafter-1.8.1/crafter/assets/arrow-down.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/arrow-left.png` & `crafter-1.8.1/crafter/assets/arrow-left.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/arrow-right.png` & `crafter-1.8.1/crafter/assets/arrow-right.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/arrow-up.png` & `crafter-1.8.1/crafter/assets/arrow-up.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/coal.png` & `crafter-1.8.1/crafter/assets/coal.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/cow.png` & `crafter-1.8.1/crafter/assets/cow.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/debug-2.png` & `crafter-1.8.1/crafter/assets/debug-2.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/debug-3.png` & `crafter-1.8.1/crafter/assets/debug-3.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/debug.png` & `crafter-1.8.1/crafter/assets/debug.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/diamond.png` & `crafter-1.8.1/crafter/assets/diamond.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/drink.png` & `crafter-1.8.1/crafter/assets/drink.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/energy.png` & `crafter-1.8.1/crafter/assets/energy.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/fence.png` & `crafter-1.8.1/crafter/assets/fence.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/food.png` & `crafter-1.8.1/crafter/assets/food.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/furnace.png` & `crafter-1.8.1/crafter/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/grass.png` & `crafter-1.8.1/crafter/assets/grass.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/health.png` & `crafter-1.8.1/crafter/assets/health.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/iron.png` & `crafter-1.8.1/crafter/assets/iron.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/iron_pickaxe.png` & `crafter-1.8.1/crafter/assets/iron_pickaxe.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/iron_sword.png` & `crafter-1.8.1/crafter/assets/iron_sword.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/lava.png` & `crafter-1.8.1/crafter/assets/lava.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/leaves.png` & `crafter-1.8.1/crafter/assets/leaves.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/log.png` & `crafter-1.8.1/crafter/assets/log.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/path.png` & `crafter-1.8.1/crafter/assets/path.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/plant-ripe.png` & `crafter-1.8.1/crafter/assets/plant-ripe.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/plant-young.png` & `crafter-1.8.1/crafter/assets/plant-young.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/plant.png` & `crafter-1.8.1/crafter/assets/plant.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/player-down.png` & `crafter-1.8.1/crafter/assets/player-down.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/player-left.png` & `crafter-1.8.1/crafter/assets/player-left.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/player-right.png` & `crafter-1.8.1/crafter/assets/player-right.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/player-sleep.png` & `crafter-1.8.1/crafter/assets/player-sleep.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/player-up.png` & `crafter-1.8.1/crafter/assets/player-up.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/player.png` & `crafter-1.8.1/crafter/assets/player.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/sand.png` & `crafter-1.8.1/crafter/assets/sand.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/sapling.png` & `crafter-1.8.1/crafter/assets/sapling.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/skeleton.png` & `crafter-1.8.1/crafter/assets/skeleton.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/stone.png` & `crafter-1.8.1/crafter/assets/stone.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/stone_pickaxe.png` & `crafter-1.8.1/crafter/assets/stone_pickaxe.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/stone_sword.png` & `crafter-1.8.1/crafter/assets/stone_sword.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/table.png` & `crafter-1.8.1/crafter/assets/table.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/tree.png` & `crafter-1.8.1/crafter/assets/tree.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/unknown.png` & `crafter-1.8.1/crafter/assets/unknown.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/water.png` & `crafter-1.8.1/crafter/assets/water.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/wood.png` & `crafter-1.8.1/crafter/assets/wood.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/wood_pickaxe.png` & `crafter-1.8.1/crafter/assets/wood_pickaxe.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/wood_sword.png` & `crafter-1.8.1/crafter/assets/wood_sword.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/assets/zombie.png` & `crafter-1.8.1/crafter/assets/zombie.png`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/data.yaml` & `crafter-1.8.1/crafter/data.yaml`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/engine.py` & `crafter-1.8.1/crafter/engine.py`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/env.py` & `crafter-1.8.1/crafter/env.py`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/objects.py` & `crafter-1.8.1/crafter/objects.py`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/recorder.py` & `crafter-1.8.1/crafter/recorder.py`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/run_gui.py` & `crafter-1.8.1/crafter/run_gui.py`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/run_random.py` & `crafter-1.8.1/crafter/run_random.py`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/run_terrain.py` & `crafter-1.8.1/crafter/run_terrain.py`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/crafter/worldgen.py` & `crafter-1.8.1/crafter/worldgen.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from . import constants
 from . import objects
 
 
 def generate_world(world, player):
   simplex = opensimplex.OpenSimplex(seed=world.random.randint(0, 2 ** 31 - 1))
-  tunnels = np.zeros(world.area, np.bool)
+  tunnels = np.zeros(world.area, bool)
   for x in range(world.area[0]):
     for y in range(world.area[1]):
       _set_material(world, (x, y), player, tunnels, simplex)
   for x in range(world.area[0]):
     for y in range(world.area[1]):
       _set_object(world, (x, y), player, tunnels)
```

### Comparing `crafter-1.8.0/crafter.egg-info/PKG-INFO` & `crafter-1.8.1/crafter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: crafter
-Version: 1.8.0
+Version: 1.8.1
 Summary: Open world survival game for reinforcement learning.
 Home-page: http://github.com/danijar/crafter
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: gui
@@ -145,9 +143,7 @@
 <img src="https://github.com/danijar/crafter/raw/main/media/scores.png" width="400"/>
 
 ## Questions
 
 Please [open an issue][issues] on Github.
 
 [issues]: https://github.com/danijar/crafter/issues
-
-
```

### Comparing `crafter-1.8.0/crafter.egg-info/SOURCES.txt` & `crafter-1.8.1/crafter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crafter-1.8.0/setup.py` & `crafter-1.8.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import setuptools
 import pathlib
 
 
 setuptools.setup(
     name='crafter',
-    version='1.8.0',
+    version='1.8.1',
     description='Open world survival game for reinforcement learning.',
     url='http://github.com/danijar/crafter',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     packages=['crafter'],
     package_data={'crafter': ['data.yaml', 'assets/*']},
     entry_points={'console_scripts': ['crafter=crafter.run_gui:main']},
     install_requires=[
         'numpy', 'imageio', 'pillow', 'opensimplex', 'ruamel.yaml',
-        # Numba is an optional dependency but we want it installed by default
-        # because it speeds up world generation by ~5x.
-        'numba',
     ],
     extras_require={'gui': ['pygame']},
     classifiers=[
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Topic :: Games/Entertainment',
```

