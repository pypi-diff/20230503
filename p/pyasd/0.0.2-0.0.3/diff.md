# Comparing `tmp/pyasd-0.0.2.tar.gz` & `tmp/pyasd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyasd-0.0.2.tar", last modified: Sun Jan  8 09:05:55 2023, max compression
+gzip compressed data, was "pyasd-0.0.3.tar", last modified: Wed May  3 05:05:39 2023, max compression
```

## Comparing `pyasd-0.0.2.tar` & `pyasd-0.0.3.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.871641 pyasd-0.0.2/
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1468 2023-01-05 06:57:53.000000 pyasd-0.0.2/LICENSE
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      488 2023-01-06 02:20:47.000000 pyasd-0.0.2/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-01-08 09:05:55.871641 pyasd-0.0.2/PKG-INFO
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1395 2023-01-05 06:45:32.000000 pyasd-0.0.2/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.803640 pyasd-0.0.2/asd/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      311 2023-01-08 09:05:55.000000 pyasd-0.0.2/asd/__init__.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.823640 pyasd-0.0.2/asd/core/
--rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2022-11-19 16:04:48.000000 pyasd-0.0.2/asd/core/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      537 2022-11-19 16:04:48.000000 pyasd-0.0.2/asd/core/constants.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      902 2022-11-19 16:04:48.000000 pyasd-0.0.2/asd/core/dipolar_interactions.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    14898 2022-12-26 07:20:12.000000 pyasd-0.0.2/asd/core/geometry.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34800 2022-12-24 03:07:21.000000 pyasd-0.0.2/asd/core/gneb.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28542 2023-01-04 12:57:14.000000 pyasd-0.0.2/asd/core/hamiltonian.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13407 2023-01-05 02:10:30.000000 pyasd-0.0.2/asd/core/llg_advanced.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    33813 2023-01-05 02:40:39.000000 pyasd-0.0.2/asd/core/llg_simple.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6377 2022-12-22 03:51:11.000000 pyasd-0.0.2/asd/core/log_general.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    35175 2022-12-22 03:52:06.000000 pyasd-0.0.2/asd/core/monte_carlo.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7330 2022-12-11 15:48:49.000000 pyasd-0.0.2/asd/core/random_vectors.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28367 2022-12-24 03:07:21.000000 pyasd-0.0.2/asd/core/shell_exchange.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    20183 2023-01-05 11:19:02.000000 pyasd-0.0.2/asd/core/spin_configurations.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13692 2022-11-29 08:08:25.000000 pyasd-0.0.2/asd/core/spin_correlations.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4455 2022-11-29 08:07:49.000000 pyasd-0.0.2/asd/core/topological_charge.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.827640 pyasd-0.0.2/asd/data_base/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.2/asd/data_base/exchange_for_Cr2I3X3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.2/asd/data_base/exchange_for_CrI3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.2/asd/data_base/exchange_for_CrMnI6_U2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.2/asd/data_base/exchange_for_CrMnI6_U4.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.2/asd/data_base/exchange_for_CrMnI6_rect.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.2/asd/data_base/exchange_for_Gd2C.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.2/asd/data_base/exchange_for_MnI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.2/asd/data_base/exchange_for_NiI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.2/asd/data_base/exchange_for_RuCl3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.2/asd/data_base/exchange_for_VOI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.2/asd/data_base/exchange_for_kagome.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.2/asd/data_base/exchange_for_skx.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.827640 pyasd-0.0.2/asd/mpi/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2556 2022-11-26 03:52:08.000000 pyasd-0.0.2/asd/mpi/mpi_tools.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.835641 pyasd-0.0.2/asd/utility/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12245 2022-11-03 09:03:40.000000 pyasd-0.0.2/asd/utility/Swq.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2022-11-03 09:03:40.000000 pyasd-0.0.2/asd/utility/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8824 2022-12-06 13:36:56.000000 pyasd-0.0.2/asd/utility/analyze_Spirit_results.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9225 2022-12-06 08:59:01.000000 pyasd-0.0.2/asd/utility/asd_arguments.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    55462 2022-11-03 09:03:40.000000 pyasd-0.0.2/asd/utility/auxiliary_colormaps.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     2158 2022-11-30 01:10:21.000000 pyasd-0.0.2/asd/utility/curve_fit.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5328 2022-12-02 03:50:43.000000 pyasd-0.0.2/asd/utility/four_state_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1873 2023-01-06 01:15:40.000000 pyasd-0.0.2/asd/utility/head_figlet.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6697 2022-12-10 09:03:53.000000 pyasd-0.0.2/asd/utility/mag_thermal.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     7594 2022-12-11 03:29:55.000000 pyasd-0.0.2/asd/utility/ovf_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7753 2022-12-24 03:07:21.000000 pyasd-0.0.2/asd/utility/plot_tools_3d.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13388 2022-11-28 08:41:51.000000 pyasd-0.0.2/asd/utility/post_llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5437 2022-12-10 09:05:12.000000 pyasd-0.0.2/asd/utility/post_mc.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    19392 2022-12-22 03:50:20.000000 pyasd-0.0.2/asd/utility/spin_visualize_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2442 2022-11-03 09:03:40.000000 pyasd-0.0.2/asd/utility/spirit_tool.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.835641 pyasd-0.0.2/examples/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-01-05 02:04:28.000000 pyasd-0.0.2/examples/README
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.835641 pyasd-0.0.2/examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.2/examples/example1/.coverage
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.2/examples/example1/single_spin_LLG.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.835641 pyasd-0.0.2/examples/example2/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      267 2023-01-05 02:44:29.000000 pyasd-0.0.2/examples/example2/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.2/examples/example2/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.835641 pyasd-0.0.2/examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      267 2022-10-28 16:09:17.000000 pyasd-0.0.2/examples/example3/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.2/examples/example3/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.835641 pyasd-0.0.2/examples/example4/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.2/examples/example4/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.2/examples/example4/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.795640 pyasd-0.0.2/misc/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.839640 pyasd-0.0.2/misc/archives/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.2/misc/archives/ovf-0.4.3.tar.gz
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.2/misc/archives/pyfiglet-0.7.tar.gz
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.847641 pyasd-0.0.2/pyasd.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-01-08 09:05:55.000000 pyasd-0.0.2/pyasd.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     4680 2023-01-08 09:05:55.000000 pyasd-0.0.2/pyasd.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-01-08 09:05:55.000000 pyasd-0.0.2/pyasd.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       43 2023-01-08 09:05:55.000000 pyasd-0.0.2/pyasd.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1083 2023-01-08 09:05:55.000000 pyasd-0.0.2/pyasd.egg-info/top_level.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-01-08 09:05:55.871641 pyasd-0.0.2/setup.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3339 2023-01-08 09:05:44.000000 pyasd-0.0.2/setup.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.799640 pyasd-0.0.2/tests_basic/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.847641 pyasd-0.0.2/tests_basic/B_eff/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.2/tests_basic/B_eff/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.2/tests_basic/B_eff/test_B_eff.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.847641 pyasd-0.0.2/tests_basic/OVF/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       64 2022-11-28 06:51:17.000000 pyasd-0.0.2/tests_basic/OVF/README
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3532 2022-11-28 04:33:12.000000 pyasd-0.0.2/tests_basic/OVF/pyasd_ovf_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2777 2022-12-11 02:09:06.000000 pyasd-0.0.2/tests_basic/OVF/test_ovf.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.851641 pyasd-0.0.2/tests_basic/mag_confs/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.851641 pyasd-0.0.2/tests_basic/mag_confs/Potts/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.2/tests_basic/mag_confs/Potts/Potts_test.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.851641 pyasd-0.0.2/tests_basic/mag_confs/domain_walls/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/domain_walls/dw_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/interpolate_images.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.851641 pyasd-0.0.2/tests_basic/mag_confs/meron/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/meron/bimeron.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/meron/meron.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.855641 pyasd-0.0.2/tests_basic/mag_confs/misc/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/misc/interpolate_images.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/misc/mpi_topo.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1067 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/misc/regular_order_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/misc/struct_factor.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      768 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/misc/test_pbc_shell.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.859641 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/Skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/a2sk.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/firework.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/mpi_firework.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/skyrmionium.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.859641 pyasd-0.0.2/tests_basic/mag_confs/spirals/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.2/tests_basic/mag_confs/spirals/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/spirals/spiral_test.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/mag_confs/test_regular_orders_honeycomb.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.859641 pyasd-0.0.2/tests_basic/mpi/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.2/tests_basic/mpi/test_group_rank.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.803640 pyasd-0.0.2/tests_basic/total_energy/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.799640 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.863641 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.863641 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5193 2022-11-28 03:36:50.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.863641 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.867641 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/simple/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.867641 pyasd-0.0.2/tests_basic/total_energy/chiral_confs/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.2/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.867641 pyasd-0.0.2/tests_basic/total_energy/large_test/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.2/tests_basic/total_energy/large_test/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/large_test/large_cell.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.867641 pyasd-0.0.2/tests_basic/total_energy/large_test/test_loop_methods/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.867641 pyasd-0.0.2/tests_basic/total_energy/local_energy/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/local_energy/CrMnI6_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/local_energy/test_local_en.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-01-08 09:05:55.871641 pyasd-0.0.2/tests_basic/total_energy/regular_orders/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7050 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1851 2023-01-05 07:16:05.000000 pyasd-0.0.2/tests_basic/total_energy/regular_orders/llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.2/tests_basic/total_energy/regular_orders/phase_diagram_tri.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1468 2023-01-05 06:57:53.000000 pyasd-0.0.3/LICENSE
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      488 2023-01-06 02:20:47.000000 pyasd-0.0.3/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-03 05:05:39.187106 pyasd-0.0.3/PKG-INFO
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1350 2023-05-03 04:42:39.000000 pyasd-0.0.3/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.139106 pyasd-0.0.3/asd/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      311 2023-05-03 05:05:38.000000 pyasd-0.0.3/asd/__init__.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.147106 pyasd-0.0.3/asd/core/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      537 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/constants.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      902 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/dipolar_interactions.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    14970 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/geometry.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34800 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/gneb.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28461 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/hamiltonian.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13407 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/llg_advanced.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34609 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/llg_simple.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6394 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/log_general.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    35175 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/monte_carlo.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7330 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/random_vectors.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28028 2023-05-01 09:54:36.000000 pyasd-0.0.3/asd/core/shell_exchange.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    20217 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/spin_configurations.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13692 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/spin_correlations.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4455 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/topological_charge.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.155106 pyasd-0.0.3/asd/data_base/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.3/asd/data_base/exchange_for_Cr2I3X3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.3/asd/data_base/exchange_for_CrI3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_U2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_U4.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_rect.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.3/asd/data_base/exchange_for_Gd2C.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.3/asd/data_base/exchange_for_MnI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.3/asd/data_base/exchange_for_NiI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.3/asd/data_base/exchange_for_RuCl3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.3/asd/data_base/exchange_for_VOI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.3/asd/data_base/exchange_for_kagome.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.3/asd/data_base/exchange_for_skx.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.155106 pyasd-0.0.3/asd/mpi/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2556 2022-11-26 03:52:08.000000 pyasd-0.0.3/asd/mpi/mpi_tools.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.163106 pyasd-0.0.3/asd/utility/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12245 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/Swq.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8824 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/analyze_Spirit_results.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9225 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/asd_arguments.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    55462 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/auxiliary_colormaps.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     2143 2023-02-03 13:19:28.000000 pyasd-0.0.3/asd/utility/curve_fit.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5328 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/four_state_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1880 2023-04-17 02:00:31.000000 pyasd-0.0.3/asd/utility/head_figlet.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6688 2023-02-07 02:54:27.000000 pyasd-0.0.3/asd/utility/mag_thermal.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     7606 2023-02-08 03:42:14.000000 pyasd-0.0.3/asd/utility/ovf_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7753 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/plot_tools_3d.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13553 2023-05-01 09:39:25.000000 pyasd-0.0.3/asd/utility/post_llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5437 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/post_mc.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    19392 2023-04-07 12:17:17.000000 pyasd-0.0.3/asd/utility/spin_visualize_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2442 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/spirit_tool.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.163106 pyasd-0.0.3/examples/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-01-11 07:09:44.000000 pyasd-0.0.3/examples/README
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.167106 pyasd-0.0.3/examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.3/examples/example1/.coverage
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.3/examples/example1/single_spin_LLG.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.167106 pyasd-0.0.3/examples/example2/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-01-11 07:10:07.000000 pyasd-0.0.3/examples/example2/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.3/examples/example2/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.167106 pyasd-0.0.3/examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      385 2023-01-11 07:09:55.000000 pyasd-0.0.3/examples/example3/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.3/examples/example3/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.167106 pyasd-0.0.3/examples/example4/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.3/examples/example4/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.3/examples/example4/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.135106 pyasd-0.0.3/misc/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.171106 pyasd-0.0.3/misc/archives/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.3/misc/archives/ovf-0.4.3.tar.gz
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.3/misc/archives/pyfiglet-0.7.tar.gz
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/pyasd.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-03 05:05:38.000000 pyasd-0.0.3/pyasd.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     4686 2023-05-03 05:05:39.000000 pyasd-0.0.3/pyasd.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-05-03 05:05:38.000000 pyasd-0.0.3/pyasd.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       43 2023-05-03 05:05:38.000000 pyasd-0.0.3/pyasd.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1083 2023-05-03 05:05:38.000000 pyasd-0.0.3/pyasd.egg-info/top_level.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-05-03 05:05:39.187106 pyasd-0.0.3/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3339 2023-05-03 05:04:28.000000 pyasd-0.0.3/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.135106 pyasd-0.0.3/tests_basic/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/B_eff/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.3/tests_basic/B_eff/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.3/tests_basic/B_eff/test_B_eff.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/OVF/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       64 2023-02-08 03:42:29.000000 pyasd-0.0.3/tests_basic/OVF/README
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3532 2023-02-08 03:43:05.000000 pyasd-0.0.3/tests_basic/OVF/pyasd_ovf_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2777 2023-02-08 03:42:25.000000 pyasd-0.0.3/tests_basic/OVF/test_ovf.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/mag_confs/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/mag_confs/Potts/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.3/tests_basic/mag_confs/Potts/Potts_test.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/mag_confs/domain_walls/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/domain_walls/dw_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/interpolate_images.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/mag_confs/meron/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/meron/bimeron.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/meron/meron.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.179106 pyasd-0.0.3/tests_basic/mag_confs/misc/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/interpolate_images.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/mpi_topo.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1067 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/regular_order_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/struct_factor.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      768 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/test_pbc_shell.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.179106 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/Skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/a2sk.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/firework.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/mpi_firework.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/skyrmionium.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/mag_confs/spirals/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.3/tests_basic/mag_confs/spirals/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/spirals/spiral_test.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/test_regular_orders_honeycomb.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/mpi/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.3/tests_basic/mpi/test_group_rank.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.139106 pyasd-0.0.3/tests_basic/total_energy/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.139106 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5188 2023-05-01 09:01:00.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/chiral_confs/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.3/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/large_test/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.3/tests_basic/total_energy/large_test/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/large_test/large_cell.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/local_energy/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/local_energy/CrMnI6_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/local_energy/test_local_en.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/regular_orders/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7050 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1851 2023-01-05 07:16:05.000000 pyasd-0.0.3/tests_basic/total_energy/regular_orders/llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/regular_orders/phase_diagram_tri.py
```

### Comparing `pyasd-0.0.2/LICENSE` & `pyasd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/core/constants.py` & `pyasd-0.0.3/asd/core/constants.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/core/dipolar_interactions.py` & `pyasd-0.0.3/asd/core/dipolar_interactions.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/core/geometry.py` & `pyasd-0.0.3/asd/core/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     for ix,iy,iat in np.ndindex(nx,ny,nat):
         rvec[ix,iy,iat] = rvec_pbc[idx[ix,iy,iat],ix,iy,iat]
     dist = np.min(dist_pbc,axis=0)
     shell_idx=np.array(np.where(dist<=radius)).T
     return shell_idx,rvec
 
 
