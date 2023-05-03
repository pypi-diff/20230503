# Comparing `tmp/ramo-0.1.2.tar.gz` & `tmp/ramo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramo-0.1.2.tar", last modified: Tue Jan  3 07:26:37 2023, max compression
+gzip compressed data, was "ramo-0.1.3.tar", last modified: Wed May  3 13:54:12 2023, max compression
```

## Comparing `ramo-0.1.2.tar` & `ramo-0.1.3.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.326948 ramo-0.1.2/
--rw-r--r--   0 willemropke   (501) staff       (20)     1069 2022-02-22 16:22:09.000000 ramo-0.1.2/LICENSE
--rw-r--r--   0 willemropke   (501) staff       (20)     1982 2023-01-03 07:26:37.326765 ramo-0.1.2/PKG-INFO
--rw-r--r--   0 willemropke   (501) staff       (20)     1564 2022-08-01 07:04:47.000000 ramo-0.1.2/README.md
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.315088 ramo-0.1.2/ramo/
--rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:07:15.000000 ramo-0.1.2/ramo/__init__.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.317606 ramo-0.1.2/ramo/commitment/
--rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:08:43.000000 ramo-0.1.2/ramo/commitment/__init__.py
--rw-r--r--   0 willemropke   (501) staff       (20)     7113 2022-10-31 15:21:47.000000 ramo-0.1.2/ramo/commitment/best_response.py
--rw-r--r--   0 willemropke   (501) staff       (20)     6100 2022-10-31 15:24:20.000000 ramo-0.1.2/ramo/commitment/comp_action.py
--rw-r--r--   0 willemropke   (501) staff       (20)     6238 2022-10-31 15:21:47.000000 ramo-0.1.2/ramo/commitment/coop_action.py
--rw-r--r--   0 willemropke   (501) staff       (20)     5684 2022-10-31 15:21:47.000000 ramo-0.1.2/ramo/commitment/coop_policy.py
--rw-r--r--   0 willemropke   (501) staff       (20)     7979 2022-11-28 17:57:14.000000 ramo-0.1.2/ramo/commitment/execute_commitment.py
--rw-r--r--   0 willemropke   (501) staff       (20)     7516 2022-10-31 15:21:47.000000 ramo-0.1.2/ramo/commitment/non_stationary.py
--rw-r--r--   0 willemropke   (501) staff       (20)     4675 2022-10-31 15:24:49.000000 ramo-0.1.2/ramo/commitment/optional_com.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.318787 ramo-0.1.2/ramo/game/
--rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-04-14 08:47:26.000000 ramo-0.1.2/ramo/game/__init__.py
--rw-r--r--   0 willemropke   (501) staff       (20)      785 2022-11-28 17:57:14.000000 ramo-0.1.2/ramo/game/checking.py
--rw-r--r--   0 willemropke   (501) staff       (20)    11641 2022-11-28 18:43:06.000000 ramo-0.1.2/ramo/game/example_games.py
--rw-r--r--   0 willemropke   (501) staff       (20)    10124 2022-11-28 18:07:54.000000 ramo-0.1.2/ramo/game/generators.py
--rw-r--r--   0 willemropke   (501) staff       (20)     1224 2022-12-20 14:26:22.000000 ramo-0.1.2/ramo/game/monfg.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.320438 ramo-0.1.2/ramo/learner/
--rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:08:56.000000 ramo-0.1.2/ramo/learner/__init__.py
--rw-r--r--   0 willemropke   (501) staff       (20)     6089 2022-11-28 18:50:40.000000 ramo-0.1.2/ramo/learner/execute_learner.py
--rw-r--r--   0 willemropke   (501) staff       (20)     3347 2022-10-31 15:25:07.000000 ramo-0.1.2/ramo/learner/indep_actor_critic.py
--rw-r--r--   0 willemropke   (501) staff       (20)     2599 2022-11-09 13:56:04.000000 ramo-0.1.2/ramo/learner/indep_q.py
--rw-r--r--   0 willemropke   (501) staff       (20)     3991 2022-10-31 15:21:47.000000 ramo-0.1.2/ramo/learner/ja_actor_critic.py
--rw-r--r--   0 willemropke   (501) staff       (20)     3435 2022-10-31 15:21:47.000000 ramo-0.1.2/ramo/learner/ja_q.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.321949 ramo-0.1.2/ramo/nash/
--rw-r--r--   0 willemropke   (501) staff       (20)     4094 2022-11-28 18:07:54.000000 ramo-0.1.2/ramo/nash/IBR.py
--rw-r--r--   0 willemropke   (501) staff       (20)     6099 2022-10-31 15:21:47.000000 ramo-0.1.2/ramo/nash/Player.py
--rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:07:23.000000 ramo-0.1.2/ramo/nash/__init__.py
--rw-r--r--   0 willemropke   (501) staff       (20)     6040 2022-11-28 18:49:59.000000 ramo-0.1.2/ramo/nash/fictitious_play.py
--rw-r--r--   0 willemropke   (501) staff       (20)     4001 2022-11-28 18:07:54.000000 ramo-0.1.2/ramo/nash/moqups.py
--rw-r--r--   0 willemropke   (501) staff       (20)      965 2022-11-28 18:20:06.000000 ramo-0.1.2/ramo/nash/mose.py
--rw-r--r--   0 willemropke   (501) staff       (20)     2676 2022-11-28 18:20:06.000000 ramo-0.1.2/ramo/nash/verify.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.322735 ramo-0.1.2/ramo/pareto/
--rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-10-31 14:59:38.000000 ramo-0.1.2/ramo/pareto/__init__.py
--rw-r--r--   0 willemropke   (501) staff       (20)      696 2022-11-28 18:20:06.000000 ramo-0.1.2/ramo/pareto/pareto_nash.py
--rw-r--r--   0 willemropke   (501) staff       (20)     6221 2023-01-02 19:18:31.000000 ramo-0.1.2/ramo/pareto/verify.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.323314 ramo-0.1.2/ramo/printing/
--rw-r--r--   0 willemropke   (501) staff       (20)      238 2022-10-31 15:32:57.000000 ramo-0.1.2/ramo/printing/__init__.py
--rw-r--r--   0 willemropke   (501) staff       (20)     5732 2022-11-29 11:20:42.000000 ramo-0.1.2/ramo/printing/printing.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.324436 ramo-0.1.2/ramo/strategy/
--rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-10-31 14:51:11.000000 ramo-0.1.2/ramo/strategy/__init__.py
--rw-r--r--   0 willemropke   (501) staff       (20)     8537 2022-11-09 13:55:58.000000 ramo-0.1.2/ramo/strategy/best_response.py
--rw-r--r--   0 willemropke   (501) staff       (20)     7677 2022-11-28 09:13:03.000000 ramo-0.1.2/ramo/strategy/operations.py
--rw-r--r--   0 willemropke   (501) staff       (20)      396 2022-10-31 14:58:13.000000 ramo-0.1.2/ramo/strategy/strategies.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.325334 ramo-0.1.2/ramo/utility_function/
--rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-04-14 08:43:00.000000 ramo-0.1.2/ramo/utility_function/__init__.py
--rw-r--r--   0 willemropke   (501) staff       (20)     1678 2022-06-17 14:34:13.000000 ramo-0.1.2/ramo/utility_function/checking.py
--rw-r--r--   0 willemropke   (501) staff       (20)     3280 2022-04-14 08:44:48.000000 ramo-0.1.2/ramo/utility_function/functions.py
--rw-r--r--   0 willemropke   (501) staff       (20)      285 2022-10-31 15:21:47.000000 ramo-0.1.2/ramo/utility_function/generators.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.326502 ramo-0.1.2/ramo/utils/
--rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:12:34.000000 ramo-0.1.2/ramo/utils/__init__.py
--rw-r--r--   0 willemropke   (501) staff       (20)     8994 2022-08-01 07:44:59.000000 ramo-0.1.2/ramo/utils/agent_loader.py
--rw-r--r--   0 willemropke   (501) staff       (20)     1453 2022-06-27 12:40:46.000000 ramo-0.1.2/ramo/utils/data.py
--rw-r--r--   0 willemropke   (501) staff       (20)     3102 2022-06-02 08:11:32.000000 ramo-0.1.2/ramo/utils/experiments.py
--rw-r--r--   0 willemropke   (501) staff       (20)      652 2022-10-31 15:02:55.000000 ramo-0.1.2/ramo/utils/helpers.py
-drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-01-03 07:26:37.315613 ramo-0.1.2/ramo.egg-info/
--rw-r--r--   0 willemropke   (501) staff       (20)     1982 2023-01-03 07:26:36.000000 ramo-0.1.2/ramo.egg-info/PKG-INFO
--rw-r--r--   0 willemropke   (501) staff       (20)     1336 2023-01-03 07:26:37.000000 ramo-0.1.2/ramo.egg-info/SOURCES.txt
--rw-r--r--   0 willemropke   (501) staff       (20)        1 2023-01-03 07:26:36.000000 ramo-0.1.2/ramo.egg-info/dependency_links.txt
--rw-r--r--   0 willemropke   (501) staff       (20)        5 2023-01-03 07:26:37.000000 ramo-0.1.2/ramo.egg-info/top_level.txt
--rw-r--r--   0 willemropke   (501) staff       (20)       38 2023-01-03 07:26:37.326996 ramo-0.1.2/setup.cfg
--rw-r--r--   0 willemropke   (501) staff       (20)      971 2023-01-03 07:23:21.000000 ramo-0.1.2/setup.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.889277 ramo-0.1.3/
+-rw-r--r--   0 willemropke   (501) staff       (20)     1069 2022-02-22 16:22:09.000000 ramo-0.1.3/LICENSE
+-rw-r--r--   0 willemropke   (501) staff       (20)     1982 2023-05-03 13:54:12.889108 ramo-0.1.3/PKG-INFO
+-rw-r--r--   0 willemropke   (501) staff       (20)     1564 2022-08-01 07:04:47.000000 ramo-0.1.3/README.md
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.875955 ramo-0.1.3/ramo/
+-rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:07:15.000000 ramo-0.1.3/ramo/__init__.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.878623 ramo-0.1.3/ramo/commitment/
+-rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:08:43.000000 ramo-0.1.3/ramo/commitment/__init__.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     7113 2022-10-31 15:21:47.000000 ramo-0.1.3/ramo/commitment/best_response.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     6100 2022-10-31 15:24:20.000000 ramo-0.1.3/ramo/commitment/comp_action.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     6238 2022-10-31 15:21:47.000000 ramo-0.1.3/ramo/commitment/coop_action.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     5684 2022-10-31 15:21:47.000000 ramo-0.1.3/ramo/commitment/coop_policy.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     7979 2022-11-28 17:57:14.000000 ramo-0.1.3/ramo/commitment/execute_commitment.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     7516 2022-10-31 15:21:47.000000 ramo-0.1.3/ramo/commitment/non_stationary.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     4675 2022-10-31 15:24:49.000000 ramo-0.1.3/ramo/commitment/optional_com.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.881039 ramo-0.1.3/ramo/game/
+-rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-04-14 08:47:26.000000 ramo-0.1.3/ramo/game/__init__.py
+-rw-r--r--   0 willemropke   (501) staff       (20)      785 2022-11-28 17:57:14.000000 ramo-0.1.3/ramo/game/checking.py
+-rw-r--r--   0 willemropke   (501) staff       (20)    11641 2022-11-28 18:43:06.000000 ramo-0.1.3/ramo/game/example_games.py
+-rw-r--r--   0 willemropke   (501) staff       (20)    10032 2023-02-23 09:44:43.000000 ramo-0.1.3/ramo/game/generators.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     1224 2022-12-20 14:26:22.000000 ramo-0.1.3/ramo/game/monfg.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.882493 ramo-0.1.3/ramo/learner/
+-rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:08:56.000000 ramo-0.1.3/ramo/learner/__init__.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     6089 2022-11-28 18:50:40.000000 ramo-0.1.3/ramo/learner/execute_learner.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     3347 2022-10-31 15:25:07.000000 ramo-0.1.3/ramo/learner/indep_actor_critic.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     2599 2022-11-09 13:56:04.000000 ramo-0.1.3/ramo/learner/indep_q.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     3991 2022-10-31 15:21:47.000000 ramo-0.1.3/ramo/learner/ja_actor_critic.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     3435 2022-10-31 15:21:47.000000 ramo-0.1.3/ramo/learner/ja_q.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.883966 ramo-0.1.3/ramo/nash/
+-rw-r--r--   0 willemropke   (501) staff       (20)     4094 2022-11-28 18:07:54.000000 ramo-0.1.3/ramo/nash/IBR.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     6099 2022-10-31 15:21:47.000000 ramo-0.1.3/ramo/nash/Player.py
+-rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:07:23.000000 ramo-0.1.3/ramo/nash/__init__.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     6040 2022-11-28 18:49:59.000000 ramo-0.1.3/ramo/nash/fictitious_play.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     4001 2022-11-28 18:07:54.000000 ramo-0.1.3/ramo/nash/moqups.py
+-rw-r--r--   0 willemropke   (501) staff       (20)      965 2022-11-28 18:20:06.000000 ramo-0.1.3/ramo/nash/mose.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     2676 2022-11-28 18:20:06.000000 ramo-0.1.3/ramo/nash/verify.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.885119 ramo-0.1.3/ramo/pareto/
+-rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-10-31 14:59:38.000000 ramo-0.1.3/ramo/pareto/__init__.py
+-rw-r--r--   0 willemropke   (501) staff       (20)      683 2023-05-03 11:43:04.000000 ramo-0.1.3/ramo/pareto/dominance.py
+-rw-r--r--   0 willemropke   (501) staff       (20)      696 2022-11-28 18:20:06.000000 ramo-0.1.3/ramo/pareto/pareto_nash.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     7083 2023-05-03 13:19:53.000000 ramo-0.1.3/ramo/pareto/verify.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.885540 ramo-0.1.3/ramo/printing/
+-rw-r--r--   0 willemropke   (501) staff       (20)      238 2022-10-31 15:32:57.000000 ramo-0.1.3/ramo/printing/__init__.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     5732 2022-11-29 11:20:42.000000 ramo-0.1.3/ramo/printing/printing.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.886560 ramo-0.1.3/ramo/strategy/
+-rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-10-31 14:51:11.000000 ramo-0.1.3/ramo/strategy/__init__.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     8096 2023-02-22 12:02:48.000000 ramo-0.1.3/ramo/strategy/best_response.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     7677 2022-11-28 09:13:03.000000 ramo-0.1.3/ramo/strategy/operations.py
+-rw-r--r--   0 willemropke   (501) staff       (20)      396 2022-10-31 14:58:13.000000 ramo-0.1.3/ramo/strategy/strategies.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.887371 ramo-0.1.3/ramo/utility_function/
+-rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-04-14 08:43:00.000000 ramo-0.1.3/ramo/utility_function/__init__.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     1678 2022-06-17 14:34:13.000000 ramo-0.1.3/ramo/utility_function/checking.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     3280 2022-04-14 08:44:48.000000 ramo-0.1.3/ramo/utility_function/functions.py
+-rw-r--r--   0 willemropke   (501) staff       (20)      285 2022-10-31 15:21:47.000000 ramo-0.1.3/ramo/utility_function/generators.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.888496 ramo-0.1.3/ramo/utils/
+-rw-r--r--   0 willemropke   (501) staff       (20)        0 2022-03-11 15:12:34.000000 ramo-0.1.3/ramo/utils/__init__.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     8994 2022-08-01 07:44:59.000000 ramo-0.1.3/ramo/utils/agent_loader.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     1453 2022-06-27 12:40:46.000000 ramo-0.1.3/ramo/utils/data.py
+-rw-r--r--   0 willemropke   (501) staff       (20)     3102 2022-06-02 08:11:32.000000 ramo-0.1.3/ramo/utils/experiments.py
+-rw-r--r--   0 willemropke   (501) staff       (20)      652 2022-10-31 15:02:55.000000 ramo-0.1.3/ramo/utils/helpers.py
+drwxr-xr-x   0 willemropke   (501) staff       (20)        0 2023-05-03 13:54:12.876515 ramo-0.1.3/ramo.egg-info/
+-rw-r--r--   0 willemropke   (501) staff       (20)     1982 2023-05-03 13:54:12.000000 ramo-0.1.3/ramo.egg-info/PKG-INFO
+-rw-r--r--   0 willemropke   (501) staff       (20)     1361 2023-05-03 13:54:12.000000 ramo-0.1.3/ramo.egg-info/SOURCES.txt
+-rw-r--r--   0 willemropke   (501) staff       (20)        1 2023-05-03 13:54:12.000000 ramo-0.1.3/ramo.egg-info/dependency_links.txt
+-rw-r--r--   0 willemropke   (501) staff       (20)        5 2023-05-03 13:54:12.000000 ramo-0.1.3/ramo.egg-info/top_level.txt
+-rw-r--r--   0 willemropke   (501) staff       (20)       38 2023-05-03 13:54:12.889331 ramo-0.1.3/setup.cfg
+-rw-r--r--   0 willemropke   (501) staff       (20)      971 2023-05-03 13:53:36.000000 ramo-0.1.3/setup.py
```

### Comparing `ramo-0.1.2/LICENSE` & `ramo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/PKG-INFO` & `ramo-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Algorithms for computing or learning equilibria in multi-objective games
 Author: Willem Röpke
 Author-email: willem.ropke@vub.be
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `ramo-0.1.2/README.md` & `ramo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/commitment/best_response.py` & `ramo-0.1.3/ramo/commitment/best_response.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/commitment/comp_action.py` & `ramo-0.1.3/ramo/commitment/comp_action.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/commitment/coop_action.py` & `ramo-0.1.3/ramo/commitment/coop_action.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/commitment/coop_policy.py` & `ramo-0.1.3/ramo/commitment/coop_policy.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/commitment/execute_commitment.py` & `ramo-0.1.3/ramo/commitment/execute_commitment.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/commitment/non_stationary.py` & `ramo-0.1.3/ramo/commitment/non_stationary.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/commitment/optional_com.py` & `ramo-0.1.3/ramo/commitment/optional_com.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/game/checking.py` & `ramo-0.1.3/ramo/game/checking.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/game/example_games.py` & `ramo-0.1.3/ramo/game/example_games.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/game/generators.py` & `ramo-0.1.3/ramo/game/generators.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,41 +71,45 @@
     for _ in range(len(player_actions)):
         payoff_matrix = rng.normal(loc=mean, scale=std, size=payoffs_shape)
         payoffs.append(payoff_matrix)
 
     return MONFG(payoffs)
 
 
-def covariance_monfg(player_actions=(2, 2), num_objectives=2, mean=0, std=1, rho=0, rng=None):
+def covariant_monfg(player_actions, num_objectives=2, mean=0, std=1, cov=0, rng=None):
     """Generate a random MONFG with payoffs from a normal distribution and given covariance.
 
     Args:
         player_actions (Tuple[int], optional): A tuple of actions indexed by player. (Default value = (2, 2))
         num_objectives (int, optional): The number of objectives in the game. (Default value = 2)
         mean (float, optional): The mean of the normal distribution. (Default value = 0)
         std (float, optional): The standard deviation of the normal distribution. (Default value = 1)
-        rho (float, optional): The covariance between the players. (Default value = 0)
+        cov (float, optional): The covariance between the players. (Default value = 0)
         rng (Generator, optional): A random number generator. (Default value = None)
 
     Returns:
         MONFG: The generated MONFG.
     """
-    rng = rng if rng is not None else np.random.default_rng()
     num_players = len(player_actions)
-    mean_arr = np.full(num_players, mean)
-    std_arr = np.full(num_players, std)
-    cov_matrix = np.full((num_players, num_players), rho)
-    np.fill_diagonal(cov_matrix, std_arr)
-    payoffs_shape = player_actions + tuple([num_objectives])  # Define the shape of the payoff matrices.
-    all_payoffs = rng.multivariate_normal(mean_arr, cov_matrix, payoffs_shape)
-    payoffs = [all_payoffs[..., -1:].reshape(payoffs_shape)]  # Set payoffs for the first player
-    for player in range(1, num_players):
-        player_payoffs = all_payoffs[..., -player - 1:-player].reshape(payoffs_shape)
-        payoffs.append(player_payoffs)
-    return MONFG(payoffs)
+    rng = rng if rng is not None else np.random.default_rng()
+
+    if type(mean) == int or type(mean) == float:
+        mean = np.full(num_players, mean)
+        cov = np.full((num_players, num_players), cov)
+        np.fill_diagonal(cov, std)
+
+    num_payoffs = np.prod(player_actions) * num_objectives
+
+    player_payoffs = rng.multivariate_normal(mean, cov, size=num_payoffs)
+    payoff_matrices = np.expand_dims(player_payoffs, -1).swapaxes(0, 1).reshape(
+        (num_players, *player_actions, num_objectives))
+    if num_objectives == 1:
+        payoff_matrices = payoff_matrices.squeeze(-1)
+
+    return MONFG(payoff_matrices)
 
 
 def identity_game(player_actions):
     """Generate an identity game.
 
     Args:
         player_actions (Tuple[int]): A tuple of actions indexed by player.
```

