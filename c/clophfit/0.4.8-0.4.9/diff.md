# Comparing `tmp/clophfit-0.4.8.tar.gz` & `tmp/clophfit-0.4.9.tar.gz`

## Comparing `clophfit-0.4.8.tar` & `clophfit-0.4.9.tar`

### file list

```diff
@@ -1,200 +1,200 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.4.8/.codespellrc
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.4.8/.darglint
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 clophfit-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.4.8/.python-version
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.4.8/.readthedocs.yml
--rw-r--r--   0        0        0    13095 2020-02-02 00:00:00.000000 clophfit-0.4.8/CHANGELOG.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 clophfit-0.4.8/CONTRIBUTING.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.4.8/bandit.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.4.8/cz_customize_info.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/dependabot.yml
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/workflows/cd.yml
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/Makefile
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/conf.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/.gitkeep
--rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f1.png
--rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f2.png
--rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f3.png
--rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f4.png
--rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f5.png
--rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f6.png
--rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f7.png
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/csvtable.png
--rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/emcee-01.png
--rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/emcee-02.png
--rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/emcee-11.png
--rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/emcee-12.png
--rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/f01.png
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/file.png
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit1.png
--rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit2.png
--rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit3.png
--rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit4.png
--rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit5.png
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit6.png
--rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit7.png
--rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit0.png
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit1.png
--rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit2.png
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit3.png
--rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit_np.r_.png
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit1.png
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit2.png
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit3.png
--rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit4.png
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit5.png
--rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel1.png
--rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel2.png
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel3.png
--rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel4.png
--rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel5.png
--rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel6.png
--rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel_H04.png
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/note_file.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/r_bs.png
--rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P-lmodel1.png
--rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P-lmodel2.png
--rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R1.png
--rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R2.png
--rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R3.png
--rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R4.png
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R5.png
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R6.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/rpy_bs.png
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/api/api.rst
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/api/prtecan.uml.rst
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/misc/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/misc/CONTRIBUTING.md -> ../../CONTRIBUTING.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/misc/license.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/misc/misc.rst
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/references/description.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/references/references.rst
--rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/prtecan.ipynb
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/usage.org
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/usage.rst
--rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/usage2.org
--rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/usage2.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/__init__.py
--rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/py.typed
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/binding/__init__.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/binding/fitting.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/dil_buffer.py
--rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/dil_correction.py
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/fit_rpy.py
--rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/fit_titration.py
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/fit_titration_global.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/merge.py
--rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/plot_tecan.py
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/fit.tecan
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/fit.tecan.cl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/new_sort_K.sh
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_all
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_e2
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_lib
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_lib2
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_s202n
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_v224q
--rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/w_ave.sh
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/prtecan/__init__.py
--rw-r--r--   0        0        0    51805 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/prtecan/prtecan.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/conftest.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/test_binding.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/test_cli.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/test_oldscripts.py
--rw-r--r--   0        0        0    26316 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/test_prtecan.py
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_100.xls
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_150.xls
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_20.xls
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_5.78.xls
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_50.xls
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_6.38.xls
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_6.83.xls
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_7.24.xls
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_7.67.xls
--rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_8.23.xls
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_8.82.xls
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_9.31.xls
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290513_5.5.xls
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290513_5.5_bad.xls
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290513_7.2.xls
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290513_8.8.xls
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/list.cl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/list.cl20
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/list.pH
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/list.pH2
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/200214 pH data.ods
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl1_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl2_200214.xls
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl3_200214.xls
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl4_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl5_200214.xls
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl6_200214.xls
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl7_200214.xls
--rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl8_200214.xls
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/additions.cl
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/additions.pH
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/fit0-1.csv
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/fit0.csv
--rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/fit1-1.csv
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/fit1.csv
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/list.cl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/list.pH
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH5.0_200214.xls
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH5.8_200214.xls
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH6.5_200214.xls
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH7.1_200214.xls
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH7.6_200214.xls
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH8.3_200214.xls
--rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH9.1_200214.xls
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/scheme.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/scheme0.txt
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
--rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/exceptions/84wells_290212_20.xlsx
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/exceptions/88wells_290212_20.xlsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/A01-20140311a.dat
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/A01.dat
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/A11.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/B01.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/H04.dat
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/NTT-A04-Cl_note
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/copyIP.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/ratio2P.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/w.txt
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_A.csv
--rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_A.png
--rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_B.csv
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_B.png
--rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_C.csv
--rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_C.png
--rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_D.csv
--rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_D.png
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_E.csv
--rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_E.png
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_F.csv
--rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_F.png
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/Cl/A11-failed.dat
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/Cl/B05-20130628-cor.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/pH/B01-failed.dat
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/pH/D05.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/pH/H04-with_nan.dat
--rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/k/D05.dat-bs.png
--rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/k/D05.dat.png
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/global/Cl/B05-20130628-cor.dat.png
--rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/global/pH/D05.dat.png
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.4.8/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.4.8/LICENSE.txt
--rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 clophfit-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/README.md
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 clophfit-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.4.9/.codespellrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.4.9/.darglint
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 clophfit-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.4.9/.python-version
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.4.9/.readthedocs.yml
+-rw-r--r--   0        0        0    13365 2020-02-02 00:00:00.000000 clophfit-0.4.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 clophfit-0.4.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.4.9/bandit.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.4.9/cz_customize_info.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.4.9/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/Makefile
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/conf.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/.gitkeep
+-rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f1.png
+-rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f2.png
+-rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f3.png
+-rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f4.png
+-rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f5.png
+-rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f6.png
+-rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/bs_pd_f7.png
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/csvtable.png
+-rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/emcee-01.png
+-rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/emcee-02.png
+-rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/emcee-11.png
+-rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/emcee-12.png
+-rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/f01.png
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/file.png
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit1.png
+-rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit2.png
+-rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit3.png
+-rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit4.png
+-rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit5.png
+-rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit6.png
+-rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/gR_fit7.png
+-rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit0.png
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit1.png
+-rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit2.png
+-rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit3.png
+-rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/glmfit_np.r_.png
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit1.png
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit2.png
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit3.png
+-rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit4.png
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmfit5.png
+-rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel1.png
+-rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel2.png
+-rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel3.png
+-rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel4.png
+-rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel5.png
+-rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel6.png
+-rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/lmodel_H04.png
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/note_file.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/r_bs.png
+-rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P-lmodel1.png
+-rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P-lmodel2.png
+-rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R1.png
+-rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R2.png
+-rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R3.png
+-rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R4.png
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R5.png
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/ratio2P_R6.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/_static/rpy_bs.png
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/api/api.rst
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/api/prtecan.uml.rst
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/misc/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/misc/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/misc/license.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/misc/misc.rst
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/references/description.rst
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/references/references.rst
+-rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/prtecan.ipynb
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/usage.org
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/usage.rst
+-rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/usage2.org
+-rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/tutorials/usage2.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/__init__.py
+-rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/py.typed
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/binding/__init__.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/binding/fitting.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/dil_buffer.py
+-rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/dil_correction.py
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/fit_rpy.py
+-rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/fit_titration.py
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/fit_titration_global.py
+-rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/merge.py
+-rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/plot_tecan.py
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/fit.tecan
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/fit.tecan.cl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/new_sort_K.sh
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_all
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_e2
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_lib
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_lib2
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_s202n
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/sum_v224q
+-rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/old/bash/w_ave.sh
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/prtecan/__init__.py
+-rw-r--r--   0        0        0    51839 2020-02-02 00:00:00.000000 clophfit-0.4.9/src/clophfit/prtecan/prtecan.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/conftest.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/test_binding.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/test_cli.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/test_oldscripts.py
+-rw-r--r--   0        0        0    26589 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/test_prtecan.py
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_100.xls
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_150.xls
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_20.xls
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_5.78.xls
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_50.xls
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_6.38.xls
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_6.83.xls
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_7.24.xls
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_7.67.xls
+-rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_8.23.xls
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_8.82.xls
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290212_9.31.xls
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290513_5.5.xls
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290513_5.5_bad.xls
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290513_7.2.xls
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/290513_8.8.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/list.cl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/list.cl20
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/list.pH
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/list.pH2
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/200214 pH data.ods
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl1_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl2_200214.xls
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl3_200214.xls
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl4_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl5_200214.xls
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl6_200214.xls
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl7_200214.xls
+-rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/NaCl8_200214.xls
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/additions.cl
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/additions.pH
+-rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/fit0-1.csv
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/fit0.csv
+-rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/fit1-1.csv
+-rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/fit1.csv
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/list.cl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/list.pH
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH5.0_200214.xls
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH5.8_200214.xls
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH6.5_200214.xls
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH7.1_200214.xls
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH7.6_200214.xls
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH8.3_200214.xls
+-rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/pH9.1_200214.xls
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/scheme.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/140220/scheme0.txt
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/exceptions/84wells_290212_20.xlsx
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/Tecan/exceptions/88wells_290212_20.xlsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/A01-20140311a.dat
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/A01.dat
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/A11.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/B01.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/H04.dat
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/NTT-A04-Cl_note
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/copyIP.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/ratio2P.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/w.txt
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_A.csv
+-rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_A.png
+-rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_B.csv
+-rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_B.png
+-rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_C.csv
+-rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_C.png
+-rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_D.csv
+-rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_D.png
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_E.csv
+-rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_E.png
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_F.csv
+-rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/Meas/A04 Cl_F.png
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/Cl/A11-failed.dat
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/Cl/B05-20130628-cor.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/pH/B01-failed.dat
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/pH/D05.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/global/pH/H04-with_nan.dat
+-rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/k/D05.dat-bs.png
+-rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/k/D05.dat.png
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/global/Cl/B05-20130628-cor.dat.png
+-rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.4.9/tests/data/output/global/pH/D05.dat.png
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.4.9/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.4.9/LICENSE.txt
+-rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 clophfit-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 clophfit-0.4.9/docs/README.md
+-rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 clophfit-0.4.9/PKG-INFO
```

