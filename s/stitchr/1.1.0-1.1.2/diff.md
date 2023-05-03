# Comparing `tmp/stitchr-1.1.0.tar.gz` & `tmp/stitchr-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stitchr-1.1.0.tar", last modified: Tue Apr 18 20:01:49 2023, max compression
+gzip compressed data, was "stitchr-1.1.2.tar", last modified: Wed May  3 20:13:19 2023, max compression
```

## Comparing `stitchr-1.1.0.tar` & `stitchr-1.1.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:49.866835 stitchr-1.1.0/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1073 2023-04-18 20:01:10.000000 stitchr-1.1.0/LICENSE
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    50455 2023-04-18 20:01:49.866835 stitchr-1.1.0/PKG-INFO
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    50095 2023-04-18 20:01:10.000000 stitchr-1.1.0/README.md
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       97 2023-04-18 20:01:10.000000 stitchr-1.1.0/pyproject.toml
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      978 2023-04-18 20:01:49.866835 stitchr-1.1.0/setup.cfg
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:49.858835 stitchr-1.1.0/src/
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:49.858835 stitchr-1.1.0/src/Data/
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:49.862835 stitchr-1.1.0/src/Data/GUI-Examples/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/__init__.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      245 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/cat_TRG-TRD.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      301 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/cow_TRG-TRD.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      294 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/dog_TRA-TRB.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      242 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/dog_TRG-TRD.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      237 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/dolphin_TRA-TRB.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      233 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/dolphin_TRG-TRD.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      241 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/dromedary_TRA-TRB.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      234 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/dromedary_TRG-TRD.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      254 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/human_TRA-TRB.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      291 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/human_TRG-TRD.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      246 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/mouse_TRA-TRB.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      285 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/mouse_TRG-TRD.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      238 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/pig_TRA-TRB.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      237 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/rabbit_TRG-TRD.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      290 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/rhesus_monkey_TRA-TRB.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      246 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/GUI-Examples/sheep_TRG-TRD.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/__init__.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     6071 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/additional-genes.fasta
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:49.862835 stitchr-1.1.0/src/Data/kazusa/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/CAT.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/COW.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/CYNOLOGOUS_MONKEY.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/DOG.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/DOLPHIN.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/DROMEDARY.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/FERRET.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1147 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/HUMAN.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/MOUSE.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/PIG.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/RABBIT.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/RHESUS_MONKEY.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/SHEEP.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/kazusa/__init__.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      292 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Data/linkers.tsv
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:49.866835 stitchr-1.1.0/src/Scripts/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Scripts/__init__.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    37856 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Scripts/functions.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    28418 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Scripts/gui_stitchr.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    24663 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Scripts/stitchr.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     2252 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Scripts/stitchrdl.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    22098 2023-04-18 20:01:10.000000 stitchr-1.1.0/src/Scripts/thimble.py
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:49.866835 stitchr-1.1.0/src/stitchr.egg-info/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    50455 2023-04-18 20:01:49.000000 stitchr-1.1.0/src/stitchr.egg-info/PKG-INFO
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1546 2023-04-18 20:01:49.000000 stitchr-1.1.0/src/stitchr.egg-info/SOURCES.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)        1 2023-04-18 20:01:49.000000 stitchr-1.1.0/src/stitchr.egg-info/dependency_links.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      154 2023-04-18 20:01:49.000000 stitchr-1.1.0/src/stitchr.egg-info/entry_points.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       45 2023-04-18 20:01:49.000000 stitchr-1.1.0/src/stitchr.egg-info/requires.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       13 2023-04-18 20:01:49.000000 stitchr-1.1.0/src/stitchr.egg-info/top_level.txt
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-05-03 20:13:19.742581 stitchr-1.1.2/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1073 2023-04-18 20:01:10.000000 stitchr-1.1.2/LICENSE
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      655 2023-05-03 20:13:19.742581 stitchr-1.1.2/PKG-INFO
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      295 2023-05-03 18:03:21.000000 stitchr-1.1.2/README.md
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       97 2023-04-18 20:01:10.000000 stitchr-1.1.2/pyproject.toml
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1028 2023-05-03 20:13:19.742581 stitchr-1.1.2/setup.cfg
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-05-03 20:13:19.734581 stitchr-1.1.2/src/
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-05-03 20:13:19.734581 stitchr-1.1.2/src/Data/
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-05-03 20:13:19.738581 stitchr-1.1.2/src/Data/GUI-Examples/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/__init__.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      245 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/cat_TRG-TRD.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      301 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/cow_TRG-TRD.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      294 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/dog_TRA-TRB.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      242 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/dog_TRG-TRD.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      237 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/dolphin_TRA-TRB.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      233 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/dolphin_TRG-TRD.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      241 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/dromedary_TRA-TRB.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      234 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/dromedary_TRG-TRD.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      254 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/human_TRA-TRB.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      291 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/human_TRG-TRD.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      246 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/mouse_TRA-TRB.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      285 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/mouse_TRG-TRD.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      238 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/pig_TRA-TRB.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      237 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/rabbit_TRG-TRD.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      290 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/rhesus_monkey_TRA-TRB.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      246 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/GUI-Examples/sheep_TRG-TRD.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/__init__.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     6071 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/additional-genes.fasta
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-05-03 20:13:19.738581 stitchr-1.1.2/src/Data/kazusa/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/CAT.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/COW.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/CYNOLOGOUS_MONKEY.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/DOG.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/DOLPHIN.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/DROMEDARY.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/FERRET.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1147 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/HUMAN.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/MOUSE.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/PIG.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/RABBIT.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/RHESUS_MONKEY.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1139 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/SHEEP.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/kazusa/__init__.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      292 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Data/linkers.tsv
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-05-03 20:13:19.738581 stitchr-1.1.2/src/Stitchr/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-18 20:01:10.000000 stitchr-1.1.2/src/Stitchr/__init__.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    28561 2023-05-03 19:56:43.000000 stitchr-1.1.2/src/Stitchr/gui_stitchr.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    24961 2023-05-03 19:56:43.000000 stitchr-1.1.2/src/Stitchr/stitchr.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     2241 2023-05-03 19:33:36.000000 stitchr-1.1.2/src/Stitchr/stitchrdl.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    38058 2023-05-03 19:56:43.000000 stitchr-1.1.2/src/Stitchr/stitchrfunctions.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    22089 2023-05-03 19:08:07.000000 stitchr-1.1.2/src/Stitchr/thimble.py
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-05-03 20:13:19.738581 stitchr-1.1.2/src/stitchr.egg-info/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      655 2023-05-03 20:13:19.000000 stitchr-1.1.2/src/stitchr.egg-info/PKG-INFO
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1553 2023-05-03 20:13:19.000000 stitchr-1.1.2/src/stitchr.egg-info/SOURCES.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)        1 2023-05-03 20:13:19.000000 stitchr-1.1.2/src/stitchr.egg-info/dependency_links.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      203 2023-05-03 20:13:19.000000 stitchr-1.1.2/src/stitchr.egg-info/entry_points.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       45 2023-05-03 20:13:19.000000 stitchr-1.1.2/src/stitchr.egg-info/requires.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       13 2023-05-03 20:13:19.000000 stitchr-1.1.2/src/stitchr.egg-info/top_level.txt
```

### Comparing `stitchr-1.1.0/LICENSE` & `stitchr-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/setup.cfg` & `stitchr-1.1.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stitchr
-version = 1.1.0
+version = 1.1.2
 author = Jamie Heather
 author_email = jheather@mgh.harvard.edu
 description = Stitch together coding TCR sequences from V/J/CDR3 information
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JamieHeather/stitchr
 project_urls = 