-def build_latt(lat_type,nx,ny,nz,latt_choice=2,return_neigh=True):
+def build_latt(lat_type,nx,ny,nz,latt_choice=2,return_neigh=True,latt_const=1):
     lat_type_list = ['chain','square','triangular','kagome','honeycomb','simple cubic']
     lat_type = lat_type.lower()
     if lat_type=='simple cubic':
         nat=1
         latt=np.eye(3)
         sites=np.zeros((1,1,1,3),float)+0.5
         neigh1_cell_idx = np.array([[1,0,0],[-1,0,0],[0,1,0],[0,-1,0],[0,0,1],[0,0,-1]])
@@ -250,19 +250,20 @@
         for iat in range(nat):
             sites_sc[...,iat,0] = sites[...,iat,0] + xx
             sites_sc[...,iat,1] = sites[...,iat,1] + yy
             sites_sc[...,iat,2] = sites[...,iat,2] + zz
 
     neigh_idx = [neigh1_idx, neigh2_idx, neigh3_idx]
     rotvecs = [rotvec_neigh1, rotvec_neigh2,rotvec_neigh3]
+    latt *= latt_const
     if return_neigh: return latt,sites_sc,neigh_idx,rotvecs
     else: return latt,sites_sc
 
 
-def rectangular_honeycomb_cell(nx,ny,nz,return_neigh=True):
+def rectangular_honeycomb_cell(nx,ny,nz,return_neigh=True,latt_const=1):
     lat_type='honeycomb'
     prim_latt,prim_sites = build_latt(lat_type,nx,ny,nz,return_neigh=False)
     nat=4
     latt=np.dot([[1,0],[1,2]],prim_latt)
     xx,yy=np.mgrid[0:nx,0:ny]
     sites=np.zeros((nx,ny,nat,2),float)
     sites_home = np.array([[1./4,1./3],[3./4,5./6],[3./4,1./6],[1./4,2./3]])
@@ -283,14 +284,15 @@
     neigh3_idx = np.array([[[0,-1,3],[ 1, 0,3],[-1, 0,3]],
                            [[0, 0,2],[ 1, 1,2],[-1, 1,2]],
                            [[0, 0,1],[-1,-1,1],[ 1,-1,1]],
                            [[0, 1,0],[-1, 0,0],[ 1,0,0]]])
 
     #check_neigh_idx(latt,sites_home,[neigh1_idx,neigh2_idx,neigh3_idx])
     neigh_idx = [neigh1_idx, neigh2_idx, neigh3_idx]
+    latt *= latt_const
     if return_neigh: return latt,sites,neigh_idx
     else: return latt,sites
 
 
 def show_neighbors(latt,sites_sc,neigh_idx):
     import matplotlib.pyplot as plt
     nx,ny,nat = sites_sc.shape[:3]
```

### Comparing `pyasd-0.0.2/asd/core/gneb.py` & `pyasd-0.0.3/asd/core/gneb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/core/hamiltonian.py` & `pyasd-0.0.3/asd/core/hamiltonian.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,29 +316,29 @@
         E_zeeman = -np.sum(np.dot(np.dot(sp_lat,self._Bfield),self._S_values.T))*self._g_factor*muB
         return E_zeeman
 
 
     def calc_isotropic_total_E(self,sp_lat,parallel=False):
         E_iso_shell = np.zeros(self._nshell_BL)
         for i,exch in enumerate(self._BL_exch): 
-            E_iso_shell[i] = exch.calc_shell_isotropic_exch_energy(sp_lat,self._boundary_condition,parallel)
+            E_iso_shell[i] = exch.shell_isotropic_exch_energy(sp_lat,self._boundary_condition,parallel)
         E_iso = np.sum(E_iso_shell)
         return E_iso
 
 
     def calc_total_E_general(self,sp_lat,interaction_resolved=False,shell_resolved=False):
         E_SIA = self.calc_self_exchange_energy(sp_lat)
         E_zeeman = self.calc_zeeman_energy(sp_lat)
         E_iso_shell    = np.zeros(self._nshell_BL)
         E_DMI_shell    = np.zeros(self._nshell_BL)
         E_Kitaev_shell = np.zeros(self._nshell_BL)
         E_bq_shell     = np.zeros(self._nshell_BQ)
 
-        for i,exch in enumerate(self._BL_exch): E_iso_shell[i], E_DMI_shell[i], E_Kitaev_shell[i] = exch.calc_shell_exch_energy(sp_lat,self._boundary_condition)
-        for i,exch in enumerate(self._BQ_exch): E_bq_shell[i] = exch.calc_shell_exch_energy(sp_lat,self._boundary_condition)
+        for i,exch in enumerate(self._BL_exch): E_iso_shell[i], E_DMI_shell[i], E_Kitaev_shell[i] = exch.shell_exch_energy(sp_lat,self._boundary_condition)
+        for i,exch in enumerate(self._BQ_exch): E_bq_shell[i] = exch.shell_exch_energy(sp_lat,self._boundary_condition)
 
         E_iso = np.sum(E_iso_shell)
         E_DMI = np.sum(E_DMI_shell)
         E_Kitaev = np.sum(E_Kitaev_shell)
         E_bq = np.sum(E_bq_shell)
 
         E_tot = E_zeeman + E_SIA + E_iso + E_DMI + E_Kitaev + E_bq
@@ -351,16 +351,16 @@
     def calc_total_E_from_sym_mat(self,sp_lat,interaction_resolved=False,shell_resolved=False):
         E_SIA = self.calc_self_exchange_energy(sp_lat)
         E_zeeman = self.calc_zeeman_energy(sp_lat)
         E_sym_shell = np.zeros(self._nshell_BL)
         E_DMI_shell = np.zeros(self._nshell_BL)
         E_bq_shell  = np.zeros(self._nshell_BQ)
 
-        for i,exch in enumerate(self._BL_exch): E_sym_shell[i],E_DMI_shell[i] = exch.calc_shell_exch_energy_from_sym_mat(sp_lat,self._boundary_condition)
-        for i,exch in enumerate(self._BQ_exch): E_bq_shell[i] = exch.calc_shell_exch_energy(sp_lat,self._boundary_condition)
+        for i,exch in enumerate(self._BL_exch): E_sym_shell[i],E_DMI_shell[i] = exch.shell_exch_energy_from_sym_mat(sp_lat,self._boundary_condition)
+        for i,exch in enumerate(self._BQ_exch): E_bq_shell[i] = exch.shell_exch_energy(sp_lat,self._boundary_condition)
 
         E_sym = np.sum(E_sym_shell)
         E_DMI = np.sum(E_DMI_shell)
         E_bq  = np.sum(E_bq_shell)
 
         E_tot = E_zeeman + E_SIA + E_sym + E_DMI + E_bq
         if interaction_resolved:
@@ -372,17 +372,17 @@
     def calc_total_E_from_Jmat(self,sp_lat,interaction_resolved=False,shell_resolved=False,use_new_method=False,parallel=False):
         E_SIA = self.calc_self_exchange_energy(sp_lat)
         E_zeeman = self.calc_zeeman_energy(sp_lat)
         E_bl_shell = np.zeros(self._nshell_BL)
         E_bq_shell = np.zeros(self._nshell_BQ)
 
         for i,exch in enumerate(self._BL_exch): 
-            if use_new_method: E_bl_shell[i] = exch.calc_shell_exch_energy_from_Jmat_new(sp_lat)
-            else: E_bl_shell[i] = exch.calc_shell_exch_energy_from_Jmat(sp_lat,self._boundary_condition,parallel)
-        for i,exch in enumerate(self._BQ_exch): E_bq_shell[i] = exch.calc_shell_exch_energy(sp_lat,self._boundary_condition,parallel)
+            if use_new_method: E_bl_shell[i] = exch.shell_exch_energy_from_Jmat_new(sp_lat)
+            else: E_bl_shell[i] = exch.shell_exch_energy_from_Jmat(sp_lat,self._boundary_condition,parallel)
+        for i,exch in enumerate(self._BQ_exch): E_bq_shell[i] = exch.shell_exch_energy(sp_lat,self._boundary_condition,parallel)
 
         E_bl = np.sum(E_bl_shell)
         E_bq = np.sum(E_bq_shell)
 
         E_tot = E_zeeman + E_SIA + E_bl + E_bq
         if interaction_resolved:
             if shell_resolved: return E_tot, E_Zeeman, E_SIA, E_bl_shell, E_bq_shell
@@ -401,23 +401,24 @@
             E_SIA = self.calc_self_exchange_energy(sp_lat)
             E_zeeman = self.calc_zeeman_energy(sp_lat)
             Etot = self.calc_isotropic_total_E(sp_lat,parallel=parallel)
             Etot+= E_SIA + E_zeeman
         else: 
             Etot = self.calc_total_E_general(sp_lat)
         if self._nshell_general>0:
-            for exch in self._general_exch: Etot += exch.calc_shell_exch_energy(sp_lat,self._boundary_condition,parallel=parallel)
+            for exch in self._general_exch: Etot += exch.shell_exch_energy(sp_lat,self._boundary_condition,parallel=parallel)
         if average_on_sites: Etot /= np.prod(sp_lat.shape[:-1])
         return Etot
 
 
     def verbose_reference_energy(self,sp_lat,file_handle=None,spin_coord=None):
         print ('\nEnergy for reference configurations (meV/site)\n',file=file_handle)
-        if self._exchange_in_matrix or self._from_sym_mat: tags = ['E_tot','E_zeeman','E_SIA','E_symmetric','E_DMI','E_bq']
-        else:               tags = ['E_tot','E_zeeman','E_SIA','E_heisenberg','E_DMI','E_Kitaev','E_bq']
+        tags = ['E_tot','E_zeeman','E_SIA']
+        if self._exchange_in_matrix or self._from_sym_mat: tags += ['E_symmetric','E_DMI','E_bq']
+        else:  tags += ['E_Heisenberg','E_DMI','E_Kitaev','E_bq']
         dirs = {0:'x',1:'y',2:'z'}
         en_ref = []
         shape=sp_lat.shape
         ndim = shape[-1]
         shape0 = np.array(shape)
         if 0 not in self._boundary_condition: shape0[:-2] = 1
         for i in range(ndim):
@@ -432,15 +433,16 @@
                 en = [Etot,E_zeeman,E_SIA,E_iso,0,0,0]
             elif self._exchange_in_matrix  or self._from_sym_mat:  
                 en = self.calc_total_E_from_sym_mat(uc_sp_lat,interaction_resolved=True)
             else: 
                 en = self.calc_total_E_general(uc_sp_lat,interaction_resolved=True)
             en_ref.append(en)
         en_ref = np.array(en_ref)/np.prod(uc_sp_lat.shape[:-1])
-        print (('{:15s}'+'{:>15s}'*4+'\n{}').format('configuration','FM along x', 'FM along y', 'FM along z','MAE','-'*75),file=file_handle)
+        head_tags = ['configuration','FM along x', 'FM along y', 'FM along z','MAE']
+        print (('{:15s}'+'{:>15s}'*4+'\n{}').format(*tuple(head_tags),'-'*75),file=file_handle)
         for i in np.arange(1,len(tags)):
             print (('{:15s}'+'{:15.8f}'*ndim).format(tags[i],*tuple(en_ref[:,i])),end=' ',file=file_handle)
             print ('{:15.8f}'.format(en_ref[-1,i]-np.min(en_ref[:-1,i])),file=file_handle)
         print ('{0}'.format('-'*75),file=file_handle)
         print (('{:15s}'+'{:15.8f}'*ndim).format(tags[0],*tuple(en_ref[:,0])),end=' ',file=file_handle)
         print ('{:15.8f}\n'.format(en_ref[-1,0]-np.min(en_ref[:-1,0])),file=file_handle)
         if file_handle is not None: file_handle.flush()
@@ -462,61 +464,61 @@
         return SIA_B_eff/(self._g_factor*self._S_values[iat]*muB)  # convert from meV to Tesla
 
 
     def calc_local_isotropic_B_eff(self,sp_lat,site_idx):
         shape = sp_lat.shape
         iat = site_idx[-1]
         B_eff = np.zeros(3)
