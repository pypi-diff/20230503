# Comparing `tmp/pyasd-0.0.3.tar.gz` & `tmp/pyasd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyasd-0.0.3.tar", last modified: Wed May  3 05:05:39 2023, max compression
+gzip compressed data, was "pyasd-0.0.4.tar", last modified: Wed May  3 11:06:49 2023, max compression
```

## Comparing `pyasd-0.0.3.tar` & `pyasd-0.0.4.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1468 2023-01-05 06:57:53.000000 pyasd-0.0.3/LICENSE
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      488 2023-01-06 02:20:47.000000 pyasd-0.0.3/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-03 05:05:39.187106 pyasd-0.0.3/PKG-INFO
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1350 2023-05-03 04:42:39.000000 pyasd-0.0.3/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.139106 pyasd-0.0.3/asd/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      311 2023-05-03 05:05:38.000000 pyasd-0.0.3/asd/__init__.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.147106 pyasd-0.0.3/asd/core/
--rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      537 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/constants.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      902 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/dipolar_interactions.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    14970 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/geometry.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34800 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/gneb.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28461 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/hamiltonian.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13407 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/llg_advanced.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34609 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/llg_simple.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6394 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/log_general.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    35175 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/monte_carlo.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7330 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/random_vectors.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28028 2023-05-01 09:54:36.000000 pyasd-0.0.3/asd/core/shell_exchange.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    20217 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/spin_configurations.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13692 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/spin_correlations.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4455 2023-05-01 09:00:05.000000 pyasd-0.0.3/asd/core/topological_charge.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.155106 pyasd-0.0.3/asd/data_base/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.3/asd/data_base/exchange_for_Cr2I3X3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.3/asd/data_base/exchange_for_CrI3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_U2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_U4.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_rect.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.3/asd/data_base/exchange_for_Gd2C.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.3/asd/data_base/exchange_for_MnI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.3/asd/data_base/exchange_for_NiI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.3/asd/data_base/exchange_for_RuCl3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.3/asd/data_base/exchange_for_VOI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.3/asd/data_base/exchange_for_kagome.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.3/asd/data_base/exchange_for_skx.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.155106 pyasd-0.0.3/asd/mpi/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2556 2022-11-26 03:52:08.000000 pyasd-0.0.3/asd/mpi/mpi_tools.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.163106 pyasd-0.0.3/asd/utility/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12245 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/Swq.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8824 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/analyze_Spirit_results.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9225 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/asd_arguments.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    55462 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/auxiliary_colormaps.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     2143 2023-02-03 13:19:28.000000 pyasd-0.0.3/asd/utility/curve_fit.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5328 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/four_state_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1880 2023-04-17 02:00:31.000000 pyasd-0.0.3/asd/utility/head_figlet.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6688 2023-02-07 02:54:27.000000 pyasd-0.0.3/asd/utility/mag_thermal.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     7606 2023-02-08 03:42:14.000000 pyasd-0.0.3/asd/utility/ovf_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7753 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/plot_tools_3d.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13553 2023-05-01 09:39:25.000000 pyasd-0.0.3/asd/utility/post_llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5437 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/post_mc.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    19392 2023-04-07 12:17:17.000000 pyasd-0.0.3/asd/utility/spin_visualize_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2442 2023-02-03 13:19:13.000000 pyasd-0.0.3/asd/utility/spirit_tool.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.163106 pyasd-0.0.3/examples/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-01-11 07:09:44.000000 pyasd-0.0.3/examples/README
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.167106 pyasd-0.0.3/examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.3/examples/example1/.coverage
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.3/examples/example1/single_spin_LLG.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.167106 pyasd-0.0.3/examples/example2/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-01-11 07:10:07.000000 pyasd-0.0.3/examples/example2/README.md
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.3/examples/example2/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.167106 pyasd-0.0.3/examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      385 2023-01-11 07:09:55.000000 pyasd-0.0.3/examples/example3/README.md
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.3/examples/example3/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.167106 pyasd-0.0.3/examples/example4/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.3/examples/example4/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.3/examples/example4/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.135106 pyasd-0.0.3/misc/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.171106 pyasd-0.0.3/misc/archives/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.3/misc/archives/ovf-0.4.3.tar.gz
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.3/misc/archives/pyfiglet-0.7.tar.gz
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/pyasd.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-03 05:05:38.000000 pyasd-0.0.3/pyasd.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     4686 2023-05-03 05:05:39.000000 pyasd-0.0.3/pyasd.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-05-03 05:05:38.000000 pyasd-0.0.3/pyasd.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       43 2023-05-03 05:05:38.000000 pyasd-0.0.3/pyasd.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1083 2023-05-03 05:05:38.000000 pyasd-0.0.3/pyasd.egg-info/top_level.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-05-03 05:05:39.187106 pyasd-0.0.3/setup.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3339 2023-05-03 05:04:28.000000 pyasd-0.0.3/setup.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.135106 pyasd-0.0.3/tests_basic/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/B_eff/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.3/tests_basic/B_eff/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.3/tests_basic/B_eff/test_B_eff.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/OVF/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       64 2023-02-08 03:42:29.000000 pyasd-0.0.3/tests_basic/OVF/README
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3532 2023-02-08 03:43:05.000000 pyasd-0.0.3/tests_basic/OVF/pyasd_ovf_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2777 2023-02-08 03:42:25.000000 pyasd-0.0.3/tests_basic/OVF/test_ovf.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/mag_confs/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/mag_confs/Potts/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.3/tests_basic/mag_confs/Potts/Potts_test.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/mag_confs/domain_walls/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/domain_walls/dw_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/interpolate_images.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.175106 pyasd-0.0.3/tests_basic/mag_confs/meron/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/meron/bimeron.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/meron/meron.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.179106 pyasd-0.0.3/tests_basic/mag_confs/misc/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/interpolate_images.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/mpi_topo.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1067 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/regular_order_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/struct_factor.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      768 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/misc/test_pbc_shell.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.179106 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/Skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/a2sk.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/firework.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/mpi_firework.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/skyrmionium.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/mag_confs/spirals/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.3/tests_basic/mag_confs/spirals/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/spirals/spiral_test.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/mag_confs/test_regular_orders_honeycomb.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/mpi/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.3/tests_basic/mpi/test_group_rank.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.139106 pyasd-0.0.3/tests_basic/total_energy/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.139106 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5188 2023-05-01 09:01:00.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.183107 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/chiral_confs/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.3/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/large_test/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.3/tests_basic/total_energy/large_test/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/large_test/large_cell.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/local_energy/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/local_energy/CrMnI6_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/local_energy/test_local_en.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 05:05:39.187106 pyasd-0.0.3/tests_basic/total_energy/regular_orders/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7050 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1851 2023-01-05 07:16:05.000000 pyasd-0.0.3/tests_basic/total_energy/regular_orders/llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.3/tests_basic/total_energy/regular_orders/phase_diagram_tri.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.759330 pyasd-0.0.4/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1468 2023-01-05 06:57:53.000000 pyasd-0.0.4/LICENSE
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      488 2023-01-06 02:20:47.000000 pyasd-0.0.4/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-03 11:06:49.759330 pyasd-0.0.4/PKG-INFO
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1350 2023-04-26 14:54:49.000000 pyasd-0.0.4/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.711331 pyasd-0.0.4/asd/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      311 2023-05-03 11:06:49.000000 pyasd-0.0.4/asd/__init__.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.719330 pyasd-0.0.4/asd/core/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      537 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/constants.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      902 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/dipolar_interactions.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    14970 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/geometry.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34800 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/gneb.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28461 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/hamiltonian.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13407 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/llg_advanced.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34609 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/llg_simple.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6394 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/log_general.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    35175 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/monte_carlo.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7330 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/random_vectors.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28028 2023-05-01 09:54:36.000000 pyasd-0.0.4/asd/core/shell_exchange.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    20217 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/spin_configurations.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13692 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/spin_correlations.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4455 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/topological_charge.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.719330 pyasd-0.0.4/asd/data_base/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.4/asd/data_base/exchange_for_Cr2I3X3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.4/asd/data_base/exchange_for_CrI3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_U2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_U4.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_rect.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.4/asd/data_base/exchange_for_Gd2C.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.4/asd/data_base/exchange_for_MnI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.4/asd/data_base/exchange_for_NiI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.4/asd/data_base/exchange_for_RuCl3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.4/asd/data_base/exchange_for_VOI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.4/asd/data_base/exchange_for_kagome.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.4/asd/data_base/exchange_for_skx.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.719330 pyasd-0.0.4/asd/mpi/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2556 2022-11-26 03:52:08.000000 pyasd-0.0.4/asd/mpi/mpi_tools.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.731330 pyasd-0.0.4/asd/utility/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12245 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/Swq.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8824 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/analyze_Spirit_results.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9225 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/asd_arguments.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    55462 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/auxiliary_colormaps.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     2143 2023-02-03 13:19:28.000000 pyasd-0.0.4/asd/utility/curve_fit.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5328 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/four_state_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1880 2023-04-17 02:00:31.000000 pyasd-0.0.4/asd/utility/head_figlet.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6688 2023-02-07 02:54:27.000000 pyasd-0.0.4/asd/utility/mag_thermal.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     7606 2023-02-08 03:42:14.000000 pyasd-0.0.4/asd/utility/ovf_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7753 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/plot_tools_3d.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13553 2023-05-01 09:39:25.000000 pyasd-0.0.4/asd/utility/post_llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5437 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/post_mc.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    19392 2023-04-07 12:17:17.000000 pyasd-0.0.4/asd/utility/spin_visualize_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2442 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/spirit_tool.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.731330 pyasd-0.0.4/examples/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-01-11 07:09:44.000000 pyasd-0.0.4/examples/README
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.731330 pyasd-0.0.4/examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.4/examples/example1/.coverage
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.4/examples/example1/single_spin_LLG.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.731330 pyasd-0.0.4/examples/example2/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-01-11 07:10:07.000000 pyasd-0.0.4/examples/example2/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.4/examples/example2/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.735330 pyasd-0.0.4/examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      385 2023-01-11 07:09:55.000000 pyasd-0.0.4/examples/example3/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.4/examples/example3/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.735330 pyasd-0.0.4/examples/example4/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.4/examples/example4/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.4/examples/example4/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.707330 pyasd-0.0.4/misc/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.735330 pyasd-0.0.4/misc/archives/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.4/misc/archives/ovf-0.4.3.tar.gz
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.4/misc/archives/pyfiglet-0.7.tar.gz
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.739330 pyasd-0.0.4/pyasd.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     4686 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       43 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1083 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/top_level.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-05-03 11:06:49.759330 pyasd-0.0.4/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3339 2023-05-03 11:06:42.000000 pyasd-0.0.4/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.707330 pyasd-0.0.4/tests_basic/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/B_eff/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.4/tests_basic/B_eff/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.4/tests_basic/B_eff/test_B_eff.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/OVF/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       64 2023-02-08 03:42:29.000000 pyasd-0.0.4/tests_basic/OVF/README
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3532 2023-02-08 03:43:05.000000 pyasd-0.0.4/tests_basic/OVF/pyasd_ovf_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2777 2023-02-08 03:42:25.000000 pyasd-0.0.4/tests_basic/OVF/test_ovf.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/mag_confs/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/mag_confs/Potts/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.4/tests_basic/mag_confs/Potts/Potts_test.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/mag_confs/domain_walls/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/domain_walls/dw_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/interpolate_images.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.747330 pyasd-0.0.4/tests_basic/mag_confs/meron/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/meron/bimeron.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/meron/meron.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.747330 pyasd-0.0.4/tests_basic/mag_confs/misc/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/interpolate_images.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/mpi_topo.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1067 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/regular_order_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/struct_factor.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      768 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/test_pbc_shell.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.751330 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/Skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/a2sk.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/firework.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/mpi_firework.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/skyrmionium.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.751330 pyasd-0.0.4/tests_basic/mag_confs/spirals/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.4/tests_basic/mag_confs/spirals/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/spirals/spiral_test.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/test_regular_orders_honeycomb.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.751330 pyasd-0.0.4/tests_basic/mpi/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.4/tests_basic/mpi/test_group_rank.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.711331 pyasd-0.0.4/tests_basic/total_energy/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.707330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.751330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5188 2023-05-01 09:01:00.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/chiral_confs/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.4/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/large_test/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.4/tests_basic/total_energy/large_test/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/large_test/large_cell.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.759330 pyasd-0.0.4/tests_basic/total_energy/local_energy/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/local_energy/CrMnI6_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/local_energy/test_local_en.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.759330 pyasd-0.0.4/tests_basic/total_energy/regular_orders/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7050 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1851 2023-01-05 07:16:05.000000 pyasd-0.0.4/tests_basic/total_energy/regular_orders/llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/regular_orders/phase_diagram_tri.py
```

### Comparing `pyasd-0.0.3/LICENSE` & `pyasd-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/README.md` & `pyasd-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/constants.py` & `pyasd-0.0.4/asd/core/constants.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/dipolar_interactions.py` & `pyasd-0.0.4/asd/core/dipolar_interactions.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/geometry.py` & `pyasd-0.0.4/asd/core/geometry.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/gneb.py` & `pyasd-0.0.4/asd/core/gneb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/hamiltonian.py` & `pyasd-0.0.4/asd/core/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/llg_advanced.py` & `pyasd-0.0.4/asd/core/llg_advanced.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/llg_simple.py` & `pyasd-0.0.4/asd/core/llg_simple.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/log_general.py` & `pyasd-0.0.4/asd/core/log_general.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/monte_carlo.py` & `pyasd-0.0.4/asd/core/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/random_vectors.py` & `pyasd-0.0.4/asd/core/random_vectors.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/shell_exchange.py` & `pyasd-0.0.4/asd/core/shell_exchange.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/spin_configurations.py` & `pyasd-0.0.4/asd/core/spin_configurations.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/spin_correlations.py` & `pyasd-0.0.4/asd/core/spin_correlations.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/core/topological_charge.py` & `pyasd-0.0.4/asd/core/topological_charge.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_Cr2I3X3.py` & `pyasd-0.0.4/asd/data_base/exchange_for_Cr2I3X3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_CrI3.py` & `pyasd-0.0.4/asd/data_base/exchange_for_CrI3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_U2.py` & `pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_U2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_U4.py` & `pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_U4.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_CrMnI6_rect.py` & `pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_rect.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_Gd2C.py` & `pyasd-0.0.4/asd/data_base/exchange_for_Gd2C.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_MnI2.py` & `pyasd-0.0.4/asd/data_base/exchange_for_MnI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_NiI2.py` & `pyasd-0.0.4/asd/data_base/exchange_for_NiI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_RuCl3.py` & `pyasd-0.0.4/asd/data_base/exchange_for_RuCl3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_VOI2.py` & `pyasd-0.0.4/asd/data_base/exchange_for_VOI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_kagome.py` & `pyasd-0.0.4/asd/data_base/exchange_for_kagome.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/data_base/exchange_for_skx.py` & `pyasd-0.0.4/asd/data_base/exchange_for_skx.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/mpi/mpi_tools.py` & `pyasd-0.0.4/asd/mpi/mpi_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/Swq.py` & `pyasd-0.0.4/asd/utility/Swq.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/analyze_Spirit_results.py` & `pyasd-0.0.4/asd/utility/analyze_Spirit_results.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/asd_arguments.py` & `pyasd-0.0.4/asd/utility/asd_arguments.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/auxiliary_colormaps.py` & `pyasd-0.0.4/asd/utility/auxiliary_colormaps.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/curve_fit.py` & `pyasd-0.0.4/asd/utility/curve_fit.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/four_state_tools.py` & `pyasd-0.0.4/asd/utility/four_state_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/head_figlet.py` & `pyasd-0.0.4/asd/utility/head_figlet.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/mag_thermal.py` & `pyasd-0.0.4/asd/utility/mag_thermal.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/ovf_tools.py` & `pyasd-0.0.4/asd/utility/ovf_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/plot_tools_3d.py` & `pyasd-0.0.4/asd/utility/plot_tools_3d.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/post_llg.py` & `pyasd-0.0.4/asd/utility/post_llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/post_mc.py` & `pyasd-0.0.4/asd/utility/post_mc.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/spin_visualize_tools.py` & `pyasd-0.0.4/asd/utility/spin_visualize_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/asd/utility/spirit_tool.py` & `pyasd-0.0.4/asd/utility/spirit_tool.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/examples/example1/.coverage` & `pyasd-0.0.4/examples/example1/.coverage`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/examples/example1/single_spin_LLG.py` & `pyasd-0.0.4/examples/example1/single_spin_LLG.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/examples/example2/llg.py` & `pyasd-0.0.4/examples/example2/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/examples/example3/llg.py` & `pyasd-0.0.4/examples/example3/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/examples/example4/llg.py` & `pyasd-0.0.4/examples/example4/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/misc/archives/ovf-0.4.3.tar.gz` & `pyasd-0.0.4/misc/archives/ovf-0.4.3.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/misc/archives/pyfiglet-0.7.tar.gz` & `pyasd-0.0.4/misc/archives/pyfiglet-0.7.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/pyasd.egg-info/SOURCES.txt` & `pyasd-0.0.4/pyasd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/pyasd.egg-info/top_level.txt` & `pyasd-0.0.4/pyasd.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/setup.py` & `pyasd-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 core_modules  = ['asd/core/{}'.format(item) for item in core_modules]
 utility_modules  = ['asd/utility/{}'.format(item) for item in utility_modules]
 mpi_modules = ['asd/mpi/mpi_tools']
 
 
 kwargs_setup = dict(
 name='pyasd',
-version='0.0.3',
+version='0.0.4',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords='spin dynamics simulation',
 py_modules = utility_modules + core_modules + database_modules + mpi_modules + init_files,
 packages = setuptools.find_packages(),
```

