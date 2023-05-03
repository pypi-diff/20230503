# Comparing `tmp/rover_arm-1.1.0.tar.gz` & `tmp/rover_arm-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rover_arm-1.1.0.tar", last modified: Tue May  2 23:40:18 2023, max compression
+gzip compressed data, was "rover_arm-1.1.1.tar", last modified: Tue May  2 23:51:56 2023, max compression
```

## Comparing `rover_arm-1.1.0.tar` & `rover_arm-1.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:40:18.340364 rover_arm-1.1.0/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-27 19:16:14.000000 rover_arm-1.1.0/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      188 2023-03-31 22:22:55.000000 rover_arm-1.1.0/.gitignore
--rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.1.0/MANIFEST.in
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-02 23:40:18.340216 rover_arm-1.1.0/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-03-31 23:16:16.000000 rover_arm-1.1.0/README.md
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:40:18.317568 rover_arm-1.1.0/rover_arm/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-31 06:14:48.000000 rover_arm-1.1.0/rover_arm/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      231 2023-04-27 19:25:40.000000 rover_arm-1.1.0/rover_arm/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:40:18.318801 rover_arm-1.1.0/rover_arm/data/
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:40:18.319224 rover_arm-1.1.0/rover_arm/data/meshes/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/.DS_Store
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:40:18.322377 rover_arm-1.1.0/rover_arm/data/meshes/collision/
--rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/link0.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/collision/link7.obj
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:40:18.337036 rover_arm-1.1.0/rover_arm/data/meshes/visual/
--rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/colors.png
--rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/finger.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/hand.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link1.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link2.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link3.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link4.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link5.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/meshes/visual/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/panda.urdf
--rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.1.0/rover_arm/data/rover_arm.xml
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:40:18.339733 rover_arm-1.1.0/rover_arm/envs/
--rw-r--r--   0 saiphani724   (501) staff       (20)      243 2023-03-30 23:20:23.000000 rover_arm-1.1.0/rover_arm/envs/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:40:18.339996 rover_arm-1.1.0/rover_arm/envs/__pycache__/
--rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.1.0/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)     7028 2023-05-02 23:39:25.000000 rover_arm-1.1.0/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)    11032 2023-05-02 23:38:54.000000 rover_arm-1.1.0/rover_arm/envs/roverarm_env.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.1.0/rover_arm/envs/roverarm_env_arrange.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.1.0/rover_arm/envs/roverarm_env_place.py
--rw-r--r--   0 saiphani724   (501) staff       (20)     2366 2023-04-27 20:10:52.000000 rover_arm-1.1.0/rover_arm/keyboard_control.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:40:18.318278 rover_arm-1.1.0/rover_arm.egg-info/
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-02 23:40:18.000000 rover_arm-1.1.0/rover_arm.egg-info/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     1740 2023-05-02 23:40:18.000000 rover_arm-1.1.0/rover_arm.egg-info/SOURCES.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-05-02 23:40:18.000000 rover_arm-1.1.0/rover_arm.egg-info/dependency_links.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       27 2023-05-02 23:40:18.000000 rover_arm-1.1.0/rover_arm.egg-info/requires.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-05-02 23:40:18.000000 rover_arm-1.1.0/rover_arm.egg-info/top_level.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-05-02 23:40:18.340412 rover_arm-1.1.0/setup.cfg
--rw-r--r--   0 saiphani724   (501) staff       (20)      570 2023-05-02 23:40:14.000000 rover_arm-1.1.0/setup.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.803413 rover_arm-1.1.1/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-27 19:16:14.000000 rover_arm-1.1.1/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      188 2023-03-31 22:22:55.000000 rover_arm-1.1.1/.gitignore
+-rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.1.1/MANIFEST.in
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-02 23:51:56.803259 rover_arm-1.1.1/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-03-31 23:16:16.000000 rover_arm-1.1.1/README.md
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.777995 rover_arm-1.1.1/rover_arm/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-31 06:14:48.000000 rover_arm-1.1.1/rover_arm/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      231 2023-04-27 19:25:40.000000 rover_arm-1.1.1/rover_arm/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.779411 rover_arm-1.1.1/rover_arm/data/
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.779825 rover_arm-1.1.1/rover_arm/data/meshes/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/.DS_Store
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.783124 rover_arm-1.1.1/rover_arm/data/meshes/collision/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link0.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/collision/link7.obj
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.799997 rover_arm-1.1.1/rover_arm/data/meshes/visual/
+-rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/colors.png
+-rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/finger.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/hand.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link1.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link2.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link3.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link4.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link5.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/meshes/visual/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/panda.urdf
+-rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.1.1/rover_arm/data/rover_arm.xml
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.802779 rover_arm-1.1.1/rover_arm/envs/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      243 2023-03-30 23:20:23.000000 rover_arm-1.1.1/rover_arm/envs/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.803046 rover_arm-1.1.1/rover_arm/envs/__pycache__/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.1.1/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)     7028 2023-05-02 23:39:25.000000 rover_arm-1.1.1/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11080 2023-05-02 23:51:32.000000 rover_arm-1.1.1/rover_arm/envs/roverarm_env.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.1.1/rover_arm/envs/roverarm_env_arrange.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.1.1/rover_arm/envs/roverarm_env_place.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2366 2023-04-27 20:10:52.000000 rover_arm-1.1.1/rover_arm/keyboard_control.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-02 23:51:56.778770 rover_arm-1.1.1/rover_arm.egg-info/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1740 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/SOURCES.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/dependency_links.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       27 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/requires.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-05-02 23:51:56.000000 rover_arm-1.1.1/rover_arm.egg-info/top_level.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-05-02 23:51:56.803467 rover_arm-1.1.1/setup.cfg
+-rw-r--r--   0 saiphani724   (501) staff       (20)      570 2023-05-02 23:51:52.000000 rover_arm-1.1.1/setup.py
```

### Comparing `rover_arm-1.1.0/.DS_Store` & `rover_arm-1.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/PKG-INFO` & `rover_arm-1.1.1/rover_arm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rover_arm
-Version: 1.1.0
+Name: rover-arm
+Version: 1.1.1
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.1.0/README.md` & `rover_arm-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/.DS_Store` & `rover_arm-1.1.1/rover_arm/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/.DS_Store` & `rover_arm-1.1.1/rover_arm/data/meshes/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/finger.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/hand.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/link0.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/link0.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/link1.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/link2.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/link3.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/link4.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/link5.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/link6.mtl` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/link6.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/collision/link7.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/collision/link7.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/colors.png` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/colors.png`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/finger.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/hand.mtl` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/hand.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/hand.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link1.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link2.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link3.mtl` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link3.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link3.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link4.mtl` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link4.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link4.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link5.mtl` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link5.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link5.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link6.mtl` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/meshes/visual/link6.obj` & `rover_arm-1.1.1/rover_arm/data/meshes/visual/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/panda.urdf` & `rover_arm-1.1.1/rover_arm/data/panda.urdf`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/data/rover_arm.xml` & `rover_arm-1.1.1/rover_arm/data/rover_arm.xml`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc` & `rover_arm-1.1.1/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/envs/roverarm_env.py` & `rover_arm-1.1.1/rover_arm/envs/roverarm_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self._cam_yaw = -0.35
         self._cam_pitch = -35
         self._cam_target_p = [0.67, -0.35, 0.20]
 
         p.resetDebugVisualizerCamera(cameraDistance= self._cam_dist , cameraYaw= self._cam_yaw, cameraPitch= self._cam_pitch, cameraTargetPosition=self._cam_target_p)
         self.action_space = spaces.Box(np.array([-1]*6), np.array([1]*6))
         self.boundary = 5