-        for exch in self._BL_exch: B_eff += exch.calc_shell_isotropic_exch_field(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._BL_exch: B_eff += exch.shell_isotropic_exch_field(sp_lat,site_idx,self._boundary_condition)
         B_eff = B_eff/(self._g_factor*self._S_values[iat]*muB)  # convert from meV to Tesla
         return B_eff
 
 
     # local effective magnetic field is tne negative derivative of energy with respect to spin
     def calc_local_B_eff_general(self,sp_lat,site_idx):
         shape = sp_lat.shape
         iat = site_idx[-1]
         B_eff = np.zeros(3)
-        for exch in self._BL_exch: B_eff += exch.calc_shell_exch_field(sp_lat,site_idx,self._boundary_condition)
-        for exch in self._BQ_exch: B_eff += exch.calc_shell_exch_field(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._BL_exch: B_eff += exch.local_exch_field(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._BQ_exch: B_eff += exch.local_exch_field(sp_lat,site_idx,self._boundary_condition)
         B_eff = B_eff/(self._g_factor*self._S_values[iat]*muB)  # convert from meV to Tesla
         return B_eff
 
 
     # local effective magnetic field is tne negative derivative of energy with respect to spin
     def calc_local_B_eff_from_sym_mat(self,sp_lat,site_idx):
         shape = sp_lat.shape
         iat = site_idx[-1]
         B_eff = np.zeros(3)
-        for exch in self._BL_exch: B_eff += exch.calc_shell_exch_field_from_sym_mat(sp_lat,site_idx,self._boundary_condition)
-        for exch in self._BQ_exch: B_eff += exch.calc_shell_exch_field(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._BL_exch: B_eff += exch.local_exch_field_from_sym_mat(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._BQ_exch: B_eff += exch.local_exch_field(sp_lat,site_idx,self._boundary_condition)
         B_eff = B_eff/(self._g_factor*self._S_values[iat]*muB)  # convert from meV to Tesla
         return B_eff
 
 
     def calc_local_B_eff_from_Jmat(self,sp_lat,site_idx):
         shape = sp_lat.shape
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         B_eff = np.zeros(3)
-        for exch in self._BL_exch: B_eff += exch.calc_shell_exch_field_from_Jmat(sp_lat,site_idx,self._boundary_condition)
-        for exch in self._BQ_exch: B_eff += exch.calc_shell_exch_field(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._BL_exch: B_eff += exch.local_exch_field_from_Jmat(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._BQ_exch: B_eff += exch.local_exch_field(sp_lat,site_idx,self._boundary_condition)
         B_eff = B_eff/(self._g_factor*self._S_values[iat]*muB)  # convert from meV to Tesla
         return B_eff
 
 
     def calc_local_B_eff(self,sp_lat,site_idx):
         if self._exchange_in_matrix:    B_eff = self.calc_local_B_eff_from_Jmat(sp_lat,site_idx)
         elif self._from_sym_mat:        B_eff = self.calc_local_B_eff_from_sym_mat(sp_lat,site_idx)
         elif self._iso_only:            B_eff = self.calc_local_isotropic_B_eff(sp_lat,site_idx)
         else:                           B_eff = self.calc_local_B_eff_general(sp_lat,site_idx)
 
         if self._nshell_general:
             iat = site_idx[-1]
-            for exch in self._general_exch: B_eff_general = exch.calc_shell_exch_field(sp_lat,site_idx)
+            for exch in self._general_exch: B_eff_general = exch.local_exch_field(sp_lat,site_idx)
             B_eff += B_eff_general/(self._g_factor*self._S_values[iat]*muB)  # convert from meV to Tesla
         B_eff+= self.calc_SIA_exch_field(sp_lat,site_idx)   # already in unit of Tesla
 
         # homogeneous Zeeman field
         B_eff += self._Bfield
 
         # imhomogeneous magnetic field
@@ -535,17 +537,17 @@
         E_SIA = 0
         for iaxis in range(self._naxis_bl):
             E_SIA -= self._BL_SIA[iaxis][iat] * np.dot(n_i,self._BL_SIA_axis[iaxis][iat])**2
         for iaxis in range(self._naxis_bq):
             E_SIA -= self._BQ_SIA[iaxis][iat] * np.dot(n_i,self._BQ_SIA_axis[iaxis][iat])**4
         E_zeeman = -np.dot(n_i, self._Bfield)*2*self._S_values[iat]*muB
         E_exch = 0.
-        for exch in self._BL_exch: E_exch += exch.calc_local_exchange_energy(sp_lat,site_idx,self._boundary_condition)
-        for exch in self._BQ_exch: E_exch += exch.calc_local_exchange_energy(sp_lat,site_idx,self._boundary_condition)
-        for exch in self._general_exch: E_exch += exch.calc_local_exchange_energy(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._BL_exch: E_exch += exch.local_exchange_energy(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._BQ_exch: E_exch += exch.local_exchange_energy(sp_lat,site_idx,self._boundary_condition)
+        for exch in self._general_exch: E_exch += exch.local_exchange_energy(sp_lat,site_idx,self._boundary_condition)
         E_local = E_SIA + E_zeeman + E_exch
         return E_local
 
 
     def calculate_MAE(self,sp_lat,rotation_plane='xoz',collinear_magmom=None,max_deg=360,deg_step=5,verbosity=1):
         return calc_MAE(self.calc_total_E,sp_lat,self._spin_coord,rotation_plane,collinear_magmom,max_deg,deg_step,verbosity)
```

### Comparing `pyasd-0.0.2/asd/core/llg_advanced.py` & `pyasd-0.0.3/asd/core/llg_advanced.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/core/llg_simple.py` & `pyasd-0.0.3/asd/core/llg_simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,25 +71,27 @@
     print ('This might lead to waste of computational resources')
     print ('No of cores = {}, No of sites for dynamics = {}'.format(size,ntask))
     print ('Duck bu bi')
     print ('Try setting number of cores no more than number of sites\n')
 
 
 shared_memory_warning = '''
-Warning from mpi_llg_simulation_shared_memory:
+{0}\nWarning from mpi_llg_simulation_shared_memory\n{0}
 You are using the shared memory functionality
 It is still under extensive tests
+
 Currently only single-node calculations have been tested
 If you invoke multi nodes, inter-node communication is important
-If you are not sure whether it works correctly on your platform
-It is recommended to use the routine parallel version: 
-mpi_llg_simulation
 Some inter-node communication problem may be solved by adding
 export I_MPI_FABRICS=shm:tcp
-to your job-submission script or .bashrc file\n'''
+to your job-submission script or .bashrc file
+
+If you are not sure whether it works correctly on your platform
+It is recommended to use the routine parallel version: 
+mpi_llg_simulation\n'''.format('#'*60)
 
 
 Note_therml_field_method = ''' 
 We currently support two fields to generate random fields for modeling the thermal effect.
 You set thermal_field_method to {}
 We recommand setting thermal_field_method to 1
 
@@ -204,14 +206,36 @@
 
     def __copy__(self):  return copy(self)
 
 
     def __deepcopy__(self, memo):   return copy.deepcopy(self)
 
 
+    def set_name(self,name):
+        self._name = name
+
+    
+    def set_alpha(self,alpha): 
+        self._alpha = alpha
+        self._factor = gamma_e/(1+self._alpha**2)
+        self._thermal_factor = 2*self._alpha*kB*self._temperature*muB/gamma_e/self._dt
+ 
+
+    def set_dt(self,dt): 
+        self._dt = dt
+        self._thermal_factor = 2*self._alpha*kB*self._temperature*muB/gamma_e/self._dt
+        self._llg_time = np.arange(0,self._dt*(self._nstep+1),self._dt)
+
+
+    def set_temperature(self, temperature):
+        self._temperature = temperature
+        self._thermal_factor = 2*self._alpha*kB*self._temperature*muB/gamma_e/self._dt
+ 
+
+
     def set_verbosity(self,verbosity):
         err = 'LLG_solver: You try to set verbosity = {}, it should be an non-negative integer!'.format(verbosity)
         assert type(verbosity)==int and verbosity>=0, err
         self._verbosity = verbosity
 
 
     def set_log_handle(self,log_handle):
@@ -458,19 +482,19 @@
         else: max_H = -1
         mm=np.average(sp_lat,axis=tuple(range(len(sp_lat.shape)-1)))
         print (fmt_log.format(it,time.time()-stime,self._llg_time[it],Etot_new,diff_E,mm[0],mm[1],mm[2],max_H))
         sys.stdout.flush()
 
 
     def finalize_LLG(self,run_steps,stime,log_time,log_ener,log_conf,verbosity,dE=0):
-        print ('-'*125)
-        print ('\nStop LLG simulation', end=' ')
-        if run_steps==self._nstep: print ('because max iteration limitation')
-        else: print ('because total energy convergence is achieved')
         if verbosity:
+            print ('-'*125)
+            print ('\nStop LLG simulation', end=' ')
+            if run_steps==self._nstep: print ('because max iteration limitation')
+            else: print ('because total energy convergence is achieved')
             print ('Finished at {}'.format(time.ctime()))
             print ('Time used : {:10.4f} s'.format(time.time()-stime))
             print ('Final energy = {:14.8f} meV/site'.format(log_ener[-1]))
             print ('\n{0}\nLLG simulation: End\n{0}\n'.format('*'*125))
         log_llg_data(log_time[-1:],log_ener[-1:],log_conf[-1:],log_conf_file=self._final_conf_file,archive_file=None,dE=dE)
 
 
@@ -552,24 +576,24 @@
         force = None
         Q = None
         sp_lat_log = copy.copy(sp_lat)
         if self._log_force: force = self.mpi_calc_A_vec(ham,sp_lat,dyn_idx,**kwargs2)
         if ham._spin_coord is not None: sp_lat_log = np.dot(sp_lat,ham._spin_coord)
         if self._log_topo_chg: Q = mpi_calc_topo_chg_one_conf(sp_lat_log,tri_simplices = self._tri_simplices)
         en0 = ham.calc_total_E(sp_lat,parallel=True,average_on_sites=True)
-        log_time,log_ener,log_conf,log_Q = self.first_step_LLG(ham,sp_lat_log,en0,force,Q,verbosity=(rank==self._rank_root))
+        log_time,log_ener,log_conf,log_Q = self.first_step_LLG(ham,sp_lat_log,en0,force,Q,verbosity=(rank==self._rank_root)*self._verbosity)
 
         stime=time.time()
         start,last = mt.assign_task(ntask,size,rank, self._free_root)
         updated_sp_lat = np.zeros((last-start,3),float)
 
         count = 0
         fil_archive = self._archive_file
         for it in range(1,self._nstep+1):
-            log_flag = (it%(max(1,self._n_log_magnetization))==0)
+            log_flag = ( (it%(max(1,self._n_log_magnetization))==0) or it==self._nstep )
             if log_flag:  Etot_old  = ham.calc_total_E(sp_lat,parallel=True,average_on_sites=True)
 
             A_vec_all = self.mpi_calc_A_vec(ham,sp_lat,dyn_idx,**kwargs1)
 
             for nn,idx0 in enumerate(dyn_idx[start:last]):
                 rot_mat = RT.from_rotvec(A_vec_all[nn]*self._dt).as_matrix()
                 updated_sp_lat[nn] = np.dot(rot_mat,sp_lat[tuple(idx0)])
@@ -655,15 +679,16 @@
         force = None
         Q = None
         sp_lat_log = copy.copy(sp_lat)
         if self._log_force: force = self.mpi_calc_A_vec_shared_memory(ham,A_vec_all,sp_lat,sp_lat_predict,B_th,dyn_idx,**kwargs2)
         if ham._spin_coord is not None: sp_lat_log = np.dot(sp_lat,ham._spin_coord)
         if self._log_topo_chg: Q = mpi_calc_topo_chg_one_conf(sp_lat_log,tri_simplices = self._tri_simplices)
         en0 = ham.calc_total_E(sp_lat,parallel=True,average_on_sites=True)
-        log_time,log_ener,log_conf,log_Q = self.first_step_LLG(ham,sp_lat_log,en0,force,Q,verbosity=(rank==self._rank_root))
+        log_time,log_ener,log_conf,log_Q = self.first_step_LLG(ham,sp_lat_log,en0,force,Q,
+        verbosity=(rank==self._rank_root)*self._verbosity,func_name='mpi_llg_simulation_shared_memory')
 
         stime=time.time()
         start,last = mt.assign_task(ntask,size,rank, self._free_root)
         comm.barrier()
         count = 0
         fil_archive = self._archive_file
         for it in range(1,self._nstep+1):
```

### Comparing `pyasd-0.0.2/asd/core/log_general.py` & `pyasd-0.0.3/asd/core/log_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,17 @@
         self._log_Q_file      = self._log_Q_file.replace(self._outdir,outdir)
         self._archive_file    = self._archive_file.replace(self._outdir,outdir)
         if self._log_file is not None: self._log_file = self._log_file.replace(self._outdir,outdir)
         self._outdir = outdir
 
 
     def prepare_logging_dir(self):
-        if self._outdir not in ['.','./',os.getcwd()] and self._remove_existing_outdir:
-            if os.path.isdir(self._outdir): os.system('rm -r {} 2>/dev/null'.format(self._outdir))
+        if self._outdir not in ['.','./',os.getcwd()]:
+            if os.path.isdir(self._outdir) and self._remove_existing_outdir: 
+                os.system('rm -r {} 2>/dev/null'.format(self._outdir))
             if not os.path.isdir(self._outdir): os.mkdir(self._outdir)
 
 
 if __name__=='__main__':
     log_handle = log_general()
     fmt = '{:>25s}  =  {:<20s}'
     for key in log_handle.__dict__.keys():
```

### Comparing `pyasd-0.0.2/asd/core/monte_carlo.py` & `pyasd-0.0.3/asd/core/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/core/random_vectors.py` & `pyasd-0.0.3/asd/core/random_vectors.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/core/shell_exchange.py` & `pyasd-0.0.3/asd/core/shell_exchange.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 #*********************************************************
 
 # Important Note: effective fields calculated in this script are in meV
 # the spins are normalized to be unit vectors
 
 
 from __future__ import print_function
+import os
 import numpy as np
 from scipy.spatial.transform import Rotation as RT
 import copy
 from asd.utility.head_figlet import err_text
 try:
     import asd.mpi.mpi_tools as mt
     comm,size,rank,node = mt.get_mpi_handles()
@@ -60,23 +61,24 @@
         nx,ny,nz,nat = shape[:4]
         mgrid = np.mgrid[:nx,:ny,:nz,:nat]
         idx=np.transpose(mgrid,(1,2,3,4,0))
         if fix_boundary: idx = idx[1:-1,1:-1,1:-1]
         idx = idx.reshape(-1,4)
     else:
         print (err_text)
-        exit ('get_latt_idx: sp_lat with invalide shape!')
+        exit ('get_latt_idx: sp_lat with invalid shape!')
     if pinned_idx is not None:
         for idx0 in pinned_idx:
             idx = idx[np.linalg.norm(idx-idx0,axis=1)!=0]
     if savetxt:
         qn = 'nx ny nz nat'.split()
         if idx.shape[1]==4: qn.remove('nz')
         fmt = '{:>5s}'+' {:>7s}'*(len(qn)-1)
-        np.savetxt('{}/dyn_idx.dat'.format(outdir),idx,fmt='%7d',header=fmt.format(*tuple(qn)))
+        if os.path.isdir(outdir)==False: print ('skip saving dyn_idx.dat because {} not found'.format(outdir))
+        else: np.savetxt('{}/dyn_idx.dat'.format(outdir),idx,fmt='%7d',header=fmt.format(*tuple(qn)))
     return nx,ny,nz,nat,idx
 
 
 
 # get the exchange matrix/vector for all neighbors, from one specific pair
 # via symmetric operation (rotation)
 def get_exchange_xyz(exch,rotvec_neighbor):
@@ -102,33 +104,14 @@
         for j,idx_n in enumerate(neigh_idx[iat]):
             idx1 = [(m+n)%s for m,n,s in zip(idx0[:-1],idx_n[:-1],shape[:-2])] + [idx_n[-1]]
             neigh_idx_all[tuple(idx0)][j] = idx1
     return neigh_idx_all
 
 
 
-# !!! UNDER TEST !!!
-# use single count to speed up the cycling
-# may be efficient for large cells than double counting
-def get_single_count_neigh_idx(neigh_idx):
-    single_count_neigh_idx = neigh_idx.tolist()
-    nat = len(neigh_idx)
-    dc_index = []  # index corresponding to double counting
-    for iat in range(nat):
-        dc_index.append([])
-        rm_list = []
-        for inn,idx in enumerate(single_count_neigh_idx[iat]):
-            if -1 in np.sign(idx[:-1]) or (np.sum(np.abs(idx[:-1]))==0 and iat>idx[-1]):
-                dc_index[iat].append(inn)
-                rm_list.append(idx)
-        for idx in rm_list: single_count_neigh_idx[iat].remove(idx)
-    return single_count_neigh_idx,dc_index
-
-
-
 # suppose a magnetic bond is composed of sites 1 and 2
 # idx0 is the index for site 1 of the bond
 # idx_n is the neighbor index given in magnetic unit cell
 # idx1 is the index for site 2 of the bond 
 # if the bond is broken down due to open boundary
 # the function returns None
 #
@@ -144,34 +127,35 @@
     for k,item in enumerate(idx1):
         if boundary_condition[k]==0 and (item<0 or item>shape[k]-1): return None
         else: idx1[k] = item%shape[k]
     idx1 += [idx_n[-1]]
     return idx1
 
 
+fmt_head = '{:>3s} '*4+'{:>10s}'*3
+fm1 = '{:3d} '+'{:3.0f} '*3+'{:10.4f}'*3
+fm2 = (' '*16+'{:10.4f}'*3+'\n')*2
+head_tags = ['iat','Rx','Ry','jat','x','y','z']
 
 def display_exchange(neigh_idx,exchange_xyz,exchange_type,file_handle=None):
     if exchange_xyz is None: return 1
     if np.max(abs(exchange_xyz)):
         print ('\n{0}'.format(exchange_type),file=file_handle)
-        print (('{:>3s} '*4+'{:>10s}'*3).format('iat','Rx','Ry','jat','x','y','z'),file=file_handle)
-    fm1 = '{:3d} '+'{:3.0f} '*3+'{:10.4f}'*3
+        print (fmt_head.format(*tuple(head_tags)),file=file_handle)
     for iat,inn in np.ndindex(*tuple(exchange_xyz.shape[:2])):
         if np.linalg.norm(exchange_xyz[iat,inn]):
             print (fm1.format(iat,*tuple(np.append(neigh_idx[iat,inn],exchange_xyz[iat,inn]))),file=file_handle)
         if inn==exchange_xyz.shape[1]-1: print ('',file=file_handle)
 
 
 def display_exchange_matrix(neigh_idx,exchange_xyz,exchange_type,file_handle=None):
-    fm1 = '{:3d} '+'{:3.0f} '*3+'{:10.4f}'*3
-    fm2 = (' '*16+'{:10.4f}'*3+'\n')*2
     if exchange_xyz is None: return 1
     if np.max(abs(exchange_xyz)):
         print ('\n{0}'.format(exchange_type),file=file_handle)
-        print (('{:>3s} '*4+'{:>10s}'*3).format('iat','Rx','Ry','jat','x','y','z'),file=file_handle)
+        print (fmt_head.format(*tuple(head_tags)),file=file_handle)
         for iat,inn in np.ndindex(*tuple(exchange_xyz.shape[:2])):
             if np.max(abs(exchange_xyz[iat,inn])):
                 print (fm1.format(iat,*tuple(np.append(neigh_idx[iat,inn],exchange_xyz[iat,inn,0]))),file=file_handle)
                 print (fm2.format(*tuple(exchange_xyz[iat,inn,1:].flatten())),file=file_handle)
     else:
         print ('{} is set but the magnitude is zero'.format(exchange_type),file=file_handle)
 
@@ -188,15 +172,14 @@
         self._J_sym_xyz = J_sym_xyz
         self._DM_xyz = DM_xyz
         self._Kitaev_mag = Kitaev_mag
         self._Kitaev_xyz = Kitaev_xyz
         self._Jmat = Jmat
         self._shell_name = shell_name
         self._nat = len(self._neigh_idx) 
-        self._single_count_neigh_idx = get_single_count_neigh_idx(neigh_idx)
 
         if J_sym_xyz is not None and self._Jmat is None: self._Jmat = self.calc_Jmat()
 
 
     def calc_Jmat(self):
         nat,nneigh = self._neigh_idx.shape[:2]
         Jmat = np.zeros((nat,nneigh,3,3),float)
@@ -234,15 +217,15 @@
             if self._Kitaev_mag is not None:
                 if np.linalg.norm(self._Kitaev_mag):
                     print (('\nKitaev strength '+'{:10.4f}'*self._nat).format(*tuple(self._Kitaev_mag)),file=file_handle)
                     display_exchange(self._neigh_idx,self._Kitaev_xyz,'Kitaev',file_handle=file_handle)
         display_exchange(self._neigh_idx,self._DM_xyz,'DM',file_handle=file_handle)
 
 
-    def calc_shell_isotropic_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
+    def shell_isotropic_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         ntask = len(idx)
         start,last = (0,ntask)
         if parallel and enable_mpi: start,last = mt.assign_task(ntask,size,rank)
         E_iso = 0.
         for ii,idx0 in enumerate(idx[start:last]):
@@ -253,15 +236,15 @@
                 if idx1 is not None:
                     n_j = sp_lat[tuple(idx1)]
                     E_iso -= self._J_iso[iat]*np.dot(n_i,n_j)
         if parallel: E_iso = comm.allreduce(E_iso)
         return E_iso/2
 
 
-    def calc_shell_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
+    def shell_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         ntask = len(idx)
         start,last = (0,ntask)
         if parallel and enable_mpi: start,last = mt.assign_task(ntask,size,rank)
  
         E_iso = 0.
@@ -283,15 +266,15 @@
         if parallel: 
             E_iso = comm.allreduce(E_iso)
             E_sym = comm.allreduce(E_sym)
             E_DMI = comm.allreduce(E_DMI)
         return E_iso/2, E_DMI/2, E_Kitaev/2
 
 
-    def calc_shell_exch_energy_from_sym_mat(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
+    def shell_exch_energy_from_sym_mat(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         ntask = len(idx)
         start,last = (0,ntask)
         if parallel and enable_mpi: start,last = mt.assign_task(ntask,size,rank)
         E_sym = 0.
         E_DMI = 0.
@@ -306,15 +289,15 @@
                     if self._DM_xyz is not None: E_DMI -= np.linalg.det([self._DM_xyz[iat,j],n_i,n_j])
         if parallel: 
             E_sym = comm.allreduce(E_sym)
             E_DMI = comm.allreduce(E_DMI)
         return E_sym/2, E_DMI/2
 
 
-    def calc_shell_exch_energy_from_Jmat(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
+    def shell_exch_energy_from_Jmat(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
         if self._Jmat is None: return 0
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         ntask = len(idx)
         start,last = (0,ntask)
         if parallel and enable_mpi: start,last = mt.assign_task(ntask,size,rank)
         E_exch = 0.
@@ -326,54 +309,55 @@
                 if idx1 is not None:
                     n_j = sp_lat[tuple(idx1)]
                     E_exch -= np.dot(np.dot(n_i,self._Jmat[iat,j]),n_j)
         if parallel: E_exch = comm.allreduce(E_exch)
         return E_exch/2
 
 
-    def calc_shell_exch_energy_from_Jmat_new(self,sp_lat):
-        neigh_idx_all = calc_neighbors_in_sp_lat(self._neigh_idx,sp_lat)
+    def shell_exch_energy_from_Jmat_new(self,sp_lat):
         nat = sp_lat.shape[-2]
         E_exch = 0
         for iat in range(nat):
             for j,idx_n in enumerate(self._neigh_idx[iat]):
-                sp_lat_tmp = np.roll(sp_lat,tuple(-idx_n[:-1][::-1]),axis=tuple(range(len(idx_n)-1)[::-1]))
-                E_exch -= np.einsum('...m,mn,...n',sp_lat[...,iat,:],self._Jmat[iat,j],sp_lat_tmp[...,idx_n[-1],:]).sum()
+                dR = idx_n[:-1]
+                jat = idx_n[-1]
+                sp_lat_tmp = np.roll(sp_lat,tuple(-dR),axis=range(len(dR)))
+                E_exch -= np.einsum('...m,mn,...n',sp_lat[...,iat,:],self._Jmat[iat,j],sp_lat_tmp[...,jat,:]).sum()
         return E_exch/2
 
 
-    def calc_local_exchange_energy(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def local_exchange_energy(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         shape=sp_lat.shape
         E_local = 0.
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         for j,idx_n in enumerate(self._neigh_idx[iat]):
             idx1 = calc_neigh_bond_idx(site_idx,idx_n,shape,boundary_condition)
             if idx1 is None: continue
             n_j = sp_lat[tuple(idx1)]
             if self._Jmat is not None: E_local -= np.dot(np.dot(n_i,self._Jmat[iat,j]),n_j)
             else: E_local -= self._J_iso[iat]*np.dot(n_i,n_j)
         return E_local
  
 
-    def calc_shell_isotropic_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def shell_isotropic_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         B_eff = np.zeros(3,float)
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         for j,idx_n in enumerate(self._neigh_idx[iat]):
             idx1 = calc_neigh_bond_idx(site_idx,idx_n,shape,boundary_condition)
             if idx1 is not None:
                 n_j = sp_lat[tuple(idx1)]
                 B_eff += self._J_iso[iat]*n_j
         return B_eff
 
 
-    def calc_shell_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def local_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         B_eff = np.zeros(3,float)
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         for j,idx_n in enumerate(self._neigh_idx[iat]):
             idx1 = calc_neigh_bond_idx(site_idx,idx_n,shape,boundary_condition)
@@ -382,45 +366,45 @@
                 B_eff += self._J_iso[iat]*n_j
                 B_eff += np.cross(n_j,self._DM_xyz[iat,j])
                 if self._Kitaev_mag is not None:
                     B_eff += self._Kitaev_mag[iat]*np.dot(n_j,self._Kitaev_xyz[iat,j])*self._Kitaev_xyz[iat,j]
         return B_eff
 
 
-    def calc_shell_exch_field_from_sym_mat(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def local_exch_field_from_sym_mat(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         B_eff = np.zeros(3,float)
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         for j,idx_n in enumerate(self._neigh_idx[iat]):
             idx1 = calc_neigh_bond_idx(site_idx,idx_n,shape,boundary_condition)
             if idx1 is not None:
                 n_j = sp_lat[tuple(idx1)]
                 B_eff += np.dot(self._J_sym_xyz[iat,j], n_j)
                 B_eff += np.cross(n_j,self._DM_xyz[iat,j])
         return B_eff
 
 
-    def calc_shell_exch_field_from_Jmat(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def local_exch_field_from_Jmat(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         if self._Jmat is None: return np.zeros(3)
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         B_eff = np.zeros(3,float)
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         for j,idx_n in enumerate(self._neigh_idx[iat]):
             idx1 = calc_neigh_bond_idx(site_idx,idx_n,shape,boundary_condition)
             if idx1 is not None:
                 n_j = sp_lat[tuple(idx1)]
                 B_eff += np.dot(self._Jmat[iat,j], n_j)
         return B_eff
 
 
-    def calc_shell_exch_field_from_Jmat_new(self,sp_lat,site_idx):
+    def local_exch_field_from_Jmat_new(self,sp_lat,site_idx):
         neigh_idx_all = calc_neighbors_in_sp_lat(self._neigh_idx,sp_lat)
         B_eff = np.zeros(3,float)
         iat = site_idx[-1]
         for j,idx1 in enumerate(neigh_idx_all[tuple(site_idx)]):
             n_j = sp_lat[tuple(idx1)]
             B_eff += np.dot(self._Jmat[iat,j], n_j)
         return B_eff
@@ -431,24 +415,23 @@
 # the magnitude is given by BQ
 class biquadratic_exchange_shell():
     def __init__(self,neigh_idx,BQ,shell_name):
         self._neigh_idx = neigh_idx
         self._BQ = BQ
         self._shell_name = shell_name
         self._nat = len(self._neigh_idx)
-        self._single_count_neigh_idx = get_single_count_neigh_idx(neigh_idx)
 
 
     def verbose_interactions(self,file_handle=None):
         print ('\nBiquadratic exchange {}'.format(self._shell_name),file=file_handle)
         try: print (('{:8.5f} '*len(self._BQ)+'\n').format(*tuple(self._BQ)),file=file_handle)
         except: print ('None',file=file_handle)
 
 
-    def calc_shell_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
+    def shell_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         ntask = len(idx)
         start,last = (0,ntask)
         if parallel and enable_mpi: start,last = mt.assign_task(ntask,size,rank)
         E_bq = 0.
         for idx0 in idx[start:last]:
@@ -458,42 +441,42 @@
                 idx1 = calc_neigh_bond_idx(idx0,idx_n,shape,boundary_condition)
                 if idx1 is not None:
                     n_j = sp_lat[tuple(idx1)]
                     E_bq -= self._BQ[iat] * (n_i[2]*n_j[2])**2
         return E_bq/2
 
 
-    def calc_shell_exch_energy_new(self,sp_lat):
+    def shell_exch_energy_new(self,sp_lat):
         neigh_idx_all = calc_neighbors_in_sp_lat(self._neigh_idx,sp_lat)
         shape = sp_lat.shape
         E_bq = 0.
         for idx0 in np.ndindex(shape[:-1]):
             n_i = sp_lat[tuple(idx0)]
             iat = idx0[-1]
             for j,idx1 in enumerate(neigh_idx_all[tuple(idx0)]):
                 n_j = sp_lat[tuple(idx1)]
                 E_bq -= self._BQ[iat] * (n_i[2]*n_j[2])**2
         if parallel: E_bq = comm.allreduce(E_bq)
         return E_bq/2
 
 
-    def calc_shell_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def local_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         shape = sp_lat.shape
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         B_eff = np.zeros(3)
         for j,idx_n in enumerate(self._neigh_idx[iat]):
             idx1 = calc_neigh_bond_idx(site_idx,idx_n,shape,boundary_condition)
             if idx1 is not None:
                 n_j = sp_lat[tuple(idx1)]
                 B_eff += 2*self._BQ[iat]*n_i[2]*n_j[2]**2
         return B_eff
 
 
-    def calc_shell_exch_field_new(self,sp_lat,site_idx):
+    def local_exch_field_new(self,sp_lat,site_idx):
         neigh_idx_all = calc_neighbors_in_sp_lat(self._neigh_idx,sp_lat)
         shape = sp_lat.shape
         n_i = sp_lat[tuple(site_idx)]
         iat = site_idx[-1]
         B_eff = np.zeros(3)
         for j,idx1 in enumerate(neigh_idx_all[tuple(site_idx)]):
             n_j = sp_lat[tuple(idx1)]
@@ -511,23 +494,22 @@
 # the previous class
 class biquadratic_exchange_shell_general():
     def __init__(self,neigh_idx,BQ,shell_name):
         self._neigh_idx = neigh_idx
         self._BQ = BQ
         self._shell_name = shell_name
         self._nat = len(self._neigh_idx)
-        self._single_count_neigh_idx = get_single_count_neigh_idx(neigh_idx)
 
 
     def verbose_interactions(self,file_handle=None):
         print ('\nBiquadratic exchange {}, in generic matrix form'.format(self._shell_name),file=file_handle)
         display_exchange_matrix(self._neigh_idx,self._BQ,'Biquadratic exchange',file_handle=file_handle)
 
 
-    def calc_shell_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
+    def shell_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         ntask = len(idx)
         start,last = (0,ntask)
         if parallel and enable_mpi: start,last = mt.assign_task(ntask,size,rank)
         E_bq = 0.
         for idx0 in idx[start:last]:
@@ -538,62 +520,81 @@
                 if idx1 is not None:
                     n_j = sp_lat[tuple(idx1)]
                     E_bq -= np.einsum('mn,m,n', self._BQ[iat,j], n_i, n_j)**2
         if parallel: E_bq = comm.allreduce(E_bq)
         return E_bq/2
 
 
-    def calc_shell_exch_energy_new(self,sp_lat):
+    def shell_exch_energy_new(self,sp_lat):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         E_bq = 0.
         for iat in range(nat):
             for j,idx_n in enumerate(self._neigh_idx[iat]):
-                sp_lat_tmp = np.roll(sp_lat,tuple(-idx_n[:-1][::-1]),axis=tuple(range(len(idx_n)-1)[::-1]))
-                E_bq -= (np.einsum('...m,mn,...n',sp_lat[...,iat,:],self._BQ[iat,j],sp_lat_tmp[...,idx_n[-1],:])**2).sum()
+                dR = idx_n[:-1]
+                jat = idx_n[-1]
+                sp_lat_tmp = np.roll(sp_lat,tuple(-dR),axis=range(len(dR)))
+                E_bq -= (np.einsum('...m,mn,...n',sp_lat[...,iat,:],self._BQ[iat,j],sp_lat_tmp[...,jat,:])**2).sum()
         return E_bq/2
 
 
-    def calc_local_exchange_energy(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def local_exchange_energy(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         shape = sp_lat.shape
         E_local = 0.
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         for j,idx_n in enumerate(self._neigh_idx[iat]):
             idx1 = calc_neigh_bond_idx(site_idx,idx_n,shape,boundary_condition)
             if idx1 is None: continue
             n_j = sp_lat[tuple(idx1)]
             E_local -= np.einsum('mn,m,n', self._BQ[iat,j], n_i, n_j)**2
         return E_local
 
 
-    def calc_shell_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def local_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         shape = sp_lat.shape
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         B_eff = np.zeros(3)
         for j,idx_n in enumerate(self._neigh_idx[iat]):
             idx1 = calc_neigh_bond_idx(site_idx,idx_n,shape,boundary_condition)
             if idx1 is not None:
                 n_j = sp_lat[tuple(idx1)]
                 B_eff += 2*np.einsum('mn,m,n',self._BQ[iat,j],n_i,n_j) * np.dot(self._BQ[iat,j], n_j)
         return B_eff
 
 
-    def calc_shell_exch_field_new(self,sp_lat,site_idx):
+    def local_exch_field_new(self,sp_lat,site_idx):
         n_i = sp_lat[tuple(site_idx)]
         iat = site_idx[-1]
         B_eff = np.zeros(3)
         for j,idx_n in enumerate(self._neigh_idx[iat]):
-            sp_lat_tmp = np.roll(sp_lat,tuple(-idx_n[:-1][::-1]),axis=tuple(range(len(idx_n)-1)[::-1]))
+            dR = idx_n[:-1]
+            jat = idx_n[-1]
+            sp_lat_tmp = np.roll(sp_lat,tuple(-dR),axis=range(len(dR)))
             n_j = sp_lat_tmp[tuple(idx_n)]
             B_eff += 2*np.einsum('mn,m,n',self._BQ[iat,j],n_i,n_j) * np.dot(self._BQ[iat,j],n_j)
         return B_eff
 
 
+    # exchange field over the whole spin lattice
+    def shell_exch_field(self,sp_lat):
+        B_eff = np.zeros_like(sp_lat)
+        nat = sp_lat.shape[-2]
+        for iat in range(nat):
+            for j,idx_n in enumerate(self._neigh_idx[iat]):
+                dR = idx_n[:-1]
+                jat = idx_n[-1]
+                sp_lat_tmp = np.roll(sp_lat,tuple(-dR),axis=tuple(range(len(dR))))
+                B_eff[...,iat,:] += 2*np.einsum('mn,...m,...n->...',self._BQ[iat,j],sp_lat[...,iat,:],sp_lat_tmp[...,jat,:]) * np.dot(self._BQ[iat,j],sp_lat_tmp[...,jat,:])
+        return B_eff
+
+
+
+
 
 # four-site biquadratic exchange coupling
 class four_site_biquadratic_exchange_shell():
     def __init__(self,neigh_idx,BQ,shell_name):
         self._neigh_idx = neigh_idx
         self._BQ = BQ
         self._shell_name = shell_name
@@ -601,15 +602,15 @@
 
 
     def verbose_interactions(self,file_handle=None):
         print ('\nFour-site Biquadratic exchange {}, in generic matrix form'.format(self._shell_name),file=file_handle)
         display_exchange_matrix(self._neigh_idx,self._BQ,'Biquadratic exchange',file_handle=file_handle)
 
 
-    def calc_shell_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
+    def shell_exch_energy(self,sp_lat,boundary_condition=[1,1,1],parallel=False):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         ntask = len(idx)
         start,last = (0,ntask)
         if parallel and enable_mpi: start,last = mt.assign_task(ntask,size,rank)
         E_bq = 0.
         for idx0 in idx[start:last]:
@@ -625,26 +626,28 @@
                 n_k = sp_lat[tuple(idx_k)]
                 n_l = sp_lat[tuple(idx_l)]
                 E_bq -= self._BQ[iat,inn] * np.dot(n_i, n_j) * np.dot(n_k, n_l)
         if parallel:  E_bq = comm.allreduce(E_bq)
         return E_bq
 
 
-    def calc_shell_exch_energy_new(self,sp_lat):
+    def shell_exch_energy_new(self,sp_lat):
         shape = sp_lat.shape
         nx,ny,nz,nat,idx = get_latt_idx(shape)
         E_bq = 0.
         for iat in range(nat):
             for j,idx_n in enumerate(self._neigh_idx[iat]):
-                sp_lat_tmp = np.roll(sp_lat,tuple(-idx_n[:-1][::-1]),axis=tuple(range(len(idx_n)-1)[::-1]))
-                E_bq -= (np.einsum('...m,mn,...n',sp_lat[...,iat,:],self._BQ[iat,j],sp_lat_tmp[...,idx_n[-1],:])**2).sum()
+                dR = idx_n[:-1]
+                jat = idx_n[-1]
+                sp_lat_tmp = np.roll(sp_lat,tuple(-dR),axis=range(len(dR)))
+                E_bq -= (np.einsum('...m,mn,...n',sp_lat[...,iat,:],self._BQ[iat,j],sp_lat_tmp[...,jat,:])**2).sum()
         return E_bq
 
 
-    def calc_local_exchange_energy(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def local_exchange_energy(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         E_local = 0.
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         for inn,idx_n in enumerate(self._neigh_idx[iat]):
             idx_j = calc_neigh_bond_idx(idx0,idx_n[0],shape,boundary_condition)
             idx_k = calc_neigh_bond_idx(idx0,idx_n[1],shape,boundary_condition)
             idx_l = calc_neigh_bond_idx(idx0,idx_n[2],shape,boundary_condition)
@@ -652,15 +655,15 @@
             n_j = sp_lat[tuple(idx_j)]
             n_k = sp_lat[tuple(idx_k)]
             n_l = sp_lat[tuple(idx_l)]
             E_local -= self._BQ[iat,inn] * np.dot(n_i, n_j) * np.dot(n_k, n_l)
         return E_local
 
 
-    def calc_shell_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
+    def local_exch_field(self,sp_lat,site_idx,boundary_condition=[1,1,1]):
         shape = sp_lat.shape
         iat = site_idx[-1]
         n_i = sp_lat[tuple(site_idx)]
         B_eff = np.zeros(3)
         for inn,idx_n in enumerate(self._neigh_idx[iat]):
             idx_j = calc_neigh_bond_idx(site_idx,idx_n[0],shape,boundary_condition)
             idx_k = calc_neigh_bond_idx(site_idx,idx_n[1],shape,boundary_condition)
@@ -670,19 +673,18 @@
             n_j = sp_lat[tuple(idx_j)]
             n_k = sp_lat[tuple(idx_k)]
             n_l = sp_lat[tuple(idx_l)]
             B_eff += self._BQ[iat,inn] * n_j * np.dot(n_k, n_l)
         return B_eff
 
 
-    def calc_shell_exch_field_new(self,sp_lat,site_idx):
+    def local_exch_field_new(self,sp_lat,site_idx):
         n_i = sp_lat[tuple(site_idx)]
         iat = site_idx[-1]
         B_eff = np.zeros(3)
         for inn,idx_n in enumerate(self._neigh_idx[iat]):
-            sp_lat_tmp = np.roll(sp_lat,tuple(-idx_n[:-1][::-1]),axis=tuple(range(len(idx_n)-1)[::-1]))
+            dR = idx_n[:-1]
+            jat = idx_n[-1]
+            sp_lat_tmp = np.roll(sp_lat,tuple(-dR),axis=range(len(dR)))
             n_j = sp_lat_tmp[tuple(idx_n)]
             B_eff += 2*np.einsum('mn,m,n',self._BQ[iat,j],n_i,n_j) * np.dot(self._BQ[iat,inn],n_j)
         return B_eff
-
-
-
```

### Comparing `pyasd-0.0.2/asd/core/spin_configurations.py` & `pyasd-0.0.3/asd/core/spin_configurations.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,16 @@
 Generating random spin configuration
 Important Note: if you use parallel mode
 Please make sure that the initial configuration is only generated
 by one process and broadcast to all other processes
 otherwise some unexpected disorder might occur
 '''
  
-def init_random(sp_lat,method='MultivarNormal',verbosity=1,q_for_Potts=3):
+def init_random(sp_lat,method='MultivarNormal',verbosity=1,q_for_Potts=3,seed=101):
+    np.random.seed(seed)
     if verbosity: print (random_conf_warning)
     shape = sp_lat.shape
     nn = np.prod(shape[:-1])
     spins = gen_random_spins_misc(nn,method,q_for_Potts)
     sp_lat = spins.reshape(shape)
     return sp_lat
```

### Comparing `pyasd-0.0.2/asd/core/spin_correlations.py` & `pyasd-0.0.3/asd/core/spin_correlations.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/core/topological_charge.py` & `pyasd-0.0.3/asd/core/topological_charge.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_Cr2I3X3.py` & `pyasd-0.0.3/asd/data_base/exchange_for_Cr2I3X3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_CrI3.py` & `pyasd-0.0.3/asd/data_base/exchange_for_CrI3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_CrMnI6_U2.py` & `pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_U2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_CrMnI6_U4.py` & `pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_U4.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_CrMnI6_rect.py` & `pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_rect.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_Gd2C.py` & `pyasd-0.0.3/asd/data_base/exchange_for_Gd2C.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_MnI2.py` & `pyasd-0.0.3/asd/data_base/exchange_for_MnI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_NiI2.py` & `pyasd-0.0.3/asd/data_base/exchange_for_NiI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_RuCl3.py` & `pyasd-0.0.3/asd/data_base/exchange_for_RuCl3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_VOI2.py` & `pyasd-0.0.3/asd/data_base/exchange_for_VOI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_kagome.py` & `pyasd-0.0.3/asd/data_base/exchange_for_kagome.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/data_base/exchange_for_skx.py` & `pyasd-0.0.3/asd/data_base/exchange_for_skx.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/mpi/mpi_tools.py` & `pyasd-0.0.3/asd/mpi/mpi_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/utility/Swq.py` & `pyasd-0.0.3/asd/utility/Swq.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/utility/analyze_Spirit_results.py` & `pyasd-0.0.3/asd/utility/analyze_Spirit_results.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/utility/asd_arguments.py` & `pyasd-0.0.3/asd/utility/asd_arguments.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/utility/auxiliary_colormaps.py` & `pyasd-0.0.3/asd/utility/auxiliary_colormaps.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/utility/curve_fit.py` & `pyasd-0.0.3/asd/utility/curve_fit.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,23 +48,23 @@
     yy=func(xx,*args)
     noise = gen_noise(ndata,np.max(np.abs(yy)),0.1)
     yy += noise # add some artificial "noise" to make the scatter points deviate from perfect values
     return xx,yy
 
 
 if __name__=='__main__':
-    from asd.utility.mag_thermal import logarithmic_magnetization
-    # fitting the logarithmic magnetization function
+    from asd.utility.mag_thermal import exponent_magnetization
+    # fitting the exponent magnetization function
     ntemperature = 201
     Tc = 45.
     beta = 0.3
-    xx,yy = gen_dataset(logarithmic_magnetization,ntemperature,(Tc,beta))
+    xx,yy = gen_dataset(exponent_magnetization,ntemperature,(Tc,beta))
 
     p0=(Tc-3,0)  # initial guess of parameters, optional
-    popt,pcov=curve_fit(logarithmic_magnetization,xx,yy,p0)
+    popt,pcov=curve_fit(exponent_magnetization,xx,yy,p0)
     report_fitting(popt,pcov)
 
     kws = dict(figname='Log_magn',
     fitted_args=popt,
     accurate_args=(Tc,beta),
     xlabel='T (K)',ylabel='M')
-    plot_fitting_function(xx,yy,logarithmic_magnetization,**kws)
+    plot_fitting_function(xx,yy,exponent_magnetization,**kws)
```

### Comparing `pyasd-0.0.2/asd/utility/four_state_tools.py` & `pyasd-0.0.3/asd/utility/four_state_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/utility/head_figlet.py` & `pyasd-0.0.3/asd/utility/head_figlet.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         import asd
         self.__dict__.update(asd.__dict__)
 
     def verbose_info(self,fw=None):
         print ('='*60,file=fw)
         print (asd_text,file=fw)
         print ('Basic information'.center(35),file=fw)
-        for key in ['__name__','__version__','__author__','__email__','__built_time__']:
-            print ('{:15s}  =  {:<20s}'.format(key.center(15),self.__dict__[key]),file=fw)
+        for key in ['__name__','__version__','__author__','__author_email__','__built_time__']:
+            print ('{:16s}  =  {:<20s}'.format(key.center(15),self.__dict__[key]),file=fw)
         print ('='*60,file=fw)
 
 
 if __name__=='__main__':
     code_info = pkg_info()
     code_info.verbose_info()
```

### Comparing `pyasd-0.0.2/asd/utility/mag_thermal.py` & `pyasd-0.0.3/asd/utility/mag_thermal.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,33 +142,33 @@
         ax[1,0].text(left,0.9,'$\chi=\\frac{<M^2>-<M>^2}{k_B T}$',fontsize=14,ha='center')
         ax[1,1].text(left,0.9,'$C_v=\\frac{<E^2>-<E>^2}{(k_B T)^2}$',fontsize=14,ha='center')
     fig.tight_layout()
     fig.savefig(figname,dpi=500)
     plt.show()
 
 
-def logarithmic_magnetization(temperature,Tc,beta):
+def exponent_magnetization(temperature,Tc,beta):
     assert Tc>0, 'Critical temperature should be positive!'
     f = 1-(temperature/Tc)
     if type(temperature)==float:
         return np.power(f,beta) if f>0 else 0
     else:
         idx1 = np.where(f>0)
         M = np.zeros_like(temperature)
         M[idx1] = np.power(f[idx1],beta)
         return M
 
 
 def display_log_magnetization_with_varying_beta(temperatures=np.linspace(0,20,100,),Tc=10,betas=[0.125,np.pi**2*3/128],show=False):
     fig,ax=plt.subplots(1,1,figsize=(6,4))
     for beta in betas:
-        yy = logarithmic_magnetization(temperatures,Tc,beta)
+        yy = exponent_magnetization(temperatures,Tc,beta)
         ax.plot(temperatures,yy,label='$\\beta\ =\ {:.3f}$'.format(beta))
     for beta,label in zip([0.125,np.pi**2*3/128],['Ising','XY']):
-        yy = logarithmic_magnetization(temperatures,Tc,beta)
+        yy = exponent_magnetization(temperatures,Tc,beta)
         ax.plot(temperatures,yy,lw=3,label='$\\beta\ =\ {0:.3f}$'.format(beta)+' 2D {}'.format(label))
     ax.legend()
     ax.set_xlabel('T (K)')
     ax.set_ylabel('M')
     fig.tight_layout()
     fig.savefig('Tc_beta_power',dpi=400)
     if show: plt.show()
```

### Comparing `pyasd-0.0.2/asd/utility/ovf_tools.py` & `pyasd-0.0.3/asd/utility/ovf_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,19 +187,20 @@
     nconf = len(start_idx)
     start = start_idx[0]
     final = final_idx[0]
     mags = np.zeros((nconf,3))
     spins = []
     stime = time.time()
     if verbosity: print (('{:>7s} '*4+'{:>12s}').format('Now','Total','Start','Last','used time'))
+    fmt = '{:7d} '*4+'  {:8.2f} s    {}'
     with open(fil_ovf) as f_input:
         for ii in range(nconf):
             if ii==0: FH = np.loadtxt(itertools.islice(f_input, start, final))
             else: FH = np.loadtxt(itertools.islice(f_input, start-2, final-2))
-            if verbosity and ii%(nconf//20): print (('{:7d} '*4+'  {:8.2f} s    {}').format(ii,start,final,final-start,time.time()-stime,FH.shape))
+            if verbosity and ii%(nconf//20): print (fmt.format(ii,start,final,final-start,time.time()-stime,FH.shape))
             mags[ii] = np.average(FH,axis=0)
             if return_spins: spins.append(FH)
     np.savetxt(fil_mag,mags,fmt='%14.6f')
     spins = np.array(spins)
     return spins, mags
```

### Comparing `pyasd-0.0.2/asd/utility/plot_tools_3d.py` & `pyasd-0.0.3/asd/utility/plot_tools_3d.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/utility/post_llg.py` & `pyasd-0.0.3/asd/utility/post_llg.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         ener = None
         diff_E = None
         force = None
     return time,ener,diff_E,force
 
 
 
-def plot_E_T(show=False):
-    time,ener,diff_E,forc = get_dE_from_out()
+def plot_E_T(outdir='.',show=False):
+    time,ener,diff_E,forc = get_dE_from_out(outdir)
     if time is None : 
         print ('skip plotting diff_E')
         return None,None,None
 
     fig,ax=plt.subplots(1,1)
     ax.plot(time,ener,'b-')
     ax.set_xlabel('Time (ps)')
@@ -73,42 +73,42 @@
     if diff_E is not None:
         axx=ax.twinx()
         axx.plot(time,np.log(abs(diff_E))/np.log(10),'r-')
         axx.set_ylabel('log|dE|',color='r')
         axx.tick_params(axis='y', labelcolor='r')
         axx.set_xlim(0,np.max(time))
     fig.tight_layout()
-    fig.savefig('E_T',dpi=500)
+    fig.savefig('{}/E_T'.format(outdir),dpi=500)
 
     if forc is not None:
         fig1,ax1=plt.subplots(1,1)
         ax1.plot(time,np.log(abs(forc))/np.log(10),'g-')
         ax1.set_xlabel('Time (ps)')
         ax1.set_ylabel('log|forcee|')
         ax1.set_xlim(0,np.max(time))
         fig1.tight_layout()
         fig1.savefig('forc',dpi=500)
     return fig,ax,axx
 
 
 def ax_plot_magnetization(ax,time,data):
     for i in range(3,6): ax.plot(time,data[:,i],label={3:'$M_x$',4:'$M_y$',5:'$M_z$'}[i])
-    ax.plot(time,np.linalg.norm(data[:,3:5],axis=1),label='$M_\parallel$')
+    ax.plot(time,np.linalg.norm(data[:,3:5],axis=1),label='$M_\perp$')
     ax.plot(time,np.linalg.norm(data[:,3:6],axis=1),label='M')
     ax.legend(ncol=2)
     ax.set_xlim(np.min(time),np.max(time))
     ax.set_ylim(-1.1,1.1)
-    ax.set_yticks([-1,0,1])
+    ax.set_yticks(np.arange(-1,1.1,0.5))
     ax.set_xlabel('Time (ps)')
     ax.set_ylabel('M')
  
 
 
-def plot_summary(fil='M.dat',plot_summary=True):
-    data=np.loadtxt(fil,skiprows=1)
+def plot_summary(outdir='.',fil='M.dat',plot_summary=True):
+    data=np.loadtxt('{}/{}'.format(outdir,fil),skiprows=1)
     time = data[:,0]
     ener = data[:,1]
     diff_E = data[:,2]
     if not plot_summary: return data,False
 
     fig,ax=plt.subplots(2,1,sharex=True,figsize=(6,6))
 
@@ -121,15 +121,15 @@
         axx=ax[0].twinx()
         axx.plot(time,np.log(abs(diff_E))/np.log(10),'r-')
         axx.set_ylabel('log|dE|',color='r')
         axx.tick_params(axis='y', labelcolor='r')
 
     ax_plot_magnetization(ax[1],time,data)
     fig.tight_layout()
-    fig.savefig('E_M_T',dpi=500)
+    fig.savefig('{}/E_M_T'.format(outdir),dpi=500)
 
     if data.shape[1]==7:
         Qs = data[:,-1]
         fig,ax=plt.subplots(1,1)
         ax.plot(time,Qs)
         ax.set_xlabel('Time (ps)')
         ax.set_ylabel('Q')
@@ -170,15 +170,15 @@
         conf = np.swapaxes(conf,0,1)
     if args.plot_superlatt: superlatt=np.dot([[nx*args.repeat_x,0],[0,ny*args.repeat_y]],latt)
     else: superlatt = None
     sites_repeat = get_repeated_sites(sites,args.repeat_x,args.repeat_y)
     sites_cart_repeat = np.dot(sites_repeat,latt)
     conf_repeat = get_repeated_conf(conf,args.repeat_x,args.repeat_y)
 
-    figname='{0}_{1}.png'.format(head,tag)
+    figname='{}/{}_{}.png'.format(args.outdir,head,tag)
     if title is None: title='{} '.format(tag)
     spin_plot_kwargs.update(
     color_mapping=args.color_mapping,
     title=title,
     figname=figname,
     superlatt=superlatt,
     colorbar_axes_position=args.colorbar_axes_position)
@@ -222,15 +222,15 @@
     spin_anim_kwargs = get_spin_anim_kwargs(args)
     spin_anim_kwargs.update(quiver_kws=quiver_kws)
 
     fil_archive='M.dat'
     if args.prefix!='': fil_archive = '{}_M.dat'.format(args.prefix)
     fil_archive = glob.glob('{}/{}'.format(args.outdir,fil_archive))
     if args.plot_out: fig,ax,axx = plot_E_T(outdir=args.outdir)
-    if fil_archive:  data,calc_Q = plot_summary(fil_archive[0],plot_summary=args.plot_summary)
+    if fil_archive:  data,calc_Q = plot_summary('.',fil_archive[0],plot_summary=args.plot_summary)
     else: calc_Q=True
     plt.show()
 
     llg = importlib.import_module(args.llg_file.rstrip('.py'))
     lat_type = args.lat_type
     if args.nx==0:  nx=llg.nx
     else: nx = args.nx
@@ -265,21 +265,22 @@
         fil_conf=fil_conf[0]
         lines=open(fil_conf).readlines()
         idx=np.where([re.search('time =',line) for line in lines])[0]
         log_time=np.array([lines[ii].split('=')[1].rstrip('ps\n') for ii in idx],float) 
         idx=np.where([re.search('ener =',line) for line in lines])[0]
         log_ener=np.array([lines[ii].split('=')[1].rstrip('meV\n') for ii in idx],float)
 
+        confs_pickle = '{}/spin_confs.pickle'.format(args.outdir)
         if args.pick_confs: 
-            assert os.path.isfile('spin_confs.pickle'),'Set pick_confs = True but spin_confs.pickle not found!'
-            print ('Load spin configurations from spin_confs.pickle')
-            confs = pickle.load(open('spin_confs.pickle','rb'))
+            assert os.path.isfile(confs_pickle), 'Set pick_confs = True but spin_confs.pickle not found!'
+            print ('Load spin configurations from {}'.format(confs_pickle))
+            confs = pickle.load(open(confs_pickle,'rb'))
         else: 
             params,confs=parse_ovf(fil_conf,parse_params=True)
-            if args.dump_confs: pickle.dump(confs,open('spin_confs.pickle','wb'))
+            if args.dump_confs: pickle.dump(confs,open(confs_pickle,'wb'))
 
         if args.write_latest:
             fil_latest = 'latest_spin_confs.ovf'
             print ('Latest configuration written to {}'.format(fil_latest))
             spins_latest = confs[-1]
             params['nsegment'] = 1
             write_ovf(params,spins_latest,filename=fil_latest)
```

### Comparing `pyasd-0.0.2/asd/utility/post_mc.py` & `pyasd-0.0.3/asd/utility/post_mc.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/utility/spin_visualize_tools.py` & `pyasd-0.0.3/asd/utility/spin_visualize_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/asd/utility/spirit_tool.py` & `pyasd-0.0.3/asd/utility/spirit_tool.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/examples/example1/.coverage` & `pyasd-0.0.3/examples/example1/.coverage`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/examples/example1/single_spin_LLG.py` & `pyasd-0.0.3/examples/example1/single_spin_LLG.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/examples/example2/llg.py` & `pyasd-0.0.3/examples/example2/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/examples/example3/llg.py` & `pyasd-0.0.3/examples/example3/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/examples/example4/llg.py` & `pyasd-0.0.3/examples/example4/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/misc/archives/ovf-0.4.3.tar.gz` & `pyasd-0.0.3/misc/archives/ovf-0.4.3.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/misc/archives/pyfiglet-0.7.tar.gz` & `pyasd-0.0.3/misc/archives/pyfiglet-0.7.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/pyasd.egg-info/SOURCES.txt` & `pyasd-0.0.3/pyasd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 asd/utility/post_llg.py
 asd/utility/post_mc.py
 asd/utility/spin_visualize_tools.py
 asd/utility/spirit_tool.py
 examples/README
 examples/example1/.coverage
 examples/example1/single_spin_LLG.py
-examples/example2/README
+examples/example2/README.md
 examples/example2/llg.py
-examples/example3/README
+examples/example3/README.md
 examples/example3/llg.py
 examples/example4/README
 examples/example4/llg.py
 misc/archives/ovf-0.4.3.tar.gz
 misc/archives/pyfiglet-0.7.tar.gz
 pyasd.egg-info/PKG-INFO
 pyasd.egg-info/SOURCES.txt
```

### Comparing `pyasd-0.0.2/pyasd.egg-info/top_level.txt` & `pyasd-0.0.3/pyasd.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/setup.py` & `pyasd-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 core_modules  = ['asd/core/{}'.format(item) for item in core_modules]
 utility_modules  = ['asd/utility/{}'.format(item) for item in utility_modules]
 mpi_modules = ['asd/mpi/mpi_tools']
 
 
 kwargs_setup = dict(
 name='pyasd',
-version='0.0.2',
+version='0.0.3',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords='spin dynamics simulation',
 py_modules = utility_modules + core_modules + database_modules + mpi_modules + init_files,
 packages = setuptools.find_packages(),
```

### Comparing `pyasd-0.0.2/tests_basic/B_eff/test_B_eff.py` & `pyasd-0.0.3/tests_basic/B_eff/test_B_eff.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/OVF/pyasd_ovf_test.py` & `pyasd-0.0.3/tests_basic/OVF/pyasd_ovf_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/OVF/test_ovf.py` & `pyasd-0.0.3/tests_basic/OVF/test_ovf.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/Potts/Potts_test.py` & `pyasd-0.0.3/tests_basic/mag_confs/Potts/Potts_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/domain_walls/analytical_single_domain.py` & `pyasd-0.0.3/tests_basic/mag_confs/domain_walls/analytical_single_domain.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/domain_walls/dw_test.py` & `pyasd-0.0.3/tests_basic/mag_confs/domain_walls/dw_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/interpolate_images.py` & `pyasd-0.0.3/tests_basic/mag_confs/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py` & `pyasd-0.0.3/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/meron/bimeron.py` & `pyasd-0.0.3/tests_basic/mag_confs/meron/bimeron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py` & `pyasd-0.0.3/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/meron/meron.py` & `pyasd-0.0.3/tests_basic/mag_confs/meron/meron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/misc/interpolate_images.py` & `pyasd-0.0.3/tests_basic/mag_confs/misc/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/misc/mpi_topo.py` & `pyasd-0.0.3/tests_basic/mag_confs/misc/mpi_topo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/misc/regular_order_test.py` & `pyasd-0.0.3/tests_basic/mag_confs/misc/regular_order_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/misc/struct_factor.py` & `pyasd-0.0.3/tests_basic/mag_confs/misc/struct_factor.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/misc/test_pbc_shell.py` & `pyasd-0.0.3/tests_basic/mag_confs/misc/test_pbc_shell.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/skyrmion/Skyrmion.py` & `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/Skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py` & `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/skyrmion/a2sk.py` & `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/a2sk.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/skyrmion/afm_skyrmion.py` & `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/afm_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/skyrmion/firework.py` & `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py` & `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/skyrmion/mpi_firework.py` & `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/mpi_firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/skyrmion/skyrmionium.py` & `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/skyrmionium.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/skyrmion/view_3d_skyr.py` & `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/view_3d_skyr.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/spirals/CrMnI6_spiral.py` & `pyasd-0.0.3/tests_basic/mag_confs/spirals/CrMnI6_spiral.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/spirals/spiral_test.py` & `pyasd-0.0.3/tests_basic/mag_confs/spirals/spiral_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/mag_confs/test_regular_orders_honeycomb.py` & `pyasd-0.0.3/tests_basic/mag_confs/test_regular_orders_honeycomb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py` & `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py` & `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py` & `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     fmt_head='\n'+'='*120+'\n' + 'idx |'+'{:>9s}'*3+' | '+'{:>14s} '*2+'{:>16s} {:>20s}' + '{:>15s}\n'+'-'*120
     print (fmt_head.format('Mx','My','Mz','E_spirit(meV)','my_E_tot(meV)','diff_E(meV)','diff_E(meV/site)',' |  boundary'))
     for i in range(nimage):
         mm=np.average(confs[i],axis=(0,1,2))
         ham.set_boundary_condition(bounds[i])
         en = ham.calc_total_E(confs[i],average_on_sites=False)
-        #en = bq_four_site.calc_shell_exch_energy(confs[i],bounds[i])
+        #en = bq_four_site.shell_exch_energy(confs[i],bounds[i])
         print (('{:3d} |'+fmt).format(i+1,*tuple(mm)),end=' | ')
         print (('{:14.7f} '*2+'{:16.7e} {:20.8e}').format(en_spirit[i],en,en-en_spirit[i],(en-en_spirit[i])/nsites),end = '    | ')
         print(('{:3d} '*3).format(*tuple(bounds[i])))
     print ('='*120)
     os.chdir('..')
```

### Comparing `pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py` & `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py` & `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/simple/input.cfg` & `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/input.cfg`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py` & `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py` & `pyasd-0.0.3/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/large_test/large_cell.py` & `pyasd-0.0.3/tests_basic/total_energy/large_test/large_cell.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py` & `pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py` & `pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/local_energy/test_local_en.py` & `pyasd-0.0.3/tests_basic/total_energy/local_energy/test_local_en.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py` & `pyasd-0.0.3/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/regular_orders/llg.py` & `pyasd-0.0.3/tests_basic/total_energy/regular_orders/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.2/tests_basic/total_energy/regular_orders/phase_diagram_tri.py` & `pyasd-0.0.3/tests_basic/total_energy/regular_orders/phase_diagram_tri.py`

 * *Files identical despite different names*