### Comparing `pyasd-0.0.3/tests_basic/B_eff/test_B_eff.py` & `pyasd-0.0.4/tests_basic/B_eff/test_B_eff.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/OVF/pyasd_ovf_test.py` & `pyasd-0.0.4/tests_basic/OVF/pyasd_ovf_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/OVF/test_ovf.py` & `pyasd-0.0.4/tests_basic/OVF/test_ovf.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/Potts/Potts_test.py` & `pyasd-0.0.4/tests_basic/mag_confs/Potts/Potts_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/domain_walls/analytical_single_domain.py` & `pyasd-0.0.4/tests_basic/mag_confs/domain_walls/analytical_single_domain.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/domain_walls/dw_test.py` & `pyasd-0.0.4/tests_basic/mag_confs/domain_walls/dw_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/interpolate_images.py` & `pyasd-0.0.4/tests_basic/mag_confs/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py` & `pyasd-0.0.4/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/meron/bimeron.py` & `pyasd-0.0.4/tests_basic/mag_confs/meron/bimeron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py` & `pyasd-0.0.4/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/meron/meron.py` & `pyasd-0.0.4/tests_basic/mag_confs/meron/meron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/misc/interpolate_images.py` & `pyasd-0.0.4/tests_basic/mag_confs/misc/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/misc/mpi_topo.py` & `pyasd-0.0.4/tests_basic/mag_confs/misc/mpi_topo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/misc/regular_order_test.py` & `pyasd-0.0.4/tests_basic/mag_confs/misc/regular_order_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/misc/struct_factor.py` & `pyasd-0.0.4/tests_basic/mag_confs/misc/struct_factor.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/misc/test_pbc_shell.py` & `pyasd-0.0.4/tests_basic/mag_confs/misc/test_pbc_shell.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/Skyrmion.py` & `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/Skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py` & `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/a2sk.py` & `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/a2sk.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/afm_skyrmion.py` & `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/afm_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/firework.py` & `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py` & `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/mpi_firework.py` & `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/mpi_firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/skyrmionium.py` & `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/skyrmionium.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/skyrmion/view_3d_skyr.py` & `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/view_3d_skyr.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/spirals/CrMnI6_spiral.py` & `pyasd-0.0.4/tests_basic/mag_confs/spirals/CrMnI6_spiral.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/spirals/spiral_test.py` & `pyasd-0.0.4/tests_basic/mag_confs/spirals/spiral_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/mag_confs/test_regular_orders_honeycomb.py` & `pyasd-0.0.4/tests_basic/mag_confs/test_regular_orders_honeycomb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py` & `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py` & `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py` & `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py` & `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py` & `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/input.cfg` & `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/input.cfg`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py` & `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py` & `pyasd-0.0.4/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/large_test/large_cell.py` & `pyasd-0.0.4/tests_basic/total_energy/large_test/large_cell.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py` & `pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py` & `pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/local_energy/test_local_en.py` & `pyasd-0.0.4/tests_basic/total_energy/local_energy/test_local_en.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py` & `pyasd-0.0.4/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/regular_orders/llg.py` & `pyasd-0.0.4/tests_basic/total_energy/regular_orders/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.3/tests_basic/total_energy/regular_orders/phase_diagram_tri.py` & `pyasd-0.0.4/tests_basic/total_energy/regular_orders/phase_diagram_tri.py`

 * *Files identical despite different names*