### Comparing `ramo-0.1.2/ramo/game/monfg.py` & `ramo-0.1.3/ramo/game/monfg.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/learner/execute_learner.py` & `ramo-0.1.3/ramo/learner/execute_learner.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/learner/indep_actor_critic.py` & `ramo-0.1.3/ramo/learner/indep_actor_critic.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/learner/indep_q.py` & `ramo-0.1.3/ramo/learner/indep_q.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/learner/ja_actor_critic.py` & `ramo-0.1.3/ramo/learner/ja_actor_critic.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/learner/ja_q.py` & `ramo-0.1.3/ramo/learner/ja_q.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/nash/IBR.py` & `ramo-0.1.3/ramo/nash/IBR.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/nash/Player.py` & `ramo-0.1.3/ramo/nash/Player.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/nash/fictitious_play.py` & `ramo-0.1.3/ramo/nash/fictitious_play.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/nash/moqups.py` & `ramo-0.1.3/ramo/nash/moqups.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/nash/mose.py` & `ramo-0.1.3/ramo/nash/mose.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/nash/verify.py` & `ramo-0.1.3/ramo/nash/verify.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/pareto/pareto_nash.py` & `ramo-0.1.3/ramo/pareto/pareto_nash.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/pareto/verify.py` & `ramo-0.1.3/ramo/pareto/verify.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
-import scipy.optimize as scopt
+from scipy.optimize import linprog, OptimizeWarning
+from scipy.spatial import ConvexHull
 from pulp import *
 
 from ramo.strategy.best_response import calc_expected_returns
