# Comparing `tmp/imephu-0.1.0.tar.gz` & `tmp/imephu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imephu-0.1.0.tar", last modified: Sun Apr 10 10:25:40 2022, max compression
+gzip compressed data, was "imephu-0.2.0.tar", last modified: Wed May  3 19:02:23 2023, max compression
```

## Comparing `imephu-0.1.0.tar` & `imephu-0.2.0.tar`

### file list

```diff
@@ -1,86 +1,116 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.099274 imephu-0.1.0/
--rw-r--r--   0 christian   (501) staff       (20)     1102 2022-01-15 12:25:41.000000 imephu-0.1.0/LICENSE
--rw-r--r--   0 christian   (501) staff       (20)       50 2022-01-15 12:25:41.000000 imephu-0.1.0/MANIFEST.in
--rw-r--r--   0 christian   (501) staff       (20)     1445 2022-04-10 10:25:40.099401 imephu-0.1.0/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     1014 2022-04-10 10:02:05.000000 imephu-0.1.0/README.md
--rw-r--r--   0 christian   (501) staff       (20)      179 2022-02-11 15:02:42.000000 imephu-0.1.0/pyproject.toml
--rw-r--r--   0 christian   (501) staff       (20)     2638 2022-04-10 10:25:40.100577 imephu-0.1.0/setup.cfg
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.057495 imephu-0.1.0/src/
--rw-r--r--   0 christian   (501) staff       (20)     6148 2022-03-15 07:56:29.000000 imephu-0.1.0/src/.DS_Store
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.063915 imephu-0.1.0/src/imephu/
--rw-r--r--   0 christian   (501) staff       (20)     6148 2022-01-19 10:57:49.000000 imephu-0.1.0/src/imephu/.DS_Store
--rw-r--r--   0 christian   (501) staff       (20)      185 2022-04-10 10:07:09.000000 imephu-0.1.0/src/imephu/__init__.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.070631 imephu-0.1.0/src/imephu/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)      345 2022-04-10 10:22:44.000000 imephu-0.1.0/src/imephu/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     9704 2022-04-06 20:55:09.000000 imephu-0.1.0/src/imephu/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)    12478 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/__pycache__/finder_chart.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     7848 2022-02-16 12:01:10.000000 imephu-0.1.0/src/imephu/__pycache__/geometry.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3528 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/__pycache__/utils.cpython-310.pyc
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.071871 imephu-0.1.0/src/imephu/annotation/
--rw-r--r--   0 christian   (501) staff       (20)     1550 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/annotation/__init__.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.073775 imephu-0.1.0/src/imephu/annotation/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)     2093 2022-02-16 12:01:09.000000 imephu-0.1.0/src/imephu/annotation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4075 2022-01-20 07:33:05.000000 imephu-0.1.0/src/imephu/annotation/__pycache__/general.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     6146 2022-02-16 12:01:10.000000 imephu-0.1.0/src/imephu/annotation/__pycache__/motion.cpython-310.pyc
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.078978 imephu-0.1.0/src/imephu/annotation/general/
--rw-r--r--   0 christian   (501) staff       (20)      746 2022-04-10 10:07:01.000000 imephu-0.1.0/src/imephu/annotation/general/__init__.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.083930 imephu-0.1.0/src/imephu/annotation/general/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)      825 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/annotation/general/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3797 2022-02-16 12:01:10.000000 imephu-0.1.0/src/imephu/annotation/general/__pycache__/arrow.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4219 2022-02-16 12:01:10.000000 imephu-0.1.0/src/imephu/annotation/general/__pycache__/circle.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     2703 2022-03-16 19:12:35.000000 imephu-0.1.0/src/imephu/annotation/general/__pycache__/crosshairs.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     2205 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/annotation/general/__pycache__/empty.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3881 2022-02-16 12:01:10.000000 imephu-0.1.0/src/imephu/annotation/general/__pycache__/group.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4998 2022-02-16 12:01:10.000000 imephu-0.1.0/src/imephu/annotation/general/__pycache__/line_path.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4715 2022-02-16 12:01:10.000000 imephu-0.1.0/src/imephu/annotation/general/__pycache__/rectangle.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     5280 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/annotation/general/__pycache__/text.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4480 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/annotation/general/arrow.py
--rw-r--r--   0 christian   (501) staff       (20)     3879 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/annotation/general/circle.py
--rw-r--r--   0 christian   (501) staff       (20)     2581 2022-03-16 15:48:57.000000 imephu-0.1.0/src/imephu/annotation/general/crosshairs.py
--rw-r--r--   0 christian   (501) staff       (20)     1646 2022-04-10 10:02:05.000000 imephu-0.1.0/src/imephu/annotation/general/empty.py
--rw-r--r--   0 christian   (501) staff       (20)     3021 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/annotation/general/group.py
--rw-r--r--   0 christian   (501) staff       (20)     4428 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/annotation/general/line_path.py
--rw-r--r--   0 christian   (501) staff       (20)     4425 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/annotation/general/rectangle.py
--rw-r--r--   0 christian   (501) staff       (20)     5316 2022-04-10 10:06:56.000000 imephu-0.1.0/src/imephu/annotation/general/text.py
--rw-r--r--   0 christian   (501) staff       (20)     9170 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/annotation/motion.py
--rw-r--r--   0 christian   (501) staff       (20)    11976 2022-04-10 10:02:05.000000 imephu-0.1.0/src/imephu/cli.py
--rw-r--r--   0 christian   (501) staff       (20)    13375 2022-04-10 10:06:52.000000 imephu-0.1.0/src/imephu/finder_chart.py
--rw-r--r--   0 christian   (501) staff       (20)     9710 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/geometry.py
--rw-r--r--   0 christian   (501) staff       (20)        0 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/py.typed
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.085241 imephu-0.1.0/src/imephu/salt/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.088613 imephu-0.1.0/src/imephu/salt/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)      168 2022-01-26 13:02:56.000000 imephu-0.1.0/src/imephu/salt/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)    12811 2022-04-10 10:22:44.000000 imephu-0.1.0/src/imephu/salt/__pycache__/finder_chart.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     6895 2022-01-26 15:41:26.000000 imephu-0.1.0/src/imephu/salt/__pycache__/general.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     1389 2022-01-26 19:29:20.000000 imephu-0.1.0/src/imephu/salt/__pycache__/rss.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     4839 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/salt/__pycache__/utils.cpython-310.pyc
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.091535 imephu-0.1.0/src/imephu/salt/annotation/
--rw-r--r--   0 christian   (501) staff       (20)        0 2022-02-11 15:02:42.000000 imephu-0.1.0/src/imephu/salt/annotation/__init__.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.095984 imephu-0.1.0/src/imephu/salt/annotation/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)      168 2022-02-16 12:01:10.000000 imephu-0.1.0/src/imephu/salt/annotation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     8892 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/salt/annotation/__pycache__/nir.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)      171 2022-02-01 19:33:00.000000 imephu-0.1.0/src/imephu/salt/annotation/__pycache__/observation.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     3687 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/salt/annotation/__pycache__/rss.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     1375 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/salt/annotation/__pycache__/salticam.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     8241 2022-04-10 10:22:45.000000 imephu-0.1.0/src/imephu/salt/annotation/__pycache__/telescope.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)    12154 2022-04-10 10:06:48.000000 imephu-0.1.0/src/imephu/salt/annotation/nir.py
--rw-r--r--   0 christian   (501) staff       (20)     3860 2022-04-10 10:06:44.000000 imephu-0.1.0/src/imephu/salt/annotation/rss.py
--rw-r--r--   0 christian   (501) staff       (20)     1196 2022-04-10 10:06:38.000000 imephu-0.1.0/src/imephu/salt/annotation/salticam.py
--rw-r--r--   0 christian   (501) staff       (20)     9025 2022-04-10 10:06:34.000000 imephu-0.1.0/src/imephu/salt/annotation/telescope.py
--rw-r--r--   0 christian   (501) staff       (20)    14796 2022-04-10 10:06:27.000000 imephu-0.1.0/src/imephu/salt/finder_chart.py
--rw-r--r--   0 christian   (501) staff       (20)     4859 2022-04-10 10:06:20.000000 imephu-0.1.0/src/imephu/salt/utils.py
--rw-r--r--   0 christian   (501) staff       (20)    10458 2022-04-10 10:02:05.000000 imephu-0.1.0/src/imephu/schema.json
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.096997 imephu-0.1.0/src/imephu/service/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.098343 imephu-0.1.0/src/imephu/service/__pycache__/
--rw-r--r--   0 christian   (501) staff       (20)     7558 2022-03-15 20:23:31.000000 imephu-0.1.0/src/imephu/service/__pycache__/horizons.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     8482 2022-03-28 08:43:20.000000 imephu-0.1.0/src/imephu/service/__pycache__/survey.cpython-310.pyc
--rw-r--r--   0 christian   (501) staff       (20)     9473 2022-04-10 10:06:12.000000 imephu-0.1.0/src/imephu/service/horizons.py
--rw-r--r--   0 christian   (501) staff       (20)     7716 2022-03-28 08:20:41.000000 imephu-0.1.0/src/imephu/service/survey.py
--rw-r--r--   0 christian   (501) staff       (20)     3680 2022-04-10 10:06:07.000000 imephu-0.1.0/src/imephu/utils.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2022-04-10 10:25:40.066887 imephu-0.1.0/src/imephu.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)     1445 2022-04-10 10:25:39.000000 imephu-0.1.0/src/imephu.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     2935 2022-04-10 10:25:40.000000 imephu-0.1.0/src/imephu.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2022-04-10 10:25:39.000000 imephu-0.1.0/src/imephu.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       42 2022-04-10 10:25:39.000000 imephu-0.1.0/src/imephu.egg-info/entry_points.txt
--rw-r--r--   0 christian   (501) staff       (20)      176 2022-04-10 10:25:39.000000 imephu-0.1.0/src/imephu.egg-info/requires.txt
--rw-r--r--   0 christian   (501) staff       (20)        7 2022-04-10 10:25:39.000000 imephu-0.1.0/src/imephu.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.477321 imephu-0.2.0/
+-rw-r--r--   0 christian   (501) staff       (20)     1102 2022-01-15 12:25:41.000000 imephu-0.2.0/LICENSE
+-rw-r--r--   0 christian   (501) staff       (20)       50 2022-01-15 12:25:41.000000 imephu-0.2.0/MANIFEST.in
+-rw-r--r--   0 christian   (501) staff       (20)     1426 2023-05-03 19:02:23.477481 imephu-0.2.0/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     1015 2023-05-03 18:55:18.000000 imephu-0.2.0/README.md
+-rw-r--r--   0 christian   (501) staff       (20)      179 2022-02-11 15:02:42.000000 imephu-0.2.0/pyproject.toml
+-rw-r--r--   0 christian   (501) staff       (20)     2631 2023-05-03 19:02:23.479383 imephu-0.2.0/setup.cfg
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.347705 imephu-0.2.0/src/
+-rw-r--r--   0 christian   (501) staff       (20)     6148 2022-03-15 07:56:29.000000 imephu-0.2.0/src/.DS_Store
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.354756 imephu-0.2.0/src/imephu/
+-rw-r--r--   0 christian   (501) staff       (20)     6148 2022-01-19 10:57:49.000000 imephu-0.2.0/src/imephu/.DS_Store
+-rw-r--r--   0 christian   (501) staff       (20)      185 2023-05-03 18:55:18.000000 imephu-0.2.0/src/imephu/__init__.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.372200 imephu-0.2.0/src/imephu/__pycache__/
+-rw-r--r--   0 christian   (501) staff       (20)      345 2023-05-03 18:57:09.000000 imephu-0.2.0/src/imephu/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)      343 2022-07-06 16:37:45.000000 imephu-0.2.0/src/imephu/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     9704 2022-06-14 07:19:18.000000 imephu-0.2.0/src/imephu/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     9693 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/__pycache__/cli.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)    12059 2023-05-03 18:57:09.000000 imephu-0.2.0/src/imephu/__pycache__/finder_chart.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)    13432 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/__pycache__/finder_chart.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     7848 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/__pycache__/geometry.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     7870 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/__pycache__/geometry.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     3528 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     3522 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/__pycache__/utils.cpython-38.pyc
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.374858 imephu-0.2.0/src/imephu/annotation/
+-rw-r--r--   0 christian   (501) staff       (20)     1550 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/__init__.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.380954 imephu-0.2.0/src/imephu/annotation/__pycache__/
+-rw-r--r--   0 christian   (501) staff       (20)     2093 2022-02-16 12:01:09.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     2105 2022-07-06 16:37:45.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4075 2022-01-20 07:33:05.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/general.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     6146 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/motion.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     6137 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/__pycache__/motion.cpython-38.pyc
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.388639 imephu-0.2.0/src/imephu/annotation/general/
+-rw-r--r--   0 christian   (501) staff       (20)      746 2022-04-10 10:07:01.000000 imephu-0.2.0/src/imephu/annotation/general/__init__.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.410065 imephu-0.2.0/src/imephu/annotation/general/__pycache__/
+-rw-r--r--   0 christian   (501) staff       (20)      825 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)      849 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     3797 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/arrow.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     3775 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/arrow.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4219 2022-07-12 19:08:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/circle.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4197 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/circle.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     2703 2022-03-16 19:12:35.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/crosshairs.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     2660 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/crosshairs.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     2205 2022-07-12 19:08:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/empty.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     2215 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/empty.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     3881 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/group.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     3890 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/group.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4998 2022-07-12 19:08:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/line_path.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4966 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/line_path.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4715 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/rectangle.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4699 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/rectangle.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     5280 2022-07-12 19:08:45.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/text.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     5242 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/annotation/general/__pycache__/text.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4480 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/general/arrow.py
+-rw-r--r--   0 christian   (501) staff       (20)     3879 2022-07-07 23:59:33.000000 imephu-0.2.0/src/imephu/annotation/general/circle.py
+-rw-r--r--   0 christian   (501) staff       (20)     2581 2022-03-16 15:48:57.000000 imephu-0.2.0/src/imephu/annotation/general/crosshairs.py
+-rw-r--r--   0 christian   (501) staff       (20)     1646 2022-07-07 23:59:33.000000 imephu-0.2.0/src/imephu/annotation/general/empty.py
+-rw-r--r--   0 christian   (501) staff       (20)     3021 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/general/group.py
+-rw-r--r--   0 christian   (501) staff       (20)     4428 2022-07-07 23:59:33.000000 imephu-0.2.0/src/imephu/annotation/general/line_path.py
+-rw-r--r--   0 christian   (501) staff       (20)     4425 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/general/rectangle.py
+-rw-r--r--   0 christian   (501) staff       (20)     5316 2022-07-07 23:59:33.000000 imephu-0.2.0/src/imephu/annotation/general/text.py
+-rw-r--r--   0 christian   (501) staff       (20)     9170 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/annotation/motion.py
+-rw-r--r--   0 christian   (501) staff       (20)    11976 2022-04-10 10:02:05.000000 imephu-0.2.0/src/imephu/cli.py
+-rw-r--r--   0 christian   (501) staff       (20)    12939 2023-05-03 18:55:18.000000 imephu-0.2.0/src/imephu/finder_chart.py
+-rw-r--r--   0 christian   (501) staff       (20)     9710 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/geometry.py
+-rw-r--r--   0 christian   (501) staff       (20)        0 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/py.typed
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.421076 imephu-0.2.0/src/imephu/salt/
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.436061 imephu-0.2.0/src/imephu/salt/__pycache__/
+-rw-r--r--   0 christian   (501) staff       (20)      168 2022-01-26 13:02:56.000000 imephu-0.2.0/src/imephu/salt/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)    12811 2022-04-10 10:22:44.000000 imephu-0.2.0/src/imephu/salt/__pycache__/finder_chart.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)    12855 2022-07-06 16:37:49.000000 imephu-0.2.0/src/imephu/salt/__pycache__/finder_chart.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     6895 2022-01-26 15:41:26.000000 imephu-0.2.0/src/imephu/salt/__pycache__/general.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     1389 2022-01-26 19:29:20.000000 imephu-0.2.0/src/imephu/salt/__pycache__/rss.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4839 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     4792 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/__pycache__/utils.cpython-38.pyc
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.442757 imephu-0.2.0/src/imephu/salt/annotation/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2022-02-11 15:02:42.000000 imephu-0.2.0/src/imephu/salt/annotation/__init__.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.464242 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/
+-rw-r--r--   0 christian   (501) staff       (20)      168 2022-02-16 12:01:10.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)      166 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     8892 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/nir.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     8889 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/nir.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)      171 2022-02-01 19:33:00.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/observation.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     3687 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/rss.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     3697 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/rss.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     1375 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/salticam.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     1376 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/salticam.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     8241 2022-04-10 10:22:45.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/telescope.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     8245 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/salt/annotation/__pycache__/telescope.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)    12154 2022-04-10 10:06:48.000000 imephu-0.2.0/src/imephu/salt/annotation/nir.py
+-rw-r--r--   0 christian   (501) staff       (20)     3860 2022-04-10 10:06:44.000000 imephu-0.2.0/src/imephu/salt/annotation/rss.py
+-rw-r--r--   0 christian   (501) staff       (20)     1196 2022-04-10 10:06:38.000000 imephu-0.2.0/src/imephu/salt/annotation/salticam.py
+-rw-r--r--   0 christian   (501) staff       (20)     9025 2022-04-10 10:06:34.000000 imephu-0.2.0/src/imephu/salt/annotation/telescope.py
+-rw-r--r--   0 christian   (501) staff       (20)    14796 2022-04-10 10:06:27.000000 imephu-0.2.0/src/imephu/salt/finder_chart.py
+-rw-r--r--   0 christian   (501) staff       (20)     4859 2022-04-10 10:06:20.000000 imephu-0.2.0/src/imephu/salt/utils.py
+-rw-r--r--   0 christian   (501) staff       (20)    10458 2022-04-10 10:02:05.000000 imephu-0.2.0/src/imephu/schema.json
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.467019 imephu-0.2.0/src/imephu/service/
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.471611 imephu-0.2.0/src/imephu/service/__pycache__/
+-rw-r--r--   0 christian   (501) staff       (20)     7558 2022-06-14 07:19:19.000000 imephu-0.2.0/src/imephu/service/__pycache__/horizons.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     7550 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/service/__pycache__/horizons.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)    14053 2023-05-03 18:57:10.000000 imephu-0.2.0/src/imephu/service/__pycache__/survey.cpython-310.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     8529 2022-07-06 16:37:52.000000 imephu-0.2.0/src/imephu/service/__pycache__/survey.cpython-38.pyc
+-rw-r--r--   0 christian   (501) staff       (20)     9473 2022-04-10 10:06:12.000000 imephu-0.2.0/src/imephu/service/horizons.py
+-rw-r--r--   0 christian   (501) staff       (20)    14909 2023-05-03 18:55:18.000000 imephu-0.2.0/src/imephu/service/survey.py
+-rw-r--r--   0 christian   (501) staff       (20)     3680 2022-04-10 10:06:07.000000 imephu-0.2.0/src/imephu/utils.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.360043 imephu-0.2.0/src/imephu.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)     1426 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     4470 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)       42 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/entry_points.txt
+-rw-r--r--   0 christian   (501) staff       (20)      161 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)        7 2023-05-03 19:02:23.000000 imephu-0.2.0/src/imephu.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-03 19:02:23.476383 imephu-0.2.0/tests/
+-rw-r--r--   0 christian   (501) staff       (20)    13797 2023-05-03 18:55:18.000000 imephu-0.2.0/tests/test_cli.py
+-rw-r--r--   0 christian   (501) staff       (20)    11263 2023-05-03 18:55:19.000000 imephu-0.2.0/tests/test_finder_chart.py
+-rw-r--r--   0 christian   (501) staff       (20)     2224 2022-02-11 15:02:42.000000 imephu-0.2.0/tests/test_geometry.py
+-rw-r--r--   0 christian   (501) staff       (20)     4282 2022-04-10 10:02:27.000000 imephu-0.2.0/tests/test_utils.py
```

### Comparing `imephu-0.1.0/LICENSE` & `imephu-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/PKG-INFO` & `imephu-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: imephu
-Version: 0.1.0
+Version: 0.2.0
 Summary: Generate finder charts for the Southern African Large Telescope (SALT).
 Home-page: https://github.com/saltastroops/saao-pypackage-cookiecutter
 Author: Southern African Large Telescope (SALT)
 Author-email: salthelp@salt.ac.za
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # imephu
 
