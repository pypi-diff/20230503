# Comparing `tmp/ifes_apt_tc_data_modeling-0.0.7.tar.gz` & `tmp/ifes_apt_tc_data_modeling-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifes_apt_tc_data_modeling-0.0.7.tar", last modified: Fri Apr 28 13:32:38 2023, max compression
+gzip compressed data, was "ifes_apt_tc_data_modeling-0.0.8.tar", last modified: Wed May  3 08:16:00 2023, max compression
```

## Comparing `ifes_apt_tc_data_modeling-0.0.7.tar` & `ifes_apt_tc_data_modeling-0.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11358 2023-01-13 23:09:44.000000 ifes_apt_tc_data_modeling-0.0.7/LICENSE.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22620 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/PKG-INFO
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9003 2023-04-28 12:07:31.000000 ifes_apt_tc_data_modeling-0.0.7/README.md
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/__init__.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     4149 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_headers.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11187 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_reader.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    19797 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_sections.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    34067 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1553 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_utils.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 09:03:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     7731 2023-03-20 09:03:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/epos_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/fig/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:58:26.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/fig/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     5731 2023-04-28 13:16:35.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/fig/fig_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:59:34.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1585 2023-03-20 09:02:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/nx_field.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8106 2023-03-20 09:02:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/nx_ion.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-20 08:58:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     3414 2023-03-20 08:59:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/pos_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:58:26.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8153 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/rng_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9558 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/rrng_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1335 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/definitions.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1713 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/mmapped_io.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    16989 2023-04-28 12:58:48.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/molecular_ions.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)   164819 2023-03-20 08:50:51.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1253 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/string_handling.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8545 2023-04-28 12:42:39.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/utils.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22620 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/PKG-INFO
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1496 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)        1 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/dependency_links.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      139 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/requires.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       26 2023-04-28 13:32:38.000000 ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/top_level.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1051 2023-04-28 11:50:07.000000 ifes_apt_tc_data_modeling-0.0.7/pyproject.toml
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       38 2023-04-28 13:32:38.248045 ifes_apt_tc_data_modeling-0.0.7/setup.cfg
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.466841 ifes_apt_tc_data_modeling-0.0.8/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11358 2023-01-13 23:09:44.000000 ifes_apt_tc_data_modeling-0.0.8/LICENSE.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22620 2023-05-03 08:16:00.466841 ifes_apt_tc_data_modeling-0.0.8/PKG-INFO
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9003 2023-04-28 12:07:31.000000 ifes_apt_tc_data_modeling-0.0.8/README.md
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/__init__.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     4093 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_headers.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11504 2023-05-03 08:04:23.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_reader.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    19741 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_sections.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    34086 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1572 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_utils.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 09:03:51.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     7524 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/epos_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:58:26.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     5774 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/fig_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:59:34.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1604 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/nx_field.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     7995 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/nx_ion.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-20 08:58:38.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     3207 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/pos_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:58:26.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8079 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/rng_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9241 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/rrng_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.466841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1354 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/definitions.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1732 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/mmapped_io.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    17104 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/molecular_ions.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)   164819 2023-03-20 08:50:51.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1272 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/string_handling.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8572 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/utils.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22620 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/PKG-INFO
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1496 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)        1 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/dependency_links.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      139 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/requires.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       26 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/top_level.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1051 2023-05-03 08:14:00.000000 ifes_apt_tc_data_modeling-0.0.8/pyproject.toml
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       38 2023-05-03 08:16:00.466841 ifes_apt_tc_data_modeling-0.0.8/setup.cfg
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/LICENSE.txt` & `ifes_apt_tc_data_modeling-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/PKG-INFO` & `ifes_apt_tc_data_modeling-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifes_apt_tc_data_modeling
-Version: 0.0.7
+Version: 0.0.8
 Summary: Foster exchange about data models and work towards clear specifications of file formats and data models in the research field of atom probe microscopy.
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/README.md` & `ifes_apt_tc_data_modeling-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/__init__.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/__init__.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_headers.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_headers.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import numpy as np
 
 from ifes_apt_tc_data_modeling.apt.apt6_utils import string_to_typed_nparray
 
 
 class AptFileHeaderMetadata():
