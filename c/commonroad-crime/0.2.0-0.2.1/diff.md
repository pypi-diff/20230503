# Comparing `tmp/commonroad-crime-0.2.0.tar.gz` & `tmp/commonroad-crime-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/commonroad-crime-0.2.0.tar", last modified: Wed Apr  5 15:38:04 2023, max compression
+gzip compressed data, was "dist/commonroad-crime-0.2.1.tar", last modified: Wed May  3 06:49:42 2023, max compression
```

## Comparing `commonroad-crime-0.2.0.tar` & `commonroad-crime-0.2.1.tar`

### file list

```diff
@@ -1,100 +1,112 @@
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/LICENSE
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      348 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/PKG-INFO
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4544 2023-04-05 15:35:26.000000 commonroad-crime-0.2.0/README.md
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8736 2023-04-04 15:37:50.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/base.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/config_defaults/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/config_defaults/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10783 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/configuration.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4835 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/configuration_builder.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3975 2023-04-04 14:41:32.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/crime_interface.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1898 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/scene.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2681 2023-04-05 15:15:40.000000 commonroad-crime-0.2.0/commonroad_crime/data_structure/type.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1209 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5075 2023-04-04 14:14:27.000000 commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/a_lat_req.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4420 2023-04-04 13:51:42.000000 commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/a_long_req.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1944 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/a_req.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2633 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/dst.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/distance/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/distance/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4064 2023-04-05 15:14:57.000000 commonroad-crime-0.2.0/commonroad_crime/measure/distance/dce.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3053 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/distance/hw.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      980 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/distance/msd.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      980 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/distance/psd.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/aci.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2147 2023-04-04 14:10:05.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/btn.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      971 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/ci.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/cpi.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/pri.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/rss.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/soi.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2079 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/stn.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2827 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/index/tci.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/jerk/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/jerk/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1875 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/jerk/lat_j.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1957 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/jerk/long_j.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/potential/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/potential/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    13780 2023-04-04 14:43:20.000000 commonroad-crime-0.2.0/commonroad_crime/measure/potential/pf.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      979 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/potential/sp.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/probability/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/probability/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6753 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/probability/p_mc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      992 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/probability/p_smh.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      992 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/probability/p_srs.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/reachable_set/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/reachable_set/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4336 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/reachable_set/drivable_area.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      972 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/ags.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/et.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      972 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/pet.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      975 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/pttc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/tc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1578 2023-04-02 11:49:42.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/tet.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4298 2023-04-04 12:29:51.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/thw.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3495 2023-04-02 11:31:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/tit.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      629 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/ttb.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5675 2023-04-04 14:41:24.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/ttc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6262 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/ttc_star.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1985 2023-04-05 15:14:57.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/ttce.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      627 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/ttk.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6537 2023-04-04 13:18:50.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/ttm.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2250 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/ttr.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2370 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/tts.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6173 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/ttz.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/tv.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5478 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/wttc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5758 2023-04-04 13:46:00.000000 commonroad-crime-0.2.0/commonroad_crime/measure/time/wttr.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/measure/velocity/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)       28 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/velocity/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      977 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/measure/velocity/cs.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2782 2023-04-04 13:51:42.000000 commonroad-crime-0.2.0/commonroad_crime/measure/velocity/delta_v.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime/utility/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/utility/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5829 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/utility/batch_evaluation.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5356 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/utility/general.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1855 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/utility/logger.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8945 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/utility/optimization.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    24999 2023-04-02 10:41:04.000000 commonroad-crime-0.2.0/commonroad_crime/utility/simulation.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     9148 2023-04-02 10:40:15.000000 commonroad-crime-0.2.0/commonroad_crime/utility/solver.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8142 2023-04-04 15:54:54.000000 commonroad-crime-0.2.0/commonroad_crime/utility/visualization.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime.egg-info/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      348 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime.egg-info/PKG-INFO
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     3283 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime.egg-info/SOURCES.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime.egg-info/dependency_links.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      252 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime.egg-info/requires.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       17 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/commonroad_crime.egg-info/top_level.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-04-05 15:38:04.000000 commonroad-crime-0.2.0/setup.cfg
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      886 2023-04-05 15:33:45.000000 commonroad-crime-0.2.0/setup.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/LICENSE
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      301 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/PKG-INFO
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4564 2023-04-09 12:14:11.000000 commonroad-crime-0.2.1/README.md
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.1/commonroad_crime/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8736 2023-04-19 15:18:31.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/base.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/config_defaults/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/config_defaults/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10783 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/configuration.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4835 2023-04-02 10:41:04.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/configuration_builder.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3975 2023-04-04 14:41:32.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/crime_interface.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1898 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/scene.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2681 2023-04-06 16:10:49.000000 commonroad-crime-0.2.1/commonroad_crime/data_structure/type.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1209 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5291 2023-04-20 08:47:33.000000 commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/a_lat_req.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4420 2023-04-04 13:51:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/a_long_req.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1944 2023-04-02 10:41:04.000000 commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/a_req.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2633 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/dst.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/distance/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/distance/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4425 2023-04-07 09:40:31.000000 commonroad-crime-0.2.1/commonroad_crime/measure/distance/dce.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3326 2023-04-19 08:48:11.000000 commonroad-crime-0.2.1/commonroad_crime/measure/distance/hw.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      980 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/distance/msd.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      980 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/distance/psd.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/aci.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2147 2023-04-04 14:10:05.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/btn.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      971 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/ci.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/cpi.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/pri.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/rss.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/soi.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2079 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/stn.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2827 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/index/tci.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/jerk/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/jerk/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1875 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/jerk/lat_j.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1957 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/jerk/long_j.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/potential/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/potential/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    13780 2023-04-04 14:43:20.000000 commonroad-crime-0.2.1/commonroad_crime/measure/potential/pf.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      979 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/potential/sp.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/probability/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/probability/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6753 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/probability/p_mc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      992 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/probability/p_smh.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      992 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/probability/p_srs.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/reachable_set/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/reachable_set/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4617 2023-04-20 08:47:33.000000 commonroad-crime-0.2.1/commonroad_crime/measure/reachable_set/drivable_area.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      972 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/ags.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/et.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      972 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/pet.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      975 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/pttc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/tc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1578 2023-04-02 11:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/tet.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4298 2023-04-04 12:29:51.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/thw.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3495 2023-04-02 11:31:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/tit.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      629 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/ttb.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5797 2023-04-20 08:59:04.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/ttc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6296 2023-05-03 06:44:51.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/ttc_star.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1988 2023-04-09 11:48:02.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/ttce.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      627 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/ttk.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6641 2023-04-20 14:19:33.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/ttm.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2250 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/ttr.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2370 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/tts.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6173 2023-04-02 10:41:04.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/ttz.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/tv.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5478 2023-05-03 06:44:51.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/wttc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5879 2023-04-09 11:45:45.000000 commonroad-crime-0.2.1/commonroad_crime/measure/time/wttr.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/velocity/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)       28 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/velocity/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      977 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/measure/velocity/cs.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2782 2023-04-04 13:51:42.000000 commonroad-crime-0.2.1/commonroad_crime/measure/velocity/delta_v.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime/utility/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.1/commonroad_crime/utility/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5829 2023-04-02 10:41:04.000000 commonroad-crime-0.2.1/commonroad_crime/utility/batch_evaluation.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5356 2023-04-20 09:32:40.000000 commonroad-crime-0.2.1/commonroad_crime/utility/general.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1855 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/commonroad_crime/utility/logger.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8945 2023-04-02 10:41:04.000000 commonroad-crime-0.2.1/commonroad_crime/utility/optimization.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    25642 2023-04-20 09:31:14.000000 commonroad-crime-0.2.1/commonroad_crime/utility/simulation.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     9390 2023-04-19 08:46:38.000000 commonroad-crime-0.2.1/commonroad_crime/utility/solver.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8546 2023-04-23 07:37:21.000000 commonroad-crime-0.2.1/commonroad_crime/utility/visualization.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime.egg-info/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      301 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime.egg-info/PKG-INFO
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     3605 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      253 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime.egg-info/requires.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       17 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/commonroad_crime.egg-info/top_level.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/setup.cfg
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      887 2023-05-03 06:49:39.000000 commonroad-crime-0.2.1/setup.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 06:49:42.000000 commonroad-crime-0.2.1/tests/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1674 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/tests/test_acceleration_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      981 2022-11-01 14:27:06.000000 commonroad-crime-0.2.1/tests/test_base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1143 2023-04-05 14:45:46.000000 commonroad-crime-0.2.1/tests/test_distance_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1493 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/tests/test_index_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1393 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/tests/test_jerk_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      801 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/tests/test_potential_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      855 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/tests/test_probability_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      968 2023-04-09 11:42:41.000000 commonroad-crime-0.2.1/tests/test_reachable_set_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6635 2023-05-03 06:44:51.000000 commonroad-crime-0.2.1/tests/test_time_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6519 2023-04-20 08:59:04.000000 commonroad-crime-0.2.1/tests/test_utils_simulation.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      787 2023-04-02 10:40:15.000000 commonroad-crime-0.2.1/tests/test_velocity_domain.py
```

### Comparing `commonroad-crime-0.2.0/LICENSE` & `commonroad-crime-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/README.md` & `commonroad-crime-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 $ cd <path-to-this-repo>
 $ pip install -e .
 $ conda develop .
 ```
 **(optional)** In order to run reachability analysis related measures 
 (e.g., ``worst-time-to-react (WTTR)``, `drivable area (DA)`), you have to install the following repositories as well:
 
-- [commonroad-reach](https://gitlab.lrz.de/tum-cps/commonroad-reach)
+- [commonroad-reach](https://gitlab.lrz.de/tum-cps/commonroad-reach) (version: >=2023.1)
 
 To test the installition, run unittest:
 ```bash
 $ cd tests
 $ python -m unittest -v
 ```
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/data_structure/base.py` & `commonroad-crime-0.2.1/commonroad_crime/data_structure/base.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/data_structure/configuration.py` & `commonroad-crime-0.2.1/commonroad_crime/data_structure/configuration.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/data_structure/configuration_builder.py` & `commonroad-crime-0.2.1/commonroad_crime/data_structure/configuration_builder.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/data_structure/crime_interface.py` & `commonroad-crime-0.2.1/commonroad_crime/data_structure/crime_interface.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/data_structure/scene.py` & `commonroad-crime-0.2.1/commonroad_crime/data_structure/scene.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/data_structure/type.py` & `commonroad-crime-0.2.1/commonroad_crime/data_structure/type.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 class TypeVelocity(str, Enum):
     Delta_V = "Delta-v"
     CS = "conflict severity"
 
 
 class TypeAcceleration(str, Enum):
     DST = "deceleration-to-safety-time"
-    ALongReq = "required longitudinal acceleration (aka deceleration-rate-to-avoid-crash)"
+    ALongReq = "required longitudinal acceleration (aka deceleration rate to avoid crash)"
     ALatReq = "required lateral acceleration"
     AReq = "required acceleration"
 
 
 class TypeJerk(str, Enum):
     LatJ = "lateral jerk"
     LongJ = "longitudinal jerk"
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/__init__.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/a_lat_req.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/a_lat_req.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import math
 import logging
 import numpy as np
 
+from commonroad.geometry.shape import Circle
+
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.type import TypeAcceleration, TypeMonotone
 from commonroad_crime.measure.time.ttc import TTC
 
 import commonroad_crime.utility.general as utils_gen
 import commonroad_crime.utility.solver as utils_sol
@@ -45,16 +47,20 @@
         :param v_rel_lat: relative velocity between two obstacles along the latteral direction
         :param ttc: time-to-collision
         :param flag_dir: direction - left or right
 
         :return a_lat: required lateral acceleration of the ego vehicle
         """
         sign = 1 if flag_dir == 'left' else -1
-        return a_obj_lat - 2 * (-d_rel_lat + sign * (self.other_vehicle.obstacle_shape.width/2 +
-                                                     self.ego_vehicle.obstacle_shape.width/2) - v_rel_lat * ttc)/ttc**2
+        if isinstance(self.other_vehicle.obstacle_shape, Circle):
+            other_width = self.other_vehicle.obstacle_shape.radius
+        else:
+            other_width = self.other_vehicle.obstacle_shape.width/2
+        return a_obj_lat - 2 * (-d_rel_lat + sign * (other_width + self.ego_vehicle.obstacle_shape.width / 2)
+                                - v_rel_lat * ttc) / ttc ** 2
 
     def compute(self, vehicle_id: int, time_step: int = 0):
         utils_log.print_and_log_info(logger, f"* Computing the {self.measure_name} at time step {time_step}")
         self.set_other_vehicles(vehicle_id)
         self.time_step = time_step
         if self._except_obstacle_in_same_lanelet(expected_value=0.0):
             # no negative acceleration is needed for avoiding a collision
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/a_long_req.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/a_long_req.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/a_req.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/a_req.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/acceleration/dst.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/acceleration/dst.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/distance/dce.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/distance/dce.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import math
 import matplotlib.pyplot as plt
 import logging
-
 import numpy as np
 
+from commonroad.geometry.shape import ShapeGroup
+
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeDistance, TypeMonotone
 from commonroad_crime.data_structure.base import CriMeBase
 import commonroad_crime.utility.visualization as utils_vis
 from commonroad_crime.utility.visualization import TUMcolor
 import commonroad_crime.utility.general as utils_gen
 import commonroad_crime.utility.logger as utils_log
@@ -46,16 +47,21 @@
         self.time_step = time_step
 
         state_list = self.ego_vehicle.prediction.trajectory.state_list
         dce = math.inf
         for i in range(time_step, len(state_list)):
             if self.other_vehicle.occupancy_at_time(i) is not None:
                 ego_poly = self.ego_vehicle.occupancy_at_time(i).shape.shapely_object
-                other_poly = self.other_vehicle.occupancy_at_time(i).shape.shapely_object
-                distance = ego_poly.distance(other_poly)
+                other_shape = self.other_vehicle.occupancy_at_time(i).shape
+                if isinstance(other_shape, ShapeGroup):
+                    distance = min(
+                        [ego_poly.distance(shape_element.shapely_object) for shape_element in other_shape.shapes])
+                else:
+                    other_poly = self.other_vehicle.occupancy_at_time(i).shape.shapely_object
+                    distance = ego_poly.distance(other_poly)
                 if distance < dce:
                     self.time_dce = i
                     dce = distance
                 if dce == 0.:
                     break
             else:
                 break
@@ -88,8 +94,7 @@
         plt.plot(x, y)
 
         if self.configuration.debug.draw_visualization:
             if self.configuration.debug.save_plots:
                 utils_vis.save_fig(self.measure_name, self.configuration.general.path_output, self.time_step)
             else:
                 plt.show()
-
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/distance/hw.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/distance/hw.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeDistance, TypeMonotone
 from commonroad_crime.measure.time.thw import THW
 import commonroad_crime.utility.visualization as utils_vis
 import commonroad_crime.utility.solver as utils_sol
 from commonroad_crime.utility.visualization import TUMcolor
 
-from commonroad.geometry.shape import Polygon
+from commonroad.geometry.shape import Polygon, Circle
 
 logger = logging.getLogger(__name__)
 
 
 class HW(THW):
     """
     https://criticality-metrics.readthedocs.io/en/latest/time-scale/THW.html
@@ -36,16 +36,20 @@
         super(HW, self).__init__(config)
 
     def cal_headway(self):
         if isinstance(self.other_vehicle.obstacle_shape, Polygon):
             # todo: fix for ttz
             other_position = self.other_vehicle.state_at_time(self.time_step).position
         else:
-            other_position = self.other_vehicle.state_at_time(self.time_step).position - \
-                             self.other_vehicle.obstacle_shape.length / 2
+            if isinstance(self.other_vehicle.obstacle_shape, Circle):
+                other_position = self.other_vehicle.state_at_time(self.time_step).position - \
+                                 self.other_vehicle.obstacle_shape.radius
+            else:
+                other_position = self.other_vehicle.state_at_time(self.time_step).position - \
+                                 self.other_vehicle.obstacle_shape.length / 2
         ego_position = self.ego_vehicle.state_at_time(self.time_step).position + \
                        self.ego_vehicle.obstacle_shape.length / 2
         headway = utils_sol.compute_clcs_distance(self.clcs, ego_position, other_position)[0]
         if headway < 0:
             return math.inf
         else:
             return headway
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/distance/msd.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/distance/msd.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/distance/psd.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/distance/psd.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/index/aci.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/index/aci.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/index/btn.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/index/btn.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/index/ci.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/index/ci.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/index/cpi.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/index/cpi.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/index/pri.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/index/pri.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/index/rss.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/index/rss.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/index/soi.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/index/soi.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/index/stn.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/index/stn.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/index/tci.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/index/tci.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/jerk/lat_j.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/jerk/lat_j.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/jerk/long_j.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/jerk/long_j.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/potential/pf.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/potential/pf.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/potential/sp.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/potential/sp.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/probability/p_mc.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/probability/p_mc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/probability/p_smh.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/probability/p_smh.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/probability/p_srs.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/probability/p_srs.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/reachable_set/drivable_area.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/reachable_set/drivable_area.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,19 @@
         if self.configuration.reachable_set.cosy == 1:
             self.reach_config.planning.coordinate_system = "CART"
         self.reach_config.update()
         self.reach_interface = ReachableSetInterface(self.reach_config)
 
     def _update_initial_state(self, target_state: Union[InitialState, CustomState]):
         self.reach_config.planning_problem.initial_state.position = target_state.position
-        self.reach_config.planning_problem.initial_state.velocity = target_state.velocity
+        if hasattr(target_state, "velocity_y"):
+            self.reach_config.planning_problem.initial_state.velocity = np.sqrt(target_state.velocity**2 +
+                                                                                target_state.velocity_y**2)
+        else:
+            self.reach_config.planning_problem.initial_state.velocity = target_state.velocity
         self.reach_config.planning_problem.initial_state.orientation = target_state.orientation
         self.reach_config.planning_problem.initial_state.time_step = target_state.time_step
 
     def compute(self, time_step: int = 0, vehicle_id: int = None, verbose: bool = True):
         self.value = 0.
         evaluated_state = copy.deepcopy(self.ego_vehicle.state_at_time(time_step))
         self._update_initial_state(target_state=evaluated_state)
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/ags.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/ags.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/et.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/et.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/pet.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/pet.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/pttc.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/pttc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/tc.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/tc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/tet.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/tet.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/thw.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/thw.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/tit.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/tit.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/ttb.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/ttb.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/ttc.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/ttc.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,18 +100,22 @@
             else:  # (delta_v >= 0 and delta_a >= 0) or (delta_v ** 2 - 2 * delta_d * delta_a < 0)
                 self.value = math.inf
 
         utils_log.print_and_log_info(logger, f"*\t\t {self.measure_name} = {self.value}")
         return self.value
 
     def visualize(self):
-        self._initialize_vis(plot_limit=utils_vis.plot_limits_from_state_list(self.time_step,
-                                                                              self.ego_vehicle.prediction.
-                                                                              trajectory.state_list,
-                                                                              margin=10))
+        if self.configuration.debug.plot_limits:
+            plot_limits = self.configuration.debug.plot_limits
+        else:
+            plot_limits = utils_vis.plot_limits_from_state_list(self.time_step,
+                                                                self.ego_vehicle.prediction.
+                                                                trajectory.state_list,
+                                                                margin=10)
+        self._initialize_vis(plot_limit=plot_limits)
         self.rnd.draw_params.time_begin = self.time_step
         self.rnd.draw_params.dynamic_obstacle.occupancy.shape.facecolor = TUMcolor.TUMred
         self.other_vehicle.draw(self.rnd)
         self.rnd.render()
         plt.title(f"{self.measure_name} at time step {self.time_step}")
         if self.configuration.debug.save_plots:
             utils_vis.save_fig(self.measure_name, self.configuration.general.path_output, self.time_step)
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/ttc_star.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/ttc_star.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,21 +81,21 @@
         self.collision_checker.draw(rnd)
 
     def visualize(self, figsize: tuple = (25, 15)):
         self._initialize_vis(figsize=figsize)
         self.draw_collision_checker(self.rnd)
         self.rnd.render()
         if self.value not in [math.inf, -math.inf]:
-            tstc = int(utils_gen.int_round(self.value / self.dt, 0))
+            tstc = int(utils_gen.int_round(self.value / self.dt, 0)) + self.time_step
             utils_vis.draw_dyn_vehicle_shape(self.rnd, self.ego_vehicle, tstc)
             utils_vis.draw_state(self.rnd, self.ego_vehicle.state_at_time(tstc), TUMcolor.TUMred)
             if self.time_step == 0 and self.ego_vehicle.prediction.trajectory.state_list[0].time_step != 0:
                 sl = [self.ego_vehicle.initial_state] + self.ego_vehicle.prediction.trajectory.state_list
             else:
-                sl = self.ego_vehicle.prediction.trajectory.state_list
+                sl = self.ego_vehicle.prediction.trajectory.state_list[self.time_step:]
             utils_vis.draw_state_list(self.rnd, sl, self.time_step, TUMcolor.TUMblue)
         else:
             tstc = self.value
         plt.title(f"{self.measure_name} at time step {self.time_step} is {self.value}")
         if self.configuration.debug.save_plots:
             utils_vis.save_fig(self.measure_name, self.configuration.general.path_output, tstc)
         else:
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/ttce.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/ttce.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
         """
         Using DCE to calculate the TTCE value. DCE marks the time step when the minimal distance is reached.
         """
         utils_log.print_and_log_info(logger, f"* Computing the {self.measure_name} at time step {time_step}")
         self._dce_object.compute(vehicle_id, time_step)
-        self.value = utils_gen.int_round((self._dce_object.time_dce - time_step) * self.dt)
+        self.value = utils_gen.int_round((self._dce_object.time_dce - time_step) * self.dt, 3)
         utils_log.print_and_log_info(logger, f"*\t\t {self.measure_name} with vehicle id {vehicle_id} = {self.value}")
         return self.value
 
     def visualize(self):
         self._dce_object.configuration.debug.draw_visualization = False
         self._dce_object.visualize()
         if self.configuration.debug.save_plots:
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/ttk.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/ttk.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/ttm.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/ttm.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,18 +53,22 @@
         return self._maneuver
 
     @maneuver.setter
     def maneuver(self, maneuver: Maneuver):
         self._maneuver = maneuver
 
     def visualize(self, figsize: tuple = (25, 15)):
-        self._initialize_vis(figsize=figsize, plot_limit=utils_vis.plot_limits_from_state_list(self.time_step,
-                                                                                               self.ego_vehicle.prediction.
-                                                                                               trajectory.state_list,
-                                                                                               margin=10))
+        if self.configuration.debug.plot_limits:
+            plot_limits = self.configuration.debug.plot_limits
+        else:
+            plot_limits = utils_vis.plot_limits_from_state_list(self.time_step,
+                                                                self.ego_vehicle.prediction.
+                                                                trajectory.state_list,
+                                                                margin=10)
+        self._initialize_vis(figsize=figsize, plot_limit=plot_limits)
         self.ttc_object.draw_collision_checker(self.rnd)
         for veh in self.sce.obstacles:
             if veh is not self.ego_vehicle:
                 veh.draw(self.rnd)
         self.rnd.render()
         if self.time_step == 0 and self.ego_vehicle.prediction.trajectory.state_list[0].time_step != 0:
             utils_vis.draw_state_list(self.rnd, [self.ego_vehicle.initial_state] +
@@ -74,15 +78,15 @@
             utils_vis.draw_state_list(self.rnd, self.ego_vehicle.prediction.trajectory.state_list[self.time_step:],
                                       color=TUMcolor.TUMblue, linewidth=5)
         for sl in self.state_list_set:
             utils_vis.draw_state_list(self.rnd, sl)
         if self.value not in [math.inf, -math.inf] and self.ttc:
             tstm = int(utils_gen.int_round(self.value / self.dt, 0)) + self.time_step
             utils_vis.draw_state(self.rnd, self.ego_vehicle.state_at_time(tstm), TUMcolor.TUMgreen)
-            tstc = int(utils_gen.int_round(self.ttc_object.value / self.dt, 0))
+            tstc = int(utils_gen.int_round(self.ttc_object.value / self.dt, 0)) + self.time_step
             utils_vis.draw_state(self.rnd, self.ego_vehicle.state_at_time(tstc), TUMcolor.TUMred)
 
             tstc = int(utils_gen.int_round(self.ttc / self.dt, 0)) + self.time_step
             utils_vis.draw_dyn_vehicle_shape(self.rnd, self.ego_vehicle, tstc)
             utils_vis.draw_state_list(self.rnd, self.selected_state_list[tstm:],
                                       color=TUMcolor.TUMgreen, linewidth=5)
         else:
@@ -118,25 +122,27 @@
 
     def binary_search(self, initial_step: int) -> float:
         """
         Binary search to find the last time to execute the maneuver.
         """
         ttm = - math.inf
         low = initial_step
-        high = int(utils_gen.int_round(self.ttc / self.dt,  str(self.dt)[::-1].find('.')))
+        high = int(utils_gen.int_round(self.ttc / self.dt + self.time_step,  str(self.dt)[::-1].find('.')))
         while low < high:
             mid = int((low + high) / 2)
             state_list = self.simulator.simulate_state_list(mid)
-            utils_gen.check_elements_state_list(state_list, self.dt)
-            self.state_list_set.append(state_list[mid:])
             # flag for successful simulation, 0: False, 1: True
             flag_succ = state_list[-1].time_step == self.ego_vehicle.prediction.final_time_step
+            if not flag_succ:
+                high = mid
+                continue
+            self.state_list_set.append(state_list[mid:])
             # flag for collision, 0: False, 1: True
             flag_coll = self.ttc_object.detect_collision(state_list)
-            if not flag_coll and flag_succ:
+            if not flag_coll:
                 low = mid + 1
                 self.selected_state_list = state_list
             else:
                 high = mid
         if low != initial_step:
             ttm = (low - initial_step - 1) * self.dt
         return ttm
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/ttr.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/ttr.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/tts.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/tts.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/ttz.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/ttz.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/tv.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/tv.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/wttc.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/wttc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/time/wttr.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/time/wttr.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     def binary_search(self, initial_step: int):
         """
         Binary search to find the last time to execute the maneuver.
         """
         wttr = - math.inf
         low = initial_step
-        tstc = int(utils_gen.int_round(self.ttc / self.dt,  str(self.dt)[::-1].find('.')))
+        tstc = int(utils_gen.int_round(self.ttc / self.dt + self.time_step,  str(self.dt)[::-1].find('.')))
         high = tstc + initial_step
         time_end = self.ego_vehicle.prediction.final_time_step
         while low < high:
             mid = int((low + high) / 2)
             mid_state = copy.deepcopy(self.ego_vehicle.state_at_time(mid))
             self._update_initial_state(mid_state)
             self.reach_config.update(planning_problem=self.reach_config.planning_problem)
@@ -99,22 +99,23 @@
                 high = mid
         if low != initial_step:
             # no -1 (differs from the binary search for TTM)
             wttr = (low - initial_step) * self.dt
         return wttr
 
     def visualize(self):
-        wtstr = int(utils_gen.int_round(self.value / self.dt, 0)) + self.time_step - 1
-        mid_state = copy.deepcopy(self.ego_vehicle.state_at_time(wtstr))
-        self._update_initial_state(mid_state)
-        self.reach_config.update(planning_problem=self.reach_config.planning_problem)
-        self.reach_config.scenario.remove_obstacle(
-            self.reach_config.scenario.obstacle_by_id(self.ego_vehicle.obstacle_id))
-        self.reach_interface.reset(self.reach_config)
-        self._end_sim = self.ego_vehicle.prediction.final_time_step
+        if self.value not in [math.inf, -math.inf]:
+            wtstr = int(utils_gen.int_round(self.value / self.dt, 0)) + self.time_step - 1
+            mid_state = copy.deepcopy(self.ego_vehicle.state_at_time(wtstr))
+            self._update_initial_state(mid_state)
+            self.reach_config.update(planning_problem=self.reach_config.planning_problem)
+            self.reach_config.scenario.remove_obstacle(
+                self.reach_config.scenario.obstacle_by_id(self.ego_vehicle.obstacle_id))
+            self.reach_interface.reset(self.reach_config)
+            self._end_sim = self.ego_vehicle.prediction.final_time_step
 
-        self.reach_interface.compute_reachable_sets(0, self._end_sim, verbose=True)
-        util_visual.plot_scenario_with_reachable_sets(self.reach_interface,
-                                                      step_start=0,
-                                                      step_end=self._end_sim)
-        # util_visual.plot_collision_checker(self.reach_interface)
+            self.reach_interface.compute_reachable_sets(0, self._end_sim, verbose=True)
+            util_visual.plot_scenario_with_reachable_sets(self.reach_interface,
+                                                          step_start=0,
+                                                          step_end=self._end_sim)
+            # util_visual.plot_collision_checker(self.reach_interface)
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/velocity/cs.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/velocity/cs.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/measure/velocity/delta_v.py` & `commonroad-crime-0.2.1/commonroad_crime/measure/velocity/delta_v.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/utility/batch_evaluation.py` & `commonroad-crime-0.2.1/commonroad_crime/utility/batch_evaluation.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/utility/general.py` & `commonroad-crime-0.2.1/commonroad_crime/utility/general.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/utility/logger.py` & `commonroad-crime-0.2.1/commonroad_crime/utility/logger.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/utility/optimization.py` & `commonroad-crime-0.2.1/commonroad_crime/utility/optimization.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.0/commonroad_crime/utility/simulation.py` & `commonroad-crime-0.2.1/commonroad_crime/utility/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,21 @@
     def initialize_state_list(self, time_step: int) -> List[KSState]:
         """
         Initializing the state list based on the given time step. All the states before the time step would be returned.
         """
         state_list = []
         if time_step is not 0:
             for ts in range(0, time_step):
-                state = self.simulated_vehicle.state_at_time(ts)
+                state = copy.deepcopy(self.simulated_vehicle.state_at_time(ts))
                 check_elements_state(state)
                 state_list.append(state)
+        # additionally check the elements
+        check_elements_state(self.simulated_vehicle.state_at_time(time_step))
+        self.input.acceleration_y = self.simulated_vehicle.state_at_time(time_step).acceleration_y
+        self.input.acceleration = self.simulated_vehicle.state_at_time(time_step).acceleration
         return state_list
 
     def update_maneuver(self, maneuver: Maneuver):
         self.maneuver = maneuver
         self.initialize_simulator()
 
     def initialize_simulator(self):
@@ -129,16 +133,17 @@
         forward simulation of the state list
         """
         pass
 
     def check_velocity_feasibility(self, state: Union[PMState, KSState]) -> bool:
         # the vehicle model in highD doesn't comply with commonroad vehicle models, thus the velocity limit
         # doesn't work for highD scenarios
-        if state.velocity < 0 or \
-                state.velocity > self.parameters.longitudinal.v_max:  # parameters.longitudinal.v_max:
+        abs_velocity = np.sqrt(state.velocity ** 2 + state.velocity_y ** 2)
+        if abs_velocity < 0.1 or \
+                abs_velocity > self.parameters.longitudinal.v_max:  # parameters.longitudinal.v_max:
             return False
         return True
 
 
 class SimulationRandoMonteCarlo(SimulationBase):
     """
     Simulate the random behavior of vehicles.
@@ -232,17 +237,17 @@
         """
         self.set_a_long_and_a_lat(ref_state)
 
     def simulate_state_list(self, start_time_step: int, given_time_limit: int = None):
         """
         Simulates the longitudinal state list from the given start time step.
         """
+        state_list = self.initialize_state_list(start_time_step)
         # using copy to prevent the change of the initial trajectory
         pre_state = copy.deepcopy(self.simulated_vehicle.state_at_time(start_time_step))
-        state_list = self.initialize_state_list(start_time_step)
         # update the input
         check_elements_state(pre_state, self.input)
         self.set_inputs(pre_state)
         state_list.append(pre_state)
 
         if given_time_limit:
             self.time_horizon = given_time_limit
@@ -257,19 +262,22 @@
                 check_elements_state(suc_state, self.input)
                 state_list.append(suc_state)
                 pre_state = suc_state
                 # update the input
             else:
                 # the simulated state is infeasible, i.e., further acceleration/deceleration is not permitted
                 if suc_state is not None:
-                    if suc_state.velocity < 0:
+                    if suc_state.velocity ** 2 + suc_state.velocity_y ** 2 < 0.1:
                         pre_state.velocity = 0
                         pre_state.velocity_y = 0
-                self.a_long = 0
-                self.update_inputs_x_y(pre_state)
+                    for time_step in range(pre_state.time_step + 1, self.time_horizon + 1):
+                        stat_state = copy.deepcopy(pre_state)
+                        stat_state.time_step = time_step
+                        state_list.append(stat_state)
+                break
         return state_list
 
 
 class SimulationLongMonteCarlo(SimulationLong):
     """
     Simulate the longitudinal trajectory using Monte-Carlo sampling
     """
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/utility/solver.py` & `commonroad-crime-0.2.1/commonroad_crime/utility/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 __status__ = "Pre-alpha"
 
 from typing import Tuple, Union
 import numpy as np
 import logging
 from scipy.spatial.distance import cdist
 
-from commonroad.scenario.obstacle import Obstacle, StaticObstacle, State
+from commonroad.scenario.obstacle import Obstacle, StaticObstacle, State, ObstacleType
 from commonroad.scenario.lanelet import Lanelet, LaneletNetwork
 
 from commonroad_dc.pycrccosy import CurvilinearCoordinateSystem
 from commonroad_dc.geometry.util import resample_polyline
 
 logger = logging.getLogger(__name__)
 
@@ -23,17 +23,23 @@
 def solver_wttc(veh_1: Obstacle,
                 veh_2: Obstacle,
                 time_step: int,
                 a_max: float, ):
     """
     Analytical solution of the worst-time-to-collision.
     """
-    r_v1, _ = compute_disc_radius_and_distance(veh_1.obstacle_shape.length,
-                                               veh_1.obstacle_shape.width)
-    r_v2, _ = compute_disc_radius_and_distance(veh_2.obstacle_shape.length,
+    if veh_1.obstacle_type == ObstacleType.PEDESTRIAN:
+        r_v1 = veh_1.obstacle_shape.radius
+    else:
+        r_v1, _ = compute_disc_radius_and_distance(veh_1.obstacle_shape.length,
+                                                   veh_1.obstacle_shape.width)
+    if veh_2.obstacle_type == ObstacleType.PEDESTRIAN:
+        r_v2 = veh_2.obstacle_shape.radius
+    else:
+        r_v2, _ = compute_disc_radius_and_distance(veh_2.obstacle_shape.length,
                                                veh_2.obstacle_shape.width)
     x_10, y_10 = veh_1.state_at_time(time_step).position
     x_20, y_20 = veh_2.state_at_time(time_step).position
     v_1x0, v_1y0 = veh_1.state_at_time(time_step).velocity, veh_1.state_at_time(time_step).velocity_y
     v_2x0, v_2y0 = veh_2.state_at_time(time_step).velocity, veh_2.state_at_time(time_step).velocity_y
     a_10 = a_20 = a_max
     if isinstance(veh_2, StaticObstacle):
```