-imephu is a package for Generating finder charts for astronomical observations. While primarily intended for the [Southern Africa Large Telescope](https://www.salt.ac.za), it can be used to create completely custom finder charts.
+imephu is a package for generating finder charts for astronomical observations. While primarily intended for the [Southern African Large Telescope](https://www.salt.ac.za), it can be used to create completely custom finder charts.
 
 ## Installation
 
 imephu can be installed with pip in the usual way with
 
 ```shell
 pip install imephu
@@ -38,9 +37,7 @@
 Alternatively, you can use an API for creating custom finder charts. An example of how to do this can be found [here](https://saltastroops.github.io/imephu/notebooks/salt.html).
 
 ## Documentation
 
 The documentation is hosted at [https://saltastroops.github.io/imephu/](https://saltastroops.github.io/imephu/).
 
 
-
-
```

### Comparing `imephu-0.1.0/README.md` & `imephu-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # imephu
 
-imephu is a package for Generating finder charts for astronomical observations. While primarily intended for the [Southern Africa Large Telescope](https://www.salt.ac.za), it can be used to create completely custom finder charts.
+imephu is a package for generating finder charts for astronomical observations. While primarily intended for the [Southern African Large Telescope](https://www.salt.ac.za), it can be used to create completely custom finder charts.
 
 ## Installation
 
 imephu can be installed with pip in the usual way with
 
 ```shell
 pip install imephu
```

### Comparing `imephu-0.1.0/setup.cfg` & `imephu-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 install_requires = 
 	astropy>=5.0
 	astroquery>=0.4.5
 	jsonschema>=4.4.0
 	python-dateutil>=2.8.2
 	defusedxml>=0.7.1
 	matplotlib>=3.1,!=3.4.0
-	pikepdf>=4.4.1
 	pyyaml>=6.0
 	requests>=2.27.1
 	typer[all]>=0.4.0
 
 [options.packages.find]
 where = src
 exclude = 
@@ -87,14 +86,15 @@
 	src/imephu
 
 [tox:tox]
 envlist = ["3.8", "3.9", "3.10"]
 isolated_build = True
 
 [testenv]
+usedevelop = True
 deps = 
 	pytest
 	pytest-cov
 	pytest-regressions
 	responses
 commands = 
 	pytest {posargs:--cov --strict-markers}
@@ -133,15 +133,14 @@
 [testenv:docs]
 deps = 
 	astropy
 	defusedxml
 	jsonschema
 	matplotlib
 	myst-nb
-	pikepdf
 	pyyaml
 	requests
 	sphinx
 	sphinx-autodoc-typehints
 	sphinx-book-theme
 	typer
 commands =
```

### Comparing `imephu-0.1.0/src/.DS_Store` & `imephu-0.2.0/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/.DS_Store` & `imephu-0.2.0/src/imephu/.DS_Store`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/__pycache__/cli.cpython-310.pyc` & `imephu-0.2.0/src/imephu/__pycache__/cli.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr  6 14:47:53 2022 UTC, .py size: 11976 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 19a8 4d62 c82e 0000  o.........Mb....
+00000000: 6f0d 0d0a 0000 0000 1dab 5262 c82e 0000  o.........Rb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 e203 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `imephu-0.1.0/src/imephu/__pycache__/finder_chart.cpython-310.pyc` & `imephu-0.2.0/src/imephu/__pycache__/finder_chart.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 10 10:06:52 2022 UTC, .py size: 13375 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,780 +1,754 @@
-00000000: 6f0d 0d0a 0000 0000 3cac 5262 3f34 0000  o.......<.Rb?4..
+00000000: 6f0d 0d0a 0000 0000 16ae 5264 8b32 0000  o.........Rd.2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0173 2001 0000 6400  .....@...s ...d.
+00000020: 0003 0000 0040 0000 0173 1401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6403 6c05 6d05 5a05 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000080: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
-00000090: 0100 6400 6402 6c11 6d12 5a13 0100 6400  ..d.d.l.m.Z...d.
-000000a0: 6402 6c14 5a14 6400 6406 6c15 6d16 5a17  d.l.Z.d.d.l.m.Z.
-000000b0: 0100 6400 6407 6c18 6d19 5a19 6d1a 5a1a  ..d.d.l.m.Z.m.Z.
-000000c0: 0100 6400 6408 6c1b 6d1c 5a1c 0100 6400  ..d.d.l.m.Z...d.
-000000d0: 6409 6c1d 6d1e 5a1e 0100 6400 640a 6c1f  d.l.m.Z...d.d.l.
-000000e0: 6d20 5a20 0100 6400 640b 6c21 6d22 5a22  m Z ..d.d.l!m"Z"
-000000f0: 0100 6400 640c 6c23 6d24 5a24 6d25 5a25  ..d.d.l#m$Z$m%Z%
-00000100: 0100 6400 640d 6c26 6d27 5a27 0100 6400  ..d.d.l&m'Z'..d.
-00000110: 6402 6c28 5a28 6400 640e 6c29 6d2a 5a2a  d.l(Z(d.d.l)m*Z*
-00000120: 0100 6400 640f 6c2b 6d2c 5a2c 0100 6400  ..d.d.l+m,Z,..d.
-00000130: 6410 6c2d 6d2e 5a2e 0100 0900 4700 6411  d.l-m.Z.....G.d.
-00000140: 6412 8400 6412 8302 5a2f 6402 5300 2913  d...d...Z/d.S.).
-00000150: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
-00000160: 696f 6e73 4e29 01da 0864 6174 6574 696d  ionsN)...datetim
-00000170: 6529 01da 0742 7974 6573 494f 2908 da03  e)...BytesIO)...
-00000180: 416e 79da 0842 696e 6172 7949 4fda 0843  Any..BinaryIO..C
-00000190: 616c 6c61 626c 65da 0947 656e 6572 6174  allable..Generat
-000001a0: 6f72 da04 4c69 7374 da08 4f70 7469 6f6e  or..List..Option
-000001b0: 616c da05 5475 706c 65da 0555 6e69 6f6e  al..Tuple..Union
-000001c0: 2901 da05 756e 6974 7329 02da 0541 6e67  )...units)...Ang
-000001d0: 6c65 da08 536b 7943 6f6f 7264 2901 da04  le..SkyCoord)...
-000001e0: 6669 7473 2901 da1c 4173 796d 6d65 7472  fits)...Asymmetr
-000001f0: 6963 5065 7263 656e 7469 6c65 496e 7465  icPercentileInte
-00000200: 7276 616c 2901 da0b 7369 6d70 6c65 5f6e  rval)...simple_n
-00000210: 6f72 6d29 01da 0e57 4353 4178 6573 5375  orm)...WCSAxesSu
-00000220: 6270 6c6f 7429 02da 0357 4353 da10 4649  bplot)...WCS..FI
-00000230: 5453 4669 7865 6457 6172 6e69 6e67 2901  TSFixedWarning).
-00000240: da06 4669 6775 7265 2901 da0a 416e 6e6f  ..Figure)...Anno
-00000250: 7461 7469 6f6e 2901 da09 6c6f 6164 5f66  tation)...load_f
-00000260: 6974 7329 01da 0945 7068 656d 6572 6973  its)...Ephemeris
-00000270: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000280: 0004 0000 0040 0000 0173 9200 0000 6500  .....@...s....e.
-00000290: 5a01 6400 5a02 6401 5a03 6438 6404 6405  Z.d.Z.d.Z.d8d.d.
-000002a0: 8404 5a04 6505 6439 640e 640f 8404 8301  ..Z.e.d9d.d.....
-000002b0: 5a06 6505 643a 6419 641a 8404 8301 5a07  Z.e.d:d.d.....Z.
-000002c0: 6508 643b 641c 641d 8404 8301 5a09 643c  e.d;d.d.....Z.d<
-000002d0: 6421 6422 8404 5a0a 643d 6423 6424 8404  d!d"..Z.d=d#d$..
-000002e0: 5a0b 0925 643e 643f 6429 642a 8405 5a0c  Z..%d>d?d)d*..Z.
-000002f0: 6440 642c 642d 8404 5a0d 6441 6430 6431  d@d,d-..Z.dAd0d1
-00000300: 8404 5a0e 6441 6432 6433 8404 5a0f 6505  ..Z.dAd2d3..Z.e.
-00000310: 6442 6436 6437 8404 8301 5a10 6425 5300  dBd6d7....Z.d%S.
-00000320: 2943 da0b 4669 6e64 6572 4368 6172 7461  )C..FinderCharta
-00000330: ad02 0000 4120 6669 6e64 6572 2063 6861  ....A finder cha
-00000340: 7274 2066 6f72 2061 6e20 6173 7472 6f6e  rt for an astron
-00000350: 6f6d 6963 616c 206f 6273 6572 7661 7469  omical observati
-00000360: 6f6e 2e0a 0a20 2020 2054 6865 2066 696e  on...    The fin
-00000370: 6465 7220 6368 6172 7420 6973 2067 656e  der chart is gen
-00000380: 6572 6174 6564 2066 726f 6d20 6120 4649  erated from a FI
-00000390: 5453 2066 696c 652e 2042 7920 6465 6661  TS file. By defa
-000003a0: 756c 7420 7468 6520 6669 6e64 6572 2063  ult the finder c
-000003b0: 6861 7274 206a 7573 740a 2020 2020 7368  hart just.    sh
-000003c0: 6f77 7320 7468 6520 7265 6769 6f6e 2077  ows the region w
-000003d0: 6974 6820 616e 206f 7665 726c 6169 6420  ith an overlaid 
-000003e0: 636f 6f72 6469 6e61 7465 2067 7269 642e  coordinate grid.
-000003f0: 2054 6865 2061 7865 7320 7368 6f77 2057   The axes show W
-00000400: 4353 2063 6f6f 7264 696e 6174 6573 2e0a  CS coordinates..
-00000410: 2020 2020 5573 6520 7468 6520 6061 6464      Use the `add
-00000420: 5f61 6e6e 6f74 6174 696f 6e60 206d 6574  _annotation` met
-00000430: 686f 6420 746f 2061 6464 206d 6f72 6520  hod to add more 
-00000440: 636f 6e74 656e 7420 746f 2074 6865 2066  content to the f
-00000450: 696e 6465 7220 6368 6172 742e 0a0a 2020  inder chart...  
-00000460: 2020 596f 7520 6361 6e20 6469 7370 6c61    You can displa
-00000470: 7920 7468 6520 6669 6e64 6572 2063 6861  y the finder cha
-00000480: 7274 206f 6e20 7468 6520 7363 7265 656e  rt on the screen
-00000490: 206f 7220 7361 7665 2069 7420 6173 2061   or save it as a
-000004a0: 2066 696c 652e 0a0a 2020 2020 5468 6973   file...    This
-000004b0: 2063 6c61 7373 2075 7365 7320 4d61 7470   class uses Matp
-000004c0: 6c6f 746c 6962 2066 6f72 2067 656e 6572  lotlib for gener
-000004d0: 6174 696e 6720 7468 6520 6669 6e64 6572  ating the finder
-000004e0: 2063 6861 7274 2e0a 0a20 2020 202e 2e20   chart...    .. 
-000004f0: 7761 726e 696e 673a 3a20 4265 2063 6172  warning:: Be car
-00000500: 6566 756c 2077 6865 6e20 776f 726b 696e  eful when workin
-00000510: 6720 7769 7468 2073 6576 6572 616c 2066  g with several f
-00000520: 696e 6465 7220 6368 6172 7473 2061 7320  inder charts as 
-00000530: 616c 6c20 7468 6520 6669 6e64 6572 0a20  all the finder. 
-00000540: 2020 2020 2020 6368 6172 7473 2075 7365        charts use
-00000550: 2074 6865 2073 616d 6520 4d61 7470 6c6f   the same Matplo
-00000560: 746c 6962 2066 6967 7572 652e 0a0a 2020  tlib figure...  
-00000570: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00000580: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000590: 6e61 6d65 3a20 6073 7472 602c 2060 7061  name: `str`, `pa
-000005a0: 7468 2d6c 696b 6560 206f 7220 6062 696e  th-like` or `bin
-000005b0: 6172 7920 6669 6c65 2d6c 696b 6560 0a20  ary file-like`. 
-000005c0: 2020 2020 2020 2046 4954 5320 6669 6c65         FITS file
-000005d0: 2074 6f20 6469 7370 6c61 792e 0a20 2020   to display..   
-000005e0: 20da 046e 616d 65fa 2655 6e69 6f6e 5b73   ..name.&Union[s
-000005f0: 7472 2c20 4269 6e61 7279 494f 2c20 6f73  tr, BinaryIO, os
-00000600: 2e50 6174 684c 696b 655b 416e 795d 5d63  .PathLike[Any]]c
-00000610: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000620: 0800 0000 4300 0001 7366 0000 0074 00a0  ....C...sf...t..
-00000630: 017c 01a1 0164 0119 007c 005f 027c 006a  .|...d...|._.|.j
-00000640: 026a 037c 005f 0474 05a0 06a1 008f 1501  .j.|._.t........
-00000650: 0074 056a 0764 0274 0864 038d 0201 0074  .t.j.d.t.d.....t
-00000660: 097c 006a 0283 017c 005f 0a57 0064 0004  .|.j...|._.W.d..
-00000670: 0004 0083 0301 006e 0831 0073 2977 0101  .......n.1.s)w..
-00000680: 0001 0001 0059 0001 0067 007c 005f 0b64  .....Y...g.|._.d
-00000690: 0053 0029 044e 7201 0000 00da 0669 676e  .S.).Nr......ign
-000006a0: 6f72 6529 01da 0863 6174 6567 6f72 7929  ore)...category)
-000006b0: 0c72 1000 0000 da04 6f70 656e da04 5f68  .r......open.._h
-000006c0: 6475 da04 6461 7461 da05 5f64 6174 61da  du..data.._data.
-000006d0: 0877 6172 6e69 6e67 73da 0e63 6174 6368  .warnings..catch
-000006e0: 5f77 6172 6e69 6e67 73da 0c73 696d 706c  _warnings..simpl
-000006f0: 6566 696c 7465 7272 1500 0000 7214 0000  efilterr....r...
-00000700: 00da 045f 7763 73da 0c5f 616e 6e6f 7461  ..._wcs.._annota
-00000710: 7469 6f6e 7329 02da 0473 656c 6672 1b00  tions)...selfr..
-00000720: 0000 a900 7229 0000 00fa 3f2f 5573 6572  ....r)....?/User
-00000730: 732f 6368 7269 7374 6961 6e2f 4964 6561  s/christian/Idea
-00000740: 5072 6f6a 6563 7473 2f69 6d65 7068 752f  Projects/imephu/
-00000750: 7372 632f 696d 6570 6875 2f66 696e 6465  src/imephu/finde
-00000760: 725f 6368 6172 742e 7079 da08 5f5f 696e  r_chart.py..__in
-00000770: 6974 5f5f 3100 0000 730e 0000 0010 010a  it__1...s.......
-00000780: 030a 010e 010e 011c fe0a 037a 1446 696e  ...........z.Fin
-00000790: 6465 7243 6861 7274 2e5f 5f69 6e69 745f  derChart.__init_
-000007a0: 5fda 0673 7572 7665 79da 0373 7472 da0b  _..survey..str..
-000007b0: 6669 7473 5f63 656e 7465 7272 0f00 0000  fits_centerr....
-000007c0: da04 7369 7a65 720e 0000 00da 0672 6574  ..sizer......ret
-000007d0: 7572 6efa 0d27 4669 6e64 6572 4368 6172  urn..'FinderChar
-000007e0: 7427 6303 0000 0000 0000 0000 0000 0004  t'c.............
-000007f0: 0000 0004 0000 0043 0000 0173 1400 0000  .......C...s....
-00000800: 7400 7c00 7c01 7c02 8303 7d03 7401 7c03  t.|.|.|...}.t.|.
-00000810: 8301 5300 2902 61a2 0100 0043 7265 6174  ..S.).a....Creat
-00000820: 6520 6120 6669 6e64 6572 2063 6861 7274  e a finder chart
-00000830: 2066 726f 6d20 6120 736b 7920 7375 7276   from a sky surv
-00000840: 6579 2046 4954 5320 696d 6167 652e 0a0a  ey FITS image...
-00000850: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00000860: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00000870: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7375  -----.        su
-00000880: 7276 6579 3a20 6073 7472 600a 2020 2020  rvey: `str`.    
-00000890: 2020 2020 2020 2020 5468 6520 6e61 6d65          The name
-000008a0: 206f 6620 7468 6520 7375 7276 6579 2074   of the survey t
-000008b0: 6f20 7175 6572 7920 666f 7220 7468 6520  o query for the 
-000008c0: 4649 5453 2066 696c 652e 0a20 2020 2020  FITS file..     
-000008d0: 2020 2066 6974 735f 6365 6e74 6572 3a20     fits_center: 
-000008e0: 607e 6173 7472 6f70 792e 636f 6f72 6469  `~astropy.coordi
-000008f0: 6e61 7465 732e 536b 7943 6f6f 7264 600a  nates.SkyCoord`.
-00000900: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00000910: 6365 6e74 6572 2070 6f73 6974 696f 6e20  center position 
-00000920: 6f66 2074 6865 206c 6f61 6465 6420 4649  of the loaded FI
-00000930: 5453 2066 696c 652e 0a20 2020 2020 2020  TS file..       
-00000940: 2073 697a 653a 2060 7e61 7374 726f 7079   size: `~astropy
-00000950: 2e63 6f6f 7264 696e 6174 6573 2e41 6e67  .coordinates.Ang
-00000960: 6c65 600a 2020 2020 2020 2020 2020 2020  le`.            
-00000970: 5468 6520 7769 6474 6820 616e 6420 6865  The width and he
-00000980: 6967 6874 206f 6620 7468 6520 4649 5453  ight of the FITS
-00000990: 2066 696c 6520 696d 6167 652c 2061 7320   file image, as 
-000009a0: 616e 2061 6e67 6c65 206f 6e20 7468 6520  an angle on the 
-000009b0: 736b 792e 0a20 2020 2020 2020 204e 2902  sky..        N).
-000009c0: 7218 0000 0072 1a00 0000 2904 722c 0000  r....r....).r,..
-000009d0: 0072 2e00 0000 722f 0000 005a 0a66 6974  .r....r/...Z.fit
-000009e0: 735f 696d 6167 6572 2900 0000 7229 0000  s_imager)...r)..
-000009f0: 0072 2a00 0000 da0b 6672 6f6d 5f73 7572  .r*.....from_sur
-00000a00: 7665 793b 0000 0073 0400 0000 0c0d 0801  vey;...s........
-00000a10: 7a17 4669 6e64 6572 4368 6172 742e 6672  z.FinderChart.fr
-00000a20: 6f6d 5f73 7572 7665 79da 0573 7461 7274  om_survey..start
-00000a30: 7203 0000 00da 0365 6e64 da0b 6570 6865  r......end..ephe
-00000a40: 6d65 7269 6465 73fa 0f4c 6973 745b 4570  merides..List[Ep
-00000a50: 6865 6d65 7269 735d da10 6d61 785f 7472  hemeris]..max_tr
-00000a60: 6163 6b5f 6c65 6e67 7468 da13 6372 6561  ack_length..crea
-00000a70: 7465 5f66 696e 6465 725f 6368 6172 74fa  te_finder_chart.
-00000a80: 2a43 616c 6c61 626c 655b 5b4c 6973 745b  *Callable[[List[
-00000a90: 4570 6865 6d65 7269 735d 5d2c 2027 4669  Ephemeris]], 'Fi
-00000aa0: 6e64 6572 4368 6172 7427 5dfa 4647 656e  nderChart'].FGen
-00000ab0: 6572 6174 6f72 5b54 7570 6c65 5b27 4669  erator[Tuple['Fi
-00000ac0: 6e64 6572 4368 6172 7427 2c20 5475 706c  nderChart', Tupl
-00000ad0: 655b 6461 7465 7469 6d65 2c20 6461 7465  e[datetime, date
-00000ae0: 7469 6d65 5d5d 2c20 4e6f 6e65 2c20 4e6f  time]], None, No
-00000af0: 6e65 5d63 0500 0000 0000 0000 0000 0000  ne]c............
-00000b00: 0e00 0000 0500 0000 6300 0001 73aa 0100  ........c...s...
-00000b10: 0081 007c 006a 0064 0175 0073 0e7c 006a  ...|.j.d.u.s.|.j
-00000b20: 00a0 0164 01a1 0164 0175 0072 1274 0264  ...d...d.u.r.t.d
-00000b30: 0283 0182 017c 016a 0064 0175 0073 1f7c  .....|.j.d.u.s.|
-00000b40: 016a 00a0 0164 01a1 0164 0175 0072 2374  .j...d...d.u.r#t
-00000b50: 0264 0383 0182 017c 007c 016b 0572 2b74  .d.....|.|.k.r+t
-00000b60: 0264 0483 0182 017c 007c 0264 0519 006a  .d.....|.|.d...j
-00000b70: 036b 0072 3674 0264 0683 0182 017c 017c  .k.r6t.d.....|.|
-00000b80: 0264 0719 006a 036b 0472 4174 0264 0883  .d...j.k.rAt.d..
-00000b90: 0182 017c 03a0 0474 056a 06a1 0164 056b  ...|...t.j...d.k
-00000ba0: 0172 4d74 0264 0983 0182 0164 0a64 0b84  .rMt.d.....d.d..
-00000bb0: 007c 0244 0083 017d 0574 07a0 087c 057c  .|.D...}.t...|.|
-00000bc0: 00a1 0264 0c18 007d 0674 07a0 077c 057c  ...d...}.t...|.|
-00000bd0: 01a1 027d 077c 0764 056b 0472 727c 057c  ...}.|.d.k.rr|.|
-00000be0: 0764 0c18 0019 007c 016b 0272 727c 0764  .d.....|.k.rr|.d
-00000bf0: 0c38 007d 077c 067c 076b 0272 7a74 0264  .8.}.|.|.k.rzt.d
-00000c00: 0d83 0182 017c 027c 0619 0067 017d 087c  .....|.|...g.}.|
-00000c10: 0867 017d 0974 097c 0664 0c17 007c 0764  .g.}.t.|.d...|.d
-00000c20: 0c17 0083 0244 005d 337d 0a7c 027c 0a19  .....D.]3}.|.|..
-00000c30: 007d 0b7c 0864 0719 006a 0aa0 0b7c 0b6a  .}.|.d...j...|.j
-00000c40: 0aa1 017c 036b 0472 a074 0264 0e83 0182  ...|.k.r.t.d....
-00000c50: 017c 0864 0519 006a 0aa0 0b7c 0b6a 0aa1  .|.d...j...|.j..
-00000c60: 017d 0c7c 0c7c 036b 0172 b37c 08a0 0c7c  .}.|.|.k.r.|...|
-00000c70: 0ba1 0101 0071 8b7c 0864 0719 007c 0b67  .....q.|.d...|.g
-00000c80: 027d 087c 09a0 0c7c 08a1 0101 0071 8b7c  .}.|...|.....q.|
-00000c90: 0944 005d 117d 0d7c 047c 0d83 017c 0d64  .D.].}.|.|...|.d
-00000ca0: 0519 006a 037c 0d64 0719 006a 0366 0266  ...j.|.d...j.f.f
-00000cb0: 0256 0001 0071 c164 0153 0029 0f61 b508  .V...q.d.S.).a..
-00000cc0: 0000 4372 6561 7465 2066 696e 6465 7220  ..Create finder 
-00000cd0: 6368 6172 7473 2066 6f72 2061 2074 696d  charts for a tim
-00000ce0: 6520 696e 7465 7276 616c 2e0a 0a20 2020  e interval...   
-00000cf0: 2020 2020 2054 6869 7320 6d65 7468 6f64       This method
-00000d00: 2069 7320 696e 7465 6e64 6564 2066 6f72   is intended for
-00000d10: 206e 6f6e 2d73 6964 6572 6561 6c20 7461   non-sidereal ta
-00000d20: 7267 6574 732c 2077 6869 6368 206d 6179  rgets, which may
-00000d30: 2072 6571 7569 7265 206d 756c 7469 706c   require multipl
-00000d40: 650a 2020 2020 2020 2020 6669 6e64 6572  e.        finder
-00000d50: 2063 6861 7274 7320 746f 2063 6f76 6572   charts to cover
-00000d60: 2074 6865 6972 2074 7261 636b 206f 7665   their track ove
-00000d70: 7220 6120 7469 6d65 2069 6e74 6572 7661  r a time interva
-00000d80: 6c2e 2049 7420 6372 6561 7465 7320 6669  l. It creates fi
-00000d90: 6e64 6572 0a20 2020 2020 2020 2063 6861  nder.        cha
-00000da0: 7274 7320 6163 636f 7264 696e 6720 746f  rts according to
-00000db0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2072   the following r
-00000dc0: 756c 6573 3a0a 0a20 2020 2020 2020 202a  ules:..        *
-00000dd0: 2054 616b 656e 2074 6f67 6574 6865 722c   Taken together,
-00000de0: 2074 6865 2066 696e 6465 7220 6368 6172   the finder char
-00000df0: 7473 2063 6f76 6572 2074 6865 2077 686f  ts cover the who
-00000e00: 6c65 2074 696d 6520 696e 7465 7276 616c  le time interval
-00000e10: 2e0a 2020 2020 2020 2020 2a20 5468 6520  ..        * The 
-00000e20: 7472 6163 6b20 6c65 6e67 7468 206f 6e20  track length on 
-00000e30: 6561 6368 2066 696e 6465 7220 6368 6172  each finder char
-00000e40: 7420 646f 6573 206e 6f74 2065 7863 6565  t does not excee
-00000e50: 6420 606d 6178 5f74 7261 636b 5f6c 656e  d `max_track_len
-00000e60: 6774 6860 2e0a 2020 2020 2020 2020 2a20  gth`..        * 
-00000e70: 4561 6368 2066 696e 6465 7220 6368 6172  Each finder char
-00000e80: 7420 6973 2063 7265 6174 6564 2075 7369  t is created usi
-00000e90: 6e67 2060 6063 7265 6174 655f 6669 6e64  ng ``create_find
-00000ea0: 6572 5f63 6861 7274 6060 2e0a 0a20 2020  er_chart``...   
-00000eb0: 2020 2020 2054 6865 206d 6574 686f 6420       The method 
-00000ec0: 6973 2063 6f6d 706c 6574 656c 7920 6167  is completely ag
-00000ed0: 6e6f 7374 6963 2061 7320 746f 2077 6861  nostic as to wha
-00000ee0: 7420 6120 6669 6e64 6572 2063 6861 7274  t a finder chart
-00000ef0: 2073 686f 756c 6420 6c6f 6f6b 206c 696b   should look lik
-00000f00: 653b 0a20 2020 2020 2020 2074 6869 7320  e;.        this 
-00000f10: 6465 6369 7369 6f6e 2069 7320 6c65 6674  decision is left
-00000f20: 2063 6f6d 706c 6574 656c 7920 746f 2060   completely to `
-00000f30: 6063 7265 6174 655f 6669 6e64 6572 5f63  `create_finder_c
-00000f40: 6861 7274 6060 2e20 496e 2070 6172 7469  hart``. In parti
-00000f50: 6375 6c61 722c 2069 660a 2020 2020 2020  cular, if.      
-00000f60: 2020 796f 7520 6e65 6564 2061 6e79 2061    you need any a
-00000f70: 6e6e 6f74 6174 696f 6e73 2066 6f72 2074  nnotations for t
-00000f80: 6865 206e 6f6e 2d73 6964 6572 6561 6c20  he non-sidereal 
-00000f90: 6e61 7475 7265 2c20 6974 2069 7320 7570  nature, it is up
-00000fa0: 2074 6f0a 2020 2020 2020 2020 6060 6372   to.        ``cr
-00000fb0: 6561 7465 5f66 696e 6465 725f 6368 6172  eate_finder_char
-00000fc0: 7460 6020 746f 2070 726f 7669 6465 2074  t`` to provide t
-00000fd0: 6865 6d2e 0a0a 2020 2020 2020 2020 5468  hem...        Th
-00000fe0: 6520 6060 6372 6561 7465 5f66 696e 6465  e ``create_finde
-00000ff0: 725f 6368 6172 7460 6020 6675 6e63 7469  r_chart`` functi
-00001000: 6f6e 2068 6173 2074 6f20 6163 6365 7074  on has to accept
-00001010: 2074 776f 2061 7267 756d 656e 7473 2c20   two arguments, 
-00001020: 696e 2074 6869 7320 6f72 6465 723a 0a0a  in this order:..
-00001030: 2020 2020 2020 2020 2a20 5468 6520 6365          * The ce
-00001040: 6e74 6572 206f 6620 7468 6520 6669 6e64  nter of the find
-00001050: 6572 2063 6861 7274 2061 7320 6120 706f  er chart as a po
-00001060: 7369 7469 6f6e 206f 6e20 7468 6520 736b  sition on the sk
-00001070: 792c 2069 6e20 7269 6768 7420 6173 6365  y, in right asce
-00001080: 6e73 696f 6e0a 2020 2020 2020 2020 2020  nsion.          
-00001090: 616e 6420 6465 636c 696e 6174 696f 6e2e  and declination.
-000010a0: 0a20 2020 2020 2020 202a 2054 6865 206c  .        * The l
-000010b0: 6973 7420 6f66 2065 7068 656d 6572 6964  ist of ephemerid
-000010c0: 6573 2074 6f20 696e 636c 7564 6520 6f6e  es to include on
-000010d0: 2074 6865 2066 696e 6465 7220 6368 6172   the finder char
-000010e0: 7420 2866 6f72 2065 7861 6d70 6c65 2077  t (for example w
-000010f0: 6865 6e0a 2020 2020 2020 2020 2020 7573  hen.          us
-00001100: 696e 6720 616e 2061 6e6e 6f74 6174 696f  ing an annotatio
-00001110: 6e20 746f 2069 6e64 6963 6174 6520 7468  n to indicate th
-00001120: 6520 7461 7267 6574 206d 6f74 696f 6e29  e target motion)
-00001130: 2e0a 0a20 2020 2020 2020 2054 6865 2066  ...        The f
-00001140: 696e 6465 7220 6368 6172 7473 2061 7265  inder charts are
-00001150: 2072 6574 7572 6e65 6420 616c 6f6e 6720   returned along 
-00001160: 7769 7468 2074 6865 2074 696d 6520 696e  with the time in
-00001170: 7465 7276 616c 2074 6865 7920 636f 7665  terval they cove
-00001180: 722e 0a0a 2020 2020 2020 2020 5061 7261  r...        Para
-00001190: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-000011a0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-000011b0: 2020 7374 6172 743a 2060 7e64 6174 6574    start: `~datet
-000011c0: 696d 652e 6461 7465 7469 6d65 600a 2020  ime.datetime`.  
-000011d0: 2020 2020 2020 2020 2020 5468 6520 7374            The st
-000011e0: 6172 7420 7469 6d65 206f 6620 7468 6520  art time of the 
-000011f0: 696e 7465 7276 616c 2074 6f20 6265 2063  interval to be c
-00001200: 6f76 6572 6564 2062 7920 7468 6520 6669  overed by the fi
-00001210: 6e64 6572 2063 6861 7274 732e 2054 6869  nder charts. Thi
-00001220: 7320 6d75 7374 0a20 2020 2020 2020 2020  s must.         
-00001230: 2020 2062 6520 6120 7469 6d65 7a6f 6e65     be a timezone
-00001240: 2d61 7761 7265 2064 6174 6574 696d 652e  -aware datetime.
-00001250: 0a20 2020 2020 2020 2065 6e64 3a20 607e  .        end: `~
-00001260: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-00001270: 6560 0a20 2020 2020 2020 2020 2020 2054  e`.            T
-00001280: 6865 2065 6e64 2074 696d 6520 6f66 2074  he end time of t
-00001290: 6865 2069 6e74 6572 7661 6c20 746f 2062  he interval to b
-000012a0: 6520 636f 7665 7265 6420 6279 2074 6865  e covered by the
-000012b0: 2066 696e 6465 7220 6368 6172 7473 2e20   finder charts. 
-000012c0: 5468 6973 206d 7573 740a 2020 2020 2020  This must.      
-000012d0: 2020 2020 2020 6265 2061 2074 696d 657a        be a timez
-000012e0: 6f6e 652d 6177 6172 6520 6461 7465 7469  one-aware dateti
-000012f0: 6d65 2e0a 2020 2020 2020 2020 6570 6865  me..        ephe
-00001300: 6d65 7269 6465 733a 206c 6973 7420 6f66  merides: list of
-00001310: 2060 7e69 6d65 7068 752e 7574 696c 732e   `~imephu.utils.
-00001320: 4570 6865 6d65 7269 7360 0a20 2020 2020  Ephemeris`.     
-00001330: 2020 2020 2020 2054 6865 206c 6973 7420         The list 
-00001340: 6f66 2065 7068 656d 6572 6964 6573 2e20  of ephemerides. 
-00001350: 5468 6520 7469 6d65 2069 6e74 6572 7661  The time interva
-00001360: 6c20 6672 6f6d 2060 6073 7461 7274 6060  l from ``start``
-00001370: 2074 6f20 6060 656e 6460 6020 6d75 7374   to ``end`` must
-00001380: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
-00001390: 6675 6c6c 7920 636f 7665 7265 6420 6279  fully covered by
-000013a0: 2074 6865 2065 7068 656d 6572 6964 6573   the ephemerides
-000013b0: 2e0a 2020 2020 2020 2020 6d61 785f 7472  ..        max_tr
-000013c0: 6163 6b5f 6c65 6e67 7468 3a20 666c 6f61  ack_length: floa
-000013d0: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
-000013e0: 6520 6d61 7869 6d75 6d20 6c65 6e67 7468  e maximum length
-000013f0: 2061 2074 7261 636b 206d 6179 2068 6176   a track may hav
-00001400: 6520 6f6e 2061 2066 696e 6465 7220 6368  e on a finder ch
-00001410: 6172 742c 2061 7320 616e 2061 6e67 6c65  art, as an angle
-00001420: 206f 6e20 7468 650a 2020 2020 2020 2020   on the.        
-00001430: 2020 2020 736b 792e 0a20 2020 2020 2020      sky..       
-00001440: 2063 7265 6174 655f 6669 6e64 6572 5f63   create_finder_c
-00001450: 6861 7274 3a20 6675 6e63 7469 6f6e 0a20  hart: function. 
-00001460: 2020 2020 2020 2020 2020 2054 6865 2066             The f
-00001470: 756e 6374 696f 6e20 666f 7220 6372 6561  unction for crea
-00001480: 7469 6e67 2061 2066 696e 6465 7220 6368  ting a finder ch
-00001490: 6172 7420 6672 6f6d 2061 206c 6973 7420  art from a list 
-000014a0: 6f66 2065 7068 656d 6572 6964 6573 2e0a  of ephemerides..
-000014b0: 0a20 2020 2020 2020 2059 6965 6c64 730a  .        Yields.
-000014c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0a20          ------. 
-000014d0: 2020 2020 2020 2074 7570 6c65 206f 6620         tuple of 
-000014e0: 6120 607e 696d 6570 6875 2e66 696e 6465  a `~imephu.finde
-000014f0: 725f 6368 6172 742e 4669 6e64 6572 4368  r_chart.FinderCh
-00001500: 6172 7460 2061 6e64 2061 2064 6174 6574  art` and a datet
-00001510: 696d 6520 696e 7465 7276 616c 0a20 2020  ime interval.   
-00001520: 2020 2020 2020 2020 2054 6865 2067 656e           The gen
-00001530: 6572 6174 6564 2066 696e 6465 7220 6368  erated finder ch
-00001540: 6172 7473 2061 6c6f 6e67 2077 6974 6820  arts along with 
-00001550: 7468 6520 7469 6d65 2069 6e74 6572 7661  the time interva
-00001560: 6c73 2074 6865 7920 636f 7665 722e 0a20  ls they cover.. 
-00001570: 2020 2020 2020 204e 7a26 5468 6520 7374         Nz&The st
-00001580: 6172 7420 7469 6d65 206d 7573 7420 6265  art time must be
-00001590: 2074 696d 657a 6f6e 652d 6177 6172 652e   timezone-aware.
-000015a0: 7a24 5468 6520 656e 6420 7469 6d65 206d  z$The end time m
-000015b0: 7573 7420 6265 2074 696d 657a 6f6e 652d  ust be timezone-
-000015c0: 6177 6172 652e 7a31 5468 6520 7374 6172  aware.z1The star
-000015d0: 7420 7469 6d65 206d 7573 7420 6265 2065  t time must be e
-000015e0: 6172 6c69 6572 2074 6861 6e20 7468 6520  arlier than the 
-000015f0: 656e 6420 7469 6d65 2e72 0100 0000 7a38  end time.r....z8
-00001600: 5468 6520 7374 6172 7420 7469 6d65 206d  The start time m
-00001610: 7573 7420 6e6f 7420 6265 2065 6172 6c69  ust not be earli
-00001620: 6572 2074 6861 6e20 7468 6520 6669 7273  er than the firs
-00001630: 7420 6570 6f63 682e e9ff ffff ff7a 3354  t epoch......z3T
-00001640: 6865 2065 6e64 2074 696d 6520 6d75 7374  he end time must
-00001650: 206e 6f74 2062 6520 6c61 7465 7220 7468   not be later th
-00001660: 616e 2074 6865 206c 6173 7420 6570 6f63  an the last epoc
-00001670: 682e 7a2a 5468 6520 6d61 7869 6d75 6d20  h.z*The maximum 
-00001680: 7472 6163 6b20 6c65 6e67 7468 206d 7573  track length mus
-00001690: 7420 6265 2070 6f73 6974 6976 652e 6301  t be positive.c.
-000016a0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000016b0: 0000 0053 0000 0173 1200 0000 6700 7c00  ...S...s....g.|.
-000016c0: 5d05 7d01 7c01 6a00 9102 7102 5300 7229  ].}.|.j...q.S.r)
-000016d0: 0000 0029 01da 0565 706f 6368 2902 da02  ...)...epoch)...
-000016e0: 2e30 da01 6572 2900 0000 7229 0000 0072  .0..er)...r)...r
-000016f0: 2a00 0000 da0a 3c6c 6973 7463 6f6d 703e  *.....<listcomp>
-00001700: 9300 0000 7302 0000 0012 007a 3146 696e  ....s......z1Fin
-00001710: 6465 7243 6861 7274 2e66 6f72 5f74 696d  derChart.for_tim
-00001720: 655f 696e 7465 7276 616c 2e3c 6c6f 6361  e_interval.<loca
-00001730: 6c73 3e2e 3c6c 6973 7463 6f6d 703e e901  ls>.<listcomp>..
-00001740: 0000 007a 2854 6865 2069 6e74 6572 7661  ...z(The interva
-00001750: 6c20 6d75 7374 2068 6176 6520 6120 706f  l must have a po
-00001760: 7369 7469 7665 206c 656e 6774 687a 3754  sitive lengthz7T
-00001770: 6865 206d 6178 696d 756d 2074 7261 636b  he maximum track
-00001780: 206c 656e 6774 6820 6f6e 2061 2066 696e   length on a fin
-00001790: 6465 7220 6368 6172 7420 6973 2065 7863  der chart is exc
-000017a0: 6565 6465 642e 290d da06 747a 696e 666f  eeded.)...tzinfo
-000017b0: da09 7574 636f 6666 7365 74da 0a56 616c  ..utcoffset..Val
-000017c0: 7565 4572 726f 7272 3c00 0000 da08 746f  ueErrorr<.....to
-000017d0: 5f76 616c 7565 da01 75da 0661 7263 6d69  _value..u..arcmi
-000017e0: 6eda 0662 6973 6563 74da 0c62 6973 6563  n..bisect..bisec
-000017f0: 745f 7269 6768 74da 0572 616e 6765 da08  t_right..range..
-00001800: 706f 7369 7469 6f6e da0a 7365 7061 7261  position..separa
-00001810: 7469 6f6e da06 6170 7065 6e64 290e 7233  tion..append).r3
-00001820: 0000 0072 3400 0000 7235 0000 0072 3700  ...r4...r5...r7.
-00001830: 0000 7238 0000 005a 0961 6c6c 5f74 696d  ..r8...Z.all_tim
-00001840: 6573 da0b 7374 6172 745f 696e 6465 78da  es..start_index.
-00001850: 0965 6e64 5f69 6e64 6578 5a0d 6375 7272  .end_indexZ.curr
-00001860: 656e 745f 6772 6f75 70da 0667 726f 7570  ent_group..group
-00001870: 73da 0169 5a0e 6e65 7874 5f65 7068 656d  s..iZ.next_ephem
-00001880: 6572 6973 5a0c 7472 6163 6b5f 6c65 6e67  erisZ.track_leng
-00001890: 7468 da05 6772 6f75 7072 2900 0000 7229  th..groupr)...r)
-000018a0: 0000 0072 2a00 0000 da11 666f 725f 7469  ...r*.....for_ti
-000018b0: 6d65 5f69 6e74 6572 7661 6c4b 0000 0073  me_intervalK...s
-000018c0: 4e00 0000 0280 1a37 0801 1a01 0801 0802  N......7........
-000018d0: 0801 0e02 0801 0e01 0801 1002 0801 0e03  ................
-000018e0: 1001 0c01 1801 0801 0803 0801 0a05 0601  ................
-000018f0: 1601 0801 1003 0201 02ff 02ff 0204 0201  ................
-00001900: 04ff 1203 0801 0c01 0c02 0c01 0803 2001  .............. .
-00001910: 04ff 7a1d 4669 6e64 6572 4368 6172 742e  ..z.FinderChart.
-00001920: 666f 725f 7469 6d65 5f69 6e74 6572 7661  for_time_interva
-00001930: 6c72 1400 0000 6301 0000 0000 0000 0000  lr....c.........
-00001940: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
-00001950: 0a00 0000 7c00 6a00 a001 a100 5300 2902  ....|.j.....S.).
-00001960: 7aa9 5265 7475 726e 2061 2064 6565 7020  z.Return a deep 
-00001970: 636f 7079 206f 6620 7468 6520 5743 5320  copy of the WCS 
-00001980: 6f62 6a65 6374 206f 6620 7468 6520 6669  object of the fi
-00001990: 6e64 6572 2063 6861 7274 2e0a 0a20 2020  nder chart...   
-000019a0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-000019b0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-000019c0: 2020 2020 2060 7e61 7374 726f 7079 2e77       `~astropy.w
-000019d0: 6373 2e57 4353 600a 2020 2020 2020 2020  cs.WCS`.        
-000019e0: 2020 2020 4120 6465 6570 2063 6f70 7920      A deep copy 
-000019f0: 6f66 2074 6865 2057 4353 206f 626a 6563  of the WCS objec
-00001a00: 742e 0a20 2020 2020 2020 204e 2902 7226  t..        N).r&
-00001a10: 0000 00da 0864 6565 7063 6f70 7929 0172  .....deepcopy).r
-00001a20: 2800 0000 7229 0000 0072 2900 0000 722a  (...r)...r)...r*
-00001a30: 0000 00da 0377 6373 b700 0000 7302 0000  .....wcs....s...
-00001a40: 000a 097a 0f46 696e 6465 7243 6861 7274  ...z.FinderChart
-00001a50: 2e77 6373 da0a 616e 6e6f 7461 7469 6f6e  .wcs..annotation
-00001a60: 7217 0000 00da 044e 6f6e 6563 0200 0000  r......Nonec....
-00001a70: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001a80: 4300 0001 7310 0000 007c 006a 00a0 017c  C...s....|.j...|
-00001a90: 01a1 0101 0064 0153 0029 027a fc41 6464  .....d.S.).z.Add
-00001aa0: 2061 6e20 616e 6e6f 7461 7469 6f6e 2074   an annotation t
-00001ab0: 6f20 7468 6520 6669 6e64 6572 2063 6861  o the finder cha
-00001ac0: 7274 2e0a 0a20 2020 2020 2020 2041 6e6e  rt...        Ann
-00001ad0: 6f74 6174 696f 6e73 2077 696c 6c20 6265  otations will be
-00001ae0: 2070 6c6f 7474 6564 206f 6e74 6f20 7468   plotted onto th
-00001af0: 6520 6669 6e64 6572 2063 6861 7274 2069  e finder chart i
-00001b00: 6e20 7468 6520 6f72 6465 7220 7468 6579  n the order they
-00001b10: 2068 6176 6520 6265 656e 0a20 2020 2020   have been.     
-00001b20: 2020 2061 6464 6564 2e20 536f 2c20 666f     added. So, fo
-00001b30: 7220 6578 616d 706c 652c 2074 6865 2061  r example, the a
-00001b40: 6e6e 6f74 6174 696f 6e20 6164 6465 6420  nnotation added 
-00001b50: 6c61 7374 2077 696c 6c20 6265 206f 7574  last will be out
-00001b60: 7075 7420 6f6e 2074 6f70 206f 6620 616c  put on top of al
-00001b70: 6c0a 2020 2020 2020 2020 7468 6520 6f74  l.        the ot
-00001b80: 6865 7220 616e 6e6f 7461 7469 6f6e 732e  her annotations.
-00001b90: 0a20 2020 2020 2020 204e 2902 7227 0000  .        N).r'..
-00001ba0: 0072 4c00 0000 2902 7228 0000 0072 5500  .rL...).r(...rU.
-00001bb0: 0000 7229 0000 0072 2900 0000 722a 0000  ..r)...r)...r*..
-00001bc0: 00da 0e61 6464 5f61 6e6e 6f74 6174 696f  ...add_annotatio
-00001bd0: 6ec2 0000 0073 0200 0000 1007 7a1a 4669  n....s......z.Fi
-00001be0: 6e64 6572 4368 6172 742e 6164 645f 616e  nderChart.add_an
-00001bf0: 6e6f 7461 7469 6f6e 6301 0000 0000 0000  notationc.......
-00001c00: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00001c10: 0173 1e00 0000 7c00 a000 a100 7d01 7401  .s....|.....}.t.
-00001c20: a002 a100 0100 7401 a003 7c01 a101 0100  ......t...|.....
-00001c30: 6401 5300 2902 7a27 4469 7370 6c61 7920  d.S.).z'Display 
-00001c40: 7468 6520 6669 6e64 6572 2063 6861 7274  the finder chart
-00001c50: 206f 6e20 7468 6520 7363 7265 656e 2e4e   on the screen.N
-00001c60: 2904 da0c 5f63 7265 6174 655f 706c 6f74  )..._create_plot
-00001c70: da03 706c 74da 0473 686f 77da 0563 6c6f  ..plt..show..clo
-00001c80: 7365 2902 7228 0000 00da 0666 6967 7572  se).r(.....figur
-00001c90: 6572 2900 0000 7229 0000 0072 2a00 0000  er)...r)...r*...
-00001ca0: 725a 0000 00cb 0000 0073 0600 0000 0802  rZ.......s......
-00001cb0: 0801 0e01 7a10 4669 6e64 6572 4368 6172  ....z.FinderChar
-00001cc0: 742e 7368 6f77 4efa 3a55 6e69 6f6e 5b73  t.showN.:Union[s
-00001cd0: 7472 2c20 4269 6e61 7279 494f 2c20 6f73  tr, BinaryIO, os
-00001ce0: 2e50 6174 684c 696b 655b 7374 725d 2c20  .PathLike[str], 
-00001cf0: 6f73 2e50 6174 684c 696b 655b 6279 7465  os.PathLike[byte
-00001d00: 735d 5dda 0666 6f72 6d61 74fa 0d4f 7074  s]]..format..Opt
-00001d10: 696f 6e61 6c5b 7374 725d 6303 0000 0000  ional[str]c.....
-00001d20: 0000 0000 0000 0007 0000 0008 0000 0043  ...............C
-00001d30: 0000 0173 a600 0000 7c00 a000 a100 7d03  ...s....|.....}.
-00001d40: 7c02 7244 7c02 a001 a100 6401 6b02 7244  |.rD|.....d.k.rD
-00001d50: 7402 8300 7d04 7403 6a04 7c04 7c02 6402  t...}.t.j.|.|.d.
-00001d60: 6403 8d03 0100 7405 a006 7c04 a007 a100  d.....t...|.....
-00001d70: a101 7d05 7408 7c01 6404 8302 7229 7c01  ..}.t.|.d...r)|.
-00001d80: a009 7c05 a101 0100 6e23 740a 7c01 6405  ..|.....n#t.|.d.
-00001d90: 8302 8f0d 7d06 7c06 a009 7c05 a101 0100  ....}.|...|.....
-00001da0: 5700 6406 0400 0400 8303 0100 6e11 3100  W.d.........n.1.
-00001db0: 733e 7701 0100 0100 0100 5900 0100 6e08  s>w.......Y...n.
-00001dc0: 7403 6a04 7c01 7c02 6402 6403 8d03 0100  t.j.|.|.d.d.....
-00001dd0: 7403 a00b 7c03 a101 0100 6406 5300 2907  t...|.....d.S.).
-00001de0: 6147 0200 0053 6176 6520 7468 6520 6669  aG...Save the fi
-00001df0: 6e64 6572 2063 6861 7274 2069 6e20 6120  nder chart in a 
-00001e00: 6669 6c65 2e0a 0a20 2020 2020 2020 2049  file...        I
-00001e10: 6620 6066 6f72 6d61 7460 2069 7320 6e6f  f `format` is no
-00001e20: 7420 7365 742c 2074 6865 2066 696c 6520  t set, the file 
-00001e30: 6578 7465 6e73 696f 6e20 6f66 2060 6e61  extension of `na
-00001e40: 6d65 6020 6973 2075 7365 6420 746f 2066  me` is used to f
-00001e50: 6967 7572 6520 6f75 7420 7468 650a 2020  igure out the.  
-00001e60: 2020 2020 2020 6669 6c65 206f 722c 2069        file or, i
-00001e70: 6620 7468 6572 6520 6973 206e 6f20 6578  f there is no ex
-00001e80: 7465 6e73 696f 6e2c 204d 6174 706c 6f74  tension, Matplot
-00001e90: 6c69 6227 7320 6465 6661 756c 7420 6973  lib's default is
-00001ea0: 2075 7365 642e 2053 6565 0a20 2020 2020   used. See.     
-00001eb0: 2020 204d 6174 706c 6f74 6c69 6227 7320     Matplotlib's 
-00001ec0: 606d 6174 706c 6f74 6c69 622e 7079 706c  `matplotlib.pypl
-00001ed0: 6f74 2e73 6176 6566 6967 6020 6675 6e63  ot.savefig` func
-00001ee0: 7469 6f6e 2066 6f72 206d 6f72 6520 6465  tion for more de
-00001ef0: 7461 696c 7320 7265 6761 7264 696e 670a  tails regarding.
-00001f00: 2020 2020 2020 2020 7468 6520 666f 726d          the form
-00001f10: 6174 2e0a 0a20 2020 2020 2020 2050 6172  at...        Par
-00001f20: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00001f30: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00001f40: 2020 206e 616d 653a 2060 7374 7260 2c20     name: `str`, 
-00001f50: 6070 6174 682d 6c69 6b65 6020 6f72 2060  `path-like` or `
-00001f60: 6269 6e61 7279 2066 696c 652d 6c69 6b65  binary file-like
-00001f70: 600a 2020 2020 2020 2020 2020 2020 5468  `.            Th
-00001f80: 6520 6669 6c65 2074 6f20 7768 6963 6820  e file to which 
-00001f90: 7468 6520 6669 6e64 6572 2063 6861 7274  the finder chart
-00001fa0: 2069 7320 7361 7665 642e 2041 6e20 6578   is saved. An ex
-00001fb0: 6973 7469 6e67 2066 696c 6520 6973 2072  isting file is r
-00001fc0: 6570 6c61 6365 642e 0a20 2020 2020 2020  eplaced..       
-00001fd0: 2066 6f72 6d61 743a 2060 7374 7260 2c20   format: `str`, 
-00001fe0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00001ff0: 2020 2020 2054 6865 2066 6f72 6d61 7420       The format 
-00002000: 696e 2077 6869 6368 2074 6f20 7374 6f72  in which to stor
-00002010: 6520 7468 6520 6669 6e64 6572 2063 6861  e the finder cha
-00002020: 7274 2e0a 2020 2020 2020 2020 da03 7064  rt..        ..pd
-00002030: 66da 0574 6967 6874 2902 725e 0000 00da  f..tight).r^....
-00002040: 0b62 626f 785f 696e 6368 6573 da05 7772  .bbox_inches..wr
-00002050: 6974 65da 0277 624e 290c 7258 0000 00da  ite..wbN).rX....
-00002060: 056c 6f77 6572 7204 0000 0072 5900 0000  .lowerr....rY...
-00002070: da07 7361 7665 6669 6772 1a00 0000 da14  ..savefigr......
-00002080: 5f75 7064 6174 655f 7064 665f 6d65 7461  _update_pdf_meta
-00002090: 6461 7461 da08 6765 7476 616c 7565 da07  data..getvalue..
-000020a0: 6861 7361 7474 7272 6300 0000 721f 0000  hasattrrc...r...
-000020b0: 0072 5b00 0000 2907 7228 0000 0072 1b00  .r[...).r(...r..
-000020c0: 0000 725e 0000 0072 5c00 0000 7260 0000  ..r^...r\...r`..
-000020d0: 005a 1170 6466 5f77 6974 685f 6d65 7461  .Z.pdf_with_meta
-000020e0: 6461 7461 da01 6672 2900 0000 7229 0000  data..fr)...r)..
-000020f0: 0072 2a00 0000 da04 7361 7665 d100 0000  .r*.....save....
-00002100: 7318 0000 0008 1310 0106 0110 010e 010a  s...............
-00002110: 010c 010c 020c 011e ff10 030e 017a 1046  .............z.F
-00002120: 696e 6465 7243 6861 7274 2e73 6176 6572  inderChart.saver
-00002130: 1600 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00002140: 0004 0000 0005 0000 0043 0000 0173 5800  .........C...sX.
-00002150: 0000 7400 6a01 6401 6402 8d01 7d01 7400  ..t.j.d.d...}.t.
-00002160: 6a02 7c00 6a03 6403 8d01 7d02 7c00 a004  j.|.j.d...}.|...
-00002170: 7c02 a101 0100 7c00 a005 7c02 a101 0100  |.....|...|.....
-00002180: 7c02 6a06 6404 6405 6406 6407 8d03 0100  |.j.d.d.d.d.....
-00002190: 7c00 6a07 4400 5d07 7d03 7c03 a008 7c02  |.j.D.].}.|...|.
-000021a0: a101 0100 7122 7c01 5300 2908 4e29 02e9  ....q"|.S.).N)..
-000021b0: 0a00 0000 e909 0000 0029 01da 0766 6967  .........)...fig
-000021c0: 7369 7a65 2901 da0a 7072 6f6a 6563 7469  size)...projecti
-000021d0: 6f6e 54da 0462 6c75 6567 9a99 9999 9999  onT..blueg......
-000021e0: c93f 2902 da05 636f 6c6f 72da 0561 6c70  .?)...color..alp
-000021f0: 6861 2909 7259 0000 0072 5c00 0000 da07  ha).rY...r\.....
-00002200: 7375 6270 6c6f 7472 2600 0000 da11 5f61  subplotr&....._a
-00002210: 6464 5f66 6974 735f 636f 6e74 656e 74da  dd_fits_content.
-00002220: 0c5f 7570 6461 7465 5f61 7865 73da 0467  ._update_axes..g
-00002230: 7269 6472 2700 0000 da06 6164 645f 746f  ridr'.....add_to
-00002240: 2904 7228 0000 0072 5c00 0000 da02 6178  ).r(...r\.....ax
-00002250: 7255 0000 0072 2900 0000 7229 0000 0072  rU...r)...r)...r
-00002260: 2a00 0000 7258 0000 00f2 0000 0073 1000  *...rX.......s..
-00002270: 0000 0c01 0e01 0a02 0a01 1002 0a02 0c01  ................
-00002280: 0402 7a18 4669 6e64 6572 4368 6172 742e  ..z.FinderChart.
-00002290: 5f63 7265 6174 655f 706c 6f74 7278 0000  _create_plotrx..
-000022a0: 0072 1300 0000 6302 0000 0000 0000 0000  .r....c.........
-000022b0: 0000 0009 0000 0008 0000 0043 0000 0173  ...........C...s
-000022c0: 8400 0000 7400 6a01 a002 6401 a101 7d02  ....t.j...d...}.
-000022d0: 6402 7d03 6403 7d04 7403 7c03 7c04 6404  d.}.d.}.t.|.|.d.
-000022e0: 6405 8d03 7d05 7c05 a004 7c00 6a05 6a06  d...}.|...|.j.j.
-000022f0: a101 5c02 7d06 7d07 6406 7c07 7c06 1800  ..\.}.}.d.|.|...
-00002300: 1400 7c06 1700 7d06 6407 7c07 7c06 1800  ..|...}.d.|.|...
-00002310: 1400 7c07 1700 7d07 7407 7c00 6a08 6408  ..|...}.t.|.j.d.
-00002320: 7c06 7c07 6409 8d04 7d08 7c01 6a09 7c00  |.|.d...}.|.j.|.
-00002330: 6a05 6a06 7c02 640a 640b 7c08 640c 640d  j.j.|.d.d.|.d.d.
-00002340: 8d06 0100 640e 5300 290f 7a6b 0a20 2020  ....d.S.).zk.   
-00002350: 2020 2020 2020 4164 6420 636f 6e74 656e        Add conten
-00002360: 7420 6f66 2074 6865 2046 4954 5320 6669  t of the FITS fi
-00002370: 6c65 2074 6f20 7468 6520 706c 6f74 2e0a  le to the plot..
-00002380: 0a20 2020 2020 2020 2054 6865 2063 6f64  .        The cod
-00002390: 6520 6861 7320 6265 656e 2061 6461 7074  e has been adapt
-000023a0: 6564 2066 726f 6d20 4150 4c70 792e 0a20  ed from APLpy.. 
-000023b0: 2020 2020 2020 20da 0967 6973 745f 7961         ..gist_ya
-000023c0: 7267 6700 0000 0000 00d0 3f67 0000 0000  rgg.......?g....
-000023d0: 00f0 5840 6910 2700 0029 01da 096e 5f73  ..X@i.'..)...n_s
-000023e0: 616d 706c 6573 679a 9999 9999 99b9 bf67  amplesg........g
-000023f0: 9a99 9999 9999 b93f e902 0000 0029 03da  .......?.....)..
-00002400: 0570 6f77 6572 da07 6d69 6e5f 6375 74da  .power..min_cut.
-00002410: 076d 6178 5f63 7574 da07 6e65 6172 6573  .max_cut..neares
-00002420: 7472 6500 0000 da05 6571 7561 6c29 05da  tre.....equal)..
-00002430: 0463 6d61 70da 0d69 6e74 6572 706f 6c61  .cmap..interpola
-00002440: 7469 6f6e da06 6f72 6967 696e da04 6e6f  tion..origin..no
-00002450: 726d da06 6173 7065 6374 4e29 0a72 5900  rm..aspectN).rY.
-00002460: 0000 da02 636d da08 6765 745f 636d 6170  ....cm..get_cmap
-00002470: 7211 0000 00da 0a67 6574 5f6c 696d 6974  r......get_limit
-00002480: 7372 2000 0000 7221 0000 0072 1200 0000  sr ...r!...r....
-00002490: 7222 0000 00da 0669 6d73 686f 7729 0972  r".....imshow).r
-000024a0: 2800 0000 7278 0000 0072 8100 0000 5a04  (...rx...r....Z.
-000024b0: 706d 696e da04 706d 6178 da08 696e 7465  pmin..pmax..inte
-000024c0: 7276 616c da04 766d 696e da04 766d 6178  rval..vmin..vmax
-000024d0: da0a 6e6f 726d 616c 697a 6572 7229 0000  ..normalizerr)..
-000024e0: 0072 2900 0000 722a 0000 0072 7400 0000  .r)...r*...rt...
-000024f0: 0001 0000 7320 0000 000c 0604 0304 010e  ....s ..........
-00002500: 0112 0110 0110 0112 0204 0206 0102 0102  ................
-00002510: 0102 0102 0102 010a fa7a 1d46 696e 6465  .........z.Finde
-00002520: 7243 6861 7274 2e5f 6164 645f 6669 7473  rChart._add_fits
-00002530: 5f63 6f6e 7465 6e74 6302 0000 0000 0000  _contentc.......
-00002540: 0000 0000 0008 0000 0004 0000 0043 0000  .............C..
-00002550: 0173 a200 0000 6401 6402 6403 9c02 7d02  .s....d.d.d...}.
-00002560: 7c00 6a00 6a01 7d03 7c03 6404 1900 7d04  |.j.j.}.|.d...}.
-00002570: 7c03 6405 1900 7d05 7c04 6406 6b03 7219  |.d...}.|.d.k.r.
-00002580: 7402 6407 8301 8201 7c05 6408 6b03 7221  t.d.....|.d.k.r!
-00002590: 7402 6409 8301 8201 7c01 6a03 6404 1900  t.d.....|.j.d...
-000025a0: 7d06 7c01 6a03 6405 1900 7d07 7c06 a004  }.|.j.d...}.|...
-000025b0: 7c02 7c04 1900 a101 0100 7c07 a004 7c02  |.|.......|...|.
-000025c0: 7c05 1900 a101 0100 7c06 a005 640a a101  |.......|...d...
-000025d0: 0100 7c07 a005 640a a101 0100 7c06 6a06  ..|...d.....|.j.
-000025e0: 640b 640c 8d01 0100 7c07 6a06 640b 640c  d.d.....|.j.d.d.
-000025f0: 8d01 0100 6400 5300 290d 4e7a 0a44 6563  ....d.S.).Nz.Dec
-00002600: 2028 4943 5253 297a 0952 4120 2849 4352   (ICRS)z.RA (ICR
-00002610: 5329 2902 fa0a 706f 732e 6571 2e64 6563  S))...pos.eq.dec
-00002620: fa09 706f 732e 6571 2e72 6172 0100 0000  ..pos.eq.rar....
-00002630: 7240 0000 0072 9000 0000 7a49 4f6e 6c79  r@...r....zIOnly
-00002640: 2070 6f73 2e65 712e 7261 2069 7320 7375   pos.eq.ra is su
-00002650: 7070 6f72 7465 6420 666f 7220 7468 6520  pported for the 
-00002660: 7068 7973 6963 616c 2074 7970 6520 6f66  physical type of
-00002670: 2074 6865 2066 6972 7374 2077 6f72 6c64   the first world
-00002680: 2061 7869 7372 8f00 0000 7a4b 4f6e 6c79   axisr....zKOnly
-00002690: 2070 6f73 2e65 712e 6465 6320 6973 2073   pos.eq.dec is s
-000026a0: 7570 706f 7274 6564 2066 6f72 2074 6865  upported for the
-000026b0: 2070 6879 7369 6361 6c20 7479 7065 206f   physical type o
-000026c0: 6620 7468 6520 7365 636f 6e64 2077 6f72  f the second wor
-000026d0: 6c64 2061 7869 7354 e907 0000 0029 0172  ld axisT.....).r
-000026e0: 2f00 0000 2907 7226 0000 00da 1977 6f72  /...).r&.....wor
-000026f0: 6c64 5f61 7869 735f 7068 7973 6963 616c  ld_axis_physical
-00002700: 5f74 7970 6573 7243 0000 00da 0663 6f6f  _typesrC.....coo
-00002710: 7264 73da 0d73 6574 5f61 7869 736c 6162  rds..set_axislab
-00002720: 656c da13 6469 7370 6c61 795f 6d69 6e6f  el..display_mino
-00002730: 725f 7469 636b 73da 0973 6574 5f74 6963  r_ticks..set_tic
-00002740: 6b73 2908 7228 0000 0072 7800 0000 da0f  ks).r(...rx.....
-00002750: 6178 6973 5f74 7970 655f 6e61 6d65 73da  axis_type_names.
-00002760: 0a61 7869 735f 7479 7065 735a 0b78 5f61  .axis_typesZ.x_a
-00002770: 7869 735f 7479 7065 5a0b 795f 6178 6973  xis_typeZ.y_axis
-00002780: 5f74 7970 65da 0178 da01 7972 2900 0000  _type..x..yr)...
-00002790: 7229 0000 0072 2a00 0000 7275 0000 001b  r)...r*...ru....
-000027a0: 0100 0073 2c00 0000 0202 0201 06fe 0804  ...s,...........
-000027b0: 0801 0801 0801 0201 0201 04ff 0804 0201  ................
-000027c0: 0201 04ff 0a05 0a01 0e01 0e01 0a02 0a01  ................
-000027d0: 0c02 1001 7a18 4669 6e64 6572 4368 6172  ....z.FinderChar
-000027e0: 742e 5f75 7064 6174 655f 6178 6573 7260  t._update_axesr`
-000027f0: 0000 00da 0562 7974 6573 6301 0000 0000  .....bytesc.....
-00002800: 0000 0000 0000 0004 0000 0009 0000 0043  ...............C
-00002810: 0000 0173 8a00 0000 7400 a001 7402 7c00  ...s....t...t.|.
-00002820: 8301 a101 8f34 7d01 7c01 a003 a100 8f14  .....4}.|.......
-00002830: 7d02 6401 7c02 6402 3c00 6403 7404 6a05  }.d.|.d.<.d.t.j.
-00002840: 9b00 9d02 7c02 6404 3c00 5700 6405 0400  ....|.d.<.W.d...
-00002850: 0400 8303 0100 6e08 3100 7323 7701 0100  ......n.1.s#w...
-00002860: 0100 0100 5900 0100 7402 8300 7d03 7c01  ....Y...t...}.|.
-00002870: a006 7c03 a101 0100 7c03 a007 a100 5700  ..|.....|.....W.
-00002880: 0200 6405 0400 0400 8303 0100 5300 3100  ..d.........S.1.
-00002890: 733e 7701 0100 0100 0100 5900 0100 6405  s>w.......Y...d.
-000028a0: 5300 2906 6150 0300 0055 7064 6174 6520  S.).aP...Update 
-000028b0: 6120 7064 6620 6279 2073 6574 7469 6e67  a pdf by setting
-000028c0: 2073 6f6d 6520 6d65 7461 6461 7461 2076   some metadata v
-000028d0: 616c 7565 732e 0a0a 2020 2020 2020 2020  alues...        
-000028e0: 5468 6520 666f 6c6c 6f77 696e 6720 6d65  The following me
-000028f0: 7461 6461 7461 2076 616c 7565 7320 6172  tadata values ar
-00002900: 6520 7365 743a 0a0a 2020 2020 2020 2020  e set:..        
-00002910: 2d20 6060 6463 3a74 6974 6c65 6060 3a20  - ``dc:title``: 
-00002920: 5468 6520 7374 7269 6e67 2060 6069 6d65  The string ``ime
-00002930: 7068 7520 782e 792e 7a60 6020 6973 2061  phu x.y.z`` is a
-00002940: 7373 6967 6e65 6420 2877 6865 7265 2060  ssigned (where `
-00002950: 6078 2e79 2e7a 6060 2069 7320 7468 650a  `x.y.z`` is the.
-00002960: 2020 2020 2020 2020 2020 7665 7273 696f            versio
-00002970: 6e29 2e0a 2020 2020 2020 2020 2d20 6060  n)..        - ``
-00002980: 786d 703a 4372 6561 746f 7254 6f6f 6c60  xmp:CreatorTool`
-00002990: 603a 2041 2073 7472 696e 6720 6f66 2074  `: A string of t
-000029a0: 6865 2066 6f72 6d20 2269 6d65 7068 7520  he form "imephu 
-000029b0: 782e 792e 7a22 2069 7320 6173 7369 676e  x.y.z" is assign
-000029c0: 6564 2e0a 0a20 2020 2020 2020 2054 6865  ed...        The
-000029d0: 2072 6573 756c 7469 6e67 2070 6466 2069   resulting pdf i
-000029e0: 7320 7265 7475 726e 6564 3b20 7468 6520  s returned; the 
-000029f0: 6f72 6967 696e 616c 2070 6466 2072 656d  original pdf rem
-00002a00: 6169 6e73 2075 6e63 6861 6e67 6564 2e0a  ains unchanged..
-00002a10: 0a20 2020 2020 2020 2053 6565 2074 6865  .        See the
-00002a20: 2043 6f72 6520 7072 6f70 6572 7469 6573   Core properties
-00002a30: 2063 6861 7074 6572 206f 6620 7468 6520   chapter of the 
-00002a40: 6058 4d50 2073 7065 6369 6669 6361 7469  `XMP specificati
-00002a50: 6f6e 0a20 2020 2020 2020 203c 6874 7470  on.        <http
-00002a60: 733a 2f2f 7777 7769 6d61 6765 7332 2e61  s://wwwimages2.a
-00002a70: 646f 6265 2e63 6f6d 2f63 6f6e 7465 6e74  dobe.com/content
-00002a80: 2f64 616d 2f61 636f 6d2f 656e 2f64 6576  /dam/acom/en/dev
-00002a90: 6e65 742f 786d 702f 7064 6673 2f58 4d50  net/xmp/pdfs/XMP
-00002aa0: 2532 3053 444b 2532 3052 656c 6561 7365  %20SDK%20Release
-00002ab0: 2532 3063 632d 3230 3136 2d30 382f 584d  %20cc-2016-08/XM
-00002ac0: 5053 7065 6369 6669 6361 7469 6f6e 5061  PSpecificationPa
-00002ad0: 7274 312e 7064 663e 605f 0a20 2020 2020  rt1.pdf>`_.     
-00002ae0: 2020 2066 6f72 206d 6f72 6520 6465 7461     for more deta
-00002af0: 696c 7320 6162 6f75 7420 7468 6520 6d65  ils about the me
-00002b00: 7461 6461 7461 2070 726f 7065 7274 6965  tadata propertie
-00002b10: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
-00002b20: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00002b30: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00002b40: 2020 7064 663a 2060 6279 7465 7360 0a20    pdf: `bytes`. 
-00002b50: 2020 2020 2020 2020 2020 2054 6865 2070             The p
-00002b60: 6466 2077 686f 7365 2060 6078 6d6c 3a63  df whose ``xml:c
-00002b70: 7265 6174 6f72 546f 6f6c 6060 206d 6574  reatorTool`` met
-00002b80: 6164 6174 6120 7661 6c75 6520 7368 6f75  adata value shou
-00002b90: 6c64 2062 6520 7365 742e 0a0a 2020 2020  ld be set...    
-00002ba0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00002bb0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00002bc0: 2020 2020 6062 7974 6573 600a 2020 2020      `bytes`.    
-00002bd0: 2020 2020 2020 2020 5468 6520 7570 6461          The upda
-00002be0: 7465 6420 7064 6620 636f 6e74 656e 742e  ted pdf content.
-00002bf0: 0a20 2020 2020 2020 207a 0c46 696e 6465  .        z.Finde
-00002c00: 7220 4368 6172 747a 0864 633a 7469 746c  r Chartz.dc:titl
-00002c10: 657a 0769 6d65 7068 7520 7a0f 786d 703a  ez.imephu z.xmp:
-00002c20: 4372 6561 746f 7254 6f6f 6c4e 2908 da07  CreatorToolN)...
-00002c30: 7069 6b65 7064 6672 1f00 0000 7204 0000  pikepdfr....r...
-00002c40: 005a 0d6f 7065 6e5f 6d65 7461 6461 7461  .Z.open_metadata
-00002c50: da06 696d 6570 6875 da0b 5f5f 7665 7273  ..imephu..__vers
-00002c60: 696f 6e5f 5f72 6b00 0000 7268 0000 0029  ion__rk...rh...)
-00002c70: 0472 6000 0000 da08 646f 6375 6d65 6e74  .r`.....document
-00002c80: da04 6d65 7461 5a0b 7570 6461 7465 645f  ..metaZ.updated_
-00002c90: 7064 6672 2900 0000 7229 0000 0072 2a00  pdfr)...r)...r*.
-00002ca0: 0000 7267 0000 0039 0100 0073 1200 0000  ..rg...9...s....
-00002cb0: 101a 0a01 0801 1201 1cfe 0603 0a01 0601  ................
-00002cc0: 24fa 7a20 4669 6e64 6572 4368 6172 742e  $.z FinderChart.
-00002cd0: 5f75 7064 6174 655f 7064 665f 6d65 7461  _update_pdf_meta
-00002ce0: 6461 7461 2902 721b 0000 0072 1c00 0000  data).r....r....
-00002cf0: 2908 722c 0000 0072 2d00 0000 722e 0000  ).r,...r-...r...
-00002d00: 0072 0f00 0000 722f 0000 0072 0e00 0000  .r....r/...r....
-00002d10: 7230 0000 0072 3100 0000 290c 7233 0000  r0...r1...).r3..
-00002d20: 0072 0300 0000 7234 0000 0072 0300 0000  .r....r4...r....
-00002d30: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
-00002d40: 0e00 0000 7238 0000 0072 3900 0000 7230  ....r8...r9...r0
-00002d50: 0000 0072 3a00 0000 2902 7230 0000 0072  ...r:...).r0...r
-00002d60: 1400 0000 2904 7255 0000 0072 1700 0000  ....).rU...r....
-00002d70: 7230 0000 0072 5600 0000 2902 7230 0000  r0...rV...).r0..
-00002d80: 0072 5600 0000 2901 4e29 0672 1b00 0000  .rV...).N).r....
-00002d90: 725d 0000 0072 5e00 0000 725f 0000 0072  r]...r^...r_...r
-00002da0: 3000 0000 7256 0000 0029 0272 3000 0000  0...rV...).r0...
-00002db0: 7216 0000 0029 0472 7800 0000 7213 0000  r....).rx...r...
-00002dc0: 0072 3000 0000 7256 0000 0029 0472 6000  .r0...rV...).r`.
-00002dd0: 0000 729b 0000 0072 3000 0000 729b 0000  ..r....r0...r...
-00002de0: 0029 11da 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
-00002df0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00002e00: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00002e10: 722b 0000 00da 0c73 7461 7469 636d 6574  r+.....staticmet
-00002e20: 686f 6472 3200 0000 7252 0000 00da 0870  hodr2...rR.....p
-00002e30: 726f 7065 7274 7972 5400 0000 7257 0000  ropertyrT...rW..
-00002e40: 0072 5a00 0000 726b 0000 0072 5800 0000  .rZ...rk...rX...
-00002e50: 7274 0000 0072 7500 0000 7267 0000 0072  rt...ru...rg...r
-00002e60: 2900 0000 7229 0000 0072 2900 0000 722a  )...r)...r)...r*
-00002e70: 0000 0072 1a00 0000 1d00 0000 7324 0000  ...r........s$..
-00002e80: 0008 0004 010a 1302 0a0c 0102 0f0c 0102  ................
-00002e90: 6b0c 010a 0a0a 0902 090c fd0a 210a 0e0a  k...........!...
-00002ea0: 1b02 1e10 0172 1a00 0000 2930 da0a 5f5f  .....r....)0..__
-00002eb0: 6675 7475 7265 5f5f 7202 0000 0072 4700  future__r....rG.
-00002ec0: 0000 da02 6f73 7223 0000 0072 0300 0000  ....osr#...r....
-00002ed0: da02 696f 7204 0000 00da 0674 7970 696e  ..ior......typin
-00002ee0: 6772 0500 0000 7206 0000 0072 0700 0000  gr....r....r....
-00002ef0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00002f00: 0b00 0000 720c 0000 00da 116d 6174 706c  ....r......matpl
-00002f10: 6f74 6c69 622e 7079 706c 6f74 da06 7079  otlib.pyplot..py
-00002f20: 706c 6f74 7259 0000 0072 9c00 0000 da07  plotrY...r......
-00002f30: 6173 7472 6f70 7972 0d00 0000 7245 0000  astropyr....rE..
-00002f40: 00da 1361 7374 726f 7079 2e63 6f6f 7264  ...astropy.coord
-00002f50: 696e 6174 6573 720e 0000 0072 0f00 0000  inatesr....r....
-00002f60: da0a 6173 7472 6f70 792e 696f 7210 0000  ..astropy.ior...
-00002f70: 005a 1e61 7374 726f 7079 2e76 6973 7561  .Z.astropy.visua
-00002f80: 6c69 7a61 7469 6f6e 2e69 6e74 6572 7661  lization.interva
-00002f90: 6c72 1100 0000 5a23 6173 7472 6f70 792e  lr....Z#astropy.
-00002fa0: 7669 7375 616c 697a 6174 696f 6e2e 6d70  visualization.mp
-00002fb0: 6c5f 6e6f 726d 616c 697a 6572 1200 0000  l_normalizer....
-00002fc0: 5a22 6173 7472 6f70 792e 7669 7375 616c  Z"astropy.visual
-00002fd0: 697a 6174 696f 6e2e 7763 7361 7865 732e  ization.wcsaxes.
-00002fe0: 636f 7265 7213 0000 00da 0b61 7374 726f  corer......astro
-00002ff0: 7079 2e77 6373 7214 0000 0072 1500 0000  py.wcsr....r....
-00003000: da11 6d61 7470 6c6f 746c 6962 2e66 6967  ..matplotlib.fig
-00003010: 7572 6572 1600 0000 729d 0000 005a 1169  urer....r....Z.i
-00003020: 6d65 7068 752e 616e 6e6f 7461 7469 6f6e  mephu.annotation
-00003030: 7217 0000 005a 1569 6d65 7068 752e 7365  r....Z.imephu.se
-00003040: 7276 6963 652e 7375 7276 6579 7218 0000  rvice.surveyr...
-00003050: 00da 0c69 6d65 7068 752e 7574 696c 7372  ...imephu.utilsr
-00003060: 1900 0000 721a 0000 0072 2900 0000 7229  ....r....r)...r)
-00003070: 0000 0072 2900 0000 722a 0000 00da 083c  ...r)...r*.....<
-00003080: 6d6f 6475 6c65 3e01 0000 0073 2e00 0000  module>....s....
-00003090: 0c00 0802 0801 0801 0c01 0c01 2801 0c02  ............(...
-000030a0: 0801 0c01 1001 0c01 0c01 0c01 0c01 1001  ................
-000030b0: 0c01 0802 0c01 0c01 0c01 0202 1203       ..............
+00000090: 6d11 5a11 0100 6400 6402 6c12 6d13 5a14  m.Z...d.d.l.m.Z.
+000000a0: 0100 6400 6406 6c15 6d16 5a17 0100 6400  ..d.d.l.m.Z...d.
+000000b0: 6407 6c18 6d19 5a19 6d1a 5a1a 0100 6400  d.l.m.Z.m.Z...d.
+000000c0: 6408 6c1b 6d1c 5a1c 0100 6400 6409 6c1d  d.l.m.Z...d.d.l.
+000000d0: 6d1e 5a1e 0100 6400 640a 6c1f 6d20 5a20  m.Z...d.d.l.m Z 
+000000e0: 0100 6400 640b 6c21 6d22 5a22 0100 6400  ..d.d.l!m"Z"..d.
+000000f0: 640c 6c23 6d24 5a24 6d25 5a25 0100 6400  d.l#m$Z$m%Z%..d.
+00000100: 640d 6c26 6d27 5a27 0100 6400 640e 6c28  d.l&m'Z'..d.d.l(
+00000110: 6d29 5a29 0100 6400 640f 6c2a 6d2b 5a2b  m)Z)..d.d.l*m+Z+
+00000120: 0100 6400 6410 6c2c 6d2d 5a2d 0100 0900  ..d.d.l,m-Z-....
+00000130: 4700 6411 6412 8400 6412 8302 5a2e 6402  G.d.d...d...Z.d.
+00000140: 5300 2913 e900 0000 0029 01da 0b61 6e6e  S.)......)...ann
+00000150: 6f74 6174 696f 6e73 4e29 01da 0864 6174  otationsN)...dat
+00000160: 6574 696d 6529 01da 0742 7974 6573 494f  etime)...BytesIO
+00000170: 2909 da03 416e 79da 0842 696e 6172 7949  )...Any..BinaryI
+00000180: 4fda 0843 616c 6c61 626c 65da 0444 6963  O..Callable..Dic
+00000190: 74da 0947 656e 6572 6174 6f72 da04 4c69  t..Generator..Li
+000001a0: 7374 da08 4f70 7469 6f6e 616c da05 5475  st..Optional..Tu
+000001b0: 706c 65da 0555 6e69 6f6e 2901 da05 756e  ple..Union)...un
+000001c0: 6974 7329 02da 0541 6e67 6c65 da08 536b  its)...Angle..Sk
+000001d0: 7943 6f6f 7264 2901 da04 6669 7473 2901  yCoord)...fits).
+000001e0: da1c 4173 796d 6d65 7472 6963 5065 7263  ..AsymmetricPerc
+000001f0: 656e 7469 6c65 496e 7465 7276 616c 2901  entileInterval).
+00000200: da0b 7369 6d70 6c65 5f6e 6f72 6d29 01da  ..simple_norm)..
+00000210: 0e57 4353 4178 6573 5375 6270 6c6f 7429  .WCSAxesSubplot)
+00000220: 02da 0357 4353 da10 4649 5453 4669 7865  ...WCS..FITSFixe
+00000230: 6457 6172 6e69 6e67 2901 da06 4669 6775  dWarning)...Figu
+00000240: 7265 2901 da0a 416e 6e6f 7461 7469 6f6e  re)...Annotation
+00000250: 2901 da09 6c6f 6164 5f66 6974 7329 01da  )...load_fits)..
+00000260: 0945 7068 656d 6572 6973 6300 0000 0000  .Ephemerisc.....
+00000270: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
+00000280: 0000 0173 9c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000290: 6401 5a03 643c 6404 6405 8404 5a04 6505  d.Z.d<d.d...Z.e.
+000002a0: 643d 640e 640f 8404 8301 5a06 6505 643e  d=d.d.....Z.e.d>
+000002b0: 6419 641a 8404 8301 5a07 6508 643f 641c  d.d.....Z.e.d?d.
+000002c0: 641d 8404 8301 5a09 6440 6421 6422 8404  d.....Z.d@d!d"..
+000002d0: 5a0a 6508 6441 6424 6425 8404 8301 5a0b  Z.e.dAd$d%....Z.
+000002e0: 6442 6429 642a 8404 5a0c 6443 642b 642c  dBd)d*..Z.dCd+d,
+000002f0: 8404 5a0d 092d 6444 6445 6431 6432 8405  ..Z..-dDdEd1d2..
+00000300: 5a0e 6446 6434 6435 8404 5a0f 6447 6438  Z.dFd4d5..Z.dGd8
+00000310: 6439 8404 5a10 6447 643a 643b 8404 5a11  d9..Z.dGd:d;..Z.
+00000320: 642d 5300 2948 da0b 4669 6e64 6572 4368  d-S.)H..FinderCh
+00000330: 6172 7461 ad02 0000 4120 6669 6e64 6572  arta....A finder
+00000340: 2063 6861 7274 2066 6f72 2061 6e20 6173   chart for an as
+00000350: 7472 6f6e 6f6d 6963 616c 206f 6273 6572  tronomical obser
+00000360: 7661 7469 6f6e 2e0a 0a20 2020 2054 6865  vation...    The
+00000370: 2066 696e 6465 7220 6368 6172 7420 6973   finder chart is
+00000380: 2067 656e 6572 6174 6564 2066 726f 6d20   generated from 
+00000390: 6120 4649 5453 2066 696c 652e 2042 7920  a FITS file. By 
+000003a0: 6465 6661 756c 7420 7468 6520 6669 6e64  default the find
+000003b0: 6572 2063 6861 7274 206a 7573 740a 2020  er chart just.  
+000003c0: 2020 7368 6f77 7320 7468 6520 7265 6769    shows the regi
+000003d0: 6f6e 2077 6974 6820 616e 206f 7665 726c  on with an overl
+000003e0: 6169 6420 636f 6f72 6469 6e61 7465 2067  aid coordinate g
+000003f0: 7269 642e 2054 6865 2061 7865 7320 7368  rid. The axes sh
+00000400: 6f77 2057 4353 2063 6f6f 7264 696e 6174  ow WCS coordinat
+00000410: 6573 2e0a 2020 2020 5573 6520 7468 6520  es..    Use the 
+00000420: 6061 6464 5f61 6e6e 6f74 6174 696f 6e60  `add_annotation`
+00000430: 206d 6574 686f 6420 746f 2061 6464 206d   method to add m
+00000440: 6f72 6520 636f 6e74 656e 7420 746f 2074  ore content to t
+00000450: 6865 2066 696e 6465 7220 6368 6172 742e  he finder chart.
+00000460: 0a0a 2020 2020 596f 7520 6361 6e20 6469  ..    You can di
+00000470: 7370 6c61 7920 7468 6520 6669 6e64 6572  splay the finder
+00000480: 2063 6861 7274 206f 6e20 7468 6520 7363   chart on the sc
+00000490: 7265 656e 206f 7220 7361 7665 2069 7420  reen or save it 
+000004a0: 6173 2061 2066 696c 652e 0a0a 2020 2020  as a file...    
+000004b0: 5468 6973 2063 6c61 7373 2075 7365 7320  This class uses 
+000004c0: 4d61 7470 6c6f 746c 6962 2066 6f72 2067  Matplotlib for g
+000004d0: 656e 6572 6174 696e 6720 7468 6520 6669  enerating the fi
+000004e0: 6e64 6572 2063 6861 7274 2e0a 0a20 2020  nder chart...   
+000004f0: 202e 2e20 7761 726e 696e 673a 3a20 4265   .. warning:: Be
+00000500: 2063 6172 6566 756c 2077 6865 6e20 776f   careful when wo
+00000510: 726b 696e 6720 7769 7468 2073 6576 6572  rking with sever
+00000520: 616c 2066 696e 6465 7220 6368 6172 7473  al finder charts
+00000530: 2061 7320 616c 6c20 7468 6520 6669 6e64   as all the find
+00000540: 6572 0a20 2020 2020 2020 6368 6172 7473  er.       charts
+00000550: 2075 7365 2074 6865 2073 616d 6520 4d61   use the same Ma
+00000560: 7470 6c6f 746c 6962 2066 6967 7572 652e  tplotlib figure.
+00000570: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00000580: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00000590: 2020 2020 6e61 6d65 3a20 6073 7472 602c      name: `str`,
+000005a0: 2060 7061 7468 2d6c 696b 6560 206f 7220   `path-like` or 
+000005b0: 6062 696e 6172 7920 6669 6c65 2d6c 696b  `binary file-lik
+000005c0: 6560 0a20 2020 2020 2020 2046 4954 5320  e`.        FITS 
+000005d0: 6669 6c65 2074 6f20 6469 7370 6c61 792e  file to display.
+000005e0: 0a20 2020 20da 046e 616d 65fa 2655 6e69  .    ..name.&Uni
+000005f0: 6f6e 5b73 7472 2c20 4269 6e61 7279 494f  on[str, BinaryIO
+00000600: 2c20 6f73 2e50 6174 684c 696b 655b 416e  , os.PathLike[An
+00000610: 795d 5d63 0200 0000 0000 0000 0000 0000  y]]c............
+00000620: 0200 0000 0800 0000 4300 0001 736e 0000  ........C...sn..
+00000630: 0074 00a0 017c 01a1 0164 0119 007c 005f  .t...|...d...|._
+00000640: 027c 006a 026a 037c 005f 0474 0583 007c  .|.j.j.|._.t...|
+00000650: 005f 0674 07a0 08a1 008f 1501 0074 076a  ._.t.........t.j
+00000660: 0964 0274 0a64 038d 0201 0074 0b7c 006a  .d.t.d.....t.|.j
+00000670: 0283 017c 005f 0c57 0064 0004 0004 0083  ...|._.W.d......
+00000680: 0301 006e 0831 0073 2d77 0101 0001 0001  ...n.1.s-w......
+00000690: 0059 0001 0067 007c 005f 0d64 0053 0029  .Y...g.|._.d.S.)
+000006a0: 044e 7201 0000 00da 0669 676e 6f72 6529  .Nr......ignore)
+000006b0: 01da 0863 6174 6567 6f72 7929 0e72 1100  ...category).r..
+000006c0: 0000 da04 6f70 656e da04 5f68 6475 da04  ....open.._hdu..
+000006d0: 6461 7461 da05 5f64 6174 61da 0464 6963  data.._data..dic
+000006e0: 74da 095f 6d65 7461 6461 7461 da08 7761  t.._metadata..wa
+000006f0: 726e 696e 6773 da0e 6361 7463 685f 7761  rnings..catch_wa
+00000700: 726e 696e 6773 da0c 7369 6d70 6c65 6669  rnings..simplefi
+00000710: 6c74 6572 7216 0000 0072 1500 0000 da04  lterr....r......
+00000720: 5f77 6373 da0c 5f61 6e6e 6f74 6174 696f  _wcs.._annotatio
+00000730: 6e73 2902 da04 7365 6c66 721c 0000 00a9  ns)...selfr.....
+00000740: 0072 2c00 0000 fa3f 2f55 7365 7273 2f63  .r,....?/Users/c
+00000750: 6872 6973 7469 616e 2f49 6465 6150 726f  hristian/IdeaPro
+00000760: 6a65 6374 732f 696d 6570 6875 2f73 7263  jects/imephu/src
+00000770: 2f69 6d65 7068 752f 6669 6e64 6572 5f63  /imephu/finder_c
+00000780: 6861 7274 2e70 79da 085f 5f69 6e69 745f  hart.py..__init_
+00000790: 5f39 0000 0073 1000 0000 1001 0a03 0801  _9...s..........
+000007a0: 0a01 0e01 0e01 1cfe 0a03 7a14 4669 6e64  ..........z.Find
+000007b0: 6572 4368 6172 742e 5f5f 696e 6974 5f5f  erChart.__init__
+000007c0: da06 7375 7276 6579 da03 7374 72da 0b66  ..survey..str..f
+000007d0: 6974 735f 6365 6e74 6572 7210 0000 00da  its_centerr.....
+000007e0: 0473 697a 6572 0f00 0000 da06 7265 7475  .sizer......retu
+000007f0: 726e fa0d 2746 696e 6465 7243 6861 7274  rn..'FinderChart
+00000800: 2763 0300 0000 0000 0000 0000 0000 0400  'c..............
+00000810: 0000 0400 0000 4300 0001 7314 0000 0074  ......C...s....t
+00000820: 007c 007c 017c 0283 037d 0374 017c 0383  .|.|.|...}.t.|..
+00000830: 0153 0029 0161 a201 0000 4372 6561 7465  .S.).a....Create
+00000840: 2061 2066 696e 6465 7220 6368 6172 7420   a finder chart 
+00000850: 6672 6f6d 2061 2073 6b79 2073 7572 7665  from a sky surve
+00000860: 7920 4649 5453 2069 6d61 6765 2e0a 0a20  y FITS image... 
+00000870: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00000880: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00000890: 2d2d 2d2d 0a20 2020 2020 2020 2073 7572  ----.        sur
+000008a0: 7665 793a 2060 7374 7260 0a20 2020 2020  vey: `str`.     
+000008b0: 2020 2020 2020 2054 6865 206e 616d 6520         The name 
+000008c0: 6f66 2074 6865 2073 7572 7665 7920 746f  of the survey to
+000008d0: 2071 7565 7279 2066 6f72 2074 6865 2046   query for the F
+000008e0: 4954 5320 6669 6c65 2e0a 2020 2020 2020  ITS file..      
+000008f0: 2020 6669 7473 5f63 656e 7465 723a 2060    fits_center: `
+00000900: 7e61 7374 726f 7079 2e63 6f6f 7264 696e  ~astropy.coordin
+00000910: 6174 6573 2e53 6b79 436f 6f72 6460 0a20  ates.SkyCoord`. 
+00000920: 2020 2020 2020 2020 2020 2054 6865 2063             The c
+00000930: 656e 7465 7220 706f 7369 7469 6f6e 206f  enter position o
+00000940: 6620 7468 6520 6c6f 6164 6564 2046 4954  f the loaded FIT
+00000950: 5320 6669 6c65 2e0a 2020 2020 2020 2020  S file..        
+00000960: 7369 7a65 3a20 607e 6173 7472 6f70 792e  size: `~astropy.
+00000970: 636f 6f72 6469 6e61 7465 732e 416e 676c  coordinates.Angl
+00000980: 6560 0a20 2020 2020 2020 2020 2020 2054  e`.            T
+00000990: 6865 2077 6964 7468 2061 6e64 2068 6569  he width and hei
+000009a0: 6768 7420 6f66 2074 6865 2046 4954 5320  ght of the FITS 
+000009b0: 6669 6c65 2069 6d61 6765 2c20 6173 2061  file image, as a
+000009c0: 6e20 616e 676c 6520 6f6e 2074 6865 2073  n angle on the s
+000009d0: 6b79 2e0a 2020 2020 2020 2020 2902 7219  ky..        ).r.
+000009e0: 0000 0072 1b00 0000 2904 722f 0000 0072  ...r....).r/...r
+000009f0: 3100 0000 7232 0000 005a 0a66 6974 735f  1...r2...Z.fits_
+00000a00: 696d 6167 6572 2c00 0000 722c 0000 0072  imager,...r,...r
+00000a10: 2d00 0000 da0b 6672 6f6d 5f73 7572 7665  -.....from_surve
+00000a20: 7944 0000 0073 0400 0000 0c0d 0801 7a17  yD...s........z.
+00000a30: 4669 6e64 6572 4368 6172 742e 6672 6f6d  FinderChart.from
+00000a40: 5f73 7572 7665 79da 0573 7461 7274 7203  _survey..startr.
+00000a50: 0000 00da 0365 6e64 da0b 6570 6865 6d65  .....end..epheme
+00000a60: 7269 6465 73fa 0f4c 6973 745b 4570 6865  rides..List[Ephe
+00000a70: 6d65 7269 735d da10 6d61 785f 7472 6163  meris]..max_trac
+00000a80: 6b5f 6c65 6e67 7468 da13 6372 6561 7465  k_length..create
+00000a90: 5f66 696e 6465 725f 6368 6172 74fa 2a43  _finder_chart.*C
+00000aa0: 616c 6c61 626c 655b 5b4c 6973 745b 4570  allable[[List[Ep
+00000ab0: 6865 6d65 7269 735d 5d2c 2027 4669 6e64  hemeris]], 'Find
+00000ac0: 6572 4368 6172 7427 5dfa 4647 656e 6572  erChart'].FGener
+00000ad0: 6174 6f72 5b54 7570 6c65 5b27 4669 6e64  ator[Tuple['Find
+00000ae0: 6572 4368 6172 7427 2c20 5475 706c 655b  erChart', Tuple[
+00000af0: 6461 7465 7469 6d65 2c20 6461 7465 7469  datetime, dateti
+00000b00: 6d65 5d5d 2c20 4e6f 6e65 2c20 4e6f 6e65  me]], None, None
+00000b10: 5d63 0500 0000 0000 0000 0000 0000 1000  ]c..............
+00000b20: 0000 0500 0000 6300 0001 73be 0100 0081  ......c...s.....
+00000b30: 007c 006a 0064 0175 0073 0e7c 006a 00a0  .|.j.d.u.s.|.j..
+00000b40: 0164 01a1 0164 0175 0072 1274 0264 0283  .d...d.u.r.t.d..
+00000b50: 0182 017c 016a 0064 0175 0073 1f7c 016a  ...|.j.d.u.s.|.j
+00000b60: 00a0 0164 01a1 0164 0175 0072 2374 0264  ...d...d.u.r#t.d
+00000b70: 0383 0182 017c 007c 016b 0572 2b74 0264  .....|.|.k.r+t.d
+00000b80: 0483 0182 017c 007c 0264 0519 006a 036b  .....|.|.d...j.k
+00000b90: 0072 3674 0264 0683 0182 017c 017c 0264  .r6t.d.....|.|.d
+00000ba0: 0719 006a 036b 0472 4174 0264 0883 0182  ...j.k.rAt.d....
+00000bb0: 017c 03a0 0474 056a 06a1 0164 056b 0172  .|...t.j...d.k.r
+00000bc0: 4d74 0264 0983 0182 0164 0a64 0b84 007c  Mt.d.....d.d...|
+00000bd0: 0244 0083 017d 0574 07a0 087c 057c 00a1  .D...}.t...|.|..
+00000be0: 0264 0c18 007d 0674 07a0 077c 057c 01a1  .d...}.t...|.|..
+00000bf0: 027d 077c 0764 056b 0472 727c 057c 0764  .}.|.d.k.rr|.|.d
+00000c00: 0c18 0019 007c 016b 0272 727c 0764 0c38  .....|.k.rr|.d.8
+00000c10: 007d 077c 067c 076b 0272 7a74 0264 0d83  .}.|.|.k.rzt.d..
+00000c20: 0182 017c 027c 0619 0067 017d 087c 0867  ...|.|...g.}.|.g
+00000c30: 017d 0974 097c 0664 0c17 007c 0764 0c17  .}.t.|.d...|.d..
+00000c40: 0083 0244 005d 337d 0a7c 027c 0a19 007d  ...D.]3}.|.|...}
+00000c50: 0b7c 0864 0719 006a 0aa0 0b7c 0b6a 0aa1  .|.d...j...|.j..
+00000c60: 017c 036b 0472 a074 0264 0e83 0182 017c  .|.k.r.t.d.....|
+00000c70: 0864 0519 006a 0aa0 0b7c 0b6a 0aa1 017d  .d...j...|.j...}
+00000c80: 0c7c 0c7c 036b 0172 b37c 08a0 0c7c 0ba1  .|.|.k.r.|...|..
+00000c90: 0101 0071 8b7c 0864 0719 007c 0b67 027d  ...q.|.d...|.g.}
+00000ca0: 087c 09a0 0c7c 08a1 0101 0071 8b7c 0944  .|...|.....q.|.D
+00000cb0: 005d 1b7d 0d7c 0d64 0519 006a 037c 0d64  .].}.|.d...j.|.d
+00000cc0: 0719 006a 0366 027d 0e7c 047c 0d83 017d  ...j.f.}.|.|...}
+00000cd0: 0f7c 0fa0 0d64 0f7c 0ea1 0201 007c 0f7c  .|...d.|.....|.|
+00000ce0: 0e66 0256 0001 0071 c164 0153 0029 1061  .f.V...q.d.S.).a
+00000cf0: 8008 0000 4372 6561 7465 2066 696e 6465  ....Create finde
+00000d00: 7220 6368 6172 7473 2066 6f72 2061 2074  r charts for a t
+00000d10: 696d 6520 696e 7465 7276 616c 2e0a 0a20  ime interval... 
+00000d20: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
+00000d30: 6f64 2069 7320 696e 7465 6e64 6564 2066  od is intended f
+00000d40: 6f72 206e 6f6e 2d73 6964 6572 6561 6c20  or non-sidereal 
+00000d50: 7461 7267 6574 732c 2077 6869 6368 206d  targets, which m
+00000d60: 6179 2072 6571 7569 7265 206d 756c 7469  ay require multi
+00000d70: 706c 650a 2020 2020 2020 2020 6669 6e64  ple.        find
+00000d80: 6572 2063 6861 7274 7320 746f 2063 6f76  er charts to cov
+00000d90: 6572 2074 6865 6972 2074 7261 636b 206f  er their track o
+00000da0: 7665 7220 6120 7469 6d65 2069 6e74 6572  ver a time inter
+00000db0: 7661 6c2e 2049 7420 6372 6561 7465 7320  val. It creates 
+00000dc0: 6669 6e64 6572 0a20 2020 2020 2020 2063  finder.        c
+00000dd0: 6861 7274 7320 6163 636f 7264 696e 6720  harts according 
+00000de0: 746f 2074 6865 2066 6f6c 6c6f 7769 6e67  to the following
+00000df0: 2072 756c 6573 3a0a 0a20 2020 2020 2020   rules:..       
+00000e00: 202a 2054 616b 656e 2074 6f67 6574 6865   * Taken togethe
+00000e10: 722c 2074 6865 2066 696e 6465 7220 6368  r, the finder ch
+00000e20: 6172 7473 2063 6f76 6572 2074 6865 2077  arts cover the w
+00000e30: 686f 6c65 2074 696d 6520 696e 7465 7276  hole time interv
+00000e40: 616c 2e0a 2020 2020 2020 2020 2a20 5468  al..        * Th
+00000e50: 6520 7472 6163 6b20 6c65 6e67 7468 206f  e track length o
+00000e60: 6e20 6561 6368 2066 696e 6465 7220 6368  n each finder ch
+00000e70: 6172 7420 646f 6573 206e 6f74 2065 7863  art does not exc
+00000e80: 6565 6420 606d 6178 5f74 7261 636b 5f6c  eed `max_track_l
+00000e90: 656e 6774 6860 2e0a 2020 2020 2020 2020  ength`..        
+00000ea0: 2a20 4561 6368 2066 696e 6465 7220 6368  * Each finder ch
+00000eb0: 6172 7420 6973 2063 7265 6174 6564 2075  art is created u
+00000ec0: 7369 6e67 2060 6063 7265 6174 655f 6669  sing ``create_fi
+00000ed0: 6e64 6572 5f63 6861 7274 6060 2e0a 0a20  nder_chart``... 
+00000ee0: 2020 2020 2020 2054 6865 206d 6574 686f         The metho
+00000ef0: 6420 6973 2063 6f6d 706c 6574 656c 7920  d is completely 
+00000f00: 6167 6e6f 7374 6963 2061 7320 746f 2077  agnostic as to w
+00000f10: 6861 7420 6120 6669 6e64 6572 2063 6861  hat a finder cha
+00000f20: 7274 2073 686f 756c 6420 6c6f 6f6b 206c  rt should look l
+00000f30: 696b 653b 0a20 2020 2020 2020 2074 6869  ike;.        thi
+00000f40: 7320 6465 6369 7369 6f6e 2069 7320 6c65  s decision is le
+00000f50: 6674 2063 6f6d 706c 6574 656c 7920 746f  ft completely to
+00000f60: 2060 6063 7265 6174 655f 6669 6e64 6572   ``create_finder
+00000f70: 5f63 6861 7274 6060 2e20 496e 2070 6172  _chart``. In par
+00000f80: 7469 6375 6c61 722c 2069 660a 2020 2020  ticular, if.    
+00000f90: 2020 2020 796f 7520 6e65 6564 2061 6e79      you need any
+00000fa0: 2061 6e6e 6f74 6174 696f 6e73 2066 6f72   annotations for
+00000fb0: 2074 6865 206e 6f6e 2d73 6964 6572 6561   the non-siderea
+00000fc0: 6c20 6e61 7475 7265 2c20 6974 2069 7320  l nature, it is 
+00000fd0: 7570 2074 6f0a 2020 2020 2020 2020 6060  up to.        ``
+00000fe0: 6372 6561 7465 5f66 696e 6465 725f 6368  create_finder_ch
+00000ff0: 6172 7460 6020 746f 2070 726f 7669 6465  art`` to provide
+00001000: 2074 6865 6d2e 0a0a 2020 2020 2020 2020   them...        
+00001010: 5468 6520 6060 6372 6561 7465 5f66 696e  The ``create_fin
+00001020: 6465 725f 6368 6172 7460 6020 6675 6e63  der_chart`` func
+00001030: 7469 6f6e 2068 6173 2074 6f20 6163 6365  tion has to acce
+00001040: 7074 2061 7320 6974 7320 7369 6e67 6c65  pt as its single
+00001050: 2061 7267 756d 656e 7420 7468 650a 2020   argument the.  
+00001060: 2020 2020 2020 6c69 7374 206f 6620 6570        list of ep
+00001070: 6865 6d65 7269 6465 7320 746f 2069 6e63  hemerides to inc
+00001080: 6c75 6465 206f 6e20 7468 6520 6669 6e64  lude on the find
+00001090: 6572 2063 6861 7274 2e0a 0a20 2020 2020  er chart...     
+000010a0: 2020 2054 6865 2066 696e 6465 7220 6368     The finder ch
+000010b0: 6172 7473 2061 7265 2072 6574 7572 6e65  arts are returne
+000010c0: 6420 616c 6f6e 6720 7769 7468 2074 6865  d along with the
+000010d0: 2074 696d 6520 696e 7465 7276 616c 2074   time interval t
+000010e0: 6865 7920 636f 7665 722e 2054 6865 2074  hey cover. The t
+000010f0: 696d 650a 2020 2020 2020 2020 696e 7465  ime.        inte
+00001100: 7276 616c 2069 7320 616c 736f 2061 6464  rval is also add
+00001110: 6564 2061 7320 6120 7475 706c 6520 6f66  ed as a tuple of
+00001120: 2060 7e64 6174 6574 696d 652e 6461 7465   `~datetime.date
+00001130: 7469 6d65 6020 7661 6c75 6573 2077 6974  time` values wit
+00001140: 6820 7468 6520 6b65 790a 2020 2020 2020  h the key.      
+00001150: 2020 6060 7661 6c69 645f 666f 7260 6020    ``valid_for`` 
+00001160: 746f 2074 6865 2066 696e 6465 7220 6368  to the finder ch
+00001170: 6172 7427 7320 6d65 7461 6461 7461 2e0a  art's metadata..
+00001180: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00001190: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+000011a0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2073  ------.        s
+000011b0: 7461 7274 3a20 607e 6461 7465 7469 6d65  tart: `~datetime
+000011c0: 2e64 6174 6574 696d 6560 0a20 2020 2020  .datetime`.     
+000011d0: 2020 2020 2020 2054 6865 2073 7461 7274         The start
+000011e0: 2074 696d 6520 6f66 2074 6865 2069 6e74   time of the int
+000011f0: 6572 7661 6c20 746f 2062 6520 636f 7665  erval to be cove
+00001200: 7265 6420 6279 2074 6865 2066 696e 6465  red by the finde
+00001210: 7220 6368 6172 7473 2e20 5468 6973 206d  r charts. This m
+00001220: 7573 740a 2020 2020 2020 2020 2020 2020  ust.            
+00001230: 6265 2061 2074 696d 657a 6f6e 652d 6177  be a timezone-aw
+00001240: 6172 6520 6461 7465 7469 6d65 2e0a 2020  are datetime..  
+00001250: 2020 2020 2020 656e 643a 2060 7e64 6174        end: `~dat
+00001260: 6574 696d 652e 6461 7465 7469 6d65 600a  etime.datetime`.
+00001270: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00001280: 656e 6420 7469 6d65 206f 6620 7468 6520  end time of the 
+00001290: 696e 7465 7276 616c 2074 6f20 6265 2063  interval to be c
+000012a0: 6f76 6572 6564 2062 7920 7468 6520 6669  overed by the fi
+000012b0: 6e64 6572 2063 6861 7274 732e 2054 6869  nder charts. Thi
+000012c0: 7320 6d75 7374 0a20 2020 2020 2020 2020  s must.         
+000012d0: 2020 2062 6520 6120 7469 6d65 7a6f 6e65     be a timezone
+000012e0: 2d61 7761 7265 2064 6174 6574 696d 652e  -aware datetime.
+000012f0: 0a20 2020 2020 2020 2065 7068 656d 6572  .        ephemer
+00001300: 6964 6573 3a20 6c69 7374 206f 6620 607e  ides: list of `~
+00001310: 696d 6570 6875 2e75 7469 6c73 2e45 7068  imephu.utils.Eph
+00001320: 656d 6572 6973 600a 2020 2020 2020 2020  emeris`.        
+00001330: 2020 2020 5468 6520 6c69 7374 206f 6620      The list of 
+00001340: 6570 6865 6d65 7269 6465 732e 2054 6865  ephemerides. The
+00001350: 2074 696d 6520 696e 7465 7276 616c 2066   time interval f
+00001360: 726f 6d20 6060 7374 6172 7460 6020 746f  rom ``start`` to
+00001370: 2060 6065 6e64 6060 206d 7573 7420 6265   ``end`` must be
+00001380: 0a20 2020 2020 2020 2020 2020 2066 756c  .            ful
+00001390: 6c79 2063 6f76 6572 6564 2062 7920 7468  ly covered by th
+000013a0: 6520 6570 6865 6d65 7269 6465 732e 0a20  e ephemerides.. 
+000013b0: 2020 2020 2020 206d 6178 5f74 7261 636b         max_track
+000013c0: 5f6c 656e 6774 683a 2066 6c6f 6174 0a20  _length: float. 
+000013d0: 2020 2020 2020 2020 2020 2054 6865 206d             The m
+000013e0: 6178 696d 756d 206c 656e 6774 6820 6120  aximum length a 
+000013f0: 7472 6163 6b20 6d61 7920 6861 7665 206f  track may have o
+00001400: 6e20 6120 6669 6e64 6572 2063 6861 7274  n a finder chart
+00001410: 2c20 6173 2061 6e20 616e 676c 6520 6f6e  , as an angle on
+00001420: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00001430: 2073 6b79 2e0a 2020 2020 2020 2020 6372   sky..        cr
+00001440: 6561 7465 5f66 696e 6465 725f 6368 6172  eate_finder_char
+00001450: 743a 2066 756e 6374 696f 6e0a 2020 2020  t: function.    
+00001460: 2020 2020 2020 2020 5468 6520 6675 6e63          The func
+00001470: 7469 6f6e 2066 6f72 2063 7265 6174 696e  tion for creatin
+00001480: 6720 6120 6669 6e64 6572 2063 6861 7274  g a finder chart
+00001490: 2066 726f 6d20 6120 6c69 7374 206f 6620   from a list of 
+000014a0: 6570 6865 6d65 7269 6465 732e 0a0a 2020  ephemerides...  
+000014b0: 2020 2020 2020 5969 656c 6473 0a20 2020        Yields.   
+000014c0: 2020 2020 202d 2d2d 2d2d 2d0a 2020 2020       ------.    
+000014d0: 2020 2020 7475 706c 6520 6f66 2061 2060      tuple of a `
+000014e0: 7e69 6d65 7068 752e 6669 6e64 6572 5f63  ~imephu.finder_c
+000014f0: 6861 7274 2e46 696e 6465 7243 6861 7274  hart.FinderChart
+00001500: 6020 616e 6420 6120 6461 7465 7469 6d65  ` and a datetime
+00001510: 2069 6e74 6572 7661 6c0a 2020 2020 2020   interval.      
+00001520: 2020 2020 2020 5468 6520 6765 6e65 7261        The genera
+00001530: 7465 6420 6669 6e64 6572 2063 6861 7274  ted finder chart
+00001540: 7320 616c 6f6e 6720 7769 7468 2074 6865  s along with the
+00001550: 2074 696d 6520 696e 7465 7276 616c 7320   time intervals 
+00001560: 7468 6579 2063 6f76 6572 2e0a 2020 2020  they cover..    
+00001570: 2020 2020 4e7a 2654 6865 2073 7461 7274      Nz&The start
+00001580: 2074 696d 6520 6d75 7374 2062 6520 7469   time must be ti
+00001590: 6d65 7a6f 6e65 2d61 7761 7265 2e7a 2454  mezone-aware.z$T
+000015a0: 6865 2065 6e64 2074 696d 6520 6d75 7374  he end time must
+000015b0: 2062 6520 7469 6d65 7a6f 6e65 2d61 7761   be timezone-awa
+000015c0: 7265 2e7a 3154 6865 2073 7461 7274 2074  re.z1The start t
+000015d0: 696d 6520 6d75 7374 2062 6520 6561 726c  ime must be earl
+000015e0: 6965 7220 7468 616e 2074 6865 2065 6e64  ier than the end
+000015f0: 2074 696d 652e 7201 0000 007a 3854 6865   time.r....z8The
+00001600: 2073 7461 7274 2074 696d 6520 6d75 7374   start time must
+00001610: 206e 6f74 2062 6520 6561 726c 6965 7220   not be earlier 
+00001620: 7468 616e 2074 6865 2066 6972 7374 2065  than the first e
+00001630: 706f 6368 2ee9 ffff ffff 7a33 5468 6520  poch......z3The 
+00001640: 656e 6420 7469 6d65 206d 7573 7420 6e6f  end time must no
+00001650: 7420 6265 206c 6174 6572 2074 6861 6e20  t be later than 
+00001660: 7468 6520 6c61 7374 2065 706f 6368 2e7a  the last epoch.z
+00001670: 2a54 6865 206d 6178 696d 756d 2074 7261  *The maximum tra
+00001680: 636b 206c 656e 6774 6820 6d75 7374 2062  ck length must b
+00001690: 6520 706f 7369 7469 7665 2e63 0100 0000  e positive.c....
+000016a0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000016b0: 5300 0001 7312 0000 0067 007c 005d 057d  S...s....g.|.].}
+000016c0: 017c 016a 0091 0271 0253 0072 2c00 0000  .|.j...q.S.r,...
+000016d0: 2901 da05 6570 6f63 6829 02da 022e 30da  )...epoch)....0.
+000016e0: 0165 722c 0000 0072 2c00 0000 722d 0000  .er,...r,...r-..
+000016f0: 00da 0a3c 6c69 7374 636f 6d70 3e9a 0000  ...<listcomp>...
+00001700: 0073 0200 0000 1200 7a31 4669 6e64 6572  .s......z1Finder
+00001710: 4368 6172 742e 666f 725f 7469 6d65 5f69  Chart.for_time_i
+00001720: 6e74 6572 7661 6c2e 3c6c 6f63 616c 733e  nterval.<locals>
+00001730: 2e3c 6c69 7374 636f 6d70 3ee9 0100 0000  .<listcomp>.....
+00001740: 7a28 5468 6520 696e 7465 7276 616c 206d  z(The interval m
+00001750: 7573 7420 6861 7665 2061 2070 6f73 6974  ust have a posit
+00001760: 6976 6520 6c65 6e67 7468 7a37 5468 6520  ive lengthz7The 
+00001770: 6d61 7869 6d75 6d20 7472 6163 6b20 6c65  maximum track le
+00001780: 6e67 7468 206f 6e20 6120 6669 6e64 6572  ngth on a finder
+00001790: 2063 6861 7274 2069 7320 6578 6365 6564   chart is exceed
+000017a0: 6564 2eda 0976 616c 6964 5f66 6f72 290e  ed...valid_for).
+000017b0: da06 747a 696e 666f da09 7574 636f 6666  ..tzinfo..utcoff
+000017c0: 7365 74da 0a56 616c 7565 4572 726f 7272  set..ValueErrorr
+000017d0: 3f00 0000 da08 746f 5f76 616c 7565 da01  ?.....to_value..
+000017e0: 75da 0661 7263 6d69 6eda 0662 6973 6563  u..arcmin..bisec
+000017f0: 74da 0c62 6973 6563 745f 7269 6768 74da  t..bisect_right.
+00001800: 0572 616e 6765 da08 706f 7369 7469 6f6e  .range..position
+00001810: da0a 7365 7061 7261 7469 6f6e da06 6170  ..separation..ap
+00001820: 7065 6e64 da0c 6164 645f 6d65 7461 6461  pend..add_metada
+00001830: 7461 2910 7236 0000 0072 3700 0000 7238  ta).r6...r7...r8
+00001840: 0000 0072 3a00 0000 723b 0000 005a 0961  ...r:...r;...Z.a
+00001850: 6c6c 5f74 696d 6573 5a0b 7374 6172 745f  ll_timesZ.start_
+00001860: 696e 6465 78da 0965 6e64 5f69 6e64 6578  index..end_index
+00001870: 5a0d 6375 7272 656e 745f 6772 6f75 70da  Z.current_group.
+00001880: 0667 726f 7570 73da 0169 5a0e 6e65 7874  .groups..iZ.next
+00001890: 5f65 7068 656d 6572 6973 5a0c 7472 6163  _ephemerisZ.trac
+000018a0: 6b5f 6c65 6e67 7468 da05 6772 6f75 7072  k_length..groupr
+000018b0: 4400 0000 da0c 6669 6e64 6572 5f63 6861  D.....finder_cha
+000018c0: 7274 722c 0000 0072 2c00 0000 722d 0000  rtr,...r,...r-..
+000018d0: 00da 1166 6f72 5f74 696d 655f 696e 7465  ...for_time_inte
+000018e0: 7276 616c 5400 0000 7352 0000 0002 801a  rvalT...sR......
+000018f0: 3508 011a 0108 0108 0208 010e 0208 010e  5...............
+00001900: 0108 0110 0208 010e 0310 010c 0118 0108  ................
+00001910: 0108 0308 010a 0506 0116 0108 0110 0302  ................
+00001920: 0104 ff02 0302 0104 ff12 0308 010c 010c  ................
+00001930: 020c 0108 0314 0108 010c 010c 0104 fc7a  ...............z
+00001940: 1d46 696e 6465 7243 6861 7274 2e66 6f72  .FinderChart.for
+00001950: 5f74 696d 655f 696e 7465 7276 616c 7215  _time_intervalr.
+00001960: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001970: 0100 0000 0200 0000 4300 0001 f30a 0000  ........C.......
+00001980: 007c 006a 00a0 01a1 0053 0029 017a a952  .|.j.....S.).z.R
+00001990: 6574 7572 6e20 6120 6465 6570 2063 6f70  eturn a deep cop
+000019a0: 7920 6f66 2074 6865 2057 4353 206f 626a  y of the WCS obj
+000019b0: 6563 7420 6f66 2074 6865 2066 696e 6465  ect of the finde
+000019c0: 7220 6368 6172 742e 0a0a 2020 2020 2020  r chart...      
+000019d0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+000019e0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000019f0: 2020 607e 6173 7472 6f70 792e 7763 732e    `~astropy.wcs.
+00001a00: 5743 5360 0a20 2020 2020 2020 2020 2020  WCS`.           
+00001a10: 2041 2064 6565 7020 636f 7079 206f 6620   A deep copy of 
+00001a20: 7468 6520 5743 5320 6f62 6a65 6374 2e0a  the WCS object..
+00001a30: 2020 2020 2020 2020 2902 7229 0000 00da          ).r)....
+00001a40: 0864 6565 7063 6f70 79a9 0172 2b00 0000  .deepcopy..r+...
+00001a50: 722c 0000 0072 2c00 0000 722d 0000 00da  r,...r,...r-....
+00001a60: 0377 6373 c100 0000 7302 0000 000a 097a  .wcs....s......z
+00001a70: 0f46 696e 6465 7243 6861 7274 2e77 6373  .FinderChart.wcs
+00001a80: da0a 616e 6e6f 7461 7469 6f6e 7218 0000  ..annotationr...
+00001a90: 00da 044e 6f6e 6563 0200 0000 0000 0000  ...Nonec........
+00001aa0: 0000 0000 0200 0000 0300 0000 4300 0001  ............C...
+00001ab0: 7310 0000 007c 006a 00a0 017c 01a1 0101  s....|.j...|....
+00001ac0: 0064 0153 0029 027a fc41 6464 2061 6e20  .d.S.).z.Add an 
+00001ad0: 616e 6e6f 7461 7469 6f6e 2074 6f20 7468  annotation to th
+00001ae0: 6520 6669 6e64 6572 2063 6861 7274 2e0a  e finder chart..
+00001af0: 0a20 2020 2020 2020 2041 6e6e 6f74 6174  .        Annotat
+00001b00: 696f 6e73 2077 696c 6c20 6265 2070 6c6f  ions will be plo
+00001b10: 7474 6564 206f 6e74 6f20 7468 6520 6669  tted onto the fi
+00001b20: 6e64 6572 2063 6861 7274 2069 6e20 7468  nder chart in th
+00001b30: 6520 6f72 6465 7220 7468 6579 2068 6176  e order they hav
+00001b40: 6520 6265 656e 0a20 2020 2020 2020 2061  e been.        a
+00001b50: 6464 6564 2e20 536f 2c20 666f 7220 6578  dded. So, for ex
+00001b60: 616d 706c 652c 2074 6865 2061 6e6e 6f74  ample, the annot
+00001b70: 6174 696f 6e20 6164 6465 6420 6c61 7374  ation added last
+00001b80: 2077 696c 6c20 6265 206f 7574 7075 7420   will be output 
+00001b90: 6f6e 2074 6f70 206f 6620 616c 6c0a 2020  on top of all.  
+00001ba0: 2020 2020 2020 7468 6520 6f74 6865 7220        the other 
+00001bb0: 616e 6e6f 7461 7469 6f6e 732e 0a20 2020  annotations..   
+00001bc0: 2020 2020 204e 2902 722a 0000 0072 5000       N).r*...rP.
+00001bd0: 0000 2902 722b 0000 0072 5c00 0000 722c  ..).r+...r\...r,
+00001be0: 0000 0072 2c00 0000 722d 0000 00da 0e61  ...r,...r-.....a
+00001bf0: 6464 5f61 6e6e 6f74 6174 696f 6ecc 0000  dd_annotation...
+00001c00: 0073 0200 0000 1007 7a1a 4669 6e64 6572  .s......z.Finder
+00001c10: 4368 6172 742e 6164 645f 616e 6e6f 7461  Chart.add_annota
+00001c20: 7469 6f6e fa0e 4469 6374 5b73 7472 2c20  tion..Dict[str, 
+00001c30: 416e 795d 6301 0000 0000 0000 0000 0000  Any]c...........
+00001c40: 0001 0000 0002 0000 0043 0000 0172 5800  .........C...rX.
+00001c50: 0000 2901 610b 0100 000a 2020 2020 2020  ..).a.....      
+00001c60: 2020 5265 7475 726e 2074 6865 206d 6574    Return the met
+00001c70: 6164 6174 6120 666f 7220 7468 6520 6669  adata for the fi
+00001c80: 6e64 6572 2063 6861 7274 2e0a 0a20 2020  nder chart...   
+00001c90: 2020 2020 204d 6574 6164 6174 6120 6361       Metadata ca
+00001ca0: 6e20 2062 6520 6164 6465 6420 7769 7468  n  be added with
+00001cb0: 2074 6865 2060 6164 645f 6d65 7461 6461   the `add_metada
+00001cc0: 7461 6020 6d65 7468 6f64 2e20 4120 7368  ta` method. A sh
+00001cd0: 616c 6c6f 7720 636f 7079 206f 6620 7468  allow copy of th
+00001ce0: 650a 2020 2020 2020 2020 6d65 7461 6461  e.        metada
+00001cf0: 7461 2069 7320 7265 7475 726e 6564 2e0a  ta is returned..
+00001d00: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001d10: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00001d20: 0a20 2020 2020 2020 2064 6963 740a 2020  .        dict.  
+00001d30: 2020 2020 2020 2020 2020 5468 6520 6d65            The me
+00001d40: 7461 6461 7461 206f 6620 7468 6520 6669  tadata of the fi
+00001d50: 6e64 6572 2063 6861 7274 2e0a 2020 2020  nder chart..    
+00001d60: 2020 2020 2902 7225 0000 00da 0463 6f70      ).r%.....cop
+00001d70: 7972 5a00 0000 722c 0000 0072 2c00 0000  yrZ...r,...r,...
+00001d80: 722d 0000 00da 086d 6574 6164 6174 61d5  r-.....metadata.
+00001d90: 0000 0073 0200 0000 0a0d 7a14 4669 6e64  ...s......z.Find
+00001da0: 6572 4368 6172 742e 6d65 7461 6461 7461  erChart.metadata
+00001db0: da03 6b65 79da 0576 616c 7565 7205 0000  ..key..valuer...
+00001dc0: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
+00001dd0: 0000 0300 0000 4300 0001 730e 0000 007c  ......C...s....|
+00001de0: 027c 006a 007c 013c 0064 0153 0029 0261  .|.j.|.<.d.S.).a
+00001df0: 2501 0000 0a20 2020 2020 2020 2041 6464  %....        Add
+00001e00: 2061 206b 6579 2d76 616c 7565 2074 6f20   a key-value to 
+00001e10: 7468 6520 6669 6e64 6572 2063 6861 7274  the finder chart
+00001e20: 2773 206d 6574 6164 6174 612e 0a0a 2020  's metadata...  
+00001e30: 2020 2020 2020 4966 2074 6865 206b 6579        If the key
+00001e40: 2065 7869 7374 7273 2069 6e20 7468 6520   existrs in the 
+00001e50: 6d65 7461 6461 7461 2061 6c72 6561 6479  metadata already
+00001e60: 2c20 7468 6520 6578 6973 7469 6e67 2076  , the existing v
+00001e70: 616c 7565 2066 6f72 2074 6865 206b 6579  alue for the key
+00001e80: 2069 730a 2020 2020 2020 2020 7265 706c   is.        repl
+00001e90: 6163 6564 2e0a 0a20 2020 2020 2020 2050  aced...        P
+00001ea0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00001eb0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00001ec0: 2020 2020 206b 6579 3a20 6073 7472 600a       key: `str`.
+00001ed0: 2020 2020 2020 2020 2020 2020 4b65 792e              Key.
+00001ee0: 0a20 2020 2020 2020 2076 616c 7565 3a20  .        value: 
+00001ef0: 607e 7479 7069 6e67 2e41 6e79 600a 2020  `~typing.Any`.  
+00001f00: 2020 2020 2020 2020 2020 5661 6c75 652e            Value.
+00001f10: 0a20 2020 2020 2020 204e 2901 7225 0000  .        N).r%..
+00001f20: 0029 0372 2b00 0000 7262 0000 0072 6300  .).r+...rb...rc.
+00001f30: 0000 722c 0000 0072 2c00 0000 722d 0000  ..r,...r,...r-..
+00001f40: 0072 5100 0000 e400 0000 7302 0000 000e  .rQ.......s.....
+00001f50: 0e7a 1846 696e 6465 7243 6861 7274 2e61  .z.FinderChart.a
+00001f60: 6464 5f6d 6574 6164 6174 6163 0100 0000  dd_metadatac....
+00001f70: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001f80: 4300 0001 731e 0000 007c 00a0 00a1 007d  C...s....|.....}
+00001f90: 0174 01a0 02a1 0001 0074 01a0 037c 01a1  .t.......t...|..
+00001fa0: 0101 0064 0153 0029 027a 2744 6973 706c  ...d.S.).z'Displ
+00001fb0: 6179 2074 6865 2066 696e 6465 7220 6368  ay the finder ch
+00001fc0: 6172 7420 6f6e 2074 6865 2073 6372 6565  art on the scree
+00001fd0: 6e2e 4e29 04da 0c5f 6372 6561 7465 5f70  n.N)..._create_p
+00001fe0: 6c6f 74da 0370 6c74 da04 7368 6f77 da05  lot..plt..show..
+00001ff0: 636c 6f73 6529 0272 2b00 0000 da06 6669  close).r+.....fi
+00002000: 6775 7265 722c 0000 0072 2c00 0000 722d  gurer,...r,...r-
+00002010: 0000 0072 6600 0000 f400 0000 7306 0000  ...rf.......s...
+00002020: 0008 0208 010e 017a 1046 696e 6465 7243  .......z.FinderC
+00002030: 6861 7274 2e73 686f 774e fa3a 556e 696f  hart.showN.:Unio
+00002040: 6e5b 7374 722c 2042 696e 6172 7949 4f2c  n[str, BinaryIO,
+00002050: 206f 732e 5061 7468 4c69 6b65 5b73 7472   os.PathLike[str
+00002060: 5d2c 206f 732e 5061 7468 4c69 6b65 5b62  ], os.PathLike[b
+00002070: 7974 6573 5d5d da06 666f 726d 6174 fa0d  ytes]]..format..
+00002080: 4f70 7469 6f6e 616c 5b73 7472 5d63 0300  Optional[str]c..
+00002090: 0000 0000 0000 0000 0000 0600 0000 0800  ................
+000020a0: 0000 4300 0001 73a0 0000 007c 00a0 00a1  ..C...s....|....
+000020b0: 007d 037c 0272 417c 02a0 01a1 0064 016b  .}.|.rA|.....d.k
+000020c0: 0272 4174 0283 007d 0474 036a 047c 047c  .rAt...}.t.j.|.|
+000020d0: 0264 0264 038d 0301 0074 057c 0164 0483  .d.d.....t.|.d..
+000020e0: 0272 247c 01a0 067c 04a0 07a1 00a1 0101  .r$|...|........
+000020f0: 006e 2574 087c 0164 0583 028f 0f7d 057c  .n%t.|.d.....}.|
+00002100: 05a0 067c 04a0 07a1 00a1 0101 0057 0064  ...|.........W.d
+00002110: 0604 0004 0083 0301 006e 0831 0073 3b77  .........n.1.s;w
+00002120: 0101 0001 0001 0059 0001 006e 0874 036a  .......Y...n.t.j
+00002130: 047c 017c 0264 0264 038d 0301 0074 03a0  .|.|.d.d.....t..
+00002140: 097c 03a1 0101 0064 0653 0029 0761 4702  .|.....d.S.).aG.
+00002150: 0000 5361 7665 2074 6865 2066 696e 6465  ..Save the finde
+00002160: 7220 6368 6172 7420 696e 2061 2066 696c  r chart in a fil
+00002170: 652e 0a0a 2020 2020 2020 2020 4966 2060  e...        If `
+00002180: 666f 726d 6174 6020 6973 206e 6f74 2073  format` is not s
+00002190: 6574 2c20 7468 6520 6669 6c65 2065 7874  et, the file ext
+000021a0: 656e 7369 6f6e 206f 6620 606e 616d 6560  ension of `name`
+000021b0: 2069 7320 7573 6564 2074 6f20 6669 6775   is used to figu
+000021c0: 7265 206f 7574 2074 6865 0a20 2020 2020  re out the.     
+000021d0: 2020 2066 696c 6520 6f72 2c20 6966 2074     file or, if t
+000021e0: 6865 7265 2069 7320 6e6f 2065 7874 656e  here is no exten
+000021f0: 7369 6f6e 2c20 4d61 7470 6c6f 746c 6962  sion, Matplotlib
+00002200: 2773 2064 6566 6175 6c74 2069 7320 7573  's default is us
+00002210: 6564 2e20 5365 650a 2020 2020 2020 2020  ed. See.        
+00002220: 4d61 7470 6c6f 746c 6962 2773 2060 6d61  Matplotlib's `ma
+00002230: 7470 6c6f 746c 6962 2e70 7970 6c6f 742e  tplotlib.pyplot.
+00002240: 7361 7665 6669 6760 2066 756e 6374 696f  savefig` functio
+00002250: 6e20 666f 7220 6d6f 7265 2064 6574 6169  n for more detai
+00002260: 6c73 2072 6567 6172 6469 6e67 0a20 2020  ls regarding.   
+00002270: 2020 2020 2074 6865 2066 6f72 6d61 742e       the format.
+00002280: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00002290: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+000022a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000022b0: 6e61 6d65 3a20 6073 7472 602c 2060 7061  name: `str`, `pa
+000022c0: 7468 2d6c 696b 6560 206f 7220 6062 696e  th-like` or `bin
+000022d0: 6172 7920 6669 6c65 2d6c 696b 6560 0a20  ary file-like`. 
+000022e0: 2020 2020 2020 2020 2020 2054 6865 2066             The f
+000022f0: 696c 6520 746f 2077 6869 6368 2074 6865  ile to which the
+00002300: 2066 696e 6465 7220 6368 6172 7420 6973   finder chart is
+00002310: 2073 6176 6564 2e20 416e 2065 7869 7374   saved. An exist
+00002320: 696e 6720 6669 6c65 2069 7320 7265 706c  ing file is repl
+00002330: 6163 6564 2e0a 2020 2020 2020 2020 666f  aced..        fo
+00002340: 726d 6174 3a20 6073 7472 602c 206f 7074  rmat: `str`, opt
+00002350: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00002360: 2020 5468 6520 666f 726d 6174 2069 6e20    The format in 
+00002370: 7768 6963 6820 746f 2073 746f 7265 2074  which to store t
+00002380: 6865 2066 696e 6465 7220 6368 6172 742e  he finder chart.
+00002390: 0a20 2020 2020 2020 20da 0370 6466 da05  .        ..pdf..
+000023a0: 7469 6768 7429 0272 6a00 0000 5a0b 6262  tight).rj...Z.bb
+000023b0: 6f78 5f69 6e63 6865 73da 0577 7269 7465  ox_inches..write
+000023c0: da02 7762 4e29 0a72 6400 0000 da05 6c6f  ..wbN).rd.....lo
+000023d0: 7765 7272 0400 0000 7265 0000 005a 0773  werr....re...Z.s
+000023e0: 6176 6566 6967 da07 6861 7361 7474 7272  avefig..hasattrr
+000023f0: 6e00 0000 da08 6765 7476 616c 7565 7220  n.....getvaluer 
+00002400: 0000 0072 6700 0000 2906 722b 0000 0072  ...rg...).r+...r
+00002410: 1c00 0000 726a 0000 0072 6800 0000 726c  ....rj...rh...rl
+00002420: 0000 00da 0166 722c 0000 0072 2c00 0000  .....fr,...r,...
+00002430: 722d 0000 00da 0473 6176 65fa 0000 0073  r-.....save....s
+00002440: 1800 0000 0813 1001 0601 1001 0a01 1001  ................
+00002450: 0c02 1001 1cff 0280 1003 0e01 7a10 4669  ............z.Fi
+00002460: 6e64 6572 4368 6172 742e 7361 7665 7217  nderChart.saver.
+00002470: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002480: 0400 0000 0500 0000 4300 0001 7358 0000  ........C...sX..
+00002490: 0074 006a 0164 0164 028d 017d 0174 006a  .t.j.d.d...}.t.j
+000024a0: 027c 006a 0364 038d 017d 027c 00a0 047c  .|.j.d...}.|...|
+000024b0: 02a1 0101 007c 00a0 057c 02a1 0101 007c  .....|...|.....|
+000024c0: 026a 0664 0464 0564 0664 078d 0301 007c  .j.d.d.d.d.....|
+000024d0: 006a 0744 005d 077d 037c 03a0 087c 02a1  .j.D.].}.|...|..
+000024e0: 0101 0071 227c 0153 0029 084e 2902 e90a  ...q"|.S.).N)...
+000024f0: 0000 00e9 0900 0000 2901 da07 6669 6773  ........)...figs
+00002500: 697a 6529 015a 0a70 726f 6a65 6374 696f  ize).Z.projectio
+00002510: 6e54 da04 626c 7565 679a 9999 9999 99c9  nT..blueg.......
+00002520: 3f29 02da 0563 6f6c 6f72 da05 616c 7068  ?)...color..alph
+00002530: 6129 0972 6500 0000 7268 0000 005a 0773  a).re...rh...Z.s
+00002540: 7562 706c 6f74 7229 0000 00da 115f 6164  ubplotr)....._ad
+00002550: 645f 6669 7473 5f63 6f6e 7465 6e74 da0c  d_fits_content..
+00002560: 5f75 7064 6174 655f 6178 6573 da04 6772  _update_axes..gr
+00002570: 6964 722a 0000 005a 0661 6464 5f74 6f29  idr*...Z.add_to)
+00002580: 0472 2b00 0000 7268 0000 00da 0261 7872  .r+...rh.....axr
+00002590: 5c00 0000 722c 0000 0072 2c00 0000 722d  \...r,...r,...r-
+000025a0: 0000 0072 6400 0000 1a01 0000 7310 0000  ...rd.......s...
+000025b0: 000c 010e 010a 020a 0110 020a 020c 0104  ................
+000025c0: 027a 1846 696e 6465 7243 6861 7274 2e5f  .z.FinderChart._
+000025d0: 6372 6561 7465 5f70 6c6f 7472 7e00 0000  create_plotr~...
+000025e0: 7214 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000025f0: 0000 0900 0000 0800 0000 4300 0001 7384  ..........C...s.
+00002600: 0000 0074 006a 01a0 0264 01a1 017d 0264  ...t.j...d...}.d
+00002610: 027d 0364 037d 0474 037c 037c 0464 0464  .}.d.}.t.|.|.d.d
+00002620: 058d 037d 057c 05a0 047c 006a 056a 06a1  ...}.|...|.j.j..
+00002630: 015c 027d 067d 0764 067c 077c 0618 0014  .\.}.}.d.|.|....
+00002640: 007c 0617 007d 0664 077c 077c 0618 0014  .|...}.d.|.|....
+00002650: 007c 0717 007d 0774 077c 006a 0864 087c  .|...}.t.|.j.d.|
+00002660: 067c 0764 098d 047d 087c 016a 097c 006a  .|.d...}.|.j.|.j
+00002670: 056a 067c 0264 0a64 0b7c 0864 0c64 0d8d  .j.|.d.d.|.d.d..
+00002680: 0601 0064 0e53 0029 0f7a 6b0a 2020 2020  ...d.S.).zk.    
+00002690: 2020 2020 2041 6464 2063 6f6e 7465 6e74       Add content
+000026a0: 206f 6620 7468 6520 4649 5453 2066 696c   of the FITS fil
+000026b0: 6520 746f 2074 6865 2070 6c6f 742e 0a0a  e to the plot...
+000026c0: 2020 2020 2020 2020 5468 6520 636f 6465          The code
+000026d0: 2068 6173 2062 6565 6e20 6164 6170 7465   has been adapte
+000026e0: 6420 6672 6f6d 2041 504c 7079 2e0a 2020  d from APLpy..  
+000026f0: 2020 2020 2020 da09 6769 7374 5f79 6172        ..gist_yar
+00002700: 6767 0000 0000 0000 d03f 6700 0000 0000  gg.......?g.....
+00002710: f058 4069 1027 0000 2901 5a09 6e5f 7361  .X@i.'..).Z.n_sa
+00002720: 6d70 6c65 7367 9a99 9999 9999 b9bf 679a  mplesg........g.
+00002730: 9999 9999 99b9 3fe9 0200 0000 2903 da05  ......?.....)...
+00002740: 706f 7765 725a 076d 696e 5f63 7574 5a07  powerZ.min_cutZ.
+00002750: 6d61 785f 6375 74da 076e 6561 7265 7374  max_cut..nearest
+00002760: 7270 0000 00da 0565 7175 616c 2905 da04  rp.....equal)...
+00002770: 636d 6170 da0d 696e 7465 7270 6f6c 6174  cmap..interpolat
+00002780: 696f 6eda 066f 7269 6769 6eda 046e 6f72  ion..origin..nor
+00002790: 6dda 0661 7370 6563 744e 290a 7265 0000  m..aspectN).re..
+000027a0: 00da 0263 6dda 0867 6574 5f63 6d61 7072  ...cm..get_cmapr
+000027b0: 1200 0000 5a0a 6765 745f 6c69 6d69 7473  ....Z.get_limits
+000027c0: 7221 0000 0072 2200 0000 7213 0000 0072  r!...r"...r....r
+000027d0: 2300 0000 5a06 696d 7368 6f77 2909 722b  #...Z.imshow).r+
+000027e0: 0000 0072 7e00 0000 7284 0000 005a 0470  ...r~...r....Z.p
+000027f0: 6d69 6e5a 0470 6d61 78da 0869 6e74 6572  minZ.pmax..inter
+00002800: 7661 6cda 0476 6d69 6eda 0476 6d61 785a  val..vmin..vmaxZ
+00002810: 0a6e 6f72 6d61 6c69 7a65 7272 2c00 0000  .normalizerr,...
+00002820: 722c 0000 0072 2d00 0000 727b 0000 0028  r,...r-...r{...(
+00002830: 0100 0073 2000 0000 0c06 0403 0401 0e01  ...s ...........
+00002840: 1201 1001 1001 1202 0402 0601 0201 0201  ................
+00002850: 0201 0201 0201 0afa 7a1d 4669 6e64 6572  ........z.Finder
+00002860: 4368 6172 742e 5f61 6464 5f66 6974 735f  Chart._add_fits_
+00002870: 636f 6e74 656e 7463 0200 0000 0000 0000  contentc........
+00002880: 0000 0000 0800 0000 0400 0000 4300 0001  ............C...
+00002890: 73a2 0000 0064 0164 0264 039c 027d 027c  s....d.d.d...}.|
+000028a0: 006a 006a 017d 037c 0364 0419 007d 047c  .j.j.}.|.d...}.|
+000028b0: 0364 0519 007d 057c 0464 066b 0372 1974  .d...}.|.d.k.r.t
+000028c0: 0264 0783 0182 017c 0564 086b 0372 2174  .d.....|.d.k.r!t
+000028d0: 0264 0983 0182 017c 016a 0364 0419 007d  .d.....|.j.d...}
+000028e0: 067c 016a 0364 0519 007d 077c 06a0 047c  .|.j.d...}.|...|
+000028f0: 027c 0419 00a1 0101 007c 07a0 047c 027c  .|.......|...|.|
+00002900: 0519 00a1 0101 007c 06a0 0564 0aa1 0101  .......|...d....
+00002910: 007c 07a0 0564 0aa1 0101 007c 066a 0664  .|...d.....|.j.d
+00002920: 0b64 0c8d 0101 007c 076a 0664 0b64 0c8d  .d.....|.j.d.d..
+00002930: 0101 0064 0053 0029 0d4e 7a0a 4465 6320  ...d.S.).Nz.Dec 
+00002940: 2849 4352 5329 7a09 5241 2028 4943 5253  (ICRS)z.RA (ICRS
+00002950: 2929 02fa 0a70 6f73 2e65 712e 6465 63fa  ))...pos.eq.dec.
+00002960: 0970 6f73 2e65 712e 7261 7201 0000 0072  .pos.eq.rar....r
+00002970: 4300 0000 728f 0000 007a 494f 6e6c 7920  C...r....zIOnly 
+00002980: 706f 732e 6571 2e72 6120 6973 2073 7570  pos.eq.ra is sup
+00002990: 706f 7274 6564 2066 6f72 2074 6865 2070  ported for the p
+000029a0: 6879 7369 6361 6c20 7479 7065 206f 6620  hysical type of 
+000029b0: 7468 6520 6669 7273 7420 776f 726c 6420  the first world 
+000029c0: 6178 6973 728e 0000 007a 4b4f 6e6c 7920  axisr....zKOnly 
+000029d0: 706f 732e 6571 2e64 6563 2069 7320 7375  pos.eq.dec is su
+000029e0: 7070 6f72 7465 6420 666f 7220 7468 6520  pported for the 
+000029f0: 7068 7973 6963 616c 2074 7970 6520 6f66  physical type of
+00002a00: 2074 6865 2073 6563 6f6e 6420 776f 726c   the second worl
+00002a10: 6420 6178 6973 54e9 0700 0000 2901 7232  d axisT.....).r2
+00002a20: 0000 0029 0772 2900 0000 5a19 776f 726c  ...).r)...Z.worl
+00002a30: 645f 6178 6973 5f70 6879 7369 6361 6c5f  d_axis_physical_
+00002a40: 7479 7065 7372 4700 0000 da06 636f 6f72  typesrG.....coor
+00002a50: 6473 5a0d 7365 745f 6178 6973 6c61 6265  dsZ.set_axislabe
+00002a60: 6c5a 1364 6973 706c 6179 5f6d 696e 6f72  lZ.display_minor
+00002a70: 5f74 6963 6b73 5a09 7365 745f 7469 636b  _ticksZ.set_tick
+00002a80: 7329 0872 2b00 0000 727e 0000 005a 0f61  s).r+...r~...Z.a
+00002a90: 7869 735f 7479 7065 5f6e 616d 6573 5a0a  xis_type_namesZ.
+00002aa0: 6178 6973 5f74 7970 6573 5a0b 785f 6178  axis_typesZ.x_ax
+00002ab0: 6973 5f74 7970 655a 0b79 5f61 7869 735f  is_typeZ.y_axis_
+00002ac0: 7479 7065 da01 78da 0179 722c 0000 0072  type..x..yr,...r
+00002ad0: 2c00 0000 722d 0000 0072 7c00 0000 4301  ,...r-...r|...C.
+00002ae0: 0000 732c 0000 0002 0202 0106 fe08 0408  ..s,............
+00002af0: 0108 0108 0102 0102 0104 ff08 0402 0102  ................
+00002b00: 0104 ff0a 050a 010e 010e 010a 020a 010c  ................
+00002b10: 0210 017a 1846 696e 6465 7243 6861 7274  ...z.FinderChart
+00002b20: 2e5f 7570 6461 7465 5f61 7865 7329 0272  ._update_axes).r
+00002b30: 1c00 0000 721d 0000 0029 0872 2f00 0000  ....r....).r/...
+00002b40: 7230 0000 0072 3100 0000 7210 0000 0072  r0...r1...r....r
+00002b50: 3200 0000 720f 0000 0072 3300 0000 7234  2...r....r3...r4
+00002b60: 0000 0029 0c72 3600 0000 7203 0000 0072  ...).r6...r....r
+00002b70: 3700 0000 7203 0000 0072 3800 0000 7239  7...r....r8...r9
+00002b80: 0000 0072 3a00 0000 720f 0000 0072 3b00  ...r:...r....r;.
+00002b90: 0000 723c 0000 0072 3300 0000 723d 0000  ..r<...r3...r=..
+00002ba0: 0029 0272 3300 0000 7215 0000 0029 0472  .).r3...r....).r
+00002bb0: 5c00 0000 7218 0000 0072 3300 0000 725d  \...r....r3...r]
+00002bc0: 0000 0029 0272 3300 0000 725f 0000 0029  ...).r3...r_...)
+00002bd0: 0672 6200 0000 7230 0000 0072 6300 0000  .rb...r0...rc...
+00002be0: 7205 0000 0072 3300 0000 725d 0000 0029  r....r3...r]...)
+00002bf0: 0272 3300 0000 725d 0000 0029 014e 2906  .r3...r]...).N).
+00002c00: 721c 0000 0072 6900 0000 726a 0000 0072  r....ri...rj...r
+00002c10: 6b00 0000 7233 0000 0072 5d00 0000 2902  k...r3...r]...).
+00002c20: 7233 0000 0072 1700 0000 2904 727e 0000  r3...r....).r~..
+00002c30: 0072 1400 0000 7233 0000 0072 5d00 0000  .r....r3...r]...
+00002c40: 2912 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00002c50: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00002c60: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
+00002c70: 2e00 0000 da0c 7374 6174 6963 6d65 7468  ......staticmeth
+00002c80: 6f64 7235 0000 0072 5700 0000 da08 7072  odr5...rW.....pr
+00002c90: 6f70 6572 7479 725b 0000 0072 5e00 0000  opertyr[...r^...
+00002ca0: 7261 0000 0072 5100 0000 7266 0000 0072  ra...rQ...rf...r
+00002cb0: 7400 0000 7264 0000 0072 7b00 0000 727c  t...rd...r{...r|
+00002cc0: 0000 0072 2c00 0000 722c 0000 0072 2c00  ...r,...r,...r,.
+00002cd0: 0000 722d 0000 0072 1b00 0000 2500 0000  ..r-...r....%...
+00002ce0: 7326 0000 0008 0004 010a 1302 0b0c 0102  s&..............
+00002cf0: 0f0c 0102 6c0c 010a 0a02 090c 010a 0e0a  ....l...........
+00002d00: 1002 090c fd0a 200a 0e0e 1b72 1b00 0000  ...... ....r....
+00002d10: 292f da0a 5f5f 6675 7475 7265 5f5f 7202  )/..__future__r.
+00002d20: 0000 0072 4b00 0000 da02 6f73 7226 0000  ...rK.....osr&..
+00002d30: 0072 0300 0000 da02 696f 7204 0000 00da  .r......ior.....
+00002d40: 0674 7970 696e 6772 0500 0000 7206 0000  .typingr....r...
+00002d50: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
+00002d60: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00002d70: 0d00 0000 da11 6d61 7470 6c6f 746c 6962  ......matplotlib
+00002d80: 2e70 7970 6c6f 74da 0670 7970 6c6f 7472  .pyplot..pyplotr
+00002d90: 6500 0000 da07 6173 7472 6f70 7972 0e00  e.....astropyr..
+00002da0: 0000 7249 0000 00da 1361 7374 726f 7079  ..rI.....astropy
+00002db0: 2e63 6f6f 7264 696e 6174 6573 720f 0000  .coordinatesr...
+00002dc0: 0072 1000 0000 da0a 6173 7472 6f70 792e  .r......astropy.
+00002dd0: 696f 7211 0000 005a 1e61 7374 726f 7079  ior....Z.astropy
+00002de0: 2e76 6973 7561 6c69 7a61 7469 6f6e 2e69  .visualization.i
+00002df0: 6e74 6572 7661 6c72 1200 0000 5a23 6173  ntervalr....Z#as
+00002e00: 7472 6f70 792e 7669 7375 616c 697a 6174  tropy.visualizat
+00002e10: 696f 6e2e 6d70 6c5f 6e6f 726d 616c 697a  ion.mpl_normaliz
+00002e20: 6572 1300 0000 5a22 6173 7472 6f70 792e  er....Z"astropy.
+00002e30: 7669 7375 616c 697a 6174 696f 6e2e 7763  visualization.wc
+00002e40: 7361 7865 732e 636f 7265 7214 0000 005a  saxes.corer....Z
+00002e50: 0b61 7374 726f 7079 2e77 6373 7215 0000  .astropy.wcsr...
+00002e60: 0072 1600 0000 5a11 6d61 7470 6c6f 746c  .r....Z.matplotl
+00002e70: 6962 2e66 6967 7572 6572 1700 0000 5a11  ib.figurer....Z.
+00002e80: 696d 6570 6875 2e61 6e6e 6f74 6174 696f  imephu.annotatio
+00002e90: 6e72 1800 0000 da15 696d 6570 6875 2e73  nr......imephu.s
+00002ea0: 6572 7669 6365 2e73 7572 7665 7972 1900  ervice.surveyr..
+00002eb0: 0000 da0c 696d 6570 6875 2e75 7469 6c73  ....imephu.utils
+00002ec0: 721a 0000 0072 1b00 0000 722c 0000 0072  r....r....r,...r
+00002ed0: 2c00 0000 722c 0000 0072 2d00 0000 da08  ,...r,...r-.....
+00002ee0: 3c6d 6f64 756c 653e 0100 0000 732a 0000  <module>....s*..
+00002ef0: 000c 0008 0208 0108 010c 010c 012c 010c  .............,..
+00002f00: 0c0c 0110 010c 010c 010c 010c 0110 010c  ................
+00002f10: 010c 020c 010c 0102 0212 03              ...........
```