@@ -27,16 +27,17 @@
 where = src
 
 [options.package_data]
 * = *.txt, *.rst, *.tsv, *.fasta, *.png
 
 [options.entry_points]
 console_scripts = 
-	stitchr = Scripts.stitchr:main
-	thimble = Scripts.thimble:main
-	gui_stitchr = Scripts.gui_stitchr:main
-	stitchrdl = Scripts.stitchrdl:main
+	stitchr = Stitchr.stitchr:main
+	stitchrfunctions = Stitchr.stitchrfunctions:main
+	thimble = Stitchr.thimble:main
+	gui_stitchr = Stitchr.gui_stitchr:main
+	stitchrdl = Stitchr.stitchrdl:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `stitchr-1.1.0/src/Data/additional-genes.fasta` & `stitchr-1.1.2/src/Data/additional-genes.fasta`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/CAT.txt` & `stitchr-1.1.2/src/Data/kazusa/CAT.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/COW.txt` & `stitchr-1.1.2/src/Data/kazusa/COW.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/CYNOLOGOUS_MONKEY.txt` & `stitchr-1.1.2/src/Data/kazusa/CYNOLOGOUS_MONKEY.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/DOG.txt` & `stitchr-1.1.2/src/Data/kazusa/DOG.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/DOLPHIN.txt` & `stitchr-1.1.2/src/Data/kazusa/DOLPHIN.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/DROMEDARY.txt` & `stitchr-1.1.2/src/Data/kazusa/DROMEDARY.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/FERRET.txt` & `stitchr-1.1.2/src/Data/kazusa/FERRET.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/HUMAN.txt` & `stitchr-1.1.2/src/Data/kazusa/HUMAN.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/MOUSE.txt` & `stitchr-1.1.2/src/Data/kazusa/MOUSE.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/PIG.txt` & `stitchr-1.1.2/src/Data/kazusa/PIG.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/RABBIT.txt` & `stitchr-1.1.2/src/Data/kazusa/RABBIT.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/RHESUS_MONKEY.txt` & `stitchr-1.1.2/src/Data/kazusa/RHESUS_MONKEY.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Data/kazusa/SHEEP.txt` & `stitchr-1.1.2/src/Data/kazusa/SHEEP.txt`

 * *Files identical despite different names*

### Comparing `stitchr-1.1.0/src/Scripts/functions.py` & `stitchr-1.1.2/src/Stitchr/stitchrfunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-#!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 """
-functions.py
+stitchrfunctions.py
 
 Functions for stiTChR and its related scripts
 """
 
 import collections as coll
 import gzip
 import os
@@ -18,26 +17,34 @@
 
 # Ensure correct importlib-resources function imported
 if sys.version_info < (3, 9):
     import importlib_resources                              # PyPI
 else:
     import importlib.resources as importlib_resources       # importlib.resources
 
-__version__ = '1.2.0'
+__version__ = '1.2.2'
 __author__ = 'Jamie Heather'
 __email__ = 'jheather@mgh.harvard.edu'
 
-#sys.tracebacklimit = 0  # comment when debugging # TODO
+sys.tracebacklimit = 0  # comment when debugging
+
 
 data_files = importlib_resources.files("Data")
 additional_genes_file = str(data_files / 'additional-genes.fasta')
 linkers_file = str(data_files / 'linkers.tsv')
-data_dir = additional_genes_file[:additional_genes_file.rfind('/') + 1]
+data_dir = os.path.dirname(additional_genes_file)
+gui_examples_dir = os.path.join(data_dir, 'GUI-Examples')
+
 
-gui_examples_dir = data_dir + 'GUI-Examples/'
+def custom_formatwarning(warning_msg, *args, **kwargs):
+    """
+    Function to make warnings.warn output just the warning text, not the underlying code
+    See https://stackoverflow.com/questions/2187269/print-only-the-message-on-warnings
+    """
+    return str(warning_msg) + '\n'
 
 
 def read_fa(ff):
     """
     :param ff: opened fasta file
     read_fa(file):Heng Li's Python implementation of his readfq function (tweaked to only bother with fasta)
     https://github.com/lh3/readfq/blob/master/readfq.py
