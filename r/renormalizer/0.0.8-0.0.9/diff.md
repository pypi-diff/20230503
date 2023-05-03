# Comparing `tmp/renormalizer-0.0.8.tar.gz` & `tmp/renormalizer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renormalizer-0.0.8.tar", last modified: Tue Feb 21 02:15:13 2023, max compression
+gzip compressed data, was "renormalizer-0.0.9.tar", last modified: Wed May  3 07:44:48 2023, max compression
```

## Comparing `renormalizer-0.0.8.tar` & `renormalizer-0.0.9.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.064945 renormalizer-0.0.8/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    10751 2022-09-01 02:59:16.000000 renormalizer-0.0.8/LICENSE
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1097 2023-02-21 02:15:13.064945 renormalizer-0.0.8/PKG-INFO
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      884 2022-10-14 02:00:06.000000 renormalizer-0.0.8/README.md
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.899813 renormalizer-0.0.8/renormalizer/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1251 2022-10-17 02:26:05.000000 renormalizer-0.0.8/renormalizer/__init__.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.912397 renormalizer-0.0.8/renormalizer/cv/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       74 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/cv/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    29813 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/cv/finitet.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     6437 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/cv/spectra_cv.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.918070 renormalizer-0.0.8/renormalizer/cv/tests/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       89 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/cv/tests/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2108 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/cv/tests/test_H_chain.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1874 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/cv/tests/test_abs.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1897 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/cv/tests/test_emi.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    17735 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/cv/zerot.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.919597 renormalizer-0.0.8/renormalizer/lib/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      381 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/__init__.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.922166 renormalizer-0.0.8/renormalizer/lib/bipartite_matching/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/bipartite_matching/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     4625 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/bipartite_matching/bipartite_matching.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.924853 renormalizer-0.0.8/renormalizer/lib/davidson/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/davidson/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    11429 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/davidson/davidson.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.928431 renormalizer-0.0.8/renormalizer/lib/integrate/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/integrate/__init__.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.936729 renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      178 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     9550 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/base.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    14730 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/common.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    21028 2022-10-09 10:52:17.000000 renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/ivp.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    15676 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/rk.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      355 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/integrate/integrate.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.939234 renormalizer-0.0.8/renormalizer/lib/krylov/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/krylov/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2725 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/lib/krylov/krylov.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.950590 renormalizer-0.0.8/renormalizer/model/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      301 2022-10-09 10:52:17.000000 renormalizer-0.0.8/renormalizer/model/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    33500 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/model/basis.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5942 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/model/h_qc.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    19524 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/model/model.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1571 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/model/mol.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    19129 2023-02-20 06:55:49.000000 renormalizer-0.0.8/renormalizer/model/op.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5042 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/model/phonon.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.971783 renormalizer-0.0.8/renormalizer/mps/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      325 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/mps/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3537 2022-09-30 03:06:18.000000 renormalizer-0.0.8/renormalizer/mps/backend.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    16235 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/gs.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3321 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/mps/hop_expr.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    15475 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/lib.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     9165 2022-09-30 03:06:18.000000 renormalizer-0.0.8/renormalizer/mps/matrix.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    40707 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/mp.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5000 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/mpdm.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    17606 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/mpo.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    74262 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/mps.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    10563 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/svd_qn.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    26331 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/symbolic_mpo.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    20043 2022-09-02 04:48:19.000000 renormalizer-0.0.8/renormalizer/mps/tda.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.989769 renormalizer-0.0.8/renormalizer/mps/tests/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      136 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/mps/tests/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1671 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_elementop.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     7319 2022-09-30 03:06:18.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_evolve.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     4774 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_gs.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5003 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_mp.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1942 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_mpdm.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     6499 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_mpo.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1141 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_mpproperty.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3446 2023-01-30 08:30:31.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_mps.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3608 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_sbm.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     4117 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/mps/tests/test_tda.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     6898 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/mps/thermalprop.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.994582 renormalizer-0.0.8/renormalizer/property/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       52 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/property/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3072 2022-10-09 10:52:17.000000 renormalizer-0.0.8/renormalizer/property/ops.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2990 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/property/property.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.998694 renormalizer-0.0.8/renormalizer/sbm/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      147 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/sbm/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5509 2022-10-09 10:52:17.000000 renormalizer-0.0.8/renormalizer/sbm/lib.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3197 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/sbm/sbm.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.006760 renormalizer-0.0.8/renormalizer/spectra/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      266 2022-10-09 10:52:17.000000 renormalizer-0.0.8/renormalizer/spectra/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1069 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/spectra/base.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3604 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/spectra/exact.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5390 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/spectra/finitet.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.009848 renormalizer-0.0.8/renormalizer/spectra/tests/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      136 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/spectra/tests/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3430 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/spectra/tests/test_spectra.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2625 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/spectra/zerot.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.016416 renormalizer-0.0.8/renormalizer/tests/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/tests/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)   143172 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/tests/c2h4_para.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1649 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/tests/parameter.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1330 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/tests/parameter_PBI.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      711 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/tests/parameter_exact.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.022266 renormalizer-0.0.8/renormalizer/transport/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      224 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/transport/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    12812 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/transport/dynamics.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    17760 2022-10-05 09:21:02.000000 renormalizer-0.0.8/renormalizer/transport/kubo.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5621 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/transport/spectral_function.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.030431 renormalizer-0.0.8/renormalizer/transport/tests/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       89 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/transport/tests/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1077 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/transport/tests/band_param.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5304 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/transport/tests/test_dynamics.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5748 2022-09-30 03:06:18.000000 renormalizer-0.0.8/renormalizer/transport/tests/test_kubo.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2753 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/transport/tests/test_spectral_function.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.044944 renormalizer-0.0.8/renormalizer/utils/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      457 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    16361 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/configs.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1566 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/constant.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3927 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/elementop.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1285 2022-10-05 09:21:02.000000 renormalizer-0.0.8/renormalizer/utils/log.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2773 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/quantity.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3621 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/qutip_utils.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     7473 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/rk.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     8190 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/tdmps.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.049505 renormalizer-0.0.8/renormalizer/utils/tests/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       24 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/tests/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      265 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/tests/test_quantity.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      630 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/tests/test_rk.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1226 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/utils/utils.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.052504 renormalizer-0.0.8/renormalizer/vibration/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       70 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/vibration/__init__.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.056277 renormalizer-0.0.8/renormalizer/vibration/tests/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       89 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/vibration/tests/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2641 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/vibration/tests/test_vscf.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3824 2023-02-20 01:57:37.000000 renormalizer-0.0.8/renormalizer/vibration/vscf.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.058813 renormalizer-0.0.8/renormalizer/vibronic/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       90 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/vibronic/__init__.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:13.063402 renormalizer-0.0.8/renormalizer/vibronic/tests/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       65 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/vibronic/tests/__init__.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    13110 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/vibronic/tests/mctdh_data.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     6056 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/vibronic/tests/test_pyr4.py
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     4124 2022-09-01 02:59:16.000000 renormalizer-0.0.8/renormalizer/vibronic/vibronic.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-02-21 02:15:12.906973 renormalizer-0.0.8/renormalizer.egg-info/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1097 2023-02-21 02:15:12.000000 renormalizer-0.0.8/renormalizer.egg-info/PKG-INFO
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3711 2023-02-21 02:15:12.000000 renormalizer-0.0.8/renormalizer.egg-info/SOURCES.txt
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        1 2023-02-21 02:15:12.000000 renormalizer-0.0.8/renormalizer.egg-info/dependency_links.txt
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       28 2023-02-21 02:15:12.000000 renormalizer-0.0.8/renormalizer.egg-info/requires.txt
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       13 2023-02-21 02:15:12.000000 renormalizer-0.0.8/renormalizer.egg-info/top_level.txt
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       38 2023-02-21 02:15:13.065456 renormalizer-0.0.8/setup.cfg
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      600 2023-02-21 02:12:47.000000 renormalizer-0.0.8/setup.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.735087 renormalizer-0.0.9/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    10751 2022-09-01 02:59:16.000000 renormalizer-0.0.9/LICENSE
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1097 2023-05-03 07:44:48.734544 renormalizer-0.0.9/PKG-INFO
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      884 2022-10-14 02:00:06.000000 renormalizer-0.0.9/README.md
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.575250 renormalizer-0.0.9/renormalizer/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1314 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/__init__.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.588150 renormalizer-0.0.9/renormalizer/cv/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       74 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/cv/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    30529 2023-03-25 09:17:20.000000 renormalizer-0.0.9/renormalizer/cv/finitet.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     6437 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/cv/spectra_cv.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.594134 renormalizer-0.0.9/renormalizer/cv/tests/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       89 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/cv/tests/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2108 2023-02-20 01:57:37.000000 renormalizer-0.0.9/renormalizer/cv/tests/test_H_chain.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1874 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/cv/tests/test_abs.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1897 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/cv/tests/test_emi.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    17735 2023-02-20 01:57:37.000000 renormalizer-0.0.9/renormalizer/cv/zerot.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.595131 renormalizer-0.0.9/renormalizer/lib/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      381 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/__init__.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.599121 renormalizer-0.0.9/renormalizer/lib/bipartite_matching/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/bipartite_matching/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     4625 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/bipartite_matching/bipartite_matching.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.602113 renormalizer-0.0.9/renormalizer/lib/davidson/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/davidson/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    11789 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/lib/davidson/davidson.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.604108 renormalizer-0.0.9/renormalizer/lib/integrate/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/integrate/__init__.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.611089 renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      178 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     9550 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/base.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    14730 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/common.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    21028 2022-10-09 10:52:17.000000 renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/ivp.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    15676 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/rk.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      355 2023-03-25 12:30:14.000000 renormalizer-0.0.9/renormalizer/lib/integrate/integrate.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.616094 renormalizer-0.0.9/renormalizer/lib/krylov/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/krylov/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2725 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/lib/krylov/krylov.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.626049 renormalizer-0.0.9/renormalizer/model/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      301 2022-10-09 10:52:17.000000 renormalizer-0.0.9/renormalizer/model/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    33606 2023-05-03 07:34:00.000000 renormalizer-0.0.9/renormalizer/model/basis.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5942 2023-02-20 01:57:37.000000 renormalizer-0.0.9/renormalizer/model/h_qc.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    20041 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/model/model.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1571 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/model/mol.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    19129 2023-03-13 07:43:07.000000 renormalizer-0.0.9/renormalizer/model/op.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5042 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/model/phonon.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.646647 renormalizer-0.0.9/renormalizer/mps/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      325 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/mps/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3537 2022-09-30 03:06:18.000000 renormalizer-0.0.9/renormalizer/mps/backend.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    16235 2023-02-20 01:57:37.000000 renormalizer-0.0.9/renormalizer/mps/gs.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3321 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/mps/hop_expr.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    15927 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/mps/lib.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     9481 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/mps/matrix.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    41825 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/mps/mp.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5162 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/mps/mpdm.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    18091 2023-03-25 09:17:31.000000 renormalizer-0.0.9/renormalizer/mps/mpo.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    76200 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/mps/mps.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    10879 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/mps/svd_qn.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    26978 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/mps/symbolic_mpo.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    20043 2022-09-02 04:48:19.000000 renormalizer-0.0.9/renormalizer/mps/tda.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.663161 renormalizer-0.0.9/renormalizer/mps/tests/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      136 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/mps/tests/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1671 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_elementop.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     7319 2023-03-29 05:53:42.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_evolve.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     4774 2023-02-20 01:57:37.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_gs.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5162 2023-04-07 09:02:54.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_mp.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1942 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_mpdm.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     6499 2023-02-20 01:57:37.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_mpo.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1141 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_mpproperty.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3446 2023-01-30 08:30:31.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_mps.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3710 2023-04-07 09:02:59.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_sbm.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     4117 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/mps/tests/test_tda.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     7066 2023-04-07 09:03:06.000000 renormalizer-0.0.9/renormalizer/mps/thermalprop.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.667148 renormalizer-0.0.9/renormalizer/property/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       52 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/property/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3072 2022-10-09 10:52:17.000000 renormalizer-0.0.9/renormalizer/property/ops.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2990 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/property/property.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.671138 renormalizer-0.0.9/renormalizer/sbm/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      147 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/sbm/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5509 2022-10-09 10:52:17.000000 renormalizer-0.0.9/renormalizer/sbm/lib.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3290 2023-04-07 09:03:43.000000 renormalizer-0.0.9/renormalizer/sbm/sbm.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.678119 renormalizer-0.0.9/renormalizer/spectra/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      266 2022-10-09 10:52:17.000000 renormalizer-0.0.9/renormalizer/spectra/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1069 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/spectra/base.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3604 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/spectra/exact.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5540 2023-04-07 09:03:53.000000 renormalizer-0.0.9/renormalizer/spectra/finitet.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.681111 renormalizer-0.0.9/renormalizer/spectra/tests/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      136 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/spectra/tests/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3430 2023-02-20 01:57:37.000000 renormalizer-0.0.9/renormalizer/spectra/tests/test_spectra.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2704 2023-04-07 09:03:53.000000 renormalizer-0.0.9/renormalizer/spectra/zerot.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.688092 renormalizer-0.0.9/renormalizer/tests/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/tests/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)   143172 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/tests/c2h4_para.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1649 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/tests/parameter.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1330 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/tests/parameter_PBI.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      711 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/tests/parameter_exact.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.693654 renormalizer-0.0.9/renormalizer/transport/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      224 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/transport/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    13107 2023-04-07 09:04:03.000000 renormalizer-0.0.9/renormalizer/transport/dynamics.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    18125 2023-04-07 09:04:03.000000 renormalizer-0.0.9/renormalizer/transport/kubo.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5758 2023-04-07 09:04:03.000000 renormalizer-0.0.9/renormalizer/transport/spectral_function.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.700652 renormalizer-0.0.9/renormalizer/transport/tests/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       89 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/transport/tests/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1077 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/transport/tests/band_param.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5304 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/transport/tests/test_dynamics.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     5748 2022-09-30 03:06:18.000000 renormalizer-0.0.9/renormalizer/transport/tests/test_kubo.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2753 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/transport/tests/test_spectral_function.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.715595 renormalizer-0.0.9/renormalizer/utils/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      457 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    16793 2023-05-03 07:33:08.000000 renormalizer-0.0.9/renormalizer/utils/configs.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1566 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/constant.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3927 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/elementop.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1285 2022-10-05 09:21:02.000000 renormalizer-0.0.9/renormalizer/utils/log.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2773 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/quantity.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3621 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/qutip_utils.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     7473 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/rk.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     8190 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/tdmps.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.719584 renormalizer-0.0.9/renormalizer/utils/tests/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       24 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/tests/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      265 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/tests/test_quantity.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      630 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/tests/test_rk.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1226 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/utils/utils.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.722589 renormalizer-0.0.9/renormalizer/vibration/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       70 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/vibration/__init__.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.725568 renormalizer-0.0.9/renormalizer/vibration/tests/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       89 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/vibration/tests/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     2641 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/vibration/tests/test_vscf.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3824 2023-02-20 01:57:37.000000 renormalizer-0.0.9/renormalizer/vibration/vscf.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.728560 renormalizer-0.0.9/renormalizer/vibronic/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       90 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/vibronic/__init__.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.732550 renormalizer-0.0.9/renormalizer/vibronic/tests/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       65 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/vibronic/tests/__init__.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)    13110 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/vibronic/tests/mctdh_data.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     6056 2022-09-01 02:59:16.000000 renormalizer-0.0.9/renormalizer/vibronic/tests/test_pyr4.py
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     4244 2023-04-07 09:04:03.000000 renormalizer-0.0.9/renormalizer/vibronic/vibronic.py
+drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-05-03 07:44:48.583164 renormalizer-0.0.9/renormalizer.egg-info/
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     1097 2023-05-03 07:44:48.000000 renormalizer-0.0.9/renormalizer.egg-info/PKG-INFO
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)     3711 2023-05-03 07:44:48.000000 renormalizer-0.0.9/renormalizer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        1 2023-05-03 07:44:48.000000 renormalizer-0.0.9/renormalizer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       28 2023-05-03 07:44:48.000000 renormalizer-0.0.9/renormalizer.egg-info/requires.txt
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       13 2023-05-03 07:44:48.000000 renormalizer-0.0.9/renormalizer.egg-info/top_level.txt
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       38 2023-05-03 07:44:48.735087 renormalizer-0.0.9/setup.cfg
+-rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      627 2023-05-03 07:44:11.000000 renormalizer-0.0.9/setup.py
```

### Comparing `renormalizer-0.0.8/LICENSE` & `renormalizer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/PKG-INFO` & `renormalizer-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renormalizer
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/shuaigroup/Renormalizer
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![logo](./doc/source/logo.png)
```

### Comparing `renormalizer-0.0.8/README.md` & `renormalizer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/__init__.py` & `renormalizer-0.0.9/renormalizer/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-# -*- coding: utf-8 -*-
-# Author: Jiajun Ren <jiajunren0522@gmail.com>
-import logging
-import os
-import sys
-import warnings
-
-
-reno_num_threads = os.environ.get("RENO_NUM_THREADS")
-if reno_num_threads is not None:
-    # Set environment variables to limit NumPy CPU usage
-    # Note that this should be done before NumPy is imported
-
-    if "numpy" in sys.modules:
-        warnings.warn("renormalizer should be imported before numpy for `RENO_NUM_THREADS` to take effect")
-    else:
-        for env in ["MKL_NUM_THREADS", "NUMEXPR_NUM_THREADS", "OMP_NUM_THREADS"]:
-            os.environ[env] = reno_num_threads
-            del env
-
-del sys, warnings
-
-from renormalizer.utils.log import init_log
-
-
-# logging.DEBUG == 10, logging.INFO == 20. See the logging built-in package for more
-log_level = int(os.environ.get("RENO_LOG_LEVEL", logging.DEBUG))
-
-init_log(log_level)
-
-del os, log_level, init_log
-
-
-# user interfaces
-from renormalizer.model import Model, HolsteinModel, SpinBosonModel, TI1DModel, Op
-from renormalizer.model.basis import BasisSHO, BasisHopsBoson, BasisSineDVR, BasisMultiElectron, \
-    BasisMultiElectronVac, BasisSimpleElectron, BasisHalfSpin
-from renormalizer.mps import Mpo, Mps, optimize_mps
-from renormalizer.utils import Quantity
+# -*- coding: utf-8 -*-
+# Author: Jiajun Ren <jiajunren0522@gmail.com>
+import logging
+import os
+import sys
+import warnings
+
+
+reno_num_threads = os.environ.get("RENO_NUM_THREADS")
+reno_num_threads = "1"
+if reno_num_threads is not None:
+    # Set environment variables to limit NumPy CPU usage
+    # Note that this should be done before NumPy is imported
+
+    if "numpy" in sys.modules:
+        warnings.warn("renormalizer should be imported before numpy for `RENO_NUM_THREADS` to take effect")
+    else:
+        for env in ["MKL_NUM_THREADS", "NUMEXPR_NUM_THREADS", "OMP_NUM_THREADS"]:
+            os.environ[env] = reno_num_threads
+            del env
+
+del sys, warnings
+
+from renormalizer.utils.log import init_log
+
+
+# logging.DEBUG == 10, logging.INFO == 20. See the logging built-in package for more
+log_level = int(os.environ.get("RENO_LOG_LEVEL", logging.DEBUG))
+
+init_log(log_level)
+
+del os, log_level, init_log
+
+
+# user interfaces
+from renormalizer.model import Model, HolsteinModel, SpinBosonModel, TI1DModel, Op
+from renormalizer.model.basis import BasisSHO, BasisHopsBoson, BasisSineDVR, BasisMultiElectron, \
+    BasisMultiElectronVac, BasisSimpleElectron, BasisHalfSpin
+from renormalizer.mps import Mpo, Mps, optimize_mps
+from renormalizer.utils import Quantity
```

### Comparing `renormalizer-0.0.8/renormalizer/cv/finitet.py` & `renormalizer-0.0.9/renormalizer/cv/finitet.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,716 +1,716 @@
-# -*- coding: utf-8 -*-
-# Author: Tong Jiang <tongjiang1000@gmail.com>
-# finite temperature absorption/emission spectrum based on Correction vector
-
-import copy
-import os
-import logging
-import scipy
-from itertools import product
-
-from renormalizer.mps.matrix import (
-    multi_tensor_contract,
-    tensordot,
-    moveaxis
-)
-from renormalizer.cv.spectra_cv import SpectraCv
-from renormalizer.mps.backend import np, xp
-from renormalizer.mps.matrix import asxp, asnumpy
-from renormalizer.mps import (
-    Mpo, svd_qn, MpDm, ThermalProp, load_thermal_state)
-from renormalizer.mps.lib import update_cv
-from renormalizer.utils import (
-    CompressConfig, EvolveConfig,
-    CompressCriteria
-)
-
-logger = logging.getLogger(__name__)
-
-
-class SpectraFtCV(SpectraCv):
-    r"""
-    Use DDMRG to calculate the finite temperature spectrum from frequency domain
-
-    Args:
-        model (:class:`~renormalizer.model.Model`): system information.
-        spectratype (string): "abs" or "emi".
-        m_max (int): maximal bond dimension of correction vector.
-        eta (float): Lorentzian broadening width (a.u.).
-        temperature (:class:`~renormalizer.utils.Quantity`): simulation temperature.
-        h_mpo (:class:`~renormalizer.mps.Mpo`): system Hamiltonian.
-        method (str): "1site" or "2site".
-        procedure_cv (list): percent used for each sweep.
-        rtol (float): the relative tolerance of the spectrum strength, default: 1e-5.
-        b_mps (:class:`~renormalizer.mps.Mps`): the b vector -eta * dipole * \psi_0, default: None.
-            (Holstein model could construct b_mps implicitly).
-        cv_mps (:class:`~renormalizer.mps.Mps`): initial guess of cv_mps, default: None.
-        icompress_config (:class:`~renormalizer.utils.CompressConfig`): config when compressing MPS/MPO during the imaginary time evolution..
-        ievolve_config (:class:`~renormalizer.utils.EvolveConfig`): evolution config for imaginary time evolution.
-        insteps (int): evolve steps for imaginary time evolution. have to be provided when calculating emission.
-        dump_dir (str): the directory for logging and numerical result output.
-            Also the directory from which to load previous thermal propagated initial state (if exists).
-        job_name (str): the name of the calculation job which determines the file name of the logging and numerical result output.
-
-    Example::
-        see test/test_abs.py for example
-
-    """
-    def __init__(
-        self,
-        model,
-        spectratype,
-        m_max,
-        eta,
-        temperature,
-        h_mpo=None,
-        method='1site',
-        procedure_cv=None,
-        rtol=1e-5,
-        b_mps=None,
-        cv_mps=None,
-        icompress_config=None,
-        ievolve_config=None,
-        insteps=None,
-        dump_dir: str=None,
-        job_name=None,
-    ):
-
-        self.temperature = temperature
-        self.evolve_config = ievolve_config
-        self.compress_config = icompress_config
-        if self.evolve_config is None:
-            self.evolve_config = \
-                EvolveConfig()
-        if self.compress_config is None:
-            self.compress_config = \
-                CompressConfig(CompressCriteria.fixed,
-                               max_bonddim=m_max)
-            self.compress_config.set_bonddim(len(model.pbond_list))
-        self.insteps = insteps
-        self.job_name = job_name
-        self.dump_dir = dump_dir
-
-        super().__init__(
-            model, spectratype, m_max, eta, h_mpo=h_mpo,
-            method=method, procedure_cv=procedure_cv,
-            rtol=rtol, b_mps=b_mps, cv_mps=cv_mps,
-        )
-
-        self.cv_mpo = self.cv_mps
-        self.b_mpo = self.b_mps
-
-        self.a_oper = None
-
-    def init_cv_mpo(self):
-        cv_mpo = Mpo.finiteT_cv(self.model, 1, self.m_max,
-                                self.spectratype, percent=1.0)
-        return cv_mpo
-
-    init_cv_mps = init_cv_mpo
-
-    def init_b_mpo(self):
-        # get the right hand site vector b, Ax=b
-        # b = -eta * dipole * \psi_0
-
-        # only support Holstien model 0/1 exciton manifold
-        beta = self.temperature.to_beta()
-        if self.spectratype == "abs":
-            dipole_mpo = Mpo.onsite(self.model, r"a^\dagger", dipole=True)
-            i_mpo = MpDm.max_entangled_gs(self.model)
-            tp = ThermalProp(i_mpo, exact=True, space='GS')
-            tp.evolve(None, 1, beta / 2j)
-            ket_mpo = tp.latest_mps
-        elif self.spectratype == "emi":
-            dipole_mpo = Mpo.onsite(self.model, "a", dipole=True)
-            if self._defined_output_path:
-                ket_mpo = \
-                    load_thermal_state(self.model, self._thermal_dump_path)
-            else:
-                ket_mpo = None
-            if ket_mpo is None:
-                impo = MpDm.max_entangled_ex(self.model)
-                impo.compress_config = self.compress_config
-                if self.job_name is None:
-                    job_name = None
-                else:
-                    job_name = self.job_name + "_thermal_prop"
-                tp = ThermalProp(
-                    impo, evolve_config=self.evolve_config,
-                    dump_dir=self.dump_dir, job_name=job_name)
-                tp.evolve(None, self.insteps, beta / 2j)
-                ket_mpo = tp.latest_mps
-                if self._defined_output_path:
-                    ket_mpo.dump(self._thermal_dump_path)
-        else:
-            assert False
-        ket_mpo = dipole_mpo.apply(ket_mpo.scale(-self.eta))
-
-        return ket_mpo, None
-
-    init_b_mps = init_b_mpo
-
-    @property
-    def _thermal_dump_path(self):
-        assert self._defined_output_path
-        return os.path.join(self.dump_dir, self.job_name + "_impo.npz")
-
-    @property
-    def _defined_output_path(self):
-        return self.dump_dir is not None and self.job_name is not None
-
-    def oper_prepare(self, omega):
-        identity = Mpo.identity(self.model).scale(omega)
-        self.a_oper = identity.add(self.h_mpo.scale(-1, inplace=False))
-
-    def optimize_cv(self, lr_group, isite, percent=0):
-        if self.spectratype == "abs":
-            # quantum number restriction, |1><0|
-            up_exciton, down_exciton = 1, 0
-        elif self.spectratype == "emi":
-            # quantum number restriction, |0><1|
-            up_exciton, down_exciton = 0, 1
-        nexciton = 1
-        first_LR, second_LR, third_LR, forth_LR = lr_group
-
-        if self.method == "1site":
-            add_list = [isite - 1]
-            first_L = asxp(first_LR[isite - 1])
-            first_R = asxp(first_LR[isite])
-            second_L = asxp(second_LR[isite - 1])
-            second_R = asxp(second_LR[isite])
-            third_L = asxp(third_LR[isite - 1])
-            third_R = asxp(third_LR[isite])
-            forth_L = asxp(forth_LR[isite - 1])
-            forth_R = asxp(forth_LR[isite])
-        else:
-            add_list = [isite - 2, isite - 1]
-            first_L = asxp(first_LR[isite - 2])
-            first_R = asxp(first_LR[isite])
-            second_L = asxp(second_LR[isite - 2])
-            second_R = asxp(second_LR[isite])
-            third_L = asxp(third_LR[isite - 2])
-            third_R = asxp(third_LR[isite])
-            forth_L = asxp(forth_LR[isite - 2])
-            forth_R = asxp(forth_LR[isite])
-
-        xqnmat, xqnbigl, xqnbigr, xshape = \
-            self.construct_X_qnmat(add_list)
-        dag_qnmat, dag_qnbigl, dag_qnbigr = self.swap(xqnmat, xqnbigl, xqnbigr)
-        nonzeros = int(np.sum(
-            self.condition(
-                dag_qnmat, [down_exciton, up_exciton])
-        ))
-
-        if self.method == "1site":
-            guess = moveaxis(self.cv_mpo[isite - 1], (1, 2), (2, 1))
-        else:
-            guess = tensordot(moveaxis(self.cv_mpo[isite - 2], (1, 2), (2, 1)),
-                              moveaxis(self.cv_mpo[isite - 1]), axes=(-1, 0))
-        guess = guess[
-            self.condition(
-                dag_qnmat, [down_exciton, up_exciton])]
-
-        if self.method == "1site":
-            # define dot path
-            path_1 = [([0, 1], "abcd, aefg -> bcdefg"),
-                      ([3, 0], "bcdefg, bfhi -> cdeghi"),
-                      ([2, 0], "cdeghi, chjk -> degijk"),
-                      ([1, 0], "degijk, gikl -> dejl")]
-            path_2 = [([0, 1], "abcd, aefg -> bcdefg"),
-                      ([3, 0], "bcdefg, bfhi -> cdeghi"),
-                      ([2, 0], "cdeghi, djek -> cghijk"),
-                      ([1, 0], "cghijk, gilk -> chjl")]
-            path_3 = [([0, 1], "ab, acde -> bcde"),
-                      ([1, 0], "bcde, ef -> bcdf")]
-
-            vecb = multi_tensor_contract(
-                path_3, forth_L,
-                moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
-                forth_R)[self.condition(dag_qnmat, [down_exciton, up_exciton])]
-
-        a_oper_isite = asxp(self.a_oper[isite - 1])
-        h_mpo_isite = asxp(self.h_mpo[isite - 1])
-        # construct preconditioner
-        Idt = xp.identity(h_mpo_isite.shape[1])
-        M1_1 = xp.einsum('abca->abc', first_L)
-        path_m1 = [([0, 1], "abc, bdef->acdef"),
-                   ([1, 0], "acdef, cegh->adfgh")]
-        M1_2 = multi_tensor_contract(path_m1, M1_1, a_oper_isite, a_oper_isite)
-        M1_2 = xp.einsum("abcbd->abcd", M1_2)
-        M1_3 = xp.einsum('ecde->ecd', first_R)
-        M1_4 = xp.einsum('ff->f', Idt)
-        path_m1 = [([0, 1], "abcd,ecd->abe"),
-                   ([1, 0], "abe,f->abef")]
-        pre_M1 = multi_tensor_contract(
-            path_m1, M1_2, M1_3, M1_4)
-        pre_M1 = xp.moveaxis(pre_M1, [-2, -1], [-1, -2])[
-            self.condition(dag_qnmat, [down_exciton, up_exciton])]
-
-        M2_1 = xp.einsum('aeag->aeg', second_L)
-        M2_2 = xp.einsum('eccf->ecf', a_oper_isite)
-        M2_3 = xp.einsum('gbbh->gbh', h_mpo_isite)
-        M2_4 = xp.einsum('dfdh->dfh', second_R)
-        path_m2 = [([0, 1], "aeg,gbh->aebh"),
-                   ([2, 0], "aebh,ecf->abchf"),
-                   ([1, 0], "abhcf,dfh->abcd")]
-        pre_M2 = multi_tensor_contract(
-            path_m2, M2_1, M2_3, M2_2, M2_4)
-        pre_M2 = pre_M2[
-            self.condition(dag_qnmat, [down_exciton, up_exciton])]
-
-        M4_1 = xp.einsum('faah->fah', third_L)
-        M4_4 = xp.einsum('gddi->gdi', third_R)
-        M4_5 = xp.einsum('cc->c', Idt)
-        M4_path = [([0, 1], "fah,febg->ahebg"),
-                   ([2, 0], "ahebg,hjei->abgji"),
-                   ([1, 0], "abgji,gdi->abjd")]
-        pre_M4 = multi_tensor_contract(
-            M4_path, M4_1, h_mpo_isite,
-            h_mpo_isite, M4_4)
-        pre_M4 = xp.einsum('abbd->abd', pre_M4)
-        pre_M4 = xp.tensordot(pre_M4, M4_5, axes=0)
-        pre_M4 = xp.moveaxis(pre_M4, [2, 3], [3, 2])[
-            self.condition(dag_qnmat, [down_exciton, up_exciton])]
-
-        M_x = lambda x: asnumpy(asxp(x) / (pre_M1 + 2 * pre_M2 + pre_M4 + xp.ones(nonzeros)*self.eta**2))
-        pre_M = scipy.sparse.linalg.LinearOperator((nonzeros, nonzeros), M_x)
-
-        count = 0
-
-        def hop(x):
-            nonlocal count
-            count += 1
-            dag_struct = asxp(self.dag2mat(
-                xshape, x, dag_qnmat))
-            if self.method == "1site":
-
-                M1 = multi_tensor_contract(
-                    path_1, first_L, dag_struct,
-                    a_oper_isite, a_oper_isite, first_R)
-                M2 = multi_tensor_contract(
-                    path_2, second_L, dag_struct,
-                    a_oper_isite,
-                    h_mpo_isite, second_R)
-                M2 = xp.moveaxis(M2, (1, 2), (2, 1))
-                M3 = multi_tensor_contract(
-                    path_2, third_L, h_mpo_isite, dag_struct,
-                    h_mpo_isite, third_R)
-                M3 = xp.moveaxis(M3, (1, 2), (2, 1))
-                cout = M1 + 2 * M2 + M3 + dag_struct * self.eta**2
-            cout = cout[
-                self.condition(dag_qnmat, [down_exciton, up_exciton])
-            ]
-            return asnumpy(cout)
-
-        # Matrix A
-        mat_a = scipy.sparse.linalg.LinearOperator((nonzeros, nonzeros), matvec=hop)
-
-        x, info = scipy.sparse.linalg.cg(
-            mat_a, asnumpy(vecb), tol=1.e-5, x0=asnumpy(guess), maxiter=500,
-            M=pre_M, atol=0)
-        # logger.info(f"linear eq dim: {nonzeros}")
-        # logger.info(f'times for hop:{count}')
-        self.hop_time.append(count)
-        if info != 0:
-            logger.warning(
-                f"cg not converged, vecb.norm:{xp.linalg.norm(vecb)}")
-        l_value = xp.dot(asxp(hop(x)), asxp(x)) - 2 * xp.dot(vecb, asxp(x))
-
-        x = self.dag2mat(xshape, x, dag_qnmat)
-        if self.method == "1site":
-            x = np.moveaxis(x, [1, 2], [2, 1])
-        x, xdim, xqn, compx = self.x_svd(
-            x, xqnbigl, xqnbigr, nexciton,
-            percent=percent)
-
-        if self.method == "1site":
-            self.cv_mpo[isite - 1] = x
-            if not self.cv_mpo.to_right:
-                if isite != 1:
-                    self.cv_mpo[isite - 2] = \
-                        tensordot(self.cv_mpo[isite - 2], compx, axes=(-1, 0))
-                    self.cv_mpo.qn[isite - 1] = xqn
-                    self.cv_mpo.qnidx = isite-2
-                else:
-                    self.cv_mpo[isite - 1] = \
-                        tensordot(compx, self.cv_mpo[isite - 1], axes=(-1, 0))
-                    self.cv_mpo.qnidx = 0
-            else:
-                if isite != len(self.cv_mpo):
-                    self.cv_mpo[isite] = \
-                        tensordot(compx, self.cv_mpo[isite], axes=(-1, 0))
-                    self.cv_mpo.qn[isite] = xqn
-                    self.cv_mpo.qnidx = isite
-                else:
-                    self.cv_mpo[isite - 1] = \
-                        tensordot(self.cv_mpo[isite - 1], compx, axes=(-1, 0))
-                    self.cv_mpo.qnidx = self.cv_mpo.site_num-1
-
-        else:
-            if not self.cv_mpo.to_right:
-                self.cv_mpo[isite - 2] = compx
-                self.cv_mpo[isite - 1] = x
-                self.cv_mpo.qnidx = isite-2
-            else:
-                self.cv_mpo[isite - 2] = x
-                self.cv_mpo[isite - 1] = compx
-                self.cv_mpo.qnidx = isite-1
-            self.cv_mpo.qn[isite - 1] = xqn
-
-        return float(l_value)
-
-    def construct_X_qnmat(self, addlist):
-
-        pbond = self.model.pbond_list
-        xqnl = np.array(self.cv_mpo.qn[addlist[0]])
-        xqnr = np.array(self.cv_mpo.qn[addlist[-1] + 1])
-        xqnmat = xqnl.copy()
-        xqnsigmalist = []
-        for idx in addlist:
-            sigmaqn = self.model.basis[idx].sigmaqn
-            xqnsigma = np.array(list(product(sigmaqn, repeat=2)))
-            xqnsigma = xqnsigma.reshape(pbond[idx], pbond[idx], 2)
-
-            xqnmat = self.qnmat_add(xqnmat, xqnsigma)
-            xqnsigmalist.append(xqnsigma)
-
-        xqnmat = self.qnmat_add(xqnmat, xqnr)
-        matshape = list(xqnmat.shape)
-        if self.method == "1site":
-            if xqnmat.ndim == 4:
-                if not self.cv_mpo.to_right:
-                    xqnmat = np.moveaxis(xqnmat.reshape(matshape+[1]), -1, -2)
-                else:
-                    xqnmat = xqnmat.reshape([1] + matshape)
-            if not self.cv_mpo.to_right:
-                xqnbigl = xqnl.copy()
-                xqnbigr = self.qnmat_add(xqnsigmalist[0], xqnr)
-                if xqnbigr.ndim == 3:
-                    rshape = list(xqnbigr.shape)
-                    xqnbigr = np.moveaxis(xqnbigr.reshape(rshape+[1]), -1, -2)
-            else:
-                xqnbigl = self.qnmat_add(xqnl, xqnsigmalist[0])
-                xqnbigr = xqnr.copy()
-                if xqnbigl.ndim == 3:
-                    lshape = list(xqnbigl.shape)
-                    xqnbigl = xqnbigl.reshape([1] + lshape)
-        else:
-            if xqnmat.ndim == 6:
-                if addlist[0] != 0:
-                    xqnmat = np.moveaxis(xqnmat.resahpe(matshape+[1]), -1, -2)
-                else:
-                    xqnmat = xqnmat.reshape([1] + matshape)
-            xqnbigl = self.qnmat_add(xqnl, xqnsigmalist[0])
-            if xqnbigl.ndim == 3:
-                lshape = list(xqnbigl.shape)
-                xqnbigl = xqnbigl.reshape([1] + lshape)
-            xqnbigr = self.qnmat_add(xqnsigmalist[-1], xqnr)
-            if xqnbigr.ndim == 3:
-                rshape = list(xqnbigr.shape)
-                xqnbigr = np.moveaxis(xqnbigr.reshape(rshape + [1]), -1, -2)
-        xshape = list(xqnmat.shape)
-        del xshape[-1]
-        if len(xshape) == 3:
-            if not self.cv_mpo.to_right:
-                xshape = xshape + [1]
-            else:
-                xshape = [1] + xshape
-        return xqnmat, xqnbigl, xqnbigr, xshape
-
-    def swap(self, mat, qnbigl, qnbigr):
-
-        def inter_change(ori_mat):
-            matshape = ori_mat.shape
-            len_mat = int(np.prod(np.array(matshape[:-1])))
-            ori_mat = ori_mat.reshape(len_mat, 2)
-            change_mat = copy.deepcopy(ori_mat)
-            change_mat[:, 0], change_mat[:, 1] = ori_mat[:, 1], ori_mat[:, 0]
-            return change_mat.reshape(matshape)
-
-        dag_qnmat = inter_change(mat)
-        if self.method == "1site":
-            dag_qnmat = np.moveaxis(dag_qnmat, [1, 2], [2, 1])
-            dag_qnbigl = inter_change(qnbigl)
-            dag_qnbigr = inter_change(qnbigr)
-            if not self.cv_mpo.to_right:
-                dag_qnbigr = np.moveaxis(dag_qnbigr, [0, 1], [1, 0])
-            else:
-                dag_qnbigl = np.moveaxis(dag_qnbigl, [1, 2], [2, 1])
-        else:
-            raise NotImplementedError
-            # we don't recommend 2-site CV-DMRG, which is a huge cost
-
-        return dag_qnmat, dag_qnbigl, dag_qnbigr
-
-    def condition(self, mat, qn):
-        condition = (mat == qn)
-        mat_shape = list(condition.shape)
-        del mat_shape[-1]
-        condition = condition.all(axis=-1)
-        condition = condition.reshape(mat_shape)
-        return condition
-
-    def qnmat_add(self, mat_l, mat_r):
-        lshape, rshape = mat_l.shape, mat_r.shape
-        lena = int(np.prod(np.array(lshape)) / 2)
-        lenb = int(np.prod(np.array(rshape)) / 2)
-        matl = mat_l.reshape(lena, 2)
-        matr = mat_r.reshape(lenb, 2)
-        lr1 = np.add.outer(matl[:, 0], matr[:, 0]).flatten()
-        lr2 = np.add.outer(matl[:, 1], matr[:, 1]).flatten()
-        lr = np.zeros((len(lr1), 2))
-        lr[:, 0] = lr1
-        lr[:, 1] = lr2
-        shapel = list(mat_l.shape)
-        del shapel[-1]
-        shaper = list(mat_r.shape)
-        del shaper[-1]
-        lr = lr.reshape(shapel + shaper + [2])
-        return lr
-
-    def dag2mat(self, xshape, x, dag_qnmat):
-        if self.spectratype == "abs":
-            up_exciton, down_exciton = 1, 0
-        else:
-            up_exciton, down_exciton = 0, 1
-        xdag = np.zeros(xshape, dtype=x.dtype)
-        mask = self.condition(dag_qnmat, [down_exciton, up_exciton])
-        np.place(xdag, mask, x)
-        shape = list(xdag.shape)
-        if xdag.ndim == 3:
-            if not self.cv_mpo.to_right:
-                xdag = xdag.reshape(shape + [1])
-            else:
-                xdag = xdag.reshape([1] + shape)
-        return xdag
-
-    def x_svd(self, xstruct, xqnbigl, xqnbigr, nexciton, percent=0):
-        Gamma = xstruct.reshape(
-            np.prod(xqnbigl.shape) // 2, np.prod(xqnbigr.shape) // 2)
-
-        localXqnl = xqnbigl.ravel()
-        localXqnr = xqnbigr.ravel()
-        list_locall = []
-        list_localr = []
-        for i in range(0, len(localXqnl), 2):
-            list_locall.append([localXqnl[i], localXqnl[i + 1]])
-        for i in range(0, len(localXqnr), 2):
-            list_localr.append([localXqnr[i], localXqnr[i + 1]])
-        localXqnl = copy.deepcopy(list_locall)
-        localXqnr = copy.deepcopy(list_localr)
-        xuset = []
-        xuset0 = []
-        xvset = []
-        xvset0 = []
-        xsset = []
-        xsuset0 = []
-        xsvset0 = []
-        xqnlset = []
-        xqnlset0 = []
-        xqnrset = []
-        xqnrset0 = []
-        if self.spectratype == "abs":
-            combine = [[[y, 0], [nexciton - y, 0]]
-                       for y in range(nexciton + 1)]
-        elif self.spectratype == "emi":
-            combine = [[[0, y], [0, nexciton - y]]
-                       for y in range(nexciton + 1)]
-        for nl, nr in combine:
-            lset = np.where(self.condition(np.array(localXqnl), [nl]))[0]
-            rset = np.where(self.condition(np.array(localXqnr), [nr]))[0]
-            if len(lset) != 0 and len(rset) != 0:
-                Gamma_block = Gamma.ravel().take(
-                    (lset * Gamma.shape[1]).reshape(-1, 1) + rset)
-                try:
-                    U, S, Vt = \
-                        scipy.linalg.svd(Gamma_block, full_matrices=True,
-                                         lapack_driver='gesdd')
-                except:
-                    U, S, Vt = \
-                        scipy.linalg.svd(Gamma_block, full_matrices=True,
-                                         lapack_driver='gesvd')
-
-                dim = S.shape[0]
-
-                xsset.append(S)
-                # U part quantum number
-                xuset.append(
-                    svd_qn.blockrecover(lset, U[:, :dim], Gamma.shape[0]))
-                xqnlset += [nl] * dim
-                xuset0.append(
-                    svd_qn.blockrecover(lset, U[:, dim:], Gamma.shape[0]))
-                xqnlset0 += [nl] * (U.shape[0] - dim)
-                xsuset0.append(np.zeros(U.shape[0] - dim))
-                # V part quantum number
-                VT = Vt.T
-                xvset.append(
-                    svd_qn.blockrecover(rset, VT[:, :dim], Gamma.shape[1]))
-                xqnrset += [nr] * dim
-                xvset0.append(
-                    svd_qn.blockrecover(rset, VT[:, dim:], Gamma.shape[1]))
-                xqnrset0 += [nr] * (VT.shape[0] - dim)
-                xsvset0.append(np.zeros(VT.shape[0] - dim))
-        xuset = np.concatenate(xuset + xuset0, axis=1)
-        xvset = np.concatenate(xvset + xvset0, axis=1)
-        xsuset = np.concatenate(xsset + xsuset0)
-        xsvset = np.concatenate(xsset + xsvset0)
-        xqnlset = xqnlset + xqnlset0
-        xqnrset = xqnrset + xqnrset0
-        bigl_shape = list(xqnbigl.shape)
-        del bigl_shape[-1]
-        bigr_shape = list(xqnbigr.shape)
-        del bigr_shape[-1]
-        if not self.cv_mpo.to_right:
-            x, xdim, xqn, compx = update_cv(
-                xvset, xsvset, xqnrset, xuset, nexciton, self.m_max,
-                self.spectratype, percent=percent)
-            if (self.method == "1site") and (len(bigr_shape + [xdim]) == 3):
-                return np.moveaxis(
-                    x.reshape(bigr_shape + [1] + [xdim]), -1, 0),\
-                    xdim, xqn, compx.reshape(bigl_shape + [xdim])
-            else:
-                return np.moveaxis(x.reshape(bigr_shape + [xdim]), -1, 0),\
-                    xdim, xqn, compx.reshape(bigl_shape + [xdim])
-        else:
-            x, xdim, xqn, compx = update_cv(
-                xuset, xsuset, xqnlset, xvset, nexciton,
-                self.m_max, self.spectratype, percent=percent)
-            if (self.method == "1site") and (len(bigl_shape + [xdim]) == 3):
-                return x.reshape([1] + bigl_shape + [xdim]), xdim, xqn, \
-                    np.moveaxis(compx.reshape(bigr_shape + [xdim]), -1, 0)
-            else:
-                return x.reshape(bigl_shape + [xdim]), xdim, xqn, \
-                    np.moveaxis(compx.reshape(bigr_shape + [xdim]), -1, 0)
-
-    def initialize_LR(self):
-
-        first_LR = [np.ones((1, 1, 1, 1))]
-        forth_LR = [np.ones((1, 1))]
-        for isite in range(1, len(self.cv_mpo)):
-            first_LR.append(None)
-            forth_LR.append(None)
-        first_LR.append(np.ones((1, 1, 1, 1)))
-        second_LR = copy.deepcopy(first_LR)
-        third_LR = copy.deepcopy(first_LR)
-        forth_LR.append(np.ones((1, 1)))
-
-        if self.cv_mpo.to_right:
-            for isite in range(len(self.cv_mpo), 1, -1):
-                cv_isite = self.cv_mpo[isite-1]
-                dag_cv_isite = moveaxis(cv_isite, (1, 2), (2, 1))
-                path1 = [([0, 1], "abcd, efga -> bcdefg"),
-                         ([3, 0], "bcdefg, hgib -> cdefhi"),
-                         ([2, 0], "cdefhi, jikc -> defhjk"),
-                         ([1, 0], "defhjk, lkfd -> ehjl")]
-                path2 = [([0, 1], "ab, cdea->bcde"),
-                         ([1, 0], "bcde, fedb->cf")]
-                first_LR[isite - 1] = asnumpy(multi_tensor_contract(
-                    path1, first_LR[isite],
-                    dag_cv_isite, self.a_oper[isite - 1],
-                    self.a_oper[isite - 1], cv_isite))
-
-                second_LR[isite - 1] = asnumpy(multi_tensor_contract(
-                    path1, second_LR[isite],
-                    dag_cv_isite,
-                    self.a_oper[isite - 1], cv_isite,
-                    self.h_mpo[isite - 1]))
-                third_LR[isite - 1] = asnumpy(multi_tensor_contract(
-                    path1, third_LR[isite], self.h_mpo[isite - 1],
-                    dag_cv_isite,
-                    cv_isite, self.h_mpo[isite - 1]))
-                forth_LR[isite - 1] = asnumpy(multi_tensor_contract(
-                    path2, forth_LR[isite],
-                    moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
-                    cv_isite))
-
-        else:
-            for isite in range(1, len(self.cv_mpo)):
-                cv_isite = self.cv_mpo[isite-1]
-                dag_cv_isite = moveaxis(cv_isite, (1, 2), (2, 1))
-                path1 = [([0, 1], "abcd, aefg -> bcdefg"),
-                         ([3, 0], "bcdefg, bfhi -> cdeghi"),
-                         ([2, 0], "cdeghi, chjk -> degijk"),
-                         ([1, 0], "degijk, djel -> gikl")]
-                path2 = [([0, 1], "ab, acde->bcde"),
-                         ([1, 0], "bcde, bdcf->ef")]
-                first_LR[isite] = asnumpy(multi_tensor_contract(
-                    path1, first_LR[isite - 1],
-                    dag_cv_isite, self.a_oper[isite - 1],
-                    self.a_oper[isite - 1], cv_isite))
-                second_LR[isite] = asnumpy(multi_tensor_contract(
-                    path1, second_LR[isite - 1],
-                    dag_cv_isite,
-                    self.a_oper[isite - 1], cv_isite,
-                    self.h_mpo[isite - 1]))
-                third_LR[isite] = asnumpy(multi_tensor_contract(
-                    path1, third_LR[isite - 1], self.h_mpo[isite - 1],
-                    dag_cv_isite,
-                    cv_isite, self.h_mpo[isite - 1]))
-                forth_LR[isite] = asnumpy(multi_tensor_contract(
-                    path2, forth_LR[isite - 1],
-                    moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
-                    cv_isite))
-        return [first_LR, second_LR, third_LR, forth_LR]
-
-    def update_LR(self, lr_group, isite):
-        first_LR, second_LR, third_LR, forth_LR = lr_group
-        cv_isite = self.cv_mpo[isite-1]
-        dag_cv_isite = moveaxis(cv_isite, (1, 2), (2, 1))
-        if self.method == "1site":
-            if not self.cv_mpo.to_right:
-                path1 = [([0, 1], "abcd, efga -> bcdefg"),
-                         ([3, 0], "bcdefg, hgib -> cdefhi"),
-                         ([2, 0], "cdefhi, jikc -> defhjk"),
-                         ([1, 0], "defhjk, lkfd -> ehjl")]
-                path2 = [([0, 1], "ab, cdea->bcde"),
-                         ([1, 0], "bcde, fedb->cf")]
-                first_LR[isite - 1] = multi_tensor_contract(
-                    path1, first_LR[isite],
-                    dag_cv_isite, self.a_oper[isite - 1],
-                    self.a_oper[isite - 1], cv_isite)
-                second_LR[isite - 1] = multi_tensor_contract(
-                    path1, second_LR[isite],
-                    dag_cv_isite,
-                    self.a_oper[isite - 1], cv_isite,
-                    self.h_mpo[isite - 1])
-                third_LR[isite - 1] = multi_tensor_contract(
-                    path1, third_LR[isite], self.h_mpo[isite - 1],
-                    dag_cv_isite,
-                    cv_isite, self.h_mpo[isite - 1])
-                forth_LR[isite - 1] = multi_tensor_contract(
-                    path2, forth_LR[isite],
-                    moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
-                    cv_isite)
-
-            else:
-                path1 = [([0, 1], "abcd, aefg -> bcdefg"),
-                         ([3, 0], "bcdefg, bfhi -> cdeghi"),
-                         ([2, 0], "cdeghi, chjk -> degijk"),
-                         ([1, 0], "degijk, djel -> gikl")]
-                path2 = [([0, 1], "ab, acde->bcde"),
-                         ([1, 0], "bcde, bdcf->ef")]
-
-                first_LR[isite] = multi_tensor_contract(
-                    path1, first_LR[isite - 1],
-                    dag_cv_isite,
-                    self.a_oper[isite - 1], self.a_oper[isite - 1], cv_isite)
-
-                second_LR[isite] = multi_tensor_contract(
-                    path1, second_LR[isite - 1],
-                    dag_cv_isite,
-                    self.a_oper[isite - 1], cv_isite,
-                    self.h_mpo[isite - 1])
-                third_LR[isite] = multi_tensor_contract(
-                    path1, third_LR[isite - 1], self.h_mpo[isite - 1],
-                    dag_cv_isite,
-                    cv_isite, self.h_mpo[isite - 1])
-                forth_LR[isite] = multi_tensor_contract(
-                    path2, forth_LR[isite - 1],
-                    moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
-                    cv_isite)
-        else:
-            # 2site for finite temperature is too expensive, so I drop it
-            # (at least for now)
-            raise NotImplementedError
-
-        return first_LR, second_LR, third_LR, forth_LR
+# -*- coding: utf-8 -*-
+# Author: Tong Jiang <tongjiang1000@gmail.com>
+# finite temperature absorption/emission spectrum based on Correction vector
+
+import copy
+import os
+import logging
+import scipy
+from itertools import product
+
+from renormalizer.mps.matrix import (
+    multi_tensor_contract,
+    tensordot,
+    moveaxis
+)
+from renormalizer.cv.spectra_cv import SpectraCv
+from renormalizer.mps.backend import np, xp
+from renormalizer.mps.matrix import asxp, asnumpy
+from renormalizer.mps import (
+    Mpo, svd_qn, MpDm, ThermalProp, load_thermal_state)
+from renormalizer.mps.lib import update_cv
+from renormalizer.utils import (
+    CompressConfig, EvolveConfig,
+    CompressCriteria
+)
+
+logger = logging.getLogger(__name__)
+
+
+class SpectraFtCV(SpectraCv):
+    r"""
+    Use DDMRG to calculate the finite temperature spectrum from frequency domain
+
+    Args:
+        model (:class:`~renormalizer.model.Model`): system information.
+        spectratype (string): "abs" or "emi".
+        m_max (int): maximal bond dimension of correction vector.
+        eta (float): Lorentzian broadening width (a.u.).
+        temperature (:class:`~renormalizer.utils.Quantity`): simulation temperature.
+        h_mpo (:class:`~renormalizer.mps.Mpo`): system Hamiltonian.
+        method (str): "1site" or "2site".
+        procedure_cv (list): percent used for each sweep.
+        rtol (float): the relative tolerance of the spectrum strength, default: 1e-5.
+        b_mps (:class:`~renormalizer.mps.Mps`): the b vector -eta * dipole * \psi_0, default: None.
+            (Holstein model could construct b_mps implicitly).
+        cv_mps (:class:`~renormalizer.mps.Mps`): initial guess of cv_mps, default: None.
+        icompress_config (:class:`~renormalizer.utils.CompressConfig`): config when compressing MPS/MPO during the imaginary time evolution..
+        ievolve_config (:class:`~renormalizer.utils.EvolveConfig`): evolution config for imaginary time evolution.
+        insteps (int): evolve steps for imaginary time evolution. have to be provided when calculating emission.
+        dump_dir (str): the directory for logging and numerical result output.
+            Also the directory from which to load previous thermal propagated initial state (if exists).
+        job_name (str): the name of the calculation job which determines the file name of the logging and numerical result output.
+
+    Example::
+        see test/test_abs.py for example
+
+    """
+    def __init__(
+        self,
+        model,
+        spectratype,
+        m_max,
+        eta,
+        temperature,
+        h_mpo=None,
+        method='1site',
+        procedure_cv=None,
+        rtol=1e-5,
+        b_mps=None,
+        cv_mps=None,
+        icompress_config=None,
+        ievolve_config=None,
+        insteps=None,
+        dump_dir: str=None,
+        job_name=None,
+    ):
+
+        self.temperature = temperature
+        self.evolve_config = ievolve_config
+        self.compress_config = icompress_config
+        if self.evolve_config is None:
+            self.evolve_config = \
+                EvolveConfig()
+        if self.compress_config is None:
+            self.compress_config = \
+                CompressConfig(CompressCriteria.fixed,
+                               max_bonddim=m_max)
+            self.compress_config.set_bonddim(len(model.pbond_list))
+        self.insteps = insteps
+        self.job_name = job_name
+        self.dump_dir = dump_dir
+
+        super().__init__(
+            model, spectratype, m_max, eta, h_mpo=h_mpo,
+            method=method, procedure_cv=procedure_cv,
+            rtol=rtol, b_mps=b_mps, cv_mps=cv_mps,
+        )
+
+        self.cv_mpo = self.cv_mps
+        self.b_mpo = self.b_mps
+
+        self.a_oper = None
+
+    def init_cv_mpo(self):
+        cv_mpo = Mpo.finiteT_cv(self.model, 1, self.m_max,
+                                self.spectratype, percent=1.0)
+        return cv_mpo
+
+    init_cv_mps = init_cv_mpo
+
+    def init_b_mpo(self):
+        # get the right hand site vector b, Ax=b
+        # b = -eta * dipole * \psi_0
+
+        # only support Holstien model 0/1 exciton manifold
+        beta = self.temperature.to_beta()
+        if self.spectratype == "abs":
+            dipole_mpo = Mpo.onsite(self.model, r"a^\dagger", dipole=True)
+            i_mpo = MpDm.max_entangled_gs(self.model)
+            tp = ThermalProp(i_mpo, exact=True, space='GS')
+            tp.evolve(None, 1, beta / 2j)
+            ket_mpo = tp.latest_mps
+        elif self.spectratype == "emi":
+            dipole_mpo = Mpo.onsite(self.model, "a", dipole=True)
+            if self._defined_output_path:
+                ket_mpo = \
+                    load_thermal_state(self.model, self._thermal_dump_path)
+            else:
+                ket_mpo = None
+            if ket_mpo is None:
+                impo = MpDm.max_entangled_ex(self.model)
+                impo.compress_config = self.compress_config
+                if self.job_name is None:
+                    job_name = None
+                else:
+                    job_name = self.job_name + "_thermal_prop"
+                tp = ThermalProp(
+                    impo, evolve_config=self.evolve_config,
+                    dump_dir=self.dump_dir, job_name=job_name)
+                tp.evolve(None, self.insteps, beta / 2j)
+                ket_mpo = tp.latest_mps
+                if self._defined_output_path:
+                    ket_mpo.dump(self._thermal_dump_path)
+        else:
+            assert False
+        ket_mpo = dipole_mpo.apply(ket_mpo.scale(-self.eta))
+
+        return ket_mpo, None
+
+    init_b_mps = init_b_mpo
+
+    @property
+    def _thermal_dump_path(self):
+        assert self._defined_output_path
+        return os.path.join(self.dump_dir, self.job_name + "_impo.npz")
+
+    @property
+    def _defined_output_path(self):
+        return self.dump_dir is not None and self.job_name is not None
+
+    def oper_prepare(self, omega):
+        identity = Mpo.identity(self.model).scale(omega)
+        self.a_oper = identity.add(self.h_mpo.scale(-1, inplace=False))
+
+    def optimize_cv(self, lr_group, isite, percent=0):
+        if self.spectratype == "abs":
+            # quantum number restriction, |1><0|
+            up_exciton, down_exciton = 1, 0
+        elif self.spectratype == "emi":
+            # quantum number restriction, |0><1|
+            up_exciton, down_exciton = 0, 1
+        nexciton = 1
+        first_LR, second_LR, third_LR, forth_LR = lr_group
+
+        if self.method == "1site":
+            add_list = [isite - 1]
+            first_L = asxp(first_LR[isite - 1])
+            first_R = asxp(first_LR[isite])
+            second_L = asxp(second_LR[isite - 1])
+            second_R = asxp(second_LR[isite])
+            third_L = asxp(third_LR[isite - 1])
+            third_R = asxp(third_LR[isite])
+            forth_L = asxp(forth_LR[isite - 1])
+            forth_R = asxp(forth_LR[isite])
+        else:
+            add_list = [isite - 2, isite - 1]
+            first_L = asxp(first_LR[isite - 2])
+            first_R = asxp(first_LR[isite])
+            second_L = asxp(second_LR[isite - 2])
+            second_R = asxp(second_LR[isite])
+            third_L = asxp(third_LR[isite - 2])
+            third_R = asxp(third_LR[isite])
+            forth_L = asxp(forth_LR[isite - 2])
+            forth_R = asxp(forth_LR[isite])
+
+        xqnmat, xqnbigl, xqnbigr, xshape = \
+            self.construct_X_qnmat(add_list)
+        dag_qnmat, dag_qnbigl, dag_qnbigr = self.swap(xqnmat, xqnbigl, xqnbigr)
+        nonzeros = int(np.sum(
+            self.condition(
+                dag_qnmat, [down_exciton, up_exciton])
+        ))
+
+        if self.method == "1site":
+            guess = moveaxis(self.cv_mpo[isite - 1], (1, 2), (2, 1))
+        else:
+            guess = tensordot(moveaxis(self.cv_mpo[isite - 2], (1, 2), (2, 1)),
+                              moveaxis(self.cv_mpo[isite - 1]), axes=(-1, 0))
+        guess = guess[
+            self.condition(
+                dag_qnmat, [down_exciton, up_exciton])]
+
+        if self.method == "1site":
+            # define dot path
+            path_1 = [([0, 1], "abcd, aefg -> bcdefg"),
+                      ([3, 0], "bcdefg, bfhi -> cdeghi"),
+                      ([2, 0], "cdeghi, chjk -> degijk"),
+                      ([1, 0], "degijk, gikl -> dejl")]
+            path_2 = [([0, 1], "abcd, aefg -> bcdefg"),
+                      ([3, 0], "bcdefg, bfhi -> cdeghi"),
+                      ([2, 0], "cdeghi, djek -> cghijk"),
+                      ([1, 0], "cghijk, gilk -> chjl")]
+            path_3 = [([0, 1], "ab, acde -> bcde"),
+                      ([1, 0], "bcde, ef -> bcdf")]
+
+            vecb = multi_tensor_contract(
+                path_3, forth_L,
+                moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
+                forth_R)[self.condition(dag_qnmat, [down_exciton, up_exciton])]
+
+        a_oper_isite = asxp(self.a_oper[isite - 1])
+        h_mpo_isite = asxp(self.h_mpo[isite - 1])
+        # construct preconditioner
+        Idt = xp.identity(h_mpo_isite.shape[1])
+        M1_1 = xp.einsum('abca->abc', first_L)
+        path_m1 = [([0, 1], "abc, bdef->acdef"),
+                   ([1, 0], "acdef, cegh->adfgh")]
+        M1_2 = multi_tensor_contract(path_m1, M1_1, a_oper_isite, a_oper_isite)
+        M1_2 = xp.einsum("abcbd->abcd", M1_2)
+        M1_3 = xp.einsum('ecde->ecd', first_R)
+        M1_4 = xp.einsum('ff->f', Idt)
+        path_m1 = [([0, 1], "abcd,ecd->abe"),
+                   ([1, 0], "abe,f->abef")]
+        pre_M1 = multi_tensor_contract(
+            path_m1, M1_2, M1_3, M1_4)
+        pre_M1 = xp.moveaxis(pre_M1, [-2, -1], [-1, -2])[
+            self.condition(dag_qnmat, [down_exciton, up_exciton])]
+
+        M2_1 = xp.einsum('aeag->aeg', second_L)
+        M2_2 = xp.einsum('eccf->ecf', a_oper_isite)
+        M2_3 = xp.einsum('gbbh->gbh', h_mpo_isite)
+        M2_4 = xp.einsum('dfdh->dfh', second_R)
+        path_m2 = [([0, 1], "aeg,gbh->aebh"),
+                   ([2, 0], "aebh,ecf->abchf"),
+                   ([1, 0], "abhcf,dfh->abcd")]
+        pre_M2 = multi_tensor_contract(
+            path_m2, M2_1, M2_3, M2_2, M2_4)
+        pre_M2 = pre_M2[
+            self.condition(dag_qnmat, [down_exciton, up_exciton])]
+
+        M4_1 = xp.einsum('faah->fah', third_L)
+        M4_4 = xp.einsum('gddi->gdi', third_R)
+        M4_5 = xp.einsum('cc->c', Idt)
+        M4_path = [([0, 1], "fah,febg->ahebg"),
+                   ([2, 0], "ahebg,hjei->abgji"),
+                   ([1, 0], "abgji,gdi->abjd")]
+        pre_M4 = multi_tensor_contract(
+            M4_path, M4_1, h_mpo_isite,
+            h_mpo_isite, M4_4)
+        pre_M4 = xp.einsum('abbd->abd', pre_M4)
+        pre_M4 = xp.tensordot(pre_M4, M4_5, axes=0)
+        pre_M4 = xp.moveaxis(pre_M4, [2, 3], [3, 2])[
+            self.condition(dag_qnmat, [down_exciton, up_exciton])]
+
+        M_x = lambda x: asnumpy(asxp(x) / (pre_M1 + 2 * pre_M2 + pre_M4 + xp.ones(nonzeros)*self.eta**2))
+        pre_M = scipy.sparse.linalg.LinearOperator((nonzeros, nonzeros), M_x)
+
+        count = 0
+
+        def hop(x):
+            nonlocal count
+            count += 1
+            dag_struct = asxp(self.dag2mat(
+                xshape, x, dag_qnmat))
+            if self.method == "1site":
+
+                M1 = multi_tensor_contract(
+                    path_1, first_L, dag_struct,
+                    a_oper_isite, a_oper_isite, first_R)
+                M2 = multi_tensor_contract(
+                    path_2, second_L, dag_struct,
+                    a_oper_isite,
+                    h_mpo_isite, second_R)
+                M2 = xp.moveaxis(M2, (1, 2), (2, 1))
+                M3 = multi_tensor_contract(
+                    path_2, third_L, h_mpo_isite, dag_struct,
+                    h_mpo_isite, third_R)
+                M3 = xp.moveaxis(M3, (1, 2), (2, 1))
+                cout = M1 + 2 * M2 + M3 + dag_struct * self.eta**2
+            cout = cout[
+                self.condition(dag_qnmat, [down_exciton, up_exciton])
+            ]
+            return asnumpy(cout)
+
+        # Matrix A
+        mat_a = scipy.sparse.linalg.LinearOperator((nonzeros, nonzeros), matvec=hop)
+
+        x, info = scipy.sparse.linalg.cg(
+            mat_a, asnumpy(vecb), tol=1.e-5, x0=asnumpy(guess), maxiter=500,
+            M=pre_M, atol=0)
+        # logger.info(f"linear eq dim: {nonzeros}")
+        # logger.info(f'times for hop:{count}')
+        self.hop_time.append(count)
+        if info != 0:
+            logger.warning(
+                f"cg not converged, vecb.norm:{xp.linalg.norm(vecb)}")
+        l_value = xp.dot(asxp(hop(x)), asxp(x)) - 2 * xp.dot(vecb, asxp(x))
+
+        x = self.dag2mat(xshape, x, dag_qnmat)
+        if self.method == "1site":
+            x = np.moveaxis(x, [1, 2], [2, 1])
+        x, xdim, xqn, compx = self.x_svd(
+            x, xqnbigl, xqnbigr, nexciton,
+            percent=percent)
+
+        if self.method == "1site":
+            self.cv_mpo[isite - 1] = x
+            if not self.cv_mpo.to_right:
+                if isite != 1:
+                    self.cv_mpo[isite - 2] = \
+                        tensordot(self.cv_mpo[isite - 2], compx, axes=(-1, 0))
+                    self.cv_mpo.qn[isite - 1] = xqn
+                    self.cv_mpo.qnidx = isite-2
+                else:
+                    self.cv_mpo[isite - 1] = \
+                        tensordot(compx, self.cv_mpo[isite - 1], axes=(-1, 0))
+                    self.cv_mpo.qnidx = 0
+            else:
+                if isite != len(self.cv_mpo):
+                    self.cv_mpo[isite] = \
+                        tensordot(compx, self.cv_mpo[isite], axes=(-1, 0))
+                    self.cv_mpo.qn[isite] = xqn
+                    self.cv_mpo.qnidx = isite
+                else:
+                    self.cv_mpo[isite - 1] = \
+                        tensordot(self.cv_mpo[isite - 1], compx, axes=(-1, 0))
+                    self.cv_mpo.qnidx = self.cv_mpo.site_num-1
+
+        else:
+            if not self.cv_mpo.to_right:
+                self.cv_mpo[isite - 2] = compx
+                self.cv_mpo[isite - 1] = x
+                self.cv_mpo.qnidx = isite-2
+            else:
+                self.cv_mpo[isite - 2] = x
+                self.cv_mpo[isite - 1] = compx
+                self.cv_mpo.qnidx = isite-1
+            self.cv_mpo.qn[isite - 1] = xqn
+
+        return float(l_value)
+
+    def construct_X_qnmat(self, addlist):
+
+        pbond = self.model.pbond_list
+        xqnl = np.array(self.cv_mpo.qn[addlist[0]])
+        xqnr = np.array(self.cv_mpo.qn[addlist[-1] + 1])
+        xqnmat = xqnl.copy()
+        xqnsigmalist = []
+        for idx in addlist:
+            sigmaqn = self.model.basis[idx].sigmaqn
+            xqnsigma = np.array(list(product(sigmaqn, repeat=2)))
+            xqnsigma = xqnsigma.reshape(pbond[idx], pbond[idx], 2)
+
+            xqnmat = self.qnmat_add(xqnmat, xqnsigma)
+            xqnsigmalist.append(xqnsigma)
+
+        xqnmat = self.qnmat_add(xqnmat, xqnr)
+        matshape = list(xqnmat.shape)
+        if self.method == "1site":
+            if xqnmat.ndim == 4:
+                if not self.cv_mpo.to_right:
+                    xqnmat = np.moveaxis(xqnmat.reshape(matshape+[1]), -1, -2)
+                else:
+                    xqnmat = xqnmat.reshape([1] + matshape)
+            if not self.cv_mpo.to_right:
+                xqnbigl = xqnl.copy()
+                xqnbigr = self.qnmat_add(xqnsigmalist[0], xqnr)
+                if xqnbigr.ndim == 3:
+                    rshape = list(xqnbigr.shape)
+                    xqnbigr = np.moveaxis(xqnbigr.reshape(rshape+[1]), -1, -2)
+            else:
+                xqnbigl = self.qnmat_add(xqnl, xqnsigmalist[0])
+                xqnbigr = xqnr.copy()
+                if xqnbigl.ndim == 3:
+                    lshape = list(xqnbigl.shape)
+                    xqnbigl = xqnbigl.reshape([1] + lshape)
+        else:
+            if xqnmat.ndim == 6:
+                if addlist[0] != 0:
+                    xqnmat = np.moveaxis(xqnmat.resahpe(matshape+[1]), -1, -2)
+                else:
+                    xqnmat = xqnmat.reshape([1] + matshape)
+            xqnbigl = self.qnmat_add(xqnl, xqnsigmalist[0])
+            if xqnbigl.ndim == 3:
+                lshape = list(xqnbigl.shape)
+                xqnbigl = xqnbigl.reshape([1] + lshape)
+            xqnbigr = self.qnmat_add(xqnsigmalist[-1], xqnr)
+            if xqnbigr.ndim == 3:
+                rshape = list(xqnbigr.shape)
+                xqnbigr = np.moveaxis(xqnbigr.reshape(rshape + [1]), -1, -2)
+        xshape = list(xqnmat.shape)
+        del xshape[-1]
+        if len(xshape) == 3:
+            if not self.cv_mpo.to_right:
+                xshape = xshape + [1]
+            else:
+                xshape = [1] + xshape
+        return xqnmat, xqnbigl, xqnbigr, xshape
+
+    def swap(self, mat, qnbigl, qnbigr):
+
+        def inter_change(ori_mat):
+            matshape = ori_mat.shape
+            len_mat = int(np.prod(np.array(matshape[:-1])))
+            ori_mat = ori_mat.reshape(len_mat, 2)
+            change_mat = copy.deepcopy(ori_mat)
+            change_mat[:, 0], change_mat[:, 1] = ori_mat[:, 1], ori_mat[:, 0]
+            return change_mat.reshape(matshape)
+
+        dag_qnmat = inter_change(mat)
+        if self.method == "1site":
+            dag_qnmat = np.moveaxis(dag_qnmat, [1, 2], [2, 1])
+            dag_qnbigl = inter_change(qnbigl)
+            dag_qnbigr = inter_change(qnbigr)
+            if not self.cv_mpo.to_right:
+                dag_qnbigr = np.moveaxis(dag_qnbigr, [0, 1], [1, 0])
+            else:
+                dag_qnbigl = np.moveaxis(dag_qnbigl, [1, 2], [2, 1])
+        else:
+            raise NotImplementedError
+            # we don't recommend 2-site CV-DMRG, which is a huge cost
+
+        return dag_qnmat, dag_qnbigl, dag_qnbigr
+
+    def condition(self, mat, qn):
+        condition = (mat == qn)
+        mat_shape = list(condition.shape)
+        del mat_shape[-1]
+        condition = condition.all(axis=-1)
+        condition = condition.reshape(mat_shape)
+        return condition
+
+    def qnmat_add(self, mat_l, mat_r):
+        lshape, rshape = mat_l.shape, mat_r.shape
+        lena = int(np.prod(np.array(lshape)) / 2)
+        lenb = int(np.prod(np.array(rshape)) / 2)
+        matl = mat_l.reshape(lena, 2)
+        matr = mat_r.reshape(lenb, 2)
+        lr1 = np.add.outer(matl[:, 0], matr[:, 0]).flatten()
+        lr2 = np.add.outer(matl[:, 1], matr[:, 1]).flatten()
+        lr = np.zeros((len(lr1), 2))
+        lr[:, 0] = lr1
+        lr[:, 1] = lr2
+        shapel = list(mat_l.shape)
+        del shapel[-1]
+        shaper = list(mat_r.shape)
+        del shaper[-1]
+        lr = lr.reshape(shapel + shaper + [2])
+        return lr
+
+    def dag2mat(self, xshape, x, dag_qnmat):
+        if self.spectratype == "abs":
+            up_exciton, down_exciton = 1, 0
+        else:
+            up_exciton, down_exciton = 0, 1
+        xdag = np.zeros(xshape, dtype=x.dtype)
+        mask = self.condition(dag_qnmat, [down_exciton, up_exciton])
+        np.place(xdag, mask, x)
+        shape = list(xdag.shape)
+        if xdag.ndim == 3:
+            if not self.cv_mpo.to_right:
+                xdag = xdag.reshape(shape + [1])
+            else:
+                xdag = xdag.reshape([1] + shape)
+        return xdag
+
+    def x_svd(self, xstruct, xqnbigl, xqnbigr, nexciton, percent=0):
+        Gamma = xstruct.reshape(
+            np.prod(xqnbigl.shape) // 2, np.prod(xqnbigr.shape) // 2)
+
+        localXqnl = xqnbigl.ravel()
+        localXqnr = xqnbigr.ravel()
+        list_locall = []
+        list_localr = []
+        for i in range(0, len(localXqnl), 2):
+            list_locall.append([localXqnl[i], localXqnl[i + 1]])
+        for i in range(0, len(localXqnr), 2):
+            list_localr.append([localXqnr[i], localXqnr[i + 1]])
+        localXqnl = copy.deepcopy(list_locall)
+        localXqnr = copy.deepcopy(list_localr)
+        xuset = []
+        xuset0 = []
+        xvset = []
+        xvset0 = []
+        xsset = []
+        xsuset0 = []
+        xsvset0 = []
+        xqnlset = []
+        xqnlset0 = []
+        xqnrset = []
+        xqnrset0 = []
+        if self.spectratype == "abs":
+            combine = [[[y, 0], [nexciton - y, 0]]
+                       for y in range(nexciton + 1)]
+        elif self.spectratype == "emi":
+            combine = [[[0, y], [0, nexciton - y]]
+                       for y in range(nexciton + 1)]
+        for nl, nr in combine:
+            lset = np.where(self.condition(np.array(localXqnl), [nl]))[0]
+            rset = np.where(self.condition(np.array(localXqnr), [nr]))[0]
+            if len(lset) != 0 and len(rset) != 0:
+                Gamma_block = Gamma.ravel().take(
+                    (lset * Gamma.shape[1]).reshape(-1, 1) + rset)
+                try:
+                    U, S, Vt = \
+                        scipy.linalg.svd(Gamma_block, full_matrices=True,
+                                         lapack_driver='gesdd')
+                except:
+                    U, S, Vt = \
+                        scipy.linalg.svd(Gamma_block, full_matrices=True,
+                                         lapack_driver='gesvd')
+
+                dim = S.shape[0]
+
+                xsset.append(S)
+                # U part quantum number
+                xuset.append(
+                    svd_qn.blockrecover(lset, U[:, :dim], Gamma.shape[0]))
+                xqnlset += [nl] * dim
+                xuset0.append(
+                    svd_qn.blockrecover(lset, U[:, dim:], Gamma.shape[0]))
+                xqnlset0 += [nl] * (U.shape[0] - dim)
+                xsuset0.append(np.zeros(U.shape[0] - dim))
+                # V part quantum number
+                VT = Vt.T
+                xvset.append(
+                    svd_qn.blockrecover(rset, VT[:, :dim], Gamma.shape[1]))
+                xqnrset += [nr] * dim
+                xvset0.append(
+                    svd_qn.blockrecover(rset, VT[:, dim:], Gamma.shape[1]))
+                xqnrset0 += [nr] * (VT.shape[0] - dim)
+                xsvset0.append(np.zeros(VT.shape[0] - dim))
+        xuset = np.concatenate(xuset + xuset0, axis=1)
+        xvset = np.concatenate(xvset + xvset0, axis=1)
+        xsuset = np.concatenate(xsset + xsuset0)
+        xsvset = np.concatenate(xsset + xsvset0)
+        xqnlset = xqnlset + xqnlset0
+        xqnrset = xqnrset + xqnrset0
+        bigl_shape = list(xqnbigl.shape)
+        del bigl_shape[-1]
+        bigr_shape = list(xqnbigr.shape)
+        del bigr_shape[-1]
+        if not self.cv_mpo.to_right:
+            x, xdim, xqn, compx = update_cv(
+                xvset, xsvset, xqnrset, xuset, nexciton, self.m_max,
+                self.spectratype, percent=percent)
+            if (self.method == "1site") and (len(bigr_shape + [xdim]) == 3):
+                return np.moveaxis(
+                    x.reshape(bigr_shape + [1] + [xdim]), -1, 0),\
+                    xdim, xqn, compx.reshape(bigl_shape + [xdim])
+            else:
+                return np.moveaxis(x.reshape(bigr_shape + [xdim]), -1, 0),\
+                    xdim, xqn, compx.reshape(bigl_shape + [xdim])
+        else:
+            x, xdim, xqn, compx = update_cv(
+                xuset, xsuset, xqnlset, xvset, nexciton,
+                self.m_max, self.spectratype, percent=percent)
+            if (self.method == "1site") and (len(bigl_shape + [xdim]) == 3):
+                return x.reshape([1] + bigl_shape + [xdim]), xdim, xqn, \
+                    np.moveaxis(compx.reshape(bigr_shape + [xdim]), -1, 0)
+            else:
+                return x.reshape(bigl_shape + [xdim]), xdim, xqn, \
+                    np.moveaxis(compx.reshape(bigr_shape + [xdim]), -1, 0)
+
+    def initialize_LR(self):
+
+        first_LR = [np.ones((1, 1, 1, 1))]
+        forth_LR = [np.ones((1, 1))]
+        for isite in range(1, len(self.cv_mpo)):
+            first_LR.append(None)
+            forth_LR.append(None)
+        first_LR.append(np.ones((1, 1, 1, 1)))
+        second_LR = copy.deepcopy(first_LR)
+        third_LR = copy.deepcopy(first_LR)
+        forth_LR.append(np.ones((1, 1)))
+
+        if self.cv_mpo.to_right:
+            for isite in range(len(self.cv_mpo), 1, -1):
+                cv_isite = self.cv_mpo[isite-1]
+                dag_cv_isite = moveaxis(cv_isite, (1, 2), (2, 1))
+                path1 = [([0, 1], "abcd, efga -> bcdefg"),
+                         ([3, 0], "bcdefg, hgib -> cdefhi"),
+                         ([2, 0], "cdefhi, jikc -> defhjk"),
+                         ([1, 0], "defhjk, lkfd -> ehjl")]
+                path2 = [([0, 1], "ab, cdea->bcde"),
+                         ([1, 0], "bcde, fedb->cf")]
+                first_LR[isite - 1] = asnumpy(multi_tensor_contract(
+                    path1, first_LR[isite],
+                    dag_cv_isite, self.a_oper[isite - 1],
+                    self.a_oper[isite - 1], cv_isite))
+
+                second_LR[isite - 1] = asnumpy(multi_tensor_contract(
+                    path1, second_LR[isite],
+                    dag_cv_isite,
+                    self.a_oper[isite - 1], cv_isite,
+                    self.h_mpo[isite - 1]))
+                third_LR[isite - 1] = asnumpy(multi_tensor_contract(
+                    path1, third_LR[isite], self.h_mpo[isite - 1],
+                    dag_cv_isite,
+                    cv_isite, self.h_mpo[isite - 1]))
+                forth_LR[isite - 1] = asnumpy(multi_tensor_contract(
+                    path2, forth_LR[isite],
+                    moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
+                    cv_isite))
+
+        else:
+            for isite in range(1, len(self.cv_mpo)):
+                cv_isite = self.cv_mpo[isite-1]
+                dag_cv_isite = moveaxis(cv_isite, (1, 2), (2, 1))
+                path1 = [([0, 1], "abcd, aefg -> bcdefg"),
+                         ([3, 0], "bcdefg, bfhi -> cdeghi"),
+                         ([2, 0], "cdeghi, chjk -> degijk"),
+                         ([1, 0], "degijk, djel -> gikl")]
+                path2 = [([0, 1], "ab, acde->bcde"),
+                         ([1, 0], "bcde, bdcf->ef")]
+                first_LR[isite] = asnumpy(multi_tensor_contract(
+                    path1, first_LR[isite - 1],
+                    dag_cv_isite, self.a_oper[isite - 1],
+                    self.a_oper[isite - 1], cv_isite))
+                second_LR[isite] = asnumpy(multi_tensor_contract(
+                    path1, second_LR[isite - 1],
+                    dag_cv_isite,
+                    self.a_oper[isite - 1], cv_isite,
+                    self.h_mpo[isite - 1]))
+                third_LR[isite] = asnumpy(multi_tensor_contract(
+                    path1, third_LR[isite - 1], self.h_mpo[isite - 1],
+                    dag_cv_isite,
+                    cv_isite, self.h_mpo[isite - 1]))
+                forth_LR[isite] = asnumpy(multi_tensor_contract(
+                    path2, forth_LR[isite - 1],
+                    moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
+                    cv_isite))
+        return [first_LR, second_LR, third_LR, forth_LR]
+
+    def update_LR(self, lr_group, isite):
+        first_LR, second_LR, third_LR, forth_LR = lr_group
+        cv_isite = self.cv_mpo[isite-1]
+        dag_cv_isite = moveaxis(cv_isite, (1, 2), (2, 1))
+        if self.method == "1site":
+            if not self.cv_mpo.to_right:
+                path1 = [([0, 1], "abcd, efga -> bcdefg"),
+                         ([3, 0], "bcdefg, hgib -> cdefhi"),
+                         ([2, 0], "cdefhi, jikc -> defhjk"),
+                         ([1, 0], "defhjk, lkfd -> ehjl")]
+                path2 = [([0, 1], "ab, cdea->bcde"),
+                         ([1, 0], "bcde, fedb->cf")]
+                first_LR[isite - 1] = multi_tensor_contract(
+                    path1, first_LR[isite],
+                    dag_cv_isite, self.a_oper[isite - 1],
+                    self.a_oper[isite - 1], cv_isite)
+                second_LR[isite - 1] = multi_tensor_contract(
+                    path1, second_LR[isite],
+                    dag_cv_isite,
+                    self.a_oper[isite - 1], cv_isite,
+                    self.h_mpo[isite - 1])
+                third_LR[isite - 1] = multi_tensor_contract(
+                    path1, third_LR[isite], self.h_mpo[isite - 1],
+                    dag_cv_isite,
+                    cv_isite, self.h_mpo[isite - 1])
+                forth_LR[isite - 1] = multi_tensor_contract(
+                    path2, forth_LR[isite],
+                    moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
+                    cv_isite)
+
+            else:
+                path1 = [([0, 1], "abcd, aefg -> bcdefg"),
+                         ([3, 0], "bcdefg, bfhi -> cdeghi"),
+                         ([2, 0], "cdeghi, chjk -> degijk"),
+                         ([1, 0], "degijk, djel -> gikl")]
+                path2 = [([0, 1], "ab, acde->bcde"),
+                         ([1, 0], "bcde, bdcf->ef")]
+
+                first_LR[isite] = multi_tensor_contract(
+                    path1, first_LR[isite - 1],
+                    dag_cv_isite,
+                    self.a_oper[isite - 1], self.a_oper[isite - 1], cv_isite)
+
+                second_LR[isite] = multi_tensor_contract(
+                    path1, second_LR[isite - 1],
+                    dag_cv_isite,
+                    self.a_oper[isite - 1], cv_isite,
+                    self.h_mpo[isite - 1])
+                third_LR[isite] = multi_tensor_contract(
+                    path1, third_LR[isite - 1], self.h_mpo[isite - 1],
+                    dag_cv_isite,
+                    cv_isite, self.h_mpo[isite - 1])
+                forth_LR[isite] = multi_tensor_contract(
+                    path2, forth_LR[isite - 1],
+                    moveaxis(self.b_mpo[isite - 1], (1, 2), (2, 1)),
+                    cv_isite)
+        else:
+            # 2site for finite temperature is too expensive, so I drop it
+            # (at least for now)
+            raise NotImplementedError
+
+        return first_LR, second_LR, third_LR, forth_LR
```

### Comparing `renormalizer-0.0.8/renormalizer/cv/spectra_cv.py` & `renormalizer-0.0.9/renormalizer/cv/spectra_cv.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/cv/tests/test_H_chain.py` & `renormalizer-0.0.9/renormalizer/cv/tests/test_H_chain.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/cv/tests/test_abs.py` & `renormalizer-0.0.9/renormalizer/cv/tests/test_abs.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/cv/tests/test_emi.py` & `renormalizer-0.0.9/renormalizer/cv/tests/test_emi.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/cv/zerot.py` & `renormalizer-0.0.9/renormalizer/cv/zerot.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/lib/bipartite_matching/bipartite_matching.py` & `renormalizer-0.0.9/renormalizer/lib/bipartite_matching/bipartite_matching.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/base.py` & `renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/base.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/common.py` & `renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/common.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/ivp.py` & `renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/ivp.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/lib/integrate/_ivp/rk.py` & `renormalizer-0.0.9/renormalizer/lib/integrate/_ivp/rk.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/lib/krylov/krylov.py` & `renormalizer-0.0.9/renormalizer/lib/krylov/krylov.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/model/basis.py` & `renormalizer-0.0.9/renormalizer/model/basis.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,17 @@
                 mat = np.zeros((1,1))
             else:
                 mat = np.diag(np.sqrt(np.arange(1, self.nbas - 1) * np.arange(2, self.nbas)), k=-2)
 
         elif op_symbol == r"b^\dagger+b":
             mat = self.op_mat(r"b^\dagger") + self.op_mat("b")
 
+        elif op_symbol == r"b^\dagger-b":
+            mat = self.op_mat(r"b^\dagger") - self.op_mat("b")
+
         elif op_symbol == r"b^\dagger b":
             # b^dagger b = n delta(n,n)
             mat = np.diag(np.arange(self.nbas))
 
         elif op_symbol == r"b b^\dagger":
             mat = np.diag(np.arange(self.nbas) + 1)
```

### Comparing `renormalizer-0.0.8/renormalizer/model/h_qc.py` & `renormalizer-0.0.9/renormalizer/model/h_qc.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/model/model.py` & `renormalizer-0.0.9/renormalizer/model/model.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,517 +1,517 @@
-# -*- coding: utf-8 -*-
-# Author: Jiajun Ren <jiajunren0522@gmail.com>
-
-import logging
-from typing import List, Union, Dict, Callable
-
-import numpy as np
-
-from renormalizer.model.basis import BasisSet, BasisSimpleElectron, BasisMultiElectronVac, BasisHalfSpin, BasisSHO
-from renormalizer.model.mol import Mol, Phonon
-from renormalizer.model.op import Op
-from renormalizer.utils import Quantity, cached_property
-
-
-logger = logging.getLogger(__name__)
-
-class Model:
-    r"""
-    The most general model that supports any Hamiltonian in sum-of-product form.
-    Base class for :class:`HolsteinModel` and :class:`SpinBosonModel`.
-
-    Parameters
-    ==========
-    basis : :class:`list` of :class:`~renormalizer.model.basis.BasisSet`
-        Local basis for each site of the MPS. The order determines the
-        DoF order in the MPS.
-    ham_terms : :class:`list` of :class:`~renormalizer.model.Op`
-        Terms of the system Hamiltonian in sum-of-product form.
-        Identities can be omitted in the operators.
-        All terms must be included, without assuming Hermitian or something else.
-    dipole : dict
-        Contains the transition dipole matrix element. The key is the dof name.
-    output_ordering : :class:`list` of :class:`~renormalizer.model.basis.BasisSet`
-        The ordering of the local basis for output. Default is the same with ``basis``.
-    """
-    def __init__(self, basis: List[BasisSet], ham_terms: List[Op], dipole: Dict = None, output_ordering: List[BasisSet]=None):
-        if not isinstance(basis, list) or len(basis) == 0:
-            raise TypeError("Basis should be a non-empty list")
-        if not isinstance(basis[0], BasisSet):
-            raise TypeError("Elements of the basis list should be of type BasisSet")
-        all_dof_list = []
-        for local_basis in basis:
-                all_dof_list.extend(local_basis.dofs)
-        if len(all_dof_list) != len(set(all_dof_list)):
-            raise ValueError("Duplicate DoF definition found in the basis list.")
-        self.basis: List[BasisSet] = basis
-        qn_size_list = [b.sigmaqn.shape[1] for b in basis]
-        if len(set(qn_size_list)) != 1:
-            raise ValueError(f"Inconsistent quantum number size: {set(qn_size_list)}")
-        self.qn_size: int = qn_size_list[0]
-        if output_ordering is None:
-            self.output_ordering = self.basis
-        else:
-            self.output_ordering = output_ordering
-
-        # alias
-        self.dof_to_siteidx = self.order = {}
-        self.dof_to_basis = {}
-        for siteidx, ba in enumerate(basis):
-            for dof_name in ba.dofs:
-                self.dof_to_siteidx[dof_name] = siteidx
-                self.dof_to_basis[dof_name] = ba
-
-        self.ham_terms: List[Op] = self.check_operator_terms(ham_terms)
-        # array(n_e, n_e)
-        self.dipole = dipole
-        # reusable mpos for the system
-        self.mpos = dict()
-        # physical bond dimension.
-        self.pbond_list = [local_basis.nbas for local_basis in self.basis]
-
-    def check_operator_terms(self, terms: List[Op]):
-        """
-        Check and clean operator terms in the input ``terms``.
-        Errors will be raised if the type of operator is not :class:`Op`
-        or the operator contains DoF not defined in ``self.basis``.
-        Operators with factor = 0 are discarded.
-
-        Parameters
-        ----------
-        terms : :class:`list` of :class:`~renormalizer.model.Op`
-            The terms to check.
-
-        Returns
-        -------
-        new_terms: :class:`list` of :class:`Op`
-            Operator list with 0-factor terms discarded.
-        """
-        # terms to return
-        new_terms = []
-        dofs = set(self.dofs)
-        for term_op in terms:
-            if not isinstance(term_op, Op):
-                raise ValueError(f"Expected Op in terms. Got {term_op}")
-            for name in term_op.dofs:
-                if name not in dofs:
-                    raise ValueError(f"{term_op} contains DoF not in the basis.")
-            # discard terms with 0 factor
-            if term_op.factor == 0:
-                continue
-            new_terms.append(term_op)
-        return new_terms
-
-    def _enumerate_dof(self, criteria=lambda x: True):
-        # enumerate DoFs and filter according to criteria.
-        dofs = []
-        for local_basis in self.output_ordering:
-            if criteria(local_basis):
-                dofs.extend(local_basis.dofs)
-        return dofs
-
-    @cached_property
-    def dofs(self) -> List:
-        """
-        :class:`list` of DoF names.
-        """
-        return self._enumerate_dof()
-    
-    @cached_property
-    def nsite(self) -> int:
-        """
-        Number of sites in the MPS/MPO to be constructed.
-        Length of ``self.basis``.
-        """
-        return len(self.basis)
-
-    @cached_property
-    def e_dofs(self) -> List:
-        """
-        :class:`list` of electronic DoF names.
-        """
-        return self._enumerate_dof(lambda basis: basis.is_electron)
-    
-    @cached_property
-    def v_dofs(self) -> List:
-        """
-        :class:`list` of vibrational DoF names.
-        """
-        return self._enumerate_dof(lambda basis: basis.is_phonon)
-
-    @cached_property
-    def n_dofs(self) -> int:
-        """
-        Number of total DoFs.
-        """
-        return len(self.dofs)
-
-    @cached_property
-    def n_edofs(self) -> int:
-        """
-        Number of total electronic DoFs.
-        """
-        return len(self.e_dofs)
-    
-    @cached_property
-    def n_vdofs(self) -> int:
-        """
-        Number of total vibrational DoFs.
-        """
-        return len(self.v_dofs)
-
-    def get_mpos(self, key: str, fun: Callable):
-        r"""
-        Get MPOs related to the model, such as MPOs to calculate
-        electronic occupations :math:`{a^\dagger_i a_i}`.
-        The purpose of the function is to avoid repeated MPO construction.
-
-        Parameters
-        ----------
-        key : str
-            Name of the MPOs. In principle other hashable types are also OK.
-        fun : callable
-            The function to generate MPOs if the MPOs have not been
-            constructed before. The function should accept only one argument
-            which is the model and return a :class:`list` of
-            :class:`~renormalizer.mps.Mpo`.
-
-        Returns
-        -------
-        mpos : list of :class:`~renormalizer.mps.Mpo`
-            The required MPOs.
-        """
-        if key not in self.mpos:
-            mpos = fun(self)
-            self.mpos[key] = mpos
-        else:
-            mpos = self.mpos[key]
-        return mpos
-
-    def copy(self):
-        # copy basis because it is mutable with OFS
-        model =  Model(self.basis.copy(), self.ham_terms, self.dipole, self.output_ordering)
-        # this is a shallow copy, in order to avoid infinite recursion
-        model.mpos = self.mpos.copy()
-        return model
-
-    def to_dict(self) -> Dict:
-        """
-        Convert the object into a dict that contains only objects of
-        Python primitive types or NumPy types.
-        This is primarily for dump purposes.
-
-        Returns
-        -------
-        info_dict : dict
-            The information of the model in a dict.
-        """
-        info_dict = {}
-        # todo: dump basis
-        info_dict["Hamiltonian"] = [op.to_tuple() for op in self.ham_terms]
-        info_dict["dipole"] = self.dipole
-        return info_dict
-
-
-class HolsteinModel(Model):
-    r"""
-    Interface for convenient Holstein model construction.
-    The Hamiltonian of the Holstein model:
-
-    .. math::
-        \hat H = \sum_{ij} J_{ij} a^\dagger_i a_j + \sum_{i\lambda} \omega_{i\lambda} b^\dagger_{i\lambda} b_{i\lambda}
-        + \sum_{i\lambda} g_{i\lambda} \omega_{i\lambda} a^\dagger_i a_i (b^\dagger_{i\lambda} + b_{i\lambda})
-
-    Parameters
-    ==========
-    mol_list : :class:`list` of :class:`~renormalizer.model.Mol`
-        Information for the molecules contains in the system.
-        See the :class:`~renormalizer.model.Mol` class for more details.
-    j_matrix : :class:`np.ndarray` or :class:`~renormalizer.utils.Quantity`.
-        :math:`J_{ij}` in the Holstein Hamiltonian. When :class:`Quantity` is used as input, the system is taken to
-        have homogeneous nearest-neighbour interaction
-        :math:`J_{ij}=J \delta_{i, j+1} + J \delta_{i, j-1}`.
-        For the boundary condition, see the ``periodic`` option.
-    scheme : int
-        The scheme of the basis for the model. Historically four numbers are permitted: 1, 2, 3, 4.
-        Now 1, 2 and 3 are equivalent, and the bases are arranged as:
-
-        .. math::
-            [\rm{e}_{0}, \rm{ph}_{0,0}, \rm{ph}_{0,1}, \cdots, \rm{e}_{1}, \rm{ph}_{1,0}, \rm{ph}_{1,1}, \cdots ]
-
-        And when ``scheme`` is set to 4, all electronic DoF is contained in one
-        :class:`~renormalizer.model.basis.BasisSet`
-        using :class:`~renormalizer.model.basis.BasisMultiElectronVac` and the bases are arranged as:
-
-        .. math::
-            [\rm{ph}_{0,0},  \rm{ph}_{0,1}, \cdots, \rm{ph}_{n/2, 0}, \rm{ph}_{n/2, 1}, \cdots, \rm{e}_{0, 1, \cdots, n}
-            \rm{ph}_{n/2+1, 0}, \rm{ph}_{n/2+1, 1}, \cdots]
-
-    periodic : bool
-        Whether use periodical boundary condition when constructing ``j_matrix``
-        from :class:`~renormalizer.utils.Quantity`. Default is ``False``.
-    """
-
-    def __init__(self,  mol_list: List[Mol], j_matrix: Union[Quantity, np.ndarray], scheme: int = 2, periodic: bool = False):
-        # construct the electronic coupling matrix
-
-        mol_num = len(mol_list)
-        self.mol_list = mol_list
-
-        if isinstance(j_matrix, Quantity):
-            j_matrix = construct_j_matrix(mol_num, j_matrix, periodic)
-        else:
-            if periodic:
-                assert j_matrix[0][-1] != 0 and j_matrix[-1][0] != 0
-            assert j_matrix.shape[0] == mol_num
-
-        self.j_matrix = j_matrix
-        self.scheme = scheme
-
-        basis = []
-        ham = []
-
-        if scheme < 4:
-            for imol, mol in enumerate(mol_list):
-                basis.append(BasisSimpleElectron(imol))
-                for iph, ph in enumerate(mol.ph_list):
-                    basis.append(BasisSHO((imol, iph), ph.omega[0], ph.n_phys_dim))
-
-        elif scheme == 4:
-
-            n_left_mol = mol_num // 2
-
-            n_left_ph = 0
-            for imol, mol in enumerate(mol_list):
-                for iph, ph in enumerate(mol.ph_list):
-                    if imol < n_left_mol:
-                        n_left_ph += 1
-                    basis.append(BasisSHO((imol, iph), ph.omega[0], ph.n_phys_dim))
-
-            basis.insert(n_left_ph, BasisMultiElectronVac(list(range(len(mol_list)))))
-
-        else:
-            raise ValueError(f"invalid model.scheme: {scheme}")
-
-        # model
-
-        # electronic term
-        for imol in range(mol_num):
-            for jmol in range(mol_num):
-                if imol == jmol:
-                    factor =  mol_list[imol].elocalex + mol_list[imol].e0
-                else:
-                    factor = j_matrix[imol, jmol]
-                ham_term = Op(r"a^\dagger a", [imol, jmol], factor)
-                ham.append(ham_term)
-        # vibration part
-        for imol, mol in enumerate(mol_list):
-            for iph, ph in enumerate(mol.ph_list):
-
-                ham.extend([
-                    Op("p^2", (imol, iph), 0.5),
-                    Op("x^2", (imol, iph), 0.5 * ph.omega[0] ** 2)
-                ])
-
-        # vibration potential part
-        for imol, mol in enumerate(mol_list):
-            for iph, ph in enumerate(mol.ph_list):
-                if np.allclose(ph.omega[0], ph.omega[1]):
-                    ham.append(
-                        Op(r"a^\dagger a", imol) * Op("x", (imol,iph)) * (-ph.omega[1] ** 2 * ph.dis[1])
-                    )
-                else:
-                    ham.extend([
-                        Op(r"a^\dagger a", imol) * Op("x^2", (imol, iph)) * (0.5 * (ph.omega[1] ** 2 - ph.omega[0] ** 2)),
-                        Op(r"a^\dagger a", imol) * Op("x", (imol, iph)) * (-ph.omega[1] ** 2 * ph.dis[1]),
-                    ])
-
-
-        dipole = {}
-        for imol, mol in enumerate(mol_list):
-            dipole[imol] = mol.dipole
-
-        super().__init__(basis, ham, dipole=dipole)
-        self.mol_num = self.n_edofs
-
-    def switch_scheme(self, scheme: int) -> "HolsteinModel":
-        """
-        Switch the scheme of the current model.
-
-        Parameters
-        ----------
-        scheme : int
-            The target scheme.
-
-        Returns
-        -------
-        new_model : HolsteinModel
-            The new model with the specified scheme.
-        """
-        return HolsteinModel(self.mol_list, self.j_matrix, scheme)
-
-    @property
-    def gs_zpe(self) -> float:
-        r"""
-        Ground state zero-point energy :math:`\sum_{i, j} \frac{1}{2}\omega_{i, j}`.
-        """
-        return sum([mol.gs_zpe for mol in self.mol_list])
-
-    @property
-    def j_constant(self):
-        """Extract electronic coupling constant from ``self.j_matrix``.
-        Useful in transport model when :math:`J` is a constant..
-        If J is actually not a constant, a value error will be raised.
-
-        Returns
-        -------
-        j constant: float
-            J constant extracted from ``self.j_matrix``.
-        """
-        j_set = set(self.j_matrix.ravel())
-        if len(j_set) == 0:
-            return j_set.pop()
-        elif len(j_set) == 2 and 0 in j_set:
-            j_set.remove(0)
-            return j_set.pop()
-        else:
-            raise ValueError("J is not constant")
-
-    def copy(self):
-        model = HolsteinModel(self.mol_list, self.j_matrix, self.scheme)
-        model.mpos = self.mpos.copy()
-        return model
-
-    def __getitem__(self, item):
-        return self.mol_list[item]
-
-    def __iter__(self):
-        return iter(self.mol_list)
-
-    def __len__(self):
-        return len(self.mol_list)
-
-
-class SpinBosonModel(Model):
-    r"""
-    Spin-Boson model
-
-        .. math::
-            \hat{H} = \epsilon \sigma_z + \Delta \sigma_x
-                + \frac{1}{2} \sum_i(p_i^2+\omega^2_i q_i^2)
-                + \sigma_z \sum_i c_i q_i
-
-    """
-    def __init__(self, epsilon: Quantity, delta: Quantity, ph_list: List[Phonon], dipole: float=None):
-
-        self.epsilon = epsilon.as_au()
-        self.delta = delta.as_au()
-        self.ph_list = ph_list
-
-        basis = [BasisHalfSpin("spin")]
-        for iph, ph in enumerate(ph_list):
-            basis.append(BasisSHO(iph, ph.omega[0], ph.n_phys_dim))
-
-        # spin
-        ham = [Op(r"sigma_z", "spin", self.epsilon), Op("sigma_x", "spin", self.delta)]
-        # vibration energy and potential
-        for iph, ph in enumerate(ph_list):
-            assert ph.is_simple
-            ham.extend([Op("p^2", iph, 0.5), Op("x^2", iph, 0.5 * ph.omega[0] ** 2)])
-            ham.append(Op("sigma_z", "spin") * Op("x", iph) *(-ph.omega[1] ** 2 * ph.dis[1]))
-        if dipole is None:
-            dipole = 0
-        super().__init__(basis, ham, dipole={"spin": dipole})
-
-
-class TI1DModel(Model):
-    r"""
-    Translational invariant one dimensional model with periodic boundary condition.
-    The Hamiltonian should take the form:
-
-    .. math::
-        \hat H = \sum_i(\hat h_i + \sum_j \hat h_{i,j})
-
-    where :math:`\hat h_i` is the local Hamiltonian acting on one single unit cell
-    and :math:`\hat h_{i,j}` represents the :math:`j` th interaction between the :math:`i` th cell
-    and other unit cells.
-
-    Yet doesn't support setting transition dipoles.
-
-    Parameters
-    ==========
-    basis : :class:`list` of :class:`~renormalizer.model.basis.BasisSet`
-        Local basis of each site for a single unit cell of the system.
-        The full basis set is constructed by repeating the basis ``ncell`` times.
-        To distinguish between different DoFs at different unit cells,
-        the DoF names in the unit cell are transformed to
-        a two-element-tuple of the form ``("cell0", dof)``, where ``dof`` is the original DoF name
-        and the ``"cell0"`` indicates the cell ID.
-    local_ham_terms : :class:`list` of :class:`~renormalizer.model.Op`
-        Terms of the system local Hamiltonian :math:`\hat h_i` in sum-of-product form.
-        DoF names should be consistent with the ``basis`` argument.
-    nonlocal_ham_terms : :class:`list` of :class:`~renormalizer.model.Op`
-        Terms of system nonlocal Hamiltonian :math:`\hat h_{i,j}`.
-        To indicate the IDs of the unit cells that are involved in the nonlocal interaction,
-        the DoF name in ``basis`` should be transformed to a two-element-tuple, in which
-        the first element is an integer indicating its distance from :math:`i`,
-        and the second element is the original DoF name.
-        For example, if one unit cell contains one electron DoF with name ``e``,
-        a nearest neighbour hopping interaction
-        should take the form ``Op(r"a^\dagger a", [(0, "e"), (1, "e")])``
-        (with its Hermite conjugation being another term).
-        The definition is not unique in that ``Op(r"a^\dagger a", [(1, "e"), (2, "e")])``
-        produces equivalent output.
-    ncell : int
-        Number of unit cells in the system.
-    """
-    def __init__(self, basis: List[BasisSet], local_ham_terms: List[Op], nonlocal_ham_terms: List[Op], ncell: int):
-        # construct basis for the full model
-        full_basis = []
-        for i in range(ncell):
-            for local_basis in basis:
-                new_dofs = [(f"cell{i}", dof) for dof in local_basis.dofs]
-                if local_basis.multi_dof:
-                    new_basis = local_basis.copy(new_dofs)
-                else:
-                    new_basis = local_basis.copy(new_dofs[0])
-                full_basis.append(new_basis)
-        # construct Hamiltonian for the full model
-        full_ham_terms = []
-        for i in range(ncell):
-            for old_op in local_ham_terms:
-                new_dofs = [(f"cell{i}", dof) for dof in old_op.dofs]
-                new_op = Op(old_op.symbol, new_dofs, old_op.factor, old_op.qn_list)
-                full_ham_terms.append(new_op)
-            for old_op in nonlocal_ham_terms:
-                new_dofs = []
-                for old_dof in old_op.dofs:
-                    assert isinstance(old_dof, tuple) and len(old_dof) == 2 and isinstance(old_dof[0], int)
-                    # take care of periodic boundary condition
-                    new_cell_id = (i + old_dof[0]) % ncell
-                    new_dofs.append((f"cell{new_cell_id}", old_dof[1]))
-                new_op = Op(old_op.symbol, new_dofs, old_op.factor, old_op.qn_list)
-                full_ham_terms.append(new_op)
-        super().__init__(full_basis, full_ham_terms)
-
-
-def construct_j_matrix(mol_num, j_constant, periodic):
-    # nearest neighbour interaction
-    j_constant_au = j_constant.as_au()
-    j_list = np.ones(mol_num - 1) * j_constant_au
-    j_matrix = np.diag(j_list, k=-1) + np.diag(j_list, k=1)
-    if periodic:
-        j_matrix[-1, 0] = j_matrix[0, -1] = j_constant_au
-    return j_matrix
-
-
-def load_from_dict(param, scheme, lam: bool):
-    temperature = Quantity(*param["temperature"])
-    ph_list = [
-        Phonon.simplest_phonon(
-            Quantity(*omega), Quantity(*displacement), temperature=temperature, lam=lam
-        )
-        for omega, displacement in param["ph modes"]
-    ]
-    j_constant = Quantity(*param["j constant"])
-    model = HolsteinModel([Mol(Quantity(0), ph_list)] * param["mol num"], j_constant, scheme)
-    return model, temperature
+# -*- coding: utf-8 -*-
+# Author: Jiajun Ren <jiajunren0522@gmail.com>
+
+import logging
+from typing import List, Union, Dict, Callable
+
+import numpy as np
+
+from renormalizer.model.basis import BasisSet, BasisSimpleElectron, BasisMultiElectronVac, BasisHalfSpin, BasisSHO
+from renormalizer.model.mol import Mol, Phonon
+from renormalizer.model.op import Op
+from renormalizer.utils import Quantity, cached_property
+
+
+logger = logging.getLogger(__name__)
+
+class Model:
+    r"""
+    The most general model that supports any Hamiltonian in sum-of-product form.
+    Base class for :class:`HolsteinModel` and :class:`SpinBosonModel`.
+
+    Parameters
+    ==========
+    basis : :class:`list` of :class:`~renormalizer.model.basis.BasisSet`
+        Local basis for each site of the MPS. The order determines the
+        DoF order in the MPS.
+    ham_terms : :class:`list` of :class:`~renormalizer.model.Op`
+        Terms of the system Hamiltonian in sum-of-product form.
+        Identities can be omitted in the operators.
+        All terms must be included, without assuming Hermitian or something else.
+    dipole : dict
+        Contains the transition dipole matrix element. The key is the dof name.
+    output_ordering : :class:`list` of :class:`~renormalizer.model.basis.BasisSet`
+        The ordering of the local basis for output. Default is the same with ``basis``.
+    """
+    def __init__(self, basis: List[BasisSet], ham_terms: List[Op], dipole: Dict = None, output_ordering: List[BasisSet]=None):
+        if not isinstance(basis, list) or len(basis) == 0:
+            raise TypeError("Basis should be a non-empty list")
+        if not isinstance(basis[0], BasisSet):
+            raise TypeError("Elements of the basis list should be of type BasisSet")
+        all_dof_list = []
+        for local_basis in basis:
+                all_dof_list.extend(local_basis.dofs)
+        if len(all_dof_list) != len(set(all_dof_list)):
+            raise ValueError("Duplicate DoF definition found in the basis list.")
+        self.basis: List[BasisSet] = basis
+        qn_size_list = [b.sigmaqn.shape[1] for b in basis]
+        if len(set(qn_size_list)) != 1:
+            raise ValueError(f"Inconsistent quantum number size: {set(qn_size_list)}")
+        self.qn_size: int = qn_size_list[0]
+        if output_ordering is None:
+            self.output_ordering = self.basis
+        else:
+            self.output_ordering = output_ordering
+
+        # alias
+        self.dof_to_siteidx = self.order = {}
+        self.dof_to_basis = {}
+        for siteidx, ba in enumerate(basis):
+            for dof_name in ba.dofs:
+                self.dof_to_siteidx[dof_name] = siteidx
+                self.dof_to_basis[dof_name] = ba
+
+        self.ham_terms: List[Op] = self.check_operator_terms(ham_terms)
+        # array(n_e, n_e)
+        self.dipole = dipole
+        # reusable mpos for the system
+        self.mpos = dict()
+        # physical bond dimension.
+        self.pbond_list = [local_basis.nbas for local_basis in self.basis]
+
+    def check_operator_terms(self, terms: List[Op]):
+        """
+        Check and clean operator terms in the input ``terms``.
+        Errors will be raised if the type of operator is not :class:`Op`
+        or the operator contains DoF not defined in ``self.basis``.
+        Operators with factor = 0 are discarded.
+
+        Parameters
+        ----------
+        terms : :class:`list` of :class:`~renormalizer.model.Op`
+            The terms to check.
+
+        Returns
+        -------
+        new_terms: :class:`list` of :class:`Op`
+            Operator list with 0-factor terms discarded.
+        """
+        # terms to return
+        new_terms = []
+        dofs = set(self.dofs)
+        for term_op in terms:
+            if not isinstance(term_op, Op):
+                raise ValueError(f"Expected Op in terms. Got {term_op}")
+            for name in term_op.dofs:
+                if name not in dofs:
+                    raise ValueError(f"{term_op} contains DoF not in the basis.")
+            # discard terms with 0 factor
+            if term_op.factor == 0:
+                continue
+            new_terms.append(term_op)
+        return new_terms
+
+    def _enumerate_dof(self, criteria=lambda x: True):
+        # enumerate DoFs and filter according to criteria.
+        dofs = []
+        for local_basis in self.output_ordering:
+            if criteria(local_basis):
+                dofs.extend(local_basis.dofs)
+        return dofs
+
+    @cached_property
+    def dofs(self) -> List:
+        """
+        :class:`list` of DoF names.
+        """
+        return self._enumerate_dof()
+    
+    @cached_property
+    def nsite(self) -> int:
+        """
+        Number of sites in the MPS/MPO to be constructed.
+        Length of ``self.basis``.
+        """
+        return len(self.basis)
+
+    @cached_property
+    def e_dofs(self) -> List:
+        """
+        :class:`list` of electronic DoF names.
+        """
+        return self._enumerate_dof(lambda basis: basis.is_electron)
+    
+    @cached_property
+    def v_dofs(self) -> List:
+        """
+        :class:`list` of vibrational DoF names.
+        """
+        return self._enumerate_dof(lambda basis: basis.is_phonon)
+
+    @cached_property
+    def n_dofs(self) -> int:
+        """
+        Number of total DoFs.
+        """
+        return len(self.dofs)
+
+    @cached_property
+    def n_edofs(self) -> int:
+        """
+        Number of total electronic DoFs.
+        """
+        return len(self.e_dofs)
+    
+    @cached_property
+    def n_vdofs(self) -> int:
+        """
+        Number of total vibrational DoFs.
+        """
+        return len(self.v_dofs)
+
+    def get_mpos(self, key: str, fun: Callable):
+        r"""
+        Get MPOs related to the model, such as MPOs to calculate
+        electronic occupations :math:`{a^\dagger_i a_i}`.
+        The purpose of the function is to avoid repeated MPO construction.
+
+        Parameters
+        ----------
+        key : str
+            Name of the MPOs. In principle other hashable types are also OK.
+        fun : callable
+            The function to generate MPOs if the MPOs have not been
+            constructed before. The function should accept only one argument
+            which is the model and return a :class:`list` of
+            :class:`~renormalizer.mps.Mpo`.
+
+        Returns
+        -------
+        mpos : list of :class:`~renormalizer.mps.Mpo`
+            The required MPOs.
+        """
+        if key not in self.mpos:
+            mpos = fun(self)
+            self.mpos[key] = mpos
+        else:
+            mpos = self.mpos[key]
+        return mpos
+
+    def copy(self):
+        # copy basis because it is mutable with OFS
+        model =  Model(self.basis.copy(), self.ham_terms, self.dipole, self.output_ordering)
+        # this is a shallow copy, in order to avoid infinite recursion
+        model.mpos = self.mpos.copy()
+        return model
+
+    def to_dict(self) -> Dict:
+        """
+        Convert the object into a dict that contains only objects of
+        Python primitive types or NumPy types.
+        This is primarily for dump purposes.
+
+        Returns
+        -------
+        info_dict : dict
+            The information of the model in a dict.
+        """
+        info_dict = {}
+        # todo: dump basis
+        info_dict["Hamiltonian"] = [op.to_tuple() for op in self.ham_terms]
+        info_dict["dipole"] = self.dipole
+        return info_dict
+
+
+class HolsteinModel(Model):
+    r"""
+    Interface for convenient Holstein model construction.
+    The Hamiltonian of the Holstein model:
+
+    .. math::
+        \hat H = \sum_{ij} J_{ij} a^\dagger_i a_j + \sum_{i\lambda} \omega_{i\lambda} b^\dagger_{i\lambda} b_{i\lambda}
+        + \sum_{i\lambda} g_{i\lambda} \omega_{i\lambda} a^\dagger_i a_i (b^\dagger_{i\lambda} + b_{i\lambda})
+
+    Parameters
+    ==========
+    mol_list : :class:`list` of :class:`~renormalizer.model.Mol`
+        Information for the molecules contains in the system.
+        See the :class:`~renormalizer.model.Mol` class for more details.
+    j_matrix : :class:`np.ndarray` or :class:`~renormalizer.utils.Quantity`.
+        :math:`J_{ij}` in the Holstein Hamiltonian. When :class:`Quantity` is used as input, the system is taken to
+        have homogeneous nearest-neighbour interaction
+        :math:`J_{ij}=J \delta_{i, j+1} + J \delta_{i, j-1}`.
+        For the boundary condition, see the ``periodic`` option.
+    scheme : int
+        The scheme of the basis for the model. Historically four numbers are permitted: 1, 2, 3, 4.
+        Now 1, 2 and 3 are equivalent, and the bases are arranged as:
+
+        .. math::
+            [\rm{e}_{0}, \rm{ph}_{0,0}, \rm{ph}_{0,1}, \cdots, \rm{e}_{1}, \rm{ph}_{1,0}, \rm{ph}_{1,1}, \cdots ]
+
+        And when ``scheme`` is set to 4, all electronic DoF is contained in one
+        :class:`~renormalizer.model.basis.BasisSet`
+        using :class:`~renormalizer.model.basis.BasisMultiElectronVac` and the bases are arranged as:
+
+        .. math::
+            [\rm{ph}_{0,0},  \rm{ph}_{0,1}, \cdots, \rm{ph}_{n/2, 0}, \rm{ph}_{n/2, 1}, \cdots, \rm{e}_{0, 1, \cdots, n}
+            \rm{ph}_{n/2+1, 0}, \rm{ph}_{n/2+1, 1}, \cdots]
+
+    periodic : bool
+        Whether use periodical boundary condition when constructing ``j_matrix``
+        from :class:`~renormalizer.utils.Quantity`. Default is ``False``.
+    """
+
+    def __init__(self,  mol_list: List[Mol], j_matrix: Union[Quantity, np.ndarray], scheme: int = 2, periodic: bool = False):
+        # construct the electronic coupling matrix
+
+        mol_num = len(mol_list)
+        self.mol_list = mol_list
+
+        if isinstance(j_matrix, Quantity):
+            j_matrix = construct_j_matrix(mol_num, j_matrix, periodic)
+        else:
+            if periodic:
+                assert j_matrix[0][-1] != 0 and j_matrix[-1][0] != 0
+            assert j_matrix.shape[0] == mol_num
+
+        self.j_matrix = j_matrix
+        self.scheme = scheme
+
+        basis = []
+        ham = []
+
+        if scheme < 4:
+            for imol, mol in enumerate(mol_list):
+                basis.append(BasisSimpleElectron(imol))
+                for iph, ph in enumerate(mol.ph_list):
+                    basis.append(BasisSHO((imol, iph), ph.omega[0], ph.n_phys_dim))
+
+        elif scheme == 4:
+
+            n_left_mol = mol_num // 2
+
+            n_left_ph = 0
+            for imol, mol in enumerate(mol_list):
+                for iph, ph in enumerate(mol.ph_list):
+                    if imol < n_left_mol:
+                        n_left_ph += 1
+                    basis.append(BasisSHO((imol, iph), ph.omega[0], ph.n_phys_dim))
+
+            basis.insert(n_left_ph, BasisMultiElectronVac(list(range(len(mol_list)))))
+
+        else:
+            raise ValueError(f"invalid model.scheme: {scheme}")
+
+        # model
+
+        # electronic term
+        for imol in range(mol_num):
+            for jmol in range(mol_num):
+                if imol == jmol:
+                    factor =  mol_list[imol].elocalex + mol_list[imol].e0
+                else:
+                    factor = j_matrix[imol, jmol]
+                ham_term = Op(r"a^\dagger a", [imol, jmol], factor)
+                ham.append(ham_term)
+        # vibration part
+        for imol, mol in enumerate(mol_list):
+            for iph, ph in enumerate(mol.ph_list):
+
+                ham.extend([
+                    Op("p^2", (imol, iph), 0.5),
+                    Op("x^2", (imol, iph), 0.5 * ph.omega[0] ** 2)
+                ])
+
+        # vibration potential part
+        for imol, mol in enumerate(mol_list):
+            for iph, ph in enumerate(mol.ph_list):
+                if np.allclose(ph.omega[0], ph.omega[1]):
+                    ham.append(
+                        Op(r"a^\dagger a", imol) * Op("x", (imol,iph)) * (-ph.omega[1] ** 2 * ph.dis[1])
+                    )
+                else:
+                    ham.extend([
+                        Op(r"a^\dagger a", imol) * Op("x^2", (imol, iph)) * (0.5 * (ph.omega[1] ** 2 - ph.omega[0] ** 2)),
+                        Op(r"a^\dagger a", imol) * Op("x", (imol, iph)) * (-ph.omega[1] ** 2 * ph.dis[1]),
+                    ])
+
+
+        dipole = {}
+        for imol, mol in enumerate(mol_list):
+            dipole[imol] = mol.dipole
+
+        super().__init__(basis, ham, dipole=dipole)
+        self.mol_num = self.n_edofs
+
+    def switch_scheme(self, scheme: int) -> "HolsteinModel":
+        """
+        Switch the scheme of the current model.
+
+        Parameters
+        ----------
+        scheme : int
+            The target scheme.
+
+        Returns
+        -------
+        new_model : HolsteinModel
+            The new model with the specified scheme.
+        """
+        return HolsteinModel(self.mol_list, self.j_matrix, scheme)
+
+    @property
+    def gs_zpe(self) -> float:
+        r"""
+        Ground state zero-point energy :math:`\sum_{i, j} \frac{1}{2}\omega_{i, j}`.
+        """
+        return sum([mol.gs_zpe for mol in self.mol_list])
+
+    @property
+    def j_constant(self):
+        """Extract electronic coupling constant from ``self.j_matrix``.
+        Useful in transport model when :math:`J` is a constant..
+        If J is actually not a constant, a value error will be raised.
+
+        Returns
+        -------
+        j constant: float
+            J constant extracted from ``self.j_matrix``.
+        """
+        j_set = set(self.j_matrix.ravel())
+        if len(j_set) == 0:
+            return j_set.pop()
+        elif len(j_set) == 2 and 0 in j_set:
+            j_set.remove(0)
+            return j_set.pop()
+        else:
+            raise ValueError("J is not constant")
+
+    def copy(self):
+        model = HolsteinModel(self.mol_list, self.j_matrix, self.scheme)
+        model.mpos = self.mpos.copy()
+        return model
+
+    def __getitem__(self, item):
+        return self.mol_list[item]
+
+    def __iter__(self):
+        return iter(self.mol_list)
+
+    def __len__(self):
+        return len(self.mol_list)
+
+
+class SpinBosonModel(Model):
+    r"""
+    Spin-Boson model
+
+        .. math::
+            \hat{H} = \epsilon \sigma_z + \Delta \sigma_x
+                + \frac{1}{2} \sum_i(p_i^2+\omega^2_i q_i^2)
+                + \sigma_z \sum_i c_i q_i
+
+    """
+    def __init__(self, epsilon: Quantity, delta: Quantity, ph_list: List[Phonon], dipole: float=None):
+
+        self.epsilon = epsilon.as_au()
+        self.delta = delta.as_au()
+        self.ph_list = ph_list
+
+        basis = [BasisHalfSpin("spin")]
+        for iph, ph in enumerate(ph_list):
+            basis.append(BasisSHO(iph, ph.omega[0], ph.n_phys_dim))
+
+        # spin
+        ham = [Op(r"sigma_z", "spin", self.epsilon), Op("sigma_x", "spin", self.delta)]
+        # vibration energy and potential
+        for iph, ph in enumerate(ph_list):
+            assert ph.is_simple
+            ham.extend([Op("p^2", iph, 0.5), Op("x^2", iph, 0.5 * ph.omega[0] ** 2)])
+            ham.append(Op("sigma_z", "spin") * Op("x", iph) *(-ph.omega[1] ** 2 * ph.dis[1]))
+        if dipole is None:
+            dipole = 0
+        super().__init__(basis, ham, dipole={"spin": dipole})
+
+
+class TI1DModel(Model):
+    r"""
+    Translational invariant one dimensional model with periodic boundary condition.
+    The Hamiltonian should take the form:
+
+    .. math::
+        \hat H = \sum_i(\hat h_i + \sum_j \hat h_{i,j})
+
+    where :math:`\hat h_i` is the local Hamiltonian acting on one single unit cell
+    and :math:`\hat h_{i,j}` represents the :math:`j` th interaction between the :math:`i` th cell
+    and other unit cells.
+
+    Yet doesn't support setting transition dipoles.
+
+    Parameters
+    ==========
+    basis : :class:`list` of :class:`~renormalizer.model.basis.BasisSet`
+        Local basis of each site for a single unit cell of the system.
+        The full basis set is constructed by repeating the basis ``ncell`` times.
+        To distinguish between different DoFs at different unit cells,
+        the DoF names in the unit cell are transformed to
+        a two-element-tuple of the form ``("cell0", dof)``, where ``dof`` is the original DoF name
+        and the ``"cell0"`` indicates the cell ID.
+    local_ham_terms : :class:`list` of :class:`~renormalizer.model.Op`
+        Terms of the system local Hamiltonian :math:`\hat h_i` in sum-of-product form.
+        DoF names should be consistent with the ``basis`` argument.
+    nonlocal_ham_terms : :class:`list` of :class:`~renormalizer.model.Op`
+        Terms of system nonlocal Hamiltonian :math:`\hat h_{i,j}`.
+        To indicate the IDs of the unit cells that are involved in the nonlocal interaction,
+        the DoF name in ``basis`` should be transformed to a two-element-tuple, in which
+        the first element is an integer indicating its distance from :math:`i`,
+        and the second element is the original DoF name.
+        For example, if one unit cell contains one electron DoF with name ``e``,
+        a nearest neighbour hopping interaction
+        should take the form ``Op(r"a^\dagger a", [(0, "e"), (1, "e")])``
+        (with its Hermite conjugation being another term).
+        The definition is not unique in that ``Op(r"a^\dagger a", [(1, "e"), (2, "e")])``
+        produces equivalent output.
+    ncell : int
+        Number of unit cells in the system.
+    """
+    def __init__(self, basis: List[BasisSet], local_ham_terms: List[Op], nonlocal_ham_terms: List[Op], ncell: int):
+        # construct basis for the full model
+        full_basis = []
+        for i in range(ncell):
+            for local_basis in basis:
+                new_dofs = [(f"cell{i}", dof) for dof in local_basis.dofs]
+                if local_basis.multi_dof:
+                    new_basis = local_basis.copy(new_dofs)
+                else:
+                    new_basis = local_basis.copy(new_dofs[0])
+                full_basis.append(new_basis)
+        # construct Hamiltonian for the full model
+        full_ham_terms = []
+        for i in range(ncell):
+            for old_op in local_ham_terms:
+                new_dofs = [(f"cell{i}", dof) for dof in old_op.dofs]
+                new_op = Op(old_op.symbol, new_dofs, old_op.factor, old_op.qn_list)
+                full_ham_terms.append(new_op)
+            for old_op in nonlocal_ham_terms:
+                new_dofs = []
+                for old_dof in old_op.dofs:
+                    assert isinstance(old_dof, tuple) and len(old_dof) == 2 and isinstance(old_dof[0], int)
+                    # take care of periodic boundary condition
+                    new_cell_id = (i + old_dof[0]) % ncell
+                    new_dofs.append((f"cell{new_cell_id}", old_dof[1]))
+                new_op = Op(old_op.symbol, new_dofs, old_op.factor, old_op.qn_list)
+                full_ham_terms.append(new_op)
+        super().__init__(full_basis, full_ham_terms)
+
+
+def construct_j_matrix(mol_num, j_constant, periodic):
+    # nearest neighbour interaction
+    j_constant_au = j_constant.as_au()
+    j_list = np.ones(mol_num - 1) * j_constant_au
+    j_matrix = np.diag(j_list, k=-1) + np.diag(j_list, k=1)
+    if periodic:
+        j_matrix[-1, 0] = j_matrix[0, -1] = j_constant_au
+    return j_matrix
+
+
+def load_from_dict(param, scheme, lam: bool):
+    temperature = Quantity(*param["temperature"])
+    ph_list = [
+        Phonon.simplest_phonon(
+            Quantity(*omega), Quantity(*displacement), temperature=temperature, lam=lam
+        )
+        for omega, displacement in param["ph modes"]
+    ]
+    j_constant = Quantity(*param["j constant"])
+    model = HolsteinModel([Mol(Quantity(0), ph_list)] * param["mol num"], j_constant, scheme)
+    return model, temperature
```

### Comparing `renormalizer-0.0.8/renormalizer/model/mol.py` & `renormalizer-0.0.9/renormalizer/model/mol.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/model/op.py` & `renormalizer-0.0.9/renormalizer/model/op.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/model/phonon.py` & `renormalizer-0.0.9/renormalizer/model/phonon.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/backend.py` & `renormalizer-0.0.9/renormalizer/mps/backend.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/gs.py` & `renormalizer-0.0.9/renormalizer/mps/gs.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/hop_expr.py` & `renormalizer-0.0.9/renormalizer/mps/hop_expr.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/lib.py` & `renormalizer-0.0.9/renormalizer/mps/lib.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,452 +1,452 @@
-# -*- coding: utf-8 -*-
-# Author: Jiajun Ren <jiajunren0522@gmail.com>
-
-from functools import reduce
-from collections import deque
-
-from renormalizer.mps.backend import np, backend, xp
-from renormalizer.mps.matrix import (Matrix, multi_tensor_contract, asxp,
-    asnumpy, tensordot)
-
-
-class Environ:
-    def __init__(self, mps, mpo, domain=None, mps_conj=None):
-        # todo: real disk and other backend
-        # todo: contract_one_site_multi_mpo could generalize contract_one_site,
-        # we could unify them in the future.
-
-        # idx indicates the exact position of L or R, like
-        # L(idx-1) - mpo(idx) - R(idx+1)
-        self._virtual_disk = {}
-        if type(mpo) is list:
-            ndim = len(mpo) + 2
-        else:
-            ndim = 3
-        self.sentinel = xp.ones([1,]*ndim, dtype=backend.real_dtype)
-        self._construct(mps, mpo, domain, mps_conj)
-
-    def _construct(self, mps, mpo, domain=None, mps_conj=None):
-
-        assert domain in ["L", "R", None]
-
-        if mps_conj is None:
-            mps_conj = mps.conj()
-
-        if domain is None:
-            self._construct(mps, mpo, "L", mps_conj)
-            self._construct(mps, mpo, "R", mps_conj)
-            return
-        if domain == "L":
-            start, end, inc = 0, len(mps) - 1, 1
-        else:
-            start, end, inc = len(mps) - 1, 0, -1
-        self.write_l_sentinel(mps)
-        self.write_r_sentinel(mps)
-
-        tensor = self.sentinel
-        for idx in range(start, end, inc):
-            if type(mpo) is list:
-                # a list of mpos
-                tensor = contract_one_site_multi_mpo(tensor, mps[idx], [mp[idx] for mp in mpo], domain, ms_conj=mps_conj[idx])
-            else:
-                # one single mpo
-                tensor = contract_one_site(tensor, mps[idx], mpo[idx], domain, ms_conj=mps_conj[idx])
-            self.write(domain, idx, tensor)
-
-    def write_l_sentinel(self, mps):
-        self.write("L", -1, self.sentinel)
-
-    def write_r_sentinel(self, mps):
-        self.write("R", len(mps), self.sentinel)
-
-    def GetLR(
-        self, domain, siteidx, mps, mpo, itensor=None, method="Scratch", mps_conj=None):
-        """
-        get the L/R Hamiltonian matrix at a random site(siteidx): 3d tensor
-        S-     -S     mpsconj
-        O- or  -O     mpo
-        S-     -S     mps
-        enviroment part from self.virtual_disk,  system part from one step calculation
-        support from scratch calculation: from two open boundary np.ones((1,1,1))
-        """
-
-        assert domain in ["L", "R"]
-        assert method in ["Enviro", "System", "Scratch"]
-        if mps_conj is None:
-            # provide a dummy value. Creating conjugation of a whole MPS should be avoided when possible
-            # since the operation is actually rather expensive.
-            mps_conj = [None] * len(mps)
-
-        if siteidx not in range(len(mps)):
-            return self.sentinel
-
-        if method == "Scratch":
-            itensor = self.sentinel
-            if domain == "L":
-                sitelist = range(siteidx + 1)
-            else:
-                sitelist = range(len(mps) - 1, siteidx - 1, -1)
-            for imps in sitelist:
-                if type(mpo) is list:
-                    itensor = contract_one_site_multi_mpo(itensor, mps[imps],
-                            [mp[imps] for mp in mpo], domain,
-                            ms_conj=mps_conj[imps])
-                else:
-                    itensor = contract_one_site(itensor, mps[imps], mpo[imps],
-                        domain, ms_conj=mps_conj[imps])
-        elif method == "Enviro":
-            itensor = self.read(domain, siteidx)
-        elif method == "System":
-            if itensor is None:
-                offset = -1 if domain == "L" else 1
-                itensor = self.read(domain, siteidx + offset)
-            if type(mpo) is list:
-                itensor = contract_one_site_multi_mpo(itensor, mps[siteidx],
-                        [mp[siteidx] for mp in mpo],
-                        domain, mps_conj[siteidx])
-            else:
-                itensor = contract_one_site(itensor, mps[siteidx], mpo[siteidx],
-                        domain, mps_conj[siteidx])
-            self.write(domain, siteidx, itensor)
-
-        return itensor
-
-    def write(self, domain, siteidx, tensor):
-        self._virtual_disk[(domain, siteidx)] = asnumpy(tensor)
-
-    def read(self, domain: str, siteidx: int):
-        return asxp(self._virtual_disk[(domain, siteidx)])
-
-
-def contract_one_site_multi_mpo(environ, ms, mos, domain, ms_conj=None):
-    """
-    contract one mpos/mps(mpdm) site, mos is a list containing several local mo
-             _   _
-            | | | |
-    S-S-    | S-|-S-
-    O-O- or | O-|-O- (the ancillary bond is traced)
-    O-O-    | O-|-O-
-    S-S-    | S-|-S-
-            |_| |_|
-    """
-    assert domain in ["L", "R"]
-    if ms_conj is None:
-        ms_conj = ms.conj()
-    if domain == "L":
-        if ms.ndim == 3:
-            outtensor = tensordot(environ, ms_conj, ([0], [0]))
-            for mo in mos:
-                outtensor = tensordot(outtensor, mo, ([0,-2], [0,1]))
-            outtensor = tensordot(outtensor, ms, ([0,-2], [0,1]))
-        elif ms.ndim == 4:
-            outtensor = tensordot(environ, ms_conj.transpose(0,2,1,3), ([0], [0]))
-            for mo in mos:
-                outtensor = tensordot(outtensor, mo, ([0,-2], [0,1]))
-            outtensor = tensordot(outtensor, ms, ([0,1,-2], [0,2,1]))
-        else:
-            raise ValueError(
-                f"MPS ndim is not 3 or 4, got {ms.ndim}"
-            )
-    else:
-        if ms.ndim == 3:
-            outtensor = tensordot(environ, ms_conj, ([0], [-1]))
-            for mo in mos:
-                outtensor = tensordot(outtensor, mo, ([0,-1], [-1,1]))
-            outtensor = tensordot(outtensor, ms, ([0,-1], [-1,1]))
-        elif ms.ndim == 4:
-            outtensor = tensordot(environ, ms_conj.transpose(0,2,1,3), ([0], [-1]))
-            for mo in mos:
-                outtensor = tensordot(outtensor, mo, ([0,-1], [-1,1]))
-            outtensor = tensordot(outtensor, ms, ([0,2,-1], [-1,2,1]))
-        else:
-            raise ValueError(
-                f"MPS ndim is not 3 or 4, got {ms.ndim}"
-            )
-
-    return outtensor
-
-
-def contract_one_site(environ, ms, mo, domain, ms_conj=None):
-    """
-    contract one mpo/mps(mpdm) site
-             _   _
-            | | | |
-    S-S-    | S-|-S-
-    O-O- or | O-|-O- (the ancillary bond is traced)
-    S-S-    | S-|-S-
-            |_| |_|
-    """
-    assert domain in ["L", "R"]
-    if isinstance(ms, Matrix):
-        ms = ms.array
-    if isinstance(mo, Matrix):
-        mo = mo.array
-    if ms_conj is None:
-        ms_conj = ms.conj()
-    if domain == "L":
-        assert environ.shape[0] == ms_conj.shape[0]
-        assert environ.shape[1] == mo.shape[0]
-        assert environ.shape[2] == ms.shape[0]
-        """
-                       l
-        S-a-S-f    O-a-O-f
-            d          d
-        O-b-O-g or O-b-O-g
-            e          e
-        S-c-S-h    O-c-O-h
-                       l
-        """
-
-        if ms.ndim == 3:
-            path = [
-                ([0, 1], "abc, adf -> bcdf"),
-                ([2, 0], "bcdf, bdeg -> cfeg"),
-                ([1, 0], "cfeg, ceh -> fgh"),
-            ]
-        elif ms.ndim == 4:
-            path = [
-                ([0, 1], "abc, adlf -> bcdlf"),
-                ([2, 0], "bcdlf, bdeg -> clfeg"),
-                ([1, 0], "clfeg, celh -> fgh"),
-            ]
-        else:
-            raise ValueError(
-                f"MPS ndim is not 3 or 4, got {ms.ndim}"
-            )
-        outtensor = multi_tensor_contract(path, environ, ms_conj, mo, ms)
-
-    else:
-        assert environ.shape[0] == ms_conj.shape[-1]
-        assert environ.shape[1] == mo.shape[-1]
-        assert environ.shape[2] == ms.shape[-1]
-        """
-                       l
-        -f-S-a-S    -f-S-a-S
-           d           d
-        -g-O-b-O or -g-O-b-O
-           e           e
-        -h-S-c-S    -h-S-c-S
-                       l
-        """
-
-        if ms.ndim == 3:
-            path = [
-                ([0, 1], "fda, abc -> fdbc"),
-                ([2, 0], "fdbc, gdeb -> fcge"),
-                ([1, 0], "fcge, hec -> fgh"),
-            ]
-        elif ms.ndim == 4:
-            path = [
-                ([0, 1], "fdla, abc -> fdlbc"),
-                ([2, 0], "fdlbc, gdeb -> flcge"),
-                ([1, 0], "flcge, helc -> fgh"),
-            ]
-        else:
-            raise ValueError(
-                f"MPS ndim is not 3 or 4, got {ms.ndim}"
-            )
-        outtensor = multi_tensor_contract(path, ms_conj, environ, mo, ms)
-
-    return outtensor
-
-
-def select_basis(vset, sset, qnlist, compset, Mmax, percent=0):
-    """
-    select basis to construct new mps, and complementary mps
-    vset, compset is the column vector
-    """
-    qnlist = [tuple(qn) for qn in qnlist]
-    # allowed qn subsection
-    qnset = set(qnlist)
-    # convert to dict
-    basdic = dict()
-    for i in range(len(qnlist)):
-        # clean quantum number outside qnlist
-        if qnlist[i] in qnset:
-            basdic[i] = [qnlist[i], sset[i]]
-
-    # each good quantum number block equally get percent/nblocks
-    def block_select(basdic, qn, n):
-        block_basdic = {i: basdic[i] for i in basdic if basdic[i][0] == qn}
-        sort_block_basdic = sorted(
-            block_basdic.items(), key=lambda x: x[1][1], reverse=True
-        )
-        nget = min(n, len(sort_block_basdic))
-        # print(qn, "block # of retained basis", nget)
-        sidx = [i[0] for i in sort_block_basdic[0:nget]]
-        for idx in sidx:
-            del basdic[idx]
-
-        return sidx
-
-    nbasis = min(len(basdic), Mmax)
-    # print("# of selected basis", nbasis)
-    sidx = []
-
-    # equally select from each quantum number block
-    if percent != 0:
-        nbas_block = int(nbasis * percent / len(qnset))
-        for iqn in qnset:
-            sidx += block_select(basdic, iqn, nbas_block)
-
-    # others
-    nbasis = nbasis - len(sidx)
-
-    sortbasdic = sorted(basdic.items(), key=lambda x: x[1][1], reverse=True)
-    sidx += [i[0] for i in sortbasdic[0:nbasis]]
-
-    assert len(sidx) == len(set(sidx))  # there must be no duplicated
-
-    mpsdim = len(sidx)
-    # need to set value column by column. better in CPU
-    ms = np.zeros((vset.shape[0], mpsdim), dtype=vset.dtype)
-
-    if compset is not None:
-        compmps = np.zeros((compset.shape[0], mpsdim), dtype=compset.dtype)
-    else:
-        compmps = None
-
-    mpsqn = []
-    stot = 0.0
-    for idim in range(mpsdim):
-        ms[:, idim] = vset[:, sidx[idim]].copy()
-        if (compset is not None) and sidx[idim] < compset.shape[1]:
-            compmps[:, idim] = compset[:, sidx[idim]].copy() * sset[sidx[idim]]
-        mpsqn.append(qnlist[sidx[idim]])
-        stot += sset[sidx[idim]] ** 2
-
-    # print("discard:", 1.0 - stot)
-    if compmps is not None:
-        compmps = asxp(compmps)
-
-    return asxp(ms), mpsdim, np.array(mpsqn), compmps
-
-
-def update_cv(vset, sset, qnset, compset, nexciton, Mmax, spectratype,
-              percent=0):
-    sidx = select_Xbasis(qnset, sset, range(nexciton + 1), Mmax, spectratype,
-                         percent=percent)
-    xdim = len(sidx)
-    x = np.zeros((vset.shape[0], xdim), dtype=vset.dtype)
-    xqn = []
-    if compset is not None:
-        compx = np.zeros((compset.shape[0], xdim), dtype=compset.dtype)
-    else:
-        compx = None
-
-    for idim in range(xdim):
-        x[:, idim] = vset[:, sidx[idim]].copy()
-        if (compset is not None) and (sidx[idim] < compset.shape[1]):
-            compx[:, idim] = compset[:, sidx[idim]].copy() * sset[sidx[idim]]
-        xqn.append(qnset[sidx[idim]])
-    if compx is not None:
-        compx = Matrix(compx)
-    return Matrix(x), xdim, xqn, compx
-
-
-def select_Xbasis(qnset, Sset, qnlist, Mmax, spectratype, percent=0.0):
-    # select basis according to Sset under qnlist requirement
-    # convert to dict
-    basdic = {}
-    sidx = []
-    for i in range(len(qnset)):
-        basdic[i] = [qnset[i], Sset[i]]
-    # print('basdic', basdic)
-    # clean quantum number outiside qnlist
-    flag = []
-    if spectratype != "conductivity":
-        if spectratype == "abs":
-            tag_1, tag_2 = 0, 1
-        else:
-            tag_1, tag_2 = 1, 0
-        for ibas in basdic:
-            if ((basdic[ibas][0][tag_1] not in qnlist) or (
-                    basdic[ibas][0][tag_2] != 0)):
-                flag.append(ibas)
-    else:
-        for ibas in basdic:
-            if (basdic[ibas][0][0] not in qnlist) or (
-                    basdic[ibas][0][1] not in qnlist):
-                flag.append(ibas)
-
-    # i = 0
-    # for j in flag:
-    #     if i == 0:
-    #         del basdic[j]
-    #     else:
-    #         del basdic[j - i]
-
-    def block_select(basdic, qn, n):
-        block_basdic = {i: basdic[i]
-                        for i in basdic if basdic[i][0] == qn}
-        sort_block_basdic = sorted(block_basdic.items(), key=lambda x: x[1][1],
-                                   reverse=True)
-        nget = min(n, len(sort_block_basdic))
-        # print('n', n)
-        # print('len', len(sort_block_basdic))
-        # print('nget', nget)
-        sidx = [i[0] for i in sort_block_basdic[0: nget]]
-        for idx in sidx:
-            del basdic[idx]
-        # print('qn', qn)
-        # print('sidx', sidx)
-        return sidx
-    nbasis = min(len(basdic), Mmax)
-    if percent != 0:
-        # print('percent', percent)
-        if spectratype == "abs":
-            nbas_block = int(nbasis * percent / len(qnlist))
-            for iqn in qnlist:
-                sidx += block_select(basdic, [iqn, 0], nbas_block)
-        elif spectratype == "emi":
-            nbas_block = int(nbasis * percent / len(qnlist))
-            for iqn in qnlist:
-                sidx += block_select(basdic, [0, iqn], nbas_block)
-        else:
-            nbas_block = int(nbasis * percent / 4)
-            for iqn in [[0, 0], [0, 1], [1, 0], [1, 1]]:
-                sidx += block_select(basdic, iqn, nbas_block)
-
-    nbasis = nbasis - len(sidx)
-    sortbasdic = sorted(basdic.items(), key=lambda y: y[1][1], reverse=True)
-    sidx += [i[0] for i in sortbasdic[0: nbasis]]
-    # print('sidx', sidx)
-    return sidx
-
-
-def compressed_sum(mps_list, batchsize=5, temp_m_trunc=None):
-    assert len(mps_list) != 0
-    mps_queue = deque(mps_list)
-    while len(mps_queue) != 1:
-        term_to_sum = []
-        for i in range(min(batchsize, len(mps_queue))):
-            term_to_sum.append(mps_queue.popleft())
-        s = _sum(term_to_sum, temp_m_trunc=temp_m_trunc)
-        mps_queue.append(s)
-    return mps_queue[0]
-
-
-def _sum(mps_list, compress=True, temp_m_trunc=None):
-    new_mps = reduce(lambda mps1, mps2: mps1.add(mps2), mps_list)
-    if compress and not mps_list[0].compress_add:
-        new_mps.canonicalise()
-        new_mps.compress(temp_m_trunc=temp_m_trunc)
-    return new_mps
-
-
-def cvec2cmat(c, qn_mask, nroots=1):
-    # recover good quantum number vector c to matrix format
-    if nroots == 1:
-        cstruct = np.zeros(qn_mask.shape, dtype=c.dtype)
-        np.place(cstruct, qn_mask, c)
-    else:
-        cstruct = []
-        if type(c) is not list:
-            assert c.ndim == 2
-            c = [c[:,iroot] for iroot in range(c.shape[1])]
-        for ic in c:
-            icstruct = np.zeros(qn_mask.shape, dtype=ic.dtype)
-            np.place(icstruct, qn_mask, ic)
-            cstruct.append(icstruct)
-
-    return cstruct
+# -*- coding: utf-8 -*-
+# Author: Jiajun Ren <jiajunren0522@gmail.com>
+
+from functools import reduce
+from collections import deque
+
+from renormalizer.mps.backend import np, backend, xp
+from renormalizer.mps.matrix import (Matrix, multi_tensor_contract, asxp,
+    asnumpy, tensordot)
+
+
+class Environ:
+    def __init__(self, mps, mpo, domain=None, mps_conj=None):
+        # todo: real disk and other backend
+        # todo: contract_one_site_multi_mpo could generalize contract_one_site,
+        # we could unify them in the future.
+
+        # idx indicates the exact position of L or R, like
+        # L(idx-1) - mpo(idx) - R(idx+1)
+        self._virtual_disk = {}
+        if type(mpo) is list:
+            ndim = len(mpo) + 2
+        else:
+            ndim = 3
+        self.sentinel = xp.ones([1,]*ndim, dtype=backend.real_dtype)
+        self._construct(mps, mpo, domain, mps_conj)
+
+    def _construct(self, mps, mpo, domain=None, mps_conj=None):
+
+        assert domain in ["L", "R", None]
+
+        if mps_conj is None:
+            mps_conj = mps.conj()
+
+        if domain is None:
+            self._construct(mps, mpo, "L", mps_conj)
+            self._construct(mps, mpo, "R", mps_conj)
+            return
+        if domain == "L":
+            start, end, inc = 0, len(mps) - 1, 1
+        else:
+            start, end, inc = len(mps) - 1, 0, -1
+        self.write_l_sentinel(mps)
+        self.write_r_sentinel(mps)
+
+        tensor = self.sentinel
+        for idx in range(start, end, inc):
+            if type(mpo) is list:
+                # a list of mpos
+                tensor = contract_one_site_multi_mpo(tensor, mps[idx], [mp[idx] for mp in mpo], domain, ms_conj=mps_conj[idx])
+            else:
+                # one single mpo
+                tensor = contract_one_site(tensor, mps[idx], mpo[idx], domain, ms_conj=mps_conj[idx])
+            self.write(domain, idx, tensor)
+
+    def write_l_sentinel(self, mps):
+        self.write("L", -1, self.sentinel)
+
+    def write_r_sentinel(self, mps):
+        self.write("R", len(mps), self.sentinel)
+
+    def GetLR(
+        self, domain, siteidx, mps, mpo, itensor=None, method="Scratch", mps_conj=None):
+        """
+        get the L/R Hamiltonian matrix at a random site(siteidx): 3d tensor
+        S-     -S     mpsconj
+        O- or  -O     mpo
+        S-     -S     mps
+        enviroment part from self.virtual_disk,  system part from one step calculation
+        support from scratch calculation: from two open boundary np.ones((1,1,1))
+        """
+
+        assert domain in ["L", "R"]
+        assert method in ["Enviro", "System", "Scratch"]
+        if mps_conj is None:
+            # provide a dummy value. Creating conjugation of a whole MPS should be avoided when possible
+            # since the operation is actually rather expensive.
+            mps_conj = [None] * len(mps)
+
+        if siteidx not in range(len(mps)):
+            return self.sentinel
+
+        if method == "Scratch":
+            itensor = self.sentinel
+            if domain == "L":
+                sitelist = range(siteidx + 1)
+            else:
+                sitelist = range(len(mps) - 1, siteidx - 1, -1)
+            for imps in sitelist:
+                if type(mpo) is list:
+                    itensor = contract_one_site_multi_mpo(itensor, mps[imps],
+                            [mp[imps] for mp in mpo], domain,
+                            ms_conj=mps_conj[imps])
+                else:
+                    itensor = contract_one_site(itensor, mps[imps], mpo[imps],
+                        domain, ms_conj=mps_conj[imps])
+        elif method == "Enviro":
+            itensor = self.read(domain, siteidx)
+        elif method == "System":
+            if itensor is None:
+                offset = -1 if domain == "L" else 1
+                itensor = self.read(domain, siteidx + offset)
+            if type(mpo) is list:
+                itensor = contract_one_site_multi_mpo(itensor, mps[siteidx],
+                        [mp[siteidx] for mp in mpo],
+                        domain, mps_conj[siteidx])
+            else:
+                itensor = contract_one_site(itensor, mps[siteidx], mpo[siteidx],
+                        domain, mps_conj[siteidx])
+            self.write(domain, siteidx, itensor)
+
+        return itensor
+
+    def write(self, domain, siteidx, tensor):
+        self._virtual_disk[(domain, siteidx)] = asnumpy(tensor)
+
+    def read(self, domain: str, siteidx: int):
+        return asxp(self._virtual_disk[(domain, siteidx)])
+
+
+def contract_one_site_multi_mpo(environ, ms, mos, domain, ms_conj=None):
+    """
+    contract one mpos/mps(mpdm) site, mos is a list containing several local mo
+             _   _
+            | | | |
+    S-S-    | S-|-S-
+    O-O- or | O-|-O- (the ancillary bond is traced)
+    O-O-    | O-|-O-
+    S-S-    | S-|-S-
+            |_| |_|
+    """
+    assert domain in ["L", "R"]
+    if ms_conj is None:
+        ms_conj = ms.conj()
+    if domain == "L":
+        if ms.ndim == 3:
+            outtensor = tensordot(environ, ms_conj, ([0], [0]))
+            for mo in mos:
+                outtensor = tensordot(outtensor, mo, ([0,-2], [0,1]))
+            outtensor = tensordot(outtensor, ms, ([0,-2], [0,1]))
+        elif ms.ndim == 4:
+            outtensor = tensordot(environ, ms_conj.transpose(0,2,1,3), ([0], [0]))
+            for mo in mos:
+                outtensor = tensordot(outtensor, mo, ([0,-2], [0,1]))
+            outtensor = tensordot(outtensor, ms, ([0,1,-2], [0,2,1]))
+        else:
+            raise ValueError(
+                f"MPS ndim is not 3 or 4, got {ms.ndim}"
+            )
+    else:
+        if ms.ndim == 3:
+            outtensor = tensordot(environ, ms_conj, ([0], [-1]))
+            for mo in mos:
+                outtensor = tensordot(outtensor, mo, ([0,-1], [-1,1]))
+            outtensor = tensordot(outtensor, ms, ([0,-1], [-1,1]))
+        elif ms.ndim == 4:
+            outtensor = tensordot(environ, ms_conj.transpose(0,2,1,3), ([0], [-1]))
+            for mo in mos:
+                outtensor = tensordot(outtensor, mo, ([0,-1], [-1,1]))
+            outtensor = tensordot(outtensor, ms, ([0,2,-1], [-1,2,1]))
+        else:
+            raise ValueError(
+                f"MPS ndim is not 3 or 4, got {ms.ndim}"
+            )
+
+    return outtensor
+
+
+def contract_one_site(environ, ms, mo, domain, ms_conj=None):
+    """
+    contract one mpo/mps(mpdm) site
+             _   _
+            | | | |
+    S-S-    | S-|-S-
+    O-O- or | O-|-O- (the ancillary bond is traced)
+    S-S-    | S-|-S-
+            |_| |_|
+    """
+    assert domain in ["L", "R"]
+    if isinstance(ms, Matrix):
+        ms = ms.array
+    if isinstance(mo, Matrix):
+        mo = mo.array
+    if ms_conj is None:
+        ms_conj = ms.conj()
+    if domain == "L":
+        assert environ.shape[0] == ms_conj.shape[0]
+        assert environ.shape[1] == mo.shape[0]
+        assert environ.shape[2] == ms.shape[0]
+        """
+                       l
+        S-a-S-f    O-a-O-f
+            d          d
+        O-b-O-g or O-b-O-g
+            e          e
+        S-c-S-h    O-c-O-h
+                       l
+        """
+
+        if ms.ndim == 3:
+            path = [
+                ([0, 1], "abc, adf -> bcdf"),
+                ([2, 0], "bcdf, bdeg -> cfeg"),
+                ([1, 0], "cfeg, ceh -> fgh"),
+            ]
+        elif ms.ndim == 4:
+            path = [
+                ([0, 1], "abc, adlf -> bcdlf"),
+                ([2, 0], "bcdlf, bdeg -> clfeg"),
+                ([1, 0], "clfeg, celh -> fgh"),
+            ]
+        else:
+            raise ValueError(
+                f"MPS ndim is not 3 or 4, got {ms.ndim}"
+            )
+        outtensor = multi_tensor_contract(path, environ, ms_conj, mo, ms)
+
+    else:
+        assert environ.shape[0] == ms_conj.shape[-1]
+        assert environ.shape[1] == mo.shape[-1]
+        assert environ.shape[2] == ms.shape[-1]
+        """
+                       l
+        -f-S-a-S    -f-S-a-S
+           d           d
+        -g-O-b-O or -g-O-b-O
+           e           e
+        -h-S-c-S    -h-S-c-S
+                       l
+        """
+
+        if ms.ndim == 3:
+            path = [
+                ([0, 1], "fda, abc -> fdbc"),
+                ([2, 0], "fdbc, gdeb -> fcge"),
+                ([1, 0], "fcge, hec -> fgh"),
+            ]
+        elif ms.ndim == 4:
+            path = [
+                ([0, 1], "fdla, abc -> fdlbc"),
+                ([2, 0], "fdlbc, gdeb -> flcge"),
+                ([1, 0], "flcge, helc -> fgh"),
+            ]
+        else:
+            raise ValueError(
+                f"MPS ndim is not 3 or 4, got {ms.ndim}"
+            )
+        outtensor = multi_tensor_contract(path, ms_conj, environ, mo, ms)
+
+    return outtensor
+
+
+def select_basis(vset, sset, qnlist, compset, Mmax, percent=0):
+    """
+    select basis to construct new mps, and complementary mps
+    vset, compset is the column vector
+    """
+    qnlist = [tuple(qn) for qn in qnlist]
+    # allowed qn subsection
+    qnset = set(qnlist)
+    # convert to dict
+    basdic = dict()
+    for i in range(len(qnlist)):
+        # clean quantum number outside qnlist
+        if qnlist[i] in qnset:
+            basdic[i] = [qnlist[i], sset[i]]
+
+    # each good quantum number block equally get percent/nblocks
+    def block_select(basdic, qn, n):
+        block_basdic = {i: basdic[i] for i in basdic if basdic[i][0] == qn}
+        sort_block_basdic = sorted(
+            block_basdic.items(), key=lambda x: x[1][1], reverse=True
+        )
+        nget = min(n, len(sort_block_basdic))
+        # print(qn, "block # of retained basis", nget)
+        sidx = [i[0] for i in sort_block_basdic[0:nget]]
+        for idx in sidx:
+            del basdic[idx]
+
+        return sidx
+
+    nbasis = min(len(basdic), Mmax)
+    # print("# of selected basis", nbasis)
+    sidx = []
+
+    # equally select from each quantum number block
+    if percent != 0:
+        nbas_block = int(nbasis * percent / len(qnset))
+        for iqn in qnset:
+            sidx += block_select(basdic, iqn, nbas_block)
+
+    # others
+    nbasis = nbasis - len(sidx)
+
+    sortbasdic = sorted(basdic.items(), key=lambda x: x[1][1], reverse=True)
+    sidx += [i[0] for i in sortbasdic[0:nbasis]]
+
+    assert len(sidx) == len(set(sidx))  # there must be no duplicated
+
+    mpsdim = len(sidx)
+    # need to set value column by column. better in CPU
+    ms = np.zeros((vset.shape[0], mpsdim), dtype=vset.dtype)
+
+    if compset is not None:
+        compmps = np.zeros((compset.shape[0], mpsdim), dtype=compset.dtype)
+    else:
+        compmps = None
+
+    mpsqn = []
+    stot = 0.0
+    for idim in range(mpsdim):
+        ms[:, idim] = vset[:, sidx[idim]].copy()
+        if (compset is not None) and sidx[idim] < compset.shape[1]:
+            compmps[:, idim] = compset[:, sidx[idim]].copy() * sset[sidx[idim]]
+        mpsqn.append(qnlist[sidx[idim]])
+        stot += sset[sidx[idim]] ** 2
+
+    # print("discard:", 1.0 - stot)
+    if compmps is not None:
+        compmps = asxp(compmps)
+
+    return asxp(ms), mpsdim, np.array(mpsqn), compmps
+
+
+def update_cv(vset, sset, qnset, compset, nexciton, Mmax, spectratype,
+              percent=0):
+    sidx = select_Xbasis(qnset, sset, range(nexciton + 1), Mmax, spectratype,
+                         percent=percent)
+    xdim = len(sidx)
+    x = np.zeros((vset.shape[0], xdim), dtype=vset.dtype)
+    xqn = []
+    if compset is not None:
+        compx = np.zeros((compset.shape[0], xdim), dtype=compset.dtype)
+    else:
+        compx = None
+
+    for idim in range(xdim):
+        x[:, idim] = vset[:, sidx[idim]].copy()
+        if (compset is not None) and (sidx[idim] < compset.shape[1]):
+            compx[:, idim] = compset[:, sidx[idim]].copy() * sset[sidx[idim]]
+        xqn.append(qnset[sidx[idim]])
+    if compx is not None:
+        compx = Matrix(compx)
+    return Matrix(x), xdim, xqn, compx
+
+
+def select_Xbasis(qnset, Sset, qnlist, Mmax, spectratype, percent=0.0):
+    # select basis according to Sset under qnlist requirement
+    # convert to dict
+    basdic = {}
+    sidx = []
+    for i in range(len(qnset)):
+        basdic[i] = [qnset[i], Sset[i]]
+    # print('basdic', basdic)
+    # clean quantum number outiside qnlist
+    flag = []
+    if spectratype != "conductivity":
+        if spectratype == "abs":
+            tag_1, tag_2 = 0, 1
+        else:
+            tag_1, tag_2 = 1, 0
+        for ibas in basdic:
+            if ((basdic[ibas][0][tag_1] not in qnlist) or (
+                    basdic[ibas][0][tag_2] != 0)):
+                flag.append(ibas)
+    else:
+        for ibas in basdic:
+            if (basdic[ibas][0][0] not in qnlist) or (
+                    basdic[ibas][0][1] not in qnlist):
+                flag.append(ibas)
+
+    # i = 0
+    # for j in flag:
+    #     if i == 0:
+    #         del basdic[j]
+    #     else:
+    #         del basdic[j - i]
+
+    def block_select(basdic, qn, n):
+        block_basdic = {i: basdic[i]
+                        for i in basdic if basdic[i][0] == qn}
+        sort_block_basdic = sorted(block_basdic.items(), key=lambda x: x[1][1],
+                                   reverse=True)
+        nget = min(n, len(sort_block_basdic))
+        # print('n', n)
+        # print('len', len(sort_block_basdic))
+        # print('nget', nget)
+        sidx = [i[0] for i in sort_block_basdic[0: nget]]
+        for idx in sidx:
+            del basdic[idx]
+        # print('qn', qn)
+        # print('sidx', sidx)
+        return sidx
+    nbasis = min(len(basdic), Mmax)
+    if percent != 0:
+        # print('percent', percent)
+        if spectratype == "abs":
+            nbas_block = int(nbasis * percent / len(qnlist))
+            for iqn in qnlist:
+                sidx += block_select(basdic, [iqn, 0], nbas_block)
+        elif spectratype == "emi":
+            nbas_block = int(nbasis * percent / len(qnlist))
+            for iqn in qnlist:
+                sidx += block_select(basdic, [0, iqn], nbas_block)
+        else:
+            nbas_block = int(nbasis * percent / 4)
+            for iqn in [[0, 0], [0, 1], [1, 0], [1, 1]]:
+                sidx += block_select(basdic, iqn, nbas_block)
+
+    nbasis = nbasis - len(sidx)
+    sortbasdic = sorted(basdic.items(), key=lambda y: y[1][1], reverse=True)
+    sidx += [i[0] for i in sortbasdic[0: nbasis]]
+    # print('sidx', sidx)
+    return sidx
+
+
+def compressed_sum(mps_list, batchsize=5, temp_m_trunc=None):
+    assert len(mps_list) != 0
+    mps_queue = deque(mps_list)
+    while len(mps_queue) != 1:
+        term_to_sum = []
+        for i in range(min(batchsize, len(mps_queue))):
+            term_to_sum.append(mps_queue.popleft())
+        s = _sum(term_to_sum, temp_m_trunc=temp_m_trunc)
+        mps_queue.append(s)
+    return mps_queue[0]
+
+
+def _sum(mps_list, compress=True, temp_m_trunc=None):
+    new_mps = reduce(lambda mps1, mps2: mps1.add(mps2), mps_list)
+    if compress and not mps_list[0].compress_add:
+        new_mps.canonicalise()
+        new_mps.compress(temp_m_trunc=temp_m_trunc)
+    return new_mps
+
+
+def cvec2cmat(c, qn_mask, nroots=1):
+    # recover good quantum number vector c to matrix format
+    if nroots == 1:
+        cstruct = np.zeros(qn_mask.shape, dtype=c.dtype)
+        np.place(cstruct, qn_mask, c)
+    else:
+        cstruct = []
+        if type(c) is not list:
+            assert c.ndim == 2
+            c = [c[:,iroot] for iroot in range(c.shape[1])]
+        for ic in c:
+            icstruct = np.zeros(qn_mask.shape, dtype=ic.dtype)
+            np.place(icstruct, qn_mask, ic)
+            cstruct.append(icstruct)
+
+    return cstruct
```

### Comparing `renormalizer-0.0.8/renormalizer/mps/matrix.py` & `renormalizer-0.0.9/renormalizer/mps/matrix.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,316 +1,316 @@
-# -*- coding: utf-8 -*-
-# Author: Jiajun Ren <jiajunren0522@gmail.com>
-
-import weakref
-import logging
-from typing import List, Union
-
-from renormalizer.mps.backend import np, backend, xp, USE_GPU
-
-logger = logging.getLogger(__name__)
-
-
-class Matrix:
-
-    def __init__(self, array, dtype=None):
-        assert array is not None
-        array = asnumpy(array)
-        if dtype == backend.real_dtype:
-            # forbid unchecked casting
-            assert not np.iscomplexobj(array)
-        if dtype is None:
-            if np.iscomplexobj(array):
-                dtype = backend.complex_dtype
-            else:
-                dtype = backend.real_dtype
-        self.array: np.ndarray = np.asarray(array, dtype=dtype)
-        self.original_shape = self.array.shape
-        self.sigmaqn = None
-        backend.running = True
-
-    def __getattr__(self, item):
-        # use this way to obtain ``array`` to prevent infinite recursion during multi-processing
-        # see https://stackoverflow.com/questions/22781872/python-pickle-got-acycle-recursion-with-getattr
-        array = super().__getattribute__("array")
-        res = getattr(array, item)
-        if isinstance(res, np.ndarray):
-            return Matrix(res)
-        functiontype = type([].append)
-        if isinstance(res, functiontype):
-
-            def wrapped(*args, **kwargs):
-                res2 = res(*args, **kwargs)
-                if isinstance(res2, np.ndarray):
-                    return Matrix(res2)
-                return res2
-
-            return wrapped
-        return res
-
-    # for debugging purpose (let it shown in debuggers)
-    @property
-    def dtype(self):
-        return self.array.dtype
-
-    def astype(self, dtype):
-        assert not (self.dtype == backend.complex_dtype and dtype == backend.real_dtype)
-        self.array = np.asarray(self.array, dtype=dtype)
-        return self
-
-    def abs(self):
-        return self.__class__(np.abs(self.array))
-
-    def norm(self):
-        return np.linalg.norm(self.array.flatten())
-
-    # physical indices exclude first and last indices
-    @property
-    def pdim(self):
-        return self.original_shape[1:-1]
-
-    @property
-    def pdim_prod(self):
-        return np.prod(self.pdim)
-
-    @property
-    def bond_dim(self):
-        return self.original_shape[0], self.original_shape[-1]
-
-    @property
-    def r_combine_shape(self):
-        return self.original_shape[0], np.prod(self.original_shape[1:])
-
-    @property
-    def l_combine_shape(self):
-        return np.prod(self.original_shape[:-1]), self.original_shape[-1]
-
-    def r_combine(self):
-        return self.reshape(self.r_combine_shape)
-
-    def l_combine(self):
-        return self.reshape(self.l_combine_shape)
-
-    def check_lortho(self, atol=None):
-        """
-        check L-orthogonal
-        """
-        if atol is None:
-            atol = backend.canonical_atol
-        tensm = asxp(self.array.reshape([np.prod(self.shape[:-1]), self.shape[-1]]))
-        s = tensm.T.conj() @ tensm
-        return xp.allclose(s, xp.eye(s.shape[0]), atol=atol)
-
-    def check_rortho(self, atol=None):
-        """
-        check R-orthogonal
-        """
-        if atol is None:
-            atol = backend.canonical_atol
-        tensm = asxp(self.array.reshape([self.shape[0], np.prod(self.shape[1:])]))
-        s = tensm @ tensm.T.conj()
-        return xp.allclose(s, xp.eye(s.shape[0]), atol=atol)
-
-    def to_complex(self):
-        # `xp.array` always creates new array, so to_complex means copy, which is
-        # in accordance with NumPy
-        return np.array(self.array, dtype=backend.complex_dtype)
-
-    def copy(self):
-        new = self.__class__(self.array.copy(), self.array.dtype)
-        new.original_shape = self.original_shape
-        new.sigmaqn = self.sigmaqn
-        return new
-
-    def nearly_zero(self):
-        if backend.is_32bits:
-            atol = 1e-10
-        else:
-            atol = 1e-20
-        return np.allclose(self.array, np.zeros_like(self.array), atol=atol)
-
-    def __hash__(self):
-        return hash((self.array.shape, self.array.tobytes()))
-
-    def __getitem__(self, item):
-        res = self.array.__getitem__(item)
-        if res.ndim != 0:
-            return self.__class__(res)
-        else:
-            return res
-
-    def __setitem__(self, key, value):
-        if isinstance(value, Matrix):
-            value = value.array
-        self.array[key] = value
-
-    def __add__(self, other):
-        if isinstance(other, Matrix):
-            other = other.array
-        return self.__class__(self.array.__add__(other))
-
-    def __radd__(self, other):
-        if isinstance(other, Matrix):
-            other = other.array
-        return self.__class__(self.array.__radd__(other))
-
-    def __mul__(self, other):
-        if isinstance(other, Matrix):
-            other = other.array
-        return self.__class__(self.array.__mul__(other))
-
-    def __rmul__(self, other):
-        if isinstance(other, Matrix):
-            other = other.array
-        return self.__class__(self.array.__rmul__(other))
-
-    def __truediv__(self, other):
-        if isinstance(other, Matrix):
-            other = other.array
-        return self.__class__(self.array.__truediv__(other))
-
-    def __repr__(self):
-        return f"<Matrix at 0x{id(self):x} {self.shape} {self.dtype}>"
-
-    def __str__(self):
-        return str(self.array)
-
-    def __float__(self):
-        return self.array.__float__()
-
-    def __complex__(self):
-        return self.array.__complex__()
-
-
-def zeros(shape, dtype=None):
-    if dtype is None:
-        dtype = backend.real_dtype
-    return Matrix(np.zeros(shape), dtype=dtype)
-
-
-def eye(N, M=None, dtype=None):
-    if dtype is None:
-        dtype = backend.real_dtype
-    return Matrix(np.eye(N, M), dtype=dtype)
-
-
-def ones(shape, dtype=None):
-    if dtype is None:
-        dtype = backend.real_dtype
-    return Matrix(np.ones(shape), dtype=dtype)
-
-
-def einsum(subscripts, *operands):
-    return Matrix(np.einsum(subscripts, *[o.array for o in operands]))
-
-
-def tensordot(a: Union[Matrix, np.ndarray], b: Union[Matrix, np.ndarray, xp.ndarray], axes) -> xp.ndarray:
-    return xp.tensordot(asxp(a), asxp(b), axes)
-
-
-def moveaxis(a: Matrix, source, destination):
-    return Matrix(np.moveaxis(a.array, source, destination))
-
-
-def vstack(tup):
-    return Matrix(np.vstack([m.array for m in tup]))
-
-
-def dstack(tup):
-    return Matrix(np.dstack([m.array for m in tup]))
-
-
-def concatenate(arrays, axis=None):
-    return Matrix(np.concatenate([m.array for m in arrays], axis))
-
-
-# can only use numpy for now. see gh-cupy-1946
-def allclose(a, b, rtol=1.0e-5, atol=1.0e-8):
-    if isinstance(a, Matrix):
-        a = a.array
-    else:
-        a = np.asarray(a)
-    if isinstance(b, Matrix):
-        b = b.array
-    else:
-        b = np.asarray(b)
-    return np.allclose(a, b, rtol=rtol, atol=atol)
-
-
-def multi_tensor_contract(path, *operands: [List[Union[Matrix, np.ndarray, xp.ndarray]]]):
-    """
-    ipath[0] is the index of the mat
-    ipaht[1] is the contraction index
-    oeprands is the arrays
-
-    For example:  in mpompsmat.py
-    path = [([0, 1],"fdla, abc -> fdlbc")   ,\
-            ([2, 0],"fdlbc, gdeb -> flcge") ,\
-            ([1, 0],"flcge, helc -> fgh")]
-    outtensor = tensorlib.multi_tensor_contract(path, MPSconj[isite], intensor,
-            MPO[isite], MPS[isite])
-    """
-
-    operands = list(operands)
-    for ipath in path:
-
-        input_str, results_str = ipath[1].split("->")
-        input_str = input_str.split(",")
-        input_str = [x.replace(" ", "") for x in input_str]
-        results_set = set(results_str)
-        inputs_set = set(input_str[0] + input_str[1])
-        idx_removed = inputs_set - (inputs_set & results_set)
-
-        tmpmat = pair_tensor_contract(
-            operands[ipath[0][0]],
-            input_str[0],
-            operands[ipath[0][1]],
-            input_str[1],
-            idx_removed,
-        )
-
-        for x in sorted(ipath[0], reverse=True):
-            del operands[x]
-
-        operands.append(tmpmat)
-
-    return operands[0]
-
-
-def pair_tensor_contract(
-    view_left: Union[Matrix, np.ndarray, xp.ndarray],
-    input_left,
-    view_right: Union[Matrix, np.ndarray, xp.ndarray],
-    input_right,
-    idx_removed,
-):
-    # Find indices to contract over
-    left_pos, right_pos = (), ()
-    for s in idx_removed:
-        left_pos += (input_left.find(s),)
-        right_pos += (input_right.find(s),)
-    return tensordot(view_left, view_right, axes=(left_pos, right_pos))
-
-
-def asnumpy(array: Union[np.ndarray, xp.ndarray, Matrix]) -> np.ndarray:
-    if array is None:
-        return None
-    if isinstance(array, Matrix):
-        return array.array
-    if not USE_GPU:
-        assert isinstance(array, np.ndarray)
-        return array
-    if isinstance(array, np.ndarray):
-        return array
-    stream = xp.cuda.get_current_stream()
-    return xp.asnumpy(array, stream=stream)
-
-
-def asxp(array: Union[np.ndarray, xp.ndarray, Matrix]) -> xp.ndarray:
-    if array is None:
-        return None
-    if isinstance(array, Matrix):
-        array = array.array
-    if not USE_GPU:
-        assert isinstance(array, np.ndarray)
-        return array
-    return xp.asarray(array)
+# -*- coding: utf-8 -*-
+# Author: Jiajun Ren <jiajunren0522@gmail.com>
+
+import weakref
+import logging
+from typing import List, Union
+
+from renormalizer.mps.backend import np, backend, xp, USE_GPU
+
+logger = logging.getLogger(__name__)
+
+
+class Matrix:
+
+    def __init__(self, array, dtype=None):
+        assert array is not None
+        array = asnumpy(array)
+        if dtype == backend.real_dtype:
+            # forbid unchecked casting
+            assert not np.iscomplexobj(array)
+        if dtype is None:
+            if np.iscomplexobj(array):
+                dtype = backend.complex_dtype
+            else:
+                dtype = backend.real_dtype
+        self.array: np.ndarray = np.asarray(array, dtype=dtype)
+        self.original_shape = self.array.shape
+        self.sigmaqn = None
+        backend.running = True
+
+    def __getattr__(self, item):
+        # use this way to obtain ``array`` to prevent infinite recursion during multi-processing
+        # see https://stackoverflow.com/questions/22781872/python-pickle-got-acycle-recursion-with-getattr
+        array = super().__getattribute__("array")
+        res = getattr(array, item)
+        if isinstance(res, np.ndarray):
+            return Matrix(res)
+        functiontype = type([].append)
+        if isinstance(res, functiontype):
+
+            def wrapped(*args, **kwargs):
+                res2 = res(*args, **kwargs)
+                if isinstance(res2, np.ndarray):
+                    return Matrix(res2)
+                return res2
+
+            return wrapped
+        return res
+
+    # for debugging purpose (let it shown in debuggers)
+    @property
+    def dtype(self):
+        return self.array.dtype
+
+    def astype(self, dtype):
+        assert not (self.dtype == backend.complex_dtype and dtype == backend.real_dtype)
+        self.array = np.asarray(self.array, dtype=dtype)
+        return self
+
+    def abs(self):
+        return self.__class__(np.abs(self.array))
+
+    def norm(self):
+        return np.linalg.norm(self.array.flatten())
+
+    # physical indices exclude first and last indices
+    @property
+    def pdim(self):
+        return self.original_shape[1:-1]
+
+    @property
+    def pdim_prod(self):
+        return np.prod(self.pdim)
+
+    @property
+    def bond_dim(self):
+        return self.original_shape[0], self.original_shape[-1]
+
+    @property
+    def r_combine_shape(self):
+        return self.original_shape[0], np.prod(self.original_shape[1:])
+
+    @property
+    def l_combine_shape(self):
+        return np.prod(self.original_shape[:-1]), self.original_shape[-1]
+
+    def r_combine(self):
+        return self.reshape(self.r_combine_shape)
+
+    def l_combine(self):
+        return self.reshape(self.l_combine_shape)
+
+    def check_lortho(self, atol=None):
+        """
+        check L-orthogonal
+        """
+        if atol is None:
+            atol = backend.canonical_atol
+        tensm = asxp(self.array.reshape([np.prod(self.shape[:-1]), self.shape[-1]]))
+        s = tensm.T.conj() @ tensm
+        return xp.allclose(s, xp.eye(s.shape[0]), atol=atol)
+
+    def check_rortho(self, atol=None):
+        """
+        check R-orthogonal
+        """
+        if atol is None:
+            atol = backend.canonical_atol
+        tensm = asxp(self.array.reshape([self.shape[0], np.prod(self.shape[1:])]))
+        s = tensm @ tensm.T.conj()
+        return xp.allclose(s, xp.eye(s.shape[0]), atol=atol)
+
+    def to_complex(self):
+        # `xp.array` always creates new array, so to_complex means copy, which is
+        # in accordance with NumPy
+        return np.array(self.array, dtype=backend.complex_dtype)
+
+    def copy(self):
+        new = self.__class__(self.array.copy(), self.array.dtype)
+        new.original_shape = self.original_shape
+        new.sigmaqn = self.sigmaqn
+        return new
+
+    def nearly_zero(self):
+        if backend.is_32bits:
+            atol = 1e-10
+        else:
+            atol = 1e-20
+        return np.allclose(self.array, np.zeros_like(self.array), atol=atol)
+
+    def __hash__(self):
+        return hash((self.array.shape, self.array.tobytes()))
+
+    def __getitem__(self, item):
+        res = self.array.__getitem__(item)
+        if res.ndim != 0:
+            return self.__class__(res)
+        else:
+            return res
+
+    def __setitem__(self, key, value):
+        if isinstance(value, Matrix):
+            value = value.array
+        self.array[key] = value
+
+    def __add__(self, other):
+        if isinstance(other, Matrix):
+            other = other.array
+        return self.__class__(self.array.__add__(other))
+
+    def __radd__(self, other):
+        if isinstance(other, Matrix):
+            other = other.array
+        return self.__class__(self.array.__radd__(other))
+
+    def __mul__(self, other):
+        if isinstance(other, Matrix):
+            other = other.array
+        return self.__class__(self.array.__mul__(other))
+
+    def __rmul__(self, other):
+        if isinstance(other, Matrix):
+            other = other.array
+        return self.__class__(self.array.__rmul__(other))
+
+    def __truediv__(self, other):
+        if isinstance(other, Matrix):
+            other = other.array
+        return self.__class__(self.array.__truediv__(other))
+
+    def __repr__(self):
+        return f"<Matrix at 0x{id(self):x} {self.shape} {self.dtype}>"
+
+    def __str__(self):
+        return str(self.array)
+
+    def __float__(self):
+        return self.array.__float__()
+
+    def __complex__(self):
+        return self.array.__complex__()
+
+
+def zeros(shape, dtype=None):
+    if dtype is None:
+        dtype = backend.real_dtype
+    return Matrix(np.zeros(shape), dtype=dtype)
+
+
+def eye(N, M=None, dtype=None):
+    if dtype is None:
+        dtype = backend.real_dtype
+    return Matrix(np.eye(N, M), dtype=dtype)
+
+
+def ones(shape, dtype=None):
+    if dtype is None:
+        dtype = backend.real_dtype
+    return Matrix(np.ones(shape), dtype=dtype)
+
+
+def einsum(subscripts, *operands):
+    return Matrix(np.einsum(subscripts, *[o.array for o in operands]))
+
+
+def tensordot(a: Union[Matrix, np.ndarray], b: Union[Matrix, np.ndarray, xp.ndarray], axes) -> xp.ndarray:
+    return xp.tensordot(asxp(a), asxp(b), axes)
+
+
+def moveaxis(a: Matrix, source, destination):
+    return Matrix(np.moveaxis(a.array, source, destination))
+
+
+def vstack(tup):
+    return Matrix(np.vstack([m.array for m in tup]))
+
+
+def dstack(tup):
+    return Matrix(np.dstack([m.array for m in tup]))
+
+
+def concatenate(arrays, axis=None):
+    return Matrix(np.concatenate([m.array for m in arrays], axis))
+
+
+# can only use numpy for now. see gh-cupy-1946
+def allclose(a, b, rtol=1.0e-5, atol=1.0e-8):
+    if isinstance(a, Matrix):
+        a = a.array
+    else:
+        a = np.asarray(a)
+    if isinstance(b, Matrix):
+        b = b.array
+    else:
+        b = np.asarray(b)
+    return np.allclose(a, b, rtol=rtol, atol=atol)
+
+
+def multi_tensor_contract(path, *operands: [List[Union[Matrix, np.ndarray, xp.ndarray]]]):
+    """
+    ipath[0] is the index of the mat
+    ipaht[1] is the contraction index
+    oeprands is the arrays
+
+    For example:  in mpompsmat.py
+    path = [([0, 1],"fdla, abc -> fdlbc")   ,\
+            ([2, 0],"fdlbc, gdeb -> flcge") ,\
+            ([1, 0],"flcge, helc -> fgh")]
+    outtensor = tensorlib.multi_tensor_contract(path, MPSconj[isite], intensor,
+            MPO[isite], MPS[isite])
+    """
+
+    operands = list(operands)
+    for ipath in path:
+
+        input_str, results_str = ipath[1].split("->")
+        input_str = input_str.split(",")
+        input_str = [x.replace(" ", "") for x in input_str]
+        results_set = set(results_str)
+        inputs_set = set(input_str[0] + input_str[1])
+        idx_removed = inputs_set - (inputs_set & results_set)
+
+        tmpmat = pair_tensor_contract(
+            operands[ipath[0][0]],
+            input_str[0],
+            operands[ipath[0][1]],
+            input_str[1],
+            idx_removed,
+        )
+
+        for x in sorted(ipath[0], reverse=True):
+            del operands[x]
+
+        operands.append(tmpmat)
+
+    return operands[0]
+
+
+def pair_tensor_contract(
+    view_left: Union[Matrix, np.ndarray, xp.ndarray],
+    input_left,
+    view_right: Union[Matrix, np.ndarray, xp.ndarray],
+    input_right,
+    idx_removed,
+):
+    # Find indices to contract over
+    left_pos, right_pos = (), ()
+    for s in idx_removed:
+        left_pos += (input_left.find(s),)
+        right_pos += (input_right.find(s),)
+    return tensordot(view_left, view_right, axes=(left_pos, right_pos))
+
+
+def asnumpy(array: Union[np.ndarray, xp.ndarray, Matrix]) -> np.ndarray:
+    if array is None:
+        return None
+    if isinstance(array, Matrix):
+        return array.array
+    if not USE_GPU:
+        assert isinstance(array, np.ndarray)
+        return array
+    if isinstance(array, np.ndarray):
+        return array
+    stream = xp.cuda.get_current_stream()
+    return xp.asnumpy(array, stream=stream)
+
+
+def asxp(array: Union[np.ndarray, xp.ndarray, Matrix]) -> xp.ndarray:
+    if array is None:
+        return None
+    if isinstance(array, Matrix):
+        array = array.array
+    if not USE_GPU:
+        assert isinstance(array, np.ndarray)
+        return array
+    return xp.asarray(array)
```

### Comparing `renormalizer-0.0.8/renormalizer/mps/mpdm.py` & `renormalizer-0.0.9/renormalizer/mps/mpdm.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-# -*- coding: utf-8 -*-
-
-import logging
-
-import numpy as np
-
-from renormalizer.mps.backend import xp
-from renormalizer.mps.matrix import tensordot
-from renormalizer.mps.svd_qn import add_outer
-from renormalizer.mps import Mpo, Mps
-
-logger = logging.getLogger(__name__)
-
-# MPS first. `digest`, `metacopy`
-class MpDm(Mps, Mpo):
-    @classmethod
-    def random(cls, mpo, qntot, m_max, percent=0):
-        # avoid misuse to produce mps
-        raise ValueError("MpDm don't have to produce random state")
-
-    @classmethod
-    def ground_state(cls, model, max_entangled):
-        raise ValueError(
-            "Use max_entangled_ex or max_entangled_gs for matrix product density matrix"
-        )
-
-    @classmethod
-    def from_mps(cls, mps: Mps):
-        mpo = cls()
-        mpo.model = mps.model
-        for ms in mps:
-            mo = np.zeros(tuple([ms.shape[0]] + [ms.shape[1]] * 2 + [ms.shape[2]]))
-            for iaxis in range(ms.shape[1]):
-                mo[:, iaxis, iaxis, :] = ms[:, iaxis, :].array
-            mpo.append(mo)
-
-        mpo.coeff = mps.coeff
-
-        mpo.optimize_config = mps.optimize_config
-        mpo.evolve_config = mps.evolve_config
-        mpo.compress_add = mps.compress_add
-
-        mpo.qn = [qn.copy() for qn in mps.qn]
-        mpo.qntot = mps.qntot
-        mpo.qnidx = mps.qnidx
-        mpo.to_right = mps.to_right
-        mpo.compress_config = mps.compress_config.copy()
-        return mpo
-
-    @classmethod
-    def from_dense(cls, model, wfn: np.ndarray):
-        raise NotImplementedError
-
-    @classmethod
-    def max_entangled_ex(cls, model, normalize=True):
-        """
-        T = \\infty locally maximal entangled EX state
-        """
-        mps = Mps.ground_state(model, max_entangled=True)
-        # the creation operator \\sum_i a^\\dagger_i
-        ex_mpo = Mpo.onsite(model, r"a^\dagger")
-
-        ex_mps = ex_mpo @ mps
-        if normalize:
-            ex_mps.normalize("mps_and_coeff")
-        return cls.from_mps(ex_mps)
-
-    @classmethod
-    def max_entangled_gs(cls, model) -> "MpDm":
-        return cls.from_mps(Mps.ground_state(model, max_entangled=True))
-
-    def _get_sigmaqn(self, idx):
-        array_up = self.model.basis[idx].sigmaqn
-        array_down = np.zeros_like(array_up)
-        return add_outer(array_up, array_down)
-
-    def evolve_exact(self, h_mpo, evolve_dt, space):
-        MPOprop = Mpo.exact_propagator(
-            self.model, -1.0j * evolve_dt, space=space, shift=-h_mpo.offset
-        )
-        # Mpdm is applied on the propagator, different from base method
-        new_mpdm = self.apply(MPOprop, canonicalise=True)
-        new_mpdm.coeff *= np.exp(-1.0j * h_mpo.offset * evolve_dt)
-        return new_mpdm
-
-    def todense(self):
-        # explicitly call to MPO because MPS is firstly inherited
-        return Mpo.todense(self)
-
-    @property
-    def is_mps(self):
-        return False
-
-    @property
-    def is_mpo(self):
-        return False
-
-    @property
-    def is_mpdm(self):
-        return True
-
-    def _expectation_path(self):
-        #       e
-        #       |
-        # S--a--S--f--S
-        # |     |     |
-        # |     d     |
-        # |     |     |
-        # O--b--O--h--O
-        # |     |     |
-        # |     g     |
-        # |     |     |
-        # S--c--S--j--S
-        #       |
-        #       e
-        path = [
-            ([0, 1], "abc, cgej -> abgej"),
-            ([3, 0], "abgej, bdgh -> aejdh"),
-            ([2, 0], "aejdh, adef -> jhf"),
-            ([1, 0], "jhf, fhj -> "),
-        ]
-        return path
-
-    def conj_trans(self):
-        raise NotImplementedError
-        logger.warning("using conj_trans on mpdm leads to dummy qn")
-        new_mpdm: "MpDmBase" = super().conj_trans()
-        new_mpdm.coeff = new_mpdm.coeff.conjugate()
-        return new_mpdm
-
-    def apply(self, mp, canonicalise=False) -> "MpDmBase":
-        # Note usually mp is an mpo
-        assert not mp.is_mps
-        new_mpdm = self.metacopy()
-        if mp.is_complex:
-            new_mpdm.to_complex(inplace=True)
-        # todo: also duplicate with MPO apply. What to do???
-        for i, (mt_self, mt_other) in enumerate(zip(self, mp)):
-            assert mt_self.shape[2] == mt_other.shape[1]
-            # mt=np.einsum("apqb,cqrd->acprbd",mt_s,mt_o)
-            mt = xp.moveaxis(
-                tensordot(mt_self.array, mt_other.array, axes=([2], [1])),
-                [-3, -2],
-                [1, 3],
-            )
-            mt = mt.reshape(
-                (
-                    mt_self.shape[0] * mt_other.shape[0],
-                    mt_self.shape[1],
-                    mt_other.shape[2],
-                    mt_self.shape[-1] * mt_other.shape[-1],
-                )
-            )
-            new_mpdm[i] = mt
-        qn = mp.dummy_qn
-        new_mpdm.qn = [
-            add_outer(np.array(qn_o), np.array(qn_m)).reshape(-1, qn_o.shape[1])
-            for qn_o, qn_m in zip(self.qn, qn)
-        ]
-        if canonicalise:
-            new_mpdm.canonicalise()
-        return new_mpdm
+# -*- coding: utf-8 -*-
+
+import logging
+
+import numpy as np
+
+from renormalizer.mps.backend import xp
+from renormalizer.mps.matrix import tensordot
+from renormalizer.mps.svd_qn import add_outer
+from renormalizer.mps import Mpo, Mps
+
+logger = logging.getLogger(__name__)
+
+# MPS first. `digest`, `metacopy`
+class MpDm(Mps, Mpo):
+    @classmethod
+    def random(cls, mpo, qntot, m_max, percent=0):
+        # avoid misuse to produce mps
+        raise ValueError("MpDm don't have to produce random state")
+
+    @classmethod
+    def ground_state(cls, model, max_entangled):
+        raise ValueError(
+            "Use max_entangled_ex or max_entangled_gs for matrix product density matrix"
+        )
+
+    @classmethod
+    def from_mps(cls, mps: Mps):
+        mpo = cls()
+        mpo.model = mps.model
+        for ms in mps:
+            mo = np.zeros(tuple([ms.shape[0]] + [ms.shape[1]] * 2 + [ms.shape[2]]))
+            for iaxis in range(ms.shape[1]):
+                mo[:, iaxis, iaxis, :] = ms[:, iaxis, :].array
+            mpo.append(mo)
+
+        mpo.coeff = mps.coeff
+
+        mpo.optimize_config = mps.optimize_config
+        mpo.evolve_config = mps.evolve_config
+        mpo.compress_add = mps.compress_add
+
+        mpo.qn = [qn.copy() for qn in mps.qn]
+        mpo.qntot = mps.qntot
+        mpo.qnidx = mps.qnidx
+        mpo.to_right = mps.to_right
+        mpo.compress_config = mps.compress_config.copy()
+        return mpo
+
+    @classmethod
+    def from_dense(cls, model, wfn: np.ndarray):
+        raise NotImplementedError
+
+    @classmethod
+    def max_entangled_ex(cls, model, normalize=True):
+        """
+        T = \\infty locally maximal entangled EX state
+        """
+        mps = Mps.ground_state(model, max_entangled=True)
+        # the creation operator \\sum_i a^\\dagger_i
+        ex_mpo = Mpo.onsite(model, r"a^\dagger")
+
+        ex_mps = ex_mpo @ mps
+        if normalize:
+            ex_mps.normalize("mps_and_coeff")
+        return cls.from_mps(ex_mps)
+
+    @classmethod
+    def max_entangled_gs(cls, model) -> "MpDm":
+        return cls.from_mps(Mps.ground_state(model, max_entangled=True))
+
+    def _get_sigmaqn(self, idx):
+        array_up = self.model.basis[idx].sigmaqn
+        array_down = np.zeros_like(array_up)
+        return add_outer(array_up, array_down)
+
+    def evolve_exact(self, h_mpo, evolve_dt, space):
+        MPOprop = Mpo.exact_propagator(
+            self.model, -1.0j * evolve_dt, space=space, shift=-h_mpo.offset
+        )
+        # Mpdm is applied on the propagator, different from base method
+        new_mpdm = self.apply(MPOprop, canonicalise=True)
+        new_mpdm.coeff *= np.exp(-1.0j * h_mpo.offset * evolve_dt)
+        return new_mpdm
+
+    def todense(self):
+        # explicitly call to MPO because MPS is firstly inherited
+        return Mpo.todense(self)
+
+    @property
+    def is_mps(self):
+        return False
+
+    @property
+    def is_mpo(self):
+        return False
+
+    @property
+    def is_mpdm(self):
+        return True
+
+    def _expectation_path(self):
+        #       e
+        #       |
+        # S--a--S--f--S
+        # |     |     |
+        # |     d     |
+        # |     |     |
+        # O--b--O--h--O
+        # |     |     |
+        # |     g     |
+        # |     |     |
+        # S--c--S--j--S
+        #       |
+        #       e
+        path = [
+            ([0, 1], "abc, cgej -> abgej"),
+            ([3, 0], "abgej, bdgh -> aejdh"),
+            ([2, 0], "aejdh, adef -> jhf"),
+            ([1, 0], "jhf, fhj -> "),
+        ]
+        return path
+
+    def conj_trans(self):
+        raise NotImplementedError
+        logger.warning("using conj_trans on mpdm leads to dummy qn")
+        new_mpdm: "MpDmBase" = super().conj_trans()
+        new_mpdm.coeff = new_mpdm.coeff.conjugate()
+        return new_mpdm
+
+    def apply(self, mp, canonicalise=False) -> "MpDmBase":
+        # Note usually mp is an mpo
+        assert not mp.is_mps
+        new_mpdm = self.metacopy()
+        if mp.is_complex:
+            new_mpdm.to_complex(inplace=True)
+        # todo: also duplicate with MPO apply. What to do???
+        for i, (mt_self, mt_other) in enumerate(zip(self, mp)):
+            assert mt_self.shape[2] == mt_other.shape[1]
+            # mt=np.einsum("apqb,cqrd->acprbd",mt_s,mt_o)
+            mt = xp.moveaxis(
+                tensordot(mt_self.array, mt_other.array, axes=([2], [1])),
+                [-3, -2],
+                [1, 3],
+            )
+            mt = mt.reshape(
+                (
+                    mt_self.shape[0] * mt_other.shape[0],
+                    mt_self.shape[1],
+                    mt_other.shape[2],
+                    mt_self.shape[-1] * mt_other.shape[-1],
+                )
+            )
+            new_mpdm[i] = mt
+        qn = mp.dummy_qn
+        new_mpdm.qn = [
+            add_outer(np.array(qn_o), np.array(qn_m)).reshape(-1, qn_o.shape[1])
+            for qn_o, qn_m in zip(self.qn, qn)
+        ]
+        if canonicalise:
+            new_mpdm.canonicalise()
+        return new_mpdm
```

### Comparing `renormalizer-0.0.8/renormalizer/mps/mpo.py` & `renormalizer-0.0.9/renormalizer/mps/mpo.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,485 +1,485 @@
-import logging
-import itertools
-from copy import deepcopy
-from typing import List, Union
-
-import numpy as np
-import scipy
-import scipy.sparse
-
-from renormalizer.model import Model, HolsteinModel
-from renormalizer.mps.backend import xp
-from renormalizer.mps.matrix import moveaxis, tensordot
-from renormalizer.mps.mp import MatrixProduct
-from renormalizer.mps.svd_qn import add_outer
-from renormalizer.mps import svd_qn
-from renormalizer.mps.lib import update_cv
-from renormalizer.mps.symbolic_mpo import construct_symbolic_mpo, _terms_to_table, symbolic_mo_to_numeric_mo, swap_site
-from renormalizer.utils import Quantity
-from renormalizer.model.op import Op
-from renormalizer.utils.elementop import (
-    construct_ph_op_dict,
-)
-
-
-logger = logging.getLogger(__name__)
-
-
-class Mpo(MatrixProduct):
-    """
-    Matrix product operator (MPO)
-    """
-
-    @classmethod
-    def exact_propagator(cls, model: HolsteinModel, x, space="GS", shift=0.0):
-        """
-        construct the GS space propagator e^{xH} exact MPO
-        H=\\sum_{in} \\omega_{in} b^\\dagger_{in} b_{in}
-        fortunately, the H is local. so e^{xH} = e^{xh1}e^{xh2}...e^{xhn}
-        the bond dimension is 1
-        shift is the a constant for H+shift
-        """
-        assert space in ["GS", "EX"]
-
-        mpo = cls()
-        if np.iscomplex(x):
-            mpo.to_complex(inplace=True)
-        mpo.model = model
-
-        for imol, mol in enumerate(model):
-            if model.scheme < 4:
-                mo = np.eye(2).reshape(1, 2, 2, 1)
-                mpo.append(mo)
-            elif model.scheme == 4:
-                if len(mpo) == model.order[0]:
-                    n = model.mol_num
-                    mpo.append(np.eye(n+1).reshape(1, n+1, n+1, 1))
-            else:
-                assert False
-
-            for ph in mol.ph_list:
-
-                if space == "EX":
-                    ph_pbond = ph.pbond
-                    # construct the matrix exponential by diagonalize the matrix first
-                    phop = construct_ph_op_dict(ph_pbond)
-
-                    h_mo = (
-                        phop[r"b^\dagger b"] * ph.omega[0]
-                        + phop[r"b^\dagger + b"] * ph.term10
-                    )
-
-                    w, v = scipy.linalg.eigh(h_mo)
-                    h_mo = np.diag(np.exp(x * w))
-                    h_mo = v.dot(h_mo)
-                    h_mo = h_mo.dot(v.T)
-                    mo = h_mo.reshape(1, ph_pbond, ph_pbond, 1)
-
-                    mpo.append(mo)
-
-                elif space == "GS":
-                    # for the ground state space
-                    ph_pbond = ph.pbond
-                    d = np.exp(
-                            x
-                            * ph.omega[0]
-                            * np.arange(ph_pbond)
-                        )
-                    mo = np.diag(d).reshape(1, ph_pbond, ph_pbond, 1)
-                    mpo.append(mo)
-                else:
-                    assert False
-        # shift the H by plus a constant
-
-        mpo.qn = [np.zeros((1, model.qn_size), dtype=int)] * (len(mpo) + 1)
-        mpo.qnidx = len(mpo) - 1
-        mpo.qntot = np.zeros(model.qn_size, dtype=int)
-
-        # np.exp(shift * x) is usually very large
-        mpo = mpo.scale(np.exp(shift * x), inplace=True)
-
-        return mpo
-
-    @classmethod
-    def onsite(cls, model: Model, opera, dipole=False, dof_set=None):
-        if dof_set is None:
-            if model.n_edofs == 0:
-                raise ValueError("No electronic DoF present in the model.")
-            dof_set = model.e_dofs
-        ops = []
-        for idx in dof_set:
-            if dipole:
-                factor = model.dipole[idx]
-            else:
-                factor = 1.
-            ops.append(Op(opera, idx, factor))
-
-        return cls(model, ops)
-
-    @classmethod
-    def ph_onsite(cls, model: HolsteinModel, opera: str, mol_idx:int, ph_idx=0):
-        assert opera in ["b", r"b^\dagger", r"b^\dagger b"]
-        if not isinstance(model, HolsteinModel):
-            raise TypeError("ph_onsite only supports HolsteinModel")
-        return cls(model, Op(opera, (mol_idx, ph_idx)))
-
-    @classmethod
-    def intersite(cls, model: HolsteinModel, e_opera: dict, ph_opera: dict, scale:
-            Quantity=Quantity(1.)):
-        r""" construct the inter site MPO
-        
-        Parameters
-        ----------
-        model : HolsteinModel
-            the molecular information
-        e_opera:
-            the electronic operators. {imol: operator}, such as {1:"a", 3:r"a^\dagger"}
-        ph_opera:
-            the vibrational operators. {(imol, iph): operator}, such as {(0,5):"b"}
-        scale: Quantity
-            scalar to scale the mpo
-
-        Note
-        -----
-        the operator index starts from 0,1,2...
-        
-        """
-
-        ops = []
-        for e_key, e_op in e_opera.items():
-            ops.append(Op(e_op, e_key))
-        for v_key, v_op in ph_opera.items():
-            ops.append(Op(v_op, v_key))
-        op = scale.as_au() * Op.product(ops)
-        return cls(model, op)
-
-    @classmethod
-    def finiteT_cv(cls, model, nexciton, m_max, spectratype, percent=1.0):
-        np.random.seed(0)
-
-        X = cls()
-        X.model = model
-        if spectratype == "abs":
-            # quantum number index, |1><0|
-            tag_1, tag_2 = 0, 1
-        elif spectratype == "emi":
-            # quantum number index, |0><1|
-            tag_1, tag_2 = 1, 0
-        X.qn = [[[0, 0]]]
-        for ix in range(model.nsite - 1):
-            X.qn.append(None)
-        X.qn.append([[0, 0]])
-        dim_list = [1]
-
-        for ix in range(model.nsite - 1):
-            sigmaqn = model.basis[ix].sigmaqn
-            sigmaqn = np.array(list(itertools.product(sigmaqn, repeat=2)))
-            qn1 = np.add.outer(np.array(X.qn[ix])[:, 0], sigmaqn[:, 0]).ravel()
-            qn2 = np.add.outer(np.array(X.qn[ix])[:, 1], sigmaqn[:, 1]).ravel()
-            qnbig = np.stack([qn1, qn2], axis=1)
-            # print('qnbig', qnbig)
-            u_set = []
-            s_set = []
-            qnset = []
-            if spectratype != "conductivity":
-                fq = list(itertools.chain.from_iterable([y[tag_1]] for y in qnbig))
-                for iblock in range(min(fq), nexciton+1):
-                    indices = [i for i, y in enumerate(qnbig) if
-                               ((y[tag_1] == iblock) and (y[tag_2] == 0))]
-                    if len(indices) != 0:
-                        np.random.seed(0)
-                        a: np.ndarray = np.random.random([len(indices), len(indices)]) - 0.5
-                        a = a + a.T
-                        s, u = scipy.linalg.eigh(a=a)
-                        u_set.append(svd_qn.blockrecover(indices, u, len(qnbig)))
-                        s_set.append(s)
-                        if spectratype == "abs":
-                            qnset += [iblock, 0] * len(indices)
-                        elif spectratype == "emi":
-                            qnset += [0, iblock] * len(indices)
-            else:
-                fq1 = list(itertools.chain.from_iterable([y[0]] for y in qnbig))
-                fq2 = list(itertools.chain.from_iterable([y[1]] for y in qnbig))
-                # print('fq1, fq2', fq1, fq2)
-                for iblock in range(min(fq1), nexciton+1):
-                    for jblock in range(min(fq2), nexciton+1):
-                        # print('iblock', iblock, jblock)
-                        indices = [i for i, y in enumerate(qnbig) if
-                                   ((y[0] == iblock) and (y[1] == jblock))]
-                        # print('indices', indices)
-                        if len(indices) != 0:
-                            a: np.ndarray = np.random.random([len(indices), len(indices)]) - 0.5
-                            a = a + a.T
-                            s, u = scipy.linalg.eigh(a=a)
-                            u_set.append(svd_qn.blockrecover(indices, u, len(qnbig)))
-                            s_set.append(s)
-                            qnset += [iblock, jblock] * len(indices)
-                            # print('iblock', iblock)
-            list_qnset = []
-            for i in range(0, len(qnset), 2):
-                list_qnset.append([qnset[i], qnset[i + 1]])
-            qnset = list_qnset
-            # print('qnset', qnset)
-            u_set = np.concatenate(u_set, axis=1)
-            s_set = np.concatenate(s_set)
-            # print('uset', u_set.shape)
-            # print('s_set', s_set.shape)
-            x, xdim, xqn, compx = update_cv(u_set, s_set, qnset, None, nexciton, m_max, spectratype, percent=percent)
-            dim_list.append(xdim)
-            X.qn[ix + 1] = xqn
-            x = x.reshape(dim_list[-2], model.pbond_list[ix], model.pbond_list[ix], dim_list[ix + 1])
-            X.append(x)
-        dim_list.append(1)
-        X.append(np.random.random([dim_list[-2], model.pbond_list[-1],
-                                   model.pbond_list[-1], dim_list[-1]]))
-        X.qnidx = len(X) - 1
-        X.to_right = False
-        X.qntot = nexciton
-        # print('dim', [X[i].shape for i in range(len(X))])
-        return X
-
-    @classmethod
-    def identity(cls, model: Model):
-        mpo = cls()
-        mpo.model = model
-        for p in model.pbond_list:
-            mpo.append(np.eye(p).reshape(1, p, p, 1))
-        mpo.build_empty_qn()
-        return mpo
-
-    def __init__(self, model: Model = None, terms: Union[Op, List[Op]] = None, offset: Quantity = Quantity(0), ):
-
-        """
-        todo: document
-        """
-        super(Mpo, self).__init__()
-        # leave the possibility to construct MPO by hand
-        if model is None:
-            return
-        if not isinstance(offset, Quantity):
-            raise ValueError(f"offset must be Quantity object. Got {offset} of {type(offset)}.")
-
-        self.offset = offset.as_au()
-        if terms is None:
-            terms = model.ham_terms
-        elif isinstance(terms, Op):
-            terms = [terms]
-
-        if len(terms) == 0:
-            raise ValueError("Terms contain nothing.")
-        terms = model.check_operator_terms(terms)
-        if len(terms) == 0:
-            raise ValueError("Terms all have factor 0.")
-
-        table, factor = _terms_to_table(model, terms, -self.offset)
-
-        self.dtype = factor.dtype
-
-        mpo_symbol, self.qn, self.qntot, self.qnidx, self.symbolic_out_ops_list, self.primary_ops = construct_symbolic_mpo(table, factor)
-        # print(_format_symbolic_mpo(mpo_symbol))
-        self.model = model
-        self.to_right = False
-
-        # evaluate the symbolic mpo
-        assert model.basis is not None
-
-        for impo, mo in enumerate(mpo_symbol):
-            mo_mat = symbolic_mo_to_numeric_mo(model.basis[impo], mo, self.dtype)
-            self.append(mo_mat)
-
-
-    def _get_sigmaqn(self, idx):
-        array_up = self.model.basis[idx].sigmaqn
-        return add_outer(array_up, -array_up)
-
-    @property
-    def is_mps(self):
-        return False
-
-    @property
-    def is_mpo(self):
-        return True
-
-    @property
-    def is_mpdm(self):
-        return False
-
-    def metacopy(self):
-        new = super().metacopy()
-        # some mpo may not have these things
-        attrs = ["scheme", "offset", "symbolic_out_ops_list", "primary_ops"]
-        for attr in attrs:
-            if hasattr(self, attr):
-                setattr(new, attr, deepcopy(getattr(self, attr)))
-        return new
-
-    @property
-    def dummy_qn(self):
-        return [np.zeros((dim, self.model.qn_size), dtype=int) for dim in self.bond_dims]
-
-    @property
-    def digest(self):
-        return np.array([mt.var() for mt in self]).var()
-
-    def promote_mt_type(self, mp):
-        if self.is_complex and not mp.is_complex:
-            mp.to_complex(inplace=True)
-        return mp
-
-    def apply(self, mp: MatrixProduct, canonicalise: bool=False) -> MatrixProduct:
-        # todo: use meta copy to save time, could be subtle when complex type is involved
-        # todo: inplace version (saved memory and can be used in `hybrid_exact_propagator`)
-        # the model is the same as the mps.model
-        new_mps = self.promote_mt_type(mp.copy())
-        if mp.is_mps:
-            # mpo x mps
-            for i, (mt_self, mt_other) in enumerate(zip(self, mp)):
-                assert mt_self.shape[2] == mt_other.shape[1]
-                # mt=np.einsum("apqb,cqd->acpbd",mpo[i],mps[i])
-                mt = xp.moveaxis(
-                    tensordot(mt_self.array, mt_other.array, axes=([2], [1])), 3, 1
-                )
-                mt = mt.reshape(
-                    (
-                        mt_self.shape[0] * mt_other.shape[0],
-                        mt_self.shape[1],
-                        mt_self.shape[-1] * mt_other.shape[-1],
-                    )
-                )
-                new_mps[i] = mt
-        elif mp.is_mpo or mp.is_mpdm:
-            # mpo x mpo
-            for i, (mt_self, mt_other) in enumerate(zip(self, mp)):
-                assert mt_self.shape[2] == mt_other.shape[1]
-                # mt=np.einsum("apqb,cqrd->acprbd",mt_s,mt_o)
-                mt = xp.moveaxis(
-                    tensordot(mt_self.array, mt_other.array, axes=([2], [1])),
-                    [-3, -2],
-                    [1, 3],
-                )
-                mt = mt.reshape(
-                    (
-                        mt_self.shape[0] * mt_other.shape[0],
-                        mt_self.shape[1],
-                        mt_other.shape[2],
-                        mt_self.shape[-1] * mt_other.shape[-1],
-                    )
-                )
-                new_mps[i] = mt
-        else:
-            assert False
-        orig_idx = new_mps.qnidx
-        new_mps.move_qnidx(self.qnidx)
-        new_mps.qn = [
-            add_outer(np.array(qn_o), np.array(qn_m)).reshape(-1, qn_o.shape[1])
-            for qn_o, qn_m in zip(self.qn, new_mps.qn)
-        ]
-        new_mps.qntot += self.qntot
-        new_mps.move_qnidx(orig_idx)
-        # concerns about whether to canonicalise:
-        # * canonicalise helps to keep mps in a truly canonicalised state
-        # * canonicalise comes with a cost. Unnecessary canonicalise (for example in P&C evolution and
-        #   expectation calculation) hampers performance.
-        if canonicalise:
-            new_mps.canonicalise()
-        return new_mps
-
-    def contract(self, mps, algo="svd"):
-        r""" an approximation of mpo @ mps/mpdm/mpo
-        
-        Parameters
-        ----------
-        mps : `Mps`, `Mpo`, `MpDm`
-        algo: str, optional
-            The algorithm to compress mpo @ mps/mpdm/mpo.  It could be ``svd``
-            (default) and ``variational``. 
-        
-        Returns
-        -------
-        new_mps : `Mps`
-            an approximation of mpo @ mps/mpdm/mpo. The input ``mps`` is not
-            overwritten.
-
-        See Also
-        --------
-        renormalizer.mps.mp.MatrixProduct.compress : svd compression.
-        renormalizer.mps.mp.MatrixProduct.variational_compress : variational
-            compression.
-
-
-        """
-        if algo == "svd":
-            # mapply->canonicalise->compress
-            new_mps = self.apply(mps)
-            new_mps.canonicalise()
-            new_mps.compress()
-        elif algo == "variational":
-            new_mps = mps.variational_compress(self)
-        else:
-            assert False
-
-        return new_mps
-
-    def try_swap_site(self, new_model: Model, swap_jw: bool):
-        # in place swapping.
-        # if swap_jw is set to True, then self.primary_ops is modified in place
-        diffs = []
-        for i, (b1, b2) in enumerate(zip(self.model.basis, new_model.basis)):
-            if b1.dofs != b2.dofs:
-                diffs.append(i)
-        if len(diffs) == 0:
-            logger.debug("MPO: No need to swap")
-            return
-        assert len(diffs) == 2
-        i, j = min(diffs), max(diffs)
-        assert j - i == 1
-        logger.debug(f"MPO: swaping {i} and {j}")
-        # although usually the `model` of MPO does not store `mpos`
-        new_model.mpos.clear()
-
-        out_ops2, out_ops3, mo1, mo2, qn = swap_site(self.symbolic_out_ops_list[i:i+3], self.primary_ops, swap_jw)
-
-        self.symbolic_out_ops_list[i+1] = out_ops2
-        self.symbolic_out_ops_list[i+2] = out_ops3
-        self.model = new_model
-        self.qn[i+1] = qn
-
-        for impo, mo in zip([i, j], [mo1, mo2]):
-            self[impo] = symbolic_mo_to_numeric_mo(new_model.basis[impo], mo, self.dtype)
-        logger.debug(self)
-
-    def conj_trans(self):
-        new_mpo = self.metacopy()
-        for i in range(new_mpo.site_num):
-            new_mpo[i] = moveaxis(self[i], (1, 2), (2, 1)).conj()
-        new_mpo.qn = [np.array([-i for i in mt_qn]) for mt_qn in new_mpo.qn]
-        return new_mpo
-
-    def todense(self):
-        dim = np.prod(self.pbond_list)
-        if 20000 < dim:
-            raise ValueError("operator too large")
-        res = np.ones((1, 1, 1, 1))
-        for mt in self:
-            dim1 = res.shape[1] * mt.shape[1]
-            dim2 = res.shape[2] * mt.shape[2]
-            dim3 = mt.shape[-1]
-            res = np.tensordot(res, mt.array, axes=1).transpose((0, 1, 3, 2, 4, 5)).reshape(1, dim1, dim2, dim3)
-        return res[0, :, :, 0]
-
-    def is_hermitian(self):
-        full = self.todense()
-        return np.allclose(full.conj().T, full, atol=1e-7)
-
-    def __matmul__(self, other):
-        return self.apply(other)
-
-    @classmethod
-    def from_mp(cls, model, mp):
-        # mpo from matrix product
-        mpo = cls()
-        mpo.model = model
-        for mt in mp:
-            mpo.append(mt)
-        mpo.build_empty_qn()
-        return mpo
+import logging
+import itertools
+from copy import deepcopy
+from typing import List, Union
+
+import numpy as np
+import scipy
+import scipy.sparse
+
+from renormalizer.model import Model, HolsteinModel
+from renormalizer.mps.backend import xp
+from renormalizer.mps.matrix import moveaxis, tensordot
+from renormalizer.mps.mp import MatrixProduct
+from renormalizer.mps.svd_qn import add_outer
+from renormalizer.mps import svd_qn
+from renormalizer.mps.lib import update_cv
+from renormalizer.mps.symbolic_mpo import construct_symbolic_mpo, _terms_to_table, symbolic_mo_to_numeric_mo, swap_site
+from renormalizer.utils import Quantity
+from renormalizer.model.op import Op
+from renormalizer.utils.elementop import (
+    construct_ph_op_dict,
+)
+
+
+logger = logging.getLogger(__name__)
+
+
+class Mpo(MatrixProduct):
+    """
+    Matrix product operator (MPO)
+    """
+
+    @classmethod
+    def exact_propagator(cls, model: HolsteinModel, x, space="GS", shift=0.0):
+        """
+        construct the GS space propagator e^{xH} exact MPO
+        H=\\sum_{in} \\omega_{in} b^\\dagger_{in} b_{in}
+        fortunately, the H is local. so e^{xH} = e^{xh1}e^{xh2}...e^{xhn}
+        the bond dimension is 1
+        shift is the a constant for H+shift
+        """
+        assert space in ["GS", "EX"]
+
+        mpo = cls()
+        if np.iscomplex(x):
+            mpo.to_complex(inplace=True)
+        mpo.model = model
+
+        for imol, mol in enumerate(model):
+            if model.scheme < 4:
+                mo = np.eye(2).reshape(1, 2, 2, 1)
+                mpo.append(mo)
+            elif model.scheme == 4:
+                if len(mpo) == model.order[0]:
+                    n = model.mol_num
+                    mpo.append(np.eye(n+1).reshape(1, n+1, n+1, 1))
+            else:
+                assert False
+
+            for ph in mol.ph_list:
+
+                if space == "EX":
+                    ph_pbond = ph.pbond
+                    # construct the matrix exponential by diagonalize the matrix first
+                    phop = construct_ph_op_dict(ph_pbond)
+
+                    h_mo = (
+                        phop[r"b^\dagger b"] * ph.omega[0]
+                        + phop[r"b^\dagger + b"] * ph.term10
+                    )
+
+                    w, v = scipy.linalg.eigh(h_mo)
+                    h_mo = np.diag(np.exp(x * w))
+                    h_mo = v.dot(h_mo)
+                    h_mo = h_mo.dot(v.T)
+                    mo = h_mo.reshape(1, ph_pbond, ph_pbond, 1)
+
+                    mpo.append(mo)
+
+                elif space == "GS":
+                    # for the ground state space
+                    ph_pbond = ph.pbond
+                    d = np.exp(
+                            x
+                            * ph.omega[0]
+                            * np.arange(ph_pbond)
+                        )
+                    mo = np.diag(d).reshape(1, ph_pbond, ph_pbond, 1)
+                    mpo.append(mo)
+                else:
+                    assert False
+        # shift the H by plus a constant
+
+        mpo.qn = [np.zeros((1, model.qn_size), dtype=int)] * (len(mpo) + 1)
+        mpo.qnidx = len(mpo) - 1
+        mpo.qntot = np.zeros(model.qn_size, dtype=int)
+
+        # np.exp(shift * x) is usually very large
+        mpo = mpo.scale(np.exp(shift * x), inplace=True)
+
+        return mpo
+
+    @classmethod
+    def onsite(cls, model: Model, opera, dipole=False, dof_set=None):
+        if dof_set is None:
+            if model.n_edofs == 0:
+                raise ValueError("No electronic DoF present in the model.")
+            dof_set = model.e_dofs
+        ops = []
+        for idx in dof_set:
+            if dipole:
+                factor = model.dipole[idx]
+            else:
+                factor = 1.
+            ops.append(Op(opera, idx, factor))
+
+        return cls(model, ops)
+
+    @classmethod
+    def ph_onsite(cls, model: HolsteinModel, opera: str, mol_idx:int, ph_idx=0):
+        assert opera in ["b", r"b^\dagger", r"b^\dagger b"]
+        if not isinstance(model, HolsteinModel):
+            raise TypeError("ph_onsite only supports HolsteinModel")
+        return cls(model, Op(opera, (mol_idx, ph_idx)))
+
+    @classmethod
+    def intersite(cls, model: HolsteinModel, e_opera: dict, ph_opera: dict, scale:
+            Quantity=Quantity(1.)):
+        r""" construct the inter site MPO
+        
+        Parameters
+        ----------
+        model : HolsteinModel
+            the molecular information
+        e_opera:
+            the electronic operators. {imol: operator}, such as {1:"a", 3:r"a^\dagger"}
+        ph_opera:
+            the vibrational operators. {(imol, iph): operator}, such as {(0,5):"b"}
+        scale: Quantity
+            scalar to scale the mpo
+
+        Note
+        -----
+        the operator index starts from 0,1,2...
+        
+        """
+
+        ops = []
+        for e_key, e_op in e_opera.items():
+            ops.append(Op(e_op, e_key))
+        for v_key, v_op in ph_opera.items():
+            ops.append(Op(v_op, v_key))
+        op = scale.as_au() * Op.product(ops)
+        return cls(model, op)
+
+    @classmethod
+    def finiteT_cv(cls, model, nexciton, m_max, spectratype, percent=1.0):
+        np.random.seed(0)
+
+        X = cls()
+        X.model = model
+        if spectratype == "abs":
+            # quantum number index, |1><0|
+            tag_1, tag_2 = 0, 1
+        elif spectratype == "emi":
+            # quantum number index, |0><1|
+            tag_1, tag_2 = 1, 0
+        X.qn = [[[0, 0]]]
+        for ix in range(model.nsite - 1):
+            X.qn.append(None)
+        X.qn.append([[0, 0]])
+        dim_list = [1]
+
+        for ix in range(model.nsite - 1):
+            sigmaqn = model.basis[ix].sigmaqn
+            sigmaqn = np.array(list(itertools.product(sigmaqn, repeat=2)))
+            qn1 = np.add.outer(np.array(X.qn[ix])[:, 0], sigmaqn[:, 0]).ravel()
+            qn2 = np.add.outer(np.array(X.qn[ix])[:, 1], sigmaqn[:, 1]).ravel()
+            qnbig = np.stack([qn1, qn2], axis=1)
+            # print('qnbig', qnbig)
+            u_set = []
+            s_set = []
+            qnset = []
+            if spectratype != "conductivity":
+                fq = list(itertools.chain.from_iterable([y[tag_1]] for y in qnbig))
+                for iblock in range(min(fq), nexciton+1):
+                    indices = [i for i, y in enumerate(qnbig) if
+                               ((y[tag_1] == iblock) and (y[tag_2] == 0))]
+                    if len(indices) != 0:
+                        np.random.seed(0)
+                        a: np.ndarray = np.random.random([len(indices), len(indices)]) - 0.5
+                        a = a + a.T
+                        s, u = scipy.linalg.eigh(a=a)
+                        u_set.append(svd_qn.blockrecover(indices, u, len(qnbig)))
+                        s_set.append(s)
+                        if spectratype == "abs":
+                            qnset += [iblock, 0] * len(indices)
+                        elif spectratype == "emi":
+                            qnset += [0, iblock] * len(indices)
+            else:
+                fq1 = list(itertools.chain.from_iterable([y[0]] for y in qnbig))
+                fq2 = list(itertools.chain.from_iterable([y[1]] for y in qnbig))
+                # print('fq1, fq2', fq1, fq2)
+                for iblock in range(min(fq1), nexciton+1):
+                    for jblock in range(min(fq2), nexciton+1):
+                        # print('iblock', iblock, jblock)
+                        indices = [i for i, y in enumerate(qnbig) if
+                                   ((y[0] == iblock) and (y[1] == jblock))]
+                        # print('indices', indices)
+                        if len(indices) != 0:
+                            a: np.ndarray = np.random.random([len(indices), len(indices)]) - 0.5
+                            a = a + a.T
+                            s, u = scipy.linalg.eigh(a=a)
+                            u_set.append(svd_qn.blockrecover(indices, u, len(qnbig)))
+                            s_set.append(s)
+                            qnset += [iblock, jblock] * len(indices)
+                            # print('iblock', iblock)
+            list_qnset = []
+            for i in range(0, len(qnset), 2):
+                list_qnset.append([qnset[i], qnset[i + 1]])
+            qnset = list_qnset
+            # print('qnset', qnset)
+            u_set = np.concatenate(u_set, axis=1)
+            s_set = np.concatenate(s_set)
+            # print('uset', u_set.shape)
+            # print('s_set', s_set.shape)
+            x, xdim, xqn, compx = update_cv(u_set, s_set, qnset, None, nexciton, m_max, spectratype, percent=percent)
+            dim_list.append(xdim)
+            X.qn[ix + 1] = xqn
+            x = x.reshape(dim_list[-2], model.pbond_list[ix], model.pbond_list[ix], dim_list[ix + 1])
+            X.append(x)
+        dim_list.append(1)
+        X.append(np.random.random([dim_list[-2], model.pbond_list[-1],
+                                   model.pbond_list[-1], dim_list[-1]]))
+        X.qnidx = len(X) - 1
+        X.to_right = False
+        X.qntot = nexciton
+        # print('dim', [X[i].shape for i in range(len(X))])
+        return X
+
+    @classmethod
+    def identity(cls, model: Model):
+        mpo = cls()
+        mpo.model = model
+        for p in model.pbond_list:
+            mpo.append(np.eye(p).reshape(1, p, p, 1))
+        mpo.build_empty_qn()
+        return mpo
+
+    def __init__(self, model: Model = None, terms: Union[Op, List[Op]] = None, offset: Quantity = Quantity(0), ):
+
+        """
+        todo: document
+        """
+        super(Mpo, self).__init__()
+        # leave the possibility to construct MPO by hand
+        if model is None:
+            return
+        if not isinstance(offset, Quantity):
+            raise ValueError(f"offset must be Quantity object. Got {offset} of {type(offset)}.")
+
+        self.offset = offset.as_au()
+        if terms is None:
+            terms = model.ham_terms
+        elif isinstance(terms, Op):
+            terms = [terms]
+
+        if len(terms) == 0:
+            raise ValueError("Terms contain nothing.")
+        terms = model.check_operator_terms(terms)
+        if len(terms) == 0:
+            raise ValueError("Terms all have factor 0.")
+
+        table, factor = _terms_to_table(model, terms, -self.offset)
+
+        self.dtype = factor.dtype
+
+        mpo_symbol, self.qn, self.qntot, self.qnidx, self.symbolic_out_ops_list, self.primary_ops = construct_symbolic_mpo(table, factor)
+        # print(_format_symbolic_mpo(mpo_symbol))
+        self.model = model
+        self.to_right = False
+
+        # evaluate the symbolic mpo
+        assert model.basis is not None
+
+        for impo, mo in enumerate(mpo_symbol):
+            mo_mat = symbolic_mo_to_numeric_mo(model.basis[impo], mo, self.dtype)
+            self.append(mo_mat)
+
+
+    def _get_sigmaqn(self, idx):
+        array_up = self.model.basis[idx].sigmaqn
+        return add_outer(array_up, -array_up)
+
+    @property
+    def is_mps(self):
+        return False
+
+    @property
+    def is_mpo(self):
+        return True
+
+    @property
+    def is_mpdm(self):
+        return False
+
+    def metacopy(self):
+        new = super().metacopy()
+        # some mpo may not have these things
+        attrs = ["scheme", "offset", "symbolic_out_ops_list", "primary_ops"]
+        for attr in attrs:
+            if hasattr(self, attr):
+                setattr(new, attr, deepcopy(getattr(self, attr)))
+        return new
+
+    @property
+    def dummy_qn(self):
+        return [np.zeros((dim, self.model.qn_size), dtype=int) for dim in self.bond_dims]
+
+    @property
+    def digest(self):
+        return np.array([mt.var() for mt in self]).var()
+
+    def promote_mt_type(self, mp):
+        if self.is_complex and not mp.is_complex:
+            mp.to_complex(inplace=True)
+        return mp
+
+    def apply(self, mp: MatrixProduct, canonicalise: bool=False) -> MatrixProduct:
+        # todo: use meta copy to save time, could be subtle when complex type is involved
+        # todo: inplace version (saved memory and can be used in `hybrid_exact_propagator`)
+        # the model is the same as the mps.model
+        new_mps = self.promote_mt_type(mp.copy())
+        if mp.is_mps:
+            # mpo x mps
+            for i, (mt_self, mt_other) in enumerate(zip(self, mp)):
+                assert mt_self.shape[2] == mt_other.shape[1]
+                # mt=np.einsum("apqb,cqd->acpbd",mpo[i],mps[i])
+                mt = xp.moveaxis(
+                    tensordot(mt_self.array, mt_other.array, axes=([2], [1])), 3, 1
+                )
+                mt = mt.reshape(
+                    (
+                        mt_self.shape[0] * mt_other.shape[0],
+                        mt_self.shape[1],
+                        mt_self.shape[-1] * mt_other.shape[-1],
+                    )
+                )
+                new_mps[i] = mt
+        elif mp.is_mpo or mp.is_mpdm:
+            # mpo x mpo
+            for i, (mt_self, mt_other) in enumerate(zip(self, mp)):
+                assert mt_self.shape[2] == mt_other.shape[1]
+                # mt=np.einsum("apqb,cqrd->acprbd",mt_s,mt_o)
+                mt = xp.moveaxis(
+                    tensordot(mt_self.array, mt_other.array, axes=([2], [1])),
+                    [-3, -2],
+                    [1, 3],
+                )
+                mt = mt.reshape(
+                    (
+                        mt_self.shape[0] * mt_other.shape[0],
+                        mt_self.shape[1],
+                        mt_other.shape[2],
+                        mt_self.shape[-1] * mt_other.shape[-1],
+                    )
+                )
+                new_mps[i] = mt
+        else:
+            assert False
+        orig_idx = new_mps.qnidx
+        new_mps.move_qnidx(self.qnidx)
+        new_mps.qn = [
+            add_outer(np.array(qn_o), np.array(qn_m)).reshape(-1, qn_o.shape[1])
+            for qn_o, qn_m in zip(self.qn, new_mps.qn)
+        ]
+        new_mps.qntot += self.qntot
+        new_mps.move_qnidx(orig_idx)
+        # concerns about whether to canonicalise:
+        # * canonicalise helps to keep mps in a truly canonicalised state
+        # * canonicalise comes with a cost. Unnecessary canonicalise (for example in P&C evolution and
+        #   expectation calculation) hampers performance.
+        if canonicalise:
+            new_mps.canonicalise()
+        return new_mps
+
+    def contract(self, mps, algo="svd"):
+        r""" an approximation of mpo @ mps/mpdm/mpo
+        
+        Parameters
+        ----------
+        mps : `Mps`, `Mpo`, `MpDm`
+        algo: str, optional
+            The algorithm to compress mpo @ mps/mpdm/mpo.  It could be ``svd``
+            (default) and ``variational``. 
+        
+        Returns
+        -------
+        new_mps : `Mps`
+            an approximation of mpo @ mps/mpdm/mpo. The input ``mps`` is not
+            overwritten.
+
+        See Also
+        --------
+        renormalizer.mps.mp.MatrixProduct.compress : svd compression.
+        renormalizer.mps.mp.MatrixProduct.variational_compress : variational
+            compression.
+
+
+        """
+        if algo == "svd":
+            # mapply->canonicalise->compress
+            new_mps = self.apply(mps)
+            new_mps.canonicalise()
+            new_mps.compress()
+        elif algo == "variational":
+            new_mps = mps.variational_compress(self)
+        else:
+            assert False
+
+        return new_mps
+
+    def try_swap_site(self, new_model: Model, swap_jw: bool):
+        # in place swapping.
+        # if swap_jw is set to True, then self.primary_ops is modified in place
+        diffs = []
+        for i, (b1, b2) in enumerate(zip(self.model.basis, new_model.basis)):
+            if b1.dofs != b2.dofs:
+                diffs.append(i)
+        if len(diffs) == 0:
+            logger.debug("MPO: No need to swap")
+            return
+        assert len(diffs) == 2
+        i, j = min(diffs), max(diffs)
+        assert j - i == 1
+        logger.debug(f"MPO: swaping {i} and {j}")
+        # although usually the `model` of MPO does not store `mpos`
+        new_model.mpos.clear()
+
+        out_ops2, out_ops3, mo1, mo2, qn = swap_site(self.symbolic_out_ops_list[i:i+3], self.primary_ops, swap_jw)
+
+        self.symbolic_out_ops_list[i+1] = out_ops2
+        self.symbolic_out_ops_list[i+2] = out_ops3
+        self.model = new_model
+        self.qn[i+1] = qn
+
+        for impo, mo in zip([i, j], [mo1, mo2]):
+            self[impo] = symbolic_mo_to_numeric_mo(new_model.basis[impo], mo, self.dtype)
+        logger.debug(self)
+
+    def conj_trans(self):
+        new_mpo = self.metacopy()
+        for i in range(new_mpo.site_num):
+            new_mpo[i] = moveaxis(self[i], (1, 2), (2, 1)).conj()
+        new_mpo.qn = [np.array([-i for i in mt_qn]) for mt_qn in new_mpo.qn]
+        return new_mpo
+
+    def todense(self):
+        dim = np.prod(self.pbond_list)
+        if 20000 < dim:
+            raise ValueError("operator too large")
+        res = np.ones((1, 1, 1, 1))
+        for mt in self:
+            dim1 = res.shape[1] * mt.shape[1]
+            dim2 = res.shape[2] * mt.shape[2]
+            dim3 = mt.shape[-1]
+            res = np.tensordot(res, mt.array, axes=1).transpose((0, 1, 3, 2, 4, 5)).reshape(1, dim1, dim2, dim3)
+        return res[0, :, :, 0]
+
+    def is_hermitian(self):
+        full = self.todense()
+        return np.allclose(full.conj().T, full, atol=1e-7)
+
+    def __matmul__(self, other):
+        return self.apply(other)
+
+    @classmethod
+    def from_mp(cls, model, mp):
+        # mpo from matrix product
+        mpo = cls()
+        mpo.model = model
+        for mt in mp:
+            mpo.append(mt)
+        mpo.build_empty_qn()
+        return mpo
```

### Comparing `renormalizer-0.0.8/renormalizer/mps/mps.py` & `renormalizer-0.0.9/renormalizer/mps/mps.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,1938 +1,1938 @@
-# -*- encoding: utf-8 -*-
-
-import logging
-from collections import Counter, deque
-from functools import wraps, reduce
-from typing import Union, List, Dict
-import itertools
-
-
-import scipy
-from scipy import stats
-
-from renormalizer.lib import solve_ivp, expm_krylov
-from renormalizer.model import Model, Op, basis as ba
-from renormalizer.mps import svd_qn
-from renormalizer.mps.svd_qn import add_outer, get_qn_mask
-from renormalizer.mps.backend import backend, np, xp
-from renormalizer.mps.lib import (
-    Environ,
-    select_basis,
-    compressed_sum,
-    contract_one_site,
-    cvec2cmat
-)
-from renormalizer.mps.matrix import (
-    multi_tensor_contract,
-    ones,
-    tensordot,
-    Matrix,
-    asnumpy,
-    asxp)
-from renormalizer.mps.mp import MatrixProduct
-from renormalizer.mps.hop_expr import hop_expr
-from renormalizer.mps.mpo import Mpo
-from renormalizer.utils import (
-    OptimizeConfig,
-    CompressCriteria,
-    EvolveConfig,
-    EvolveMethod
-)
-from renormalizer.utils.utils import calc_vn_entropy
-
-logger = logging.getLogger(__name__)
-
-
-def adaptive_tdvp(fun):
-    # evolve t/2 (twice) and t to obtain the O(dt^3) error term in 2nd-order Trotter decomposition
-    # J. Chem. Phys. 146, 174107 (2017)
-
-    @wraps(fun)
-    def adaptive_fun(self: "Mps", mpo, evolve_target_t):
-
-        if not self.evolve_config.adaptive:
-            return fun(self, mpo, evolve_target_t)
-        config: EvolveConfig = self.evolve_config.copy()
-        config.check_valid_dt(evolve_target_t)
-
-        cur_mps = self
-        # prevent bug
-        del self
-
-        # setup some constant
-        p_restart = 0.5  # restart threshold
-        p_min = 0.1  # safeguard for minimal allowed p
-        p_max = 2.  # safeguard for maximal allowed p
-
-        evolved_t = 0
-
-        while True:
-
-            dt = min_abs(config.guess_dt, evolve_target_t - evolved_t)
-            logger.debug(
-                    f"guess_dt: {config.guess_dt}, try time step size: {dt}"
-            )
-            
-            mps_half1 = fun(cur_mps, mpo, dt / 2)
-            mps_half2 = fun(mps_half1, mpo, dt / 2)
-            mps = fun(cur_mps, mpo, dt)
-            dis = mps.distance(mps_half2)
-
-            # prevent bug. save "some" memory.
-            del mps_half1, mps
-
-            p = (0.75 * config.adaptive_rtol / (dis/mps_half2.mp_norm + 1e-30)) ** (1./3)
-            logger.debug(f"distance: {dis}, enlarge p parameter: {p}")
-            if p < p_min:
-                p = p_min
-            if p_max < p:
-                p = p_max
-
-            # rejected
-            if p < p_restart:
-                config.guess_dt = dt * p
-                logger.debug(
-                    f"evolution not converged, new guess_dt: {config.guess_dt}"
-                )
-                continue
-
-            # accepted
-            evolved_t += dt
-            if np.allclose(evolved_t, evolve_target_t):
-                # normal exit. Note that `dt` could be much less than actually tolerated for the last step
-                # so use `guess_dt` for the last step. Slight inaccuracy won't harm.
-                mps_half2.evolve_config.guess_dt = config.guess_dt
-                logger.debug(
-                    f"evolution converged, new guess_dt: {mps_half2.evolve_config.guess_dt}"
-                )
-                return mps_half2
-            else:
-                # in this case `config.guess_dt == dt`
-                config.guess_dt *= p
-                logger.debug(f"sub-step {dt} further, evolved: {evolved_t}, new guess_dt: {config.guess_dt}")
-                cur_mps = mps_half2
-
-    return adaptive_fun
-
-
-class Mps(MatrixProduct):
-    @classmethod
-    def random(cls, model: Model, qntot, m_max, percent=1.0) -> "Mps":
-        # a high percent makes the result more random
-        # sometimes critical for getting correct optimization result
-        mps = cls()
-        mps.model = model
-        if isinstance(qntot, int):
-            qntot = np.array([qntot])
-        qn_size = len(qntot)
-        assert qn_size == model.qn_size
-        mps.qn = [np.zeros((1, qn_size), dtype=int)]
-        dim_list = [1]
-
-        for imps in range(model.nsite - 1):
-
-            # quantum number
-            qnbig = add_outer(mps.qn[imps], mps._get_sigmaqn(imps)).reshape(-1, qn_size)
-            u_set = []
-            s_set = []
-            qnset = []
-
-            for iblock in set([tuple(t) for t in qnbig]):
-                if np.all(np.array(qntot) < np.array(iblock)):
-                    continue
-                # find the quantum number index
-                indices = [i for i, x in enumerate(qnbig) if tuple(x) == iblock]
-                assert len(indices) != 0
-                a = np.random.random([len(indices), len(indices)]) - 0.5
-                a = a + a.T
-                s, u = scipy.linalg.eigh(a=a)
-                u_set.append(svd_qn.blockrecover(indices, u, len(qnbig)))
-                s_set.append(s)
-                qnset += [iblock] * len(indices)
-
-            u_set = np.concatenate(u_set, axis=1)
-            s_set = np.concatenate(s_set)
-            mt, mpsdim, mpsqn, nouse = select_basis(
-                u_set, s_set, qnset, u_set, m_max, percent=percent
-            )
-            # add the next mpsdim
-            dim_list.append(mpsdim)
-            mps.append(mt.reshape((dim_list[imps], -1, dim_list[imps + 1])))
-            mps.qn.append(mpsqn)
-
-        # the last site
-        mps.qn.append(np.zeros((1, qn_size), dtype=int))
-        dim_list.append(1)
-        last_mt = (
-            xp.random.random([dim_list[-2], mps.pbond_list[-1], dim_list[-1]]) - 0.5
-        )
-        # normalize the mt so that the whole mps is normalized
-        last_mt /= xp.linalg.norm(last_mt.flatten())
-        mps.append(last_mt)
-
-        mps.qnidx = len(mps) - 1
-        mps.to_right = False
-        mps.qntot = np.array(qntot)
-
-        return mps
-
-    @classmethod
-    def hartree_product_state(cls, model, condition: Dict):
-        r"""
-        Construct a Hartree product state
-        
-        Args:
-            model (:class:`~renormalizer.model.Model`): Model information.
-            condition (Dict): Dict with format ``{dof:local_state}``.
-                The default local state for dofs not specified is the "0" state.
-                An example is ``{"e_1":1, "v_0":2, "v_3":[0, 0.707, 0.707]}``.
-
-                Note:
-                    If there are bases that contain multiple dofs in the model, the value of the dict
-                    is the state of all dofs of the basis. For example,
-                    if a basis contains ``"e_1"``, ``"e_2"`` and ``"e_3"``,
-                    ``{"e_1": 2}`` (``{"e_1": [0, 0, 1]}``) means ``"e_3"`` is occupied and
-                    ``{"e_1": 1}`` (``{"e_1": [0, 1, 0]}``) means ``"e_2"`` is occupied.
-                    Be aware that in :class:`renormalizer.utils.basis.BasisMultiElectronVac` the vacuum state
-                    is added to the ``0`` index.
-
-        Returns:
-            Constructed mps (:class:`Mps`)
-        """
-        
-        mps = cls()
-        mps.model = model
-        mps.build_empty_mp(model.nsite)
-        qn_size = model.qn_size
-        mps.qn = [np.zeros((1, qn_size), dtype=int)]
-
-        # check that the condition is not duplicated
-        # each site has at most 1 single key to assign the occupation  
-        index = [model.dof_to_siteidx[key] for key in condition.keys()]
-        assert len(index) == len(set(index))
-        # replace the dof_name key to site_index key
-        condition = {model.dof_to_siteidx[key]:value for key, value in
-                condition.items()}
-
-        for isite, local_basis in enumerate(model.basis):
-            pdim = local_basis.nbas
-            ms = np.zeros((1, pdim, 1))
-            local_state = condition.pop(isite,0)
-            if isinstance(local_state, int):
-                ms[0, local_state, 0] = 1.
-                qn = local_basis.sigmaqn[local_state]
-            else:
-                ms[0, :, 0] = local_state
-                # quantum numbers for all states occupied
-                all_qn = np.array(local_basis.sigmaqn)[np.nonzero(local_state)]
-                if not np.allclose(all_qn.std(axis=0), 0):
-                    raise ValueError("Quantum numbers are mixed in the condition.")
-                qn = all_qn[0]
-
-            mps[isite] = ms
-            mps.qn.append(mps.qn[-1] + qn.reshape(1, qn_size))
-
-        if len(condition) != 0:
-            raise ValueError(f"Condition not completely used: {condition}")
-        mps.qntot = mps.qn[-1][0]
-        mps.qn[-1] = np.zeros((1, qn_size), dtype=int)
-        mps.qnidx = model.nsite - 1
-        mps.to_right = False
-
-        return mps
-
-    @classmethod
-    def ground_state(cls, model: Model, max_entangled: bool,
-            normalize:bool=True, condition:Dict=None):
-        r"""
-        Obtain ground state at :math:`T = 0` or :math:`T = \infty` (maximum entangled).
-        Electronic DOFs are always at ground state. and vibrational DOFs depend on ``max_entangled``.
-        For Spin-Boson model the electronic DOF also depends on ``max_entangled``.
-        
-
-        Parameters
-        ----------
-            model : :class:`~renormalizer.model.Model`
-                system information.
-            max_entangled : bool
-                temperature of the vibrational DOFs. If set to ``True``,
-                :math:`T = \infty` and if set to ``False``, :math:`T = 0`.
-            normalize: bool, optional
-                if the returned Mps are normalized when ``max_entangled=True``.
-                Default is True. If ``normalize=False``, the vibrational part is identity.
-            condition: dict, optional
-                the same as `hartree_product_state`. only used in ba.BasisMultiElectron
-                cases to define the occupation. Default is ``None``.
-        Returns
-        -------
-            mps : renormalizer.mps.Mps
-        
-        """
-        
-        mps = cls()
-        mps.model = model
-        mps.qn = [np.zeros((1, model.qn_size), dtype=int)] * (model.nsite + 1)
-        mps.qnidx = model.nsite - 1
-        mps.to_right = False
-        mps.qntot = np.zeros(model.qn_size, dtype=int)
-            
-        mps.build_empty_mp(model.nsite)
-        
-        if condition is not None:
-            # check that the condition is not duplicated
-            # each site has at most 1 single key to assign the occupation  
-            index = [model.dof_to_siteidx[key] for key in condition.keys()]
-            assert len(index) == len(set(index))
-            # replace the dof_name key to site_index key
-            condition = {model.dof_to_siteidx[key]:value for key, value in
-                    condition.items()}
-
-        for isite, local_basis in enumerate(model.basis):
-            pdim = local_basis.nbas
-            ms = np.zeros((1, pdim, 1))
-            if local_basis.is_phonon:
-                if max_entangled:
-                    if normalize:
-                        ms[0, :, 0] = 1.0 / np.sqrt(pdim)
-                    else:
-                        ms[0, :, 0] = 1.0
-                else:
-                    ms[0, 0, 0] = 1.0
-                mps[isite] = ms
-
-            elif local_basis.is_electron or local_basis.is_spin:
-
-                if isinstance(local_basis, ba.BasisSimpleElectron):
-                    # simple electron site
-                    ms[0,0,0] = 1.
-                elif isinstance(local_basis, ba.BasisMultiElectron):
-                    assert condition is not None
-                    local_state = condition.pop(isite)
-                    if isinstance(local_state, int):
-                        ms[0, local_state, 0] = 1.
-                        qn = local_basis.sigmaqn[local_state]
-                    else:
-                        ms[0, :, 0] = local_state
-                        qn = local_basis.sigmaqn[np.nonzero(local_state)]
-                    assert np.allclose(qn, 0)
-                    if max_entangled and normalize:
-                        ms /= np.linalg.norm(ms)
-
-                elif isinstance(local_basis, ba.BasisMultiElectronVac):
-                        ms[0,0,0] = 1.
-                elif isinstance(local_basis, ba.BasisHalfSpin):
-                    if max_entangled:
-                        if normalize:
-                            ms[0,:,0] = 1. / np.sqrt(2.)
-                        else:
-                            ms[0,:,0] = 1.
-                    else:
-                        ms[0,0,0] = 1.
-                else:
-                    raise NotImplementedError
-                mps[isite] = ms
-        for ms in mps:
-            assert ms is not None
-        return mps
-
-    @classmethod
-    def load(cls, model: Model, fname: str):
-        npload = np.load(fname, allow_pickle=True)
-        mp = cls()
-        mp.model = model
-        for i in range(int(npload["nsites"])):
-            mt = npload[f"mt_{i}"]
-            if np.iscomplexobj(mt):
-                mp.dtype = backend.complex_dtype
-            else:
-                mp.dtype = backend.real_dtype
-            mp.append(mt)
-        mp.qn = npload["qn"]
-        mp.qnidx = int(npload["qnidx"])
-        mp.qntot = npload["qntot"]
-        version = npload["version"]
-        if version == "0.1":
-            mp.to_right = bool(npload["left"])
-            # in this protocol, TDH and coeff is not dumped
-            logger.warning("Using old dump/load protocol. TD Hartree part will be lost")
-            mp.coeff = 1
-        elif version == "0.2":
-            mp.to_right = bool(npload["to_right"])
-            # in this protocol, TDH is dumped, but it's not useful anymore
-            logger.warning("Using old dump/load protocol. TD Hartree part will be lost")
-            mp.coeff = npload["tdh_wfns"][-1]
-        elif version == "0.3":
-            mp.to_right = bool(npload["to_right"])
-            mp.coeff = npload["coeff"].item(0)
-        else:
-            raise ValueError(f"Unknown dump version: {version}")
-        return mp
-
-    @classmethod
-    def from_dense(cls, model, wfn: np.ndarray):
-        # for debugging
-        mp = cls()
-        mp.model = model
-        if np.iscomplexobj(wfn):
-            mp.dtype = backend.complex_dtype
-        else:
-            mp.dtype = backend.real_dtype
-        residual_wfn = wfn.reshape([1] + [b.nbas for b in model.basis] + [1])
-        for i in range(len(model.basis) - 1):
-            wfn_2d = residual_wfn.reshape(residual_wfn.shape[0] * residual_wfn.shape[1], -1)
-            q, r = np.linalg.qr(wfn_2d)
-            mp.append(q.reshape(residual_wfn.shape[0], residual_wfn.shape[1], q.shape[1]))
-            residual_wfn = r.reshape([r.shape[0]] + list(residual_wfn.shape[2:]))
-        assert residual_wfn.ndim == 3
-        mp.append(residual_wfn)
-        mp.build_empty_qn()
-        return mp
-
-    def __init__(self):
-        super().__init__()
-        self.coeff: Union[float, complex] = 1
-
-        self.optimize_config: OptimizeConfig = OptimizeConfig()
-        self.evolve_config: EvolveConfig = EvolveConfig()
-
-    def conj(self) -> "Mps":
-        new_mps = super().conj()
-        new_mps.coeff = new_mps.coeff.conjugate()
-        return new_mps
-
-    def to_complex(self, inplace=False) -> "Mps":
-        new_mp = super(Mps, self).to_complex(inplace=inplace)
-        new_mp.coeff = complex(new_mp.coeff)
-        return new_mp
-
-    def _get_sigmaqn(self, idx):
-        return self.model.basis[idx].sigmaqn
-
-    @property
-    def is_mps(self):
-        return True
-
-    @property
-    def is_mpo(self):
-        return False
-
-    @property
-    def is_mpdm(self):
-        return False
-
-    @property
-    def nexciton(self):
-        return self.qntot
-
-    @property
-    def norm(self):
-        '''the norm of the total wavefunction
-        '''
-        return np.linalg.norm(self.coeff) * self.mp_norm
-
-    def _expectation_path(self):
-        # S--a--S--e--S
-        # |     |     |
-        # |     d     |
-        # |     |     |
-        # O--b--O--g--O
-        # |     |     |
-        # |     f     |
-        # |     |     |
-        # S--c--S--h--S
-        path = [
-            ([0, 1], "abc, cfh -> abfh"),
-            ([3, 0], "abfh, bdfg -> ahdg"),
-            ([2, 0], "ahdg, ade -> hge"),
-            ([1, 0], "hge, egh -> "),
-        ]
-        return path
-
-    def _expectation_conj(self):
-        return self.conj()
-
-    def expectation(self, mpo, self_conj=None) -> Union[float, complex]:
-        if self_conj is None:
-            self_conj = self._expectation_conj()
-        environ = Environ(self, mpo, "R", mps_conj=self_conj)
-        l = xp.ones((1, 1, 1), dtype=self.dtype)
-        r = environ.read("R", 1)
-        path = self._expectation_path()
-        val = multi_tensor_contract(path, l, self[0], mpo[0], self_conj[0], r)
-        if np.isclose(float(val.imag), 0):
-            return float(val.real)
-        else:
-            return complex(val)
-        # This is time and memory consuming
-        # return self_conj.dot(mpo.apply(self)).real
-
-    def expectations(self, mpos, self_conj=None, opt=True) -> np.ndarray:
-
-        if not opt:
-            # the naive way, slow and time consuming. Yet predictable and reliable
-            return np.array([self.expectation(mpo, self_conj) for mpo in mpos])
-
-        # optimized way, cache for intermediates
-        # hash is used as indices of the matrices.
-        # The chance for collision (the same hash for two different matrices) is
-        # about 1-0.99999999999997 in 1000 matrices.
-        # In which case a RuntimeError is raised and rerun the job should solve the problem
-        hash_to_obj = dict()
-        mpos_hash: List[List] = []
-        for mpo in mpos:
-            mpo_hash = []
-            for m in mpo:
-                m_hash = hash(m)
-                if m_hash not in hash_to_obj:
-                    hash_to_obj[m_hash] = m
-                else:
-                    if not np.allclose(hash_to_obj[m_hash], m.array):
-                        raise RuntimeError("Rare hash collision")
-                mpo_hash.append(m_hash)
-            mpos_hash.append(mpo_hash)
-
-        if self_conj is None:
-            self_conj = self._expectation_conj()
-        l_environ_dict = _construct_freq_environ(mpos_hash, hash_to_obj, self, "L", self_conj)
-        r_environ_dict = _construct_freq_environ(mpos_hash, hash_to_obj, self, "R", self_conj)
-        results = []
-        for mpo in mpos:
-            l_environ, l_idx = _get_freq_environ(l_environ_dict, mpo, "L", np.inf)
-            r_environ, r_idx = _get_freq_environ(r_environ_dict, mpo, "R", len(mpo)-l_idx-1)
-            for i in range(l_idx+1, r_idx):
-                l_environ = contract_one_site(l_environ, self[i], mpo[i], "L", self_conj[i])
-            results.append(complex(l_environ.flatten() @ r_environ.flatten()))  # cast to python type
-
-        results = np.array(results)
-        if np.allclose(results.imag, 0):
-            return results.real
-        else:
-            return results
-
-    @property
-    def ph_occupations(self):
-        r"""
-        phonon occupations :math:`b^\dagger_i b_i` for each electronic DoF.
-        The order is defined by :attr:`~renormalizer.model.model.v_dofs`.
-        """
-        key = "ph_occupations"
-        # ph_occupations is actually the occupation of the basis
-        if key not in self.model.mpos:
-            mpos = []
-            for dof in self.model.v_dofs:
-                mpos.append(Mpo(self.model, Op("n", dof)))
-            self.model.mpos[key] = mpos
-        else:
-            mpos = self.model.mpos[key]
-
-        return self.expectations(mpos)
-
-    @property
-    def e_occupations(self):
-        r"""
-        Electronic occupations :math:`a^\dagger_i a_i` for each electronic DoF.
-        The order is defined by :attr:`~renormalizer.model.model.e_dofs`.
-        """
-        key = "e_occupations"
-        if key not in self.model.mpos:
-            mpos = []
-            for dof in self.model.e_dofs:
-                mpos.append(Mpo(self.model, Op(r"a^\dagger a", dof)))
-            self.model.mpos[key] = mpos
-        else:
-            mpos = self.model.mpos[key]
-        return self.expectations(mpos)
-
-    def metacopy(self) -> "Mps":
-        new: Mps = super().metacopy()
-        new.coeff = self.coeff
-        new.optimize_config = self.optimize_config
-        # evolve_config has its own data
-        new.evolve_config = self.evolve_config.copy()
-        return new
-
-    def normalize(self, kind):
-        r''' normalize the wavefunction
-
-        Parameters
-        ----------
-        kind: str
-            "mps_only": the mps part is normalized and coeff is not modified;
-            "mps_norm_to_coeff": the mps part is normalized and the norm is multiplied to coeff;
-            "mps_and_coeff": both mps and coeff is normalized
-
-        Returns
-        -------
-        ``self`` is overwritten.
-        '''
-
-        if kind == "mps_only":
-            new_coeff = self.coeff
-        elif kind == "mps_and_coeff":
-            new_coeff = self.coeff / np.linalg.norm(self.coeff)
-        elif kind == "mps_norm_to_coeff":
-            new_coeff = self.coeff * self.mp_norm
-        else:
-            raise ValueError(f"kind={kind} is not valid.")
-        new_mps = self.scale(1.0 / self.mp_norm, inplace=True)
-        new_mps.coeff = new_coeff
-
-        return new_mps
-
-
-    def expand_bond_dimension(self, hint_mpo=None, coef=1e-10, include_ex=True):
-        """
-        expand bond dimension as required in compress_config
-        """
-        # expander m target
-        m_target = self.compress_config.bond_dim_max_value - self.bond_dims_mean
-        # will be restored at exit
-        self.compress_config.bond_dim_max_value = m_target
-        if self.compress_config.criteria is not CompressCriteria.fixed:
-            logger.warning("Setting compress criteria to fixed")
-            self.compress_config.criteria = CompressCriteria.fixed
-        logger.debug(f"target for expander: {m_target}")
-        if hint_mpo is None:
-            expander = self.__class__.random(self.model, 1, m_target)
-        else:
-            # fill states related to `hint_mpo`
-            logger.debug(
-                f"average bond dimension of hint mpo: {hint_mpo.bond_dims_mean}"
-            )
-            # in case of localized `self`
-            if include_ex:
-                if self.is_mps:
-                    ex_state: MatrixProduct = self.ground_state(self.model, False)
-                    # for self.qntot >= 1
-                    assert self.model.qn_size == 1 # otherwise not supported
-                    for i in range(self.qntot[0]):
-                        ex_state = Mpo.onsite(self.model, r"a^\dagger") @ ex_state
-                elif self.is_mpdm:
-                    assert self.qntot == 1
-                    ex_state: MatrixProduct = self.max_entangled_ex(self.model)
-                else:
-                    assert False
-                ex_state.compress_config = self.compress_config
-                ex_state.move_qnidx(self.qnidx)
-                ex_state.to_right = self.to_right
-                lastone = self + ex_state
-
-            else:
-                lastone = self
-            expander_list: List["MatrixProduct"] = []
-            cumulated_m = 0
-            while True:
-                lastone.compress_config.criteria = CompressCriteria.fixed
-                expander_list.append(lastone)
-                expander = compressed_sum(expander_list)
-                if cumulated_m == expander.bond_dims_mean:
-                    # probably a small system, the required bond dimension can't be reached
-                    break
-                cumulated_m = expander.bond_dims_mean
-                logger.debug(
-                    f"cumulated bond dimension: {cumulated_m}. lastone bond dimension: {lastone.bond_dims}"
-                )
-                if m_target < cumulated_m:
-                    break
-                if m_target < 0.8 * (lastone.bond_dims_mean * hint_mpo.bond_dims_mean):
-                    lastone = lastone.canonicalise().compress(
-                        m_target // hint_mpo.bond_dims_mean + 1
-                    )
-                lastone = (hint_mpo @ lastone).normalize("mps_and_coeff")
-        logger.debug(f"expander bond dimension: {expander.bond_dims}")
-        self.compress_config.bond_dim_max_value += self.bond_dims_mean
-        return (self + expander.scale(coef*self.norm, inplace=True)).canonicalise().canonicalise().normalize("mps_norm_to_coeff")
-
-    def evolve(self, mpo, evolve_dt, normalize=True) -> "Mps":
-
-        method = {
-            EvolveMethod.prop_and_compress: self._evolve_prop_and_compress,
-            EvolveMethod.prop_and_compress_tdrk4: self._evolve_prop_and_compress_tdrk4,
-            EvolveMethod.prop_and_compress_tdrk: self._evolve_prop_and_compress_tdrk,
-            EvolveMethod.tdvp_mu_vmf: self._evolve_tdvp_mu_vmf,
-            EvolveMethod.tdvp_vmf: self._evolve_tdvp_mu_vmf,
-            EvolveMethod.tdvp_mu_cmf: self._evolve_tdvp_mu_cmf,
-            EvolveMethod.tdvp_ps: self._evolve_tdvp_ps,
-            EvolveMethod.tdvp_ps2: self._evolve_tdvp_ps2
-        }[self.evolve_config.method]
-        new_mps = method(mpo, evolve_dt)
-        if normalize:
-            if np.iscomplex(evolve_dt):
-                new_mps.normalize("mps_and_coeff")
-            else:
-                new_mps.normalize("mps_only")
-        return new_mps
-    
-    def _evolve_prop_and_compress_tdrk4(self, mpo, evolve_dt) -> "Mps":
-        """
-        classical 4th order Runge-Kutta solver for time-dependent Hamiltonian
-        """
-        
-        if isinstance(mpo, Mpo): 
-            def mpo_t(t, *args, **kwargs):
-                return mpo
-        elif callable(mpo):
-            # mpo can be a function of time, the range is 0 -> evolve_dt
-            mpo_t = mpo
-        else:
-            raise TypeError(f"unsupported mpo type: {mpo}")
-
-        k1 = mpo_t(0).contract(self).scale(-1j)
-        logger.debug(f"k1:{k1}")  
-        tmp_mps = self + k1.scale(0.5*evolve_dt)
-        tmp_mps.canonicalise().compress()
-        k2 = mpo_t(0.5*evolve_dt).contract(tmp_mps).scale(-1j)
-        logger.debug(f"k2:{k2}")  
-        tmp_mps = self + k2.scale(0.5*evolve_dt)
-        tmp_mps.canonicalise().compress()
-        k3 = mpo_t(0.5*evolve_dt).contract(tmp_mps).scale(-1j)
-        logger.debug(f"k3:{k3}")  
-        tmp_mps = self + k3.scale(evolve_dt)
-        tmp_mps.canonicalise().compress()
-        k4 = mpo_t(evolve_dt).contract(tmp_mps).scale(-1j)
-        logger.debug(f"k4:{k4}")  
-        
-        new_mps = compressed_sum([self, k1.scale(1/6*evolve_dt),
-            k2.scale(2/6*evolve_dt), 
-            k3.scale(2/6*evolve_dt),
-            k4.scale(1/6*evolve_dt)])
-        logger.info(f"new_mps:{new_mps}")  
-        
-        return new_mps
-    
-    def _evolve_prop_and_compress_tdrk(self, mpo, evolve_dt) -> "Mps":
-        """
-            The most general Runge-Kutta solver for both time-dependent and
-            time-independnet Hamiltonian and adaptive or unadaptive time-step
-            size evolution
-        """
-        if isinstance(mpo, Mpo): 
-            def mpo_t(t, *args, **kwargs):
-                return mpo
-        elif callable(mpo):
-            mpo_t = mpo
-        else:
-            raise TypeError(f"unsupported mpo type: {mpo}")
-        
-        rk_config = self.evolve_config.rk_config
-        a,b,c = rk_config.tableau
-        
-        def sub_time_step_evolve(y,tau,t0):
-            # error is relative error
-            k_list = []
-            for istage in range(rk_config.stage):
-                k = compressed_sum([y]+[k_list[i].scale(a[istage,i]*tau) for
-                    i in range(istage) if a[istage,i] != 0], batchsize=6)
-                k = mpo_t(c[istage]*tau+t0, mps=k).contract(k).scale(-1j)
-                logger.debug(f"k_{istage}: {k}") 
-                k_list.append(k)        
-            
-            new_mps = compressed_sum([y] +
-                    [k_list[istage].scale(b[0,istage]*tau) \
-                    for istage in range(rk_config.stage) if b[0,istage]!=0],
-                    batchsize=6)   
-            logger.debug(f"order_{rk_config.order[0]}: {new_mps}") 
-            
-            if self.evolve_config.adaptive:
-                assert len(rk_config.order) == 2
-                assert rk_config.order[0] - rk_config.order[1] == 1
-                error = reduce(lambda mps1, mps2: mps1.add(mps2),
-                    [k_list[istage].scale((b[0,istage]-b[1,istage])*tau) \
-                    for istage in range(rk_config.stage) if not \
-                    np.allclose(b[0,istage],b[1,istage])])
-
-                error = error.norm / new_mps.norm
-            else:
-                assert len(rk_config.order) == 1
-                error = 0
-                
-            return new_mps, error
-        
-        self.evolve_config.check_valid_dt(evolve_dt)
-        
-        if self.evolve_config.adaptive:
-            p_restart = 0.5  # restart threshold
-            p_min = 0.1  # safeguard for minimal allowed p
-            p_max = 2.0  # safeguard for maximal allowed p
-            
-            evolved_dt = 0
-            new_mps = self
-
-            while True:
-                dt = min_abs(new_mps.evolve_config.guess_dt, evolve_dt-evolved_dt)
-                logger.debug(f"guess_dt: {new_mps.evolve_config.guess_dt}, try time step size: {dt}")
-                new_mps, error = sub_time_step_evolve(new_mps, dt, evolved_dt)    
-                p = (new_mps.evolve_config.adaptive_rtol / (error + 1e-30)) ** (1/rk_config.order[0])
-                logger.debug(f"RKsolver:{rk_config.method} relative error: {error}, enlarge p parameter: {p}")
-                
-                if p < p_restart:
-                    # not accurate, will restart
-                    new_mps.evolve_config.guess_dt = dt * max(p_min, p)
-                    logger.debug(
-                        f"evolution not converged, new guess_dt: {new_mps.evolve_config.guess_dt}"
-                    )
-                else:
-                    if xp.allclose(dt+evolved_dt, evolve_dt):
-                        new_mps.evolve_config.guess_dt = min_abs(
-                            dt * p, new_mps.evolve_config.guess_dt
-                        )
-                        # normal exit
-                        logger.debug(
-                            f"evolution converged, new guess_dt: {new_mps.evolve_config.guess_dt}"
-                        )
-                        break
-                    else:
-                        new_mps.evolve_config.guess_dt *= min(p, p_max)
-                        evolved_dt += dt
-                        logger.debug(
-                            f"evolution converged, new guess_dt: {new_mps.evolve_config.guess_dt}"
-                        )
-                        logger.debug(f"sub-step {dt} further, remaining: {evolve_dt-evolved_dt}")
-        else:
-            new_mps, _ = sub_time_step_evolve(self, evolve_dt, 0)
-
-        return new_mps
-
-    def _evolve_prop_and_compress(self, mpo, evolve_dt) -> "Mps":
-        """
-        The global propagation & compression evolution scheme
-        only for time-independent Hamiltonian
-        Taylor expansion approximation to the formal propagator
-        """
-        config = self.evolve_config
-        assert evolve_dt is not None
-
-        propagation_c = config.taylor_config.coeff
-        order = len(propagation_c)-1
-        termlist = [self]
-        # don't let bond dim grow when contracting
-        orig_compress_config = self.compress_config
-        contract_compress_config = self.compress_config.copy()
-        if contract_compress_config.criteria is CompressCriteria.threshold:
-            contract_compress_config.criteria = CompressCriteria.both
-        # contract_compress_config.min_dims = None
-        # contract_compress_config.max_dims = np.array(self.bond_dims) + 4
-        self.compress_config = contract_compress_config
-
-        while len(termlist) < len(propagation_c):
-            termlist.append(mpo.contract(termlist[-1]))
-        # bond dim can grow after adding
-        for t in termlist:
-            t.compress_config = orig_compress_config
-
-        if config.adaptive:
-            config.check_valid_dt(evolve_dt)
-
-            p_restart = 0.5  # restart threshold
-            p_min = 0.1  # safeguard for minimal allowed p
-            p_max = 2.0  # safeguard for maximal allowed p
-
-            while True:
-                scaled_termlist = []
-                dt = min_abs(config.guess_dt, evolve_dt)
-                logger.debug(f"guess_dt: {config.guess_dt}, try time step size: {dt}")
-                for idx, term in enumerate(termlist):
-                    scale = (-1.0j * dt) ** idx * propagation_c[idx]
-                    scaled_termlist.append(term.scale(scale))
-                    del term
-                
-                new_mps1 = compressed_sum(scaled_termlist[:-1])
-                new_mps2 = compressed_sum(
-                    [new_mps1, scaled_termlist[-1]]
-                )
-                dis = new_mps1.distance(new_mps2)
-                p = (config.adaptive_rtol / (dis/new_mps2.mp_norm + 1e-30)) ** (1/order)
-                logger.debug(f"RK45 error distance: {dis}, enlarge p parameter: {p}")
-
-                if xp.allclose(dt, evolve_dt):
-                    # approahes the end
-                    if p < p_restart:
-                        # not accurate in this final sub-step will restart
-                        config.guess_dt = dt * max(p_min, p)
-                        logger.debug(
-                            f"evolution not converged, new guess_dt: {config.guess_dt}"
-                        )
-                    else:
-                        # normal exit
-                        new_mps2.evolve_config.guess_dt = min_abs(
-                            dt * p, config.guess_dt
-                        )
-                        logger.debug(
-                            f"evolution converged, new guess_dt: {new_mps2.evolve_config.guess_dt}"
-                        )
-                        return new_mps2
-                else:
-                    # sub-steps
-                    if p < p_restart:
-                        config.guess_dt *= max(p_min, p)
-                        logger.debug(
-                            f"evolution not converged, new guess_dt: {config.guess_dt}"
-                        )
-                    else:
-                        new_dt = evolve_dt - dt
-                        config.guess_dt *= min(p, p_max)
-                        new_mps2.evolve_config.guess_dt = config.guess_dt
-                        # memory consuming and not useful anymore
-                        del new_mps1, termlist, scaled_termlist
-                        logger.debug(
-                            f"evolution converged, new guess_dt: {config.guess_dt}"
-                        )
-                        logger.debug(f"sub-step {dt} further, remaining: {new_dt}")
-                        return new_mps2._evolve_prop_and_compress(mpo, new_dt)
-        else:
-            for idx, term in enumerate(termlist):
-                term.scale(
-                    (-1.0j * evolve_dt) ** idx * propagation_c[idx], inplace=True
-                )
-            return compressed_sum(termlist)
-    
-    def _evolve_tdvp_mu_vmf(self, mpo, evolve_dt) -> "Mps":
-        """
-        variable mean field
-        see the difference between VMF and CMF, refer to Z. Phys. D 42, 113–129 (1997)
-        the matrix unfolding algorithm, see arXiv:1907.12044
-        only the RKF45 integration is used.
-        The default RKF45 local step error tolerance is rtol:1e-5, atol:1e-8
-        regulation of S is 1e-10, these default parameters could be changed in
-        /utils/configs.py
-
-        """
-        
-        if isinstance(mpo, Mpo): 
-            def mpo_t(t, *args, **kwargs):
-                return mpo
-        elif callable(mpo):
-            mpo_t = mpo
-        else:
-            raise TypeError(f"unsupported mpo type: {mpo}")
-        
-        # a workaround for https://github.com/scipy/scipy/issues/10164
-        imag_time = np.iscomplex(evolve_dt)
-        if imag_time:
-            evolve_dt = -evolve_dt.imag
-            # used in calculating derivatives
-            coef = -1
-        else:
-            coef = 1j
-        
-        # only not canonicalise when force_ovlp=True and to_right=False
-        if not (self.evolve_config.force_ovlp and not self.to_right):
-            self.ensure_left_canonical()
-
-        # `self` should not be modified during the evolution
-        if imag_time:
-            mps = self.copy()
-        else:
-            mps = self.to_complex()
-
-        # the quantum number symmetry is used
-        qn_mask_list = []
-        position = [0]
-        qntot = mps.qntot
-        for imps in range(mps.site_num):
-            mps.move_qnidx(imps)
-            qnbigl, qnbigr, qnmat = mps._get_big_qn([imps])
-            qn_mask = get_qn_mask(qnmat, mps.qntot)
-            qn_mask_list.append(qn_mask)
-            position.append(position[-1]+np.sum(qn_mask))
-
-        sw_min_list = []
-        
-        def func_vmf(t,y):
-            
-            sw_min_list.clear()
-
-            # update mps: from left to right
-            for imps in range(mps.site_num):
-                mps[imps] = cvec2cmat(asnumpy(y[position[imps]:position[imps + 1]]), qn_mask_list[imps])
-            mpo = mpo_t(t, mps=mps)
-
-            if self.evolve_config.method == EvolveMethod.tdvp_mu_vmf:
-                environ_mps = mps.copy()
-            elif self.evolve_config.method == EvolveMethod.tdvp_vmf:
-                environ_mps = mps
-                # the first S_R
-                S_R = np.ones([1, 1], dtype=mps.dtype)
-            else:
-                assert False
-
-            environ = Environ(environ_mps, mpo, "L")
-
-            if self.evolve_config.force_ovlp:
-                # construct the S_L list (type: Matrix) and S_L_inv list (type: xp.array)
-                # len: mps.site_num+1
-                S_L_list = [
-                    np.ones([1, 1], dtype=mps.dtype),
-                ]
-                for imps in range(mps.site_num):
-                    S_L_list.append(
-                        transferMat(mps, None, "L", imps, S_L_list[imps])
-                    )
-
-
-                S_L_inv_list = []
-                for imps in range(mps.site_num + 1):
-                    w, u = scipy.linalg.eigh(S_L_list[imps])
-                    S_L_inv = u.dot(np.diag(1.0 / w)).dot(u.T.conj())
-                    S_L_inv_list.append(S_L_inv)
-            else:
-                S_L_list = [None,] * (mps.site_num + 1)
-                S_L_inv_list = [None,] * (mps.site_num + 1)
-
-            # calculate hop_y: from right to left
-            hop_y = xp.empty_like(y)
-
-            for imps in mps.iter_idx_list(full=True):
-                shape = list(mps[imps].shape)
-                ltensor = asxp(environ.read("L", imps - 1))
-
-                if imps == self.site_num - 1:
-                    # the coefficient site
-                    rtensor = xp.ones((1, 1, 1), dtype=mps.dtype)
-                    hop =hop_expr(ltensor, rtensor, [asxp(mpo[imps])], shape)
-
-                    S_inv = xp.diag(xp.ones(1,dtype=mps.dtype))
-                    func = integrand_func_factory(shape, hop, True, S_inv, True,
-                            coef, ovlp_inv1=S_L_inv_list[imps+1],
-                            ovlp_inv0=S_L_inv_list[imps], ovlp0=S_L_list[imps])
-
-                    hop_y[position[imps]:position[imps+1]] = func(0,
-                            mps[imps].array.ravel()).reshape(mps[imps].shape)[qn_mask_list[imps]]
-
-                    continue
-
-                if self.evolve_config.method == EvolveMethod.tdvp_mu_vmf:
-                    # perform qr on the environment mps
-                    qnbigl, qnbigr, _ = environ_mps._get_big_qn([imps + 1])
-                    u, s, qnlset, v, s, qnrset = svd_qn.svd_qn(
-                            environ_mps[imps + 1].array, qnbigl, qnbigr,
-                            environ_mps.qntot, system="R", full_matrices=False)
-                    vt = v.T
-
-                    environ_mps[imps + 1] = vt.reshape(environ_mps[imps + 1].shape)
-
-                    rtensor = environ.GetLR(
-                        "R", imps + 1, environ_mps, mpo, itensor=None, method="System"
-                    )
-
-                    sw_min_list.append(s.min())
-                    regular_s = _mu_regularize(s, epsilon=self.evolve_config.reg_epsilon)
-
-                    u = asxp(u)
-                    us = u.dot(xp.diag(s))
-
-                    rtensor = xp.tensordot(rtensor, us, axes=(-1, -1))
-
-                    environ_mps[imps] = xp.tensordot(asxp(environ_mps[imps]), us, axes=(-1, 0))
-                    environ_mps.qn[imps + 1] = qnrset
-                    environ_mps.qnidx = imps
-
-                    S_inv = u.conj().dot(xp.diag(1.0 / regular_s)).T
-
-                elif self.evolve_config.method == EvolveMethod.tdvp_vmf:
-                    rtensor = environ.GetLR(
-                        "R", imps + 1, environ_mps, mpo, itensor=None, method="System")
-
-                    # regularize density matrix
-                    # Note that S_R is (#.conj, #)
-                    S_R = transferMat(environ_mps, None, "R", imps + 1, S_R)
-                    w, u = scipy.linalg.eigh(asnumpy(S_R))
-                    # discard the negative eigenvalues due to numerical error
-                    w = np.where(w>0, w, 0)
-
-                    sw_min_list.append(w.min())
-
-                    epsilon = self.evolve_config.reg_epsilon
-                    w = w + epsilon * np.exp(-w / epsilon)
-
-                    u = asxp(u)
-                    # S_inv is (#.conj, #)
-                    S_inv = u.dot(xp.diag(1.0 / w)).dot(u.T.conj()).T
-
-                hop = hop_expr(ltensor, rtensor, [asxp(mpo[imps])], shape)
-
-                func = integrand_func_factory(shape, hop, False, S_inv, True,
-                        coef, ovlp_inv1=S_L_inv_list[imps+1],
-                        ovlp_inv0=S_L_inv_list[imps], ovlp0=S_L_list[imps])
-
-                hop_y[position[imps]:position[imps+1]] = func(0,
-                        asxp(mps[imps].array.ravel())).reshape(mps[imps].shape)[qn_mask_list[imps]]
-
-            return hop_y
-
-        init_y = xp.concatenate([asxp(ms.array[qn_mask_list[ims]]) for ims, ms in enumerate(mps)])
-        # the ivp local error, please refer to the Scipy default setting
-        sol = solve_ivp(
-            func_vmf,
-            (0, evolve_dt),
-            init_y,
-            method="RK45",
-            rtol=self.evolve_config.ivp_rtol,
-            atol=self.evolve_config.ivp_atol,
-        )
-
-        # update mps: from left to right
-        for imps in range(mps.site_num):
-            mps[imps] = cvec2cmat(asnumpy(sol.y[:, -1][position[imps]:position[imps + 1]]), qn_mask_list[imps])
-
-        logger.info(f"{self.evolve_config.method} VMF func called: {sol.nfev}. RKF steps: {len(sol.t)}")
-
-        sw_min_list = xp.array(sw_min_list)
-        # auto-switch between tdvp_mu_vmf and tdvp_vmf
-        if self.evolve_config.vmf_auto_switch:
-            if sw_min_list.min() > np.sqrt(self.evolve_config.reg_epsilon*10.) and \
-                mps.evolve_config.method == EvolveMethod.tdvp_mu_vmf:
-
-                logger.debug(f"sw.min={sw_min_list.min()}, Switch to tdvp_vmf")
-                mps.evolve_config.method =  EvolveMethod.tdvp_vmf
-
-            elif sw_min_list.min() < self.evolve_config.reg_epsilon and \
-                mps.evolve_config.method == EvolveMethod.tdvp_vmf:
-
-                logger.debug(f"sw.min={sw_min_list.min()}, Switch to tdvp_mu_vmf")
-                mps.evolve_config.method =  EvolveMethod.tdvp_mu_vmf
-
-        # The caller do not want to deal with an MPS that is not canonicalised
-        return mps.canonicalise()
-
-    @adaptive_tdvp
-    def _evolve_tdvp_mu_cmf(self, mpo, evolve_dt) -> "Mps":
-        """
-        evolution scheme: TDVP + constant mean field + matrix-unfolding
-        regularization
-        MPS :  LLLLLLC
-        1st / 2nd order(default) CMF
-
-        for 2nd order CMF:
-        L is evolved with midpoint scheme
-        C is evolved with midpoint(default) / trapz scheme
-        """
-
-        if self.evolve_config.tdvp_cmf_c_trapz:
-            assert self.evolve_config.tdvp_cmf_midpoint
-
-        imag_time = np.iscomplex(evolve_dt)
-
-        # a workaround for https://github.com/scipy/scipy/issues/10164
-        if imag_time:
-            evolve_dt = -evolve_dt.imag
-            # used in calculating derivatives
-            coef = -1
-        else:
-            coef = 1j
-
-        self.ensure_left_canonical()
-
-        # `self` should not be modified during the evolution
-        # mps: the mps to return
-        # environ_mps: mps to construct environ
-        if imag_time:
-            mps = self.copy()
-        else:
-            mps = self.to_complex()
-
-        if self.evolve_config.tdvp_cmf_midpoint:
-            # mps at t/2 (1st order) as environment
-            orig_config = self.evolve_config.copy()
-            self.evolve_config.tdvp_cmf_midpoint = False
-            self.evolve_config.tdvp_cmf_c_trapz = False
-            self.evolve_config.adaptive = False
-            environ_mps = self.evolve(mpo, evolve_dt / 2)
-            self.evolve_config = orig_config
-        else:
-            # mps at t=0 as environment
-            environ_mps = mps.copy()
-
-        if self.evolve_config.tdvp_cmf_c_trapz:
-            loop = 2
-            mps[-1] = environ_mps[-1].copy()
-        else:
-            loop = 1
-
-        while loop > 0:
-
-            # construct the environment matrix
-            environ = Environ(environ_mps, mpo, "L")
-
-            # statistics for debug output
-            cmf_rk_steps = []
-
-            if self.evolve_config.force_ovlp:
-                # construct the S_L list (type: Matrix) and S_L_inv list (type: xp.array)
-                # len: mps.site_num+1
-                S_L_list = [np.ones([1, 1], dtype=mps.dtype),]
-                for imps in range(mps.site_num):
-                    S_L_list.append(transferMat(environ_mps, None, "L", imps,
-                        S_L_list[imps]))
-
-                S_L_inv_list = []
-                for imps in range(mps.site_num+1):
-                    w, u = scipy.linalg.eigh(S_L_list[imps])
-                    S_L_inv = xp.asarray(u.dot(np.diag(1.0 / w)).dot(u.T.conj()))
-                    S_L_inv_list.append(S_L_inv)
-                    S_L_list[imps] = S_L_list[imps]
-            else:
-                S_L_list = [None,] * (mps.site_num+1)
-                S_L_inv_list = [None,] * (mps.site_num+1)
-
-            for imps in mps.iter_idx_list(full=True):
-                shape = list(mps[imps].shape)
-                ltensor = environ.read("L", imps - 1)
-                if imps == self.site_num - 1:
-                    if loop == 1:
-                        # the coefficient site
-                        rtensor = ones((1, 1, 1))
-                        hop = hop_expr(ltensor, rtensor, [mpo[imps]], shape)
-
-                        S_inv = xp.diag(xp.ones(1,dtype=mps.dtype))
-                        def func1(y):
-                            func = integrand_func_factory(shape, hop, True, S_inv, True,
-                                    coef, ovlp_inv1=S_L_inv_list[imps+1],
-                                    ovlp_inv0=S_L_inv_list[imps], ovlp0=S_L_list[imps])
-                            return func(0, y)
-
-                        ms, Lanczos_vectors = expm_krylov(func1, evolve_dt, mps[imps].ravel().array)
-                        logger.debug(f"# of Lanczos_vectors, {Lanczos_vectors}")
-                        mps[imps] = ms.reshape(shape)
-
-                    if loop == 1 and self.evolve_config.tdvp_cmf_c_trapz:
-                        break
-                    else:
-                        continue
-
-                # perform qr on the environment mps
-                qnbigl, qnbigr, _ = environ_mps._get_big_qn([imps + 1])
-                u, s, qnlset, v, s, qnrset = svd_qn.svd_qn(
-                    environ_mps[imps + 1].array,
-                    qnbigl,
-                    qnbigr,
-                    environ_mps.qntot,
-                    system="R",
-                    full_matrices=False,
-                )
-                vt = v.T
-
-                environ_mps[imps + 1] = vt.reshape(environ_mps[imps + 1].shape)
-
-                rtensor = environ.GetLR(
-                    "R", imps + 1, environ_mps, mpo, itensor=None, method="System"
-                )
-
-                regular_s = _mu_regularize(s, epsilon=self.evolve_config.reg_epsilon)
-
-                us = u.dot(np.diag(s))
-
-                rtensor = tensordot(rtensor, us, axes=(-1, -1))
-
-                environ_mps[imps] = tensordot(environ_mps[imps], us, axes=(-1, 0))
-                environ_mps.qn[imps + 1] = qnrset
-                environ_mps.qnidx = imps
-
-                S_inv = u.conj().dot(np.diag(1.0 / regular_s)).T
-
-                hop = hop_expr(ltensor, rtensor, [mpo[imps]], shape)
-                func = integrand_func_factory(shape, hop, False, S_inv, True,
-                        coef, ovlp_inv1=S_L_inv_list[imps+1],
-                        ovlp_inv0=S_L_inv_list[imps], ovlp0=S_L_list[imps])
-
-                sol = solve_ivp(
-                    func, (0, evolve_dt), mps[imps].ravel().array, method="RK45"
-                )
-                cmf_rk_steps.append(len(sol.t))
-                ms = sol.y[:, -1].reshape(shape)
-                mps[imps] = ms
-
-            if len(cmf_rk_steps) > 0:
-                steps_stat = stats.describe(cmf_rk_steps)
-                logger.debug(f"{self.evolve_config.method} CMF steps: {steps_stat}")
-
-            if loop == 2:
-                environ_mps = mps
-                evolve_dt /= 2.
-            loop -= 1
-            # new_mps.evolve_config.stat = steps_stat
-
-        return mps
-
-    @adaptive_tdvp
-    def _evolve_tdvp_ps(self, mpo, evolve_dt) -> "Mps":
-        # PhysRevB.94.165116
-        # TDVP projector splitting
-        # one-site
-        if np.iscomplex(evolve_dt):
-            mps = self.copy()
-        else:
-            mps = self.to_complex()
-
-        # construct the environment matrix
-        # almost half is not used. Not a big deal.
-        environ = Environ(mps, mpo)
-
-        # statistics for debug output
-        local_steps = []
-        # sweep for 2 rounds
-        for i in range(2):
-            for imps in mps.iter_idx_list(full=True):
-                system = "L" if mps.to_right else "R"
-                l_array = environ.read("L", imps - 1)
-                r_array = environ.read("R", imps + 1)
-
-                shape = list(mps[imps].shape)
-                hop = hop_expr(l_array, r_array, [asxp(mpo[imps].array)], shape)
-                mps_t, j = expm_krylov(
-                    lambda y: hop(y.reshape(shape)).ravel(),
-                    -1j * evolve_dt / 2, mps[imps].ravel().array
-                )
-                local_steps.append(j)
-                mps_t = mps_t.reshape(shape)
-
-                qnbigl, qnbigr, _ = mps._get_big_qn([imps])
-                u, qnlset, v, qnrset = svd_qn.svd_qn(
-                    asnumpy(mps_t),
-                    qnbigl,
-                    qnbigr,
-                    mps.qntot,
-                    QR=True,
-                    system=system,
-                    full_matrices=False,
-                )
-                vt = v.T
-
-                if not mps.to_right and imps != 0:
-                    mps[imps] = vt.reshape([-1] + shape[1:])
-                    mps.qn[imps] = qnrset
-                    mps.qnidx = imps-1
-
-                    r_array = environ.GetLR(
-                        "R", imps, mps, mpo, itensor=r_array, method="System"
-                    )
-
-                    # reverse update u site
-                    shape_u = u.shape
-                    hop_u = hop_expr(l_array, r_array, [], shape_u)
-                    mps_t, j = expm_krylov(
-                        lambda y: hop_u(y.reshape(shape_u)).ravel(),
-                        1j * evolve_dt / 2, u.ravel()
-                    )
-                    local_steps.append(j)
-                    mps_t = mps_t.reshape(shape_u)
-
-                    mps[imps - 1] = tensordot(mps[imps - 1].array, mps_t, axes=(-1, 0),)
-
-                elif mps.to_right and imps != len(mps) - 1:
-                    mps[imps] = u.reshape(shape[:-1] + [-1])
-                    mps.qn[imps + 1] = qnlset
-                    mps.qnidx = imps+1
-
-                    l_array = environ.GetLR(
-                        "L", imps, mps, mpo, itensor=l_array, method="System"
-                    )
-
-                    # reverse update svt site
-                    shape_svt = vt.shape
-                    hop_svt = hop_expr(l_array, r_array, [], shape_svt)
-                    mps_t, j = expm_krylov(
-                        lambda y: hop_svt(y.reshape(shape_svt)).ravel(),
-                        1j * evolve_dt / 2, vt.ravel()
-                    )
-                    local_steps.append(j)
-                    mps_t = mps_t.reshape(shape_svt)
-
-                    mps[imps + 1] = tensordot(mps_t, mps[imps + 1].array, axes=(1, 0),)
-
-                else:
-                    mps[imps] = mps_t
-            mps._switch_direction()
-
-        steps_stat = stats.describe(local_steps)
-        logger.debug(f"TDVP-PS Krylov space: {steps_stat}")
-        mps.evolve_config.stat = steps_stat
-
-        return mps
-
-    @adaptive_tdvp
-    def _evolve_tdvp_ps2(self, mpo, evolve_dt) -> "Mps":
-        # PhysRevB.94.165116
-        # TDVP projector splitting
-        # two-site
-        if np.iscomplex(evolve_dt):
-            mps = self.copy()
-        else:
-            mps = self.to_complex()
-
-        M = self.compress_config.bond_dim_max_value
-
-        # construct the environment matrix
-        # almost half is not used. Not a big deal.
-        environ = Environ(mps, mpo)
-
-        # statistics for debug output
-        local_steps = []
-        # sweep for 2 rounds
-        for i in range(2):
-            for imps in mps.iter_idx_list(full=False):
-                if mps.to_right:
-                    lidx, cidx0, cidx1, ridx = range(imps - 1, imps + 3)
-                    # the idx of the next site
-                    cidx2 = cidx1
-                    # the idx of the last site
-                    last_idx = len(mps) - 2
-                else:
-                    lidx, cidx0, cidx1, ridx = range(imps - 2, imps + 2)
-                    cidx2 = cidx0
-                    last_idx = 1
-
-                l_array = environ.read("L", lidx)
-                r_array = environ.read("R", ridx)
-
-                # the two-site matrix state
-                ms2 = tensordot(mps[cidx0], mps[cidx1], axes=1)
-                hop = hop_expr(l_array, r_array, [mpo[cidx0], mpo[cidx1]], ms2.shape)
-                mps_t, j = expm_krylov(
-                    lambda y: hop(y.reshape(ms2.shape)).ravel(),
-                    -1j * evolve_dt / 2,
-                    ms2.ravel()
-                )
-                local_steps.append(j)
-
-                mps_t = mps_t.reshape(ms2.shape)
-                qnbigl, qnbigr, _ = mps._get_big_qn([cidx0, cidx1])
-                mps._update_mps(mps_t, [cidx0, cidx1], qnbigl, qnbigr, M)
-                if mps.compress_config.ofs is not None:
-                    mpo.try_swap_site(mps.model, mps.compress_config.ofs_swap_jw)
-                if imps == last_idx:
-                    continue
-
-                if mps.to_right:
-                    l_array = environ.GetLR(
-                        "L", lidx + 1, mps, mpo, itensor=l_array, method="System"
-                    )
-                else:
-                    r_array = environ.GetLR(
-                        "R", ridx - 1, mps, mpo, itensor=r_array, method="System"
-                    )
-
-                # reverse update the next site
-                ms1 = mps[cidx2]
-                hop = hop_expr(l_array, r_array, [mpo[cidx2]], ms1.shape)
-                mps_t, j = expm_krylov(
-                    lambda y: hop(y.reshape(ms1.shape)).ravel(),
-                    1j * evolve_dt / 2, ms1.ravel()
-                )
-                local_steps.append(j)
-                mps_t = mps_t.reshape(ms1.shape)
-                mps[cidx2] = mps_t
-                mps._push_cano(cidx2)
-
-            mps._switch_direction()
-
-        steps_stat = stats.describe(local_steps)
-        logger.debug(f"TDVP-PS Krylov space: {steps_stat}")
-        mps.evolve_config.stat = steps_stat
-
-        return mps
-
-    def evolve_exact(self, h_mpo, evolve_dt, space):
-        MPOprop = Mpo.exact_propagator(self.model, -1j * evolve_dt, space, -h_mpo.offset)
-        new_mps = MPOprop.apply(self, canonicalise=True)
-        self.coeff *= np.exp(-1j * h_mpo.offset * evolve_dt)
-        return new_mps
-
-    @property
-    def digest(self):
-        # used for debugging. Mostly for quickly comparing how two MPSs differ.
-        if 10 < self.site_num or self.is_mpdm:
-            return None
-        prod = np.eye(1).reshape(1, 1, 1)
-        for ms in self:
-            prod = np.tensordot(prod, ms, axes=1)
-            prod = prod.reshape((prod.shape[0], -1, prod.shape[-1]))
-        return {"var": prod.var(), "mean": prod.mean(), "ptp": prod.ptp()}
-
-    def todense(self) -> np.array:
-        dim = np.prod(self.pbond_list)
-        if 20000 < dim:
-            raise ValueError("wavefunction too large")
-        res = np.ones((1, 1, 1))
-        for mt in self:
-            dim1 = res.shape[1] * mt.shape[1]
-            dim2 = mt.shape[-1]
-            res = np.tensordot(res, mt.array, axes=1).reshape(1, dim1, dim2)
-        return res[0, :, 0]
-    
-    def calc_1site_rdm(self, idx=None):
-        r""" Calculate 1-site reduced density matrix
-        
-            :math:`\rho_i = \textrm{Tr}_{j \neq i} | \Psi \rangle \langle \Psi|`
-        
-        Parameters
-        ----------
-        idx : int, list, tuple, optional
-            site index of 1site_rdm. Default is None, which mean all the rdms
-            are calculated.
-        
-        Returns
-        -------
-        rdm: Dict
-            :math:`\{0:\rho_0, 1:\rho_1, \cdots\}`. The key is the index of the site.
-        """
-
-        identity = Mpo.identity(self.model)
-        environ = Environ(self, identity, "R")
-        if idx is None:
-            idx = list(range(self.site_num))
-        elif type(idx) is int:
-            idx = [idx]
-        elif (type(idx) is list) or (type(idx) is tuple):  
-            idx = list(idx)
-        else:
-            assert False
-
-        rdm = {}
-        for ims, ms in enumerate(self):
-            ltensor = environ.GetLR(
-                "L", ims-1, self, identity, itensor=None, method="System"
-            )
-            rtensor = environ.GetLR(
-                "R", ims+1, self, identity, itensor=None, method="Enviro"
-            )
-            if ims not in idx:
-                continue
-
-            ltensor = ltensor.reshape(ltensor.shape[0], ltensor.shape[-1])
-            rtensor = rtensor.reshape(rtensor.shape[0], rtensor.shape[-1])
-            
-            tensor = tensordot(ltensor, ms.conj(), ([0],[0]))
-            tensor = tensordot(tensor, rtensor, ([-1],[0]))
-            if ms.ndim == 3:
-                tensor = tensordot(tensor, ms, ([0,-1],[0,-1]))
-            else:
-                tensor = tensordot(tensor, ms, ([0,-1,-2],[0,-1,-2]))
-            assert xp.allclose(tensor, tensor.T.conj())
-            rdm[ims] = asnumpy(tensor)
-
-        return rdm
-    
-    def calc_2site_rdm(self):
-        r""" Calculate 2-site reduced density matrix
-        
-        :math:`\rho_{ij} = \textrm{Tr}_{k \neq i, k \neq j} | \Psi \rangle \langle \Psi |`.
-        
-        Returns
-        -------
-        rdm: Dict
-            :math:`\{(0,1):\rho_{01}, (0,2):\rho_{02}, \cdots\}`. The key is a tuple of index of the site.
-        """
-        
-        identity = Mpo.identity(self.model)
-        environ_R = Environ(self, identity, "R")
-        environ_L = Environ(self, identity, "L")
-        L_component = []
-        R_component = []
-        rdm = {}
-        # first construct 1-site environment
-        for ims, ms in enumerate(self):
-            ltensor = environ_L.GetLR("L", ims-1, self, identity,
-                    itensor=None, method="Enviro")
-            ltensor = ltensor.reshape(ltensor.shape[0], ltensor.shape[-1])
-            tensor = tensordot(ltensor, ms.conj(), ([0],[0]))
-            if ms.ndim == 3:
-                tensor = tensordot(tensor, ms, ([0],[0]))
-            elif ms.ndim == 4:
-                tensor = tensordot(tensor, ms, ([0,2],[0,2]))
-            L_component.append(tensor.transpose((0,2,1,3)))
-            
-            rtensor = environ_R.GetLR("R", ims+1, self, identity,
-                    itensor=None, method="Enviro")
-            rtensor = rtensor.reshape(rtensor.shape[0], rtensor.shape[-1])
-            tensor = tensordot(ms.conj(), rtensor, ([-1],[0]))
-            if ms.ndim == 3:
-                tensor = tensordot(tensor, ms, ([-1],[-1]))
-            elif ms.ndim == 4:
-                tensor = tensordot(tensor, ms, ([2,-1],[2,-1]))
-            R_component.append(tensor.transpose((0,2,1,3)))
-        
-        # merge two 1-site environment together
-        for ims in range(self.site_num):
-            tensor = L_component[ims]
-            for jms in range(ims+1, self.site_num):
-                if jms != ims+1:
-                    kms = jms - 1
-                    tensor = tensordot(tensor, self[kms].conj(), ([2],[0]))
-                    if self[kms].ndim == 3:
-                        tensor = tensordot(tensor, self[kms], ([2,3],[0,1]))
-                    elif self[kms].ndim == 4:
-                        tensor = tensordot(tensor, self[kms], ([2,3,4],[0,1,2]))
-                
-                rtensor = R_component[jms]
-                res = tensordot(tensor, rtensor,
-                        ([2,3],[0,1])).transpose(0,2,1,3)
-                rdm[(ims, jms)] = asnumpy(res.reshape(res.shape[0]*res.shape[1],-1))
-        return rdm
-    
-    def calc_edof_rdm(self) -> np.ndarray:
-        r"""Calculate the reduced density matrix of electronic DoF
-        
-        :math:`\rho_{ij} = \langle \Psi | a_i^\dagger a_j | \Psi \rangle`
-        
-        """
-        
-        key = "edof_reduced_density_matrix"
-        n_e = self.model.n_edofs
-        e_dofs = self.model.e_dofs
-        if key not in self.model.mpos:
-            mpos = []
-            for idx, dof1 in enumerate(e_dofs):
-                for dof2 in e_dofs[idx:]:
-                    op = Op(r"a^\dagger a", [dof1, dof2])
-                    mpo = Mpo(self.model, terms=op)
-                    mpos.append(mpo)
-            self.model.mpos[key] = mpos
-        else:
-            mpos = self.model.mpos[key]
-        expectations = deque(self.expectations(mpos))
-        reduced_density_matrix = np.zeros((n_e, n_e), dtype=backend.complex_dtype)
-        for idx in range(n_e):
-            for jdx in range(idx, n_e):
-                reduced_density_matrix[idx, jdx] = expectations.popleft()
-                reduced_density_matrix[jdx, idx] = np.conj(reduced_density_matrix[idx, jdx])
-
-        return reduced_density_matrix
-    
-    def calc_entropy(self, entropy_type):
-        r""" Calculate 1site, 2site, mutual and bond Von Neumann entropy
-
-            :math:`\textrm{entropy} = -\textrm{Tr}(\rho \ln \rho)`
-            where :math:`\ln` stands for natural logarithm.
-            
-            1site entropy is the entropy between any site and the other
-            ``(N-1)`` sites.
-            2site entropy is the entropy between any two sites and the other 
-            ``(N-2)`` sites.
-            mutual entropy characterize the entropy between any two sites.
-            bond entropy is the entropy between L-block and R-block.
-
-        Parameters
-        ----------
-        entropy_type : str
-            "1site", "2site", "mutual", "bond"
-        
-        Returns
-        -------
-        entropy : dict, ndarray
-            if entropy_type = "1site" or "2site", a dictionary is returned and the
-            key is the index or the tuple of index of mps sites, else
-            an ndarray is returned.
-        
-        """
-
-        if entropy_type in ["1site", "2site"]:
-            if entropy_type == "1site":
-                rdm = self.calc_1site_rdm()
-            else:
-                rdm = self.calc_2site_rdm()
-            
-            entropy = {}
-            for key, dm in rdm.items():
-                w, v = scipy.linalg.eigh(dm)
-                entropy[key] = calc_vn_entropy(w)
-
-        elif entropy_type == "mutual":
-            entropy = self.calc_2site_mutual_entropy()
-        elif entropy_type == "bond":
-            entropy = self.calc_bond_entropy()
-        else:
-            raise ValueError(f"unsupported entropy type {entropy_type}")
-        return entropy
-    
-    def calc_2site_mutual_entropy(self):
-        r""" 
-        Calculate mutual entropy between two sites.
-        
-        :math:`m_{ij} = (s_i + s_j - s_{ij})/2`
-            
-        See Chemical Physics 323 (2006) 519–531
-        
-        Returns
-        -------
-        mutual_entropy : 2d np.ndarry
-            mutual entropy with shape (nsite, nsite)
-
-        """
-        entropy_1site = self.calc_entropy("1site")
-        entropy_2site = self.calc_entropy("2site")
-        nsites = self.site_num
-        mut_entropy = np.zeros((nsites, nsites))
-        for isite, jsite in itertools.combinations(range(nsites),2):
-            key = (isite, jsite) if (isite, jsite) in entropy_2site.keys() else (jsite, isite)
-            mut_entropy[isite, jsite] = (entropy_1site[isite] + entropy_1site[jsite] -
-                    entropy_2site[key]) / 2
-        mut_entropy += mut_entropy.T
-        return mut_entropy
-
-    def calc_bond_entropy(self) -> np.ndarray:
-        r"""
-        Calculate von Neumann entropy at each bond according to :math:`S = -\textrm{Tr}(\rho \ln \rho)`
-        where :math:`\rho` is the reduced density matrix of either block.
-
-        Returns
-        -------
-        S : 1D array
-            a NumPy array containing the entropy values.
-        
-        """
-        
-        # Make sure that the bond entropy is from the left to the right and not
-        # destroy the original mps
-        mps = self.copy()
-        mps.ensure_right_canonical()
-        _, s_list = mps.compress(temp_m_trunc=np.inf, ret_s=True)
-        return np.array([calc_vn_entropy(sigma ** 2) for sigma in s_list])
-
-    def dump(self, fname):
-        super().dump(fname, other_attrs=["coeff"])
-
-    def __setitem__(self, key, value):
-        return super().__setitem__(key, value)
-
-    
-    def add(self, other):
-        if not np.allclose(self.coeff, other.coeff):
-            self.scale(self.coeff, inplace=True)
-            other.scale(other.coeff, inplace=True)
-            self.coeff = 1
-            other.coeff = 1
-        return super().add(other)
-    
-    def distance(self, other) -> float:
-        if not np.allclose(self.coeff, other.coeff):
-            self.scale(self.coeff, inplace=True)
-            other.scale(other.coeff, inplace=True)
-            self.coeff = 1
-            other.coeff = 1
-        return super().distance(other)
-
-
-def projector(
-    ms: xp.ndarray, left: bool, Ovlp_inv1: xp.ndarray = None, Ovlp0: xp.ndarray = None
-) -> xp.ndarray:
-    if left:
-        axes = (-1, -1)
-    else:
-        axes = (0, 0)
-
-    if Ovlp_inv1 is None:
-        proj = xp.tensordot(ms, ms.conj(), axes=axes)
-    else:
-        # consider the case that the canonical condition is not fulfilled
-        if left:
-            proj = xp.tensordot(Ovlp0, ms, axes=(-1, 0))
-            proj = xp.tensordot(proj, Ovlp_inv1, axes=(-1, 0))
-            proj = xp.tensordot(proj, ms.conj(), axes=(-1, -1))
-        else:
-            proj = xp.tensordot(ms, Ovlp0, axes=(-1, 0))
-            proj = xp.tensordot(Ovlp_inv1, proj, axes=(-1, 0))
-            proj = xp.tensordot(proj, ms.conj(), axes=(0, 0))
-
-    if left:
-        sz = int(np.prod(ms.shape[:-1]))
-    else:
-        sz = int(np.prod(ms.shape[1:]))
-    Iden = xp.array(xp.diag(xp.ones(sz)), dtype=backend.real_dtype).reshape(proj.shape)
-    proj = Iden - proj
-    return proj
-
-def integrand_func_factory(
-    shape,
-    hop,
-    islast,
-    S_inv: Union[np.ndarray, xp.ndarray],
-    left: bool,
-    coef: complex,
-    ovlp_inv1: Union[xp.ndarray, np.ndarray] = None,
-    ovlp_inv0: Union[xp.ndarray, np.ndarray] = None,
-    ovlp0: Union[xp.ndarray, np.ndarray] = None,
-):
-    S_inv, ovlp_inv1, ovlp_inv0, ovlp0 = map(asxp, [S_inv, ovlp_inv1, ovlp_inv0, ovlp0])
-    # left == True: projector operate on the left side of the HC
-    # Ovlp0 is (#.conj, #), Ovlp_inv0 = (#, #.conj), Ovlp_inv1 = (#, #.conj)
-    # S_inv is (#.conj, #)
-    def func(t, y):
-        y0 = asxp(y.reshape(shape))
-        HC = hop(y0)
-        if not islast:
-            proj = projector(y0, left, ovlp_inv1, ovlp0)
-            if y0.ndim == 3:
-                if left:
-                    HC = tensordot(proj, HC, axes=([2, 3], [0, 1]))
-                else:
-                    HC = tensordot(HC, proj, axes=([1, 2], [2, 3]))
-            elif y0.ndim == 4:
-                if left:
-                    HC = tensordot(proj, HC, axes=([3, 4, 5], [0, 1, 2]))
-                else:
-                    HC = tensordot(HC, proj, axes=([1, 2, 3], [3, 4, 5]))
-
-        if left:
-            if ovlp_inv0 is not None:
-                HC = tensordot(ovlp_inv0, HC, axes=(-1, 0))
-            return tensordot(HC, S_inv, axes=(-1, 0)).ravel() / coef
-        else:
-            if ovlp_inv0 is not None:
-                HC = tensordot(HC, ovlp_inv0, axes=(-1, -1))
-            return tensordot(S_inv, HC, axes=(0, 0)).ravel() / coef
-
-    return func
-
-
-def transferMat(mps, mpsconj, domain, imps, val) -> np.ndarray:
-    """
-    calculate the transfer matrix from the left hand or the right hand
-    """
-    if mpsconj is not None:
-        ms, ms_conj = mps[imps].array, mpsconj[imps].array
-    else:
-        ms = mps[imps].array
-        ms_conj = ms.conj()
-
-    if mps[0].ndim == 3:
-        if domain == "R":
-            val = tensordot(ms_conj, val, axes=(2, 0))
-            val = tensordot(val, ms, axes=([1, 2], [1, 2]))
-        elif domain == "L":
-            val = tensordot(ms_conj, val, axes=(0, 0))
-            val = tensordot(val, ms, axes=([0, 2], [1, 0]))
-        else:
-            assert False
-    elif mps[0].ndim == 4:
-        if domain == "R":
-            val = tensordot(ms_conj, val, axes=(3, 0))
-            val = tensordot(val, ms, axes=([1, 2, 3], [1, 2, 3]))
-        elif domain == "L":
-            val = tensordot(ms_conj, val, axes=(0, 0))
-            val = tensordot(val, ms, axes=([0, 3, 1], [1, 0, 2]))
-        else:
-            assert False
-    else:
-        raise ValueError(f"the dim of local mps is not correct: {mps[0].ndim}")
-
-    return asnumpy(val)
-
-
-def _mu_regularize(s, epsilon=1e-10):
-    """
-    regularization of the singular value of the reduced density matrix
-    """
-    epsilon = np.sqrt(epsilon)
-    return s + epsilon * np.exp(-s / epsilon)
-
-
-class BraKetPair:
-    def __init__(self, bra_mps, ket_mps, mpo=None):
-        self.bra_mps = bra_mps
-        self.ket_mps = ket_mps
-        self.mpo = mpo
-        self.ft = self.calc_ft()
-
-    def calc_ft(self):
-        if self.mpo is None:
-            dot = self.bra_mps.conj().dot(self.ket_mps)
-        else:
-            dot = self.ket_mps.expectation(self.mpo, self.bra_mps.conj())
-        return complex(
-            dot * np.conjugate(self.bra_mps.coeff)
-            * self.ket_mps.coeff
-        )
-
-    def __str__(self):
-        if np.iscomplexobj(self.ft):
-            # if negative, sign is included in the imag part
-            sign = "+" if 0 <= self.ft.imag else ""
-            ft_str = "%g%s%gj" % (self.ft.real, sign, self.ft.imag)
-        else:
-            ft_str = "%g" % self.ft
-        return "bra: %s, ket: %s, ft: %s" % (self.bra_mps, self.ket_mps, ft_str)
-
-    def __iter__(self):
-        return iter((self.bra_mps, self.ket_mps))
-
-
-def min_abs(t1, t2):
-    # t1, t2 could be int, float, complex
-    # return the number with smaller norm
-
-    assert xp.iscomplex(t1) == xp.iscomplex(t2)
-
-    if xp.absolute(t1) < xp.absolute(t2):
-        return t1
-    else:
-        return t2
-
-
-def _construct_freq_environ(mpos_hash: List[List[int]], hash_to_obj: Dict[int, Matrix], mps: Mps, domain: str, mps_conj):
-    """
-    Construct environment tensors that are most frequently shown in the group of MPOs
-    """
-    assert domain in ["L", "R"]
-    # count mpo sequence frequency
-    counter = Counter()
-    for mpo_hash in mpos_hash:
-        for i in range(1, len(mpo_hash)+1):
-            if domain == "L":
-                mpo_seq = mpo_hash[:i]
-            else:
-                mpo_seq = reversed(mpo_hash[-i:])
-            counter.update([tuple(mpo_seq)])
-
-    # transform the counter into a list of matrices.
-    # The most frequent sequences first. If the same freq, then shorter sequences first
-    # Note that shorter sequences are not less frequent than longer sequences
-    most_common = list(counter.items())
-    most_common.sort(key=lambda x: (-x[1], len(x[0])))
-    matrices_list = []
-    hash_list = []
-    for hashes, n in most_common:
-        # discard unique ones because they do not need to be cached
-        if n == 1:
-            break
-        # cache ``len(mps)`` sequences
-        # sequences with the same length may be treated differently.
-        if len(mps) < len(matrices_list):
-            break
-        hash_list.append(hashes)
-        matrices_list.append(list(map(hash_to_obj.get, hashes)))
-
-    # contract the tensors
-    result = {(): xp.ones((1, 1, 1), dtype=backend.real_dtype)}
-    for m_hashes, matrices in zip(hash_list, matrices_list):
-        environ = result[tuple(m_hashes[:-1])]
-        if domain == "L":
-            idx = len(matrices)-1
-        else:
-            idx = -len(matrices)
-        ms, ms_conj = mps[idx], mps_conj[idx]
-        result[tuple(m_hashes)] = contract_one_site(environ, ms, matrices[-1], domain=domain, ms_conj=ms_conj)
-    return result
-
-
-def _get_freq_environ(environ_dict, mpo, domain, max_length):
-    assert domain in ["L", "R"]
-
-    if domain == "L":
-        it = mpo
-    else:
-        it = reversed(mpo)
-
-    hashes = []
-    for mo in it:
-        hashes.append(hash(mo))
-        if (not tuple(hashes) in environ_dict) or (max_length < len(hashes)):
-            hashes.pop()
-            break
-    if domain == "L":
-        i = len(hashes) - 1
-    else:
-        i = len(mpo) - len(hashes)
-
-    environ = environ_dict[tuple(hashes)]
-    return environ, i
+# -*- encoding: utf-8 -*-
+
+import logging
+from collections import Counter, deque
+from functools import wraps, reduce
+from typing import Union, List, Dict
+import itertools
+
+
+import scipy
+from scipy import stats
+
+from renormalizer.lib import solve_ivp, expm_krylov
+from renormalizer.model import Model, Op, basis as ba
+from renormalizer.mps import svd_qn
+from renormalizer.mps.svd_qn import add_outer, get_qn_mask
+from renormalizer.mps.backend import backend, np, xp
+from renormalizer.mps.lib import (
+    Environ,
+    select_basis,
+    compressed_sum,
+    contract_one_site,
+    cvec2cmat
+)
+from renormalizer.mps.matrix import (
+    multi_tensor_contract,
+    ones,
+    tensordot,
+    Matrix,
+    asnumpy,
+    asxp)
+from renormalizer.mps.mp import MatrixProduct
+from renormalizer.mps.hop_expr import hop_expr
+from renormalizer.mps.mpo import Mpo
+from renormalizer.utils import (
+    OptimizeConfig,
+    CompressCriteria,
+    EvolveConfig,
+    EvolveMethod
+)
+from renormalizer.utils.utils import calc_vn_entropy
+
+logger = logging.getLogger(__name__)
+
+
+def adaptive_tdvp(fun):
+    # evolve t/2 (twice) and t to obtain the O(dt^3) error term in 2nd-order Trotter decomposition
+    # J. Chem. Phys. 146, 174107 (2017)
+
+    @wraps(fun)
+    def adaptive_fun(self: "Mps", mpo, evolve_target_t):
+
+        if not self.evolve_config.adaptive:
+            return fun(self, mpo, evolve_target_t)
+        config: EvolveConfig = self.evolve_config.copy()
+        config.check_valid_dt(evolve_target_t)
+
+        cur_mps = self
+        # prevent bug
+        del self
+
+        # setup some constant
+        p_restart = 0.5  # restart threshold
+        p_min = 0.1  # safeguard for minimal allowed p
+        p_max = 2.  # safeguard for maximal allowed p
+
+        evolved_t = 0
+
+        while True:
+
+            dt = min_abs(config.guess_dt, evolve_target_t - evolved_t)
+            logger.debug(
+                    f"guess_dt: {config.guess_dt}, try time step size: {dt}"
+            )
+            
+            mps_half1 = fun(cur_mps, mpo, dt / 2)
+            mps_half2 = fun(mps_half1, mpo, dt / 2)
+            mps = fun(cur_mps, mpo, dt)
+            dis = mps.distance(mps_half2)
+
+            # prevent bug. save "some" memory.
+            del mps_half1, mps
+
+            p = (0.75 * config.adaptive_rtol / (dis/mps_half2.mp_norm + 1e-30)) ** (1./3)
+            logger.debug(f"distance: {dis}, enlarge p parameter: {p}")
+            if p < p_min:
+                p = p_min
+            if p_max < p:
+                p = p_max
+
+            # rejected
+            if p < p_restart:
+                config.guess_dt = dt * p
+                logger.debug(
+                    f"evolution not converged, new guess_dt: {config.guess_dt}"
+                )
+                continue
+
+            # accepted
+            evolved_t += dt
+            if np.allclose(evolved_t, evolve_target_t):
+                # normal exit. Note that `dt` could be much less than actually tolerated for the last step
+                # so use `guess_dt` for the last step. Slight inaccuracy won't harm.
+                mps_half2.evolve_config.guess_dt = config.guess_dt
+                logger.debug(
+                    f"evolution converged, new guess_dt: {mps_half2.evolve_config.guess_dt}"
+                )
+                return mps_half2
+            else:
+                # in this case `config.guess_dt == dt`
+                config.guess_dt *= p
+                logger.debug(f"sub-step {dt} further, evolved: {evolved_t}, new guess_dt: {config.guess_dt}")
+                cur_mps = mps_half2
+
+    return adaptive_fun
+
+
+class Mps(MatrixProduct):
+    @classmethod
+    def random(cls, model: Model, qntot, m_max, percent=1.0) -> "Mps":
+        # a high percent makes the result more random
+        # sometimes critical for getting correct optimization result
+        mps = cls()
+        mps.model = model
+        if isinstance(qntot, int):
+            qntot = np.array([qntot])
+        qn_size = len(qntot)
+        assert qn_size == model.qn_size
+        mps.qn = [np.zeros((1, qn_size), dtype=int)]
+        dim_list = [1]
+
+        for imps in range(model.nsite - 1):
+
+            # quantum number
+            qnbig = add_outer(mps.qn[imps], mps._get_sigmaqn(imps)).reshape(-1, qn_size)
+            u_set = []
+            s_set = []
+            qnset = []
+
+            for iblock in set([tuple(t) for t in qnbig]):
+                if np.all(np.array(qntot) < np.array(iblock)):
+                    continue
+                # find the quantum number index
+                indices = [i for i, x in enumerate(qnbig) if tuple(x) == iblock]
+                assert len(indices) != 0
+                a = np.random.random([len(indices), len(indices)]) - 0.5
+                a = a + a.T
+                s, u = scipy.linalg.eigh(a=a)
+                u_set.append(svd_qn.blockrecover(indices, u, len(qnbig)))
+                s_set.append(s)
+                qnset += [iblock] * len(indices)
+
+            u_set = np.concatenate(u_set, axis=1)
+            s_set = np.concatenate(s_set)
+            mt, mpsdim, mpsqn, nouse = select_basis(
+                u_set, s_set, qnset, u_set, m_max, percent=percent
+            )
+            # add the next mpsdim
+            dim_list.append(mpsdim)
+            mps.append(mt.reshape((dim_list[imps], -1, dim_list[imps + 1])))
+            mps.qn.append(mpsqn)
+
+        # the last site
+        mps.qn.append(np.zeros((1, qn_size), dtype=int))
+        dim_list.append(1)
+        last_mt = (
+            xp.random.random([dim_list[-2], mps.pbond_list[-1], dim_list[-1]]) - 0.5
+        )
+        # normalize the mt so that the whole mps is normalized
+        last_mt /= xp.linalg.norm(last_mt.flatten())
+        mps.append(last_mt)
+
+        mps.qnidx = len(mps) - 1
+        mps.to_right = False
+        mps.qntot = np.array(qntot)
+
+        return mps
+
+    @classmethod
+    def hartree_product_state(cls, model, condition: Dict):
+        r"""
+        Construct a Hartree product state
+        
+        Args:
+            model (:class:`~renormalizer.model.Model`): Model information.
+            condition (Dict): Dict with format ``{dof:local_state}``.
+                The default local state for dofs not specified is the "0" state.
+                An example is ``{"e_1":1, "v_0":2, "v_3":[0, 0.707, 0.707]}``.
+
+                Note:
+                    If there are bases that contain multiple dofs in the model, the value of the dict
+                    is the state of all dofs of the basis. For example,
+                    if a basis contains ``"e_1"``, ``"e_2"`` and ``"e_3"``,
+                    ``{"e_1": 2}`` (``{"e_1": [0, 0, 1]}``) means ``"e_3"`` is occupied and
+                    ``{"e_1": 1}`` (``{"e_1": [0, 1, 0]}``) means ``"e_2"`` is occupied.
+                    Be aware that in :class:`renormalizer.utils.basis.BasisMultiElectronVac` the vacuum state
+                    is added to the ``0`` index.
+
+        Returns:
+            Constructed mps (:class:`Mps`)
+        """
+        
+        mps = cls()
+        mps.model = model
+        mps.build_empty_mp(model.nsite)
+        qn_size = model.qn_size
+        mps.qn = [np.zeros((1, qn_size), dtype=int)]
+
+        # check that the condition is not duplicated
+        # each site has at most 1 single key to assign the occupation  
+        index = [model.dof_to_siteidx[key] for key in condition.keys()]
+        assert len(index) == len(set(index))
+        # replace the dof_name key to site_index key
+        condition = {model.dof_to_siteidx[key]:value for key, value in
+                condition.items()}
+
+        for isite, local_basis in enumerate(model.basis):
+            pdim = local_basis.nbas
+            ms = np.zeros((1, pdim, 1))
+            local_state = condition.pop(isite,0)
+            if isinstance(local_state, int):
+                ms[0, local_state, 0] = 1.
+                qn = local_basis.sigmaqn[local_state]
+            else:
+                ms[0, :, 0] = local_state
+                # quantum numbers for all states occupied
+                all_qn = np.array(local_basis.sigmaqn)[np.nonzero(local_state)]
+                if not np.allclose(all_qn.std(axis=0), 0):
+                    raise ValueError("Quantum numbers are mixed in the condition.")
+                qn = all_qn[0]
+
+            mps[isite] = ms
+            mps.qn.append(mps.qn[-1] + qn.reshape(1, qn_size))
+
+        if len(condition) != 0:
+            raise ValueError(f"Condition not completely used: {condition}")
+        mps.qntot = mps.qn[-1][0]
+        mps.qn[-1] = np.zeros((1, qn_size), dtype=int)
+        mps.qnidx = model.nsite - 1
+        mps.to_right = False
+
+        return mps
+
+    @classmethod
+    def ground_state(cls, model: Model, max_entangled: bool,
+            normalize:bool=True, condition:Dict=None):
+        r"""
+        Obtain ground state at :math:`T = 0` or :math:`T = \infty` (maximum entangled).
+        Electronic DOFs are always at ground state. and vibrational DOFs depend on ``max_entangled``.
+        For Spin-Boson model the electronic DOF also depends on ``max_entangled``.
+        
+
+        Parameters
+        ----------
+            model : :class:`~renormalizer.model.Model`
+                system information.
+            max_entangled : bool
+                temperature of the vibrational DOFs. If set to ``True``,
+                :math:`T = \infty` and if set to ``False``, :math:`T = 0`.
+            normalize: bool, optional
+                if the returned Mps are normalized when ``max_entangled=True``.
+                Default is True. If ``normalize=False``, the vibrational part is identity.
+            condition: dict, optional
+                the same as `hartree_product_state`. only used in ba.BasisMultiElectron
+                cases to define the occupation. Default is ``None``.
+        Returns
+        -------
+            mps : renormalizer.mps.Mps
+        
+        """
+        
+        mps = cls()
+        mps.model = model
+        mps.qn = [np.zeros((1, model.qn_size), dtype=int)] * (model.nsite + 1)
+        mps.qnidx = model.nsite - 1
+        mps.to_right = False
+        mps.qntot = np.zeros(model.qn_size, dtype=int)
+            
+        mps.build_empty_mp(model.nsite)
+        
+        if condition is not None:
+            # check that the condition is not duplicated
+            # each site has at most 1 single key to assign the occupation  
+            index = [model.dof_to_siteidx[key] for key in condition.keys()]
+            assert len(index) == len(set(index))
+            # replace the dof_name key to site_index key
+            condition = {model.dof_to_siteidx[key]:value for key, value in
+                    condition.items()}
+
+        for isite, local_basis in enumerate(model.basis):
+            pdim = local_basis.nbas
+            ms = np.zeros((1, pdim, 1))
+            if local_basis.is_phonon:
+                if max_entangled:
+                    if normalize:
+                        ms[0, :, 0] = 1.0 / np.sqrt(pdim)
+                    else:
+                        ms[0, :, 0] = 1.0
+                else:
+                    ms[0, 0, 0] = 1.0
+                mps[isite] = ms
+
+            elif local_basis.is_electron or local_basis.is_spin:
+
+                if isinstance(local_basis, ba.BasisSimpleElectron):
+                    # simple electron site
+                    ms[0,0,0] = 1.
+                elif isinstance(local_basis, ba.BasisMultiElectron):
+                    assert condition is not None
+                    local_state = condition.pop(isite)
+                    if isinstance(local_state, int):
+                        ms[0, local_state, 0] = 1.
+                        qn = local_basis.sigmaqn[local_state]
+                    else:
+                        ms[0, :, 0] = local_state
+                        qn = local_basis.sigmaqn[np.nonzero(local_state)]
+                    assert np.allclose(qn, 0)
+                    if max_entangled and normalize:
+                        ms /= np.linalg.norm(ms)
+
+                elif isinstance(local_basis, ba.BasisMultiElectronVac):
+                        ms[0,0,0] = 1.
+                elif isinstance(local_basis, ba.BasisHalfSpin):
+                    if max_entangled:
+                        if normalize:
+                            ms[0,:,0] = 1. / np.sqrt(2.)
+                        else:
+                            ms[0,:,0] = 1.
+                    else:
+                        ms[0,0,0] = 1.
+                else:
+                    raise NotImplementedError
+                mps[isite] = ms
+        for ms in mps:
+            assert ms is not None
+        return mps
+
+    @classmethod
+    def load(cls, model: Model, fname: str):
+        npload = np.load(fname, allow_pickle=True)
+        mp = cls()
+        mp.model = model
+        for i in range(int(npload["nsites"])):
+            mt = npload[f"mt_{i}"]
+            if np.iscomplexobj(mt):
+                mp.dtype = backend.complex_dtype
+            else:
+                mp.dtype = backend.real_dtype
+            mp.append(mt)
+        mp.qn = npload["qn"]
+        mp.qnidx = int(npload["qnidx"])
+        mp.qntot = npload["qntot"]
+        version = npload["version"]
+        if version == "0.1":
+            mp.to_right = bool(npload["left"])
+            # in this protocol, TDH and coeff is not dumped
+            logger.warning("Using old dump/load protocol. TD Hartree part will be lost")
+            mp.coeff = 1
+        elif version == "0.2":
+            mp.to_right = bool(npload["to_right"])
+            # in this protocol, TDH is dumped, but it's not useful anymore
+            logger.warning("Using old dump/load protocol. TD Hartree part will be lost")
+            mp.coeff = npload["tdh_wfns"][-1]
+        elif version == "0.3":
+            mp.to_right = bool(npload["to_right"])
+            mp.coeff = npload["coeff"].item(0)
+        else:
+            raise ValueError(f"Unknown dump version: {version}")
+        return mp
+
+    @classmethod
+    def from_dense(cls, model, wfn: np.ndarray):
+        # for debugging
+        mp = cls()
+        mp.model = model
+        if np.iscomplexobj(wfn):
+            mp.dtype = backend.complex_dtype
+        else:
+            mp.dtype = backend.real_dtype
+        residual_wfn = wfn.reshape([1] + [b.nbas for b in model.basis] + [1])
+        for i in range(len(model.basis) - 1):
+            wfn_2d = residual_wfn.reshape(residual_wfn.shape[0] * residual_wfn.shape[1], -1)
+            q, r = np.linalg.qr(wfn_2d)
+            mp.append(q.reshape(residual_wfn.shape[0], residual_wfn.shape[1], q.shape[1]))
+            residual_wfn = r.reshape([r.shape[0]] + list(residual_wfn.shape[2:]))
+        assert residual_wfn.ndim == 3
+        mp.append(residual_wfn)
+        mp.build_empty_qn()
+        return mp
+
+    def __init__(self):
+        super().__init__()
+        self.coeff: Union[float, complex] = 1
+
+        self.optimize_config: OptimizeConfig = OptimizeConfig()
+        self.evolve_config: EvolveConfig = EvolveConfig()
+
+    def conj(self) -> "Mps":
+        new_mps = super().conj()
+        new_mps.coeff = new_mps.coeff.conjugate()
+        return new_mps
+
+    def to_complex(self, inplace=False) -> "Mps":
+        new_mp = super(Mps, self).to_complex(inplace=inplace)
+        new_mp.coeff = complex(new_mp.coeff)
+        return new_mp
+
+    def _get_sigmaqn(self, idx):
+        return self.model.basis[idx].sigmaqn
+
+    @property
+    def is_mps(self):
+        return True
+
+    @property
+    def is_mpo(self):
+        return False
+
+    @property
+    def is_mpdm(self):
+        return False
+
+    @property
+    def nexciton(self):
+        return self.qntot
+
+    @property
+    def norm(self):
+        '''the norm of the total wavefunction
+        '''
+        return np.linalg.norm(self.coeff) * self.mp_norm
+
+    def _expectation_path(self):
+        # S--a--S--e--S
+        # |     |     |
+        # |     d     |
+        # |     |     |
+        # O--b--O--g--O
+        # |     |     |
+        # |     f     |
+        # |     |     |
+        # S--c--S--h--S
+        path = [
+            ([0, 1], "abc, cfh -> abfh"),
+            ([3, 0], "abfh, bdfg -> ahdg"),
+            ([2, 0], "ahdg, ade -> hge"),
+            ([1, 0], "hge, egh -> "),
+        ]
+        return path
+
+    def _expectation_conj(self):
+        return self.conj()
+
+    def expectation(self, mpo, self_conj=None) -> Union[float, complex]:
+        if self_conj is None:
+            self_conj = self._expectation_conj()
+        environ = Environ(self, mpo, "R", mps_conj=self_conj)
+        l = xp.ones((1, 1, 1), dtype=self.dtype)
+        r = environ.read("R", 1)
+        path = self._expectation_path()
+        val = multi_tensor_contract(path, l, self[0], mpo[0], self_conj[0], r)
+        if np.isclose(float(val.imag), 0):
+            return float(val.real)
+        else:
+            return complex(val)
+        # This is time and memory consuming
+        # return self_conj.dot(mpo.apply(self)).real
+
+    def expectations(self, mpos, self_conj=None, opt=True) -> np.ndarray:
+
+        if not opt:
+            # the naive way, slow and time consuming. Yet predictable and reliable
+            return np.array([self.expectation(mpo, self_conj) for mpo in mpos])
+
+        # optimized way, cache for intermediates
+        # hash is used as indices of the matrices.
+        # The chance for collision (the same hash for two different matrices) is
+        # about 1-0.99999999999997 in 1000 matrices.
+        # In which case a RuntimeError is raised and rerun the job should solve the problem
+        hash_to_obj = dict()
+        mpos_hash: List[List] = []
+        for mpo in mpos:
+            mpo_hash = []
+            for m in mpo:
+                m_hash = hash(m)
+                if m_hash not in hash_to_obj:
+                    hash_to_obj[m_hash] = m
+                else:
+                    if not np.allclose(hash_to_obj[m_hash], m.array):
+                        raise RuntimeError("Rare hash collision")
+                mpo_hash.append(m_hash)
+            mpos_hash.append(mpo_hash)
+
+        if self_conj is None:
+            self_conj = self._expectation_conj()
+        l_environ_dict = _construct_freq_environ(mpos_hash, hash_to_obj, self, "L", self_conj)
+        r_environ_dict = _construct_freq_environ(mpos_hash, hash_to_obj, self, "R", self_conj)
+        results = []
+        for mpo in mpos:
+            l_environ, l_idx = _get_freq_environ(l_environ_dict, mpo, "L", np.inf)
+            r_environ, r_idx = _get_freq_environ(r_environ_dict, mpo, "R", len(mpo)-l_idx-1)
+            for i in range(l_idx+1, r_idx):
+                l_environ = contract_one_site(l_environ, self[i], mpo[i], "L", self_conj[i])
+            results.append(complex(l_environ.flatten() @ r_environ.flatten()))  # cast to python type
+
+        results = np.array(results)
+        if np.allclose(results.imag, 0):
+            return results.real
+        else:
+            return results
+
+    @property
+    def ph_occupations(self):
+        r"""
+        phonon occupations :math:`b^\dagger_i b_i` for each electronic DoF.
+        The order is defined by :attr:`~renormalizer.model.model.v_dofs`.
+        """
+        key = "ph_occupations"
+        # ph_occupations is actually the occupation of the basis
+        if key not in self.model.mpos:
+            mpos = []
+            for dof in self.model.v_dofs:
+                mpos.append(Mpo(self.model, Op("n", dof)))
+            self.model.mpos[key] = mpos
+        else:
+            mpos = self.model.mpos[key]
+
+        return self.expectations(mpos)
+
+    @property
+    def e_occupations(self):
+        r"""
+        Electronic occupations :math:`a^\dagger_i a_i` for each electronic DoF.
+        The order is defined by :attr:`~renormalizer.model.model.e_dofs`.
+        """
+        key = "e_occupations"
+        if key not in self.model.mpos:
+            mpos = []
+            for dof in self.model.e_dofs:
+                mpos.append(Mpo(self.model, Op(r"a^\dagger a", dof)))
+            self.model.mpos[key] = mpos
+        else:
+            mpos = self.model.mpos[key]
+        return self.expectations(mpos)
+
+    def metacopy(self) -> "Mps":
+        new: Mps = super().metacopy()
+        new.coeff = self.coeff
+        new.optimize_config = self.optimize_config
+        # evolve_config has its own data
+        new.evolve_config = self.evolve_config.copy()
+        return new
+
+    def normalize(self, kind):
+        r''' normalize the wavefunction
+
+        Parameters
+        ----------
+        kind: str
+            "mps_only": the mps part is normalized and coeff is not modified;
+            "mps_norm_to_coeff": the mps part is normalized and the norm is multiplied to coeff;
+            "mps_and_coeff": both mps and coeff is normalized
+
+        Returns
+        -------
+        ``self`` is overwritten.
+        '''
+
+        if kind == "mps_only":
+            new_coeff = self.coeff
+        elif kind == "mps_and_coeff":
+            new_coeff = self.coeff / np.linalg.norm(self.coeff)
+        elif kind == "mps_norm_to_coeff":
+            new_coeff = self.coeff * self.mp_norm
+        else:
+            raise ValueError(f"kind={kind} is not valid.")
+        new_mps = self.scale(1.0 / self.mp_norm, inplace=True)
+        new_mps.coeff = new_coeff
+
+        return new_mps
+
+
+    def expand_bond_dimension(self, hint_mpo=None, coef=1e-10, include_ex=True):
+        """
+        expand bond dimension as required in compress_config
+        """
+        # expander m target
+        m_target = self.compress_config.bond_dim_max_value - self.bond_dims_mean
+        # will be restored at exit
+        self.compress_config.bond_dim_max_value = m_target
+        if self.compress_config.criteria is not CompressCriteria.fixed:
+            logger.warning("Setting compress criteria to fixed")
+            self.compress_config.criteria = CompressCriteria.fixed
+        logger.debug(f"target for expander: {m_target}")
+        if hint_mpo is None:
+            expander = self.__class__.random(self.model, 1, m_target)
+        else:
+            # fill states related to `hint_mpo`
+            logger.debug(
+                f"average bond dimension of hint mpo: {hint_mpo.bond_dims_mean}"
+            )
+            # in case of localized `self`
+            if include_ex:
+                if self.is_mps:
+                    ex_state: MatrixProduct = self.ground_state(self.model, False)
+                    # for self.qntot >= 1
+                    assert self.model.qn_size == 1 # otherwise not supported
+                    for i in range(self.qntot[0]):
+                        ex_state = Mpo.onsite(self.model, r"a^\dagger") @ ex_state
+                elif self.is_mpdm:
+                    assert self.qntot == 1
+                    ex_state: MatrixProduct = self.max_entangled_ex(self.model)
+                else:
+                    assert False
+                ex_state.compress_config = self.compress_config
+                ex_state.move_qnidx(self.qnidx)
+                ex_state.to_right = self.to_right
+                lastone = self + ex_state
+
+            else:
+                lastone = self
+            expander_list: List["MatrixProduct"] = []
+            cumulated_m = 0
+            while True:
+                lastone.compress_config.criteria = CompressCriteria.fixed
+                expander_list.append(lastone)
+                expander = compressed_sum(expander_list)
+                if cumulated_m == expander.bond_dims_mean:
+                    # probably a small system, the required bond dimension can't be reached
+                    break
+                cumulated_m = expander.bond_dims_mean
+                logger.debug(
+                    f"cumulated bond dimension: {cumulated_m}. lastone bond dimension: {lastone.bond_dims}"
+                )
+                if m_target < cumulated_m:
+                    break
+                if m_target < 0.8 * (lastone.bond_dims_mean * hint_mpo.bond_dims_mean):
+                    lastone = lastone.canonicalise().compress(
+                        m_target // hint_mpo.bond_dims_mean + 1
+                    )
+                lastone = (hint_mpo @ lastone).normalize("mps_and_coeff")
+        logger.debug(f"expander bond dimension: {expander.bond_dims}")
+        self.compress_config.bond_dim_max_value += self.bond_dims_mean
+        return (self + expander.scale(coef*self.norm, inplace=True)).canonicalise().canonicalise().normalize("mps_norm_to_coeff")
+
+    def evolve(self, mpo, evolve_dt, normalize=True) -> "Mps":
+
+        method = {
+            EvolveMethod.prop_and_compress: self._evolve_prop_and_compress,
+            EvolveMethod.prop_and_compress_tdrk4: self._evolve_prop_and_compress_tdrk4,
+            EvolveMethod.prop_and_compress_tdrk: self._evolve_prop_and_compress_tdrk,
+            EvolveMethod.tdvp_mu_vmf: self._evolve_tdvp_mu_vmf,
+            EvolveMethod.tdvp_vmf: self._evolve_tdvp_mu_vmf,
+            EvolveMethod.tdvp_mu_cmf: self._evolve_tdvp_mu_cmf,
+            EvolveMethod.tdvp_ps: self._evolve_tdvp_ps,
+            EvolveMethod.tdvp_ps2: self._evolve_tdvp_ps2
+        }[self.evolve_config.method]
+        new_mps = method(mpo, evolve_dt)
+        if normalize:
+            if np.iscomplex(evolve_dt):
+                new_mps.normalize("mps_and_coeff")
+            else:
+                new_mps.normalize("mps_only")
+        return new_mps
+    
+    def _evolve_prop_and_compress_tdrk4(self, mpo, evolve_dt) -> "Mps":
+        """
+        classical 4th order Runge-Kutta solver for time-dependent Hamiltonian
+        """
+        
+        if isinstance(mpo, Mpo): 
+            def mpo_t(t, *args, **kwargs):
+                return mpo
+        elif callable(mpo):
+            # mpo can be a function of time, the range is 0 -> evolve_dt
+            mpo_t = mpo
+        else:
+            raise TypeError(f"unsupported mpo type: {mpo}")
+
+        k1 = mpo_t(0).contract(self).scale(-1j)
+        logger.debug(f"k1:{k1}")  
+        tmp_mps = self + k1.scale(0.5*evolve_dt)
+        tmp_mps.canonicalise().compress()
+        k2 = mpo_t(0.5*evolve_dt).contract(tmp_mps).scale(-1j)
+        logger.debug(f"k2:{k2}")  
+        tmp_mps = self + k2.scale(0.5*evolve_dt)
+        tmp_mps.canonicalise().compress()
+        k3 = mpo_t(0.5*evolve_dt).contract(tmp_mps).scale(-1j)
+        logger.debug(f"k3:{k3}")  
+        tmp_mps = self + k3.scale(evolve_dt)
+        tmp_mps.canonicalise().compress()
+        k4 = mpo_t(evolve_dt).contract(tmp_mps).scale(-1j)
+        logger.debug(f"k4:{k4}")  
+        
+        new_mps = compressed_sum([self, k1.scale(1/6*evolve_dt),
+            k2.scale(2/6*evolve_dt), 
+            k3.scale(2/6*evolve_dt),
+            k4.scale(1/6*evolve_dt)])
+        logger.info(f"new_mps:{new_mps}")  
+        
+        return new_mps
+    
+    def _evolve_prop_and_compress_tdrk(self, mpo, evolve_dt) -> "Mps":
+        """
+            The most general Runge-Kutta solver for both time-dependent and
+            time-independnet Hamiltonian and adaptive or unadaptive time-step
+            size evolution
+        """
+        if isinstance(mpo, Mpo): 
+            def mpo_t(t, *args, **kwargs):
+                return mpo
+        elif callable(mpo):
+            mpo_t = mpo
+        else:
+            raise TypeError(f"unsupported mpo type: {mpo}")
+        
+        rk_config = self.evolve_config.rk_config
+        a,b,c = rk_config.tableau
+        
+        def sub_time_step_evolve(y,tau,t0):
+            # error is relative error
+            k_list = []
+            for istage in range(rk_config.stage):
+                k = compressed_sum([y]+[k_list[i].scale(a[istage,i]*tau) for
+                    i in range(istage) if a[istage,i] != 0], batchsize=6)
+                k = mpo_t(c[istage]*tau+t0, mps=k).contract(k).scale(-1j)
+                logger.debug(f"k_{istage}: {k}") 
+                k_list.append(k)        
+            
+            new_mps = compressed_sum([y] +
+                    [k_list[istage].scale(b[0,istage]*tau) \
+                    for istage in range(rk_config.stage) if b[0,istage]!=0],
+                    batchsize=6)   
+            logger.debug(f"order_{rk_config.order[0]}: {new_mps}") 
+            
+            if self.evolve_config.adaptive:
+                assert len(rk_config.order) == 2
+                assert rk_config.order[0] - rk_config.order[1] == 1
+                error = reduce(lambda mps1, mps2: mps1.add(mps2),
+                    [k_list[istage].scale((b[0,istage]-b[1,istage])*tau) \
+                    for istage in range(rk_config.stage) if not \
+                    np.allclose(b[0,istage],b[1,istage])])
+
+                error = error.norm / new_mps.norm
+            else:
+                assert len(rk_config.order) == 1
+                error = 0
+                
+            return new_mps, error
+        
+        self.evolve_config.check_valid_dt(evolve_dt)
+        
+        if self.evolve_config.adaptive:
+            p_restart = 0.5  # restart threshold
+            p_min = 0.1  # safeguard for minimal allowed p
+            p_max = 2.0  # safeguard for maximal allowed p
+            
+            evolved_dt = 0
+            new_mps = self
+
+            while True:
+                dt = min_abs(new_mps.evolve_config.guess_dt, evolve_dt-evolved_dt)
+                logger.debug(f"guess_dt: {new_mps.evolve_config.guess_dt}, try time step size: {dt}")
+                new_mps, error = sub_time_step_evolve(new_mps, dt, evolved_dt)    
+                p = (new_mps.evolve_config.adaptive_rtol / (error + 1e-30)) ** (1/rk_config.order[0])
+                logger.debug(f"RKsolver:{rk_config.method} relative error: {error}, enlarge p parameter: {p}")
+                
+                if p < p_restart:
+                    # not accurate, will restart
+                    new_mps.evolve_config.guess_dt = dt * max(p_min, p)
+                    logger.debug(
+                        f"evolution not converged, new guess_dt: {new_mps.evolve_config.guess_dt}"
+                    )
+                else:
+                    if xp.allclose(dt+evolved_dt, evolve_dt):
+                        new_mps.evolve_config.guess_dt = min_abs(
+                            dt * p, new_mps.evolve_config.guess_dt
+                        )
+                        # normal exit
+                        logger.debug(
+                            f"evolution converged, new guess_dt: {new_mps.evolve_config.guess_dt}"
+                        )
+                        break
+                    else:
+                        new_mps.evolve_config.guess_dt *= min(p, p_max)
+                        evolved_dt += dt
+                        logger.debug(
+                            f"evolution converged, new guess_dt: {new_mps.evolve_config.guess_dt}"
+                        )
+                        logger.debug(f"sub-step {dt} further, remaining: {evolve_dt-evolved_dt}")
+        else:
+            new_mps, _ = sub_time_step_evolve(self, evolve_dt, 0)
+
+        return new_mps
+
+    def _evolve_prop_and_compress(self, mpo, evolve_dt) -> "Mps":
+        """
+        The global propagation & compression evolution scheme
+        only for time-independent Hamiltonian
+        Taylor expansion approximation to the formal propagator
+        """
+        config = self.evolve_config
+        assert evolve_dt is not None
+
+        propagation_c = config.taylor_config.coeff
+        order = len(propagation_c)-1
+        termlist = [self]
+        # don't let bond dim grow when contracting
+        orig_compress_config = self.compress_config
+        contract_compress_config = self.compress_config.copy()
+        if contract_compress_config.criteria is CompressCriteria.threshold:
+            contract_compress_config.criteria = CompressCriteria.both
+        # contract_compress_config.min_dims = None
+        # contract_compress_config.max_dims = np.array(self.bond_dims) + 4
+        self.compress_config = contract_compress_config
+
+        while len(termlist) < len(propagation_c):
+            termlist.append(mpo.contract(termlist[-1]))
+        # bond dim can grow after adding
+        for t in termlist:
+            t.compress_config = orig_compress_config
+
+        if config.adaptive:
+            config.check_valid_dt(evolve_dt)
+
+            p_restart = 0.5  # restart threshold
+            p_min = 0.1  # safeguard for minimal allowed p
+            p_max = 2.0  # safeguard for maximal allowed p
+
+            while True:
+                scaled_termlist = []
+                dt = min_abs(config.guess_dt, evolve_dt)
+                logger.debug(f"guess_dt: {config.guess_dt}, try time step size: {dt}")
+                for idx, term in enumerate(termlist):
+                    scale = (-1.0j * dt) ** idx * propagation_c[idx]
+                    scaled_termlist.append(term.scale(scale))
+                    del term
+                
+                new_mps1 = compressed_sum(scaled_termlist[:-1])
+                new_mps2 = compressed_sum(
+                    [new_mps1, scaled_termlist[-1]]
+                )
+                dis = new_mps1.distance(new_mps2)
+                p = (config.adaptive_rtol / (dis/new_mps2.mp_norm + 1e-30)) ** (1/order)
+                logger.debug(f"RK45 error distance: {dis}, enlarge p parameter: {p}")
+
+                if xp.allclose(dt, evolve_dt):
+                    # approahes the end
+                    if p < p_restart:
+                        # not accurate in this final sub-step will restart
+                        config.guess_dt = dt * max(p_min, p)
+                        logger.debug(
+                            f"evolution not converged, new guess_dt: {config.guess_dt}"
+                        )
+                    else:
+                        # normal exit
+                        new_mps2.evolve_config.guess_dt = min_abs(
+                            dt * p, config.guess_dt
+                        )
+                        logger.debug(
+                            f"evolution converged, new guess_dt: {new_mps2.evolve_config.guess_dt}"
+                        )
+                        return new_mps2
+                else:
+                    # sub-steps
+                    if p < p_restart:
+                        config.guess_dt *= max(p_min, p)
+                        logger.debug(
+                            f"evolution not converged, new guess_dt: {config.guess_dt}"
+                        )
+                    else:
+                        new_dt = evolve_dt - dt
+                        config.guess_dt *= min(p, p_max)
+                        new_mps2.evolve_config.guess_dt = config.guess_dt
+                        # memory consuming and not useful anymore
+                        del new_mps1, termlist, scaled_termlist
+                        logger.debug(
+                            f"evolution converged, new guess_dt: {config.guess_dt}"
+                        )
+                        logger.debug(f"sub-step {dt} further, remaining: {new_dt}")
+                        return new_mps2._evolve_prop_and_compress(mpo, new_dt)
+        else:
+            for idx, term in enumerate(termlist):
+                term.scale(
+                    (-1.0j * evolve_dt) ** idx * propagation_c[idx], inplace=True
+                )
+            return compressed_sum(termlist)
+    
+    def _evolve_tdvp_mu_vmf(self, mpo, evolve_dt) -> "Mps":
+        """
+        variable mean field
+        see the difference between VMF and CMF, refer to Z. Phys. D 42, 113–129 (1997)
+        the matrix unfolding algorithm, see arXiv:1907.12044
+        only the RKF45 integration is used.
+        The default RKF45 local step error tolerance is rtol:1e-5, atol:1e-8
+        regulation of S is 1e-10, these default parameters could be changed in
+        /utils/configs.py
+
+        """
+        
+        if isinstance(mpo, Mpo): 
+            def mpo_t(t, *args, **kwargs):
+                return mpo
+        elif callable(mpo):
+            mpo_t = mpo
+        else:
+            raise TypeError(f"unsupported mpo type: {mpo}")
+        
+        # a workaround for https://github.com/scipy/scipy/issues/10164
+        imag_time = np.iscomplex(evolve_dt)
+        if imag_time:
+            evolve_dt = -evolve_dt.imag
+            # used in calculating derivatives
+            coef = -1
+        else:
+            coef = 1j
+        
+        # only not canonicalise when force_ovlp=True and to_right=False
+        if not (self.evolve_config.force_ovlp and not self.to_right):
+            self.ensure_left_canonical()
+
+        # `self` should not be modified during the evolution
+        if imag_time:
+            mps = self.copy()
+        else:
+            mps = self.to_complex()
+
+        # the quantum number symmetry is used
+        qn_mask_list = []
+        position = [0]
+        qntot = mps.qntot
+        for imps in range(mps.site_num):
+            mps.move_qnidx(imps)
+            qnbigl, qnbigr, qnmat = mps._get_big_qn([imps])
+            qn_mask = get_qn_mask(qnmat, mps.qntot)
+            qn_mask_list.append(qn_mask)
+            position.append(position[-1]+np.sum(qn_mask))
+
+        sw_min_list = []
+        
+        def func_vmf(t,y):
+            
+            sw_min_list.clear()
+
+            # update mps: from left to right
+            for imps in range(mps.site_num):
+                mps[imps] = cvec2cmat(asnumpy(y[position[imps]:position[imps + 1]]), qn_mask_list[imps])
+            mpo = mpo_t(t, mps=mps)
+
+            if self.evolve_config.method == EvolveMethod.tdvp_mu_vmf:
+                environ_mps = mps.copy()
+            elif self.evolve_config.method == EvolveMethod.tdvp_vmf:
+                environ_mps = mps
+                # the first S_R
+                S_R = np.ones([1, 1], dtype=mps.dtype)
+            else:
+                assert False
+
+            environ = Environ(environ_mps, mpo, "L")
+
+            if self.evolve_config.force_ovlp:
+                # construct the S_L list (type: Matrix) and S_L_inv list (type: xp.array)
+                # len: mps.site_num+1
+                S_L_list = [
+                    np.ones([1, 1], dtype=mps.dtype),
+                ]
+                for imps in range(mps.site_num):
+                    S_L_list.append(
+                        transferMat(mps, None, "L", imps, S_L_list[imps])
+                    )
+
+
+                S_L_inv_list = []
+                for imps in range(mps.site_num + 1):
+                    w, u = scipy.linalg.eigh(S_L_list[imps])
+                    S_L_inv = u.dot(np.diag(1.0 / w)).dot(u.T.conj())
+                    S_L_inv_list.append(S_L_inv)
+            else:
+                S_L_list = [None,] * (mps.site_num + 1)
+                S_L_inv_list = [None,] * (mps.site_num + 1)
+
+            # calculate hop_y: from right to left
+            hop_y = xp.empty_like(y)
+
+            for imps in mps.iter_idx_list(full=True):
+                shape = list(mps[imps].shape)
+                ltensor = asxp(environ.read("L", imps - 1))
+
+                if imps == self.site_num - 1:
+                    # the coefficient site
+                    rtensor = xp.ones((1, 1, 1), dtype=mps.dtype)
+                    hop =hop_expr(ltensor, rtensor, [asxp(mpo[imps])], shape)
+
+                    S_inv = xp.diag(xp.ones(1,dtype=mps.dtype))
+                    func = integrand_func_factory(shape, hop, True, S_inv, True,
+                            coef, ovlp_inv1=S_L_inv_list[imps+1],
+                            ovlp_inv0=S_L_inv_list[imps], ovlp0=S_L_list[imps])
+
+                    hop_y[position[imps]:position[imps+1]] = func(0,
+                            mps[imps].array.ravel()).reshape(mps[imps].shape)[qn_mask_list[imps]]
+
+                    continue
+
+                if self.evolve_config.method == EvolveMethod.tdvp_mu_vmf:
+                    # perform qr on the environment mps
+                    qnbigl, qnbigr, _ = environ_mps._get_big_qn([imps + 1])
+                    u, s, qnlset, v, s, qnrset = svd_qn.svd_qn(
+                            environ_mps[imps + 1].array, qnbigl, qnbigr,
+                            environ_mps.qntot, system="R", full_matrices=False)
+                    vt = v.T
+
+                    environ_mps[imps + 1] = vt.reshape(environ_mps[imps + 1].shape)
+
+                    rtensor = environ.GetLR(
+                        "R", imps + 1, environ_mps, mpo, itensor=None, method="System"
+                    )
+
+                    sw_min_list.append(s.min())
+                    regular_s = _mu_regularize(s, epsilon=self.evolve_config.reg_epsilon)
+
+                    u = asxp(u)
+                    us = u.dot(xp.diag(s))
+
+                    rtensor = xp.tensordot(rtensor, us, axes=(-1, -1))
+
+                    environ_mps[imps] = xp.tensordot(asxp(environ_mps[imps]), us, axes=(-1, 0))
+                    environ_mps.qn[imps + 1] = qnrset
+                    environ_mps.qnidx = imps
+
+                    S_inv = u.conj().dot(xp.diag(1.0 / regular_s)).T
+
+                elif self.evolve_config.method == EvolveMethod.tdvp_vmf:
+                    rtensor = environ.GetLR(
+                        "R", imps + 1, environ_mps, mpo, itensor=None, method="System")
+
+                    # regularize density matrix
+                    # Note that S_R is (#.conj, #)
+                    S_R = transferMat(environ_mps, None, "R", imps + 1, S_R)
+                    w, u = scipy.linalg.eigh(asnumpy(S_R))
+                    # discard the negative eigenvalues due to numerical error
+                    w = np.where(w>0, w, 0)
+
+                    sw_min_list.append(w.min())
+
+                    epsilon = self.evolve_config.reg_epsilon
+                    w = w + epsilon * np.exp(-w / epsilon)
+
+                    u = asxp(u)
+                    # S_inv is (#.conj, #)
+                    S_inv = u.dot(xp.diag(1.0 / w)).dot(u.T.conj()).T
+
+                hop = hop_expr(ltensor, rtensor, [asxp(mpo[imps])], shape)
+
+                func = integrand_func_factory(shape, hop, False, S_inv, True,
+                        coef, ovlp_inv1=S_L_inv_list[imps+1],
+                        ovlp_inv0=S_L_inv_list[imps], ovlp0=S_L_list[imps])
+
+                hop_y[position[imps]:position[imps+1]] = func(0,
+                        asxp(mps[imps].array.ravel())).reshape(mps[imps].shape)[qn_mask_list[imps]]
+
+            return hop_y
+
+        init_y = xp.concatenate([asxp(ms.array[qn_mask_list[ims]]) for ims, ms in enumerate(mps)])
+        # the ivp local error, please refer to the Scipy default setting
+        sol = solve_ivp(
+            func_vmf,
+            (0, evolve_dt),
+            init_y,
+            method="RK45",
+            rtol=self.evolve_config.ivp_rtol,
+            atol=self.evolve_config.ivp_atol,
+        )
+
+        # update mps: from left to right
+        for imps in range(mps.site_num):
+            mps[imps] = cvec2cmat(asnumpy(sol.y[:, -1][position[imps]:position[imps + 1]]), qn_mask_list[imps])
+
+        logger.info(f"{self.evolve_config.method} VMF func called: {sol.nfev}. RKF steps: {len(sol.t)}")
+
+        sw_min_list = xp.array(sw_min_list)
+        # auto-switch between tdvp_mu_vmf and tdvp_vmf
+        if self.evolve_config.vmf_auto_switch:
+            if sw_min_list.min() > np.sqrt(self.evolve_config.reg_epsilon*10.) and \
+                mps.evolve_config.method == EvolveMethod.tdvp_mu_vmf:
+
+                logger.debug(f"sw.min={sw_min_list.min()}, Switch to tdvp_vmf")
+                mps.evolve_config.method =  EvolveMethod.tdvp_vmf
+
+            elif sw_min_list.min() < self.evolve_config.reg_epsilon and \
+                mps.evolve_config.method == EvolveMethod.tdvp_vmf:
+
+                logger.debug(f"sw.min={sw_min_list.min()}, Switch to tdvp_mu_vmf")
+                mps.evolve_config.method =  EvolveMethod.tdvp_mu_vmf
+
+        # The caller do not want to deal with an MPS that is not canonicalised
+        return mps.canonicalise()
+
+    @adaptive_tdvp
+    def _evolve_tdvp_mu_cmf(self, mpo, evolve_dt) -> "Mps":
+        """
+        evolution scheme: TDVP + constant mean field + matrix-unfolding
+        regularization
+        MPS :  LLLLLLC
+        1st / 2nd order(default) CMF
+
+        for 2nd order CMF:
+        L is evolved with midpoint scheme
+        C is evolved with midpoint(default) / trapz scheme
+        """
+
+        if self.evolve_config.tdvp_cmf_c_trapz:
+            assert self.evolve_config.tdvp_cmf_midpoint
+
+        imag_time = np.iscomplex(evolve_dt)
+
+        # a workaround for https://github.com/scipy/scipy/issues/10164
+        if imag_time:
+            evolve_dt = -evolve_dt.imag
+            # used in calculating derivatives
+            coef = -1
+        else:
+            coef = 1j
+
+        self.ensure_left_canonical()
+
+        # `self` should not be modified during the evolution
+        # mps: the mps to return
+        # environ_mps: mps to construct environ
+        if imag_time:
+            mps = self.copy()
+        else:
+            mps = self.to_complex()
+
+        if self.evolve_config.tdvp_cmf_midpoint:
+            # mps at t/2 (1st order) as environment
+            orig_config = self.evolve_config.copy()
+            self.evolve_config.tdvp_cmf_midpoint = False
+            self.evolve_config.tdvp_cmf_c_trapz = False
+            self.evolve_config.adaptive = False
+            environ_mps = self.evolve(mpo, evolve_dt / 2)
+            self.evolve_config = orig_config
+        else:
+            # mps at t=0 as environment
+            environ_mps = mps.copy()
+
+        if self.evolve_config.tdvp_cmf_c_trapz:
+            loop = 2
+            mps[-1] = environ_mps[-1].copy()
+        else:
+            loop = 1
+
+        while loop > 0:
+
+            # construct the environment matrix
+            environ = Environ(environ_mps, mpo, "L")
+
+            # statistics for debug output
+            cmf_rk_steps = []
+
+            if self.evolve_config.force_ovlp:
+                # construct the S_L list (type: Matrix) and S_L_inv list (type: xp.array)
+                # len: mps.site_num+1
+                S_L_list = [np.ones([1, 1], dtype=mps.dtype),]
+                for imps in range(mps.site_num):
+                    S_L_list.append(transferMat(environ_mps, None, "L", imps,
+                        S_L_list[imps]))
+
+                S_L_inv_list = []
+                for imps in range(mps.site_num+1):
+                    w, u = scipy.linalg.eigh(S_L_list[imps])
+                    S_L_inv = xp.asarray(u.dot(np.diag(1.0 / w)).dot(u.T.conj()))
+                    S_L_inv_list.append(S_L_inv)
+                    S_L_list[imps] = S_L_list[imps]
+            else:
+                S_L_list = [None,] * (mps.site_num+1)
+                S_L_inv_list = [None,] * (mps.site_num+1)
+
+            for imps in mps.iter_idx_list(full=True):
+                shape = list(mps[imps].shape)
+                ltensor = environ.read("L", imps - 1)
+                if imps == self.site_num - 1:
+                    if loop == 1:
+                        # the coefficient site
+                        rtensor = ones((1, 1, 1))
+                        hop = hop_expr(ltensor, rtensor, [mpo[imps]], shape)
+
+                        S_inv = xp.diag(xp.ones(1,dtype=mps.dtype))
+                        def func1(y):
+                            func = integrand_func_factory(shape, hop, True, S_inv, True,
+                                    coef, ovlp_inv1=S_L_inv_list[imps+1],
+                                    ovlp_inv0=S_L_inv_list[imps], ovlp0=S_L_list[imps])
+                            return func(0, y)
+
+                        ms, Lanczos_vectors = expm_krylov(func1, evolve_dt, mps[imps].ravel().array)
+                        logger.debug(f"# of Lanczos_vectors, {Lanczos_vectors}")
+                        mps[imps] = ms.reshape(shape)
+
+                    if loop == 1 and self.evolve_config.tdvp_cmf_c_trapz:
+                        break
+                    else:
+                        continue
+
+                # perform qr on the environment mps
+                qnbigl, qnbigr, _ = environ_mps._get_big_qn([imps + 1])
+                u, s, qnlset, v, s, qnrset = svd_qn.svd_qn(
+                    environ_mps[imps + 1].array,
+                    qnbigl,
+                    qnbigr,
+                    environ_mps.qntot,
+                    system="R",
+                    full_matrices=False,
+                )
+                vt = v.T
+
+                environ_mps[imps + 1] = vt.reshape(environ_mps[imps + 1].shape)
+
+                rtensor = environ.GetLR(
+                    "R", imps + 1, environ_mps, mpo, itensor=None, method="System"
+                )
+
+                regular_s = _mu_regularize(s, epsilon=self.evolve_config.reg_epsilon)
+
+                us = u.dot(np.diag(s))
+
+                rtensor = tensordot(rtensor, us, axes=(-1, -1))
+
+                environ_mps[imps] = tensordot(environ_mps[imps], us, axes=(-1, 0))
+                environ_mps.qn[imps + 1] = qnrset
+                environ_mps.qnidx = imps
+
+                S_inv = u.conj().dot(np.diag(1.0 / regular_s)).T
+
+                hop = hop_expr(ltensor, rtensor, [mpo[imps]], shape)
+                func = integrand_func_factory(shape, hop, False, S_inv, True,
+                        coef, ovlp_inv1=S_L_inv_list[imps+1],
+                        ovlp_inv0=S_L_inv_list[imps], ovlp0=S_L_list[imps])
+
+                sol = solve_ivp(
+                    func, (0, evolve_dt), mps[imps].ravel().array, method="RK45"
+                )
+                cmf_rk_steps.append(len(sol.t))
+                ms = sol.y[:, -1].reshape(shape)
+                mps[imps] = ms
+
+            if len(cmf_rk_steps) > 0:
+                steps_stat = stats.describe(cmf_rk_steps)
+                logger.debug(f"{self.evolve_config.method} CMF steps: {steps_stat}")
+
+            if loop == 2:
+                environ_mps = mps
+                evolve_dt /= 2.
+            loop -= 1
+            # new_mps.evolve_config.stat = steps_stat
+
+        return mps
+
+    @adaptive_tdvp
+    def _evolve_tdvp_ps(self, mpo, evolve_dt) -> "Mps":
+        # PhysRevB.94.165116
+        # TDVP projector splitting
+        # one-site
+        if np.iscomplex(evolve_dt):
+            mps = self.copy()
+        else:
+            mps = self.to_complex()
+
+        # construct the environment matrix
+        # almost half is not used. Not a big deal.
+        environ = Environ(mps, mpo)
+
+        # statistics for debug output
+        local_steps = []
+        # sweep for 2 rounds
+        for i in range(2):
+            for imps in mps.iter_idx_list(full=True):
+                system = "L" if mps.to_right else "R"
+                l_array = environ.read("L", imps - 1)
+                r_array = environ.read("R", imps + 1)
+
+                shape = list(mps[imps].shape)
+                hop = hop_expr(l_array, r_array, [asxp(mpo[imps].array)], shape)
+                mps_t, j = expm_krylov(
+                    lambda y: hop(y.reshape(shape)).ravel(),
+                    -1j * evolve_dt / 2, mps[imps].ravel().array
+                )
+                local_steps.append(j)
+                mps_t = mps_t.reshape(shape)
+
+                qnbigl, qnbigr, _ = mps._get_big_qn([imps])
+                u, qnlset, v, qnrset = svd_qn.svd_qn(
+                    asnumpy(mps_t),
+                    qnbigl,
+                    qnbigr,
+                    mps.qntot,
+                    QR=True,
+                    system=system,
+                    full_matrices=False,
+                )
+                vt = v.T
+
+                if not mps.to_right and imps != 0:
+                    mps[imps] = vt.reshape([-1] + shape[1:])
+                    mps.qn[imps] = qnrset
+                    mps.qnidx = imps-1
+
+                    r_array = environ.GetLR(
+                        "R", imps, mps, mpo, itensor=r_array, method="System"
+                    )
+
+                    # reverse update u site
+                    shape_u = u.shape
+                    hop_u = hop_expr(l_array, r_array, [], shape_u)
+                    mps_t, j = expm_krylov(
+                        lambda y: hop_u(y.reshape(shape_u)).ravel(),
+                        1j * evolve_dt / 2, u.ravel()
+                    )
+                    local_steps.append(j)
+                    mps_t = mps_t.reshape(shape_u)
+
+                    mps[imps - 1] = tensordot(mps[imps - 1].array, mps_t, axes=(-1, 0),)
+
+                elif mps.to_right and imps != len(mps) - 1:
+                    mps[imps] = u.reshape(shape[:-1] + [-1])
+                    mps.qn[imps + 1] = qnlset
+                    mps.qnidx = imps+1
+
+                    l_array = environ.GetLR(
+                        "L", imps, mps, mpo, itensor=l_array, method="System"
+                    )
+
+                    # reverse update svt site
+                    shape_svt = vt.shape
+                    hop_svt = hop_expr(l_array, r_array, [], shape_svt)
+                    mps_t, j = expm_krylov(
+                        lambda y: hop_svt(y.reshape(shape_svt)).ravel(),
+                        1j * evolve_dt / 2, vt.ravel()
+                    )
+                    local_steps.append(j)
+                    mps_t = mps_t.reshape(shape_svt)
+
+                    mps[imps + 1] = tensordot(mps_t, mps[imps + 1].array, axes=(1, 0),)
+
+                else:
+                    mps[imps] = mps_t
+            mps._switch_direction()
+
+        steps_stat = stats.describe(local_steps)
+        logger.debug(f"TDVP-PS Krylov space: {steps_stat}")
+        mps.evolve_config.stat = steps_stat
+
+        return mps
+
+    @adaptive_tdvp
+    def _evolve_tdvp_ps2(self, mpo, evolve_dt) -> "Mps":
+        # PhysRevB.94.165116
+        # TDVP projector splitting
+        # two-site
+        if np.iscomplex(evolve_dt):
+            mps = self.copy()
+        else:
+            mps = self.to_complex()
+
+        M = self.compress_config.bond_dim_max_value
+
+        # construct the environment matrix
+        # almost half is not used. Not a big deal.
+        environ = Environ(mps, mpo)
+
+        # statistics for debug output
+        local_steps = []
+        # sweep for 2 rounds
+        for i in range(2):
+            for imps in mps.iter_idx_list(full=False):
+                if mps.to_right:
+                    lidx, cidx0, cidx1, ridx = range(imps - 1, imps + 3)
+                    # the idx of the next site
+                    cidx2 = cidx1
+                    # the idx of the last site
+                    last_idx = len(mps) - 2
+                else:
+                    lidx, cidx0, cidx1, ridx = range(imps - 2, imps + 2)
+                    cidx2 = cidx0
+                    last_idx = 1
+
+                l_array = environ.read("L", lidx)
+                r_array = environ.read("R", ridx)
+
+                # the two-site matrix state
+                ms2 = tensordot(mps[cidx0], mps[cidx1], axes=1)
+                hop = hop_expr(l_array, r_array, [mpo[cidx0], mpo[cidx1]], ms2.shape)
+                mps_t, j = expm_krylov(
+                    lambda y: hop(y.reshape(ms2.shape)).ravel(),
+                    -1j * evolve_dt / 2,
+                    ms2.ravel()
+                )
+                local_steps.append(j)
+
+                mps_t = mps_t.reshape(ms2.shape)
+                qnbigl, qnbigr, _ = mps._get_big_qn([cidx0, cidx1])
+                mps._update_mps(mps_t, [cidx0, cidx1], qnbigl, qnbigr, M)
+                if mps.compress_config.ofs is not None:
+                    mpo.try_swap_site(mps.model, mps.compress_config.ofs_swap_jw)
+                if imps == last_idx:
+                    continue
+
+                if mps.to_right:
+                    l_array = environ.GetLR(
+                        "L", lidx + 1, mps, mpo, itensor=l_array, method="System"
+                    )
+                else:
+                    r_array = environ.GetLR(
+                        "R", ridx - 1, mps, mpo, itensor=r_array, method="System"
+                    )
+
+                # reverse update the next site
+                ms1 = mps[cidx2]
+                hop = hop_expr(l_array, r_array, [mpo[cidx2]], ms1.shape)
+                mps_t, j = expm_krylov(
+                    lambda y: hop(y.reshape(ms1.shape)).ravel(),
+                    1j * evolve_dt / 2, ms1.ravel()
+                )
+                local_steps.append(j)
+                mps_t = mps_t.reshape(ms1.shape)
+                mps[cidx2] = mps_t
+                mps._push_cano(cidx2)
+
+            mps._switch_direction()
+
+        steps_stat = stats.describe(local_steps)
+        logger.debug(f"TDVP-PS Krylov space: {steps_stat}")
+        mps.evolve_config.stat = steps_stat
+
+        return mps
+
+    def evolve_exact(self, h_mpo, evolve_dt, space):
+        MPOprop = Mpo.exact_propagator(self.model, -1j * evolve_dt, space, -h_mpo.offset)
+        new_mps = MPOprop.apply(self, canonicalise=True)
+        self.coeff *= np.exp(-1j * h_mpo.offset * evolve_dt)
+        return new_mps
+
+    @property
+    def digest(self):
+        # used for debugging. Mostly for quickly comparing how two MPSs differ.
+        if 10 < self.site_num or self.is_mpdm:
+            return None
+        prod = np.eye(1).reshape(1, 1, 1)
+        for ms in self:
+            prod = np.tensordot(prod, ms, axes=1)
+            prod = prod.reshape((prod.shape[0], -1, prod.shape[-1]))
+        return {"var": prod.var(), "mean": prod.mean(), "ptp": prod.ptp()}
+
+    def todense(self) -> np.array:
+        dim = np.prod(self.pbond_list)
+        if 20000 < dim:
+            raise ValueError("wavefunction too large")
+        res = np.ones((1, 1, 1))
+        for mt in self:
+            dim1 = res.shape[1] * mt.shape[1]
+            dim2 = mt.shape[-1]
+            res = np.tensordot(res, mt.array, axes=1).reshape(1, dim1, dim2)
+        return res[0, :, 0]
+    
+    def calc_1site_rdm(self, idx=None):
+        r""" Calculate 1-site reduced density matrix
+        
+            :math:`\rho_i = \textrm{Tr}_{j \neq i} | \Psi \rangle \langle \Psi|`
+        
+        Parameters
+        ----------
+        idx : int, list, tuple, optional
+            site index of 1site_rdm. Default is None, which mean all the rdms
+            are calculated.
+        
+        Returns
+        -------
+        rdm: Dict
+            :math:`\{0:\rho_0, 1:\rho_1, \cdots\}`. The key is the index of the site.
+        """
+
+        identity = Mpo.identity(self.model)
+        environ = Environ(self, identity, "R")
+        if idx is None:
+            idx = list(range(self.site_num))
+        elif type(idx) is int:
+            idx = [idx]
+        elif (type(idx) is list) or (type(idx) is tuple):  
+            idx = list(idx)
+        else:
+            assert False
+
+        rdm = {}
+        for ims, ms in enumerate(self):
+            ltensor = environ.GetLR(
+                "L", ims-1, self, identity, itensor=None, method="System"
+            )
+            rtensor = environ.GetLR(
+                "R", ims+1, self, identity, itensor=None, method="Enviro"
+            )
+            if ims not in idx:
+                continue
+
+            ltensor = ltensor.reshape(ltensor.shape[0], ltensor.shape[-1])
+            rtensor = rtensor.reshape(rtensor.shape[0], rtensor.shape[-1])
+            
+            tensor = tensordot(ltensor, ms.conj(), ([0],[0]))
+            tensor = tensordot(tensor, rtensor, ([-1],[0]))
+            if ms.ndim == 3:
+                tensor = tensordot(tensor, ms, ([0,-1],[0,-1]))
+            else:
+                tensor = tensordot(tensor, ms, ([0,-1,-2],[0,-1,-2]))
+            assert xp.allclose(tensor, tensor.T.conj())
+            rdm[ims] = asnumpy(tensor)
+
+        return rdm
+    
+    def calc_2site_rdm(self):
+        r""" Calculate 2-site reduced density matrix
+        
+        :math:`\rho_{ij} = \textrm{Tr}_{k \neq i, k \neq j} | \Psi \rangle \langle \Psi |`.
+        
+        Returns
+        -------
+        rdm: Dict
+            :math:`\{(0,1):\rho_{01}, (0,2):\rho_{02}, \cdots\}`. The key is a tuple of index of the site.
+        """
+        
+        identity = Mpo.identity(self.model)
+        environ_R = Environ(self, identity, "R")
+        environ_L = Environ(self, identity, "L")
+        L_component = []
+        R_component = []
+        rdm = {}
+        # first construct 1-site environment
+        for ims, ms in enumerate(self):
+            ltensor = environ_L.GetLR("L", ims-1, self, identity,
+                    itensor=None, method="Enviro")
+            ltensor = ltensor.reshape(ltensor.shape[0], ltensor.shape[-1])
+            tensor = tensordot(ltensor, ms.conj(), ([0],[0]))
+            if ms.ndim == 3:
+                tensor = tensordot(tensor, ms, ([0],[0]))
+            elif ms.ndim == 4:
+                tensor = tensordot(tensor, ms, ([0,2],[0,2]))
+            L_component.append(tensor.transpose((0,2,1,3)))
+            
+            rtensor = environ_R.GetLR("R", ims+1, self, identity,
+                    itensor=None, method="Enviro")
+            rtensor = rtensor.reshape(rtensor.shape[0], rtensor.shape[-1])
+            tensor = tensordot(ms.conj(), rtensor, ([-1],[0]))
+            if ms.ndim == 3:
+                tensor = tensordot(tensor, ms, ([-1],[-1]))
+            elif ms.ndim == 4:
+                tensor = tensordot(tensor, ms, ([2,-1],[2,-1]))
+            R_component.append(tensor.transpose((0,2,1,3)))
+        
+        # merge two 1-site environment together
+        for ims in range(self.site_num):
+            tensor = L_component[ims]
+            for jms in range(ims+1, self.site_num):
+                if jms != ims+1:
+                    kms = jms - 1
+                    tensor = tensordot(tensor, self[kms].conj(), ([2],[0]))
+                    if self[kms].ndim == 3:
+                        tensor = tensordot(tensor, self[kms], ([2,3],[0,1]))
+                    elif self[kms].ndim == 4:
+                        tensor = tensordot(tensor, self[kms], ([2,3,4],[0,1,2]))
+                
+                rtensor = R_component[jms]
+                res = tensordot(tensor, rtensor,
+                        ([2,3],[0,1])).transpose(0,2,1,3)
+                rdm[(ims, jms)] = asnumpy(res.reshape(res.shape[0]*res.shape[1],-1))
+        return rdm
+    
+    def calc_edof_rdm(self) -> np.ndarray:
+        r"""Calculate the reduced density matrix of electronic DoF
+        
+        :math:`\rho_{ij} = \langle \Psi | a_i^\dagger a_j | \Psi \rangle`
+        
+        """
+        
+        key = "edof_reduced_density_matrix"
+        n_e = self.model.n_edofs
+        e_dofs = self.model.e_dofs
+        if key not in self.model.mpos:
+            mpos = []
+            for idx, dof1 in enumerate(e_dofs):
+                for dof2 in e_dofs[idx:]:
+                    op = Op(r"a^\dagger a", [dof1, dof2])
+                    mpo = Mpo(self.model, terms=op)
+                    mpos.append(mpo)
+            self.model.mpos[key] = mpos
+        else:
+            mpos = self.model.mpos[key]
+        expectations = deque(self.expectations(mpos))
+        reduced_density_matrix = np.zeros((n_e, n_e), dtype=backend.complex_dtype)
+        for idx in range(n_e):
+            for jdx in range(idx, n_e):
+                reduced_density_matrix[idx, jdx] = expectations.popleft()
+                reduced_density_matrix[jdx, idx] = np.conj(reduced_density_matrix[idx, jdx])
+
+        return reduced_density_matrix
+    
+    def calc_entropy(self, entropy_type):
+        r""" Calculate 1site, 2site, mutual and bond Von Neumann entropy
+
+            :math:`\textrm{entropy} = -\textrm{Tr}(\rho \ln \rho)`
+            where :math:`\ln` stands for natural logarithm.
+            
+            1site entropy is the entropy between any site and the other
+            ``(N-1)`` sites.
+            2site entropy is the entropy between any two sites and the other 
+            ``(N-2)`` sites.
+            mutual entropy characterize the entropy between any two sites.
+            bond entropy is the entropy between L-block and R-block.
+
+        Parameters
+        ----------
+        entropy_type : str
+            "1site", "2site", "mutual", "bond"
+        
+        Returns
+        -------
+        entropy : dict, ndarray
+            if entropy_type = "1site" or "2site", a dictionary is returned and the
+            key is the index or the tuple of index of mps sites, else
+            an ndarray is returned.
+        
+        """
+
+        if entropy_type in ["1site", "2site"]:
+            if entropy_type == "1site":
+                rdm = self.calc_1site_rdm()
+            else:
+                rdm = self.calc_2site_rdm()
+            
+            entropy = {}
+            for key, dm in rdm.items():
+                w, v = scipy.linalg.eigh(dm)
+                entropy[key] = calc_vn_entropy(w)
+
+        elif entropy_type == "mutual":
+            entropy = self.calc_2site_mutual_entropy()
+        elif entropy_type == "bond":
+            entropy = self.calc_bond_entropy()
+        else:
+            raise ValueError(f"unsupported entropy type {entropy_type}")
+        return entropy
+    
+    def calc_2site_mutual_entropy(self):
+        r""" 
+        Calculate mutual entropy between two sites.
+        
+        :math:`m_{ij} = (s_i + s_j - s_{ij})/2`
+            
+        See Chemical Physics 323 (2006) 519–531
+        
+        Returns
+        -------
+        mutual_entropy : 2d np.ndarry
+            mutual entropy with shape (nsite, nsite)
+
+        """
+        entropy_1site = self.calc_entropy("1site")
+        entropy_2site = self.calc_entropy("2site")
+        nsites = self.site_num
+        mut_entropy = np.zeros((nsites, nsites))
+        for isite, jsite in itertools.combinations(range(nsites),2):
+            key = (isite, jsite) if (isite, jsite) in entropy_2site.keys() else (jsite, isite)
+            mut_entropy[isite, jsite] = (entropy_1site[isite] + entropy_1site[jsite] -
+                    entropy_2site[key]) / 2
+        mut_entropy += mut_entropy.T
+        return mut_entropy
+
+    def calc_bond_entropy(self) -> np.ndarray:
+        r"""
+        Calculate von Neumann entropy at each bond according to :math:`S = -\textrm{Tr}(\rho \ln \rho)`
+        where :math:`\rho` is the reduced density matrix of either block.
+
+        Returns
+        -------
+        S : 1D array
+            a NumPy array containing the entropy values.
+        
+        """
+        
+        # Make sure that the bond entropy is from the left to the right and not
+        # destroy the original mps
+        mps = self.copy()
+        mps.ensure_right_canonical()
+        _, s_list = mps.compress(temp_m_trunc=np.inf, ret_s=True)
+        return np.array([calc_vn_entropy(sigma ** 2) for sigma in s_list])
+
+    def dump(self, fname):
+        super().dump(fname, other_attrs=["coeff"])
+
+    def __setitem__(self, key, value):
+        return super().__setitem__(key, value)
+
+    
+    def add(self, other):
+        if not np.allclose(self.coeff, other.coeff):
+            self.scale(self.coeff, inplace=True)
+            other.scale(other.coeff, inplace=True)
+            self.coeff = 1
+            other.coeff = 1
+        return super().add(other)
+    
+    def distance(self, other) -> float:
+        if not np.allclose(self.coeff, other.coeff):
+            self.scale(self.coeff, inplace=True)
+            other.scale(other.coeff, inplace=True)
+            self.coeff = 1
+            other.coeff = 1
+        return super().distance(other)
+
+
+def projector(
+    ms: xp.ndarray, left: bool, Ovlp_inv1: xp.ndarray = None, Ovlp0: xp.ndarray = None
+) -> xp.ndarray:
+    if left:
+        axes = (-1, -1)
+    else:
+        axes = (0, 0)
+
+    if Ovlp_inv1 is None:
+        proj = xp.tensordot(ms, ms.conj(), axes=axes)
+    else:
+        # consider the case that the canonical condition is not fulfilled
+        if left:
+            proj = xp.tensordot(Ovlp0, ms, axes=(-1, 0))
+            proj = xp.tensordot(proj, Ovlp_inv1, axes=(-1, 0))
+            proj = xp.tensordot(proj, ms.conj(), axes=(-1, -1))
+        else:
+            proj = xp.tensordot(ms, Ovlp0, axes=(-1, 0))
+            proj = xp.tensordot(Ovlp_inv1, proj, axes=(-1, 0))
+            proj = xp.tensordot(proj, ms.conj(), axes=(0, 0))
+
+    if left:
+        sz = int(np.prod(ms.shape[:-1]))
+    else:
+        sz = int(np.prod(ms.shape[1:]))
+    Iden = xp.array(xp.diag(xp.ones(sz)), dtype=backend.real_dtype).reshape(proj.shape)
+    proj = Iden - proj
+    return proj
+
+def integrand_func_factory(
+    shape,
+    hop,
+    islast,
+    S_inv: Union[np.ndarray, xp.ndarray],
+    left: bool,
+    coef: complex,
+    ovlp_inv1: Union[xp.ndarray, np.ndarray] = None,
+    ovlp_inv0: Union[xp.ndarray, np.ndarray] = None,
+    ovlp0: Union[xp.ndarray, np.ndarray] = None,
+):
+    S_inv, ovlp_inv1, ovlp_inv0, ovlp0 = map(asxp, [S_inv, ovlp_inv1, ovlp_inv0, ovlp0])
+    # left == True: projector operate on the left side of the HC
+    # Ovlp0 is (#.conj, #), Ovlp_inv0 = (#, #.conj), Ovlp_inv1 = (#, #.conj)
+    # S_inv is (#.conj, #)
+    def func(t, y):
+        y0 = asxp(y.reshape(shape))
+        HC = hop(y0)
+        if not islast:
+            proj = projector(y0, left, ovlp_inv1, ovlp0)
+            if y0.ndim == 3:
+                if left:
+                    HC = tensordot(proj, HC, axes=([2, 3], [0, 1]))
+                else:
+                    HC = tensordot(HC, proj, axes=([1, 2], [2, 3]))
+            elif y0.ndim == 4:
+                if left:
+                    HC = tensordot(proj, HC, axes=([3, 4, 5], [0, 1, 2]))
+                else:
+                    HC = tensordot(HC, proj, axes=([1, 2, 3], [3, 4, 5]))
+
+        if left:
+            if ovlp_inv0 is not None:
+                HC = tensordot(ovlp_inv0, HC, axes=(-1, 0))
+            return tensordot(HC, S_inv, axes=(-1, 0)).ravel() / coef
+        else:
+            if ovlp_inv0 is not None:
+                HC = tensordot(HC, ovlp_inv0, axes=(-1, -1))
+            return tensordot(S_inv, HC, axes=(0, 0)).ravel() / coef
+
+    return func
+
+
+def transferMat(mps, mpsconj, domain, imps, val) -> np.ndarray:
+    """
+    calculate the transfer matrix from the left hand or the right hand
+    """
+    if mpsconj is not None:
+        ms, ms_conj = mps[imps].array, mpsconj[imps].array
+    else:
+        ms = mps[imps].array
+        ms_conj = ms.conj()
+
+    if mps[0].ndim == 3:
+        if domain == "R":
+            val = tensordot(ms_conj, val, axes=(2, 0))
+            val = tensordot(val, ms, axes=([1, 2], [1, 2]))
+        elif domain == "L":
+            val = tensordot(ms_conj, val, axes=(0, 0))
+            val = tensordot(val, ms, axes=([0, 2], [1, 0]))
+        else:
+            assert False
+    elif mps[0].ndim == 4:
+        if domain == "R":
+            val = tensordot(ms_conj, val, axes=(3, 0))
+            val = tensordot(val, ms, axes=([1, 2, 3], [1, 2, 3]))
+        elif domain == "L":
+            val = tensordot(ms_conj, val, axes=(0, 0))
+            val = tensordot(val, ms, axes=([0, 3, 1], [1, 0, 2]))
+        else:
+            assert False
+    else:
+        raise ValueError(f"the dim of local mps is not correct: {mps[0].ndim}")
+
+    return asnumpy(val)
+
+
+def _mu_regularize(s, epsilon=1e-10):
+    """
+    regularization of the singular value of the reduced density matrix
+    """
+    epsilon = np.sqrt(epsilon)
+    return s + epsilon * np.exp(-s / epsilon)
+
+
+class BraKetPair:
+    def __init__(self, bra_mps, ket_mps, mpo=None):
+        self.bra_mps = bra_mps
+        self.ket_mps = ket_mps
+        self.mpo = mpo
+        self.ft = self.calc_ft()
+
+    def calc_ft(self):
+        if self.mpo is None:
+            dot = self.bra_mps.conj().dot(self.ket_mps)
+        else:
+            dot = self.ket_mps.expectation(self.mpo, self.bra_mps.conj())
+        return complex(
+            dot * np.conjugate(self.bra_mps.coeff)
+            * self.ket_mps.coeff
+        )
+
+    def __str__(self):
+        if np.iscomplexobj(self.ft):
+            # if negative, sign is included in the imag part
+            sign = "+" if 0 <= self.ft.imag else ""
+            ft_str = "%g%s%gj" % (self.ft.real, sign, self.ft.imag)
+        else:
+            ft_str = "%g" % self.ft
+        return "bra: %s, ket: %s, ft: %s" % (self.bra_mps, self.ket_mps, ft_str)
+
+    def __iter__(self):
+        return iter((self.bra_mps, self.ket_mps))
+
+
+def min_abs(t1, t2):
+    # t1, t2 could be int, float, complex
+    # return the number with smaller norm
+
+    assert xp.iscomplex(t1) == xp.iscomplex(t2)
+
+    if xp.absolute(t1) < xp.absolute(t2):
+        return t1
+    else:
+        return t2
+
+
+def _construct_freq_environ(mpos_hash: List[List[int]], hash_to_obj: Dict[int, Matrix], mps: Mps, domain: str, mps_conj):
+    """
+    Construct environment tensors that are most frequently shown in the group of MPOs
+    """
+    assert domain in ["L", "R"]
+    # count mpo sequence frequency
+    counter = Counter()
+    for mpo_hash in mpos_hash:
+        for i in range(1, len(mpo_hash)+1):
+            if domain == "L":
+                mpo_seq = mpo_hash[:i]
+            else:
+                mpo_seq = reversed(mpo_hash[-i:])
+            counter.update([tuple(mpo_seq)])
+
+    # transform the counter into a list of matrices.
+    # The most frequent sequences first. If the same freq, then shorter sequences first
+    # Note that shorter sequences are not less frequent than longer sequences
+    most_common = list(counter.items())
+    most_common.sort(key=lambda x: (-x[1], len(x[0])))
+    matrices_list = []
+    hash_list = []
+    for hashes, n in most_common:
+        # discard unique ones because they do not need to be cached
+        if n == 1:
+            break
+        # cache ``len(mps)`` sequences
+        # sequences with the same length may be treated differently.
+        if len(mps) < len(matrices_list):
+            break
+        hash_list.append(hashes)
+        matrices_list.append(list(map(hash_to_obj.get, hashes)))
+
+    # contract the tensors
+    result = {(): xp.ones((1, 1, 1), dtype=backend.real_dtype)}
+    for m_hashes, matrices in zip(hash_list, matrices_list):
+        environ = result[tuple(m_hashes[:-1])]
+        if domain == "L":
+            idx = len(matrices)-1
+        else:
+            idx = -len(matrices)
+        ms, ms_conj = mps[idx], mps_conj[idx]
+        result[tuple(m_hashes)] = contract_one_site(environ, ms, matrices[-1], domain=domain, ms_conj=ms_conj)
+    return result
+
+
+def _get_freq_environ(environ_dict, mpo, domain, max_length):
+    assert domain in ["L", "R"]
+
+    if domain == "L":
+        it = mpo
+    else:
+        it = reversed(mpo)
+
+    hashes = []
+    for mo in it:
+        hashes.append(hash(mo))
+        if (not tuple(hashes) in environ_dict) or (max_length < len(hashes)):
+            hashes.pop()
+            break
+    if domain == "L":
+        i = len(hashes) - 1
+    else:
+        i = len(mpo) - len(hashes)
+
+    environ = environ_dict[tuple(hashes)]
+    return environ, i
```

### Comparing `renormalizer-0.0.8/renormalizer/mps/svd_qn.py` & `renormalizer-0.0.9/renormalizer/mps/svd_qn.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,316 +1,316 @@
-# -*- coding: utf-8 -*-
-# Author: Jiajun Ren <jiajunren0522@gmail.com>
-import logging
-
-import scipy.linalg
-
-from renormalizer.mps.backend import np, backend
-
-logger = logging.getLogger(__name__)
-
-
-def optimized_svd(a, full_matrices, opt_full_matrices):
-    # optimize performance when ``full_matrices = opt_full_matrices = True``
-    # and the shape of ``a`` is extremely unbalanced
-    # The idea is to construct only a limited number of orthogonal basis rather than all of them
-    # (which are not necessary in most cases)
-    m, n = a.shape
-    if not full_matrices:
-        opt_full_matrices = False
-
-    # whether do the optimization
-    # here 1/3 and 3 are only empirical
-    opt = opt_full_matrices and not (1 / 3 < m / n < 3)
-
-    # if opt, always set ``full_matrices=False``
-    try:
-        U, S, Vt = scipy.linalg.svd(
-            a,
-            full_matrices=full_matrices and not opt,
-            lapack_driver="gesdd",
-        )
-    except scipy.linalg.LinAlgError:
-        logger.warning("SVD failed to converge")
-        U, S, Vt = scipy.linalg.svd(
-            a,
-            full_matrices=full_matrices and not opt,
-            lapack_driver="gesvd",
-        )
-    if not opt:
-        return U, S, Vt
-
-    # if opt, add n additional basis assuming  2 * n < m
-    if m < n:
-        Vt = add_orthonormal_basis(Vt.T).T
-    elif n < m:
-        U = add_orthonormal_basis(U)
-    else:
-        assert False
-    return U, S, Vt
-
-
-def add_orthonormal_basis(u):
-    # add `n` basis. `n` is empirical
-    m, n = u.shape
-    assert 2 * n < m
-    assert np.allclose(u.T.conj() @ u, np.eye(n), atol=backend.canonical_atol)
-    a = np.random.rand(m,n)
-    a = a - u @ (u.T.conj() @ a)
-    q, _ = scipy.linalg.qr(a, mode='economic')
-    res = np.concatenate([u, q], axis=1)
-
-    assert np.allclose(res.T.conj() @ res, np.eye(2 * n), atol=backend.canonical_atol)
-    return res
-
-
-def blockappend(
-        block_v_list,
-        block_v_list0,
-        qn_list,
-        qn_list0,
-        sv_list0,
-        v,
-        n,
-        dim,
-        indice,
-        shape,
-        full_matrices=True,
-):
-    block_v_list.append(blockrecover(indice, v[:, :dim], shape))
-    qn_list += [n] * dim
-    if full_matrices:
-        block_v_list0.append(blockrecover(indice, v[:, dim:], shape))
-        qn_list0 += [n] * (v.shape[1] - dim)
-        sv_list0.append(np.zeros(v.shape[1] - dim))
-
-    return block_v_list, block_v_list0, qn_list, qn_list0, sv_list0
-
-
-def blockrecover(indices, U, dim):
-    """
-    recover the block element to its original position
-    """
-    resortU = np.zeros([dim, U.shape[1]], dtype=U.dtype)
-    resortU[indices, :] = U
-
-    return resortU
-
-
-def svd_qn(
-        coef_array: np.ndarray,
-        qnbigl: np.ndarray,
-        qnbigr: np.ndarray,
-        qntot: np.ndarray,
-        QR: bool=False,
-        system: str=None,
-        full_matrices: bool=True,
-        opt_full_matrices: bool=True
-):
-    r""" Block decompose the coefficient array (l, sigmal, sigmar, r) or (l,sigma,r) by SVD/QR according to
-    the quantum number.
-
-    Parameters
-    ----------
-    coef_array : np.ndarray
-        The coefficient array to be decomposed
-    qnbigl : np.ndarray
-        Quantum number of the left side (aka the super-L-block quantum number).
-        Corresponds to the first index (or indices) of ``cstruct``.
-    qnbigr : np.ndarray
-        Quantum number of the right side (aka the super-R-block quantum number)
-        Corresponds to the last index (or indices) of ``cstruct``.
-    qntot : np.ndarray
-        The quantum number to be preserved.
-    QR : bool
-        Whether carry out QR decomposition instead of SVD decomposition. Default is False.
-        QR decomposition is in principle faster than SVD decomposition, but it can not obtain
-        singular values. Default is ``False``.
-    system: str
-        The side of the system, required when ``QR=True``.
-        Possible values are ``"L"`` and ``"R"``, corresponding to QR and RQ decomposition respectively.
-    full_matrices: bool
-        Whether obtain full matrices for the SVD/QR decomposition.
-        See the documentation of ``scipy.linalg.svd`` and ``scipy.linalg.qr`` for details.
-        Default is ``True``
-    opt_full_matrices: bool
-        Whether perform optimization if ``full_matrices=True``.
-        The optimized version does not calculate full matrices but adds a limited amount of
-        additional orthonormal basis (in contrast to all of the basis when ``full_matrices=True``)
-        to the decomposition.
-
-    Returns
-    -------
-    U: np.ndarray
-        U matrix for SVD decomposition.
-    S_u: np.ndarray
-        Singular values for the singular vectors in U. Not returned when ``QR=True``.
-    new_qnl: list
-        New quantum number for U (super-L-block).
-    V: np.ndarray
-        V matrix for SVD decomposition.
-    S_v: np.ndarray
-        Singular values for the singular vectors in V. Not returned when ``QR=True``.
-    new_qnr: list
-        New quantum number for V (super-R-block).
-    """
-    SVD = not QR
-    coef_matrix = coef_array.reshape((np.prod(qnbigl.shape[:-1]), np.prod(qnbigr.shape[:-1])))
-
-    qn_size = len(qntot)
-    localqnl = qnbigl.reshape(-1, qn_size)
-    localqnr = qnbigr.reshape(-1, qn_size)
-
-    block_u_list = []  # corresponds to nonzero svd value
-    block_u_list0 = []  # corresponds to zero svd value
-    block_v_list = []   # the same hereinafter
-    block_v_list0 = []
-    block_s_list = []
-    block_su_list0 = []
-    block_sv_list0 = []
-    qnl_list = []
-    qnl_list0 = []
-    qnr_list = []
-    qnr_list0 = []
-
-    # loop through each set of valid quantum numbers
-    for nl in set([tuple(t) for t in localqnl]):
-        nr = qntot - nl
-        rset = np.where(get_qn_mask(localqnr, nr))[0]
-        if len(rset) == 0:
-            continue
-        lset = np.where(get_qn_mask(localqnl, nl))[0]
-        block = coef_matrix.ravel().take(
-            (lset * coef_matrix.shape[1]).reshape(-1, 1) + rset
-        )
-        dim = min(block.shape)
-        if SVD:
-            block_u, block_s, block_vt = optimized_svd(
-                block,
-                full_matrices=full_matrices,
-                opt_full_matrices=opt_full_matrices
-            )
-            block_s_list.append(block_s)
-        else:
-            if full_matrices:
-                mode = "full"
-            else:
-                mode = "economic"
-            if system == "R":
-                block_u, block_vt = scipy.linalg.rq(block, mode=mode)
-            elif system == "L":
-                block_u, block_vt = scipy.linalg.qr(block, mode=mode)
-            else:
-                assert False
-
-        blockappend(
-            block_u_list, block_u_list0, qnl_list, qnl_list0, block_su_list0,
-            block_u, nl, dim, lset, coef_matrix.shape[0], full_matrices=full_matrices,
-        )
-        blockappend(
-            block_v_list, block_v_list0, qnr_list, qnr_list0, block_sv_list0,
-            block_vt.T, nr, dim, rset, coef_matrix.shape[1], full_matrices=full_matrices,
-        )
-
-    # sanity check
-    if not full_matrices:
-        for l in [block_u_list0, block_v_list0, block_su_list0, block_sv_list0, qnl_list0, qnr_list0]:
-            assert len(l) == 0
-    if len(block_u_list) + len(block_u_list0) == 0 or len(block_v_list) + len(block_v_list0) == 0:
-        raise ValueError("Invalid quantum number")
-    # concatenate the blocks and return them
-    u = np.concatenate(block_u_list + block_u_list0, axis=1)
-    v = np.concatenate(block_v_list + block_v_list0, axis=1)
-    new_qnl = qnl_list + qnl_list0
-    new_qnr = qnr_list + qnr_list0
-    if QR:
-        return u, new_qnl, v, new_qnr
-
-    su = np.concatenate(block_s_list + block_su_list0)
-    sv = np.concatenate(block_s_list + block_sv_list0)
-    if not full_matrices:
-        # sort the singular values
-        assert np.allclose(su, sv)
-        s_order = np.argsort(su)[::-1]
-        u = u[:, s_order]
-        v = v[:, s_order]
-        su = sv = su[s_order]
-        new_qnl = np.array(new_qnl)[s_order].tolist()
-        new_qnr = np.array(new_qnr)[s_order].tolist()
-    return u, su, new_qnl, v, sv, new_qnr
-
-
-def eigh_qn(dm, qnbigl, qnbigr, qntot, system):
-    r""" Diagonalization of the reduced density matrix for multistate algorithms.
-
-    Parameters
-    ----------
-    dm : np.ndarray
-        The reduced density matrix to be decomposed
-    qnbigl : np.ndarray
-        Quantum number of the left side (aka the super-L-block quantum number).
-    qnbigr : np.ndarray
-        Quantum number of the right side (aka the super-R-block quantum number)
-    qntot : np.ndarray
-        The quantum number to be preserved.
-    system: str
-        The side of the system. Possible values are ``"L"`` and ``"R"``.
-
-    Returns
-    -------
-    U: np.ndarray
-        U matrix for the diagonalization (eigenvectors).
-    S: np.ndarray
-        Singular values for the singular vectors in U obtained by the square root of the eigenvalues.
-    new_qn: list
-        New quantum number for U.
-    """
-    assert system in ["L", "R"]
-    if system == "L":
-        # qnbig and complementary qnbig
-        qnbig, comp_qnbig = qnbigl, qnbigr
-    else:
-        qnbig, comp_qnbig = qnbigr, qnbigl
-    del qnbigl, qnbigr
-    qn_size = len(qntot)
-    localqn = qnbig.reshape(-1, qn_size)
-
-    block_u_list = []
-    block_s_list = []
-    new_qn = []
-
-    for nl in set([tuple(t) for t in localqn]):
-        nr = qntot - nl
-        if np.sum(get_qn_mask(comp_qnbig, nr)) == 0:
-            continue
-        lset = rset = np.where(get_qn_mask(localqn, nl))[0]
-        block = dm.ravel().take(
-            (lset * len(localqn)).reshape(-1, 1) + rset
-        )
-        block_s2, block_u = scipy.linalg.eigh(block)
-        # numerical error for eigenvalue < 0
-        block_s2[block_s2 < 0] = 0
-        block_s = np.sqrt(block_s2)
-        block_s_list.append(block_s)
-        blockappend(
-            block_u_list, [], new_qn, [], [],
-            block_u, nl, len(lset), lset, len(localqn), full_matrices=False,
-        )
-
-    u = np.concatenate(block_u_list, axis=1)
-    s = np.concatenate(block_s_list)
-    return u, s, new_qn
-
-
-def add_outer(a:np.ndarray, b:np.ndarray):
-    # a variant of np.add.outer which keeps the last dimension
-    assert a.shape[-1] == b.shape[-1]
-    qn_size = a.shape[-1]
-    out_list = []
-    for i in range(qn_size):
-        out_list.append(np.add.outer(a[..., i], b[..., i]))
-    out_list = np.array(out_list)
-    return out_list.transpose(list(range(1, out_list.ndim))+[0])
-
-
-def get_qn_mask(qnmat:np.ndarray, qntot):
-    return np.all(qnmat == np.array(qntot), axis=-1)
+# -*- coding: utf-8 -*-
+# Author: Jiajun Ren <jiajunren0522@gmail.com>
+import logging
+
+import scipy.linalg
+
+from renormalizer.mps.backend import np, backend
+
+logger = logging.getLogger(__name__)
+
+
+def optimized_svd(a, full_matrices, opt_full_matrices):
+    # optimize performance when ``full_matrices = opt_full_matrices = True``
+    # and the shape of ``a`` is extremely unbalanced
+    # The idea is to construct only a limited number of orthogonal basis rather than all of them
+    # (which are not necessary in most cases)
+    m, n = a.shape
+    if not full_matrices:
+        opt_full_matrices = False
+
+    # whether do the optimization
+    # here 1/3 and 3 are only empirical
+    opt = opt_full_matrices and not (1 / 3 < m / n < 3)
+
+    # if opt, always set ``full_matrices=False``
+    try:
+        U, S, Vt = scipy.linalg.svd(
+            a,
+            full_matrices=full_matrices and not opt,
+            lapack_driver="gesdd",
+        )
+    except scipy.linalg.LinAlgError:
+        logger.warning("SVD failed to converge")
+        U, S, Vt = scipy.linalg.svd(
+            a,
+            full_matrices=full_matrices and not opt,
+            lapack_driver="gesvd",
+        )
+    if not opt:
+        return U, S, Vt
+
+    # if opt, add n additional basis assuming  2 * n < m
+    if m < n:
+        Vt = add_orthonormal_basis(Vt.T).T
+    elif n < m:
+        U = add_orthonormal_basis(U)
+    else:
+        assert False
+    return U, S, Vt
+
+
+def add_orthonormal_basis(u):
+    # add `n` basis. `n` is empirical
+    m, n = u.shape
+    assert 2 * n < m
+    assert np.allclose(u.T.conj() @ u, np.eye(n), atol=backend.canonical_atol)
+    a = np.random.rand(m,n)
+    a = a - u @ (u.T.conj() @ a)
+    q, _ = scipy.linalg.qr(a, mode='economic')
+    res = np.concatenate([u, q], axis=1)
+
+    assert np.allclose(res.T.conj() @ res, np.eye(2 * n), atol=backend.canonical_atol)
+    return res
+
+
+def blockappend(
+        block_v_list,
+        block_v_list0,
+        qn_list,
+        qn_list0,
+        sv_list0,
+        v,
+        n,
+        dim,
+        indice,
+        shape,
+        full_matrices=True,
+):
+    block_v_list.append(blockrecover(indice, v[:, :dim], shape))
+    qn_list += [n] * dim
+    if full_matrices:
+        block_v_list0.append(blockrecover(indice, v[:, dim:], shape))
+        qn_list0 += [n] * (v.shape[1] - dim)
+        sv_list0.append(np.zeros(v.shape[1] - dim))
+
+    return block_v_list, block_v_list0, qn_list, qn_list0, sv_list0
+
+
+def blockrecover(indices, U, dim):
+    """
+    recover the block element to its original position
+    """
+    resortU = np.zeros([dim, U.shape[1]], dtype=U.dtype)
+    resortU[indices, :] = U
+
+    return resortU
+
+
+def svd_qn(
+        coef_array: np.ndarray,
+        qnbigl: np.ndarray,
+        qnbigr: np.ndarray,
+        qntot: np.ndarray,
+        QR: bool=False,
+        system: str=None,
+        full_matrices: bool=True,
+        opt_full_matrices: bool=True
+):
+    r""" Block decompose the coefficient array (l, sigmal, sigmar, r) or (l,sigma,r) by SVD/QR according to
+    the quantum number.
+
+    Parameters
+    ----------
+    coef_array : np.ndarray
+        The coefficient array to be decomposed
+    qnbigl : np.ndarray
+        Quantum number of the left side (aka the super-L-block quantum number).
+        Corresponds to the first index (or indices) of ``cstruct``.
+    qnbigr : np.ndarray
+        Quantum number of the right side (aka the super-R-block quantum number)
+        Corresponds to the last index (or indices) of ``cstruct``.
+    qntot : np.ndarray
+        The quantum number to be preserved.
+    QR : bool
+        Whether carry out QR decomposition instead of SVD decomposition. Default is False.
+        QR decomposition is in principle faster than SVD decomposition, but it can not obtain
+        singular values. Default is ``False``.
+    system: str
+        The side of the system, required when ``QR=True``.
+        Possible values are ``"L"`` and ``"R"``, corresponding to QR and RQ decomposition respectively.
+    full_matrices: bool
+        Whether obtain full matrices for the SVD/QR decomposition.
+        See the documentation of ``scipy.linalg.svd`` and ``scipy.linalg.qr`` for details.
+        Default is ``True``
+    opt_full_matrices: bool
+        Whether perform optimization if ``full_matrices=True``.
+        The optimized version does not calculate full matrices but adds a limited amount of
+        additional orthonormal basis (in contrast to all of the basis when ``full_matrices=True``)
+        to the decomposition.
+
+    Returns
+    -------
+    U: np.ndarray
+        U matrix for SVD decomposition.
+    S_u: np.ndarray
+        Singular values for the singular vectors in U. Not returned when ``QR=True``.
+    new_qnl: list
+        New quantum number for U (super-L-block).
+    V: np.ndarray
+        V matrix for SVD decomposition.
+    S_v: np.ndarray
+        Singular values for the singular vectors in V. Not returned when ``QR=True``.
+    new_qnr: list
+        New quantum number for V (super-R-block).
+    """
+    SVD = not QR
+    coef_matrix = coef_array.reshape((np.prod(qnbigl.shape[:-1]), np.prod(qnbigr.shape[:-1])))
+
+    qn_size = len(qntot)
+    localqnl = qnbigl.reshape(-1, qn_size)
+    localqnr = qnbigr.reshape(-1, qn_size)
+
+    block_u_list = []  # corresponds to nonzero svd value
+    block_u_list0 = []  # corresponds to zero svd value
+    block_v_list = []   # the same hereinafter
+    block_v_list0 = []
+    block_s_list = []
+    block_su_list0 = []
+    block_sv_list0 = []
+    qnl_list = []
+    qnl_list0 = []
+    qnr_list = []
+    qnr_list0 = []
+
+    # loop through each set of valid quantum numbers
+    for nl in set([tuple(t) for t in localqnl]):
+        nr = qntot - nl
+        rset = np.where(get_qn_mask(localqnr, nr))[0]
+        if len(rset) == 0:
+            continue
+        lset = np.where(get_qn_mask(localqnl, nl))[0]
+        block = coef_matrix.ravel().take(
+            (lset * coef_matrix.shape[1]).reshape(-1, 1) + rset
+        )
+        dim = min(block.shape)
+        if SVD:
+            block_u, block_s, block_vt = optimized_svd(
+                block,
+                full_matrices=full_matrices,
+                opt_full_matrices=opt_full_matrices
+            )
+            block_s_list.append(block_s)
+        else:
+            if full_matrices:
+                mode = "full"
+            else:
+                mode = "economic"
+            if system == "R":
+                block_u, block_vt = scipy.linalg.rq(block, mode=mode)
+            elif system == "L":
+                block_u, block_vt = scipy.linalg.qr(block, mode=mode)
+            else:
+                assert False
+
+        blockappend(
+            block_u_list, block_u_list0, qnl_list, qnl_list0, block_su_list0,
+            block_u, nl, dim, lset, coef_matrix.shape[0], full_matrices=full_matrices,
+        )
+        blockappend(
+            block_v_list, block_v_list0, qnr_list, qnr_list0, block_sv_list0,
+            block_vt.T, nr, dim, rset, coef_matrix.shape[1], full_matrices=full_matrices,
+        )
+
+    # sanity check
+    if not full_matrices:
+        for l in [block_u_list0, block_v_list0, block_su_list0, block_sv_list0, qnl_list0, qnr_list0]:
+            assert len(l) == 0
+    if len(block_u_list) + len(block_u_list0) == 0 or len(block_v_list) + len(block_v_list0) == 0:
+        raise ValueError("Invalid quantum number")
+    # concatenate the blocks and return them
+    u = np.concatenate(block_u_list + block_u_list0, axis=1)
+    v = np.concatenate(block_v_list + block_v_list0, axis=1)
+    new_qnl = qnl_list + qnl_list0
+    new_qnr = qnr_list + qnr_list0
+    if QR:
+        return u, new_qnl, v, new_qnr
+
+    su = np.concatenate(block_s_list + block_su_list0)
+    sv = np.concatenate(block_s_list + block_sv_list0)
+    if not full_matrices:
+        # sort the singular values
+        assert np.allclose(su, sv)
+        s_order = np.argsort(su)[::-1]
+        u = u[:, s_order]
+        v = v[:, s_order]
+        su = sv = su[s_order]
+        new_qnl = np.array(new_qnl)[s_order].tolist()
+        new_qnr = np.array(new_qnr)[s_order].tolist()
+    return u, su, new_qnl, v, sv, new_qnr
+
+
+def eigh_qn(dm, qnbigl, qnbigr, qntot, system):
+    r""" Diagonalization of the reduced density matrix for multistate algorithms.
+
+    Parameters
+    ----------
+    dm : np.ndarray
+        The reduced density matrix to be decomposed
+    qnbigl : np.ndarray
+        Quantum number of the left side (aka the super-L-block quantum number).
+    qnbigr : np.ndarray
+        Quantum number of the right side (aka the super-R-block quantum number)
+    qntot : np.ndarray
+        The quantum number to be preserved.
+    system: str
+        The side of the system. Possible values are ``"L"`` and ``"R"``.
+
+    Returns
+    -------
+    U: np.ndarray
+        U matrix for the diagonalization (eigenvectors).
+    S: np.ndarray
+        Singular values for the singular vectors in U obtained by the square root of the eigenvalues.
+    new_qn: list
+        New quantum number for U.
+    """
+    assert system in ["L", "R"]
+    if system == "L":
+        # qnbig and complementary qnbig
+        qnbig, comp_qnbig = qnbigl, qnbigr
+    else:
+        qnbig, comp_qnbig = qnbigr, qnbigl
+    del qnbigl, qnbigr
+    qn_size = len(qntot)
+    localqn = qnbig.reshape(-1, qn_size)
+
+    block_u_list = []
+    block_s_list = []
+    new_qn = []
+
+    for nl in set([tuple(t) for t in localqn]):
+        nr = qntot - nl
+        if np.sum(get_qn_mask(comp_qnbig, nr)) == 0:
+            continue
+        lset = rset = np.where(get_qn_mask(localqn, nl))[0]
+        block = dm.ravel().take(
+            (lset * len(localqn)).reshape(-1, 1) + rset
+        )
+        block_s2, block_u = scipy.linalg.eigh(block)
+        # numerical error for eigenvalue < 0
+        block_s2[block_s2 < 0] = 0
+        block_s = np.sqrt(block_s2)
+        block_s_list.append(block_s)
+        blockappend(
+            block_u_list, [], new_qn, [], [],
+            block_u, nl, len(lset), lset, len(localqn), full_matrices=False,
+        )
+
+    u = np.concatenate(block_u_list, axis=1)
+    s = np.concatenate(block_s_list)
+    return u, s, new_qn
+
+
+def add_outer(a:np.ndarray, b:np.ndarray):
+    # a variant of np.add.outer which keeps the last dimension
+    assert a.shape[-1] == b.shape[-1]
+    qn_size = a.shape[-1]
+    out_list = []
+    for i in range(qn_size):
+        out_list.append(np.add.outer(a[..., i], b[..., i]))
+    out_list = np.array(out_list)
+    return out_list.transpose(list(range(1, out_list.ndim))+[0])
+
+
+def get_qn_mask(qnmat:np.ndarray, qntot):
+    return np.all(qnmat == np.array(qntot), axis=-1)
```

### Comparing `renormalizer-0.0.8/renormalizer/mps/symbolic_mpo.py` & `renormalizer-0.0.9/renormalizer/mps/symbolic_mpo.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,647 +1,647 @@
-# -*- coding: utf-8 -*-
-import logging
-import itertools
-from collections import namedtuple
-from typing import List, Set, Tuple, Dict
-
-import numpy as np
-import scipy
-import scipy.sparse
-
-from renormalizer.model import Model
-from renormalizer.model.op import Op
-from renormalizer.lib import bipartite_vertex_cover
-
-logger = logging.getLogger(__name__)
-
-# The `Op` class is transformed to a light-weight named tuple
-# for better performance
-OpTuple = namedtuple("OpTuple", ["symbol", "qn", "factor"])
-
-
-def construct_symbolic_mpo(table, factor, algo="Hopcroft-Karp"):
-    r"""
-    A General Compact (Symbolic) MPO Construction Routine
-
-    Args:
-
-    table: an operator table with shape (operator nterm, nsite). Each entry contains elementary operators on each site.
-    factor (np.ndarray): one prefactor vector (dim: operator nterm)
-    algo: the algorithm used to select local ops, "Hopcroft-Karp"(default), "Hungarian".
-          They are both global optimal and have only minor performance difference.
-
-    Note:
-    op with the same op.symbol must have the same op.qn and op.factor
-
-    Return:
-    mpo: symbolic mpo
-    mpoqn: quantum number
-    qntot: total quantum number of the operator
-    qnidx: the index of the qn
-
-    The idea:
-
-    the index of the primary ops {0:"I", 1:"a", 2:r"a^\dagger"}
-
-    for example: H = 2.0 * a_1 a_2^dagger   + 3.0 * a_2^\dagger a_3 + 4.0*a_0^\dagger a_3
-    The column names are the site indices with 0 and 4 imaginary (see the note below)
-    and the content of the table is the index of primary operators.
-                        s0   s1   s2   s3  s4  factor
-    a_1 a_2^dagger      0    1    2    0   0   2.0
-    a_2^\dagger a_3     0    0    2    1   0   3.0
-    a_1^\dagger a_3     0    2    0    1   0   4.0
-    for convenience the first and last column mean that the operator of the left and right hand of the system is I
-
-    cut the string to construct the row(left) and column(right) operator and find the duplicated/independent terms
-                        s0   s1 |  s2   s3  s4 factor
-    a_1 a_2^dagger      0    1  |  2    0   0  2.0
-    a_2^\dagger a_3     0    0  |  2    1   0  3.0
-    a_1^\dagger a_3     0    2  |  0    1   0  4.0
-
-     The content of the table below means matrix elements with basis explained in the notes.
-     In the matrix elements, 1 means combination and 0 means no combination.
-          (2,0,0) (2,1,0) (0,1,0)  -> right side of the above table
-     (0,1)   1       0       0
-     (0,0)   0       1       0
-     (0,2)   0       0       1
-       |
-       v
-     left side of the above table
-     In this case all operators are independent so the content of the matrix is diagonal
-
-    and select the terms and rearrange the table
-    The selection rule is to find the minimal number of rows+cols that can eliminate the
-    matrix
-                      s1   s2 |  s3 s4 factor
-    a_1 a_2^dagger    0'   2  |  0  0  2.0
-    a_2^\dagger a_3   1'   2  |  1  0  3.0
-    a_1^\dagger a_3   2'   0  |  1  0  4.0
-    0'/1'/2' are three new operators(could be non-elementary)
-    The local mpo is the transformation matrix between 0,0,0 to 0',1',2'.
-    In this case, the local mpo is simply (1, 0, 2)
-
-    cut the string and find the duplicated/independent terms
-            (0,0), (1,0)
-     (0',2)   1      0
-     (1',2)   0      1
-     (2',0)   0      1
-
-    and select the terms and rearrange the table
-    apparently choose the (1,0) column and construct the complementary operator (1',2)+(2',0) is better
-    0'' =  3.0 * (1', 2) + 4.0 * (2', 0)
-                                                 s2     s3 | s4 factor
-    (4.0 * a_1^dagger + 3.0 * a_2^dagger) a_3    0''    1  | 0  1.0
-    a_1 a_2^dagger                               1''    0  | 0  2.0
-    0''/1'' are another two new operators(non-elementary)
-    The local mpo is the transformation matrix between 0',1',2' to 0'',1''
-
-             (0)
-     (0'',1)  1
-     (1'',0)  1
-
-    The local mpo is the transformation matrix between 0'',1'' to 0'''
-    """
-
-    qn_size = len(table[0][0].qn)
-    # Simplest case. Cut to the chase
-    if len(table) == 1:
-        # The first layer: number of sites. The 2nd and 3rd layer: in and out virtual bond
-        # the 4th layer: operator sums
-        mpo: List[List[List[List[[Op]]]]] = []
-        mpoqn = [np.zeros((1, qn_size), dtype=int)]
-        primary_ops = list(set(table[0]))
-        op2idx = dict(zip(primary_ops, range(len(primary_ops))))
-        out_ops_list: List[List[OpTuple]] = [[OpTuple([0], qn=0, factor=1)]]
-        for op in table[0]:
-            mpo.append([[[op]]])
-            qn = mpoqn[-1][0] + op.qn
-            mpoqn.append(np.array([qn]))
-            out_ops_list.append([OpTuple([0, op2idx[op]], qn=qn, factor=1)])
-
-        mpo[-1][0][0][0] = factor[0] * mpo[-1][0][0][0]
-        last_optuple = out_ops_list[-1][0]
-        out_ops_list[-1][0] = OpTuple(last_optuple.symbol, qn=last_optuple.qn, factor=factor[0]*last_optuple.factor)
-        qntot = qn
-        mpoqn[-1] = np.zeros((1, qn_size), dtype=int)
-        qnidx = len(mpo) - 1
-        # the last two terms are not set for fast construction of the operators
-        return mpo, mpoqn, qntot, qnidx, out_ops_list, primary_ops
-
-    # use np.uint32, np.uint16 to save memory
-    max_uint32 = np.iinfo(np.uint32).max
-    max_uint16 = np.iinfo(np.uint16).max
-
-    logger.debug(f"symbolic mpo algorithm: {algo}")
-    logger.debug(f"Input operator terms: {len(table)}")
-
-    # translate the symbolic operator table to an easy to manipulate numpy array
-    table = np.array(table)
-    # unique operators with DoF names taken into consideration
-    # The inclusion of DoF names is necessary for multi-dof basis.
-    unique_op: Set[Op] = set(table.ravel())
-
-    # check the index of different operators could be represented with np.uint16
-    assert len(unique_op) < max_uint16
-
-    # Construct mapping from easy-to-manipulate integer to actual Op
-    primary_ops = list(unique_op)
-
-    op2idx = dict(zip(unique_op, range(len(unique_op))))
-    new_table = np.vectorize(op2idx.get)(table).astype(np.uint16)
-
-    del unique_op
-
-    if __debug__:
-        qn_table = np.array([[x.qn for x in ta] for ta in table])
-        factor_table = np.array([[x.factor for x in ta] for ta in table])
-        for idx in range(len(primary_ops)):
-            coord = np.nonzero(new_table == idx)
-            # check that op with the same symbol has the same factor and qn
-            for j in range(qn_size):
-                assert np.unique(qn_table[:, :, j][coord]).size == 1
-            assert np.all(factor_table[coord] == factor_table[coord][0])
-
-        del factor_table, qn_table
-
-    # combine the same terms but with different factors(add them together)
-    unique_term, unique_inverse = np.unique(new_table, axis=0, return_inverse=True)
-    # it is efficient to vectorize the operation that moves the rows and cols
-    # and sum them together
-    coord = np.array([[newidx, oldidx] for oldidx, newidx in enumerate(unique_inverse)])
-    mask = scipy.sparse.csr_matrix((np.ones(len(coord)), (coord[:, 0], coord[:, 1])))
-    factor = mask.dot(factor)
-
-    # add the first and last column for convenience
-    ta = np.zeros((unique_term.shape[0], 1), dtype=np.uint16)
-    table = np.concatenate((ta, unique_term, ta), axis=1)
-    logger.debug(f"After combination of the same terms: {table.shape[0]}")
-    # check the index of interaction could be represented with np.uint32
-    assert table.shape[0] < max_uint32
-
-    del unique_term, unique_inverse
-
-    # 0 represents the identity symbol. Identity might not present
-    # in `primary_ops` but the algorithm still works.
-
-    in_ops = [[OpTuple([0], qn=np.zeros(qn_size, dtype=int), factor=1)]]
-
-    out_ops_list = _construct_symbolic_mpo(table, in_ops, factor, primary_ops, algo)
-    # number of sites + 1. Note that the table was expanded for convenience
-    assert len(out_ops_list) == len(table[0]) - 1
-    mpo = []
-    for i in range(len(out_ops_list)-1):
-        mo = compose_symbolic_mo(out_ops_list[i], out_ops_list[i+1], primary_ops)
-        mpo.append(mo)
-
-    mpoqn = []
-    for out_ops in out_ops_list:
-        qn = np.array([out_op[0].qn for out_op in out_ops])
-        mpoqn.append(qn)
-
-    qntot = mpoqn[-1][0]
-    mpoqn[-1] = np.zeros((1, qn_size), dtype=int)
-    qnidx = len(mpo) - 1
-
-    return mpo, mpoqn, qntot, qnidx, out_ops_list, primary_ops
-
-
-def _construct_symbolic_mpo(table, in_ops, factor, primary_ops, algo="Hopcroft-Karp"):
-
-    nsite = table.shape[1] - 2
-
-    out_ops_list = [in_ops]
-
-    for isite in range(nsite):
-        # split table into the row and col part
-        term_row, row_unique_inverse = np.unique(table[:, :2], axis=0, return_inverse=True)
-
-        # faster version of the following code
-        # term_col, col_unique_inverse = np.unique(table[:, 2:], axis=0, return_inverse=True)
-        term_col = {}
-        col_unique_inverse = []
-        for row in table[:, 2:]:
-            row_bytes = row.tobytes()
-            i_and_row = term_col.get(row_bytes)
-            if i_and_row is None:
-                i_and_row = (len(term_col), row)
-                term_col[row_bytes] = i_and_row
-            col_unique_inverse.append(i_and_row[0])
-        term_col = [v[1] for v in term_col.values()]
-
-        # get the non_redudant ops
-        # the +1 trick is to use the csr sparse matrix format
-        non_red = scipy.sparse.diags(np.arange(1, table.shape[0] + 1), format="csr", dtype=np.uint32)
-        coord = np.array([[newidx, oldidx] for oldidx, newidx in enumerate(row_unique_inverse)])
-        mask = scipy.sparse.csr_matrix((np.ones(len(coord), dtype=np.uint32), (coord[:, 0], coord[:, 1])))
-        non_red = mask.dot(non_red)
-        coord = np.array([[oldidx, newidx] for oldidx, newidx in enumerate(col_unique_inverse)])
-        mask = scipy.sparse.csr_matrix((np.ones(len(coord), dtype=np.uint32), (coord[:, 0], coord[:, 1])))
-        non_red = non_red.dot(mask)
-        # use sparse matrix to represent non_red will be inefficient a little
-        # bit compared to dense matrix, but saves a lot of memory when the
-        # number of terms is huge
-        # logger.info(f"isite: {isite}, bipartite graph size: {non_red.shape}")
-
-        # the usual case
-
-        bigraph = []
-        if non_red.shape[0] < non_red.shape[1]:
-            for i in range(non_red.shape[0]):
-                bigraph.append(non_red.indices[non_red.indptr[i]:non_red.indptr[i + 1]])
-            rowbool, colbool = bipartite_vertex_cover(bigraph, algo=algo)
-        else:
-            non_red_csc = non_red.tocsc()
-            for i in range(non_red.shape[1]):
-                bigraph.append(non_red_csc.indices[non_red_csc.indptr[i]:non_red_csc.indptr[i + 1]])
-            colbool, rowbool = bipartite_vertex_cover(bigraph, algo=algo)
-
-        row_select = np.nonzero(rowbool)[0]
-        # largest cover first
-        row_select = sorted(row_select, key=lambda i: non_red.indptr[i + 1] - non_red.indptr[i], reverse=True)
-        col_select = np.nonzero(colbool)[0]
-
-
-        if len(row_select) > 0:
-            assert np.amax(row_select) < non_red.shape[0]
-        if len(col_select) > 0:
-            assert np.amax(col_select) < non_red.shape[1]
-
-        # select the reserved ops
-        out_ops: List[List[OpTuple]] = []
-        new_table = []
-        new_factor = []
-
-        for row_idx in row_select:
-            # construct out_op
-            # dealing with row (left side of the table). One row corresponds to multiple cols.
-            # Produce one out operator and multiple new_table entries
-            symbol = term_row[row_idx]
-            qn = in_ops[symbol[0]][0].qn + primary_ops[symbol[1]].qn
-            out_op = OpTuple(symbol, qn, factor=1.0)
-            out_ops.append([out_op])
-
-            col_link = non_red.indices[non_red.indptr[row_idx]:non_red.indptr[row_idx + 1]]
-            stack = np.array([len(out_ops) - 1] * len(col_link), dtype=np.uint16).reshape(-1, 1)
-            new_table.append(np.hstack((stack, [term_col[i] for i in col_link])))
-            new_factor.append(factor[non_red[row_idx, col_link].toarray() - 1])
-            non_red.data[non_red.indptr[row_idx]:non_red.indptr[row_idx + 1]] = 0
-
-        non_red.eliminate_zeros()
-
-        nonzero_row_idx, nonzero_col_idx = non_red.nonzero()
-        for col_idx in col_select:
-
-            out_ops.append([])
-            # complementary operator
-            # dealing with column (right side of the table). One col correspond to multiple rows.
-            # Produce multiple out operators and one new_table entry
-            non_red_one_col = non_red[:, col_idx].toarray().flatten()
-            for i in nonzero_row_idx[np.nonzero(nonzero_col_idx == col_idx)[0]]:
-                symbol = term_row[i]
-                qn = in_ops[symbol[0]][0].qn + primary_ops[symbol[1]].qn
-                out_op = OpTuple(symbol, qn, factor=factor[non_red_one_col[i] - 1])
-                out_ops[-1].append(out_op)
-
-            new_table.append(np.array([len(out_ops) - 1] + list(term_col[col_idx]), dtype=np.uint16).reshape(1, -1))
-            new_factor.append(1.0)
-
-            # it is not necessary to remove the column nonzero elements
-            # non_red[:, col_idx] = 0
-            # non_red.eliminate_zeros()
-
-        # reconstruct the table in new operator
-        table = np.concatenate(new_table)
-        # check the number of incoming operators could be represent as np.uint16
-        assert len(out_ops) <= np.iinfo(np.uint16).max
-        factor = np.concatenate(new_factor, axis=None)
-
-        assert len(table) == len(factor)
-
-        # debug
-        # logger.debug(f"in_ops: {in_ops}")
-        # logger.debug(f"out_ops: {out_ops}")
-        # logger.debug(f"new_factor: {new_factor}")
-
-        in_ops = out_ops
-        # in_ops_full_symbol = out_ops_full_symbol
-        out_ops_list.append(out_ops)
-
-    return out_ops_list
-
-
-def add_idx(symbol, idx):
-    symbols = symbol.split(" ")
-    for i in range(len(symbols)):
-        symbols[i] = symbols[i] + f"_{idx}"
-    return " ".join(symbols)
-
-
-def _terms_to_table(model: Model, terms: List[Op], const: float):
-    r"""
-    constructing a general operator table
-    according to model.model and model.order
-    """
-
-    table = []
-    factor_list = []
-    
-    dummy_table_entry = []
-    for b in model.basis:
-        if b.multi_dof:
-            dof = b.dof[0]
-        else:
-            dof = b.dof
-        op = Op.identity(dof, qn_size=model.qn_size)
-        dummy_table_entry.append(op)
-    for op in terms:
-        elem_ops, factor = op.split_elementary(model.dof_to_siteidx)
-        table_entry = dummy_table_entry.copy()
-        for elem_op in elem_ops:
-            # it is ensured in `elem_op` every symbol is on the same site
-            site_idx = model.dof_to_siteidx[elem_op.dofs[0]]
-            table_entry[site_idx] = elem_op
-        table.append(table_entry)
-        factor_list.append(factor)
-
-    # const
-    if const != 0:
-        table_entry = dummy_table_entry.copy()
-        factor_list.append(const)
-        table.append(table_entry)
-
-    factor_list = np.array(factor_list)
-    logger.debug(f"# of operator terms: {len(table)}")
-
-    return table, factor_list
-
-
-# translate the numbers into symbolic Matrix Operator
-def compose_symbolic_mo(in_ops, out_ops, primary_ops):
-    mo = [[[] for o in range(len(out_ops))] for i in range(len(in_ops))]
-    for iop, out_op in enumerate(out_ops):
-        for composed_op in out_op:
-            in_idx = composed_op.symbol[0]
-            op = primary_ops[composed_op.symbol[1]]
-            mo[in_idx][iop].append(composed_op.factor * op)
-    return mo
-
-
-# translate symbolic Matrix Operator to numerical matrix operator defined with certain basis
-def symbolic_mo_to_numeric_mo(basis, mo, dtype):
-    pdim = basis.nbas
-    nrow, ncol = len(mo), len(mo[0])
-    mo_mat = np.zeros((nrow, pdim, pdim, ncol), dtype=dtype)
-
-    for irow, icol in itertools.product(range(nrow), range(ncol)):
-        for term in mo[irow][icol]:
-            mo_mat[irow, :, :, icol] += basis.op_mat(term)
-    return mo_mat
-
-
-def _format_symbolic_mpo(symbolic_mpo):
-    # debug tool. Used in the comment of Mpo.__init__
-
-    # helper function
-    def format_op(op: Op):
-        op_str = op.symbol
-        op_str = op_str.replace(r"^\dagger", "†")
-        if op.factor != 1:
-            op_str = f"{op.factor:.1e} * " + op_str
-        return op_str
-
-    result_str_list = []
-    # print the MPO sites one by one
-    for mo in symbolic_mpo:
-        # firstly convert the site into an array of strings
-        mo_str_array = np.full((len(mo), len(mo[0])), None)
-        for irol, row in enumerate(mo):
-            for icol, terms in enumerate(row):
-                if len(terms) == 0:
-                    terms_str = "0"
-                else:
-                    terms_str = " + ".join(format_op(op) for op in terms)
-                mo_str_array[irol][icol] = terms_str
-        # array of element length
-        mo_str_length = np.vectorize(lambda x: len(x))(mo_str_array)
-        max_length_per_col = mo_str_length.max(axis=0)
-        # format each line
-        lines = []
-        for row in mo_str_array:
-            terms_with_space = [term + " " * (max_length_per_col[icol] - len(term)) for icol, term in enumerate(row)]
-            row_str = "   ".join(terms_with_space)
-            lines.append("│ " + row_str + " │")
-        # make it prettier
-        if len(lines) != 1:
-            lines[0] = "┏" + lines[0][1:-1] + "┓"
-            lines[-1] = "┗" + lines[-1][1:-1] + "┛"
-        # str of a single mo
-        result_str_list.append("\n".join(lines))
-    return "\n".join(result_str_list)
-
-
-##############################################################################################
-# symbolic MPO swapping algorithm
-
-
-ExpandedOp = namedtuple("ExpandedOp", ["factor", "out_ops1_idx", "site1_op_idx", "site2_op_idx"])
-
-
-def multiply_out_op_sum_list_by_out_op(l1: List, out_op: OpTuple):
-    res = []
-    for op_in_sum_list in l1:
-        term = ExpandedOp(
-            op_in_sum_list.factor * out_op.factor,
-            op_in_sum_list.symbol[0], op_in_sum_list.symbol[1], out_op.symbol[1]
-        )
-        res.append(term)
-    return res
-
-
-def expand_out_op_sum_list(out_ops1: List, l2: List):
-    res = []
-    for out_op in l2:
-        out_op_sum_list1 = out_ops1[out_op.symbol[0]]
-        res.extend(multiply_out_op_sum_list_by_out_op(out_op_sum_list1, out_op))
-    return res
-
-
-def check_swap_consistency(new_out_ops2, new_out_ops3, out_ops3_expanded):
-    # check consistency
-    new_out_ops3_expanded: List[List[ExpandedOp]] = []
-    for out_op_sum_list in new_out_ops3:
-        new_out_ops3_expanded.append(expand_out_op_sum_list(new_out_ops2, out_op_sum_list))
-    # item ordering: out_ops1, site1, site2, factor. (site indices are before swapping)
-    # put the float-point factor to the last position for robust sorting
-    swapped_new_out_ops3_expanded: List[List[Tuple]] = []
-    for out_op_sum_list in new_out_ops3_expanded:
-        swapped_new_out_ops3_expanded.append([])
-        for op in out_op_sum_list:
-            swapped_new_out_ops3_expanded[-1].append((op.out_ops1_idx, op.site2_op_idx, op.site1_op_idx, op.factor))
-        swapped_new_out_ops3_expanded[-1].sort()
-
-    swapped_out_ops3_expanded: List[List[Tuple]] = []
-    for out_op_sum_list in out_ops3_expanded:
-        swapped_out_ops3_expanded.append([])
-        for op in out_op_sum_list:
-            swapped_out_ops3_expanded[-1].append((op.out_ops1_idx, op.site1_op_idx, op.site2_op_idx, op.factor))
-        swapped_out_ops3_expanded[-1].sort()
-
-    # the following check ensures that the swapping logic is correct
-    # so avoid using `assert` which will be disabled when the python optimization flag is set
-    error_msg = "Swapping failed. Please open a GitHub issue and report the bug."
-    for row1, row2 in zip(swapped_out_ops3_expanded, swapped_new_out_ops3_expanded):
-        if not len(row1) == len(row2):
-            raise RuntimeError(error_msg)
-        assert sorted(row1) == row1
-        assert sorted(row2) == row2
-        for op1, op2 in zip(sorted(row1), sorted(row2)):
-            if  op1[:-1] != op2[:-1]:
-                raise RuntimeError(error_msg)
-            if not np.allclose(op1[-1], op2[-1], rtol=1e-8, atol=1e-11):
-                raise RuntimeError(error_msg)
-
-
-def table_row_swapped_jw(row, primary_ops: List, op2idx: Dict):
-    assert len(row) == 5
-    assert row[-1] == 0
-    # mapping rule
-    # a1 -> a1 z2, a1^d -> a1^d z2
-    # a2 -> z1 a2, a2^d -> z1 a2^d
-    op1: Op = primary_ops[row[1]]
-    op2: Op = primary_ops[row[2]]
-
-    # remember: all possible operators: I Z + -
-    # new sigma_z produced for dof1 by op2
-    op1_new_sigma_z = (op1.split_symbol.count("sigma_+") + op1.split_symbol.count("sigma_-")) % 2
-    # similar except by op2
-    op2_new_sigma_z = (op2.split_symbol.count("sigma_+") + op2.split_symbol.count("sigma_-")) % 2
-    # determine the coefficient
-    op1_n_sigma_plus = op1.split_symbol.count("sigma_+")
-    op1_n_sigma_minus = op1.split_symbol.count("sigma_-")
-    assert op1_n_sigma_plus in [0, 1]
-    assert op1_n_sigma_minus in [0, 1]
-    n_permutes = op2_new_sigma_z * (op1_n_sigma_plus + op1_n_sigma_minus)
-    coeff = (-1) ** n_permutes
-    # cancel sigma_z as much as possible
-    def prepend_sigma_z(op: Op):
-        symbol_list = op.split_symbol
-        if symbol_list[0] == "I":
-            assert len(symbol_list) == 1
-            new_op = Op("sigma_z", op.dofs[0], qn=0)
-        elif symbol_list[0] == "sigma_z":
-            if len(symbol_list) == 1:
-                new_op = Op.identity(op.dofs[0])
-            else:
-                new_op = Op(" ".join(symbol_list[1:]), op.dofs[1:], qn=op.qn_list[1:])
-        elif symbol_list[0] == "sigma_+" or symbol_list[0] == "sigma_-":
-            new_op = Op("sigma_z " + op.symbol, [op.dofs[0]] + op.dofs, qn=[0] + op.qn_list)
-        else:
-            assert False
-        return new_op
-    if op1_new_sigma_z:
-        new_op2 = prepend_sigma_z(op2)
-    else:
-        new_op2 = op2
-    if op2_new_sigma_z:
-        new_op1 = prepend_sigma_z(op1)
-    else:
-        new_op1 = op1
-
-    if new_op1 not in op2idx:
-        op2idx[new_op1] = len(primary_ops)
-        primary_ops.append(new_op1)
-    if new_op2 not in op2idx:
-        op2idx[new_op2] = len(primary_ops)
-        primary_ops.append(new_op2)
-
-    return [row[0], op2idx[new_op1], op2idx[new_op2], row[3], row[4]], coeff
-
-
-def table_and_factor_swapped_jw(table, factor, primary_ops: List):
-    # modifies primary_ops in place !!
-    new_table = []
-    new_factor = []
-    op2idx = {op: i for i, op in enumerate(primary_ops)}
-    for row, factor_row in zip(table, factor):
-        new_row, coeff = table_row_swapped_jw(row, primary_ops, op2idx)
-        new_table.append(new_row)
-        new_factor.append(coeff * factor_row)
-    return np.array(new_table), np.array(new_factor)
-
-
-def swap_site(out_ops_list, primary_ops: List, swap_jw: bool):
-    # the MPO at hand is - # - # -
-    # the bond indices are 1, 2, 3 and the site indices are 1 and 2
-    # the operators at each of the bond
-    out_ops1, out_ops2, out_ops3 = out_ops_list
-
-    # the expanded sum-of-product form of the operator represented by the two site MPO
-    # i.e. the expanded form of out_ops3
-    # the number of items is equal to the index of bond 3
-    # each item [factor, out_ops[1]idx, primary_ops @ site 1, primary_ops @ site 2]
-    out_ops3_expanded: List[List[ExpandedOp]] = []
-    for out_op_sum_list in out_ops3:
-        out_ops3_expanded.append(expand_out_op_sum_list(out_ops2, out_op_sum_list))
-        # lots of del in the following code. The purposes are
-        # 1. to indicate the variables are local
-        # 2. to help avoid mis-using these variables in the following code (by typo etc.)
-        del out_op_sum_list
-    table = []
-    factor = []
-    # to be extended after primary_ops, used to label each bond for out_ops3
-    auxiliary_dummy_primary_ops = []
-    DummyOp = namedtuple("DummyOp", ["qn"])
-    for out_ops3_sum_list in out_ops3:
-        auxiliary_dummy_primary_ops.append(DummyOp(-out_ops3_sum_list[0].qn))
-    n_primary_ops = len(primary_ops)
-
-    if not swap_jw:
-        # modify primary_ops in place can be avoided
-        primary_ops = primary_ops.copy()
-        primary_ops.extend(auxiliary_dummy_primary_ops)
-
-    for i, out_ops3_sum_list in enumerate(out_ops3_expanded):
-        for op in out_ops3_sum_list:
-            # swap the sites and add two more columns at the end
-            row = [op.out_ops1_idx, op.site2_op_idx, op.site1_op_idx, n_primary_ops + i, 0]
-            table.append(row)
-            factor.append(op.factor)
-            del op, row
-    table = np.array(table)
-    factor = np.array(factor)
-
-    if swap_jw:
-        # modifies primary_ops in place !!
-        table, factor = table_and_factor_swapped_jw(table, factor, primary_ops)
-        table[:, 3] = table[:, 3] + (len(primary_ops) - n_primary_ops)
-        n_primary_ops = len(primary_ops)
-        primary_ops = primary_ops.copy()
-        primary_ops.extend(auxiliary_dummy_primary_ops)
-
-    new_out_ops = _construct_symbolic_mpo(table, out_ops1, factor, primary_ops)
-    assert len(new_out_ops) == 4
-    new_out_ops1, new_out_ops2, new_out_ops3_unsorted = new_out_ops[:3]
-
-    # sort the out operators
-    new_out_ops3 = [None] * len(new_out_ops3_unsorted)
-    assert len(new_out_ops3) == len(primary_ops) - n_primary_ops == len(auxiliary_dummy_primary_ops)
-    assert len(new_out_ops[-1]) == 1
-    for dummy_op in new_out_ops[-1][0]:
-        idx1, idx2 = dummy_op.symbol
-        idx2 -= n_primary_ops
-        new_out_ops3[idx2] = new_out_ops3_unsorted[idx1]
-        if dummy_op.factor != 1:
-            for i, op in enumerate(new_out_ops3[idx2]):
-                new_out_ops3[idx2][i] = OpTuple(symbol=op.symbol, qn=op.qn, factor=op.factor * dummy_op.factor)
-        del dummy_op, idx1, idx2
-    assert None not in new_out_ops3
-
-    if not swap_jw:
-        # if swap_jw == True, it's bound to fail
-        check_swap_consistency(new_out_ops2, new_out_ops3, out_ops3_expanded)
-
-    mo1 = compose_symbolic_mo(out_ops1, new_out_ops2, primary_ops)
-    mo2 = compose_symbolic_mo(new_out_ops2, new_out_ops3, primary_ops)
-    # print(_format_symbolic_mpo([mo1, mo2]))
-    qn = [opsum[0].qn for opsum in new_out_ops2]
-    return new_out_ops2, new_out_ops3, mo1, mo2, qn
+# -*- coding: utf-8 -*-
+import logging
+import itertools
+from collections import namedtuple
+from typing import List, Set, Tuple, Dict
+
+import numpy as np
+import scipy
+import scipy.sparse
+
+from renormalizer.model import Model
+from renormalizer.model.op import Op
+from renormalizer.lib import bipartite_vertex_cover
+
+logger = logging.getLogger(__name__)
+
+# The `Op` class is transformed to a light-weight named tuple
+# for better performance
+OpTuple = namedtuple("OpTuple", ["symbol", "qn", "factor"])
+
+
+def construct_symbolic_mpo(table, factor, algo="Hopcroft-Karp"):
+    r"""
+    A General Compact (Symbolic) MPO Construction Routine
+
+    Args:
+
+    table: an operator table with shape (operator nterm, nsite). Each entry contains elementary operators on each site.
+    factor (np.ndarray): one prefactor vector (dim: operator nterm)
+    algo: the algorithm used to select local ops, "Hopcroft-Karp"(default), "Hungarian".
+          They are both global optimal and have only minor performance difference.
+
+    Note:
+    op with the same op.symbol must have the same op.qn and op.factor
+
+    Return:
+    mpo: symbolic mpo
+    mpoqn: quantum number
+    qntot: total quantum number of the operator
+    qnidx: the index of the qn
+
+    The idea:
+
+    the index of the primary ops {0:"I", 1:"a", 2:r"a^\dagger"}
+
+    for example: H = 2.0 * a_1 a_2^dagger   + 3.0 * a_2^\dagger a_3 + 4.0*a_0^\dagger a_3
+    The column names are the site indices with 0 and 4 imaginary (see the note below)
+    and the content of the table is the index of primary operators.
+                        s0   s1   s2   s3  s4  factor
+    a_1 a_2^dagger      0    1    2    0   0   2.0
+    a_2^\dagger a_3     0    0    2    1   0   3.0
+    a_1^\dagger a_3     0    2    0    1   0   4.0
+    for convenience the first and last column mean that the operator of the left and right hand of the system is I
+
+    cut the string to construct the row(left) and column(right) operator and find the duplicated/independent terms
+                        s0   s1 |  s2   s3  s4 factor
+    a_1 a_2^dagger      0    1  |  2    0   0  2.0
+    a_2^\dagger a_3     0    0  |  2    1   0  3.0
+    a_1^\dagger a_3     0    2  |  0    1   0  4.0
+
+     The content of the table below means matrix elements with basis explained in the notes.
+     In the matrix elements, 1 means combination and 0 means no combination.
+          (2,0,0) (2,1,0) (0,1,0)  -> right side of the above table
+     (0,1)   1       0       0
+     (0,0)   0       1       0
+     (0,2)   0       0       1
+       |
+       v
+     left side of the above table
+     In this case all operators are independent so the content of the matrix is diagonal
+
+    and select the terms and rearrange the table
+    The selection rule is to find the minimal number of rows+cols that can eliminate the
+    matrix
+                      s1   s2 |  s3 s4 factor
+    a_1 a_2^dagger    0'   2  |  0  0  2.0
+    a_2^\dagger a_3   1'   2  |  1  0  3.0
+    a_1^\dagger a_3   2'   0  |  1  0  4.0
+    0'/1'/2' are three new operators(could be non-elementary)
+    The local mpo is the transformation matrix between 0,0,0 to 0',1',2'.
+    In this case, the local mpo is simply (1, 0, 2)
+
+    cut the string and find the duplicated/independent terms
+            (0,0), (1,0)
+     (0',2)   1      0
+     (1',2)   0      1
+     (2',0)   0      1
+
+    and select the terms and rearrange the table
+    apparently choose the (1,0) column and construct the complementary operator (1',2)+(2',0) is better
+    0'' =  3.0 * (1', 2) + 4.0 * (2', 0)
+                                                 s2     s3 | s4 factor
+    (4.0 * a_1^dagger + 3.0 * a_2^dagger) a_3    0''    1  | 0  1.0
+    a_1 a_2^dagger                               1''    0  | 0  2.0
+    0''/1'' are another two new operators(non-elementary)
+    The local mpo is the transformation matrix between 0',1',2' to 0'',1''
+
+             (0)
+     (0'',1)  1
+     (1'',0)  1
+
+    The local mpo is the transformation matrix between 0'',1'' to 0'''
+    """
+
+    qn_size = len(table[0][0].qn)
+    # Simplest case. Cut to the chase
+    if len(table) == 1:
+        # The first layer: number of sites. The 2nd and 3rd layer: in and out virtual bond
+        # the 4th layer: operator sums
+        mpo: List[List[List[List[[Op]]]]] = []
+        mpoqn = [np.zeros((1, qn_size), dtype=int)]
+        primary_ops = list(set(table[0]))
+        op2idx = dict(zip(primary_ops, range(len(primary_ops))))
+        out_ops_list: List[List[OpTuple]] = [[OpTuple([0], qn=0, factor=1)]]
+        for op in table[0]:
+            mpo.append([[[op]]])
+            qn = mpoqn[-1][0] + op.qn
+            mpoqn.append(np.array([qn]))
+            out_ops_list.append([OpTuple([0, op2idx[op]], qn=qn, factor=1)])
+
+        mpo[-1][0][0][0] = factor[0] * mpo[-1][0][0][0]
+        last_optuple = out_ops_list[-1][0]
+        out_ops_list[-1][0] = OpTuple(last_optuple.symbol, qn=last_optuple.qn, factor=factor[0]*last_optuple.factor)
+        qntot = qn
+        mpoqn[-1] = np.zeros((1, qn_size), dtype=int)
+        qnidx = len(mpo) - 1
+        # the last two terms are not set for fast construction of the operators
+        return mpo, mpoqn, qntot, qnidx, out_ops_list, primary_ops
+
+    # use np.uint32, np.uint16 to save memory
+    max_uint32 = np.iinfo(np.uint32).max
+    max_uint16 = np.iinfo(np.uint16).max
+
+    logger.debug(f"symbolic mpo algorithm: {algo}")
+    logger.debug(f"Input operator terms: {len(table)}")
+
+    # translate the symbolic operator table to an easy to manipulate numpy array
+    table = np.array(table)
+    # unique operators with DoF names taken into consideration
+    # The inclusion of DoF names is necessary for multi-dof basis.
+    unique_op: Set[Op] = set(table.ravel())
+
+    # check the index of different operators could be represented with np.uint16
+    assert len(unique_op) < max_uint16
+
+    # Construct mapping from easy-to-manipulate integer to actual Op
+    primary_ops = list(unique_op)
+
+    op2idx = dict(zip(unique_op, range(len(unique_op))))
+    new_table = np.vectorize(op2idx.get)(table).astype(np.uint16)
+
+    del unique_op
+
+    if __debug__:
+        qn_table = np.array([[x.qn for x in ta] for ta in table])
+        factor_table = np.array([[x.factor for x in ta] for ta in table])
+        for idx in range(len(primary_ops)):
+            coord = np.nonzero(new_table == idx)
+            # check that op with the same symbol has the same factor and qn
+            for j in range(qn_size):
+                assert np.unique(qn_table[:, :, j][coord]).size == 1
+            assert np.all(factor_table[coord] == factor_table[coord][0])
+
+        del factor_table, qn_table
+
+    # combine the same terms but with different factors(add them together)
+    unique_term, unique_inverse = np.unique(new_table, axis=0, return_inverse=True)
+    # it is efficient to vectorize the operation that moves the rows and cols
+    # and sum them together
+    coord = np.array([[newidx, oldidx] for oldidx, newidx in enumerate(unique_inverse)])
+    mask = scipy.sparse.csr_matrix((np.ones(len(coord)), (coord[:, 0], coord[:, 1])))
+    factor = mask.dot(factor)
+
+    # add the first and last column for convenience
+    ta = np.zeros((unique_term.shape[0], 1), dtype=np.uint16)
+    table = np.concatenate((ta, unique_term, ta), axis=1)
+    logger.debug(f"After combination of the same terms: {table.shape[0]}")
+    # check the index of interaction could be represented with np.uint32
+    assert table.shape[0] < max_uint32
+
+    del unique_term, unique_inverse
+
+    # 0 represents the identity symbol. Identity might not present
+    # in `primary_ops` but the algorithm still works.
+
+    in_ops = [[OpTuple([0], qn=np.zeros(qn_size, dtype=int), factor=1)]]
+
+    out_ops_list = _construct_symbolic_mpo(table, in_ops, factor, primary_ops, algo)
+    # number of sites + 1. Note that the table was expanded for convenience
+    assert len(out_ops_list) == len(table[0]) - 1
+    mpo = []
+    for i in range(len(out_ops_list)-1):
+        mo = compose_symbolic_mo(out_ops_list[i], out_ops_list[i+1], primary_ops)
+        mpo.append(mo)
+
+    mpoqn = []
+    for out_ops in out_ops_list:
+        qn = np.array([out_op[0].qn for out_op in out_ops])
+        mpoqn.append(qn)
+
+    qntot = mpoqn[-1][0]
+    mpoqn[-1] = np.zeros((1, qn_size), dtype=int)
+    qnidx = len(mpo) - 1
+
+    return mpo, mpoqn, qntot, qnidx, out_ops_list, primary_ops
+
+
+def _construct_symbolic_mpo(table, in_ops, factor, primary_ops, algo="Hopcroft-Karp"):
+
+    nsite = table.shape[1] - 2
+
+    out_ops_list = [in_ops]
+
+    for isite in range(nsite):
+        # split table into the row and col part
+        term_row, row_unique_inverse = np.unique(table[:, :2], axis=0, return_inverse=True)
+
+        # faster version of the following code
+        # term_col, col_unique_inverse = np.unique(table[:, 2:], axis=0, return_inverse=True)
+        term_col = {}
+        col_unique_inverse = []
+        for row in table[:, 2:]:
+            row_bytes = row.tobytes()
+            i_and_row = term_col.get(row_bytes)
+            if i_and_row is None:
+                i_and_row = (len(term_col), row)
+                term_col[row_bytes] = i_and_row
+            col_unique_inverse.append(i_and_row[0])
+        term_col = [v[1] for v in term_col.values()]
+
+        # get the non_redudant ops
+        # the +1 trick is to use the csr sparse matrix format
+        non_red = scipy.sparse.diags(np.arange(1, table.shape[0] + 1), format="csr", dtype=np.uint32)
+        coord = np.array([[newidx, oldidx] for oldidx, newidx in enumerate(row_unique_inverse)])
+        mask = scipy.sparse.csr_matrix((np.ones(len(coord), dtype=np.uint32), (coord[:, 0], coord[:, 1])))
+        non_red = mask.dot(non_red)
+        coord = np.array([[oldidx, newidx] for oldidx, newidx in enumerate(col_unique_inverse)])
+        mask = scipy.sparse.csr_matrix((np.ones(len(coord), dtype=np.uint32), (coord[:, 0], coord[:, 1])))
+        non_red = non_red.dot(mask)
+        # use sparse matrix to represent non_red will be inefficient a little
+        # bit compared to dense matrix, but saves a lot of memory when the
+        # number of terms is huge
+        # logger.info(f"isite: {isite}, bipartite graph size: {non_red.shape}")
+
+        # the usual case
+
+        bigraph = []
+        if non_red.shape[0] < non_red.shape[1]:
+            for i in range(non_red.shape[0]):
+                bigraph.append(non_red.indices[non_red.indptr[i]:non_red.indptr[i + 1]])
+            rowbool, colbool = bipartite_vertex_cover(bigraph, algo=algo)
+        else:
+            non_red_csc = non_red.tocsc()
+            for i in range(non_red.shape[1]):
+                bigraph.append(non_red_csc.indices[non_red_csc.indptr[i]:non_red_csc.indptr[i + 1]])
+            colbool, rowbool = bipartite_vertex_cover(bigraph, algo=algo)
+
+        row_select = np.nonzero(rowbool)[0]
+        # largest cover first
+        row_select = sorted(row_select, key=lambda i: non_red.indptr[i + 1] - non_red.indptr[i], reverse=True)
+        col_select = np.nonzero(colbool)[0]
+
+
+        if len(row_select) > 0:
+            assert np.amax(row_select) < non_red.shape[0]
+        if len(col_select) > 0:
+            assert np.amax(col_select) < non_red.shape[1]
+
+        # select the reserved ops
+        out_ops: List[List[OpTuple]] = []
+        new_table = []
+        new_factor = []
+
+        for row_idx in row_select:
+            # construct out_op
+            # dealing with row (left side of the table). One row corresponds to multiple cols.
+            # Produce one out operator and multiple new_table entries
+            symbol = term_row[row_idx]
+            qn = in_ops[symbol[0]][0].qn + primary_ops[symbol[1]].qn
+            out_op = OpTuple(symbol, qn, factor=1.0)
+            out_ops.append([out_op])
+
+            col_link = non_red.indices[non_red.indptr[row_idx]:non_red.indptr[row_idx + 1]]
+            stack = np.array([len(out_ops) - 1] * len(col_link), dtype=np.uint16).reshape(-1, 1)
+            new_table.append(np.hstack((stack, [term_col[i] for i in col_link])))
+            new_factor.append(factor[non_red[row_idx, col_link].toarray() - 1])
+            non_red.data[non_red.indptr[row_idx]:non_red.indptr[row_idx + 1]] = 0
+
+        non_red.eliminate_zeros()
+
+        nonzero_row_idx, nonzero_col_idx = non_red.nonzero()
+        for col_idx in col_select:
+
+            out_ops.append([])
+            # complementary operator
+            # dealing with column (right side of the table). One col correspond to multiple rows.
+            # Produce multiple out operators and one new_table entry
+            non_red_one_col = non_red[:, col_idx].toarray().flatten()
+            for i in nonzero_row_idx[np.nonzero(nonzero_col_idx == col_idx)[0]]:
+                symbol = term_row[i]
+                qn = in_ops[symbol[0]][0].qn + primary_ops[symbol[1]].qn
+                out_op = OpTuple(symbol, qn, factor=factor[non_red_one_col[i] - 1])
+                out_ops[-1].append(out_op)
+
+            new_table.append(np.array([len(out_ops) - 1] + list(term_col[col_idx]), dtype=np.uint16).reshape(1, -1))
+            new_factor.append(1.0)
+
+            # it is not necessary to remove the column nonzero elements
+            # non_red[:, col_idx] = 0
+            # non_red.eliminate_zeros()
+
+        # reconstruct the table in new operator
+        table = np.concatenate(new_table)
+        # check the number of incoming operators could be represent as np.uint16
+        assert len(out_ops) <= np.iinfo(np.uint16).max
+        factor = np.concatenate(new_factor, axis=None)
+
+        assert len(table) == len(factor)
+
+        # debug
+        # logger.debug(f"in_ops: {in_ops}")
+        # logger.debug(f"out_ops: {out_ops}")
+        # logger.debug(f"new_factor: {new_factor}")
+
+        in_ops = out_ops
+        # in_ops_full_symbol = out_ops_full_symbol
+        out_ops_list.append(out_ops)
+
+    return out_ops_list
+
+
+def add_idx(symbol, idx):
+    symbols = symbol.split(" ")
+    for i in range(len(symbols)):
+        symbols[i] = symbols[i] + f"_{idx}"
+    return " ".join(symbols)
+
+
+def _terms_to_table(model: Model, terms: List[Op], const: float):
+    r"""
+    constructing a general operator table
+    according to model.model and model.order
+    """
+
+    table = []
+    factor_list = []
+    
+    dummy_table_entry = []
+    for b in model.basis:
+        if b.multi_dof:
+            dof = b.dof[0]
+        else:
+            dof = b.dof
+        op = Op.identity(dof, qn_size=model.qn_size)
+        dummy_table_entry.append(op)
+    for op in terms:
+        elem_ops, factor = op.split_elementary(model.dof_to_siteidx)
+        table_entry = dummy_table_entry.copy()
+        for elem_op in elem_ops:
+            # it is ensured in `elem_op` every symbol is on the same site
+            site_idx = model.dof_to_siteidx[elem_op.dofs[0]]
+            table_entry[site_idx] = elem_op
+        table.append(table_entry)
+        factor_list.append(factor)
+
+    # const
+    if const != 0:
+        table_entry = dummy_table_entry.copy()
+        factor_list.append(const)
+        table.append(table_entry)
+
+    factor_list = np.array(factor_list)
+    logger.debug(f"# of operator terms: {len(table)}")
+
+    return table, factor_list
+
+
+# translate the numbers into symbolic Matrix Operator
+def compose_symbolic_mo(in_ops, out_ops, primary_ops):
+    mo = [[[] for o in range(len(out_ops))] for i in range(len(in_ops))]
+    for iop, out_op in enumerate(out_ops):
+        for composed_op in out_op:
+            in_idx = composed_op.symbol[0]
+            op = primary_ops[composed_op.symbol[1]]
+            mo[in_idx][iop].append(composed_op.factor * op)
+    return mo
+
+
+# translate symbolic Matrix Operator to numerical matrix operator defined with certain basis
+def symbolic_mo_to_numeric_mo(basis, mo, dtype):
+    pdim = basis.nbas
+    nrow, ncol = len(mo), len(mo[0])
+    mo_mat = np.zeros((nrow, pdim, pdim, ncol), dtype=dtype)
+
+    for irow, icol in itertools.product(range(nrow), range(ncol)):
+        for term in mo[irow][icol]:
+            mo_mat[irow, :, :, icol] += basis.op_mat(term)
+    return mo_mat
+
+
+def _format_symbolic_mpo(symbolic_mpo):
+    # debug tool. Used in the comment of Mpo.__init__
+
+    # helper function
+    def format_op(op: Op):
+        op_str = op.symbol
+        op_str = op_str.replace(r"^\dagger", "†")
+        if op.factor != 1:
+            op_str = f"{op.factor:.1e} * " + op_str
+        return op_str
+
+    result_str_list = []
+    # print the MPO sites one by one
+    for mo in symbolic_mpo:
+        # firstly convert the site into an array of strings
+        mo_str_array = np.full((len(mo), len(mo[0])), None)
+        for irol, row in enumerate(mo):
+            for icol, terms in enumerate(row):
+                if len(terms) == 0:
+                    terms_str = "0"
+                else:
+                    terms_str = " + ".join(format_op(op) for op in terms)
+                mo_str_array[irol][icol] = terms_str
+        # array of element length
+        mo_str_length = np.vectorize(lambda x: len(x))(mo_str_array)
+        max_length_per_col = mo_str_length.max(axis=0)
+        # format each line
+        lines = []
+        for row in mo_str_array:
+            terms_with_space = [term + " " * (max_length_per_col[icol] - len(term)) for icol, term in enumerate(row)]
+            row_str = "   ".join(terms_with_space)
+            lines.append("│ " + row_str + " │")
+        # make it prettier
+        if len(lines) != 1:
+            lines[0] = "┏" + lines[0][1:-1] + "┓"
+            lines[-1] = "┗" + lines[-1][1:-1] + "┛"
+        # str of a single mo
+        result_str_list.append("\n".join(lines))
+    return "\n".join(result_str_list)
+
+
+##############################################################################################
+# symbolic MPO swapping algorithm
+
+
+ExpandedOp = namedtuple("ExpandedOp", ["factor", "out_ops1_idx", "site1_op_idx", "site2_op_idx"])
+
+
+def multiply_out_op_sum_list_by_out_op(l1: List, out_op: OpTuple):
+    res = []
+    for op_in_sum_list in l1:
+        term = ExpandedOp(
+            op_in_sum_list.factor * out_op.factor,
+            op_in_sum_list.symbol[0], op_in_sum_list.symbol[1], out_op.symbol[1]
+        )
+        res.append(term)
+    return res
+
+
+def expand_out_op_sum_list(out_ops1: List, l2: List):
+    res = []
+    for out_op in l2:
+        out_op_sum_list1 = out_ops1[out_op.symbol[0]]
+        res.extend(multiply_out_op_sum_list_by_out_op(out_op_sum_list1, out_op))
+    return res
+
+
+def check_swap_consistency(new_out_ops2, new_out_ops3, out_ops3_expanded):
+    # check consistency
+    new_out_ops3_expanded: List[List[ExpandedOp]] = []
+    for out_op_sum_list in new_out_ops3:
+        new_out_ops3_expanded.append(expand_out_op_sum_list(new_out_ops2, out_op_sum_list))
+    # item ordering: out_ops1, site1, site2, factor. (site indices are before swapping)
+    # put the float-point factor to the last position for robust sorting
+    swapped_new_out_ops3_expanded: List[List[Tuple]] = []
+    for out_op_sum_list in new_out_ops3_expanded:
+        swapped_new_out_ops3_expanded.append([])
+        for op in out_op_sum_list:
+            swapped_new_out_ops3_expanded[-1].append((op.out_ops1_idx, op.site2_op_idx, op.site1_op_idx, op.factor))
+        swapped_new_out_ops3_expanded[-1].sort()
+
+    swapped_out_ops3_expanded: List[List[Tuple]] = []
+    for out_op_sum_list in out_ops3_expanded:
+        swapped_out_ops3_expanded.append([])
+        for op in out_op_sum_list:
+            swapped_out_ops3_expanded[-1].append((op.out_ops1_idx, op.site1_op_idx, op.site2_op_idx, op.factor))
+        swapped_out_ops3_expanded[-1].sort()
+
+    # the following check ensures that the swapping logic is correct
+    # so avoid using `assert` which will be disabled when the python optimization flag is set
+    error_msg = "Swapping failed. Please open a GitHub issue and report the bug."
+    for row1, row2 in zip(swapped_out_ops3_expanded, swapped_new_out_ops3_expanded):
+        if not len(row1) == len(row2):
+            raise RuntimeError(error_msg)
+        assert sorted(row1) == row1
+        assert sorted(row2) == row2
+        for op1, op2 in zip(sorted(row1), sorted(row2)):
+            if  op1[:-1] != op2[:-1]:
+                raise RuntimeError(error_msg)
+            if not np.allclose(op1[-1], op2[-1], rtol=1e-8, atol=1e-11):
+                raise RuntimeError(error_msg)
+
+
+def table_row_swapped_jw(row, primary_ops: List, op2idx: Dict):
+    assert len(row) == 5
+    assert row[-1] == 0
+    # mapping rule
+    # a1 -> a1 z2, a1^d -> a1^d z2
+    # a2 -> z1 a2, a2^d -> z1 a2^d
+    op1: Op = primary_ops[row[1]]
+    op2: Op = primary_ops[row[2]]
+
+    # remember: all possible operators: I Z + -
+    # new sigma_z produced for dof1 by op2
+    op1_new_sigma_z = (op1.split_symbol.count("sigma_+") + op1.split_symbol.count("sigma_-")) % 2
+    # similar except by op2
+    op2_new_sigma_z = (op2.split_symbol.count("sigma_+") + op2.split_symbol.count("sigma_-")) % 2
+    # determine the coefficient
+    op1_n_sigma_plus = op1.split_symbol.count("sigma_+")
+    op1_n_sigma_minus = op1.split_symbol.count("sigma_-")
+    assert op1_n_sigma_plus in [0, 1]
+    assert op1_n_sigma_minus in [0, 1]
+    n_permutes = op2_new_sigma_z * (op1_n_sigma_plus + op1_n_sigma_minus)
+    coeff = (-1) ** n_permutes
+    # cancel sigma_z as much as possible
+    def prepend_sigma_z(op: Op):
+        symbol_list = op.split_symbol
+        if symbol_list[0] == "I":
+            assert len(symbol_list) == 1
+            new_op = Op("sigma_z", op.dofs[0], qn=0)
+        elif symbol_list[0] == "sigma_z":
+            if len(symbol_list) == 1:
+                new_op = Op.identity(op.dofs[0])
+            else:
+                new_op = Op(" ".join(symbol_list[1:]), op.dofs[1:], qn=op.qn_list[1:])
+        elif symbol_list[0] == "sigma_+" or symbol_list[0] == "sigma_-":
+            new_op = Op("sigma_z " + op.symbol, [op.dofs[0]] + op.dofs, qn=[0] + op.qn_list)
+        else:
+            assert False
+        return new_op
+    if op1_new_sigma_z:
+        new_op2 = prepend_sigma_z(op2)
+    else:
+        new_op2 = op2
+    if op2_new_sigma_z:
+        new_op1 = prepend_sigma_z(op1)
+    else:
+        new_op1 = op1
+
+    if new_op1 not in op2idx:
+        op2idx[new_op1] = len(primary_ops)
+        primary_ops.append(new_op1)
+    if new_op2 not in op2idx:
+        op2idx[new_op2] = len(primary_ops)
+        primary_ops.append(new_op2)
+
+    return [row[0], op2idx[new_op1], op2idx[new_op2], row[3], row[4]], coeff
+
+
+def table_and_factor_swapped_jw(table, factor, primary_ops: List):
+    # modifies primary_ops in place !!
+    new_table = []
+    new_factor = []
+    op2idx = {op: i for i, op in enumerate(primary_ops)}
+    for row, factor_row in zip(table, factor):
+        new_row, coeff = table_row_swapped_jw(row, primary_ops, op2idx)
+        new_table.append(new_row)
+        new_factor.append(coeff * factor_row)
+    return np.array(new_table), np.array(new_factor)
+
+
+def swap_site(out_ops_list, primary_ops: List, swap_jw: bool):
+    # the MPO at hand is - # - # -
+    # the bond indices are 1, 2, 3 and the site indices are 1 and 2
+    # the operators at each of the bond
+    out_ops1, out_ops2, out_ops3 = out_ops_list
+
+    # the expanded sum-of-product form of the operator represented by the two site MPO
+    # i.e. the expanded form of out_ops3
+    # the number of items is equal to the index of bond 3
+    # each item [factor, out_ops[1]idx, primary_ops @ site 1, primary_ops @ site 2]
+    out_ops3_expanded: List[List[ExpandedOp]] = []
+    for out_op_sum_list in out_ops3:
+        out_ops3_expanded.append(expand_out_op_sum_list(out_ops2, out_op_sum_list))
+        # lots of del in the following code. The purposes are
+        # 1. to indicate the variables are local
+        # 2. to help avoid mis-using these variables in the following code (by typo etc.)
+        del out_op_sum_list
+    table = []
+    factor = []
+    # to be extended after primary_ops, used to label each bond for out_ops3
+    auxiliary_dummy_primary_ops = []
+    DummyOp = namedtuple("DummyOp", ["qn"])
+    for out_ops3_sum_list in out_ops3:
+        auxiliary_dummy_primary_ops.append(DummyOp(-out_ops3_sum_list[0].qn))
+    n_primary_ops = len(primary_ops)
+
+    if not swap_jw:
+        # modify primary_ops in place can be avoided
+        primary_ops = primary_ops.copy()
+        primary_ops.extend(auxiliary_dummy_primary_ops)
+
+    for i, out_ops3_sum_list in enumerate(out_ops3_expanded):
+        for op in out_ops3_sum_list:
+            # swap the sites and add two more columns at the end
+            row = [op.out_ops1_idx, op.site2_op_idx, op.site1_op_idx, n_primary_ops + i, 0]
+            table.append(row)
+            factor.append(op.factor)
+            del op, row
+    table = np.array(table)
+    factor = np.array(factor)
+
+    if swap_jw:
+        # modifies primary_ops in place !!
+        table, factor = table_and_factor_swapped_jw(table, factor, primary_ops)
+        table[:, 3] = table[:, 3] + (len(primary_ops) - n_primary_ops)
+        n_primary_ops = len(primary_ops)
+        primary_ops = primary_ops.copy()
+        primary_ops.extend(auxiliary_dummy_primary_ops)
+
+    new_out_ops = _construct_symbolic_mpo(table, out_ops1, factor, primary_ops)
+    assert len(new_out_ops) == 4
+    new_out_ops1, new_out_ops2, new_out_ops3_unsorted = new_out_ops[:3]
+
+    # sort the out operators
+    new_out_ops3 = [None] * len(new_out_ops3_unsorted)
+    assert len(new_out_ops3) == len(primary_ops) - n_primary_ops == len(auxiliary_dummy_primary_ops)
+    assert len(new_out_ops[-1]) == 1
+    for dummy_op in new_out_ops[-1][0]:
+        idx1, idx2 = dummy_op.symbol
+        idx2 -= n_primary_ops
+        new_out_ops3[idx2] = new_out_ops3_unsorted[idx1]
+        if dummy_op.factor != 1:
+            for i, op in enumerate(new_out_ops3[idx2]):
+                new_out_ops3[idx2][i] = OpTuple(symbol=op.symbol, qn=op.qn, factor=op.factor * dummy_op.factor)
+        del dummy_op, idx1, idx2
+    assert None not in new_out_ops3
+
+    if not swap_jw:
+        # if swap_jw == True, it's bound to fail
+        check_swap_consistency(new_out_ops2, new_out_ops3, out_ops3_expanded)
+
+    mo1 = compose_symbolic_mo(out_ops1, new_out_ops2, primary_ops)
+    mo2 = compose_symbolic_mo(new_out_ops2, new_out_ops3, primary_ops)
+    # print(_format_symbolic_mpo([mo1, mo2]))
+    qn = [opsum[0].qn for opsum in new_out_ops2]
+    return new_out_ops2, new_out_ops3, mo1, mo2, qn
```

### Comparing `renormalizer-0.0.8/renormalizer/mps/tda.py` & `renormalizer-0.0.9/renormalizer/mps/tda.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_elementop.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_elementop.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_evolve.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_evolve.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_gs.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_gs.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_mp.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_mp.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-# -*- coding: utf-8 -*-
-
-import os
-
-import numpy as np
-import pytest
-
-from renormalizer.mps import Mps, Mpo, MpDm
-from renormalizer.mps.matrix import tensordot, asnumpy
-from renormalizer.mps.lib import Environ
-from renormalizer.tests.parameter import custom_model, holstein_model
-from renormalizer.utils import CompressCriteria
-
-def test_save_load():
-    model = holstein_model
-    mps = Mpo.onsite(model, r"a^\dagger", dof_set={0}) @ Mps.ground_state(model, False)
-    mpo = Mpo(model)
-    mps1 = mps.copy()
-    for i in range(2):
-        mps1 = mps1.evolve(mpo, 10)
-    mps2 = mps.evolve(mpo, 10)
-    fname = "test.npz"
-    mps2.dump(fname)
-    mps2 = Mps.load(model, fname)
-    mps2 = mps2.evolve(mpo, 10)
-    assert np.allclose(mps1.e_occupations, mps2.e_occupations)
-    os.remove(fname)
-
-
-def check_distance(a: Mps, b: Mps):
-    d1 = (a - b).mp_norm
-    d2 = a.distance(b)
-    a_array = a.todense()
-    b_array = b.todense()
-    d3 = np.linalg.norm(a_array - b_array)
-    assert d1 == pytest.approx(d2) == pytest.approx(d3)
-
-
-def test_distance():
-    model = custom_model(n_phys_dim=(2, 2))
-    a = Mps.random(model, 1, 10)
-    b = Mps.random(model, 1, 10)
-    check_distance(a, b)
-    h = Mpo(model)
-    for i in range(100):
-        a = a.evolve(h, 10)
-        b = b.evolve(h, 10)
-        check_distance(a, b)
-
-
-def test_environ():
-    mps = Mps.random(holstein_model, 1, 10)
-    mpo = Mpo(holstein_model)
-    mps = mps.evolve(mpo, 10)
-    environ = Environ(mps, mpo)
-    for i in range(len(mps)-1):
-        l = environ.read("L", i)
-        r = environ.read("R", i+1)
-        e = complex(tensordot(l, r, axes=((0, 1, 2), (0, 1, 2)))).real
-        assert pytest.approx(e) == mps.expectation(mpo)
-
-# multi_mpo routine for single mpo calculation
-@pytest.mark.parametrize("mpdm", (True, False))
-def test_environ_multi_mpo(mpdm):
-    mps = Mps.random(holstein_model, 1, 10)
-    if mpdm:
-        mps = MpDm.from_mps(mps)
-    mpo = Mpo(holstein_model)
-    mps = mps.evolve(mpo, 10)
-    environ = Environ(mps, mpo)
-    environ_multi_mpo = Environ(mps, [mpo])
-    for i in range(len(mps)-1):
-        l = environ.read("L", i)
-        r = environ.read("R", i+1)
-        l2 = environ_multi_mpo.read("L", i)
-        r2 = environ_multi_mpo.read("R", i+1) 
-        assert np.allclose(asnumpy(l), asnumpy(l2))
-        assert np.allclose(asnumpy(r), asnumpy(r2))
-
-@pytest.mark.parametrize("comp", (True, False))
-@pytest.mark.parametrize("mp", (
-        "mps",
-        "mpdm",
-        "mpo",
-))
-def test_svd_compress(comp, mp):
-    
-    if mp == "mpo":
-        mps = Mpo(holstein_model)
-        M = 22
-    else:
-        mps = Mps.random(holstein_model, 1, 10)
-        if mp == "mpdm":
-            mps = MpDm.from_mps(mps)
-        mps.canonicalise().normalize("mps_only")
-        M = 36
-    if comp:
-        mps = mps.to_complex(inplace=True)
-    print(f"{mps}")
-    
-    mpo = Mpo(holstein_model)
-    if comp:
-        mpo = mpo.scale(-1.0j)
-    print(f"{mpo.bond_dims}")
-    
-    std_mps = mpo.apply(mps, canonicalise=True).canonicalise()
-    print(f"std_mps: {std_mps}")
-    mps.compress_config.bond_dim_max_value = M
-    mps.compress_config.criteria = CompressCriteria.fixed
-    svd_mps = mpo.contract(mps)
-    dis = svd_mps.distance(std_mps)/std_mps.mp_norm
-    print(f"svd_mps: {svd_mps}, dis: {dis}")
-    assert np.allclose(dis, 0.0, atol=1e-3)
-    assert np.allclose(svd_mps.mp_norm, std_mps.mp_norm, atol=1e-4)
-    
-    
-@pytest.mark.parametrize("comp", (True, False))
-@pytest.mark.parametrize("mp", ("mps", "mpdm", "mpo" ))
-def test_variational_compress(comp, mp):
-    
-    if mp == "mpo":
-        mps = Mpo(holstein_model)
-        M = 20
-    else:
-        mps = Mps.random(holstein_model, 1, 10)
-        if mp == "mpdm":
-            mps = MpDm.from_mps(mps)
-        mps.canonicalise().normalize("mps_only")
-        M = 36
-    if comp:
-        mps = mps.to_complex(inplace=True)
-    print(f"{mps}")
-    
-    mpo = Mpo(holstein_model)
-    if comp:
-        mpo = mpo.scale(-1.0j)
-    print(f"{mpo.bond_dims}")
-    
-    std_mps = mpo.apply(mps, canonicalise=True).canonicalise()
-    print(f"std_mps: {std_mps}")
-    
-    # 2site algorithm
-    mps.compress_config.vprocedure = [[M,1.0],[M,0.2],[M,0.1]]+[[M,0],]*10
-    mps.compress_config.vmethod = "2site"
-    var_mps = mps.variational_compress(mpo, guess=None)
-    dis = var_mps.distance(std_mps)/std_mps.mp_norm
-    print(f"var2_mps: {var_mps}, dis: {dis}")
-    assert np.allclose(dis, 0.0, atol=1e-4)
-    assert np.allclose(var_mps.mp_norm, std_mps.mp_norm, atol=1e-4)
-    
-    # 1site algorithm with 2site result as a guess
-    # 1site algorithm is easy to be trapped in a local minimum
-    var_mps.compress_config.vprocedure = [[M,0],]*10
-    var_mps.compress_config.vmethod = "1site"
-    var_mps = mps.variational_compress(mpo, guess=var_mps)
-    dis = var_mps.distance(std_mps)/std_mps.mp_norm
-    print(f"var1_mps: {var_mps}, dis: {dis}")
-    assert np.allclose(dis, 0.0, atol=1e-4)
-    assert np.allclose(var_mps.mp_norm, std_mps.mp_norm, atol=1e-4)
+# -*- coding: utf-8 -*-
+
+import os
+
+import numpy as np
+import pytest
+
+from renormalizer.mps import Mps, Mpo, MpDm
+from renormalizer.mps.matrix import tensordot, asnumpy
+from renormalizer.mps.lib import Environ
+from renormalizer.tests.parameter import custom_model, holstein_model
+from renormalizer.utils import CompressCriteria
+
+def test_save_load():
+    model = holstein_model
+    mps = Mpo.onsite(model, r"a^\dagger", dof_set={0}) @ Mps.ground_state(model, False)
+    mpo = Mpo(model)
+    mps1 = mps.copy()
+    for i in range(2):
+        mps1 = mps1.evolve(mpo, 10)
+    mps2 = mps.evolve(mpo, 10)
+    fname = "test.npz"
+    mps2.dump(fname)
+    mps2 = Mps.load(model, fname)
+    mps2 = mps2.evolve(mpo, 10)
+    assert np.allclose(mps1.e_occupations, mps2.e_occupations)
+    os.remove(fname)
+
+
+def check_distance(a: Mps, b: Mps):
+    d1 = (a - b).mp_norm
+    d2 = a.distance(b)
+    a_array = a.todense()
+    b_array = b.todense()
+    d3 = np.linalg.norm(a_array - b_array)
+    assert d1 == pytest.approx(d2) == pytest.approx(d3)
+
+
+def test_distance():
+    model = custom_model(n_phys_dim=(2, 2))
+    a = Mps.random(model, 1, 10)
+    b = Mps.random(model, 1, 10)
+    check_distance(a, b)
+    h = Mpo(model)
+    for i in range(100):
+        a = a.evolve(h, 10)
+        b = b.evolve(h, 10)
+        check_distance(a, b)
+
+
+def test_environ():
+    mps = Mps.random(holstein_model, 1, 10)
+    mpo = Mpo(holstein_model)
+    mps = mps.evolve(mpo, 10)
+    environ = Environ(mps, mpo)
+    for i in range(len(mps)-1):
+        l = environ.read("L", i)
+        r = environ.read("R", i+1)
+        e = complex(tensordot(l, r, axes=((0, 1, 2), (0, 1, 2)))).real
+        assert pytest.approx(e) == mps.expectation(mpo)
+
+# multi_mpo routine for single mpo calculation
+@pytest.mark.parametrize("mpdm", (True, False))
+def test_environ_multi_mpo(mpdm):
+    mps = Mps.random(holstein_model, 1, 10)
+    if mpdm:
+        mps = MpDm.from_mps(mps)
+    mpo = Mpo(holstein_model)
+    mps = mps.evolve(mpo, 10)
+    environ = Environ(mps, mpo)
+    environ_multi_mpo = Environ(mps, [mpo])
+    for i in range(len(mps)-1):
+        l = environ.read("L", i)
+        r = environ.read("R", i+1)
+        l2 = environ_multi_mpo.read("L", i)
+        r2 = environ_multi_mpo.read("R", i+1) 
+        assert np.allclose(asnumpy(l), asnumpy(l2))
+        assert np.allclose(asnumpy(r), asnumpy(r2))
+
+@pytest.mark.parametrize("comp", (True, False))
+@pytest.mark.parametrize("mp", (
+        "mps",
+        "mpdm",
+        "mpo",
+))
+def test_svd_compress(comp, mp):
+    
+    if mp == "mpo":
+        mps = Mpo(holstein_model)
+        M = 22
+    else:
+        mps = Mps.random(holstein_model, 1, 10)
+        if mp == "mpdm":
+            mps = MpDm.from_mps(mps)
+        mps.canonicalise().normalize("mps_only")
+        M = 36
+    if comp:
+        mps = mps.to_complex(inplace=True)
+    print(f"{mps}")
+    
+    mpo = Mpo(holstein_model)
+    if comp:
+        mpo = mpo.scale(-1.0j)
+    print(f"{mpo.bond_dims}")
+    
+    std_mps = mpo.apply(mps, canonicalise=True).canonicalise()
+    print(f"std_mps: {std_mps}")
+    mps.compress_config.bond_dim_max_value = M
+    mps.compress_config.criteria = CompressCriteria.fixed
+    svd_mps = mpo.contract(mps)
+    dis = svd_mps.distance(std_mps)/std_mps.mp_norm
+    print(f"svd_mps: {svd_mps}, dis: {dis}")
+    assert np.allclose(dis, 0.0, atol=1e-3)
+    assert np.allclose(svd_mps.mp_norm, std_mps.mp_norm, atol=1e-4)
+    
+    
+@pytest.mark.parametrize("comp", (True, False))
+@pytest.mark.parametrize("mp", ("mps", "mpdm", "mpo" ))
+def test_variational_compress(comp, mp):
+    
+    if mp == "mpo":
+        mps = Mpo(holstein_model)
+        M = 20
+    else:
+        mps = Mps.random(holstein_model, 1, 10)
+        if mp == "mpdm":
+            mps = MpDm.from_mps(mps)
+        mps.canonicalise().normalize("mps_only")
+        M = 36
+    if comp:
+        mps = mps.to_complex(inplace=True)
+    print(f"{mps}")
+    
+    mpo = Mpo(holstein_model)
+    if comp:
+        mpo = mpo.scale(-1.0j)
+    print(f"{mpo.bond_dims}")
+    
+    std_mps = mpo.apply(mps, canonicalise=True).canonicalise()
+    print(f"std_mps: {std_mps}")
+    
+    # 2site algorithm
+    mps.compress_config.vprocedure = [[M,1.0],[M,0.2],[M,0.1]]+[[M,0],]*10
+    mps.compress_config.vmethod = "2site"
+    var_mps = mps.variational_compress(mpo, guess=None)
+    dis = var_mps.distance(std_mps)/std_mps.mp_norm
+    print(f"var2_mps: {var_mps}, dis: {dis}")
+    assert np.allclose(dis, 0.0, atol=1e-4)
+    assert np.allclose(var_mps.mp_norm, std_mps.mp_norm, atol=1e-4)
+    
+    # 1site algorithm with 2site result as a guess
+    # 1site algorithm is easy to be trapped in a local minimum
+    var_mps.compress_config.vprocedure = [[M,0],]*10
+    var_mps.compress_config.vmethod = "1site"
+    var_mps = mps.variational_compress(mpo, guess=var_mps)
+    dis = var_mps.distance(std_mps)/std_mps.mp_norm
+    print(f"var1_mps: {var_mps}, dis: {dis}")
+    assert np.allclose(dis, 0.0, atol=1e-4)
+    assert np.allclose(var_mps.mp_norm, std_mps.mp_norm, atol=1e-4)
```

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_mpdm.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_mpdm.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_mpo.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_mpo.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_mpproperty.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_mpproperty.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_mps.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_mps.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_sbm.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_sbm.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-# -*- coding: utf-8 -*-
-
-import numpy as np
-import qutip
-
-from renormalizer.model import Phonon, SpinBosonModel
-from renormalizer.mps import Mps, Mpo, MpDm, ThermalProp
-from renormalizer.utils import Quantity, CompressConfig, EvolveConfig
-from renormalizer.model.op import Op
-
-
-def get_model():
-    nphonons = 5
-    ph_levels = 2
-
-    epsilon = 1
-    delta = 1
-
-    ph_list = [Phonon.simple_phonon(Quantity(1), Quantity(1), ph_levels)] * nphonons
-    return SpinBosonModel(Quantity(epsilon), Quantity(delta), ph_list)
-
-def test_zt():
-    model = get_model()
-
-    mps = Mps.ground_state(model, False)
-    mps.compress_config = CompressConfig(threshold=1e-6)
-    mps.evolve_config = EvolveConfig(adaptive=True, guess_dt=0.1)
-    mpo = Mpo(model)
-    time_series = [0]
-    spin = [1]
-    sigma_z_oper = Mpo(model, Op("sigma_z", "spin"))
-    for i in range(30):
-        dt = mps.evolve_config.guess_dt
-        mps = mps.evolve(mpo, evolve_dt=dt)
-        time_series.append(time_series[-1] + dt)
-        spin.append(mps.expectation(sigma_z_oper))
-    qutip_res = get_qutip_zt(model, time_series)
-    assert np.allclose(qutip_res, spin, atol=1e-3)
-
-
-def test_ft():
-    model = get_model()
-    mpo = Mpo(model)
-    impdm = MpDm.max_entangled_gs(model)
-    impdm.compress_config = CompressConfig(threshold=1e-6)
-    temperature = Quantity(3)
-    evolve_config = EvolveConfig(adaptive=True, guess_dt=-0.001j)
-    tp = ThermalProp(impdm, evolve_config=evolve_config)
-    tp.evolve(nsteps=1, evolve_time=temperature.to_beta() / 2j)
-    mpdm = tp.latest_mps
-    mpdm = Mpo(model, Op("sigma_x", "spin")).contract(mpdm)
-    mpdm.evolve_config = EvolveConfig(adaptive=True, guess_dt=0.1)
-    time_series = [0]
-    sigma_z_oper = Mpo(model, Op("sigma_z", "spin"))
-    spin = [mpdm.expectation(sigma_z_oper)]
-    for i in range(29):
-        dt = mpdm.evolve_config.guess_dt
-        mpdm = mpdm.evolve(mpo, evolve_dt=dt)
-        time_series.append(time_series[-1] + dt)
-        spin.append(mpdm.expectation(sigma_z_oper))
-    qutip_res = get_qutip_ft(model, temperature, time_series)
-    assert np.allclose(qutip_res, spin, atol=1e-3)
-
-
-def get_qutip_operator(model):
-    blist = []
-    for i, ph1 in enumerate(model.ph_list):
-        basis = [qutip.identity(2)]
-        for j, ph2 in enumerate(model.ph_list):
-            if j == i:
-                state = qutip.destroy(ph1.n_phys_dim)
-            else:
-                state = qutip.identity(ph2.n_phys_dim)
-            basis.append(state)
-        blist.append(qutip.tensor(basis))
-
-    ph_iden = [qutip.identity(ph.n_phys_dim) for ph in model.ph_list]
-
-    sigma_x = qutip.tensor([qutip.sigmax()] + ph_iden)
-    sigma_z = qutip.tensor([qutip.sigmaz()] + ph_iden)
-    terms = [model.delta * sigma_x, model.epsilon * sigma_z]
-    for i, ph in enumerate(model.ph_list):
-        g = ph.coupling_constant
-        terms.append(ph.omega[0] * blist[i].dag() * blist[i])
-        terms.append(ph.omega[0] * g * sigma_z * (blist[i].dag() + blist[i]))
-    H = sum(terms)
-
-    return H, sigma_x, sigma_z
-
-
-def get_qutip_zt(model, time_series):
-    H, _, sigma_z = get_qutip_operator(model)
-    init_state = qutip.tensor([qutip.basis(2)] + [qutip.basis(ph.n_phys_dim) for ph in model.ph_list])
-    result = qutip.mesolve(H, init_state, time_series, e_ops=[sigma_z])
-    return result.expect[0]
-
-
-def get_qutip_ft(model, temperature, time_series):
-    H, sigma_x, sigma_z = get_qutip_operator(model)
-    init_state =  sigma_x * (-temperature.to_beta() * H).expm().unit() * sigma_x.dag()
-    result = qutip.mesolve(H, init_state, time_series, e_ops=[sigma_z])
-    return result.expect[0]
+# -*- coding: utf-8 -*-
+
+import numpy as np
+import qutip
+
+from renormalizer.model import Phonon, SpinBosonModel
+from renormalizer.mps import Mps, Mpo, MpDm, ThermalProp
+from renormalizer.utils import Quantity, CompressConfig, EvolveConfig
+from renormalizer.model.op import Op
+
+
+def get_model():
+    nphonons = 5
+    ph_levels = 2
+
+    epsilon = 1
+    delta = 1
+
+    ph_list = [Phonon.simple_phonon(Quantity(1), Quantity(1), ph_levels)] * nphonons
+    return SpinBosonModel(Quantity(epsilon), Quantity(delta), ph_list)
+
+def test_zt():
+    model = get_model()
+
+    mps = Mps.ground_state(model, False)
+    mps.compress_config = CompressConfig(threshold=1e-6)
+    mps.evolve_config = EvolveConfig(adaptive=True, guess_dt=0.1)
+    mpo = Mpo(model)
+    time_series = [0]
+    spin = [1]
+    sigma_z_oper = Mpo(model, Op("sigma_z", "spin"))
+    for i in range(30):
+        dt = mps.evolve_config.guess_dt
+        mps = mps.evolve(mpo, evolve_dt=dt)
+        time_series.append(time_series[-1] + dt)
+        spin.append(mps.expectation(sigma_z_oper))
+    qutip_res = get_qutip_zt(model, time_series)
+    assert np.allclose(qutip_res, spin, atol=1e-3)
+
+
+def test_ft():
+    model = get_model()
+    mpo = Mpo(model)
+    impdm = MpDm.max_entangled_gs(model)
+    impdm.compress_config = CompressConfig(threshold=1e-6)
+    temperature = Quantity(3)
+    evolve_config = EvolveConfig(adaptive=True, guess_dt=-0.001j)
+    tp = ThermalProp(impdm, evolve_config=evolve_config)
+    tp.evolve(nsteps=1, evolve_time=temperature.to_beta() / 2j)
+    mpdm = tp.latest_mps
+    mpdm = Mpo(model, Op("sigma_x", "spin")).contract(mpdm)
+    mpdm.evolve_config = EvolveConfig(adaptive=True, guess_dt=0.1)
+    time_series = [0]
+    sigma_z_oper = Mpo(model, Op("sigma_z", "spin"))
+    spin = [mpdm.expectation(sigma_z_oper)]
+    for i in range(29):
+        dt = mpdm.evolve_config.guess_dt
+        mpdm = mpdm.evolve(mpo, evolve_dt=dt)
+        time_series.append(time_series[-1] + dt)
+        spin.append(mpdm.expectation(sigma_z_oper))
+    qutip_res = get_qutip_ft(model, temperature, time_series)
+    assert np.allclose(qutip_res, spin, atol=1e-3)
+
+
+def get_qutip_operator(model):
+    blist = []
+    for i, ph1 in enumerate(model.ph_list):
+        basis = [qutip.identity(2)]
+        for j, ph2 in enumerate(model.ph_list):
+            if j == i:
+                state = qutip.destroy(ph1.n_phys_dim)
+            else:
+                state = qutip.identity(ph2.n_phys_dim)
+            basis.append(state)
+        blist.append(qutip.tensor(basis))
+
+    ph_iden = [qutip.identity(ph.n_phys_dim) for ph in model.ph_list]
+
+    sigma_x = qutip.tensor([qutip.sigmax()] + ph_iden)
+    sigma_z = qutip.tensor([qutip.sigmaz()] + ph_iden)
+    terms = [model.delta * sigma_x, model.epsilon * sigma_z]
+    for i, ph in enumerate(model.ph_list):
+        g = ph.coupling_constant
+        terms.append(ph.omega[0] * blist[i].dag() * blist[i])
+        terms.append(ph.omega[0] * g * sigma_z * (blist[i].dag() + blist[i]))
+    H = sum(terms)
+
+    return H, sigma_x, sigma_z
+
+
+def get_qutip_zt(model, time_series):
+    H, _, sigma_z = get_qutip_operator(model)
+    init_state = qutip.tensor([qutip.basis(2)] + [qutip.basis(ph.n_phys_dim) for ph in model.ph_list])
+    result = qutip.mesolve(H, init_state, time_series, e_ops=[sigma_z])
+    return result.expect[0]
+
+
+def get_qutip_ft(model, temperature, time_series):
+    H, sigma_x, sigma_z = get_qutip_operator(model)
+    init_state =  sigma_x * (-temperature.to_beta() * H).expm().unit() * sigma_x.dag()
+    result = qutip.mesolve(H, init_state, time_series, e_ops=[sigma_z])
+    return result.expect[0]
```

### Comparing `renormalizer-0.0.8/renormalizer/mps/tests/test_tda.py` & `renormalizer-0.0.9/renormalizer/mps/tests/test_tda.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/mps/thermalprop.py` & `renormalizer-0.0.9/renormalizer/mps/thermalprop.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-import logging
-
-import numpy as np
-
-from renormalizer.model import Model
-from renormalizer.mps import MpDm, Mpo
-from renormalizer.utils import TdMpsJob, Quantity, EvolveConfig
-from renormalizer.property import Property
-
-logger = logging.getLogger(__name__)
-
-
-class ThermalProp(TdMpsJob):
-    r"""
-    Thermally Propagate initial matrix product density operator (:class:`~renormalizer.mps.MpDm`) in imaginary time.
-
-    Args:
-        init_mpdm (:class:`~renormalizer.mps.MpDm`): the initial density matrix to be propagated. Usually identity.
-        h_mpo_model (:class:`~renormalizer.model.model.Model`): Model for the system Hamiltonian.
-            Default is the same with ``init_mpdm.model``.
-        exact (bool): whether propagate assuming Hamiltonian is local
-            :math:`\hat H = \sum_i \hat H_i = \sum_{in} \omega_{in} b^\dagger_{in} b_{in}` and
-            exact propagation is possible through :math:`e^{xH} = e^{xh_1}e^{xh_2} \cdots e^{xh_n}`.
-            If set to ``True``, properties such as occupations are not calculated during
-            time evolution for better efficiency.
-        space (str): the space of exact propagation. Possible options are ``"GS"`` or ``"EX"``.
-            If set to ``"GS"``, then the exact propagation is performed in zero exciton space.
-            If set to ``"EX"``, then the exact propagation is performed in one exciton space,
-            i.e. the vibrations are regarded as displaced oscillators.
-        evolve_config (:class:`~renormalizer.utils.EvolveConfig`): config when evolving the MpDm in imaginary time.
-        dump_mps (str): if dump mps when dumping, "all", "one", None; Default to None
-        dump_dir (str): the directory for logging and numerical result output.
-        job_name (str): the name of the calculation job which determines the file name of the logging and numerical result output.
-        properties (:class:`~renormalizer.property.Property`) calculate other properties with interface in Property
-    """
-    def __init__(
-        self,
-        init_mpdm: MpDm,
-        h_mpo_model: Model = None,
-        exact: bool = False,
-        space: str = "GS",
-        evolve_config: EvolveConfig = None,
-        dump_mps: bool = None, 
-        dump_dir: str = None,
-        job_name: str = None,
-        properties: Property = None,
-        auto_expand: bool = True,
-    ):
-        self.init_mpdm: MpDm = init_mpdm.canonicalise()
-        if h_mpo_model is None:
-            h_mpo_model = self.init_mpdm.model
-        self.h_mpo = Mpo(h_mpo_model)
-        logger.info(f"Bond dim of h_mpo: {self.h_mpo.bond_dims}")
-        self.exact = exact
-        assert space in ["GS", "EX"]
-        self.space = space
-        self.energies = []
-        self._e_occupations_array = []
-        self._ph_occupations_array = []
-        self._vn_entropy_array = []
-        self.properties = properties
-        self.auto_expand = auto_expand
-
-        super().__init__(evolve_config=evolve_config, dump_mps=dump_mps, dump_dir=dump_dir,
-                job_name=job_name)
-
-    def init_mps(self):
-        self.init_mpdm.evolve_config = self.evolve_config
-        if self.evolve_config.is_tdvp and self.auto_expand:
-            self.init_mpdm = self.init_mpdm.expand_bond_dimension(self.h_mpo)
-        return self.init_mpdm
-
-    def process_mps(self, mps):
-        new_energy = mps.expectation(self.h_mpo)
-        self.energies.append(new_energy)
-        if self.exact:
-            # skip the fuss for efficiency
-            return
-        for attr_str in ["e_occupations", "ph_occupations"]:
-            attr = getattr(mps, attr_str)
-            logger.info(f"{attr_str}: {attr}")
-            self_array = getattr(self, f"_{attr_str}_array")
-            self_array.append(attr)
-        vn_entropy = mps.calc_bond_entropy()
-        self._vn_entropy_array.append(vn_entropy)
-        logger.info(f"vn entropy: {vn_entropy}")
-        logger.info(
-            f"Energy: {new_energy}, total electron: {self._e_occupations_array[-1].sum()}"
-        )
-        
-        # calculate other properties defined in Property
-        if self.properties is not None:
-            self.properties.calc_properties(mps)
-
-    def evolve_exact(self, old_mpdm: MpDm, evolve_dt):
-        MPOprop = Mpo.exact_propagator(
-            old_mpdm.model, evolve_dt.imag, space=self.space, shift=-self.energies[-1]
-        )
-        new_mpdm = MPOprop.apply(old_mpdm, canonicalise=True)
-        # partition function can't be obtained. It's not practical anyway.
-        # The function is too large to be fit into float64 even float128
-        new_mpdm.normalize("mps_and_coeff")
-        return new_mpdm
-
-    def evolve_prop(self, old_mpdm, evolve_dt):
-        h_mpo = Mpo(self.h_mpo.model, offset=Quantity(self.energies[-1]))
-        return old_mpdm.evolve(h_mpo, evolve_dt)
-
-    def evolve_single_step(self, evolve_dt):
-        old_mpdm = self.latest_mps
-        if self.exact:
-            new_mpdm = self.evolve_exact(old_mpdm, evolve_dt)
-        else:
-            new_mpdm = self.evolve_prop(old_mpdm, evolve_dt)
-        return new_mpdm
-
-    def evolve(self, evolve_dt=None, nsteps=None, evolve_time=None):
-        if evolve_dt is not None:
-            assert np.iscomplex(evolve_dt) and evolve_dt.imag < 0
-        if evolve_time is not None:
-            assert np.iscomplex(evolve_time) and evolve_time.imag < 0
-        super().evolve(evolve_dt, nsteps, evolve_time)
-
-    @property
-    def e_occupations_array(self):
-        return np.array(self._e_occupations_array)
-
-    @property
-    def ph_occupations_array(self):
-        return np.array(self._ph_occupations_array)
-
-    @property
-    def vn_entropy_array(self):
-        return np.array(self._vn_entropy_array)
-
-    def get_dump_dict(self):
-        dump_dict = dict()
-        dump_dict["time series"] = [-t.imag for t in self.evolve_times]
-        dump_dict["energies"] = self.energies
-        dump_dict["electron occupations array"] = self.e_occupations_array.tolist()
-        dump_dict["phonon occupations array"] = self.ph_occupations_array.tolist()
-        dump_dict["vn entropy array"] = self.vn_entropy_array.tolist()
-        
-        if self.properties is not None:
-            for prop_str in self.properties.prop_res.keys():
-                dump_dict[prop_str] = self.properties.prop_res[prop_str]
-
-        return dump_dict
-
-
-def load_thermal_state(model, path: str):
-    """
-    Load thermal propagated state from disk. Return None if the file is not found.
-
-    Args:
-        model (:class:`MolList`): system information
-        path (str): the path to load thermal state from. Should be an numpy ``.npz`` file.
-    Returns: Loaded MpDm
-    """
-    try:
-        logger.info(f"Try load from {path}")
-        mpdm = MpDm.load(model, path)
-        logger.info(f"Init mpdm loaded: {mpdm}")
-    except FileNotFoundError:
-        logger.info(f"No file found in {path}")
-        mpdm = None
-
-    return mpdm
+import logging
+
+import numpy as np
+
+from renormalizer.model import Model
+from renormalizer.mps import MpDm, Mpo
+from renormalizer.utils import TdMpsJob, Quantity, EvolveConfig
+from renormalizer.property import Property
+
+logger = logging.getLogger(__name__)
+
+
+class ThermalProp(TdMpsJob):
+    r"""
+    Thermally Propagate initial matrix product density operator (:class:`~renormalizer.mps.MpDm`) in imaginary time.
+
+    Args:
+        init_mpdm (:class:`~renormalizer.mps.MpDm`): the initial density matrix to be propagated. Usually identity.
+        h_mpo_model (:class:`~renormalizer.model.model.Model`): Model for the system Hamiltonian.
+            Default is the same with ``init_mpdm.model``.
+        exact (bool): whether propagate assuming Hamiltonian is local
+            :math:`\hat H = \sum_i \hat H_i = \sum_{in} \omega_{in} b^\dagger_{in} b_{in}` and
+            exact propagation is possible through :math:`e^{xH} = e^{xh_1}e^{xh_2} \cdots e^{xh_n}`.
+            If set to ``True``, properties such as occupations are not calculated during
+            time evolution for better efficiency.
+        space (str): the space of exact propagation. Possible options are ``"GS"`` or ``"EX"``.
+            If set to ``"GS"``, then the exact propagation is performed in zero exciton space.
+            If set to ``"EX"``, then the exact propagation is performed in one exciton space,
+            i.e. the vibrations are regarded as displaced oscillators.
+        evolve_config (:class:`~renormalizer.utils.EvolveConfig`): config when evolving the MpDm in imaginary time.
+        dump_mps (str): if dump mps when dumping, "all", "one", None; Default to None
+        dump_dir (str): the directory for logging and numerical result output.
+        job_name (str): the name of the calculation job which determines the file name of the logging and numerical result output.
+        properties (:class:`~renormalizer.property.Property`) calculate other properties with interface in Property
+    """
+    def __init__(
+        self,
+        init_mpdm: MpDm,
+        h_mpo_model: Model = None,
+        exact: bool = False,
+        space: str = "GS",
+        evolve_config: EvolveConfig = None,
+        dump_mps: bool = None, 
+        dump_dir: str = None,
+        job_name: str = None,
+        properties: Property = None,
+        auto_expand: bool = True,
+    ):
+        self.init_mpdm: MpDm = init_mpdm.canonicalise()
+        if h_mpo_model is None:
+            h_mpo_model = self.init_mpdm.model
+        self.h_mpo = Mpo(h_mpo_model)
+        logger.info(f"Bond dim of h_mpo: {self.h_mpo.bond_dims}")
+        self.exact = exact
+        assert space in ["GS", "EX"]
+        self.space = space
+        self.energies = []
+        self._e_occupations_array = []
+        self._ph_occupations_array = []
+        self._vn_entropy_array = []
+        self.properties = properties
+        self.auto_expand = auto_expand
+
+        super().__init__(evolve_config=evolve_config, dump_mps=dump_mps, dump_dir=dump_dir,
+                job_name=job_name)
+
+    def init_mps(self):
+        self.init_mpdm.evolve_config = self.evolve_config
+        if self.evolve_config.is_tdvp and self.auto_expand:
+            self.init_mpdm = self.init_mpdm.expand_bond_dimension(self.h_mpo)
+        return self.init_mpdm
+
+    def process_mps(self, mps):
+        new_energy = mps.expectation(self.h_mpo)
+        self.energies.append(new_energy)
+        if self.exact:
+            # skip the fuss for efficiency
+            return
+        for attr_str in ["e_occupations", "ph_occupations"]:
+            attr = getattr(mps, attr_str)
+            logger.info(f"{attr_str}: {attr}")
+            self_array = getattr(self, f"_{attr_str}_array")
+            self_array.append(attr)
+        vn_entropy = mps.calc_bond_entropy()
+        self._vn_entropy_array.append(vn_entropy)
+        logger.info(f"vn entropy: {vn_entropy}")
+        logger.info(
+            f"Energy: {new_energy}, total electron: {self._e_occupations_array[-1].sum()}"
+        )
+        
+        # calculate other properties defined in Property
+        if self.properties is not None:
+            self.properties.calc_properties(mps)
+
+    def evolve_exact(self, old_mpdm: MpDm, evolve_dt):
+        MPOprop = Mpo.exact_propagator(
+            old_mpdm.model, evolve_dt.imag, space=self.space, shift=-self.energies[-1]
+        )
+        new_mpdm = MPOprop.apply(old_mpdm, canonicalise=True)
+        # partition function can't be obtained. It's not practical anyway.
+        # The function is too large to be fit into float64 even float128
+        new_mpdm.normalize("mps_and_coeff")
+        return new_mpdm
+
+    def evolve_prop(self, old_mpdm, evolve_dt):
+        h_mpo = Mpo(self.h_mpo.model, offset=Quantity(self.energies[-1]))
+        return old_mpdm.evolve(h_mpo, evolve_dt)
+
+    def evolve_single_step(self, evolve_dt):
+        old_mpdm = self.latest_mps
+        if self.exact:
+            new_mpdm = self.evolve_exact(old_mpdm, evolve_dt)
+        else:
+            new_mpdm = self.evolve_prop(old_mpdm, evolve_dt)
+        return new_mpdm
+
+    def evolve(self, evolve_dt=None, nsteps=None, evolve_time=None):
+        if evolve_dt is not None:
+            assert np.iscomplex(evolve_dt) and evolve_dt.imag < 0
+        if evolve_time is not None:
+            assert np.iscomplex(evolve_time) and evolve_time.imag < 0
+        super().evolve(evolve_dt, nsteps, evolve_time)
+
+    @property
+    def e_occupations_array(self):
+        return np.array(self._e_occupations_array)
+
+    @property
+    def ph_occupations_array(self):
+        return np.array(self._ph_occupations_array)
+
+    @property
+    def vn_entropy_array(self):
+        return np.array(self._vn_entropy_array)
+
+    def get_dump_dict(self):
+        dump_dict = dict()
+        dump_dict["time series"] = [-t.imag for t in self.evolve_times]
+        dump_dict["energies"] = self.energies
+        dump_dict["electron occupations array"] = self.e_occupations_array.tolist()
+        dump_dict["phonon occupations array"] = self.ph_occupations_array.tolist()
+        dump_dict["vn entropy array"] = self.vn_entropy_array.tolist()
+        
+        if self.properties is not None:
+            for prop_str in self.properties.prop_res.keys():
+                dump_dict[prop_str] = self.properties.prop_res[prop_str]
+
+        return dump_dict
+
+
+def load_thermal_state(model, path: str):
+    """
+    Load thermal propagated state from disk. Return None if the file is not found.
+
+    Args:
+        model (:class:`MolList`): system information
+        path (str): the path to load thermal state from. Should be an numpy ``.npz`` file.
+    Returns: Loaded MpDm
+    """
+    try:
+        logger.info(f"Try load from {path}")
+        mpdm = MpDm.load(model, path)
+        logger.info(f"Init mpdm loaded: {mpdm}")
+    except FileNotFoundError:
+        logger.info(f"No file found in {path}")
+        mpdm = None
+
+    return mpdm
```

### Comparing `renormalizer-0.0.8/renormalizer/property/ops.py` & `renormalizer-0.0.9/renormalizer/property/ops.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/property/property.py` & `renormalizer-0.0.9/renormalizer/property/property.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/sbm/lib.py` & `renormalizer-0.0.9/renormalizer/sbm/lib.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/sbm/sbm.py` & `renormalizer-0.0.9/renormalizer/sbm/sbm.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# -*- coding: utf-8 -*-
-
-import logging
-from functools import partial
-
-from renormalizer.model import Model
-from renormalizer.mps import Mpo, Mps
-from renormalizer.utils import TdMpsJob, Quantity, CompressConfig
-import numpy as np
-
-logger = logging.getLogger(__name__)
-
-
-class SpinBosonDynamics(TdMpsJob):
-    
-    r"""
-    The Spin-Boson Model
-
-    The initial state is a Hartree product state with all vibrations at :math:`|
-    0 \rangle` and spin at spin up state. 
-    The class can be used at zero temperature or finite temperature with
-    thermofield dynamics method. 
-    
-    """
-
-    def __init__(self, 
-            model: Model, 
-            auto_expand: bool = True,
-            compress_config=None, 
-            evolve_config=None, 
-            dump_dir=None,
-            dump_mps=None, 
-            job_name=None
-            ):
-        self.model = model
-        self.h_mpo = Mpo(model)
-        self.auto_expand = auto_expand
-        
-        if compress_config is None:
-            self.compress_config = CompressConfig()
-        else:
-            self.compress_config = compress_config
-
-        self.sigma_x = []
-        self.sigma_z = []
-        self.rho = []
-        self.bond_entropy = []
-
-        super().__init__(evolve_config=evolve_config, dump_dir=dump_dir,
-                dump_mps=dump_mps, job_name=job_name)
-
-    def init_mps(self):
-        logger.debug(f"mpo bond and physical dimension: {self.h_mpo.bond_dims}, {self.h_mpo.pbond_list}")
-        init_mps = Mps.ground_state(self.model, False)
-        init_mps.compress_config = self.compress_config
-        init_mps.evolve_config = self.evolve_config
-        
-        if self.evolve_config.is_tdvp and self.auto_expand: 
-            init_mps = init_mps.expand_bond_dimension(self.h_mpo, coef=1e-16, include_ex=False)
-        return init_mps
-
-    def process_mps(self, mps):
-        for idx, bas in enumerate(self.model.basis):
-            if bas.is_spin:
-                break
-        rho = mps.calc_1site_rdm(idx=idx)[idx]
-        self.rho.append(rho)
-        
-        #sigma_z_mpo = self.model.get_mpos("sigma_z", partial(Mpo.onsite, opera="sigma_z", dof_set={"spin"}))
-        #sigma_z0 = mps.expectation(sigma_z_mpo)
-        #assert np.allclose(sigma_z0, rho[0,0]-rho[1,1])
-        self.sigma_z.append((rho[0,0]-rho[1,1]).real)
-        
-        #sigma_x_mpo = self.model.get_mpos("sigma_x", partial(Mpo.onsite, opera="sigma_x", dof_set={"spin"}))
-        #sigma_x0 = mps.expectation(sigma_x_mpo)
-        #assert np.allclose(sigma_x0, rho[0,1]+rho[1,0])
-        self.sigma_x.append((rho[0,1]+rho[1,0]).real)
-        logger.info(f"sigma_z: {self.sigma_z[-1]}. sigma_x: {self.sigma_x[-1]}")
-        
-        bond_entropy = mps.calc_entropy("bond")
-        self.bond_entropy.append(bond_entropy)
-
-    def evolve_single_step(self, evolve_dt):
-        return self.latest_mps.evolve(self.h_mpo, evolve_dt)
-
-    def get_dump_dict(self):
-        dump_dict = dict()
-        dump_dict["time series"] = self.evolve_times
-        dump_dict["sigma_x"] = self.sigma_x
-        dump_dict["sigma_z"] = self.sigma_z
-        dump_dict["rho"] = self.rho
-        dump_dict["bond_entropy"] = self.bond_entropy
-        return dump_dict
+# -*- coding: utf-8 -*-
+
+import logging
+from functools import partial
+
+from renormalizer.model import Model
+from renormalizer.mps import Mpo, Mps
+from renormalizer.utils import TdMpsJob, Quantity, CompressConfig
+import numpy as np
+
+logger = logging.getLogger(__name__)
+
+
+class SpinBosonDynamics(TdMpsJob):
+    
+    r"""
+    The Spin-Boson Model
+
+    The initial state is a Hartree product state with all vibrations at :math:`|
+    0 \rangle` and spin at spin up state. 
+    The class can be used at zero temperature or finite temperature with
+    thermofield dynamics method. 
+    
+    """
+
+    def __init__(self, 
+            model: Model, 
+            auto_expand: bool = True,
+            compress_config=None, 
+            evolve_config=None, 
+            dump_dir=None,
+            dump_mps=None, 
+            job_name=None
+            ):
+        self.model = model
+        self.h_mpo = Mpo(model)
+        self.auto_expand = auto_expand
+        
+        if compress_config is None:
+            self.compress_config = CompressConfig()
+        else:
+            self.compress_config = compress_config
+
+        self.sigma_x = []
+        self.sigma_z = []
+        self.rho = []
+        self.bond_entropy = []
+
+        super().__init__(evolve_config=evolve_config, dump_dir=dump_dir,
+                dump_mps=dump_mps, job_name=job_name)
+
+    def init_mps(self):
+        logger.debug(f"mpo bond and physical dimension: {self.h_mpo.bond_dims}, {self.h_mpo.pbond_list}")
+        init_mps = Mps.ground_state(self.model, False)
+        init_mps.compress_config = self.compress_config
+        init_mps.evolve_config = self.evolve_config
+        
+        if self.evolve_config.is_tdvp and self.auto_expand: 
+            init_mps = init_mps.expand_bond_dimension(self.h_mpo, coef=1e-16, include_ex=False)
+        return init_mps
+
+    def process_mps(self, mps):
+        for idx, bas in enumerate(self.model.basis):
+            if bas.is_spin:
+                break
+        rho = mps.calc_1site_rdm(idx=idx)[idx]
+        self.rho.append(rho)
+        
+        #sigma_z_mpo = self.model.get_mpos("sigma_z", partial(Mpo.onsite, opera="sigma_z", dof_set={"spin"}))
+        #sigma_z0 = mps.expectation(sigma_z_mpo)
+        #assert np.allclose(sigma_z0, rho[0,0]-rho[1,1])
+        self.sigma_z.append((rho[0,0]-rho[1,1]).real)
+        
+        #sigma_x_mpo = self.model.get_mpos("sigma_x", partial(Mpo.onsite, opera="sigma_x", dof_set={"spin"}))
+        #sigma_x0 = mps.expectation(sigma_x_mpo)
+        #assert np.allclose(sigma_x0, rho[0,1]+rho[1,0])
+        self.sigma_x.append((rho[0,1]+rho[1,0]).real)
+        logger.info(f"sigma_z: {self.sigma_z[-1]}. sigma_x: {self.sigma_x[-1]}")
+        
+        bond_entropy = mps.calc_entropy("bond")
+        self.bond_entropy.append(bond_entropy)
+
+    def evolve_single_step(self, evolve_dt):
+        return self.latest_mps.evolve(self.h_mpo, evolve_dt)
+
+    def get_dump_dict(self):
+        dump_dict = dict()
+        dump_dict["time series"] = self.evolve_times
+        dump_dict["sigma_x"] = self.sigma_x
+        dump_dict["sigma_z"] = self.sigma_z
+        dump_dict["rho"] = self.rho
+        dump_dict["bond_entropy"] = self.bond_entropy
+        return dump_dict
```

### Comparing `renormalizer-0.0.8/renormalizer/spectra/base.py` & `renormalizer-0.0.9/renormalizer/spectra/base.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/spectra/exact.py` & `renormalizer-0.0.9/renormalizer/spectra/exact.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/spectra/tests/test_spectra.py` & `renormalizer-0.0.9/renormalizer/spectra/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/spectra/zerot.py` & `renormalizer-0.0.9/renormalizer/spectra/zerot.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-# -*- coding: utf-8 -*-
-# Author: Jiajun Ren <jiajunren0522@gmail.com>
-#         Weitang Li <liwt31@163.com>
-
-import logging
-
-from renormalizer.mps import Mpo, Mps, gs
-from renormalizer.spectra.base import SpectraTdMpsJobBase
-from renormalizer.mps.mps import BraKetPair
-from renormalizer.utils import Quantity, OptimizeConfig
-
-logger = logging.getLogger(__name__)
-
-
-class SpectraZeroT(SpectraTdMpsJobBase):
-    '''Calculate the zero temprature absorption & emission spectrum using TD-DMRG
-
-    Parameters:
-        model : MolList
-            the molecular information
-        spectratype : string
-            "abs" or "emi"
-        optimize_config :
-            parameter for ground state sweep
-        evolve_config :
-            time evolution
-    '''
-    def __init__(
-        self,
-        model,
-        spectratype,
-        optimize_config=None,
-        evolve_config=None,
-        offset=Quantity(0),
-    ):
-        if optimize_config is None:
-            self.optimize_config = OptimizeConfig()
-        else:
-            self.optimize_config = optimize_config
-
-        super(SpectraZeroT, self).__init__(
-            model, spectratype, Quantity(0), evolve_config, offset
-        )
-
-    def init_mps(self):
-        if self.spectratype == "emi":
-            operator = "a"
-        else:
-            operator = r"a^\dagger"
-        dipole_mpo = Mpo.onsite(self.model, operator, dipole=True)
-        a_ket_mps = dipole_mpo.apply(self.get_imps(), canonicalise=True)
-        a_ket_mps.normalize("mps_norm_to_coeff")
-        a_ket_mps.evolve_config = self.evolve_config
-        a_bra_mps = a_ket_mps.copy()
-        return BraKetPair(a_bra_mps, a_ket_mps)
-
-    def get_imps(self):
-        mmax = self.optimize_config.procedure[0][0]
-        i_mps = Mps.random(self.h_mpo.model, self.nexciton, mmax, 1)
-        i_mps.optimize_config = self.optimize_config
-        energy, i_mps = gs.optimize_mps(i_mps, self.h_mpo)
-        return i_mps
-
-
-class SpectraOneWayPropZeroT(SpectraZeroT):
-    def evolve_single_step(self, evolve_dt):
-        latest_bra_mps, latest_ket_mps = self.latest_mps
-        latest_ket_mps = latest_ket_mps.evolve(self.h_mpo, evolve_dt)
-        return BraKetPair(latest_bra_mps, latest_ket_mps)
-
-
-class SpectraTwoWayPropZeroT(SpectraZeroT):
-    def evolve_single_step(self, evolve_dt):
-        latest_bra_mps, latest_ket_mps = self.latest_mps
-        if len(self.evolve_times) % 2 == 1:
-            latest_ket_mps = latest_ket_mps.evolve(self.h_mpo, evolve_dt)
-        else:
-            latest_bra_mps = latest_bra_mps.evolve(self.h_mpo, -evolve_dt)
-        return BraKetPair(latest_bra_mps, latest_ket_mps)
+# -*- coding: utf-8 -*-
+# Author: Jiajun Ren <jiajunren0522@gmail.com>
+#         Weitang Li <liwt31@163.com>
+
+import logging
+
+from renormalizer.mps import Mpo, Mps, gs
+from renormalizer.spectra.base import SpectraTdMpsJobBase
+from renormalizer.mps.mps import BraKetPair
+from renormalizer.utils import Quantity, OptimizeConfig
+
+logger = logging.getLogger(__name__)
+
+
+class SpectraZeroT(SpectraTdMpsJobBase):
+    '''Calculate the zero temprature absorption & emission spectrum using TD-DMRG
+
+    Parameters:
+        model : MolList
+            the molecular information
+        spectratype : string
+            "abs" or "emi"
+        optimize_config :
+            parameter for ground state sweep
+        evolve_config :
+            time evolution
+    '''
+    def __init__(
+        self,
+        model,
+        spectratype,
+        optimize_config=None,
+        evolve_config=None,
+        offset=Quantity(0),
+    ):
+        if optimize_config is None:
+            self.optimize_config = OptimizeConfig()
+        else:
+            self.optimize_config = optimize_config
+
+        super(SpectraZeroT, self).__init__(
+            model, spectratype, Quantity(0), evolve_config, offset
+        )
+
+    def init_mps(self):
+        if self.spectratype == "emi":
+            operator = "a"
+        else:
+            operator = r"a^\dagger"
+        dipole_mpo = Mpo.onsite(self.model, operator, dipole=True)
+        a_ket_mps = dipole_mpo.apply(self.get_imps(), canonicalise=True)
+        a_ket_mps.normalize("mps_norm_to_coeff")
+        a_ket_mps.evolve_config = self.evolve_config
+        a_bra_mps = a_ket_mps.copy()
+        return BraKetPair(a_bra_mps, a_ket_mps)
+
+    def get_imps(self):
+        mmax = self.optimize_config.procedure[0][0]
+        i_mps = Mps.random(self.h_mpo.model, self.nexciton, mmax, 1)
+        i_mps.optimize_config = self.optimize_config
+        energy, i_mps = gs.optimize_mps(i_mps, self.h_mpo)
+        return i_mps
+
+
+class SpectraOneWayPropZeroT(SpectraZeroT):
+    def evolve_single_step(self, evolve_dt):
+        latest_bra_mps, latest_ket_mps = self.latest_mps
+        latest_ket_mps = latest_ket_mps.evolve(self.h_mpo, evolve_dt)
+        return BraKetPair(latest_bra_mps, latest_ket_mps)
+
+
+class SpectraTwoWayPropZeroT(SpectraZeroT):
+    def evolve_single_step(self, evolve_dt):
+        latest_bra_mps, latest_ket_mps = self.latest_mps
+        if len(self.evolve_times) % 2 == 1:
+            latest_ket_mps = latest_ket_mps.evolve(self.h_mpo, evolve_dt)
+        else:
+            latest_bra_mps = latest_bra_mps.evolve(self.h_mpo, -evolve_dt)
+        return BraKetPair(latest_bra_mps, latest_ket_mps)
```

### Comparing `renormalizer-0.0.8/renormalizer/tests/c2h4_para.py` & `renormalizer-0.0.9/renormalizer/tests/c2h4_para.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/tests/parameter.py` & `renormalizer-0.0.9/renormalizer/tests/parameter.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/tests/parameter_PBI.py` & `renormalizer-0.0.9/renormalizer/tests/parameter_PBI.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/tests/parameter_exact.py` & `renormalizer-0.0.9/renormalizer/tests/parameter_exact.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/transport/dynamics.py` & `renormalizer-0.0.9/renormalizer/transport/dynamics.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,295 +1,295 @@
-# -*- coding: utf-8 -*-
-# Author: Jiajun Ren <jiajunren0522@gmail.com>
-#         Weitang Li <liwt31@163.com>
-
-import logging
-import os
-from enum import Enum
-from collections import OrderedDict
-from functools import partial
-
-from scipy.linalg import logm
-
-from renormalizer.mps import Mpo, Mps, MpDm, ThermalProp, load_thermal_state
-from renormalizer.model import HolsteinModel
-from renormalizer.utils import TdMpsJob, Quantity, CompressConfig, EvolveConfig
-
-import numpy as np
-
-logger = logging.getLogger(__name__)
-
-EDGE_THRESHOLD = 1e-4
-
-
-class InitElectron(Enum):
-    """
-    Available methods to prepare initial state of charge diffusion
-    """
-    fc = "franck-condon excitation"
-    relaxed = "analytically relaxed phonon(s)"
-
-
-class ChargeDiffusionDynamics(TdMpsJob):
-    r"""
-    Simulate charge diffusion dynamics by TD-DMRG. It is possible to obtain mobility from the simulation,
-    but care must be taken to ensure that mean square displacement grows linearly with time.
-
-    Args:
-        model (:class:`~renormalizer.model.model.HolsteinModel`): system information.
-            Currently only support :class:`~renormalizer.model.model.HolsteinModel`.
-        temperature (:class:`~renormalizer.utils.quantity.Quantity`): simulation temperature.
-            Default is zero temperature. For finite temperature charge dynamics, it is recommended to use
-            thermal field dynamics and transform the Hamiltonian.
-            See the documentation of :class:`~renormalizer.transport.spectral_function.SpectralFunctionZT`
-            for more details.
-        compress_config (:class:`~renormalizer.utils.configs.CompressConfig`): config when compressing MPS.
-        evolve_config (:class:`~renormalizer.utils.configs.EvolveConfig`): config when evolving MPS.
-        stop_at_edge (bool): whether stop when charge has diffused to the boundary of the system. Default is ``True``.
-        init_electron (:class:`~renormalizer.transport.transport.InitElectron`):
-            the method to prepare the initial state.
-        rdm (bool): whether calculate reduced density matrix and k-space representation for the electron.
-            Default is ``False`` because usually the calculation is time consuming.
-            Using scheme 4 might partly solve the problem.
-        dump_dir (str): the directory for logging and numerical result output.
-            Also the directory from which to load previous thermal propagated initial state (if exists).
-        job_name (str): the name of the calculation job which determines the file name of the logging and numerical result output.
-            For thermal propagated initial state input/output the file name is appended with ``"_impdm.npz"``.
-
-    Attributes:
-        energies (np.ndarray): calculated energy of the states during the time evolution.
-            Without dissipation or TD-Hartree the value should remain unchanged and to some extent
-            can be used to measure the error during time evolution.
-        r_square_array (np.ndarray): calculated mean square displacement
-            :math:`\langle \psi | \hat r^2 | \psi \rangle - \langle \psi | \hat r | \psi \rangle^2`
-            at each evolution time step.
-        e_occupations_array (np.ndarray): calculated electron occupations in real space on each site for each evolution time step.
-        ph_occupations_array (np.ndarray): calculated phonon occupations on each site for each evolution time step.
-        reduced_density_matrices (list): calculated reduced density matrices of the electron for each evolution time step.
-            Only available when ``rdm`` is set to ``True``.
-        k_occupations_array (np.ndarray): calculated electron occupations in momentum (k) space
-            on each site for each evolution time step. Only available when ``rdm`` is set to ``True``.
-            The basis transformation is based on:
-
-            .. math::
-                | k \rangle = \sum_j e^{-ijk} | j \rangle
-
-            where :math:`k` starts from :math:`-\pi` to :math:`\pi` with interval :math:`2\pi/N`.
-            :math:`N` represents total number of electronic sites.
-        coherent_length_array (np.ndarray): coherent length :math:`L` calculated for each evolution time step.
-
-            .. math::
-                L = \sum_{ij, i \neq j} | \rho_{ij} |
-
-            where :math:`\rho` is the density matrix of the electron. Naturally this is only available when
-            ``rdm`` is set to ``True``.
-
-    """
-
-    def __init__(
-        self,
-        model: HolsteinModel,
-        temperature: Quantity = Quantity(0, "K"),
-        compress_config: CompressConfig = None,
-        evolve_config: EvolveConfig = None,
-        stop_at_edge: bool = True,
-        init_electron=InitElectron.relaxed,
-        rdm: bool = False,
-        dump_dir: str = None,
-        job_name: str = None,
-    ):
-        self.model: HolsteinModel = model
-        self.temperature = temperature
-        self.mpo = None
-        self.init_electron = init_electron
-        if compress_config is None:
-            self.compress_config: CompressConfig = CompressConfig()
-        else:
-            self.compress_config: CompressConfig = compress_config
-        self.energies = []
-        self.r_square_array = []
-        self.e_occupations_array = []
-        self.ph_occupations_array = []
-        self.reduced_density_matrices = [] if rdm else None
-        self.k_occupations_array = []
-        # von Neumann entropy between e and ph
-        self.eph_vn_entropy_array = []
-        # entropy at each bond
-        self.bond_vn_entropy_array = []
-        self.coherent_length_array = []
-
-        if dump_dir is not None and job_name is not None:
-            self.thermal_dump_path = os.path.join(dump_dir, job_name + '_impdm.npz')
-        else:
-            self.thermal_dump_path = None
-
-        super(ChargeDiffusionDynamics, self).__init__(evolve_config=evolve_config,
-                                                      dump_dir=dump_dir, job_name=job_name)
-        assert self.mpo is not None
-
-        self.elocalex_arrays = []
-        self.j_arrays = []
-        self.custom_dump_info = OrderedDict()
-        self.stop_at_edge = stop_at_edge
-
-    @property
-    def mol_num(self):
-        return self.model.mol_num
-
-    def create_electron_fc(self, gs_mp):
-        center_mol_idx = self.mol_num // 2
-        creation_operator = Mpo.onsite(
-            self.model, r"a^\dagger", dof_set={center_mol_idx}
-        )
-        mps = creation_operator.apply(gs_mp)
-        return mps
-
-    def create_electron_relaxed(self, gs_mp):
-        assert np.allclose(gs_mp.bond_dims, np.ones_like(gs_mp.bond_dims))
-        center_mol_idx = self.mol_num // 2
-        center_mol = self.model[center_mol_idx]
-        # start from phonon
-        for i, ph in enumerate(center_mol.ph_list):
-            idx = self.model.order[(center_mol_idx, i)]
-            mt = gs_mp[idx][0, ..., 0].array
-            evecs = ph.get_displacement_evecs()
-            mt = evecs.dot(mt)
-            logger.debug(f"relaxed mt: {mt}")
-            gs_mp[idx] = mt.reshape([1] + list(mt.shape) + [1])
-
-        creation_operator = Mpo.onsite(
-            self.model, r"a^\dagger", dof_set={center_mol_idx}
-        )
-        mps = creation_operator.apply(gs_mp)
-        return mps
-
-    def create_electron(self, gs_mp):
-        method_mapping = {
-            InitElectron.fc: self.create_electron_fc,
-            InitElectron.relaxed: self.create_electron_relaxed,
-        }
-        logger.info(f"Creating electron using {self.init_electron}")
-        return method_mapping[self.init_electron](gs_mp)
-
-    def init_mps(self):
-        tentative_mpo = Mpo(self.model)
-        if self.temperature == 0:
-            gs_mp = Mps.ground_state(self.model, max_entangled=False)
-        else:
-            if self.thermal_dump_path is not None:
-                gs_mp = load_thermal_state(self.model, self.thermal_dump_path)
-            else:
-                gs_mp = None
-            if gs_mp is None:
-                gs_mp = MpDm.max_entangled_gs(self.model)
-                tp = ThermalProp(gs_mp, exact=True, space="GS")
-                tp.evolve(None, max(20, len(gs_mp)), self.temperature.to_beta() / 2j)
-                gs_mp = tp.latest_mps
-                if self.thermal_dump_path is not None:
-                    gs_mp.dump(self.thermal_dump_path)
-        init_mp = self.create_electron(gs_mp)
-        energy = Quantity(init_mp.expectation(tentative_mpo))
-        self.mpo = Mpo(self.model, offset=energy)
-        logger.info(f"mpo bond dims: {self.mpo.bond_dims}")
-        logger.info(f"mpo physical dims: {self.mpo.pbond_list}")
-        init_mp.evolve_config = self.evolve_config
-        init_mp.compress_config = self.compress_config
-        if self.evolve_config.is_tdvp:
-            init_mp = init_mp.expand_bond_dimension(self.mpo)
-        init_mp.canonicalise()
-        return init_mp
-
-    def process_mps(self, mps):
-        new_energy = mps.expectation(self.mpo)
-        self.energies.append(new_energy)
-        logger.debug(f"Energy: {new_energy}")
-
-        if self.reduced_density_matrices is not None:
-            logger.debug("Calculating reduced density matrix")
-            rdm = mps.calc_edof_rdm()
-            logger.debug("Calculate reduced density matrix finished")
-            self.reduced_density_matrices.append(rdm)
-
-            # k_space transform matrix
-            n = len(self.model)
-            assert rdm.shape == (n, n)
-            transform = np.exp(-1j * (np.arange(-n, n, 2)/n * np.pi).reshape(-1, 1) * np.arange(0, n).reshape(1, -1)) / np.sqrt(n)
-            k = np.diag(transform @ rdm @ transform.conj().T).real
-            self.k_occupations_array.append(k)
-
-            # von Neumann entropy
-            entropy = -np.trace(rdm @ logm(rdm))
-            self.eph_vn_entropy_array.append(entropy)
-
-            self.coherent_length_array.append(np.abs(rdm).sum() - np.trace(rdm).real)
-
-        else:
-            rdm = None
-
-        if rdm is not None:
-            e_occupations = np.diag(rdm).real
-        else:
-            e_occupations = mps.e_occupations
-        self.e_occupations_array.append(e_occupations)
-        self.r_square_array.append(calc_r_square(e_occupations))
-        self.ph_occupations_array.append(mps.ph_occupations)
-        logger.info(f"e occupations: {self.e_occupations_array[-1]}")
-
-        bond_vn_entropy = mps.calc_bond_entropy()
-        logger.info(f"bond entropy: {bond_vn_entropy}")
-        self.bond_vn_entropy_array.append(bond_vn_entropy)
-
-    def evolve_single_step(self, evolve_dt):
-        old_mps = self.latest_mps
-        new_mps = old_mps.evolve(self.mpo, evolve_dt)
-        return new_mps
-
-    def stop_evolve_criteria(self):
-        # electron has moved to the edge
-        return self.stop_at_edge and EDGE_THRESHOLD < self.e_occupations_array[-1][0]
-
-    def get_dump_dict(self):
-        dump_dict = OrderedDict()
-        dump_dict["mol list"] = self.model.to_dict()
-        dump_dict["tempearture"] = self.temperature.as_au()
-        dump_dict["total time"] = self.evolve_times[-1]
-        dump_dict["other info"] = self.custom_dump_info
-        # make np array json serializable
-        dump_dict["r square array"] = self.r_square_array
-        dump_dict["electron occupations array"] = self.e_occupations_array
-        dump_dict["phonon occupations array"] = self.ph_occupations_array
-        dump_dict["k occupations array"] = self.k_occupations_array
-        dump_dict["eph entropy"] = self.eph_vn_entropy_array
-        dump_dict["bond entropy"] = self.bond_vn_entropy_array
-        dump_dict["coherent length array"] = self.coherent_length_array
-        if self.reduced_density_matrices:
-            dump_dict["reduced density matrices"] = self.reduced_density_matrices
-        dump_dict["time series"] = list(self.evolve_times)
-        return dump_dict
-
-    def is_similar(self, other: "ChargeDiffusionDynamics", rtol=1e-3):
-        all_close_with_tol = partial(np.allclose, rtol=rtol, atol=1e-3)
-        if len(self.evolve_times) != len(other.evolve_times):
-            return False
-        attrs = [
-            "evolve_times",
-            "r_square_array",
-            "energies",
-            "e_occupations_array",
-            "ph_occupations_array",
-            "coherent_length_array",
-        ]
-        for attr in attrs:
-            s = getattr(self, attr)
-            o = getattr(other, attr)
-            if not all_close_with_tol(s, o):
-                return False
-        return True
-
-
-def calc_r_square(e_occupations):
-    r_list = np.arange(0, len(e_occupations))
-    if np.allclose(e_occupations, np.zeros_like(e_occupations)):
-        return 0
-    r_mean_square = np.average(r_list, weights=e_occupations) ** 2
-    mean_r_square = np.average(r_list ** 2, weights=e_occupations)
-    return float(mean_r_square - r_mean_square)
+# -*- coding: utf-8 -*-
+# Author: Jiajun Ren <jiajunren0522@gmail.com>
+#         Weitang Li <liwt31@163.com>
+
+import logging
+import os
+from enum import Enum
+from collections import OrderedDict
+from functools import partial
+
+from scipy.linalg import logm
+
+from renormalizer.mps import Mpo, Mps, MpDm, ThermalProp, load_thermal_state
+from renormalizer.model import HolsteinModel
+from renormalizer.utils import TdMpsJob, Quantity, CompressConfig, EvolveConfig
+
+import numpy as np
+
+logger = logging.getLogger(__name__)
+
+EDGE_THRESHOLD = 1e-4
+
+
+class InitElectron(Enum):
+    """
+    Available methods to prepare initial state of charge diffusion
+    """
+    fc = "franck-condon excitation"
+    relaxed = "analytically relaxed phonon(s)"
+
+
+class ChargeDiffusionDynamics(TdMpsJob):
+    r"""
+    Simulate charge diffusion dynamics by TD-DMRG. It is possible to obtain mobility from the simulation,
+    but care must be taken to ensure that mean square displacement grows linearly with time.
+
+    Args:
+        model (:class:`~renormalizer.model.model.HolsteinModel`): system information.
+            Currently only support :class:`~renormalizer.model.model.HolsteinModel`.
+        temperature (:class:`~renormalizer.utils.quantity.Quantity`): simulation temperature.
+            Default is zero temperature. For finite temperature charge dynamics, it is recommended to use
+            thermal field dynamics and transform the Hamiltonian.
+            See the documentation of :class:`~renormalizer.transport.spectral_function.SpectralFunctionZT`
+            for more details.
+        compress_config (:class:`~renormalizer.utils.configs.CompressConfig`): config when compressing MPS.
+        evolve_config (:class:`~renormalizer.utils.configs.EvolveConfig`): config when evolving MPS.
+        stop_at_edge (bool): whether stop when charge has diffused to the boundary of the system. Default is ``True``.
+        init_electron (:class:`~renormalizer.transport.transport.InitElectron`):
+            the method to prepare the initial state.
+        rdm (bool): whether calculate reduced density matrix and k-space representation for the electron.
+            Default is ``False`` because usually the calculation is time consuming.
+            Using scheme 4 might partly solve the problem.
+        dump_dir (str): the directory for logging and numerical result output.
+            Also the directory from which to load previous thermal propagated initial state (if exists).
+        job_name (str): the name of the calculation job which determines the file name of the logging and numerical result output.
+            For thermal propagated initial state input/output the file name is appended with ``"_impdm.npz"``.
+
+    Attributes:
+        energies (np.ndarray): calculated energy of the states during the time evolution.
+            Without dissipation or TD-Hartree the value should remain unchanged and to some extent
+            can be used to measure the error during time evolution.
+        r_square_array (np.ndarray): calculated mean square displacement
+            :math:`\langle \psi | \hat r^2 | \psi \rangle - \langle \psi | \hat r | \psi \rangle^2`
+            at each evolution time step.
+        e_occupations_array (np.ndarray): calculated electron occupations in real space on each site for each evolution time step.
+        ph_occupations_array (np.ndarray): calculated phonon occupations on each site for each evolution time step.
+        reduced_density_matrices (list): calculated reduced density matrices of the electron for each evolution time step.
+            Only available when ``rdm`` is set to ``True``.
+        k_occupations_array (np.ndarray): calculated electron occupations in momentum (k) space
+            on each site for each evolution time step. Only available when ``rdm`` is set to ``True``.
+            The basis transformation is based on:
+
+            .. math::
+                | k \rangle = \sum_j e^{-ijk} | j \rangle
+
+            where :math:`k` starts from :math:`-\pi` to :math:`\pi` with interval :math:`2\pi/N`.
+            :math:`N` represents total number of electronic sites.
+        coherent_length_array (np.ndarray): coherent length :math:`L` calculated for each evolution time step.
+
+            .. math::
+                L = \sum_{ij, i \neq j} | \rho_{ij} |
+
+            where :math:`\rho` is the density matrix of the electron. Naturally this is only available when
+            ``rdm`` is set to ``True``.
+
+    """
+
+    def __init__(
+        self,
+        model: HolsteinModel,
+        temperature: Quantity = Quantity(0, "K"),
+        compress_config: CompressConfig = None,
+        evolve_config: EvolveConfig = None,
+        stop_at_edge: bool = True,
+        init_electron=InitElectron.relaxed,
+        rdm: bool = False,
+        dump_dir: str = None,
+        job_name: str = None,
+    ):
+        self.model: HolsteinModel = model
+        self.temperature = temperature
+        self.mpo = None
+        self.init_electron = init_electron
+        if compress_config is None:
+            self.compress_config: CompressConfig = CompressConfig()
+        else:
+            self.compress_config: CompressConfig = compress_config
+        self.energies = []
+        self.r_square_array = []
+        self.e_occupations_array = []
+        self.ph_occupations_array = []
+        self.reduced_density_matrices = [] if rdm else None
+        self.k_occupations_array = []
+        # von Neumann entropy between e and ph
+        self.eph_vn_entropy_array = []
+        # entropy at each bond
+        self.bond_vn_entropy_array = []
+        self.coherent_length_array = []
+
+        if dump_dir is not None and job_name is not None:
+            self.thermal_dump_path = os.path.join(dump_dir, job_name + '_impdm.npz')
+        else:
+            self.thermal_dump_path = None
+
+        super(ChargeDiffusionDynamics, self).__init__(evolve_config=evolve_config,
+                                                      dump_dir=dump_dir, job_name=job_name)
+        assert self.mpo is not None
+
+        self.elocalex_arrays = []
+        self.j_arrays = []
+        self.custom_dump_info = OrderedDict()
+        self.stop_at_edge = stop_at_edge
+
+    @property
+    def mol_num(self):
+        return self.model.mol_num
+
+    def create_electron_fc(self, gs_mp):
+        center_mol_idx = self.mol_num // 2
+        creation_operator = Mpo.onsite(
+            self.model, r"a^\dagger", dof_set={center_mol_idx}
+        )
+        mps = creation_operator.apply(gs_mp)
+        return mps
+
+    def create_electron_relaxed(self, gs_mp):
+        assert np.allclose(gs_mp.bond_dims, np.ones_like(gs_mp.bond_dims))
+        center_mol_idx = self.mol_num // 2
+        center_mol = self.model[center_mol_idx]
+        # start from phonon
+        for i, ph in enumerate(center_mol.ph_list):
+            idx = self.model.order[(center_mol_idx, i)]
+            mt = gs_mp[idx][0, ..., 0].array
+            evecs = ph.get_displacement_evecs()
+            mt = evecs.dot(mt)
+            logger.debug(f"relaxed mt: {mt}")
+            gs_mp[idx] = mt.reshape([1] + list(mt.shape) + [1])
+
+        creation_operator = Mpo.onsite(
+            self.model, r"a^\dagger", dof_set={center_mol_idx}
+        )
+        mps = creation_operator.apply(gs_mp)
+        return mps
+
+    def create_electron(self, gs_mp):
+        method_mapping = {
+            InitElectron.fc: self.create_electron_fc,
+            InitElectron.relaxed: self.create_electron_relaxed,
+        }
+        logger.info(f"Creating electron using {self.init_electron}")
+        return method_mapping[self.init_electron](gs_mp)
+
+    def init_mps(self):
+        tentative_mpo = Mpo(self.model)
+        if self.temperature == 0:
+            gs_mp = Mps.ground_state(self.model, max_entangled=False)
+        else:
+            if self.thermal_dump_path is not None:
+                gs_mp = load_thermal_state(self.model, self.thermal_dump_path)
+            else:
+                gs_mp = None
+            if gs_mp is None:
+                gs_mp = MpDm.max_entangled_gs(self.model)
+                tp = ThermalProp(gs_mp, exact=True, space="GS")
+                tp.evolve(None, max(20, len(gs_mp)), self.temperature.to_beta() / 2j)
+                gs_mp = tp.latest_mps
+                if self.thermal_dump_path is not None:
+                    gs_mp.dump(self.thermal_dump_path)
+        init_mp = self.create_electron(gs_mp)
+        energy = Quantity(init_mp.expectation(tentative_mpo))
+        self.mpo = Mpo(self.model, offset=energy)
+        logger.info(f"mpo bond dims: {self.mpo.bond_dims}")
+        logger.info(f"mpo physical dims: {self.mpo.pbond_list}")
+        init_mp.evolve_config = self.evolve_config
+        init_mp.compress_config = self.compress_config
+        if self.evolve_config.is_tdvp:
+            init_mp = init_mp.expand_bond_dimension(self.mpo)
+        init_mp.canonicalise()
+        return init_mp
+
+    def process_mps(self, mps):
+        new_energy = mps.expectation(self.mpo)
+        self.energies.append(new_energy)
+        logger.debug(f"Energy: {new_energy}")
+
+        if self.reduced_density_matrices is not None:
+            logger.debug("Calculating reduced density matrix")
+            rdm = mps.calc_edof_rdm()
+            logger.debug("Calculate reduced density matrix finished")
+            self.reduced_density_matrices.append(rdm)
+
+            # k_space transform matrix
+            n = len(self.model)
+            assert rdm.shape == (n, n)
+            transform = np.exp(-1j * (np.arange(-n, n, 2)/n * np.pi).reshape(-1, 1) * np.arange(0, n).reshape(1, -1)) / np.sqrt(n)
+            k = np.diag(transform @ rdm @ transform.conj().T).real
+            self.k_occupations_array.append(k)
+
+            # von Neumann entropy
+            entropy = -np.trace(rdm @ logm(rdm))
+            self.eph_vn_entropy_array.append(entropy)
+
+            self.coherent_length_array.append(np.abs(rdm).sum() - np.trace(rdm).real)
+
+        else:
+            rdm = None
+
+        if rdm is not None:
+            e_occupations = np.diag(rdm).real
+        else:
+            e_occupations = mps.e_occupations
+        self.e_occupations_array.append(e_occupations)
+        self.r_square_array.append(calc_r_square(e_occupations))
+        self.ph_occupations_array.append(mps.ph_occupations)
+        logger.info(f"e occupations: {self.e_occupations_array[-1]}")
+
+        bond_vn_entropy = mps.calc_bond_entropy()
+        logger.info(f"bond entropy: {bond_vn_entropy}")
+        self.bond_vn_entropy_array.append(bond_vn_entropy)
+
+    def evolve_single_step(self, evolve_dt):
+        old_mps = self.latest_mps
+        new_mps = old_mps.evolve(self.mpo, evolve_dt)
+        return new_mps
+
+    def stop_evolve_criteria(self):
+        # electron has moved to the edge
+        return self.stop_at_edge and EDGE_THRESHOLD < self.e_occupations_array[-1][0]
+
+    def get_dump_dict(self):
+        dump_dict = OrderedDict()
+        dump_dict["mol list"] = self.model.to_dict()
+        dump_dict["tempearture"] = self.temperature.as_au()
+        dump_dict["total time"] = self.evolve_times[-1]
+        dump_dict["other info"] = self.custom_dump_info
+        # make np array json serializable
+        dump_dict["r square array"] = self.r_square_array
+        dump_dict["electron occupations array"] = self.e_occupations_array
+        dump_dict["phonon occupations array"] = self.ph_occupations_array
+        dump_dict["k occupations array"] = self.k_occupations_array
+        dump_dict["eph entropy"] = self.eph_vn_entropy_array
+        dump_dict["bond entropy"] = self.bond_vn_entropy_array
+        dump_dict["coherent length array"] = self.coherent_length_array
+        if self.reduced_density_matrices:
+            dump_dict["reduced density matrices"] = self.reduced_density_matrices
+        dump_dict["time series"] = list(self.evolve_times)
+        return dump_dict
+
+    def is_similar(self, other: "ChargeDiffusionDynamics", rtol=1e-3):
+        all_close_with_tol = partial(np.allclose, rtol=rtol, atol=1e-3)
+        if len(self.evolve_times) != len(other.evolve_times):
+            return False
+        attrs = [
+            "evolve_times",
+            "r_square_array",
+            "energies",
+            "e_occupations_array",
+            "ph_occupations_array",
+            "coherent_length_array",
+        ]
+        for attr in attrs:
+            s = getattr(self, attr)
+            o = getattr(other, attr)
+            if not all_close_with_tol(s, o):
+                return False
+        return True
+
+
+def calc_r_square(e_occupations):
+    r_list = np.arange(0, len(e_occupations))
+    if np.allclose(e_occupations, np.zeros_like(e_occupations)):
+        return 0
+    r_mean_square = np.average(r_list, weights=e_occupations) ** 2
+    mean_r_square = np.average(r_list ** 2, weights=e_occupations)
+    return float(mean_r_square - r_mean_square)
```

### Comparing `renormalizer-0.0.8/renormalizer/transport/kubo.py` & `renormalizer-0.0.9/renormalizer/transport/kubo.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,365 +1,365 @@
-# -*- coding: utf-8 -*-
-
-import logging
-import os
-
-import scipy.integrate
-
-from renormalizer.mps import MpDm, Mpo, BraKetPair, ThermalProp, load_thermal_state
-from renormalizer.mps.backend import np
-from renormalizer.utils.constant import mobility2au
-from renormalizer.utils import TdMpsJob, Quantity, EvolveConfig, CompressConfig
-from renormalizer.model import Model
-from renormalizer.property import Property
-
-logger = logging.getLogger(__name__)
-
-
-class TransportKubo(TdMpsJob):
-    r"""
-    Calculate mobility via Green-Kubo formula:
-
-        .. math::
-            \mu = \frac{1}{k_B T} \int_0^\infty dt \langle \hat j (t) \hat j(0) \rangle
-            = \frac{1}{k_B T} \int_0^\infty dt C(t)
-
-    where
-
-        .. math::
-           \hat j = -\frac{i}{\hbar}[\hat P, \hat H]
-
-    and :math:`\hat P = e_0 \sum_m R_m a^\dagger_m a_m` is the polarization operator.
-
-    .. note::
-        In principle :math:`\hat H` can take any form, however only Holstein-Peierls Hamiltonian is well tested.
-
-    More explicitly, :math:`C(t)` has the form:
-
-        .. math::
-            C(t) = \textrm{Tr}\{\rho(T) e^{i \hat H t} \hat j(0) e^{- i \hat H t} \hat j (0)\}
-
-    where we have assumed :math:`\rho(T)` is normalized
-    (i.e. it is divided by the partition function :math:`\textrm{Tr}\{\rho(T)\}`).
-
-    In terms of practical implementation, it is ideal if :math:`\rho(T)` is split into two parts
-    to (hopefully) speed up calculation and minimize time evolution error:
-
-        .. math::
-            \begin{align}
-             C(t) & = \textrm{Tr}\{\rho(T) e^{i \hat H t} \hat j(0) e^{- i \hat H t} \hat j(0)\} \\
-                  & = \textrm{Tr}\{e^{-\beta \hat H} e^{i \hat H t} \hat j(0) e^{- i \hat H t} \hat j(0)\} \\
-                  & = \textrm{Tr}\{e^{-\beta \hat H / 2} e^{i \hat H t} \hat j(0) e^{- i \hat H t} \hat j(0) e^{-\beta \hat H / 2}\}
-            \end{align}
-
-    In this class, imaginary time propagation from infinite temperature to :math:`\beta/2` is firstly carried out
-    to obtain :math:`e^{-\beta \hat H / 2}`, and then real time propagation is carried out for :math:`e^{-\beta \hat H / 2}`
-    and :math:`\hat J(0) e^{-\beta \hat H / 2}` respectively to obtain :math:`e^{-\beta \hat H / 2} e^{i \hat H t}`
-    and :math:`e^{- i \hat H t} \hat j(0) e^{-\beta \hat H / 2}`. The correlation function at time :math:`t` can thus
-    be calculated via expectation calculation.
-
-    .. note::
-        Although the class is able to carry out imaginary time propagation, in practice for large scale calculation
-        it is usually preferable to carry out imaginary time propagation in another job and load the dumped initial
-        state directly in this class.
-
-    Args:
-        model (:class:`~renormalizer.model.Model`): system information.
-        temperature (:class:`~renormalizer.utils.quantity.Quantity`): simulation temperature.
-            Zero temperature is not supported.
-        distance_matrix (:class:`np.ndarray`): two-dimensional array :math:`D_{ij} = P_i - P_j` representing
-            distance between the :math:`i` th electronic degree of freedom and the :math:`j` th degree of freedom.
-            The index is the same with ``model.e_dofs``.
-            The parameter takes the role of :math:`\hat P` and can better handle periodic boundary condition.
-            The default value is ``None`` in which case the distance matrix is constructed assuming the system
-            is a one-dimensional chain.
-
-            .. note::
-                The construction of the matrix should be taken with great care if periodic boundary condition
-                is applied. Take a one-dimensional chain as an example, the distance between the leftmost site
-                and the rightmost site is :math:`\pm R` where :math:`R` is the intersite distance,
-                rather than :math:`\pm (N-1)R` where :math:`N` is the total number of electronic degrees of freedom.
-        insteps (int): steps for imaginary time propagation.
-        ievolve_config (:class:`~renormalizer.utils.configs.EvolveConfig`): config when carrying out imaginary time propagation.
-        compress_config (:class:`~renormalizer.utils.configs.CompressConfig`): config when compressing MPS.
-            Note that if TDVP based methods are chosen for time evolution, compression is necessary
-            when :math:`\hat j` is applied on :math:`e^{-\beta \hat H / 2}` but no compression is carried out
-            for :math:`e^{-\beta \hat H / 2} e^{i \hat H t}`.
-        evolve_config (:class:`~renormalizer.utils.configs.EvolveConfig`): config when carrying out real time propagation.
-        dump_dir (str): the directory for logging and numerical result output.
-        job_name (str): the name of the calculation job which determines the file name of the logging and numerical result output.
-        thermal_dump_path (str): the path to load previously thermal propagated initial state if it exists or the path
-            to dump the thermal state if it does not exist. The default value is determined by appending ``"_impdm.npz"``
-            to the path joined by ``dump_dir`` and ``job_name``.
-        properties (:class:`~renormalizer.property.property.Property`): other properties to calculate during real time evolution.
-            Currently only supports Holstein model.
-    """
-    def __init__(self, model: Model, temperature: Quantity, distance_matrix: np.ndarray = None,
-                 insteps: int=1, ievolve_config=None, compress_config=None,
-                 evolve_config=None, dump_dir: str=None, job_name: str=None,
-                 thermal_dump_path: str=None, properties: Property = None):
-        self.model = model
-        self.distance_matrix = distance_matrix
-        self.h_mpo = Mpo(model)
-        logger.info(f"Bond dim of h_mpo: {self.h_mpo.bond_dims}")
-        self._construct_current_operator()
-        if temperature == 0:
-            raise ValueError("Can't set temperature to 0.")
-        self.temperature = temperature
-
-        # imaginary time evolution config
-        if ievolve_config is None:
-            self.ievolve_config = EvolveConfig()
-            if insteps is None:
-                self.ievolve_config.adaptive = True
-                # start from a small step
-                self.ievolve_config.guess_dt = temperature.to_beta() / 1e5j
-                insteps = 1
-        else:
-            self.ievolve_config = ievolve_config
-        self.insteps = insteps
-
-        if compress_config is None:
-            logger.debug("using default compress config")
-            self.compress_config = CompressConfig()
-        else:
-            self.compress_config = compress_config
-
-        if thermal_dump_path is not None:
-            self.thermal_dump_path = thermal_dump_path
-        elif dump_dir is not None and job_name is not None:
-            self.thermal_dump_path = os.path.join(dump_dir, job_name + '_impdm.npz')
-        else:
-            self.thermal_dump_path = None
-
-        self.properties = properties
-        self._auto_corr = []
-        self._auto_corr_deomposition = []
-        super().__init__(evolve_config=evolve_config, dump_dir=dump_dir,
-                job_name=job_name)
-
-    def _construct_current_operator(self):
-        # Construct current operator. The operator is taken to be real as an optimization.
-        logger.info("constructing current operator ")
-
-        mol_num = self.model.n_edofs
-        ham_terms = self.model.ham_terms
-
-        if self.distance_matrix is None:
-            logger.info("Constructing distance matrix based on a periodic one-dimension chain.")
-            self.distance_matrix = np.arange(mol_num).reshape(-1, 1) - np.arange(mol_num).reshape(1, -1)
-            self.distance_matrix[0][-1] = 1
-            self.distance_matrix[-1][0] = -1
-
-        # current caused by pure eletronic coupling
-        holstein_current_terms = []
-        # current related to phonons
-        peierls_current_terms = []
-        # loop through the Hamiltonian to construct current operator
-        for ham_op in ham_terms:
-            # find out terms that contains two electron operators
-            # idx of the dof for the model
-            dof_op_idx1 = dof_op_idx2 = None
-            for dof_idx, dof_name in enumerate(ham_op.dofs):
-                site_idx = self.model.dof_to_siteidx[dof_name]
-                if self.model.basis[site_idx].is_electron:
-                    e_idx = self.model.e_dofs.index(dof_name)
-                    if dof_op_idx1 is None:
-                        dof_op_idx1 = dof_idx
-                        e_idx1 = e_idx
-                    elif dof_op_idx2 is None:
-                        dof_op_idx2 = dof_idx
-                        e_idx2 = e_idx
-                    else:
-                        raise ValueError(f"The model contains three-electron (or more complex) operator {ham_op}")
-                del dof_idx, dof_name
-            # two electron operators not found. Not relevant to the current operator
-            if dof_op_idx1 is None or dof_op_idx2 is None:
-                continue
-            # electron operator on the same site. Not relevant to the current operator.
-            if e_idx1 == e_idx2:
-                continue
-            # two electron operators found. Relevant to the current operator
-            # perform a bunch of sanity check
-            # at most 3 dofs are involved. More complex cases are probably supported but not tested
-            if len(ham_op.dofs) not in (2, 3):
-                raise NotImplementedError("Complex vibration potential not implemented")
-
-            # check linear coupling. More complex cases are probably supported but not tested.
-            if len(ham_op.dofs) == 3:
-                # total term idx should be 0 + 1 + 2 = 3
-                phonon_dof_idx = 3 - dof_op_idx1 - dof_op_idx2
-                assert ham_op.split_symbol[phonon_dof_idx] in (r"b^\dagger+b", "x")
-            symbol1, symbol2 = ham_op.split_symbol[dof_op_idx1], ham_op.split_symbol[dof_op_idx2]
-            if not {symbol1, symbol2} == {r"a^\dagger", "a"}:
-                raise ValueError(f"Unknown symbol: {symbol1}, {symbol2}")
-
-            # translate the term in the Hamiltonian into the term in the current operator
-            if symbol1 == r"a^\dagger":
-                factor = self.distance_matrix[e_idx1][e_idx2]
-            else:
-                factor = self.distance_matrix[e_idx2][e_idx1]
-
-            current_op = ham_op * factor
-            # Holstein terms
-            if len(ham_op.dofs) == 2:
-                holstein_current_terms.append(current_op)
-            # Peierls terms
-            else:
-                peierls_current_terms.append(current_op)
-
-        self.j_oper = Mpo(self.model, holstein_current_terms)
-        logger.info(f"current operator bond dim: {self.j_oper.bond_dims}")
-        if len(peierls_current_terms) != 0:
-            self.j_oper2  = Mpo(self.model, peierls_current_terms)
-            logger.info(f"Peierls coupling induced current operator bond dim: {self.j_oper2.bond_dims}")
-        else:
-            self.j_oper2 = None
-
-    def init_mps(self):
-        # first try to load
-        if self.thermal_dump_path is not None:
-            mpdm = load_thermal_state(self.model, self.thermal_dump_path)
-        else:
-            mpdm = None
-        # then try to calculate
-        if mpdm is None:
-            i_mpdm = MpDm.max_entangled_ex(self.model)
-            i_mpdm.compress_config = self.compress_config
-            if self.job_name is None:
-                job_name = None
-            else:
-                job_name = self.job_name + "_thermal_prop"
-            tp = ThermalProp(i_mpdm, evolve_config=self.ievolve_config, dump_dir=self.dump_dir, job_name=job_name)
-            # only propagate half beta
-            tp.evolve(None, self.insteps, self.temperature.to_beta() / 2j)
-            mpdm = tp.latest_mps
-            if self.thermal_dump_path is not None:
-                mpdm.dump(self.thermal_dump_path)
-        mpdm.compress_config = self.compress_config
-        e = mpdm.expectation(self.h_mpo)
-        self.h_mpo = Mpo(self.model, offset=Quantity(e))
-        mpdm.evolve_config = self.evolve_config
-        logger.debug("Applying current operator")
-        ket_mpdm = self.j_oper.contract(mpdm).normalize("mps_norm_to_coeff")
-        bra_mpdm = mpdm.copy()
-        if self.j_oper2 is None:
-            return BraKetPair(bra_mpdm, ket_mpdm, self.j_oper)
-        else:
-            logger.debug("Applying the second current operator")
-            ket_mpdm2 = self.j_oper2.contract(mpdm).normalize("mps_norm_to_coeff")
-            return BraKetPair(bra_mpdm, ket_mpdm, self.j_oper), BraKetPair(bra_mpdm, ket_mpdm2, self.j_oper2)
-
-    def process_mps(self, mps):
-        # add the negative sign because `self.j_oper` is taken to be real
-        if self.j_oper2 is None:
-            self._auto_corr.append(-mps.ft)
-            # calculate other properties defined in Property
-            if self.properties is not None:
-                self.properties.calc_properties_braketpair(mps)
-        else:
-            (bra_mpdm, ket_mpdm), (bra_mpdm, ket_mpdm2) = mps
-            # <J_1(t) J_1(0)>
-            ft1 = -BraKetPair(bra_mpdm, ket_mpdm, self.j_oper).ft
-            # <J_1(t) J_2(0)>
-            ft2 = -BraKetPair(bra_mpdm, ket_mpdm2, self.j_oper).ft
-            # <J_2(t) J_1(0)>
-            ft3 = -BraKetPair(bra_mpdm, ket_mpdm, self.j_oper2).ft
-            # <J_2(t) J_2(0)>
-            ft4 = -BraKetPair(bra_mpdm, ket_mpdm2, self.j_oper2).ft
-            self._auto_corr.append(ft1 + ft2 + ft3 + ft4)
-            self._auto_corr_deomposition.append([ft1, ft2, ft3, ft4])
-
-    def evolve_single_step(self, evolve_dt):
-        if self.j_oper2 is None:
-            prev_bra_mpdm, prev_ket_mpdm = self.latest_mps
-            prev_ket_mpdm2 = None
-        else:
-            (prev_bra_mpdm, prev_ket_mpdm), (prev_bra_mpdm, prev_ket_mpdm2) = self.latest_mps
-
-        latest_ket_mpdm = prev_ket_mpdm.evolve(self.h_mpo, evolve_dt)
-        latest_bra_mpdm = prev_bra_mpdm.evolve(self.h_mpo, evolve_dt)
-        if self.j_oper2 is None:
-            return BraKetPair(latest_bra_mpdm, latest_ket_mpdm, self.j_oper)
-        else:
-            latest_ket_mpdm2 = prev_ket_mpdm2.evolve(self.h_mpo, evolve_dt)
-            return BraKetPair(latest_bra_mpdm, latest_ket_mpdm, self.j_oper), \
-                   BraKetPair(latest_bra_mpdm, latest_ket_mpdm2, self.j_oper2)
-
-    def stop_evolve_criteria(self):
-        corr = self.auto_corr
-        if len(corr) < 10:
-            return False
-        last_corr = corr[-10:]
-        first_corr = corr[0]
-        return np.abs(last_corr.mean()) < 1e-5 * np.abs(first_corr) and last_corr.std() < 1e-5 * np.abs(first_corr)
-
-    @property
-    def auto_corr(self) -> np.ndarray:
-        """
-        Correlation function :math:`C(t)`.
-
-        :returns: 1-d numpy array containing the correlation function evaluated at each time step.
-        """
-        return np.array(self._auto_corr)
-
-    @property
-    def auto_corr_decomposition(self) -> np.ndarray:
-        r"""
-        Correlation function :math:`C(t)` decomposed into contributions from different parts
-        of the current operator. Generally, the current operator can be split into two parts:
-        current without phonon assistance and current with phonon assistance.
-        For example, if the Holstein-Peierls model is considered:
-
-        .. math::
-            \hat H = \sum_{mn}  [\epsilon_{mn} + \sum_\lambda \hbar g_{mn\lambda} \omega_\lambda
-            (b^\dagger_\lambda + b_\lambda) ] a^\dagger_m a_n
-            + \sum_\lambda \hbar \omega_\lambda b^\dagger_\lambda  b_\lambda
-
-        Then current operator without phonon assistance is defined as:
-
-        .. math::
-            \hat j_1 = \frac{e_0}{i\hbar} \sum_{mn} (R_m - R_n) \epsilon_{mn} a^\dagger_m a_n
-
-        and the current operator with phonon assistance is defined as:
-
-        .. math::
-            \hat j_2 = \frac{e_0}{i\hbar} \sum_{mn} (R_m - R_n) \hbar g_{mn\lambda} \omega_\lambda
-            (b^\dagger_\lambda + b_\lambda) a^\dagger_m a_n
-
-        With :math:`\hat j = \hat j_1 + \hat j_2`, the correlation function can be
-        decomposed into four parts:
-
-        .. math::
-            \begin{align}
-            C(t) & = \langle \hat j(t) \hat j(0) \rangle \\
-                 & = \langle ( \hat j_1(t) + \hat j_2(t) ) (\hat j_1(0) + \hat j_2(0) ) \rangle \\
-                 & = \langle \hat j_1(t) \hat j_1(0) \rangle + \langle \hat j_1(t) \hat j_2(0) \rangle
-                 + \langle \hat j_2(t) \hat j_1(0) \rangle + \langle \hat j_2(t) \hat j_2(0) \rangle
-            \end{align}
-
-        :return: :math:`n \times 4` array for the decomposed correlation function defined as above
-            where :math:`n` is the number of time steps.
-        """
-        return np.array(self._auto_corr_deomposition)
-
-    def get_dump_dict(self):
-        dump_dict = dict()
-        dump_dict["mol list"] = self.model.to_dict()
-        dump_dict["temperature"] = self.temperature.as_au()
-        dump_dict["time series"] = self.evolve_times
-        dump_dict["auto correlation"] = self.auto_corr
-        dump_dict["auto correlation decomposition"] = self.auto_corr_decomposition
-        dump_dict["mobility"] = self.calc_mobility()[1]
-        if self.properties is not None:
-            for prop_str in self.properties.prop_res.keys():
-                dump_dict[prop_str] = self.properties.prop_res[prop_str]
-
-        return dump_dict
-
-    def calc_mobility(self):
-        time_series = self.evolve_times
-        corr_real = self.auto_corr.real
-        inte = scipy.integrate.trapz(corr_real, time_series)
-        mobility_in_au = inte / self.temperature.as_au()
-        mobility = mobility_in_au / mobility2au
-        return mobility_in_au, mobility
+# -*- coding: utf-8 -*-
+
+import logging
+import os
+
+import scipy.integrate
+
+from renormalizer.mps import MpDm, Mpo, BraKetPair, ThermalProp, load_thermal_state
+from renormalizer.mps.backend import np
+from renormalizer.utils.constant import mobility2au
+from renormalizer.utils import TdMpsJob, Quantity, EvolveConfig, CompressConfig
+from renormalizer.model import Model
+from renormalizer.property import Property
+
+logger = logging.getLogger(__name__)
+
+
+class TransportKubo(TdMpsJob):
+    r"""
+    Calculate mobility via Green-Kubo formula:
+
+        .. math::
+            \mu = \frac{1}{k_B T} \int_0^\infty dt \langle \hat j (t) \hat j(0) \rangle
+            = \frac{1}{k_B T} \int_0^\infty dt C(t)
+
+    where
+
+        .. math::
+           \hat j = -\frac{i}{\hbar}[\hat P, \hat H]
+
+    and :math:`\hat P = e_0 \sum_m R_m a^\dagger_m a_m` is the polarization operator.
+
+    .. note::
+        In principle :math:`\hat H` can take any form, however only Holstein-Peierls Hamiltonian is well tested.
+
+    More explicitly, :math:`C(t)` has the form:
+
+        .. math::
+            C(t) = \textrm{Tr}\{\rho(T) e^{i \hat H t} \hat j(0) e^{- i \hat H t} \hat j (0)\}
+
+    where we have assumed :math:`\rho(T)` is normalized
+    (i.e. it is divided by the partition function :math:`\textrm{Tr}\{\rho(T)\}`).
+
+    In terms of practical implementation, it is ideal if :math:`\rho(T)` is split into two parts
+    to (hopefully) speed up calculation and minimize time evolution error:
+
+        .. math::
+            \begin{align}
+             C(t) & = \textrm{Tr}\{\rho(T) e^{i \hat H t} \hat j(0) e^{- i \hat H t} \hat j(0)\} \\
+                  & = \textrm{Tr}\{e^{-\beta \hat H} e^{i \hat H t} \hat j(0) e^{- i \hat H t} \hat j(0)\} \\
+                  & = \textrm{Tr}\{e^{-\beta \hat H / 2} e^{i \hat H t} \hat j(0) e^{- i \hat H t} \hat j(0) e^{-\beta \hat H / 2}\}
+            \end{align}
+
+    In this class, imaginary time propagation from infinite temperature to :math:`\beta/2` is firstly carried out
+    to obtain :math:`e^{-\beta \hat H / 2}`, and then real time propagation is carried out for :math:`e^{-\beta \hat H / 2}`
+    and :math:`\hat J(0) e^{-\beta \hat H / 2}` respectively to obtain :math:`e^{-\beta \hat H / 2} e^{i \hat H t}`
+    and :math:`e^{- i \hat H t} \hat j(0) e^{-\beta \hat H / 2}`. The correlation function at time :math:`t` can thus
+    be calculated via expectation calculation.
+
+    .. note::
+        Although the class is able to carry out imaginary time propagation, in practice for large scale calculation
+        it is usually preferable to carry out imaginary time propagation in another job and load the dumped initial
+        state directly in this class.
+
+    Args:
+        model (:class:`~renormalizer.model.Model`): system information.
+        temperature (:class:`~renormalizer.utils.quantity.Quantity`): simulation temperature.
+            Zero temperature is not supported.
+        distance_matrix (:class:`np.ndarray`): two-dimensional array :math:`D_{ij} = P_i - P_j` representing
+            distance between the :math:`i` th electronic degree of freedom and the :math:`j` th degree of freedom.
+            The index is the same with ``model.e_dofs``.
+            The parameter takes the role of :math:`\hat P` and can better handle periodic boundary condition.
+            The default value is ``None`` in which case the distance matrix is constructed assuming the system
+            is a one-dimensional chain.
+
+            .. note::
+                The construction of the matrix should be taken with great care if periodic boundary condition
+                is applied. Take a one-dimensional chain as an example, the distance between the leftmost site
+                and the rightmost site is :math:`\pm R` where :math:`R` is the intersite distance,
+                rather than :math:`\pm (N-1)R` where :math:`N` is the total number of electronic degrees of freedom.
+        insteps (int): steps for imaginary time propagation.
+        ievolve_config (:class:`~renormalizer.utils.configs.EvolveConfig`): config when carrying out imaginary time propagation.
+        compress_config (:class:`~renormalizer.utils.configs.CompressConfig`): config when compressing MPS.
+            Note that if TDVP based methods are chosen for time evolution, compression is necessary
+            when :math:`\hat j` is applied on :math:`e^{-\beta \hat H / 2}` but no compression is carried out
+            for :math:`e^{-\beta \hat H / 2} e^{i \hat H t}`.
+        evolve_config (:class:`~renormalizer.utils.configs.EvolveConfig`): config when carrying out real time propagation.
+        dump_dir (str): the directory for logging and numerical result output.
+        job_name (str): the name of the calculation job which determines the file name of the logging and numerical result output.
+        thermal_dump_path (str): the path to load previously thermal propagated initial state if it exists or the path
+            to dump the thermal state if it does not exist. The default value is determined by appending ``"_impdm.npz"``
+            to the path joined by ``dump_dir`` and ``job_name``.
+        properties (:class:`~renormalizer.property.property.Property`): other properties to calculate during real time evolution.
+            Currently only supports Holstein model.
+    """
+    def __init__(self, model: Model, temperature: Quantity, distance_matrix: np.ndarray = None,
+                 insteps: int=1, ievolve_config=None, compress_config=None,
+                 evolve_config=None, dump_dir: str=None, job_name: str=None,
+                 thermal_dump_path: str=None, properties: Property = None):
+        self.model = model
+        self.distance_matrix = distance_matrix
+        self.h_mpo = Mpo(model)
+        logger.info(f"Bond dim of h_mpo: {self.h_mpo.bond_dims}")
+        self._construct_current_operator()
+        if temperature == 0:
+            raise ValueError("Can't set temperature to 0.")
+        self.temperature = temperature
+
+        # imaginary time evolution config
+        if ievolve_config is None:
+            self.ievolve_config = EvolveConfig()
+            if insteps is None:
+                self.ievolve_config.adaptive = True
+                # start from a small step
+                self.ievolve_config.guess_dt = temperature.to_beta() / 1e5j
+                insteps = 1
+        else:
+            self.ievolve_config = ievolve_config
+        self.insteps = insteps
+
+        if compress_config is None:
+            logger.debug("using default compress config")
+            self.compress_config = CompressConfig()
+        else:
+            self.compress_config = compress_config
+
+        if thermal_dump_path is not None:
+            self.thermal_dump_path = thermal_dump_path
+        elif dump_dir is not None and job_name is not None:
+            self.thermal_dump_path = os.path.join(dump_dir, job_name + '_impdm.npz')
+        else:
+            self.thermal_dump_path = None
+
+        self.properties = properties
+        self._auto_corr = []
+        self._auto_corr_deomposition = []
+        super().__init__(evolve_config=evolve_config, dump_dir=dump_dir,
+                job_name=job_name)
+
+    def _construct_current_operator(self):
+        # Construct current operator. The operator is taken to be real as an optimization.
+        logger.info("constructing current operator ")
+
+        mol_num = self.model.n_edofs
+        ham_terms = self.model.ham_terms
+
+        if self.distance_matrix is None:
+            logger.info("Constructing distance matrix based on a periodic one-dimension chain.")
+            self.distance_matrix = np.arange(mol_num).reshape(-1, 1) - np.arange(mol_num).reshape(1, -1)
+            self.distance_matrix[0][-1] = 1
+            self.distance_matrix[-1][0] = -1
+
+        # current caused by pure eletronic coupling
+        holstein_current_terms = []
+        # current related to phonons
+        peierls_current_terms = []
+        # loop through the Hamiltonian to construct current operator
+        for ham_op in ham_terms:
+            # find out terms that contains two electron operators
+            # idx of the dof for the model
+            dof_op_idx1 = dof_op_idx2 = None
+            for dof_idx, dof_name in enumerate(ham_op.dofs):
+                site_idx = self.model.dof_to_siteidx[dof_name]
+                if self.model.basis[site_idx].is_electron:
+                    e_idx = self.model.e_dofs.index(dof_name)
+                    if dof_op_idx1 is None:
+                        dof_op_idx1 = dof_idx
+                        e_idx1 = e_idx
+                    elif dof_op_idx2 is None:
+                        dof_op_idx2 = dof_idx
+                        e_idx2 = e_idx
+                    else:
+                        raise ValueError(f"The model contains three-electron (or more complex) operator {ham_op}")
+                del dof_idx, dof_name
+            # two electron operators not found. Not relevant to the current operator
+            if dof_op_idx1 is None or dof_op_idx2 is None:
+                continue
+            # electron operator on the same site. Not relevant to the current operator.
+            if e_idx1 == e_idx2:
+                continue
+            # two electron operators found. Relevant to the current operator
+            # perform a bunch of sanity check
+            # at most 3 dofs are involved. More complex cases are probably supported but not tested
+            if len(ham_op.dofs) not in (2, 3):
+                raise NotImplementedError("Complex vibration potential not implemented")
+
+            # check linear coupling. More complex cases are probably supported but not tested.
+            if len(ham_op.dofs) == 3:
+                # total term idx should be 0 + 1 + 2 = 3
+                phonon_dof_idx = 3 - dof_op_idx1 - dof_op_idx2
+                assert ham_op.split_symbol[phonon_dof_idx] in (r"b^\dagger+b", "x")
+            symbol1, symbol2 = ham_op.split_symbol[dof_op_idx1], ham_op.split_symbol[dof_op_idx2]
+            if not {symbol1, symbol2} == {r"a^\dagger", "a"}:
+                raise ValueError(f"Unknown symbol: {symbol1}, {symbol2}")
+
+            # translate the term in the Hamiltonian into the term in the current operator
+            if symbol1 == r"a^\dagger":
+                factor = self.distance_matrix[e_idx1][e_idx2]
+            else:
+                factor = self.distance_matrix[e_idx2][e_idx1]
+
+            current_op = ham_op * factor
+            # Holstein terms
+            if len(ham_op.dofs) == 2:
+                holstein_current_terms.append(current_op)
+            # Peierls terms
+            else:
+                peierls_current_terms.append(current_op)
+
+        self.j_oper = Mpo(self.model, holstein_current_terms)
+        logger.info(f"current operator bond dim: {self.j_oper.bond_dims}")
+        if len(peierls_current_terms) != 0:
+            self.j_oper2  = Mpo(self.model, peierls_current_terms)
+            logger.info(f"Peierls coupling induced current operator bond dim: {self.j_oper2.bond_dims}")
+        else:
+            self.j_oper2 = None
+
+    def init_mps(self):
+        # first try to load
+        if self.thermal_dump_path is not None:
+            mpdm = load_thermal_state(self.model, self.thermal_dump_path)
+        else:
+            mpdm = None
+        # then try to calculate
+        if mpdm is None:
+            i_mpdm = MpDm.max_entangled_ex(self.model)
+            i_mpdm.compress_config = self.compress_config
+            if self.job_name is None:
+                job_name = None
+            else:
+                job_name = self.job_name + "_thermal_prop"
+            tp = ThermalProp(i_mpdm, evolve_config=self.ievolve_config, dump_dir=self.dump_dir, job_name=job_name)
+            # only propagate half beta
+            tp.evolve(None, self.insteps, self.temperature.to_beta() / 2j)
+            mpdm = tp.latest_mps
+            if self.thermal_dump_path is not None:
+                mpdm.dump(self.thermal_dump_path)
+        mpdm.compress_config = self.compress_config
+        e = mpdm.expectation(self.h_mpo)
+        self.h_mpo = Mpo(self.model, offset=Quantity(e))
+        mpdm.evolve_config = self.evolve_config
+        logger.debug("Applying current operator")
+        ket_mpdm = self.j_oper.contract(mpdm).normalize("mps_norm_to_coeff")
+        bra_mpdm = mpdm.copy()
+        if self.j_oper2 is None:
+            return BraKetPair(bra_mpdm, ket_mpdm, self.j_oper)
+        else:
+            logger.debug("Applying the second current operator")
+            ket_mpdm2 = self.j_oper2.contract(mpdm).normalize("mps_norm_to_coeff")
+            return BraKetPair(bra_mpdm, ket_mpdm, self.j_oper), BraKetPair(bra_mpdm, ket_mpdm2, self.j_oper2)
+
+    def process_mps(self, mps):
+        # add the negative sign because `self.j_oper` is taken to be real
+        if self.j_oper2 is None:
+            self._auto_corr.append(-mps.ft)
+            # calculate other properties defined in Property
+            if self.properties is not None:
+                self.properties.calc_properties_braketpair(mps)
+        else:
+            (bra_mpdm, ket_mpdm), (bra_mpdm, ket_mpdm2) = mps
+            # <J_1(t) J_1(0)>
+            ft1 = -BraKetPair(bra_mpdm, ket_mpdm, self.j_oper).ft
+            # <J_1(t) J_2(0)>
+            ft2 = -BraKetPair(bra_mpdm, ket_mpdm2, self.j_oper).ft
+            # <J_2(t) J_1(0)>
+            ft3 = -BraKetPair(bra_mpdm, ket_mpdm, self.j_oper2).ft
+            # <J_2(t) J_2(0)>
+            ft4 = -BraKetPair(bra_mpdm, ket_mpdm2, self.j_oper2).ft
+            self._auto_corr.append(ft1 + ft2 + ft3 + ft4)
+            self._auto_corr_deomposition.append([ft1, ft2, ft3, ft4])
+
+    def evolve_single_step(self, evolve_dt):
+        if self.j_oper2 is None:
+            prev_bra_mpdm, prev_ket_mpdm = self.latest_mps
+            prev_ket_mpdm2 = None
+        else:
+            (prev_bra_mpdm, prev_ket_mpdm), (prev_bra_mpdm, prev_ket_mpdm2) = self.latest_mps
+
+        latest_ket_mpdm = prev_ket_mpdm.evolve(self.h_mpo, evolve_dt)
+        latest_bra_mpdm = prev_bra_mpdm.evolve(self.h_mpo, evolve_dt)
+        if self.j_oper2 is None:
+            return BraKetPair(latest_bra_mpdm, latest_ket_mpdm, self.j_oper)
+        else:
+            latest_ket_mpdm2 = prev_ket_mpdm2.evolve(self.h_mpo, evolve_dt)
+            return BraKetPair(latest_bra_mpdm, latest_ket_mpdm, self.j_oper), \
+                   BraKetPair(latest_bra_mpdm, latest_ket_mpdm2, self.j_oper2)
+
+    def stop_evolve_criteria(self):
+        corr = self.auto_corr
+        if len(corr) < 10:
+            return False
+        last_corr = corr[-10:]
+        first_corr = corr[0]
+        return np.abs(last_corr.mean()) < 1e-5 * np.abs(first_corr) and last_corr.std() < 1e-5 * np.abs(first_corr)
+
+    @property
+    def auto_corr(self) -> np.ndarray:
+        """
+        Correlation function :math:`C(t)`.
+
+        :returns: 1-d numpy array containing the correlation function evaluated at each time step.
+        """
+        return np.array(self._auto_corr)
+
+    @property
+    def auto_corr_decomposition(self) -> np.ndarray:
+        r"""
+        Correlation function :math:`C(t)` decomposed into contributions from different parts
+        of the current operator. Generally, the current operator can be split into two parts:
+        current without phonon assistance and current with phonon assistance.
+        For example, if the Holstein-Peierls model is considered:
+
+        .. math::
+            \hat H = \sum_{mn}  [\epsilon_{mn} + \sum_\lambda \hbar g_{mn\lambda} \omega_\lambda
+            (b^\dagger_\lambda + b_\lambda) ] a^\dagger_m a_n
+            + \sum_\lambda \hbar \omega_\lambda b^\dagger_\lambda  b_\lambda
+
+        Then current operator without phonon assistance is defined as:
+
+        .. math::
+            \hat j_1 = \frac{e_0}{i\hbar} \sum_{mn} (R_m - R_n) \epsilon_{mn} a^\dagger_m a_n
+
+        and the current operator with phonon assistance is defined as:
+
+        .. math::
+            \hat j_2 = \frac{e_0}{i\hbar} \sum_{mn} (R_m - R_n) \hbar g_{mn\lambda} \omega_\lambda
+            (b^\dagger_\lambda + b_\lambda) a^\dagger_m a_n
+
+        With :math:`\hat j = \hat j_1 + \hat j_2`, the correlation function can be
+        decomposed into four parts:
+
+        .. math::
+            \begin{align}
+            C(t) & = \langle \hat j(t) \hat j(0) \rangle \\
+                 & = \langle ( \hat j_1(t) + \hat j_2(t) ) (\hat j_1(0) + \hat j_2(0) ) \rangle \\
+                 & = \langle \hat j_1(t) \hat j_1(0) \rangle + \langle \hat j_1(t) \hat j_2(0) \rangle
+                 + \langle \hat j_2(t) \hat j_1(0) \rangle + \langle \hat j_2(t) \hat j_2(0) \rangle
+            \end{align}
+
+        :return: :math:`n \times 4` array for the decomposed correlation function defined as above
+            where :math:`n` is the number of time steps.
+        """
+        return np.array(self._auto_corr_deomposition)
+
+    def get_dump_dict(self):
+        dump_dict = dict()
+        dump_dict["mol list"] = self.model.to_dict()
+        dump_dict["temperature"] = self.temperature.as_au()
+        dump_dict["time series"] = self.evolve_times
+        dump_dict["auto correlation"] = self.auto_corr
+        dump_dict["auto correlation decomposition"] = self.auto_corr_decomposition
+        dump_dict["mobility"] = self.calc_mobility()[1]
+        if self.properties is not None:
+            for prop_str in self.properties.prop_res.keys():
+                dump_dict[prop_str] = self.properties.prop_res[prop_str]
+
+        return dump_dict
+
+    def calc_mobility(self):
+        time_series = self.evolve_times
+        corr_real = self.auto_corr.real
+        inte = scipy.integrate.trapz(corr_real, time_series)
+        mobility_in_au = inte / self.temperature.as_au()
+        mobility = mobility_in_au / mobility2au
+        return mobility_in_au, mobility
```

### Comparing `renormalizer-0.0.8/renormalizer/transport/spectral_function.py` & `renormalizer-0.0.9/renormalizer/transport/spectral_function.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-# -*- coding: utf-8 -*-
-
-import logging
-
-from renormalizer.mps.backend import np
-from renormalizer.mps import Mpo, Mps
-from renormalizer.utils import TdMpsJob, Quantity, EvolveConfig, CompressConfig
-from renormalizer.model import Model, TI1DModel
-
-
-logger = logging.getLogger(__name__)
-
-
-
-class SpectralFunctionZT(TdMpsJob):
-    r"""
-    Calculate one-particle retarded Green's function at zero temperature for translational invariant one-dimensional model:
-
-    .. math::
-        iG_{ij}(t) = \langle 0 |c_i(t) c^\dagger_j | 0 \rangle
-
-    The value of the array is stored with key ``"G array"`` in the dumped output file.
-    Because of the translational invariance, there are only two dimension in this array.
-    The first dimension is :math:`t` and the second dimension is :math:`|i-j|`.
-    In k-space, :math:`iG_{ij}` is transformed to:
-
-    .. math::
-        iG_k(t) = \langle 0 |c_k(t) c^\dagger_k | 0 \rangle
-
-    and :math:`G_k(t)` is saved with key ``"Gk array"`` in the dumped output file.
-    Fourier transformation of :math:`G_k(t)` results in the spectral function:
-
-    .. math::
-        A(k, \omega) = -\frac{1}{\pi} \rm{Im} \int_0^\infty dt e^{i \omega t} G_k(t)
-
-    However, this value is not calculated directly in this class, since usually an broadening to :math:`G_k(t)`
-    is required and an optimal range of :math:`\omega` can not be determined without additional knowledge.
-
-    For finite temperature spectral function, it is recommended to use
-    thermal field dynamics and transform the Hamiltonian.
-    An example is included in the test case.
-    See J. Chem.Phys.145, 224101 (2016) and
-    Phys. Rev. Lett.123, 090402 (2019) for details.
-
-    Parameters
-    ==========
-    model : :class:`~renormalizer.model.TI1DModel`
-        system information. In principle should use :class:`~renormalizer.model.TI1DModel`.
-        Using custom :class:`~renormalizer.model.Model` is possible however
-        in this case the user should be responsible to ensure the translational invariance.
-        It is recommended to set the number of the electronic DoFs to be an even number
-        so that the :math:`k=\pi` point is well defined.
-    compress_config : :class:`~renormalizer.utils.configs.CompressConfig`
-        config when compressing MPS.
-    evolve_config : :class:`~renormalizer.utils.configs.EvolveConfig`
-        config when carrying out real time propagation.
-    dump_dir : str
-        the directory for logging and numerical result output.
-    job_name : str
-        the name of the calculation job which determines the file name of the logging and numerical result output.
-    """
-
-    def __init__(
-            self,
-            model: TI1DModel,
-            compress_config: CompressConfig = None,
-            evolve_config: EvolveConfig = None,
-            dump_dir: str = None,
-            job_name: str = None,
-    ):
-        self.model: TI1DModel = model
-        self.compress_config = compress_config
-        if self.compress_config is None:
-            self.compress_config = CompressConfig()
-        # electron-addition Green's function at different $t$ assuming translational invariance
-        self._G_array = []
-        self.e_occupations_array = []
-        self.temperature = Quantity(0)
-        super().__init__(evolve_config, dump_dir, job_name)
-
-    @property
-    def G_array(self):
-        """
-        :math:`G_{ij}(t)` as a two dimensional array.
-        The first dimension is :math:`t` and the second dimension is :math:`|i-j|`.
-
-        Returns
-        =======
-        G_array : np.ndarray
-            The Green's function array
-        """
-        return np.array(self._G_array)
-
-    def init_mps(self):
-        creation_oper = Mpo.onsite(self.model, r"a^\dagger", dof_set={self.model.e_dofs[0]})
-        gs = Mps.ground_state(self.model, False)
-        self.h_mpo = Mpo(self.model, offset=Quantity(gs.expectation(Mpo(self.model))))
-        a_ket = creation_oper.apply(gs, canonicalise=True)
-        a_ket.compress_config = self.compress_config
-        a_ket.evolve_config = self.evolve_config
-        a_ket.normalize("mps_norm_to_coeff")
-        if self.evolve_config.is_tdvp:
-            a_ket = a_ket.expand_bond_dimension(self.h_mpo)
-        return (gs, a_ket)
-
-    def process_mps(self, mps):
-        key = "a"
-        if key not in self.model.mpos:
-            a_opers = [Mpo.onsite(self.model, "a", dof_set={dof}) for dof in self.model.e_dofs]
-            self.model.mpos[key] = a_opers
-        else:
-            a_opers = self.model.mpos[key]
-
-        a_bra_mpo, a_ket_mpo = mps
-        G = a_ket_mpo.expectations(a_opers, a_bra_mpo.conj()) / 1j
-        self._G_array.append(G)
-        self.e_occupations_array.append(a_ket_mpo.e_occupations)
-
-    def evolve_single_step(self, evolve_dt):
-        prev_bra_mpdm, prev_ket_mpdm = self.latest_mps
-        latest_ket_mpdm = prev_ket_mpdm.evolve(self.h_mpo, evolve_dt)
-        return (prev_bra_mpdm, latest_ket_mpdm)
-
-    def get_dump_dict(self):
-        dump_dict = dict()
-        dump_dict['temperature'] = self.temperature.as_au()
-        dump_dict['time series'] = self.evolve_times
-        dump_dict["G array"] = self.G_array
-        ne = self.model.n_edofs
-        kpoints_distance = (2 * np.pi) / ne
-        n_kpoints = ne // 2 + 1
-        ka = (np.arange(n_kpoints) * kpoints_distance).reshape(1, 1, -1)
-        ijdiff = np.arange(ne).reshape(1, -1, 1)
-        # Green's function in k space
-        dump_dict["Gk array"] = np.sum(self.G_array.reshape(-1, ne, 1) * np.exp(1j * ka * ijdiff), axis=1)
-        dump_dict["electron occupations array"] = self.e_occupations_array
-        return dump_dict
+# -*- coding: utf-8 -*-
+
+import logging
+
+from renormalizer.mps.backend import np
+from renormalizer.mps import Mpo, Mps
+from renormalizer.utils import TdMpsJob, Quantity, EvolveConfig, CompressConfig
+from renormalizer.model import Model, TI1DModel
+
+
+logger = logging.getLogger(__name__)
+
+
+
+class SpectralFunctionZT(TdMpsJob):
+    r"""
+    Calculate one-particle retarded Green's function at zero temperature for translational invariant one-dimensional model:
+
+    .. math::
+        iG_{ij}(t) = \langle 0 |c_i(t) c^\dagger_j | 0 \rangle
+
+    The value of the array is stored with key ``"G array"`` in the dumped output file.
+    Because of the translational invariance, there are only two dimension in this array.
+    The first dimension is :math:`t` and the second dimension is :math:`|i-j|`.
+    In k-space, :math:`iG_{ij}` is transformed to:
+
+    .. math::
+        iG_k(t) = \langle 0 |c_k(t) c^\dagger_k | 0 \rangle
+
+    and :math:`G_k(t)` is saved with key ``"Gk array"`` in the dumped output file.
+    Fourier transformation of :math:`G_k(t)` results in the spectral function:
+
+    .. math::
+        A(k, \omega) = -\frac{1}{\pi} \rm{Im} \int_0^\infty dt e^{i \omega t} G_k(t)
+
+    However, this value is not calculated directly in this class, since usually an broadening to :math:`G_k(t)`
+    is required and an optimal range of :math:`\omega` can not be determined without additional knowledge.
+
+    For finite temperature spectral function, it is recommended to use
+    thermal field dynamics and transform the Hamiltonian.
+    An example is included in the test case.
+    See J. Chem.Phys.145, 224101 (2016) and
+    Phys. Rev. Lett.123, 090402 (2019) for details.
+
+    Parameters
+    ==========
+    model : :class:`~renormalizer.model.TI1DModel`
+        system information. In principle should use :class:`~renormalizer.model.TI1DModel`.
+        Using custom :class:`~renormalizer.model.Model` is possible however
+        in this case the user should be responsible to ensure the translational invariance.
+        It is recommended to set the number of the electronic DoFs to be an even number
+        so that the :math:`k=\pi` point is well defined.
+    compress_config : :class:`~renormalizer.utils.configs.CompressConfig`
+        config when compressing MPS.
+    evolve_config : :class:`~renormalizer.utils.configs.EvolveConfig`
+        config when carrying out real time propagation.
+    dump_dir : str
+        the directory for logging and numerical result output.
+    job_name : str
+        the name of the calculation job which determines the file name of the logging and numerical result output.
+    """
+
+    def __init__(
+            self,
+            model: TI1DModel,
+            compress_config: CompressConfig = None,
+            evolve_config: EvolveConfig = None,
+            dump_dir: str = None,
+            job_name: str = None,
+    ):
+        self.model: TI1DModel = model
+        self.compress_config = compress_config
+        if self.compress_config is None:
+            self.compress_config = CompressConfig()
+        # electron-addition Green's function at different $t$ assuming translational invariance
+        self._G_array = []
+        self.e_occupations_array = []
+        self.temperature = Quantity(0)
+        super().__init__(evolve_config, dump_dir, job_name)
+
+    @property
+    def G_array(self):
+        """
+        :math:`G_{ij}(t)` as a two dimensional array.
+        The first dimension is :math:`t` and the second dimension is :math:`|i-j|`.
+
+        Returns
+        =======
+        G_array : np.ndarray
+            The Green's function array
+        """
+        return np.array(self._G_array)
+
+    def init_mps(self):
+        creation_oper = Mpo.onsite(self.model, r"a^\dagger", dof_set={self.model.e_dofs[0]})
+        gs = Mps.ground_state(self.model, False)
+        self.h_mpo = Mpo(self.model, offset=Quantity(gs.expectation(Mpo(self.model))))
+        a_ket = creation_oper.apply(gs, canonicalise=True)
+        a_ket.compress_config = self.compress_config
+        a_ket.evolve_config = self.evolve_config
+        a_ket.normalize("mps_norm_to_coeff")
+        if self.evolve_config.is_tdvp:
+            a_ket = a_ket.expand_bond_dimension(self.h_mpo)
+        return (gs, a_ket)
+
+    def process_mps(self, mps):
+        key = "a"
+        if key not in self.model.mpos:
+            a_opers = [Mpo.onsite(self.model, "a", dof_set={dof}) for dof in self.model.e_dofs]
+            self.model.mpos[key] = a_opers
+        else:
+            a_opers = self.model.mpos[key]
+
+        a_bra_mpo, a_ket_mpo = mps
+        G = a_ket_mpo.expectations(a_opers, a_bra_mpo.conj()) / 1j
+        self._G_array.append(G)
+        self.e_occupations_array.append(a_ket_mpo.e_occupations)
+
+    def evolve_single_step(self, evolve_dt):
+        prev_bra_mpdm, prev_ket_mpdm = self.latest_mps
+        latest_ket_mpdm = prev_ket_mpdm.evolve(self.h_mpo, evolve_dt)
+        return (prev_bra_mpdm, latest_ket_mpdm)
+
+    def get_dump_dict(self):
+        dump_dict = dict()
+        dump_dict['temperature'] = self.temperature.as_au()
+        dump_dict['time series'] = self.evolve_times
+        dump_dict["G array"] = self.G_array
+        ne = self.model.n_edofs
+        kpoints_distance = (2 * np.pi) / ne
+        n_kpoints = ne // 2 + 1
+        ka = (np.arange(n_kpoints) * kpoints_distance).reshape(1, 1, -1)
+        ijdiff = np.arange(ne).reshape(1, -1, 1)
+        # Green's function in k space
+        dump_dict["Gk array"] = np.sum(self.G_array.reshape(-1, ne, 1) * np.exp(1j * ka * ijdiff), axis=1)
+        dump_dict["electron occupations array"] = self.e_occupations_array
+        return dump_dict
```

### Comparing `renormalizer-0.0.8/renormalizer/transport/tests/band_param.py` & `renormalizer-0.0.9/renormalizer/transport/tests/band_param.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/transport/tests/test_dynamics.py` & `renormalizer-0.0.9/renormalizer/transport/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/transport/tests/test_kubo.py` & `renormalizer-0.0.9/renormalizer/transport/tests/test_kubo.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/transport/tests/test_spectral_function.py` & `renormalizer-0.0.9/renormalizer/transport/tests/test_spectral_function.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/utils/constant.py` & `renormalizer-0.0.9/renormalizer/utils/constant.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/utils/elementop.py` & `renormalizer-0.0.9/renormalizer/utils/elementop.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/utils/log.py` & `renormalizer-0.0.9/renormalizer/utils/log.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/utils/quantity.py` & `renormalizer-0.0.9/renormalizer/utils/quantity.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/utils/qutip_utils.py` & `renormalizer-0.0.9/renormalizer/utils/qutip_utils.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/utils/rk.py` & `renormalizer-0.0.9/renormalizer/utils/rk.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/utils/tdmps.py` & `renormalizer-0.0.9/renormalizer/utils/tdmps.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/utils/tests/test_rk.py` & `renormalizer-0.0.9/renormalizer/utils/tests/test_rk.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/utils/utils.py` & `renormalizer-0.0.9/renormalizer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/vibration/tests/test_vscf.py` & `renormalizer-0.0.9/renormalizer/vibration/tests/test_vscf.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/vibration/vscf.py` & `renormalizer-0.0.9/renormalizer/vibration/vscf.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/vibronic/tests/mctdh_data.py` & `renormalizer-0.0.9/renormalizer/vibronic/tests/mctdh_data.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/vibronic/tests/test_pyr4.py` & `renormalizer-0.0.9/renormalizer/vibronic/tests/test_pyr4.py`

 * *Files identical despite different names*

### Comparing `renormalizer-0.0.8/renormalizer/vibronic/vibronic.py` & `renormalizer-0.0.9/renormalizer/vibronic/vibronic.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-from renormalizer.utils import TdMpsJob, CompressConfig, EvolveConfig
-from renormalizer.mps import Mps, Mpo
-from renormalizer.model import Model
-
-import logging
-import numpy as np
-
-logger = logging.getLogger(__name__)
-
-
-class VibronicModelDynamics(TdMpsJob):
-    r"""
-    Vibronic Hamiltonian Dynamics
-    Args:
-        model (:class:`~renormalizer.model.Model`)
-
-    """
-    
-    def __init__(
-            self, 
-            model: Model,
-            compress_config: CompressConfig = None,
-            evolve_config: EvolveConfig = None,
-            h_mpo = None,
-            mps0 = None,
-            init_condition = None, 
-            dump_mps: str = None, 
-            dump_dir: str = None,
-            job_name: str = None,
-            auto_expand: bool = False
-        ):
-
-        self.model = model
-        
-        if compress_config is None:
-            self.compress_config = CompressConfig()
-        else:
-            self.compress_config = compress_config
-        
-        if h_mpo is None:
-            self.h_mpo = Mpo(model)
-        else:
-            self.h_mpo = h_mpo
-
-        self.mps0 = mps0
-        self.init_condition = init_condition
-        self.auto_expand = auto_expand
-        
-        self.e_occupations_array = []
-        self.autocorr_array = []
-        self.energies = []
-        self.autocorr_time = []
-        self.edof_rdm = []
-        super().__init__(evolve_config=evolve_config, dump_mps=dump_mps, dump_dir=dump_dir,
-                job_name=job_name)
-    
-
-    def init_mps(self):
-        if self.mps0 is None:
-            assert self.init_condition is not None
-            init_mp = Mps.hartree_product_state(self.model, self.init_condition)
-            self.mps0 = init_mp.copy()
-        else:
-            init_mp = self.mps0.copy()
-        init_mp.compress_config = self.compress_config
-        init_mp.evolve_config = self.evolve_config
-        init_mp.model = self.model
-        if self.evolve_config.is_tdvp and self.auto_expand:
-            init_mp = init_mp.expand_bond_dimension(self.h_mpo, include_ex=False)
-        return init_mp
-
-    def evolve_single_step(self, evolve_dt):
-        old_mps = self.latest_mps
-        mpo = self.h_mpo
-        new_mps = old_mps.evolve(mpo, evolve_dt)
-        
-        return new_mps
-
-    def process_mps(self, mps):
-        # energy
-        new_energy = mps.expectation(self.h_mpo)
-        self.energies.append(new_energy)
-        logger.debug(f"Energy: {new_energy}")
-        # electron population
-        e_occupations = mps.e_occupations
-        self.e_occupations_array.append(e_occupations)
-        logger.debug(f"e occupations: {self.e_occupations_array[-1]}")
-        # electron DoF reduced density matrix
-        rdm = mps.calc_edof_rdm()
-        self.edof_rdm.append(rdm)
-        # autocorrelation function
-        if self.mps0.is_complex:
-            autocorr = self.mps0.conj().dot(mps)
-            self.autocorr_array.append(autocorr)
-            self.autocorr_time.append(self.evolve_times[-1])
-        else:
-            # make sure the latest mps is the last step mps and not ruined by
-            # evolve_single_step
-            # in tdmps latest_mps = new_mps after process_mps
-            if not np.allclose(self.evolve_times[-1], 0):
-                autocorr = mps.dot(self.latest_mps)
-                self.autocorr_array.append(autocorr)
-                self.autocorr_time.append(self.evolve_times[-1] + self.evolve_times[-2])
-            autocorr = mps.dot(mps)
-            self.autocorr_array.append(autocorr)
-            self.autocorr_time.append(self.evolve_times[-1] + self.evolve_times[-1])
-
-    def get_dump_dict(self):
-        """
-        :return: return a (ordered) dict to dump as json or npz
-        """
-        dump_dict = dict()
-        dump_dict["time series"] = list(self.evolve_times)
-        dump_dict["electron occupations array"] = self.e_occupations_array
-        dump_dict["autocorrelation function"] = self.autocorr_array
-        dump_dict["autocorrelation time"] = self.autocorr_time
-        dump_dict["energy"] = self.energies
-        dump_dict["edof_rdm"] = self.edof_rdm
-
-        return dump_dict
+from renormalizer.utils import TdMpsJob, CompressConfig, EvolveConfig
+from renormalizer.mps import Mps, Mpo
+from renormalizer.model import Model
+
+import logging
+import numpy as np
+
+logger = logging.getLogger(__name__)
+
+
+class VibronicModelDynamics(TdMpsJob):
+    r"""
+    Vibronic Hamiltonian Dynamics
+    Args:
+        model (:class:`~renormalizer.model.Model`)
+
+    """
+    
+    def __init__(
+            self, 
+            model: Model,
+            compress_config: CompressConfig = None,
+            evolve_config: EvolveConfig = None,
+            h_mpo = None,
+            mps0 = None,
+            init_condition = None, 
+            dump_mps: str = None, 
+            dump_dir: str = None,
+            job_name: str = None,
+            auto_expand: bool = False
+        ):
+
+        self.model = model
+        
+        if compress_config is None:
+            self.compress_config = CompressConfig()
+        else:
+            self.compress_config = compress_config
+        
+        if h_mpo is None:
+            self.h_mpo = Mpo(model)
+        else:
+            self.h_mpo = h_mpo
+
+        self.mps0 = mps0
+        self.init_condition = init_condition
+        self.auto_expand = auto_expand
+        
+        self.e_occupations_array = []
+        self.autocorr_array = []
+        self.energies = []
+        self.autocorr_time = []
+        self.edof_rdm = []
+        super().__init__(evolve_config=evolve_config, dump_mps=dump_mps, dump_dir=dump_dir,
+                job_name=job_name)
+    
+
+    def init_mps(self):
+        if self.mps0 is None:
+            assert self.init_condition is not None
+            init_mp = Mps.hartree_product_state(self.model, self.init_condition)
+            self.mps0 = init_mp.copy()
+        else:
+            init_mp = self.mps0.copy()
+        init_mp.compress_config = self.compress_config
+        init_mp.evolve_config = self.evolve_config
+        init_mp.model = self.model
+        if self.evolve_config.is_tdvp and self.auto_expand:
+            init_mp = init_mp.expand_bond_dimension(self.h_mpo, include_ex=False)
+        return init_mp
+
+    def evolve_single_step(self, evolve_dt):
+        old_mps = self.latest_mps
+        mpo = self.h_mpo
+        new_mps = old_mps.evolve(mpo, evolve_dt)
+        
+        return new_mps
+
+    def process_mps(self, mps):
+        # energy
+        new_energy = mps.expectation(self.h_mpo)
+        self.energies.append(new_energy)
+        logger.debug(f"Energy: {new_energy}")
+        # electron population
+        e_occupations = mps.e_occupations
+        self.e_occupations_array.append(e_occupations)
+        logger.debug(f"e occupations: {self.e_occupations_array[-1]}")
+        # electron DoF reduced density matrix
+        rdm = mps.calc_edof_rdm()
+        self.edof_rdm.append(rdm)
+        # autocorrelation function
+        if self.mps0.is_complex:
+            autocorr = self.mps0.conj().dot(mps)
+            self.autocorr_array.append(autocorr)
+            self.autocorr_time.append(self.evolve_times[-1])
+        else:
+            # make sure the latest mps is the last step mps and not ruined by
+            # evolve_single_step
+            # in tdmps latest_mps = new_mps after process_mps
+            if not np.allclose(self.evolve_times[-1], 0):
+                autocorr = mps.dot(self.latest_mps)
+                self.autocorr_array.append(autocorr)
+                self.autocorr_time.append(self.evolve_times[-1] + self.evolve_times[-2])
+            autocorr = mps.dot(mps)
+            self.autocorr_array.append(autocorr)
+            self.autocorr_time.append(self.evolve_times[-1] + self.evolve_times[-1])
+
+    def get_dump_dict(self):
+        """
+        :return: return a (ordered) dict to dump as json or npz
+        """
+        dump_dict = dict()
+        dump_dict["time series"] = list(self.evolve_times)
+        dump_dict["electron occupations array"] = self.e_occupations_array
+        dump_dict["autocorrelation function"] = self.autocorr_array
+        dump_dict["autocorrelation time"] = self.autocorr_time
+        dump_dict["energy"] = self.energies
+        dump_dict["edof_rdm"] = self.edof_rdm
+
+        return dump_dict
```

### Comparing `renormalizer-0.0.8/renormalizer.egg-info/PKG-INFO` & `renormalizer-0.0.9/renormalizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renormalizer
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/shuaigroup/Renormalizer
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![logo](./doc/source/logo.png)
```

### Comparing `renormalizer-0.0.8/renormalizer.egg-info/SOURCES.txt` & `renormalizer-0.0.9/renormalizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