@@ -44,22 +44,22 @@
         # 64-bit value, which represents the number of 100-nanosecond intervals
         # since January 1, 1601, as per the MSDN specification
         self.ft_creation_time = np.uint64(0)
         # number of ions represented by file
         self.ll_ion_count = np.uint64(0)  # or an int64 ?
 
     @classmethod
-    def get_numpy_struct(cls) -> np.dtype:  # pylint: disable=R0801
-        """Create customized numpy struct to read a file header at once."""  # pylint: disable=R0801
+    def get_numpy_struct(cls) -> np.dtype:
+        """Create customized numpy struct to read a file header at once."""
         return np.dtype([('cSignature', np.uint8, (4,)),
                          ('iHeaderSize', np.int32),
                          ('iHeaderVersion', np.int32),
                          ('wcFilename', np.uint16, 256),
                          ('ftCreationTime', np.uint64),
-                         ('llIonCount', np.uint64)])  # pylint: disable=R0801
+                         ('llIonCount', np.uint64)])
 
     def set_ll_ion_count(self, value: np.uint64):
         """Check and set total ion count."""
         assert isinstance(value, np.uint64), \
             'llIonCount needs to be an int!'
         assert value > 0, \
             'llIonCount needs to be positive and not zero!'
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_reader.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import os
 
 import numpy as np
 
 import pandas as pd
 
@@ -192,18 +192,24 @@
             'Cannot create table, Mass section not available to guide \
                 the creation of the table header!'
         for key in self.available_sections['Mass'].get_metadata().keys():
             column_names.append(key)
         data_frame = pd.DataFrame(columns=column_names)
 
         for keyword, value in self.available_sections.items():
-            row = {'section': keyword}
-            row = {**row, **value.get_metadata()}
-            data_frame = data_frame.append(row, ignore_index=True)
+            row_dct = {'section': keyword}
+            # print(f"{keyword}")
+            row_dct = {**row_dct, **value.get_metadata()}
+            # print(value.get_metadata())
+            row_df = pd.DataFrame(row_dct, index=[0])
+            # print(row_df)
+            data_frame = pd.concat([data_frame, row_df], ignore_index=True)
 
+        data_frame.style.format(precision=3, thousands=",", decimal=".") \
+            .format_index(str.upper, axis=1)
         return data_frame
 
     def get_named_quantity(self, keyword: str):
         """Read quantity with name in keyword from APT file if it exists."""
         if keyword in self.available_sections.keys() \
            and keyword in self.byte_offsets.keys():
             byte_position_start = self.byte_offsets[keyword] \
@@ -223,15 +229,15 @@
             unit = self.available_sections[keyword].meta['wc_data_unit']
 
             return NxField(
                 np.reshape(data, newshape=shape), np_uint16_to_string(unit))
 
         return NxField()
 
-    def get_mass_to_charge_state_ratios(self):
+    def get_mass_to_charge_state_ratio(self):
         """Read mass-to-charge."""
         return self.get_named_quantity('Mass')
 
     def get_reconstructed_positions(self):
         """Read reconstructed positions."""
         return self.get_named_quantity('Position')
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_sections.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_sections.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import numpy as np
 
 from ifes_apt_tc_data_modeling.apt.apt6_utils import np_uint16_to_string
 from ifes_apt_tc_data_modeling.apt.apt6_utils import string_to_typed_nparray
 
 
@@ -217,29 +217,29 @@
 
     def set_accepted_units(self, value: list):
         """Set which unit strings are accepted."""
         # add further checks using e.g. pint
         self.accepted_units = value
 
     @classmethod