+from ramo.pareto.dominance import pareto_dominates
 
 
 def in_hull(x, points):
     """Check whether a point is a convex combination of a set of points.
 
     Args:
         x (ndarray): The point to check.
@@ -16,19 +18,61 @@
         bool: Whether the point was in the convex hull.
     """
     n_points = len(points)  # The number of points.
     c = np.zeros(n_points)  # Make an array of zeros of this size as the objective to minimise.
     A = np.r_[points.T, np.ones((1, n_points))]  # Add row of ones such that the strategy sums to 1.
     b = np.r_[x, np.ones(1)]  # The strategy array.
     with warnings.catch_warnings():
-        warnings.filterwarnings('ignore', category=scopt.OptimizeWarning)  # Suppress full row rank warnings.
-        lp = scopt.linprog(c, A_eq=A, b_eq=b)  # Check if we can find a convex combination by linear programming.
+        warnings.filterwarnings('ignore', category=OptimizeWarning)  # Suppress full row rank warnings.
+        lp = linprog(c, A_eq=A, b_eq=b)  # Check if we can find a convex combination by linear programming.
     return lp.success
 
 
+def find_weight(vector, candidates):
+    """Find a weight for which a specific vector improves on a CCS [1].
+
+    References:
+        .. [1] Roijers, D. M., & Whiteson, S. (2017). Multi-objective decision making. 34, 129–129.
+            https://doi.org/10.2200/S00765ED1V01Y201704AIM034
+
+    Args:
+        vector (Tuple): A payoff vector.
+        candidates (Set[Tuple]): The current CCS.
+
+    Returns:
+        ndarray | None: A weight array if it found one, otherwise None.
+    """
+    candidates = list(candidates)
+    num_objectives = len(candidates[0])
+
+    problem = LpProblem('findWeight', LpMaximize)
+    x = LpVariable('x')
+    w = []
+
+    for obj in range(num_objectives):  # Make weight decision variables.
+        w.append(LpVariable(f'w{obj}', 0, 1))
+
+    for candidate in candidates:  # Add the constraints on the improvement of w.
+        diff = list(np.subtract(vector, candidate))
+        problem += lpDot(w, diff) - x >= 0
+
+    problem += lpSum(w) == 1  # Weights should sum to one.
+    problem += x  # Add x as the objective to maximise.
+    success = problem.solve(solver=PULP_CBC_CMD(msg=False))  # Solve the problem.
+    x = problem.objective.value()  # Get the objective value.
+    weight_vec = np.zeros(num_objectives)
+    for var in problem.variables():  # Get the weight values.
+        if var.name[0] == 'w':
+            weight_idx = int(var.name[-1])
+            weight_vec[weight_idx] = var.value()
+    if success and x > 0:
+        return weight_vec
+    return None
+
+
 def c_prune(candidates):
     """Create a convex coverage set from a set of candidate points.
 
     References:
         .. [1] Roijers, D. M., & Whiteson, S. (2017). Multi-objective decision making. 34, 129–129.
             https://doi.org/10.2200/S00765ED1V01Y201704AIM034
 
@@ -56,29 +100,14 @@
             p_candidates.remove(new_vector)
             ccs.add(new_vector)
 
     ccs.remove(zero_vec)
     return ccs
 
 
-def pareto_dominates(a, b):
-    """Check if the vector in a Pareto dominates vector b.
-
-    Args:
-        a (ndarray): A numpy array.
-        b (ndarray): A numpy array.
-
-    Returns:
-        bool: Whether vector a dominates vector b.
-    """
-    a = np.array(a)
-    b = np.array(b)
-    return np.all(a >= b) and np.any(a > b)
-
-
 def p_prune(candidates):
     """Create a Pareto coverage set from a set of candidate points.
 
     References:
         .. [1] Roijers, D. M., & Whiteson, S. (2017). Multi-objective decision making. 34, 129–129.
             https://doi.org/10.2200/S00765ED1V01Y201704AIM034
 
