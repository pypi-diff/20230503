# Comparing `tmp/aiida-fleur-1.3.1.tar.gz` & `tmp/aiida-fleur-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-fleur-1.3.1.tar", last modified: Thu Apr  7 08:37:42 2022, max compression
+gzip compressed data, was "aiida-fleur-2.0.0.tar", last modified: Wed May  3 19:47:03 2023, max compression
```

## Comparing `aiida-fleur-1.3.1.tar` & `aiida-fleur-2.0.0.tar`

### file list

```diff
@@ -1,254 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:42.003314 aiida-fleur-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9643 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15376 2022-04-07 08:37:42.003314 aiida-fleur-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14112 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.939313 aiida-fleur-1.3.1/aiida_fleur/
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.943313 aiida-fleur-1.3.1/aiida_fleur/calculation/
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/calculation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25867 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/calculation/fleur.py
--rw-r--r--   0 runner    (1001) docker     (121)    12542 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/calculation/fleurinputgen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.943313 aiida-fleur-1.3.1/aiida_fleur/cmdline/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3828 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.943313 aiida-fleur-1.3.1/aiida_fleur/cmdline/data/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1246 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6315 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/data/fleurinp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4083 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/data/parameters.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2545 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/data/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.943313 aiida-fleur-1.3.1/aiida_fleur/cmdline/launch/
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/launch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15226 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/launch/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.943313 aiida-fleur-1.3.1/aiida_fleur/cmdline/list/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1008 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.943313 aiida-fleur-1.3.1/aiida_fleur/cmdline/util/
--rwxr-xr-x   0 runner    (1001) docker     (121)      821 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/util/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7990 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/util/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/util/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.947313 aiida-fleur-1.3.1/aiida_fleur/cmdline/visualization/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3112 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.947313 aiida-fleur-1.3.1/aiida_fleur/cmdline/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6382 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/cmdline/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.947313 aiida-fleur-1.3.1/aiida_fleur/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/common/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/common/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/common/node_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.947313 aiida-fleur-1.3.1/aiida_fleur/data/
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29025 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/data/fleurinp.py
--rw-r--r--   0 runner    (1001) docker     (121)    32105 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/data/fleurinpmodifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.947313 aiida-fleur-1.3.1/aiida_fleur/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13751 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/parsers/fleur.py
--rw-r--r--   0 runner    (1001) docker     (121)     6457 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/parsers/fleur_inputgen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.959313 aiida-fleur-1.3.1/aiida_fleur/tools/
--rw-r--r--   0 runner    (1001) docker     (121)    98996 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/StructureData_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8702 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/common_aiida.py
--rw-r--r--   0 runner    (1001) docker     (121)    24463 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/common_fleur_wf.py
--rw-r--r--   0 runner    (1001) docker     (121)    19655 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/common_fleur_wf_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     7824 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/create_corehole.py
--rw-r--r--   0 runner    (1001) docker     (121)     6308 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/create_kpoints_from_distance.py
--rw-r--r--   0 runner    (1001) docker     (121)     8952 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/decide_ncore.py
--rw-r--r--   0 runner    (1001) docker     (121)     4670 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (121)   128560 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/element_econfig_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    64282 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/exp_bindingenergies.json
--rw-r--r--   0 runner    (1001) docker     (121)    16722 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/extract_corelevels.py
--rw-r--r--   0 runner    (1001) docker     (121)     7915 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/io_routines.py
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/merge_parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.959313 aiida-fleur-1.3.1/aiida_fleur/tools/plot/
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22476 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/plot/fleur.py
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/queue_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     8915 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/read_cif_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/tools/xml_aiida_modifiers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.963313 aiida-fleur-1.3.1/aiida_fleur/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29621 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/banddos.py
--rw-r--r--   0 runner    (1001) docker     (121)    17381 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/base_fleur.py
--rw-r--r--   0 runner    (1001) docker     (121)    15923 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/base_relax.py
--rw-r--r--   0 runner    (1001) docker     (121)    46779 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/cfcoeff.py
--rw-r--r--   0 runner    (1001) docker     (121)    57985 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/corehole.py
--rw-r--r--   0 runner    (1001) docker     (121)    22730 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/create_magnetic_film.py
--rw-r--r--   0 runner    (1001) docker     (121)    22551 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/dmi.py
--rw-r--r--   0 runner    (1001) docker     (121)     8766 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/dos.py
--rw-r--r--   0 runner    (1001) docker     (121)    21020 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/eos.py
--rw-r--r--   0 runner    (1001) docker     (121)    51358 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/initial_cls.py
--rw-r--r--   0 runner    (1001) docker     (121)    22378 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/mae.py
--rw-r--r--   0 runner    (1001) docker     (121)     9092 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/mae_conv.py
--rw-r--r--   0 runner    (1001) docker     (121)     8154 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/optimize_para.py
--rw-r--r--   0 runner    (1001) docker     (121)    42513 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/orbcontrol.py
--rw-r--r--   0 runner    (1001) docker     (121)    26088 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/relax.py
--rw-r--r--   0 runner    (1001) docker     (121)    41115 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/scf.py
--rw-r--r--   0 runner    (1001) docker     (121)    20977 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/ssdisp.py
--rw-r--r--   0 runner    (1001) docker     (121)     9395 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/ssdisp_conv.py
--rw-r--r--   0 runner    (1001) docker     (121)    17793 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/aiida_fleur/workflows/strain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.943313 aiida-fleur-1.3.1/aiida_fleur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15376 2022-04-07 08:37:41.000000 aiida-fleur-1.3.1/aiida_fleur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9141 2022-04-07 08:37:41.000000 aiida-fleur-1.3.1/aiida_fleur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-07 08:37:41.000000 aiida-fleur-1.3.1/aiida_fleur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-04-07 08:37:41.000000 aiida-fleur-1.3.1/aiida_fleur.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-04-07 08:37:41.000000 aiida-fleur-1.3.1/aiida_fleur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-07 08:37:41.000000 aiida-fleur-1.3.1/aiida_fleur.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.963313 aiida-fleur-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     5814 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/rtd_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.963313 aiida-fleur-1.3.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.967313 aiida-fleur-1.3.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (121)    14997 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.967313 aiida-fleur-1.3.1/docs/source/devel_guide/
--rw-r--r--   0 runner    (1001) docker     (121)    18306 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/devel_guide/dg_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.979313 aiida-fleur-1.3.1/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (121)    76300 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/AiiDA_transparent_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    69068 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/Bands_colored.png
--rw-r--r--   0 runner    (1001) docker     (121)    32204 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/Lattice_constant.png
--rw-r--r--   0 runner    (1001) docker     (121)    30306 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/Logo-JLVMD.png
--rw-r--r--   0 runner    (1001) docker     (121)   166602 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/MAX-orizz.png
--rw-r--r--   0 runner    (1001) docker     (121)   151790 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/Workchain_charts_corehole_wc.png
--rw-r--r--   0 runner    (1001) docker     (121)   143048 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/Workchain_charts_dos_wc.png
--rw-r--r--   0 runner    (1001) docker     (121)   101867 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/Workchain_charts_eos_wc.png
--rw-r--r--   0 runner    (1001) docker     (121)   180439 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/Workchain_charts_initial_state.png
--rw-r--r--   0 runner    (1001) docker     (121)   140196 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/Workchain_charts_relaxation.png
--rw-r--r--   0 runner    (1001) docker     (121)   172833 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/Workchain_charts_scf_wc.png
--rw-r--r--   0 runner    (1001) docker     (121)   303108 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/aiida_work2_ed.png
--rw-r--r--   0 runner    (1001) docker     (121)   905411 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/all_logos.odg
--rw-r--r--   0 runner    (1001) docker     (121)    56481 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/all_logos.png
--rw-r--r--   0 runner    (1001) docker     (121)    39864 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/all_rmts_oqmd.png
--rw-r--r--   0 runner    (1001) docker     (121)    76300 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/b_AiiDA_transparent_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    40667 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/band_d_like.png
--rw-r--r--   0 runner    (1001) docker     (121)    24267 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/band_f_like.png
--rw-r--r--   0 runner    (1001) docker     (121)    49117 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/band_p_like.png
--rw-r--r--   0 runner    (1001) docker     (121)    40276 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/band_s_like.png
--rw-r--r--   0 runner    (1001) docker     (121)    25548 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/bandstructure.png
--rw-r--r--   0 runner    (1001) docker     (121)   220261 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/convergence_all_MP_metals.png
--rw-r--r--   0 runner    (1001) docker     (121)    90461 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/convergence_all_MP_metals1.png
--rw-r--r--   0 runner    (1001) docker     (121)    55113 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/corehole_si_30528.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    23310 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/dos_76867.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    29416 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/dos_plot.png
--rw-r--r--   0 runner    (1001) docker     (121)    66472 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/eos_49670.pdf
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/eos_wc_outputnode.py
--rw-r--r--   0 runner    (1001) docker     (121)    16720 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/fleur.png
--rw-r--r--   0 runner    (1001) docker     (121)   108741 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/plot_fleur_capabilities.png
--rw-r--r--   0 runner    (1001) docker     (121)   165390 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/plot_fleur_eos_mn.png
--rw-r--r--   0 runner    (1001) docker     (121)    93663 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/plot_fleur_eos_sn.png
--rw-r--r--   0 runner    (1001) docker     (121)    27980 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/plot_fleur_scf1.png
--rw-r--r--   0 runner    (1001) docker     (121)    35159 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/plot_fleur_scf2.png
--rw-r--r--   0 runner    (1001) docker     (121)   209736 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/plot_fleur_scf_m1.png
--rw-r--r--   0 runner    (1001) docker     (121)   134392 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/plot_fleur_scf_m2.png
--rw-r--r--   0 runner    (1001) docker     (121)    27046 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/images/scf_50816.pdf
--rw-r--r--   0 runner    (1001) docker     (121)     7295 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.983313 aiida-fleur-1.3.1/docs/source/module_guide/
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/module_guide/code.rst
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/module_guide/mg_index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/module_guide/tools.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.983313 aiida-fleur-1.3.1/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/reference/_changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.983313 aiida-fleur-1.3.1/docs/source/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.983313 aiida-fleur-1.3.1/docs/source/user_guide/calculations/
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/calculations/fleur_calculation_plugins.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11973 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/calculations/fleurcode_plugin.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.983313 aiida-fleur-1.3.1/docs/source/user_guide/calculations/images/
--rw-r--r--   0 runner    (1001) docker     (121)    37131 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/calculations/images/fleur_calc.png
--rw-r--r--   0 runner    (1001) docker     (121)    43028 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/calculations/images/fleurinpgen_calc.png
--rw-r--r--   0 runner    (1001) docker     (121)     8870 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/calculations/inpgen_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/calculations/output_node_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/calculations/parameter_example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.983313 aiida-fleur-1.3.1/docs/source/user_guide/cmd/
--rw-r--r--   0 runner    (1001) docker     (121)    14720 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/cmd/cmd_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.983313 aiida-fleur-1.3.1/docs/source/user_guide/data/
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/data/fleur_data_plugins.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8384 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/data/fleurinp_data.rst
--rw-r--r--   0 runner    (1001) docker     (121)    17276 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/data/fleurinp_modifier.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.987313 aiida-fleur-1.3.1/docs/source/user_guide/data/images/
--rw-r--r--   0 runner    (1001) docker     (121)   161558 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/data/images/fleurinpdata.png
--rw-r--r--   0 runner    (1001) docker     (121)   194046 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/data/images/fleurinpmodifier.png
--rw-r--r--   0 runner    (1001) docker     (121)   169818 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/data/images/registration_methods.png
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/data/parameter_example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.987313 aiida-fleur-1.3.1/docs/source/user_guide/getting_started/
--rw-r--r--   0 runner    (1001) docker     (121)    12904 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/getting_started/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.987313 aiida-fleur-1.3.1/docs/source/user_guide/hints/
--rw-r--r--   0 runner    (1001) docker     (121)    19090 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/hints/exit_codes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/hints/hints_faq.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.987313 aiida-fleur-1.3.1/docs/source/user_guide/tools/
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/tools/tools_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.987313 aiida-fleur-1.3.1/docs/source/user_guide/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/ug_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.991314 aiida-fleur-1.3.1/docs/source/user_guide/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/base_relax_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8500 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/base_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6416 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/cfcoeff_wc.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:41.995314 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/banddos_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/banddos_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/cfcoeff_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/corehole_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/corehole_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/corehole_wc_outputnode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/create_magnetic_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/create_magnetic_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/dmi_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2602 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/dmi_wc_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/initial_cls_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/initial_cls_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/initial_cls_wc_outputnode.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/mae_conv_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/mae_conv_wc_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/mae_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/mae_wc_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/orbcontrol_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/orbcontrol_wc_outputnode.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/relax_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/relax_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/scf_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/scf_wc_outputnode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/scf_wc_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/ssdisp_conv_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/ssdisp_conv_wc_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/ssdisp_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/ssdisp_wc_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/tutorial_submit_eos.py
--rw-r--r--   0 runner    (1001) docker     (121)     5376 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/corehole_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)    16087 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/create_magnetic_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13052 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/dmi_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12638 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/dos_band_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/eos_wc.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 08:37:42.003314 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/
--rw-r--r--   0 runner    (1001) docker     (121)   126414 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/base_restart_scheme.png
--rw-r--r--   0 runner    (1001) docker     (121)   146504 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/create_magnetic_AFM_bcc110.png
--rw-r--r--   0 runner    (1001) docker     (121)   111317 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/create_magnetic_AFM_fcc110.png
--rw-r--r--   0 runner    (1001) docker     (121)   136960 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/create_magnetic_scheme.png
--rw-r--r--   0 runner    (1001) docker     (121)   143867 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/dmi.png
--rw-r--r--   0 runner    (1001) docker     (121)   200622 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/mae_conv.png
--rw-r--r--   0 runner    (1001) docker     (121)   131020 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/mae_energies.png
--rw-r--r--   0 runner    (1001) docker     (121)   243259 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/mae_force.png
--rw-r--r--   0 runner    (1001) docker     (121)    18168 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/plot_fleur_orbcontrol.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   114438 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/ssdisp_conv.png
--rw-r--r--   0 runner    (1001) docker     (121)    54145 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/ssdisp_energies.png
--rw-r--r--   0 runner    (1001) docker     (121)   136589 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/ssdisp_force.png
--rw-r--r--   0 runner    (1001) docker     (121)   156786 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/workchains2.png
--rw-r--r--   0 runner    (1001) docker     (121)     6991 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/initial_cls_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6715 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/mae_conv_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11470 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/mae_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13046 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/orbcontrol_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7013 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/relax_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13350 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/scf_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6588 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/ssdisp_conv_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11607 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/ssdisp_wc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4242 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/docs/source/user_guide/workflows/wc_index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-07 08:37:42.003314 aiida-fleur-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/setup.json
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-04-07 08:37:27.000000 aiida-fleur-1.3.1/setup_requirements.txt
+-rw-r--r--   0        0        0     5803 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      816 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2080 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/.gitignore
+-rw-r--r--   0        0        0      517 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/.gource.conf
+-rw-r--r--   0        0        0     1424 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      461 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0     3947 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/.zenodo.json
+-rw-r--r--   0        0        0      518 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/AUTHORS.txt
+-rw-r--r--   0        0        0    12199 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1264 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/LICENSE
+-rw-r--r--   0        0        0    31224 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/README.md
+-rw-r--r--   0        0        0     3526 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/STYLE_CONVENTION.txt
+-rw-r--r--   0        0        0      946 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/calculation/__init__.py
+-rw-r--r--   0        0        0    26258 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/calculation/fleur.py
+-rw-r--r--   0        0        0    12389 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/calculation/fleurinputgen.py
+-rwxr-xr-x   0        0        0     3828 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/__init__.py
+-rwxr-xr-x   0        0        0     1246 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/data/__init__.py
+-rwxr-xr-x   0        0        0     9076 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/data/fleurinp.py
+-rw-r--r--   0        0        0     4083 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/data/parameters.py
+-rwxr-xr-x   0        0        0     2545 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/data/structure.py
+-rw-r--r--   0        0        0     1968 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/launch/__init__.py
+-rwxr-xr-x   0        0        0    15151 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/launch/launch.py
+-rwxr-xr-x   0        0        0     1008 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/list/__init__.py
+-rwxr-xr-x   0        0        0      821 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/util/__init__.py
+-rw-r--r--   0        0        0     4167 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/util/defaults.py
+-rwxr-xr-x   0        0        0     8035 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/util/options.py
+-rw-r--r--   0        0        0     3131 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/util/types.py
+-rw-r--r--   0        0        0     2338 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/util/utils.py
+-rwxr-xr-x   0        0        0     3112 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/visualization/__init__.py
+-rwxr-xr-x   0        0        0     6382 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/cmdline/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/common/__init__.py
+-rw-r--r--   0        0        0     1282 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/common/defaults.py
+-rw-r--r--   0        0        0     4391 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/common/node_generators.py
+-rw-r--r--   0        0        0     1041 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/data/__init__.py
+-rw-r--r--   0        0        0    33530 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/data/fleurinp.py
+-rw-r--r--   0        0        0    23767 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/data/fleurinpmodifier.py
+-rw-r--r--   0        0        0     1104 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/parsers/__init__.py
+-rw-r--r--   0        0        0    14103 2023-05-03 19:46:57.903333 aiida-fleur-2.0.0/aiida_fleur/parsers/fleur.py
+-rw-r--r--   0        0        0     6453 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/parsers/fleur_inputgen.py
+-rw-r--r--   0        0        0    97177 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/StructureData_util.py
+-rw-r--r--   0        0        0      823 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/__init__.py
+-rw-r--r--   0        0        0     5394 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/bfgs.py
+-rw-r--r--   0        0        0     8696 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/common_aiida.py
+-rw-r--r--   0        0        0    24330 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/common_fleur_wf.py
+-rw-r--r--   0        0        0    19552 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/common_fleur_wf_util.py
+-rw-r--r--   0        0        0     7824 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/create_corehole.py
+-rw-r--r--   0        0        0     6303 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/create_kpoints_from_distance.py
+-rw-r--r--   0        0        0     8962 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/data_handling.py
+-rw-r--r--   0        0        0     4670 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/dict_util.py
+-rw-r--r--   0        0        0   128578 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/element_econfig_list.py
+-rw-r--r--   0        0        0    64282 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/exp_bindingenergies.json
+-rw-r--r--   0        0        0    17026 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/extract_corelevels.py
+-rw-r--r--   0        0        0     7931 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/io_routines.py
+-rw-r--r--   0        0        0     5643 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/merge_parameter.py
+-rw-r--r--   0        0        0      844 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/plot/__init__.py
+-rw-r--r--   0        0        0    22832 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/plot/fleur.py
+-rw-r--r--   0        0        0     2803 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/queue_defaults.py
+-rw-r--r--   0        0        0     8925 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/read_cif_folder.py
+-rw-r--r--   0        0        0     1998 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/straight_torque.py
+-rw-r--r--   0        0        0     3089 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/tools/xml_aiida_modifiers.py
+-rw-r--r--   0        0        0      831 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/workflows/__init__.py
+-rw-r--r--   0        0        0    29296 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/workflows/banddos.py
+-rw-r--r--   0        0        0    17840 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/workflows/base_fleur.py
+-rw-r--r--   0        0        0    15151 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/workflows/base_relax.py
+-rw-r--r--   0        0        0    45939 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/workflows/cfcoeff.py
+-rw-r--r--   0        0        0    57115 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/workflows/corehole.py
+-rw-r--r--   0        0        0    23371 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/workflows/create_magnetic_film.py
+-rw-r--r--   0        0        0    21449 2023-05-03 19:46:57.907333 aiida-fleur-2.0.0/aiida_fleur/workflows/dmi.py
+-rw-r--r--   0        0        0     8740 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/dos.py
+-rw-r--r--   0        0        0    21053 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/eos.py
+-rw-r--r--   0        0        0    50999 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/initial_cls.py
+-rw-r--r--   0        0        0    21508 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/mae.py
+-rw-r--r--   0        0        0     8585 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/mae_conv.py
+-rw-r--r--   0        0        0    51043 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/orbcontrol.py
+-rw-r--r--   0        0        0    25660 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/relax.py
+-rw-r--r--   0        0        0    22932 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/relax_torque.py
+-rw-r--r--   0        0        0    46717 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/scf.py
+-rw-r--r--   0        0        0    19872 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/ssdisp.py
+-rw-r--r--   0        0        0     8719 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/ssdisp_conv.py
+-rw-r--r--   0        0        0    17769 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/aiida_fleur/workflows/strain.py
+-rw-r--r--   0        0        0     5814 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/docs/Makefile
+-rw-r--r--   0        0        0      738 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/docs/README.rst
+-rw-r--r--   0        0        0     2734 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/docs/rtd_settings.py
+-rw-r--r--   0        0        0      365 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0        0        0    15051 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0    18354 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/docs/source/devel_guide/dg_index.rst
+-rw-r--r--   0        0        0    76300 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/docs/source/images/AiiDA_transparent_logo.png
+-rw-r--r--   0        0        0    69068 2023-05-03 19:46:57.911333 aiida-fleur-2.0.0/docs/source/images/Bands_colored.png
+-rw-r--r--   0        0        0    32204 2023-05-03 19:46:57.915333 aiida-fleur-2.0.0/docs/source/images/Lattice_constant.png
+-rw-r--r--   0        0        0    30306 2023-05-03 19:46:57.915333 aiida-fleur-2.0.0/docs/source/images/Logo-JLVMD.png
+-rw-r--r--   0        0        0   166602 2023-05-03 19:46:57.915333 aiida-fleur-2.0.0/docs/source/images/MAX-orizz.png
+-rw-r--r--   0        0        0   151790 2023-05-03 19:46:57.915333 aiida-fleur-2.0.0/docs/source/images/Workchain_charts_corehole_wc.png
+-rw-r--r--   0        0        0   143048 2023-05-03 19:46:57.915333 aiida-fleur-2.0.0/docs/source/images/Workchain_charts_dos_wc.png
+-rw-r--r--   0        0        0   101867 2023-05-03 19:46:57.919333 aiida-fleur-2.0.0/docs/source/images/Workchain_charts_eos_wc.png
+-rw-r--r--   0        0        0   180439 2023-05-03 19:46:57.919333 aiida-fleur-2.0.0/docs/source/images/Workchain_charts_initial_state.png
+-rw-r--r--   0        0        0   140196 2023-05-03 19:46:57.919333 aiida-fleur-2.0.0/docs/source/images/Workchain_charts_relaxation.png
+-rw-r--r--   0        0        0   172833 2023-05-03 19:46:57.919333 aiida-fleur-2.0.0/docs/source/images/Workchain_charts_scf_wc.png
+-rw-r--r--   0        0        0   303108 2023-05-03 19:46:57.919333 aiida-fleur-2.0.0/docs/source/images/aiida_work2_ed.png
+-rw-r--r--   0        0        0   905411 2023-05-03 19:46:57.923333 aiida-fleur-2.0.0/docs/source/images/all_logos.odg
+-rw-r--r--   0        0        0    56481 2023-05-03 19:46:57.923333 aiida-fleur-2.0.0/docs/source/images/all_logos.png
+-rw-r--r--   0        0        0    39864 2023-05-03 19:46:57.927333 aiida-fleur-2.0.0/docs/source/images/all_rmts_oqmd.png
+-rw-r--r--   0        0        0    76300 2023-05-03 19:46:57.927333 aiida-fleur-2.0.0/docs/source/images/b_AiiDA_transparent_logo.png
+-rw-r--r--   0        0        0    40667 2023-05-03 19:46:57.927333 aiida-fleur-2.0.0/docs/source/images/band_d_like.png
+-rw-r--r--   0        0        0    24267 2023-05-03 19:46:57.927333 aiida-fleur-2.0.0/docs/source/images/band_f_like.png
+-rw-r--r--   0        0        0    49117 2023-05-03 19:46:57.927333 aiida-fleur-2.0.0/docs/source/images/band_p_like.png
+-rw-r--r--   0        0        0    40276 2023-05-03 19:46:57.927333 aiida-fleur-2.0.0/docs/source/images/band_s_like.png
+-rw-r--r--   0        0        0    25548 2023-05-03 19:46:57.927333 aiida-fleur-2.0.0/docs/source/images/bandstructure.png
+-rw-r--r--   0        0        0   220261 2023-05-03 19:46:57.927333 aiida-fleur-2.0.0/docs/source/images/convergence_all_MP_metals.png
+-rw-r--r--   0        0        0    90461 2023-05-03 19:46:57.931333 aiida-fleur-2.0.0/docs/source/images/convergence_all_MP_metals1.png
+-rw-r--r--   0        0        0    55113 2023-05-03 19:46:57.931333 aiida-fleur-2.0.0/docs/source/images/corehole_si_30528.pdf
+-rw-r--r--   0        0        0    23310 2023-05-03 19:46:57.931333 aiida-fleur-2.0.0/docs/source/images/dos_76867.pdf
+-rw-r--r--   0        0        0    29416 2023-05-03 19:46:57.931333 aiida-fleur-2.0.0/docs/source/images/dos_plot.png
+-rw-r--r--   0        0        0    66472 2023-05-03 19:46:57.931333 aiida-fleur-2.0.0/docs/source/images/eos_49670.pdf
+-rw-r--r--   0        0        0     1306 2023-05-03 19:46:57.931333 aiida-fleur-2.0.0/docs/source/images/eos_wc_outputnode.py
+-rw-r--r--   0        0        0    16720 2023-05-03 19:46:57.931333 aiida-fleur-2.0.0/docs/source/images/fleur.png
+-rw-r--r--   0        0        0   108741 2023-05-03 19:46:57.931333 aiida-fleur-2.0.0/docs/source/images/plot_fleur_capabilities.png
+-rw-r--r--   0        0        0   165390 2023-05-03 19:46:57.931333 aiida-fleur-2.0.0/docs/source/images/plot_fleur_eos_mn.png
+-rw-r--r--   0        0        0    93663 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/images/plot_fleur_eos_sn.png
+-rw-r--r--   0        0        0    27980 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/images/plot_fleur_scf1.png
+-rw-r--r--   0        0        0    35159 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/images/plot_fleur_scf2.png
+-rw-r--r--   0        0        0   209736 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/images/plot_fleur_scf_m1.png
+-rw-r--r--   0        0        0   134392 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/images/plot_fleur_scf_m2.png
+-rw-r--r--   0        0        0    27046 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/images/scf_50816.pdf
+-rw-r--r--   0        0        0     7295 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/index.rst
+-rw-r--r--   0        0        0     3581 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/module_guide/code.rst
+-rw-r--r--   0        0        0      140 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/module_guide/mg_index.rst
+-rw-r--r--   0        0        0     1239 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/module_guide/tools.rst
+-rw-r--r--   0        0        0     5603 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/nitpick-exceptions
+-rw-r--r--   0        0        0       79 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/reference/_changelog.md
+-rw-r--r--   0        0        0       71 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/reference/index.rst
+-rw-r--r--   0        0        0      508 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/user_guide/calculations/fleur_calculation_plugins.rst
+-rw-r--r--   0        0        0    13241 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/user_guide/calculations/fleurcode_plugin.rst
+-rw-r--r--   0        0        0    37131 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/user_guide/calculations/images/fleur_calc.png
+-rw-r--r--   0        0        0    43028 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/user_guide/calculations/images/fleurinpgen_calc.png
+-rw-r--r--   0        0        0     8866 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/user_guide/calculations/inpgen_plugin.rst
+-rw-r--r--   0        0        0     2662 2023-05-03 19:46:57.935333 aiida-fleur-2.0.0/docs/source/user_guide/calculations/output_node_example.py
+-rw-r--r--   0        0        0      837 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/calculations/parameter_example.py
+-rw-r--r--   0        0        0    14720 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/cmd/cmd_index.rst
+-rw-r--r--   0        0        0      821 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/data/fleur_data_plugins.rst
+-rw-r--r--   0        0        0     8370 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/data/fleurinp_data.rst
+-rw-r--r--   0        0        0    20011 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/data/fleurinp_modifier.rst
+-rw-r--r--   0        0        0   161558 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/data/images/fleurinpdata.png
+-rw-r--r--   0        0        0   194046 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/data/images/fleurinpmodifier.png
+-rw-r--r--   0        0        0   169818 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/data/images/registration_methods.png
+-rw-r--r--   0        0        0      918 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/data/parameter_example.py
+-rw-r--r--   0        0        0    12904 2023-05-03 19:46:57.939333 aiida-fleur-2.0.0/docs/source/user_guide/getting_started/getting_started.rst
+-rw-r--r--   0        0        0    19090 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/hints/exit_codes.rst
+-rw-r--r--   0        0        0     1762 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/hints/hints_faq.rst
+-rw-r--r--   0        0        0      887 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/tools/tools_index.rst
+-rw-r--r--   0        0        0     1591 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/tutorials/tutorials.rst
+-rw-r--r--   0        0        0      353 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/ug_index.rst
+-rw-r--r--   0        0        0      930 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/base_relax_wc.rst
+-rw-r--r--   0        0        0     8500 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/base_wc.rst
+-rw-r--r--   0        0        0     6416 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/cfcoeff_wc.rst
+-rw-r--r--   0        0        0      499 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/banddos_parameters.py
+-rw-r--r--   0        0        0     2009 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/banddos_submission.py
+-rw-r--r--   0        0        0      713 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/cfcoeff_parameters.py
+-rw-r--r--   0        0        0      966 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/corehole_parameters.py
+-rw-r--r--   0        0        0     1044 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/corehole_submission.py
+-rw-r--r--   0        0        0     1675 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/corehole_wc_outputnode.py
+-rw-r--r--   0        0        0     1865 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/create_magnetic_parameters.py
+-rw-r--r--   0        0        0     3675 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/create_magnetic_submission.py
+-rw-r--r--   0        0        0      946 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/dmi_parameters.py
+-rw-r--r--   0        0        0     2602 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/dmi_wc_submission.py
+-rw-r--r--   0        0        0      653 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/initial_cls_parameters.py
+-rw-r--r--   0        0        0     1093 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/initial_cls_submission.py
+-rw-r--r--   0        0        0     3188 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/initial_cls_wc_outputnode.py
+-rw-r--r--   0        0        0      176 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/mae_conv_parameters.py
+-rw-r--r--   0        0        0     1945 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/mae_conv_wc_submission.py
+-rw-r--r--   0        0        0      840 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/mae_parameters.py
+-rw-r--r--   0        0        0     2489 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/mae_wc_submission.py
+-rw-r--r--   0        0        0     1053 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/orbcontrol_parameters.py
+-rw-r--r--   0        0        0     1100 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/orbcontrol_wc_outputnode.py
+-rw-r--r--   0        0        0      266 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/relax_parameters.py
+-rw-r--r--   0        0        0     2066 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/relax_submission.py
+-rw-r--r--   0        0        0     1038 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/scf_parameters.py
+-rw-r--r--   0        0        0      735 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/scf_wc_outputnode.py
+-rw-r--r--   0        0        0     1354 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/scf_wc_submission.py
+-rw-r--r--   0        0        0      299 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/ssdisp_conv_parameters.py
+-rw-r--r--   0        0        0     2097 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/ssdisp_conv_wc_submission.py
+-rw-r--r--   0        0        0      837 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/ssdisp_parameters.py
+-rw-r--r--   0        0        0     2124 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/ssdisp_wc_submission.py
+-rw-r--r--   0        0        0     1463 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/tutorial_submit_eos.py
+-rw-r--r--   0        0        0     5376 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/corehole_wc.rst
+-rw-r--r--   0        0        0    16087 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/create_magnetic_wc.rst
+-rw-r--r--   0        0        0    13052 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/dmi_wc.rst
+-rw-r--r--   0        0        0    12638 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/dos_band_wc.rst
+-rw-r--r--   0        0        0     5828 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/eos_wc.rst
+-rw-r--r--   0        0        0   126414 2023-05-03 19:46:57.943333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/base_restart_scheme.png
+-rw-r--r--   0        0        0   146504 2023-05-03 19:46:57.947333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/create_magnetic_AFM_bcc110.png
+-rw-r--r--   0        0        0   111317 2023-05-03 19:46:57.947333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/create_magnetic_AFM_fcc110.png
+-rw-r--r--   0        0        0   136960 2023-05-03 19:46:57.947333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/create_magnetic_scheme.png
+-rw-r--r--   0        0        0   143867 2023-05-03 19:46:57.947333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/dmi.png
+-rw-r--r--   0        0        0   200622 2023-05-03 19:46:57.947333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/mae_conv.png
+-rw-r--r--   0        0        0   131020 2023-05-03 19:46:57.951333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/mae_energies.png
+-rw-r--r--   0        0        0   243259 2023-05-03 19:46:57.951333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/mae_force.png
+-rw-r--r--   0        0        0    18168 2023-05-03 19:46:57.951333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/plot_fleur_orbcontrol.pdf
+-rw-r--r--   0        0        0   114438 2023-05-03 19:46:57.951333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/ssdisp_conv.png
+-rw-r--r--   0        0        0    54145 2023-05-03 19:46:57.951333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/ssdisp_energies.png
+-rw-r--r--   0        0        0   136589 2023-05-03 19:46:57.951333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/ssdisp_force.png
+-rw-r--r--   0        0        0   156786 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/workchains2.png
+-rw-r--r--   0        0        0     6991 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/initial_cls_wc.rst
+-rw-r--r--   0        0        0     6715 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/mae_conv_wc.rst
+-rw-r--r--   0        0        0    11470 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/mae_wc.rst
+-rw-r--r--   0        0        0    13046 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/orbcontrol_wc.rst
+-rw-r--r--   0        0        0     7013 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/relax_wc.rst
+-rw-r--r--   0        0        0    13568 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/scf_wc.rst
+-rw-r--r--   0        0        0     6588 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/ssdisp_conv_wc.rst
+-rw-r--r--   0        0        0    11607 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/ssdisp_wc.rst
+-rw-r--r--   0        0        0     4242 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/docs/source/user_guide/workflows/wc_index.rst
+-rw-r--r--   0        0        0     6774 2023-05-03 19:46:57.955333 aiida-fleur-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    33734 1970-01-01 00:00:00.000000 aiida-fleur-2.0.0/PKG-INFO
```

### Comparing `aiida-fleur-1.3.1/AUTHORS.txt` & `aiida-fleur-2.0.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/LICENSE` & `aiida-fleur-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/README.md` & `aiida-fleur-2.0.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,226 +1,253 @@
-# FLEUR with AiiDA
+# Changelog
 
-[![MIT license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
-[![GitHub release](https://img.shields.io/github/release/JuDFTteam/aiida-fleur.svg)](https://github.com/JuDFTteam/aiida-fleur/releases)
-[![PyPI version](https://badge.fury.io/py/aiida-fleur.svg)](https://badge.fury.io/py/aiida-fleur)
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-fleur.svg)](https://pypi.python.org/pypi/aiida-fleur)
-[![Build status](https://github.com/JuDFTteam/aiida-fleur/workflows/aiida-fleur/badge.svg?branch=develop&event=push)](https://github.com/JuDFTteam/aiida-fleur/actions)
-[![Documentation Status](https://readthedocs.org/projects/aiida-fleur/badge/?version=develop)](https://aiida-fleur.readthedocs.io/en/develop/?badge=develop)
-[![codecov](https://codecov.io/gh/JuDFTteam/aiida-fleur/branch/develop/graph/badge.svg)](https://codecov.io/gh/JuDFTteam/aiida-fleur)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5531549.svg)](https://doi.org/10.5281/zenodo.5531549)
+## v.2.0.0
+First release with official support for AiiDA version 2.0. Support for AiiDA 1.X is only
+available with releases from the 1.X series of aiida-fleur. Dropped python 3.7 support.
+Added support for python 3.11.
+
+### Breaking changes
+- The entries `last_calc_uuid` from output dictionary of `FleurSCFWorkChain` and `last_scf_wc_uuid` from `FleurRelaxWorkChain` are removed. Reasoning for this is that having UUIDs in the output dictionary makes it impossible to take advantage of AiiDA's caching mechanism. Both workchains expose the relevant outputs of the under the namespaces `last_calc` and `last_scf` respectively
+- Several input/output port changes:
+  - `FleurBandDOSworkChain`: Removed `last_calc_retrieved`, replaced with namespace `banddos_calc`
+  - `FleurBaseWorkChain`: Removed `final_calc_uuid`
+  - Adjusted name of output dictionary to the naming schema `output_<wc_abbrev>_wc_para`: `FleurDMIWorkChain`, `FleurMAEConvWorkChain`, `FleurSSDispWorkChain`, `FleurSSDicpConvWorkChain`
+  - `FleurSCFWorkChain`: Removed `last_fleur_calc_output`. Is available under `last_calc.output_parameters`
+  - Ports for generic `FleurinpData` are renamed to consistently be `fleurinp`. Affects `FleurCalculation`, `FleurinputgenCalculation`, `FleurBaseWorkChain`
+
+### Expired Deprecations
+- `FleurinpModifier`: Removed compatibility with old method names/behaviour before introducing `masci-tools`
+- `FleurinpData`: Removed `get_tag`. Use `load_inpxml` and any evaluation routine afterwards instead
+- Coordinate conversion functions `abs_to_rel`, etc., These are available in `masci-tools`
+- Removed `constants` module. Now only available in `masci-tools`
+
+
+### Improvements
+- New workchain `FleurRelaxTorqueWorkChain` for relaxing non-collinear magnetic configurations
+- Fixes in DFT+U handling
+  - `FleurCalculation`: added `fleurinp_nmmpmat_priority` key to `settings` to control from where to take the `n_mmp_mat` file if it's in the fleurinp and parent_folder input
+  - Fixed several errors in orbcontrol workchain when handling non-converged/failed calculation
+  - Added inputs to orbcontrol to restart from intermediate charge densities
+- Added `inpxml_changes` contextmanager for easier creation of the workflow parameters input of the same name
+```python
+from aiida_fleur.data import inpxml_changes
+
+wf_parameters = {}
+
+with inpxml_changes(wf_parameters) as fm:
+  fm.set_inpchanges({'kmax': 4, 'itmax': 100})
+  fm.set_species('all', {'mtsphere': {'radius': 3}})
 
-This software contains a plugin that enables the usage of the all-electron
-DFT [FLEUR code](http://www.flapw.de) with the [AiiDA framework](http://www.aiida.net).
-
-Developed at [Forschungszentrum Jülich GmbH](http://www.fz-juelich.de/pgi/pgi-1/DE/Home/home_node.html)
-
-## Compatibility matrix
-
-| FLEUR Plugin | AiiDA CORE | Python | FLEUR |
-|-|-|-|-|
-| `v1.0.0 < v2.0.0` | <img class="svg-badge" title="Compatible with aiida-core >=1.3.0,<2.0.0" src="https://img.shields.io/badge/AiiDA->=1.3.0,<2.0.0-007ec6.svg?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAACMAAAAhCAYAAABTERJSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAFhgAABYYBG6Yz4AAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAUbSURBVFiFzZhrbFRVEMd%2Fc%2B5uu6UUbIFC%2FUAUVEQCLbQJBIiBDyiImJiIhmohYNCkqJAQxASLF8tDgYRHBLXRhIcKNtFEhVDgAxBJqgmVh4JEKg3EIn2QYqBlt917xg%2BFss%2ByaDHOtzsz5z%2B%2FuZl7ztmF%2F5HJvxVQN6cPYX8%2FPLnOmsvNAvqfwuib%2FbNIk9cQeQnLcKRL5xLIV%2Fic9eJeunjPYbRs4FjQSpTB3aS1IpRKeeOOewajy%2FKKEO8Q0DuVdKy8IqsbPulxGHUfCBBu%2BwUYGuFuBTK7wQnht6PEbf4tlRomVRjCbXNjQEB0AyrFQOL5ENIJm7dTLZE6DPJCnEtFZVXDLny%2B4Sjv0PmmYu1ZdUek9RiMgoDmJ8V0L7XJqsZ3UW8YsBOwEeHeeFce7jEYXBy0m9m4BbXqSj2%2Bxnkg26MCVrN6DEZcwggtd8pTFx%2Fh3B9B50YLaFOPwXQKUt0tBLegtSomfBlfY13PwijbEnhztGzgJsK5h9W9qeWwBqjvyhB2iBs1Qz0AU974DciRGO8CVN8AJhAeMAdA3KbrKEtvxhsI%2B9emWiJlGBEU680Cfk%2BSsVqXZvcFYGXjF8ABVJ%2BTNfVXehyms1zzn1gmIOxLEB6E31%2FWBe5rnCarmo7elf7dJEeaLh80GasliI5F6Q9cAz1GY1OJVNDxTzQTw7iY%2FHEZRQY7xqJ9RU2LFe%2FYqakdP911ha0XhjjiTVAkDwgatWfCGeYocx8M3glG8g8EXhSrLrHnEFJ5Ymow%2FkhIYv6ttYUW1iFmEqqxdVoUs9FmsDYSqmtmJh3Cl1%2BVtl2s7owDUdocR5bceiyoSivGTT5vzpbzL1uoBpmcAAQgW7ArnKD9ng9rc%2BNgrobSNwpSkkhcRN%2BvmXLjIsDovYHHEfmsYFygPAnIDEQrQPzJYCOaLHLUfIt7Oq0LJn9fxkSgNCb1qEIQ5UKgT%2Fs6gJmVOOroJhQBXVqw118QtWLdyUxEP45sUpSzqP7RDdFYMyB9UReMiF1MzPwoUqHt8hjGFFeP5wZAbZ%2F0%2BcAtAAcji6LeSq%2FMYiAvSsdw3GtrfVSVFUBbIhwRWYR7yOcr%2FBi%2FB1MSJZ16JlgH1AGM3EO2QnmMyrSbTSiACgFBv4yCUapZkt9qwWVL7aeOyHvArJjm8%2Fz9BhdI4XcZgz2%2FvRALosjsk1ODOyMcJn9%2FYI6IrkS5vxMGdUwou2YKfyVqJpn5t9aNs3gbQMbdbkxnGdsr4bTHm2AxWo9yNZK4PXR3uzhAh%2BM0AZejnCrGdy0UvJxl0oMKgWSLR%2B1LH2aE9ViejiFs%2BXn6bTjng3MlIhJ1I1TkuLdg6OcAbD7Xx%2Bc3y9TrWAiSHqVkbZ2v9ilCo6s4AjwZCzFyD9mOL305nV9aonvsQeT2L0gVk4OwOJqXXVRW7naaxswDKVdlYLyMXAnntteYmws2xcVVZzq%2BtHPAooQggmJkc6TLSusOiL4RKgwzzYU1iFQgiUBA1H7E8yPau%2BZl9P7AblVNebtHqTgxLfRqrNvZWjsHZFuqMqKcDWdlFjF7UGvX8Jn24DyEAykJwNcdg0OvJ4p5pQ9tV6SMlP4A0PNh8aYze1ArROyUNTNouy8tNF3Rt0CSXb6bRFl4%2FIfQzNMjaE9WwpYOWQnOdEF%2BTdJNO0iFh7%2BI0kfORzQZb6P2kymS9oTxzBiM9rUqLWr1WE5G6ODhycQd%2FUnNVeMbcH68hYkGycNoUNWc8fxaxfwhDbHpfwM5oeTY7rUX8QAAAABJRU5ErkJggg%3D%3D"> |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-fleur.svg)](https://pypi.org/project/aiida-fleur.svg) | MaXR1 < MaXR5 (v0.29)|
-| `< v0.6.3` | <img class="svg-badge" title="Compatible with aiida-core >=0.12,<1.0.0" src="https://img.shields.io/badge/AiiDA->=0.12,<1.0.0-007ec6.svg?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAACMAAAAhCAYAAABTERJSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAFhgAABYYBG6Yz4AAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAAUbSURBVFiFzZhrbFRVEMd%2Fc%2B5uu6UUbIFC%2FUAUVEQCLbQJBIiBDyiImJiIhmohYNCkqJAQxASLF8tDgYRHBLXRhIcKNtFEhVDgAxBJqgmVh4JEKg3EIn2QYqBlt917xg%2BFss%2ByaDHOtzsz5z%2B%2FuZl7ztmF%2F5HJvxVQN6cPYX8%2FPLnOmsvNAvqfwuib%2FbNIk9cQeQnLcKRL5xLIV%2Fic9eJeunjPYbRs4FjQSpTB3aS1IpRKeeOOewajy%2FKKEO8Q0DuVdKy8IqsbPulxGHUfCBBu%2BwUYGuFuBTK7wQnht6PEbf4tlRomVRjCbXNjQEB0AyrFQOL5ENIJm7dTLZE6DPJCnEtFZVXDLny%2B4Sjv0PmmYu1ZdUek9RiMgoDmJ8V0L7XJqsZ3UW8YsBOwEeHeeFce7jEYXBy0m9m4BbXqSj2%2Bxnkg26MCVrN6DEZcwggtd8pTFx%2Fh3B9B50YLaFOPwXQKUt0tBLegtSomfBlfY13PwijbEnhztGzgJsK5h9W9qeWwBqjvyhB2iBs1Qz0AU974DciRGO8CVN8AJhAeMAdA3KbrKEtvxhsI%2B9emWiJlGBEU680Cfk%2BSsVqXZvcFYGXjF8ABVJ%2BTNfVXehyms1zzn1gmIOxLEB6E31%2FWBe5rnCarmo7elf7dJEeaLh80GasliI5F6Q9cAz1GY1OJVNDxTzQTw7iY%2FHEZRQY7xqJ9RU2LFe%2FYqakdP911ha0XhjjiTVAkDwgatWfCGeYocx8M3glG8g8EXhSrLrHnEFJ5Ymow%2FkhIYv6ttYUW1iFmEqqxdVoUs9FmsDYSqmtmJh3Cl1%2BVtl2s7owDUdocR5bceiyoSivGTT5vzpbzL1uoBpmcAAQgW7ArnKD9ng9rc%2BNgrobSNwpSkkhcRN%2BvmXLjIsDovYHHEfmsYFygPAnIDEQrQPzJYCOaLHLUfIt7Oq0LJn9fxkSgNCb1qEIQ5UKgT%2Fs6gJmVOOroJhQBXVqw118QtWLdyUxEP45sUpSzqP7RDdFYMyB9UReMiF1MzPwoUqHt8hjGFFeP5wZAbZ%2F0%2BcAtAAcji6LeSq%2FMYiAvSsdw3GtrfVSVFUBbIhwRWYR7yOcr%2FBi%2FB1MSJZ16JlgH1AGM3EO2QnmMyrSbTSiACgFBv4yCUapZkt9qwWVL7aeOyHvArJjm8%2Fz9BhdI4XcZgz2%2FvRALosjsk1ODOyMcJn9%2FYI6IrkS5vxMGdUwou2YKfyVqJpn5t9aNs3gbQMbdbkxnGdsr4bTHm2AxWo9yNZK4PXR3uzhAh%2BM0AZejnCrGdy0UvJxl0oMKgWSLR%2B1LH2aE9ViejiFs%2BXn6bTjng3MlIhJ1I1TkuLdg6OcAbD7Xx%2Bc3y9TrWAiSHqVkbZ2v9ilCo6s4AjwZCzFyD9mOL305nV9aonvsQeT2L0gVk4OwOJqXXVRW7naaxswDKVdlYLyMXAnntteYmws2xcVVZzq%2BtHPAooQggmJkc6TLSusOiL4RKgwzzYU1iFQgiUBA1H7E8yPau%2BZl9P7AblVNebtHqTgxLfRqrNvZWjsHZFuqMqKcDWdlFjF7UGvX8Jn24DyEAykJwNcdg0OvJ4p5pQ9tV6SMlP4A0PNh8aYze1ArROyUNTNouy8tNF3Rt0CSXb6bRFl4%2FIfQzNMjaE9WwpYOWQnOdEF%2BTdJNO0iFh7%2BI0kfORzQZb6P2kymS9oTxzBiM9rUqLWr1WE5G6ODhycQd%2FUnNVeMbcH68hYkGycNoUNWc8fxaxfwhDbHpfwM5oeTY7rUX8QAAAABJRU5ErkJggg%3D%3D"> |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-fleur/0.6.svg)](https://pypi.python.org/pypi/aiida-fleur/0.6.3/) | MaXR1 < MaXR3 (v0.28)|
-
-### Documentation and User Support
-
-Hosted at http://aiida-fleur.readthedocs.io/en/develop/index.html.
-For other information see the AiiDA-core docs or http://www.flapw.de.
-
-Users can post any questions in the Fleur user [forum](http://fleur.xobor.de/)
-
-For bugs, feature requests and further issues please use the issue tracker on github of the aiida-fleur repository.
-
-### License:
-
-MIT license.
-See the license file.
-
-### How to cite:
-If you use this package please consider citing:
-```
-J. Broeder, D. Wortmann, and S. Blügel,
-Using the AiiDA-FLEUR package for all-electron ab initio electronic structure
-data generation and processing in materials science,
-In Extreme Data Workshop 2018 Proceedings, 2019, vol 40, p 43-48
+print(wf_parameters['inpxml_changes']) #now contains the list like before
 ```
 
 
-### Comments/Disclaimer:
-
-The plug-in and the workflows will only work with a Fleur version using xml files as I/O, i.e >v0.27.
-
-
-### Contents
-
-1. [Introduction](#Introduction)
-2. [Installation Instructions](#Installation)
-3. [Code Dependencies](#Dependencies)
-4. [Further Information](#FurtherInfo)
-
-## Introduction <a name="Introduction"></a>
-
-This is a python package (AiiDA plugin, workflows and utility)
-allowing to use the FLEUR-code in the AiiDA Framework.
-The FLEUR-code is an all-electron DFT code using the FLAPW method,
-that is widely applied in the material science and physics community.
-
-### The plugin :
-
-The Fleur plugin consists of:
-
-    1. A data-structure representing input files and called FleurinpData.
-    2. inpgen calculation
-    3. FLEUR calculation
-    4. Workchains
-    5. utility
-
-### Workchains in this package:
-
-workflow entry point name | Description
---------------|------------
-fleur.scf | SCF-cycle of Fleur. Converge the charge density and the Total energy with multiple FLEUR runs
-fleur.eos | Calculate and Equation of States with FLEUR (currently cubic systems only)
-fleur.dos | Calculate a Density of States (DOS) with FLEUR
-fleur.band | Calculate a Band structure with FLEUR
-fleur.relax | Relaxation of the atomic positions of a crystal structure with FLEUR
-fleur.init_cls | Calculate initial corelevel shifts and formation energies with FLEUR
-fleur.corehole | Workflow for corehole calculations, calculation of Binding energies with FLEUR
-fleur.dmi | Calculates Dzyaloshinskii–Moriya Interaction energy dispersion of a spin spiral
-fleur.ssdisp | Calculates exchange interaction energy dispersion of a spin spiral
-fleur.mae | Calculates Magnetic Anisotropy Energy
-
-See the AiiDA documentation for general info about the AiiDA workflow system or how to write workflows.
-
-
-### Utility/tools:
-
-filename | Description
----------|------------
-Structure_util.py | Constains some methods to handle AiiDA structures (some of them might now be methods of the AiiDA structureData, if so use them from there!)
-merge_parameter.py | Methods to handle parameterData nodes, i.e merge them. Which is very useful for all-electron codes, because instead of pseudo potentialsfamilies you can create now families of parameter nodes for the periodic table.
-read_cif.py | This can be used as stand-alone to create StructureData nodes from .cif files from an directory tree.
-
-Utility and tools, which are independend of AiiDA are moved to the [masci-tools](https://github.com/JuDFTteam/masci-tools) (material science tools) repository,
-which is a dependency of aiida-fleur.
-
-
-### Command line interface (CLI)
-
-Besides the python API, aiida-fleur comes with a builtin CLI: `aiida-fleur`. 
-This interface is built using the click library and supports tab-completion. 
-
-To enable tab-completion, add the following to your shell loading script, e.g. the .bashrc or virtual environment activate script:
-
-    eval "$(_AIIDA_FLEUR_COMPLETE=source aiida-fleur)"
-
-the main subcommands include:
-
-    data: Commands to create and inspect data nodes
-        fleurinp   Commands to handle `FleurinpData` nodes.
-        parameter  Commands to create and inspect `Dict` nodes containing FLAPW parameters
-        structure  Commands to create and inspect `StructureData` nodes.
-    launch: Commands to launch workflows and calcjobs of aiida-fleur
-
-        banddos          Launch a banddos workchain
-        corehole         Launch a corehole workchain
-        create_magnetic  Launch a create_magnetic workchain
-        dmi              Launch a dmi workchain
-        eos              Launch a eos workchain
-        fleur            Launch a base_fleur workchain.
-        init_cls         Launch an init_cls workchain
-        inpgen           Launch an inpgen calcjob on given input If no    code is...
-        mae              Launch a mae workchain
-        relax            Launch a base relax workchain # TODO final scf    input
-        scf              Launch a scf workchain
-        ssdisp           Launch a ssdisp workchain
-    
-    plot: Invoke the plot_fleur command on given nodes
-    
-    workflow: Commands to inspect aiida-fleur workchains and prepare inputs
-
-for example to launch an scf workchain on a given structure execute:
-    
-    $ aiida-fleur launch scf -i <inpgenpk> -f <fleurpk> -S <structurepk>
-
-the command can also process structures in any format `ase` can handle, this includes `Cif`, `xsf` and `poscar` files. In such a case simply parse the path to the file:
-
-    $ aiida-fleur launch scf -i <inpgenpk> -f <fleurpk> -S ./structure/Cu.cif
-
-## Installation Instructions <a name="Installation"></a>
-
-From the aiida-fleur folder (after downloading the code, recommended) use:
-
-    $ pip install .
-    # or which is very useful to keep track of the changes (developers)
-    $ pip install -e .
-
-To uninstall use:
-
-    $ pip uninstall aiida-fleur
-
-Or install latest release version from pypi:
-
-    $ pip install aiida-fleur
-
-### Test Installation
-To test rather the installation was successful use:
-```bash
-$ verdi plugins list aiida.calculations
-```
-```bash
-   # example output:
-
-   ## Pass as a further parameter one (or more) plugin names
-   ## to get more details on a given plugin.
-   ...
-   * fleur.fleur
-   * fleur.inpgen
-```
-You should see 'fleur.*' in the list
-
-The other entry points can be checked with the AiiDA Factories (Data, Workflow, Calculation, Parser).
-(this is done in test_entry_points.py)
-
-We suggest to run all the (unit)tests in the aiida-fleur/aiida_fleur/tests/ folder.
-
-    $ bash run_all_cov.sh
-
-___
-
-## Code Dependencies <a name="Dependencies"></a>
-
-Requirements are listed in 'setup_requirements.txt' and setup.json.
-
-most important are:
-
-* aiida_core >= 1.0.1
-* lxml
-* ase
-* masci-tools
-
-Mainly AiiDA:
-
-1. Download from [www.aiida.net -> Download](www.aiida.net)
-2. install and setup -> [aiida's documentation](http://aiida-core.readthedocs.org/en/stable)
-
-Easy plotting and other useful routines that do not depend on aiida_core are part of
-the [masci-tools](https://github.com/JuDFTteam/masci-tools) (material science tools) repository.
-
-For easy plotting we recommend using 'plot_methods' from masci-tools, which are also deployed by the 'plot_fleur(<node(s)>)' function.
-
-## Further Information <a name="FurtherInfo"></a>
-
-The plug-in source code documentation is [here](http://aiida-fleur.readthedocs.io/en/develop/index.html).
-also some documentation of the plug-in, further things can be found at www.flapw.de.
-Usage examples are shown in 'examples'.
-
-
-## Acknowledgements
 
-Besides the Forschungszentrum Juelich, this work is supported by the European MaX Centre of Excellence 'Materials design at the Exascale' [MaX](<http://www.max-centre.eu/>) funded by the Horizon 2020 EINFRA-5 program, Grant No. 676598 and under grant agreement No. 824143. This work is further supported by the Joint Lab Virtual Materials Design (JLVMD) of the Forschungszentrum Jülich.
+## v.1.3.1
+### release compatible with AiiDA-core 1.3.0+
+- Fix for masci-tools dependency constraint. The constraint would previously reject the next minor version of masci-tools (i.e `0.10.0`)
+- Small fixes in zenodo metadata
+- Added `convert_inpxml` method to `FleurinpData` to convert to different file versions
+
+## v.1.3.0
+### release compatible with AiiDA-core 1.3.0+
+- Guraranteed support for Fleur versions up to Max6
+- Dropped support for python 3.6
+- Added CFCoeff Workchain for calculating 4f crystal field coefficients
+- General Improvements of Forcetheorem workchains, allow switching kpoints for force theorem calculations
+- General Improvements of Orbcontrol workchain, allow starting from structure/charge density without SCF workchain
+- Added support for inpgen profiles
+- Refactored BaseFleurWorkChain; switched implementation of BaseRestartWorkChain from aiida-fleur to implementation provided by aiida-core
+- Added support for starting SCF Workchain with first calculation using straight mixing either for the charge density or the DTF+U density matrix
+
+## v.1.2.1
+### release compatible with AiiDA-core 1.3.0+
+- General improvements for CreateMagnetic workchain and related methods
+- Added OrbControl workchain
+- FleurBandDosWorkchain provides AiiDA BandsData for bandstructure calculations and XyData for DOS calculations as outputs
+- General Improvements to plot_fleur function, e.g. can now visualize FleurBandDosWorkChain
+
+## v.1.2.0
+### release compatible with AiiDA-core 1.3.0+
+possibly ready for aiida-core 2.0.0
+- supports Fleur MaXR4 and MaXR5 versions with new inpgen
+MaXR4 requires providing versions in the code nodes
+- Some features relying on the id in the inpgen files,
+may be broken by the new inpgen interface change when using MaXR5.1
+- Added support for GW calculations with Spex, and the Strain workchain
+- Major code refactoring, moving all xml tools to masci-tools (therefore requires masci-tools >=0.4.8)
+- Also all file parsers are overworked and moved to masci-tools
+- Work over of the BanddosWorkChain.
+- FleurinpData now consistently supports more included xml files (kpts.xml, sym.xml, ...)
+- Added new modification functions to the FleurinpModifier for kpoint manipulation for Max5
+
+
+## v.1.1.4
+### release compatible with AiiDA-core 1.3.0
+- still support of Fleur MaXR4 version with inpgen
+- Does not support yet Fleur MaXR5 and new inpgen
+- Fixed numpy dependency issue with aiida-common-workflows and quantum mobile
+
+## v1.1.3
+### release compatible with AiiDA-core 1.3.0
+- still support of Fleur MaXR4 version with inpgen
+- Does not support yet for Fleur MaXR5 and new inpgen
+- Set_kpoints was moved from fleurinp to fleurinpmodifier
+- Break_symmetry of a structure was refactored
+- Implemented feature in fleurinputCalculation to set significant figures
+- Implemented feature scf can now use default queues specified in code extras
+- First implementation of relax type None, which cases the relax workchain to skip the
+relaxation, becoming a usual scf wc,  which might make it easier to switch relaxation on
+and off in other workchains.
+- Fleur parser parses now the total magnetic moment of the cell
+- Introduced common constants, for bohr and htr, increased precision
+- Command line interface (CLI) `aiida-fleur` with various functionalities exposed
+- For devs: Increased test coverage, codecov is now added to CI and linked to badge
+removed some older outdated code
+
+## v1.1.2
+### release compatible with AiiDA-core 1.3.0
+- still support of Fleur MaX4 version (release branch) with inpgen
+- downdgraded aiida-core dependency, do release does not depend on aiida-testing
+- Added userfriendly LDA+U support
+- SCF workchain can generate kpoints from a given density
+- Base fleur has now time limit error handler
+- Relax workchain can now run a final scf
+- Update documentation for corehole, initial CLS and create magnetic workchains
+- Various bug fixes and robustness improvements of magnetic workchains
+- For devs: Enforced pre-commit, tests dir moved out of source
+
+## v1.1.1
+### release compatible with AiiDA-core 1.4.0
+- still support of Fleur MaX4 version (release branch) with inpgen
+- bugfixes and other general improvements
+- new: BandDos workchain: workchain for Band and DOS calculation using the new Fleur BandDOS file
+- basic workchains are now cachable, by moving cf out of workchains
+- first calcjob and workchain regression tests for outside CI env
+- provenance of the result nodes of magnetic workchains is fixed
+- corehole and initial_cls workchain are fixed and working
+- exit codes for inpgen parser
+
+## v1.1.0
+### release compatible with AiiDA-core 1.1.0
+- support of Fleur Max4 version (release branch)
+- make use of namespaces for nested workchains
+- inputs for the workchains are checked more strictly
+- exit codes are organised and consistent
+- FleurRestart workchain: automatic parallelisation is able to make OMP threading
+- new: BaseRelax workchain wrapping RelaxWorkChain and fixes its failures
+- new: CreateMagnetic workchain that creates relaxed film structure
+- increased unit test coverage for tools and utilities
+- code clean-ups, pylint score increased to 7.49
+
+## v1.0.0a
+### release compatible with AiiDA-core 1.0.0b5
+- added magnetic workchains
+- added geometry optimisation (relax) workchain
+- implemented the use of exit codes
+- added FLEUR restart workchain
+- integrated new Fleur input schema files
+- other improvements of the workchains and calculations
+- code clean-ups, documentation updates
+
+## v0.6.0
+### release for MaX virtual machine, not so well testet, but used in production mode. some things are currently half done
+- added CI
+- added basic tests, coverage still bad, but tests if plugin is installed right
+- added MANIFEST
+- fixed fleur_schema isssued if installed as python package (with manifest)
+- integrated the new Fleur schema files
+- bunch of new utiltity
+- advancements of workflows
+- correction of AiiDA graphs of most workchains, Quick and dirt, still unclear what is the right way to do these things, aiida_core still changes
+- increased pylint score from 0 to >5
+
+## v0.5.0
+### Merge with advanced workflow repo
+- this included the corehole and inital corehole workflow as well calculation of formation energies
+  Therefore this is the first public released verison of them with in MaX
+- all the utility of the corelevel repo is now under aiida_fleur/tools
+
+
+## v0.4.0
+- further improvment of scf, eos and other workchains
+- a workchain delta form calculation a delta value, or performing calculation on the delta structures or a group of structures in a single shot
+- lots of new utilty methods for structure dealings, fleur parameters and so on
+- lots of bugfixes
+- new system for the schema files, user does not has to add aiida-fleur to pythonpath or hack the schema paths.
+- added new tests, submission tests and standard fleur tests
+- first documention online, still very rusty still some issues there (stay with local one)
+
+## v0.3.0
+
+### Merge with workflows repo
+- the second repository with basic workflows was merged into the plugin repostitory.
+- Afterwards the repo was renamed from aiida_fleur_plugin to aiida-fleur
+
+### Installation (new aiida plugin system):
+- everything is now pip installable (pip install -e .) (not yet on pypi)
+Therefore the files do not have to be copied anymore into the aiida_core source folder
+(make sure to add the aiida-fleur folder to your PYTHONPATH variable)
+- all modules are now importet from the aiida_fleur folder
+ (example 'from aiida.tools.codespecific.fleur.convergence import fleur_convergence' -> 'from aiida_fleur.workflows.scf import fleur_scf_wc)
+
+### Renaming
+- In the process (and due to the entry points some things have to be renamed)
+  The plugin in aiida (fleur_inp.fleur -> fleur.fleur; fleur_inp.fleurinp -> fleur.fleurinp; fleur_inp.fleurinputgen -> fleur.inpgen)
+
+### Workflows
+- some fine tuning of workflows. Naming scheme was introduced.
+- Some first error catching and controlled shutdown (because of new AiiDA features).
+- added consistent through all workflows the 'serial' key in wf_parameter nodes, which will turn of mpi.
+- scf now uses minDistance and passes the walltime to fleur by default.
+
+### Dokumentation
+- Due to the new plugin system of AiiDA the Dokumentation is now online on read-the-docs.
+(so far incomplete because of old AiiDA version on pypi) We still recommend to take a look at the docs in the repo itself (ggf build it)
+
+### Utils
+- read fleur cif folder does not break the proverance any more
+
+
+### Further stuff
+- 0.28 Fleur schema added to aiida-fleur
+
+
+
+## v0.2.0 tutorial version
+
+Version for used at the MAX AiiDA-fleur tutorial in May 2017
+
+### Dokumentation
+- added some basic explainations pages beyond the pure in code docs
+
+
+### Tests
+- added basic tests of Fleur itself and tests for submission
+
+### Ploting
+- There is a plot_methods repo on bitbucket which has methods to visualize common workflow output nodes.
+
+### Workflows
+- first basic working workflows available
+- some common workflow stuff is now in common_fleur_wf.py
+
+### Fleurmodifier
+- Introduction of the Fleurinpmodifier class, to change fleurinp data
+
+### Fleurinp data
+- restructureing of fleurinp data and Fleurinpmodifier, moved most xml methods into xml_util
+- plus added further xml routines and rough tests.
+
+
+## v0.1 Base commit
+
+### Moved everything von bitbucket to github
 
-For this work essential is AiiDA, which itself is supported by the [MARVEL National Centre for Competency in Research](<http://nccr-marvel.ch>) funded by the [Swiss National Science Foundation](<http://www.snf.ch/en>).
+### Dokumentation
+-Basic docs available locally
 
+### Installation
+- provided copy_files script to copy the plugin files into AiiDA folder
 
-<img src="docs/source/images/MAX-orizz.png" alt="MaX" width="200"/>
-<img src="docs/source/images/Logo-JLVMD.png" alt="JLVMD" width="200"/>
+### Workflows
+- Some basic sketches of basic workflows available (working AiiDa workflow system just released)i
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,10 +5,9 @@
 #                                                                             #
 # The code is hosted on GitHub at https://github.com/JuDFTteam/aiida-fleur    #
 # For further information on the license, see the LICENSE.txt file            #
 # For further information please visit http://www.flapw.de or                 #
 # http://aiida-fleur.readthedocs.io/en/develop/                               #
 ###############################################################################
 '''
-AiiDA-FLEUR
+AiiDA-FLEUR workflows
 '''
-__version__ = '1.3.1'
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/calculation/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/calculation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/calculation/fleur.py` & `aiida-fleur-2.0.0/aiida_fleur/calculation/fleur.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from aiida.engine import CalcJob
 from aiida.orm import Dict
 from aiida.orm import RemoteData
 from aiida.common.datastructures import CalcInfo, CodeInfo
 from aiida.common.utils import classproperty
 from aiida.common.exceptions import InputValidationError
-from aiida.common.exceptions import UniquenessError
 from aiida_fleur.data.fleurinp import FleurinpData
 from aiida_fleur.calculation.fleurinputgen import FleurinputgenCalculation
 
 
 class FleurCalculation(CalcJob):
     """
     A CalcJob class that represents FLEUR DFT calculation.
@@ -181,35 +180,37 @@
     _copy_scf_ldau_noinp_nohdf = [[_CDN1_FILE_NAME, _CDN1_FILE_NAME], [_NMMPMAT_FILE_NAME, _NMMPMAT_FILE_NAME]]
 
     # files need for rerun
     _copy_filelist_dos = [_INPXML_FILE_NAME, _CDN1_FILE_NAME]
 
     _copy_filelist_band = [_INPXML_FILE_NAME, _POT_FILE_NAME, _CDN1_FILE_NAME]
 
+    _copy_filelist_spex = ['basis.hdf', 'pot.hdf', 'ecore']
+
     _copy_filelist_hybrid = []
     _copy_filelist_jij = []
 
     # possible settings_dict keys
     _settings_keys = [
         'additional_retrieve_list', 'remove_from_retrieve_list', 'additional_remotecopy_list',
-        'remove_from_remotecopy_list', 'cmdline'
+        'remove_from_remotecopy_list', 'cmdline', 'fleurinp_nmmpmat_priority'
     ]
 
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
-        # spec.input('metadata.options.input_filename', valid_type=six.string_types,
+        # spec.input('metadata.options.input_filename', valid_type=str,
         #            default=cls._INPXML_FILE_NAME)
         spec.input('metadata.options.output_filename', valid_type=str, default=cls._OUTXML_FILE_NAME)
         spec.input('metadata.options.use_kpoints', valid_type=bool, default=cls._use_kpoints)
         spec.input('metadata.options.parser_name', valid_type=str, default='fleur.fleurparser')
 
         # inputs
-        spec.input('fleurinpdata',
+        spec.input('fleurinp',
                    valid_type=FleurinpData,
                    required=False,
                    help='Use a FleurinpData node that specifies the input parameters'
                    'usually copy from the parent calculation, basically makes'
                    'the inp.xml file visible in the db and makes sure it has '
                    'the files needed.')
         spec.input('parent_folder',
@@ -296,32 +297,28 @@
                 with_hdf5 = True
             elif 'Hdf5' in codesdesc:
                 with_hdf5 = True
             elif 'HDF5' in codesdesc:
                 with_hdf5 = True
             else:
                 with_hdf5 = False
-        # a Fleur calc can be created from a fleurinpData alone
+        # a Fleur calc can be created from a FleurinpData alone
         # (then no parent is needed) all files are in the repo, but usually it is
         # a child of a inpgen calc or an other fleur calc (some or all files are
         # in a remote source). if the User has not changed something, the
         # calculation does not need theoretical a new FleurinpData it could use
         # the one from the parent, but the plug-in desgin is in a way that it has
         # to be there and it just copies files if changes occurred..
 
-        if 'fleurinpdata' in self.inputs:
-            fleurinp = self.inputs.fleurinpdata
+        has_fleurinp = 'fleurinp' in self.inputs
+        if has_fleurinp:
+            fleurinp = self.inputs.fleurinp
         else:
             fleurinp = None
 
-        if fleurinp is None:
-            has_fleurinp = False
-        else:
-            has_fleurinp = True
-
         if 'parent_folder' in self.inputs:
             parent_calc_folder = self.inputs.parent_folder
         else:
             parent_calc_folder = None
 
         if parent_calc_folder is None:
             has_parent = False
@@ -398,15 +395,20 @@
                     mode_retrieved_filelist.append(self._CFDATA_HDF5_FILE_NAME)
                 else:
                     self.logger.warning('CF calculation without HDF5 not supported for automatic file retrieval.')
             if modes['force_theorem'] or modes['cf_coeff']:
                 cdn_file = self._CDN_LAST_HDF5_FILE_NAME if with_hdf5 else self._CDN1_FILE_NAME
                 settings_dict.setdefault('remove_from_retrieve_list', []).append(cdn_file)
 
-            # if noco, ldau, gw...
+            #This construct is to avoid problems with masci-tools versions where the mode is still called gw
+            if modes.get('spex', modes.get('gw', False)):
+                mode_retrieved_filelist.extend(self._copy_filelist_spex)
+                settings_dict.setdefault('additional_remotecopy_list', []).extend(self._copy_filelist_spex)
+
+            # if noco, ldau, spex...
             # TODO: check from where it was copied, and copy files of its parent
             # if needed
 
         if has_parent:
             # copy necessary files
             # TODO: check first if file exist and throw a warning if not
             outfolder_uuid = parent_calc.outputs.retrieved.uuid
@@ -414,18 +416,24 @@
 
             outfolder_filenames = parent_calc.outputs.retrieved.list_object_names()
             has_nmmpmat_file = self._NMMPMAT_FILE_NAME in outfolder_filenames
             if (self._NMMPMAT_FILE_NAME in outfolder_filenames or \
                 self._NMMPMAT_HDF5_FILE_NAME in outfolder_filenames):
                 if has_fleurinp:
                     if self._NMMPMAT_FILE_NAME in fleurinp.files:
-                        self.logger.warning('Ignoring {filename} from fleurinp. '
-                                            'There is already an {filename} file '
-                                            'for the parent calculation'.format(filename=self._NMMPMAT_FILE_NAME))
-                        local_copy_list.remove((fleurinp.uuid, self._NMMPMAT_FILE_NAME, self._NMMPMAT_FILE_NAME))
+                        if settings_dict.get('fleurinp_nmmpmat_priority', False):
+                            self.logger.warning('Ignoring {filename} from remote. '
+                                                'There is already an {filename} file '
+                                                'for the fleurinp node'.format(filename=self._NMMPMAT_FILE_NAME))
+                            has_nmmpmat_file = False
+                        else:
+                            self.logger.warning('Ignoring {filename} from fleurinp. '
+                                                'There is already an {filename} file '
+                                                'for the parent calculation'.format(filename=self._NMMPMAT_FILE_NAME))
+                            local_copy_list.remove((fleurinp.uuid, self._NMMPMAT_FILE_NAME, self._NMMPMAT_FILE_NAME))
 
             if fleurinpgen and (not has_fleurinp):
                 for file1 in self._copy_filelist_inpgen:
                     if file1 not in outfolder_filenames:
                         raise InputValidationError(
                             f'File {file1} not found in parent folder but needed to start calculation')
                     local_copy_list.append((outfolder_uuid, file1, file1))
@@ -435,40 +443,34 @@
                     copylist = self._copy_scf_hdf
                 elif has_nmmpmat_file:
                     copylist = self._copy_scf_ldau_nohdf
                 else:
                     copylist = self._copy_scf
                 for file_orig, file_dest in copylist:
                     if file_orig not in outfolder_filenames:
+                        message = f'File {file_orig} not found in parent folder but needed to start calculation.\n'
                         if file_orig in (self._CDN1_FILE_NAME, self._CDN_LAST_HDF5_FILE_NAME):
-                            raise InputValidationError(
-                                f'File {file_orig} not found in parent folder but needed to start calculation'
-                                'Make sure that the given Fleur code is correctly labelled with/without HDF5')
-                        else:
-                            raise InputValidationError(
-                                f'File {file_orig} not found in parent folder but needed to start calculation')
+                            message += 'Make sure that the given Fleur code is correctly labelled with/without HDF5'
+                        raise InputValidationError(message)
                     local_copy_list.append((outfolder_uuid, file_orig, file_dest))
-                # TODO: get inp.xml from parent fleurinpdata; otherwise it will be doubled in rep
+                # TODO: get inp.xml from parent FleurinpData; otherwise it will be doubled in rep
             elif not fleurinpgen and has_fleurinp:
                 # inp.xml will be copied from fleurinp
                 if with_hdf5:
                     copylist = self._copy_scf_noinp_hdf
                 elif has_nmmpmat_file:
                     copylist = self._copy_scf_ldau_noinp_nohdf
                 else:
                     copylist = self._copy_scf_noinp
                 for file_orig, file_dest in copylist:
                     if file_orig not in outfolder_filenames:
+                        message = f'File {file_orig} not found in parent folder but needed to start calculation.\n'
                         if file_orig in (self._CDN1_FILE_NAME, self._CDN_LAST_HDF5_FILE_NAME):
-                            raise InputValidationError(
-                                f'File {file_orig} not found in parent folder but needed to start calculation'
-                                'Make sure that the given Fleur code is correctly labelled with/without HDF5')
-                        else:
-                            raise InputValidationError(
-                                f'File {file_orig} not found in parent folder but needed to start calculation')
+                            message += 'Make sure that the given Fleur code is correctly labelled with/without HDF5'
+                        raise InputValidationError(message)
                     local_copy_list.append((outfolder_uuid, file_orig, file_dest))
 
             # TODO: not on same computer -> copy needed files from repository
             # if they are not there throw an error
             if copy_remotely:  # on same computer.
                 filelist_tocopy_remote = filelist_tocopy_remote + self._copy_filelist_scf_remote
                 # from settings, user specified
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/calculation/fleurinputgen.py` & `aiida-fleur-2.0.0/aiida_fleur/calculation/fleurinputgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,15 @@
                    'the retrieve list, or add command line switches, '
                    'for all available features here check the documentation.')
 
         # parser
         spec.input('metadata.options.parser_name', valid_type=str, default='fleur.fleurinpgenparser')
 
         # declaration of outputs of the calclation
-        #TODO: Should this be renamed? FleurinpData inputs/outputs are called fleurinp everywhere
-        #else
-        spec.output('fleurinpData', valid_type=FleurinpData, required=True)
+        spec.output('fleurinp', valid_type=FleurinpData, required=True)
 
         # exit codes
         # spec.exit_code(251, 'ERROR_WRONG_INPUT_PARAMS',
         #                message='Input parameters for inpgen contain unknown keys.')
         # spec.exit_code(253, 'ERROR_ATOM_POSITION_NEEDED',
         #                message='Fleur lattice needs atom positions as input.')
         # spec.exit_code(254, 'ERROR_INPUT_PARAMS_LEFTOVER',
@@ -240,26 +238,26 @@
     Converts every entry in a dictionary to lowercase
 
     :param dic: parameters dictionary
     :param dict_name: dictionary name
     """
     from collections import Counter
 
-    if isinstance(dic, dict):
-        new_dict = {str(k).lower(): val for k, val in dic.items()}
-        if len(new_dict) != len(dic):
-            num_items = Counter(str(k).lower() for k in dic.keys())
-            double_keys = ','.join([k for k, val in num_items if val > 1])
-            raise InputValidationError("Inside the dictionary '{}' there are the following keys that "
-                                       'are repeated more than once when compared case-insensitively:'
-                                       '{}.This is not allowed.'.format(dict_name, double_keys))
-        return new_dict
-    else:
+    if not isinstance(dic, dict):
         raise TypeError('_lowercase_dict accepts only dictionaries as argument')
 
+    new_dict = {str(k).lower(): val for k, val in dic.items()}
+    if len(new_dict) != len(dic):
+        num_items = Counter(str(k).lower() for k in dic.keys())
+        double_keys = ','.join([k for k, val in num_items if val > 1])
+        raise InputValidationError("Inside the dictionary '{}' there are the following keys that "
+                                   'are repeated more than once when compared case-insensitively:'
+                                   '{}.This is not allowed.'.format(dict_name, double_keys))
+    return new_dict
+
 
 def write_inpgen_file_aiida_struct(structure, file, input_params=None, settings=None):
     """Wraps around masci_tools write inpgen_file, unpacks aiida structure"""
     from masci_tools.io.fleur_inpgen import write_inpgen_file
 
     atoms_dict_list = []
     kind_list = []
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/data/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/data/fleurinp.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/data/fleurinp.py`

 * *Files 22% similar despite different names*

```diff
@@ -123,14 +123,86 @@
     """
     Dumb the content of a file contained in given fleurinpdata, per default dump
     inp.xml
     """
     echo.echo(node.get_content(filename=filename))
 
 
+@cmd_fleurinp.command('open')
+@arguments.NODE('node', type=DataParamType(sub_classes=('aiida.data:fleur.fleurinp',)))
+@click.option('-f',
+              '--filename',
+              'filename',
+              default='inp.xml',
+              show_default=True,
+              help='Open the file of the given filename.')
+@click.option('-s', '--save', is_flag=True, help='Write out the changed content')
+@click.option('-o', '--output-filename', default='', show_default=True, help='Filename of the outpu.t')
+def open_inp(node, filename, save, output_filename):
+    """
+    opens the inp.xml in some editor, readonly.
+    inp.xml this way looking at xml might be more convenient.
+    """
+    if not save:
+        echo.echo_info('Any changes you make in the editor will not be stored in the node')
+    if not output_filename:
+        output_filename = filename
+    content = click.edit(node.get_content(filename=filename), extension='.xml')
+
+    if save:
+        with open(output_filename, 'w', encoding='utf-8') as file:
+            file.write(content)
+        echo.echo_success(f'Saved edited content to {output_filename}')
+
+
+@cmd_fleurinp.command('extract-inpgen')
+@arguments.NODE('node', type=DataParamType(sub_classes=('aiida.data:fleur.fleurinp',)))
+@click.option('-o',
+              '--output-filename',
+              'output_filename',
+              default='',
+              show_default=True,
+              help='Name of the file to write out.')
+@click.option('--para/--no-para', default=True, show_default=True, help='Add additional LAPW parameters to output file')
+def extract_inpgen_file(node, output_filename, para):
+    """
+    Write out a inpgen input file, that most closely
+    reproduces the input file in the node when run through the
+    inpgen
+    """
+    from aiida_fleur.calculation.fleurinputgen import write_inpgen_file_aiida_struct
+    from aiida import orm
+    import tempfile
+    from pathlib import Path
+
+    structure = node.get_structuredata()
+    lapw_parameters = {}
+    if para:
+        lapw_parameters = node.get_parameterdata(write_ids=orm.Bool(False)).get_dict()
+
+    if 'inpgen' not in lapw_parameters.get('title'):
+        echo.echo_info("Added 'inpgen file' to file title")
+        if 'title' in lapw_parameters:
+            lapw_parameters['title'] = f"{lapw_parameters['title']} (inpgen file)"
+        else:
+            lapw_parameters['title'] = 'File for the inpgen executable'
+
+    if output_filename:
+        with open(output_filename, 'w', encoding='utf-8') as file:
+            write_inpgen_file_aiida_struct(structure, file, input_params=lapw_parameters)
+        echo.echo_success(f'Inpgen file written to: {output_filename}')
+    else:
+        with tempfile.TemporaryDirectory() as td:
+            write_inpgen_file_aiida_struct(structure, Path(td) / 'aiida.in', input_params=lapw_parameters)
+
+            with open(Path(td) / 'aiida.in', encoding='utf-8') as file:
+                echo.echo(file.read())
+        echo.echo_success('Inpgen file extracted')
+
+
 '''
 @cmd_fleurinp.command('info')
 def info():
     """
     Shows some basic information about the fleurinp datastructure and dumbs the
     inp.xml
     """
@@ -141,23 +213,14 @@
 def cmd_show():
     """
     Shows the content of a certain file
     """
     click.echo('Not implemented yet, sorry. Please implement me!')
 
 
-@cmd_fleurinp.command('open')
-def open_inp():
-    """
-    opens the inp.xml in some editor, readonly.
-    inp.xml this way looking at xml might be more convenient.
-    """
-    click.echo('Not implemented yet, sorry. Please implement me!')
-
-
 # this is a maybe
 @cmd_fleurinp.command()
 def get_structure():
     """
     Prints some basic information about the structure data and return a structure uuid/pk
     """
     click.echo('Not implemented yet, sorry. Please implement me!')
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/data/parameters.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/data/parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/data/structure.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/data/structure.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/launch/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/launch/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/launch/launch.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/launch/launch.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Module with CLI commands to launch for calcjob and workflows of aiida-fleur.
 '''
 # TODO: these launch commands should be put in separate files, if this one becomes to large..
 
 import click
 from ..util import options, utils, defaults
 from aiida_fleur.tools.dict_util import clean_nones
-from aiida.orm import Code, load_node, Dict
+from aiida.orm import Dict
 from aiida.plugins import WorkflowFactory
 from aiida.plugins import CalculationFactory
 
 
 @click.command('inpgen')
 @options.STRUCTURE_OR_FILE(default=defaults.get_si_bulk_structure, show_default=True)
 @options.INPGEN()
@@ -112,41 +112,40 @@
     if option_node:
         opt_dict = option_node.get_dict()
         for key, val in opt_dict.items():
             options_d[key] = val
 
     inputs = {
         'code': fleur,
-        'fleurinpdata': fleurinp,
+        'fleurinp': fleurinp,
         'parent_folder': parent_folder,
         'settings': settings,
         'metadata': {
             'options': options_d
         }
     }
 
     if not launch_base:
         inputs = clean_nones(inputs)
         builder = process_class.get_builder()
         builder.update(inputs)
     else:
         if option_node is None:
-            option_node = Dict(
-                dict={
-                    'withmpi': with_mpi,
-                    'max_wallclock_seconds': max_wallclock_seconds,
-                    'resources': {
-                        'num_machines': max_num_machines,
-                        'num_mpiprocs_per_machine': num_mpiprocs_per_machine
-                    }
-                })
+            option_node = Dict({
+                'withmpi': with_mpi,
+                'max_wallclock_seconds': max_wallclock_seconds,
+                'resources': {
+                    'num_machines': max_num_machines,
+                    'num_mpiprocs_per_machine': num_mpiprocs_per_machine
+                }
+            })
 
         inputs_base = {
             'code': fleur,
-            'fleurinpdata': fleurinp,
+            'fleurinp': fleurinp,
             'parent_folder': parent_folder,
             'settings': settings,
             'options': option_node
         }
         inputs_base = clean_nones(inputs_base)
         builder = workchain_class.get_builder()
         builder.update(**inputs_base)
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/list/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/list/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/util/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/util/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/util/defaults.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/util/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,22 +56,22 @@
     created and stored. This function should be used as a default for CLI options that require a `StructureData` node.
     This way new users can launch the command without having to construct or import a structure first. This is the
     reason that we hardcode a FePt film to be returned. More flexibility is not required for this purpose.
 
     :return: the uuid of  `StructureData` representing a FePt film
     """
     from aiida.orm import StructureData, QueryBuilder
+    from masci_tools.util.constants import BOHR_A
 
-    bohr_a_0 = 0.52917721092  # A
-    a = 7.497 * bohr_a_0
+    a = 7.497 * BOHR_A
     cell = [[0.7071068 * a, 0.0, 0.0], [0.0, 1.0 * a, 0.0], [0.0, 0.0, 0.7071068 * a]]
     structure = StructureData(cell=cell)
-    structure.append_atom(position=(0.0, 0.0, -1.99285 * bohr_a_0), symbols='Fe', name='Fe123')
+    structure.append_atom(position=(0.0, 0.0, -1.99285 * BOHR_A), symbols='Fe', name='Fe123')
     structure.append_atom(position=(0.5 * 0.7071068 * a, 0.5 * a, 0.0), symbols='Pt')
-    structure.append_atom(position=(0., 0., 2.65059 * bohr_a_0), symbols='Pt')
+    structure.append_atom(position=(0., 0., 2.65059 * BOHR_A), symbols='Pt')
     structure.pbc = (True, True, False)
 
     builder = QueryBuilder().append(StructureData, filters={'extras._aiida_hash': structure._get_hash()})
     results = builder.first()
 
     if not results:
         structure.store()
@@ -112,11 +112,8 @@
 
     builder = QueryBuilder().append(Code, filters=filters)
     builder.order_by({Code: {'ctime': 'asc'}})
     results = builder.first()
 
     if not results:
         raise NotExistent(f'ERROR: Could not find any Code in the database with entry point: {entry_point_name}!')
-    else:
-        inpgen = results[0]
-
-    return inpgen.uuid
+    return results[0].uuid
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/util/options.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/util/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     '-s',
     '--structure',
     type=StructureNodeOrFileParamType(),
     help='StructureData node, given by pk or uuid or file in any for mat which will be converted.')
 
 STRUCTURE = OverridableOption('-s',
                               '--structure',
-                              type=types.DataParamType(sub_classes=('aiida.data:structure',)),
+                              type=types.DataParamType(sub_classes=('aiida.data:core.structure',)),
                               help='StructureData node, given by pk or uuid.')
 
 FULL_PROVENANCE = OverridableOption('-fp',
                                     '--full-provenance',
                                     is_flag=True,
                                     default=False,
                                     show_default=True,
@@ -57,45 +57,45 @@
                              '--fleurinp',
                              type=types.DataParamType(sub_classes=('aiida.data:fleur.fleurinp',)),
                              help='FleurinpData node for the fleur calculation.')
 
 CALC_PARAMETERS = OverridableOption(
     '-calc_p',
     '--calc-parameters',
-    type=types.DataParamType(sub_classes=('aiida.data:dict',)),
+    type=types.DataParamType(sub_classes=('aiida.data:core.dict',)),
     help='Dict with calculation (FLAPW) parameters to build, which will be given to inpgen.')
 
 SETTINGS = OverridableOption('-set',
                              '--settings',
-                             type=types.DataParamType(sub_classes=('aiida.data:dict',)),
+                             type=types.DataParamType(sub_classes=('aiida.data:core.dict',)),
                              help='Settings node for the calcjob.')
 
 WF_PARAMETERS = OverridableOption('-wf',
                                   '--wf-parameters',
-                                  type=types.DataParamType(sub_classes=('aiida.data:dict',)),
+                                  type=types.DataParamType(sub_classes=('aiida.data:core.dict',)),
                                   help='Dict containing parameters given to the workchain.')
 
 SCF_PARAMETERS = OverridableOption('-scf',
                                    '--scf-parameters',
-                                   type=types.DataParamType(sub_classes=('aiida.data:dict',)),
+                                   type=types.DataParamType(sub_classes=('aiida.data:core.dict',)),
                                    help='Dict containing parameters given to the sub SCF workchains.')
 
 EOS_PARAMETERS = OverridableOption('-eos',
                                    '--eos-parameters',
-                                   type=types.DataParamType(sub_classes=('aiida.data:dict',)),
+                                   type=types.DataParamType(sub_classes=('aiida.data:core.dict',)),
                                    help='Dict containing wf parameters given to the sub EOS workchains.')
 
 RELAX_PARAMETERS = OverridableOption('-relax',
                                      '--relax-parameters',
-                                     type=types.DataParamType(sub_classes=('aiida.data:dict',)),
+                                     type=types.DataParamType(sub_classes=('aiida.data:core.dict',)),
                                      help='Dict containing wf parameters given to the sub relax workchains.')
 
 OPTION_NODE = OverridableOption('-opt',
                                 '--option-node',
-                                type=types.DataParamType(sub_classes=('aiida.data:dict',)),
+                                type=types.DataParamType(sub_classes=('aiida.data:core.dict',)),
                                 help='Dict, an option node for the workchain.')
 
 MAX_NUM_MACHINES = OverridableOption('-N',
                                      '--max-num-machines',
                                      type=click.INT,
                                      default=1,
                                      show_default=True,
@@ -128,15 +128,15 @@
                              default=False,
                              show_default=True,
                              help='Run the calculations with MPI enabled.')
 
 REMOTE = OverridableOption('-P',
                            '--parent-folder',
                            'parent_folder',
-                           type=types.DataParamType(sub_classes=('aiida.data:remote',)),
+                           type=types.DataParamType(sub_classes=('aiida.data:core.remote',)),
                            show_default=True,
                            required=False,
                            help='The PK of a parent remote folder (for restarts).')
 
 DAEMON = OverridableOption('-d',
                            '--daemon',
                            is_flag=True,
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/util/types.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/util/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def convert(self, value, param, ctx):
         is_path = False
         # Alternative one could check if int or uuid
         # aiida allows also for shorten uuids
         from aiida.orm import StructureData, QueryBuilder
 
         try:
-            structure = types.DataParamType(sub_classes=('aiida.data:structure',)).convert(value, param, ctx)
+            structure = types.DataParamType(sub_classes=('aiida.data:core.structure',)).convert(value, param, ctx)
         except (NotExistent, click.exceptions.BadParameter) as er:
             echo.echo(f'Tried to load node, could not fine one for {value}. '
                       'I will further check if it is a filepath.')
             is_path = True
 
         if is_path:
             # If it is a path to a file try to convert the structure
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/util/utils.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/util/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/visualization/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/cmdline/workflows/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/cmdline/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/common/defaults.py` & `aiida-fleur-2.0.0/aiida_fleur/common/defaults.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/common/node_generators.py` & `aiida-fleur-2.0.0/aiida_fleur/common/node_generators.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/data/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/data/fleurinp.py` & `aiida-fleur-2.0.0/aiida_fleur/data/fleurinp.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,69 +14,121 @@
 """
 # TODO: maybe add a modify method which returns a fleurinpmodifier class
 # TODO: inpxml to dict: maybe kpts should not be written to the dict? same with symmetry
 # TODO: test for large input files, I believe the recursion is still quite slow..
 # TODO: 2D cell get kpoints and get structure also be carefull with tria = T!!!
 # TODO : maybe save when get_structure or get_kpoints was executed on fleurinp,
 # because otherwise return this node instead of creating a new one!
+from __future__ import annotations
 import os
 import io
 import re
-
-from lxml import etree
 import warnings
+import pathlib
 
 from aiida import orm
-from aiida.orm import Data, Node, load_node, CalcJobNode, Bool
+from aiida.engine import calcfunction as cf
 from aiida.common.exceptions import InputValidationError, ValidationError
-from aiida.engine.processes.functions import calcfunction as cf
 
+from typing import Any, cast, Iterator, BinaryIO, TextIO, ContextManager, Dict, List
+
+from lxml import etree
+from masci_tools.io.parsers.fleur_schema import InputSchemaDict
+
+__all__ = ('FleurinpData', 'get_fleurinp_from_folder_data', 'get_fleurinp_from_remote_data', 'get_structuredata',
+           'get_kpointsdata', 'get_parameterdata', 'convert_inpxml', 'get_fleurinp_from_folder_data_cf',
+           'get_fleurinp_from_remote_data_cf')
+
+
+@cf
+def get_fleurinp_from_folder_data_cf(folder_node: orm.FolderData,
+                                     additional_files: orm.List | None = None) -> FleurinpData:
+    """
+    Create FleurinpData object from the given FolderData object
+
+    :param remote_node: FolderData to use for the generation of the FleurinpData
+
+    :returns: FleurinpData object with the input xml files from the FolderData
+    """
+
+    if additional_files is None:
+        additional_files = orm.List(list=[])
+
+    return get_fleurinp_from_folder_data(folder_node, additional_files=additional_files.get_list())
+
+
+@cf
+def get_fleurinp_from_remote_data_cf(remote_node: orm.RemoteData,
+                                     additional_files: orm.List | None = None) -> FleurinpData:
+    """
+    Create FleurinpData object from the given RemoteData object
+
+    :param remote_node: RemoteData to use for the generation of the FleurinpData
+    :param store: bool, if True the FleurinpData object will be stored after generation
+
+    :returns: FleurinpData object with the input xml files from the retrieved folder
+              of the calculation associated RemoteData
+    """
+
+    if additional_files is None:
+        additional_files = orm.List(list=[])
 
-def get_fleurinp_from_folder_data(folder_node, store=False, additional_files=None):
+    return get_fleurinp_from_remote_data(remote_node, additional_files=additional_files.get_list())
+
+
+def get_fleurinp_from_folder_data(folder_node: orm.FolderData,
+                                  store: bool = False,
+                                  additional_files: list[str] | None = None) -> FleurinpData:
     """
     Create FleurinpData object from the given RemoteData object
 
     :param remote_node: RemoteData to use for the generation of the FleurinpData
     :param store: bool, if True the FleurinpData object will be stored after generation
 
     :returns: FleurinpData object with the input xml files from the retrieved folder
               of the calculation associated RemoteData
     """
     if additional_files is None:
         additional_files = []
+    if isinstance(additional_files, orm.List):
+        additional_files = additional_files.get_list()
 
     input_xml_files = [file for file in folder_node.list_object_names() if file.endswith('.xml') and 'out' not in file]
 
     fleurinp = FleurinpData(files=input_xml_files + additional_files, node=folder_node)
     if store:
         fleurinp.store()
 
     return fleurinp
 
 
-def get_fleurinp_from_remote_data(remote_node, store=False, additional_files=None):
+def get_fleurinp_from_remote_data(remote_node: orm.RemoteData,
+                                  store: bool = False,
+                                  additional_files: list[str] | None = None) -> FleurinpData:
     """
     Create FleurinpData object from the given RemoteData object
 
     :param remote_node: RemoteData to use for the generation of the FleurinpData
     :param store: bool, if True the FleurinpData object will be stored after generation
 
     :returns: FleurinpData object with the input xml files from the retrieved folder
               of the calculation associated RemoteData
     """
 
-    for link in remote_node.get_incoming().all():
-        if isinstance(link.node, CalcJobNode):
+    for link in remote_node.base.links.get_incoming().all():
+        if isinstance(link.node, orm.CalcJobNode):
             parent_calc_node = link.node
-    retrieved = parent_calc_node.get_outgoing().get_node_by_label('retrieved')
+    retrieved = parent_calc_node.base.links.get_outgoing().get_node_by_label('retrieved')
 
-    return get_fleurinp_from_folder_data(retrieved, store=store, additional_files=additional_files)
+    return get_fleurinp_from_folder_data(cast(orm.FolderData, retrieved),
+                                         store=store,
+                                         additional_files=additional_files)
 
 
-class FleurinpData(Data):
+class FleurinpData(orm.Data):
     """
     AiiDA data object representing everything a FLEUR calculation needs.
 
     It is initialized with an absolute path to an ``inp.xml`` file or a
     FolderData node containing ``inp.xml``.
     Other files can also be added that will be copied to the remote machine, where the
     calculation takes place.
@@ -94,131 +146,127 @@
 
     Remember that most attributes of AiiDA nodes can not be changed after they
     have been stored in the database! Therefore, you have to use the FleurinpModifier class and its
     methods if you want to change somthing in the ``inp.xml`` file. You will retrieve a new
     FleurinpData that way and start a new calculation from it.
     """
 
-    __version__ = '0.6.0'
+    __version__ = '0.6.1'
 
-    def __init__(self, **kwargs):
+    def __init__(self, files: list[str] | None = None, node: orm.Node | str | int | None = None, **kwargs: Any) -> None:
         """
         Initialize a FleurinpData object set the files given
         """
-        files = kwargs.pop('files', None)
+        super().__init__(**kwargs)
+        if files is None:
+            files = []
+
         for filename in files:
             if 'inp.xml' in filename:
                 files.pop(files.index(filename))
                 files.append(filename)
                 break
-        node = kwargs.pop('node', None)
-        super().__init__(**kwargs)
 
         if files:
-            if node:
-                self.set_files(files, node=node)
-            else:
-                self.set_files(files)
+            self.set_files(files, node=node)
 
     @property
-    def parser_info(self):
+    def parser_info(self) -> dict[str, Any]:
         """
         Dict property, with the info and warnings from the inpxml_parser
         """
-        return self.get_extra('_parser_info', {})
+        return self.base.extras.get('_parser_info', {})
 
     @parser_info.setter
-    def parser_info(self, info_dict):
+    def parser_info(self, info_dict: dict[str, Any]) -> None:
         """
         Setter for has_schema
         """
-        self.set_extra('_parser_info', info_dict)
+        self.base.extras.set('_parser_info', info_dict)
 
     # files
     @property
-    def files(self):
+    def files(self) -> list[str]:
         """
         Returns the list of the names of the files stored
         """
-        return self.get_attribute('files', [])
+        return self.base.attributes.get('files', [])
 
     @files.setter
-    def files(self, filelist, node=None):
+    def files(self, filelist: list[str]) -> None:
         """
         Add a list of files to FleurinpData.
         Alternative use setter method.
 
         :param files: list of filepaths or filenames of node is specified
-        :param node: a Folder node containing files from the filelist
         """
-        for file1 in filelist:
-            self.set_file(file1, node=node)
+        self.set_files(filelist)
 
-    def set_files(self, files, node=None):
+    def set_files(self, files: list[str], node: orm.Node | str | int | None = None) -> None:
         """
         Add the list of files to the :class:`~aiida_fleur.data.fleurinp.FleurinpData` instance.
         Can by used as an alternative to the setter.
 
         :param files: list of abolute filepaths or filenames of node is specified
         :param node: a :class:`~aiida.orm.FolderData` node containing files from the filelist
         """
-        for file1 in files:
-            self.set_file(file1, node=node)
+        for filename in files:
+            self.set_file(filename, node=node)
 
-    def set_file(self, filename, dst_filename=None, node=None):
+    def set_file(self,
+                 filename: str,
+                 dst_filename: str | None = None,
+                 node: orm.Node | str | int | None = None) -> None:
         """
         Add a file to the :class:`~aiida_fleur.data.fleurinp.FleurinpData` instance.
 
         :param filename: absolute path to the file or a filename of node is specified
         :param node: a :class:`~aiida.orm.FolderData` node containing the file
         """
         self._add_path(filename, dst_filename=dst_filename, node=node)
 
-    def open(self, path='inp.xml', mode='r', key=None):  #pylint: disable=arguments-differ
+    def open(self, path: str = 'inp.xml', mode: str = 'r') -> ContextManager[BinaryIO | TextIO]:
         """
         Returns an open file handle to the content of this data node.
 
         :param key: name of the file to be opened
         :param mode: the mode with which to open the file handle
         :returns: A file handle in read mode
-         """
-
-        if key is not None:
-            path = key
-
-        return super().open(path, mode=mode)
+        """
+        return self.base.repository.open(path, mode=mode)
 
-    def get_content(self, filename='inp.xml'):
+    def get_content(self, filename: str = 'inp.xml') -> str:
         """
         Returns the content of the single file stored for this data node.
 
         :returns: A string of the file content
         """
         with self.open(path=filename, mode='r') as handle:
-            return handle.read()
+            return handle.read()  #type: ignore[return-value]
 
-    def del_file(self, filename):
+    def del_file(self, filename: str) -> None:
         """
         Remove a file from FleurinpData instancefind
 
         :param filename: name of the file to be removed from FleurinpData instance
         """
         # remove from files attr list
-        if filename in self.get_attribute('files'):
-            try:
-                self.get_attribute('files').remove(filename)
-                # self._del_attribute(‘filename')
-            except AttributeError:
-                # There was no file set
-                pass
-        # remove from sandbox folder
-        if filename in self.list_object_names():  # get_folder_list():
+        filelist_attribute = self.base.attributes.get('files', [])
+        if filename in filelist_attribute:
+            filelist_attribute.remove(filename)
+            self.base.attributes.set('files', filelist_attribute)
             self.delete_object(filename)
+        else:
+            raise ValueError(f'Could not delete file {filename} from fleurinp node {self.pk}'
+                             'File does not exist on the node')
 
-    def _add_path(self, file1, dst_filename=None, node=None):
+    def _add_path(self,
+                  path_or_handle: str | pathlib.Path | BinaryIO,
+                  dst_filename: str | None = None,
+                  node: orm.Node | str | int | None = None) -> None:
         """
         Add a single file to the FleurinpData folder.
         The destination name can be different. ``inp.xml`` is a special case.
         file names are stored in the db, the whole file in the reporsitory.
 
         :param file1: the file to be added, either string, absolute path, or filelike object whose contents to copy
             Hint: Pass io.BytesIO(b"my string") to construct the file directly from a string.
@@ -228,138 +276,132 @@
         :raise: ValueError, InputValidationError
         :return: None
         """
         # TODO? Maybe only certain files should be allowed to be added
         # contra: has to be maintained, also these files can be inputed from byte strings...
         #_list_of_allowed_files = ['inp.xml', 'enpara', 'cdn1', 'sym.out', 'kpts']
 
-        if node:
-            if not isinstance(node, Node):
-                node = load_node(node)  # if this fails it will raise
-            if file1 not in node.list_object_names():
+        if node is not None:
+            if not isinstance(node, orm.Node):
+                node = orm.load_node(node)
+            if not isinstance(path_or_handle, str):
+                raise ValueError('When providing node the path has to be a string')
+
+            if path_or_handle not in node.list_object_names():
                 # throw error, you try to add something that is not there
-                raise ValueError('file1 has to be in the specified node')
+                raise ValueError(f'The file {path_or_handle} has to be present in the specified node {node.pk}')
 
             is_filelike = True
-            if dst_filename is None:
-                final_filename = file1
-            else:
-                final_filename = dst_filename
-            # Override file1 with bytestring of file
+            final_filename = path_or_handle
+
+            # Get bytestring of file
             # since we have to use 'with', and node has no method to copy files
             # we read the whole file and write it again later
             # this is not so nice, but we assume that input files are rather small...
-            with node.open(file1, mode='rb') as file2:
-                file1 = io.BytesIO(file2.read())
+            with node.base.repository.open(path_or_handle, mode='rb') as file:
+                path_or_handle = io.BytesIO(file.read())  #type: ignore[arg-type]
 
-        elif isinstance(file1, str):
+        elif isinstance(path_or_handle, (str, pathlib.Path)):
             is_filelike = False
+            path_or_handle = pathlib.Path(path_or_handle)
+
+            if not path_or_handle.is_absolute():
+                path_or_handle = path_or_handle.resolve()
 
-            if not os.path.isabs(file1):
-                file1 = os.path.abspath(file1)
-                #raise ValueError("Pass an absolute path for file1: {}".format(file1))
-
-            if not os.path.isfile(file1):
-                raise ValueError(f'file1 must exist and must be a single file: {file1}')
-
-            if dst_filename is None:
-                final_filename = os.path.split(file1)[1]
-            else:
-                final_filename = dst_filename
+            if not path_or_handle.is_file():
+                raise ValueError(f'Path {os.fspath(path_or_handle)} must exist and must be a single file')
+
+            final_filename = path_or_handle.name
         else:
             is_filelike = True
-            if dst_filename is None:
-                try:
-                    final_filename = os.path.basename(file1.name)  # Not sure if this still works for aiida>2.0
-                except AttributeError:
-                    final_filename = 'inp.xml'  # fall back to default
-            else:
-                final_filename = dst_filename
 
-        key = final_filename
+            try:
+                final_filename = os.path.basename(path_or_handle.name)
+            except AttributeError:
+                final_filename = 'UNKNOWN'
+
+        if dst_filename is not None:
+            final_filename = dst_filename
+
+        if final_filename == 'UNKNOWN':
+            raise ValueError('Provided an anonymous file handle without a filename')
 
-        old_file_list = self.list_object_names()
-        old_files_list = self.get_attribute('files', [])
+        old_files_list = self.base.attributes.get('files', [])
 
         # remove file from folder first if it exists
-        if final_filename not in old_file_list:
+        if final_filename not in old_files_list:
             old_files_list.append(final_filename)
-        else:
-            try:
-                old_file_list.remove(final_filename)
-            except ValueError:
-                pass
 
         if is_filelike:
-            try:
-                self.put_object_from_filelike(file1, key, mode='wb')
-            except TypeError:
-                self.put_object_from_filelike(file1, key)
+            self.put_object_from_filelike(path_or_handle, final_filename)
         else:
-            self.put_object_from_file(file1, key)
+            self.put_object_from_file(path_or_handle, final_filename)
 
-        self.set_attribute('files', old_files_list)  # We want to keep the other files
+        self.base.attributes.set('files', old_files_list)  # We want to keep the other files
 
         ### Special case: 'inp.xml' ###
         # here this is hardcoded, might want to change? get filename from elsewhere
 
         if final_filename == 'inp.xml':
             # get input file version number
             inp_version_number = None
             lines = self.get_content(filename=final_filename).split('\n')
             for line in lines:
                 if re.search('fleurInputVersion', str(line)):
                     inp_version_number = re.findall(r'\d+.\d+', str(line))[0]
                     break
             if inp_version_number is None:
                 raise InputValidationError('No fleurInputVersion number found '
-                                           'in given input file: {}. {}'
+                                           f'in given input file: {path_or_handle}. {lines}'
                                            'Please check if this is a valid fleur input file. '
-                                           'It can not be validated and I can not use it. '
-                                           ''.format(file1, lines))
+                                           'It can not be validated and I can not use it. ')
 
-            self.set_attribute('inp_version', inp_version_number)
+            self.base.attributes.set('inp_version', inp_version_number)
             # finally set inp dict of Fleurinpdata
             self._set_inp_dict()
 
-    def _set_inp_dict(self):
+    def _set_inp_dict(self) -> None:
         """
         Sets the inputxml_dict from the ``inp.xml`` file attached to FleurinpData
 
         1. load ``inp.xml`` file
         2. insert all files to include into the etree
         3. call masci-tools input file parser (Validation happens inside here)
         4. set inputxml_dict
         """
         from masci_tools.io.parsers.fleur import inpxml_parser
 
         #The schema_dict is not needed outside the inpxml_parser so we ignore it with the underscore
-        xmltree, _ = self.load_inpxml()
+        xmltree, _ = self.load_inpxml()  #type: ignore[misc]
 
-        parser_info = {}
+        parser_info: dict[str, Any] = {}
         try:
             inpxml_dict = inpxml_parser(xmltree, parser_info_out=parser_info)
         except (ValueError, FileNotFoundError) as exc:
             raise InputValidationError(f'inp.xml parser failed: {exc}') from exc
         finally:
             #Always try to provide the error/warning information
             self.parser_info = parser_info
 
         # set inpxml_dict attribute
-        self.set_attribute('inp_dict', inpxml_dict)
+        self.base.attributes.set('inp_dict', inpxml_dict)
 
-    def load_inpxml(self, validate_xml_schema=True, return_included_tags=False, **kwargs):
+    def load_inpxml(
+        self,
+        validate_xml_schema: bool = True,
+        return_included_tags: bool = False,
+        **kwargs: Any
+    ) -> tuple[etree._ElementTree, InputSchemaDict] | tuple[etree._ElementTree, InputSchemaDict, set[str]]:
         """
         Returns the lxml etree and the schema dictionary corresponding to the version. If validate_xml_schema=True
         the file will also be validated against the schema
 
         Keyword arguments are passed on to the parser
         """
-        from masci_tools.io.io_fleurxml import load_inpxml
-        from masci_tools.util.xml.common_functions import validate_xml
+        from masci_tools.io.fleur_xml import load_inpxml
 
         self._validate()
 
         with self.open(path='inp.xml', mode='rb') as inpxmlfile:
             try:
                 xmltree, schema_dict = load_inpxml(inpxmlfile, **kwargs)
             except ValueError as exc:
@@ -372,31 +414,28 @@
                 raise InputValidationError(err_msg) from exc
 
         xmltree, included_tags = self._include_files(xmltree)
         develop_version = self.inp_version != schema_dict['inp_version']
 
         if validate_xml_schema and not develop_version:
             try:
-                validate_xml(xmltree,
-                             schema_dict.xmlschema,
-                             error_header='Input file is not validated against the schema')
-            except etree.DocumentInvalid as err:
+                schema_dict.validate(xmltree)
+            except ValueError as err:
                 raise InputValidationError(err) from err
-        elif develop_version:
+        elif develop_version and self.logger is not None:
             self.logger.warning(f'You are using a Fleur input file with file version {self.inp_version}.\n'
                                 'This version has no corresponding XML Schema stored in masci-tools.\n'
                                 'Unexpected Errors can occur. If that is the case you can try to add the '
                                 'XML Schema for this file version to masci-tools')
 
         if return_included_tags:
             return xmltree, schema_dict, included_tags
-        else:
-            return xmltree, schema_dict
+        return xmltree, schema_dict
 
-    def _include_files(self, xmltree):
+    def _include_files(self, xmltree: etree._ElementTree) -> tuple[etree._ElementTree, set[str]]:
         """
         Tries to insert all .xml, which are not inp.xml file into the etree since they are
         not naturally available for the parser (open vs self.open)
 
         Creates a NamedTemporaryFile for each one with their content
         and replaces the name in the `href` attributes of the `xi:include` tags.
         Then these are expanded with `xmltree.xinclude()`
@@ -432,262 +471,234 @@
         for file in temp_files:
             os.remove(file)
 
         return cleared_tree, included_tags
 
     # dict with inp paramters parsed from inp.xml
     @property
-    def inp_dict(self):
+    def inp_dict(self) -> dict[str, Any]:
         """
         Returns the inp_dict (the representation of the ``inp.xml`` file) as it will
         or is stored in the database.
         """
-        return self.get_attribute('inp_dict', {})
+        return self.base.attributes.get('inp_dict', {})
 
     # version of the inp.xml file
     @property
-    def inp_version(self):
+    def inp_version(self) -> str | None:
         """
         Returns the version string corresponding to the inp.xml file
         """
-        return self.get_attribute('inp_version', None)
+        return self.base.attributes.get('inp_version', None)
 
-    def _validate(self):
+    def _validate(self) -> None:  #type: ignore[override]
         """
         A validation method. Checks if an ``inp.xml`` file is in the FleurinpData.
         """
         #from aiida.common.exceptions import ValidationError
         # check if schema file path exists.
         super()._validate()
 
-        if 'inp.xml' in self.files:
-            # has_inpxml = True # does nothing so far
-            pass
-        else:
+        if 'inp.xml' not in self.files:
             raise ValidationError('inp.xml file not in attribute "files". '
                                   'FleurinpData needs to have and inp.xml file!')
 
-    def get_fleur_modes(self):
+    def get_fleur_modes(self) -> dict[str, Any]:
         """
         Analyses ``inp.xml`` file to set up a calculation mode. 'Modes' are paths a FLEUR
         calculation can take, resulting in different output.
         This files can be automatically addded to the retrieve_list of the calculation.
 
         Common modes are: scf, jspin2, dos, band, pot8, lda+U, eels, ...
 
         :return: a dictionary containing all possible modes.
         """
         from masci_tools.util.xml.xml_getters import get_fleur_modes
 
-        xmltree, schema_dict = self.load_inpxml()
+        xmltree, schema_dict = self.load_inpxml()  #type: ignore[misc]
 
         return get_fleur_modes(xmltree, schema_dict)
 
-    def get_nkpts(self):
+    def get_nkpts(self) -> int:
         """
         This routine returns the number of kpoints used in the fleur calculation
         defined in this input
 
         :returns: int with the number of kPoints
         """
         from masci_tools.util.xml.xml_getters import get_nkpts
 
-        xmltree, schema_dict = self.load_inpxml()
+        xmltree, schema_dict = self.load_inpxml()  #type: ignore[misc]
 
         return get_nkpts(xmltree, schema_dict)
 
-    def get_structuredata_ncf(self, normalize_kind_name=True):
+    def get_structuredata_ncf(self, normalize_kind_name: bool = True) -> orm.StructureData:
         """
         This routine returns an AiiDA Structure Data type produced from the ``inp.xml``
         file. not a calcfunction
 
         :param self: a FleurinpData instance to be parsed into a StructureData
         :returns: StructureData node, or None
         """
-        from aiida.orm import StructureData
-        from masci_tools.util.xml.xml_getters import get_structure_data
+        from masci_tools.util.xml.xml_getters import get_structuredata as get_structuredata_xml
 
-        xmltree, schema_dict = self.load_inpxml()
+        xmltree, schema_dict = self.load_inpxml()  #type: ignore[misc]
 
-        atoms, cell, pbc = get_structure_data(xmltree,
-                                              schema_dict,
-                                              site_namedtuple=True,
-                                              normalize_kind_name=normalize_kind_name)
+        atoms, cell, pbc = get_structuredata_xml(xmltree, schema_dict, normalize_kind_name=normalize_kind_name)
 
-        struc = StructureData(cell=cell, pbc=pbc)
+        struc = orm.StructureData(cell=cell, pbc=pbc)
 
         for atom in atoms:
             struc.append_atom(position=atom.position, symbols=atom.symbol, name=atom.kind)
 
         # TODO DATA-DATA links are not wanted, you might want to use a cf instead
         #struc.add_link_from(self, label='self.structure', link_type=LinkType.CREATE)
         # label='self.structure'
         # return {label : struc}
         return struc
 
-    @cf
-    def get_structuredata(self, normalize_kind_name=None):
+    def get_structuredata(self, normalize_kind_name: orm.Bool | None = None) -> orm.StructureData:
         """
         This routine return an AiiDA Structure Data type produced from the ``inp.xml``
         file. If this was done before, it returns the existing structure data node.
         This is a calcfunction and therefore keeps the provenance.
 
         :param fleurinp: a FleurinpData instance to be parsed into a StructureData
         :returns: StructureData node
         """
-        if normalize_kind_name is None:
-            normalize_kind_name = Bool(True)
-        return self.get_structuredata_ncf(normalize_kind_name=normalize_kind_name)
+        return get_structuredata(self, normalize_kind_name=normalize_kind_name)
 
-    def get_kpointsdata_ncf(self, name=None, index=None, only_used=False):
+    def get_kpointsdata_ncf(self,
+                            name: str | None = None,
+                            index: int | None = None,
+                            only_used: bool = False) -> orm.KpointsData | dict[str, orm.KpointsData]:
         """
         This routine returns an AiiDA :class:`~aiida.orm.KpointsData` type produced from the
         ``inp.xml`` file. This only works if the kpoints are listed in the in inpxml.
         This is NOT a calcfunction and does not keep the provenance!
 
         :param name: str, optional, if given only the kpoint set with the given name
                      is returned
         :param index: int, optional, if given only the kpoint set with the given index
                       is returned
 
         :returns: :class:`~aiida.orm.KpointsData` node
         """
-        from aiida.orm import KpointsData
-        from masci_tools.util.xml.xml_getters import get_kpoints_data
+        from masci_tools.util.xml.xml_getters import get_kpointsdata as get_kpointsdata_xml
 
         # HINT, TODO:? in this routine, the 'cell' you might get in an other way
         # exp: StructureData.cell, but for this you have to make a structureData Node,
         # which might take more time for structures with lots of atoms.
         # then just parsing the cell from the inp.xml
         # as in the routine get_structureData
 
-        xmltree, schema_dict = self.load_inpxml()
+        xmltree, schema_dict = self.load_inpxml()  #type: ignore[misc]
 
         if name is None and index is None:
-            kpoints, weights, cell, pbc = get_kpoints_data(xmltree, schema_dict, only_used=only_used)
+            kpoints, weights, cell, pbc = get_kpointsdata_xml(xmltree, schema_dict, only_used=only_used)
         else:
-            kpoints, weights, cell, pbc = get_kpoints_data(xmltree,
-                                                           schema_dict,
-                                                           name=name,
-                                                           index=index,
-                                                           only_used=only_used)
+            kpoints, weights, cell, pbc = get_kpointsdata_xml(xmltree,
+                                                              schema_dict,
+                                                              name=name,
+                                                              index=index,
+                                                              only_used=only_used)
 
         if isinstance(kpoints, dict):
+            weights = cast(Dict[str, List[float]], weights)
             kpoints_data = {}
             for (label, kpoints_set), weights_set in zip(kpoints.items(), weights.values()):
-                kps = KpointsData()
+                kps = orm.KpointsData()
                 kps.set_cell(cell)
                 kps.pbc = pbc
                 kps.set_kpoints(kpoints_set, cartesian=False, weights=weights_set)
                 #kpoints_data.add_link_from(self, label='fleurinp.kpts', link_type=LinkType.CREATE)
                 pattern = re.compile(r'\W', re.UNICODE)
                 kpoint_identifier = re.sub(pattern, '', label.replace('-', '_'))
                 if kpoint_identifier != label.replace('-', '_'):
                     warnings.warn(
                         f'Normed the name of the kpoint set {label} to {kpoint_identifier}'
                         ' to be able to use it as a link label', UserWarning)
                 kps.label = f'fleurinp.kpts.{kpoint_identifier}'
                 kpoints_data[kpoint_identifier] = kps
-        else:
-            kpoints_data = KpointsData()
-            kpoints_data.set_cell(cell)
-            kpoints_data.pbc = pbc
-            kpoints_data.set_kpoints(kpoints, cartesian=False, weights=weights)
-            #kpoints_data.add_link_from(self, label='fleurinp.kpts', link_type=LinkType.CREATE)
-            kpoints_data.label = 'fleurinp.kpts'
+            return kpoints_data
 
-        return kpoints_data
-
-    @cf
-    def get_kpointsdata(self, name=None, index=None):
+        kps = orm.KpointsData()
+        kps.set_cell(cell)
+        kps.pbc = pbc
+        kps.set_kpoints(kpoints, cartesian=False, weights=weights)
+        #kps.add_link_from(self, label='fleurinp.kpts', link_type=LinkType.CREATE)
+        kps.label = 'fleurinp.kpts'
+        return kps
+
+    def get_kpointsdata(self,
+                        name: orm.Str | None = None,
+                        index: orm.Int | None = None,
+                        only_used: orm.Bool | None = None) -> orm.KpointsData | dict[str, orm.KpointsData]:
         """
         This routine returns an AiiDA :class:`~aiida.orm.KpointsData` type produced from the
         ``inp.xml`` file. This only works if the kpoints are listed in the in inpxml.
         This is a calcfunction and keeps the provenance!
 
         :returns: :class:`~aiida.orm.KpointsData` node
         """
-        return self.get_kpointsdata_ncf(name=name, index=index)
+        return get_kpointsdata(self, name=name, index=index, only_used=only_used)
 
-    def get_parameterdata_ncf(self, inpgen_ready=True, write_ids=True):
+    def get_parameterdata_ncf(self, inpgen_ready: bool = True, write_ids: bool = True) -> orm.Dict:
         """
         This routine returns an AiiDA :class:`~aiida.orm.Dict` type produced from the ``inp.xml``
         file. This node can be used for inpgen as `calc_parameters`.
         This is NOT a calcfunction and does NOT keep the provenance!
 
         :returns: :class:`~aiida.orm.Dict` node
         """
-        from aiida.orm import Dict
-        from masci_tools.util.xml.xml_getters import get_parameter_data
+        from masci_tools.util.xml.xml_getters import get_parameterdata as get_parameterdata_xml
 
-        xmltree, schema_dict = self.load_inpxml()
+        xmltree, schema_dict = self.load_inpxml()  #type: ignore[misc]
 
-        parameter_data = get_parameter_data(xmltree, schema_dict, inpgen_ready=inpgen_ready, write_ids=write_ids)
+        parameter_data = get_parameterdata_xml(xmltree, schema_dict, inpgen_ready=inpgen_ready, write_ids=write_ids)
 
-        return Dict(dict=parameter_data)
+        return orm.Dict(parameter_data)
 
-    @cf
-    def get_parameterdata(self):
+    def get_parameterdata(self, inpgen_ready: orm.Bool | None = None, write_ids: orm.Bool | None = None) -> orm.Dict:
         """
         This routine returns an AiiDA :class:`~aiida.orm.Dict` type produced from the ``inp.xml``
         file. The returned node can be used for inpgen as `calc_parameters`.
         This is a calcfunction and keeps the provenance!
 
         :returns: :class:`~aiida.orm.Dict` node
         """
+        return get_parameterdata(self, inpgen_ready=inpgen_ready, write_ids=write_ids)
 
-        return self.get_parameterdata_ncf()
-
-    def get_tag(self, xpath):
-        """
-        Tries to evaluate an xpath expression for ``inp.xml`` file. If it fails it logs it.
-
-        :param xpath: an xpath expression
-        :returns: A node list retrived using given xpath
-        """
-        from masci_tools.util.xml.common_functions import eval_xpath
-
-        warnings.warn(
-            'The get_tag method is deprecated. Instead you can use the load_inpxml method to access '
-            'the xmltree and schema of the stored inp.xml. Then the required information can be accessed '
-            'via the XML functions in masci-tools or directly', DeprecationWarning)
-
-        xmltree, _ = self.load_inpxml()
-        root = xmltree.getroot()
-
-        return eval_xpath(root, xpath)
-
-    @cf
-    def convert_inpxml(self, to_version: orm.Str) -> 'FleurinpData':
+    def convert_inpxml(self, to_version: orm.Str) -> FleurinpData:
         """
         Convert the fleurinp data node to a different inp.xml version
         and return a clone of the node
 
         .. note::
             If the Fleurinp contains included xml trees the resulting
             FleurinpData will contain only the combined inp.xml
         """
-        return self.convert_inpxml_ncf(to_version.value)
+        return convert_inpxml(self, to_version.value)
 
-    def convert_inpxml_ncf(self, to_version: str) -> 'FleurinpData':
+    def convert_inpxml_ncf(self, to_version: str) -> FleurinpData:
         """
         Convert the fleurinp data node to a different inp.xml version
         and return a clone of the node
 
         .. note::
             If the Fleurinp contains included xml trees the resulting
             FleurinpData will contain only the combined inp.xml
         """
-        from masci_tools.tools.fleur_inpxml_converter import convert_inpxml
+        from masci_tools.tools.fleur_inpxml_converter import convert_inpxml as convert_inpxml_actual
         import tempfile
         clone = self.clone()
 
         xmltree, schema_dict = clone.load_inpxml(remove_blank_text=True)
         try:
-            converted_tree = convert_inpxml(xmltree, schema_dict, to_version)
+            converted_tree = convert_inpxml_actual(xmltree, schema_dict, to_version)
         except FileNotFoundError as exc:
             raise ValueError(
                 f"No conversion available from version {schema_dict['inp_version']} to {to_version}\n"
                 'Please create the conversion by running\n'
                 f"     masci-tools generate-conversion {schema_dict['inp_version']}  {to_version}\n") from exc
 
         clone.del_file('inp.xml')
@@ -697,7 +708,72 @@
             clone.set_file(inpxml_path, 'inp.xml')
 
         # default label and description
         clone.label = 'fleurinp_converted'
         clone.description = f"Fleurinpdata converted from version {schema_dict['inp_version']} to {to_version}"
 
         return clone
+
+
+@cf
+def get_kpointsdata(fleurinp: FleurinpData,
+                    name: orm.Str | None = None,
+                    index: orm.Int | None = None,
+                    only_used: orm.Bool | None = None) -> orm.KpointsData | dict[str, orm.KpointsData]:
+    """
+    This routine returns an AiiDA :class:`~aiida.orm.KpointsData` type produced from the
+    ``inp.xml`` file. This only works if the kpoints are listed in the in inpxml.
+    This is a calcfunction and keeps the provenance!
+
+    :returns: :class:`~aiida.orm.KpointsData` node or dict of :class:`~aiida.orm.KpointsData`
+    """
+    if only_used is None:
+        only_used = orm.Bool(False)
+    return fleurinp.get_kpointsdata_ncf(name=name, index=index, only_used=only_used)  #type: ignore[arg-type]
+
+
+@cf
+def get_structuredata(fleurinp: FleurinpData, normalize_kind_name: orm.Bool | None = None) -> orm.StructureData:
+    """
+    This routine return an AiiDA Structure Data type produced from the ``inp.xml``
+    file. If this was done before, it returns the existing structure data node.
+    This is a calcfunction and therefore keeps the provenance.
+
+    :param fleurinp: a FleurinpData instance to be parsed into a StructureData
+    :returns: StructureData node
+    """
+    if normalize_kind_name is None:
+        normalize_kind_name = orm.Bool(True)
+    return fleurinp.get_structuredata_ncf(normalize_kind_name=normalize_kind_name.value)
+
+
+@cf
+def get_parameterdata(fleurinp: FleurinpData,
+                      inpgen_ready: orm.Bool | None = None,
+                      write_ids: orm.Bool | None = None) -> orm.Dict:
+    """
+    This routine returns an AiiDA :class:`~aiida.orm.Dict` type produced from the ``inp.xml``
+    file. The returned node can be used for inpgen as `calc_parameters`.
+    This is a calcfunction and keeps the provenance!
+
+    :returns: :class:`~aiida.orm.Dict` node
+    """
+    if inpgen_ready is None:
+        inpgen_ready = orm.Bool(True)
+
+    if write_ids is None:
+        write_ids = orm.Bool(True)
+
+    return fleurinp.get_parameterdata_ncf(inpgen_ready=inpgen_ready.value, write_ids=write_ids.value)
+
+
+@cf
+def convert_inpxml(fleurinp: FleurinpData, to_version: orm.Str) -> FleurinpData:
+    """
+    Convert the fleurinp data node to a different inp.xml version
+    and return a clone of the node
+
+    .. note::
+        If the Fleurinp contains included xml trees the resulting
+        FleurinpData will contain only the combined inp.xml
+    """
+    return fleurinp.convert_inpxml_ncf(to_version.value)
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/parsers/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/parsers/fleur.py` & `aiida-fleur-2.0.0/aiida_fleur/parsers/fleur.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 from aiida.parsers import Parser
 from aiida.orm import Dict
 from aiida.common.exceptions import NotExistent
 
 from masci_tools.io.parsers.fleur import outxml_parser
 from masci_tools.io.parsers.fleur_schema import InputSchemaDict
 
+#Phrases in this list are used to detect out of
+#memory errors
+OUT_OF_MEMORY_PHRASES = [
+    'cgroup out-of-memory handler',
+    'Out Of Memory',
+    'Allocation of array for communication failed'  #from io/eig66_mpi
+]
+
 
 class FleurParser(Parser):
     """
     This class is the implementation of the Parser class for FLEUR.
     It parses the FLEUR output if the calculation was successful,
     i.e checks if all files are there that should be and their condition.
     Then it parses the out.xml file and returns a (simple) parameterData node
@@ -164,50 +172,53 @@
                         time_avail_sec = self.node.attributes['last_job_info']['requested_wallclock_time_seconds']
                         time_calculated = self.node.attributes['last_job_info']['wallclock_time_seconds']
                         if 0.97 * time_avail_sec < time_calculated:
                             return self.exit_codes.ERROR_TIME_LIMIT
                     except KeyError:
                         pass
 
-                    if (kb_used * mpiprocs / mem_kb_avail > 0.93 or
-                            'cgroup out-of-memory handler' in error_file_lines or 'Out Of Memory' in error_file_lines):
+                    if kb_used * mpiprocs / mem_kb_avail > 0.93 or \
+                        any(phrase in error_file_lines for phrase in OUT_OF_MEMORY_PHRASES):
                         return self.exit_codes.ERROR_NOT_ENOUGH_MEMORY
-                    elif 'TIME LIMIT' in error_file_lines or 'time limit' in error_file_lines:
+                    if 'TIME LIMIT' in error_file_lines or 'time limit' in error_file_lines:
                         return self.exit_codes.ERROR_TIME_LIMIT
-                    elif 'Atom spills out into vacuum during relaxation' in error_file_lines:
+                    if 'Atom spills out into vacuum during relaxation' in error_file_lines:
                         return self.exit_codes.ERROR_VACUUM_SPILL_RELAX
-                    elif 'Error checking M.T. radii' in error_file_lines:
+                    if 'Error checking M.T. radii' in error_file_lines:
                         return self.exit_codes.ERROR_MT_RADII
-                    elif 'No solver linked for Hubbard 1' in error_file_lines:
+                    if 'No solver linked for Hubbard 1' in error_file_lines:
                         return self.exit_codes.ERROR_MISSING_DEPENDENCY.format(name='edsolver')
-                    elif 'Overlapping MT-spheres during relaxation: ' in error_file_lines:
+                    if 'FLEUR is not linked against libxc' in error_file_lines:
+                        return self.exit_codes.ERROR_MISSING_DEPENDENCY.format(name='libxc')
+                    if 'Overlapping MT-spheres during relaxation: ' in error_file_lines:
                         overlap_line = re.findall(r'\S+ +\S+ olap: +\S+', error_file_lines)[0].split()
                         with output_folder.open('relax.xml', 'r') as rlx:
                             schema_dict = InputSchemaDict.fromVersion('0.34')
                             relax_dict = parse_relax_file(rlx, schema_dict)
                             it_number = len(relax_dict['energies']) + 1  # relax.xml was not updated
                         error_params = {
                             'error_name': 'MT_OVERLAP_RELAX',
                             'description': ('This output node contains information'
                                             'about FLEUR error'),
                             'overlapped_indices': overlap_line[:2],
                             'overlaping_value': overlap_line[3],
                             'iteration_number': it_number
                         }
                         link_name = self.get_linkname_outparams()
-                        error_params = Dict(dict=error_params)
+                        error_params = Dict(error_params)
                         self.out('error_params', error_params)
                         return self.exit_codes.ERROR_MT_RADII_RELAX
-                    elif 'parent_folder' in calc.inputs:  # problem in reusing cdn for relaxations, drop cdn
-                        if 'fleurinpdata' in calc.inputs:
-                            if 'relax.xml' in calc.inputs.fleurinpdata.files:
+                    if 'parent_folder' in calc.inputs:  # problem in reusing cdn for relaxations, drop cdn
+                        if 'fleurinp' in calc.inputs:
+                            if 'relax.xml' in calc.inputs.fleurinp.files:
                                 return self.exit_codes.ERROR_DROP_CDN
                         return self.exit_codes.ERROR_FLEUR_CALC_FAILED
-                    else:
-                        return self.exit_codes.ERROR_FLEUR_CALC_FAILED
+
+                    #Catch all exit code for an unknown failure
+                    return self.exit_codes.ERROR_FLEUR_CALC_FAILED
 
         # if a relax.xml was retrieved
         if FleurCalculation._RELAX_FILE_NAME in list_of_files:
             self.logger.info('relax.xml file found in retrieved folder')
             has_relax_file = True
 
         ####### Parse the files ########
@@ -224,32 +235,33 @@
             except (ValueError, FileNotFoundError, KeyError) as exc:
                 self.logger.error(f'XML output parsing failed: {str(exc)}')
                 success = False
 
         # Call routines for output node creation
         if not success:
             self.logger.error('Parsing of XML output file was not successfull.')
-            outxml_params = Dict(dict=parser_info)
+            outxml_params = Dict(parser_info)
             link_name = self.get_linkname_outparams()
             self.out(link_name, outxml_params)
             return self.exit_codes.ERROR_XMLOUT_PARSING_FAILED
-        elif out_dict:
-            outxml_params = Dict(dict={**out_dict, **parser_info})
+
+        if out_dict:
+            outxml_params = Dict({**out_dict, **parser_info})
             link_name = self.get_linkname_outparams()
             self.out(link_name, outxml_params)
         else:
             self.logger.error('Something went wrong, no out_dict found')
-            outxml_params = Dict(dict=parser_info)
+            outxml_params = Dict(parser_info)
             link_name = self.get_linkname_outparams()
             self.out(link_name, outxml_params)
 
         if has_relax_file:
             relax_name = FleurCalculation._RELAX_FILE_NAME
             try:
-                fleurinp = calc.inputs.fleurinpdata
+                fleurinp = calc.inputs.fleurinp
             except NotExistent:
                 old_relax_text = ''
             else:
                 if relax_name in fleurinp.list_object_names():
                     with fleurinp.open(relax_name, 'r') as rlx:
                         old_relax_text = rlx.read()
                 else:
@@ -276,8 +288,8 @@
     from masci_tools.util.xml.xml_getters import get_relaxation_information
 
     relax_file.seek(0)
     tree = etree.parse(relax_file)
 
     out_dict = get_relaxation_information(tree, schema_dict)
 
-    return Dict(dict=out_dict)
+    return Dict(out_dict)
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/parsers/fleur_inputgen.py` & `aiida-fleur-2.0.0/aiida_fleur/parsers/fleur_inputgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,8 +125,8 @@
                 self.logger.error(f'Parser output: {pprint.pformat(fleurinp.parser_info)}')
             return self.exit_codes.ERROR_FLEURINPDATA_INPUT_NOT_VALID
         except ValidationError as ex:
             self.logger.error(f'FleurinpData validation failed: {str(ex)}')
             return self.exit_codes.ERROR_FLEURINPDATA_NOT_VALID
 
         self.logger.info('FleurinpData initialized')
-        self.out('fleurinpData', fleurinp)
+        self.out('fleurinp', fleurinp)
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/StructureData_util.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/StructureData_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,23 @@
 # For further information please visit http://www.flapw.de or                 #
 # http://aiida-fleur.readthedocs.io/en/develop/                               #
 ###############################################################################
 """
 Collection of utility routines dealing with StructureData objects
 """
 # TODO move imports to workfuncitons namespace?
+# TODO: MPrester has a new backwards incompatible version in pymatgen
+#       Migrate and solve pylint warning deactivated below
+#pylint: disable=not-context-manager
 
 # from ase import *
 # from ase.lattice.surface import *
 # from ase.io import *
 
+import warnings
 from pymatgen.core.surface import generate_all_slabs  #, get_symmetrically_distinct_miller_indices
 from pymatgen.core.surface import SlabGenerator
 
 import numpy as np
 
 from aiida.plugins import DataFactory
 from aiida.orm import load_node, Bool
@@ -32,26 +36,25 @@
     """
     Test if the given input is a StructureData node, by object, id, or pk
     :param structure: AiiDA StructureData
     :return: if yes returns a StructureData node in all cases, if no returns None
     """
     from aiida.common import NotExistent
 
-    StructureData = DataFactory('structure')
+    StructureData = DataFactory('core.structure')
 
     # Test if StructureData
     if isinstance(structure, StructureData):
         return structure
 
     try:
         structure = load_node(structure)
         if isinstance(structure, StructureData):
             return structure
-        else:
-            return None
+        return None
     except NotExistent:
         return None
 
 
 def is_primitive(structure):
     """
     Checks if a structure is primitive or not,
@@ -102,15 +105,15 @@
     if not structure:
         # TODO: log something
         return None
 
     the_ase = structure.get_ase()
     new_ase = the_ase.copy()
     new_ase.set_cell(the_ase.get_cell() * np.power(float(scale), 1.0 / 3), scale_atoms=True)
-    rescaled_structure = DataFactory('structure')(ase=new_ase)
+    rescaled_structure = DataFactory('core.structure')(ase=new_ase)
     rescaled_structure.label = f'{scale}  rescaled'  #, structure.uuid)
     #uuids in node labels are bad for caching
     rescaled_structure.pbc = structure.pbc
 
     return rescaled_structure
 
 
@@ -160,15 +163,15 @@
     na3 = int(n_a3)
 
     # new cell
     new_a1 = [i * na1 for i in old_a1]
     new_a2 = [i * na2 for i in old_a2]
     new_a3 = [i * na3 for i in old_a3]
     new_cell = [new_a1, new_a2, new_a3]
-    new_structure = DataFactory('structure')(cell=new_cell, pbc=old_pbc)
+    new_structure = DataFactory('core.structure')(cell=new_cell, pbc=old_pbc)
 
     # insert atoms
     # first create all kinds
     old_kinds = structure.kinds
     for kind in old_kinds:
         new_structure.append_kind(kind)
 
@@ -205,104 +208,14 @@
     new_structure.label = f'supercell of {formula}'
     new_structure.description = f'{n_a1}x{n_a2}x{n_a3} supercell of {formula}'
     return new_structure
 
 
 # Structure util
 # after ths is in plugin code import these in fleurinp.
-def abs_to_rel(vector, cell):
-    """
-    Converts a position vector in absolute coordinates to relative coordinates.
-
-    :param vector: list or np.array of length 3, vector to be converted
-    :param cell: Bravais matrix of a crystal 3x3 Array, List of list or np.array
-    :return: list of legth 3 of scaled vector, or False if vector was not length 3
-    """
-
-    if len(vector) == 3:
-        cell_np = np.array(cell)
-        inv_cell_np = np.linalg.inv(cell_np)
-        postionR = np.array(vector)
-        # np.matmul(inv_cell_np, postionR)#
-        new_rel_post = np.matmul(postionR, inv_cell_np)
-        new_rel_pos = list(new_rel_post)
-        return new_rel_pos
-    else:
-        return False
-
-
-def abs_to_rel_f(vector, cell, pbc):
-    """
-    Converts a position vector in absolute coordinates to relative coordinates
-    for a film system.
-
-    :param vector: list or np.array of length 3, vector to be converted
-    :param cell: Bravais matrix of a crystal 3x3 Array, List of list or np.array
-    :param pbc: Boundary conditions, List or Tuple of 3 Boolean
-    :return: list of legth 3 of scaled vector, or False if vector was not length 3
-    """
-    # TODO this currently only works if the z-coordinate is the one with no pbc
-    # Therefore if a structure with x non pbc is given this should also work.
-    # maybe write a 'tranform film to fleur_film routine'?
-    if len(vector) == 3:
-        if not pbc[2]:
-            # leave z coordinate absolute
-            # convert only x and y.
-            postionR = np.array(vector)
-            postionR_f = np.array(postionR[:2])
-            cell_np = np.array(cell)
-            cell_np = np.array(cell_np[0:2, 0:2])
-            inv_cell_np = np.linalg.inv(cell_np)
-            # np.matmul(inv_cell_np, postionR_f)]
-            new_xy = np.matmul(postionR_f, inv_cell_np)
-            new_rel_pos_f = [new_xy[0], new_xy[1], postionR[2]]
-            return new_rel_pos_f
-        else:
-            print('FLEUR can not handle this type of film coordinate')
-    else:
-        return False
-
-
-def rel_to_abs(vector, cell):
-    """
-    Converts a position vector in internal coordinates to absolute coordinates
-    in Angstrom.
-
-    :param vector: list or np.array of length 3, vector to be converted
-    :param cell: Bravais matrix of a crystal 3x3 Array, List of list or np.array
-    :return: list of legth 3 of scaled vector, or False if vector was not lenth 3
-    """
-    if len(vector) == 3:
-        cell_np = np.array(cell)
-        postionR = np.array(vector)
-        new_abs_post = np.matmul(postionR, cell_np)
-        new_abs_pos = list(new_abs_post)
-        return new_abs_pos
-    else:
-        return False
-
-
-def rel_to_abs_f(vector, cell):
-    """
-    Converts a position vector in internal coordinates to absolute coordinates
-    in Angstrom for a film structure (2D).
-    """
-    # TODO this currently only works if the z-coordinate is the one with no pbc
-    # Therefore if a structure with x non pbc is given this should also work.
-    # maybe write a 'tranform film to fleur_film routine'?
-    if len(vector) == 3:
-        postionR = np.array(vector)
-        postionR_f = np.array(postionR[:2])
-        cell_np = np.array(cell)
-        cell_np = np.array(cell_np[0:2, 0:2])
-        new_xy = np.matmul(postionR_f, cell_np)
-        new_abs_pos_f = [new_xy[0], new_xy[1], postionR[2]]
-        return new_abs_pos_f
-    else:
-        return False
 
 
 @cf
 def break_symmetry_wf(structure, wf_para, parameterdata=None):
     """
     This is the calcfunction of the routine break_symmetry, which
     introduces different 'kind objects' in a structure
@@ -325,17 +238,17 @@
                           This will create a new kind for the atom at that position.
                           Be carefull the number given has to match EXACTLY the position
                           in the structure.
 
     :param parameterdata: AiiDa ParameterData
     :return: StructureData, a AiiDA crystal structure with new kind specification.
     """
-    Dict = DataFactory('dict')
+    Dict = DataFactory('core.dict')
     if parameterdata is None:
-        parameterdata = Dict(dict={})
+        parameterdata = Dict({})
     wf_dict = wf_para.get_dict()
     atoms = wf_dict.get('atoms', ['all'])
     sites = wf_dict.get('site', [])
     pos = wf_dict.get('pos', [])
     new_kinds_names = wf_dict.get('new_kinds_names', {})
     new_structure, para_new = break_symmetry(structure,
                                              atoms=atoms,
@@ -410,15 +323,15 @@
         print('Error, no structure given')
         # throw error?
         return None, None
 
     cell = struc.cell
     pbc = struc.pbc
     sites = struc.sites
-    new_structure = DataFactory('structure')(cell=cell, pbc=pbc)
+    new_structure = DataFactory('core.structure')(cell=cell, pbc=pbc)
 
     for sym in atoms:
         replace.append(sym)
     for position in pos:
         replace_pos.append(position)
     for atom in site:
         replace_siteN.append(atom)
@@ -834,15 +747,20 @@
 
     equi_info = []
     equi_info_symbol = []
     n_equi_info_symbol = {}
     k_symbols = {}
 
     s_ase = structure.get_ase()
-    sym = spglib.get_symmetry(s_ase, symprec=1e-5)
+
+    lattice = s_ase.get_cell()
+    positions = s_ase.get_scaled_positions()
+    numbers = s_ase.get_atomic_numbers()
+
+    sym = spglib.get_symmetry((lattice, positions, numbers), symprec=1e-5)
     equi = sym['equivalent_atoms']
     unique = np.unique(equi)
 
     for uni in unique:
         equi_info.append(np.where(equi == uni)[0])
 
     sites = structure.sites
@@ -863,15 +781,18 @@
 def get_spacegroup(structure):
     """
     :param structure: AiiDA StructureData
     :return: the spacegroup (spglib class) of a given AiiDA structure
     """
     import spglib
     s_ase = structure.get_ase()
-    spacegroup = spglib.get_spacegroup(s_ase, symprec=1e-5)
+    lattice = s_ase.get_cell()
+    positions = s_ase.get_scaled_positions()
+    numbers = s_ase.get_atomic_numbers()
+    spacegroup = spglib.get_spacegroup((lattice, positions, numbers), symprec=1e-5)
     return spacegroup
 
 
 @cf
 # , _label='move_atoms_in_unitcell_wf', _description='WF, that moves all atoms in a unit cell by a given vector'):#Float1, Float2, Float3, test=None):
 def move_atoms_incell_wf(structure, wf_para):
     """
@@ -896,15 +817,15 @@
     moves all atoms in a unit cell by a given vector
 
     :param structure: AiiDA structure
     :param vector: tuple of 3, or array
     :return: AiiDA structure
     """
 
-    StructureData = DataFactory('structure')
+    StructureData = DataFactory('core.structure')
     new_structure = StructureData(cell=structure.cell)
     new_structure.pbc = structure.pbc
     sites = structure.sites
     for kind in structure.kinds:
         new_structure.append_kind(kind)
 
     for site in sites:
@@ -926,20 +847,23 @@
     :param sructure: AiiDA structure data
     :return: list of new AiiDA structure data
     """
     # TODO: if refinced structure is the same as given structure
     # return the given structure (Is this good practise for prov?)
     from spglib import find_primitive
     from ase.atoms import Atoms
-    StructureData = DataFactory('structure')
+    StructureData = DataFactory('core.structure')
 
     symprec = 1e-7
     # print('old {}'.format(len(structure.sites)))
     ase_structure = structure.get_ase()
-    lattice, scaled_positions, numbers = find_primitive(ase_structure, symprec=symprec)
+    lattice = ase_structure.get_cell()
+    positions = ase_structure.get_scaled_positions()
+    numbers = ase_structure.get_atomic_numbers()
+    lattice, scaled_positions, numbers = find_primitive((lattice, positions, numbers), symprec=symprec)
     new_structure_ase = Atoms(numbers, scaled_positions=scaled_positions, cell=lattice, pbc=True)
     new_structure = StructureData(ase=new_structure_ase)
     # print('new {}'.format(len(new_structure.sites)))
 
     new_structure.label = structure.label + ' primitive'
     new_structure.description = structure.description + ' primitive cell'
     return new_structure
@@ -1035,15 +959,15 @@
                      center_slab=False,
                      primitive=False,
                      max_normal_search=1,
                      symmetrize=False):  # , reorient_lattice=True):
     """
     :return: a dictionary of structures
     """
-    StructureData = DataFactory('structure')
+    StructureData = DataFactory('core.structure')
     aiida_strucs = {}
     # pymat_struc = initial_structure.get_pymatgen_structure()
     indices = get_all_miller_indices(initial_structure, miller_index)
     for index in indices:
         slab = create_slap(initial_structure, index, min_slab_size_ang, min_vacuum_size, min_slab_size_ang)
         #film_struc = StructureData(pymatgen_structure=slab)
         #film_struc.pbc = (True, True, False)
@@ -1061,15 +985,15 @@
                 primitive=False,
                 max_normal_search=1,
                 reorient_lattice=True):
     """
     wraps the pymatgen slab generator
     """
     # minimum slab size is in Angstrom!!!
-    StructureData = DataFactory('structure')
+    StructureData = DataFactory('core.structure')
     pymat_struc = initial_structure.get_pymatgen_structure()
     slabg = SlabGenerator(pymat_struc,
                           miller_index,
                           min_slab_size,
                           min_vacuum_size,
                           lll_reduce=lll_reduce,
                           center_slab=center_slab,
@@ -1119,15 +1043,15 @@
 def sort_atoms_z_value(structure):
     """
     Resorts the atoms in a structure by there Z-value
 
     :param structure: AiiDA structure
     :return: AiiDA structure
     """
-    StructureData = DataFactory('structure')
+    StructureData = DataFactory('core.structure')
     new_structure = StructureData(cell=structure.cell)
     new_structure.pbc = structure.pbc
     for kind in structure.kinds:
         new_structure.append_kind(kind)
 
     sites = structure.sites
     new_site_list = []
@@ -1506,15 +1430,20 @@
             atom[0][2] = -(prev_layer_z + prev_distance)  # minus inverses back
             rebuilt_structure.append_atom(position=atom[0], symbols=atom[1], name=atom[1])
 
     rebuilt_structure = center_film(rebuilt_structure)
     return rebuilt_structure
 
 
-def adjust_sym_film_relaxation(structure, suggestion, scale_as=None, bond_length=None, last_layer_factor=0.85):
+def adjust_sym_film_relaxation(structure,
+                               suggestion,
+                               scale_as=None,
+                               bond_length=None,
+                               last_layer_factor=0.85,
+                               ILD=None):
     """
     Tries to optimize interlayer distances. Can be used before RelaxWC to improve its behaviour.
     Works only for films having z-reflection symmetry, for other films check out the adjust_film_relaxation
 
     .. warning:
 
         This should work ony for metallic bonding since bond length can drastically
@@ -1541,14 +1470,16 @@
     if scale_as and not bond_length:
         raise ValueError('bond_length is required when scale_as was provided')
 
     structure = center_film(structure)
     structure = sort_atoms_z_value(structure)
 
     suggestion = deepcopy(suggestion)
+    if ILD is not None:
+        ILD = deepcopy(ILD)
     if scale_as:
         norm = suggestion[scale_as][scale_as]
         for sym1, sym2 in product(suggestion.keys(), suggestion.keys()):
             try:
                 suggestion[sym1][sym2] = suggestion[sym1][sym2] / norm
             except KeyError:
                 pass  # do nothing, happens for magnetic-magnetic or substrate-substrate combinations
@@ -1607,36 +1538,53 @@
             z_first = max(z_distances2) / 2
             rebuilt_structure.append_atom(symbols=atom[1], position=(atom[0][0], atom[0][1], z_first), name=atom[1])
             rebuilt_structure.append_atom(symbols=atom[1], position=(atom[0][0], atom[0][1], -z_first), name=atom[1])
         else:  # if the first layer is in the center we can simply add it
             rebuilt_structure.append_atom(symbols=atom[1], position=(atom[0][0], atom[0][1], atom[0][2]), name=atom[1])
 
     prev_distance = 0
-
+    if ILD is not None:
+        if len(ILD.keys()) > 0:
+            #Init Counting
+            keyILD = list(ILD)  #List of keys
+    else:
+        keyILD = 0
+    #Now iterate over all other layers
     for i, layer in enumerate(sorted_layers[1:]):
+        layer_copy = deepcopy(layer)
         add_distance1, add_distance2 = suggest_distance_to_previous(i + 1)
         if i == 0:  # the 2nd distance is the distance to the mirror image in films with no central layer
             # for a film with central layer add_distance2 == 0
             add_distance2 = add_distance2 / 2
         else:
             add_distance2 = add_distance2 - prev_distance
         if add_distance1 <= 0 and add_distance2 <= 0:
             raise ValueError('error not implemented')
         prev_distance = max(add_distance1, add_distance2)
+
         if i == len(sorted_layers) - 2 and last_layer_factor:
-            prev_distance = prev_distance * last_layer_factor  # last layer should be closer
+            if ILD is None:
+                prev_distance = prev_distance * last_layer_factor  # last layer should be closer
 
-        layer_copy = deepcopy(layer)
         prev_layer_z = max(x.position[2] for x in rebuilt_structure.sites)
 
         for atom in layer_copy:
-            atom[0][2] = prev_layer_z + prev_distance  # minus because I build from bottom (inverse)
+            if ILD is None:
+                atom[0][2] = prev_layer_z + prev_distance
+            else:
+                if ILD[keyILD[i]] == 0.0:
+                    atom[0][2] = prev_layer_z + prev_distance
+                else:
+                    atom[0][2] = prev_layer_z + ILD[keyILD[i]]
+                    print(atom)
+            print("We're here")
             rebuilt_structure.append_atom(position=atom[0], symbols=atom[1], name=atom[1])
-            rebuilt_structure.append_atom(position=(atom[0][0], atom[0][1], -atom[0][2]), symbols=atom[1], name=atom[1])
-
+            rebuilt_structure.append_atom(
+                position=(atom[0][0], atom[0][1], -atom[0][2]), symbols=atom[1],
+                name=atom[1])  # minus at atom[0][2] because the film is built from bottom (inverse)
     rebuilt_structure = center_film(rebuilt_structure)
     return rebuilt_structure
 
 
 def mark_fixed_atoms(structure, hold_layers=None):
     '''
     Marks atom in layers, that should be fixed in the relaxation. Uses reserved 49999 label
@@ -1733,22 +1681,22 @@
     else:
         symbols = first_bin + second_bin
         second_bin_calculate = second_bin
 
     for sym in symbols:
         distance = 0
         partition_function = 0
-        with MPRester(user_api_key) as mat_project:
+        with MPRester(user_api_key) as mat_project:  #pylint: disable=not-context-manager
             mp_entries = mat_project.get_entries_in_chemsys([sym])
         fcc_structure = None
         bcc_structure = None
         for entry in mp_entries:
             if sym != entry.name:
                 continue
-            with MPRester(user_api_key) as mat_project:
+            with MPRester(user_api_key) as mat_project:  #pylint: disable=not-context-manager
                 structure_analyse = mat_project.get_structure_by_material_id(entry.entry_id)
                 en_per_atom = mat_project.query(entry.entry_id, ['energy_per_atom'])[0]['energy_per_atom']
                 structure_analyse.make_supercell([2, 2, 2])
             factor = exp(-(en_per_atom / 0.0259))
             partition_function = partition_function + factor
             indices1 = structure_analyse.indices_from_symbol(sym)
             distances = (structure_analyse.get_distance(x, y) for x, y in combinations(indices1, 2))
@@ -1765,21 +1713,21 @@
         print('Request completed for {symst} {symst} pair'.format(symst=sym))
 
     for sym1, sym2 in product(first_bin, second_bin_calculate):
         if sym1 == sym2:
             continue
         distance = 0
         partition_function = 0
-        with MPRester(user_api_key) as mat_project:
+        with MPRester(user_api_key) as mat_project:  #pylint: disable=not-context-manager
             mp_entries = mat_project.get_entries_in_chemsys([sym1, sym2])
         for entry in mp_entries:
             name = ''.join([i for i in entry.name if not i.isdigit()])
             if name not in (sym1 + sym2, sym2 + sym1):
                 continue
-            with MPRester(user_api_key) as mat_project:
+            with MPRester(user_api_key) as mat_project:  #pylint: disable=not-context-manager
                 structure_analyse = mat_project.get_structure_by_material_id(entry.entry_id)
                 en_per_atom = mat_project.query(entry.entry_id, ['energy_per_atom'])[0]['energy_per_atom']
                 structure_analyse.make_supercell([2, 2, 2])
             factor = exp(-(en_per_atom / 0.0259))
             partition_function = partition_function + factor
             indices1 = structure_analyse.indices_from_symbol(sym1)
             indices2 = structure_analyse.indices_from_symbol(sym2)
@@ -1789,15 +1737,15 @@
             distance = (bond_data[sym1][sym1] + bond_data[sym2][sym2]) / 2
         else:
             distance = distance / partition_function
         bond_data[sym1][sym2] = distance
         bond_data[sym2][sym1] = distance
         print(f'Request completed for {sym1} {sym2} pair')
 
-    return Dict(dict=bond_data)
+    return Dict(bond_data)
 
 
 @cf
 def replace_element(inp_structure, replace_dict, replace_all=None):
     """
     Replaces the given element with the element_replacement, but keeps the structure the same.
     If there are more than one site they are either all replaced or a list with one replacement
@@ -1843,15 +1791,15 @@
 
     # test if structure:
     structure = is_structure(inp_structure)
     if not structure:
         # TODO: log something
         return None
 
-    StructureData = DataFactory('structure')
+    StructureData = DataFactory('core.structure')
 
     replace_dict = replace_dict.get_dict()
 
     new_structures = {}
 
     ase_struc = structure.get_ase()
     if replace_all:
@@ -1901,16 +1849,15 @@
 
 def simplify_kind_name(kind_name):
     '''
     Simplifies the kind name string. Example: "W-1" -> "W", "Iron (Fe)" -> "Fe"
     '''
     if '(' in kind_name:
         return kind_name[kind_name.find('(') + 1:kind_name.find(')')]
-    else:
-        return kind_name.split('-')[0]
+    return kind_name.split('-')[0]
 
 
 def define_AFM_structures(structure,
                           lattice,
                           directions,
                           host_symbol,
                           replacements,
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,10 +4,11 @@
 # This file is part of the AiiDA-FLEUR package.                               #
 #                                                                             #
 # The code is hosted on GitHub at https://github.com/JuDFTteam/aiida-fleur    #
 # For further information on the license, see the LICENSE.txt file            #
 # For further information please visit http://www.flapw.de or                 #
 # http://aiida-fleur.readthedocs.io/en/develop/                               #
 ###############################################################################
-'''
-FLEUR plug-in
-'''
+"""
+AiiDA Plugin for running the FLEUR code and its input generator. Also includes high-level workchains and utilities
+"""
+__version__ = '2.0.0'
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/common_aiida.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/common_aiida.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 delete_trash (FIXME)
 create_group
 
 """
 # TODO import, export of descriptions, and labels...?
 import json
 
-from six.moves import input as input_six
-
 from aiida.orm import load_node
 from aiida.orm.querybuilder import QueryBuilder
 from aiida.orm import Group, Node
 from aiida.common.exceptions import NotExistent
 
 
 def export_extras(nodes, filename='node_extras.txt'):
@@ -54,15 +52,15 @@
         if not isinstance(node, Node):  # pk or uuid
             node = load_node(node)
 
         uuid = node.uuid
         extras_dict = node.extras
         outdict[uuid] = extras_dict
 
-    with open(filename, 'w') as file:
+    with open(filename, 'w', encoding='utf-8') as file:
         json.dump(outdict, file, sort_keys=True, indent=4, separators=(',', ': '))
 
 
 def import_extras(filename):
     """
     Reads in node uuids and extras from a file (most probably generated by
     :func:`~aiida_fleur.tools.common_aiida.export_extras`) and applies them to nodes in the DB.
@@ -73,15 +71,15 @@
     :param: filename, string what file to read from (has to be json format)
 
     example use:
     import_extras('node_extras.txt')
     """
 
     all_extras = {}
-    with open(filename) as file1:
+    with open(filename, encoding='utf-8') as file1:
         try:
             all_extras = json.load(file1)
         except json.JSONDecodeError:
             print('The file has to be loadable by json. i.e json format (which it is not).')
 
     for uuid, extras in all_extras.items():
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/common_fleur_wf.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/common_fleur_wf.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,28 +38,33 @@
 
         inputs_build = get_inputs_inpgen(structure, inpgencode, options, label,
                                          description, params=params)
         future = self.submit(inputs_build)
 
 
     '''
-    Dict = DataFactory('dict')
+    Dict = DataFactory('core.dict')
     inputs = {}
 
-    add_comp_para_default = {'only_even_MPI': False, 'max_queue_nodes': 20, 'max_queue_wallclock_sec': 86400}
+    add_comp_para_default = {
+        'only_even_MPI': False,
+        'forbid_single_mpi': False,
+        'max_queue_nodes': 20,
+        'max_queue_wallclock_sec': 86400
+    }
     if add_comp_para is None:
         add_comp_para = {}
     add_comp_para = {**add_comp_para_default, **add_comp_para}
 
     if remote:
         inputs['parent_folder'] = remote
     if code:
         inputs['code'] = code
     if fleurinp:
-        inputs['fleurinpdata'] = fleurinp
+        inputs['fleurinp'] = fleurinp
 
     if description:
         inputs['description'] = description
     else:
         inputs['description'] = ''
     if label:
         inputs['label'] = label
@@ -82,24 +87,24 @@
         if not options['withmpi'] and 'resources' not in options:
             # TODO not every machine/scheduler type takes number of machines
             #  lsf takes number of total_mpi_procs,slurm and psb take num_machines,\
             # also a full will run here mpi on that node... also not what we want.ß
             options['resources'] = {'num_machines': 1, 'num_mpiprocs_per_machine': 1}
 
     inputs['clean_workdir'] = Bool(add_comp_para.pop('clean_workdir', False))
-    inputs['add_comp_para'] = Dict(dict=add_comp_para)
+    inputs['add_comp_para'] = Dict(add_comp_para)
 
     if settings:
         if isinstance(settings, Dict):
             inputs['settings'] = settings
         else:
-            inputs['settings'] = Dict(dict=settings)
+            inputs['settings'] = Dict(settings)
 
     if options:
-        inputs['options'] = Dict(dict=options)
+        inputs['options'] = Dict(options)
 
     return inputs
 
 
 def get_inputs_inpgen(structure, inpgencode, options, label='', description='', settings=None, params=None, **kwargs):
     '''
     Assembles the input dictionary for Fleur Calculation.
@@ -152,76 +157,61 @@
     # Currently this does not work, find out howto...
     # for key, val in kwargs.items():
     #    inputs[key] = val
 
     return inputs
 
 
-def test_and_get_codenode(codenode, expected_code_type, use_exceptions=False):
+def test_and_get_codenode(codenode, expected_code_type):
     """
     Pass a code node and an expected code (plugin) type. Check that the
     code exists, is unique, and return the Code object.
 
     :param codenode: the name of the code to load (in the form label@machine)
     :param expected_code_type: a string with the plugin that is expected to
       be loaded. In case no plugins exist with the given name, show all existing
       plugins of that type
-    :param use_exceptions: if True, raise a ValueError exception instead of
-      calling sys.exit(1)
     :return: a Code object
     """
-    import sys
-    from aiida.common.exceptions import NotExistent
-    from aiida.orm import Code
+    from aiida.orm.querybuilder import QueryBuilder
+    from aiida.orm import Code, load_code
+
+    if not isinstance(codenode, Code):
+        codenode = load_code(codenode)
+
+    plugin_name = codenode.get_input_plugin_name()
+    if plugin_name != expected_code_type:
+        message = f'Expected Code of type {expected_code_type}. Got: {plugin_name}\n'
 
-    try:
-        if codenode is None or not isinstance(codenode, Code):
-            raise ValueError
-        code = codenode
-        if code.get_input_plugin_name() != expected_code_type:
-            raise ValueError
-    except ValueError as exc:
-        from aiida.orm.querybuilder import QueryBuilder
         qb = QueryBuilder()
         qb.append(Code, filters={'attributes.input_plugin': {'==': expected_code_type}}, project='*')
 
-        valid_code_labels = [f'{c.label}@{c.computer.label}' for [c] in qb.all()]
+        valid_code_labels = [f'{c.label}@{c.computer.label}' for c in qb.all(flat=True)]
 
         if valid_code_labels:
-            msg = ('Given Code node is not of expected code type.\n'
-                   'Valid labels for a {} executable are:\n'.format(expected_code_type))
-            msg += '\n'.join(f'* {l}' for l in valid_code_labels)
-
-            if use_exceptions:
-                raise ValueError(msg) from exc
-            else:
-                print(msg)  # , file=sys.stderr)
-                sys.exit(1)
+            message += f'Valid labels for a {expected_code_type} executable are:\n'
+            message += '\n'.join(f'* {l}' for l in valid_code_labels)
         else:
-            msg = ('Code not valid, and no valid codes for {}.\n'
-                   'Configure at least one first using\n'
-                   '    verdi code setup'.format(expected_code_type))
-            if use_exceptions:
-                raise ValueError(msg) from exc
-            else:
-                print(msg)  # , file=sys.stderr)
-                sys.exit(1)
+            message += f'No valid labels for a {expected_code_type} executable are available\n' \
+                        'Configure at least one first using\n' \
+                        '    verdi code setup'
+        raise ValueError(message)
 
-    return code
+    return codenode
 
 
 def get_kpoints_mesh_from_kdensity(structure, kpoint_density):
     """
     params: structuredata, Aiida structuredata
     params: kpoint_density
 
     returns: tuple (mesh, offset)
     returns: kpointsdata node
     """
-    KpointsData = DataFactory('array.kpoints')
+    KpointsData = DataFactory('core.array.kpoints')
     kp = KpointsData()
     kp.set_cell_from_structure(structure)
     density = kpoint_density  # 1/A
     kp.set_kpoints_mesh_from_density(density)
     mesh = kp.get_kpoints_mesh()
     return mesh, kp
 
@@ -472,15 +462,16 @@
                           mpi_per_node,
                           omp_per_mpi,
                           use_omp,
                           mpi_omp_ratio,
                           fleurinpData=None,
                           kpts=None,
                           sacrifice_level=0.9,
-                          only_even_MPI=False):
+                          only_even_MPI=False,
+                          forbid_single_mpi=False):
     """
     Makes a suggestion on parallelisation setup for a particular fleurinpData.
     Only the total number of k-points is analysed: the function suggests ideal k-point
     parallelisation + OMP parallelisation (if required). Note: the total number of used CPUs
     per node will not exceed mpi_per_node * omp_per_mpi.
 
     Sometimes perfect parallelisation is terms of idle CPUs is not what
@@ -494,15 +485,16 @@
     :param omp_per_mpi: an input suggestion for OMP tasks per MPI process
     :param use_omp: False if OMP parallelisation is not needed
     :param mpi_omp_ratio: requested MPI/OMP ratio
     :param fleurinpData: FleurinpData to extract total number of kpts from
     :param kpts: the total number of kpts
     :param sacrifice_level: sets a level of performance sacrifice that a user can afford for better
                             MPI/OMP ratio.
-    :parm only_even_MPI: if set to True, the function does not set MPI to an odd number (if possible)
+    :param only_even_MPI: if set to True, the function does not set MPI to an odd number (if possible)
+    :param forbid_single_mpi: if set to True, the configuration 1 node 1 MPI per node will be forbidden
     :returns nodes, MPI_tasks, OMP_per_MPI, message: first three are parallelisation info and
                                                      the last one is an exit message.
     """
     from sympy.ntheory.factor_ import divisors
     import numpy as np
 
     cpus_per_node = mpi_per_node * omp_per_mpi
@@ -538,14 +530,21 @@
     suggestions = np.array(add_omp(suggestions, only_even_MPI))
     if not len(suggestions):  # only odd MPI parallelisations possible, ignore only_even_MPI
         suggestions = np.array(add_omp(suggestions_save, False))
 
     best_resources = max(np.prod(suggestions, axis=1))
     top_suggestions = suggestions[np.prod(suggestions, axis=1) > sacrifice_level * best_resources]
 
+    if forbid_single_mpi:
+        top_suggestions = [s for s in top_suggestions if s[0] * s[1] != 1]
+
+    if len(top_suggestions) == 0:
+        raise ValueError('A Parallelization meeting the requirements could not be determined'
+                         f'for the given number k-points ({kpts})')
+
     def best_criterion(suggestion):
         if use_omp:
             return -abs(suggestion[1] / suggestion[2] - mpi_omp_ratio)
         return (suggestion[0] * suggestion[1], -suggestion[0])
 
     best_suggestion = max(top_suggestions, key=best_criterion)
 
@@ -556,15 +555,16 @@
                    'from {} to {}.'
                    'Changed the number of nodes from {} to {}. '
                    'Computational setup, needed for a given number k-points ({})'
                    ' provides less then 60% of node load.'
                    ''.format(mpi_per_node, best_suggestion[1], omp_per_mpi, best_suggestion[2], nodes,
                              best_suggestion[0], kpts))
         raise ValueError(message)
-    elif best_suggestion[1] * best_suggestion[2] == cpus_per_node:
+
+    if best_suggestion[1] * best_suggestion[2] == cpus_per_node:
         if best_suggestion[0] != nodes:
             message = f'WARNING: Changed the number of nodes from {nodes} to {best_suggestion[0]}'
         else:
             message = ('Computational setup is perfect! Nodes: {}, MPIs per node {}, OMP per MPI '
                        '{}. Number of k-points is {}'.format(best_suggestion[0], best_suggestion[1], best_suggestion[2],
                                                              kpts))
     else:
@@ -579,37 +579,33 @@
 def find_last_submitted_calcjob(restart_wc):
     """
     Finds the last CalcJob submitted in a higher-level workchain
     and returns it's uuid
     """
     from aiida.common.exceptions import NotExistent
     from aiida.orm import CalcJobNode
-    links = restart_wc.get_outgoing().all()
-    calls = [x for x in links if isinstance(x.node, CalcJobNode)]
+    calls = restart_wc.get_outgoing(node_class=CalcJobNode).all()
     if calls:
         calls = sorted(calls, key=lambda x: x.node.pk)
         return calls[-1].node.uuid
-    else:
-        raise NotExistent
+    raise NotExistent
 
 
 def find_last_submitted_workchain(restart_wc):
     """
     Finds the last WorkChain submitted in a higher-level workchain
     and returns it's uuid
     """
     from aiida.common.exceptions import NotExistent
     from aiida.orm import WorkChainNode
-    links = restart_wc.get_outgoing().all()
-    calls = [x for x in links if isinstance(x.node, WorkChainNode)]
+    calls = restart_wc.get_outgoing(node_class=WorkChainNode).all()
     if calls:
         calls = sorted(calls, key=lambda x: x.node.pk)
         return calls[-1].node.uuid
-    else:
-        raise NotExistent
+    raise NotExistent
 
 
 def find_nested_process(wc_node, p_class):
     '''
     This function finds all nested child processes of p_class
     '''
     child_process = []
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/common_fleur_wf_util.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/common_fleur_wf_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,54 +496,53 @@
     #   for c in s:
     #       prod = '%d*%s' % (c[1], c[0])
     #       res1 = res1 + '+' + prod
     #   Qs.append(res1)
     #Qs + [Ys['a'] - a]
 
     k = solve(Qs, *Ys)
-    if k:  # if a solution is found multiply by gcd
-        # TODO? check if solution has linear dependence: and evaluate
-        #for c in k.values():
-        #    for char in list(letters):
-        #        if char in str(c):
-        #             pass
-        N = []  #[k[Ys[s]]for s in sorted(Ys)]
-        rescale_N = False
-        denom_list = []
-        for s in sorted(Ys):
-            n = k[Ys[s]]
-            # idea: check if char in n, then linear depended, then
-            try:  # since solver gives also a linear depended solution if correct, but code fails then
-                if n < 0 and not allow_negativ:  # We allow for 0 but might be an other case to think about
-                    return None
-            except TypeError:
-                return None  # TODO Maybe other return value... maybe list of some values for
-                # linear dependencies, d,e,....? also choose them that the value is positive...?
-            if n == 0 and not allow_zero:
+    if not k:  # if a solution is found multiply by gcd
+        return None
+    # TODO? check if solution has linear dependence: and evaluate
+    #for c in k.values():
+    #    for char in list(letters):
+    #        if char in str(c):
+    #             pass
+    N = []  #[k[Ys[s]]for s in sorted(Ys)]
+    rescale_N = False
+    denom_list = []
+    for s in sorted(Ys):
+        n = k[Ys[s]]
+        # idea: check if char in n, then linear depended, then
+        try:  # since solver gives also a linear depended solution if correct, but code fails then
+            if n < 0 and not allow_negativ:  # We allow for 0 but might be an other case to think about
                 return None
-            N.append(n)
+        except TypeError:
+            return None  # TODO Maybe other return value... maybe list of some values for
+            # linear dependencies, d,e,....? also choose them that the value is positive...?
+        if n == 0 and not allow_zero:
+            return None
+        N.append(n)
 
-            # Rationals are a problem in gcd, so we have to get rid of them
-            if isinstance(n, Rational):
-                rescale_N = True
-                denom_list.append(n.as_numer_denom()[1])
-        if rescale_N:
-            multiplier = 1
-            for denom in denom_list:
-                multiplier = multiplier * int(denom)
-            N = [int(n * multiplier) for n in N]
-        g = N[0]
-        for a1, a2 in zip(N[0::2], N[0::2]):
-            g = gcd(g, a2)
-        N = [int(i / g) for i in N]
-        pM = lambda c: str(c) + '*'  # if c!=1 else ''
-        res = '->'.join('+'.join(pM(N.pop(0)) + str(t) for t in p.split('+')) for p in eq.split('->'))
-        return res
-    else:
-        return None
+        # Rationals are a problem in gcd, so we have to get rid of them
+        if isinstance(n, Rational):
+            rescale_N = True
+            denom_list.append(n.as_numer_denom()[1])
+    if rescale_N:
+        multiplier = 1
+        for denom in denom_list:
+            multiplier = multiplier * int(denom)
+        N = [int(n * multiplier) for n in N]
+    g = N[0]
+    for a1, a2 in zip(N[0::2], N[0::2]):
+        g = gcd(g, a2)
+    N = [int(i / g) for i in N]
+    pM = lambda c: str(c) + '*'  # if c!=1 else '' #pylint: disable=unnecessary-lambda-assignment
+    res = '->'.join('+'.join(pM(N.pop(0)) + str(t) for t in p.split('+')) for p in eq.split('->'))
+    return res
 
 
 def check_eos_energies(energylist):
     """
     Checks if there is an abnormality in the total energies from the Equation of states.
     i.e. if one point has a larger energy then its two neighbors
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/create_corehole.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/create_corehole.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/create_kpoints_from_distance.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/create_kpoints_from_distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,13 +105,13 @@
         nkpoints = max(kpointsmesh)
         kpointsmesh = [nkpoints, nkpoints, nkpoints]
 
     mesh_spec = {'kpt': {'div1': kpointsmesh[0], 'div2': kpointsmesh[1], 'div3': kpointsmesh[2]}}
     if include_gamma:
         mesh_spec['kpt']['gamma'] = True
 
-    new_calc_para = Dict(dict=mesh_spec)
+    new_calc_para = Dict(mesh_spec)
     if calc_parameters is not None:
         # Override false, since we want to keep other kpts keys in calc_parameters
         new_calc_para = merge_parameter(new_calc_para, calc_parameters, overwrite=False, merge=True)
 
     return new_calc_para
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/data_handling.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/data_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,22 +26,22 @@
     returns that information as a dict, which could be used for further evalation
     #keys = ['uuid', 'formula', 'pk', 'symmetry', 'pbc', 'volume', 'total_energy',
     'child_nodes', 'natoms', 'group', extras', 'label', 'description', 'cif_file',
     'cif_number', 'cif_uuid', 'cif_ref', 'calcfunctions', 'band', 'dos', 'eos',
     'init_cls', 'corehole', primitive]
 
     """
-    StructureData = DataFactory('structure')
+    StructureData = DataFactory('core.structure')
     structure_list = []
 
     from aiida_fleur.tools.StructureData_util import get_spacegroup, is_structure
     from aiida_fleur.tools.StructureData_util import is_primitive
 
     if not structures:
-        StructureData = DataFactory('structure')
+        StructureData = DataFactory('core.structure')
         #t = time.time()
         qb = QB()
         qb.append(StructureData)
         structures = qb.all()
         #elapsed = time.time() - t
         # print "Total number of structures: {} (retrieved in {} s.)".format(len(structures), elapsed)
         #t = time.time()
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/dict_util.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/dict_util.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/element_econfig_list.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/element_econfig_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1639,15 +1639,15 @@
 # TODO maybe use a panda file format or something for this...
 # export to json, read in here.
 import aiida_fleur
 import os
 
 aiida_path = os.path.dirname(aiida_fleur.__file__)
 EXP_BINDENERGIES_PATH = os.path.join(aiida_path, 'tools/exp_bindingenergies.json')
-with open(EXP_BINDENERGIES_PATH) as fn:
+with open(EXP_BINDENERGIES_PATH, encoding='utf-8') as fn:
     exp_bindingenergies = json.load(fn)
 """
 exp_bindingenergies = {
  1 : {'binding_energy': {'1s1/2': []}, 'name': 'Hydrogen', 'symbol': 'H'},
  2: {'binding_energy': {'1s1/2': []}, 'name': 'Helium', 'symbol': 'He'},
  3: {'binding_energy': {'1s1/2': [56], '2s1/2': []},
      'name': 'Lithium',
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/exp_bindingenergies.json` & `aiida-fleur-2.0.0/aiida_fleur/tools/exp_bindingenergies.json`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/extract_corelevels.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/extract_corelevels.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,14 +120,17 @@
     species_xpath = '/fleurOutput/inputData/atomSpecies'
     iteration_xpath = '/fleurOutput/scfLoop/iteration'
     atomgroup_xpath = '/fleurOutput/inputData/atomGroups'
     coreconfig_xpath = 'electronConfig/coreConfig/text()'
     valenceconfig_xpath = 'electronConfig/valenceConfig/text()'
     state_occ_xpath = 'electronConfig/stateOccupation'
 
+    new_species_xpath = '/fleurOutput/fleurInput/atomSpecies'
+    new_atomgroup_xpath = '/fleurOutput/fleurInput/atomGroups'
+
     relcoreStates_xpath = 'coreStates'
     relpos_xpath = 'relPos'
     abspos_xpath = 'absPos'
     filmpos_xpath = 'filmPos'
     #TODO all the attribute names...
     ######################
 
@@ -158,14 +161,16 @@
     #if parse_xml:
     root = tree.getroot()
 
     # 2. get all species from input
     # get element, name, coreStates
     # TODO why can this not be eval_xpath2?
     species_nodes = eval_xpath(root, species_xpath)
+    if not species_nodes:
+        species_nodes = eval_xpath(root, new_species_xpath)
     species_atts = {}
     species_names = []
     for species in species_nodes:
         species_name = species.get('name')
         species_corestates = species.get('coreStates')
         species_element = species.get('element')
         species_atomicnumber = species.get('atomicNumber')
@@ -195,14 +200,16 @@
             'stateOccupation': state_results
         }
         species_names.append(species_name)
 
     #3. get number of atom types and their species from input
     atomtypes = []
     atomgroup_nodes = eval_xpath(root, atomgroup_xpath)  #/fleurinp/
+    if not atomgroup_nodes:
+        atomgroup_nodes = eval_xpath(root, new_atomgroup_xpath)
     # always a list?
     for atomgroup in atomgroup_nodes:
         types_dict = {}
         group_species = atomgroup.get('species')
         if group_species in species_names:
             species_atts[group_species]['atomgroups'].append(atomgroup)
             element = species_atts[group_species]['element']
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/io_routines.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/io_routines.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
     Writes data to a file
 
     param headerstring: string with information
     param data: 2D array (numpy,scipy) with data [colum1 colum2, ...]
     """
 
-    with open(destination, 'w') as thefile:
+    with open(destination, 'w', encoding='utf-8') as thefile:
         thefile.write(headerstring)
         datastring = ''
         #seperator = seperator  # '\t'
         if transpose:
             datat = data.transpose()
         else:
             datat = data
@@ -119,15 +119,15 @@
      outxmlsrc = '/Users/broeder/test/FePt_out.xml'
      compress_fleuroutxml(outxmlsrc, dest_file_path=outxmldes, iterations_to_keep=14)
      compress_fleuroutxml(outxmlsrc, dest_file_path=outxmldes, iterations_to_keep=-1)
     """
     from masci_tools.util.xml.xml_setters_names import delete_tag
     from masci_tools.util.schema_dict_util import get_number_of_nodes
     from masci_tools.util.schema_dict_util import eval_simple_xpath
-    from masci_tools.io.io_fleurxml import load_outxml
+    from masci_tools.io.fleur_xml import load_outxml
     from lxml import etree
 
     xmltree, schema_dict = load_outxml(outxmlfilepath)
     xpath_iteration = schema_dict.tag_xpath('iteration')
 
     # delete eigenvalues (all)
     if delete_eig:
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/merge_parameter.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/merge_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         raise InputValidationError('Dict1, must be of type Dict')
     if not isinstance(Dict2, Dict):
         raise InputValidationError('Dict2, must be of type Dict')
     dict1 = Dict1.get_dict()
     dict2 = Dict2.get_dict()
 
     if dict1 == dict2:
-        return Dict(dict=dict1)
+        return Dict(dict1)
 
     for key in list(dict1.keys()):
         if 'atom' in key:
             val = dict1.pop(key)
             atomlist.append(val)
 
     for key in list(dict2.keys()):
@@ -95,23 +95,23 @@
             new_dict.update(dict1)
         # TODO mergeing does not make sense for all namelist keys.
         # be more specific here.
     new_dict.update(atoms_dict)
 
     # be carefull with atom namelist
 
-    return Dict(dict=new_dict)
+    return Dict(new_dict)
 
 
 def merge_parameters(DictList, overwrite=True):
     """
     Merge together all parameter nodes in the given list.
     """
     #Dict = DataFactory('dict')
-    paremeter_data_new = Dict(dict={})
+    paremeter_data_new = Dict({})
 
     for i, parameter in enumerate(DictList):
         if isinstance(parameter, Dict):
             # merge
             paremeter_data_new = merge_parameter(paremeter_data_new, parameter, overwrite=overwrite)
         else:
             print(f'WARNING: Entry : {i} {parameter} is not of type Dict, I skip it.')
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/plot/__init__.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/plot/fleur.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/plot/fleur.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 #  (that user can put pks or structure formulas in there)
 # INFO: AiiDAlab has implemented an extendable viewer class for data structures,
 # which might be some point moved to aiida-core and extensible over entrypoints.
 
 from pprint import pprint
 import warnings
 import numpy as np
+import re
 
+from aiida.common.links import LinkType
 from aiida.orm import load_node, Node, WorkChainNode, Dict
-from aiida.common.exceptions import UniquenessError, NotExistent
 
 from masci_tools.util.constants import HTR_TO_EV
 from masci_tools.vis.common import set_defaults, set_default_backend, show_defaults, save_defaults, load_defaults, reset_defaults
 
 __all__ = ('plot_fleur', 'set_defaults', 'set_default_backend', 'show_defaults', 'save_defaults', 'load_defaults',
            'reset_defaults')
 
@@ -161,15 +162,15 @@
 
     :returns: tuple of nodes to pass to the corresponding visualization function,
               name of the workflow and label of the node
     """
 
     #Define any additional node hat should be passed to the plotting function
     ADDITIONAL_OUTPUTS = {
-        'FleurBandDosWorkChain': ('last_calc_retrieved',),
+        'FleurBandDosWorkChain': ('banddos_calc__retrieved',),
         'FleurCFCoeffWorkChain': ('output_cfcoeff_wc_charge_densities', 'output_cfcoeff_wc_potentials')
     }
 
     if isinstance(node, (int, str)):
         node = load_node(node)
 
     if not isinstance(node, Node):
@@ -177,42 +178,32 @@
 
     label = node.label
 
     parameter_node = None
     workchain_node = None
     if isinstance(node, WorkChainNode):
         workchain_node = node
-        output_list = workchain_node.get_outgoing().all()
+        output_list = workchain_node.get_outgoing(link_type=LinkType.RETURN).all()
         for out_link in output_list:
-            if 'output_' in out_link.link_label:
-                if 'wc' in out_link.link_label or 'wf' in out_link.link_label:
-                    if 'para' in out_link.link_label:  # We are just looking for parameter
-                        #nodes, structures, bands, dos and so on we tread different
-                        parameter_node = out_link.node  # we only visualize last output node
+            if re.fullmatch('output_.+_w[cf]_para', out_link.link_label):
+                parameter_node = out_link.node  # we only visualize last output node
     elif isinstance(node, Dict):
         parameter_node = node
 
-    if isinstance(parameter_node, Dict):
-        parameter_dict = parameter_node.get_dict()
-        workflow_name = parameter_dict.get('workflow_name', None)
-    else:
+    if parameter_node is None:
         raise ValueError(f'I do not know how to visualize this node: {node}')
 
+    parameter_dict = parameter_node.get_dict()
+    workflow_name = parameter_dict.get('workflow_name', None)
+
     add_outputs = ADDITIONAL_OUTPUTS.get(workflow_name, tuple())
     add_nodes = tuple()
     if add_outputs:
         if workchain_node is None:
-            incoming = parameter_node.get_incoming(node_class=WorkChainNode).all()
-            n_parents = len(incoming)
-            if n_parents > 1:
-                raise UniquenessError(f'Parameter node {parameter_node} has no unique WorkChainNode parent')
-            if n_parents == 0:
-                raise NotExistent(f'Parameter node {parameter_node} has no WorkChainNode parent')
-            workchain_node = incoming[0].node
-
+            workchain_node = parameter_node.get_incoming(node_class=WorkChainNode).one().node
         add_nodes = tuple(workchain_node.get_outgoing().get_node_by_label(out_label) for out_label in add_outputs)
 
     outputs = (parameter_node,) + add_nodes
 
     return outputs, workflow_name, label
 
 
@@ -478,81 +469,98 @@
 
 def plot_fleur_orbcontrol_wc(nodes,
                              labels=None,
                              save=False,
                              show=True,
                              line_labels=None,
                              backend='matplotlib',
+                             size_func=None,
                              **kwargs):
     """
     This methods takes AiiDA output parameter nodes from a orbcontrol
     workchain and plots the energy of the individual configurations.
     """
-    from masci_tools.vis.common import scatter
+    from masci_tools.vis.common import scatter, PlotBackend
     from itertools import chain
 
     if labels is None:
         labels = []
 
     if not isinstance(nodes, list):
         nodes = [nodes]
 
     offset = 0
     lines = []
     converged_configs = []
     converged_energy = []
     non_converged_configs = []
     non_converged_energy = []
+    converged_size_data = []
+    non_converged_size_data = []
     for node in nodes:
         outputs = node.get_dict()
 
         total_energy = outputs['total_energy']
 
         non_converged = outputs['non_converged_configs']
         converged = [i for i in outputs['successful_configs'] if i not in non_converged]
 
         converged_configs.extend(i + offset for i in converged)
         converged_energy.extend(total_energy[i] for i in converged)
 
         non_converged_configs.extend(i + offset for i in non_converged)
         non_converged_energy.extend(total_energy[i] for i in non_converged)
 
+        if size_func is not None:
+            #The size_func operates on the original workchain node (to make introspection easier)
+            wc_node = node.get_incoming(link_type=LinkType.RETURN).one().node
+            size = size_func(wc_node)
+            if not isinstance(size, list) or len(size) != len(total_energy):
+                raise ValueError(f'Wrong length of size data. Expected {len(total_energy)} entries: '
+                                 f'Got {len(size) if isinstance(size, list) else size}')
+
+            converged_size_data.extend(size[i] for i in converged)
+            non_converged_size_data.extend(size[i] for i in non_converged)
+
         offset += max(chain(converged, non_converged, outputs['failed_configs'])) + 1
         lines.append(offset - 0.5)
 
     #Convert to relative eV
     refE = min(converged_energy)
     converged_energy = np.array(converged_energy) - refE
     non_converged_energy = np.array(non_converged_energy) - refE
 
     converged_energy *= HTR_TO_EV
     non_converged_energy *= HTR_TO_EV
 
-    if backend == 'matplotlib':
+    backend = PlotBackend.from_str(backend)
+    if backend == PlotBackend.mpl:
         kwargs.setdefault('plot_label', ['converged', 'not converged'])
     else:
         kwargs.setdefault('legend_label', ['converged', 'not converged'])
 
     kwargs.setdefault('xlabel', 'Configurations')
     kwargs.setdefault('ylabel', r'$E_{rel}$ [eV]')
     kwargs.setdefault('title', 'Results for orbcontrol node')
-    kwargs.setdefault('legend_option', {'loc': 'upper right'})
+    kwargs.setdefault('legend_options', {'loc': 'upper right'})
     kwargs.setdefault('markersize', 10.0)
     kwargs.setdefault('legend', True)
     if len(lines) > 1:
         kwargs.setdefault('lines', {'vertical': lines[:-1]})
+    if size_func is not None:
+        kwargs.setdefault('size_data', [converged_size_data, non_converged_size_data])
 
     p1 = scatter([converged_configs, non_converged_configs], [converged_energy, non_converged_energy],
                  color=['darkblue', 'darkred'],
                  save_plots=save,
                  show=show,
                  backend=backend,
                  **kwargs)
 
-    if line_labels and backend == 'matplotlib':
+    if line_labels and backend == PlotBackend.mpl:
         for label, pos in zip(line_labels, [0] + [p + 0.25 for p in lines]):
             p1.annotate(label, xy=(pos, 0.95), xycoords=('data', 'axes fraction'), ha='left', va='center', size=16)
 
     return p1
 
 
 def plot_fleur_cfcoeff_wc(param_node,
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/queue_defaults.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/queue_defaults.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/read_cif_folder.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/read_cif_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     :params: log: bool, if True, writes a logfile with information (pks, and co)
     :params: comments: string: comment to add to the structures
     :params: extras: dir/string/arb: extras added to the structures stored in the db
 
     """
     # TODO check for duplicates in the database, so that reruning the functions
     # won't import anything else in the database
-    cifdata = DataFactory('cif')
+    cifdata = DataFactory('core.cif')
     ############ parameters for the user to set ########
 
     parent_cif_folder = path  # folder path
     store_db = store  # True # store stuff in database?
     write_log = log  # write a logfiles on what was saved
     comment = comments  # comments and extras to add to the structure nodes.
     extra = extras  # helpfull for finding them again in the db
@@ -154,15 +154,15 @@
 @cf
 def wf_struc_from_cif(cif):
     return struc_from_cif(cif)
 
 
 def struc_from_cif(cif):
     asecell = cif.get_ase()
-    struc = DataFactory('structure')(ase=asecell)
+    struc = DataFactory('core.structure')(ase=asecell)
     return struc
 
 
 # TODO add this to command line, or better move to aiida-jutools
 # ggf add what Roman has done there.
 '''
 if __name__ == '__main__':
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/tools/xml_aiida_modifiers.py` & `aiida-fleur-2.0.0/aiida_fleur/tools/xml_aiida_modifiers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 """
 This module defines XML modifying functions, that require an aiida node as input
 """
+from __future__ import annotations
 
-
-def set_kpointsdata_f(xmltree, schema_dict, kpointsdata_uuid, name=None, switch=False, kpoint_type='path'):
+from masci_tools.util.typing import XMLLike
+from masci_tools.io.parsers.fleur_schema import InputSchemaDict
+from aiida import orm
+
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal  #type: ignore[assignment]
+
+
+def set_kpointsdata_f(xmltree: XMLLike,
+                      schema_dict: InputSchemaDict,
+                      kpointsdata_uuid: orm.KpointsData | int | str,
+                      name: str | None = None,
+                      switch: bool = False,
+                      kpoint_type: Literal['path', 'mesh', 'tria', 'tria-bulk', 'spex-mesh'] = 'path') -> XMLLike:
     """This function creates a kpoint list in the inp.xml from a :py:class:`~aiida.orm.KpointsData` Node
     If no weights are given the weight is distibuted equally along the kpoints
 
     :param xmltree: an xmltree that represents inp.xml
     :param schema_dict: InputSchemaDict containing all information about the structure of the input
     :param kpointsdata_uuid: node identifier or :class:`~aiida.orm.KpointsData` node to be written into ``inp.xml``
     :param name: str name to give the newly entered kpoint list (only MaX5 or later)
     :param switch: bool if True the entered kpoint list will be used directly (only Max5 or later)
     :param kpoint_type: str of the type of kpoint list given (mesh, path, etc.) only Max5 or later
 
     :return: xmltree with entered kpoint list
     """
     # TODO: check on weights,
     import numpy as np
-    from aiida.orm import KpointsData, load_node
     from aiida.common.exceptions import InputValidationError
     from masci_tools.util.xml.xml_setters_names import set_kpointlist
 
-    if not isinstance(kpointsdata_uuid, KpointsData):
-        KpointsDataNode = load_node(kpointsdata_uuid)
+    if not isinstance(kpointsdata_uuid, orm.KpointsData):
+        KpointsDataNode = orm.load_node(kpointsdata_uuid)
     else:
         KpointsDataNode = kpointsdata_uuid
 
-    if not isinstance(KpointsDataNode, KpointsData):
+    if not isinstance(KpointsDataNode, orm.KpointsData):
         raise InputValidationError('The node given is not a valid KpointsData node.')
 
     try:
         kpoints, weights = KpointsDataNode.get_kpoints(also_weights=True, cartesian=False)
     except AttributeError:
         kpoints = KpointsDataNode.get_kpoints(cartesian=False)
         weights = np.ones(len(kpoints)) / len(kpoints)
@@ -57,10 +71,7 @@
                                  weights,
                                  special_labels=labels_dict,
                                  kpoint_type=kpoint_type,
                                  name=name,
                                  switch=switch)
 
     return xmltree
-
-
-FLEURINPMODIFIER_EXTRA_FUNCS = {'schema_dict': {'set_kpointsdata': set_kpointsdata_f}}
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/banddos.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/banddos.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # TODO alow certain kpoint path, or kpoint node, so far auto
 import copy
 from lxml import etree
 from ase.dft.kpoints import bandpath
 import numpy as np
 
 from aiida.orm import Code, Dict, RemoteData, KpointsData
-from aiida.orm import load_node, CalcJobNode, FolderData, BandsData, XyData
+from aiida.orm import load_node, FolderData, BandsData, XyData
 from aiida.engine import WorkChain, ToContext, if_
 from aiida.engine import calcfunction as cf
 from aiida.common.exceptions import NotExistent
 from aiida.common import AttributeDict
 from aiida.tools.data.array.kpoints import get_explicit_kpoints_path
 
 from aiida_fleur.workflows.scf import FleurScfWorkChain
@@ -40,15 +40,15 @@
 
     :Params: a Fleurcalculation node
     :returns: Success, last result node, list with convergence behavior
     '''
     # wf_parameters: {  'tria', 'nkpts', 'sigma', 'emin', 'emax'}
     # defaults : tria = True, nkpts = 800, sigma=0.005, emin= , emax =
 
-    _workflowversion = '0.5.2'
+    _workflowversion = '0.7.0'
 
     _default_options = {
         'resources': {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1
         },
         'max_wallclock_seconds': 60 * 60,
@@ -97,15 +97,15 @@
                          cls.converge_scf,
                          cls.banddos_after_scf,
                      ).else_(
                          cls.banddos_wo_scf,
                      ), cls.return_results)
 
         spec.output('output_banddos_wc_para', valid_type=Dict)
-        spec.output('last_calc_retrieved', valid_type=FolderData)
+        spec.expose_outputs(FleurBaseWorkChain, namespace='banddos_calc')
         spec.output('output_banddos_wc_bands', valid_type=BandsData, required=False)
         spec.output('output_banddos_wc_dos', valid_type=XyData, required=False)
 
         spec.exit_code(230, 'ERROR_INVALID_INPUT_PARAM', message='Invalid workchain parameters.')
         spec.exit_code(231, 'ERROR_INVALID_INPUT_CONFIG', message='Invalid input configuration.')
         spec.exit_code(233,
                        'ERROR_INVALID_CODE_PROVIDED',
@@ -165,15 +165,15 @@
         # extend options given by user using defaults
         for key, val in defaultoptions.items():
             options[key] = options.get(key, val)
         self.ctx.options = options
 
         if 'fleur' in inputs:
             try:
-                test_and_get_codenode(inputs.fleur, 'fleur.fleur', use_exceptions=True)
+                test_and_get_codenode(inputs.fleur, 'fleur.fleur')
             except ValueError:
                 error = 'The code you provided for FLEUR does not use the plugin fleur.fleur'
                 self.report(error)
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
         if 'scf' in inputs:
             self.ctx.scf_needed = True
@@ -483,30 +483,23 @@
     def return_results(self):
         '''
         return the results of the calculations
         '''
         # TODO more here
         self.report('BandDOS workflow Done')
 
-        from aiida_fleur.tools.common_fleur_wf import find_last_submitted_calcjob
         if self.ctx.banddos_calc:
             self.report(f'A bandstructure/DOS was calculated and is found under pk={self.ctx.banddos_calc.pk}, '
                         f'calculation {self.ctx.banddos_calc}')
-            try:
-                last_calc_uuid = find_last_submitted_calcjob(self.ctx.banddos_calc)
-            except NotExistent:
-                last_calc_uuid = None
-        else:
-            last_calc_uuid = None
 
         try:  # if something failed, we still might be able to retrieve something
             last_calc_out = self.ctx.banddos_calc.outputs.output_parameters
             retrieved = self.ctx.banddos_calc.outputs.retrieved
-            if 'fleurinpdata' in self.ctx.banddos_calc.inputs:
-                fleurinp = self.ctx.banddos_calc.inputs.fleurinpdata
+            if 'fleurinp' in self.ctx.banddos_calc.inputs:
+                fleurinp = self.ctx.banddos_calc.inputs.fleurinp
             else:
                 fleurinp = get_fleurinp_from_remote_data(self.ctx.banddos_calc.inputs.parent_folder)
             last_calc_out_dict = last_calc_out.get_dict()
         except (NotExistent, AttributeError):
             last_calc_out = None
             last_calc_out_dict = {}
             retrieved = None
@@ -552,26 +545,25 @@
             diff_bandgap = bandgap_scf - bandgap_band
 
         outputnode_dict = {}
 
         outputnode_dict['workflow_name'] = self.__class__.__name__
         outputnode_dict['Warnings'] = self.ctx.warnings
         outputnode_dict['successful'] = self.ctx.successful
-        outputnode_dict['last_calc_uuid'] = last_calc_uuid
         outputnode_dict['mode'] = self.ctx.wf_dict.get('mode')
         outputnode_dict['fermi_energy_band'] = efermi_band
         outputnode_dict['bandgap_band'] = bandgap_band
         outputnode_dict['fermi_energy_scf'] = efermi_scf
         outputnode_dict['bandgap_scf'] = bandgap_scf
         outputnode_dict['diff_efermi'] = diff_efermi
         outputnode_dict['diff_bandgap'] = diff_bandgap
         outputnode_dict['bandgap_units'] = 'eV'
         outputnode_dict['fermi_energy_units'] = 'Htr'
 
-        outputnode_t = Dict(dict=outputnode_dict)
+        outputnode_t = Dict(outputnode_dict)
         if last_calc_out:
             outdict = create_band_result_node(outpara=outputnode_t,
                                               last_calc_out=last_calc_out,
                                               last_calc_retrieved=retrieved)
 
             if self.ctx.wf_dict.get('mode') == 'band' and fleurinp is not None and retrieved is not None:
                 bands = create_aiida_bands_data(fleurinp=fleurinp, retrieved=retrieved)
@@ -581,16 +573,16 @@
                 dos = create_aiida_dos_data(retrieved=retrieved)
                 if isinstance(dos, XyData):
                     outdict['output_banddos_wc_dos'] = dos
 
         else:
             outdict = create_band_result_node(outpara=outputnode_t)
 
-        if retrieved:
-            outdict['last_calc_retrieved'] = retrieved
+        if self.ctx.banddos_calc:
+            self.out_many(self.exposed_outputs(self.ctx.banddos_calc, FleurBaseWorkChain, namespace='banddos_calc'))
 
         #TODO parse Bandstructure
         for link_name, node in outdict.items():
             self.out(link_name, node)
 
     def control_end_wc(self, errormsg):
         """
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/base_fleur.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/base_fleur.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 from aiida.common import AttributeDict
 from aiida.engine import while_
 from aiida.engine.processes.workchains import BaseRestartWorkChain
 from aiida.engine.processes.workchains.utils import process_handler, ProcessHandlerReport
 
 from aiida_fleur.tools.common_fleur_wf import optimize_calc_options
 from aiida_fleur.calculation.fleur import FleurCalculation
+from aiida_fleur.data.fleurinp import get_fleurinp_from_remote_data
 
 
 class FleurBaseWorkChain(BaseRestartWorkChain):
     """Workchain to run a FLEUR calculation with automated error handling and restarts"""
-    _workflowversion = '0.2.0'
+    _workflowversion = '0.2.1'
     _process_class = FleurCalculation
 
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
         spec.expose_inputs(FleurCalculation, exclude=('metadata.options',))
@@ -39,14 +40,15 @@
         spec.input('description', valid_type=str, required=False, non_db=True, help='Calculation description.')
         spec.input('label', valid_type=str, required=False, non_db=True, help='Calculation label.')
         spec.input(
             'add_comp_para',
             valid_type=orm.Dict,
             default=lambda: orm.Dict(dict={
                 'only_even_MPI': False,
+                'forbid_single_mpi': False,
                 'max_queue_nodes': 20,
                 'max_queue_wallclock_sec': 86400
             }),
             help='Gives additional control over computational parameters'
             'only_even_MPI: set to true if you want to suppress odd number of MPI processes in parallelisation.'
             'This might speedup a calculation for machines having even number of sockets per node.'
             'max_queue_nodes: maximal number of nodes allowed on the remote machine. Used only to automatically solve some FLEUR failures.'
@@ -60,15 +62,14 @@
                 cls.run_process,
                 cls.inspect_process,
             ),
             cls.results,
         )
 
         spec.expose_outputs(FleurCalculation)
-        spec.output('final_calc_uuid', valid_type=orm.Str, required=False)
 
         spec.exit_code(311,
                        'ERROR_VACUUM_SPILL_RELAX',
                        message='FLEUR calculation failed because an atom spilled to the'
                        'vacuum during relaxation')
         spec.exit_code(313, 'ERROR_MT_RADII_RELAX', message='Overlapping MT-spheres during relaxation.')
         spec.exit_code(388, 'ERROR_TIME_LIMIT_NO_SOLUTION', message='Computational resources are not optimal.')
@@ -120,56 +121,58 @@
                 self.ctx.use_omp = True
                 self.ctx.suggest_mpi_omp_ratio = self.ctx.num_mpiprocs_per_machine / self.ctx.num_cores_per_mpiproc
             except KeyError:
                 self.ctx.num_cores_per_mpiproc = 1
                 self.ctx.use_omp = False
                 self.ctx.suggest_mpi_omp_ratio = 1
 
-            try:
-                self.check_kpts()
+            status = self.check_kpts()
+            if status is None:
                 self.ctx.can_be_optimised = True
-            except Warning:
+            else:
                 self.report('ERROR: Not optimal computational resources.')
-                return self.exit_codes.ERROR_NOT_OPTIMAL_RESOURCES
+                return status
 
     def check_kpts(self):
         """
         This routine checks if the total number of requested cpus
         is a factor of kpts and makes an optimisation.
 
         If suggested number of num_mpiprocs_per_machine is 60% smaller than
         requested, it throws an exit code and calculation stop withour submission.
         """
-        fleurinp = self.ctx.inputs.fleurinpdata
-        machines = self.ctx.num_machines
-        mpi_proc = self.ctx.num_mpiprocs_per_machine
-        omp_per_mpi = self.ctx.num_cores_per_mpiproc
+        if 'fleurinp' in self.ctx.inputs:
+            fleurinp = self.ctx.inputs.fleurinp
+        else:
+            fleurinp = get_fleurinp_from_remote_data(self.ctx.inputs.parent_folder)
+
         only_even_MPI = self.inputs.add_comp_para['only_even_MPI']
+        forbid_single_mpi = self.inputs.add_comp_para['forbid_single_mpi']
         try:
-            adv_nodes, adv_mpi_tasks, adv_omp_per_mpi, message = optimize_calc_options(machines,
-                                                                                       mpi_proc,
-                                                                                       omp_per_mpi,
-                                                                                       self.ctx.use_omp,
-                                                                                       self.ctx.suggest_mpi_omp_ratio,
-                                                                                       fleurinp,
-                                                                                       only_even_MPI=only_even_MPI)
+            machines, mpi_tasks, omp_threads, message = optimize_calc_options(self.ctx.num_machines,
+                                                                              self.ctx.num_mpiprocs_per_machine,
+                                                                              self.ctx.num_cores_per_mpiproc,
+                                                                              self.ctx.use_omp,
+                                                                              self.ctx.suggest_mpi_omp_ratio,
+                                                                              fleurinp,
+                                                                              only_even_MPI=only_even_MPI,
+                                                                              forbid_single_mpi=forbid_single_mpi)
         except ValueError as exc:
-            raise Warning('Not optimal computational resources, load less than 60%') from exc
+            self.report(exc)
+            return self.exit_codes.ERROR_NOT_OPTIMAL_RESOURCES
 
         self.report(message)
 
-        self.ctx.inputs.metadata.options['resources']['num_machines'] = adv_nodes
-        self.ctx.inputs.metadata.options['resources']['num_mpiprocs_per_machine'] = adv_mpi_tasks
+        self.ctx.inputs.metadata.options['resources']['num_machines'] = machines
+        self.ctx.inputs.metadata.options['resources']['num_mpiprocs_per_machine'] = mpi_tasks
         if self.ctx.use_omp:
-            self.ctx.inputs.metadata.options['resources']['num_cores_per_mpiproc'] = adv_omp_per_mpi
-            if 'environment_variables' in self.ctx.inputs.metadata.options:
-                self.ctx.inputs.metadata.options['environment_variables']['OMP_NUM_THREADS'] = str(adv_omp_per_mpi)
-            else:
+            self.ctx.inputs.metadata.options['resources']['num_cores_per_mpiproc'] = omp_threads
+            if 'environment_variables' not in self.ctx.inputs.metadata.options:
                 self.ctx.inputs.metadata.options['environment_variables'] = {}
-                self.ctx.inputs.metadata.options['environment_variables']['OMP_NUM_THREADS'] = str(adv_omp_per_mpi)
+            self.ctx.inputs.metadata.options['environment_variables']['OMP_NUM_THREADS'] = str(omp_threads)
 
     @process_handler(priority=1,
                      exit_codes=[
                          FleurCalculation.exit_codes.ERROR_FLEUR_CALC_FAILED,
                          FleurCalculation.exit_codes.ERROR_MT_RADII,
                          FleurCalculation.exit_codes.ERROR_NO_RETRIEVED_FOLDER,
                          FleurCalculation.exit_codes.ERROR_OPENING_OUTPUTS,
@@ -193,16 +196,16 @@
         """
         Sometimes relaxation calculation fails with Diraq problem which is usually caused by
         problems with reusing charge density. In this case we resubmit the calculation, dropping the input cdn.
         """
 
         # try to drop remote folder and see if it helps
         is_fleurinp_from_relax = False
-        if 'fleurinpdata' in self.ctx.inputs:
-            if 'relax.xml' in self.ctx.inputs.fleurinpdata.files:
+        if 'fleurinp' in self.ctx.inputs:
+            if 'relax.xml' in self.ctx.inputs.fleurinp.files:
                 is_fleurinp_from_relax = True
 
         if 'parent_folder' in self.ctx.inputs and is_fleurinp_from_relax:
             del self.ctx.inputs.parent_folder
             self.ctx.restart_calc = None
             self.ctx.is_finished = False
             self.report('Calculation seems to fail due to corrupted charge density (can happen'
@@ -242,58 +245,74 @@
     @process_handler(priority=50, exit_codes=FleurCalculation.exit_codes.ERROR_NOT_ENOUGH_MEMORY)
     def _handle_not_enough_memory(self, calculation):
         """
         Calculation failed due to lack of memory.
         Probably works for JURECA only, has to be tested for other systems.
         """
 
-        if self.ctx.can_be_optimised:
-            self.ctx.restart_calc = None
-            self.ctx.is_finished = False
-            self.report('Calculation failed due to lack of memory, I resubmit it with twice larger'
-                        ' amount of computational nodes and smaller MPI/OMP ratio')
-
-            # increase number of nodes
-            propose_nodes = self.ctx.num_machines * 2
-            if propose_nodes > self.ctx.max_queue_nodes:
-                propose_nodes = self.ctx.max_queue_nodes
-            self.ctx.num_machines = propose_nodes
-
-            self.ctx.suggest_mpi_omp_ratio = self.ctx.suggest_mpi_omp_ratio / 2
-            self.check_kpts()
-
-            if 'settings' not in self.ctx.inputs:
-                self.ctx.inputs.settings = {}
-            else:
-                self.ctx.inputs.settings = self.ctx.inputs.settings.get_dict()
-            self.ctx.inputs.settings.setdefault('remove_from_remotecopy_list', [])
-            if 'mixing_history*' not in self.ctx.inputs.settings['remove_from_remotecopy_list']:
-                self.ctx.inputs.settings['remove_from_remotecopy_list'].append('mixing_history*')
-            return ProcessHandlerReport(True)
-        else:
+        if not self.ctx.can_be_optimised:
             self.ctx.restart_calc = calculation
             self.ctx.is_finished = True
             self.report('I am not allowed to optimize your settings. Consider providing at least'
                         'num_machines and num_mpiprocs_per_machine')
             self.results()
             return ProcessHandlerReport(True, self.exit_codes.ERROR_MEMORY_ISSUE_NO_SOLUTION)
 
+        self.ctx.restart_calc = None
+        self.ctx.is_finished = False
+        self.report('Calculation failed due to lack of memory, I resubmit it with twice larger'
+                    ' amount of computational nodes and smaller MPI/OMP ratio')
+
+        # increase number of nodes
+        propose_nodes = self.ctx.num_machines * 2
+        if propose_nodes > self.ctx.max_queue_nodes:
+            propose_nodes = self.ctx.max_queue_nodes
+        self.ctx.num_machines = propose_nodes
+
+        self.ctx.suggest_mpi_omp_ratio = self.ctx.suggest_mpi_omp_ratio / 2
+
+        status = self.check_kpts()
+        if status is not None:
+            self.ctx.is_finished = True
+            self.results()
+            return ProcessHandlerReport(True, self.exit_codes.ERROR_NOT_OPTIMAL_RESOURCES)
+
+        if 'settings' not in self.ctx.inputs:
+            settings = {}
+        else:
+            settings = self.ctx.inputs.settings.get_dict()
+        settings.setdefault('remove_from_remotecopy_list', [])
+        if 'mixing_history*' not in settings['remove_from_remotecopy_list']:
+            settings['remove_from_remotecopy_list'].append('mixing_history*')
+        self.ctx.inputs.settings = orm.Dict(dict=settings)
+
+        #check if the cdn.hdf can be reused
+        #Out of memory can also occur after a couple of iterations if the mixing_history gets too large
+        remote = calculation.base.links.get_outgoing().get_node_by_label('remote_folder')
+        if _is_remote_reusable(self.ctx.inputs, calculation):
+            if 'fleurinp' in self.ctx.inputs:
+                del self.ctx.inputs.fleurinp
+            self.ctx.inputs.parent_folder = remote
+
+        return ProcessHandlerReport(True)
+
     @process_handler(priority=47, exit_codes=FleurCalculation.exit_codes.ERROR_TIME_LIMIT)
     def _handle_time_limits(self, calculation):
         """
         If calculation fails due to time limits, we simply resubmit it.
         """
         from aiida.common.exceptions import NotExistent
 
         # if previous calculation failed for the same reason, do not restart
         try:
-            prev_calculation_remote = calculation.get_incoming().get_node_by_label('parent_folder')
-            prev_calculation_status = prev_calculation_remote.get_incoming().all()[-1].node.exit_status
+            prev_calculation_remote = calculation.base.links.get_incoming().get_node_by_label('parent_folder')
+            prev_calculation_status = prev_calculation_remote.creator.exit_status
             if prev_calculation_status in FleurCalculation.get_exit_statuses(['ERROR_TIME_LIMIT']):
                 self.ctx.is_finished = True
+                self.results()
                 return ProcessHandlerReport(True)
         except NotExistent:
             pass
 
         self.report('FleurCalculation failed due to time limits, I restart it from where it ended')
 
         # increase wallclock time
@@ -304,38 +323,43 @@
 
         # increase number of nodes
         propose_nodes = self.ctx.num_machines * 2
         if propose_nodes > self.ctx.max_queue_nodes:
             propose_nodes = self.ctx.max_queue_nodes
         self.ctx.num_machines = propose_nodes
 
-        remote = calculation.get_outgoing().get_node_by_label('remote_folder')
+        remote = calculation.base.links.get_outgoing().get_node_by_label('remote_folder')
 
         # resubmit providing inp.xml and cdn from the remote folder
         self.ctx.is_finished = False
-        check_remote = False
-
-        if 'fleurinpdata' in self.ctx.inputs:
-            modes = self.ctx.inputs.fleurinpdata.get_fleur_modes()
-            if not (modes['force_theorem'] or modes['dos'] or modes['band']):
-                # in modes listed above it makes no sense copying cdn.hdf
-                self.ctx.inputs.parent_folder = remote
-                del self.ctx.inputs.fleurinpdata
-                check_remote = True
-        else:
-            # it is harder to extract modes in this case - simply try to reuse cdn.hdf and hope it works
+        if _is_remote_reusable(self.ctx.inputs, calculation):
+            if 'fleurinp' in self.ctx.inputs:
+                del self.ctx.inputs.fleurinp
             self.ctx.inputs.parent_folder = remote
-            check_remote = True
-
-        if check_remote:
-            #If no charge density file is available to restart from the calculation will except
-            #with a not nice error message. So we try to catch these cases to produce a nice error message
-            retrieved_filenames = calculation.get_outgoing().get_node_by_label('retrieved').list_object_names()
-            if all(file not in retrieved_filenames for file in (
-                    'cdn_last.hdf',
-                    'cdn1',
-            )):
-                self.report(
-                    'FleurCalculation failed due to time limits and no charge density file is available. Aborting!')
-                return ProcessHandlerReport(True, self.exit_codes.ERROR_TIME_LIMIT_NO_SOLUTION)
 
         return ProcessHandlerReport(True)
+
+
+def _is_remote_reusable(inputs, calculation):
+    """
+    Check whether the remote folder of the given calculation
+    can be resubmitted
+    """
+    can_use_remote = False
+    #If no charge density file is available to restart from the calculation will except
+    #with a not nice error message. So we can only reuse the charge density if these files are available
+    retrieved_filenames = calculation.base.links.get_outgoing().get_node_by_label('retrieved').list_object_names()
+    if any(file in retrieved_filenames for file in (
+            'cdn_last.hdf',
+            'cdn1',
+    )):
+        can_use_remote = True
+
+    if 'fleurinp' in inputs:
+        modes = inputs.fleurinp.get_fleur_modes()
+        if modes['force_theorem'] or modes['dos'] or modes['band']:
+            # in modes listed above it makes no sense copying cdn.hdf
+            can_use_remote = False
+    # without fleurinp it is harder to extract modes in this case
+    # - simply try to reuse cdn.hdf and hope it works
+
+    return can_use_remote
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/base_relax.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/base_relax.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 allows to add scenarios to restart a calculation in an
 automatic way if an expected failure occurred.
 """
 
 from aiida.common import AttributeDict
 from aiida.common.exceptions import ValidationError
 from aiida.engine import while_
-from aiida.orm import load_node, Dict, WorkChainNode
+from aiida.orm import Dict, WorkChainNode
 from aiida.plugins import WorkflowFactory, DataFactory
 from aiida.engine.processes.workchains import BaseRestartWorkChain
 from aiida.engine.processes.workchains.utils import process_handler, ProcessHandlerReport
 
-from aiida_fleur.data.fleurinpmodifier import modify_fleurinpdata
-from aiida_fleur.tools.common_fleur_wf import find_last_submitted_workchain
+from masci_tools.util.schema_dict_util import evaluate_attribute
 
 # pylint: disable=invalid-name
 RelaxProcess = WorkflowFactory('fleur.relax')
 FleurinpData = DataFactory('fleur.fleurinp')
 # pylint: enable=invalid-name
 
 
@@ -124,15 +123,15 @@
                 else:
                     stashed_changes.append(change)
             self.ctx.shift_value_methods_stash = stashed_changes
         else:
             raise ValidationError('Stashed methods are not used and fixing_methods is not empty')
 
         wf_param['inpxml_changes'] = new_changes
-        self.ctx.inputs.scf.wf_parameters = Dict(dict=wf_param)
+        self.ctx.inputs.scf.wf_parameters = Dict(wf_param)
 
     # @process_handler(priority=50, exit_codes=RelaxProcess.exit_codes.ERROR_DID_NOT_RELAX)
     # def _handle_not_conv_error(self, calculation):
     #     """
     #     Calculation failed for unknown reason.
     #     """
 
@@ -167,27 +166,26 @@
         """
         SCF can be switched to BFGS. For now cdn and relax.xml are kept because the current progress is
         treated as successful.
         """
 
         self.ctx.is_finished = False
         self.report('It is time to switch from straight to BFGS relaxation')
-        last_scf_calc = load_node(calculation.outputs.output_relax_wc_para.get_dict()['last_scf_wc_uuid'])
-        remote = last_scf_calc.outputs.last_calc.remote_folder
+        remote = calculation.outputs.last_scf.last_calc.remote_folder
         if 'wf_parameters' in self.ctx.inputs:
             parameters = self.ctx.inputs.wf_parameters
             run_final = parameters.get_dict().get('run_final_scf', False)
         else:
             run_final = False
 
         self.ctx.inputs.scf.remote_data = remote
 
         scf_para = self.ctx.inputs.scf.wf_parameters.get_dict()
         scf_para['force_dict']['forcemix'] = 'BFGS'
-        self.ctx.inputs.scf.wf_parameters = Dict(dict=scf_para)
+        self.ctx.inputs.scf.wf_parameters = Dict(scf_para)
 
         if 'structure' in self.ctx.inputs.scf:
             del self.ctx.inputs.scf.structure
         if 'inpgen' in self.ctx.inputs.scf:
             if run_final:
                 self.ctx.inputs.final_scf.inpgen = self.ctx.inputs.scf.inpgen
             del self.ctx.inputs.scf.inpgen
@@ -236,15 +234,15 @@
 
         self.ctx.is_finished = False
         self.report('Relax WC failed because atom was spilled to the vacuum, I change the vacuum parameter')
 
         wf_para_dict = self.ctx.inputs.scf.wf_parameters.get_dict()
         if wf_para_dict['force_dict']['forcemix'] != self.ctx.initial_mixing:
             wf_para_dict['force_dict']['forcemix'] = self.ctx.initial_mixing
-            self.ctx.inputs.scf.wf_parameters = Dict(dict=wf_para_dict)
+            self.ctx.inputs.scf.wf_parameters = Dict(wf_para_dict)
 
         self.ctx.use_stashed_shift_methods = True
         self.ctx.fixing_methods = [('shift_value', {'change_dict': {'dTilda': 0.2, 'dVac': 0.2}})]
 
         return ProcessHandlerReport(True)
 
     @process_handler(priority=101, exit_codes=RelaxProcess.exit_codes.ERROR_MT_RADII_RELAX)
@@ -260,46 +258,34 @@
                 self.ctx.inputs.scf.fleurinp = inputs
             else:
                 self.ctx.inputs.scf.structure = inputs[0]
                 self.ctx.inputs.scf.inpgen = inputs[1]
                 if len(inputs) == 3:
                     self.ctx.inputs.scf.calc_parameters = inputs[2]
 
-        last_scf_wc_uuid = calculation.outputs.output_relax_wc_para.get_dict()['last_scf_wc_uuid']
-        last_scf = load_node(last_scf_wc_uuid)
-        error_params = last_scf.outputs.last_calc.error_params.get_dict()
+        error_params = calculation.outputs.last_scf.last_calc.error_params.get_dict()
         label1 = int(error_params['overlapped_indices'][0])
         label2 = int(error_params['overlapped_indices'][1])
         value = -(float(error_params['overlaping_value']) + 0.01) / 2
 
         self.ctx.is_finished = False
         self.report('Relax WC failed because MT overlapped during relaxation. Try to fix this')
         wf_para_dict = self.ctx.inputs.scf.wf_parameters.get_dict()
 
-        relax_wc = load_node(find_last_submitted_workchain(self.node))
-        scf_wc = load_node(find_last_submitted_workchain(relax_wc))
-        mixing = ''
-        for link in scf_wc.get_outgoing().all():
-            try:
-                if link.node.process_class is modify_fleurinpdata:
-                    tasks = link.node.inputs.modifications.get_dict()['tasks']
-                    for task in tasks:
-                        try:
-                            mixing = task[1][0]['forcemix']
-                        except (IndexError, KeyError):
-                            pass
-            except AttributeError:
-                pass
+        xmltree, schema_dict = calculation.outputs.last_scf.fleurinp.load_inpxml()
+        mixing = evaluate_attribute(xmltree, schema_dict, 'forcemix', optional=True)
+        if not mixing:
+            mixing = 'BFGS'
 
         if value < -0.2 and error_params['iteration_number'] >= 3 and mixing == 'BFGS':
             self.ctx.initial_mixing = 'straight'
 
             self_wf_para = self.ctx.inputs.wf_parameters.get_dict()
             self_wf_para['change_mixing_criterion'] = self_wf_para['change_mixing_criterion'] / 1.4
-            self.ctx.inputs.wf_parameters = Dict(dict=self_wf_para)
+            self.ctx.inputs.wf_parameters = Dict(self_wf_para)
             self.report('Seems it is too early for BFGS. I switch back to straight mixing'
                         ' and reduce change_mixing_criterion by a factor of 1.25')
         elif error_params['iteration_number'] == 2:
             wf_para_dict['force_dict']['forcealpha'] = wf_para_dict['force_dict']['forcealpha'] / 2
             self.report('forcealpha might be too large.')
         else:  # reduce MT radii
             self.report('MT radii might be too large. I reduce them.')
@@ -318,15 +304,15 @@
                 'mode': 'abs'
             }))
 
         self.ctx.use_stashed_shift_methods = True  # even if we set mixing only, calculation should restart from scratch
 
         if wf_para_dict['force_dict']['forcemix'] != self.ctx.initial_mixing:
             wf_para_dict['force_dict']['forcemix'] = self.ctx.initial_mixing
-            self.ctx.inputs.scf.wf_parameters = Dict(dict=wf_para_dict)
+            self.ctx.inputs.scf.wf_parameters = Dict(wf_para_dict)
 
         return ProcessHandlerReport(True)
 
 
 def find_inputs_relax(remote_node):
     """
     Finds the original inputs of the relaxation workchain which can be either
@@ -343,11 +329,12 @@
     if 'remote_data' in scf_wc_node.inputs:
         return find_inputs_relax(scf_wc_node.inputs.remote_data)
 
     if 'structure' in scf_wc_node.inputs:
         if 'calc_parameters' in scf_wc_node.inputs:
             return scf_wc_node.inputs.structure, scf_wc_node.inputs.inpgen, scf_wc_node.inputs.calc_parameters
         return scf_wc_node.inputs.structure, scf_wc_node.inputs.inpgen
-    elif 'fleurinp' in scf_wc_node.inputs:
+
+    if 'fleurinp' in scf_wc_node.inputs:
         return scf_wc_node.inputs.fleurinp
 
     raise ValueError('Did not find original inputs for Relax WC')
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/cfcoeff.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/cfcoeff.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from aiida.common import AttributeDict
 from aiida.common.exceptions import NotExistent
 from aiida import orm
 from aiida.common.constants import elements as PeriodicTableElements
 
 from aiida_fleur.tools.StructureData_util import replace_element, mark_atoms, get_atomtype_site_symmetry
 from aiida_fleur.tools.common_fleur_wf import get_inputs_fleur
-from aiida_fleur.data.fleurinpmodifier import FleurinpModifier
+from aiida_fleur.data.fleurinpmodifier import FleurinpModifier, inpxml_changes
 from aiida_fleur.calculation.fleur import FleurCalculation
 
 from aiida_fleur.workflows.scf import FleurScfWorkChain
 from aiida_fleur.workflows.base_fleur import FleurBaseWorkChain
 from aiida_fleur.workflows.orbcontrol import FleurOrbControlWorkChain
 
 from masci_tools.tools.cf_calculation import CFCalculation, CFCoefficient
@@ -206,30 +206,31 @@
             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
         inputs = self.inputs
         if 'scf' not in inputs and 'orbcontrol' not in inputs:
             error = 'ERROR: Missing input. Provide one of the scf or orbcontrol inputs.'
             self.report(error)
             return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
-        elif 'scf' in inputs and 'orbcontrol' in inputs:
+
+        if 'scf' in inputs and 'orbcontrol' in inputs:
             error = 'ERROR: Invalid Input. Provide only one of the scf or orbcontrol inputs.'
             self.report(error)
             return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
 
         element = self.ctx.wf_dict['element']
         atomic_numbers = {data['symbol']: num for num, data in PeriodicTableElements.items()}
         if element not in atomic_numbers:
             error = f'ERROR: Invalid Input. Element not a valid element: {element}'
             self.report(error)
             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
-        else:
-            if atomic_numbers[element] < 57 and atomic_numbers[element] > 70:
-                error = 'ERROR: Invalid Input. CF coefficient workflow only implemented for 4f rare-earths'
-                self.report(error)
-                return self.exit_codes.ERROR_INVALID_INPUT_PARAM
+
+        if atomic_numbers[element] < 57 and atomic_numbers[element] > 70:
+            error = 'ERROR: Invalid Input. CF coefficient workflow only implemented for 4f rare-earths'
+            self.report(error)
+            return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
     def run_scfcalculations(self):
 
         self.report('INFO: Starting SCF calculations')
         inputs = {}
         calcs = {}
         if self.ctx.wf_dict['rare_earth_analogue']:
@@ -317,23 +318,16 @@
 
             if self.ctx.wf_dict['soc_off']:
                 if 'wf_parameters' not in inputs_analogue:
                     scf_wf_dict = {}
                 else:
                     scf_wf_dict = inputs_analogue.wf_parameters.get_dict()
 
-                scf_wf_dict.setdefault('inpxml_changes', []).append(('set_species', {
-                    'attributedict': {
-                        'special': {
-                            'socscale': 0.0
-                        }
-                    },
-                    'species_name':
-                    f"all-{self.ctx.wf_dict['analogue_element']}"
-                }))
+                with inpxml_changes(scf_wf_dict) as fm:
+                    fm.set_species(f"all-{self.ctx.wf_dict['analogue_element']}", {'special': {'socscale': 0}})
 
             inputs_analogue.wf_parameters = orm.Dict(dict=scf_wf_dict)
             inputs_analogue.metadata.call_link_label = f'analogue_scf_{index}'
             inputs[f'analogue_scf_{index}'] = inputs_analogue
 
         return inputs
 
@@ -342,23 +336,16 @@
         input_scf = AttributeDict(self.exposed_inputs(FleurScfWorkChain, namespace='scf'))
 
         if self.ctx.wf_dict['soc_off']:
             if 'wf_parameters' not in input_scf:
                 scf_wf_dict = {}
             else:
                 scf_wf_dict = input_scf.wf_parameters.get_dict()
-
-            scf_wf_dict.setdefault('inpxml_changes', []).append(('set_species', {
-                'species_name': f"all-{self.ctx.wf_dict['element']}",
-                'attributedict': {
-                    'special': {
-                        'socscale': 0.0
-                    }
-                }
-            }))
+            with inpxml_changes(scf_wf_dict) as fm:
+                fm.set_species(f"all-{self.ctx.wf_dict['element']}", {'special': {'socscale': 0}})
 
             input_scf.wf_parameters = orm.Dict(dict=scf_wf_dict)
         input_scf.metadata.call_link_label = 'rare_earth_scf'
 
         return input_scf
 
     def get_inputs_orbcontrol(self):
@@ -367,38 +354,26 @@
 
         if self.ctx.wf_dict['soc_off'] and 'scf_no_ldau' in input_orbcontrol:
             if 'wf_parameters' not in input_orbcontrol['scf_no_ldau']:
                 scf_wf_dict = {}
             else:
                 scf_wf_dict = input_orbcontrol['scf_no_ldau'].wf_parameters.get_dict()
 
-            scf_wf_dict.setdefault('inpxml_changes', []).append(('set_species', {
-                'species_name': f"all-{self.ctx.wf_dict['element']}",
-                'attributedict': {
-                    'special': {
-                        'socscale': 0.0
-                    }
-                }
-            }))
+            with inpxml_changes(scf_wf_dict) as fm:
+                fm.set_species(f"all-{self.ctx.wf_dict['element']}", {'special': {'socscale': 0}})
 
             input_orbcontrol.scf_no_ldau.wf_parameters = orm.Dict(dict=scf_wf_dict)
         elif self.ctx.wf_dict['soc_off']:
             if 'wf_parameters' not in input_orbcontrol:
                 orbcontrol_wf_dict = {}
             else:
                 orbcontrol_wf_dict = input_orbcontrol.wf_parameters.get_dict()
 
-            orbcontrol_wf_dict.setdefault('inpxml_changes', []).append(('set_species', {
-                'species_name': f"all-{self.ctx.wf_dict['element']}",
-                'attributedict': {
-                    'special': {
-                        'socscale': 0.0
-                    }
-                }
-            }))
+            with inpxml_changes(orbcontrol_wf_dict) as fm:
+                fm.set_species(f"all-{self.ctx.wf_dict['element']}", {'special': {'socscale': 0}})
 
             input_orbcontrol.wf_parameters = orm.Dict(dict=orbcontrol_wf_dict)
         input_orbcontrol.metadata.call_link_label = 'rare_earth_orbcontrol'
 
         return input_orbcontrol
 
     def run_cfcalculation(self):
@@ -493,15 +468,15 @@
             if 'options' in inputs:
                 options = inputs.options.get_dict()
             else:
                 options = {}
 
             fm = FleurinpModifier(fleurinp_scf)
 
-            fm.set_atomgroup(attributedict={'cFCoeffs': {
+            fm.set_atomgroup({'cFCoeffs': {
                 'chargeDensity': False,
                 'potential': True
             }},
                              species=f"all-{self.ctx.wf_dict['analogue_element']}")
 
             try:
                 fm.show(display=False, validate=True)
@@ -560,22 +535,18 @@
         else:
             description = 'Calculation of crystal field potential/charge density'
 
         fm = FleurinpModifier(fleurinp_scf)
         element = self.ctx.wf_dict['element']
         if self.ctx.wf_dict['rare_earth_analogue']:
             #Only charge density
-            fm.set_atomgroup(attributedict={'cFCoeffs': {
-                'chargeDensity': True,
-                'potential': False
-            }},
-                             species=f'all-{element}')
+            fm.set_atomgroup({'cFCoeffs': {'chargeDensity': True, 'potential': False}}, species=f'all-{element}')
         else:
             #Both potential and charge density
-            fm.set_atomgroup(attributedict={'cFCoeffs': {
+            fm.set_atomgroup({'cFCoeffs': {
                 'chargeDensity': True,
                 'potential': True,
                 'remove4f': True
             }},
                              species=f'all-{element}')
 
         try:
@@ -650,15 +621,15 @@
 
         #This calculation is always there
         success = self.check_cf_calculation('rare_earth_cf')
         if success:
             link_label = 'rare_earth_cf'
             outnodedict[link_label] = self.ctx.rare_earth_cf.outputs.output_parameters
             cdn_retrieved = self.ctx.rare_earth_cf.outputs.retrieved
-            xmltree, schema_dict = self.ctx.rare_earth_cf.inputs.fleurinpdata.load_inpxml()
+            xmltree, schema_dict = self.ctx.rare_earth_cf.inputs.fleurinp.load_inpxml()
 
             groups = eval_simple_xpath(xmltree, schema_dict, 'atomGroup', list_return=True)
             atomTypes = []
             for index, group in enumerate(groups):
                 if tag_exists(group, schema_dict, 'cfcoeffs'):
                     atomTypes.append(index + 1)
 
@@ -685,15 +656,15 @@
                     calc_name = f'analogue_cf_{index}'
                     success = self.check_cf_calculation(calc_name)
                     if not success:
                         continue
                     pot_retrieved = self.ctx[calc_name].outputs.retrieved
                     outnodedict[link_label] = self.ctx[calc_name].outputs.output_parameters
 
-                    xmltree, schema_dict = self.ctx[calc_name].inputs.fleurinpdata.load_inpxml()
+                    xmltree, schema_dict = self.ctx[calc_name].inputs.fleurinp.load_inpxml()
                     groups = eval_simple_xpath(xmltree, schema_dict, 'atomGroup', list_return=True)
                     atomTypes = []
                     for group_index, group in enumerate(groups):
                         if tag_exists(group, schema_dict, 'cfcoeffs'):
                             atomTypes.append(group_index + 1)
 
                     cf_calc_out_analogue = calculate_cf_coefficients(cdn_retrieved,
@@ -744,15 +715,15 @@
                 _, cf_calc_out['cf_coefficients_spin_up_imag'] = cf_calc_out['cf_coefficients_spin_up_imag'].popitem()
                 _, cf_calc_out['cf_coefficients_spin_down_imag'] = cf_calc_out[
                     'cf_coefficients_spin_down_imag'].popitem()
 
         rare_earth_site_symmetries = []
         if success and len(cf_calc_out['cf_coefficients_atomtypes']) > 0:
             #For this to work the order of the atomtype CANNOT change between the conversions
-            struc = self.ctx.rare_earth_cf.inputs.fleurinpdata.get_structuredata_ncf()
+            struc = self.ctx.rare_earth_cf.inputs.fleurinp.get_structuredata_ncf()
             site_symmetries = get_atomtype_site_symmetry(struc)
             rare_earth_site_symmetries = [
                 site_symmetries[atomtype - 1] for atomtype in cf_calc_out['cf_coefficients_atomtypes']
             ]
 
         out = {
             'workflow_name': self.__class__.__name__,
@@ -1010,29 +981,29 @@
     cdn_data.description = ('Contains XyData for the Charge density used in the crystal field calculation')
 
     pot_data = orm.XyData()
     pot_data.set_x(potentials_rmesh, 'rmesh', x_units='Bohr')
 
     y_names, y_arrays = zip(*potentials.items())
     y_units = ['htr'] * len(y_names)
-    pot_data.set_y(y_arrays, y_names, y_units=y_units)
+    pot_data.set_y([d.real for d in y_arrays], y_names, y_units=y_units)
 
     pot_data.label = 'cfcoeff_pot_data'
     pot_data.description = ('Contains XyData for the Poteintials used in the crystal field calculation')
 
     return {'out': out_dict, 'charge_densities': cdn_data, 'potentials': pot_data}
 
 
 def _calculate_single_atomtype(cf_cdn_folder, cf_pot_folder, convert, **kwargs):
     """
     Private method wrapping the calculation of coefficients
     """
     CRYSTAL_FIELD_FILE = FleurCalculation._CFDATA_HDF5_FILE_NAME
 
-    cfcalc = CFCalculation(quiet=True)
+    cfcalc = CFCalculation()
     #Reading in the HDF files
     if CRYSTAL_FIELD_FILE in cf_cdn_folder.list_object_names():
         try:
             with cf_cdn_folder.open(CRYSTAL_FIELD_FILE, 'rb') as f:
                 with h5py.File(f, 'r') as cffile:
                     cfcalc.read_charge_density(cffile, **kwargs)
         except ValueError as exc:
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/corehole.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/corehole.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from aiida_fleur.tools.StructureData_util import break_symmetry
 from aiida_fleur.tools.StructureData_util import find_equi_atoms
 from aiida_fleur.tools.element_econfig_list import get_econfig, get_coreconfig
 from aiida_fleur.tools.element_econfig_list import econfigstr_hole, states_spin
 from aiida_fleur.tools.element_econfig_list import get_state_occ, highest_unocc_valence
 from aiida_fleur.tools.dict_util import dict_merger, extract_elementpara
 from aiida_fleur.data.fleurinp import FleurinpData
+from aiida_fleur.data.fleurinpmodifier import inpxml_changes
 
 
 class FleurCoreholeWorkChain(WorkChain):
     """
     Turn key solution for a corehole calculation with the FLEUR code.
     Has different protocols for different core-hole types (valence, charge).
 
@@ -214,15 +215,26 @@
         # input variables
         inputs = self.inputs
         if 'calc_parameters' in inputs:
             self.ctx.ref_para = inputs.get('calc_parameters')
         else:
             self.ctx.ref_para = None
 
-        wf_dict = inputs.wf_parameters.get_dict()
+        wf_default = self._default_wf_para
+        if 'wf_parameters' in self.inputs:
+            wf_dict = self.inputs.wf_parameters.get_dict()
+        else:
+            wf_dict = wf_default
+
+        for key, val in wf_default.items():
+            if isinstance(val, dict):
+                wf_dict[key] = {**val, **wf_dict.get(key, {})}
+            else:
+                wf_dict[key] = wf_dict.get(key, val)
+
         self.ctx.method = wf_dict.get('method', 'valence')
         self.ctx.joblimit = wf_dict.get('joblimit')
         self.ctx.add_comp_para = wf_dict['add_comp_para']
         self.ctx.same_para = wf_dict.get('same_para')
         self.ctx.scf_para = wf_dict.get('scf_para', {})
         self.ctx.be_to_calc = wf_dict.get('corelevel')
         self.ctx.atoms_to_calc = wf_dict.get('atoms')
@@ -390,15 +402,15 @@
             hole_charge = self.ctx.hole_charge
             correct_val_charge = False  # the routines add the electron per default to the valence
 
         ##########
         # 1. Find out what atoms to put coreholes on
         self.report(f'Atoms to calculate : {atoms_toc}')
         for atom_info in atoms_toc:
-            if isinstance(atom_info, str):  # , six.text_type)):  #basestring):
+            if isinstance(atom_info, str):
                 if atom_info == 'all':
                     # add all symmetry equivivalent atoms of structure to create coreholes
                     #coreholes_atoms = base_atoms_sites
                     coreholes_atoms = []
                     for equi_group in equi_info_symbol:
                         # only calculate first element of group, 0 entry is an element string
                         # and there is always a first atom element
@@ -446,15 +458,15 @@
         dict_corelevel = {}
         # dict_corelevel['W' : {corelevel: ['1s 1/2','4f 7/2', '4f 3/2'], econfig: [config], fleur_changes : []}]
 
         #########
         # 2. now check what type of corelevel shall we create on those atoms
         self.report(f'Corelevels to calculate : {corelevels_toc}')
         for corel in corelevels_toc:
-            if isinstance(corel, str):  # , six.text_type)):  #basestring):
+            if isinstance(corel, str):
                 # split string (Be1s) s.replace(';',' ')... could get rid of re
                 elm_cl = re.split('[, ;:-]', corel)
                 #print(elm_cl)
                 if len(elm_cl) != 2:
                     # something went wrong, wrong input
                     # TODO log, error and hint
                     error = (f'ERROR: corelevel was given in the wrong format: {elm_cl},'
@@ -545,69 +557,52 @@
                     #print(cl_dict.get('corelevel')[i])
                     #print(cl_dict.get('valence')[i])
                     #print(econfig)
                     state_tag_list = get_state_occ(econfig,
                                                    corehole=cl_dict.get('corelevel')[i],
                                                    valence=cl_dict.get('valence')[i],
                                                    ch_occ=hole_charge)
-                    attributedict = {'electronConfig': {'stateOccupation': state_tag_list}}
-                    #pprint(state_tag_list)
-                    change = ('set_species', {
-                        'species_name': change_kind,
-                        'attributedict': attributedict,
-                        'create': False
-                    })
-                    fleurinp_change.append(change)
-                    if correct_val_charge:  # only needed in certain methods
-                        charge_change = (
-                            'add_number_to_first_attrib',
-                            {
-                                'attributename': 'valenceElectrons',
-                                'add_number': -1.0,  #-hole_charge,  #one electron was added by inpgen, we remove it
-                                'mode': 'abs',
-                            })
-                        fleurinp_change.append(charge_change)
-                    elif hole_charge != 1.0:  # fractional valence hole
-                        charge_change = (
-                            'add_number_to_first_attrib',
-                            {
-                                'attributename': 'valenceElectrons',
-                                'add_number': -1.0 + hole_charge,  # one electron was already added by inpgen
-                                'mode': 'abs',
-                            })
-                        fleurinp_change.append(charge_change)
-                    if self.ctx.magnetic:  # Do a collinear magnetic calculation
-                        charge_change = ('set_inpchanges', {'change_dict': {'jspins': 2}})
-                        fleurinp_change.append(charge_change)
-                    #self.report('{}'.format(fleurinp_change))
-                    # because there might be already some kinds and another number is right...
-                    # repacking of sites, because input to a calcfunction, otherwise not storeable...
                     corehole = {
                         'site': {
                             'kind_name': kind,  #site.kind_name,
                             'position': site.position
                         },
                         'econfig': econfig,
                         'kindname': change_kind,
-                        'inpxml_changes': fleurinp_change
                     }
+                    with inpxml_changes(corehole) as fm:
+                        fm.set_species(change_kind, {'electronConfig': {'stateOccupation': state_tag_list}})
+
+                        if correct_val_charge:  # only needed in certain methods
+                            fm.add_number_to_first_attrib('valenceElectrons', -1, mode='abs')
+                        elif hole_charge != 1.0:  # fractional valence hole
+                            # one electron was already added by inpgen
+                            fm.add_number_to_first_attrib('valenceElectrons', -1 + hole_charge, mode='abs')
+
+                        if self.ctx.magnetic:  # Do a collinear magnetic calculation
+                            fm.set_inpchanges({'jspins': 2})
+
+                    #self.report('{}'.format(fleurinp_change))
+                    # because there might be already some kinds and another number is right...
+                    # repacking of sites, because input to a calcfunction, otherwise not storeable...
+
                     corehole_to_create.append(corehole)
 
         #state_tag_list = get_state_occ(econfigstr, corehole = '', valence = '', ch_occ = 1.0):
 
         # lesson go over site position to get atom in supercell
         # set econfig for this atom in the supercell
         # (default kind name = element + id) use this for paramter settings
 
         # fill calcs_torun with (sturcutre, parameter, wf_para)
         #corehole_to_create = [{'site' : sites[8], 'kindname' : 'W1', 'econfig': "[Kr] 5s2 4d10 4f13 | 5p6 5d5 6s2", 'fleurinp_change' : []}]
         calcs = []
         for corehole in corehole_to_create:
             para = self.ctx.ref_para
-            wf_para = Dict(dict=corehole)
+            wf_para = Dict(corehole)
             #print(corehole)
             #print(base_supercell)
             #print(para)
             # all these steps can be calcfunctions, we have grouped them all in one
             ret_dict = prepare_struc_corehole_wf(base_supercell, wf_para, para)
             moved_struc = ret_dict['moved_struc']
             calc_para = ret_dict['hole_para']
@@ -621,15 +616,15 @@
                 wf_parameter = {}
             else:
                 wf_parameter = para
             #print(wf_parameter)
             wf_parameter['add_comp_para'] = self.ctx.add_comp_para
             wf_parameter['inpxml_changes'] = corehole['inpxml_changes']
 
-            wf_parameters = Dict(dict=wf_parameter)
+            wf_parameters = Dict(wf_parameter)
             calcs.append([moved_struc, calc_para, wf_parameters])
         self.ctx.calcs_torun = calcs
         #print('ctx.calcs_torun {}'.format(self.ctx.calcs_torun))
         #self.report('INFO: end of create coreholes')
 
     '''
     def run_scf2(self):
@@ -666,16 +661,16 @@
         print('INFO: In run_ref_scf FleurCoreholeWorkChain')
         para = self.ctx.scf_para
         if para is None:
             wf_parameter = {}
         else:
             wf_parameter = para
         wf_parameter['add_comp_para'] = self.ctx.add_comp_para
-        wf_parameters = Dict(dict=wf_parameter)
-        options = Dict(dict=self.ctx.options)
+        wf_parameters = Dict(wf_parameter)
+        options = Dict(self.ctx.options)
         '''
         #res_all = []
         calcs = {}
 
         i = 0
         for node in self.ctx.calcs_ref_torun: # usually just 1, but we leave the default.
             #print(node)
@@ -812,16 +807,16 @@
         if para is None:
             wf_parameter = {}
         else:
             wf_parameter = para
         wf_parameter['add_comp_para'] = self.ctx.add_comp_para
         #wf_parameter['queue_name'] = self.ctx.queue
         #wf_parameter['custom_scheduler_commands'] = self.ctx.custom_scheduler_commands
-        wf_parameters = Dict(dict=wf_parameter)
-        options = Dict(dict=self.ctx.options)
+        wf_parameters = Dict(wf_parameter)
+        options = Dict(self.ctx.options)
         #res_all = []
         calcs = {}
         scf_label = 'FleurCoreholeWorkChain cell'
         scf_desc = '|FleurCoreholeWorkChain|'
         # now in parallel
         #print self.ctx.ref_calcs_torun
         i = 0  #
@@ -994,30 +989,30 @@
         outputnode_dict['bandgap_units'] = 'eV'
         outputnode_dict['reference_bandgaps'] = self.ctx.ref_bandgaps
         outputnode_dict['atomtypes'] = self.ctx.atomtypes
         outputnode_dict['warnings'] = self.ctx.warnings
         outputnode_dict['errors'] = self.ctx.errors
         outputnode_dict['hints'] = self.ctx.hints
 
-        outputnode = Dict(dict=outputnode_dict)
+        outputnode = Dict(outputnode_dict)
         outdict = {}
         outdict['output_corehole_wc_para'] = outputnode
 
         # To have to ouput node linked to the calculation output nodes
         outnodedict = {}
-        outnode = Dict(dict=outputnode_dict)
+        outnode = Dict(outputnode_dict)
         outnodedict['results_node'] = outnode
 
         # TODO: bad design, make bullet proof.
         for i, label in enumerate(self.ctx.labels):
             calc = self.ctx[label]
             #print(calc)
             #print(calc.get_outgoing().all())
             try:
-                calc_dict = calc.get_outgoing().get_node_by_label(
+                calc_dict = calc.base.links.get_outgoing().get_node_by_label(
                     'output_scf_wc_para')  #calc.outputs.output_scf_wc_para
             except (KeyError, ValueError):
                 print('continue 2')
             outnodedict[label] = calc_dict
 
         outdict = create_corehole_result_node(**outnodedict)
 
@@ -1087,19 +1082,21 @@
     species_name = wf_para_dict['kindname']
     broke_kn = site_info['kind_name']
     new_kinds_names = {broke_kn: [species_name]}
     #print pos
     npos = -np.array(pos)
 
     # break the symmetry, make corehole atoms its own species. # pos has to be tuple, unpack problem here.. #TODO rather not so nice
-    inputs = dict(structure=base_supercell,
-                  atoms=[],
-                  site=[],
-                  pos=[(pos[0], pos[1], pos[2])],
-                  new_kinds_names=new_kinds_names)
+    inputs = {
+        'structure': base_supercell,
+        'atoms': [],
+        'site': [],
+        'pos': [(pos[0], pos[1], pos[2])],
+        'new_kinds_names': new_kinds_names
+    }
     if para is not None:
         inputs['parameterdata'] = para
     new_struc, new_para = break_symmetry(**inputs)
     #kinds = new_struc.kinds
     #for kind in kinds:
     #    if kind.name == broke_kn:
     #        kind.name = species_name
@@ -1125,19 +1122,19 @@
 
     params: calcs : list of scf workchains nodes
     """
     # TODO maybe import from somewhere move to common wf
 
     calc_uuids = []
     for calc in calcs:
-        print(calc)
-        print(calc.exit_status, calc.exit_message)
-        print(calc.get_outgoing().all())
+        # print(calc)
+        # print(calc.exit_status, calc.exit_message)
+        # print(calc.get_outgoing().all())
         try:
-            calc_uuid = calc.outputs.output_scf_wc_para.get_dict()['last_calc_uuid']
+            calc_uuid = calc.outputs.last_calc.remote_folder.creator.uuid
         except (KeyError, AttributeError):
             print('continue')
             continue
         if calc_uuid is not None:
             calc_uuids.append(calc_uuid)
     #print(calc_uuids)
 
@@ -1159,21 +1156,17 @@
         calc = load_node(uuid)
         if not isinstance(calc, CalcJobNode):
             #raise ValueError("Calculation with pk {} must be a FleurCalculation".format(pk))
             # log and continue
             continue
         if calc.is_finished_ok:
             # get out.xml file of calculation
-            #outxml = calc.outputs.retrieved.folder.get_abs_path('path/out.xml')
-            outxml = calc.outputs.retrieved.open('out.xml')
-            #print outxml
-            try:
+            with calc.outputs.retrieved.open('out.xml', 'rb') as outxml:
                 corelevels, atomtypes = extract_corelevels(outxml)
-            finally:
-                outxml.close()
+
             #all_corelevels.append(core)
             #print('corelevels: {}'.format(corelevels))
             #print('atomtypes: {}'.format(atomtypes))
             #for i in range(0,len(corelevels[0][0]['corestates'])):
             #    print corelevels[0][0]['corestates'][i]['energy']
 
             #TODO how to store?
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/create_magnetic_film.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/create_magnetic_film.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
                                'populate_defaults': False
                            },
                            namespace='relax',
                            exclude=('structure',))
         spec.input('wf_parameters', valid_type=Dict, required=False)
         spec.input('eos_output', valid_type=Dict, required=False)
         spec.input('optimized_structure', valid_type=StructureData, required=False)
+        spec.input('interlayer_dist', valid_type=Dict, required=False)
         spec.input('distance_suggestion', valid_type=Dict, required=False)
 
         spec.outline(cls.start,
                      if_(cls.eos_needed)(cls.run_eos,),
                      if_(cls.relax_needed)(cls.run_relax,), cls.make_magnetic)
 
         spec.output('magnetic_structure', valid_type=StructureData)
@@ -268,18 +269,23 @@
             else:
                 try:
                     eos_output = self.ctx.eos_wc.outputs.output_eos_wc_para
                 except NotExistent:
                     return self.exit_codes.ERROR_EOS_FAILED
             # print(eos_output.get_dict())
             scaling_param = eos_output.get_dict()['scaling_gs']
-
+            if 'interlayer_dist' in self.inputs:
+                ild = self.inputs.interlayer_dist
+            else:
+                ild = None
             out_create_structure = create_film_to_relax(wf_dict_node=Dict(dict=self.ctx.wf_dict),
                                                         scaling_parameter=Float(scaling_param),
-                                                        suggestion_node=self.inputs.distance_suggestion)
+                                                        suggestion_node=self.inputs.distance_suggestion,
+                                                        ild=ild)
+
             inputs.scf.structure = out_create_structure['structure']
             substrate = out_create_structure['substrate']
             # TODO: error handling might be needed
             self.ctx.substrate = substrate.uuid  # can not store aiida data nodes directly in ctx.
 
             if not isinstance(inputs.scf.structure, StructureData):
                 return inputs, inputs.scf.structure
@@ -379,15 +385,15 @@
                                   latticeconstant=latticeconstant,
                                   size=size)
 
     return StructureData(ase=structure)
 
 
 @cf
-def create_film_to_relax(wf_dict_node, scaling_parameter, suggestion_node):
+def create_film_to_relax(wf_dict_node, scaling_parameter, suggestion_node, ild=None):
     """
     Create a film structure those interlayers will be relaxed.
     """
     from aiida_fleur.tools.StructureData_util import create_manual_slab_ase, center_film
     from aiida_fleur.tools.StructureData_util import adjust_film_relaxation, adjust_sym_film_relaxation
     from aiida_fleur.tools.StructureData_util import mark_fixed_atoms, has_z_reflection
     from aiida_fleur.tools.StructureData_util import define_AFM_structures
@@ -441,20 +447,28 @@
                                            host_symbol=host_symbol,
                                            latticeconstant=latticeconstant,
                                            size=(2, 2, 2),
                                            replacements=None,
                                            decimals=decimals)
 
     bond_length = find_min_distance_unary_structure(tmp_substrate)
-
+    if ild is None:
+        ILD = None
+    else:
+        ILD = ild.get_dict()
     suggestion = suggestion_node.get_dict()
 
     if adjustment_needed:
         if has_z_reflection(structure):
-            structure = adjust_sym_film_relaxation(structure, suggestion, host_symbol, bond_length, last_layer_factor)
+            if ild is not None:
+                structure = adjust_sym_film_relaxation(structure, suggestion, host_symbol, bond_length,
+                                                       last_layer_factor, ILD)
+            else:
+                structure = adjust_sym_film_relaxation(structure, suggestion, host_symbol, bond_length,
+                                                       last_layer_factor)
             sym_film = True
         else:
             structure = adjust_film_relaxation(structure, suggestion, host_symbol, bond_length, last_layer_factor,
                                                first_layer_factor)
             sym_film = False
 
     try:
@@ -526,10 +540,9 @@
             inputs = find_inputs_relax(relax_wc.inputs.scf__remote_data)
         else:
             return relax_wc.inputs.scf__structure.get_incoming().all()[0].node.get_outgoing().get_node_by_label(
                 'substrate').uuid
 
     if isinstance(inputs, FleurinpData):
         raise ValueError('Did not expect to find Relax WC started from FleurinpData')
-    else:
-        orig_structure = inputs[0]
-        return orig_structure.get_incoming().all()[0].node.get_outgoing().get_node_by_label('substrate').uuid
+    orig_structure = inputs[0]
+    return orig_structure.get_incoming().all()[0].node.get_outgoing().get_node_by_label('substrate').uuid
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/dmi.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/dmi.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,24 +26,26 @@
 from aiida.common.exceptions import NotExistent
 
 from aiida_fleur.tools.common_fleur_wf import test_and_get_codenode
 from aiida_fleur.tools.common_fleur_wf import get_inputs_fleur
 from aiida_fleur.workflows.scf import FleurScfWorkChain
 from aiida_fleur.data.fleurinpmodifier import FleurinpModifier
 from aiida_fleur.workflows.base_fleur import FleurBaseWorkChain
-from aiida_fleur.common.constants import HTR_TO_EV
 from aiida_fleur.data.fleurinp import FleurinpData, get_fleurinp_from_remote_data
+from aiida_fleur.data.fleurinpmodifier import inpxml_changes
+
+from masci_tools.util.constants import HTR_TO_EV
 
 
 class FleurDMIWorkChain(WorkChain):
     """
     This workflow calculates DMI energy dispersion of a structure.
     """
 
-    _workflowversion = '0.2.1'
+    _workflowversion = '0.3.0'
 
     _default_options = {
         'resources': {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1
         },
         'max_wallclock_seconds': 2 * 60 * 60,
@@ -91,15 +93,15 @@
                      if_(cls.scf_needed)(
                          cls.converge_scf,
                          cls.force_after_scf,
                      ).else_(
                          cls.force_wo_scf,
                      ), cls.get_results, cls.return_results)
 
-        spec.output('out', valid_type=Dict)
+        spec.output('output_dmi_wc_para', valid_type=Dict)
 
         # exit codes
         spec.exit_code(230, 'ERROR_INVALID_INPUT_PARAM', message='Invalid workchain parameters.')
         spec.exit_code(231, 'ERROR_INVALID_INPUT_CONFIG', message='Invalid input configuration.')
         spec.exit_code(233,
                        'ERROR_INVALID_CODE_PROVIDED',
                        message='Invalid code node specified, check inpgen and fleur code nodes.')
@@ -171,15 +173,15 @@
             options[key] = options.get(key, val)
         self.ctx.options = options
 
         # Check if user gave valid fleur executable
         inputs = self.inputs
         if 'fleur' in inputs:
             try:
-                test_and_get_codenode(inputs.fleur, 'fleur.fleur', use_exceptions=True)
+                test_and_get_codenode(inputs.fleur, 'fleur.fleur')
             except ValueError:
                 error = ('The code you provided for FLEUR does not use the plugin fleur.fleur')
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
         # Check if user gave an input setup making any sense
         if 'scf' in inputs:
@@ -216,59 +218,46 @@
 
     def get_inputs_scf(self):
         """
         Initialize inputs for the scf cycle
         """
         input_scf = AttributeDict(self.exposed_inputs(FleurScfWorkChain, namespace='scf'))
 
-        if 'wf_parameters' not in input_scf:
-            scf_wf_dict = {}
-        else:
-            scf_wf_dict = input_scf.wf_parameters.get_dict()
-
-        if 'inpxml_changes' not in scf_wf_dict:
-            scf_wf_dict['inpxml_changes'] = []
-
-        # set up q vector for the reference calculation
-        list_ref_qss = self.ctx.wf_dict['ref_qss']
-        if [x for x in list_ref_qss if x != 0]:
-            changes_dict = {
-                'qss': self.ctx.wf_dict['ref_qss'],
-                'l_noco': True,
-                'ctail': False,
-                'l_ss': True,
-                'l_soc': False
-            }
-        else:
-            changes_dict = {'qss': ' 0.0 0.0 0.0 ', 'l_noco': False, 'ctail': True, 'l_ss': False, 'l_soc': False}
-
-        scf_wf_dict['inpxml_changes'].append(('set_inpchanges', {'change_dict': changes_dict}))
+        with inpxml_changes(input_scf) as fm:
 
-        # change beta parameter
-        for key, val in self.ctx.wf_dict.get('beta', {}).items():
-            scf_wf_dict['inpxml_changes'].append(('set_atomgroup_label', {
-                'attributedict': {
-                    'nocoParams': {
-                        'beta': val
-                    }
-                },
-                'atom_label': key
-            }))
-
-        input_scf.wf_parameters = Dict(dict=scf_wf_dict)
+            if [x for x in self.ctx.wf_dict['ref_qss'] if x != 0]:
+                fm.set_inpchanges({
+                    'qss': self.ctx.wf_dict['ref_qss'],
+                    'l_noco': True,
+                    'ctail': False,
+                    'l_ss': True,
+                    'l_soc': False
+                })
+            else:
+                fm.set_inpchanges({
+                    'qss': ' 0.0 0.0 0.0 ',
+                    'l_noco': False,
+                    'ctail': True,
+                    'l_ss': False,
+                    'l_soc': False
+                })
+
+            # change beta parameter
+            for key, val in self.ctx.wf_dict['beta'].items():
+                fm.set_atomgroup_label(key, {'nocoParams': {'beta': val}})
 
         if 'structure' in input_scf:  # add info about spin spiral propagation
             if 'calc_parameters' in input_scf:
                 calc_parameters = input_scf.calc_parameters.get_dict()
             else:
                 calc_parameters = {}
             sum_vec = np.array([np.pi / 4.0, np.e / 3.0, np.euler_gamma])
             calc_parameters['qss'] = {'x': sum_vec[0], 'y': sum_vec[1], 'z': sum_vec[2]}
             calc_parameters['soc'] = {'theta': 0.7, 'phi': 0.7}
-            input_scf.calc_parameters = Dict(dict=calc_parameters)
+            input_scf.calc_parameters = Dict(calc_parameters)
         return input_scf
 
     def change_fleurinp(self):
         """
         This routine sets somethings in the fleurinp file before running a fleur
         calculation.
         """
@@ -286,100 +275,76 @@
                 fleurin = self.inputs.fleurinp
             else:
                 # In this case only remote is given
                 # fleurinp data has to be generated from the remote inp.xml file
                 fleurin = get_fleurinp_from_remote_data(self.inputs.remote)
 
         # copy inpchanges from wf parameters
-        fchanges = self.ctx.wf_dict.get('inpxml_changes', [])
-        # create forceTheorem tags
-        fchanges.append(('set_complex_tag', {
-            'tag_name': 'DMI',
-            'create': True,
-            'changes': {
+        with inpxml_changes(self.ctx.wf_dict) as fm:
+            fm.set_complex_tag('DMI', {
                 'qVectors': {
                     'q': self.ctx.wf_dict['q_vectors']
                 },
                 'theta': self.ctx.wf_dict['sqas_theta'],
                 'phi': self.ctx.wf_dict['sqas_phi']
-            }
-        }))
-
-        changes_dict = {
-            'itmax': 1,
-            'l_noco': True,
-            'ctail': False,
-            'spav': True,
-            # 'l_soc': True,
-            'l_ss': True
-        }
-        fchanges.append(('set_inpchanges', {'change_dict': changes_dict}))
-
-        if self.ctx.wf_dict['kmesh_force_theorem'] is not None:
-            kmesh = KpointsData()
-            kmesh.set_kpoints(monkhorst_pack(self.ctx.wf_dict['kmesh_force_theorem']))
-            kmesh.store()
-            fchanges.append(('set_kpointsdata', {
-                'kpointsdata_uuid': kmesh.uuid,
-                'switch': True,
-                'kpoint_type': 'mesh'
-            }))
-
-        # change beta parameter
-        for label, beta in self.ctx.wf_dict['beta'].items():
-            fchanges.append(('set_atomgroup_label', {
-                'attributedict': {
-                    'nocoParams': {
-                        'beta': beta
-                    }
-                },
-                'atom_label': label
-            }))
-
-        # switch off SOC on an atom specie
-        for atom_label in self.ctx.wf_dict['soc_off']:
-            fchanges.append(('set_species_label', {
-                'atom_label': atom_label,
-                'attributedict': {
-                    'special': {
+            },
+                               create=True)
+            fm.set_inpchanges({
+                'itmax': 1,
+                'l_noco': True,
+                'ctail': False,
+                'spav': True,
+                # 'l_soc': True,
+                'l_ss': True
+            })
+
+            if self.ctx.wf_dict['kmesh_force_theorem'] is not None:
+                kmesh = KpointsData()
+                kmesh.set_kpoints(monkhorst_pack(self.ctx.wf_dict['kmesh_force_theorem']))
+                kmesh.store()
+                fm.set_kpointsdata(kmesh.uuid, switch=True, kpoint_type='mesh')
+
+            # change beta parameter
+            for key, val in self.ctx.wf_dict['beta'].items():
+                fm.set_atomgroup_label(key, {'nocoParams': {'beta': val}})
+
+            # switch off SOC on an atom specie
+            for atom_label in self.ctx.wf_dict['soc_off']:
+                fm.set_species_label(
+                    atom_label,
+                    {'special': {
                         'socscale': 0.0
-                    }
-                },
-            }))
-
-        if fchanges:  # change inp.xml file
-            fleurmode = FleurinpModifier(fleurin)
-            try:
-                fleurmode.add_task_list(fchanges)
-            except (ValueError, TypeError) as exc:
-                error = ('ERROR: Changing the inp.xml file failed. Tried to apply inpxml_changes'
-                         f', which failed with {exc}. I abort, good luck next time!')
-                self.control_end_wc(error)
-                return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
+                    }},
+                )
 
-            # validate?
-            try:
-                fleurmode.show(display=False, validate=True)
-            except etree.DocumentInvalid:
-                error = ('ERROR: input, user wanted inp.xml changes did not validate')
-                self.report(error)
-                return self.exit_codes.ERROR_INVALID_INPUT_FILE
-            except ValueError as exc:
-                error = ('ERROR: input, user wanted inp.xml changes could not be applied.'
-                         f'The following error was raised {exc}')
-                self.control_end_wc(error)
-                return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
+        fleurmode = FleurinpModifier(fleurin)
+        try:
+            fleurmode.add_task_list(self.ctx.wf_dict['inpxml_changes'])
+        except (ValueError, TypeError) as exc:
+            error = ('ERROR: Changing the inp.xml file failed. Tried to apply inpxml_changes'
+                     f', which failed with {exc}. I abort, good luck next time!')
+            self.control_end_wc(error)
+            return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
 
-            # apply
-            out = fleurmode.freeze()
-            self.ctx.fleurinp = out
-        else:  # otherwise do not change the inp.xml
-            self.ctx.fleurinp = fleurin
+        # validate?
+        try:
+            fleurmode.show(display=False, validate=True)
+        except etree.DocumentInvalid:
+            error = ('ERROR: input, user wanted inp.xml changes did not validate')
+            self.report(error)
+            return self.exit_codes.ERROR_INVALID_INPUT_FILE
+        except ValueError as exc:
+            error = ('ERROR: input, user wanted inp.xml changes could not be applied.'
+                     f'The following error was raised {exc}')
+            self.control_end_wc(error)
+            return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
 
-        return
+        # apply
+        out = fleurmode.freeze()
+        self.ctx.fleurinp = out
 
     def force_after_scf(self):
         '''
         This routine uses the force theorem to calculate energies dispersion of
         spin spirals. The force theorem calculations implemented into the FLEUR
         code. Hence a single iteration FLEUR input file having <forceTheorem> tag
         has to be created and submitted.
@@ -548,15 +513,15 @@
             'energy_units': 'eV',
             'info': self.ctx.info,
             'warnings': self.ctx.warnings,
             'errors': self.ctx.errors,
         }
 
         out = save_output_node(Dict(dict=out))
-        self.out('out', out)
+        self.out('output_dmi_wc_para', out)
 
     def control_end_wc(self, errormsg):
         """
         Controlled way to shutdown the workchain. will initialize the output nodes
         The shutdown of the workchain will has to be done afterwards
         """
         self.report(errormsg)  # because return_results still fails somewhen
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/dos.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/dos.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             self.ctx.options = inputs.options.get_dict()
 
         if 'remote_data' in inputs:
             self.ctx.remote = inputs.remote_data
 
         if 'fleur' in inputs:
             try:
-                test_and_get_codenode(inputs.fleur, 'fleur.fleur', use_exceptions=True)
+                test_and_get_codenode(inputs.fleur, 'fleur.fleur')
             except ValueError:
                 error = ('The code you provided for FLEUR does not use the plugin fleur.fleur')
                 # self.control_end_wc(error)
                 self.report(error)
                 return 1
 
     def create_new_fleurinp(self):
@@ -199,15 +199,15 @@
         outputnode_dict['successful'] = self.ctx.successful
         #outputnode_dict['last_calc_pk'] = self.ctx.last_calc.pk
         #outputnode_dict['last_calc_uuid'] = self.ctx.last_calc.uuid
         outputnode_dict['dosfile'] = dosfilepath
         # add nkpoints, emin, emax, sigma, tria
 
         # print outputnode_dict
-        outputnode = Dict(dict=outputnode_dict)
+        outputnode = Dict(outputnode_dict)
         outdict = {}
         # TODO parse dos to dosnode
         #dosnode = ''
         #outdict['output_band'] = dosnode
         # or if spin =2
         #outdict['output_band1'] = dosnode1
         #outdict['output_band2'] = dosnode2
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/eos.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/eos.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """
 # TODO: print more user info
 # allow different inputs, make things optional(don't know yet how)
 # half number of iteration if you are close to be converged. (therefore
 # one can start with 18 iterations, and if thats not enough run again 9 or something)
 import numpy as np
 
+from aiida import orm
 from aiida.orm import load_node
 from aiida.orm import Float, StructureData, Dict, List
 from aiida.engine import WorkChain, ToContext
 from aiida.engine import calcfunction as cf
 from aiida.common import AttributeDict
 
 from masci_tools.util.constants import HTR_TO_EV
@@ -178,15 +179,15 @@
         first_scf = self.ctx[label]
         if not first_scf.is_finished_ok:
             self.report('Initial sub process did not finish successfully; aborting the workchain.')
             # return self.exit_codes.ERROR_SUB_PROCESS_FAILED.format(cls=self.inputs.sub_process_class)  # pylint: disable=no-member
             return self.exit_codes.ERROR_SUB_PROCESS_FAILED
 
         fleurinp = first_scf.outputs.fleurinp
-        self.ctx.first_calc_parameters = fleurinp.get_parameterdata()
+        self.ctx.first_calc_parameters = fleurinp.get_parameterdata(write_ids=orm.Bool(False))
 
     def converge_scf(self):
         """
         Launch fleur_scfs from the generated structures
         """
         calcs = {}
 
@@ -290,15 +291,15 @@
         write_defaults_fit = False
         # TODO: different fits
         if len(en_array):  # for some reason just en_array does not work
             volume, bulk_modulus, bulk_deriv, residuals = birch_murnaghan_fit(en_array, vol_array)
 
             # something went wrong with the fit
             for i in volume, bulk_modulus, bulk_deriv, residuals:
-                if issubclass(type(i), np.complex):
+                if isinstance(i, complex):
                     write_defaults_fit = True
 
             if all(i is not None for i in (volume, bulk_modulus, bulk_deriv, residuals)):
                 # cast float, because np datatypes are sometimes not serialable
                 volume, bulk_modulus = float(volume), float(bulk_modulus)
                 bulk_deriv, residuals = float(bulk_deriv), residuals.tolist()
 
@@ -355,15 +356,15 @@
 
         if self.ctx.successful:
             self.report('Done, Equation of states calculation complete')
         else:
             self.report('Done, but something went wrong.... Probably some individual calculation failed or'
                         ' a scf-cycle did not reach the desired distance.')
 
-        outnode = Dict(dict=out)
+        outnode = Dict(out)
         outnodedict['results_node'] = outnode
 
         # create links between all these nodes...
         outputnode_dict = create_eos_result_node(**outnodedict)
         outputnode = outputnode_dict.get('output_eos_wc_para')
         outputnode.label = 'output_eos_wc_para'
         outputnode.description = ('Contains equation of states results and information of an FleurEosWorkChain run.')
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/initial_cls.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/initial_cls.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         self.ctx.bandgaps = {}
         self.ctx.atomtypes = {}
         # set values, or defaults for Wf_para
         # 'wf_parameters' always there
         wf_dict = self.inputs.wf_parameters.get_dict()
         default = self._default_wf_para
 
-        self.ctx.add_comp_para = wf_dict.get('add_para_calc', default.get('add_para_calc'))
+        self.ctx.add_comp_para = wf_dict.get('add_comp_para', default.get('add_comp_para'))
         self.ctx.same_para = wf_dict.get('same_para', default.get('same_para'))
         self.ctx.scf_para = wf_dict.get('scf_para', default.get('scf_para'))
         self.ctx.relax = wf_dict.get('relax', default.get('relax'))
         self.ctx.relax_mode = wf_dict.get('relax_mode', default.get('relax_mode'))
         self.ctx.relax_para = wf_dict.get('relax_para', default.get('dos_para'))
 
         defaultoptions = self._default_options
@@ -400,18 +400,18 @@
         para = self.ctx.scf_para
         if para == 'default':
             wf_parameter = {}
         else:
             wf_parameter = para
         wf_parameter['add_comp_para'] = self.ctx.add_comp_para
         #wf_parameter['options'] = self.ctx.options
-        wf_parameters = Dict(dict=wf_parameter)
+        wf_parameters = Dict(wf_parameter)
         resall = {}
         calc_labels = []
-        options = Dict(dict=self.ctx.options)
+        options = Dict(self.ctx.options)
         # for each calulation in self.ctx.calcs_torun #TODO what about wf params?
         res = None
         #print(self.ctx.calcs_torun)
         for i, node in enumerate(self.ctx.calcs_torun):
             #print node
             calclabel = f'ori_calc_{i}'
             calc_labels.append(calclabel)
@@ -530,16 +530,16 @@
         if para == 'default':
             wf_parameter = {}
         else:
             wf_parameter = para
         wf_parameter['add_comp_para'] = self.ctx.add_comp_para
         # TODO maybe use less resources, or default of one machine
         #wf_parameter['options'] = self.ctx.options
-        wf_parameters = Dict(dict=wf_parameter)
-        options = Dict(dict=self.ctx.options)
+        wf_parameters = Dict(wf_parameter)
+        options = Dict(self.ctx.options)
 
         res_all = []
         calcs = {}
         # now in parallel
         #print self.ctx.ref_calcs_torun
         i = 0
         #print(self.ctx.ref_calcs_torun)
@@ -819,25 +819,25 @@
         outputnode_dict['total_energy_units'] = 'eV'
         outputnode_dict['total_energy_ref'] = list(tE_ref.values())
         outputnode_dict['total_energy_ref_des'] = list(tE_ref.keys())
         #outputnode = Dict(dict=outputnode_dict)
 
         # To have to ouput node linked to the calculation output nodes
         outnodedict = {}
-        outnode = Dict(dict=outputnode_dict)
+        outnode = Dict(outputnode_dict)
         outnodedict['results_node'] = outnode
 
         # TODO: bad design, put in calcfunction and make bullet proof.
         calc = self.ctx[self.ctx.calc_labels[-1]]
-        calc_dict = calc.get_outgoing().get_node_by_label('output_scf_wc_para')
+        calc_dict = calc.base.links.get_outgoing().get_node_by_label('output_scf_wc_para')
         outnodedict['input_structure'] = calc_dict
 
         for label in self.ctx.ref_labels:
             calc = self.ctx[label]
-            calc_dict = calc.get_outgoing().get_node_by_label('output_scf_wc_para')
+            calc_dict = calc.base.links.get_outgoing().get_node_by_label('output_scf_wc_para')
             outnodedict[label] = calc_dict
 
         outdict = create_initcls_result_node(**outnodedict)
 
         #outdict = {}
         #outdict['output_initial_cls_wc_para'] = outputnode
         #print outdict
@@ -917,15 +917,15 @@
 
 
 def fleur_calc_get_structure(calc_node):
     """
     Get the AiiDA data structure from a fleur calculations
     """
     #get fleurinp
-    fleurinp = calc_node.inp.fleurinpdata
+    fleurinp = calc_node.inp.fleurinp
     structure = fleurinp.get_structuredata(fleurinp)
     return structure
 
 
 def extract_results(calcs):
     """
     Collect results from certain calculation, check if everything is fine,
@@ -936,23 +936,21 @@
 
     from aiida_fleur.tools.extract_corelevels import extract_corelevels
     log = []
     calc_uuids = []
     for calc in calcs:
         #print(calc)
         try:
-            calc_uuid = calc.get_outgoing().get_node_by_label('output_scf_wc_para').get_dict()['last_calc_uuid']
+            calc_uuid = calc.outputs.last_calc.remote_folder.creator.uuid
         except (NotExistent, MultipleObjectsError, ValueError, TypeError, KeyError):  #TODO which error
-            logmsg = ('ERROR: No output_scf_wc_para node found or no "last_calc_uuid" '
-                      'key in it for calculation: {}'.format(calc))
+            logmsg = f'ERROR: No FleurCalculation node found in SCF workchain: {calc.uuid}'
             log.append(logmsg)
             continue
         if calc_uuid is not None:
             calc_uuids.append(calc_uuid)
-        #calc_uuids.append(calc['output_scf_wc_para'].get_dict()['last_calc_uuid'])
 
     all_corelevels = {}
     fermi_energies = {}
     bandgaps = {}
     all_atomtypes = {}
     total_energy = {}
 
@@ -963,21 +961,18 @@
         calc = load_node(uuid)
         if not isinstance(calc, CalcJobNode):
             #raise ValueError("Calculation with pk {} must be a FleurCalculation".format(pk))
             # log and continue
             continue
         if calc.is_finished_ok:
             # get out.xml file of calculation
-            #outxml = calc.outputs.retrieved.folder.get_abs_path('path/out.xml')
-            outxml = calc.outputs.retrieved.open('out.xml')
-            #print outxml
-            try:
+
+            with calc.outputs.retrieved.open('out.xml', 'rb') as outxml:
                 corelevels, atomtypes = extract_corelevels(outxml)
-            finally:
-                outxml.close()
+
             #all_corelevels.append(core)
             #print('corelevels: {}'.format(corelevels))
             #print('atomtypes: {}'.format(atomtypes))
             #for i in range(0,len(corelevels[0][0]['corestates'])):
             #    print corelevels[0][0]['corestates'][i]['energy']
 
             #TODO how to store?
@@ -1008,15 +1003,15 @@
             atomtypes = [float('nan')]
             logmsg = f'ERROR: Fleur Calculation with uuid {uuid} was not in in state FINISHED'
             log.append(logmsg)
             #continue
             #raise ValueError("Calculation with pk {} must be in state FINISHED".format(pk))
 
         # TODO: maybe different, because it is prob know from before
-        fleurinp = calc.inputs.fleurinpdata
+        fleurinp = calc.inputs.fleurinp
         structure = fleurinp.get_structuredata_ncf()
         compound = structure.get_formula()
         #print compound
         fermi_energies[compound] = efermi
         bandgaps[compound] = bandgap
         all_atomtypes[compound] = atomtypes
         all_corelevels[compound] = corelevels
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/mae.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/mae.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,31 +11,30 @@
 """
     In this module you find the workflow 'FleurMaeWorkChain' for the calculation of
     Magnetic Anisotropy Energy via the force theorem.
 """
 
 import copy
 
-#from six.moves import map
 from lxml import etree
 from ase.dft.kpoints import monkhorst_pack
 
 from aiida.engine import WorkChain, ToContext, if_
 from aiida.engine import calcfunction as cf
 from aiida.orm import Code, load_node
 from aiida.orm import RemoteData, Dict, KpointsData
 from aiida.common import AttributeDict
 from aiida.common.exceptions import NotExistent
 
 from aiida_fleur.tools.common_fleur_wf import test_and_get_codenode, get_inputs_fleur
 from aiida_fleur.workflows.scf import FleurScfWorkChain
 from aiida_fleur.workflows.base_fleur import FleurBaseWorkChain
-from aiida_fleur.data.fleurinpmodifier import FleurinpModifier
+from aiida_fleur.data.fleurinpmodifier import FleurinpModifier, inpxml_changes
 from aiida_fleur.data.fleurinp import FleurinpData, get_fleurinp_from_remote_data
-from aiida_fleur.common.constants import HTR_TO_EV
+from masci_tools.util.constants import HTR_TO_EV
 
 
 class FleurMaeWorkChain(WorkChain):
     """
         This workflow calculates the Magnetic Anisotropy Energy of a structure.
     """
 
@@ -140,24 +139,17 @@
 
         # extend wf parameters given by user using defaults
         for key, val in wf_default.items():
             wf_dict[key] = wf_dict.get(key, val)
         self.ctx.wf_dict = wf_dict
 
         # switch off SOC on an atom specie
-        for atom_label in self.ctx.wf_dict['soc_off']:
-            self.ctx.wf_dict['inpxml_changes'].append(('set_species_label', {
-                'at_label': atom_label,
-                'attributedict': {
-                    'special': {
-                        'socscale': 0.0
-                    }
-                },
-                'create': True
-            }))
+        with inpxml_changes(self.ctx.wf_dict) as fm:
+            for atom_label in self.ctx.wf_dict['soc_off']:
+                fm.set_species(atom_label, {'special': {'socscale': 0}})
 
         # Check if sqas_theta and sqas_phi have the same length
         if len(self.ctx.wf_dict.get('sqas_theta')) != len(self.ctx.wf_dict.get('sqas_phi')):
             error = ('Number of sqas_theta has to be equal to the number of sqas_phi')
             self.control_end_wc(error)
             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
@@ -173,15 +165,15 @@
             options[key] = options.get(key, val)
         self.ctx.options = options
 
         # Check if user gave valid fleur executable
         inputs = self.inputs
         if 'fleur' in inputs:
             try:
-                test_and_get_codenode(inputs.fleur, 'fleur.fleur', use_exceptions=True)
+                test_and_get_codenode(inputs.fleur, 'fleur.fleur')
             except ValueError:
                 error = ('The code you provided for FLEUR does not use the plugin fleur.fleur')
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
         # Check if user gave an input setup making any sense
         if 'scf' in inputs:
@@ -220,50 +212,42 @@
     def get_inputs_scf(self):
         """
         Initialize inputs for scf workflow:
         wf_param, options, calculation parameters, codes, structure
         """
         input_scf = AttributeDict(self.exposed_inputs(FleurScfWorkChain, namespace='scf'))
 
-        if 'wf_parameters' not in input_scf:
-            scf_wf_dict = {}
-        else:
-            scf_wf_dict = input_scf.wf_parameters.get_dict()
-
-        if 'inpxml_changes' not in scf_wf_dict:
-            scf_wf_dict['inpxml_changes'] = []
-
         soc = self.ctx.wf_dict.get('sqa_ref')
-        if not self.ctx.wf_dict.get('use_soc_ref'):
-            scf_wf_dict['inpxml_changes'].append(('set_inpchanges', {'change_dict': {'l_soc': False}}))
-        else:  # set soc parameters explicitly
-            changes_dict = {'theta': soc[0], 'phi': soc[1], 'l_soc': True}
-            scf_wf_dict['inpxml_changes'].append(('set_inpchanges', {
-                'change_dict': changes_dict,
-                'path_spec': {
-                    'phi': {
-                        'contains': 'soc'
-                    },
-                    'theta': {
-                        'contains': 'soc'
-                    }
-                }
-            }))
-
-        input_scf.wf_parameters = Dict(dict=scf_wf_dict)
+        with inpxml_changes(input_scf) as fm:
+            if not self.ctx.wf_dict.get('use_soc_ref'):
+                fm.set_inpchanges({'l_soc': False})
+            else:
+                fm.set_inpchanges({
+                    'theta': soc[0],
+                    'phi': soc[1],
+                    'l_soc': True
+                },
+                                  path_spec={
+                                      'phi': {
+                                          'contains': 'soc'
+                                      },
+                                      'theta': {
+                                          'contains': 'soc'
+                                      }
+                                  })
 
         if 'structure' in input_scf:
             if 'calc_parameters' in input_scf:
                 calc_parameters = input_scf.calc_parameters.get_dict()
             else:
                 calc_parameters = {}
             if not self.ctx.wf_dict.get('use_symmetries_reference'):
                 # break symmetries, SOC will be removed if not set
                 calc_parameters['soc'] = {'theta': soc[0], 'phi': soc[1]}
-            input_scf.calc_parameters = Dict(dict=calc_parameters)
+            input_scf.calc_parameters = Dict(calc_parameters)
 
         return input_scf
 
     def change_fleurinp(self):
         """
         This routine sets somethings in the fleurinp file before running a fleur
         calculation.
@@ -279,76 +263,63 @@
             if 'fleurinp' in self.inputs:
                 fleurin = self.inputs.fleurinp
             else:
                 # In this case only remote is given
                 # fleurinp data has to be generated from the remote inp.xml file
                 fleurin = get_fleurinp_from_remote_data(self.inputs.remote)
 
-        # copy default changes
-        fchanges = self.ctx.wf_dict.get('inpxml_changes', [])
-
-        # add forceTheorem tag into inp.xml
-        fchanges.append(('set_complex_tag', {
-            'tag_name': 'MAE',
-            'create': True,
-            'changes': {
+        with inpxml_changes(self.ctx.wf_dict) as fm:
+            # add forceTheorem tag into inp.xml
+            fm.set_complex_tag('MAE', {
                 'theta': self.ctx.wf_dict['sqas_theta'],
                 'phi': self.ctx.wf_dict['sqas_phi']
-            }
-        }))
-        fchanges.append(('set_inpchanges', {'change_dict': {'itmax': 1, 'l_soc': True}}),)
-
-        if self.ctx.wf_dict['kmesh_force_theorem'] is not None:
-            # set k-mesh for the full BZ
-            kmesh = KpointsData()
-            kmesh.set_kpoints(monkhorst_pack(self.ctx.wf_dict['kmesh_force_theorem']))
-            kmesh.store()
-            fchanges.append(('set_kpointsdata', {
-                'kpointsdata_uuid': kmesh.uuid,
-                'switch': True,
-                'kpoint_type': 'mesh'
-            }))
-
-        # if self.ctx.wf_dict['use_symmetries_reference']:
-        #     # remove symmetries from the inp.xml
-        #     fchanges.append(('delete_tag', {
-        #         'tag_name': 'symOp',
-        #         'occurrences': range(1, len(fleurin.inp_dict['cell']['symmetryOperations']))
-        #     }))
+            },
+                               create=True)
 
-        if fchanges:  # change inp.xml file
-            fleurmode = FleurinpModifier(fleurin)
-            try:
-                fleurmode.add_task_list(fchanges)
-            except (ValueError, TypeError) as exc:
-                error = ('ERROR: Changing the inp.xml file failed. Tried to apply inpxml_changes'
-                         f', which failed with {exc}. I abort, good luck next time!')
-                self.control_end_wc(error)
-                return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
+            fm.set_inpchanges({'itmax': 1, 'l_soc': True})
 
-            # validate?
-            try:
-                fleurmode.show(display=False, validate=True)
-            except etree.DocumentInvalid:
-                error = ('ERROR: input, user wanted inp.xml changes did not validate')
-                self.report(error)
-                return self.exit_codes.ERROR_INVALID_INPUT_FILE
-            except ValueError as exc:
-                error = ('ERROR: input, user wanted inp.xml changes could not be applied.'
-                         f'The following error was raised {exc}')
-                self.control_end_wc(error)
-                return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
+            if self.ctx.wf_dict['kmesh_force_theorem'] is not None:
+                # set k-mesh for the full BZ
+                kmesh = KpointsData()
+                kmesh.set_kpoints(monkhorst_pack(self.ctx.wf_dict['kmesh_force_theorem']))
+                kmesh.store()
+                fm.set_kpointsdata(kmesh.uuid, switch=True, kpoint_type='mesh')
+
+            # if self.ctx.wf_dict['use_symmetries_reference']:
+            #     # remove symmetries from the inp.xml
+            #     fchanges.append(('delete_tag', {
+            #         'tag_name': 'symOp',
+            #         'occurrences': range(1, len(fleurin.inp_dict['cell']['symmetryOperations']))
+            #     }))
 
-            # apply
-            out = fleurmode.freeze()
-            self.ctx.fleurinp = out
-        else:  # otherwise do not change the inp.xml
-            self.ctx.fleurinp = fleurin
+        fleurmode = FleurinpModifier(fleurin)
+        try:
+            fleurmode.add_task_list(self.ctx.wf_dict['inpxml_changes'])
+        except (ValueError, TypeError) as exc:
+            error = ('ERROR: Changing the inp.xml file failed. Tried to apply inpxml_changes'
+                     f', which failed with {exc}. I abort, good luck next time!')
+            self.control_end_wc(error)
+            return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
+
+        # validate?
+        try:
+            fleurmode.show(display=False, validate=True)
+        except etree.DocumentInvalid:
+            error = ('ERROR: input, user wanted inp.xml changes did not validate')
+            self.report(error)
+            return self.exit_codes.ERROR_INVALID_INPUT_FILE
+        except ValueError as exc:
+            error = ('ERROR: input, user wanted inp.xml changes could not be applied.'
+                     f'The following error was raised {exc}')
+            self.control_end_wc(error)
+            return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
 
-        return
+        # apply
+        out = fleurmode.freeze()
+        self.ctx.fleurinp = out
 
     def force_after_scf(self):
         """
         Calculate energy of a system for given SQAs
         using the force theorem. Converged reference is stored in self.ctx['xyz'].
         """
         calc = self.ctx.reference
@@ -514,15 +485,15 @@
             'info': self.ctx.info,
             'warnings': self.ctx.warnings,
             'errors': self.ctx.errors
         }
 
         # ensure provenance of output nodes
 
-        out_dict = {'out': Dict(dict=out)}
+        out_dict = {'out': Dict(out)}
         if self.ctx.fleuroutuuid is not None:
             out_dict['last_fleur_out'] = load_node(self.ctx.fleuroutuuid)
 
         out_nodes = save_mae_output_node(**out_dict)
         out = out_nodes.get('output_mae_wc_para')
 
         # make wc return out node
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/mae_conv.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/mae_conv.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,23 +17,25 @@
 
 from aiida.engine import WorkChain
 from aiida.engine import calcfunction as cf
 from aiida.orm import Dict
 from aiida.common import AttributeDict
 
 from aiida_fleur.workflows.scf import FleurScfWorkChain
-from aiida_fleur.common.constants import HTR_TO_EV
+from aiida_fleur.data.fleurinpmodifier import inpxml_changes
+
+from masci_tools.util.constants import HTR_TO_EV
 
 
 class FleurMaeConvWorkChain(WorkChain):
     """
     This workflow calculates the Magnetic Anisotropy Energy of a structure.
     """
 
-    _workflowversion = '0.2.1'
+    _workflowversion = '0.3.0'
 
     _default_wf_para = {'sqas': {'label': [0.0, 0.0]}, 'soc_off': []}
     _default_options = {
         'resources': {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1
         },
@@ -48,15 +50,15 @@
     def define(cls, spec):
         super().define(spec)
         spec.expose_inputs(FleurScfWorkChain, namespace='scf')
         spec.input('wf_parameters', valid_type=Dict, required=False)
 
         spec.outline(cls.start, cls.converge_scf, cls.get_results, cls.return_results)
 
-        spec.output('out', valid_type=Dict)
+        spec.output('output_mae_conv_wc_para', valid_type=Dict)
 
         # exit codes
         spec.exit_code(230, 'ERROR_INVALID_INPUT_PARAM', message='Invalid workchain parameters.')
         spec.exit_code(343, 'ERROR_ALL_SQAS_FAILED', message='Convergence MAE calculation failed for all SQAs.')
         spec.exit_code(344, 'ERROR_SOME_SQAS_FAILED', message='Convergence MAE calculation failed for some SQAs.')
 
     def start(self):
@@ -92,66 +94,48 @@
             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
         # extend wf parameters given by user using defaults
         for key, val in wf_default.items():
             wf_dict[key] = wf_dict.get(key, val)
         self.ctx.wf_dict = wf_dict
 
-    def converge_scf(self):
-        """
-        Converge charge density with or without SOC.
-        Depending on a branch of MAE calculation, submit a single Fleur calculation to obtain
-        a reference for further force theorem calculations or
-        submit a set of Fleur calculations to converge charge density for all given SQAs.
-        """
-        inputs = {}
-        for key, soc in self.ctx.wf_dict['sqas'].items():
-            inputs[key] = self.get_inputs_scf()
-            inputs[key].calc_parameters['soc'] = {'theta': soc[0], 'phi': soc[1]}
-            inputs[key].calc_parameters = Dict(dict=inputs[key].calc_parameters)
-            res = self.submit(FleurScfWorkChain, **inputs[key])
-            res.label = key
-            self.to_context(**{key: res})
-
-    def get_inputs_scf(self):
+    def get_inputs_scf(self, sqa):
         """
         Initialize inputs for scf workflow
         """
         input_scf = AttributeDict(self.exposed_inputs(FleurScfWorkChain, namespace='scf'))
 
-        if 'wf_parameters' not in input_scf:
-            scf_wf_dict = {}
-        else:
-            scf_wf_dict = input_scf.wf_parameters.get_dict()
-
-        if 'inpxml_changes' not in scf_wf_dict:
-            scf_wf_dict['inpxml_changes'] = []
-
-        # switch off SOC on an atom specie
-        for atom_label in self.ctx.wf_dict['soc_off']:
-            scf_wf_dict['inpxml_changes'].append(('set_species_label', {
-                'at_label': atom_label,
-                'attributedict': {
-                    'special': {
-                        'socscale': 0.0
-                    }
-                },
-                'create': True
-            }))
-
-        input_scf.wf_parameters = Dict(dict=scf_wf_dict)
+        with inpxml_changes(input_scf) as fm:
+            for atom_label in self.ctx.wf_dict['soc_off']:
+                fm.set_species_label(atom_label, {'special': {'socscale': 0}})
 
         if 'calc_parameters' in input_scf:
             calc_parameters = input_scf.calc_parameters.get_dict()
         else:
             calc_parameters = {}
-        input_scf.calc_parameters = calc_parameters
+        calc_parameters['soc'] = {'theta': sqa[0], 'phi': sqa[1]}
+
+        input_scf.calc_parameters = Dict(calc_parameters)
 
         return input_scf
 
+    def converge_scf(self):
+        """
+        Converge charge density with or without SOC.
+        Depending on a branch of MAE calculation, submit a single Fleur calculation to obtain
+        a reference for further force theorem calculations or
+        submit a set of Fleur calculations to converge charge density for all given SQAs.
+        """
+        inputs = {}
+        for key, soc in self.ctx.wf_dict['sqas'].items():
+            inputs[key] = self.get_inputs_scf(sqa=soc)
+            res = self.submit(FleurScfWorkChain, **inputs[key])
+            res.label = key
+            self.to_context(**{key: res})
+
     def get_results(self):
         """
         Retrieve results of converge calculations
         """
         t_energydict = {}
         original_t_energydict = {}
         outnodedict = {}
@@ -217,19 +201,19 @@
             'info': self.ctx.info,
             'warnings': self.ctx.warnings,
             'errors': self.ctx.errors
         }
 
         # create link to workchain node
         out = save_output_node(Dict(dict=out))
-        self.out('out', out)
+        self.out('output_mae_conv_wc_para', out)
 
         if not self.ctx.energydict:
             return self.exit_codes.ERROR_ALL_SQAS_FAILED
-        elif failed_labels:
+        if failed_labels:
             return self.exit_codes.ERROR_SOME_SQAS_FAILED
 
     def control_end_wc(self, errormsg):
         """
         Controlled way to shutdown the workchain. will initialize the output nodes
         The shutdown of the workchain will has to be done afterwards
         """
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/orbcontrol.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/orbcontrol.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,33 @@
 # For further information please visit http://www.flapw.de or                 #
 # http://aiida-fleur.readthedocs.io/en/develop/                               #
 ###############################################################################
 """
     In this module you find the workflow 'FleurOrbControlWorkChain' for finding the groundstate
     in a DFT+U calculation.
 """
-from aiida.engine import WorkChain, ToContext, if_
+from aiida import orm
+from aiida.engine import WorkChain, ToContext, if_, ExitCode
 from aiida.engine import calcfunction as cf
 from aiida.orm import Dict, Code, StructureData, RemoteData
 from aiida.common import AttributeDict
 from aiida.common.exceptions import NotExistent
 
 from aiida_fleur.tools.common_fleur_wf import test_and_get_codenode
 from aiida_fleur.tools.common_fleur_wf import get_inputs_fleur, get_inputs_inpgen
 
 from aiida_fleur.calculation.fleur import FleurCalculation
 from aiida_fleur.workflows.scf import FleurScfWorkChain
 from aiida_fleur.workflows.base_fleur import FleurBaseWorkChain
-from aiida_fleur.data.fleurinpmodifier import FleurinpModifier
+from aiida_fleur.data.fleurinpmodifier import FleurinpModifier, inpxml_changes
 from aiida_fleur.data.fleurinp import FleurinpData, get_fleurinp_from_remote_data
 
 import numpy as np
 from lxml import etree
+import re
 
 
 def generate_density_matrix_configurations(occupations=None, configurations=None):
     """
     Generate all the necessary density matrix configurations from either the occupations or
     the explicitly given configurations for each species/orbital
 
@@ -134,15 +136,15 @@
     :param structure: (StructureData) Structure to start from if no SCF should be done
     :param calc_parameters: (Dict), Inpgen Parameters
     :param settings: (Dict), additional settings for e.g retrieving files
     :param options: (Dict), Options for the submission of the jobs
     :param inpgen: (Code)
     :param fleur: (Code)
     """
-    _workflowversion = '0.3.3'
+    _workflowversion = '0.6.0'
 
     _default_options = {
         'resources': {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1
         },
         'max_wallclock_seconds': 2 * 60 * 60,
@@ -150,19 +152,25 @@
         'custom_scheduler_commands': '',
         'import_sys_environment': False,
         'environment_variables': {}
     }
 
     _wf_default = {
         'iterations_fixed': 30,
+        'distance_cutoff_relaxed': 5,
         'ldau_dict': None,
         'use_orbital_occupation': False,
         'fixed_occupations': None,
         'fixed_configurations': None,
-        'inpxml_changes': []
+        'inpxml_changes': [],
+        'add_comp_para': {
+            'only_even_MPI': False,
+            'max_queue_nodes': 20,
+            'max_queue_wallclock_sec': 86400
+        },
     }
 
     @classmethod
     def define(cls, spec):
         super().define(spec)
         spec.expose_inputs(FleurScfWorkChain,
                            namespace_options={
@@ -187,19 +195,24 @@
         spec.input('inpgen', valid_type=Code, required=False)
         spec.input('wf_parameters', valid_type=Dict, required=False)
         spec.input('options', valid_type=Dict, required=False)
         spec.input('options_inpgen', valid_type=Dict, required=False)
         spec.input('settings', valid_type=Dict, required=False)
         spec.input('settings_inpgen', valid_type=Dict, required=False)
 
+        spec.input_namespace('fixed_remotes', valid_type=orm.RemoteData, dynamic=True, required=False)
+        spec.input_namespace('relaxed_remotes', valid_type=orm.RemoteData, dynamic=True, required=False)
+
         spec.outline(cls.start, cls.validate_input,
                      if_(cls.scf_no_ldau_needed)(cls.converge_scf_no_ldau).elif_(cls.inpgen_needed)(cls.run_inpgen),
-                     cls.create_configurations, cls.run_fleur_fixed, cls.converge_scf, cls.return_results)
+                     cls.create_configurations,
+                     if_(cls.run_fixed_calculations)(cls.run_fleur_fixed), cls.converge_scf, cls.return_results)
 
         spec.output('output_orbcontrol_wc_para', valid_type=Dict)
+        spec.output('groundstate_denmat', valid_type=orm.SinglefileData, required=False)
         spec.expose_outputs(FleurScfWorkChain, namespace='groundstate_scf')
 
         spec.exit_code(230, 'ERROR_INVALID_INPUT_PARAM', message='Invalid workchain parameters.')
         spec.exit_code(231, 'ERROR_INVALID_INPUT_CONFIG', message='Invalid input configuration.')
         spec.exit_code(233,
                        'ERROR_INVALID_CODE_PROVIDED',
                        message='Input codes do not correspond to fleur or inpgen respectively.')
@@ -210,25 +223,68 @@
                        message='Convergence LDA+U calculation failed for some Initial configurations.')
         spec.exit_code(343,
                        'ERROR_ALL_CONFIGS_FAILED',
                        message='Convergence LDA+U calculation failed for all Initial configurations.')
         spec.exit_code(360, 'ERROR_INPGEN_CALCULATION_FAILED', message='Inpgen calculation failed.')
         spec.exit_code(450, 'ERROR_SCF_NOLDAU_FAILED', message='Convergence workflow without LDA+U failed.')
 
+    @classmethod
+    def get_builder_continue_fixed(cls, node):
+        """
+        Get a Builder prepared with inputs to continue from the charge densities of
+        a already finished MagRotateWorkChain
+
+        :param node: Instance, from which the calculation should be continued
+        """
+        builder = node.get_builder_restart()
+        scf_nodes = node.get_outgoing(node_class=FleurBaseWorkChain).all()
+        for link in scf_nodes:
+            if not link.node.is_finished_ok:
+                continue
+            if not re.fullmatch(r'Fixed\_[0-9]+', link.link_label):
+                continue
+            builder.fixed_remotes[link.link_label] = link.node.outputs.remote_folder
+
+        return builder
+
+    @classmethod
+    def get_builder_continue_relaxed(cls, node, allow_nonconverged=True):
+        """
+        Get a Builder prepared with inputs to continue from the charge densities of
+        a already finished MagRotateWorkChain
+
+        :param node: Instance, from which the calculation should be continued
+        """
+        builder = node.get_builder_restart()
+        scf_nodes = node.get_outgoing(node_class=FleurScfWorkChain).all()
+        for link in scf_nodes:
+            if not link.node.is_finished_ok:
+                if allow_nonconverged:
+                    if link.node.exit_status not in FleurScfWorkChain.get_exit_statuses(['ERROR_DID_NOT_CONVERGE']):
+                        continue
+                else:
+                    continue
+            if not re.fullmatch(r'Relaxed\_[0-9]+', link.link_label):
+                continue
+            builder.relaxed_remotes[link.link_label] = link.node.outputs.remote_folder
+
+        return builder
+
     def start(self):
         """
         init context and some parameters
         """
         self.report(f'INFO: started orbital occupation control workflow version {self._workflowversion}')
 
         ####### init    #######
 
         # internal para /control para
         self.ctx.scf_no_ldau = None
         self.ctx.scf_no_ldau_needed = False
+        self.ctx.skip_fixed_calculations = False
         self.ctx.inpgen_needed = False
         self.ctx.fixed_configurations = []
         self.ctx.successful = True
         self.ctx.info = []
         self.ctx.warnings = []
         self.ctx.errors = []
         self.ctx.description_wf = self.inputs.get('description', '') + '|fleur_orbcontrol_wc|'
@@ -304,30 +360,29 @@
 
             for species, occ_species in occupations_dict.items():
                 for orbital, occ in occ_species.items():
                     if species not in ldau_dict:
                         error = f'ERROR: Invalid input: {species} defined in fixed_occupations but not in ldau_dict'
                         self.report(error)
                         return self.exit_codes.ERROR_INVALID_INPUT_PARAM
+                    missing = False
+                    if isinstance(ldau_dict[species], dict):
+                        if int(orbital) != ldau_dict[species]['l']:
+                            missing = True
                     else:
-                        missing = False
-                        if isinstance(ldau_dict[species], dict):
-                            if int(orbital) != ldau_dict[species]['l']:
+                        for index, current_dict in enumerate(ldau_dict[species]):
+                            if int(orbital) == current_dict['l']:
+                                break
+                            if index == len(ldau_dict) - 1:
                                 missing = True
-                        else:
-                            for index, current_dict in enumerate(ldau_dict[species]):
-                                if int(orbital) == current_dict['l']:
-                                    break
-                                if index == len(ldau_dict) - 1:
-                                    missing = True
-                        if missing:
-                            error = f'ERROR: Invalid input: Orbital {orbital} is given in fixed_occupations for {species}, ' \
-                                     ' but it is not defined in ldau_dict'
-                            self.report(error)
-                            return self.exit_codes.ERROR_INVALID_INPUT_PARAM
+                    if missing:
+                        error = f'ERROR: Invalid input: Orbital {orbital} is given in fixed_occupations for {species}, ' \
+                                    ' but it is not defined in ldau_dict'
+                        self.report(error)
+                        return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
                     if not isinstance(occ, list):
                         error = f'ERROR: Invalid input: {species} defined in fixed_occupations invalid type'
                         self.report(error)
                         return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
         else:
@@ -336,54 +391,56 @@
                 for species, occ_species in occupations_dict.items():
                     for orbital, occ in occ_species.items():
 
                         if species not in ldau_dict:
                             error = f'ERROR: Invalid input: {species} defined in fixed_configurations but not in ldau_dict'
                             self.report(error)
                             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
+
+                        missing = False
+                        if isinstance(ldau_dict[species], dict):
+                            if int(orbital) != ldau_dict[species]['l']:
+                                missing = True
                         else:
-                            missing = False
-                            if isinstance(ldau_dict[species], dict):
-                                if int(orbital) != ldau_dict[species]['l']:
+                            for index, current_dict in enumerate(ldau_dict[species]):
+                                if int(orbital) == current_dict['l']:
+                                    break
+                                if index == len(ldau_dict) - 1:
                                     missing = True
-                            else:
-                                for index, current_dict in enumerate(ldau_dict[species]):
-                                    if int(orbital) == current_dict['l']:
-                                        break
-                                    if index == len(ldau_dict) - 1:
-                                        missing = True
-                            if missing:
-                                error = f'ERROR: Invalid input: Orbital {orbital} is given in fixed_configurations for {species}, ' \
-                                         ' but it is not defined in ldau_dict'
-                                self.report(error)
-                                return self.exit_codes.ERROR_INVALID_INPUT_PARAM
+                        if missing:
+                            error = f'ERROR: Invalid input: Orbital {orbital} is given in fixed_configurations for {species}, ' \
+                                        ' but it is not defined in ldau_dict'
+                            self.report(error)
+                            return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
                         if not isinstance(occ, list):
                             error = f'ERROR: Invalid input: {species} defined in fixed_configurations invalid type'
                             self.report(error)
                             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
             else:
                 error = 'ERROR: Missing input: Provide one of fixed_occupations or fixed_configurations'
                 self.report(error)
                 return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
         inputs = self.inputs
         if 'fleur' in inputs:
             try:
-                test_and_get_codenode(inputs.fleur, 'fleur.fleur', use_exceptions=True)
+                test_and_get_codenode(inputs.fleur, 'fleur.fleur')
             except ValueError:
-                error = ('The code you provided for FLEUR does not use the plugin fleur.fleur')
+                error = 'The code you provided for FLEUR does not use the plugin fleur.fleur'
+                self.report(error)
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
         if 'inpgen' in inputs:
             try:
-                test_and_get_codenode(inputs.inpgen, 'fleur.inpgen', use_exceptions=True)
+                test_and_get_codenode(inputs.inpgen, 'fleur.inpgen')
             except ValueError:
-                error = ('The code you provided for INPGEN does not use the plugin fleur.inpgen')
+                error = 'The code you provided for INPGEN does not use the plugin fleur.inpgen'
+                self.report(error)
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
         fleurinp = None
         remote = None
         if 'scf_no_ldau' in inputs:
             input_scf = AttributeDict(self.exposed_inputs(FleurScfWorkChain, namespace='scf_no_ldau'))
             self.ctx.scf_no_ldau_needed = True
@@ -407,37 +464,59 @@
                 error = 'ERROR: you gave SCF input + calc_parameters for the Orbcontrol calculation'
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
             if 'inpgen' in inputs:
                 error = 'ERROR: you gave SCF input + inpgen for the Orbcontrol calculation'
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
+            if 'relaxed_remotes' in inputs:
+                error = 'ERROR: you gave SCF input + Charge densities for relaxation to start from'
+                self.control_end_wc(error)
+                return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
         elif 'structure' in inputs:
             self.ctx.inpgen_needed = True
             if 'inpgen' not in inputs:
                 error = 'ERROR: you gave structure input but no inpgen code Orbcontrol calculation'
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
-        elif 'remote' not in inputs and 'fleurinp' not in inputs:
+            if 'relaxed_remotes' in inputs:
+                error = 'ERROR: you gave structure input + Charge densities for relaxation to start from'
+                self.control_end_wc(error)
+                return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
+        elif 'remote' not in inputs and 'fleurinp' not in inputs and 'relaxed_remotes' not in inputs:
             error = 'ERROR: you gave neither SCF input nor remote or fleurinp'
             self.control_end_wc(error)
             return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
         else:
             if 'calc_parameters' in inputs:
-                error = 'ERROR: you gave remote/fleurinp input + calc_parameters for the Orbcontrol calculation'
+                error = 'ERROR: you gave remote(s)/fleurinp input + calc_parameters for the Orbcontrol calculation'
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
             if 'structure' in inputs:
-                error = 'ERROR: you gave remote/fleurinp input + structure for the Orbcontrol calculation'
+                error = 'ERROR: you gave remote(s)/fleurinp input + structure for the Orbcontrol calculation'
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
             if 'inpgen' in inputs:
-                error = 'ERROR: you gave remote/fleurinp input + inpgen for the Orbcontrol calculation'
+                error = 'ERROR: you gave remote(s)/fleurinp input + inpgen for the Orbcontrol calculation'
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
+            if 'relaxed_remotes' in inputs:
+                if 'fixed_remotes' in inputs:
+                    error = 'ERROR: you gave fixed and relaxed remotes for the Orbcontrol calculation'
+                    self.control_end_wc(error)
+                    return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
+                if 'remote' in inputs:
+                    error = 'ERROR: you gave relaxed remotes + remote for the Orbcontrol calculation'
+                    self.control_end_wc(error)
+                    return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
+                if 'fleurinp' in inputs:
+                    error = 'ERROR: you gave relaxed remotes + fleurinp for the Orbcontrol calculation'
+                    self.control_end_wc(error)
+                    return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
+                self.ctx.skip_fixed_calculations = True
             if 'remote' in inputs:
                 remote = inputs.remote
             if 'fleurinp' in inputs:
                 fleurinp = inputs.fleurinp
 
         if fleurinp is not None:
             modes = fleurinp.get_fleur_modes()
@@ -456,14 +535,20 @@
 
     def scf_no_ldau_needed(self):
         """
         Returns whether to run an additional scf workchain before adding LDA+U
         """
         return self.ctx.scf_no_ldau_needed
 
+    def run_fixed_calculations(self):
+        """
+        Returns whether to run frozen density matrix calculations
+        """
+        return not self.ctx.skip_fixed_calculations
+
     def converge_scf_no_ldau(self):
         """
         Launch fleur.scf for the system without LDA+U
         """
         inputs = self.get_inputs_scf_no_ldau()
 
         self.report('Info: Run SCF without LDA+U')
@@ -606,46 +691,60 @@
                 return {}, self.exit_codes.ERROR_SCF_NOLDAU_FAILED
         elif self.ctx.inpgen_needed:
             if not self.ctx.inpgen.is_finished_ok:
                 error = 'Inpgen calculation failed'
                 self.control_end_wc(error)
                 return {}, self.exit_codes.ERROR_INPGEN_CALCULATION_FAILED
             try:
-                fleurinp = self.ctx.inpgen.outputs.fleurinpData
+                fleurinp = self.ctx.inpgen.outputs.fleurinp
             except (AttributeError, NotExistent):
                 return {}, self.exit_codes.ERROR_INPGEN_CALCULATION_FAILED
         else:
             if 'remote' in self.inputs:
                 remote_data = self.inputs.remote
+            if 'fixed_remotes' in self.inputs and \
+                f'Fixed_{index}' in self.inputs.fixed_remotes:
+                self.report(f'INFO: overwriting remote folder with given fixed remote for configuration {index}')
+                remote_data = self.inputs.fixed_remotes[f'Fixed_{index}']
+
             if 'fleurinp' not in self.inputs:
                 fleurinp = get_fleurinp_from_remote_data(remote_data, store=True)
                 self.report(
                     f'INFO: generated FleurinpData from {fleurinp.files} from remote folder pk={remote_data.pk}')
             else:
                 fleurinp = self.inputs.fleurinp
 
         inputs = self.inputs
 
         label = f'Fixed_{index}'
         description = f'LDA+U with fixed nmmpmat for config {index}'
 
-        if 'settings' not in inputs:
-            settings = {}
-        else:
+        settings = {}
+        if 'settings' in inputs:
             settings = inputs.settings.get_dict()
         settings.setdefault('remove_from_remotecopy_list', []).append('mixing_history*')
 
         self.report(f'INFO: create fleurinp for config {index}')
         fm = FleurinpModifier(fleurinp)
         modes = fleurinp.get_fleur_modes()
 
         fm.set_inpchanges({'itmax': self.ctx.wf_dict['iterations_fixed'], 'l_linMix': True, 'mixParam': 0.0})
 
+        fchanges = self.ctx.wf_dict['inpxml_changes']
+        if fchanges:
+            try:
+                fm.add_task_list(fchanges)
+            except (ValueError, TypeError) as exc:
+                error = ('ERROR: Changing the inp.xml file failed. Tried to apply inpxml_changes'
+                         f', which failed with {exc}. I abort, good luck next time!')
+                self.control_end_wc(error)
+                return {}, self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
+
         for atom_species, ldau_dict in self.ctx.wf_dict['ldau_dict'].items():
-            fm.set_species(species_name=atom_species, attributedict={'ldaU': ldau_dict})
+            fm.set_species(atom_species, {'ldaU': ldau_dict})
 
         for config_index, config_species in config.items():
             orbital = config_index.split('-')[-1]
             atom_species = '-'.join(config_index.split('-')[:-1])
 
             if len(config_species) == 2 and modes['jspin'] == 1:
                 self.report(f'Configuration for species {atom_species} is given spin-polarized, '
@@ -660,24 +759,14 @@
                                    orbital_occupations=config_spin)
                 else:
                     fm.set_nmmpmat(species_name=atom_species,
                                    orbital=int(orbital),
                                    spin=spin + 1,
                                    state_occupations=config_spin)
 
-        fchanges = self.ctx.wf_dict['inpxml_changes']
-        if fchanges:
-            try:
-                fm.add_task_list(fchanges)
-            except (ValueError, TypeError) as exc:
-                error = ('ERROR: Changing the inp.xml file failed. Tried to apply inpxml_changes'
-                         f', which failed with {exc}. I abort, good luck next time!')
-                self.control_end_wc(error)
-                return {}, self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
-
         try:
             fm.show(display=False, validate=True)
         except etree.DocumentInvalid:
             self.control_end_wc('ERROR: input, inp.xml changes did not validate')
             return {}, self.exit_codes.ERROR_INVALID_INPUT_FILE
         except ValueError as exc:
             error = ('ERROR: input, inp.xml changes could not be applied.'
@@ -689,42 +778,51 @@
 
         input_fixed = get_inputs_fleur(inputs.fleur,
                                        remote_data,
                                        fleurinp_fixed,
                                        self.ctx.options,
                                        label,
                                        description,
-                                       settings=settings)
+                                       settings=settings,
+                                       add_comp_para=self.ctx.wf_dict['add_comp_para'])
 
         return input_fixed, None
 
     def converge_scf(self):
         """
         Launch fleur.scf after the fixed density matrix calculations to relax the density matrix
         """
         self.report('INFO: Relax density matrices')
         for index, config in enumerate(self.ctx.fixed_configurations):
 
             inputs = self.get_inputs_scf()
-            fixed_calc = self.ctx[f'Fixed_{index}']
 
-            if not fixed_calc.is_finished_ok:
-                message = f'One Base workflow (fixed nmmpmat) failed: {index}'
-                self.ctx.warnings.append(message)
-                continue
+            if self.ctx.skip_fixed_calculations:
+                if f'Relaxed_{index}' not in self.inputs.relaxed_remotes:
+                    self.report(f'INFO: Skipping configuration {index}')
+                    continue
+                inputs.remote_data = self.inputs.relaxed_remotes[f'Relaxed_{index}']
+            else:
 
-            try:
-                fixed_calc.outputs.output_parameters
-            except NotExistent:
-                message = f'One Base workflow (fixed nmmpmat) failed, no output node: {index}. I skip this one.'
-                self.ctx.errors.append(message)
-                continue
+                fixed_calc = self.ctx[f'Fixed_{index}']
 
-            inputs.fleurinp = fixed_calc.inputs.fleurinpdata
-            inputs.remote_data = fixed_calc.outputs.remote_folder
+                if not fixed_calc.is_finished_ok:
+                    message = f'One Base workflow (fixed nmmpmat) failed: {index}'
+                    self.ctx.warnings.append(message)
+                    continue
+
+                try:
+                    fixed_calc.outputs.output_parameters
+                except NotExistent:
+                    message = f'One Base workflow (fixed nmmpmat) failed, no output node: {index}. I skip this one.'
+                    self.ctx.errors.append(message)
+                    continue
+
+                inputs.fleurinp = fixed_calc.inputs.fleurinp
+                inputs.remote_data = fixed_calc.outputs.remote_folder
 
             label = f'Relaxed_{index}'
             inputs.setdefault('metadata', {})['call_link_label'] = label
             res = self.submit(FleurScfWorkChain, **inputs)
             res.label = label
             res.description = f'DFT+U calculation for configuration number {index} converging the density matrix'
             self.to_context(**{label: res})
@@ -746,54 +844,66 @@
             input_scf.options = self.inputs.options
 
         if 'settings' not in input_scf:
             settings = {}
         else:
             settings = input_scf.settings.get_dict()
         settings.setdefault('remove_from_remotecopy_list', []).append('mixing_history*')
+        input_scf.settings = Dict(settings)
 
-        if 'wf_parameters' not in input_scf:
-            scf_wf_dict = {}
-        else:
-            scf_wf_dict = input_scf.wf_parameters.get_dict()
+        scf_wf_parameters = {}
+        if 'wf_parameters' in input_scf:
+            scf_wf_parameters = input_scf.wf_parameters.get_dict()
+        scf_wf_parameters['stop_if_last_distance_exceeds'] = self.ctx.wf_dict['distance_cutoff_relaxed']
 
-        scf_wf_dict.setdefault('inpxml_changes', []).append(('set_inpchanges', {
-            'change_dict': {
-                'l_linMix': False,
-            }
-        }))
+        with inpxml_changes(scf_wf_parameters) as fm:
+            fm.set_inpchanges({'l_linmix': False})
 
-        input_scf.wf_parameters = Dict(dict=scf_wf_dict)
-        input_scf.settings = Dict(dict=settings)
+        input_scf.wf_parameters = Dict(scf_wf_parameters)
+        input_scf.settings = Dict(settings)
 
         return input_scf
 
     def return_results(self):
         """
         return the results of the relaxed DFT+U calculations (scf workchains)
         """
         distancelist = []
         t_energylist = []
         failed_configs = []
+        skipped_configs = []
         non_converged_configs = []
         configs_list = []
         outnodedict = {}
         e_u = 'htr'
         dis_u = 'me/bohr^3'
         for index, config in enumerate(self.ctx.fixed_configurations):
             if f'Relaxed_{index}' in self.ctx:
                 calc = self.ctx[f'Relaxed_{index}']
-            else:
+            elif not self.ctx.skip_fixed_calculations:
                 message = (f'One SCF workflow was not run because the fixed calculation failed: Relaxed_{index}')
                 self.ctx.warnings.append(message)
                 self.ctx.successful = False
                 failed_configs.append(index)
                 t_energylist.append(None)
                 distancelist.append(None)
                 continue
+            elif f'Relaxed_{index}' in self.inputs.relaxed_remotes:
+                message = (f'One SCF workflow was not run for unknown reasons: Relaxed_{index}')
+                self.ctx.warnings.append(message)
+                self.ctx.successful = False
+                failed_configs.append(index)
+                t_energylist.append(None)
+                distancelist.append(None)
+                continue
+            else:
+                skipped_configs.append(index)
+                t_energylist.append(None)
+                distancelist.append(None)
+                continue
 
             if not calc.is_finished_ok:
                 message = f'One SCF workflow was not successful: Relaxed_{index}'
                 self.ctx.warnings.append(message)
                 self.ctx.successful = False
                 #We dont skip simply non-converged calculations
                 #because we want to try to exctract the total_energy
@@ -838,51 +948,89 @@
             t_e = outpara.get('total_energy', None)
             e_u = outpara.get('total_energy_units', 'htr')
             dis = outpara.get('distance_charge', None)
             dis_u = outpara.get('distance_charge_units', 'me/bohr^3')
             t_energylist.append(t_e)
             distancelist.append(dis)
             configs_list.append(index)
+        converged_configs = [index for index in configs_list if index not in non_converged_configs]
 
         out = {
             'workflow_name': self.__class__.__name__,
             'workflow_version': self._workflowversion,
             'configurations': self.ctx.fixed_configurations,
             'total_energy': t_energylist,
             'total_energy_units': e_u,
             'distance_charge': distancelist,
             'distance_charge_units': dis_u,
             'successful_configs': configs_list,
+            'converged_configs': converged_configs,
             'non_converged_configs': non_converged_configs,
             'failed_configs': failed_configs,
+            'skipped_configs': skipped_configs,
             'groundstate_configuration': None,
             'info': self.ctx.info,
             'warnings': self.ctx.warnings,
             'errors': self.ctx.errors
         }
 
         if self.ctx.successful:
             self.report('Done, Orbital occupation control calculation complete')
-        elif len(t_energylist) != 0:
+        elif any(e is not None for e in t_energylist):
             self.report('Done, but something went wrong.... Probably some individual calculation failed or'
                         ' a scf-cycle did not reach the desired distance.')
         else:
             self.report('Done, but something went wrong.... All Calculations failed. Probably something is'
                         ' wrong in your setup')
 
         #Find the minimal total energy in the list
-        if len(t_energylist) != 0:
-            groundstate_index = np.nanargmin(np.array(t_energylist, dtype=np.float))
-            out['groundstate_configuration'] = groundstate_index
-
-            if f'Relaxed_{groundstate_index}' in self.ctx:
-                groundstate_scf = self.ctx[f'Relaxed_{groundstate_index}']
-                self.out_many(self.exposed_outputs(groundstate_scf, FleurScfWorkChain, namespace='groundstate_scf'))
+        if any(e is not None for e in t_energylist):
+            energy = np.array(t_energylist, dtype=float)
 
-        outnode = Dict(dict=out)
+            converged_mask = np.ones(energy.size, dtype=bool)
+            converged_mask[non_converged_configs] = False
+            converged_mask[failed_configs] = False
+            converged_mask[skipped_configs] = False
+
+            non_converged_mask = np.ones(energy.size, dtype=bool)
+            non_converged_mask[converged_configs] = False
+            non_converged_mask[failed_configs] = False
+            non_converged_mask[skipped_configs] = False
+
+            if len(energy[converged_mask]) != 0:
+                converged_minimum_energy = np.nanmin(energy[converged_mask])
+                if len(energy[non_converged_mask]) != 0:
+                    if np.nanmin(energy[non_converged_mask]) < converged_minimum_energy:
+                        lower_non_converged = np.array(non_converged_configs)[energy[non_converged_mask] <
+                                                                              converged_minimum_energy]
+                        out['warnings'].extend(f"Configuration 'Relaxed_{index}' did not converge "
+                                               'but is lower in energy than the lowest converged configuration'
+                                               for index in lower_non_converged)
+
+                #Replace the non-converged calculations with NaN
+                #If we were to simply do np.nanargmin(energy[converged_mask])
+                #The index will no longer match up with the complete list
+                energy[~converged_mask] = np.nan
+                groundstate_index = np.nanargmin(energy)
+                out['groundstate_configuration'] = groundstate_index
+
+                if f'Relaxed_{groundstate_index}' in self.ctx:
+                    groundstate_scf = self.ctx[f'Relaxed_{groundstate_index}']
+                    self.out_many(self.exposed_outputs(groundstate_scf, FleurScfWorkChain, namespace='groundstate_scf'))
+
+                    #Retrieve the nmmpmat file and provide it as an singlefiledata output
+                    retrieved = groundstate_scf.outputs.last_calc.retrieved
+                    nmmp_node = extract_nmmp_file(retrieved)
+                    if not isinstance(nmmp_node, ExitCode):
+                        self.out('groundstate_denmat', nmmp_node)
+                    else:
+                        self.report(
+                            'Something went wrong. The groundstate SCF calculation contains no density matrix file')
+
+        outnode = Dict(out)
         outnodedict['results_node'] = outnode
 
         # create links between all these nodes...
         outputnode_dict = create_orbcontrol_result_node(**outnodedict)
 
         outputnode = outputnode_dict.get('output_orbcontrol_wc_para')
         outputnode.label = 'output_orbcontrol_wc_para'
@@ -893,17 +1041,17 @@
 
         outputscf = outputnode_dict.get('output_orbcontrol_wc_gs_scf', None)
         if outputscf:
             outputscf.label = 'output_orbcontrol_wc_gs_scf'
             outputscf.description = ('SCF output from the run with the lowest total '
                                      'energy extracted from FleurOrbControlWorkChain')
 
-        if all(e is None for e in t_energylist):
+        if all(e is None for e in t_energylist) or out.get('groundstate_configuration') is None:
             return self.exit_codes.ERROR_ALL_CONFIGS_FAILED
-        elif not self.ctx.successful:
+        if not self.ctx.successful:
             return self.exit_codes.ERROR_SOME_CONFIGS_FAILED
 
     def control_end_wc(self, errormsg):
         """
         Controlled way to shutdown the workchain. It will initialize the output nodes
         The shutdown of the workchain will has to be done afterwards
         """
@@ -936,7 +1084,33 @@
 
     if f'configuration_{groundstate_index}' in kwargs:
         outdict['output_orbcontrol_wc_gs_scf'] = kwargs[f'configuration_{groundstate_index}'].clone()
     if f'fleurinp_{groundstate_index}' in kwargs:
         outdict['output_orbcontrol_wc_gs_fleurinp'] = kwargs[f'fleurinp_{groundstate_index}'].clone()
 
     return outdict
+
+
+@cf
+def extract_nmmp_file(folder):
+    """
+    Extract the density matrix file from the given folder data
+
+    :raises: ExitCode 300, No density matrix file found
+    """
+    filenames = folder.list_object_names()
+
+    nmmp_filename = None
+    if FleurCalculation._NMMPMAT_FILE_NAME in filenames:
+        nmmp_filename = FleurCalculation._NMMPMAT_FILE_NAME
+    elif FleurCalculation._NMMPMAT_HDF5_FILE_NAME in filenames:
+        nmmp_filename = FleurCalculation._NMMPMAT_HDF5_FILE_NAME
+
+    if nmmp_filename is None:
+        return ExitCode(300, message='FolderData has no density matrix file')
+
+    with folder.open(nmmp_filename, 'rb') as nmmp_file:
+        nmmp_node = orm.SinglefileData(nmmp_file, filename=FleurCalculation._NMMPMAT_FILE_NAME)
+
+    nmmp_node.label = 'groundstate_denmat'
+    nmmp_node.description = 'Converged density matrix file calculated in the orbcontrol workchain'
+    return nmmp_node
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/relax.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/relax.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,32 +12,31 @@
     In this module you find the workflow 'FleurRelaxWorkChain' for geometry optimization.
 """
 import copy
 import numpy as np
 
 from aiida.engine import WorkChain, ToContext, while_, if_
 from aiida.engine import calcfunction as cf
-from aiida.orm import load_node
 from aiida.orm import StructureData, Dict
 from aiida.common import AttributeDict
 from aiida.common.exceptions import NotExistent
 
 from aiida_fleur.workflows.scf import FleurScfWorkChain
 from aiida_fleur.workflows.base_fleur import FleurBaseWorkChain
 from aiida_fleur.data.fleurinp import FleurinpData
-from aiida_fleur.common.constants import BOHR_A
+from aiida_fleur.data.fleurinpmodifier import inpxml_changes
 from aiida_fleur.tools.StructureData_util import break_symmetry_wf
 
 
 class FleurRelaxWorkChain(WorkChain):
     """
     This workflow performs structure optimization.
     """
 
-    _workflowversion = '0.4.0'
+    _workflowversion = '0.5.0'
 
     _default_wf_para = {
         'relax_iter': 5,  # Stop if not converged after so many relaxation steps
         'film_distance_relaxation': False,  # Do not relax the z coordinates
         'force_criterion': 0.001,  # Converge the force until lower this value in atomic units
         'run_final_scf': False,  # Run a final scf on the final relaxed structure
         'break_symmetry': False,  # Break the symmetry for the relaxation each atom own type
@@ -180,16 +179,15 @@
         This allows to call the workchain to run an scf only and makes
         logic of other higher workflows a lot easier
         """
         relaxtype = self.ctx.wf_dict.get('relaxation_type', 'atoms')
         if relaxtype is None:
             self.ctx.reached_relax = True
             return False
-        else:
-            return True
+        return True
 
     def converge_scf(self):
         """
         Submits :class:`aiida_fleur.workflows.scf.FleurScfWorkChain`.
         """
         inputs = {}
         if self.ctx.loop_count:
@@ -208,70 +206,48 @@
         input_scf.metadata.description = 'The SCF workchain converging forces, part of the Relax'
 
         if self.ctx.wf_dict['break_symmetry']:
             calc_para = None
             if 'calc_parameters' in input_scf:
                 calc_para = input_scf.calc_parameters
             # currently we always break the full symmetry
-            break_dict = Dict(dict={'atoms': ['all']})  # for provenance
+            break_dict = Dict({'atoms': ['all']})  # for provenance
             broken_sys = break_symmetry_wf(input_scf.structure, wf_para=break_dict, parameterdata=calc_para)
             input_scf.structure = broken_sys['new_structure']
             input_scf.calc_parameters = broken_sys['new_parameters']
 
         if 'wf_parameters' not in input_scf:
             scf_wf_dict = {}
         else:
             scf_wf_dict = input_scf.wf_parameters.get_dict()
+        scf_wf_dict['mode'] = 'force'
 
-        if 'inpxml_changes' not in scf_wf_dict:
-            scf_wf_dict['inpxml_changes'] = []
+        with inpxml_changes(scf_wf_dict) as fm:
+            if self.ctx.wf_dict['film_distance_relaxation']:
+                fm.set_atomgroup({'force': {'relaxXYZ': 'FFT'}}, species='all')
 
-        scf_wf_dict['mode'] = 'force'
+            for specie_off in self.ctx.wf_dict['atoms_off']:
+                fm.set_atomgroup_label(specie_off, {'force': {'relaxXYZ': 'FFF'}})
 
-        if self.ctx.wf_dict['film_distance_relaxation']:
-            scf_wf_dict['inpxml_changes'].append(('set_atomgroup', {
-                'attributedict': {
-                    'force': {
-                        'relaxXYZ': 'FFT'
-                    }
-                },
-                'species': 'all'
-            }))
-
-        for specie_off in self.ctx.wf_dict['atoms_off']:
-            scf_wf_dict['inpxml_changes'].append(('set_atomgroup_label', {
-                'attributedict': {
-                    'force': {
-                        'relaxXYZ': 'FFF'
-                    }
-                },
-                'atom_label': specie_off
-            }))
-
-        scf_wf_dict['inpxml_changes'].append(('set_atomgroup_label', {
-            'attributedict': {
-                'force': {
-                    'relaxXYZ': 'FFF'
-                }
-            },
-            'atom_label': '49999'
-        }))
+            fm.set_atomgroup_label('49999', {'force': {'relaxXYZ': 'FFF'}})
 
-        input_scf.wf_parameters = Dict(dict=scf_wf_dict)
+        input_scf.wf_parameters = Dict(scf_wf_dict)
 
         return input_scf
 
     def get_inputs_scf(self):
         """
         Initializes inputs for further iterations.
         """
         input_scf = AttributeDict(self.exposed_inputs(FleurScfWorkChain, namespace='scf'))
         if 'structure' in input_scf:
             del input_scf.structure
+        if 'inpgen' in input_scf:
             del input_scf.inpgen
+        if 'calc_parameters' in input_scf:
             del input_scf.calc_parameters
 
         if 'wf_parameters' not in input_scf:
             scf_wf_dict = {}
         else:
             scf_wf_dict = input_scf.wf_parameters.get_dict()
             if 'inpxml_changes' in scf_wf_dict:
@@ -279,15 +255,15 @@
                 new_changes = []
                 for change in old_changes:
                     if 'shift_value' not in change[0]:
                         new_changes.append(change)
                 scf_wf_dict['inpxml_changes'] = new_changes
 
         scf_wf_dict['mode'] = 'force'
-        input_scf.wf_parameters = Dict(dict=scf_wf_dict)
+        input_scf.wf_parameters = Dict(scf_wf_dict)
 
         scf_wc = self.ctx.scf_res
         input_scf.remote_data = scf_wc.outputs.last_calc.remote_folder
         if self.ctx.new_fleurinp:
             input_scf.fleurinp = self.ctx.new_fleurinp
 
         return input_scf
@@ -306,15 +282,15 @@
         if not scf_wc.is_finished_ok:
             exit_statuses = FleurScfWorkChain.get_exit_statuses(['ERROR_FLEUR_CALCULATION_FAILED'])
             if scf_wc.exit_status == exit_statuses[0]:
                 fleur_calc = scf_wc.outputs.last_calc.remote_folder.creator
                 if fleur_calc.exit_status == FleurBaseWorkChain.get_exit_statuses(['ERROR_VACUUM_SPILL_RELAX'])[0]:
                     self.control_end_wc('ERROR: Failed due to atom and vacuum overlap')
                     return self.exit_codes.ERROR_VACUUM_SPILL_RELAX
-                elif fleur_calc.exit_status == FleurBaseWorkChain.get_exit_statuses(['ERROR_MT_RADII_RELAX'])[0]:
+                if fleur_calc.exit_status == FleurBaseWorkChain.get_exit_statuses(['ERROR_MT_RADII_RELAX'])[0]:
                     self.control_end_wc('ERROR: Failed due to MT overlap')
                     return self.exit_codes.ERROR_MT_RADII_RELAX
             return self.exit_codes.ERROR_SCF_FAILED
 
     def condition(self):
         """
         Checks if relaxation criteria is achieved.
@@ -337,20 +313,27 @@
             for force in forces_data:
                 all_forces.extend(force[-3:])
             all_forces = [abs(x) for x in all_forces]
             self.ctx.forces.append(max(all_forces))
 
         largest_now = self.ctx.forces[-1]
 
+        # get force mixing (straight or BFGS) setting
+        # defaults to stright mixing if not set in scf.wf_parameters
+        if 'wf_parameters' in self.inputs.scf:
+            force_dict = self.inputs.scf.wf_parameters.get_dict().get('force_dict', {})
+            force_strmix = force_dict.get('forcemix', 'straight') == 'straight'
+        else:
+            force_strmix = True
+
         if largest_now < self.ctx.wf_dict['force_criterion']:
             self.report(f'INFO: Structure is converged to the largest force {self.ctx.forces[-1]}')
             self.ctx.reached_relax = True
             return False
-        elif largest_now < self.ctx.wf_dict['change_mixing_criterion'] and self.inputs.scf.wf_parameters['force_dict'][
-                'forcemix'] == 'straight':
+        if largest_now < self.ctx.wf_dict['change_mixing_criterion'] and force_strmix:
             self.report(f'INFO: Seems it is safe to switch to BFGS. Current largest force: {self.ctx.forces[-1]}')
             self.ctx.switch_bfgs = True
             return False
 
         self.ctx.loop_count = self.ctx.loop_count + 1
         if self.ctx.loop_count == self.ctx.wf_dict['relax_iter']:
             self.report('INFO: Reached optimization iteration number {}. Largest force is {}, '
@@ -424,15 +407,15 @@
                     new_changes = []
                     for change in old_changes:
                         if 'shift_value' not in change[0]:
                             new_changes.append(change)
                     scf_wf_dict['inpxml_changes'] = new_changes
 
             scf_wf_dict['mode'] = 'density'
-            input_final_scf.wf_parameters = Dict(dict=scf_wf_dict)
+            input_final_scf.wf_parameters = Dict(scf_wf_dict)
         structure = self.ctx.final_structure
         formula = structure.get_formula()
         input_final_scf.structure = structure
         input_final_scf.fleur = input_scf.fleur
         input_final_scf.metadata.label = f'SCF_final_{formula}'
         input_final_scf.metadata.description = ('Final SCF workchain running on optimized structure {}, '
                                                 'part of relax workchain'.format(formula))
@@ -467,15 +450,15 @@
                 pass
             self.ctx.final_structure = structure
             self.ctx.final_cell = structure.cell
             # The others are already put to None
             return
 
         try:
-            relax_out = self.ctx.scf_res.outputs.last_fleur_calc_output
+            relax_out = self.ctx.scf_res.outputs.last_calc.output_parameters
             retrieved_node = self.ctx.scf_res.outputs.last_calc.retrieved
         except NotExistent:
             return self.exit_codes.ERROR_NO_SCF_OUTPUT
 
         relax_out = relax_out.get_dict()
 
         try:
@@ -496,15 +479,15 @@
 
     def get_results_final_scf(self):
         """
         Parser some results of final scf
         """
 
         try:
-            scf_out = self.ctx.scf_final_res.outputs.last_fleur_calc_output
+            scf_out = self.ctx.scf_final_res.outputs.last_calc.output_parameters
         except NotExistent:
             return self.exit_codes.ERROR_NO_SCF_OUTPUT
 
         scf_out_d = scf_out.get_dict()
         try:
             total_energy = scf_out_d['energy']
             total_energy_units = scf_out_d['energy_units']
@@ -538,33 +521,30 @@
             'energy': self.ctx.total_energy_last,
             'energy_units': self.ctx.total_energy_units,
             'info': self.ctx.info,
             'warnings': self.ctx.warnings,
             'errors': self.ctx.errors,
             'force': self.ctx.forces,
             'force_iter_done': self.ctx.loop_count,
-            # uuids in the output are bad for caching should be avoided,
-            # instead better return the node.
-            'last_scf_wc_uuid': self.ctx.scf_res.uuid,
             'total_magnetic_moment_cell': self.ctx.total_magnetic_moment,
             'total_magnetic_moment_cell_units': 'muBohr'
         }
-        outnode = Dict(dict=out)
+        outnode = Dict(out)
 
         con_nodes = {}
         try:
-            relax_out = self.ctx.scf_res.outputs.last_fleur_calc_output
+            relax_out = self.ctx.scf_res.outputs.last_calc.output_parameters
         except NotExistent:
             relax_out = None
         if relax_out is not None:
             con_nodes['last_fleur_calc_output'] = relax_out
 
         if all([self.ctx.wf_dict.get('run_final_scf', False), self.ctx.reached_relax]):
             try:
-                scf_out = self.ctx.scf_final_res.outputs.last_fleur_calc_output
+                scf_out = self.ctx.scf_final_res.outputs.last_calc.output_parameters
             except NotExistent:
                 scf_out = None
             if relax_out is not None:
                 con_nodes['last_scf__output'] = scf_out
 
         # TODO: for a trajectory output node all corresponding nodes have to go into
         # con_nodes
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/scf.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/scf.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 cycle management of a FLEUR calculation with AiiDA.
 """
 # TODO: more info in output, log warnings
 # TODO: make smarter, ggf delete mixing_history or restart with more or less iterations
 # you can use the pattern of the density convergence for this
 # TODO: maybe write dict schema for wf_parameter inputs, how?
 from lxml import etree
+from copy import deepcopy
 
 from aiida.orm import Code, load_node
 from aiida.orm import StructureData, RemoteData, Dict, Bool, Float
 from aiida.engine import WorkChain, while_, if_, ToContext
 from aiida.engine import calcfunction as cf
 from aiida.common.exceptions import NotExistent
 
 from aiida_fleur.data.fleurinpmodifier import FleurinpModifier
 from aiida_fleur.tools.common_fleur_wf import get_inputs_fleur, get_inputs_inpgen
 from aiida_fleur.tools.common_fleur_wf import test_and_get_codenode
-from aiida_fleur.tools.common_fleur_wf import find_last_submitted_calcjob
 from aiida_fleur.tools.create_kpoints_from_distance import create_kpoints_from_distance_parameter
 from aiida_fleur.workflows.base_fleur import FleurBaseWorkChain
+from aiida_fleur.calculation.fleur import FleurCalculation
 
-from aiida_fleur.data.fleurinp import FleurinpData, get_fleurinp_from_remote_data
+from aiida_fleur.data.fleurinp import FleurinpData, get_fleurinp_from_remote_data_cf
 
 from masci_tools.io.parsers.fleur import outxml_parser
 
 
 class FleurScfWorkChain(WorkChain):
     """
     Workchain for converging a FLEUR calculation (SCF).
@@ -54,40 +55,43 @@
     :param inpgen: (Code)
     :param fleur: (Code)
 
     :return: output_scf_wc_para (Dict), Information of workflow results
         like Success, last result node, list with convergence behavior
     """
 
-    _workflowversion = '0.5.1'
+    _workflowversion = '0.6.3'
     _default_wf_para = {
         'fleur_runmax': 4,
         'density_converged': 0.00002,
+        'stop_if_last_distance_exceeds': None,
         'energy_converged': 0.002,
         'force_converged': 0.002,
+        'torque_converged': 0.0002,
         'kpoints_distance': None,  # in 1/A, usually 0.1
         'kpoints_force_parity': False,
         'kpoints_force_odd': False,
-        'kpoints_force_false': False,
+        'kpoints_force_even': False,
         'kpoints_force_gamma': False,
         'nmmp_converged': 0.002,
-        'mode': 'density',  # 'density', 'energy' or 'force'
+        'mode': 'density',  # 'density', 'energy', 'force' or 'gw'
         'add_comp_para': {
             'only_even_MPI': False,
             'max_queue_nodes': 20,
             'max_queue_wallclock_sec': 86400
         },
         'itmax_per_run': 30,
         'force_dict': {
             'qfix': 2,
             'forcealpha': 1.0,
             'forcemix': 'straight'
         },
         'use_relax_xml': False,
         'inpxml_changes': [],
+        'drop_mixing_first_iteration': True,
         'straight_iterations': None,
         'initial_straight_mixing': False,
         'initial_ldau_straight_mixing': False,
         'initial_ldau_straight_mix_param': 0.0,  #Density matrix frozen by default, since it is the most stable option
     }
 
     _default_options = {
@@ -118,15 +122,14 @@
         spec.input('settings_inpgen', valid_type=Dict, required=False)
         spec.outline(cls.start, cls.validate_input,
                      if_(cls.fleurinpgen_needed)(cls.run_fleurinpgen), cls.run_fleur, cls.inspect_fleur, cls.get_res,
                      while_(cls.condition)(cls.run_fleur, cls.inspect_fleur, cls.get_res), cls.return_results)
 
         spec.output('fleurinp', valid_type=FleurinpData)
         spec.output('output_scf_wc_para', valid_type=Dict)
-        spec.output('last_fleur_calc_output', valid_type=Dict)
         spec.expose_outputs(FleurBaseWorkChain, namespace='last_calc')
 
         # exit codes
         spec.exit_code(230, 'ERROR_INVALID_INPUT_PARAM', message='Invalid workchain parameters.')
         spec.exit_code(231, 'ERROR_INVALID_INPUT_CONFIG', message='Invalid input configuration.')
         spec.exit_code(233,
                        'ERROR_INVALID_CODE_PROVIDED',
@@ -157,23 +160,26 @@
         wf_default = self._default_wf_para
         if 'wf_parameters' in self.inputs:
             wf_dict = self.inputs.wf_parameters.get_dict()
         else:
             wf_dict = wf_default
 
         for key, val in wf_default.items():
-            wf_dict[key] = wf_dict.get(key, val)
+            if isinstance(val, dict):
+                wf_dict[key] = {**val, **wf_dict.get(key, {})}
+            else:
+                wf_dict[key] = wf_dict.get(key, val)
         self.ctx.wf_dict = wf_dict
 
-        fleur = self.inputs.fleur
-        fleur_extras = fleur.extras
-        inpgen_extras = None
-        if 'inpgen' in self.inputs:
-            inpgen = self.inputs.inpgen
-            inpgen_extras = inpgen.extras
+        # fleur = self.inputs.fleur
+        # fleur_extras = fleur.extras
+        # inpgen_extras = None
+        # if 'inpgen' in self.inputs:
+        #     inpgen = self.inputs.inpgen
+        #     inpgen_extras = inpgen.extras
 
         defaultoptions = self._default_options.copy()
         user_options = {}
         if 'options' in self.inputs:
             user_options = self.inputs.options.get_dict()
         '''
         # extend options by code defaults given in code extras
@@ -193,31 +199,36 @@
         # and queue does not matter in case of direct scheduler
 
         # extend options given by user using defaults
         for key, val in defaultoptions.items():
             options[key] = options.get(key, val)
         self.ctx.options = options
 
-        self.ctx.max_number_runs = self.ctx.wf_dict.get('fleur_runmax', 4)
+        self.ctx.max_number_runs = self.ctx.wf_dict['fleur_runmax']
         self.ctx.description_wf = self.inputs.get('description', '') + '|fleur_scf_wc|'
         self.ctx.label_wf = self.inputs.get('label', 'fleur_scf_wc')
-        self.ctx.default_itmax = self.ctx.wf_dict.get('itmax_per_run', 30)
-        self.ctx.straight_mixing_iters = self.ctx.wf_dict.get('straight_iterations')
+        self.ctx.default_itmax = self.ctx.wf_dict['itmax_per_run']
+        self.ctx.straight_mixing_iters = self.ctx.wf_dict['straight_iterations']
         if self.ctx.straight_mixing_iters is None:
             self.ctx.straight_mixing_iters = self.ctx.default_itmax
 
         # return para/vars
         self.ctx.successful = True
         self.ctx.parse_last = True
         self.ctx.distance = []
         self.ctx.all_forces = []
         self.ctx.total_energy = []
         self.ctx.nmmp_distance = []
+        self.ctx.x_torques = []
+        self.ctx.y_torques = []
+        self.ctx.alpha_angles = []
+        self.ctx.beta_angles = []
         self.ctx.energydiff = 10000
         self.ctx.forcediff = 10000
+        self.ctx.torquediff = None
         self.ctx.last_charge_density = 10000
         self.ctx.last_nmmp_distance = -10000
         self.ctx.warnings = []
         # "debug": {},
         self.ctx.errors = []
         self.ctx.info = []
         self.ctx.possible_info = [
@@ -277,57 +288,57 @@
         else:
             error = 'ERROR: No StructureData nor FleurinpData nor RemoteData was provided'
             self.report(error)
             return self.exit_codes.ERROR_INVALID_INPUT_CONFIG
 
         if 'inpgen' in inputs:
             try:
-                test_and_get_codenode(inputs.inpgen, 'fleur.inpgen', use_exceptions=True)
+                test_and_get_codenode(inputs.inpgen, 'fleur.inpgen')
             except ValueError:
                 error = 'The code you provided for inpgen of FLEUR does not use the plugin fleur.inpgen'
                 self.report(error)
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
         if 'fleur' in inputs:
             try:
-                test_and_get_codenode(inputs.fleur, 'fleur.fleur', use_exceptions=True)
+                test_and_get_codenode(inputs.fleur, 'fleur.fleur')
             except ValueError:
                 error = ('The code you provided for FLEUR does not use the plugin fleur.fleur')
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
         # check the mode in wf_dict
-        mode = self.ctx.wf_dict.get('mode')
-        if mode not in ['force', 'density', 'energy', 'gw']:
+        mode = self.ctx.wf_dict['mode']
+        if mode not in ['force', 'density', 'energy', 'spex', 'torque']:
             error = "ERROR: Wrong mode of convergence: one of 'force', 'density', 'energy' or 'gw' was expected."
             self.report(error)
             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
-        max_iters = self.ctx.wf_dict.get('itmax_per_run')
+        max_iters = self.ctx.wf_dict['itmax_per_run']
         if max_iters <= 1:
             error = "ERROR: 'itmax_per_run' should be equal at least 2"
             self.report(error)
             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
-        straight_iterations = self.ctx.wf_dict.get('straight_iterations')
+        straight_iterations = self.ctx.wf_dict['straight_iterations']
         if straight_iterations is not None and straight_iterations <= 1:
             error = "ERROR: 'straight_iterations' should be atleast 2 if given"
             self.report(error)
             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
-        self.ctx.run_straight_mixing = self.ctx.wf_dict.get('initial_straight_mixing') or \
-                                       self.ctx.wf_dict.get('initial_ldau_straight_mixing')
+        self.ctx.run_straight_mixing = self.ctx.wf_dict['initial_straight_mixing'] or \
+                                       self.ctx.wf_dict['initial_ldau_straight_mixing']
 
         if straight_iterations is not None:
             if not self.ctx.run_straight_mixing:
                 error = "ERROR: 'initial_straight_mixing' or 'initial_ldau_straight_mixing' should be True if 'straight_iterations' is given"
                 self.report(error)
                 return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
         # check format of inpxml_changes
-        fchanges = self.ctx.wf_dict.get('inpxml_changes', [])
+        fchanges = self.ctx.wf_dict['inpxml_changes']
         if fchanges:
             for change in fchanges:
                 # somehow the tuple type gets destroyed on the way and becomes a list
                 if not isinstance(change, (tuple, list)):
                     error = f'ERROR: Wrong Input inpxml_changes wrong format of: {change} should be tuple of 2. I abort'
                     self.report(error)
                     return self.exit_codes.ERROR_INVALID_INPUT_PARAM
@@ -360,24 +371,23 @@
 
         if 'settings_inpgen' in self.inputs:
             settings = self.inputs.settings_inpgen
         else:
             settings = None
 
         # If given kpt_dist has prio over given calc_parameters
-        kpt_dist = self.ctx.wf_dict.get('kpoints_distance', None)
+        kpt_dist = self.ctx.wf_dict['kpoints_distance']
         if kpt_dist is not None:
-            cf_para_kpt = Dict(
-                dict={
-                    'distance': kpt_dist,
-                    'force_parity': self.ctx.wf_dict.get('kpoints_force_parity', False),
-                    'force_even': self.ctx.wf_dict.get('kpoints_force_even', False),
-                    'force_odd': self.ctx.wf_dict.get('kpoints_force_odd', False),
-                    'include_gamma': self.ctx.wf_dict.get('kpoints_force_gamma', False)
-                })
+            cf_para_kpt = Dict({
+                'distance': kpt_dist,
+                'force_parity': self.ctx.wf_dict['kpoints_force_parity'],
+                'force_even': self.ctx.wf_dict['kpoints_force_even'],
+                'force_odd': self.ctx.wf_dict['kpoints_force_odd'],
+                'include_gamma': self.ctx.wf_dict['kpoints_force_gamma']
+            })
             inputs = {
                 'structure': structure,
                 'calc_parameters': params,
                 'cf_para': cf_para_kpt,
                 'metadata': {
                     'call_link_label': 'create_kpoints_from_distance'
                 }
@@ -413,17 +423,17 @@
 
         wf_dict = self.ctx.wf_dict
 
         fleurmode = FleurinpModifier(self.ctx.fleurinp)
 
         fleurmode.set_inpchanges({'itmax': self.ctx.default_itmax})
         #Take out straight mixing
-        if wf_dict.get('initial_straight_mixing'):
+        if wf_dict['initial_straight_mixing']:
             fleurmode.set_inpchanges({'imix': 'Anderson'})  #TODO: should take the actual value from before
-        if wf_dict.get('initial_ldau_straight_mixing'):
+        if wf_dict['initial_ldau_straight_mixing']:
             fleurmode.set_inpchanges({'l_linmix': False})
 
         # validate?
         try:
             fleurmode.show(display=False, validate=True)
         except etree.DocumentInvalid:
             error = ('ERROR: input, user wanted inp.xml changes did not validate')
@@ -448,81 +458,108 @@
         self.report('INFO: run change_fleurinp')
 
         inputs = self.inputs
 
         # Has to never crash because corresponding check was done in validate function
         if self.ctx.fleurinp:  # something was already changed
             return
-        elif 'fleurinp' in inputs:
+
+        if 'fleurinp' in inputs:
             fleurin = self.inputs.fleurinp
         elif 'structure' in inputs:
             if not self.ctx['inpgen'].is_finished_ok:
                 error = 'Inpgen calculation failed'
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INPGEN_CALCULATION_FAILED
-            fleurin = self.ctx['inpgen'].outputs.fleurinpData
+            fleurin = self.ctx['inpgen'].outputs.fleurinp
         elif 'remote_data' in inputs:
             # In this case only remote_data for input structure is given
             # fleurinp data has to be generated from the remote inp.xml file to use change_fleurinp
-            fleurin = get_fleurinp_from_remote_data(self.inputs.remote_data, store=True)
+            fleurin = get_fleurinp_from_remote_data_cf(self.inputs.remote_data)
             self.report(
                 f'INFO: generated FleurinpData from files {fleurin.files} from remote folder pk={self.inputs.remote_data.pk}'
             )
 
         wf_dict = self.ctx.wf_dict
-        force_dict = wf_dict.get('force_dict')
-        converge_mode = wf_dict.get('mode')
-        fchanges = wf_dict.get('inpxml_changes', [])
+        force_dict = wf_dict['force_dict']
+        converge_mode = wf_dict['mode']
+        fchanges = wf_dict['inpxml_changes']
 
         fleurmode = FleurinpModifier(fleurin)
 
         itmax = self.ctx.default_itmax
         if self.ctx.run_straight_mixing:
             if self.ctx.loop_count == 0:
                 #Set up straight mixing
                 itmax = self.ctx.straight_mixing_iters  #Is set further below
-                if wf_dict.get('initial_straight_mixing'):
+                if wf_dict['initial_straight_mixing']:
                     fleurmode.set_inpchanges({'imix': 'straight'})
-                if wf_dict.get('initial_ldau_straight_mixing'):
-                    fleurmode.set_inpchanges({
-                        'l_linmix': True,
-                        'mixParam': wf_dict.get('initial_ldau_straight_mix_param')
-                    })
+                if wf_dict['initial_ldau_straight_mixing']:
+                    fleurmode.set_inpchanges({'l_linmix': True, 'mixParam': wf_dict['initial_ldau_straight_mix_param']})
 
         # set proper convergence parameters in inp.xml
         if converge_mode == 'density':
-            dist = wf_dict.get('density_converged')
-            fleurmode.set_inpchanges({'itmax': itmax, 'minDistance': dist})
+            fleurmode.set_inpchanges({'itmax': itmax, 'minDistance': wf_dict['density_converged']})
         elif converge_mode == 'force':
-            force_converged = wf_dict.get('force_converged')
-            dist = wf_dict.get('density_converged')
             fleurmode.set_inpchanges({
                 'itmax': itmax,
-                'minDistance': dist,
-                'force_converged': force_converged,
+                'minDistance': wf_dict['density_converged'],
+                'force_converged': wf_dict['force_converged'],
                 'l_f': True,
-                'qfix': force_dict.get('qfix'),
-                'forcealpha': force_dict.get('forcealpha'),
-                'forcemix': force_dict.get('forcemix')
+                'qfix': force_dict['qfix'],
+                'forcealpha': force_dict['forcealpha'],
+                'forcemix': force_dict['forcemix']
             })
         elif converge_mode == 'energy':
-            dist = 0.0
-            fleurmode.set_inpchanges({'itmax': itmax, 'minDistance': dist})
+            fleurmode.set_inpchanges({'itmax': itmax, 'minDistance': 0.0})
 
-        elif converge_mode == 'gw':
-            dist = 0.0
-            fleurmode.set_inpchanges({'itmax': itmax, 'minDistance': dist, 'gw': 1})
-            if 'settings' in self.inputs:
-                self.inputs.settings.append({'additional_retrieve_list': ['basis.hdf', 'pot.hdf', 'ecore']})
-                self.inputs.settings.append({'additional_remotecopy_list': ['basis.hdf', 'pot.hdf', 'ecore']})
+        elif converge_mode == 'spex':
+            if fleurin.inp_version >= (0, 34):
+                fleurmode.set_inpchanges({'itmax': itmax, 'minDistance': 0.0, 'spex': 1})
             else:
-                self.inputs.settings = {
-                    'additional_retrieve_list': ['basis.hdf', 'pot.hdf', 'ecore'],
-                    'additional_remotecopy_list': ['basis.hdf', 'pot.hdf', 'ecore']
+                fleurmode.set_inpchanges({'itmax': itmax, 'minDistance': 0.0, 'gw': 1})
+        elif converge_mode == 'torque':
+            #TODO: Allow to select orbitals
+            dist = wf_dict.get('density_converged')
+            fleurmode.set_inpchanges({
+                'itmax': self.ctx.default_itmax,
+                'minDistance': dist,
+                'l_noco': True,
+                # 'numbands': 'all',
+                'ctail': False
+            })
+            fleurmode.set_complex_tag('greensFunction',
+                                      changes={
+                                          'realAxis': {
+                                              'ne': 5400,
+                                              'ellow': -1,
+                                              'elup': 1.0
+                                          },
+                                          'contourSemicircle': {
+                                              'n': 128,
+                                              'eb': -1.0,
+                                              'et': 0.0,
+                                              'alpha': 1.0
+                                          }
+                                      },
+                                      create=True)
+            fleurmode.set_species('all', {
+                'torqueCalculation': {
+                    'kkintgrCutoff': 'd',
+                    'greensfElements': {
+                        's': ['F', 'F', 'F', 'F'],
+                        'p': ['F', 'T', 'T', 'F'],
+                        'd': ['F', 'T', 'T', 'F'],
+                        'f': ['F', 'F', 'F', 'F']
+                    }
                 }
+            },
+                                  create=True)
+            fleurmode.set_attrib_value('l_mperp', True, tag_name='mtNocoParams')
+            fleurmode.set_attrib_value('l_mperp', True, tag_name='greensFunction')
 
         # apply further user dependend changes
         if fchanges:
             try:
                 fleurmode.add_task_list(fchanges)
             except (ValueError, TypeError) as exc:
                 error = ('ERROR: Changing the inp.xml file failed. Tried to apply inpxml_changes'
@@ -533,15 +570,15 @@
         # validate?
         try:
             fleurmode.show(display=False, validate=True)
         except etree.DocumentInvalid:
             error = ('ERROR: input, user wanted inp.xml changes did not validate')
             self.report(error)
             return self.exit_codes.ERROR_INVALID_INPUT_FILE
-        except ValueError as exc:
+        except (ValueError, TypeError) as exc:
             error = ('ERROR: input, user wanted inp.xml changes could not be applied.'
                      f'The following error was raised {exc}')
             self.control_end_wc(error)
             return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
 
         # apply
         out = fleurmode.freeze()
@@ -555,18 +592,26 @@
         self.report('INFO: run FLEUR')
 
         status = self.change_fleurinp()
         if status:
             return status
 
         if 'settings' in self.inputs:
-            settings = self.inputs.settings
+            settings = deepcopy(self.inputs.settings.get_dict())
         else:
             settings = None
 
+        if self.ctx.wf_dict['drop_mixing_first_iteration'] and self.ctx.loop_count == 0:
+            if settings is None:
+                settings = {}
+            remotecopy_list = settings.get('remove_from_remotecopy_list', [])
+            if 'mixing_history*' not in remotecopy_list:
+                remotecopy_list.append('mixing_history*')
+            settings['remove_from_remotecopy_list'] = remotecopy_list
+
         if self.ctx.run_straight_mixing and self.ctx.loop_count == 1:
             status = self.reset_straight_mixing()
             if status:
                 return status
 
             if settings is None:
                 settings = {}
@@ -630,34 +675,33 @@
             return self.exit_codes.ERROR_FLEUR_CALCULATION_FAILED
 
         exit_status = base_wc.exit_status
         if not base_wc.is_finished_ok:
             error = f'ERROR: Last Fleur calculation failed with exit status {exit_status}'
             self.control_end_wc(error)
             return self.exit_codes.ERROR_FLEUR_CALCULATION_FAILED
-        else:
-            self.ctx.parse_last = True
+
+        self.ctx.parse_last = True
 
     def get_res(self):
         """
         Check how the last Fleur calculation went
         Parse some results.
         """
         self.report('INFO: get results FLEUR')
 
         mode = self.ctx.wf_dict.get('mode')
         if self.ctx.parse_last:
             last_base_wc = self.ctx.last_base_wc
-            fleur_calcjob = load_node(find_last_submitted_calcjob(last_base_wc))
-            walltime = last_base_wc.outputs.output_parameters.dict.walltime
 
+            walltime = last_base_wc.outputs.output_parameters['walltime']
             if isinstance(walltime, int):
                 self.ctx.total_wall_time = self.ctx.total_wall_time + walltime
-            with fleur_calcjob.outputs.retrieved.open(fleur_calcjob.process_class._OUTXML_FILE_NAME,
-                                                      'rb') as outxmlfile:
+
+            with last_base_wc.outputs.retrieved.open(FleurCalculation._OUTXML_FILE_NAME, 'rb') as outxmlfile:
                 output_dict = outxml_parser(outxmlfile,
                                             minimal_mode=True,
                                             list_return=True,
                                             iteration_to_parse='all',
                                             ignore_validation=True)
 
             energies = output_dict.get('energy_hartree', [])
@@ -680,14 +724,38 @@
 
             if mode == 'force':
                 forces = output_dict.get('force_atoms', [])
                 if forces is not None:
                     for force_iter in forces:
                         self.ctx.all_forces.append([force for atom, force in force_iter])
 
+            if mode == 'torque':
+
+                with last_base_wc.outputs.retrieved.open(FleurCalculation._OUTXML_FILE_NAME, 'rb') as outxmlfile:
+                    output_dict_torque = outxml_parser(outxmlfile,
+                                                       iteration_to_parse='all',
+                                                       optional_tasks=['torques', 'noco_angles'],
+                                                       ignore_validation=True)
+
+                    x_torques = output_dict_torque.get('torque_x', [])
+                    y_torques = output_dict_torque.get('torque_y', [])
+                    if not isinstance(x_torques[0], list):  # only 1 iterations was done
+                        x_torques = [x_torques]
+                        y_torques = [y_torques]
+
+                    # extract angles from inp.xml because out.xml causes alpha and beta to jump
+                    # alpha_angles = output_dict_torque.get('noco_alpha', [])
+                    # beta_angles = output_dict_torque.get('noco_beta', [])
+                    alpha_angles = [x['nocoParams']['alpha'] for x in self.ctx.fleurinp.inp_dict['atomGroups']]
+                    beta_angles = [x['nocoParams']['beta'] for x in self.ctx.fleurinp.inp_dict['atomGroups']]
+
+                    self.ctx.x_torques.extend(x_torques)
+                    self.ctx.y_torques.extend(y_torques)
+                    self.ctx.alpha_angles = alpha_angles
+                    self.ctx.beta_angles = beta_angles
         else:
             errormsg = 'ERROR: scf wc was not successful, check log for details'
             self.control_end_wc(errormsg)
             return self.exit_codes.ERROR_FLEUR_CALCULATION_FAILED
 
         if not self.ctx.distance:
             # if fleur relaxes an already converged crystal it stops directly
@@ -702,85 +770,120 @@
             self.ctx.last_charge_density = self.ctx.distance[-1]
 
         if self.ctx.nmmp_distance:
             if isinstance(self.ctx.nmmp_distance[-1], list):
                 self.ctx.last_nmmp_distance = max(self.ctx.nmmp_distance[-1])
             else:
                 self.ctx.last_nmmp_distance = self.ctx.nmmp_distance[-1]
+            if self.ctx.last_nmmp_distance is None:
+                self.report('No LDA+U distance found but only one iteration performed\n'
+                            'Assuming that the calculatin should be continued')
+                self.ctx.last_nmmp_distance = self.ctx.wf_dict['nmmp_converged'] + 1
 
     def condition(self):
         """
         check convergence condition
         """
         self.report('INFO: checking condition FLEUR')
-        mode = self.ctx.wf_dict.get('mode')
+        mode = self.ctx.wf_dict['mode']
         ldau_notconverged = False
 
         energy = self.ctx.total_energy
         if len(energy) >= 2:
             self.ctx.energydiff = abs(energy[-1] - energy[-2])
 
         if mode == 'force':
             forces = self.ctx.all_forces
             if len(forces) >= 2:
                 self.ctx.forcediff = max(
                     abs(forces[-1][i][k] - forces[-2][i][k]) for i in range(len(forces[-1])) for k in range(3))
         else:
             self.ctx.forcediff = 'can not be determined'
 
+        if mode == 'torque':
+            x_torques = self.ctx.x_torques
+            y_torques = self.ctx.y_torques
+            if len(x_torques) > 1 and len(y_torques) > 1:
+                max_x_torque_diff = max(abs(x_torques[-1][i] - x_torques[-2][i]) for i in range(len(x_torques[0])))
+                max_y_torque_diff = max(abs(y_torques[-1][i] - y_torques[-2][i]) for i in range(len(y_torques[0])))
+                self.ctx.torquediff = max(max_x_torque_diff, max_y_torque_diff)
+            else:
+                self.ctx.torquediff = 'can not be determined'
+
         if self.ctx.last_nmmp_distance > 0.0 and \
-           self.ctx.last_nmmp_distance >= self.ctx.wf_dict.get('nmmp_converged'):
+           self.ctx.last_nmmp_distance >= self.ctx.wf_dict['nmmp_converged']:
             ldau_notconverged = True
 
         if mode == 'density':
-            if self.ctx.wf_dict.get('density_converged') >= self.ctx.last_charge_density:
+            if self.ctx.wf_dict['density_converged'] >= self.ctx.last_charge_density:
                 if not ldau_notconverged:
                     return False
-        elif mode in ('energy', 'gw'):
-            if self.ctx.wf_dict.get('energy_converged') >= self.ctx.energydiff:
+        elif mode in ('energy', 'spex'):
+            if self.ctx.wf_dict['energy_converged'] >= self.ctx.energydiff:
                 if not ldau_notconverged:
                     return False
         elif mode == 'force':
             if self.ctx.last_charge_density is None:
                 try:
                     _ = self.ctx.last_base_wc.outputs.relax_parameters
                 except NotExistent:
                     pass
                 else:
                     if not ldau_notconverged:
                         return False
 
-            elif self.ctx.wf_dict.get('density_converged') >= self.ctx.last_charge_density:
+            elif self.ctx.wf_dict['density_converged'] >= self.ctx.last_charge_density:
                 try:
                     _ = self.ctx.last_base_wc.outputs.relax_parameters
                 except NotExistent:
                     pass
                 else:
                     if not ldau_notconverged:
                         return False
+        elif mode == 'torque':
+            if self.ctx.torquediff == 'can not be determined' and self.ctx.wf_dict.get(
+                    'density_converged') >= self.ctx.last_charge_density:
+                if not ldau_notconverged:
+                    return False
+            elif self.ctx.wf_dict.get('torque_converged') >= self.ctx.torquediff:
+                if not ldau_notconverged:
+                    return False
 
         if self.ctx.loop_count >= self.ctx.max_number_runs:
             self.ctx.reached_conv = False
             return False
 
+        if self.ctx.wf_dict['stop_if_last_distance_exceeds'] is not None:
+            if mode == 'density' and \
+               self.ctx.last_charge_density >= self.ctx.wf_dict['stop_if_last_distance_exceeds']:
+
+                self.report(
+                    f'Stopping because last charge density distance {self.ctx.last_charge_density} me/bohr^3'
+                    f' of the last calculation exceeded the given limit of {self.ctx.wf_dict["stop_if_last_distance_exceeds"]} me/bohr^3'
+                )
+                self.ctx.reached_conv = False
+                return False
+            if mode in ('energy', 'spex') and \
+               self.ctx.energydiff >= self.ctx.wf_dict['stop_if_last_distance_exceeds']:
+
+                self.report(
+                    f'Stopping because last energy difference {self.ctx.energydiff} htr'
+                    f' of the last calculation exceeded the given limit of {self.ctx.wf_dict["stop_if_last_distance_exceeds"]} htr'
+                )
+                self.ctx.reached_conv = False
+                return False
+
         return True
 
     def return_results(self):
         """
         return the results of the calculations
         This should run through and produce output nodes even if everything failed,
         therefore it only uses results from context.
         """
-        if self.ctx.last_base_wc:
-            try:
-                last_calc_uuid = find_last_submitted_calcjob(self.ctx.last_base_wc)
-            except NotExistent:
-                last_calc_uuid = None
-        else:
-            last_calc_uuid = None
 
         try:  # if something failed, we still might be able to retrieve something
             last_calc_out = self.ctx.last_base_wc.outputs.output_parameters
             retrieved = self.ctx.last_base_wc.outputs.retrieved
             last_calc_out_dict = last_calc_out.get_dict()
         except (NotExistent, AttributeError):
             last_calc_out = None
@@ -791,34 +894,39 @@
         if self.ctx.last_nmmp_distance > 0.0:
             last_nmmp_distance = self.ctx.last_nmmp_distance
 
         outputnode_dict = {}
         outputnode_dict['workflow_name'] = self.__class__.__name__
         outputnode_dict['workflow_version'] = self._workflowversion
         outputnode_dict['material'] = self.ctx.formula
-        outputnode_dict['conv_mode'] = self.ctx.wf_dict.get('mode')
+        outputnode_dict['conv_mode'] = self.ctx.wf_dict['mode']
         outputnode_dict['loop_count'] = self.ctx.loop_count
         outputnode_dict['iterations_total'] = last_calc_out_dict.get('number_of_iterations_total', None)
         outputnode_dict['distance_charge'] = self.ctx.last_charge_density
         outputnode_dict['distance_charge_all'] = self.ctx.distance
         outputnode_dict['total_energy'] = last_calc_out_dict.get('energy_hartree', None)
         outputnode_dict['total_energy_all'] = self.ctx.total_energy
         outputnode_dict['force_diff_last'] = self.ctx.forcediff
         outputnode_dict['force_largest'] = last_calc_out_dict.get('force_largest', None)
         outputnode_dict['distance_charge_units'] = 'me/bohr^3'
         outputnode_dict['total_energy_units'] = 'Htr'
         outputnode_dict['nmmp_distance'] = last_nmmp_distance
         outputnode_dict['nmmp_distance_all'] = self.ctx.nmmp_distance
-        outputnode_dict['last_calc_uuid'] = last_calc_uuid
         outputnode_dict['total_wall_time'] = self.ctx.total_wall_time
         outputnode_dict['total_wall_time_units'] = 's'
         outputnode_dict['info'] = self.ctx.info
         outputnode_dict['warnings'] = self.ctx.warnings
         outputnode_dict['errors'] = self.ctx.errors
 
+        if self.ctx.x_torques:
+            outputnode_dict['last_x_torques'] = self.ctx.x_torques[-1]
+            outputnode_dict['last_y_torques'] = self.ctx.y_torques[-1]
+            outputnode_dict['alphas'] = self.ctx.alpha_angles
+            outputnode_dict['betas'] = self.ctx.beta_angles
+
         num_iterations = last_calc_out_dict.get('number_of_iterations_total', None)
         if self.ctx.successful and self.ctx.reached_conv:
             if len(self.ctx.total_energy) <= 1:  # then len(self.ctx.all_forces) <= 1 too
                 self.report('STATUS: Done, the convergence criteria are reached.\n'
                             'INFO: The charge density of the FLEUR calculation '
                             f'converged after {self.ctx.loop_count} FLEUR runs, {num_iterations} '
                             f'iterations and {self.ctx.total_wall_time} sec '
@@ -854,34 +962,35 @@
                             'INFO: The total energy difference of the last two iterations '
                             f'is {self.ctx.energydiff} Htr and largest force difference is'
                             f'{self.ctx.forcediff} Htr/bohr\n')
         else:  # Termination ok, but not converged yet...
             if self.ctx.abort:  # some error occurred, do not use the output.
                 self.report('STATUS/ERROR: I abort, see logs and errors/warning/hints in output_scf_wc_para')
 
+        if self.ctx.torquediff is None:
+            self.ctx.torquediff = 9999
+        self.report(f'Torque diff {self.ctx.torquediff}')
+        outputnode_t = Dict(dict=outputnode_dict)
         if self.ctx.last_nmmp_distance > 0.0:
             self.report(f'INFO: The LDA+U density matrix is converged to {self.ctx.last_nmmp_distance} change '
                         'of all matrix elements')
 
-        outputnode_t = Dict(dict=outputnode_dict)
+        outputnode_t = Dict(outputnode_dict)
         # this is unsafe so far, because last_calc_out could not exist...
         if last_calc_out:
             outdict = create_scf_result_node(outpara=outputnode_t,
                                              last_calc_out=last_calc_out,
                                              last_calc_retrieved=retrieved)
         else:
             outdict = create_scf_result_node(outpara=outputnode_t)
 
         # Now it always returns changed fleurinp that was actually used in the calculation
         if self.ctx.fleurinp is not None:
             outdict['fleurinp'] = self.ctx.fleurinp
 
-        if last_calc_out:
-            outdict['last_fleur_calc_output'] = last_calc_out
-
         if self.ctx.last_base_wc:
             self.out_many(self.exposed_outputs(self.ctx.last_base_wc, FleurBaseWorkChain, namespace='last_calc'))
 
         #outdict['output_scf_wc_para'] = outputnode
         for link_name, node in outdict.items():
             self.out(link_name, node)
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/ssdisp.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/ssdisp.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,41 +10,42 @@
 ###############################################################################
 """
     In this module you find the workflow 'FleurSSDispWorkChain' for the calculation of
     spin spiral dispersion using scalar-relatevistic Hamiltonian.
 """
 
 import copy
+from typing import Type
 
-#from six.moves import map
 from lxml import etree
 from ase.dft.kpoints import monkhorst_pack
 
 from aiida.engine import WorkChain, ToContext, if_
 from aiida.engine import calcfunction as cf
 from aiida.orm import Code, load_node
 from aiida.orm import RemoteData, Dict, KpointsData
 from aiida.common import AttributeDict
 from aiida.common.exceptions import NotExistent
 
+from masci_tools.util.constants import HTR_TO_EV
+
 from aiida_fleur.tools.common_fleur_wf import test_and_get_codenode
 from aiida_fleur.tools.common_fleur_wf import get_inputs_fleur
 from aiida_fleur.workflows.scf import FleurScfWorkChain
-from aiida_fleur.data.fleurinpmodifier import FleurinpModifier
+from aiida_fleur.data.fleurinpmodifier import FleurinpModifier, inpxml_changes
 from aiida_fleur.workflows.base_fleur import FleurBaseWorkChain
-from aiida_fleur.common.constants import HTR_TO_EV
 from aiida_fleur.data.fleurinp import FleurinpData, get_fleurinp_from_remote_data
 
 
 class FleurSSDispWorkChain(WorkChain):
     """
     This workflow calculates spin spiral dispersion of a structure.
     """
 
-    _workflowversion = '0.2.1'
+    _workflowversion = '0.3.0'
 
     _default_options = {
         'resources': {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1
         },
         'max_wallclock_seconds': 2 * 60 * 60,
@@ -89,15 +90,15 @@
                      if_(cls.scf_needed)(
                          cls.converge_scf,
                          cls.force_after_scf,
                      ).else_(
                          cls.force_wo_scf,
                      ), cls.get_results, cls.return_results)
 
-        spec.output('out', valid_type=Dict)
+        spec.output('output_ssdisp_wc_para', valid_type=Dict)
 
         # exit codes
         spec.exit_code(230, 'ERROR_INVALID_INPUT_PARAM', message='Invalid workchain parameters.')
         spec.exit_code(231, 'ERROR_INVALID_INPUT_CONFIG', message='Invalid input configuration.')
         spec.exit_code(233,
                        'ERROR_INVALID_CODE_PROVIDED',
                        message='Invalid code node specified, check inpgen and fleur code nodes.')
@@ -158,15 +159,15 @@
             options[key] = options.get(key, val)
         self.ctx.options = options
 
         # Check if user gave valid fleur executable
         inputs = self.inputs
         if 'fleur' in inputs:
             try:
-                test_and_get_codenode(inputs.fleur, 'fleur.fleur', use_exceptions=True)
+                test_and_get_codenode(inputs.fleur, 'fleur.fleur')
             except ValueError:
                 error = 'The code you provided for FLEUR does not use the plugin fleur.fleur'
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
         # Check if user gave an input setup making any sense
         if 'scf' in inputs:
@@ -211,49 +212,38 @@
                                           ' density for Spin Spiral Dispersion')
 
         if 'wf_parameters' not in input_scf:
             scf_wf_dict = {}
         else:
             scf_wf_dict = input_scf.wf_parameters.get_dict()
 
-        if 'inpxml_changes' not in scf_wf_dict:
-            scf_wf_dict['inpxml_changes'] = []
-        # set up q vector for the reference calculation
-        string_ref_qss = ' '.join(map(str, self.ctx.wf_dict['ref_qss']))
-        if [x for x in self.ctx.wf_dict['ref_qss'] if x != 0]:
-            changes_dict = {'qss': string_ref_qss, 'l_noco': True, 'ctail': False, 'l_ss': True}
-        else:
-            changes_dict = {'qss': ' 0.0 0.0 0.0 ', 'l_noco': False, 'ctail': True, 'l_ss': False}
+        with inpxml_changes(scf_wf_dict) as fm:
 
-        scf_wf_dict['inpxml_changes'].append(('set_inpchanges', {'change_dict': changes_dict}))
+            if [x for x in self.ctx.wf_dict['ref_qss'] if x != 0]:
+                fm.set_inpchanges({'qss': self.ctx.wf_dict['ref_qss'], 'l_noco': True, 'ctail': False, 'l_ss': True})
+            else:
+                fm.set_inpchanges({'qss': ' 0.0 0.0 0.0 ', 'l_noco': False, 'ctail': True, 'l_ss': False})
 
-        # change beta parameter
-        for key, val in self.ctx.wf_dict.get('beta').items():
-            scf_wf_dict['inpxml_changes'].append(('set_atomgroup_label', {
-                'attributedict': {
-                    'nocoParams': {
-                        'beta': val
-                    }
-                },
-                'atom_label': key
-            }))
+            # change beta parameter
+            for key, val in self.ctx.wf_dict['beta'].items():
+                fm.set_atomgroup_label(key, {'nocoParams': {'beta': val}})
 
-        input_scf.wf_parameters = Dict(dict=scf_wf_dict)
+        input_scf.wf_parameters = Dict(scf_wf_dict)
 
         if 'structure' in input_scf:  # add info about spin spiral propagation
             if 'calc_parameters' in input_scf:
                 calc_parameters = input_scf.calc_parameters.get_dict()
             else:
                 calc_parameters = {}
             calc_parameters['qss'] = {
                 'x': self.ctx.wf_dict['prop_dir'][0],
                 'y': self.ctx.wf_dict['prop_dir'][1],
                 'z': self.ctx.wf_dict['prop_dir'][2]
             }
-            input_scf.calc_parameters = Dict(dict=calc_parameters)
+            input_scf.calc_parameters = Dict(calc_parameters)
 
         return input_scf
 
     def change_fleurinp(self):
         """
         This routine sets somethings in the fleurinp file before running a fleur
         calculation.
@@ -270,78 +260,53 @@
         else:
             if 'fleurinp' in self.inputs:  # use the given fleurinp
                 fleurin = self.inputs.fleurinp
             else:  # or generate a new one from inp.xml located in the remote folder
                 fleurin = get_fleurinp_from_remote_data(self.inputs.remote)
 
         # copy inpchanges from wf parameters
-        fchanges = self.ctx.wf_dict.get('inpxml_changes', [])
-        # create forceTheorem tags
-        fchanges.append(('set_complex_tag', {
-            'tag_name': 'spinSpiralDispersion',
-            'create': True,
-            'changes': {
-                'q': self.ctx.wf_dict['q_vectors']
-            }
-        }))
-
-        changes_dict = {'itmax': 1, 'l_noco': True, 'ctail': False, 'l_ss': True}
-        fchanges.append(('set_inpchanges', {'change_dict': changes_dict}))
-
-        if self.ctx.wf_dict['kmesh_force_theorem'] is not None:
-            kmesh = KpointsData()
-            kmesh.set_kpoints(monkhorst_pack(self.ctx.wf_dict['kmesh_force_theorem']))
-            kmesh.store()
-            fchanges.append(('set_kpointsdata', {
-                'kpointsdata_uuid': kmesh.uuid,
-                'switch': True,
-                'kpoint_type': 'mesh'
-            }))
-
-        # change beta parameter
-        for label, beta in self.ctx.wf_dict['beta'].items():
-            fchanges.append(('set_atomgroup_label', {
-                'attributedict': {
-                    'nocoParams': {
-                        'beta': beta
-                    }
-                },
-                'atom_label': label
-            }))
-
-        if fchanges:  # change inp.xml file
-            fleurmode = FleurinpModifier(fleurin)
-            try:
-                fleurmode.add_task_list(fchanges)
-            except (ValueError, TypeError) as exc:
-                error = ('ERROR: Changing the inp.xml file failed. Tried to apply inpxml_changes'
-                         f', which failed with {exc}. I abort, good luck next time!')
-                self.control_end_wc(error)
-                return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
+        with inpxml_changes(self.ctx.wf_dict) as fm:
+            fm.set_complex_tag('spinSpiralDispersion', {'q': self.ctx.wf_dict['q_vectors']}, create=True)
+            fm.set_inpchanges({'itmax': 1, 'l_noco': True, 'ctail': False, 'l_ss': True})
+
+            if self.ctx.wf_dict['kmesh_force_theorem'] is not None:
+                kmesh = KpointsData()
+                kmesh.set_kpoints(monkhorst_pack(self.ctx.wf_dict['kmesh_force_theorem']))
+                kmesh.store()
+                fm.set_kpointsdata(kmesh.uuis, switch=True, kpoint_type='mesh')
+
+            # change beta parameter
+            for label, beta in self.ctx.wf_dict['beta'].items():
+                fm.set_atomgroup_label(label, {'nocoParams': {'beta': beta}})
 
-            # validate?
-            try:
-                fleurmode.show(display=False, validate=True)
-            except etree.DocumentInvalid:
-                error = ('ERROR: input, user wanted inp.xml changes did not validate')
-                self.report(error)
-                return self.exit_codes.ERROR_INVALID_INPUT_FILE
-            except ValueError as exc:
-                error = ('ERROR: input, user wanted inp.xml changes could not be applied.'
-                         f'The following error was raised {exc}')
-                self.control_end_wc(error)
-                return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
+        fleurmode = FleurinpModifier(fleurin)
+        try:
+            fleurmode.add_task_list(self.ctx.wf_dict['inpxml_changes'])
+        except (ValueError, TypeError) as exc:
+            error = ('ERROR: Changing the inp.xml file failed. Tried to apply inpxml_changes'
+                     f', which failed with {exc}. I abort, good luck next time!')
+            self.control_end_wc(error)
+            return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
 
-            # apply
-            out = fleurmode.freeze()
-            self.ctx.fleurinp = out
-        else:  # otherwise do not change the inp.xml
-            self.ctx.fleurinp = fleurin
+        # validate?
+        try:
+            fleurmode.show(display=False, validate=True)
+        except etree.DocumentInvalid:
+            error = ('ERROR: input, user wanted inp.xml changes did not validate')
+            self.report(error)
+            return self.exit_codes.ERROR_INVALID_INPUT_FILE
+        except (ValueError, TypeError) as exc:
+            error = ('ERROR: input, user wanted inp.xml changes could not be applied.'
+                     f'The following error was raised {exc}')
+            self.control_end_wc(error)
+            return self.exit_codes.ERROR_CHANGING_FLEURINPUT_FAILED
 
-        return
+        # apply
+        out = fleurmode.freeze()
+        self.ctx.fleurinp = out
 
     def force_after_scf(self):
         '''
         This routine uses the force theorem to calculate energies dispersion of
         spin spirals. The force theorem calculations implemented into the FLEUR
         code. Hence a single iteration FLEUR input file having <forceTheorem> tag
         has to be created and submitted.
@@ -495,15 +460,15 @@
             'energy_units': 'eV',
             'info': self.ctx.info,
             'warnings': self.ctx.warnings,
             'errors': self.ctx.errors
         }
 
         out = save_output_node(Dict(dict=out))
-        self.out('out', out)
+        self.out('output_ssdisp_wc_para', out)
 
     def control_end_wc(self, errormsg):
         """
         Controlled way to shutdown the workchain. It will initialize the output nodes
         The shutdown of the workchain will has to be done afterwards
         """
         self.report(errormsg)  # because return_results still fails sometimes
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/ssdisp_conv.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/ssdisp_conv.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,25 @@
 
 from aiida.engine import WorkChain
 from aiida.engine import calcfunction as cf
 from aiida.orm import Dict
 from aiida.common import AttributeDict
 
 from aiida_fleur.workflows.scf import FleurScfWorkChain
+from aiida_fleur.data.fleurinpmodifier import inpxml_changes
+
+from masci_tools.util.constants import HTR_TO_EV
 
 
 class FleurSSDispConvWorkChain(WorkChain):
     """
         This workflow calculates the Spin Spiral Dispersion of a structure.
     """
 
-    _workflowversion = '0.2.1'
+    _workflowversion = '0.3.0'
 
     _default_wf_para = {
         'beta': {
             'all': 1.57079
         },
         'q_vectors': {
             'label': [0.0, 0.0, 0.0],
@@ -45,15 +48,15 @@
     def define(cls, spec):
         super().define(spec)
         spec.expose_inputs(FleurScfWorkChain, namespace='scf')
         spec.input('wf_parameters', valid_type=Dict, required=False)
 
         spec.outline(cls.start, cls.converge_scf, cls.get_results, cls.return_results)
 
-        spec.output('out', valid_type=Dict)
+        spec.output('output_ssdisp_conv_wc_para', valid_type=Dict)
 
         # exit codes
         spec.exit_code(230, 'ERROR_INVALID_INPUT_PARAM', message='Invalid workchain parameters.')
         spec.exit_code(340,
                        'ERROR_ALL_QVECTORS_FAILED',
                        message='Convergence SSDisp calculation failed for all q-vectors.')
         spec.exit_code(341,
@@ -89,81 +92,60 @@
             return self.exit_codes.ERROR_INVALID_INPUT_PARAM
 
         # extend wf parameters given by user using defaults
         for key, val in wf_default.items():
             wf_dict[key] = wf_dict.get(key, val)
         self.ctx.wf_dict = wf_dict
 
-    def converge_scf(self):
-        """
-        Converge charge density with or without SOC.
-        Depending on a branch of Spiral calculation, submit a single Fleur calculation to obtain
-        a reference for further force theorem calculations or
-        submit a set of Fleur calculations to converge charge density for all given SQAs.
-        """
-        inputs = {}
-        for key, q_vector in self.ctx.wf_dict['q_vectors'].items():
-            inputs[key] = self.get_inputs_scf()
-            if self.ctx.wf_dict['suppress_symmetries']:
-                inputs[key].calc_parameters['qss'] = {'x': 1.221, 'y': 0.522, 'z': -0.5251}
-                changes_dict = {'qss': ' '.join(map(str, q_vector))}
-                wf_para = inputs[key].wf_parameters.get_dict()
-                wf_para['inpxml_changes'].append(('set_inpchanges', {'change_dict': changes_dict}))
-                inputs[key].wf_parameters = Dict(dict=wf_para)
-            else:
-                inputs[key].calc_parameters['qss'] = {'x': q_vector[0], 'y': q_vector[1], 'z': q_vector[2]}
-            inputs[key].calc_parameters = Dict(dict=inputs[key]['calc_parameters'])
-            res = self.submit(FleurScfWorkChain, **inputs[key])
-            res.label = key
-            self.to_context(**{key: res})
-
-    def get_inputs_scf(self):
+    def get_inputs_scf(self, qss):
         """
         Initialize inputs for scf workflow:
         wf_param, options, calculation parameters, codes, structure
         """
         input_scf = AttributeDict(self.exposed_inputs(FleurScfWorkChain, namespace='scf'))
 
-        if 'wf_parameters' not in input_scf:
-            scf_wf_dict = {}
-        else:
-            scf_wf_dict = input_scf.wf_parameters.get_dict()
-
-        if 'inpxml_changes' not in scf_wf_dict:
-            scf_wf_dict['inpxml_changes'] = []
-
-        # change beta parameter
-        for key, val in self.ctx.wf_dict.get('beta').items():
-            scf_wf_dict['inpxml_changes'].append(('set_atomgroup_label', {
-                'attributedict': {
-                    'nocoParams': {
-                        'beta': val
-                    }
-                },
-                'atom_label': key
-            }))
-
-        input_scf.wf_parameters = Dict(dict=scf_wf_dict)
+        with inpxml_changes(input_scf) as fm:
+            for key, val in self.ctx.wf_dict['beta'].items():
+                fm.set_atomgroup_label(key, {'nocoParams': {'beta': val}})
+            if self.ctx.wf_dict['suppress_symmetries']:
+                fm.set_inpchanges({'qss': qss})
 
         if 'calc_parameters' in input_scf:
             calc_parameters = input_scf.calc_parameters.get_dict()
         else:
             calc_parameters = {}
-        input_scf.calc_parameters = calc_parameters
+        if self.ctx.wf_dict['suppress_symmetries']:
+            calc_parameters['qss'] = {'x': 1.221, 'y': 0.522, 'z': -0.5251}
+        else:
+            calc_parameters['qss'] = {'x': qss[0], 'y': qss[1], 'z': qss[2]}
+        input_scf.calc_parameters = Dict(calc_parameters)
 
         return input_scf
 
+    def converge_scf(self):
+        """
+        Converge charge density with or without SOC.
+        Depending on a branch of Spiral calculation, submit a single Fleur calculation to obtain
+        a reference for further force theorem calculations or
+        submit a set of Fleur calculations to converge charge density for all given SQAs.
+        """
+        inputs = {}
+        for key, q_vector in self.ctx.wf_dict['q_vectors'].items():
+            inputs[key] = self.get_inputs_scf(q_vector)
+            res = self.submit(FleurScfWorkChain, **inputs[key])
+            res.label = key
+            self.to_context(**{key: res})
+
     def get_results(self):
         """
         Retrieve results of converge calculations
         """
         t_energydict = {}
         original_t_energydict = {}
         outnodedict = {}
-        htr_to_eV = 27.21138602
 
         for label in self.ctx.wf_dict['q_vectors'].keys():
             calc = self.ctx[label]
 
             if not calc.is_finished_ok:
                 message = f'One SCF workflow was not successful: {label}'
                 self.ctx.warnings.append(message)
@@ -181,15 +163,15 @@
             t_e = outpara.get('total_energy', 'failed')
             if not isinstance(t_e, float):
                 message = f'Did not manage to extract float total energy from one SCF workflow: {label}'
                 self.ctx.warnings.append(message)
                 continue
             e_u = outpara.get('total_energy_units', 'Htr')
             if e_u in ['Htr', 'htr']:
-                t_e = t_e * htr_to_eV
+                t_e = t_e * HTR_TO_EV
             t_energydict[label] = t_e
 
         if t_energydict:
             # Find a minimal value of Spiral and count it as 0
             minenergy = min(t_energydict.values())
 
             for key, energy in t_energydict.items():
@@ -222,19 +204,19 @@
             'info': self.ctx.info,
             'warnings': self.ctx.warnings,
             'errors': self.ctx.errors
         }
 
         # create link to workchain node
         out = save_output_node(Dict(dict=out))
-        self.out('out', out)
+        self.out('output_ssdisp_conv_wc_para', out)
 
         if not self.ctx.energydict:
             return self.exit_codes.ERROR_ALL_QVECTORS_FAILED
-        elif failed_labels:
+        if failed_labels:
             return self.exit_codes.ERROR_SOME_QVECTORS_FAILED
 
     def control_end_wc(self, errormsg):
         """
         Controlled way to shutdown the workchain. will initialize the output nodes
         The shutdown of the workchain will has to be done afterwards
         """
```

### Comparing `aiida-fleur-1.3.1/aiida_fleur/workflows/strain.py` & `aiida-fleur-2.0.0/aiida_fleur/workflows/strain.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from aiida.engine import calcfunction as cf
 
 from aiida_fleur.tools.StructureData_util import rescale, rescale_nowf, is_structure
 from aiida_fleur.workflows.scf import FleurScfWorkChain
 from aiida_fleur.tools.common_fleur_wf import test_and_get_codenode
 from aiida_fleur.tools.common_fleur_wf_util import check_eos_energies
 
+from masci_tools.util.constants import HTR_TO_EV
+
 # pylint: disable=invalid-name
 FleurInpData = DataFactory('fleur.fleurinp')
 # pylint: enable=invalid-name
 
 
 class FleurStrainWorkChain(WorkChain):
     """
@@ -147,23 +149,23 @@
             options[key] = options.get(key, val)
         self.ctx.options = options
 
         # Check if user gave valid inpgen and fleur executables
         inputs = self.inputs
         if 'inpgen' in inputs:
             try:
-                test_and_get_codenode(inputs.inpgen, 'fleur.inpgen', use_exceptions=True)
+                test_and_get_codenode(inputs.inpgen, 'fleur.inpgen')
             except ValueError:
                 error = ('The code you provided for inpgen of FLEUR does not use the plugin fleur.inpgen')
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
         if 'fleur' in inputs:
             try:
-                test_and_get_codenode(inputs.fleur, 'fleur.fleur', use_exceptions=True)
+                test_and_get_codenode(inputs.fleur, 'fleur.fleur')
             except ValueError:
                 error = ('The code you provided for FLEUR does not use the plugin fleur.fleur')
                 self.control_end_wc(error)
                 return self.exit_codes.ERROR_INVALID_CODE_PROVIDED
 
     def structures(self):
         """
@@ -225,17 +227,17 @@
         except AttributeError:
             calc_para = {}
         inputs['calc_parameters'] = calc_para
 
         inputs['inpgen'] = self.inputs.inpgen
         inputs['fleur'] = self.inputs.fleur
 
-        inputs['options'] = Dict(dict=inputs['options'])
-        inputs['wf_parameters'] = Dict(dict=inputs['wf_parameters'])
-        inputs['calc_parameters'] = Dict(dict=inputs['calc_parameters'])
+        inputs['options'] = Dict(inputs['options'])
+        inputs['wf_parameters'] = Dict(inputs['wf_parameters'])
+        inputs['calc_parameters'] = Dict(inputs['calc_parameters'])
 
         return inputs
 
     def return_results(self):
         """
         Return the results of the calculations  (scf workchains) and do a
         polynomial fit
@@ -243,15 +245,14 @@
         distancelist = []
         t_energylist = []
         t_energylist_peratom = []
         bandgaplist = []
         calc_uuids = []
         vol_peratom_success = []
         natoms = len(self.inputs.structure.sites)
-        htr_to_ev = 27.21138602
 
         for label in self.ctx.labels:
             calc = self.ctx[label]
 
             if not calc.is_finished_ok:
                 message = f'One SCF workflow was not successful: {label}'
                 self.ctx.warnings.append(message)
@@ -267,22 +268,22 @@
                 continue
 
             outpara = calc.outputs.output_scf_wc_para.get_dict()
 
             t_e = outpara.get('total_energy', float('nan'))
             e_u = outpara.get('total_energy_units', 'eV')
             if e_u in ('Htr', 'htr'):
-                t_e = t_e * htr_to_ev
+                t_e = t_e * HTR_TO_EV
             dis = outpara.get('distance_charge', float('nan'))
             dis_u = outpara.get('distance_charge_units')
             t_energylist.append(t_e)
             t_energylist_peratom.append(t_e / natoms)
             vol_peratom_success.append(self.ctx.volume_peratom[label])
             distancelist.append(dis)
-            calc_uuid = outpara.get('last_calc_uuid')
+            calc_uuid = calc.outputs.last_calc.remote_folder.creator.uuid
             calc_uuids.append(calc_uuid)
             bandgaplist.append(load_node(calc_uuid).res.bandgap)
 
         en_array = np.array(t_energylist_peratom)
         vol_array = np.array(vol_peratom_success)
         eg_array = np.array(bandgaplist)
         vol_unitcell_array = vol_array * natoms
@@ -346,15 +347,15 @@
 
         if self.ctx.successful:
             self.report('Done, Strain calculation complete')
         else:
             self.report('Done, but something went wrong.... Probably some individual calculation failed or'
                         ' a scf-cycle did not reach the desired distance.')
 
-        outputnode_t = Dict(dict=outputnode_dict)
+        outputnode_t = Dict(outputnode_dict)
         outdict = create_strain_result_node(outpara=outputnode_t)
 
         # create link to work-chain node
         for link_name, node in outdict.items():
             self.out(link_name, node)
 
     def control_end_wc(self, errormsg):
```

### Comparing `aiida-fleur-1.3.1/docs/Makefile` & `aiida-fleur-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/README.rst` & `aiida-fleur-2.0.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/rtd_settings.py` & `aiida-fleur-2.0.0/docs/rtd_settings.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/conf.py` & `aiida-fleur-2.0.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
               'sphinx.ext.intersphinx',
               'sphinx.ext.viewcode',
               'sphinx_click.ext']
 
 todo_include_todos = True
 
 intersphinx_mapping = {
-    'aiida': ('https://aiida-core.readthedocs.io/en/latest/', None),
+    'aiida': ('https://aiida-core.readthedocs.io/en/v1.6.8/', None),
     'masci-tools': ('https://masci-tools.readthedocs.io/en/latest/', None),
     'ase': ('https://wiki.fysik.dtu.dk/ase/', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'python': ('https://docs.python.org/3', None),
     'lxml': ('https://lxml.de/apidoc/',None),
     'h5py': ('https://docs.h5py.org/en/latest/', None)
 }
@@ -304,16 +304,19 @@
 else:
     # Back-end settings for readthedocs online documentation.
     from aiida.manage import configuration
     configuration.IN_RT_DOC_MODE = True
     configuration.BACKEND = 'django'
     configuration.AIIDADB_PROFILE = 'default'
     #Perform reentry scan
-    from reentry import manager
-    manager.scan()
+    try:
+        from reentry import manager
+        manager.scan()
+    except ImportError:
+        pass
 
 
 '''
 def run_apidoc(_):
     """Runs sphinx-apidoc when building the documentation.
 
     Needs to be done in conf.py in order to include the APIdoc in the
```

### Comparing `aiida-fleur-1.3.1/docs/source/devel_guide/dg_index.rst` & `aiida-fleur-2.0.0/docs/source/devel_guide/dg_index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,17 @@
 #. Outsource methods to test for calculation failure, that you have only one routine in all workchains, that one can improve
 
 
 Entrypoints
 +++++++++++
 
 In order to make AiiDA aware of any classes (plugins) like (calculations, parsers, data, workchains, workflows, commandline)
-the python entrypoint system is used. Therefore, you have to register any  of the above classes as an entrypoint in the 'setup.json' file.
+the python entrypoint system is used. Therefore, you have to register any  of the above classes as an entrypoint in the 'pyproject.toml' file.
+
+.. TODO: Rewrite for pyproject.toml syntax
 
 Example::
 
     "entry_points" : {
         "aiida.calculations" : [
             "fleur.fleur = aiida_fleur.calculation.fleur:FleurCalculation",
             "fleur.inpgen = aiida_fleur.calculation.fleurinputgen:FleurinputgenCalculation"
```

### Comparing `aiida-fleur-1.3.1/docs/source/images/AiiDA_transparent_logo.png` & `aiida-fleur-2.0.0/docs/source/images/AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/Bands_colored.png` & `aiida-fleur-2.0.0/docs/source/images/Bands_colored.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/Lattice_constant.png` & `aiida-fleur-2.0.0/docs/source/images/Lattice_constant.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/Logo-JLVMD.png` & `aiida-fleur-2.0.0/docs/source/images/Logo-JLVMD.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/MAX-orizz.png` & `aiida-fleur-2.0.0/docs/source/images/MAX-orizz.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/Workchain_charts_corehole_wc.png` & `aiida-fleur-2.0.0/docs/source/images/Workchain_charts_corehole_wc.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/Workchain_charts_dos_wc.png` & `aiida-fleur-2.0.0/docs/source/images/Workchain_charts_dos_wc.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/Workchain_charts_eos_wc.png` & `aiida-fleur-2.0.0/docs/source/images/Workchain_charts_eos_wc.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/Workchain_charts_initial_state.png` & `aiida-fleur-2.0.0/docs/source/images/Workchain_charts_initial_state.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/Workchain_charts_relaxation.png` & `aiida-fleur-2.0.0/docs/source/images/Workchain_charts_relaxation.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/Workchain_charts_scf_wc.png` & `aiida-fleur-2.0.0/docs/source/images/Workchain_charts_scf_wc.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/aiida_work2_ed.png` & `aiida-fleur-2.0.0/docs/source/images/aiida_work2_ed.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/all_logos.odg` & `aiida-fleur-2.0.0/docs/source/images/all_logos.odg`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/all_logos.png` & `aiida-fleur-2.0.0/docs/source/images/all_logos.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/all_rmts_oqmd.png` & `aiida-fleur-2.0.0/docs/source/images/all_rmts_oqmd.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/b_AiiDA_transparent_logo.png` & `aiida-fleur-2.0.0/docs/source/images/b_AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/band_d_like.png` & `aiida-fleur-2.0.0/docs/source/images/band_d_like.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/band_f_like.png` & `aiida-fleur-2.0.0/docs/source/images/band_f_like.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/band_p_like.png` & `aiida-fleur-2.0.0/docs/source/images/band_p_like.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/band_s_like.png` & `aiida-fleur-2.0.0/docs/source/images/band_s_like.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/bandstructure.png` & `aiida-fleur-2.0.0/docs/source/images/bandstructure.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/convergence_all_MP_metals.png` & `aiida-fleur-2.0.0/docs/source/images/convergence_all_MP_metals.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/convergence_all_MP_metals1.png` & `aiida-fleur-2.0.0/docs/source/images/convergence_all_MP_metals1.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/corehole_si_30528.pdf` & `aiida-fleur-2.0.0/docs/source/images/corehole_si_30528.pdf`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/dos_76867.pdf` & `aiida-fleur-2.0.0/docs/source/images/dos_76867.pdf`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/dos_plot.png` & `aiida-fleur-2.0.0/docs/source/images/dos_plot.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/eos_49670.pdf` & `aiida-fleur-2.0.0/docs/source/images/eos_49670.pdf`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/eos_wc_outputnode.py` & `aiida-fleur-2.0.0/docs/source/images/eos_wc_outputnode.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/fleur.png` & `aiida-fleur-2.0.0/docs/source/images/fleur.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/plot_fleur_capabilities.png` & `aiida-fleur-2.0.0/docs/source/images/plot_fleur_capabilities.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/plot_fleur_eos_mn.png` & `aiida-fleur-2.0.0/docs/source/images/plot_fleur_eos_mn.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/plot_fleur_eos_sn.png` & `aiida-fleur-2.0.0/docs/source/images/plot_fleur_eos_sn.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/plot_fleur_scf1.png` & `aiida-fleur-2.0.0/docs/source/images/plot_fleur_scf1.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/plot_fleur_scf2.png` & `aiida-fleur-2.0.0/docs/source/images/plot_fleur_scf2.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/plot_fleur_scf_m1.png` & `aiida-fleur-2.0.0/docs/source/images/plot_fleur_scf_m1.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/plot_fleur_scf_m2.png` & `aiida-fleur-2.0.0/docs/source/images/plot_fleur_scf_m2.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/images/scf_50816.pdf` & `aiida-fleur-2.0.0/docs/source/images/scf_50816.pdf`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/index.rst` & `aiida-fleur-2.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/module_guide/code.rst` & `aiida-fleur-2.0.0/docs/source/module_guide/code.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/module_guide/tools.rst` & `aiida-fleur-2.0.0/docs/source/module_guide/tools.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/nitpick-exceptions` & `aiida-fleur-2.0.0/docs/source/nitpick-exceptions`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
 py:class aiida.engine.processes.workchains.workchain.WorkChainSpec
 py:class aiida.manage.manager.Manager
 py:class aiida.orm.nodes.node.WarnWhenNotEntered
 py:class aiida.orm.utils.links.LinkQuadruple
 py:class aiida.tools.importexport.dbexport.ExportReport
 py:class aiida.tools.importexport.dbexport.ArchiveData
 py:class aiida.tools.groups.paths.WalkNodeResult
+py:class orm.Dict
 
 py:class Backend
 py:class BackendEntity
 py:class BackendNode
 py:class AuthInfo
 py:class CalcJob
 py:class CalcJobNode
@@ -201,14 +202,15 @@
 py:class JobInfo
 py:class JobState
 py:class Node
 py:class Parser
 py:class PersistenceError
 py:class Process
 py:class ProcessBuilder
+py:class ProcessBuilderNamespace
 py:class ProcessNode
 py:class ProcessSpec
 py:class Port
 py:class PortNamespace
 py:class Repository
 py:class Runner
 py:class Transport
```

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/calculations/fleurcode_plugin.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/calculations/fleurcode_plugin.rst`

 * *Files 20% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The table below shows all possible inputs for the FleurCalculation:
 
 +------------------+--------------+--------------------------------------+----------+
 | name             | type         | description                          | required |
 +==================+==============+======================================+==========+
 | code             | Code         | Fleur code                           | yes      |
 +------------------+--------------+--------------------------------------+----------+
-| fleurinpdata     | FleurinpData | Object representing inp.xml          | no       |
+| fleurinp         | FleurinpData | Object representing inp.xml          | no       |
 +------------------+--------------+--------------------------------------+----------+
 | parent_folder    | RemoteData   | Remote folder of another calculation | no       |
 +------------------+--------------+--------------------------------------+----------+
 | settings         | Dict         | special settings                     | no       |
 +------------------+--------------+--------------------------------------+----------+
 | metadata.options | Dict         | computational resources              | yes      |
 +------------------+--------------+--------------------------------------+----------+
@@ -157,24 +157,60 @@
 | 314       | Problem with cdn is suspected                                |
 +-----------+--------------------------------------------------------------+
 | 315       | Invalid Elements found in the LDA+U density matrix.          |
 +-----------+--------------------------------------------------------------+
 | 316       | Calculation failed due to time limits.                       |
 +-----------+--------------------------------------------------------------+
 
+.. _fleur_parallelization:
+
+Parallelization options
+''''''''''''''''''''''''
+
+For parallel FLEUR calculations the input under ``metadata.options`` can be used.
+In higher level workchains this input might be present as a plain ``options`` input,
+but it is completely equivalent to the ``metadata.options`` input.
+
+.. code-block:: python
+
+    inputs.metadata.options = {
+      'resources': {
+        'num_machines': 2, #Number of computing nodes
+        'num_mpiprocs_per_machine': 4, #Number of MPI processes per node
+        'num_cpus_per_mpiproc': 12, #Number of OMP threads per MPI process
+      },
+      'withmpi': True, #This flag makes sure that the process is submitted using MPI
+      'max_wallclock_seconds': 3600, #Maximum wallclock time in seconds
+    }
+
+This will result in setting the following slurm Parallelization variables in the submit script.
+
+.. code-block:: bash
+
+  #SBATCH --nodes=1
+  #SBATCH --ntasks-per-node=6
+  #SBATCH --cpus-per-task=8
+  #SBATCH --time=01:00:00
+  #... Further configuration options unrelated to parallelization...
+
+  'srun' '/path/to/fleur/' '<further FLEUR cmdline flags, e.g. -last_extra>'
+
+Note, that the ``srun`` command is computer specific and is configured in ``verdi computer setup``
+with the ``Mpirun command`` option.
+
 .. _Fleur_settings:
 
 Additional advanced features
 ''''''''''''''''''''''''''''
 
 .. _documentation: www.flapw.de
 
 In general see the FLEUR `documentation`_.
 
-While the input link with name **fleurinpdata** is used for the content of the
+While the input link with name **fleurinp** is used for the content of the
 inp.xml, additional parameters for changing the plugin behavior, can be specified in the
 **settings** input, also of type :py:class:`~aiida.orm.Dict`.
 
 Below we summarise some of the options that you can specify, and their effect.
 In each case, after having defined the content of ``settings_dict``, you can use
 it as input of a calculation ``calc`` by doing::
```

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/calculations/images/fleur_calc.png` & `aiida-fleur-2.0.0/docs/source/user_guide/calculations/images/fleur_calc.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/calculations/images/fleurinpgen_calc.png` & `aiida-fleur-2.0.0/docs/source/user_guide/calculations/images/fleurinpgen_calc.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/calculations/inpgen_plugin.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/calculations/inpgen_plugin.rst`

 * *Files 1% similar despite different names*

```diff
@@ -109,24 +109,24 @@
 '''''''
 The table below shows all the output nodes generated by
 :py:class:`~aiida_fleur.calculation.fleurinputgen.FleurinputgenCalculation`:
 
 +------------------+---------------+-------------------------------+
 | name             | type          | comment                       |
 +==================+===============+===============================+
-| fleurinpData     | FleurinpData  | represents `inp.xml`          |
+| fleurinp         | FleurinpData  | represents `inp.xml`          |
 +------------------+---------------+-------------------------------+
 | remote_folder    | FolderData    | represents calculation folder |
 +------------------+---------------+-------------------------------+
 | retrieved        | FolderData    | represents retrieved folder   |
 +------------------+---------------+-------------------------------+
 
 All output nodes can be accessed via ``calculation.outputs``.
 
-* **fleurinpData**: :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` -
+* **fleurinp**: :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` -
   Data structure which represents the inp.xml file and provides useful methods.
   For more information see :ref:`fleurinp_data`
 * **remote_folder**: :py:class:`~aiida.orm.RemoteData` -
   RemoteData which represents the calculation folder on the remote machine.
 * **retrieved**: :py:class:`~aiida.orm.FolderData` -
   FolderData which represents the retrieved folder on the remote machine.
```

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/calculations/output_node_example.py` & `aiida-fleur-2.0.0/docs/source/user_guide/calculations/output_node_example.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/calculations/parameter_example.py` & `aiida-fleur-2.0.0/docs/source/user_guide/calculations/parameter_example.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/cmd/cmd_index.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/cmd/cmd_index.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/data/fleur_data_plugins.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/data/fleur_data_plugins.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/data/fleurinp_data.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/data/fleurinp_data.rst`

 * *Files 0% similar despite different names*

```diff
@@ -161,8 +161,8 @@
                                               },
                                           'create': True
                                          })]
 
   # in this example the atomgroup, to which the atom with label '222' belongs,
   # will be modified
   fm = FleurinpModifier(SomeFleurinp)
-  fm.set_atomgroup_label(attributedict={'force': {'relaxXYZ': 'FFF'}, atom_label='                 222')
+  fm.set_atomgroup_label({'force': {'relaxXYZ': 'FFF'}, atom_label='                 222')
```

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/data/fleurinp_modifier.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/data/fleurinp_modifier.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .. _fleurinp_mod:
 
 FleurinpModifier
 ================
 
+.. contents::
+
 Description
 -----------
 The :py:class:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier` class has
 to be used if you want to change anything in a stored
 :py:class:`~aiida_fleur.data.fleurinp.FleurinpData`.
 It will store and validate all the changes you wish to do and produce a new
 :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` node
@@ -35,15 +37,15 @@
 After that, a user should register
 certain modifications which will be cached and can be previewed. They will be applied on
 a new :py:class:`~aiida_fleur.data.fleurinp.FleurinpData`
 object when the freeze method is executed. A code example:
 
 .. code-block:: python
 
-  from aiida_fleur.data.fleurinpmodifier import  FleurinpModifier
+  from aiida_fleur.data.fleurinpmodifier import FleurinpModifier
 
   F = FleurinpData(files=['inp.xml'])
   fm = FleurinpModifier(F)                                # Initialise FleurinpModifier class
   fm.set_inpchanges({'dos' : True, 'Kmax': 3.9 })         # Add changes
   fm.show()                                               # Preview
   new_fleurinpdata = fm.freeze()                          # Apply
 
@@ -160,22 +162,22 @@
     * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.replace_tag()` is now a higher-level function. The old function requiring an xpath is now called :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.xml_replace_tag()`
     * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.delete_tag()` is now a higher-level function. The old function requiring an xpath is now called :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.xml_delete_tag()`
     * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.delete_att()` is now a higher-level function. The old function requiring an xpath is now called :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.xml_delete_att()`
       an xml element in the xml tree.
     * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.add_num_to_att()` was renamed to :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.add_number_to_attrib()` or :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.add_number_to_first_attrib()`. However, these are also higher-level functions now longer requiring a concrete xpath
     * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.set_atomgr_att()` and :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.set_atomgr_att_label()` were renamed to :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.set_atomgroup()` and :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.set_atomgroup_label()`. These functions now also take the changes in the form ``attributedict={'nocoParams':{'beta': val}}`` instead of ``attributedict={'nocoParams':[('beta': val)]}``
 
-.. warning:: Passing XML Elements to modification functions
+.. .. warning:: Passing XML Elements to modification functions
 
-    Some of the low-level implementations of the XML modification functions accept explicit XML elements as arguments for replacing/inserting. However, these can only be used within limits in the :py:class:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier` at the moment. The reason for this is that there is currently no support for serializing these objects for the input of the Aiida calcfunction. The following functions are affected by this:
+..     Some of the low-level implementations of the XML modification functions accept explicit XML elements as arguments for replacing/inserting. However, these can only be used within limits in the :py:class:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier` at the moment. The reason for this is that there is currently no support for serializing these objects for the input of the Aiida calcfunction. The following functions are affected by this:
 
-    * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.xml_replace_tag()` (Only usable with show and validate)
-    * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.replace_tag()` (Only usable with show and validate)
-    * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.xml_create_tag()` (Can only be used with string names of tags)
-    * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.create_tag()`  (Can only be used with string names of tags)
+..     * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.xml_replace_tag()` (Only usable with show and validate)
+..     * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.replace_tag()` (Only usable with show and validate)
+..     * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.xml_create_tag()` (Can only be used with string names of tags)
+..     * :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.create_tag()`  (Can only be used with string names of tags)
 
 Modifying the density matrix for LDA+U calculations
 ---------------------------------------------------
 
 The above mentioned :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.set_nmmpmat()` takes a special
 role in the modification registration methods, as the modifications are not done on the ``inp.xml`` file but the
 density matrix file ``n_mmp_mat`` used by Fleur for LDA+U calculations. The resulting density matrix file is stored
@@ -184,15 +186,15 @@
 density matrix if a calculation is started from this :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` instance.
 
 The code example below shows how to use this method to add a LDA+U procedure to an atom species and provide
 an initial guess for the density matrix.
 
 .. code-block:: python
 
-  from aiida_fleur.data.fleurinpmodifier import  FleurinpModifier
+  from aiida_fleur.data.fleurinpmodifier import FleurinpModifier
 
   F = FleurinpData(files=['inp.xml'])
   fm = FleurinpModifier(F)                                             # Initialise FleurinpModifier class
   fm.set_species('Nd-1', {'ldaU':                                      # Add LDA+U procedure
                          {'l': 3, 'U': 6.76, 'J': 0.76, 'l_amf': 'F'}}) 
   fm.set_nmmpmat('Nd-1', orbital=3, spin=1, occStates=[1,1,1,1,0,0,0]) # Initialize n_mmp_mat file with the states
                                                                        # m = -3 to m = 0 occupied for spin up
@@ -204,14 +206,82 @@
     LDA+U procedure. They are read in the same order as they appear in the ``inp.xml``. For this reason the ``n_mmp_mat``
     file can become invalid if one adds/removes a LDA+U procedure to the ``inp.xml`` after the ``n_mmp_mat`` file was 
     initialized. To circumvent these problems always remove any existing ``n_mmp_mat`` file from the 
     :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` instance, before adding/removing or modifying the LDA+U configuration.
     Furthermore the :py:func:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier.set_nmmpmat()` should always be called 
     after any modifications to the LDA+U configuration.
     
+Usage in Workflows
+-------------------
+
+The :py:class:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier` class can be used nicely to explicitly
+modify the :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` instances in scripts. However, when a ``inp.xml``
+file should be modified during the run of a aiida-fleur workflow this class cannot be used directly.
+Each workflow specifies a ``wf_parameters`` dictionary input (potentially more in sub workflows), which contains
+a ``inpxml_changes`` entry. This entry can be used to modify the used inputs inside the workchain at points
+defined by the workflow itself. The syntax for the ``inpxml_changes`` entry is as follows:
+
+Explicit definition
+___________________
+
+.. code-block:: python
+
+  wf_parameters = {
+    'inpxml_changes': [
+      ('set_inpchanges', {'changes': {'dos': True}}),
+      ('set_species', {'species_name': 'Fe-1', {'changes': {'electronConfig': {'flipspins': True}}}})
+    ]
+  }
+
+is equivalent to
+
+.. code-block:: python
+
+  from aiida_fleur.data.fleurinpmodifier import FleurinpModifier
+
+  F = FleurinpData(files=['inp.xml'])
+  fm = FleurinpModifier(F)
+  fm.set_inpchanges({'dos': True})
+  fm.set_species('Fe-1', {'electronConfig': {'flipspins': True}})
+
+Using :py:func:`~aiida_fleur.data.fleurinpmodifier.inpxml_changes()`
+____________________________________________________________________
+
+As can be seen from the above example, the syntax for the ``inpxml_changes`` entry is quite verbose,
+especially if compared with the more compact formulation using the :py:class:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier`
+directly.
+For this reason a helper function :py:func:`~aiida_fleur.data.fleurinpmodifier.inpxml_changes()` is implemented
+to construct the ``inpxml_changes`` entry with the exact same syntax as the :py:class:`~aiida_fleur.data.fleurinpmodifier.FleurinpModifier`
+
+It is used as a contextmanager, which behaves exactly like the Modifier inside it's with block and
+enters a ``inpxml_changes`` entry into the dictionary passed to this function after the with block
+is terminated.
+
+.. code-block:: python
+
+  from aiida_fleur.data.fleurinpmodifier import inpxml_changes
+
+  parameters = {}
+  with inpxml_changes(parameters) as fm:
+    fm.set_inpchanges({'dos': True})
+    fm.set_species('Fe-1', {'electronConfig': {'flipspins': True}})
+  
+  print(parameters)
+
+.. code-block:: python
+
+  from aiida_fleur.data.fleurinpmodifier import inpxml_changes
+  from aiida import plugins
+
+  FleurBandDOS = plugins.WorkflowFactory('fleur.banddos')
+  inputs = FleurBandDOS.get_builder()
+
+  with inpxml_changes(inputs) as fm:
+    fm.set_inpchanges({'dos': True})
+    fm.set_species('Fe-1', {'electronConfig': {'flipspins': True}})
 
 .. Node graphs
 .. -----------
 
 .. 1. After any modification was applied to fleurinpData the following nodes will be found in the
       database to keep the Provenance
```

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/data/images/fleurinpdata.png` & `aiida-fleur-2.0.0/docs/source/user_guide/data/images/fleurinpdata.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/data/images/fleurinpmodifier.png` & `aiida-fleur-2.0.0/docs/source/user_guide/data/images/fleurinpmodifier.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/data/images/registration_methods.png` & `aiida-fleur-2.0.0/docs/source/user_guide/data/images/registration_methods.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/data/parameter_example.py` & `aiida-fleur-2.0.0/docs/source/user_guide/data/parameter_example.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/getting_started/getting_started.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/getting_started/getting_started.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/hints/exit_codes.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/hints/exit_codes.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/hints/hints_faq.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/hints/hints_faq.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/tools/tools_index.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/tools/tools_index.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/tutorials/tutorials.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/tutorials/tutorials.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/base_relax_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/base_relax_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/base_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/base_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/cfcoeff_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/cfcoeff_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/banddos_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/banddos_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/cfcoeff_parameters.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/cfcoeff_parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/corehole_parameters.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/corehole_parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/corehole_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/corehole_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/corehole_wc_outputnode.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/corehole_wc_outputnode.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/create_magnetic_parameters.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/create_magnetic_parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/create_magnetic_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/create_magnetic_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/dmi_parameters.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/dmi_parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/dmi_wc_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/dmi_wc_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/initial_cls_parameters.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/initial_cls_parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/initial_cls_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/initial_cls_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/initial_cls_wc_outputnode.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/initial_cls_wc_outputnode.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/mae_conv_wc_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/mae_conv_wc_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/mae_parameters.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/mae_parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/mae_wc_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/mae_wc_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/orbcontrol_parameters.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/orbcontrol_parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/orbcontrol_wc_outputnode.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/orbcontrol_wc_outputnode.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/relax_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/relax_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/scf_parameters.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/scf_parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/scf_wc_outputnode.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/scf_wc_outputnode.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     ],
     'distance_charge_units': 'me/bohr^3',
     'errors': [],
     'force_diff_last': 'can not be determined',
     'force_largest': 0.0,
     'info': [],
     'iterations_total': 23,
-    'last_calc_uuid': 'b20b5b94-5d80-41a8-82bf-b4d8eee9bddc',
     'loop_count': 1,
     'material': 'FePt2',
     'total_energy': -38166.176928494,
     'total_energy_all': [
         -38166.542950054,
         -38166.345602746,
         ...
```

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/scf_wc_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/scf_wc_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/ssdisp_conv_wc_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/ssdisp_conv_wc_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/ssdisp_parameters.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/ssdisp_parameters.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/ssdisp_wc_submission.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/ssdisp_wc_submission.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/code/tutorial_submit_eos.py` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/code/tutorial_submit_eos.py`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/corehole_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/corehole_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/create_magnetic_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/create_magnetic_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/dmi_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/dmi_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/dos_band_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/dos_band_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/eos_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/eos_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/base_restart_scheme.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/base_restart_scheme.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/create_magnetic_AFM_bcc110.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/create_magnetic_AFM_bcc110.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/create_magnetic_AFM_fcc110.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/create_magnetic_AFM_fcc110.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/create_magnetic_scheme.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/create_magnetic_scheme.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/dmi.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/dmi.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/mae_conv.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/mae_conv.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/mae_energies.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/mae_energies.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/mae_force.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/mae_force.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/plot_fleur_orbcontrol.pdf` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/plot_fleur_orbcontrol.pdf`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/ssdisp_conv.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/ssdisp_conv.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/ssdisp_energies.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/ssdisp_energies.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/ssdisp_force.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/ssdisp_force.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/images/workchains2.png` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/images/workchains2.png`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/initial_cls_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/initial_cls_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/mae_conv_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/mae_conv_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/mae_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/mae_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/orbcontrol_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/orbcontrol_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/relax_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/relax_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/scf_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/scf_wc.rst`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 
       Only one of ``density_converged``, ``energy_converged`` or ``force_converged``
       is used by the workchain that corresponds to the **'mode'**. The other two are ignored.
       Exception: force mode uses both ``density_converged`` and ``force_converged`` because FLEUR
       code always converges density before forces.
 
   * ``options``: :py:class:`~aiida.orm.Dict` - AiiDA options (computational resources).
+    Also see :ref:`fleur_parallelization` section.
     Example:
 
     .. code-block:: python
 
          'resources': {"num_machines": 1, "num_mpiprocs_per_machine": 1},
          'max_wallclock_seconds': 6*60*60,
          'queue_name': '',
@@ -110,33 +111,33 @@
          'environment_variables': {}
 
 Returns nodes
 ^^^^^^^^^^^^^
 
 The table below shows all the possible output nodes of the SCF workchain.
 
-+-------------------------+------------------------------------------------------+------------------------------------------------------+
-| name                    | type                                                 | comment                                              |
-+=========================+======================================================+======================================================+
-| output_scf_wc_para      | :py:class:`~aiida.orm.Dict`                          | results of the workchain                             |
-+-------------------------+------------------------------------------------------+------------------------------------------------------+
-| fleurinp                | :py:class:`~aiida_fleur.data.fleurinp.FleurinpData`  | FleurinpData that was used (after all modifications) |
-+-------------------------+------------------------------------------------------+------------------------------------------------------+
-| last_fleur_calc_output  | :py:class:`~aiida.orm.Dict`                          | Link to last FleurCalculation output dict            |
-+-------------------------+------------------------------------------------------+------------------------------------------------------+
++--------------------+-----------------------------------------------------+--------------------------------------------------------------------------+
+| name               | type                                                | comment                                                                  |
++====================+=====================================================+==========================================================================+
+| output_scf_wc_para | :py:class:`~aiida.orm.Dict`                         | results of the workchain                                                 |
++--------------------+-----------------------------------------------------+--------------------------------------------------------------------------+
+| fleurinp           | :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` | FleurinpData that was used (after all modifications)                     |
++--------------------+-----------------------------------------------------+--------------------------------------------------------------------------+
+| last_calc          | Namespace                                           | Link to all output nodes (out dict, retrieved) of last Fleur calculation |
++--------------------+-----------------------------------------------------+--------------------------------------------------------------------------+
 
 More details:
 
   * ``fleurinp``: :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` - A
     :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` that was
     actually used for last :py:class:`~aiida_fleur.workflows.scf.FleurScfWorkChain`.
     It usually differs from the input :py:class:`~aiida_fleur.data.fleurinp.FleurinpData`
     because there are some hard-coded modifications in the SCF workchain.
-  * ``last_fleur_calc_output``: :py:class:`~aiida.orm.Dict` - A link to the output node
-    of the last Fleur calculation.
+  * ``last_calc``: namespace - A link to the output nodes
+    of the last Fleur calculation. This includes the retrieved files, remote folder and output dictionary
   * ``output_scf_wc_para``: :py:class:`~aiida.orm.Dict` -  Main results of the workchain. Contains
     errors, warnings, convergence history and other information. An example:
 
     .. literalinclude:: code/scf_wc_outputnode.py
 
 .. _scf_wc_layout:
 
@@ -162,15 +163,15 @@
 3. **structure** + **inpgen** + *calc_parameters*:
 
       inpgen code and optional *calc_parameters* will be used to generate a
       new :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` using a given **structure**.
       Generated :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` will
       be used as an input for the first FLEUR calculation.
 
-3. **structure** + **inpgen** + *calc_parameters* + **remote_data** (FLEUR):
+4. **structure** + **inpgen** + *calc_parameters* + **remote_data** (FLEUR):
 
       inpgen code and optional *calc_parameters* will be used to generate a
       new :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` using a given **structure**.
       Generated :py:class:`~aiida_fleur.data.fleurinp.FleurinpData` will
       be used as an input for the first FLEUR calculation. Initial charge density will be taken from given
       **remote_data** (FLEUR). **Note**: make sure that **remote_data** (FLEUR) corresponds to the same structure.
```

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/ssdisp_conv_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/ssdisp_conv_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/ssdisp_wc.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/ssdisp_wc.rst`

 * *Files identical despite different names*

### Comparing `aiida-fleur-1.3.1/docs/source/user_guide/workflows/wc_index.rst` & `aiida-fleur-2.0.0/docs/source/user_guide/workflows/wc_index.rst`

 * *Files identical despite different names*