@@ -124,30 +131,30 @@
                          "both from the same chain (alpha or beta). Should start \'TR[ABGD]\'.")
 
 
 def find_species_covered():
     """
     :return: list of data directories for different species available
     """
-    species_list = [x for x in os.listdir(data_dir) if os.path.isdir(data_dir + '/' + x) and
+    species_list = [x for x in os.listdir(data_dir) if os.path.isdir(os.path.normpath(os.path.join(data_dir, x))) and
                     x != 'kazusa' and x != 'GUI-Examples' and '__' not in x]
 
     if not species_list:
         raise ValueError("No species data detected. Please run stitchrdl first, or otherwise install data in the Data"
                          " directory (" + data_dir + ").")
     species_list.sort()
     return species_list
 
 
 def infer_species(path_to_file):
     """
     :param path_to_file: str of a path to an input file that may or may not contain
     :return: the species detected, if one found that fits the data available in the data directory
     """
-    in_file_name = path_to_file.split('/')[-1]
+    in_file_name = os.path.basename(path_to_file)
     species_search = [x for x in find_species_covered() if x in in_file_name.upper()]
 
     if len(species_search) == 1:
         return species_search[0]
     else:
         return ''
 
@@ -294,16 +301,15 @@
             if 'partial' in partial_flag:
                 partial_genes[gene][allele] = partial_flag
             else:
                 tcr_data[seq_type][gene][allele] = seq.upper()
 
     for gene_type in gene_types:
         if len(tcr_data[gene_type]) == 0:
-            raise Exception("No entries for " + gene_type + " in IMGT data.\nPlease ensure all appropriate data is in "
-                            "the Data/imgt-data.fasta file, and re-run split-imgt-data.py. ")
+            raise Exception("No entries for " + gene_type + " in IMGT data. ")
 
     return tcr_data, functionality, partial_genes
 
 
 def strip_functionality(functionality_str):
     """
     :param functionality_str: functionality string as present in an IMGT FASTA header
@@ -727,21 +733,20 @@
 
 
 def get_linker_dict():
     """
     :return: Dictionary of linkers contained in the Data/linkers.tsv file
     """
 
-    linker_file_path = data_dir + 'linkers.tsv'
-    if not os.path.isfile(linker_file_path):
-        raise IOError(linker_file_path + " not detected - please check linker file is present and run again. ")
+    if not os.path.isfile(linkers_file):
+        raise IOError(linkers_file + " not detected - please check linker file is present and run again. ")
 
     else:
         linkers = coll.defaultdict()
-        with open(linker_file_path, 'r') as in_file:
+        with open(linkers_file, 'r') as in_file:
             for line in in_file:
                 bits = line.rstrip().split('\t')
                 linkers[bits[0]] = bits[1]
 
         return linkers
 
 
@@ -872,14 +877,18 @@
         if len(overlap) > len(longest_overlap):
             longest_overlap = overlap
             index_longest = i
 
     return j_germline[index_longest + len(longest_overlap):]
 
 
+def main():
+    print("Please use the appropriate 'stitchr', 'thimble', 'gui_stitchr' or 'stitchrdl' command.")
+
+
 codons = {'AAA': 'K', 'AAC': 'N', 'AAG': 'K', 'AAT': 'N',
           'ACA': 'T', 'ACC': 'T', 'ACG': 'T', 'ACT': 'T',
           'AGA': 'R', 'AGC': 'S', 'AGG': 'R', 'AGT': 'S',
           'ATA': 'I', 'ATC': 'I', 'ATG': 'M', 'ATT': 'I',
           'CAA': 'Q', 'CAC': 'H', 'CAG': 'Q', 'CAT': 'H',
           'CCA': 'P', 'CCC': 'P', 'CCG': 'P', 'CCT': 'P',
           'CGA': 'R', 'CGC': 'R', 'CGG': 'R', 'CGT': 'R',
```

### Comparing `stitchr-1.1.0/src/Scripts/gui_stitchr.py` & `stitchr-1.1.2/src/Stitchr/gui_stitchr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-#!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 """
 gui_stitchr.py
 
 A graphical user interface for stitchr, powered by PySimpleGUI
 
 """
 
 
 import PySimpleGUI as sg
 import os
-from . import functions as fxn
+from . import stitchrfunctions as fxn
 from . import stitchr as st
 from . import thimble as th
 import collections as coll
 import warnings
 
 
-__version__ = '1.3.0'
+__version__ = '1.3.2'
 __author__ = 'Jamie Heather'
 __email__ = 'jheather@mgh.harvard.edu'
 
 
 def read_fasta_box(fasta_text):
     """
     :param fasta_text: Contents of text box containing FASTA format text
@@ -208,15 +207,15 @@
 
     return set_values
 
 
 def main():
 
     # Define needed/starting variables
-    extra_gene_text = ">TCRgenename*01\nATCG...\n"
+    extra_gene_text = ">TCRgenename*01\nATG\n"
     box_width = 70
     sz = (int(box_width * 0.9), 1)
     half_sz = (int(box_width * 0.44), 1)  # For half a column
     third_sz = (int(box_width / 3 - 1.3), 1)  # For one third of a column
     quart_sz = (int(box_width / 4 - 1.1), 1)  # For one quarter of a column
     out_box_font = ('Courier New', 10)
     fnt = 'Arial'
@@ -381,15 +380,16 @@
 
             else:
                 if len(example_matches) > 1:
                     sg.Popup('More than one ' + receptor + 'TCR example files available for species ' + species + ':\n'
                              'using the first alphabetically.')
                     example_matches.sort()
 
-                receptor, species = upload_tcr_details(examples_path + example_matches[0], receptor, species)
+                receptor, species = upload_tcr_details(os.path.join(examples_path, example_matches[0]),
+                                                       receptor, species)
 
         elif event == 'change_receptor':
 
             receptor = change_receptors(receptor)
 
         elif event == 'Reset form':
 
@@ -416,16 +416,15 @@
         elif event == 'Upload TCR details':
 
             receptor, species = upload_tcr_details(values['uploaded_tcr'], receptor, species)
 
         elif event == 'find_preferred_alleles':
 
             preferred_file = values['find_preferred_alleles']
-            just_file = preferred_file.split('/')[-1]
-            window['preferred_allele_button'].update(just_file)
+            window['preferred_allele_button'].update(os.path.basename(preferred_file))
 
         elif event == 'Run Stitchr':
             warning_msgs = coll.defaultdict(str)
 
             window['linked_out'].update('')
             window['linked_log'].update('')
 
@@ -456,15 +455,17 @@
                     if '*' in extra_gene[0]:
                         outputs['additional_fastas'].append(extra_gene)
                     else:
                         outputs['additional_fastas'].append((extra_gene[0] + '*01', extra_gene[1]))
 
                     # Also throw in an alert if non-DNA characters used
                     if not fxn.dna_check(extra_gene[1]):
-                        warnings.warn("Warning: user-provided gene " + extra_gene[0] + " contains non-DNA sequences.")
+                        if fxn.dna_check(extra_gene[1]) != extra_gene_text:
+                            warnings.warn("Warning: user-provided gene " + extra_gene[0] +
+                                          " contains non-DNA sequences.")
 
             # Check if seamless stitching selected
             if values['chk_seamless']:
                 seamless = True
             else:
                 seamless = False
```

### Comparing `stitchr-1.1.0/src/Scripts/stitchr.py` & `stitchr-1.1.2/src/Stitchr/stitchr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-#!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 """
 stitchr.py
 
 Takes command line V, J and (amino acid) CDR3 information
 to generate a full length coding nucleotide TCR sequence.
 Can be used for TCR vector design, and other purposes.
 
 """
 
-from . import functions as fxn
+from . import stitchrfunctions as fxn
 import argparse
+import sys
 import warnings
 
 
-__version__ = '1.1.0'
+__version__ = '1.1.2'
 __author__ = 'Jamie Heather'
 __email__ = 'jheather@mgh.harvard.edu'
 
-#sys.tracebacklimit = 0  # comment when debugging # TODO
-
+sys.tracebacklimit = 0  # comment when debugging
+warnings.formatwarning = fxn.custom_formatwarning
 
 def args():
     """
     args(): Obtains command line arguments which dictate the script's behaviour
     """
 
     # Help flag
@@ -85,14 +85,17 @@
 
     parser.add_argument('-jt', '--j_warning_threshold', required=False, type=int, default=3, help="J gene substring "
                         "length warning threshold. Default = 3. Decrease to get fewer notes on short J matches.")
 
     parser.add_argument('-sc', '--skip_c_checks', action='store_true', required=False, default=False,
                         help="Optional flag to skip usual constant region gene checks.")
 
+    parser.add_argument('-sw', '--suppress_warnings', action='store_true', required=False, default=False,
+                        help="Optional flag to suppress warnings.")
+
     parser.add_argument('--version', action='version', version=__version__, help="Print current stitchr version.")
 
     parser.add_argument('--cite', action='version', help="Print citation details.", version=fxn.citation)
 
     parser.add_argument('-dd', '--data_dir', action='version', help="Print installed stitchr data directory path.",
                         version=fxn.data_dir)
 
@@ -396,14 +399,17 @@
 def main():
 
     # Get input arguments, determine the TCR chain in use, get codon table, then load the IMGT data in
     input_args, chain = fxn.sort_input(vars(args()))
     codons = fxn.get_optimal_codons(input_args['codon_usage_path'], input_args['species'])
     imgt_dat, tcr_functionality, partial = fxn.get_imgt_data(chain, gene_types, input_args['species'])
 
+    if input_args['suppress_warnings']:
+        warnings.filterwarnings('ignore')
+
     if input_args['extra_genes']:
         imgt_dat, tcr_functionality = fxn.get_additional_genes(imgt_dat, tcr_functionality)
         input_args['skip_c_checks'] = True
 
     if input_args['preferred_alleles_path']:
         preferred_alleles = fxn.get_preferred_alleles(input_args['preferred_alleles_path'],
                                                       gene_types, imgt_dat, partial, chain)
```

### Comparing `stitchr-1.1.0/src/Scripts/stitchrdl.py` & `stitchr-1.1.2/src/Stitchr/stitchrdl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-#!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 """
 stitchrdl.py
 
 Download IMGT/GENE-DB data for stitching, for a given species
 """
 
 
 import os
-from . import functions as fxn
+from . import stitchrfunctions as fxn
 import argparse
 import subprocess
 import sys
 import shutil
 
 # Make sure IMGTgeneDL is installed
 try:
     import IMGTgeneDL
 except (ImportError, ModuleNotFoundError) as err:
     print("IMGTgeneDL is required to run this script (pip install IMGTgeneDL)")
     sys.exit()
 
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 __author__ = 'Jamie Heather'
 __email__ = 'jheather@mgh.harvard.edu'
 
 sys.tracebacklimit = 0  # comment when debugging
 
 
 def args():
@@ -67,8 +66,8 @@
         # Delete older entries
         if species in os.listdir(fxn.data_dir):
             print("Note: a directory for this species exists: overwriting.")
             shutil.rmtree(os.path.join(fxn.data_dir, species))
         shutil.move(os.path.join(os.getcwd(), species), os.path.join(fxn.data_dir, species))
 
     else:
-        raise IOError("Failed to produce the expected species\' output directory. ")
+        raise IOError("Failed to produce the expected species\' output directory. ")
```

### Comparing `stitchr-1.1.0/src/Scripts/thimble.py` & `stitchr-1.1.2/src/Stitchr/thimble.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 """
 thimble.py
 
 Runs stiTChR in a high-throughput manner, on a tab separated input file.
 
 No fancy backronym or contrived silent capitals - it just helps you stitch faster.
 
 """
 
 
-from . import functions as fxn
+from . import stitchrfunctions as fxn
 from . import stitchr as st
 import warnings
 import argparse
 import os
+import sys
 from time import time
 
-__version__ = '1.2.0'
+__version__ = '1.2.2'
 __author__ = 'Jamie Heather'
 __email__ = 'jheather@mgh.harvard.edu'
 
-#sys.tracebacklimit = 0  # comment when debugging # TODO
+sys.tracebacklimit = 0  # comment when debugging
 
 
 def args():
     """
     args(): Obtains command line arguments which dictate the script's behaviour
     """
```

### Comparing `stitchr-1.1.0/src/stitchr.egg-info/SOURCES.txt` & `stitchr-1.1.2/src/stitchr.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 src/Data/kazusa/HUMAN.txt
 src/Data/kazusa/MOUSE.txt
 src/Data/kazusa/PIG.txt
 src/Data/kazusa/RABBIT.txt
 src/Data/kazusa/RHESUS_MONKEY.txt
 src/Data/kazusa/SHEEP.txt
 src/Data/kazusa/__init__.py
-src/Scripts/__init__.py
-src/Scripts/functions.py
-src/Scripts/gui_stitchr.py
-src/Scripts/stitchr.py
-src/Scripts/stitchrdl.py
-src/Scripts/thimble.py
+src/Stitchr/__init__.py
+src/Stitchr/gui_stitchr.py
+src/Stitchr/stitchr.py
+src/Stitchr/stitchrdl.py
+src/Stitchr/stitchrfunctions.py
+src/Stitchr/thimble.py
 src/stitchr.egg-info/PKG-INFO
 src/stitchr.egg-info/SOURCES.txt
 src/stitchr.egg-info/dependency_links.txt
 src/stitchr.egg-info/entry_points.txt
 src/stitchr.egg-info/requires.txt
 src/stitchr.egg-info/top_level.txt
```