### Comparing `clophfit-0.4.8/.pre-commit-config.yaml` & `clophfit-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/CHANGELOG.md` & `clophfit-0.4.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## v0.4.9 (2023-05-03)
+
+### Build
+
+- bump sphinx from 6.2.1 to 7.0.0 (#236)
+- bump ruff from 0.0.263 to 0.0.264 (#243)
+- bump autodocsumm from 0.2.10 to 0.2.11 (#242)
+- update lmfit requirement from <1.2.1 to <1.2.2 (#241)
+
+### Refactor
+
+- update typeguard to 4.0.0rc5
+
 ## v0.4.8 (2023-05-02)
 
 ### Docs
 
 - Lint README.md with markdownlint-cli
 
 ### Build
```

### Comparing `clophfit-0.4.8/CONTRIBUTING.md` & `clophfit-0.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/cz_customize_info.txt` & `clophfit-0.4.9/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/.github/workflows/cd.yml` & `clophfit-0.4.9/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/.github/workflows/ci.yml` & `clophfit-0.4.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/.github/workflows/docs.yml` & `clophfit-0.4.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/Makefile` & `clophfit-0.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/conf.py` & `clophfit-0.4.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "ClopHfit"
 copyright = "2021, Daniele Arosio"  # noqa: A001
 author = "Daniele Arosio"
 
 # The full version, including alpha/beta/rc tags
-release = "0.4.8"
+release = "0.4.9"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `clophfit-0.4.8/docs/make.bat` & `clophfit-0.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/bs_pd_f1.png` & `clophfit-0.4.9/docs/_static/bs_pd_f1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/bs_pd_f2.png` & `clophfit-0.4.9/docs/_static/bs_pd_f2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/bs_pd_f3.png` & `clophfit-0.4.9/docs/_static/bs_pd_f3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/bs_pd_f4.png` & `clophfit-0.4.9/docs/_static/bs_pd_f4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/bs_pd_f5.png` & `clophfit-0.4.9/docs/_static/bs_pd_f5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/bs_pd_f6.png` & `clophfit-0.4.9/docs/_static/bs_pd_f6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/bs_pd_f7.png` & `clophfit-0.4.9/docs/_static/bs_pd_f7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/csvtable.png` & `clophfit-0.4.9/docs/_static/csvtable.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/emcee-01.png` & `clophfit-0.4.9/docs/_static/emcee-01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/emcee-02.png` & `clophfit-0.4.9/docs/_static/emcee-02.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/emcee-11.png` & `clophfit-0.4.9/docs/_static/emcee-11.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/emcee-12.png` & `clophfit-0.4.9/docs/_static/emcee-12.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/f01.png` & `clophfit-0.4.9/docs/_static/f01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/file.png` & `clophfit-0.4.9/docs/_static/file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/gR_fit1.png` & `clophfit-0.4.9/docs/_static/gR_fit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/gR_fit2.png` & `clophfit-0.4.9/docs/_static/gR_fit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/gR_fit3.png` & `clophfit-0.4.9/docs/_static/gR_fit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/gR_fit4.png` & `clophfit-0.4.9/docs/_static/gR_fit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/gR_fit5.png` & `clophfit-0.4.9/docs/_static/gR_fit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/gR_fit6.png` & `clophfit-0.4.9/docs/_static/gR_fit6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/gR_fit7.png` & `clophfit-0.4.9/docs/_static/gR_fit7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/glmfit0.png` & `clophfit-0.4.9/docs/_static/glmfit0.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/glmfit1.png` & `clophfit-0.4.9/docs/_static/glmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/glmfit2.png` & `clophfit-0.4.9/docs/_static/glmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/glmfit3.png` & `clophfit-0.4.9/docs/_static/glmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/glmfit_np.r_.png` & `clophfit-0.4.9/docs/_static/glmfit_np.r_.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmfit1.png` & `clophfit-0.4.9/docs/_static/lmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmfit2.png` & `clophfit-0.4.9/docs/_static/lmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmfit3.png` & `clophfit-0.4.9/docs/_static/lmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmfit4.png` & `clophfit-0.4.9/docs/_static/lmfit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmfit5.png` & `clophfit-0.4.9/docs/_static/lmfit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmodel1.png` & `clophfit-0.4.9/docs/_static/lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmodel2.png` & `clophfit-0.4.9/docs/_static/lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmodel3.png` & `clophfit-0.4.9/docs/_static/lmodel3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmodel4.png` & `clophfit-0.4.9/docs/_static/lmodel4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmodel5.png` & `clophfit-0.4.9/docs/_static/lmodel5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmodel6.png` & `clophfit-0.4.9/docs/_static/lmodel6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/lmodel_H04.png` & `clophfit-0.4.9/docs/_static/lmodel_H04.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/note_file.png` & `clophfit-0.4.9/docs/_static/note_file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/r_bs.png` & `clophfit-0.4.9/docs/_static/r_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/ratio2P-lmodel1.png` & `clophfit-0.4.9/docs/_static/ratio2P-lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/ratio2P-lmodel2.png` & `clophfit-0.4.9/docs/_static/ratio2P-lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/ratio2P_R1.png` & `clophfit-0.4.9/docs/_static/ratio2P_R1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/ratio2P_R2.png` & `clophfit-0.4.9/docs/_static/ratio2P_R2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/ratio2P_R3.png` & `clophfit-0.4.9/docs/_static/ratio2P_R3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/ratio2P_R4.png` & `clophfit-0.4.9/docs/_static/ratio2P_R4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/ratio2P_R5.png` & `clophfit-0.4.9/docs/_static/ratio2P_R5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/ratio2P_R6.png` & `clophfit-0.4.9/docs/_static/ratio2P_R6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/_static/rpy_bs.png` & `clophfit-0.4.9/docs/_static/rpy_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/api/prtecan.uml.rst` & `clophfit-0.4.9/docs/api/prtecan.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/references/description.rst` & `clophfit-0.4.9/docs/references/description.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/tutorials/prtecan.ipynb` & `clophfit-0.4.9/docs/tutorials/prtecan.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/tutorials/usage.org` & `clophfit-0.4.9/docs/tutorials/usage.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/tutorials/usage.rst` & `clophfit-0.4.9/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/tutorials/usage2.org` & `clophfit-0.4.9/docs/tutorials/usage2.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/docs/tutorials/usage2.rst` & `clophfit-0.4.9/docs/tutorials/usage2.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/__main__.py` & `clophfit-0.4.9/src/clophfit/__main__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/binding/fitting.py` & `clophfit-0.4.9/src/clophfit/binding/fitting.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/old/dil_buffer.py` & `clophfit-0.4.9/src/clophfit/old/dil_buffer.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/old/dil_correction.py` & `clophfit-0.4.9/src/clophfit/old/dil_correction.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/old/fit_rpy.py` & `clophfit-0.4.9/src/clophfit/old/fit_rpy.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/old/fit_titration.py` & `clophfit-0.4.9/src/clophfit/old/fit_titration.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/old/fit_titration_global.py` & `clophfit-0.4.9/src/clophfit/old/fit_titration_global.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/old/merge.py` & `clophfit-0.4.9/src/clophfit/old/merge.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/old/plot_tecan.py` & `clophfit-0.4.9/src/clophfit/old/plot_tecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/old/bash/w_ave.sh` & `clophfit-0.4.9/src/clophfit/old/bash/w_ave.sh`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/prtecan/__init__.py` & `clophfit-0.4.9/src/clophfit/prtecan/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/src/clophfit/prtecan/prtecan.py` & `clophfit-0.4.9/src/clophfit/prtecan/prtecan.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 """
 from __future__ import annotations
 
 import hashlib
 import itertools
 import warnings
-from collections import defaultdict
 from contextlib import suppress
 from dataclasses import InitVar
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
 from typing import Callable
 from typing import Sequence
@@ -248,16 +247,16 @@
 
     Returns
     -------
     NDArray[float]
         Dilution correction vector.
     """
     volumes = np.cumsum(additions)
-    correction = volumes / volumes[0]
-    return np.array(correction)
+    corrections: NDArray[np.float_] = volumes / volumes[0]
+    return corrections
 
 
 @dataclass
 class Labelblock:
     """Parse a label block within a Tecan file.
 
     Parameters
@@ -561,42 +560,39 @@
     def __post_init__(self) -> None:
         """Create common metadata and data."""
         if not self.allequal:
             self.allequal = all(
                 self.labelblocks[0] == lb for lb in self.labelblocks[1:]
             )
         if self.allequal:
-            self._data = defaultdict(list)
+            self._data = {}
             for key in self.labelblocks[0].data:
-                for lb in self.labelblocks:
-                    self._data[key].append(lb.data[key])
+                self._data[key] = [lb.data[key] for lb in self.labelblocks]
         # labelblocks that can be merged only after normalization
         elif all(self.labelblocks[0].__almost_eq__(lb) for lb in self.labelblocks[1:]):
-            self._data_norm = defaultdict(list)
+            self._data_norm = {}
             for key in self.labelblocks[0].data:
-                for lb in self.labelblocks:
-                    self._data_norm[key].append(lb.data_norm[key])
+                self._data_norm[key] = [lb.data_norm[key] for lb in self.labelblocks]
         else:
             msg = "Creation of labelblock group failed."
             raise ValueError(msg)
         self.metadata = merge_md([lb.metadata for lb in self.labelblocks])
 
     @property
     def data(self) -> dict[str, list[float]] | None:
         """Return None or data."""
         return self._data
 
     @property
     def data_norm(self) -> dict[str, list[float]]:
         """Normalize data by number of flashes, integration time and gain."""
         if self._data_norm is None:
-            self._data_norm = defaultdict(list)
+            self._data_norm = {}
             for key in self.labelblocks[0].data:
-                for lb in self.labelblocks:
-                    self._data_norm[key].append(lb.data_norm[key])
+                self._data_norm[key] = [lb.data_norm[key] for lb in self.labelblocks]
         return self._data_norm
 
     @property
     def buffer_wells(self) -> list[str] | None:
         """List of buffer wells."""
         return self._buffer_wells
 
@@ -777,14 +773,15 @@
         return tecanfiles, conc
 
     @property
     def additions(self) -> list[float] | None:
         """List of initial volume followed by additions."""
         return self._additions
 
+    # Here there is not any check on the validity of additions (e.g. length).
     @additions.setter
     def additions(self, additions: list[float]) -> None:
         self._additions = additions
         self._dil_corr = dilution_correction(additions)
         self._data_dilutioncorrected = None
         self._data_dilutioncorrected_norm = None
 
@@ -807,28 +804,31 @@
         self._data_dilutioncorrected_norm = None
 
     @property
     def data_dilutioncorrected(self) -> list[dict[str, list[float]] | None] | None:
         """Buffer subtracted data."""
         if self._data_dilutioncorrected is None and self.additions:
             self._data_dilutioncorrected = [
-                {k: v * self._dil_corr for k, v in lbg.data_buffersubtracted.items()}
+                {
+                    k: (np.array(v) * self._dil_corr).tolist()
+                    for k, v in lbg.data_buffersubtracted.items()
+                }
                 if lbg.data_buffersubtracted
                 else None
                 for lbg in self.labelblocksgroups
             ]
         return self._data_dilutioncorrected
 
     @property
     def data_dilutioncorrected_norm(self) -> list[dict[str, list[float]]] | None:
         """Buffer subtracted data."""
         if self._data_dilutioncorrected_norm is None and self.additions:
             self._data_dilutioncorrected_norm = [
                 {
-                    k: v * self._dil_corr
+                    k: (np.array(v) * self._dil_corr).tolist()
                     for k, v in lbg.data_buffersubtracted_norm.items()
                 }
                 for lbg in self.labelblocksgroups
             ]
         return self._data_dilutioncorrected_norm
 
     def export_data(self, out_folder: Path) -> None:
```

### Comparing `clophfit-0.4.8/tests/test_binding.py` & `clophfit-0.4.9/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/test_cli.py` & `clophfit-0.4.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/test_oldscripts.py` & `clophfit-0.4.9/tests/test_oldscripts.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/test_prtecan.py` & `clophfit-0.4.9/tests/test_prtecan.py`

 * *Files 12% similar despite different names*

```diff
@@ -94,21 +94,19 @@
     """Test labelblock class."""
 
     @pytest.fixture(autouse=True)
     def _init(self) -> None:
         """Simulate csvl with 2 labelblocks."""
         csvl = prtecan.read_xls(data_tests / "140220/pH6.5_200214.xls")
         idxs = prtecan.lookup_listoflines(csvl)
-        lb0 = prtecan.Labelblock(csvl[idxs[0] : idxs[1]])
-        lb1 = prtecan.Labelblock(csvl[idxs[1] :])
-        lb0.buffer_wells = ["D01", "D12", "E01", "E12"]
-        lb1.buffer_wells = ["D01", "D12", "E01", "E12"]
         # pylint: disable=W0201
-        self.lb0 = lb0
-        self.lb1 = lb1
+        self.lb0 = prtecan.Labelblock(csvl[idxs[0] : idxs[1]])
+        self.lb1 = prtecan.Labelblock(csvl[idxs[1] :])
+        self.lb0.buffer_wells = ["D01", "D12", "E01", "E12"]
+        self.lb1.buffer_wells = ["D01", "D12", "E01", "E12"]
 
     def test_metadata(self) -> None:
         """It parses "Temperature" metadata."""
         assert self.lb0.metadata["Temperature"].value == 25.6
         assert self.lb1.metadata["Temperature"].value == 25.3
 
     def test_data(self) -> None:
@@ -282,31 +280,33 @@
         assert self.lbg1.labelblocks[1].metadata["Gain"].value == 99
         # Common metadata.
         assert self.lbg0.metadata["Gain"].value == 94
         assert self.lbg0.metadata["Number of Flashes"].value == 10
 
     def test_data(self) -> None:
         """Merge data."""
-        assert self.lbg0.data["A01"] == [18713, 17088]  # type: ignore
-        assert self.lbg0.data["H12"] == [28596, 25771]  # type: ignore
+        assert self.lbg0.data is not None
+        assert self.lbg0.data["A01"] == [18713, 17088]
+        assert self.lbg0.data["H12"] == [28596, 25771]
         assert self.lbg1.data is None
 
     def test_data_normalized(self) -> None:
         """Merge data_normalized."""
         np.testing.assert_almost_equal(
             self.lbg1.data_norm["H12"], [693.980, 714.495], 3
         )
         np.testing.assert_almost_equal(
             self.lbg0.data_norm["A01"], [995.372, 908.936], 3
         )
 
     def test_data_buffersubtracted(self) -> None:
         """Merge data_buffersubtracted."""
+        assert self.lbg0.data_buffersubtracted is not None
         np.testing.assert_almost_equal(
-            self.lbg0.data_buffersubtracted["B07"], [7069, 5716.7], 1  # type: ignore
+            self.lbg0.data_buffersubtracted["B07"], [7069, 5716.7], 1
         )
         assert self.lbg1.data_buffersubtracted is None
 
     def test_data_buffersubtracted_norm(self) -> None:
         """Merge data_buffersubtracted."""
         np.testing.assert_almost_equal(
             self.lbg0.data_buffersubtracted_norm["B07"], [376.01, 304.08], 2
@@ -344,18 +344,20 @@
             lbg0 = tfg.labelblocksgroups[0]
             lbg1 = tfg.labelblocksgroups[1]
             # metadata
             assert lbg0.metadata["Number of Flashes"].value == 10.0
             assert lbg1.metadata["Gain"].value == 98.0
             # data normalized ... enough in lbg
             # data
-            assert lbg0.data["A01"] == [18713, 17088]  # type: ignore
-            assert lbg0.data["H12"] == [28596, 25771]  # type: ignore
-            assert lbg1.data["A01"] == [7878, 8761]  # type: ignore
-            assert lbg1.data["H12"] == [14226, 13602]  # type: ignore
+            assert lbg0.data is not None
+            assert lbg0.data["A01"] == [18713, 17088]
+            assert lbg0.data["H12"] == [28596, 25771]
+            assert lbg1.data is not None
+            assert lbg1.data["A01"] == [7878, 8761]
+            assert lbg1.data["H12"] == [14226, 13602]
 
     class TestAlmostEqLbgs:
         """Test TfG when 1 LbG equal and a second with almost equal labelblocks."""
 
         @pytest.fixture(autouse=True)
         def _init(self) -> None:  # pragma: no cover
             """Initialize Tfg when 1 LbG equal and a second with almost equal labelblocks."""
@@ -378,16 +380,17 @@
         def test_labelblocksgroups(self) -> None:
             """Generate 1 LbG with .data and .metadata."""
             lbg0 = self.group.labelblocksgroups[0]
             # metadata
             assert lbg0.metadata["Number of Flashes"].value == 10.0
             assert lbg0.metadata["Gain"].value == 94
             # data
-            assert lbg0.data["A01"] == [18713.0, 17088.0, 17123.0]  # type: ignore
-            assert lbg0.data["H12"] == [28596.0, 25771.0, 28309.0]  # type: ignore
+            assert lbg0.data is not None
+            assert lbg0.data["A01"] == [18713.0, 17088.0, 17123.0]
+            assert lbg0.data["H12"] == [28596.0, 25771.0, 28309.0]
 
         def test_mergeable_labelblocksgroups(self) -> None:
             """Generate 1 Lbg only with .data_normalized and only common .metadata."""
             lbg1 = self.group.labelblocksgroups[1]
             # metadata
             assert lbg1.metadata["Number of Flashes"].value == 10.0
             assert lbg1.metadata.get("Gain") is None
@@ -425,16 +428,17 @@
         def test_labelblocksgroups(self) -> None:
             """Generates 1 LbG with .data and .metadata."""
             lbg = self.group.labelblocksgroups[0]
             # metadata
             assert lbg.metadata["Number of Flashes"].value == 10.0
             assert lbg.metadata["Gain"].value == 93.0
             # data
-            assert lbg.data["A01"] == [6289, 6462, 6465]  # type: ignore
-            assert lbg.data["H12"] == [4477, 4705, 4918]  # type: ignore
+            assert lbg.data is not None
+            assert lbg.data["A01"] == [6289, 6462, 6465]
+            assert lbg.data["H12"] == [4477, 4705, 4918]
 
     class TestFailToMerge:
         """Test TfG without mergeable labelblocks."""
 
         def test_raise_exception(self) -> None:
             """Raise Exception when there is no way to build labelblocksGroup."""
             filenames = ["290513_5.5.xls", "290513_5.5_bad.xls"]
@@ -462,24 +466,27 @@
         lbg0 = self.tit_ph.labelblocksgroups[0]
         lbg1 = self.tit_ph.labelblocksgroups[1]
         # metadata
         assert lbg0.metadata["Number of Flashes"].value == 10.0
         # pH9.3 is 93 Optimal not Manual
         assert lbg1.metadata["Gain"] == prtecan.Metadata(93.0)
         # data
-        assert lbg0.data["A01"][::2] == [30344, 31010, 33731, 37967]  # type: ignore
-        assert lbg1.data["A01"][1::2] == [9165, 15591, 20788, 22534]  # type: ignore
-        assert lbg0.data["H12"][1::2] == [20888, 21711, 23397, 25045]  # type: ignore
-        assert lbg1.data["H12"] == [4477, 5849, 7165, 8080, 8477, 8822, 9338, 9303]  # type: ignore
+        assert lbg0.data is not None
+        assert lbg1.data is not None
+        assert lbg0.data["A01"][::2] == [30344, 31010, 33731, 37967]
+        assert lbg1.data["A01"][1::2] == [9165, 15591, 20788, 22534]
+        assert lbg0.data["H12"][1::2] == [20888, 21711, 23397, 25045]
+        assert lbg1.data["H12"] == [4477, 5849, 7165, 8080, 8477, 8822, 9338, 9303]
 
     def test_labelblocksgroups_cl(self) -> None:
         """It reads labelblocksgroups data for Cl too."""
         lbg = self.tit_cl.labelblocksgroups[0]
-        assert lbg.data["A01"] == [6462, 6390, 6465, 6774]  # type: ignore
-        assert lbg.data["H12"] == [4705, 4850, 4918, 5007]  # type: ignore
+        assert lbg.data is not None
+        assert lbg.data["A01"] == [6462, 6390, 6465, 6774]
+        assert lbg.data["H12"] == [4705, 4850, 4918, 5007]
 
     def test_export_data(self, tmp_path: Path) -> None:
         """It exports titrations data to files e.g. "A01.dat"."""
         self.tit_ph.export_data(tmp_path)
         a01 = pd.read_csv(tmp_path / "dat/A01.dat")
         h12 = pd.read_csv(tmp_path / "dat/H12.dat")
         assert a01["y1"].tolist()[1::2] == [30072, 32678, 36506, 37725]
@@ -536,43 +543,46 @@
         lbg0 = self.titan.labelblocksgroups[0]
         lbg1 = self.titan.labelblocksgroups[1]
         np.testing.assert_almost_equal(
             lbg0.data_norm["E01"][::2],
             [601.72, 641.505, 674.355, 706.774],
             3,
         )
-        if lbg0.data:
-            assert lbg0.data["E01"][::2] == [11192.0, 11932.0, 12543.0, 13146.0]
-        if lbg0.data_buffersubtracted:
-            np.testing.assert_array_equal(
-                lbg0.data_buffersubtracted["A12"][::3],
-                [8084.5, 16621.75, 13775.0],
-            )
+        assert lbg0.data is not None
+        assert lbg0.data["E01"][::2] == [11192.0, 11932.0, 12543.0, 13146.0]
+        assert lbg0.data_buffersubtracted is not None
+        np.testing.assert_array_equal(
+            lbg0.data_buffersubtracted["A12"][::3], [8084.5, 16621.75, 13775.0]
+        )
+        assert lbg1.data_buffersubtracted is not None
         np.testing.assert_array_equal(
-            lbg1.data_buffersubtracted["A12"][::3],  # type: ignore
-            [9758.25, 1334.0, 283.5],
+            lbg1.data_buffersubtracted["A12"][::3], [9758.25, 1334.0, 283.5]
         )
 
     def test_dilution_correction(self) -> None:
         """It applies dilution correction read from file listing additions."""
-        np.testing.assert_array_equal(self.titan.additions, [100, 2, 2, 2, 2, 2, 2])  # type: ignore
+        assert self.titan.additions is not None
+        np.testing.assert_array_equal(self.titan.additions, [100, 2, 2, 2, 2, 2, 2])
+        assert self.titan.data_dilutioncorrected is not None
+        assert self.titan.data_dilutioncorrected[1] is not None
         np.testing.assert_almost_equal(
-            self.titan.data_dilutioncorrected[1]["A12"],  # type: ignore
+            self.titan.data_dilutioncorrected[1]["A12"],
             [9758.25, 7524.795, 3079.18, 1414.04, 641.79, 402.325, 317.52],
         )
 
     def test_data_dilutioncorrected_norma(self) -> None:
         """It normalizes data."""
+        assert self.titan.data_dilutioncorrected_norm is not None
         np.testing.assert_almost_equal(
-            self.titan.data_dilutioncorrected_norm[0]["A12"][::2],  # type: ignore
+            self.titan.data_dilutioncorrected_norm[0]["A12"][::2],
             [434.65, 878.73, 975.58, 829.46],
             2,
         )
         np.testing.assert_almost_equal(
-            self.titan.data_dilutioncorrected_norm[1]["A12"][::2],  # type: ignore
+            self.titan.data_dilutioncorrected_norm[1]["A12"][::2],
             [871.272, 274.927, 57.303, 28.35],
             3,
         )
 
     def test_keys(self) -> None:
         """It gets well positions for ctrl and unknown samples."""
         assert set(self.titan.scheme.names) == {"NTT", "G03", "V224Q", "S202N"}
```

### Comparing `clophfit-0.4.8/tests/Tecan/290212_100.xls` & `clophfit-0.4.9/tests/Tecan/290212_100.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_150.xls` & `clophfit-0.4.9/tests/Tecan/290212_150.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_20.xls` & `clophfit-0.4.9/tests/Tecan/290212_20.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_5.78.xls` & `clophfit-0.4.9/tests/Tecan/290212_5.78.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_50.xls` & `clophfit-0.4.9/tests/Tecan/290212_50.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_6.38.xls` & `clophfit-0.4.9/tests/Tecan/290212_6.38.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_6.83.xls` & `clophfit-0.4.9/tests/Tecan/290212_6.83.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_7.24.xls` & `clophfit-0.4.9/tests/Tecan/290212_7.24.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_7.67.xls` & `clophfit-0.4.9/tests/Tecan/290212_7.67.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_8.23.xls` & `clophfit-0.4.9/tests/Tecan/290212_8.23.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_8.82.xls` & `clophfit-0.4.9/tests/Tecan/290212_8.82.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290212_9.31.xls` & `clophfit-0.4.9/tests/Tecan/290212_9.31.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290513_5.5.xls` & `clophfit-0.4.9/tests/Tecan/290513_5.5.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290513_5.5_bad.xls` & `clophfit-0.4.9/tests/Tecan/290513_5.5_bad.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290513_7.2.xls` & `clophfit-0.4.9/tests/Tecan/290513_7.2.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/290513_8.8.xls` & `clophfit-0.4.9/tests/Tecan/290513_8.8.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/200214 pH data.ods` & `clophfit-0.4.9/tests/Tecan/140220/200214 pH data.ods`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/NaCl1_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/NaCl1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/NaCl2_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/NaCl2_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/NaCl3_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/NaCl3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/NaCl4_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/NaCl4_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/NaCl5_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/NaCl5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/NaCl6_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/NaCl6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/NaCl7_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/NaCl7_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/NaCl8_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/NaCl8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/fit0-1.csv` & `clophfit-0.4.9/tests/Tecan/140220/fit0-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/fit0.csv` & `clophfit-0.4.9/tests/Tecan/140220/fit0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/fit1-1.csv` & `clophfit-0.4.9/tests/Tecan/140220/fit1-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/fit1.csv` & `clophfit-0.4.9/tests/Tecan/140220/fit1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/pH5.0_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/pH5.0_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/pH5.8_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/pH5.8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/pH6.5_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/pH6.5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/pH7.1_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/pH7.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/pH7.6_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/pH7.6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/pH8.3_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/pH8.3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/140220/pH9.1_200214.xls` & `clophfit-0.4.9/tests/Tecan/140220/pH9.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx` & `clophfit-0.4.9/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls` & `clophfit-0.4.9/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/exceptions/84wells_290212_20.xlsx` & `clophfit-0.4.9/tests/Tecan/exceptions/84wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/Tecan/exceptions/88wells_290212_20.xlsx` & `clophfit-0.4.9/tests/Tecan/exceptions/88wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/A01-20140311a.dat` & `clophfit-0.4.9/tests/data/A01-20140311a.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/A01.dat` & `clophfit-0.4.9/tests/data/A01.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/NTT-A04-Cl_note` & `clophfit-0.4.9/tests/data/NTT-A04-Cl_note`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_A.csv` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_A.png` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_B.csv` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_B.png` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_C.csv` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_C.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_C.png` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_C.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_D.csv` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_D.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_D.png` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_D.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_E.csv` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_E.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_E.png` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_E.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_F.csv` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_F.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/Meas/A04 Cl_F.png` & `clophfit-0.4.9/tests/data/Meas/A04 Cl_F.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/k/D05.dat-bs.png` & `clophfit-0.4.9/tests/data/k/D05.dat-bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/k/D05.dat.png` & `clophfit-0.4.9/tests/data/k/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.4.9/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.4.9/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.4.9/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.4.9/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/output/global/Cl/B05-20130628-cor.dat.png` & `clophfit-0.4.9/tests/data/output/global/Cl/B05-20130628-cor.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/tests/data/output/global/pH/D05.dat.png` & `clophfit-0.4.9/tests/data/output/global/pH/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/.gitignore` & `clophfit-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/LICENSE.txt` & `clophfit-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.8/pyproject.toml` & `clophfit-0.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Topic :: Scientific/Engineering",
   "Development Status :: 3 - Alpha"
 ]
 dependencies = [
   'click < 8.1.4',
   'corner < 2.2.3',
   'emcee < 3.1.5',
-  'lmfit < 1.2.1',
+  'lmfit < 1.2.2',
   'matplotlib < 3.7.2',
   'numpy < 1.24.4',
   'openpyxl < 3.1.3',
   'pandas < 2.0.2',
   'rpy2 < 3.5.12',
   'scipy < 1.10.2',
   'seaborn < 0.12.3',
@@ -44,42 +44,42 @@
   "macromolecule binding"
 ]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "clophfit"
 readme = "docs/README.md"
 requires-python = ">=3.8, <3.12"
-version = "0.4.8"
+version = "0.4.9"
 
 [project.optional-dependencies]
 dev = [
   "commitizen < 3.2.1",
   "ipykernel",
   "jupyter",
-  "ruff == 0.0.263",
+  "ruff == 0.0.264",
   "pylsp-mypy",
   "python-lsp-ruff"
 ]
 docs = [
-  "autodocsumm == 0.2.10",
+  "autodocsumm == 0.2.11",
   "myst-parser == 1.0.0",
   "nbsphinx == 0.9.1",
   "pydata-sphinx-theme == 0.13.3",
   "Sphinx == 6.2.1",
   "sphinx-click == 4.4.0",
   "sphinx_autodoc_typehints == 1.23.0",
   "sphinxcontrib-plantuml == 0.25"
 ]
 tests = [
   "coverage[toml] < 7.2.6",
   "mypy < 1.3",
   "pandas-stubs == 2.0.1.230501",
   "Pygments < 2.15.2",
   "pytest < 7.3.2",
-  "typeguard < 2.13.4",
+  "typeguard == 4.0.0rc5",
   "xdoctest < 1.1.2"
 ]
 
 [project.scripts]
 "clop" = "clophfit.__main__:clop"
 
 [project.urls]
@@ -106,15 +106,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.4.8"
+version = "0.4.9"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "docs/README.md:Version"
 ]
 
 [tool.commitizen.customize]
```

### Comparing `clophfit-0.4.8/docs/README.md` & `clophfit-0.4.9/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 Cli for fitting macromolecule pH titration or binding assay data, e.g.
 fluorescence spectra.
 
-- Version: "0.4.8"
+- Version: "0.4.9"
 
 ## Features
 
 - Plate Reader data Parser.
 - Perform non-linear least square fitting.
 - Extract and fit pH and chloride titrations of GFP libraries.
   - For 2 labelblocks (e.g. 400, 485 nm) fit data separately and globally.
```

### Comparing `clophfit-0.4.8/PKG-INFO` & `clophfit-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clophfit
-Version: 0.4.8
+Version: 0.4.9
 Summary: Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra.
 Project-URL: Bug Tracker, https://github.com/darosio/ClopHfit/issues
 Project-URL: Changelog, https://darosio.github.io/ClopHfit/misc/CHANGELOG.html
 Project-URL: Discussions, https://github.com/darosio/ClopHfit/discussions
 Project-URL: Documentation, https://clophfit.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/ClopHfit/releases
 Project-URL: Homepage, https://github.com/darosio/ClopHfit
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.12,>=3.8
 Requires-Dist: click<8.1.4
 Requires-Dist: corner<2.2.3
 Requires-Dist: emcee<3.1.5
-Requires-Dist: lmfit<1.2.1
+Requires-Dist: lmfit<1.2.2
 Requires-Dist: matplotlib<3.7.2
 Requires-Dist: numpy<1.24.4
 Requires-Dist: openpyxl<3.1.3
 Requires-Dist: pandas<2.0.2
 Requires-Dist: rpy2<3.5.12
 Requires-Dist: scipy<1.10.2
 Requires-Dist: seaborn<0.12.3
@@ -40,46 +40,46 @@
 Requires-Dist: xlrd<2.0.2
 Provides-Extra: dev
 Requires-Dist: commitizen<3.2.1; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
 Requires-Dist: python-lsp-ruff; extra == 'dev'
-Requires-Dist: ruff==0.0.263; extra == 'dev'
+Requires-Dist: ruff==0.0.264; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: autodocsumm==0.2.10; extra == 'docs'
+Requires-Dist: autodocsumm==0.2.11; extra == 'docs'
 Requires-Dist: myst-parser==1.0.0; extra == 'docs'
 Requires-Dist: nbsphinx==0.9.1; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme==0.13.3; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints==1.23.0; extra == 'docs'
 Requires-Dist: sphinx-click==4.4.0; extra == 'docs'
 Requires-Dist: sphinx==6.2.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-plantuml==0.25; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: coverage[toml]<7.2.6; extra == 'tests'
 Requires-Dist: mypy<1.3; extra == 'tests'
 Requires-Dist: pandas-stubs==2.0.1.230501; extra == 'tests'
 Requires-Dist: pygments<2.15.2; extra == 'tests'
 Requires-Dist: pytest<7.3.2; extra == 'tests'
-Requires-Dist: typeguard<2.13.4; extra == 'tests'
+Requires-Dist: typeguard==4.0.0rc5; extra == 'tests'
 Requires-Dist: xdoctest<1.1.2; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # ClopHfit
 
 [![PyPI](https://img.shields.io/pypi/v/ClopHfit.svg)](https://pypi.org/project/ClopHfit/)
 [![CI](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
 Cli for fitting macromolecule pH titration or binding assay data, e.g.
 fluorescence spectra.
 
-- Version: "0.4.8"
+- Version: "0.4.9"
 
 ## Features
 
 - Plate Reader data Parser.
 - Perform non-linear least square fitting.
 - Extract and fit pH and chloride titrations of GFP libraries.
   - For 2 labelblocks (e.g. 400, 485 nm) fit data separately and globally.
```