-    def get_numpy_struct(cls) -> np.dtype:  # pylint: disable=R0801
-        """Create customized numpy struct to read a section header at once."""  # pylint: disable=R0801
+    def get_numpy_struct(cls) -> np.dtype:
+        """Create customized numpy struct to read a section header at once."""
         return np.dtype([('cSignature', np.uint8, (4,)),
                          ('iHeaderSize', np.int32),
                          ('iHeaderVersion', np.int32),
                          ('wcSectionType', np.uint16, 32),
                          ('iSectionVersion', np.int32),
                          ('eRelationshipType', np.uint32),
                          ('eRecordType', np.uint32),
                          ('eRecordDataType', np.uint32),
                          ('iDataTypeSize', np.int32),
                          ('iRecordSize', np.int32),
                          ('wcDataUnit', np.uint16, 16),
                          ('llRecordCount', np.uint64),
-                         ('llByteCount', np.uint64)])  # pylint: disable=R0801
+                         ('llByteCount', np.uint64)])
 
     def get_ametek_size(self) -> np.uint64:
         """Compute how many byte raw data in bytes to read from AMETEK defs."""
         return np.uint64(self.meta['ll_byte_count'])
 
     def get_ametek_type(self) -> str:
         """Interpret numpy endianess/datatype from AMETEK defs."""
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 from ifes_apt_tc_data_modeling.apt.apt6_sections import AptFileSectionMetadata
 
 
 # define which header and sections to expect in an *.apt file
 # the sections below are referred to as branches in the commercial software
 # APSuite enables users select prior I/O which of the sections to write
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/apt/apt6_utils.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import numpy as np
 
 
 def np_uint16_to_string(uint16_array: np.ndarray) -> str:
     """Create string from array of uint16 numbers (UTF-16)."""
     str_parsed = ''
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/__init__.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/epos/epos_reader.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/epos_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import os
 
 import numpy as np
 
 from ifes_apt_tc_data_modeling.nexus.nx_field import NxField
 
@@ -56,39 +56,39 @@
         #               "Ion impact x-coordinate at the detector (mm)",
         #               "Ion impact y-coordinate at the detector (mm)",
         #               "Number of pulses since the last detected ion (pulses)",
         #               "Hit multiplicity (ions)"]
         # raw = np.fromfile( fnm, dtype= {"names": dtyp_names,
         # "formats": (, ">f4",">f4",">f4",">f4",">f4",">f4",">u4",">u4") } )
 
-    def get_reconstructed_positions(self):  # pylint: disable=R0801
-        """Read xyz columns."""  # pylint: disable=R0801
+    def get_reconstructed_positions(self):
+        """Read xyz columns."""
 
-        xyz = NxField()  # pylint: disable=R0801
+        xyz = NxField()
         xyz.typed_value = np.zeros(
-            [self.number_of_events, 3], np.float32)  # pylint: disable=R0801
-        xyz.unit = "nm"  # pylint: disable=R0801
+            [self.number_of_events, 3], np.float32)
+        xyz.unit = "nm"
 
         xyz.typed_value[:, 0] = \
             get_memory_mapped_data(self.filename, ">f4",
                                    0 * 4, 11 * 4, self.number_of_events)  # x
         xyz.typed_value[:, 1] = \
             get_memory_mapped_data(self.filename, ">f4",
                                    1 * 4, 11 * 4, self.number_of_events)  # y
         xyz.typed_value[:, 2] = \
             get_memory_mapped_data(self.filename, ">f4",
                                    2 * 4, 11 * 4, self.number_of_events)  # z
         return xyz
 
-    def get_mass_to_charge(self):  # pylint: disable=R0801
-        """Read mass-to-charge column."""  # pylint: disable=R0801
-        m_n = NxField()  # pylint: disable=R0801
+    def get_mass_to_charge_state_ratio(self):
+        """Read mass-to-charge-state-ratio column."""
+        m_n = NxField()
         m_n.typed_value = np.zeros(
-            [self.number_of_events, 1], np.float32)  # pylint: disable=R0801
-        m_n.unit = "Da"  # pylint: disable=R0801
+            [self.number_of_events, 1], np.float32)
+        m_n.unit = "Da"
 
         m_n.typed_value[:, 0] = \
             get_memory_mapped_data(self.filename, ">f4",
                                    3 * 4, 11 * 4, self.number_of_events)
         return m_n
 
     def get_raw_time_of_flight(self):
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/fig/__init__.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/fig/fig_reader.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/fig_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101,R0801
+# pylint: disable=no-member,duplicate-code
 
 import re
 
 import numpy as np
 
 from ifes_apt_tc_data_modeling.nexus.nx_ion import NxField, NxIon
 
@@ -102,33 +102,33 @@
                             neutron_number = mass_number - proton_number
                             ivec.append(isotope_to_hash(proton_number, neutron_number))
             ivec = np.sort(np.asarray(ivec, np.uint16))[::-1]
             ivector = np.zeros((MAX_NUMBER_OF_ATOMS_PER_ION,), np.uint16)
             ivector[0:len(ivec)] = ivec
             # print(ivector)
 