### Comparing `commonroad-crime-0.2.0/commonroad_crime/utility/visualization.py` & `commonroad-crime-0.2.1/commonroad_crime/utility/visualization.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Union, List
 from enum import Enum
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 
 from commonroad.visualization.mp_renderer import MPRenderer
+from commonroad.geometry.shape import ShapeGroup
 from commonroad.scenario.state import PMState
 from commonroad.scenario.scenario import Scenario
 from commonroad.scenario.obstacle import DynamicObstacle
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.scene import Scene
 from commonroad_crime.data_structure.type import TypeMonotone
@@ -66,16 +67,22 @@
     rnd.ax.add_patch(cir_c)
     rnd.ax.add_patch(cir_b)
 
 
 def draw_dyn_vehicle_shape(rnd: MPRenderer, obstacle: DynamicObstacle, time_step: int,
                            color: TUMcolor = TUMcolor.TUMblue):
     global zorder
-    x, y = obstacle.occupancy_at_time(time_step).shape.shapely_object.exterior.xy
-    rnd.ax.fill(x, y, alpha=0.5, fc=color, ec=None, zorder=zorder)
+    obs_shape = obstacle.occupancy_at_time(time_step).shape
+    if isinstance(obs_shape, ShapeGroup):
+        for shape_element in obs_shape.shapes:
+            x, y = shape_element.shapely_object.exterior.xy
+            rnd.ax.fill(x, y, alpha=0.5, fc=color, ec=None, zorder=zorder)
+    else:
+        x, y = obs_shape.shapely_object.exterior.xy
+        rnd.ax.fill(x, y, alpha=0.5, fc=color, ec=None, zorder=zorder)
     zorder += 1
 
 
 def draw_circle(rnd: MPRenderer, center: np.ndarray, radius: float,
                 opacity: float = 0.5, color: TUMcolor = TUMcolor.TUMblue):
     global zorder
     cir = plt.Circle((center[0], center[1]), radius, color=color, zorder=zorder, alpha=opacity)