@@ -87,66 +116,63 @@
 
     Returns:
         Set[Tuple]: A Pareto coverage set.
     """
     pcs = set()
     while candidates:
         vector = candidates.pop()
-        to_remove = set(vector)
+
         for alternative in candidates:
             if pareto_dominates(alternative, vector):
                 vector = alternative
-                to_remove.add(alternative)
+
+        to_remove = set(vector)
+        for alternative in candidates:
             if pareto_dominates(vector, alternative):
                 to_remove.add(alternative)
+
         candidates -= to_remove
         pcs.add(vector)
     return pcs
 
 
-def find_weight(vector, candidates):
-    """Find a weight for which a specific vector improves on a CCS [1].
+def fast_c_prune(candidates):
+    """A fast version to prune a set of points to its convex hull. This leverages the QuickHull algorithm.
 
-    References:
-        .. [1] Roijers, D. M., & Whiteson, S. (2017). Multi-objective decision making. 34, 129–129.
-            https://doi.org/10.2200/S00765ED1V01Y201704AIM034
+    This algorithm first computes the convex hull of the set of points and then prunes the Pareto dominated points.
 
     Args:
-        vector (Tuple): A payoff vector.
-        candidates (Set[Tuple]): The current CCS.
+        candidates (ndarray): A numpy array of vectors.
 
     Returns:
-        ndarray | None: A weight array if it found one, otherwise None.
+        ndarray: A convex coverage set.
     """