-            m_ion = NxIon(isotope_vector=ivector, charge=charge_state)
+            m_ion = NxIon(isotope_vector=ivector, charge_state=charge_state)
             m_ion.add_range(mqmin, mqmax)
             m_ion.comment = NxField(ionname, "")
             # m_ion.report()
 
             crawler = MolecularIonBuilder(
                 min_abundance=PRACTICAL_ABUNDANCE,
                 min_abundance_product=PRACTICAL_ABUNDANCE_PRODUCT,
                 min_half_life=PRACTICAL_MIN_HALF_LIFE,
                 sacrifice_uniqueness=SACRIFICE_ISOTOPIC_UNIQUENESS,
                 verbose=VERBOSE)
-            recovered_charge, m_ion_candidates = crawler.combinatorics(
+            recovered_charge_state, m_ion_candidates = crawler.combinatorics(
                 m_ion.isotope_vector.typed_value,
                 m_ion.ranges.typed_value[0, 0],
                 m_ion.ranges.typed_value[0, 1])
-            # print(" " + str(recovered_charge))
-            m_ion.charge = NxField(np.int8(recovered_charge), "")
+            # print(f"{recovered_charge_state}")
+            m_ion.charge_state = NxField(np.int8(recovered_charge_state), "")
             m_ion.update_human_readable_name()
-            m_ion.add_charge_model(
+            m_ion.add_charge_state_model(
                 {"min_abundance": PRACTICAL_ABUNDANCE,
                  "min_abundance_product": PRACTICAL_ABUNDANCE_PRODUCT,
                  "min_half_life": PRACTICAL_MIN_HALF_LIFE,
                  "sacrifice_isotopic_uniqueness": SACRIFICE_ISOTOPIC_UNIQUENESS},
                 m_ion_candidates)
 
             self.fig["molecular_ions"].append(m_ion)
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/__init__.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/nexus/nx_field.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/nx_field.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import typing
 
 from typing import Tuple
 
 import numpy as np
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/__init__.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/pos/pos_reader.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/pos_reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import os
 
 import numpy as np
 
 from ifes_apt_tc_data_modeling.nexus.nx_field import NxField
 
@@ -47,38 +47,38 @@
 
         # https://doi.org/10.1007/978-1-4614-3436-8 for file format details
         # dtyp_names = ["Reconstructed position along the x-axis (nm)",
         #               "Reconstructed position along the y-axis (nm)",
         #               "Reconstructed position along the z-axis (nm)",
         #               "Reconstructed mass-to-charge-state ratio (Da)"]
 
-    def get_reconstructed_positions(self):  # pylint: disable=R0801
-        """Read xyz columns."""  # pylint: disable=R0801
+    def get_reconstructed_positions(self):
+        """Read xyz columns."""
 
-        xyz = NxField()  # pylint: disable=R0801
+        xyz = NxField()
         xyz.typed_value = np.zeros(
-            [self.number_of_events, 3], np.float32)  # pylint: disable=R0801
-        xyz.unit = "nm"  # pylint: disable=R0801
+            [self.number_of_events, 3], np.float32)
+        xyz.unit = "nm"
 
         xyz.typed_value[:, 0] = \
             get_memory_mapped_data(self.filename, ">f4",
                                    0 * 4, 4 * 4, self.number_of_events)  # x
         xyz.typed_value[:, 1] = \
             get_memory_mapped_data(self.filename, ">f4",
                                    1 * 4, 4 * 4, self.number_of_events)  # y
         xyz.typed_value[:, 2] = \
             get_memory_mapped_data(self.filename, ">f4",
                                    2 * 4, 4 * 4, self.number_of_events)  # z
         return xyz
 
-    def get_mass_to_charge(self):  # pylint: disable=R0801
-        """Read mass-to-charge column."""  # pylint: disable=R0801
+    def get_mass_to_charge_state_ratio(self):
+        """Read mass-to-charge-state-ratio column."""
 
-        m_n = NxField()  # pylint: disable=R0801
+        m_n = NxField()
         m_n.typed_value = np.zeros(
-            [self.number_of_events, 1], np.float32)  # pylint: disable=R0801
-        m_n.unit = "Da"  # pylint: disable=R0801
+            [self.number_of_events, 1], np.float32)
+        m_n.unit = "Da"
 
         m_n.typed_value[:, 0] = \
             get_memory_mapped_data(self.filename, ">f4",
                                    3 * 4, 4 * 4, self.number_of_events)
         return m_n
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/__init__.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rng/rng_reader.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/rng_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import re
 
 import numpy as np
 
 from ifes_apt_tc_data_modeling.nexus.nx_ion import NxField, NxIon
 from ifes_apt_tc_data_modeling.utils.utils import \