### Comparing `imephu-0.1.0/src/imephu/__pycache__/geometry.cpython-310.pyc` & `imephu-0.2.0/src/imephu/__pycache__/geometry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/__pycache__/utils.cpython-310.pyc` & `imephu-0.2.0/src/imephu/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/__init__.py` & `imephu-0.2.0/src/imephu/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/__pycache__/__init__.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/__pycache__/general.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/__pycache__/general.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/__pycache__/motion.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/__pycache__/motion.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__init__.py` & `imephu-0.2.0/src/imephu/annotation/general/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__pycache__/__init__.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/general/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__pycache__/arrow.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/general/__pycache__/arrow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__pycache__/circle.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/general/__pycache__/circle.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Feb 11 15:02:42 2022 UTC, .py size: 3879 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 927a 0662 270f 0000  o........z.b'...
+00000000: 6f0d 0d0a 0000 0000 6573 c762 270f 0000  o.......es.b'...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__pycache__/crosshairs.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/general/__pycache__/crosshairs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__pycache__/empty.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/general/__pycache__/empty.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 10 10:02:05 2022 UTC, .py size: 1646 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1dab 5262 6e06 0000  o.........Rbn...
+00000000: 6f0d 0d0a 0000 0000 6573 c762 6e06 0000  o.......es.bn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6508 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 00a9 01da  Z.d.S.).........
```

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__pycache__/group.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/general/__pycache__/group.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__pycache__/line_path.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/general/__pycache__/line_path.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Feb 11 15:02:42 2022 UTC, .py size: 4428 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 927a 0662 4c11 0000  o........z.bL...
+00000000: 6f0d 0d0a 0000 0000 6573 c762 4c11 0000  o.......es.bL...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__pycache__/rectangle.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/general/__pycache__/rectangle.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/__pycache__/text.cpython-310.pyc` & `imephu-0.2.0/src/imephu/annotation/general/__pycache__/text.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 10 10:06:56 2022 UTC, .py size: 5316 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 40ac 5262 c414 0000  o.......@.Rb....
+00000000: 6f0d 0d0a 0000 0000 6573 c762 c414 0000  o.......es.b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 5a09 6400  m.Z...d.d.l.Z.d.
 00000060: 6403 6c0a 6d02 5a0b 0100 6400 6404 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 6d0e 5a0e 0100 6400 6405 6c0f  m.Z.m.Z...d.d.l.
```