-    candidates = list(candidates)
-    num_objectives = len(candidates[0])
+    hull = ConvexHull(candidates)
+    ccs = candidates[hull.vertices]
+    return fast_p_prune(ccs)
 
-    problem = LpProblem('findWeight', LpMaximize)
-    x = LpVariable('x')
-    w = []
 
-    for obj in range(num_objectives):  # Make weight decision variables.
-        w.append(LpVariable(f'w{obj}', 0, 1))
+def fast_p_prune(candidates):
+    """A batched and fast version of the Pareto coverage set algorithm.
 
-    for candidate in candidates:  # Add the constraints on the improvement of w.
-        diff = list(np.subtract(vector, candidate))
-        problem += lpDot(w, diff) - x >= 0
+    Args:
+        candidates (ndarray): A numpy array of vectors.
 
-    problem += lpSum(w) == 1  # Weights should sum to one.
-    problem += x  # Add x as the objective to maximise.
-    success = problem.solve(solver=PULP_CBC_CMD(msg=False))  # Solve the problem.
-    x = problem.objective.value()  # Get the objective value.
-    weight_vec = np.zeros(num_objectives)
-    for var in problem.variables():  # Get the weight values.
-        if var.name[0] == 'w':
-            weight_idx = int(var.name[-1])
-            weight_vec[weight_idx] = var.value()
-    if success and x > 0:
-        return weight_vec
-    return None
+    Returns:
+        ndarray: A Pareto coverage set.
+    """
+    candidates = np.unique(candidates, axis=0)
+    if len(candidates) == 1:
+        return candidates
+
+    res_eq = np.all(candidates[:, None, None] <= candidates, axis=-1).squeeze()
+    res_g = np.all(candidates[:, None, None] < candidates, axis=-1).squeeze()
+    c1 = np.sum(res_eq, axis=-1) == 1
+    c2 = np.any(~res_g, axis=-1)
+    return candidates[np.logical_and(c1, c2)]
 
 
 def verify_pareto_nash(monfg, joint_strat):
     """Verify whether a joint strategy is a Pareto Nash equilibrium.
 
     Args:
         monfg (MONFG): An MONFG object.
```

### Comparing `ramo-0.1.2/ramo/printing/printing.py` & `ramo-0.1.3/ramo/printing/printing.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/strategy/best_response.py` & `ramo-0.1.3/ramo/strategy/best_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,38 +101,31 @@
         payoff_matrix (ndarray): The payoff matrix for the given player.
         joint_strategy (List[ndarray]): A list of each player's individual strategy.
 
     Returns:
         ndarray: The expected returns for the given player's actions.
 
     """
