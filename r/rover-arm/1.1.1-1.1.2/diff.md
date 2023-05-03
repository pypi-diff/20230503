# Comparing `tmp/rover_arm-1.1.1.tar.gz` & `tmp/rover_arm-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rover_arm-1.1.1.tar", last modified: Tue May  2 23:51:56 2023, max compression
+gzip compressed data, was "rover_arm-1.1.2.tar", last modified: Wed May  3 00:01:11 2023, max compression
```

## Comparing `rover_arm-1.1.1.tar` & `rover_arm-1.1.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.803413 rover_arm-1.1.1/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-27 19:16:14.000000 rover_arm-1.1.1/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      188 2023-03-31 22:22:55.000000 rover_arm-1.1.1/.gitignore
--rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.1.1/MANIFEST.in
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-02 23:51:56.803259 rover_arm-1.1.1/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-03-31 23:16:16.000000 rover_arm-1.1.1/README.md
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.777995 rover_arm-1.1.1/rover_arm/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-31 06:14:48.000000 rover_arm-1.1.1/rover_arm/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      231 2023-04-27 19:25:40.000000 rover_arm-1.1.1/rover_arm/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.779411 rover_arm-1.1.1/rover_arm/data/
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.779825 rover_arm-1.1.1/rover_arm/data/meshes/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/.DS_Store
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.783124 rover_arm-1.1.1/rover_arm/data/meshes/collision/
--rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link0.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link7.obj
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.799997 rover_arm-1.1.1/rover_arm/data/meshes/visual/
--rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/colors.png
--rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/finger.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/hand.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link1.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link2.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link3.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link4.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link5.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/panda.urdf
--rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/rover_arm.xml
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.802779 rover_arm-1.1.1/rover_arm/envs/
--rw-r--r--   0 saiphani724   (501) staff       (20)      243 2023-03-30 23:20:23.000000 rover_arm-1.1.1/rover_arm/envs/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.803046 rover_arm-1.1.1/rover_arm/envs/__pycache__/
--rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.1.1/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)     7028 2023-05-02 23:39:25.000000 rover_arm-1.1.1/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)    11080 2023-05-02 23:51:32.000000 rover_arm-1.1.1/rover_arm/envs/roverarm_env.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.1.1/rover_arm/envs/roverarm_env_arrange.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.1.1/rover_arm/envs/roverarm_env_place.py
--rw-r--r--   0 saiphani724   (501) staff       (20)     2366 2023-04-27 20:10:52.000000 rover_arm-1.1.1/rover_arm/keyboard_control.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.778770 rover_arm-1.1.1/rover_arm.egg-info/
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     1740 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/SOURCES.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/dependency_links.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       27 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/requires.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/top_level.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-05-02 23:51:56.803467 rover_arm-1.1.1/setup.cfg
--rw-r--r--   0 saiphani724   (501) staff       (20)      570 2023-05-02 23:51:52.000000 rover_arm-1.1.1/setup.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:01:11.034361 rover_arm-1.1.2/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-27 19:16:14.000000 rover_arm-1.1.2/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      188 2023-03-31 22:22:55.000000 rover_arm-1.1.2/.gitignore
+-rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.1.2/MANIFEST.in
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-03 00:01:11.034192 rover_arm-1.1.2/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-03-31 23:16:16.000000 rover_arm-1.1.2/README.md
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:01:11.005221 rover_arm-1.1.2/rover_arm/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-31 06:14:48.000000 rover_arm-1.1.2/rover_arm/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      231 2023-04-27 19:25:40.000000 rover_arm-1.1.2/rover_arm/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:01:11.007015 rover_arm-1.1.2/rover_arm/data/
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:01:11.007430 rover_arm-1.1.2/rover_arm/data/meshes/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/.DS_Store
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:01:11.010615 rover_arm-1.1.2/rover_arm/data/meshes/collision/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/link0.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/collision/link7.obj
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:01:11.027519 rover_arm-1.1.2/rover_arm/data/meshes/visual/
+-rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/colors.png
+-rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/finger.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/hand.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link1.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link2.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link3.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link4.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link5.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/meshes/visual/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/panda.urdf
+-rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.1.2/rover_arm/data/rover_arm.xml
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:01:11.033484 rover_arm-1.1.2/rover_arm/envs/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      243 2023-03-30 23:20:23.000000 rover_arm-1.1.2/rover_arm/envs/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:01:11.033937 rover_arm-1.1.2/rover_arm/envs/__pycache__/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.1.2/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)     7093 2023-05-02 23:58:57.000000 rover_arm-1.1.2/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11164 2023-05-02 23:58:37.000000 rover_arm-1.1.2/rover_arm/envs/roverarm_env.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.1.2/rover_arm/envs/roverarm_env_arrange.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.1.2/rover_arm/envs/roverarm_env_place.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2366 2023-04-27 20:10:52.000000 rover_arm-1.1.2/rover_arm/keyboard_control.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:01:11.006498 rover_arm-1.1.2/rover_arm.egg-info/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-03 00:01:10.000000 rover_arm-1.1.2/rover_arm.egg-info/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1740 2023-05-03 00:01:10.000000 rover_arm-1.1.2/rover_arm.egg-info/SOURCES.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-05-03 00:01:10.000000 rover_arm-1.1.2/rover_arm.egg-info/dependency_links.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       27 2023-05-03 00:01:10.000000 rover_arm-1.1.2/rover_arm.egg-info/requires.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-05-03 00:01:10.000000 rover_arm-1.1.2/rover_arm.egg-info/top_level.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-05-03 00:01:11.034411 rover_arm-1.1.2/setup.cfg
+-rw-r--r--   0 saiphani724   (501) staff       (20)      570 2023-05-03 00:00:59.000000 rover_arm-1.1.2/setup.py
```

### Comparing `rover_arm-1.1.1/.DS_Store` & `rover_arm-1.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/PKG-INFO` & `rover_arm-1.1.2/rover_arm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rover_arm
-Version: 1.1.1
+Name: rover-arm
+Version: 1.1.2
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.1.1/README.md` & `rover_arm-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/.DS_Store` & `rover_arm-1.1.2/rover_arm/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/.DS_Store` & `rover_arm-1.1.2/rover_arm/data/meshes/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/finger.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/hand.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/link0.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/link0.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/link1.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/link2.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/link3.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/link4.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/link5.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/link6.mtl` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/link6.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/collision/link7.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/collision/link7.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/colors.png` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/colors.png`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/finger.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/hand.mtl` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/hand.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/hand.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link1.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link2.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link3.mtl` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link3.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link3.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link4.mtl` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link4.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link4.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link5.mtl` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link5.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link5.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link6.mtl` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/meshes/visual/link6.obj` & `rover_arm-1.1.2/rover_arm/data/meshes/visual/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/panda.urdf` & `rover_arm-1.1.2/rover_arm/data/panda.urdf`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/data/rover_arm.xml` & `rover_arm-1.1.2/rover_arm/data/rover_arm.xml`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc` & `rover_arm-1.1.2/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue May  2 23:38:54 2023 UTC, .py size: 11032 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,440 +1,444 @@
-00000000: 610d 0d0a 0000 0000 0e9f 5164 182b 0000  a.........Qd.+..
+00000000: 610d 0d0a 0000 0000 ada3 5164 9c2b 0000  a.........Qd.+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6402 6c00 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6401 6c07 5a07 6400  m.Z...d.d.l.Z.d.
 00000060: 6401 6c08 5a09 6400 6401 6c0a 5a0a 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c0b 5a0b 6400 6401 6c0c 5a0d 6400  d.l.Z.d.d.l.Z.d.
 00000080: 6401 6c0e 5a0e 6400 6401 6c0f 5a0f 4700  d.l.Z.d.d.l.Z.G.
 00000090: 6404 6405 8400 6405 6501 6a10 8303 5a11  d.d...d.e.j...Z.
 000000a0: 6401 5300 2906 e900 0000 004e 2903 da05  d.S.)......N)...
 000000b0: 6572 726f 72da 0673 7061 6365 73da 0575  error..spaces..u
 000000c0: 7469 6c73 2901 da07 7365 6564 696e 6763  tils)...seedingc
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000e0: 0600 0000 4000 0000 735c 0000 0065 005a  ....@...s\...e.Z
-000000f0: 0164 005a 0264 0164 0264 0367 0269 015a  .d.Z.d.d.d.g.i.Z
-00000100: 0364 0364 0464 0565 04a0 05a1 0064 0664  .d.d.d.e.....d.d
-00000110: 0666 0664 0764 0884 015a 0664 0964 0a84  .f.d.d...Z.d.d..
-00000120: 005a 0764 0b64 0c84 005a 0864 1464 0e64  .Z.d.d...Z.d.d.d
-00000130: 0f84 015a 0964 1064 1184 005a 0a64 1264  ...Z.d.d...Z.d.d
-00000140: 1384 005a 0b64 0d53 0029 15da 0b52 6f76  ...Z.d.S.)...Rov
-00000150: 6572 4172 6d45 6e76 7a0c 7265 6e64 6572  erArmEnvz.render
-00000160: 2e6d 6f64 6573 da05 6875 6d61 6eda 0972  .modes..human..r
-00000170: 6762 5f61 7272 6179 6910 2700 0046 69e0  gb_arrayi.'..Fi.
-00000180: 0100 0063 0700 0000 0000 0000 0000 0000  ...c............
-00000190: 0800 0000 0f00 0000 4300 0000 7368 0100  ........C...sh..
-000001a0: 007c 017c 005f 007c 037c 005f 0164 017c  .|.|._.|.|._.d.|
-000001b0: 005f 027c 047c 005f 037c 027c 005f 047c  ._.|.|._.|.|._.|
-000001c0: 057c 005f 057c 067c 005f 067c 006a 0064  .|._.|.|._.|.j.d
-000001d0: 026b 0272 6a74 07a0 0874 076a 09a1 017d  .k.rjt...t.j...}
-000001e0: 077c 0764 036b 0072 5474 07a0 0874 076a  .|.d.k.rTt...t.j
-000001f0: 0aa1 017d 0774 07a0 0b64 0464 0564 0667  ...}.t...d.d.d.g
-00000200: 0064 07a2 01a1 0401 006e 0c74 07a0 0874  .d.......n.t...t
-00000210: 076a 0ca1 0101 0064 087c 005f 0d64 097c  .j.....d.|._.d.|
-00000220: 005f 0e64 0a7c 005f 0f67 0064 0ba2 017c  ._.d.|._.g.d...|
-00000230: 005f 1074 076a 0b7c 006a 0d7c 006a 0e7c  ._.t.j.|.j.|.j.|
-00000240: 006a 0f7c 006a 1064 0c8d 0401 0074 11a0  .j.|.j.d.....t..
-00000250: 1274 13a0 1464 0d67 0164 0e14 00a1 0174  .t...d.g.d.....t
-00000260: 13a0 1464 0f67 0164 0e14 00a1 01a1 027c  ...d.g.d.......|
-00000270: 005f 1564 107c 005f 1674 11a0 1274 13a0  ._.d.|._.t...t..
-00000280: 147c 006a 160b 007c 006a 160b 0064 0d64  .|.j...|.j...d.d
-00000290: 0d64 0d64 0364 037c 006a 160b 007c 006a  .d.d.d.|.j...|.j
-000002a0: 160b 0064 0d67 0aa1 0174 13a0 147c 006a  ...d.g...t...|.j
-000002b0: 167c 006a 1664 0f64 0f64 0f64 1164 117c  .|.j.d.d.d.d.d.|
-000002c0: 006a 167c 006a 1664 0f67 0aa1 01a1 027c  .j.|.j.d.g.....|
-000002d0: 005f 1764 0364 1267 027c 005f 1867 0064  ._.d.d.g.|._.g.d
-000002e0: 13a2 017c 005f 1964 037c 005f 1a64 147c  ...|._.d.|._.d.|
-000002f0: 005f 1b64 157c 005f 1c64 167c 005f 1d64  ._.d.|._.d.|._.d
-00000300: 177c 005f 1e64 0053 0029 184e 6711 1111  .|._.d.S.).Ng...
-00000310: 1111 1171 3f72 0700 0000 7201 0000 0067  ...q?r....r....g
-00000320: cdcc cccc cccc f43f e9b4 0000 0069 d7ff  .......?.....i..
-00000330: ffff 2903 67a4 703d 0ad7 a3e0 3fe7 9a99  ..).g.p=....?...
-00000340: 9999 9999 c9bf 671f 85eb 51b8 1ed5 bfe9  ......g...Q.....
-00000350: 0300 0000 e766 6666 6666 66d6 bf69 ddff  .....ffffff..i..
-00000360: ffff 2903 6771 3d0a d7a3 70e5 3f72 0c00  ..).gq=...p.?r..
-00000370: 0000 679a 9999 9999 99c9 3f29 045a 0e63  ..g.......?).Z.c
-00000380: 616d 6572 6144 6973 7461 6e63 655a 0963  ameraDistanceZ.c
-00000390: 616d 6572 6159 6177 5a0b 6361 6d65 7261  ameraYawZ.camera
-000003a0: 5069 7463 68da 1463 616d 6572 6154 6172  Pitch..cameraTar
-000003b0: 6765 7450 6f73 6974 696f 6ee9 ffff ffff  getPosition.....
-000003c0: e906 0000 00e9 0100 0000 e905 0000 00e7  ................
-000003d0: ec51 b81e 85eb b13f e902 0000 0029 0472  .Q.....?.....).r
-000003e0: 1000 0000 720b 0000 00e9 0400 0000 7211  ....r.........r.
-000003f0: 0000 0067 3333 3333 3333 d33f 677b 14ae  ...g333333.?g{..
-00000400: 47e1 7a84 3fe9 c800 0000 e914 0000 0029  G.z.?..........)
-00000410: 1fda 0b72 656e 6465 725f 6d6f 6465 5a0b  ...render_modeZ.
-00000420: 5f69 7344 6973 6372 6574 655a 095f 7469  _isDiscreteZ._ti
-00000430: 6d65 5374 6570 da09 5f75 7264 6652 6f6f  meStep.._urdfRoo
-00000440: 74da 095f 6d61 7853 7465 7073 da06 5f77  t.._maxSteps.._w
-00000450: 6964 7468 da07 5f68 6569 6768 74da 0170  idth.._height..p
-00000460: da07 636f 6e6e 6563 74da 0d53 4841 5245  ..connect..SHARE
-00000470: 445f 4d45 4d4f 5259 da03 4755 49da 1a72  D_MEMORY..GUI..r
-00000480: 6573 6574 4465 6275 6756 6973 7561 6c69  esetDebugVisuali
-00000490: 7a65 7243 616d 6572 61da 0644 4952 4543  zerCamera..DIREC
-000004a0: 54da 095f 6361 6d5f 6469 7374 da08 5f63  T.._cam_dist.._c
-000004b0: 616d 5f79 6177 da0a 5f63 616d 5f70 6974  am_yaw.._cam_pit
-000004c0: 6368 da0d 5f63 616d 5f74 6172 6765 745f  ch.._cam_target_
-000004d0: 7072 0300 0000 da03 426f 78da 026e 70da  pr......Box..np.
-000004e0: 0561 7272 6179 da0c 6163 7469 6f6e 5f73  .array..action_s
-000004f0: 7061 6365 da08 626f 756e 6461 7279 da11  pace..boundary..
-00000500: 6f62 7365 7276 6174 696f 6e5f 7370 6163  observation_spac
-00000510: 65da 0f73 7465 6572 696e 675f 6a6f 696e  e..steering_join
-00000520: 7473 da0c 6472 6976 655f 6a6f 696e 7473  ts..drive_joints
-00000530: da0b 6a6f 696e 745f 7370 6565 64da 0963  ..joint_speed..c
-00000540: 5f72 6f6c 6c69 6e67 da06 635f 6472 6167  _rolling..c_drag
-00000550: da0a 635f 7468 726f 7474 6c65 da09 4d41  ..c_throttle..MA
-00000560: 585f 5350 4545 4429 08da 0473 656c 6672  X_SPEED)...selfr
-00000570: 1700 0000 5a08 6d61 7853 7465 7073 5a0a  ....Z.maxStepsZ.
-00000580: 6973 4469 7363 7265 7465 5a08 7572 6466  isDiscreteZ.urdf
-00000590: 526f 6f74 da05 7769 6474 68da 0668 6569  Root..width..hei
-000005a0: 6768 745a 0363 6964 a900 7236 0000 00fa  ghtZ.cid..r6....
-000005b0: 4e2f 5573 6572 732f 7361 6970 6861 6e69  N/Users/saiphani
-000005c0: 3732 342f 4465 736b 746f 702f 4169 2f52  724/Desktop/Ai/R
-000005d0: 6f62 6f74 6963 732f 526f 7665 7241 726d  obotics/RoverArm
-000005e0: 2f72 6f76 6572 5f61 726d 2f65 6e76 732f  /rover_arm/envs/
-000005f0: 726f 7665 7261 726d 5f65 6e76 2e70 79da  roverarm_env.py.
-00000600: 085f 5f69 6e69 745f 5f11 0000 0073 3800  .__init__....s8.
-00000610: 0000 0002 0601 0601 0601 0601 0601 0601  ................
-00000620: 0601 0a01 0c01 0801 0c01 1602 0c01 0601  ................
-00000630: 0601 0601 0a02 1a01 2601 0601 5a03 0a01  ........&...Z...
-00000640: 0a02 0602 0601 0602 0602 7a14 526f 7665  ..........z.Rove
-00000650: 7241 726d 456e 762e 5f5f 696e 6974 5f5f  rArmEnv.__init__
-00000660: 6301 0000 0000 0000 0000 0000 000f 0000  c...............
-00000670: 0008 0000 0043 0000 0073 1002 0000 6401  .....C...s....d.
-00000680: 7c00 5f00 7401 a002 a100 0100 7401 a003  |._.t.......t...
-00000690: 7401 6a04 6401 a102 0100 7401 a005 6401  t.j.d.....t...d.
-000006a0: 6401 6402 a103 0100 7401 6a06 7407 6a08  d.d.....t.j.t.j.
-000006b0: a009 7c00 6a0a 6403 a102 6700 6404 a201  ..|.j.d...g.d...
-000006c0: 6405 8d02 7d01 6700 6406 a201 7d02 740b  d...}.g.d...}.t.
-000006d0: 6a0c a00d 740c a00e 6407 6408 a102 740c  j...t...d.d...t.
-000006e0: a00e 6409 640a a102 6702 a101 7d03 740c  ..d.d...g...}.t.
-000006f0: a00e 6407 640b a102 7d04 740f a010 a100  ..d.d...}.t.....
-00000700: 6401 1900 640c 1700 7d05 7401 6a06 7c05  d...d...}.t.j.|.
-00000710: 640d 1700 7c03 7c04 640e 6703 6405 8d02  d...|.|.d.g.d...
-00000720: 7c00 5f11 7412 640f 6410 8302 4400 5d1c  |._.t.d.d...D.].
-00000730: 7d06 7401 a013 7c00 6a11 7c06 7c02 7c06  }.t...|.j.|.|.|.
-00000740: 640f 1800 1900 a103 0100 71b0 7401 a013  d.........q.t...
-00000750: 7c00 6a11 6411 6412 a103 0100 7401 a013  |.j.d.d.....t...
-00000760: 7c00 6a11 6413 6412 a103 0100 7401 6a06  |.j.d.d.....t.j.
-00000770: 7407 6a08 a009 7c00 6a0a 6414 a102 6700  t.j...|.j.d...g.
-00000780: 6415 a201 6416 6417 8d03 7d07 7401 6a06  d...d.d...}.t.j.
-00000790: 7407 6a08 a009 7c00 6a0a 6418 a102 6700  t.j...|.j.d...g.
-000007a0: 6419 a201 6416 6417 8d03 7d08 740c a00e  d...d.d...}.t...
-000007b0: 641a 6416 a102 740c a00e 641b 641c a102  d.d...t...d.d...
-000007c0: 641d 6703 7d09 7401 6a06 7407 6a08 a009  d.g.}.t.j.t.j...
-000007d0: 7c00 6a0a 641e a102 7c09 641f 6417 8d03  |.j.d...|.d.d...
-000007e0: 7c00 5f14 7401 a015 7c00 6a11 6401 a102  |._.t...|.j.d...
-000007f0: 6401 1900 6400 640a 8502 1900 7d0a 7401  d...d.d.....}.t.
-00000800: a015 7c00 6a11 6420 a102 6401 1900 7d0b  ..|.j.d ..d...}.
-00000810: 7401 a016 7c00 6a11 6411 a102 6401 1900  t...|.j.d...d...
-00000820: 7401 a016 7c00 6a11 6413 a102 6401 1900  t...|.j.d...d...
-00000830: 6602 7d0c 7401 a017 7c00 6a14 a101 5c02  f.}.t...|.j...\.
-00000840: 7d09 7d0d 7c0a 7c0b 1700 7c0c 1700 7418  }.}.|.|...|...t.
-00000850: 7c09 8301 1700 7c00 5f19 7401 a003 7401  |.....|._.t...t.
-00000860: 6a04 6421 a102 0100 7c0a 7c0b 7c0c 7c09  j.d!....|.|.|.|.
-00000870: 6422 9c04 7d0e 740b a01a 7c00 6a19 a101  d"..}.t...|.j...
-00000880: a01b 740b 6a1c a101 7c0e 6602 5300 2923  ..t.j...|.f.S.)#
-00000890: 4e72 0100 0000 69f6 ffff ff7a 0a70 6c61  Nr....i....z.pla
-000008a0: 6e65 2e75 7264 6629 0372 0100 0000 7201  ne.urdf).r....r.
-000008b0: 0000 00e7 cdcc cccc cccc e4bf 2901 da0c  ............)...
-000008c0: 6261 7365 506f 7369 7469 6f6e 2909 7201  basePosition).r.
-000008d0: 0000 0067 85eb 51b8 1e85 cbbf 7201 0000  ...g..Q.....r...
-000008e0: 0067 8fc2 f528 5c8f 04c0 7201 0000 00e7  .g...(\...r.....
-000008f0: 0c02 2b87 16d9 0240 723b 0000 00e7 7b14  ..+....@r;....{.
-00000900: ae47 e17a b43f 723c 0000 0072 0e00 0000  .G.z.?r<...r....
-00000910: 6733 3333 3333 33d3 bf67 0000 0000 0000  g333333..g......
-00000920: f43f 7213 0000 0067 0000 0000 0000 0440  .?r....g.......@
-00000930: 7a10 2f72 6f76 6572 5f61 726d 2f64 6174  z./rover_arm/dat
-00000940: 612f 7a0d 726f 7665 725f 6172 6d2e 786d  a/z.rover_arm.xm
-00000950: 6c67 0000 0000 0000 e0bf e907 0000 00e9  lg..............
-00000960: 0e00 0000 e910 0000 0072 1200 0000 e911  .........r......
-00000970: 0000 007a 1074 6162 6c65 2f74 6162 6c65  ...z.table/table
-00000980: 2e75 7264 6629 03e7 0000 0000 0000 e03f  .urdf).........?
-00000990: 7201 0000 0072 3900 0000 7241 0000 0029  r....r9...rA...)
-000009a0: 0272 3a00 0000 5a0d 676c 6f62 616c 5363  .r:...Z.globalSc
-000009b0: 616c 696e 677a 1174 7261 792f 7472 6179  alingz.tray/tray
-000009c0: 626f 782e 7572 6466 2903 67cd cccc cccc  box.urdf).g.....
-000009d0: ccdc 3f72 0100 0000 6771 3d0a d7a3 70d5  ..?r....gq=...p.
-000009e0: bf67 9a99 9999 9999 d93f 679a 9999 9999  .g.......?g.....
-000009f0: 99a9 bfe7 9a99 9999 9999 a93f 720a 0000  ...........?r...
-00000a00: 007a 1972 616e 646f 6d5f 7572 6466 732f  .z.random_urdfs/
-00000a10: 3030 302f 3030 302e 7572 6466 679a 9999  000/000.urdfg...
-00000a20: 9999 99e9 3fe9 1200 0000 7210 0000 00a9  ....?.....r.....
-00000a30: 04da 0b73 7461 7465 5f72 6f76 6572 da09  ...state_rover..
-00000a40: 7374 6174 655f 6172 6dda 0d73 7461 7465  state_arm..state
-00000a50: 5f66 696e 6765 7273 da0c 7374 6174 655f  _fingers..state_
-00000a60: 6f62 6a65 6374 291d da0c 7374 6570 5f63  object)...step_c
-00000a70: 6f75 6e74 6572 721c 0000 00da 0f72 6573  ounterr......res
-00000a80: 6574 5369 6d75 6c61 7469 6f6e da18 636f  etSimulation..co
-00000a90: 6e66 6967 7572 6544 6562 7567 5669 7375  nfigureDebugVisu
-00000aa0: 616c 697a 6572 da14 434f 565f 454e 4142  alizer..COV_ENAB
-00000ab0: 4c45 5f52 454e 4445 5249 4e47 da0a 7365  LE_RENDERING..se
-00000ac0: 7447 7261 7669 7479 da08 6c6f 6164 5552  tGravity..loadUR
-00000ad0: 4446 da02 6f73 da04 7061 7468 da04 6a6f  DF..os..path..jo
-00000ae0: 696e 7218 0000 0072 2700 0000 da06 7261  inr....r'.....ra
-00000af0: 6e64 6f6d da06 6368 6f69 6365 da07 756e  ndom..choice..un
-00000b00: 6966 6f72 6dda 0473 6974 65da 0f67 6574  iform..site..get
-00000b10: 7369 7465 7061 636b 6167 6573 da0b 726f  sitepackages..ro
-00000b20: 7665 7261 726d 5569 64da 0572 616e 6765  verarmUid..range
-00000b30: da0f 7265 7365 744a 6f69 6e74 5374 6174  ..resetJointStat
-00000b40: 65da 096f 626a 6563 7455 6964 da0c 6765  e..objectUid..ge
-00000b50: 744c 696e 6b53 7461 7465 da0d 6765 744a  tLinkState..getJ
-00000b60: 6f69 6e74 5374 6174 65da 1d67 6574 4261  ointState..getBa
-00000b70: 7365 506f 7369 7469 6f6e 416e 644f 7269  sePositionAndOri
-00000b80: 656e 7461 7469 6f6e da05 7475 706c 65da  entation..tuple.
-00000b90: 0b6f 6273 6572 7661 7469 6f6e 7228 0000  .observationr(..
-00000ba0: 00da 0661 7374 7970 65da 0766 6c6f 6174  ...astype..float
-00000bb0: 3332 290f 7233 0000 005a 0870 6c61 6e65  32).r3...Z.plane
-00000bc0: 5569 645a 0a72 6573 745f 706f 7365 735a  UidZ.rest_posesZ
-00000bd0: 0578 5f70 6f73 5a05 795f 706f 73da 0842  .x_posZ.y_pos..B
-00000be0: 4153 455f 4449 52da 0169 5a08 7461 626c  ASE_DIR..iZ.tabl
-00000bf0: 6555 6964 5a07 7472 6179 5569 6472 4800  eUidZ.trayUidrH.
-00000c00: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
-00000c10: 00da 015f da04 696e 666f 7236 0000 0072  ..._..infor6...r
-00000c20: 3600 0000 7237 0000 00da 0572 6573 6574  6...r7.....reset
-00000c30: 3800 0000 7334 0000 0000 0106 0108 010e  8...s4..........
-00000c40: 020e 021e 0208 0220 010c 0210 021a 030e  ....... ........
-00000c50: 011a 0110 0110 0220 0120 021a 011e 021a  ....... . ......
-00000c60: 0112 0124 0110 0216 020e 010e 017a 1152  ...$.........z.R
-00000c70: 6f76 6572 4172 6d45 6e76 2e72 6573 6574  overArmEnv.reset
-00000c80: 6302 0000 0000 0000 0000 0000 0022 0000  c............"..
-00000c90: 0008 0000 0003 0000 0073 5203 0000 7400  .........sR...t.
-00000ca0: a001 6401 7402 6a03 0b00 7402 6a03 6402  ..d.t.j...t.j.d.
-00000cb0: 1b00 6703 a101 7d02 6403 8900 8700 6601  ..g...}.d.....f.
-00000cc0: 6404 6405 8408 7c01 6406 6407 8502 1900  d.d...|.d.d.....
-00000cd0: 4400 8301 5c03 7d03 7d04 7d05 7c01 6407  D...\.}.}.}.|.d.
-00000ce0: 1900 7d06 7404 a005 7c06 6408 6409 6702  ..}.t...|.d.d.g.
-00000cf0: 640a 640b 6702 a103 7d06 7400 a006 8801  d.d.g...}.t.....
-00000d00: 6a07 640c a102 7d07 7c07 640a 1900 7d08  j.d...}.|.d...}.
-00000d10: 7c08 640a 1900 7c03 1700 7c08 6409 1900  |.d...|...|.d...
-00000d20: 7c04 1700 7c08 6406 1900 7c05 1700 6703  |...|.d...|...g.
-00000d30: 7d09 7400 a008 8801 6a07 640c 7c09 7c02  }.t.....j.d.|.|.
-00000d40: a104 7d0a 7c0a 6400 640d 8502 1900 7c0a  ..}.|.d.d.....|.
-00000d50: 640d 640e 8502 1900 0200 7d0b 7d0c 7400  d.d.......}.}.t.
-00000d60: a009 8801 6a07 740a 740b 640f 6410 8302  ....j.t.t.d.d...
-00000d70: 8301 6411 6412 6702 1700 7400 6a0c 740a  ..d.d.g...t.j.t.
-00000d80: 7c0c 8301 6406 7c06 6701 1400 1700 a104  |...d.|.g.......
-00000d90: 0100 7c01 6400 6406 8502 1900 5c02 7d0d  ..|.d.d.....\.}.
-00000da0: 7d0e 740d 740e 7c0d 6408 8302 6409 8302  }.t.t.|.d...d...
-00000db0: 7d0d 7404 a005 7c0e 6408 6409 6702 6413  }.t...|.d.d.g.d.
-00000dc0: 6414 6702 a103 7d0e 7400 6a09 8801 6a07  d.g...}.t.j...j.
-00000dd0: 8801 6a0f 7400 6a0c 7c0e 6701 6406 1400  ..j.t.j.|.g.d...
-00000de0: 6415 8d04 0100 8801 6a10 0b00 8801 6a10  d.......j.....j.
-00000df0: 8801 6a11 1400 8801 6a12 1700 1400 7d0f  ..j.....j.....}.
-00000e00: 8801 6a13 7c0d 1400 7c0f 1700 7d10 8801  ..j.|...|...}...
-00000e10: 6a10 6416 7c10 1400 1700 8801 5f10 740d  j.d.|......._.t.
-00000e20: 740e 8801 6a10 8801 6a14 0b00 8302 8801  t...j...j.......
-00000e30: 6a14 8302 8801 5f10 7400 6a09 8801 6a07  j....._.t.j...j.
-00000e40: 8801 6a15 7400 6a16 8801 6a10 6701 6417  ..j.t.j...j.g.d.
-00000e50: 1400 6418 6701 6417 1400 6419 8d05 0100  ..d.g.d...d.....
-00000e60: 7400 a017 8801 6a18 a101 5c02 7d11 7d12  t.....j...\.}.}.
-00000e70: 7400 a019 a100 0100 7400 a017 8801 6a18  t.......t.....j.
-00000e80: a101 5c02 7d13 7d12 7400 a006 8801 6a07  ..\.}.}.t.....j.
-00000e90: 640a a102 640a 1900 6400 6406 8502 1900  d...d...d.d.....
-00000ea0: 7d14 7400 a006 8801 6a07 640c a102 640a  }.t.....j.d...d.
-00000eb0: 1900 7d15 7400 a01a 8801 6a07 6411 a102  ..}.t.....j.d...
-00000ec0: 640a 1900 7400 a01a 8801 6a07 6412 a102  d...t.....j.d...
-00000ed0: 640a 1900 6602 7d16 641a 5c02 7d17 7d18  d...f.}.d.\.}.}.
-00000ee0: 7c13 6406 1900 640a 6b04 9002 725a 6409  |.d...d.k...rZd.
-00000ef0: 7d19 641b 7d17 6e74 7404 a01b 7404 a01c  }.d.}.ntt...t...
-00000f00: 7c08 a101 7404 a01c 7c11 a101 1800 a101  |...t...|.......
-00000f10: 5c03 7d1a 7d1b 7d1c 7404 a01b 7404 a01c  \.}.}.}.t...t...
-00000f20: 7c15 a101 7404 a01c 7c13 a101 1800 a101  |...t...|.......
-00000f30: 5c03 7d1d 7d1e 7d1f 7c1a 7c1d 1800 7c1b  \.}.}.}.|.|...|.
-00000f40: 1700 7c1e 1800 7c1c 1700 7c1f 1800 7d19  ..|...|...|...}.
-00000f50: 741b 7c19 8301 641c 6b04 9002 72ca 7c19  t.|...d.k...r.|.
-00000f60: 6418 1b00 7d19 6e04 640a 7d19 8801 0400  d...}.n.d.}.....
-00000f70: 6a1d 6409 3700 0200 5f1d 8701 6601 641d  j.d.7..._...f.d.
-00000f80: 641e 8408 7d20 7c20 7c14 8301 9002 73fa  d...} | |.....s.
-00000f90: 6408 7d19 641b 7d17 8801 6a1d 8801 6a1e  d.}.d.}...j...j.
-00000fa0: 6b04 9003 7210 640a 7d19 641b 7d18 7c14  k...r.d.}.d.}.|.
-00000fb0: 7c15 1700 7c16 1700 741f 7c13 8301 1700  |...|...t.|.....
-00000fc0: 8801 5f20 7c14 7c15 7c16 7c13 641f 9c04  .._ |.|.|.|.d...
-00000fd0: 7d21 7404 a01c 8801 6a20 a101 a021 7404  }!t.....j ...!t.
-00000fe0: 6a22 a101 7c19 7c17 7c18 7c21 6605 5300  j"..|.|.|.|!f.S.
-00000ff0: 2920 4e67 0000 0000 0000 0000 6700 0000  ) Ng........g...
-00001000: 0000 0000 4072 4200 0000 6301 0000 0000  ....@rB...c.....
-00001010: 0000 0000 0000 0002 0000 0004 0000 0013  ................
-00001020: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
-00001030: 7c01 8800 1400 9102 7104 5300 7236 0000  |.......q.S.r6..
-00001040: 0072 3600 0000 2902 da02 2e30 da01 7829  .r6...)....0..x)
-00001050: 01da 0264 7672 3600 0000 7237 0000 00da  ...dvr6...r7....
-00001060: 0a3c 6c69 7374 636f 6d70 3e65 0000 00f3  .<listcomp>e....
-00001070: 0000 0000 7a24 526f 7665 7241 726d 456e  ....z$RoverArmEn
-00001080: 762e 7374 6570 2e3c 6c6f 6361 6c73 3e2e  v.step.<locals>.
-00001090: 3c6c 6973 7463 6f6d 703e 7213 0000 0072  <listcomp>r....r
-000010a0: 1100 0000 720e 0000 0072 1000 0000 7201  ....r....r....r.
-000010b0: 0000 0072 1200 0000 7243 0000 0072 0f00  ...r....rC...r..
-000010c0: 0000 e90d 0000 0072 3d00 0000 723e 0000  .......r=...r>..
-000010d0: 0072 3f00 0000 7240 0000 0067 3333 3333  .r?...r@...g3333
-000010e0: 3333 e3bf 6733 3333 3333 33e3 3f29 02da  33..g333333.?)..
-000010f0: 0b63 6f6e 7472 6f6c 4d6f 6465 5a0f 7461  .controlModeZ.ta
-00001100: 7267 6574 506f 7369 7469 6f6e 7367 1111  rgetPositionsg..
-00001110: 1111 1111 a13f 7214 0000 00e9 0a00 0000  .....?r.........
-00001120: 2905 5a0c 626f 6479 556e 6971 7565 4964  ).Z.bodyUniqueId
-00001130: 5a0c 6a6f 696e 7449 6e64 6963 6573 726d  Z.jointIndicesrm
-00001140: 0000 005a 1074 6172 6765 7456 656c 6f63  ...Z.targetVeloc
-00001150: 6974 6965 735a 0666 6f72 6365 7329 0246  itiesZ.forces).F
-00001160: 4654 67fc a9f1 d24d 6250 3f63 0100 0000  FTg....MbP?c....
-00001170: 0000 0000 0000 0000 0400 0000 0200 0000  ................
-00001180: 1300 0000 733c 0000 007c 005c 027d 017d  ....s<...|.\.}.}
-00001190: 027c 0188 006a 000b 006b 046f 1c7c 0188  .|...j...k.o.|..
-000011a0: 006a 006b 007d 037c 036f 367c 0288 006a  .j.k.}.|.o6|...j
-000011b0: 000b 006b 046f 367c 0288 006a 006b 007d  ...k.o6|...j.k.}
-000011c0: 037c 0353 00a9 014e 2901 722a 0000 0029  .|.S...N).r*...)
-000011d0: 0472 4500 0000 da02 7278 5a02 7279 5a07  .rE.....rxZ.ryZ.
-000011e0: 696e 426f 756e 64a9 0172 3300 0000 7236  inBound..r3...r6
-000011f0: 0000 0072 3700 0000 da06 696e 4761 6d65  ...r7.....inGame
-00001200: ad00 0000 7308 0000 0000 0108 0116 011a  ....s...........
-00001210: 017a 2052 6f76 6572 4172 6d45 6e76 2e73  .z RoverArmEnv.s
-00001220: 7465 702e 3c6c 6f63 616c 733e 2e69 6e47  tep.<locals>.inG
-00001230: 616d 6572 4400 0000 2923 721c 0000 00da  amerD...)#r.....
-00001240: 1667 6574 5175 6174 6572 6e69 6f6e 4672  .getQuaternionFr
-00001250: 6f6d 4575 6c65 72da 046d 6174 68da 0270  omEuler..math..p
-00001260: 6972 2700 0000 da06 696e 7465 7270 725b  ir'.....interpr[
-00001270: 0000 0072 5700 0000 da1a 6361 6c63 756c  ...rW.....calcul
-00001280: 6174 6549 6e76 6572 7365 4b69 6e65 6d61  ateInverseKinema
-00001290: 7469 6373 da19 7365 744a 6f69 6e74 4d6f  tics..setJointMo
-000012a0: 746f 7243 6f6e 7472 6f6c 4172 7261 79da  torControlArray.
-000012b0: 046c 6973 7472 5800 0000 da10 504f 5349  .listrX.....POSI
-000012c0: 5449 4f4e 5f43 4f4e 5452 4f4c da03 6d69  TION_CONTROL..mi
-000012d0: 6eda 036d 6178 722c 0000 0072 2e00 0000  n..maxr,...r....
-000012e0: 7230 0000 0072 2f00 0000 7231 0000 0072  r0...r/...r1...r
-000012f0: 3200 0000 722d 0000 00da 1056 454c 4f43  2...r-.....VELOC
-00001300: 4954 595f 434f 4e54 524f 4c72 5d00 0000  ITY_CONTROLr]...
-00001310: 725a 0000 00da 0e73 7465 7053 696d 756c  rZ.....stepSimul
-00001320: 6174 696f 6e72 5c00 0000 da03 6162 7372  ationr\.....absr
-00001330: 2800 0000 7249 0000 0072 1900 0000 725e  (...rI...r....r^
-00001340: 0000 0072 5f00 0000 7260 0000 0072 6100  ...r_...r`...ra.
-00001350: 0000 2922 7233 0000 00da 0661 6374 696f  ..)"r3.....actio
-00001360: 6e5a 0b6f 7269 656e 7461 7469 6f6e 5a04  nZ.orientationZ.
-00001370: 6478 5f61 5a04 6479 5f61 5a04 647a 5f61  dx_aZ.dy_aZ.dz_a
-00001380: 5a07 6669 6e67 6572 735a 0b63 7572 7265  Z.fingersZ.curre
-00001390: 6e74 506f 7365 5a0f 6375 7272 656e 7450  ntPoseZ.currentP
-000013a0: 6f73 6974 696f 6e5a 0b6e 6577 506f 7369  ositionZ.newPosi
-000013b0: 7469 6f6e 5a0a 6a6f 696e 7450 6f73 6573  tionZ.jointPoses
-000013c0: 5a10 6a6f 696e 7450 6f73 6573 5f72 6f76  Z.jointPoses_rov
-000013d0: 6572 5a0e 6a6f 696e 7450 6f73 6573 5f61  erZ.jointPoses_a
-000013e0: 726d 5a08 7468 726f 7474 6c65 5a0e 7374  rmZ.throttleZ.st
-000013f0: 6565 7269 6e67 5f61 6e67 6c65 5a08 6672  eering_angleZ.fr
-00001400: 6963 7469 6f6e 5a0c 6163 6365 6c65 7261  ictionZ.accelera
-00001410: 7469 6f6e 5a11 7374 6174 655f 6f62 6a65  tionZ.state_obje
-00001420: 6374 5f70 7265 7672 6400 0000 7248 0000  ct_prevrd...rH..
-00001430: 0072 4500 0000 7246 0000 0072 4700 0000  .rE...rF...rG...
-00001440: da0a 7465 726d 696e 6174 6564 da09 7472  ..terminated..tr
-00001450: 756e 6361 7465 64da 0672 6577 6172 64da  uncated..reward.
-00001460: 0278 305a 0279 305a 027a 30da 0278 31da  .x0Z.y0Z.z0..x1.
-00001470: 0279 31da 027a 3172 7200 0000 7265 0000  .y1..z1rr...re..
-00001480: 0072 3600 0000 2902 7269 0000 0072 3300  .r6...).ri...r3.
-00001490: 0000 7237 0000 00da 0473 7465 7061 0000  ..r7.....stepa..
-000014a0: 0073 7a00 0000 0002 1a01 0401 2001 0801  .sz......... ...
-000014b0: 1602 0e02 0802 0a01 0a01 0afe 0403 1201  ................
-000014c0: 1a01 3402 1004 1001 1604 0c01 0401 08fe  ..4.............
-000014d0: 0606 1001 04ff 0603 0e03 1002 1a04 0401  ................
-000014e0: 0401 0401 0401 0a01 08fb 0607 1002 0802  ................
-000014f0: 1001 1a01 1201 2402 0801 0e01 0401 0602  ......$.........
-00001500: 2001 2001 1801 0e01 0a02 0402 0e01 0c06   . .............
-00001510: 0a01 0401 0402 0e01 0401 0402 1601 0e02  ................
-00001520: 7a10 526f 7665 7241 726d 456e 762e 7374  z.RoverArmEnv.st
-00001530: 6570 4e63 0300 0000 0000 0000 0000 0000  epNc............
-00001540: 0c00 0000 0800 0000 4300 0000 7342 0100  ........C...sB..
-00001550: 007c 0164 006b 0273 107c 0264 006b 0272  .|.d.k.s.|.d.k.r
-00001560: 1c7c 006a 007d 017c 006a 017d 027c 006a  .|.j.}.|.j.}.|.j
-00001570: 0264 016b 0372 2a64 0053 0074 036a 047c  .d.k.r*d.S.t.j.|
-00001580: 006a 057c 006a 067c 006a 077c 006a 0864  .j.|.j.|.j.|.j.d
-00001590: 0264 0364 048d 067d 0374 036a 0467 0064  .d.d...}.t.j.g.d
-000015a0: 05a2 0164 0664 0764 0864 0264 0364 048d  ...d.d.d.d.d.d..
-000015b0: 067d 0474 036a 0964 0974 0a7c 0183 017c  .}.t.j.d.t.|...|
-000015c0: 021b 0064 0a64 0b64 0c8d 047d 0574 036a  ...d.d.d...}.t.j
-000015d0: 0b7c 017c 027c 037c 0574 036a 0c64 0d8d  .|.|.|.|.t.j.d..
-000015e0: 055c 057d 067d 067d 077d 067d 0674 036a  .\.}.}.}.}.}.t.j
-000015f0: 0b7c 017c 027c 047c 0574 036a 0c64 0d8d  .|.|.|.|.t.j.d..
-00001600: 055c 057d 067d 067d 087d 067d 0674 0d6a  .\.}.}.}.}.}.t.j
-00001610: 0e7c 0774 0d6a 0f64 0e8d 027d 0974 0da0  .|.t.j.d...}.t..
-00001620: 107c 097c 027c 0164 0f66 03a1 0264 0064  .|.|.|.d.f...d.d
-00001630: 0085 0264 0064 0085 0264 0064 1085 0266  ...d.d...d.d...f
-00001640: 0319 007d 0974 0d6a 0e7c 0874 0d6a 0f64  ...}.t.j.|.t.j.d
-00001650: 0e8d 027d 0a74 0da0 107c 0a7c 027c 0164  ...}.t...|.|.|.d
-00001660: 0f66 03a1 0264 0064 0085 0264 0064 0085  .f...d.d...d.d..
-00001670: 0264 0064 1085 0266 0319 007d 0a74 0d6a  .d.d...f...}.t.j
-00001680: 117c 097c 0a66 0264 0364 118d 027d 0b7c  .|.|.f.d.d...}.|
-00001690: 0b53 0029 124e 7208 0000 0072 0100 0000  .S.).Nr....r....
-000016a0: 7213 0000 0029 0672 0d00 0000 da08 6469  r....).r......di
-000016b0: 7374 616e 6365 5a03 7961 775a 0570 6974  stanceZ.yawZ.pit
-000016c0: 6368 da04 726f 6c6c 5a0b 7570 4178 6973  ch..rollZ.upAxis
-000016d0: 496e 6465 7829 03e7 6666 6666 6666 e63f  Index)..ffffff.?
-000016e0: 7201 0000 0072 4200 0000 728b 0000 00e9  r....rB...r.....
-000016f0: 5a00 0000 69ba ffff ffe9 3c00 0000 679a  Z...i.....<...g.
-00001700: 9999 9999 99b9 3f67 0000 0000 0000 5940  ......?g......Y@
-00001710: 2904 5a03 666f 76da 0661 7370 6563 745a  ).Z.fov..aspectZ
-00001720: 076e 6561 7256 616c 5a06 6661 7256 616c  .nearValZ.farVal
-00001730: 2905 7234 0000 0072 3500 0000 5a0a 7669  ).r4...r5...Z.vi
-00001740: 6577 4d61 7472 6978 5a10 7072 6f6a 6563  ewMatrixZ.projec
-00001750: 7469 6f6e 4d61 7472 6978 5a08 7265 6e64  tionMatrixZ.rend
-00001760: 6572 6572 2901 da05 6474 7970 6572 1400  erer)...dtyper..
-00001770: 0000 720b 0000 0029 01da 0461 7869 7329  ..r....)...axis)
-00001780: 1272 1a00 0000 721b 0000 0072 1700 0000  .r....r....r....
-00001790: 721c 0000 00da 2163 6f6d 7075 7465 5669  r.....!computeVi
-000017a0: 6577 4d61 7472 6978 4672 6f6d 5961 7750  ewMatrixFromYawP
-000017b0: 6974 6368 526f 6c6c 7225 0000 0072 2200  itchRollr%...r".
-000017c0: 0000 7223 0000 0072 2400 0000 da1a 636f  ..r#...r$.....co
-000017d0: 6d70 7574 6550 726f 6a65 6374 696f 6e4d  mputeProjectionM
-000017e0: 6174 7269 7846 4f56 da05 666c 6f61 74da  atrixFOV..float.
-000017f0: 0e67 6574 4361 6d65 7261 496d 6167 65da  .getCameraImage.
-00001800: 1945 525f 4255 4c4c 4554 5f48 4152 4457  .ER_BULLET_HARDW
-00001810: 4152 455f 4f50 454e 474c 7227 0000 0072  ARE_OPENGLr'...r
-00001820: 2800 0000 da05 7569 6e74 38da 0772 6573  (.....uint8..res
-00001830: 6861 7065 da0b 636f 6e63 6174 656e 6174  hape..concatenat
-00001840: 6529 0c72 3300 0000 7234 0000 0072 3500  e).r3...r4...r5.
-00001850: 0000 5a0c 7669 6577 5f6d 6174 7269 7831  ..Z.view_matrix1
-00001860: 5a0c 7669 6577 5f6d 6174 7269 7832 5a0b  Z.view_matrix2Z.
-00001870: 7072 6f6a 5f6d 6174 7269 7872 6400 0000  proj_matrixrd...
-00001880: 5a03 7078 315a 0370 7832 5a0a 7267 625f  Z.px1Z.px2Z.rgb_
-00001890: 6172 7261 7931 5a0a 7267 625f 6172 7261  array1Z.rgb_arra
-000018a0: 7932 7208 0000 0072 3600 0000 7236 0000  y2r....r6...r6..
-000018b0: 0072 3700 0000 da06 7265 6e64 6572 c100  .r7.....render..
-000018c0: 0000 7354 0000 0000 0710 0106 0106 010a  ..sT............
-000018d0: 0104 0108 0104 0104 0104 0102 0102 fb06  ................
-000018e0: 060a 0102 0102 0102 0102 0102 fb06 0606  ................
-000018f0: 010a 0102 0102 fd06 0506 0102 0102 0102  ................
-00001900: 0104 fc10 0606 0102 0102 0102 0104 fc10  ................
-00001910: 0610 0128 0210 0128 0312 027a 1252 6f76  ...(...(...z.Rov
-00001920: 6572 4172 6d45 6e76 2e72 656e 6465 7263  erArmEnv.renderc
-00001930: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001940: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
-00001950: 0053 0072 6f00 0000 2901 725f 0000 0072  .S.ro...).r_...r
-00001960: 7100 0000 7236 0000 0072 3600 0000 7237  q...r6...r6...r7
-00001970: 0000 00da 0a5f 6765 745f 7374 6174 65f5  ....._get_state.
-00001980: 0000 0073 0200 0000 0001 7a16 526f 7665  ...s......z.Rove
-00001990: 7241 726d 456e 762e 5f67 6574 5f73 7461  rArmEnv._get_sta
-000019a0: 7465 6301 0000 0000 0000 0000 0000 0001  tec.............
-000019b0: 0000 0002 0000 0043 0000 0073 0c00 0000  .......C...s....
-000019c0: 7400 a001 a100 0100 6400 5300 726f 0000  t.......d.S.ro..
-000019d0: 0029 0272 1c00 0000 da0a 6469 7363 6f6e  .).r......discon
-000019e0: 6e65 6374 7271 0000 0072 3600 0000 7236  nectrq...r6...r6
-000019f0: 0000 0072 3700 0000 da05 636c 6f73 65f8  ...r7.....close.
-00001a00: 0000 0073 0200 0000 0001 7a11 526f 7665  ...s......z.Rove
-00001a10: 7241 726d 456e 762e 636c 6f73 6529 024e  rArmEnv.close).N
-00001a20: 4e29 0cda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00001a30: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00001a40: 6c6e 616d 655f 5fda 086d 6574 6164 6174  lname__..metadat
-00001a50: 61da 0d70 7962 756c 6c65 745f 6461 7461  a..pybullet_data
-00001a60: 5a0b 6765 7444 6174 6150 6174 6872 3800  Z.getDataPathr8.
-00001a70: 0000 7266 0000 0072 8800 0000 7299 0000  ..rf...r....r...
-00001a80: 0072 9a00 0000 729c 0000 0072 3600 0000  .r....r....r6...
-00001a90: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
-00001aa0: 0600 0000 0e00 0000 7312 0000 0008 010c  ........s.......
-00001ab0: 020c 0104 ff0a 2708 2908 600a 3408 0372  ......'.).`.4..r
-00001ac0: 0600 0000 2912 da09 6779 6d6e 6173 6975  ....)...gymnasiu
-00001ad0: 6dda 0367 796d 7202 0000 0072 0300 0000  m..gymr....r....
-00001ae0: 7204 0000 00da 0f67 796d 6e61 7369 756d  r......gymnasium
-00001af0: 2e75 7469 6c73 7205 0000 0072 4f00 0000  .utilsr....rO...
-00001b00: da08 7079 6275 6c6c 6574 721c 0000 0072  ..pybulletr....r
-00001b10: a100 0000 7274 0000 00da 056e 756d 7079  ....rt.....numpy
-00001b20: 7227 0000 0072 5200 0000 7255 0000 00da  r'...rR...rU....
-00001b30: 0345 6e76 7206 0000 0072 3600 0000 7236  .Envr....r6...r6
-00001b40: 0000 0072 3600 0000 7237 0000 00da 083c  ...r6...r7.....<
-00001b50: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
-00001b60: 0801 1401 0c02 0801 0801 0801 0801 0801  ................
-00001b70: 0801 0803                                ....
+000000e0: 0600 0000 4000 0000 7352 0000 0065 005a  ....@...sR...e.Z
+000000f0: 0164 005a 0264 0164 0264 0365 03a0 04a1  .d.Z.d.d.d.e....
+00000100: 0064 0464 0466 0664 0564 0684 015a 0564  .d.d.f.d.d...Z.d
+00000110: 1364 0864 0984 015a 0664 0a64 0b84 005a  .d.d...Z.d.d...Z
+00000120: 0764 1464 0d64 0e84 015a 0864 0f64 1084  .d.d.d...Z.d.d..
+00000130: 005a 0964 1164 1284 005a 0a64 0c53 0029  .Z.d.d...Z.d.S.)
+00000140: 15da 0b52 6f76 6572 4172 6d45 6e76 da09  ...RoverArmEnv..
+00000150: 7267 625f 6172 7261 7969 1027 0000 4669  rgb_arrayi.'..Fi
+00000160: e001 0000 6307 0000 0000 0000 0000 0000  ....c...........
+00000170: 0008 0000 000f 0000 0043 0000 0073 8201  .........C...s..
+00000180: 0000 6401 6402 6403 6702 6901 7c00 5f00  ..d.d.d.g.i.|._.
+00000190: 7c01 7c00 5f01 7c03 7c00 5f02 6404 7c00  |.|._.|.|._.d.|.
+000001a0: 5f03 7c04 7c00 5f04 7c02 7c00 5f05 7c05  _.|.|._.|.|._.|.
+000001b0: 7c00 5f06 7c06 7c00 5f07 7c00 6a01 6402  |._.|.|._.|.j.d.
+000001c0: 6b02 7278 7408 a009 7408 6a0a a101 7d07  k.rxt...t.j...}.
+000001d0: 7c07 6405 6b00 7262 7408 a009 7408 6a0b  |.d.k.rbt...t.j.
+000001e0: a101 7d07 7408 a00c 6406 6407 6408 6700  ..}.t...d.d.d.g.
+000001f0: 6409 a201 a104 0100 6e0c 7408 a009 7408  d.......n.t...t.
+00000200: 6a0d a101 0100 640a 7c00 5f0e 640b 7c00  j.....d.|._.d.|.
+00000210: 5f0f 640c 7c00 5f10 6700 640d a201 7c00  _.d.|._.g.d...|.
+00000220: 5f11 7408 6a0c 7c00 6a0e 7c00 6a0f 7c00  _.t.j.|.j.|.j.|.
+00000230: 6a10 7c00 6a11 640e 8d04 0100 7412 a013  j.|.j.d.....t...
+00000240: 7414 a015 640f 6701 6410 1400 a101 7414  t...d.g.d.....t.
+00000250: a015 6411 6701 6410 1400 a101 a102 7c00  ..d.g.d.......|.
+00000260: 5f16 6412 7c00 5f17 7412 a013 7414 a015  _.d.|._.t...t...
+00000270: 7c00 6a17 0b00 7c00 6a17 0b00 7c00 6a17  |.j...|.j...|.j.
+00000280: 0b00 7c00 6a17 0b00 640f 6405 6405 7c00  ..|.j...d.d.d.|.
+00000290: 6a17 0b00 7c00 6a17 0b00 640f 670a a101  j...|.j...d.g...
+000002a0: 7414 a015 7c00 6a17 7c00 6a17 7c00 6a17  t...|.j.|.j.|.j.
+000002b0: 7c00 6a17 6411 6413 6413 7c00 6a17 7c00  |.j.d.d.d.|.j.|.
+000002c0: 6a17 6411 670a a101 a102 7c00 5f18 6405  j.d.g.....|._.d.
+000002d0: 6414 6702 7c00 5f19 6700 6415 a201 7c00  d.g.|._.g.d...|.
+000002e0: 5f1a 6405 7c00 5f1b 6416 7c00 5f1c 6417  _.d.|._.d.|._.d.
+000002f0: 7c00 5f1d 6418 7c00 5f1e 6419 7c00 5f1f  |._.d.|._.d.|._.
+00000300: 6400 5300 291a 4e7a 0c72 656e 6465 722e  d.S.).Nz.render.
+00000310: 6d6f 6465 73da 0568 756d 616e 7207 0000  modes..humanr...
+00000320: 0067 1111 1111 1111 713f 7201 0000 0067  .g......q?r....g
+00000330: cdcc cccc cccc f43f e9b4 0000 0069 d7ff  .......?.....i..
+00000340: ffff 2903 67a4 703d 0ad7 a3e0 3fe7 9a99  ..).g.p=....?...
+00000350: 9999 9999 c9bf 671f 85eb 51b8 1ed5 bfe9  ......g...Q.....
+00000360: 0300 0000 e766 6666 6666 66d6 bf69 ddff  .....ffffff..i..
+00000370: ffff 2903 6771 3d0a d7a3 70e5 3f72 0c00  ..).gq=...p.?r..
+00000380: 0000 679a 9999 9999 99c9 3f29 045a 0e63  ..g.......?).Z.c
+00000390: 616d 6572 6144 6973 7461 6e63 655a 0963  ameraDistanceZ.c
+000003a0: 616d 6572 6159 6177 5a0b 6361 6d65 7261  ameraYawZ.camera
+000003b0: 5069 7463 68da 1463 616d 6572 6154 6172  Pitch..cameraTar
+000003c0: 6765 7450 6f73 6974 696f 6ee9 ffff ffff  getPosition.....
+000003d0: e906 0000 00e9 0100 0000 e905 0000 00e7  ................
+000003e0: ec51 b81e 85eb b13f e902 0000 0029 0472  .Q.....?.....).r
+000003f0: 1000 0000 720b 0000 00e9 0400 0000 7211  ....r.........r.
+00000400: 0000 0067 3333 3333 3333 d33f 677b 14ae  ...g333333.?g{..
+00000410: 47e1 7a84 3fe9 c800 0000 e914 0000 0029  G.z.?..........)
+00000420: 20da 086d 6574 6164 6174 61da 0b72 656e   ..metadata..ren
+00000430: 6465 725f 6d6f 6465 5a0b 5f69 7344 6973  der_modeZ._isDis
+00000440: 6372 6574 655a 095f 7469 6d65 5374 6570  creteZ._timeStep
+00000450: da09 5f75 7264 6652 6f6f 74da 095f 6d61  .._urdfRoot.._ma
+00000460: 7853 7465 7073 da06 5f77 6964 7468 da07  xSteps.._width..
+00000470: 5f68 6569 6768 74da 0170 da07 636f 6e6e  _height..p..conn
+00000480: 6563 74da 0d53 4841 5245 445f 4d45 4d4f  ect..SHARED_MEMO
+00000490: 5259 da03 4755 49da 1a72 6573 6574 4465  RY..GUI..resetDe
+000004a0: 6275 6756 6973 7561 6c69 7a65 7243 616d  bugVisualizerCam
+000004b0: 6572 61da 0644 4952 4543 54da 095f 6361  era..DIRECT.._ca
+000004c0: 6d5f 6469 7374 da08 5f63 616d 5f79 6177  m_dist.._cam_yaw
+000004d0: da0a 5f63 616d 5f70 6974 6368 da0d 5f63  .._cam_pitch.._c
+000004e0: 616d 5f74 6172 6765 745f 7072 0300 0000  am_target_pr....
+000004f0: da03 426f 78da 026e 70da 0561 7272 6179  ..Box..np..array
+00000500: da0c 6163 7469 6f6e 5f73 7061 6365 da08  ..action_space..
+00000510: 626f 756e 6461 7279 da11 6f62 7365 7276  boundary..observ
+00000520: 6174 696f 6e5f 7370 6163 65da 0f73 7465  ation_space..ste
+00000530: 6572 696e 675f 6a6f 696e 7473 da0c 6472  ering_joints..dr
+00000540: 6976 655f 6a6f 696e 7473 da0b 6a6f 696e  ive_joints..join
+00000550: 745f 7370 6565 64da 0963 5f72 6f6c 6c69  t_speed..c_rolli
+00000560: 6e67 da06 635f 6472 6167 da0a 635f 7468  ng..c_drag..c_th
+00000570: 726f 7474 6c65 da09 4d41 585f 5350 4545  rottle..MAX_SPEE
+00000580: 4429 08da 0473 656c 6672 1800 0000 5a08  D)...selfr....Z.
+00000590: 6d61 7853 7465 7073 5a0a 6973 4469 7363  maxStepsZ.isDisc
+000005a0: 7265 7465 5a08 7572 6466 526f 6f74 da05  reteZ.urdfRoot..
+000005b0: 7769 6474 68da 0668 6569 6768 745a 0363  width..heightZ.c
+000005c0: 6964 a900 7237 0000 00fa 4e2f 5573 6572  id..r7....N/User
+000005d0: 732f 7361 6970 6861 6e69 3732 342f 4465  s/saiphani724/De
+000005e0: 736b 746f 702f 4169 2f52 6f62 6f74 6963  sktop/Ai/Robotic
+000005f0: 732f 526f 7665 7241 726d 2f72 6f76 6572  s/RoverArm/rover
+00000600: 5f61 726d 2f65 6e76 732f 726f 7665 7261  _arm/envs/rovera
+00000610: 726d 5f65 6e76 2e70 79da 085f 5f69 6e69  rm_env.py..__ini
+00000620: 745f 5f10 0000 0073 3a00 0000 0002 0e01  t__....s:.......
+00000630: 0601 0601 0601 0601 0601 0601 0601 0a01  ................
+00000640: 0c01 0801 0c01 1602 0c01 0601 0601 0601  ................
+00000650: 0a02 1a01 2601 0601 6603 0a01 0a02 0602  ....&...f.......
+00000660: 0601 0602 0602 7a14 526f 7665 7241 726d  ......z.RoverArm
+00000670: 456e 762e 5f5f 696e 6974 5f5f e92a 0000  Env.__init__.*..
+00000680: 0063 0200 0000 0000 0000 0000 0000 1000  .c..............
+00000690: 0000 0800 0000 4300 0000 7326 0200 0074  ......C...s&...t
+000006a0: 00a0 017c 01a1 0101 0074 026a 00a0 017c  ...|.....t.j...|
+000006b0: 01a1 0101 0064 017c 005f 0374 04a0 05a1  .....d.|._.t....
+000006c0: 0001 0074 04a0 0674 046a 0764 01a1 0201  ...t...t.j.d....
+000006d0: 0074 04a0 0864 0164 0164 02a1 0301 0074  .t...d.d.d.....t
+000006e0: 046a 0974 0a6a 0ba0 0c7c 006a 0d64 03a1  .j.t.j...|.j.d..
+000006f0: 0267 0064 04a2 0164 058d 027d 0267 0064  .g.d...d...}.g.d
+00000700: 06a2 017d 0374 026a 00a0 0e74 00a0 0f64  ...}.t.j...t...d
+00000710: 0764 08a1 0274 00a0 0f64 0964 0aa1 0267  .d...t...d.d...g
+00000720: 02a1 017d 0474 00a0 0f64 0764 0ba1 027d  ...}.t...d.d...}
+00000730: 0574 10a0 11a1 0064 0119 0064 0c17 007d  .t.....d...d...}
+00000740: 0674 046a 097c 0664 0d17 007c 047c 0564  .t.j.|.d...|.|.d
+00000750: 0e67 0364 058d 027c 005f 1274 1364 0f64  .g.d...|._.t.d.d
+00000760: 1083 0244 005d 1c7d 0774 04a0 147c 006a  ...D.].}.t...|.j
+00000770: 127c 077c 037c 0764 0f18 0019 00a1 0301  .|.|.|.d........
+00000780: 0071 c674 04a0 147c 006a 1264 1164 12a1  .q.t...|.j.d.d..
+00000790: 0301 0074 04a0 147c 006a 1264 1364 12a1  ...t...|.j.d.d..
+000007a0: 0301 0074 046a 0974 0a6a 0ba0 0c7c 006a  ...t.j.t.j...|.j
+000007b0: 0d64 14a1 0267 0064 15a2 0164 1664 178d  .d...g.d...d.d..
+000007c0: 037d 0874 046a 0974 0a6a 0ba0 0c7c 006a  .}.t.j.t.j...|.j
+000007d0: 0d64 18a1 0267 0064 19a2 0164 1664 178d  .d...g.d...d.d..
+000007e0: 037d 0974 00a0 0f64 1a64 16a1 0274 00a0  .}.t...d.d...t..
+000007f0: 0f64 1b64 1ca1 0264 1d67 037d 0a74 046a  .d.d...d.g.}.t.j
+00000800: 0974 0a6a 0ba0 0c7c 006a 0d64 1ea1 027c  .t.j...|.j.d...|
+00000810: 0a64 1f64 178d 037c 005f 1574 04a0 167c  .d.d...|._.t...|
+00000820: 006a 1264 01a1 0264 0119 0064 0064 0a85  .j.d...d...d.d..
+00000830: 0219 007d 0b74 04a0 167c 006a 1264 20a1  ...}.t...|.j.d .
+00000840: 0264 0119 007d 0c74 04a0 177c 006a 1264  .d...}.t...|.j.d
+00000850: 11a1 0264 0119 0074 04a0 177c 006a 1264  ...d...t...|.j.d
+00000860: 13a1 0264 0119 0066 027d 0d74 04a0 187c  ...d...f.}.t...|
+00000870: 006a 15a1 015c 027d 0a7d 0e7c 0b7c 0c17  .j...\.}.}.|.|..
+00000880: 007c 0d17 0074 197c 0a83 0117 007c 005f  .|...t.|.....|._
+00000890: 1a74 04a0 0674 046a 0764 21a1 0201 007c  .t...t.j.d!....|
+000008a0: 0b7c 0c7c 0d7c 0a64 229c 047d 0f74 02a0  .|.|.|.d"..}.t..
+000008b0: 1b7c 006a 1aa1 01a0 1c74 026a 1da1 017c  .|.j.....t.j...|
+000008c0: 0f66 0253 0029 234e 7201 0000 0069 f6ff  .f.S.)#Nr....i..
+000008d0: ffff 7a0a 706c 616e 652e 7572 6466 2903  ..z.plane.urdf).
+000008e0: 7201 0000 0072 0100 0000 e7cd cccc cccc  r....r..........
+000008f0: cce4 bf29 01da 0c62 6173 6550 6f73 6974  ...)...basePosit
+00000900: 696f 6e29 0972 0100 0000 6785 eb51 b81e  ion).r....g..Q..
+00000910: 85cb bf72 0100 0000 678f c2f5 285c 8f04  ...r....g...(\..
+00000920: c072 0100 0000 e70c 022b 8716 d902 4072  .r.......+....@r
+00000930: 3d00 0000 e77b 14ae 47e1 7ab4 3f72 3e00  =....{..G.z.?r>.
+00000940: 0000 720e 0000 0067 3333 3333 3333 d3bf  ..r....g333333..
+00000950: 6700 0000 0000 00f4 3f72 1300 0000 6700  g.......?r....g.
+00000960: 0000 0000 0004 407a 102f 726f 7665 725f  ......@z./rover_
+00000970: 6172 6d2f 6461 7461 2f7a 0d72 6f76 6572  arm/data/z.rover
+00000980: 5f61 726d 2e78 6d6c 6700 0000 0000 00e0  _arm.xmlg.......
+00000990: bfe9 0700 0000 e90e 0000 00e9 1000 0000  ................
+000009a0: 7212 0000 00e9 1100 0000 7a10 7461 626c  r.........z.tabl
+000009b0: 652f 7461 626c 652e 7572 6466 2903 e700  e/table.urdf)...
+000009c0: 0000 0000 00e0 3f72 0100 0000 723b 0000  ......?r....r;..
+000009d0: 0072 4300 0000 2902 723c 0000 005a 0d67  .rC...).r<...Z.g
+000009e0: 6c6f 6261 6c53 6361 6c69 6e67 7a11 7472  lobalScalingz.tr
+000009f0: 6179 2f74 7261 7962 6f78 2e75 7264 6629  ay/traybox.urdf)
+00000a00: 0367 cdcc cccc cccc dc3f 7201 0000 0067  .g.......?r....g
+00000a10: 713d 0ad7 a370 d5bf 679a 9999 9999 99d9  q=...p..g.......
+00000a20: 3f67 9a99 9999 9999 a9bf e79a 9999 9999  ?g..............
+00000a30: 99a9 3f72 0a00 0000 7a19 7261 6e64 6f6d  ..?r....z.random
+00000a40: 5f75 7264 6673 2f30 3030 2f30 3030 2e75  _urdfs/000/000.u
+00000a50: 7264 6667 9a99 9999 9999 e93f e912 0000  rdfg.......?....
+00000a60: 0072 1000 0000 a904 da0b 7374 6174 655f  .r........state_
+00000a70: 726f 7665 72da 0973 7461 7465 5f61 726d  rover..state_arm
+00000a80: da0d 7374 6174 655f 6669 6e67 6572 73da  ..state_fingers.
+00000a90: 0c73 7461 7465 5f6f 626a 6563 7429 1eda  .state_object)..
+00000aa0: 0672 616e 646f 6dda 0473 6565 6472 2800  .random..seedr(.
+00000ab0: 0000 da0c 7374 6570 5f63 6f75 6e74 6572  ....step_counter
+00000ac0: 721d 0000 00da 0f72 6573 6574 5369 6d75  r......resetSimu
+00000ad0: 6c61 7469 6f6e da18 636f 6e66 6967 7572  lation..configur
+00000ae0: 6544 6562 7567 5669 7375 616c 697a 6572  eDebugVisualizer
+00000af0: da14 434f 565f 454e 4142 4c45 5f52 454e  ..COV_ENABLE_REN
+00000b00: 4445 5249 4e47 da0a 7365 7447 7261 7669  DERING..setGravi
+00000b10: 7479 da08 6c6f 6164 5552 4446 da02 6f73  ty..loadURDF..os
+00000b20: da04 7061 7468 da04 6a6f 696e 7219 0000  ..path..joinr...
+00000b30: 00da 0663 686f 6963 65da 0775 6e69 666f  ...choice..unifo
+00000b40: 726d da04 7369 7465 da0f 6765 7473 6974  rm..site..getsit
+00000b50: 6570 6163 6b61 6765 73da 0b72 6f76 6572  epackages..rover
+00000b60: 6172 6d55 6964 da05 7261 6e67 65da 0f72  armUid..range..r
+00000b70: 6573 6574 4a6f 696e 7453 7461 7465 da09  esetJointState..
+00000b80: 6f62 6a65 6374 5569 64da 0c67 6574 4c69  objectUid..getLi
+00000b90: 6e6b 5374 6174 65da 0d67 6574 4a6f 696e  nkState..getJoin
+00000ba0: 7453 7461 7465 da1d 6765 7442 6173 6550  tState..getBaseP
+00000bb0: 6f73 6974 696f 6e41 6e64 4f72 6965 6e74  ositionAndOrient
+00000bc0: 6174 696f 6eda 0574 7570 6c65 da0b 6f62  ation..tuple..ob
+00000bd0: 7365 7276 6174 696f 6e72 2900 0000 da06  servationr).....
+00000be0: 6173 7479 7065 da07 666c 6f61 7433 3229  astype..float32)
+00000bf0: 1072 3400 0000 724c 0000 005a 0870 6c61  .r4...rL...Z.pla
+00000c00: 6e65 5569 645a 0a72 6573 745f 706f 7365  neUidZ.rest_pose
+00000c10: 735a 0578 5f70 6f73 5a05 795f 706f 73da  sZ.x_posZ.y_pos.
+00000c20: 0842 4153 455f 4449 52da 0169 5a08 7461  .BASE_DIR..iZ.ta
+00000c30: 626c 6555 6964 5a07 7472 6179 5569 6472  bleUidZ.trayUidr
+00000c40: 4a00 0000 7247 0000 0072 4800 0000 7249  J...rG...rH...rI
+00000c50: 0000 00da 015f da04 696e 666f 7237 0000  ....._..infor7..
+00000c60: 0072 3700 0000 7238 0000 00da 0572 6573  .r7...r8.....res
+00000c70: 6574 3800 0000 7338 0000 0000 010a 010c  et8...s8........
+00000c80: 0206 0108 010e 020e 021e 0208 0220 010c  ............. ..
+00000c90: 0210 021a 030e 011a 0110 0110 0220 0120  ............. . 
+00000ca0: 021a 011e 021a 0112 0124 0110 0216 020e  .........$......
+00000cb0: 010e 017a 1152 6f76 6572 4172 6d45 6e76  ...z.RoverArmEnv
+00000cc0: 2e72 6573 6574 6302 0000 0000 0000 0000  .resetc.........
+00000cd0: 0000 0022 0000 0008 0000 0003 0000 0073  ..."...........s
+00000ce0: 5203 0000 7400 a001 6401 7402 6a03 0b00  R...t...d.t.j...
+00000cf0: 7402 6a03 6402 1b00 6703 a101 7d02 6403  t.j.d...g...}.d.
+00000d00: 8900 8700 6601 6404 6405 8408 7c01 6406  ....f.d.d...|.d.
+00000d10: 6407 8502 1900 4400 8301 5c03 7d03 7d04  d.....D...\.}.}.
+00000d20: 7d05 7c01 6407 1900 7d06 7404 a005 7c06  }.|.d...}.t...|.
+00000d30: 6408 6409 6702 640a 640b 6702 a103 7d06  d.d.g.d.d.g...}.
+00000d40: 7400 a006 8801 6a07 640c a102 7d07 7c07  t.....j.d...}.|.
+00000d50: 640a 1900 7d08 7c08 640a 1900 7c03 1700  d...}.|.d...|...
+00000d60: 7c08 6409 1900 7c04 1700 7c08 6406 1900  |.d...|...|.d...
+00000d70: 7c05 1700 6703 7d09 7400 a008 8801 6a07  |...g.}.t.....j.
+00000d80: 640c 7c09 7c02 a104 7d0a 7c0a 6400 640d  d.|.|...}.|.d.d.
+00000d90: 8502 1900 7c0a 640d 640e 8502 1900 0200  ....|.d.d.......
+00000da0: 7d0b 7d0c 7400 a009 8801 6a07 740a 740b  }.}.t.....j.t.t.
+00000db0: 640f 6410 8302 8301 6411 6412 6702 1700  d.d.....d.d.g...
+00000dc0: 7400 6a0c 740a 7c0c 8301 6406 7c06 6701  t.j.t.|...d.|.g.
+00000dd0: 1400 1700 a104 0100 7c01 6400 6406 8502  ........|.d.d...
+00000de0: 1900 5c02 7d0d 7d0e 740d 740e 7c0d 6408  ..\.}.}.t.t.|.d.
+00000df0: 8302 6409 8302 7d0d 7404 a005 7c0e 6408  ..d...}.t...|.d.
+00000e00: 6409 6702 6413 6414 6702 a103 7d0e 7400  d.g.d.d.g...}.t.
+00000e10: 6a09 8801 6a07 8801 6a0f 7400 6a0c 7c0e  j...j...j.t.j.|.
+00000e20: 6701 6406 1400 6415 8d04 0100 8801 6a10  g.d...d.......j.
+00000e30: 0b00 8801 6a10 8801 6a11 1400 8801 6a12  ....j...j.....j.
+00000e40: 1700 1400 7d0f 8801 6a13 7c0d 1400 7c0f  ....}...j.|...|.
+00000e50: 1700 7d10 8801 6a10 6416 7c10 1400 1700  ..}...j.d.|.....
+00000e60: 8801 5f10 740d 740e 8801 6a10 8801 6a14  .._.t.t...j...j.
+00000e70: 0b00 8302 8801 6a14 8302 8801 5f10 7400  ......j....._.t.
+00000e80: 6a09 8801 6a07 8801 6a15 7400 6a16 8801  j...j...j.t.j...
+00000e90: 6a10 6701 6417 1400 6418 6701 6417 1400  j.g.d...d.g.d...
+00000ea0: 6419 8d05 0100 7400 a017 8801 6a18 a101  d.....t.....j...
+00000eb0: 5c02 7d11 7d12 7400 a019 a100 0100 7400  \.}.}.t.......t.
+00000ec0: a017 8801 6a18 a101 5c02 7d13 7d12 7400  ....j...\.}.}.t.
+00000ed0: a006 8801 6a07 640a a102 640a 1900 6400  ....j.d...d...d.
+00000ee0: 6406 8502 1900 7d14 7400 a006 8801 6a07  d.....}.t.....j.
+00000ef0: 640c a102 640a 1900 7d15 7400 a01a 8801  d...d...}.t.....
+00000f00: 6a07 6411 a102 640a 1900 7400 a01a 8801  j.d...d...t.....
+00000f10: 6a07 6412 a102 640a 1900 6602 7d16 641a  j.d...d...f.}.d.
+00000f20: 5c02 7d17 7d18 7c13 6406 1900 640a 6b04  \.}.}.|.d...d.k.
+00000f30: 9002 725a 6409 7d19 641b 7d17 6e74 7404  ..rZd.}.d.}.ntt.
+00000f40: a01b 7404 a01c 7c08 a101 7404 a01c 7c11  ..t...|...t...|.
+00000f50: a101 1800 a101 5c03 7d1a 7d1b 7d1c 7404  ......\.}.}.}.t.
+00000f60: a01b 7404 a01c 7c15 a101 7404 a01c 7c13  ..t...|...t...|.
+00000f70: a101 1800 a101 5c03 7d1d 7d1e 7d1f 7c1a  ......\.}.}.}.|.
+00000f80: 7c1d 1800 7c1b 1700 7c1e 1800 7c1c 1700  |...|...|...|...
+00000f90: 7c1f 1800 7d19 741b 7c19 8301 641c 6b04  |...}.t.|...d.k.
+00000fa0: 9002 72ca 7c19 6418 1b00 7d19 6e04 640a  ..r.|.d...}.n.d.
+00000fb0: 7d19 8801 0400 6a1d 6409 3700 0200 5f1d  }.....j.d.7..._.
+00000fc0: 8701 6601 641d 641e 8408 7d20 7c20 7c14  ..f.d.d...} | |.
+00000fd0: 8301 9002 73fa 6408 7d19 641b 7d17 8801  ....s.d.}.d.}...
+00000fe0: 6a1d 8801 6a1e 6b04 9003 7210 640a 7d19  j...j.k...r.d.}.
+00000ff0: 641b 7d18 7c14 7c15 1700 7c16 1700 741f  d.}.|.|...|...t.
+00001000: 7c13 8301 1700 8801 5f20 7c14 7c15 7c16  |......._ |.|.|.
+00001010: 7c13 641f 9c04 7d21 7404 a01c 8801 6a20  |.d...}!t.....j 
+00001020: a101 a021 7404 6a22 a101 7c19 7c17 7c18  ...!t.j"..|.|.|.
+00001030: 7c21 6605 5300 2920 4e67 0000 0000 0000  |!f.S.) Ng......
+00001040: 0000 6700 0000 0000 0000 4072 4400 0000  ..g.......@rD...
+00001050: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001060: 0004 0000 0013 0000 0073 1400 0000 6700  .........s....g.
+00001070: 7c00 5d0c 7d01 7c01 8800 1400 9102 7104  |.].}.|.......q.
+00001080: 5300 7237 0000 0072 3700 0000 2902 da02  S.r7...r7...)...
+00001090: 2e30 da01 7829 01da 0264 7672 3700 0000  .0..x)...dvr7...
+000010a0: 7238 0000 00da 0a3c 6c69 7374 636f 6d70  r8.....<listcomp
+000010b0: 3e68 0000 00f3 0000 0000 7a24 526f 7665  >h........z$Rove
+000010c0: 7241 726d 456e 762e 7374 6570 2e3c 6c6f  rArmEnv.step.<lo
+000010d0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000010e0: 7213 0000 0072 1100 0000 720e 0000 0072  r....r....r....r
+000010f0: 1000 0000 7201 0000 0072 1200 0000 7245  ....r....r....rE
+00001100: 0000 0072 0f00 0000 e90d 0000 0072 3f00  ...r.........r?.
+00001110: 0000 7240 0000 0072 4100 0000 7242 0000  ..r@...rA...rB..
+00001120: 0067 3333 3333 3333 e3bf 6733 3333 3333  .g333333..g33333
+00001130: 33e3 3f29 02da 0b63 6f6e 7472 6f6c 4d6f  3.?)...controlMo
+00001140: 6465 5a0f 7461 7267 6574 506f 7369 7469  deZ.targetPositi
+00001150: 6f6e 7367 1111 1111 1111 a13f 7214 0000  onsg.......?r...
+00001160: 00e9 0a00 0000 2905 5a0c 626f 6479 556e  ......).Z.bodyUn
+00001170: 6971 7565 4964 5a0c 6a6f 696e 7449 6e64  iqueIdZ.jointInd
+00001180: 6963 6573 7270 0000 005a 1074 6172 6765  icesrp...Z.targe
+00001190: 7456 656c 6f63 6974 6965 735a 0666 6f72  tVelocitiesZ.for
+000011a0: 6365 7329 0246 4654 67fc a9f1 d24d 6250  ces).FFTg....MbP
+000011b0: 3f63 0100 0000 0000 0000 0000 0000 0400  ?c..............
+000011c0: 0000 0200 0000 1300 0000 733c 0000 007c  ..........s<...|
+000011d0: 005c 027d 017d 027c 0188 006a 000b 006b  .\.}.}.|...j...k
+000011e0: 046f 1c7c 0188 006a 006b 007d 037c 036f  .o.|...j.k.}.|.o
+000011f0: 367c 0288 006a 000b 006b 046f 367c 0288  6|...j...k.o6|..
+00001200: 006a 006b 007d 037c 0353 00a9 014e 2901  .j.k.}.|.S...N).
+00001210: 722b 0000 0029 0472 4700 0000 da02 7278  r+...).rG.....rx
+00001220: 5a02 7279 5a07 696e 426f 756e 64a9 0172  Z.ryZ.inBound..r
+00001230: 3400 0000 7237 0000 0072 3800 0000 da06  4...r7...r8.....
+00001240: 696e 4761 6d65 b000 0000 7308 0000 0000  inGame....s.....
+00001250: 0108 0116 011a 017a 2052 6f76 6572 4172  .......z RoverAr
+00001260: 6d45 6e76 2e73 7465 702e 3c6c 6f63 616c  mEnv.step.<local
+00001270: 733e 2e69 6e47 616d 6572 4600 0000 2923  s>.inGamerF...)#
+00001280: 721d 0000 00da 1667 6574 5175 6174 6572  r......getQuater
+00001290: 6e69 6f6e 4672 6f6d 4575 6c65 72da 046d  nionFromEuler..m
+000012a0: 6174 68da 0270 6972 2800 0000 da06 696e  ath..pir(.....in
+000012b0: 7465 7270 725e 0000 0072 5a00 0000 da1a  terpr^...rZ.....
+000012c0: 6361 6c63 756c 6174 6549 6e76 6572 7365  calculateInverse
+000012d0: 4b69 6e65 6d61 7469 6373 da19 7365 744a  Kinematics..setJ
+000012e0: 6f69 6e74 4d6f 746f 7243 6f6e 7472 6f6c  ointMotorControl
+000012f0: 4172 7261 79da 046c 6973 7472 5b00 0000  Array..listr[...
+00001300: da10 504f 5349 5449 4f4e 5f43 4f4e 5452  ..POSITION_CONTR
+00001310: 4f4c da03 6d69 6eda 036d 6178 722d 0000  OL..min..maxr-..
+00001320: 0072 2f00 0000 7231 0000 0072 3000 0000  .r/...r1...r0...
+00001330: 7232 0000 0072 3300 0000 722e 0000 00da  r2...r3...r.....
+00001340: 1056 454c 4f43 4954 595f 434f 4e54 524f  .VELOCITY_CONTRO
+00001350: 4c72 6000 0000 725d 0000 00da 0e73 7465  Lr`...r].....ste
+00001360: 7053 696d 756c 6174 696f 6e72 5f00 0000  pSimulationr_...
+00001370: da03 6162 7372 2900 0000 724d 0000 0072  ..absr)...rM...r
+00001380: 1a00 0000 7261 0000 0072 6200 0000 7263  ....ra...rb...rc
+00001390: 0000 0072 6400 0000 2922 7234 0000 00da  ...rd...)"r4....
+000013a0: 0661 6374 696f 6e5a 0b6f 7269 656e 7461  .actionZ.orienta
+000013b0: 7469 6f6e 5a04 6478 5f61 5a04 6479 5f61  tionZ.dx_aZ.dy_a
+000013c0: 5a04 647a 5f61 5a07 6669 6e67 6572 735a  Z.dz_aZ.fingersZ
+000013d0: 0b63 7572 7265 6e74 506f 7365 5a0f 6375  .currentPoseZ.cu
+000013e0: 7272 656e 7450 6f73 6974 696f 6e5a 0b6e  rrentPositionZ.n
+000013f0: 6577 506f 7369 7469 6f6e 5a0a 6a6f 696e  ewPositionZ.join
+00001400: 7450 6f73 6573 5a10 6a6f 696e 7450 6f73  tPosesZ.jointPos
+00001410: 6573 5f72 6f76 6572 5a0e 6a6f 696e 7450  es_roverZ.jointP
+00001420: 6f73 6573 5f61 726d 5a08 7468 726f 7474  oses_armZ.thrott
+00001430: 6c65 5a0e 7374 6565 7269 6e67 5f61 6e67  leZ.steering_ang
+00001440: 6c65 5a08 6672 6963 7469 6f6e 5a0c 6163  leZ.frictionZ.ac
+00001450: 6365 6c65 7261 7469 6f6e 5a11 7374 6174  celerationZ.stat
+00001460: 655f 6f62 6a65 6374 5f70 7265 7672 6700  e_object_prevrg.
+00001470: 0000 724a 0000 0072 4700 0000 7248 0000  ..rJ...rG...rH..
+00001480: 0072 4900 0000 da0a 7465 726d 696e 6174  .rI.....terminat
+00001490: 6564 da09 7472 756e 6361 7465 64da 0672  ed..truncated..r
+000014a0: 6577 6172 64da 0278 305a 0279 305a 027a  eward..x0Z.y0Z.z
+000014b0: 30da 0278 31da 0279 31da 027a 3172 7500  0..x1..y1..z1ru.
+000014c0: 0000 7268 0000 0072 3700 0000 2902 726c  ..rh...r7...).rl
+000014d0: 0000 0072 3400 0000 7238 0000 00da 0473  ...r4...r8.....s
+000014e0: 7465 7064 0000 0073 7a00 0000 0002 1a01  tepd...sz.......
+000014f0: 0401 2001 0801 1602 0e02 0802 0a01 0a01  .. .............
+00001500: 0afe 0403 1201 1a01 3402 1004 1001 1604  ........4.......
+00001510: 0c01 0401 08fe 0606 1001 04ff 0603 0e03  ................
+00001520: 1002 1a04 0401 0401 0401 0401 0a01 08fb  ................
+00001530: 0607 1002 0802 1001 1a01 1201 2402 0801  ............$...
+00001540: 0e01 0401 0602 2001 2001 1801 0e01 0a02  ...... . .......
+00001550: 0402 0e01 0c06 0a01 0401 0402 0e01 0401  ................
+00001560: 0402 1601 0e02 7a10 526f 7665 7241 726d  ......z.RoverArm
+00001570: 456e 762e 7374 6570 4e63 0300 0000 0000  Env.stepNc......
+00001580: 0000 0000 0000 0c00 0000 0800 0000 4300  ..............C.
+00001590: 0000 7342 0100 007c 0164 006b 0273 107c  ..sB...|.d.k.s.|
+000015a0: 0264 006b 0272 1c7c 006a 007d 017c 006a  .d.k.r.|.j.}.|.j
+000015b0: 017d 027c 006a 0264 016b 0372 2a64 0053  .}.|.j.d.k.r*d.S
+000015c0: 0074 036a 047c 006a 057c 006a 067c 006a  .t.j.|.j.|.j.|.j
+000015d0: 077c 006a 0864 0264 0364 048d 067d 0374  .|.j.d.d.d...}.t
+000015e0: 036a 0467 0064 05a2 0164 0664 0764 0864  .j.g.d...d.d.d.d
+000015f0: 0264 0364 048d 067d 0474 036a 0964 0974  .d.d...}.t.j.d.t
+00001600: 0a7c 0183 017c 021b 0064 0a64 0b64 0c8d  .|...|...d.d.d..
+00001610: 047d 0574 036a 0b7c 017c 027c 037c 0574  .}.t.j.|.|.|.|.t
+00001620: 036a 0c64 0d8d 055c 057d 067d 067d 077d  .j.d...\.}.}.}.}
+00001630: 067d 0674 036a 0b7c 017c 027c 047c 0574  .}.t.j.|.|.|.|.t
+00001640: 036a 0c64 0d8d 055c 057d 067d 067d 087d  .j.d...\.}.}.}.}
+00001650: 067d 0674 0d6a 0e7c 0774 0d6a 0f64 0e8d  .}.t.j.|.t.j.d..
+00001660: 027d 0974 0da0 107c 097c 027c 0164 0f66  .}.t...|.|.|.d.f
+00001670: 03a1 0264 0064 0085 0264 0064 0085 0264  ...d.d...d.d...d
+00001680: 0064 1085 0266 0319 007d 0974 0d6a 0e7c  .d...f...}.t.j.|
+00001690: 0874 0d6a 0f64 0e8d 027d 0a74 0da0 107c  .t.j.d...}.t...|
+000016a0: 0a7c 027c 0164 0f66 03a1 0264 0064 0085  .|.|.d.f...d.d..
+000016b0: 0264 0064 0085 0264 0064 1085 0266 0319  .d.d...d.d...f..
+000016c0: 007d 0a74 0d6a 117c 097c 0a66 0264 0364  .}.t.j.|.|.f.d.d
+000016d0: 118d 027d 0b7c 0b53 0029 124e 7207 0000  ...}.|.S.).Nr...
+000016e0: 0072 0100 0000 7213 0000 0029 0672 0d00  .r....r....).r..
+000016f0: 0000 da08 6469 7374 616e 6365 5a03 7961  ....distanceZ.ya
+00001700: 775a 0570 6974 6368 da04 726f 6c6c 5a0b  wZ.pitch..rollZ.
+00001710: 7570 4178 6973 496e 6465 7829 03e7 6666  upAxisIndex)..ff
+00001720: 6666 6666 e63f 7201 0000 0072 4400 0000  ffff.?r....rD...
+00001730: 728e 0000 00e9 5a00 0000 69ba ffff ffe9  r.....Z...i.....
+00001740: 3c00 0000 679a 9999 9999 99b9 3f67 0000  <...g.......?g..
+00001750: 0000 0000 5940 2904 5a03 666f 76da 0661  ....Y@).Z.fov..a
+00001760: 7370 6563 745a 076e 6561 7256 616c 5a06  spectZ.nearValZ.
+00001770: 6661 7256 616c 2905 7235 0000 0072 3600  farVal).r5...r6.
+00001780: 0000 5a0a 7669 6577 4d61 7472 6978 5a10  ..Z.viewMatrixZ.
+00001790: 7072 6f6a 6563 7469 6f6e 4d61 7472 6978  projectionMatrix
+000017a0: 5a08 7265 6e64 6572 6572 2901 da05 6474  Z.renderer)...dt
+000017b0: 7970 6572 1400 0000 720b 0000 0029 01da  yper....r....)..
+000017c0: 0461 7869 7329 1272 1b00 0000 721c 0000  .axis).r....r...
+000017d0: 0072 1800 0000 721d 0000 00da 2163 6f6d  .r....r.....!com
+000017e0: 7075 7465 5669 6577 4d61 7472 6978 4672  puteViewMatrixFr
+000017f0: 6f6d 5961 7750 6974 6368 526f 6c6c 7226  omYawPitchRollr&
+00001800: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+00001810: 0000 da1a 636f 6d70 7574 6550 726f 6a65  ....computeProje
+00001820: 6374 696f 6e4d 6174 7269 7846 4f56 da05  ctionMatrixFOV..
+00001830: 666c 6f61 74da 0e67 6574 4361 6d65 7261  float..getCamera
+00001840: 496d 6167 65da 1945 525f 4255 4c4c 4554  Image..ER_BULLET
+00001850: 5f48 4152 4457 4152 455f 4f50 454e 474c  _HARDWARE_OPENGL
+00001860: 7228 0000 0072 2900 0000 da05 7569 6e74  r(...r).....uint
+00001870: 38da 0772 6573 6861 7065 da0b 636f 6e63  8..reshape..conc
+00001880: 6174 656e 6174 6529 0c72 3400 0000 7235  atenate).r4...r5
+00001890: 0000 0072 3600 0000 5a0c 7669 6577 5f6d  ...r6...Z.view_m
+000018a0: 6174 7269 7831 5a0c 7669 6577 5f6d 6174  atrix1Z.view_mat
+000018b0: 7269 7832 5a0b 7072 6f6a 5f6d 6174 7269  rix2Z.proj_matri
+000018c0: 7872 6700 0000 5a03 7078 315a 0370 7832  xrg...Z.px1Z.px2
+000018d0: 5a0a 7267 625f 6172 7261 7931 5a0a 7267  Z.rgb_array1Z.rg
+000018e0: 625f 6172 7261 7932 7207 0000 0072 3700  b_array2r....r7.
+000018f0: 0000 7237 0000 0072 3800 0000 da06 7265  ..r7...r8.....re
+00001900: 6e64 6572 c400 0000 7354 0000 0000 0710  nder....sT......
+00001910: 0106 0106 010a 0104 0108 0104 0104 0104  ................
+00001920: 0102 0102 fb06 060a 0102 0102 0102 0102  ................
+00001930: 0102 fb06 0606 010a 0102 0102 fd06 0506  ................
+00001940: 0102 0102 0102 0104 fc10 0606 0102 0102  ................
+00001950: 0102 0104 fc10 0610 0128 0210 0128 0312  .........(...(..
+00001960: 027a 1252 6f76 6572 4172 6d45 6e76 2e72  .z.RoverArmEnv.r
+00001970: 656e 6465 7263 0100 0000 0000 0000 0000  enderc..........
+00001980: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00001990: 0000 007c 006a 0053 0072 7200 0000 2901  ...|.j.S.rr...).
+000019a0: 7262 0000 0072 7400 0000 7237 0000 0072  rb...rt...r7...r
+000019b0: 3700 0000 7238 0000 00da 0a5f 6765 745f  7...r8....._get_
+000019c0: 7374 6174 65f8 0000 0073 0200 0000 0001  state....s......
+000019d0: 7a16 526f 7665 7241 726d 456e 762e 5f67  z.RoverArmEnv._g
+000019e0: 6574 5f73 7461 7465 6301 0000 0000 0000  et_statec.......
+000019f0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00001a00: 0073 0c00 0000 7400 a001 a100 0100 6400  .s....t.......d.
+00001a10: 5300 7272 0000 0029 0272 1d00 0000 da0a  S.rr...).r......
+00001a20: 6469 7363 6f6e 6e65 6374 7274 0000 0072  disconnectrt...r
+00001a30: 3700 0000 7237 0000 0072 3800 0000 da05  7...r7...r8.....
+00001a40: 636c 6f73 65fb 0000 0073 0200 0000 0001  close....s......
+00001a50: 7a11 526f 7665 7241 726d 456e 762e 636c  z.RoverArmEnv.cl
+00001a60: 6f73 6529 0172 3a00 0000 2902 4e4e 290b  ose).r:...).NN).
+00001a70: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00001a80: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00001a90: 6d65 5f5f da0d 7079 6275 6c6c 6574 5f64  me__..pybullet_d
+00001aa0: 6174 615a 0b67 6574 4461 7461 5061 7468  ataZ.getDataPath
+00001ab0: 7239 0000 0072 6900 0000 728b 0000 0072  r9...ri...r....r
+00001ac0: 9c00 0000 729d 0000 0072 9f00 0000 7237  ....r....r....r7
+00001ad0: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+00001ae0: 0000 7206 0000 000e 0000 0073 1000 0000  ..r........s....
+00001af0: 0802 0c01 04ff 0a28 0a2c 0860 0a34 0803  .......(.,.`.4..
+00001b00: 7206 0000 0029 12da 0967 796d 6e61 7369  r....)...gymnasi
+00001b10: 756d da03 6779 6d72 0200 0000 7203 0000  um..gymr....r...
+00001b20: 0072 0400 0000 da0f 6779 6d6e 6173 6975  .r......gymnasiu
+00001b30: 6d2e 7574 696c 7372 0500 0000 7253 0000  m.utilsr....rS..
+00001b40: 00da 0870 7962 756c 6c65 7472 1d00 0000  ...pybulletr....
+00001b50: 72a3 0000 0072 7700 0000 da05 6e75 6d70  r....rw.....nump
+00001b60: 7972 2800 0000 724b 0000 0072 5800 0000  yr(...rK...rX...
+00001b70: da03 456e 7672 0600 0000 7237 0000 0072  ..Envr....r7...r
+00001b80: 3700 0000 7237 0000 0072 3800 0000 da08  7...r7...r8.....
+00001b90: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
+00001ba0: 0008 0114 010c 0208 0108 0108 0108 0108  ................
+00001bb0: 0108 0108 03                             .....
```

### Comparing `rover_arm-1.1.1/rover_arm/envs/roverarm_env.py` & `rover_arm-1.1.2/rover_arm/envs/roverarm_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 import math
 import numpy as np
 import random
 import site
 
 
 class RoverArmEnv(gym.Env):
-    metadata = {'render.modes': ['human' , 'rgb_array']}
 
     def __init__(self, render_mode = 'rgb_array', maxSteps=10 * 1000, isDiscrete=False, urdfRoot = pybullet_data.getDataPath(), 
     width = 480, height = 480):
+        self.metadata = {'render.modes': ['human' , 'rgb_array']}
         self.render_mode = render_mode
         self._isDiscrete = isDiscrete
         self._timeStep = 1. / 240.
         self._urdfRoot = urdfRoot
         self._maxSteps = maxSteps
         self._width = width
         self._height = height
@@ -49,15 +49,18 @@
         self.c_rolling = 0.3
         self.c_drag = 0.01
         # Throttle constant increases "speed" of the car
         self.c_throttle = 200
         
         self.MAX_SPEED = 20
 
-    def reset(self):
+    def reset(self, seed = 42):
+        random.seed(seed)
+        np.random.seed(seed)
+        
         self.step_counter = 0
         p.resetSimulation()
         p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,0) # we will enable rendering after we loaded everything
         
         p.setGravity(0,0,-10)
 
         planeUid = p.loadURDF(os.path.join(self._urdfRoot,"plane.urdf"), basePosition=[0,0,-0.65])
```

### Comparing `rover_arm-1.1.1/rover_arm/envs/roverarm_env_arrange.py` & `rover_arm-1.1.2/rover_arm/envs/roverarm_env_arrange.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/envs/roverarm_env_place.py` & `rover_arm-1.1.2/rover_arm/envs/roverarm_env_place.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm/keyboard_control.py` & `rover_arm-1.1.2/rover_arm/keyboard_control.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/rover_arm.egg-info/PKG-INFO` & `rover_arm-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rover-arm
-Version: 1.1.1
+Name: rover_arm
+Version: 1.1.2
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.1.1/rover_arm.egg-info/SOURCES.txt` & `rover_arm-1.1.2/rover_arm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.1/setup.py` & `rover_arm-1.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name='rover_arm',
-    version='1.1.1',
+    version='1.1.2',
     description="A OpenAI Gym Env for Rover with Arm",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author="Sai Phani",
     packages = setuptools.find_packages(include="rover_arm*"),
     package_data={'data' :['rover_arm/data/*']},
     include_package_data=True,
```