@@ -184,17 +191,19 @@
                 count_row += 1
         plt.show()
 
 
 def visualize_scenario_at_time_steps(scenario: Scenario, plot_limit, time_steps: List[int]):
     rnd = MPRenderer(plot_limits=plot_limit)
     rnd.draw_params.time_begin = time_steps[0]
+    if time_steps:
+        rnd.draw_params.time_end = time_steps[-1]
     rnd.draw_params.trajectory.draw_trajectory = False
     rnd.draw_params.dynamic_obstacle.draw_icon = True
     scenario.draw(rnd)
     rnd.render()
     for obs in scenario.obstacles:
-        draw_state_list(rnd, obs.prediction.trajectory.state_list[time_steps[0]:],
+        draw_state_list(rnd, obs.prediction.trajectory.state_list[time_steps[0]:time_steps[-1] + 1],
                         color=TUMcolor.TUMblue, linewidth=5)
         for ts in time_steps[1:]:
             draw_dyn_vehicle_shape(rnd, obs, ts, color=TUMcolor.TUMblue)
     plt.show()
```

### Comparing `commonroad-crime-0.2.0/setup.py` & `commonroad-crime-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='commonroad-crime',
-      version='0.2.0',
+      version='0.2.1',
       description='criticality measures of automated vehicles',
       keywords="criticality, autonomous driving",
       author='Yuanfei Lin, Oliver Specht, Ivana Peneva',
       author_email='yuanfei.lin@tum.de',
       license='BSD 3-Clause',
       packages=find_packages(),
       install_requires=[
           'commonroad-io>=2022.3',
           'commonroad-vehicle-models>=3.0.0',
-          'commonroad-route-planner>=2022.1',
+          'commonroad-route-planner>=2022.3',
           'commonroad-drivability-checker>=2022.2',
-          'matplotlib>=3.5.2'
+          'matplotlib>=3.5.2',
           'numpy>=1.23.0',
           'scipy>=1.7.3',
           'shapely<3.0.0,>=2.0.1',
           'omegaconf>=2.1.1',
           'casadi>=3.5.5, <3.6.0',
       ],
       extras_require={
```