-    num_objectives = payoff_matrix.shape[-1]
-    num_actions = len(joint_strategy[player])
-    num_players = len(joint_strategy)
-    opponents = np.delete(np.arange(num_players), player)
+    opponents = [i for i in range(len(joint_strategy)) if i != player]
     expected_returns = payoff_matrix
 
     for opponent in opponents:  # Loop over all opponent strategies.
         strategy = joint_strategy[opponent]  # Get this opponent's strategy.
 
         # We reshape this strategy to be able to multiply along the correct axis for weighting expected returns.
         # For example if you end up in [1, 2] or [2, 3] with 50% probability.
         # We calculate the individual expected returns first: [0.5, 1] or [1, 1.5]
-        dim_array = np.ones((1, expected_returns.ndim), int).ravel()
+        dim_array = [1] * expected_returns.ndim
         dim_array[opponent] = -1
         strategy_reshaped = strategy.reshape(dim_array)
 
         expected_returns = expected_returns * strategy_reshaped  # Calculate the probability of a joint state occurring.
-        # We now take the sum of the weighted returns to get the expected returns.
-        # We need keepdims=True to make sure that the opponent still exists at the correct axis, their action space is
-        # just reduced to one action resulting in the expected return now.
-        expected_returns = np.sum(expected_returns, axis=opponent, keepdims=True)
-
-    expected_returns = expected_returns.reshape(num_actions, num_objectives)  # Cast the result to a correct shape.
 