@@ -113,19 +113,19 @@
         self.read_rng()
 
     def read_rng(self):
         """Read RNG range file content."""
         with open(self.filename, mode="r", encoding="utf8") as rngf:
             txt = rngf.read()
 
-        txt = txt.replace("\r\n", "\n")  # pylint: disable=R0801 # windows to unix EOL conversion
-        txt = txt.replace(",", ".")  # pylint: disable=R0801 # use decimal dots instead of comma
-        txt_stripped = [line for line in txt.split("\n")  # pylint: disable=R0801
-                        if line.strip() != "" and line.startswith("#") is False]  # pylint: disable=R0801
-        del txt  # pylint: disable=R0801
+        txt = txt.replace("\r\n", "\n")  # windows to unix EOL conversion
+        txt = txt.replace(",", ".")  # use decimal dots instead of comma
+        txt_stripped = [line for line in txt.split("\n")
+                        if line.strip() != "" and line.startswith("#") is False]
+        del txt
 
         # see DOI: 10.1007/978-1-4899-7430-3 for further details to this
         # Oak Ridge National Lab / Oxford *.rng file format
         # only the first ------ line is relevant
         # it details all ion labels aka ions
         # AMETEK"s IVAS/APSuite-specific trailing
         # polyatomic extension is redundant info
@@ -156,35 +156,35 @@
                 i - current_line_id, txt_stripped[i],
                 header["column_id_to_label"],
                 n_element_symbols + 3)
             assert dct is not None, \
                 "Line " + txt_stripped[i] + " is corrupted!"
 
             m_ion = NxIon(isotope_vector=create_isotope_vector(
-                dct["atoms"]), charge=0)
+                dct["atoms"]), charge_state=0)
             m_ion.add_range(dct["range"][0], dct["range"][1])
             m_ion.comment = NxField(dct["name"], "")
             m_ion.color = NxField(dct["color"], "")
             m_ion.volume = NxField(dct["volume"], "")
             # m_ion.report()
 
             crawler = MolecularIonBuilder(
                 min_abundance=PRACTICAL_ABUNDANCE,
                 min_abundance_product=PRACTICAL_ABUNDANCE_PRODUCT,
                 min_half_life=PRACTICAL_MIN_HALF_LIFE,
                 sacrifice_uniqueness=SACRIFICE_ISOTOPIC_UNIQUENESS,
                 verbose=VERBOSE)