### Comparing `imephu-0.1.0/src/imephu/annotation/general/arrow.py` & `imephu-0.2.0/src/imephu/annotation/general/arrow.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/circle.py` & `imephu-0.2.0/src/imephu/annotation/general/circle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/crosshairs.py` & `imephu-0.2.0/src/imephu/annotation/general/crosshairs.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/empty.py` & `imephu-0.2.0/src/imephu/annotation/general/empty.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/group.py` & `imephu-0.2.0/src/imephu/annotation/general/group.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/line_path.py` & `imephu-0.2.0/src/imephu/annotation/general/line_path.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/rectangle.py` & `imephu-0.2.0/src/imephu/annotation/general/rectangle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/general/text.py` & `imephu-0.2.0/src/imephu/annotation/general/text.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/annotation/motion.py` & `imephu-0.2.0/src/imephu/annotation/motion.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/cli.py` & `imephu-0.2.0/src/imephu/cli.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/finder_chart.py` & `imephu-0.2.0/src/imephu/finder_chart.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from __future__ import annotations
 
 import bisect
 import os
 import warnings
 from datetime import datetime
 from io import BytesIO
-from typing import Any, BinaryIO, Callable, Generator, List, Optional, Tuple, Union
+from typing import (
+    Any,
+    BinaryIO,
+    Callable,
+    Dict,
+    Generator,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 
 import matplotlib.pyplot as plt
-import pikepdf
 from astropy import units as u
 from astropy.coordinates import Angle, SkyCoord
 from astropy.io import fits
 from astropy.visualization.interval import AsymmetricPercentileInterval
 from astropy.visualization.mpl_normalize import simple_norm
 from astropy.visualization.wcsaxes.core import WCSAxesSubplot
 from astropy.wcs import WCS, FITSFixedWarning
 from matplotlib.figure import Figure
 
-import imephu
 from imephu.annotation import Annotation
 from imephu.service.survey import load_fits
 from imephu.utils import Ephemeris
 
 """A finder chart."""
 
 
@@ -47,14 +55,15 @@
     """
 
     def __init__(self, name: Union[str, BinaryIO, os.PathLike[Any]]):
         self._hdu = fits.open(name)[0]
         # The FITS data is read in only when it is needed. To avoid trying to read from
         # a closed stream later on, we thus force the data to be read in immediately.
         self._data = self._hdu.data
+        self._metadata: Dict[str, Any] = dict()
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=FITSFixedWarning)
             self._wcs = WCS(self._hdu)
         self._annotations: List[Annotation] = []
 
     @staticmethod
     def from_survey(survey: str, fits_center: SkyCoord, size: Angle) -> "FinderChart":
@@ -91,22 +100,20 @@
         * Each finder chart is created using ``create_finder_chart``.
 
         The method is completely agnostic as to what a finder chart should look like;
         this decision is left completely to ``create_finder_chart``. In particular, if
         you need any annotations for the non-sidereal nature, it is up to
         ``create_finder_chart`` to provide them.
 
-        The ``create_finder_chart`` function has to accept two arguments, in this order:
+        The ``create_finder_chart`` function has to accept as its single argument the
+        list of ephemerides to include on the finder chart.
 
-        * The center of the finder chart as a position on the sky, in right ascension
-          and declination.
-        * The list of ephemerides to include on the finder chart (for example when
-          using an annotation to indicate the target motion).
-
-        The finder charts are returned along with the time interval they cover.
+        The finder charts are returned along with the time interval they cover. The time
+        interval is also added as a tuple of `~datetime.datetime` values with the key
+        ``valid_for`` to the finder chart's metadata.
 
         Parameters
         ----------
         start: `~datetime.datetime`
             The start time of the interval to be covered by the finder charts. This must
             be a timezone-aware datetime.
         end: `~datetime.datetime`
@@ -174,15 +181,18 @@
                 current_group.append(next_ephemeris)
             else:
                 current_group = [current_group[-1], next_ephemeris]
                 groups.append(current_group)
 
         # Create the finder charts
         for group in groups:
-            yield create_finder_chart(group), (group[0].epoch, group[-1].epoch)
+            valid_for = (group[0].epoch, group[-1].epoch)
+            finder_chart = create_finder_chart(group)
+            finder_chart.add_metadata("valid_for", valid_for)
+            yield finder_chart, valid_for
 
     @property
     def wcs(self) -> WCS:
         """Return a deep copy of the WCS object of the finder chart.
 
         Returns
         -------
@@ -196,14 +206,45 @@
 
         Annotations will be plotted onto the finder chart in the order they have been
         added. So, for example, the annotation added last will be output on top of all
         the other annotations.
         """
         self._annotations.append(annotation)
 
+    @property
+    def metadata(self) -> Dict[str, Any]:
+        """
+        Return the metadata for the finder chart.
+
+        Metadata can  be added with the `add_metadata` method. A shallow copy of the
+        metadata is returned.
+
+        Returns
+        -------
+        dict
+            The metadata of the finder chart.
+        """
+        return self._metadata.copy()
+
+    def add_metadata(self, key: str, value: Any) -> None:
+        """
+        Add a key-value to the finder chart's metadata.
+
+        If the key existrs in the metadata already, the existing value for the key is
+        replaced.
+
+        Parameters
+        ----------
+        key: `str`
+            Key.
+        value: `~typing.Any`
+            Value.
+        """
+        self._metadata[key] = value
+
     def show(self) -> None:
         """Display the finder chart on the screen."""
         figure = self._create_plot()
         plt.show()
         plt.close(figure)
 
     def save(
@@ -225,20 +266,19 @@
         format: `str`, optional
             The format in which to store the finder chart.
         """
         figure = self._create_plot()
         if format and format.lower() == "pdf":
             pdf = BytesIO()
             plt.savefig(pdf, format=format, bbox_inches="tight")
-            pdf_with_metadata = FinderChart._update_pdf_metadata(pdf.getvalue())
             if hasattr(name, "write"):
-                name.write(pdf_with_metadata)  # type: ignore
+                name.write(pdf.getvalue())  # type: ignore
             else:
                 with open(name, "wb") as f:  # type: ignore
-                    f.write(pdf_with_metadata)
+                    f.write(pdf.getvalue())
         else:
             plt.savefig(name, format=format, bbox_inches="tight")
         plt.close(figure)
 
     def _create_plot(self) -> Figure:
         figure = plt.figure(figsize=(10, 9))
         ax = plt.subplot(projection=self._wcs)
@@ -305,41 +345,7 @@
         y.set_axislabel(axis_type_names[y_axis_type])
 
         x.display_minor_ticks(True)
         y.display_minor_ticks(True)
 
         x.set_ticks(size=7)
         y.set_ticks(size=7)
-
-    @staticmethod
-    def _update_pdf_metadata(pdf: bytes) -> bytes:
-        """Update a pdf by setting some metadata values.
-
-        The following metadata values are set:
-
-        - ``dc:title``: The string ``imephu x.y.z`` is assigned (where ``x.y.z`` is the
-          version).
-        - ``xmp:CreatorTool``: A string of the form "imephu x.y.z" is assigned.
-
-        The resulting pdf is returned; the original pdf remains unchanged.
-
-        See the Core properties chapter of the `XMP specification
-        <https://wwwimages2.adobe.com/content/dam/acom/en/devnet/xmp/pdfs/XMP%20SDK%20Release%20cc-2016-08/XMPSpecificationPart1.pdf>`_
-        for more details about the metadata properties.
-
-        Parameters
-        ----------
-        pdf: `bytes`
-            The pdf whose ``xml:creatorTool`` metadata value should be set.
-
-        Returns
-        -------
-        `bytes`
-            The updated pdf content.
-        """
-        with pikepdf.open(BytesIO(pdf)) as document:
-            with document.open_metadata() as meta:
-                meta["dc:title"] = "Finder Chart"
-                meta["xmp:CreatorTool"] = f"imephu {imephu.__version__}"
-            updated_pdf = BytesIO()
-            document.save(updated_pdf)
-            return updated_pdf.getvalue()
```

### Comparing `imephu-0.1.0/src/imephu/geometry.py` & `imephu-0.2.0/src/imephu/geometry.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/__pycache__/finder_chart.cpython-310.pyc` & `imephu-0.2.0/src/imephu/salt/__pycache__/finder_chart.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/__pycache__/general.cpython-310.pyc` & `imephu-0.2.0/src/imephu/salt/__pycache__/general.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/__pycache__/rss.cpython-310.pyc` & `imephu-0.2.0/src/imephu/salt/__pycache__/rss.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/__pycache__/utils.cpython-310.pyc` & `imephu-0.2.0/src/imephu/salt/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/annotation/__pycache__/nir.cpython-310.pyc` & `imephu-0.2.0/src/imephu/salt/annotation/__pycache__/nir.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/annotation/__pycache__/rss.cpython-310.pyc` & `imephu-0.2.0/src/imephu/salt/annotation/__pycache__/rss.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/annotation/__pycache__/salticam.cpython-310.pyc` & `imephu-0.2.0/src/imephu/salt/annotation/__pycache__/salticam.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/annotation/__pycache__/telescope.cpython-310.pyc` & `imephu-0.2.0/src/imephu/salt/annotation/__pycache__/telescope.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/annotation/nir.py` & `imephu-0.2.0/src/imephu/salt/annotation/nir.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/annotation/rss.py` & `imephu-0.2.0/src/imephu/salt/annotation/rss.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/annotation/salticam.py` & `imephu-0.2.0/src/imephu/salt/annotation/salticam.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/annotation/telescope.py` & `imephu-0.2.0/src/imephu/salt/annotation/telescope.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/finder_chart.py` & `imephu-0.2.0/src/imephu/salt/finder_chart.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/salt/utils.py` & `imephu-0.2.0/src/imephu/salt/utils.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/schema.json` & `imephu-0.2.0/src/imephu/schema.json`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/service/__pycache__/horizons.cpython-310.pyc` & `imephu-0.2.0/src/imephu/service/__pycache__/horizons.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 15 20:22:38 2022 UTC, .py size: 9473 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8ef5 3062 0125 0000  o.........0b.%..
+00000000: 6f0d 0d0a 0000 0000 14ac 5262 0125 0000  o.........Rb.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 6d02 5a02 6d03 5a03 0100 6400 6403 6c04  m.Z.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `imephu-0.1.0/src/imephu/service/__pycache__/survey.cpython-310.pyc` & `imephu-0.2.0/src/imephu/service/__pycache__/survey.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar 28 08:20:41 2022 UTC, .py size: 7716 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,531 +1,534 @@
-00000000: 6f0d 0d0a 0000 0000 d96f 4162 241e 0000  o........oAb$...
+00000000: 550d 0d0a 0000 0000 d96f 4162 241e 0000  U........oAb$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
+00000020: 0009 0000 0040 0000 0073 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a05 6400 6404 6c06 6d07 5a08 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 6d0b 5a0b 0100 4700  d.l.m.Z.m.Z...G.
 00000070: 6406 6407 8400 6407 650c 8303 5a0d 6408  d.d...d.e...Z.d.
 00000080: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000090: 9c08 5a0e 6411 6412 6413 6414 9c03 5a0f  ..Z.d.d.d.d...Z.
 000000a0: 4700 6415 6416 8400 6416 6504 8303 5a10  G.d.d...d.e...Z.
 000000b0: 4700 6417 6418 8400 6418 6510 8303 5a11  G.d.d...d.e...Z.
 000000c0: 4700 6419 641a 8400 641a 6510 8303 5a12  G.d.d...d.e...Z.
-000000d0: 641b 6513 641c 650b 641d 650a 641e 6503  d.e.d.e.d.e.d.e.
-000000e0: 6608 641f 6420 8404 5a14 6403 5300 2921  f.d.d ..Z.d.S.)!
-000000f0: e900 0000 0029 01da 0742 7974 6573 494f  .....)...BytesIO
-00000100: 2902 da08 4269 6e61 7279 494f da08 5072  )...BinaryIO..Pr
-00000110: 6f74 6f63 6f6c 4e29 01da 0575 6e69 7473  otocolN)...units
-00000120: 2902 da05 416e 676c 65da 0853 6b79 436f  )...Angle..SkyCo
-00000130: 6f72 6463 0000 0000 0000 0000 0000 0000  ordc............
-00000140: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
-00000150: 0065 005a 0164 005a 0264 015a 0364 0253  .e.Z.d.Z.d.Z.d.S
-00000160: 0029 03da 0b53 7572 7665 7945 7272 6f72  .)...SurveyError
-00000170: 7a30 416e 2065 7863 6570 7469 6f6e 2061  z0An exception a
-00000180: 7269 7369 6e67 2077 6865 6e20 7175 6572  rising when quer
-00000190: 7969 6e67 2061 2073 6b79 2073 7572 7665  ying a sky surve
-000001a0: 792e 4e29 04da 085f 5f6e 616d 655f 5fda  y.N)...__name__.
-000001b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000001c0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-000001d0: 5f5f a900 720d 0000 0072 0d00 0000 fa41  __..r....r.....A
-000001e0: 2f55 7365 7273 2f63 6872 6973 7469 616e  /Users/christian
-000001f0: 2f49 6465 6150 726f 6a65 6374 732f 696d  /IdeaProjects/im
-00000200: 6570 6875 2f73 7263 2f69 6d65 7068 752f  ephu/src/imephu/
-00000210: 7365 7276 6963 652f 7375 7276 6579 2e70  service/survey.p
-00000220: 7972 0800 0000 0900 0000 7306 0000 0008  yr........s.....
-00000230: 0004 0104 0272 0800 0000 5a0e 706f 7373  .....r....Z.poss
-00000240: 3275 6b73 7475 5f72 6564 5a0f 706f 7373  2ukstu_redZ.poss
-00000250: 3275 6b73 7475 5f62 6c75 655a 0d70 6f73  2ukstu_blueZ.pos
-00000260: 7332 756b 7374 755f 6972 5a09 706f 7373  s2ukstu_irZ.poss
-00000270: 315f 7265 645a 0a70 6f73 7331 5f62 6c75  1_redZ.poss1_blu
-00000280: 655a 0671 7569 636b 765a 0b70 6861 7365  eZ.quickvZ.phase
-00000290: 325f 6773 6332 5a0b 7068 6173 6532 5f67  2_gsc2Z.phase2_g
-000002a0: 7363 3129 087a 0f50 4f53 5332 2f55 4b53  sc1).z.POSS2/UKS
-000002b0: 5455 2052 6564 7a10 504f 5353 322f 554b  TU Redz.POSS2/UK
-000002c0: 5354 5520 426c 7565 7a0e 504f 5353 322f  STU Bluez.POSS2/
-000002d0: 554b 5354 5520 4952 7a09 504f 5353 3120  UKSTU IRz.POSS1 
-000002e0: 5265 647a 0a50 4f53 5331 2042 6c75 657a  Redz.POSS1 Bluez
-000002f0: 0751 7569 636b 2d56 7a11 4853 5420 5068  .Quick-Vz.HST Ph
-00000300: 6173 6532 2028 4753 4332 297a 1148 5354  ase2 (GSC2)z.HST
-00000310: 2050 6861 7365 3220 2847 5343 3129 7a07   Phase2 (GSC1)z.
-00000320: 326d 6173 732d 687a 0732 6d61 7373 2d6a  2mass-hz.2mass-j
-00000330: 7a07 326d 6173 732d 6b29 037a 0732 4d41  z.2mass-k).z.2MA
-00000340: 5353 2d48 7a07 324d 4153 532d 4a7a 0732  SS-Hz.2MASS-Jz.2
-00000350: 4d41 5353 2d4b 6300 0000 0000 0000 0000  MASS-Kc.........
-00000360: 0000 0000 0000 0008 0000 0040 0000 0073  ...........@...s
-00000370: 2a00 0000 6500 5a01 6400 5a02 6401 5a03  *...e.Z.d.Z.d.Z.
-00000380: 6402 6504 6403 6505 6404 6506 6405 6507  d.e.d.e.d.e.d.e.
-00000390: 6608 6406 6407 8404 5a08 6408 5300 2909  f.d.d...Z.d.S.).
-000003a0: da09 536b 7953 7572 7665 797a 3441 2073  ..SkySurveyz4A s
-000003b0: 6b79 2073 7572 7665 7920 6672 6f6d 2077  ky survey from w
-000003c0: 6869 6368 2066 6974 7320 6669 6c65 7320  hich fits files 
-000003d0: 6361 6e20 6265 2072 6571 7565 7374 6564  can be requested
-000003e0: 2eda 0673 7572 7665 79da 0b66 6974 735f  ...survey..fits_
-000003f0: 6365 6e74 6572 da04 7369 7a65 da06 7265  center..size..re
-00000400: 7475 726e 6304 0000 0000 0000 0000 0000  turnc...........
-00000410: 0004 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-00000420: 0000 7400 8201 2902 6129 0200 004c 6f61  ..t...).a)...Loa
-00000430: 6420 6120 4649 5453 2066 696c 6520 666f  d a FITS file fo
-00000440: 7220 6120 6769 7665 6e20 706f 7369 7469  r a given positi
-00000450: 6f6e 2066 726f 6d20 7468 6520 736b 7920  on from the sky 
-00000460: 7375 7276 6579 2e0a 0a20 2020 2020 2020  survey...       
-00000470: 2054 6865 2073 697a 6520 6f66 2074 6865   The size of the
-00000480: 2072 6574 7572 6e65 6420 4649 5453 2066   returned FITS f
-00000490: 696c 6520 6973 2064 6574 6572 6d69 6e65  ile is determine
-000004a0: 6420 6279 2074 6865 2063 6c61 7373 2069  d by the class i
-000004b0: 6d70 6c65 6d65 6e74 696e 6720 7468 6973  mplementing this
-000004c0: 0a20 2020 2020 2020 2070 726f 746f 636f  .        protoco
-000004d0: 6c20 286f 7220 7468 6520 7765 6220 7365  l (or the web se
-000004e0: 7276 6963 6520 7573 6564 292e 0a0a 2020  rvice used)...  
-000004f0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00000500: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00000510: 2d2d 2d0a 2020 2020 2020 2020 7375 7276  ---.        surv
-00000520: 6579 3a20 6073 7472 600a 2020 2020 2020  ey: `str`.      
-00000530: 2020 2020 2020 5468 6520 6e61 6d65 206f        The name o
-00000540: 6620 7468 6520 7375 7276 6579 2074 6f20  f the survey to 
-00000550: 7175 6572 7920 666f 7220 7468 6520 4649  query for the FI
-00000560: 5453 2066 696c 652e 0a20 2020 2020 2020  TS file..       
-00000570: 2066 6974 735f 6365 6e74 6572 3a20 607e   fits_center: `~
-00000580: 6173 7472 6f70 792e 636f 6f72 6469 6e61  astropy.coordina
-00000590: 7465 732e 536b 7943 6f6f 7264 600a 2020  tes.SkyCoord`.  
-000005a0: 2020 2020 2020 2020 2020 5468 6520 6365            The ce
-000005b0: 6e74 6572 2070 6f73 6974 696f 6e20 6f66  nter position of
-000005c0: 2074 6865 206c 6f61 6465 6420 4649 5453   the loaded FITS
-000005d0: 2066 696c 652e 0a20 2020 2020 2020 2073   file..        s
-000005e0: 697a 653a 2060 7e61 7374 726f 7079 2e63  ize: `~astropy.c
-000005f0: 6f6f 7264 696e 6174 6573 2e41 6e67 6c65  oordinates.Angle
-00000600: 600a 2020 2020 2020 2020 2020 2020 5468  `.            Th
-00000610: 6520 7769 6474 6820 616e 6420 6865 6967  e width and heig
-00000620: 6874 206f 6620 7468 6520 4649 5453 2069  ht of the FITS i
-00000630: 6d61 6765 2c20 6173 2061 6e20 616e 676c  mage, as an angl
-00000640: 6520 6f6e 2074 6865 2073 6b79 2e0a 2020  e on the sky..  
-00000650: 2020 2020 2020 4e29 01da 134e 6f74 496d        N)...NotIm
-00000660: 706c 656d 656e 7465 6445 7272 6f72 2904  plementedError).
-00000670: da04 7365 6c66 7210 0000 0072 1100 0000  ..selfr....r....
-00000680: 7212 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000690: 0e00 0000 da09 6c6f 6164 5f66 6974 7325  ......load_fits%
-000006a0: 0000 0073 0200 0000 040f 7a13 536b 7953  ...s......z.SkyS
-000006b0: 7572 7665 792e 6c6f 6164 5f66 6974 734e  urvey.load_fitsN
-000006c0: 2909 7209 0000 0072 0a00 0000 720b 0000  ).r....r....r...
-000006d0: 0072 0c00 0000 da03 7374 7272 0700 0000  .r......strr....
-000006e0: 7206 0000 0072 0300 0000 7216 0000 0072  r....r....r....r
-000006f0: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00000700: 0000 0072 0f00 0000 2200 0000 7306 0000  ...r...."...s...
-00000710: 0008 0004 011e 0272 0f00 0000 6300 0000  .......r....c...
-00000720: 0000 0000 0000 0000 0000 0000 0008 0000  ................
-00000730: 0040 0000 0073 4600 0000 6500 5a01 6400  .@...sF...e.Z.d.
-00000740: 5a02 6401 5a03 640d 6404 6405 8404 5a04  Z.d.Z.d.d.d...Z.
-00000750: 6406 6505 6407 6506 6408 6507 6402 6508  d.e.d.e.d.e.d.e.
-00000760: 6608 6409 640a 8404 5a09 6406 6505 6402  f.d.d...Z.d.e.d.
-00000770: 6505 6604 640b 640c 8404 5a0a 6403 5300  e.f.d.d...Z.d.S.
-00000780: 290e da12 4469 6769 7469 7a65 6453 6b79  )...DigitizedSky
-00000790: 5375 7276 6579 7aac 4120 636c 6173 7320  Surveyz.A class 
-000007a0: 666f 7220 6c6f 6164 696e 6720 4649 5453  for loading FITS
-000007b0: 2066 696c 6573 2066 726f 6d20 7468 6520   files from the 
-000007c0: 4469 6769 7469 7a65 6420 536b 7920 5375  Digitized Sky Su
-000007d0: 7276 6579 2028 4453 5329 2e0a 0a20 2020  rvey (DSS)...   
-000007e0: 2053 6565 2074 6865 2060 4453 5320 6172   See the `DSS ar
-000007f0: 6368 6976 6520 7765 6273 6974 6520 3c68  chive website <h
-00000800: 7474 7073 3a2f 2f61 7263 6869 7665 2e73  ttps://archive.s
-00000810: 7473 6369 2e65 6475 2f64 7373 2f69 6e64  tsci.edu/dss/ind
-00000820: 6578 2e68 746d 6c3e 6020 666f 7220 6d6f  ex.html>` for mo
-00000830: 7265 0a20 2020 2064 6574 6169 6c73 2e0a  re.    details..
-00000840: 2020 2020 7213 0000 004e 6301 0000 0000      r....Nc.....
-00000850: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000860: 0000 0073 1800 0000 6401 6402 8400 7400  ...s....d.d...t.
-00000870: a001 a100 4400 8301 7c00 5f02 6400 5300  ....D...|._.d.S.
-00000880: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00000890: 0300 0000 0400 0000 5300 0000 f31a 0000  ........S.......
-000008a0: 0069 007c 005d 095c 027d 017d 027c 01a0  .i.|.].\.}.}.|..
-000008b0: 00a1 007c 0293 0271 0253 0072 0d00 0000  ...|...q.S.r....
-000008c0: a901 da05 6c6f 7765 72a9 03da 022e 30da  ....lower.....0.
-000008d0: 036b 6579 da05 7661 6c75 6572 0d00 0000  .key..valuer....
-000008e0: 720d 0000 0072 0e00 0000 da0a 3c64 6963  r....r......<dic
-000008f0: 7463 6f6d 703e 3f00 0000 f306 0000 0006  tcomp>?.........
-00000900: 000e 0106 ff7a 2f44 6967 6974 697a 6564  .....z/Digitized
-00000910: 536b 7953 7572 7665 792e 5f5f 696e 6974  SkySurvey.__init
-00000920: 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  __.<locals>.<dic
-00000930: 7463 6f6d 703e 2903 da10 5f44 5353 5f49  tcomp>)..._DSS_I
-00000940: 4445 4e54 4946 4945 5253 da05 6974 656d  DENTIFIERS..item
-00000950: 73da 135f 7375 7276 6579 5f69 6465 6e74  s.._survey_ident
-00000960: 6966 6965 7273 2901 7215 0000 0072 0d00  ifiers).r....r..
-00000970: 0000 720d 0000 0072 0e00 0000 da08 5f5f  ..r....r......__
-00000980: 696e 6974 5f5f 3e00 0000 7306 0000 0006  init__>...s.....
-00000990: 0106 010c ff7a 1b44 6967 6974 697a 6564  .....z.Digitized
-000009a0: 536b 7953 7572 7665 792e 5f5f 696e 6974  SkySurvey.__init
-000009b0: 5f5f 7210 0000 0072 1100 0000 7212 0000  __r....r....r...
-000009c0: 0063 0400 0000 0000 0000 0000 0000 0700  .c..............
-000009d0: 0000 0900 0000 4300 0000 736e 0000 0064  ......C...sn...d
-000009e0: 017d 047c 00a0 007c 01a1 017c 026a 01a0  .}.|...|...|.j..
-000009f0: 0274 036a 04a1 017c 026a 05a0 0274 036a  .t.j...|.j...t.j
-00000a00: 04a1 0164 027c 03a0 0274 036a 06a1 017c  ...d.|...t.j...|
-00000a10: 03a0 0274 036a 06a1 0164 0364 0464 059c  ...t.j...d.d.d..
-00000a20: 087d 0574 076a 087c 047c 0564 068d 027d  .}.t.j.|.|.d...}
-00000a30: 067c 066a 0964 076b 0372 3274 0a64 0883  .|.j.d.k.r2t.d..
-00000a40: 0182 0174 0b7c 066a 0c83 0153 0029 0a61  ...t.|.j...S.).a
-00000a50: 7203 0000 4c6f 6164 2061 2046 4954 5320  r...Load a FITS 
-00000a60: 6669 6c65 2066 6f72 2061 2067 6976 656e  file for a given
-00000a70: 2070 6f73 6974 696f 6e20 6672 6f6d 2074   position from t
-00000a80: 6865 2073 6b79 2073 7572 7665 792e 0a0a  he sky survey...
-00000a90: 2020 2020 2020 2020 5468 6520 666f 6c6c          The foll
-00000aa0: 6f77 696e 6720 7375 7276 6579 7320 6361  owing surveys ca
-00000ab0: 6e20 6265 2071 7565 7269 6564 2066 6f72  n be queried for
-00000ac0: 2046 4954 5320 696d 6167 6573 3a0a 0a20   FITS images:.. 
-00000ad0: 2020 2020 2020 202d 2050 4f53 5332 2f55         - POSS2/U
-00000ae0: 4b53 5455 2052 6564 0a20 2020 2020 2020  KSTU Red.       
-00000af0: 202d 2050 4f53 5332 2f55 4b53 5455 2042   - POSS2/UKSTU B
-00000b00: 6c75 650a 2020 2020 2020 2020 2d20 504f  lue.        - PO
-00000b10: 5353 322f 554b 5354 5520 4952 0a20 2020  SS2/UKSTU IR.   
-00000b20: 2020 2020 202d 2050 4f53 5331 2052 6564       - POSS1 Red
-00000b30: 0a20 2020 2020 2020 202d 2050 4f53 5331  .        - POSS1
-00000b40: 2042 6c75 650a 2020 2020 2020 2020 2d20   Blue.        - 
-00000b50: 5175 6963 6b2d 560a 2020 2020 2020 2020  Quick-V.        
-00000b60: 2d20 4853 5420 5068 6173 6532 2028 4753  - HST Phase2 (GS
-00000b70: 4332 290a 2020 2020 2020 2020 2d20 4853  C2).        - HS
-00000b80: 5420 5068 6173 6532 2028 4753 4331 290a  T Phase2 (GSC1).
-00000b90: 0a20 2020 2020 2020 2053 6565 2074 6865  .        See the
-00000ba0: 2060 4453 5320 7375 7276 6579 2070 6167   `DSS survey pag
-00000bb0: 6520 3c68 7474 703a 2f2f 6773 7373 2e73  e <http://gsss.s
-00000bc0: 7473 6369 2e65 6475 2f53 6b79 5375 7276  tsci.edu/SkySurv
-00000bd0: 6579 732f 5375 7276 6579 732e 6874 6d3e  eys/Surveys.htm>
-00000be0: 6020 666f 720a 2020 2020 2020 2020 6465  ` for.        de
-00000bf0: 7461 696c 7320 6162 6f75 7420 7468 6573  tails about thes
-00000c00: 6520 7375 7276 6579 732e 0a0a 2020 2020  e surveys...    
-00000c10: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000c20: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00000c30: 2d0a 2020 2020 2020 2020 7375 7276 6579  -.        survey
-00000c40: 3a20 6073 7472 600a 2020 2020 2020 2020  : `str`.        
-00000c50: 2020 2020 5468 6520 6e61 6d65 206f 6620      The name of 
-00000c60: 7468 6520 7375 7276 6579 2074 6f20 7175  the survey to qu
-00000c70: 6572 7920 666f 7220 7468 6520 4649 5453  ery for the FITS
-00000c80: 2066 696c 652e 0a20 2020 2020 2020 2066   file..        f
-00000c90: 6974 735f 6365 6e74 6572 3a20 607e 6173  its_center: `~as
-00000ca0: 7472 6f70 792e 636f 6f72 6469 6e61 7465  tropy.coordinate
-00000cb0: 732e 536b 7943 6f6f 7264 600a 2020 2020  s.SkyCoord`.    
-00000cc0: 2020 2020 2020 2020 5468 6520 6365 6e74          The cent
-00000cd0: 6572 2070 6f73 6974 696f 6e20 6f66 2074  er position of t
-00000ce0: 6865 206c 6f61 6465 6420 4649 5453 2066  he loaded FITS f
-00000cf0: 696c 652e 0a20 2020 2020 2020 2073 697a  ile..        siz
-00000d00: 653a 2060 7e61 7374 726f 7079 2e63 6f6f  e: `~astropy.coo
-00000d10: 7264 696e 6174 6573 2e41 6e67 6c65 600a  rdinates.Angle`.
-00000d20: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00000d30: 7769 6474 6820 616e 6420 6865 6967 6874  width and height
-00000d40: 206f 6620 7468 6520 4649 5453 2069 6d61   of the FITS ima
-00000d50: 6765 2c20 6173 2061 6e20 616e 676c 6520  ge, as an angle 
-00000d60: 6f6e 2074 6865 2073 6b79 2e0a 0a20 2020  on the sky...   
-00000d70: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00000d80: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00000d90: 2020 2020 2062 696e 6172 7920 7374 7265       binary stre
-00000da0: 616d 0a20 2020 2020 2020 2020 2020 2054  am.            T
-00000db0: 6865 2046 4954 5320 6669 6c65 2e0a 2020  he FITS file..  
-00000dc0: 2020 2020 2020 7a2c 6874 7470 733a 2f2f        z,https://
-00000dd0: 6172 6368 6976 652e 7374 7363 692e 6564  archive.stsci.ed
-00000de0: 752f 6367 692d 6269 6e2f 6473 735f 7365  u/cgi-bin/dss_se
-00000df0: 6172 6368 da05 4a32 3030 30da 0466 6974  arch..J2000..fit
-00000e00: 73da 046e 6f6e 6529 08da 0176 da01 72da  s..none)...v..r.
-00000e10: 0164 da01 65da 0168 da01 77da 0166 da01  .d..e..h..w..f..
-00000e20: 63a9 01da 0670 6172 616d 73e9 c800 0000  c....params.....
-00000e30: fa1d 4e6f 2046 4954 5320 6669 6c65 2063  ..No FITS file c
-00000e40: 6f75 6c64 2062 6520 6c6f 6164 6564 2e4e  ould be loaded.N
-00000e50: 290d da12 5f73 7572 7665 795f 6964 656e  )..._survey_iden
-00000e60: 7469 6669 6572 da02 7261 da08 746f 5f76  tifier..ra..to_v
-00000e70: 616c 7565 da01 75da 0364 6567 da03 6465  alue..u..deg..de
-00000e80: 63da 0661 7263 6d69 6eda 0872 6571 7565  c..arcmin..reque
-00000e90: 7374 73da 0367 6574 da0b 7374 6174 7573  sts..get..status
-00000ea0: 5f63 6f64 6572 0800 0000 7202 0000 00da  _coder....r.....
-00000eb0: 0763 6f6e 7465 6e74 a907 7215 0000 0072  .content..r....r
-00000ec0: 1000 0000 7211 0000 0072 1200 0000 da03  ....r....r......
-00000ed0: 7572 6c72 3200 0000 da08 7265 7370 6f6e  urlr2.....respon
-00000ee0: 7365 720d 0000 0072 0d00 0000 720e 0000  ser....r....r...
-00000ef0: 0072 1600 0000 4300 0000 731c 0000 0004  .r....C...s.....
-00000f00: 1f08 020c 010c 0102 010a 010a 0102 0102  ................
-00000f10: 0106 f80e 0a0a 0108 010a 017a 1c44 6967  ...........z.Dig
-00000f20: 6974 697a 6564 536b 7953 7572 7665 792e  itizedSkySurvey.
-00000f30: 6c6f 6164 5f66 6974 7363 0200 0000 0000  load_fitsc......
-00000f40: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00000f50: 0000 f32a 0000 007c 01a0 00a1 007c 006a  ...*...|.....|.j
-00000f60: 0176 0172 0e74 0264 017c 019b 009d 0283  .v.r.t.d.|......
-00000f70: 0182 017c 006a 017c 01a0 00a1 0019 0053  ...|.j.|.......S
-00000f80: 00a9 024e fa10 556e 6b6e 6f77 6e20 7375  ...N..Unknown su
-00000f90: 7276 6579 3a20 a903 721b 0000 0072 2400  rvey: ..r....r$.
-00000fa0: 0000 da0a 5661 6c75 6545 7272 6f72 a902  ....ValueError..
-00000fb0: 7215 0000 0072 1000 0000 720d 0000 0072  r....r....r....r
-00000fc0: 0d00 0000 720e 0000 0072 3500 0000 7200  ....r....r5...r.
-00000fd0: 0000 f306 0000 000e 010e 010e 027a 2544  .............z%D
-00000fe0: 6967 6974 697a 6564 536b 7953 7572 7665  igitizedSkySurve
-00000ff0: 792e 5f73 7572 7665 795f 6964 656e 7469  y._survey_identi
-00001000: 6669 6572 2902 7213 0000 004e 290b 7209  fier).r....N).r.
-00001010: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
-00001020: 0000 7225 0000 0072 1700 0000 7207 0000  ..r%...r....r...
-00001030: 0072 0600 0000 7203 0000 0072 1600 0000  .r....r....r....
-00001040: 7235 0000 0072 0d00 0000 720d 0000 0072  r5...r....r....r
-00001050: 0d00 0000 720e 0000 0072 1800 0000 3700  ....r....r....7.
-00001060: 0000 730a 0000 0008 0004 010a 061a 0516  ..s.............
-00001070: 2f72 1800 0000 6300 0000 0000 0000 0000  /r....c.........
-00001080: 0000 0000 0000 0008 0000 0040 0000 0073  ...........@...s
-00001090: 5000 0000 6500 5a01 6400 5a02 6401 5a03  P...e.Z.d.Z.d.Z.
-000010a0: 640f 6403 6504 6404 6405 6604 6406 6407  d.d.e.d.d.f.d.d.
-000010b0: 8405 5a05 6408 6506 6409 6507 640a 6508  ..Z.d.e.d.e.d.e.
-000010c0: 6404 6509 6608 640b 640c 8404 5a0a 6408  d.e.f.d.d...Z.d.
-000010d0: 6506 6404 6506 6604 640d 640e 8404 5a0b  e.d.e.f.d.d...Z.
-000010e0: 6405 5300 2910 da07 536b 7956 6965 7761  d.S.)...SkyViewa
-000010f0: 0b01 0000 4120 636c 6173 7320 666f 7220  ....A class for 
-00001100: 6c6f 6164 696e 6720 4649 5453 2066 696c  loading FITS fil
-00001110: 6573 2066 726f 6d20 536b 7956 6965 772e  es from SkyView.
-00001120: 0a0a 2020 2020 5365 6520 7468 6520 6053  ..    See the `S
-00001130: 6b79 5669 6577 2073 6974 6520 3c68 7474  kyView site <htt
-00001140: 7073 3a2f 2f73 6b79 7669 6577 2e67 7366  ps://skyview.gsf
-00001150: 632e 6e61 7361 2e67 6f76 2f63 7572 7265  c.nasa.gov/curre
-00001160: 6e74 2f63 6769 2f74 6974 6c65 7061 6765  nt/cgi/titlepage
-00001170: 2e70 6c3e 6020 666f 720a 2020 2020 6d6f  .pl>` for.    mo
-00001180: 7265 2064 6574 6169 6c73 2061 626f 7574  re details about
-00001190: 2053 6b79 5669 6577 2e0a 0a20 2020 2050   SkyView...    P
-000011a0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-000011b0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2070 6978  --------.    pix
-000011c0: 656c 733a 2060 696e 7460 2c20 6465 6661  els: `int`, defa
-000011d0: 756c 743a 2033 3030 0a20 2020 2020 2020  ult: 300.       
-000011e0: 2054 6865 2069 6d61 6765 2073 697a 6520   The image size 
-000011f0: 696e 2070 6978 656c 732e 0a20 2020 20e9  in pixels..    .
-00001200: 2c01 0000 da06 7069 7865 6c73 7213 0000  ,.....pixelsr...
-00001210: 004e 6302 0000 0000 0000 0000 0000 0002  .Nc.............
-00001220: 0000 0003 0000 0043 0000 0073 1e00 0000  .......C...s....
-00001230: 7c01 7c00 5f00 6401 6402 8400 7401 a002  |.|._.d.d...t...
-00001240: a100 4400 8301 7c00 5f03 6400 5300 2903  ..D...|._.d.S.).
-00001250: 4e63 0100 0000 0000 0000 0000 0000 0300  Nc..............
-00001260: 0000 0400 0000 5300 0000 7219 0000 0072  ......S...r....r
-00001270: 0d00 0000 721a 0000 0072 1c00 0000 720d  ....r....r....r.
-00001280: 0000 0072 0d00 0000 720e 0000 0072 2000  ...r....r....r .
-00001290: 0000 8700 0000 7221 0000 007a 2453 6b79  ......r!...z$Sky
-000012a0: 5669 6577 2e5f 5f69 6e69 745f 5f2e 3c6c  View.__init__.<l
-000012b0: 6f63 616c 733e 2e3c 6469 6374 636f 6d70  ocals>.<dictcomp
-000012c0: 3e29 04da 075f 7069 7865 6c73 da14 5f53  >)..._pixels.._S
-000012d0: 4b59 5649 4557 5f49 4445 4e54 4946 4945  KYVIEW_IDENTIFIE
-000012e0: 5253 7223 0000 0072 2400 0000 2902 7215  RSr#...r$...).r.
-000012f0: 0000 0072 4c00 0000 720d 0000 0072 0d00  ...rL...r....r..
-00001300: 0000 720e 0000 0072 2500 0000 8500 0000  ..r....r%.......
-00001310: 7308 0000 0006 0106 0106 010c ff7a 1053  s............z.S
-00001320: 6b79 5669 6577 2e5f 5f69 6e69 745f 5f72  kyView.__init__r
-00001330: 1000 0000 7211 0000 0072 1200 0000 6304  ....r....r....c.
-00001340: 0000 0000 0000 0000 0000 0007 0000 0008  ................
-00001350: 0000 0043 0000 0073 6e00 0000 6401 7d04  ...C...sn...d.}.
-00001360: 7c02 6a00 a001 7402 6a03 a101 9b00 6402  |.j...t.j.....d.
-00001370: 7c02 6a04 a001 7402 6a03 a101 9b00 9d03  |.j...t.j.......
-00001380: 7c00 a005 7c01 a101 6403 6404 7c00 6a06  |...|...d.d.|.j.
-00001390: 7c03 a001 7402 6a03 a101 6405 9c06 7d05  |...t.j...d...}.
-000013a0: 7407 6a08 7c04 7c05 6406 8d02 7d06 7c06  t.j.|.|.d...}.|.
-000013b0: 6a09 6407 6b03 7232 740a 6408 8301 8201  j.d.k.r2t.d.....
-000013c0: 740b 7c06 6a0c 8301 5300 290a 6109 0300  t.|.j...S.).a...
-000013d0: 004c 6f61 6420 6120 4649 5453 2066 696c  .Load a FITS fil
-000013e0: 6520 666f 7220 6120 6769 7665 6e20 706f  e for a given po
-000013f0: 7369 7469 6f6e 2066 726f 6d20 7468 6520  sition from the 
-00001400: 736b 7920 7375 7276 6579 2e0a 0a20 2020  sky survey...   
-00001410: 2020 2020 2054 6865 2066 6f6c 6c6f 7769       The followi
-00001420: 6e67 2073 7562 7365 7420 6f66 2073 7572  ng subset of sur
-00001430: 7665 7973 2073 7570 706f 7274 6564 2062  veys supported b
-00001440: 7920 536b 7956 6965 7720 6361 6e20 6265  y SkyView can be
-00001450: 2071 7565 7269 6564 3a0a 0a20 2020 2020   queried:..     
-00001460: 2020 202d 2032 4d41 5353 2d48 0a20 2020     - 2MASS-H.   
-00001470: 2020 2020 202d 2032 4d41 5353 2d4a 0a20       - 2MASS-J. 
-00001480: 2020 2020 2020 202d 2032 4d41 5353 2d4b         - 2MASS-K
-00001490: 0a0a 2020 2020 2020 2020 5365 6520 7468  ..        See th
-000014a0: 6520 6053 6b79 5669 6577 2073 7572 7665  e `SkyView surve
-000014b0: 7920 7061 6765 0a20 2020 2020 2020 203c  y page.        <
-000014c0: 6874 7470 733a 2f2f 736b 7976 6965 772e  https://skyview.
-000014d0: 6773 6663 2e6e 6173 612e 676f 762f 6375  gsfc.nasa.gov/cu
-000014e0: 7272 656e 742f 6367 692f 7375 7276 6579  rrent/cgi/survey
-000014f0: 2e70 6c3e 6020 666f 7220 6465 7461 696c  .pl>` for detail
-00001500: 7320 6162 6f75 7420 7468 6573 650a 2020  s about these.  
-00001510: 2020 2020 2020 7375 7276 6579 732e 0a0a        surveys...
-00001520: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00001530: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00001540: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7375  -----.        su
-00001550: 7276 6579 3a20 6073 7472 600a 2020 2020  rvey: `str`.    
-00001560: 2020 2020 2020 2020 5468 6520 6e61 6d65          The name
-00001570: 206f 6620 7468 6520 7375 7276 6579 2074   of the survey t
-00001580: 6f20 7175 6572 7920 666f 7220 7468 6520  o query for the 
-00001590: 4649 5453 2066 696c 652e 0a20 2020 2020  FITS file..     
-000015a0: 2020 2066 6974 735f 6365 6e74 6572 3a20     fits_center: 
-000015b0: 607e 6173 7472 6f70 792e 636f 6f72 6469  `~astropy.coordi
-000015c0: 6e61 7465 732e 536b 7943 6f6f 7264 600a  nates.SkyCoord`.
-000015d0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000015e0: 6365 6e74 6572 2070 6f73 6974 696f 6e20  center position 
-000015f0: 6f66 2074 6865 206c 6f61 6465 6420 4649  of the loaded FI
-00001600: 5453 2066 696c 652e 0a20 2020 2020 2020  TS file..       
-00001610: 2073 697a 653a 2060 7e61 7374 726f 7079   size: `~astropy
-00001620: 2e63 6f6f 7264 696e 6174 6573 2e41 6e67  .coordinates.Ang
-00001630: 6c65 600a 2020 2020 2020 2020 2020 2020  le`.            
-00001640: 5468 6520 7769 6474 6820 616e 6420 6865  The width and he
-00001650: 6967 6874 206f 6620 7468 6520 4649 5453  ight of the FITS
-00001660: 2069 6d61 6765 2c20 6173 2061 6e20 616e   image, as an an
-00001670: 676c 6520 6f6e 2074 6865 2073 6b79 2e0a  gle on the sky..
-00001680: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00001690: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000016a0: 0a20 2020 2020 2020 2062 696e 6172 7920  .        binary 
-000016b0: 7374 7265 616d 0a20 2020 2020 2020 2020  stream.         
-000016c0: 2020 2054 6865 2046 4954 5320 6669 6c65     The FITS file
-000016d0: 2e0a 2020 2020 2020 2020 7a35 6874 7470  ..        z5http
-000016e0: 733a 2f2f 736b 7976 6965 772e 6773 6663  s://skyview.gsfc
-000016f0: 2e6e 6173 612e 676f 762f 6375 7272 656e  .nasa.gov/curren
-00001700: 742f 6367 692f 7275 6e71 7565 7279 2e70  t/cgi/runquery.p
-00001710: 6c7a 022c 20da 0449 4352 53da 0446 4954  lz., ..ICRS..FIT
-00001720: 5329 065a 0850 6f73 6974 696f 6e5a 0653  S).Z.PositionZ.S
-00001730: 7572 7665 795a 0b43 6f6f 7264 696e 6174  urveyZ.Coordinat
-00001740: 6573 da06 5265 7475 726e 5a06 5069 7865  es..ReturnZ.Pixe
-00001750: 6c73 da04 5369 7a65 7231 0000 0072 3300  ls..Sizer1...r3.
-00001760: 0000 7234 0000 004e 290d 7236 0000 0072  ..r4...N).r6...r
-00001770: 3700 0000 7238 0000 0072 3900 0000 723a  7...r8...r9...r:
-00001780: 0000 0072 3500 0000 724d 0000 0072 3c00  ...r5...rM...r<.
-00001790: 0000 723d 0000 0072 3e00 0000 7208 0000  ..r=...r>...r...
-000017a0: 0072 0200 0000 723f 0000 0072 4000 0000  .r....r?...r@...
-000017b0: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-000017c0: 1600 0000 8b00 0000 731c 0000 0004 1b10  ........s.......
-000017d0: 020c 0104 ff08 0202 0102 0104 010a 0106  ................
-000017e0: f90e 090a 0108 010a 017a 1153 6b79 5669  .........z.SkyVi
-000017f0: 6577 2e6c 6f61 645f 6669 7473 6302 0000  ew.load_fitsc...
-00001800: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00001810: 0043 0000 0072 4300 0000 7244 0000 0072  .C...rC...rD...r
-00001820: 4600 0000 7248 0000 0072 0d00 0000 720d  F...rH...r....r.
-00001830: 0000 0072 0e00 0000 7235 0000 00b5 0000  ...r....r5......
-00001840: 0072 4900 0000 7a1a 536b 7956 6965 772e  .rI...z.SkyView.
-00001850: 5f73 7572 7665 795f 6964 656e 7469 6669  _survey_identifi
-00001860: 6572 2901 724b 0000 0029 0c72 0900 0000  er).rK...).r....
-00001870: 720a 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-00001880: 0369 6e74 7225 0000 0072 1700 0000 7207  .intr%...r....r.
-00001890: 0000 0072 0600 0000 7203 0000 0072 1600  ...r....r....r..
-000018a0: 0000 7235 0000 0072 0d00 0000 720d 0000  ..r5...r....r...
-000018b0: 0072 0d00 0000 720e 0000 0072 4a00 0000  .r....r....rJ...
-000018c0: 7900 0000 730a 0000 0008 0004 0114 0b1a  y...s...........
-000018d0: 0616 2a72 4a00 0000 7210 0000 0072 1100  ..*rJ...r....r..
-000018e0: 0000 7212 0000 0072 1300 0000 6303 0000  ..r....r....c...
-000018f0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
-00001900: 0043 0000 0073 6400 0000 7c00 a000 a100  .C...sd...|.....
-00001910: 6401 6402 8400 7401 a002 a100 4400 8301  d.d...t.....D...
-00001920: 7600 7211 7403 8300 7d03 6e1a 7c00 a000  v.r.t...}.n.|...
-00001930: a100 6403 6402 8400 7404 a002 a100 4400  ..d.d...t.....D.
-00001940: 8301 7600 7224 7405 6404 6405 8d01 7d03  ..v.r$t.d.d...}.
-00001950: 6e07 7406 6406 7c00 9b00 9d02 8301 8201  n.t.d.|.........
-00001960: 7c03 a007 7c00 7c01 7c02 a103 5300 2908  |...|.|.|...S.).
-00001970: 6173 0500 0052 6571 7565 7374 2061 2046  as...Request a F
-00001980: 4954 5320 696d 6167 6520 6672 6f6d 2061  ITS image from a
-00001990: 2073 6b79 2073 7572 7665 792e 0a0a 2020   sky survey...  
-000019a0: 2020 496e 2070 7269 6e63 6970 6c65 2c20    In principle, 
-000019b0: 7468 6973 2066 756e 6374 696f 6e20 6973  this function is
-000019c0: 2065 7175 6976 616c 656e 7420 746f 2074   equivalent to t
-000019d0: 6865 2060 6c6f 6164 5f66 6974 7360 206d  he `load_fits` m
-000019e0: 6574 686f 6473 206f 6620 7468 650a 2020  ethods of the.  
-000019f0: 2020 6053 6b79 5375 7276 6579 6020 696d    `SkySurvey` im
-00001a00: 706c 656d 656e 7461 7469 6f6e 732e 2046  plementations. F
-00001a10: 6f72 2065 7861 6d70 6c65 2c0a 0a20 2020  or example,..   
-00001a20: 202e 2e20 636f 6465 3a3a 2070 7974 686f   .. code:: pytho
-00001a30: 6e0a 0a20 2020 2020 2020 6672 6f6d 2061  n..       from a
-00001a40: 7374 726f 7079 2069 6d70 6f72 7420 756e  stropy import un
-00001a50: 6974 7320 6173 2075 0a20 2020 2020 2020  its as u.       
-00001a60: 6672 6f6d 2061 7374 726f 7079 2e63 6f6f  from astropy.coo
-00001a70: 7264 696e 6174 6573 2069 6d70 6f72 7420  rdinates import 
-00001a80: 536b 7943 6f6f 7264 0a0a 2020 2020 2020  SkyCoord..      
-00001a90: 206c 6f61 645f 6669 7473 2822 504f 5353   load_fits("POSS
-00001aa0: 322f 554b 5354 5520 5265 6422 2c0a 2020  2/UKSTU Red",.  
-00001ab0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00001ac0: 6b79 436f 6f72 6428 7261 3d31 3230 202a  kyCoord(ra=120 *
-00001ad0: 2075 2e64 6567 2c20 6465 633d 2d33 3020   u.deg, dec=-30 
-00001ae0: 2a20 752e 6465 6729 2c0a 2020 2020 2020  * u.deg),.      
-00001af0: 2020 2020 2020 2020 2020 2031 3020 2a20             10 * 
-00001b00: 752e 6172 636d 696e 290a 0a20 2020 2069  u.arcmin)..    i
-00001b10: 7320 7468 6520 7361 6d65 2061 730a 0a20  s the same as.. 
-00001b20: 2020 202e 2e20 636f 6465 3a3a 2070 7974     .. code:: pyt
-00001b30: 686f 6e0a 0a20 2020 2020 2020 7375 7276  hon..       surv
-00001b40: 6579 203d 2044 6967 6974 697a 6564 536b  ey = DigitizedSk
-00001b50: 7953 7572 7665 7928 290a 2020 2020 2020  ySurvey().      
-00001b60: 2073 7572 7665 792e 6c6f 6164 5f66 6974   survey.load_fit
-00001b70: 7328 2250 4f53 5332 2f55 4b53 5455 2052  s("POSS2/UKSTU R
-00001b80: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
-00001b90: 2020 2020 2020 2020 2020 2020 2053 6b79               Sky
-00001ba0: 436f 6f72 6428 7261 3d31 3230 202a 2075  Coord(ra=120 * u
-00001bb0: 2e64 6567 2c20 6465 633d 2d33 3020 2a20  .deg, dec=-30 * 
-00001bc0: 752e 6465 6729 2c0a 2020 2020 2020 2020  u.deg),.        
-00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001be0: 3130 202a 2075 2e61 7263 6d69 6e29 0a0a  10 * u.arcmin)..
-00001bf0: 2020 2020 5468 6520 6164 7661 6e74 6167      The advantag
-00001c00: 6520 6f66 2074 6869 7320 6675 6e63 7469  e of this functi
-00001c10: 6f6e 2069 7320 7468 6174 2079 6f75 2064  on is that you d
-00001c20: 6f6e 2774 2068 6176 6520 746f 2072 656d  on't have to rem
-00001c30: 656d 6265 7220 7768 6963 6820 7375 7276  ember which surv
-00001c40: 6579 0a20 2020 2062 656c 6f6e 6773 2074  ey.    belongs t
-00001c50: 6f20 7768 6963 6820 6053 6b79 5375 7276  o which `SkySurv
-00001c60: 6579 6020 696d 706c 656d 656e 7461 7469  ey` implementati
-00001c70: 6f6e 2e20 5468 6520 6469 7361 6476 616e  on. The disadvan
-00001c80: 7461 6765 2069 7320 7468 6174 2074 6865  tage is that the
-00001c90: 0a20 2020 2060 536b 7953 7572 7665 7960  .    `SkySurvey`
-00001ca0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
-00001cb0: 206d 6179 206f 6666 6572 206d 6f72 6520   may offer more 
-00001cc0: 6675 6e63 7469 6f6e 616c 6974 792e 2028  functionality. (
-00001cd0: 5468 6520 6053 6b79 5669 6577 6020 636f  The `SkyView` co
-00001ce0: 6e73 7472 7563 746f 720a 2020 2020 6c65  nstructor.    le
-00001cf0: 7473 2079 6f20 6368 6f6f 7365 2074 6865  ts yo choose the
-00001d00: 2046 4954 5320 696d 6167 6520 7369 7a65   FITS image size
-00001d10: 2069 6e20 7069 7865 6c73 2e29 0a0a 2020   in pixels.)..  
-00001d20: 2020 5365 6520 7468 6520 6053 6b79 5375    See the `SkySu
-00001d30: 7276 6579 6020 696d 706c 656d 656e 7461  rvey` implementa
-00001d40: 7469 6f6e 7320 666f 7220 7468 6520 7375  tions for the su
-00001d50: 7070 6f72 7465 6420 7375 7276 6579 732e  pported surveys.
-00001d60: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00001d70: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00001d80: 2020 2020 7375 7276 6579 3a20 6073 7472      survey: `str
-00001d90: 600a 2020 2020 2020 2020 5468 6520 6e61  `.        The na
-00001da0: 6d65 206f 6620 7468 6520 7375 7276 6579  me of the survey
-00001db0: 2074 6f20 7175 6572 7920 666f 7220 7468   to query for th
-00001dc0: 6520 4649 5453 2066 696c 652e 0a20 2020  e FITS file..   
-00001dd0: 2066 6974 735f 6365 6e74 6572 3a20 607e   fits_center: `~
-00001de0: 6173 7472 6f70 792e 636f 6f72 6469 6e61  astropy.coordina
-00001df0: 7465 732e 536b 7943 6f6f 7264 600a 2020  tes.SkyCoord`.  
-00001e00: 2020 2020 2020 5468 6520 6365 6e74 6572        The center
-00001e10: 2070 6f73 6974 696f 6e20 6f66 2074 6865   position of the
-00001e20: 206c 6f61 6465 6420 4649 5453 2066 696c   loaded FITS fil
-00001e30: 652e 0a20 2020 2073 697a 653a 2060 7e61  e..    size: `~a
-00001e40: 7374 726f 7079 2e63 6f6f 7264 696e 6174  stropy.coordinat
-00001e50: 6573 2e41 6e67 6c65 600a 2020 2020 2020  es.Angle`.      
-00001e60: 2020 5468 6520 7769 6474 6820 616e 6420    The width and 
-00001e70: 6865 6967 6874 206f 6620 7468 6520 4649  height of the FI
-00001e80: 5453 2069 6d61 6765 2c20 6173 2061 6e20  TS image, as an 
-00001e90: 616e 676c 6520 6f6e 2074 6865 2073 6b79  angle on the sky
-00001ea0: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
-00001eb0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2062     -------.    b
-00001ec0: 696e 6172 7920 7374 7265 616d 0a20 2020  inary stream.   
-00001ed0: 2020 2020 2054 6865 2046 4954 5320 6669       The FITS fi
-00001ee0: 6c65 2e0a 2020 2020 6301 0000 0000 0000  le..    c.......
-00001ef0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00001f00: 00f3 1400 0000 6700 7c00 5d06 7d01 7c01  ......g.|.].}.|.
-00001f10: a000 a100 9102 7102 5300 720d 0000 0072  ......q.S.r....r
-00001f20: 1a00 0000 a902 721d 0000 00da 0173 720d  ......r......sr.
-00001f30: 0000 0072 0d00 0000 720e 0000 00da 0a3c  ...r....r......<
-00001f40: 6c69 7374 636f 6d70 3ee9 0000 00f3 0200  listcomp>.......
-00001f50: 0000 1400 7a1d 6c6f 6164 5f66 6974 732e  ....z.load_fits.
-00001f60: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00001f70: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-00001f80: 0200 0000 0400 0000 5300 0000 7254 0000  ........S...rT..
-00001f90: 0072 0d00 0000 721a 0000 0072 5500 0000  .r....r....rU...
-00001fa0: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00001fb0: 5700 0000 eb00 0000 7258 0000 0069 bc02  W.......rX...i..
-00001fc0: 0000 2901 724c 0000 0072 4500 0000 4e29  ..).rL...rE...N)
-00001fd0: 0872 1b00 0000 7222 0000 00da 046b 6579  .r....r".....key
-00001fe0: 7372 1800 0000 724e 0000 0072 4a00 0000  sr....rN...rJ...
-00001ff0: 7247 0000 0072 1600 0000 2904 7210 0000  rG...r....).r...
-00002000: 0072 1100 0000 7212 0000 005a 0773 7572  .r....r....Z.sur
-00002010: 7665 795f 720d 0000 0072 0d00 0000 720e  vey_r....r....r.
-00002020: 0000 0072 1600 0000 bc00 0000 730c 0000  ...r........s...
-00002030: 001a 2d08 011a 010c 010e 020e 0272 1600  ..-..........r..
-00002040: 0000 2915 da02 696f 7202 0000 00da 0674  ..)...ior......t
-00002050: 7970 696e 6772 0300 0000 7204 0000 0072  ypingr....r....r
-00002060: 3c00 0000 da07 6173 7472 6f70 7972 0500  <.....astropyr..
-00002070: 0000 7238 0000 00da 1361 7374 726f 7079  ..r8.....astropy
-00002080: 2e63 6f6f 7264 696e 6174 6573 7206 0000  .coordinatesr...
-00002090: 0072 0700 0000 da0d 4261 7365 4578 6365  .r......BaseExce
-000020a0: 7074 696f 6e72 0800 0000 7222 0000 0072  ptionr....r"...r
-000020b0: 4e00 0000 720f 0000 0072 1800 0000 724a  N...r....r....rJ
-000020c0: 0000 0072 1700 0000 7216 0000 0072 0d00  ...r....r....r..
-000020d0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-000020e0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000020f0: 2e00 0000 0c00 1001 0802 0c01 1001 1003  ................
-00002100: 0207 0201 0201 0201 0201 0201 0201 0201  ................
-00002110: 06f8 020d 0201 0201 06fd 1007 1015 1042  ...............B
-00002120: 1e43                                     .C
+000000d0: 6513 650b 650a 6503 641b 9c04 641c 641d  e.e.e.e.d...d.d.
+000000e0: 8404 5a14 6403 5300 291e e900 0000 0029  ..Z.d.S.)......)
+000000f0: 01da 0742 7974 6573 494f 2902 da08 4269  ...BytesIO)...Bi
+00000100: 6e61 7279 494f da08 5072 6f74 6f63 6f6c  naryIO..Protocol
+00000110: 4e29 01da 0575 6e69 7473 2902 da05 416e  N)...units)...An
+00000120: 676c 65da 0853 6b79 436f 6f72 6463 0000  gle..SkyCoordc..
+00000130: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00000140: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
+00000150: 005a 0264 015a 0364 0253 0029 03da 0b53  .Z.d.Z.d.S.)...S
+00000160: 7572 7665 7945 7272 6f72 7a30 416e 2065  urveyErrorz0An e
+00000170: 7863 6570 7469 6f6e 2061 7269 7369 6e67  xception arising
+00000180: 2077 6865 6e20 7175 6572 7969 6e67 2061   when querying a
+00000190: 2073 6b79 2073 7572 7665 792e 4e29 04da   sky survey.N)..
+000001a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000001b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000001c0: 655f 5fda 075f 5f64 6f63 5f5f a900 720d  e__..__doc__..r.
+000001d0: 0000 0072 0d00 0000 fa41 2f55 7365 7273  ...r.....A/Users
+000001e0: 2f63 6872 6973 7469 616e 2f49 6465 6150  /christian/IdeaP
+000001f0: 726f 6a65 6374 732f 696d 6570 6875 2f73  rojects/imephu/s
+00000200: 7263 2f69 6d65 7068 752f 7365 7276 6963  rc/imephu/servic
+00000210: 652f 7375 7276 6579 2e70 7972 0800 0000  e/survey.pyr....
+00000220: 0900 0000 7304 0000 0008 0104 0272 0800  ....s........r..
+00000230: 0000 5a0e 706f 7373 3275 6b73 7475 5f72  ..Z.poss2ukstu_r
+00000240: 6564 5a0f 706f 7373 3275 6b73 7475 5f62  edZ.poss2ukstu_b
+00000250: 6c75 655a 0d70 6f73 7332 756b 7374 755f  lueZ.poss2ukstu_
+00000260: 6972 5a09 706f 7373 315f 7265 645a 0a70  irZ.poss1_redZ.p
+00000270: 6f73 7331 5f62 6c75 655a 0671 7569 636b  oss1_blueZ.quick
+00000280: 765a 0b70 6861 7365 325f 6773 6332 5a0b  vZ.phase2_gsc2Z.
+00000290: 7068 6173 6532 5f67 7363 3129 087a 0f50  phase2_gsc1).z.P
+000002a0: 4f53 5332 2f55 4b53 5455 2052 6564 7a10  OSS2/UKSTU Redz.
+000002b0: 504f 5353 322f 554b 5354 5520 426c 7565  POSS2/UKSTU Blue
+000002c0: 7a0e 504f 5353 322f 554b 5354 5520 4952  z.POSS2/UKSTU IR
+000002d0: 7a09 504f 5353 3120 5265 647a 0a50 4f53  z.POSS1 Redz.POS
+000002e0: 5331 2042 6c75 657a 0751 7569 636b 2d56  S1 Bluez.Quick-V
+000002f0: 7a11 4853 5420 5068 6173 6532 2028 4753  z.HST Phase2 (GS
+00000300: 4332 297a 1148 5354 2050 6861 7365 3220  C2)z.HST Phase2 
+00000310: 2847 5343 3129 7a07 326d 6173 732d 687a  (GSC1)z.2mass-hz
+00000320: 0732 6d61 7373 2d6a 7a07 326d 6173 732d  .2mass-jz.2mass-
+00000330: 6b29 037a 0732 4d41 5353 2d48 7a07 324d  k).z.2MASS-Hz.2M
+00000340: 4153 532d 4a7a 0732 4d41 5353 2d4b 6300  ASS-Jz.2MASS-Kc.
+00000350: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+00000360: 0000 0040 0000 0073 2400 0000 6500 5a01  ...@...s$...e.Z.
+00000370: 6400 5a02 6401 5a03 6504 6505 6506 6507  d.Z.d.Z.e.e.e.e.
+00000380: 6402 9c04 6403 6404 8404 5a08 6405 5300  d...d.d...Z.d.S.
+00000390: 2906 da09 536b 7953 7572 7665 797a 3441  )...SkySurveyz4A
+000003a0: 2073 6b79 2073 7572 7665 7920 6672 6f6d   sky survey from
+000003b0: 2077 6869 6368 2066 6974 7320 6669 6c65   which fits file
+000003c0: 7320 6361 6e20 6265 2072 6571 7565 7374  s can be request
+000003d0: 6564 2ea9 04da 0673 7572 7665 79da 0b66  ed.....survey..f
+000003e0: 6974 735f 6365 6e74 6572 da04 7369 7a65  its_center..size
+000003f0: da06 7265 7475 726e 6304 0000 0000 0000  ..returnc.......
+00000400: 0000 0000 0004 0000 0001 0000 0043 0000  .............C..
+00000410: 0073 0800 0000 7400 8201 6401 5300 2902  .s....t...d.S.).
+00000420: 6129 0200 004c 6f61 6420 6120 4649 5453  a)...Load a FITS
+00000430: 2066 696c 6520 666f 7220 6120 6769 7665   file for a give
+00000440: 6e20 706f 7369 7469 6f6e 2066 726f 6d20  n position from 
+00000450: 7468 6520 736b 7920 7375 7276 6579 2e0a  the sky survey..
+00000460: 0a20 2020 2020 2020 2054 6865 2073 697a  .        The siz
+00000470: 6520 6f66 2074 6865 2072 6574 7572 6e65  e of the returne
+00000480: 6420 4649 5453 2066 696c 6520 6973 2064  d FITS file is d
+00000490: 6574 6572 6d69 6e65 6420 6279 2074 6865  etermined by the
+000004a0: 2063 6c61 7373 2069 6d70 6c65 6d65 6e74   class implement
+000004b0: 696e 6720 7468 6973 0a20 2020 2020 2020  ing this.       
+000004c0: 2070 726f 746f 636f 6c20 286f 7220 7468   protocol (or th
+000004d0: 6520 7765 6220 7365 7276 6963 6520 7573  e web service us
+000004e0: 6564 292e 0a0a 2020 2020 2020 2020 5061  ed)...        Pa
+000004f0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00000500: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00000510: 2020 2020 7375 7276 6579 3a20 6073 7472      survey: `str
+00000520: 600a 2020 2020 2020 2020 2020 2020 5468  `.            Th
+00000530: 6520 6e61 6d65 206f 6620 7468 6520 7375  e name of the su
+00000540: 7276 6579 2074 6f20 7175 6572 7920 666f  rvey to query fo
+00000550: 7220 7468 6520 4649 5453 2066 696c 652e  r the FITS file.
+00000560: 0a20 2020 2020 2020 2066 6974 735f 6365  .        fits_ce
+00000570: 6e74 6572 3a20 607e 6173 7472 6f70 792e  nter: `~astropy.
+00000580: 636f 6f72 6469 6e61 7465 732e 536b 7943  coordinates.SkyC
+00000590: 6f6f 7264 600a 2020 2020 2020 2020 2020  oord`.          
+000005a0: 2020 5468 6520 6365 6e74 6572 2070 6f73    The center pos
+000005b0: 6974 696f 6e20 6f66 2074 6865 206c 6f61  ition of the loa
+000005c0: 6465 6420 4649 5453 2066 696c 652e 0a20  ded FITS file.. 
+000005d0: 2020 2020 2020 2073 697a 653a 2060 7e61         size: `~a
+000005e0: 7374 726f 7079 2e63 6f6f 7264 696e 6174  stropy.coordinat
+000005f0: 6573 2e41 6e67 6c65 600a 2020 2020 2020  es.Angle`.      
+00000600: 2020 2020 2020 5468 6520 7769 6474 6820        The width 
+00000610: 616e 6420 6865 6967 6874 206f 6620 7468  and height of th
+00000620: 6520 4649 5453 2069 6d61 6765 2c20 6173  e FITS image, as
+00000630: 2061 6e20 616e 676c 6520 6f6e 2074 6865   an angle on the
+00000640: 2073 6b79 2e0a 2020 2020 2020 2020 4e29   sky..        N)
+00000650: 01da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
+00000660: 6445 7272 6f72 2904 da04 7365 6c66 7211  dError)...selfr.
+00000670: 0000 0072 1200 0000 7213 0000 0072 0d00  ...r....r....r..
+00000680: 0000 720d 0000 0072 0e00 0000 da09 6c6f  ..r....r......lo
+00000690: 6164 5f66 6974 7325 0000 0073 0200 0000  ad_fits%...s....
+000006a0: 000f 7a13 536b 7953 7572 7665 792e 6c6f  ..z.SkySurvey.lo
+000006b0: 6164 5f66 6974 734e 2909 7209 0000 0072  ad_fitsN).r....r
+000006c0: 0a00 0000 720b 0000 0072 0c00 0000 da03  ....r....r......
+000006d0: 7374 7272 0700 0000 7206 0000 0072 0300  strr....r....r..
+000006e0: 0000 7217 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+000006f0: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000700: 2200 0000 7304 0000 0008 0104 0272 0f00  "...s........r..
+00000710: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000720: 0000 0005 0000 0040 0000 0073 4200 0000  .......@...sB...
+00000730: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
+00000740: 9c01 6404 6405 8404 5a04 6505 6506 6507  ..d.d...Z.e.e.e.
+00000750: 6508 6406 9c04 6407 6408 8404 5a09 6505  e.d...d.d...Z.e.
+00000760: 6505 6409 9c02 640a 640b 8404 5a0a 6402  e.d...d.d...Z.d.
+00000770: 5300 290c da12 4469 6769 7469 7a65 6453  S.)...DigitizedS
+00000780: 6b79 5375 7276 6579 7aac 4120 636c 6173  kySurveyz.A clas
+00000790: 7320 666f 7220 6c6f 6164 696e 6720 4649  s for loading FI
+000007a0: 5453 2066 696c 6573 2066 726f 6d20 7468  TS files from th
+000007b0: 6520 4469 6769 7469 7a65 6420 536b 7920  e Digitized Sky 
+000007c0: 5375 7276 6579 2028 4453 5329 2e0a 0a20  Survey (DSS)... 
+000007d0: 2020 2053 6565 2074 6865 2060 4453 5320     See the `DSS 
+000007e0: 6172 6368 6976 6520 7765 6273 6974 6520  archive website 
+000007f0: 3c68 7474 7073 3a2f 2f61 7263 6869 7665  <https://archive
+00000800: 2e73 7473 6369 2e65 6475 2f64 7373 2f69  .stsci.edu/dss/i
+00000810: 6e64 6578 2e68 746d 6c3e 6020 666f 7220  ndex.html>` for 
+00000820: 6d6f 7265 0a20 2020 2064 6574 6169 6c73  more.    details
+00000830: 2e0a 2020 2020 4e29 0172 1400 0000 6301  ..    N).r....c.
+00000840: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000850: 0000 0043 0000 0073 1800 0000 6401 6402  ...C...s....d.d.
+00000860: 8400 7400 a001 a100 4400 8301 7c00 5f02  ..t.....D...|._.
+00000870: 6400 5300 2903 4e63 0100 0000 0000 0000  d.S.).Nc........
+00000880: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
+00000890: 731a 0000 0069 007c 005d 125c 027d 017d  s....i.|.].\.}.}
+000008a0: 027c 01a0 00a1 007c 0293 0271 0453 0072  .|.....|...q.S.r
+000008b0: 0d00 0000 a901 da05 6c6f 7765 72a9 03da  ........lower...
+000008c0: 022e 30da 036b 6579 da05 7661 6c75 6572  ..0..key..valuer
+000008d0: 0d00 0000 720d 0000 0072 0e00 0000 da0a  ....r....r......
+000008e0: 3c64 6963 7463 6f6d 703e 3f00 0000 7306  <dictcomp>?...s.
+000008f0: 0000 0006 0106 0006 007a 2f44 6967 6974  .........z/Digit
+00000900: 697a 6564 536b 7953 7572 7665 792e 5f5f  izedSkySurvey.__
+00000910: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00000920: 3c64 6963 7463 6f6d 703e 2903 da10 5f44  <dictcomp>)..._D
+00000930: 5353 5f49 4445 4e54 4946 4945 5253 da05  SS_IDENTIFIERS..
+00000940: 6974 656d 73da 135f 7375 7276 6579 5f69  items.._survey_i
+00000950: 6465 6e74 6966 6965 7273 2901 7216 0000  dentifiers).r...
+00000960: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00000970: da08 5f5f 696e 6974 5f5f 3e00 0000 7306  ..__init__>...s.
+00000980: 0000 0000 0106 0106 ff7a 1b44 6967 6974  .........z.Digit
+00000990: 697a 6564 536b 7953 7572 7665 792e 5f5f  izedSkySurvey.__
+000009a0: 696e 6974 5f5f 7210 0000 0063 0400 0000  init__r....c....
+000009b0: 0000 0000 0000 0000 0700 0000 0900 0000  ................
+000009c0: 4300 0000 736e 0000 0064 017d 047c 00a0  C...sn...d.}.|..
+000009d0: 007c 01a1 017c 026a 01a0 0274 036a 04a1  .|...|.j...t.j..
+000009e0: 017c 026a 05a0 0274 036a 04a1 0164 027c  .|.j...t.j...d.|
+000009f0: 03a0 0274 036a 06a1 017c 03a0 0274 036a  ...t.j...|...t.j
+00000a00: 06a1 0164 0364 0464 059c 087d 0574 076a  ...d.d.d...}.t.j
+00000a10: 087c 047c 0564 068d 027d 067c 066a 0964  .|.|.d...}.|.j.d
+00000a20: 076b 0372 6474 0a64 0883 0182 0174 0b7c  .k.rdt.d.....t.|
+00000a30: 066a 0c83 0153 0029 0961 7203 0000 4c6f  .j...S.).ar...Lo
+00000a40: 6164 2061 2046 4954 5320 6669 6c65 2066  ad a FITS file f
+00000a50: 6f72 2061 2067 6976 656e 2070 6f73 6974  or a given posit
+00000a60: 696f 6e20 6672 6f6d 2074 6865 2073 6b79  ion from the sky
+00000a70: 2073 7572 7665 792e 0a0a 2020 2020 2020   survey...      
+00000a80: 2020 5468 6520 666f 6c6c 6f77 696e 6720    The following 
+00000a90: 7375 7276 6579 7320 6361 6e20 6265 2071  surveys can be q
+00000aa0: 7565 7269 6564 2066 6f72 2046 4954 5320  ueried for FITS 
+00000ab0: 696d 6167 6573 3a0a 0a20 2020 2020 2020  images:..       
+00000ac0: 202d 2050 4f53 5332 2f55 4b53 5455 2052   - POSS2/UKSTU R
+00000ad0: 6564 0a20 2020 2020 2020 202d 2050 4f53  ed.        - POS
+00000ae0: 5332 2f55 4b53 5455 2042 6c75 650a 2020  S2/UKSTU Blue.  
+00000af0: 2020 2020 2020 2d20 504f 5353 322f 554b        - POSS2/UK
+00000b00: 5354 5520 4952 0a20 2020 2020 2020 202d  STU IR.        -
+00000b10: 2050 4f53 5331 2052 6564 0a20 2020 2020   POSS1 Red.     
+00000b20: 2020 202d 2050 4f53 5331 2042 6c75 650a     - POSS1 Blue.
+00000b30: 2020 2020 2020 2020 2d20 5175 6963 6b2d          - Quick-
+00000b40: 560a 2020 2020 2020 2020 2d20 4853 5420  V.        - HST 
+00000b50: 5068 6173 6532 2028 4753 4332 290a 2020  Phase2 (GSC2).  
+00000b60: 2020 2020 2020 2d20 4853 5420 5068 6173        - HST Phas
+00000b70: 6532 2028 4753 4331 290a 0a20 2020 2020  e2 (GSC1)..     
+00000b80: 2020 2053 6565 2074 6865 2060 4453 5320     See the `DSS 
+00000b90: 7375 7276 6579 2070 6167 6520 3c68 7474  survey page <htt
+00000ba0: 703a 2f2f 6773 7373 2e73 7473 6369 2e65  p://gsss.stsci.e
+00000bb0: 6475 2f53 6b79 5375 7276 6579 732f 5375  du/SkySurveys/Su
+00000bc0: 7276 6579 732e 6874 6d3e 6020 666f 720a  rveys.htm>` for.
+00000bd0: 2020 2020 2020 2020 6465 7461 696c 7320          details 
+00000be0: 6162 6f75 7420 7468 6573 6520 7375 7276  about these surv
+00000bf0: 6579 732e 0a0a 2020 2020 2020 2020 5061  eys...        Pa
+00000c00: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00000c10: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00000c20: 2020 2020 7375 7276 6579 3a20 6073 7472      survey: `str
+00000c30: 600a 2020 2020 2020 2020 2020 2020 5468  `.            Th
+00000c40: 6520 6e61 6d65 206f 6620 7468 6520 7375  e name of the su
+00000c50: 7276 6579 2074 6f20 7175 6572 7920 666f  rvey to query fo
+00000c60: 7220 7468 6520 4649 5453 2066 696c 652e  r the FITS file.
+00000c70: 0a20 2020 2020 2020 2066 6974 735f 6365  .        fits_ce
+00000c80: 6e74 6572 3a20 607e 6173 7472 6f70 792e  nter: `~astropy.
+00000c90: 636f 6f72 6469 6e61 7465 732e 536b 7943  coordinates.SkyC
+00000ca0: 6f6f 7264 600a 2020 2020 2020 2020 2020  oord`.          
+00000cb0: 2020 5468 6520 6365 6e74 6572 2070 6f73    The center pos
+00000cc0: 6974 696f 6e20 6f66 2074 6865 206c 6f61  ition of the loa
+00000cd0: 6465 6420 4649 5453 2066 696c 652e 0a20  ded FITS file.. 
+00000ce0: 2020 2020 2020 2073 697a 653a 2060 7e61         size: `~a
+00000cf0: 7374 726f 7079 2e63 6f6f 7264 696e 6174  stropy.coordinat
+00000d00: 6573 2e41 6e67 6c65 600a 2020 2020 2020  es.Angle`.      
+00000d10: 2020 2020 2020 5468 6520 7769 6474 6820        The width 
+00000d20: 616e 6420 6865 6967 6874 206f 6620 7468  and height of th
+00000d30: 6520 4649 5453 2069 6d61 6765 2c20 6173  e FITS image, as
+00000d40: 2061 6e20 616e 676c 6520 6f6e 2074 6865   an angle on the
+00000d50: 2073 6b79 2e0a 0a20 2020 2020 2020 2052   sky...        R
+00000d60: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00000d70: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2062  ------.        b
+00000d80: 696e 6172 7920 7374 7265 616d 0a20 2020  inary stream.   
+00000d90: 2020 2020 2020 2020 2054 6865 2046 4954           The FIT
+00000da0: 5320 6669 6c65 2e0a 2020 2020 2020 2020  S file..        
+00000db0: 7a2c 6874 7470 733a 2f2f 6172 6368 6976  z,https://archiv
+00000dc0: 652e 7374 7363 692e 6564 752f 6367 692d  e.stsci.edu/cgi-
+00000dd0: 6269 6e2f 6473 735f 7365 6172 6368 da05  bin/dss_search..
+00000de0: 4a32 3030 30da 0466 6974 73da 046e 6f6e  J2000..fits..non
+00000df0: 6529 08da 0176 da01 72da 0164 da01 65da  e)...v..r..d..e.
+00000e00: 0168 da01 77da 0166 da01 63a9 01da 0670  .h..w..f..c....p
+00000e10: 6172 616d 73e9 c800 0000 fa1d 4e6f 2046  arams.......No F
+00000e20: 4954 5320 6669 6c65 2063 6f75 6c64 2062  ITS file could b
+00000e30: 6520 6c6f 6164 6564 2e29 0dda 125f 7375  e loaded.)..._su
+00000e40: 7276 6579 5f69 6465 6e74 6966 6965 72da  rvey_identifier.
+00000e50: 0272 61da 0874 6f5f 7661 6c75 65da 0175  .ra..to_value..u
+00000e60: da03 6465 67da 0364 6563 da06 6172 636d  ..deg..dec..arcm
+00000e70: 696e da08 7265 7175 6573 7473 da03 6765  in..requests..ge
+00000e80: 74da 0b73 7461 7475 735f 636f 6465 7208  t..status_coder.
+00000e90: 0000 0072 0200 0000 da07 636f 6e74 656e  ...r......conten
+00000ea0: 74a9 0772 1600 0000 7211 0000 0072 1200  t..r....r....r..
+00000eb0: 0000 7213 0000 00da 0375 726c 7231 0000  ..r......urlr1..
+00000ec0: 00da 0872 6573 706f 6e73 6572 0d00 0000  ...responser....
+00000ed0: 720d 0000 0072 0e00 0000 7217 0000 0043  r....r....r....C
+00000ee0: 0000 0073 1c00 0000 001f 0402 0801 0c01  ...s............
+00000ef0: 0c01 0201 0a01 0a01 0201 02f8 060a 0e01  ................
+00000f00: 0a01 0801 7a1c 4469 6769 7469 7a65 6453  ....z.DigitizedS
+00000f10: 6b79 5375 7276 6579 2e6c 6f61 645f 6669  kySurvey.load_fi
+00000f20: 7473 a902 7211 0000 0072 1400 0000 6302  ts..r....r....c.
+00000f30: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00000f40: 0000 0043 0000 0073 2a00 0000 7c01 a000  ...C...s*...|...
+00000f50: a100 7c00 6a01 6b07 721c 7402 6401 7c01  ..|.j.k.r.t.d.|.
+00000f60: 9b00 9d02 8301 8201 7c00 6a01 7c01 a000  ........|.j.|...
+00000f70: a100 1900 5300 a902 4efa 1055 6e6b 6e6f  ....S...N..Unkno
+00000f80: 776e 2073 7572 7665 793a 20a9 0372 1b00  wn survey: ..r..
+00000f90: 0000 7223 0000 00da 0a56 616c 7565 4572  ..r#.....ValueEr
+00000fa0: 726f 72a9 0272 1600 0000 7211 0000 0072  ror..r....r....r
+00000fb0: 0d00 0000 720d 0000 0072 0e00 0000 7234  ....r....r....r4
+00000fc0: 0000 0072 0000 0073 0600 0000 0001 0e01  ...r...s........
+00000fd0: 0e02 7a25 4469 6769 7469 7a65 6453 6b79  ..z%DigitizedSky
+00000fe0: 5375 7276 6579 2e5f 7375 7276 6579 5f69  Survey._survey_i
+00000ff0: 6465 6e74 6966 6965 7229 0b72 0900 0000  dentifier).r....
+00001000: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00001010: 2400 0000 7218 0000 0072 0700 0000 7206  $...r....r....r.
+00001020: 0000 0072 0300 0000 7217 0000 0072 3400  ...r....r....r4.
+00001030: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00001040: 0072 0e00 0000 7219 0000 0037 0000 0073  .r....r....7...s
+00001050: 0800 0000 0801 0406 0e05 142f 7219 0000  .........../r...
+00001060: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001070: 0000 0500 0000 4000 0000 7346 0000 0065  ......@...sF...e
+00001080: 005a 0164 005a 0264 015a 0364 0d65 0464  .Z.d.Z.d.Z.d.e.d
+00001090: 0364 049c 0264 0564 0684 055a 0565 0665  .d...d.d...Z.e.e
+000010a0: 0765 0865 0964 079c 0464 0864 0984 045a  .e.e.d...d.d...Z
+000010b0: 0a65 0665 0664 0a9c 0264 0b64 0c84 045a  .e.e.d...d.d...Z
+000010c0: 0b64 0353 0029 0eda 0753 6b79 5669 6577  .d.S.)...SkyView
+000010d0: 610b 0100 0041 2063 6c61 7373 2066 6f72  a....A class for
+000010e0: 206c 6f61 6469 6e67 2046 4954 5320 6669   loading FITS fi
+000010f0: 6c65 7320 6672 6f6d 2053 6b79 5669 6577  les from SkyView
+00001100: 2e0a 0a20 2020 2053 6565 2074 6865 2060  ...    See the `
+00001110: 536b 7956 6965 7720 7369 7465 203c 6874  SkyView site <ht
+00001120: 7470 733a 2f2f 736b 7976 6965 772e 6773  tps://skyview.gs
+00001130: 6663 2e6e 6173 612e 676f 762f 6375 7272  fc.nasa.gov/curr
+00001140: 656e 742f 6367 692f 7469 746c 6570 6167  ent/cgi/titlepag
+00001150: 652e 706c 3e60 2066 6f72 0a20 2020 206d  e.pl>` for.    m
+00001160: 6f72 6520 6465 7461 696c 7320 6162 6f75  ore details abou
+00001170: 7420 536b 7956 6965 772e 0a0a 2020 2020  t SkyView...    
+00001180: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00001190: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7069  ---------.    pi
+000011a0: 7865 6c73 3a20 6069 6e74 602c 2064 6566  xels: `int`, def
+000011b0: 6175 6c74 3a20 3330 300a 2020 2020 2020  ault: 300.      
+000011c0: 2020 5468 6520 696d 6167 6520 7369 7a65    The image size
+000011d0: 2069 6e20 7069 7865 6c73 2e0a 2020 2020   in pixels..    
+000011e0: e92c 0100 004e 2902 da06 7069 7865 6c73  .,...N)...pixels
+000011f0: 7214 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00001200: 0000 0200 0000 0300 0000 4300 0000 731e  ..........C...s.
+00001210: 0000 007c 017c 005f 0064 0164 0284 0074  ...|.|._.d.d...t
+00001220: 01a0 02a1 0044 0083 017c 005f 0364 0053  .....D...|._.d.S
+00001230: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00001240: 0003 0000 0004 0000 0053 0000 0073 1a00  .........S...s..
+00001250: 0000 6900 7c00 5d12 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
+00001260: a000 a100 7c02 9302 7104 5300 720d 0000  ....|...q.S.r...
+00001270: 0072 1a00 0000 721c 0000 0072 0d00 0000  .r....r....r....
+00001280: 720d 0000 0072 0e00 0000 7220 0000 0087  r....r....r ....
+00001290: 0000 0073 0600 0000 0601 0600 0600 7a24  ...s..........z$
+000012a0: 536b 7956 6965 772e 5f5f 696e 6974 5f5f  SkyView.__init__
+000012b0: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+000012c0: 6f6d 703e 2904 da07 5f70 6978 656c 73da  omp>)..._pixels.
+000012d0: 145f 534b 5956 4945 575f 4944 454e 5449  ._SKYVIEW_IDENTI
+000012e0: 4649 4552 5372 2200 0000 7223 0000 0029  FIERSr"...r#...)
+000012f0: 0272 1600 0000 724a 0000 0072 0d00 0000  .r....rJ...r....
+00001300: 720d 0000 0072 0e00 0000 7224 0000 0085  r....r....r$....
+00001310: 0000 0073 0800 0000 0001 0601 0601 06ff  ...s............
+00001320: 7a10 536b 7956 6965 772e 5f5f 696e 6974  z.SkyView.__init
+00001330: 5f5f 7210 0000 0063 0400 0000 0000 0000  __r....c........
+00001340: 0000 0000 0700 0000 0800 0000 4300 0000  ............C...
+00001350: 736e 0000 0064 017d 047c 026a 00a0 0174  sn...d.}.|.j...t
+00001360: 026a 03a1 019b 0064 027c 026a 04a0 0174  .j.....d.|.j...t
+00001370: 026a 03a1 019b 009d 037c 00a0 057c 01a1  .j.......|...|..
+00001380: 0164 0364 047c 006a 067c 03a0 0174 026a  .d.d.|.j.|...t.j
+00001390: 03a1 0164 059c 067d 0574 076a 087c 047c  ...d...}.t.j.|.|
+000013a0: 0564 068d 027d 067c 066a 0964 076b 0372  .d...}.|.j.d.k.r
+000013b0: 6474 0a64 0883 0182 0174 0b7c 066a 0c83  dt.d.....t.|.j..
+000013c0: 0153 0029 0961 0903 0000 4c6f 6164 2061  .S.).a....Load a
+000013d0: 2046 4954 5320 6669 6c65 2066 6f72 2061   FITS file for a
+000013e0: 2067 6976 656e 2070 6f73 6974 696f 6e20   given position 
+000013f0: 6672 6f6d 2074 6865 2073 6b79 2073 7572  from the sky sur
+00001400: 7665 792e 0a0a 2020 2020 2020 2020 5468  vey...        Th
+00001410: 6520 666f 6c6c 6f77 696e 6720 7375 6273  e following subs
+00001420: 6574 206f 6620 7375 7276 6579 7320 7375  et of surveys su
+00001430: 7070 6f72 7465 6420 6279 2053 6b79 5669  pported by SkyVi
+00001440: 6577 2063 616e 2062 6520 7175 6572 6965  ew can be querie
+00001450: 643a 0a0a 2020 2020 2020 2020 2d20 324d  d:..        - 2M
+00001460: 4153 532d 480a 2020 2020 2020 2020 2d20  ASS-H.        - 
+00001470: 324d 4153 532d 4a0a 2020 2020 2020 2020  2MASS-J.        
+00001480: 2d20 324d 4153 532d 4b0a 0a20 2020 2020  - 2MASS-K..     
+00001490: 2020 2053 6565 2074 6865 2060 536b 7956     See the `SkyV
+000014a0: 6965 7720 7375 7276 6579 2070 6167 650a  iew survey page.
+000014b0: 2020 2020 2020 2020 3c68 7474 7073 3a2f          <https:/
+000014c0: 2f73 6b79 7669 6577 2e67 7366 632e 6e61  /skyview.gsfc.na
+000014d0: 7361 2e67 6f76 2f63 7572 7265 6e74 2f63  sa.gov/current/c
+000014e0: 6769 2f73 7572 7665 792e 706c 3e60 2066  gi/survey.pl>` f
+000014f0: 6f72 2064 6574 6169 6c73 2061 626f 7574  or details about
+00001500: 2074 6865 7365 0a20 2020 2020 2020 2073   these.        s
+00001510: 7572 7665 7973 2e0a 0a20 2020 2020 2020  urveys...       
+00001520: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00001530: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00001540: 2020 2020 2020 2073 7572 7665 793a 2060         survey: `
+00001550: 7374 7260 0a20 2020 2020 2020 2020 2020  str`.           
+00001560: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00001570: 2073 7572 7665 7920 746f 2071 7565 7279   survey to query
+00001580: 2066 6f72 2074 6865 2046 4954 5320 6669   for the FITS fi
+00001590: 6c65 2e0a 2020 2020 2020 2020 6669 7473  le..        fits
+000015a0: 5f63 656e 7465 723a 2060 7e61 7374 726f  _center: `~astro
+000015b0: 7079 2e63 6f6f 7264 696e 6174 6573 2e53  py.coordinates.S
+000015c0: 6b79 436f 6f72 6460 0a20 2020 2020 2020  kyCoord`.       
+000015d0: 2020 2020 2054 6865 2063 656e 7465 7220       The center 
+000015e0: 706f 7369 7469 6f6e 206f 6620 7468 6520  position of the 
+000015f0: 6c6f 6164 6564 2046 4954 5320 6669 6c65  loaded FITS file
+00001600: 2e0a 2020 2020 2020 2020 7369 7a65 3a20  ..        size: 
+00001610: 607e 6173 7472 6f70 792e 636f 6f72 6469  `~astropy.coordi
+00001620: 6e61 7465 732e 416e 676c 6560 0a20 2020  nates.Angle`.   
+00001630: 2020 2020 2020 2020 2054 6865 2077 6964           The wid
+00001640: 7468 2061 6e64 2068 6569 6768 7420 6f66  th and height of
+00001650: 2074 6865 2046 4954 5320 696d 6167 652c   the FITS image,
+00001660: 2061 7320 616e 2061 6e67 6c65 206f 6e20   as an angle on 
+00001670: 7468 6520 736b 792e 0a0a 2020 2020 2020  the sky...      
+00001680: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00001690: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000016a0: 2020 6269 6e61 7279 2073 7472 6561 6d0a    binary stream.
+000016b0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000016c0: 4649 5453 2066 696c 652e 0a20 2020 2020  FITS file..     
+000016d0: 2020 207a 3568 7474 7073 3a2f 2f73 6b79     z5https://sky
+000016e0: 7669 6577 2e67 7366 632e 6e61 7361 2e67  view.gsfc.nasa.g
+000016f0: 6f76 2f63 7572 7265 6e74 2f63 6769 2f72  ov/current/cgi/r
+00001700: 756e 7175 6572 792e 706c 7a02 2c20 da04  unquery.plz., ..
+00001710: 4943 5253 da04 4649 5453 2906 5a08 506f  ICRS..FITS).Z.Po
+00001720: 7369 7469 6f6e 5a06 5375 7276 6579 5a0b  sitionZ.SurveyZ.
+00001730: 436f 6f72 6469 6e61 7465 73da 0652 6574  Coordinates..Ret
+00001740: 7572 6e5a 0650 6978 656c 73da 0453 697a  urnZ.Pixels..Siz
+00001750: 6572 3000 0000 7232 0000 0072 3300 0000  er0...r2...r3...
+00001760: 290d 7235 0000 0072 3600 0000 7237 0000  ).r5...r6...r7..
+00001770: 0072 3800 0000 7239 0000 0072 3400 0000  .r8...r9...r4...
+00001780: 724b 0000 0072 3b00 0000 723c 0000 0072  rK...r;...r<...r
+00001790: 3d00 0000 7208 0000 0072 0200 0000 723e  =...r....r....r>
+000017a0: 0000 0072 3f00 0000 720d 0000 0072 0d00  ...r?...r....r..
+000017b0: 0000 720e 0000 0072 1700 0000 8b00 0000  ..r....r........
+000017c0: 7318 0000 0000 1b04 0220 0208 0102 0102  s........ ......
+000017d0: 0104 010a f906 090e 010a 0108 017a 1153  .............z.S
+000017e0: 6b79 5669 6577 2e6c 6f61 645f 6669 7473  kyView.load_fits
+000017f0: 7242 0000 0063 0200 0000 0000 0000 0000  rB...c..........
+00001800: 0000 0200 0000 0300 0000 4300 0000 732a  ..........C...s*
+00001810: 0000 007c 01a0 00a1 007c 006a 016b 0772  ...|.....|.j.k.r
+00001820: 1c74 0264 017c 019b 009d 0283 0182 017c  .t.d.|.........|
+00001830: 006a 017c 01a0 00a1 0019 0053 0072 4300  .j.|.......S.rC.
+00001840: 0000 7245 0000 0072 4700 0000 720d 0000  ..rE...rG...r...
+00001850: 0072 0d00 0000 720e 0000 0072 3400 0000  .r....r....r4...
+00001860: b500 0000 7306 0000 0000 010e 010e 027a  ....s..........z
+00001870: 1a53 6b79 5669 6577 2e5f 7375 7276 6579  .SkyView._survey
+00001880: 5f69 6465 6e74 6966 6965 7229 0172 4900  _identifier).rI.
+00001890: 0000 290c 7209 0000 0072 0a00 0000 720b  ..).r....r....r.
+000018a0: 0000 0072 0c00 0000 da03 696e 7472 2400  ...r......intr$.
+000018b0: 0000 7218 0000 0072 0700 0000 7206 0000  ..r....r....r...
+000018c0: 0072 0300 0000 7217 0000 0072 3400 0000  .r....r....r4...
+000018d0: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+000018e0: 0e00 0000 7248 0000 0079 0000 0073 0800  ....rH...y...s..
+000018f0: 0000 0801 040b 1206 142a 7248 0000 0072  .........*rH...r
+00001900: 1000 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00001910: 0004 0000 0005 0000 0043 0000 0073 6400  .........C...sd.
+00001920: 0000 7c00 a000 a100 6401 6402 8400 7401  ..|.....d.d...t.
+00001930: a002 a100 4400 8301 6b06 7222 7403 8300  ....D...k.r"t...
+00001940: 7d03 6e34 7c00 a000 a100 6403 6402 8400  }.n4|.....d.d...
+00001950: 7404 a002 a100 4400 8301 6b06 7248 7405  t.....D...k.rHt.
+00001960: 6404 6405 8d01 7d03 6e0e 7406 6406 7c00  d.d...}.n.t.d.|.
+00001970: 9b00 9d02 8301 8201 7c03 a007 7c00 7c01  ........|...|.|.
+00001980: 7c02 a103 5300 2907 6173 0500 0052 6571  |...S.).as...Req
+00001990: 7565 7374 2061 2046 4954 5320 696d 6167  uest a FITS imag
+000019a0: 6520 6672 6f6d 2061 2073 6b79 2073 7572  e from a sky sur
+000019b0: 7665 792e 0a0a 2020 2020 496e 2070 7269  vey...    In pri
+000019c0: 6e63 6970 6c65 2c20 7468 6973 2066 756e  nciple, this fun
+000019d0: 6374 696f 6e20 6973 2065 7175 6976 616c  ction is equival
+000019e0: 656e 7420 746f 2074 6865 2060 6c6f 6164  ent to the `load
+000019f0: 5f66 6974 7360 206d 6574 686f 6473 206f  _fits` methods o
+00001a00: 6620 7468 650a 2020 2020 6053 6b79 5375  f the.    `SkySu
+00001a10: 7276 6579 6020 696d 706c 656d 656e 7461  rvey` implementa
+00001a20: 7469 6f6e 732e 2046 6f72 2065 7861 6d70  tions. For examp
+00001a30: 6c65 2c0a 0a20 2020 202e 2e20 636f 6465  le,..    .. code
+00001a40: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
+00001a50: 2020 6672 6f6d 2061 7374 726f 7079 2069    from astropy i
+00001a60: 6d70 6f72 7420 756e 6974 7320 6173 2075  mport units as u
+00001a70: 0a20 2020 2020 2020 6672 6f6d 2061 7374  .       from ast
+00001a80: 726f 7079 2e63 6f6f 7264 696e 6174 6573  ropy.coordinates
+00001a90: 2069 6d70 6f72 7420 536b 7943 6f6f 7264   import SkyCoord
+00001aa0: 0a0a 2020 2020 2020 206c 6f61 645f 6669  ..       load_fi
+00001ab0: 7473 2822 504f 5353 322f 554b 5354 5520  ts("POSS2/UKSTU 
+00001ac0: 5265 6422 2c0a 2020 2020 2020 2020 2020  Red",.          
+00001ad0: 2020 2020 2020 2053 6b79 436f 6f72 6428         SkyCoord(
+00001ae0: 7261 3d31 3230 202a 2075 2e64 6567 2c20  ra=120 * u.deg, 
+00001af0: 6465 633d 2d33 3020 2a20 752e 6465 6729  dec=-30 * u.deg)
+00001b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001b10: 2020 2031 3020 2a20 752e 6172 636d 696e     10 * u.arcmin
+00001b20: 290a 0a20 2020 2069 7320 7468 6520 7361  )..    is the sa
+00001b30: 6d65 2061 730a 0a20 2020 202e 2e20 636f  me as..    .. co
+00001b40: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
+00001b50: 2020 2020 7375 7276 6579 203d 2044 6967      survey = Dig
+00001b60: 6974 697a 6564 536b 7953 7572 7665 7928  itizedSkySurvey(
+00001b70: 290a 2020 2020 2020 2073 7572 7665 792e  ).       survey.
+00001b80: 6c6f 6164 5f66 6974 7328 2250 4f53 5332  load_fits("POSS2
+00001b90: 2f55 4b53 5455 2052 6564 222c 0a20 2020  /UKSTU Red",.   
+00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bb0: 2020 2020 2053 6b79 436f 6f72 6428 7261       SkyCoord(ra
+00001bc0: 3d31 3230 202a 2075 2e64 6567 2c20 6465  =120 * u.deg, de
+00001bd0: 633d 2d33 3020 2a20 752e 6465 6729 2c0a  c=-30 * u.deg),.
+00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bf0: 2020 2020 2020 2020 3130 202a 2075 2e61          10 * u.a
+00001c00: 7263 6d69 6e29 0a0a 2020 2020 5468 6520  rcmin)..    The 
+00001c10: 6164 7661 6e74 6167 6520 6f66 2074 6869  advantage of thi
+00001c20: 7320 6675 6e63 7469 6f6e 2069 7320 7468  s function is th
+00001c30: 6174 2079 6f75 2064 6f6e 2774 2068 6176  at you don't hav
+00001c40: 6520 746f 2072 656d 656d 6265 7220 7768  e to remember wh
+00001c50: 6963 6820 7375 7276 6579 0a20 2020 2062  ich survey.    b
+00001c60: 656c 6f6e 6773 2074 6f20 7768 6963 6820  elongs to which 
+00001c70: 6053 6b79 5375 7276 6579 6020 696d 706c  `SkySurvey` impl
+00001c80: 656d 656e 7461 7469 6f6e 2e20 5468 6520  ementation. The 
+00001c90: 6469 7361 6476 616e 7461 6765 2069 7320  disadvantage is 
+00001ca0: 7468 6174 2074 6865 0a20 2020 2060 536b  that the.    `Sk
+00001cb0: 7953 7572 7665 7960 2069 6d70 6c65 6d65  ySurvey` impleme
+00001cc0: 6e74 6174 696f 6e73 206d 6179 206f 6666  ntations may off
+00001cd0: 6572 206d 6f72 6520 6675 6e63 7469 6f6e  er more function
+00001ce0: 616c 6974 792e 2028 5468 6520 6053 6b79  ality. (The `Sky
+00001cf0: 5669 6577 6020 636f 6e73 7472 7563 746f  View` constructo
+00001d00: 720a 2020 2020 6c65 7473 2079 6f20 6368  r.    lets yo ch
+00001d10: 6f6f 7365 2074 6865 2046 4954 5320 696d  oose the FITS im
+00001d20: 6167 6520 7369 7a65 2069 6e20 7069 7865  age size in pixe
+00001d30: 6c73 2e29 0a0a 2020 2020 5365 6520 7468  ls.)..    See th
+00001d40: 6520 6053 6b79 5375 7276 6579 6020 696d  e `SkySurvey` im
+00001d50: 706c 656d 656e 7461 7469 6f6e 7320 666f  plementations fo
+00001d60: 7220 7468 6520 7375 7070 6f72 7465 6420  r the supported 
+00001d70: 7375 7276 6579 732e 0a0a 2020 2020 5061  surveys...    Pa
+00001d80: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00001d90: 2d2d 2d2d 2d2d 2d0a 2020 2020 7375 7276  -------.    surv
+00001da0: 6579 3a20 6073 7472 600a 2020 2020 2020  ey: `str`.      
+00001db0: 2020 5468 6520 6e61 6d65 206f 6620 7468    The name of th
+00001dc0: 6520 7375 7276 6579 2074 6f20 7175 6572  e survey to quer
+00001dd0: 7920 666f 7220 7468 6520 4649 5453 2066  y for the FITS f
+00001de0: 696c 652e 0a20 2020 2066 6974 735f 6365  ile..    fits_ce
+00001df0: 6e74 6572 3a20 607e 6173 7472 6f70 792e  nter: `~astropy.
+00001e00: 636f 6f72 6469 6e61 7465 732e 536b 7943  coordinates.SkyC
+00001e10: 6f6f 7264 600a 2020 2020 2020 2020 5468  oord`.        Th
+00001e20: 6520 6365 6e74 6572 2070 6f73 6974 696f  e center positio
+00001e30: 6e20 6f66 2074 6865 206c 6f61 6465 6420  n of the loaded 
+00001e40: 4649 5453 2066 696c 652e 0a20 2020 2073  FITS file..    s
+00001e50: 697a 653a 2060 7e61 7374 726f 7079 2e63  ize: `~astropy.c
+00001e60: 6f6f 7264 696e 6174 6573 2e41 6e67 6c65  oordinates.Angle
+00001e70: 600a 2020 2020 2020 2020 5468 6520 7769  `.        The wi
+00001e80: 6474 6820 616e 6420 6865 6967 6874 206f  dth and height o
+00001e90: 6620 7468 6520 4649 5453 2069 6d61 6765  f the FITS image
+00001ea0: 2c20 6173 2061 6e20 616e 676c 6520 6f6e  , as an angle on
+00001eb0: 2074 6865 2073 6b79 2e0a 0a20 2020 2052   the sky...    R
+00001ec0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00001ed0: 2d2d 0a20 2020 2062 696e 6172 7920 7374  --.    binary st
+00001ee0: 7265 616d 0a20 2020 2020 2020 2054 6865  ream.        The
+00001ef0: 2046 4954 5320 6669 6c65 2e0a 2020 2020   FITS file..    
+00001f00: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001f10: 0004 0000 0053 0000 0073 1400 0000 6700  .....S...s....g.
+00001f20: 7c00 5d0c 7d01 7c01 a000 a100 9102 7104  |.].}.|.......q.
+00001f30: 5300 720d 0000 0072 1a00 0000 a902 721d  S.r....r......r.
+00001f40: 0000 00da 0173 720d 0000 0072 0d00 0000  .....sr....r....
+00001f50: 720e 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
+00001f60: 3ee9 0000 0073 0400 0000 0600 0200 7a1d  >....s........z.
+00001f70: 6c6f 6164 5f66 6974 732e 3c6c 6f63 616c  load_fits.<local
+00001f80: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
+00001f90: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001fa0: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
+00001fb0: 0c7d 017c 01a0 00a1 0091 0271 0453 0072  .}.|.......q.S.r
+00001fc0: 0d00 0000 721a 0000 0072 5200 0000 720d  ....r....rR...r.
+00001fd0: 0000 0072 0d00 0000 720e 0000 0072 5400  ...r....r....rT.
+00001fe0: 0000 eb00 0000 7304 0000 0006 0002 0069  ......s........i
+00001ff0: bc02 0000 2901 724a 0000 0072 4400 0000  ....).rJ...rD...
+00002000: 2908 721b 0000 0072 2100 0000 da04 6b65  ).r....r!.....ke
+00002010: 7973 7219 0000 0072 4c00 0000 7248 0000  ysr....rL...rH..
+00002020: 0072 4600 0000 7217 0000 0029 0472 1100  .rF...r....).r..
+00002030: 0000 7212 0000 0072 1300 0000 5a07 7375  ..r....r....Z.su
+00002040: 7276 6579 5f72 0d00 0000 720d 0000 0072  rvey_r....r....r
+00002050: 0e00 0000 7217 0000 00bc 0000 0073 0c00  ....r........s..
+00002060: 0000 002d 1a01 0801 1a01 0c02 0e02 7217  ...-..........r.
+00002070: 0000 0029 15da 0269 6f72 0200 0000 da06  ...)...ior......
+00002080: 7479 7069 6e67 7203 0000 0072 0400 0000  typingr....r....
+00002090: 723b 0000 00da 0761 7374 726f 7079 7205  r;.....astropyr.
+000020a0: 0000 0072 3700 0000 da13 6173 7472 6f70  ...r7.....astrop
+000020b0: 792e 636f 6f72 6469 6e61 7465 7372 0600  y.coordinatesr..
+000020c0: 0000 7207 0000 00da 0d42 6173 6545 7863  ..r......BaseExc
+000020d0: 6570 7469 6f6e 7208 0000 0072 2100 0000  eptionr....r!...
+000020e0: 724c 0000 0072 0f00 0000 7219 0000 0072  rL...r....r....r
+000020f0: 4800 0000 7218 0000 0072 1700 0000 720d  H...r....r....r.
+00002100: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00002110: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00002120: 732c 0000 000c 0110 0208 010c 0110 0310  s,..............
+00002130: 0702 0102 0102 0102 0102 0102 0102 0102  ................
+00002140: f806 0d02 0102 0102 fd06 0710 1510 4210  ..............B.
+00002150: 43                                       C
```

### Comparing `imephu-0.1.0/src/imephu/service/horizons.py` & `imephu-0.2.0/src/imephu/service/horizons.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu/utils.py` & `imephu-0.2.0/src/imephu/utils.py`

 * *Files identical despite different names*

### Comparing `imephu-0.1.0/src/imephu.egg-info/PKG-INFO` & `imephu-0.2.0/src/imephu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: imephu
-Version: 0.1.0
+Version: 0.2.0
 Summary: Generate finder charts for the Southern African Large Telescope (SALT).
 Home-page: https://github.com/saltastroops/saao-pypackage-cookiecutter
 Author: Southern African Large Telescope (SALT)
 Author-email: salthelp@salt.ac.za
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # imephu
 