-        self.observation_space = spaces.Box(np.array([-self.boundary, -self.boundary, -1, -1, -1, 0,0 , -self.boundary, -self.boundary, -1]), np.array([self.boundary, self.boundary, 1, 1, 1, 0.07, 0.07, self.boundary, self.boundary, 1]))
+        self.observation_space = spaces.Box(np.array([-self.boundary, -self.boundary, -self.boundary, -self.boundary, -1, 0,0 , -self.boundary, -self.boundary, -1]), np.array([self.boundary, self.boundary, self.boundary, self.boundary, 1, 0.07, 0.07, self.boundary, self.boundary, 1]))
 
         # Joint indices as found by p.getJointInfo()
         self.steering_joints = [0, 2]
         self.drive_joints = [1, 3, 4, 5]
         # Joint speed
         self.joint_speed = 0
         # Drag constants
```

### Comparing `rover_arm-1.1.0/rover_arm/envs/roverarm_env_arrange.py` & `rover_arm-1.1.1/rover_arm/envs/roverarm_env_arrange.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/envs/roverarm_env_place.py` & `rover_arm-1.1.1/rover_arm/envs/roverarm_env_place.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm/keyboard_control.py` & `rover_arm-1.1.1/rover_arm/keyboard_control.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/rover_arm.egg-info/PKG-INFO` & `rover_arm-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rover-arm
-Version: 1.1.0
+Name: rover_arm
+Version: 1.1.1
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.1.0/rover_arm.egg-info/SOURCES.txt` & `rover_arm-1.1.1/rover_arm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.0/setup.py` & `rover_arm-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name='rover_arm',
-    version='1.1.0',
+    version='1.1.1',
     description="A OpenAI Gym Env for Rover with Arm",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author="Sai Phani",
     packages = setuptools.find_packages(include="rover_arm*"),
     package_data={'data' :['rover_arm/data/*']},
     include_package_data=True,
```