-            recovered_charge, m_ion_candidates = crawler.combinatorics(
+            recovered_charge_state, m_ion_candidates = crawler.combinatorics(
                 m_ion.isotope_vector.typed_value,
                 m_ion.ranges.typed_value[0, 0],
                 m_ion.ranges.typed_value[0, 1])
-            # print(" " + str(recovered_charge))
-            m_ion.charge = NxField(np.int8(recovered_charge), "")
+            # print(f"{recovered_charge_state}")
+            m_ion.charge_state = NxField(np.int8(recovered_charge_state), "")
             m_ion.update_human_readable_name()
-            m_ion.add_charge_model(
+            m_ion.add_charge_state_model(
                 {"min_abundance": PRACTICAL_ABUNDANCE,
                  "min_abundance_product": PRACTICAL_ABUNDANCE_PRODUCT,
                  "min_half_life": PRACTICAL_MIN_HALF_LIFE,
                  "sacrifice_isotopic_uniqueness": SACRIFICE_ISOTOPIC_UNIQUENESS},
                 m_ion_candidates)
 
             self.rng["molecular_ions"].append(m_ion)
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/__init__.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/rrng/rrng_reader.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/rrng_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import re
 
 import numpy as np
 
 from ifes_apt_tc_data_modeling.nexus.nx_ion import NxField, NxIon
 from ifes_apt_tc_data_modeling.utils.utils import \
@@ -112,28 +112,28 @@
         self.read_rrng()
 
     def read_rrng(self):
         """Read content of an RRNG range file."""
         with open(self.filename, mode="r", encoding="utf8") as rrngf:
             txt = rrngf.read()
 
-        txt = txt.replace("\r\n", "\n")  # pylint: disable=R0801 # windows to unix EOL conversion
-        txt = txt.replace(",", ".")  # pylint: disable=R0801 # use decimal dots instead of comma
-        txt_stripped = [line for line in txt.split("\n")  # pylint: disable=R0801
-                        if line.strip() != "" and line.startswith("#") is False]  # pylint: disable=R0801
-        del txt  # pylint: disable=R0801
-
-        # see DOI: 10.1007/978-1-4899-7430-3 for further details to this  # pylint: disable=R0801
-        # AMETEK/Cameca"s *.rrng file format  # pylint: disable=R0801
-
-        # pylint: disable=R0801 # first, parse [Ions] section, which holds a list of element names
-        # pylint: disable=R0801 # there are documented cases where experimentalists add custom strings
-        # pylint: disable=R0801 # to specify ranges they consider special
-        # pylint: disable=R0801 # these are loaded as user types
-        # pylint: disable=R0801 # with isotope_vector np.iinfo(np.uint16).max
+        txt = txt.replace("\r\n", "\n")  # windows to unix EOL conversion
+        txt = txt.replace(",", ".")  # use decimal dots instead of comma
+        txt_stripped = [line for line in txt.split("\n")
+                        if line.strip() != "" and line.startswith("#") is False]
+        del txt
+
+        # see DOI: 10.1007/978-1-4899-7430-3 for further details to this
+        # AMETEK/Cameca"s *.rrng file format
+
+        # first, parse [Ions] section, which holds a list of element names
+        # there are documented cases where experimentalists add custom strings
+        # to specify ranges they consider special
+        # these are loaded as user types
+        # with isotope_vector np.iinfo(np.uint16).max
         where = [idx for idx, element in
                  enumerate(txt_stripped) if element == "[Ions]"]
         assert isinstance(where, list), "Section [Ions] not found!"
         assert len(where) == 1, "Section [Ions] not found or ambiguous!"
         current_line_id = where[0] + 1
 
         tmp = re.split(r"[\s=]+", txt_stripped[current_line_id])
@@ -162,42 +162,41 @@
         assert len(tmp) == 2, "[Ranges]/Number line corrupted!"
         assert tmp[0] == "Number", "[Ranges]/Number incorrectly formatted!"
         assert tmp[1].isnumeric(), "[Ranges]/Number not a number!"
         number_of_ranges = int(tmp[1])
         assert number_of_ranges > 0, "No ranges defined!"
         current_line_id += 1
 
-        # print("Parsing range, progress via recovered charge state...")
         for i in np.arange(0, number_of_ranges):
             dct = evaluate_rrng_range_line(i + 1, txt_stripped[current_line_id + i])
             assert dct, \
                 "Line " + txt_stripped[current_line_id + i] + " is corrupted!"
 
             m_ion = NxIon(isotope_vector=create_isotope_vector(
-                dct["atoms"]), charge=0)
+                dct["atoms"]), charge_state=0)
             m_ion.add_range(dct["range"][0], dct["range"][1])
             m_ion.comment = NxField(dct["name"], "")
             m_ion.color = NxField(dct["color"], "")
             m_ion.volume = NxField(dct["volume"], "")
             # m_ion.report()
 
             crawler = MolecularIonBuilder(
                 min_abundance=PRACTICAL_ABUNDANCE,
                 min_abundance_product=PRACTICAL_ABUNDANCE_PRODUCT,
                 min_half_life=PRACTICAL_MIN_HALF_LIFE,
                 sacrifice_uniqueness=SACRIFICE_ISOTOPIC_UNIQUENESS,
                 verbose=VERBOSE)