+    # We now take the sum of the weighted returns over the correct axes to get the expected returns.
+    expected_returns = np.sum(expected_returns, axis=tuple(opponents))
     return expected_returns
 
 
 def calc_utility_from_joint_strat(u, player, payoff_matrix, joint_strategy):
     """Calculate the utility from a given joint strategy.
 
     Args:
```

### Comparing `ramo-0.1.2/ramo/strategy/operations.py` & `ramo-0.1.3/ramo/strategy/operations.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/utility_function/checking.py` & `ramo-0.1.3/ramo/utility_function/checking.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/utility_function/functions.py` & `ramo-0.1.3/ramo/utility_function/functions.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/utils/agent_loader.py` & `ramo-0.1.3/ramo/utils/agent_loader.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/utils/data.py` & `ramo-0.1.3/ramo/utils/data.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/utils/experiments.py` & `ramo-0.1.3/ramo/utils/experiments.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo/utils/helpers.py` & `ramo-0.1.3/ramo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `ramo-0.1.2/ramo.egg-info/PKG-INFO` & `ramo-0.1.3/ramo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Algorithms for computing or learning equilibria in multi-objective games
 Author: Willem Röpke
 Author-email: willem.ropke@vub.be
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `ramo-0.1.2/ramo.egg-info/SOURCES.txt` & `ramo-0.1.3/ramo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 ramo/nash/Player.py
 ramo/nash/__init__.py
 ramo/nash/fictitious_play.py
 ramo/nash/moqups.py
 ramo/nash/mose.py
 ramo/nash/verify.py
 ramo/pareto/__init__.py
+ramo/pareto/dominance.py
 ramo/pareto/pareto_nash.py
 ramo/pareto/verify.py
 ramo/printing/__init__.py
 ramo/printing/printing.py
 ramo/strategy/__init__.py
 ramo/strategy/best_response.py
 ramo/strategy/operations.py
```

### Comparing `ramo-0.1.2/setup.py` & `ramo-0.1.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ramo",  # The name of the package.
-    version="0.1.2",  # The current release version.
+    version="0.1.3",  # The current release version.
     author="Willem Röpke",  # The full name of the author.
     author_email="willem.ropke@vub.be",  # Email address of the author.
     description="Algorithms for computing or learning equilibria in multi-objective games",  # Short tagline.
     long_description=long_description,  # Long description read from the readme file.
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed.
     classifiers=[
```