-imephu is a package for Generating finder charts for astronomical observations. While primarily intended for the [Southern Africa Large Telescope](https://www.salt.ac.za), it can be used to create completely custom finder charts.
+imephu is a package for generating finder charts for astronomical observations. While primarily intended for the [Southern African Large Telescope](https://www.salt.ac.za), it can be used to create completely custom finder charts.
 
 ## Installation
 
 imephu can be installed with pip in the usual way with
 
 ```shell
 pip install imephu
@@ -38,9 +37,7 @@
 Alternatively, you can use an API for creating custom finder charts. An example of how to do this can be found [here](https://saltastroops.github.io/imephu/notebooks/salt.html).
 
 ## Documentation
 
 The documentation is hosted at [https://saltastroops.github.io/imephu/](https://saltastroops.github.io/imephu/).
 
 
-
-
```

### Comparing `imephu-0.1.0/src/imephu.egg-info/SOURCES.txt` & `imephu-0.2.0/src/imephu.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,56 +15,85 @@
 src/imephu.egg-info/PKG-INFO
 src/imephu.egg-info/SOURCES.txt
 src/imephu.egg-info/dependency_links.txt
 src/imephu.egg-info/entry_points.txt
 src/imephu.egg-info/requires.txt
 src/imephu.egg-info/top_level.txt
 src/imephu/__pycache__/__init__.cpython-310.pyc
+src/imephu/__pycache__/__init__.cpython-38.pyc
 src/imephu/__pycache__/cli.cpython-310.pyc
+src/imephu/__pycache__/cli.cpython-38.pyc
 src/imephu/__pycache__/finder_chart.cpython-310.pyc
+src/imephu/__pycache__/finder_chart.cpython-38.pyc
 src/imephu/__pycache__/geometry.cpython-310.pyc
+src/imephu/__pycache__/geometry.cpython-38.pyc
 src/imephu/__pycache__/utils.cpython-310.pyc
+src/imephu/__pycache__/utils.cpython-38.pyc
 src/imephu/annotation/__init__.py
 src/imephu/annotation/motion.py
 src/imephu/annotation/__pycache__/__init__.cpython-310.pyc
+src/imephu/annotation/__pycache__/__init__.cpython-38.pyc
 src/imephu/annotation/__pycache__/general.cpython-310.pyc
 src/imephu/annotation/__pycache__/motion.cpython-310.pyc
+src/imephu/annotation/__pycache__/motion.cpython-38.pyc
 src/imephu/annotation/general/__init__.py
 src/imephu/annotation/general/arrow.py
 src/imephu/annotation/general/circle.py
 src/imephu/annotation/general/crosshairs.py
 src/imephu/annotation/general/empty.py
 src/imephu/annotation/general/group.py
 src/imephu/annotation/general/line_path.py
 src/imephu/annotation/general/rectangle.py
 src/imephu/annotation/general/text.py
 src/imephu/annotation/general/__pycache__/__init__.cpython-310.pyc
+src/imephu/annotation/general/__pycache__/__init__.cpython-38.pyc
 src/imephu/annotation/general/__pycache__/arrow.cpython-310.pyc
+src/imephu/annotation/general/__pycache__/arrow.cpython-38.pyc
 src/imephu/annotation/general/__pycache__/circle.cpython-310.pyc
+src/imephu/annotation/general/__pycache__/circle.cpython-38.pyc
 src/imephu/annotation/general/__pycache__/crosshairs.cpython-310.pyc
+src/imephu/annotation/general/__pycache__/crosshairs.cpython-38.pyc
 src/imephu/annotation/general/__pycache__/empty.cpython-310.pyc
+src/imephu/annotation/general/__pycache__/empty.cpython-38.pyc
 src/imephu/annotation/general/__pycache__/group.cpython-310.pyc
+src/imephu/annotation/general/__pycache__/group.cpython-38.pyc
 src/imephu/annotation/general/__pycache__/line_path.cpython-310.pyc
+src/imephu/annotation/general/__pycache__/line_path.cpython-38.pyc
 src/imephu/annotation/general/__pycache__/rectangle.cpython-310.pyc
+src/imephu/annotation/general/__pycache__/rectangle.cpython-38.pyc
 src/imephu/annotation/general/__pycache__/text.cpython-310.pyc
+src/imephu/annotation/general/__pycache__/text.cpython-38.pyc
 src/imephu/salt/finder_chart.py
 src/imephu/salt/utils.py
 src/imephu/salt/__pycache__/__init__.cpython-310.pyc
 src/imephu/salt/__pycache__/finder_chart.cpython-310.pyc
+src/imephu/salt/__pycache__/finder_chart.cpython-38.pyc
 src/imephu/salt/__pycache__/general.cpython-310.pyc
 src/imephu/salt/__pycache__/rss.cpython-310.pyc
 src/imephu/salt/__pycache__/utils.cpython-310.pyc
+src/imephu/salt/__pycache__/utils.cpython-38.pyc
 src/imephu/salt/annotation/__init__.py
 src/imephu/salt/annotation/nir.py
 src/imephu/salt/annotation/rss.py
 src/imephu/salt/annotation/salticam.py
 src/imephu/salt/annotation/telescope.py
 src/imephu/salt/annotation/__pycache__/__init__.cpython-310.pyc
+src/imephu/salt/annotation/__pycache__/__init__.cpython-38.pyc
 src/imephu/salt/annotation/__pycache__/nir.cpython-310.pyc
+src/imephu/salt/annotation/__pycache__/nir.cpython-38.pyc
 src/imephu/salt/annotation/__pycache__/observation.cpython-310.pyc
 src/imephu/salt/annotation/__pycache__/rss.cpython-310.pyc
+src/imephu/salt/annotation/__pycache__/rss.cpython-38.pyc
 src/imephu/salt/annotation/__pycache__/salticam.cpython-310.pyc
+src/imephu/salt/annotation/__pycache__/salticam.cpython-38.pyc
 src/imephu/salt/annotation/__pycache__/telescope.cpython-310.pyc
+src/imephu/salt/annotation/__pycache__/telescope.cpython-38.pyc
 src/imephu/service/horizons.py
 src/imephu/service/survey.py
 src/imephu/service/__pycache__/horizons.cpython-310.pyc
-src/imephu/service/__pycache__/survey.cpython-310.pyc
+src/imephu/service/__pycache__/horizons.cpython-38.pyc
+src/imephu/service/__pycache__/survey.cpython-310.pyc
+src/imephu/service/__pycache__/survey.cpython-38.pyc
+tests/test_cli.py
+tests/test_finder_chart.py
+tests/test_geometry.py
+tests/test_utils.py
```