-            recovered_charge, m_ion_candidates = crawler.combinatorics(
+            recovered_charge_state, m_ion_candidates = crawler.combinatorics(
                 m_ion.isotope_vector.typed_value,
                 m_ion.ranges.typed_value[0, 0],
                 m_ion.ranges.typed_value[0, 1])
-            # print(" " + str(recovered_charge))
-            m_ion.charge = NxField(np.int8(recovered_charge), "")
+            # print(f"{recovered_charge_state}")
+            m_ion.charge_state = NxField(np.int8(recovered_charge_state), "")
             m_ion.update_human_readable_name()
-            m_ion.add_charge_model(
+            m_ion.add_charge_state_model(
                 {"min_abundance": PRACTICAL_ABUNDANCE,
                  "min_abundance_product": PRACTICAL_ABUNDANCE_PRODUCT,
                  "min_half_life": PRACTICAL_MIN_HALF_LIFE,
                  "sacrifice_isotopic_uniqueness": SACRIFICE_ISOTOPIC_UNIQUENESS},
                 m_ion_candidates)
 
             self.rrng["molecular_ions"].append(m_ion)
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/__init__.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/definitions.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import numpy as np
 
 
 # restrict the number distinguished ion types
 MAX_NUMBER_OF_ION_SPECIES = 256
 # restrict number of atoms for molecular ion fragments
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/mmapped_io.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/mmapped_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import typing
 
 from typing import Tuple
 
 import mmap
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/molecular_ions.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/molecular_ions.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import typing
 
 from typing import Tuple
 
 import numpy as np
 
@@ -57,26 +57,26 @@
 # molecular ion candidate (which is non-trivial and maybe not even
 # with first principles theory possible...
 SACRIFICE_ISOTOPIC_UNIQUENESS = True
 VERBOSE=False
 
 
 class MolecularIonCandidate:
-    def __init__(self, ivec=[], charge=0, mass_sum=0., nat_abun_prod=0., min_half_life=np.inf):
+    def __init__(self, ivec=[], charge_state=0, mass_sum=0., nat_abun_prod=0., min_half_life=np.inf):
         self.isotope_vector = np.asarray(np.atleast_1d(ivec), np.uint16)
-        self.charge = np.int8(charge)
+        self.charge_state = np.int8(charge_state)
         self.mass = np.float64(mass_sum)
         self.abundance_product = np.float64(nat_abun_prod)
         self.shortest_half_life = np.float64(min_half_life)
 
     def unique_keyword(self):
         keyword = ""
         keyword += isotope_vector_to_dict_keyword(
             np.sort(np.asarray(self.isotope_vector, np.uint16), kind="stable")[::-1])
-        keyword += "__" + str(self.charge)
+        keyword += "__" + str(self.charge_state)
         return keyword
 
 
 class MolecularIonBuilder:
     def __init__(self,
                  min_abundance=1.0e-6,
                  min_abundance_product=1.0e-6,
@@ -174,15 +174,15 @@
         #     else:
         #         nuclids = np.append(nuclids, source_hashvalue)
         # return nuclids
 
     def get_isotope_mass_sum(self, nuclid_arr=[]):
         """Evaluate cumulated atomic_mass of isotopes in ivec."""
         # assuming no relativistic effects or other quantum effects
-        # mass loss due to charge state considered insignificant
+        # mass loss due to charge_state considered insignificant
         mass = 0.
         for hashvalue in nuclid_arr:
             if hashvalue != 0:
                 mass += self.nuclid_mass[hashvalue]
             # else:  # because ivec are systematically filled sorted in descending order !
             #   break
         return mass
@@ -236,15 +236,15 @@
             cand_arr_curr = []  # combinatorially add nuclids while recursing deeper
             self.iterate_molecular_ion(
                 element_arr, ith_nuclids, cand_arr_curr,
                 depth, max_depth, low, high)
             if self.parms["verbose"] is True:
                 print(f"Found {len(self.candidates)} candidates!")
             return self.try_to_reduce_to_unique_solution()
-            # will return a tuple of charge and list of relevant_candidates
+            # will return a tuple of charge_state and list of relevant_candidates
         else:
             return (0, [])
 
     def iterate_molecular_ion(self,
                               element_arr, jth_nuclids, cand_arr_prev,
                               i, max_n, low, high):
         if i < (max_n - 1):
@@ -316,36 +316,36 @@
             if self.parms["verbose"] is True:
                 print("One relevant candidate which meets all criteria")
             keywords = []
             for key in self.relevant.keys():
                 if isinstance(key, str):
                     keywords.append(key)
             assert len(keywords) >= 1, "List of relevant keywords is empty!"
-            return (self.relevant[keywords[0]].charge, relevant_candidates)
+            return (self.relevant[keywords[0]].charge_state, relevant_candidates)
         else:
             if self.parms["verbose"] is True:
                 print("Multiple relevant candidates meet all selection criteria")
             keywords = []
             for key in self.relevant.keys():
                 if isinstance(key, str):
                     keywords.append(key)
             assert len(keywords) >= 1, "List of relevant keywords is empty!"
-            charge = self.relevant[keywords[0]].charge
+            charge_state = self.relevant[keywords[0]].charge_state
             for key, val in self.relevant.items():
-                if val.charge == charge:
+                if val.charge_state == charge_state:
                     continue
                 else:
                     if self.parms["verbose"] is True:
-                        print("WARNING::Multiple relevant candidates differ in charge!")
+                        print("WARNING::Multiple relevant candidates differ in charge_state!")
                         print("WARNING::No unique solution possible for given criteria!")
                     return (0, relevant_candidates)
-            # not returned yet, so all relevant candidates have the same charge
+            # not returned yet, so all relevant candidates have the same charge_state
             if self.parms["verbose"] is True:
-                print(f"Multiple relevant candidates have all the same charge {charge}")
+                print(f"Multiple relevant candidates have all the same charge_state {charge_state}")
             if self.parms["sacrifice_isotopic_uniqueness"] is True:
-                return (charge, relevant_candidates)
+                return (charge_state, relevant_candidates)
 
             if self.parms["verbose"] is True:
                 print("WARNING::Multiple relevant candidates differ in isotopes!")
-                print("WARNING::But these have the same charge!")
+                print("WARNING::But these have the same charge_state!")
                 print("WARNING::No unique solution possible for given criteria!")
             return (0, relevant_candidates)
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/string_handling.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/string_handling.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import typing
 
 from typing import Tuple
 
 
 def rchop(string: str = "", suffix: str = "") -> str:
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling/utils/utils.py` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=E1101
+# pylint: disable=no-member,duplicate-code
 
 import re
 
 import typing
 
 from typing import Tuple
 
@@ -144,33 +144,33 @@
         if hashvalue != 0:
             lst.append(str(hashvalue))
     if lst != []:
         return "_".join(lst)
     return "0"  # "_".join(np.asarray(np.zeros((MAX_NUMBER_OF_ATOMS_PER_ION,)), np.uint16))
 
 
-def isotope_vector_to_human_readable_name(ivec: np.ndarray, charge: np.int8) -> str:
+def isotope_vector_to_human_readable_name(ivec: np.ndarray, charge_state: np.int8) -> str:
     """Get human-readable name from an isotope_vector."""
     assert len(ivec) <= MAX_NUMBER_OF_ATOMS_PER_ION, \
         "Argument isotope_vector len <= MAX_NUMBER_OF_ATOMS_PER_ION !"
     human_readable = ""
     if np.sum(ivec) != 0:
         for hashvalue in ivec:
             if hashvalue != 0:
                 protons, neutrons = hash_to_isotope(int(hashvalue))
                 if neutrons > 0:
                     human_readable += str(protons + neutrons) \
                         + chemical_symbols[protons]
                 else:
                     human_readable += chemical_symbols[protons]
                 human_readable += " "
-        if charge > 0 and charge < 8:
-            human_readable += "+" * charge
-        elif charge > -8 and charge < 0:
-            human_readable += "-" * -charge
+        if 0 < charge_state < 8:
+            human_readable += "+" * charge_state
+        elif -8 < charge_state < 0:
+            human_readable += "-" * -charge_state
         else:
             human_readable = human_readable.rstrip()
         return human_readable
     else:
         return "unknown_iontype"
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/PKG-INFO` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifes-apt-tc-data-modeling
-Version: 0.0.7
+Version: 0.0.8
 Summary: Foster exchange about data models and work towards clear specifications of file formats and data models in the research field of atom probe microscopy.
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ifes_apt_tc_data_modeling-0.0.7/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt` & `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.7/pyproject.toml` & `ifes_apt_tc_data_modeling-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifes_apt_tc_data_modeling"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "The NOMAD Authors" },
 ]
 description = "Foster exchange about data models and work towards clear specifications of file formats and data models in the research field of atom probe microscopy."
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.8,<3.11"
```

