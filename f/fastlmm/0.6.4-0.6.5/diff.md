# Comparing `tmp/fastlmm-0.6.4.tar.gz` & `tmp/fastlmm-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlmm-0.6.4.tar", last modified: Mon Oct 31 20:40:30 2022, max compression
+gzip compressed data, was "fastlmm-0.6.5.tar", last modified: Tue May  2 22:08:51 2023, max compression
```

## Comparing `fastlmm-0.6.4.tar` & `fastlmm-0.6.5.tar`

### file list

```diff
@@ -1,171 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.708217 fastlmm-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-10-31 20:39:18.000000 fastlmm-0.6.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11554 2022-10-31 20:39:18.000000 fastlmm-0.6.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-31 20:39:18.000000 fastlmm-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4825 2022-10-31 20:40:30.708217 fastlmm-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4028 2022-10-31 20:39:18.000000 fastlmm-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.672217 fastlmm-0.6.4/fastlmm/
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.676217 fastlmm-0.6.4/fastlmm/association/
--rw-r--r--   0 runner    (1001) docker     (121)    72493 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/FastLmmSet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3303 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/FastLmmSetLOOC.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.696217 fastlmm-0.6.4/fastlmm/association/Fastlmm_autoselect/
--rw-r--r--   0 runner    (1001) docker     (121)   562014 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf
--rw-r--r--   0 runner    (1001) docker     (121)  8451072 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe
--rw-r--r--   0 runner    (1001) docker     (121) 12772999 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/Fastlmm_autoselect/fastlmmc
--rw-r--r--   0 runner    (1001) docker     (121)  1170360 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/LeaveOneChromosomeOut.py
--rw-r--r--   0 runner    (1001) docker     (121)    14080 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/LocoGwas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/PairResult.py
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/PrecomputeLocoPcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/Result.py
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/_matchscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     9351 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/_pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.700217 fastlmm-0.6.4/fastlmm/association/altset_list/
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/altset_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/altset_list/consecutive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/altset_list/minmaxsetsize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/altset_list/snpandsetnamecollection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/altset_list/subset.py
--rw-r--r--   0 runner    (1001) docker     (121)    27965 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/epistasis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/fixed.py
--rw-r--r--   0 runner    (1001) docker     (121)    12264 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/gwas.py
--rw-r--r--   0 runner    (1001) docker     (121)    12633 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/gwas_eval.py
--rw-r--r--   0 runner    (1001) docker     (121)    40985 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/heritability_spatial_correction.py
--rw-r--r--   0 runner    (1001) docker     (121)    13950 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/lrt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4586 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/meta_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    19358 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/score.py
--rw-r--r--   0 runner    (1001) docker     (121)    72932 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/single_snp.py
--rw-r--r--   0 runner    (1001) docker     (121)    22659 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/single_snp_all_plus_select.py
--rw-r--r--   0 runner    (1001) docker     (121)     9760 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/single_snp_linreg.py
--rw-r--r--   0 runner    (1001) docker     (121)    76444 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/single_snp_scale.py
--rw-r--r--   0 runner    (1001) docker     (121)    12086 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/single_snp_select.py
--rw-r--r--   0 runner    (1001) docker     (121)     5695 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/snp_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     9337 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/testCV.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.700217 fastlmm-0.6.4/fastlmm/association/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     8919 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/Cv.py
--rw-r--r--   0 runner    (1001) docker     (121)     9080 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/LRT_up.py
--rw-r--r--   0 runner    (1001) docker     (121)     5929 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/Lrt.py
--rw-r--r--   0 runner    (1001) docker     (121)     5903 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/Sc.py
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19723 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/test_gpu_perf.py
--rw-r--r--   0 runner    (1001) docker     (121)    16671 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/test_gwas.py
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/test_heritability_spatial_correction.py
--rw-r--r--   0 runner    (1001) docker     (121)    50694 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/test_single_snp.py
--rw-r--r--   0 runner    (1001) docker     (121)    10926 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/test_single_snp_all_plus_select.py
--rw-r--r--   0 runner    (1001) docker     (121)     4742 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/test_single_snp_linreg.py
--rw-r--r--   0 runner    (1001) docker     (121)    15418 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/test_single_snp_scale.py
--rw-r--r--   0 runner    (1001) docker     (121)     9447 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/test_single_snp_select.py
--rw-r--r--   0 runner    (1001) docker     (121)     7217 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/test_snp_set.py
--rw-r--r--   0 runner    (1001) docker     (121)    20281 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/testepistasis.py
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/tests/tests_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/varcomp_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7170 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/association/windowing_gwas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.700217 fastlmm-0.6.4/fastlmm/external/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29588 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/external/pca.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.700217 fastlmm-0.6.4/fastlmm/external/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/external/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/external/util/math.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.700217 fastlmm-0.6.4/fastlmm/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (121)    19608 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/PerformSelectionDistributable.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.704217 fastlmm-0.6.4/fastlmm/feature_selection/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/bronze.txt
--rw-r--r--   0 runner    (1001) docker     (121)  1250003 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.5chrom.bed
--rw-r--r--   0 runner    (1001) docker     (121)   237784 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.5chrom.bim
--rw-r--r--   0 runner    (1001) docker     (121)    14861 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.5chrom.fam
--rw-r--r--   0 runner    (1001) docker     (121)    10798 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.cov
--rw-r--r--   0 runner    (1001) docker     (121)   197784 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.map
--rw-r--r--   0 runner    (1001) docker     (121)    11016 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.phe
--rw-r--r--   0 runner    (1001) docker     (121)    11164 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.shufflePlus.phe
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.sim
--rw-r--r--   0 runner    (1001) docker     (121)     5357 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydataTest.phe
--rw-r--r--   0 runner    (1001) docker     (121)     5473 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/examples/toydataTrain.phe
--rw-r--r--   0 runner    (1001) docker     (121)    42277 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/feature_selection_cv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/feature_selection_example.py
--rw-r--r--   0 runner    (1001) docker     (121)    13201 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/feature_selection_two_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6370 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/kernel_ridge_cv.py
--rw-r--r--   0 runner    (1001) docker     (121)    22814 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/feature_selection/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.704217 fastlmm-0.6.4/fastlmm/inference/
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11787 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/ep.py
--rw-r--r--   0 runner    (1001) docker     (121)    34250 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/fastlmm_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)    25662 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/glmm.py
--rw-r--r--   0 runner    (1001) docker     (121)    16327 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/laplace.py
--rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)    20114 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)    39078 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/lmm.py
--rw-r--r--   0 runner    (1001) docker     (121)    21876 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/lmm2k.py
--rw-r--r--   0 runner    (1001) docker     (121)    54272 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/lmm_cov.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.704217 fastlmm-0.6.4/fastlmm/inference/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26408 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (121)    50646 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/tests/test_fastlmm_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)     9606 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/inference/tests/test_linear_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.704217 fastlmm-0.6.4/fastlmm/pyplink/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.704217 fastlmm-0.6.4/fastlmm/pyplink/altset_list/
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/altset_list/Consecutive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/altset_list/MinMaxSetSize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/altset_list/Subset.py
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/altset_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7144 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/plink.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.708217 fastlmm-0.6.4/fastlmm/pyplink/snpreader/
--rw-r--r--   0 runner    (1001) docker     (121)    11952 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpreader/Bed.py
--rw-r--r--   0 runner    (1001) docker     (121)     7392 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpreader/Dat.py
--rw-r--r--   0 runner    (1001) docker     (121)     8770 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpreader/Hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpreader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.708217 fastlmm-0.6.4/fastlmm/pyplink/snpset/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpset/AllSnps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpset/PositionRange.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpset/RandomSnpSet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpset/SnpIndexList.py
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpset/SnpSetAndName.py
--rw-r--r--   0 runner    (1001) docker     (121)     1717 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpset/SnpsFromFile.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/snpset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2752 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/pyplink/vcfpy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.708217 fastlmm-0.6.4/fastlmm/util/
--rw-r--r--   0 runner    (1001) docker     (121)    11285 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/NearBronze.py
--rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/VertexCut.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/_example_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/computePC.py
--rw-r--r--   0 runner    (1001) docker     (121)     6556 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/compute_auto_pcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/est_h2.py
--rw-r--r--   0 runner    (1001) docker     (121)     6435 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/fastlmm.hashdown.json
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/genphen.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/gensnp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.708217 fastlmm-0.6.4/fastlmm/util/matrix/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9899 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/matrix/mmultfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     5338 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/mingrid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/pickle_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     8827 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/run_fastlmmc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.708217 fastlmm-0.6.4/fastlmm/util/standardizer/
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/standardizer/Beta.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/standardizer/Unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/standardizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.708217 fastlmm-0.6.4/fastlmm/util/stats/
--rw-r--r--   0 runner    (1001) docker     (121)     5629 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13209 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/stats/chi2mixture.py
--rw-r--r--   0 runner    (1001) docker     (121)    29437 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/stats/plotp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/test.py
--rw-r--r--   0 runner    (1001) docker     (121)    21384 2022-10-31 20:39:19.000000 fastlmm-0.6.4/fastlmm/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 20:40:30.672217 fastlmm-0.6.4/fastlmm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4825 2022-10-31 20:40:30.000000 fastlmm-0.6.4/fastlmm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5470 2022-10-31 20:40:30.000000 fastlmm-0.6.4/fastlmm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 20:40:30.000000 fastlmm-0.6.4/fastlmm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-31 20:40:30.000000 fastlmm-0.6.4/fastlmm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-10-31 20:40:30.000000 fastlmm-0.6.4/fastlmm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-31 20:39:19.000000 fastlmm-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 20:40:30.708217 fastlmm-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2022-10-31 20:39:19.000000 fastlmm-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.481542 fastlmm-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-02 22:07:16.000000 fastlmm-0.6.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-05-02 22:07:16.000000 fastlmm-0.6.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 22:07:16.000000 fastlmm-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-02 22:08:51.481542 fastlmm-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-02 22:07:16.000000 fastlmm-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.429536 fastlmm-0.6.5/fastlmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-02 22:07:16.000000 fastlmm-0.6.5/fastlmm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.433536 fastlmm-0.6.5/fastlmm/association/
+-rw-r--r--   0 runner    (1001) docker     (123)    72493 2023-05-02 22:07:16.000000 fastlmm-0.6.5/fastlmm/association/FastLmmSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-02 22:07:16.000000 fastlmm-0.6.5/fastlmm/association/FastLmmSetLOOC.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.461539 fastlmm-0.6.5/fastlmm/association/Fastlmm_autoselect/
+-rw-r--r--   0 runner    (1001) docker     (123)   562014 2023-05-02 22:07:16.000000 fastlmm-0.6.5/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)  8451072 2023-05-02 22:07:16.000000 fastlmm-0.6.5/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe
+-rw-r--r--   0 runner    (1001) docker     (123) 12772999 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/Fastlmm_autoselect/fastlmmc
+-rw-r--r--   0 runner    (1001) docker     (123)  1170360 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/LeaveOneChromosomeOut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/LocoGwas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/PairResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/PrecomputeLocoPcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/Result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/_matchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.461539 fastlmm-0.6.5/fastlmm/association/altset_list/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/altset_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/altset_list/consecutive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/altset_list/minmaxsetsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/altset_list/snpandsetnamecollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/altset_list/subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27965 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/epistasis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/gwas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/gwas_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40985 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/heritability_spatial_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/meta_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19358 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72932 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/single_snp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22659 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/single_snp_all_plus_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/single_snp_linreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76444 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/single_snp_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/single_snp_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/snp_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/testCV.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.465540 fastlmm-0.6.5/fastlmm/association/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/Cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/LRT_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/Lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/Sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/test_gpu_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16671 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/test_gwas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/test_heritability_spatial_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50694 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/test_single_snp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/test_single_snp_all_plus_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/test_single_snp_linreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15418 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/test_single_snp_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/test_single_snp_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/test_snp_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20281 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/testepistasis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/tests/tests_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/varcomp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/association/windowing_gwas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.465540 fastlmm-0.6.5/fastlmm/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29588 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/external/pca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.465540 fastlmm-0.6.5/fastlmm/external/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/external/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/external/util/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.469540 fastlmm-0.6.5/fastlmm/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/PerformSelectionDistributable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.473541 fastlmm-0.6.5/fastlmm/feature_selection/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/bronze.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1250003 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.5chrom.bed
+-rw-r--r--   0 runner    (1001) docker     (123)   237784 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.5chrom.bim
+-rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.5chrom.fam
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.cov
+-rw-r--r--   0 runner    (1001) docker     (123)   197784 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.phe
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.shufflePlus.phe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.sim
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydataTest.phe
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/examples/toydataTrain.phe
+-rw-r--r--   0 runner    (1001) docker     (123)    42221 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/feature_selection_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/feature_selection_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/feature_selection_two_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/kernel_ridge_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22814 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/feature_selection/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.473541 fastlmm-0.6.5/fastlmm/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11787 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/ep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34250 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/fastlmm_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25662 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/glmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20114 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39098 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/lmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21895 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/lmm2k.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54637 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/lmm_cov.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.477541 fastlmm-0.6.5/fastlmm/inference/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26427 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50646 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/tests/test_fastlmm_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/inference/tests/test_linear_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.477541 fastlmm-0.6.5/fastlmm/pyplink/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.477541 fastlmm-0.6.5/fastlmm/pyplink/altset_list/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/altset_list/Consecutive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/altset_list/MinMaxSetSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/altset_list/Subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/altset_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/plink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.477541 fastlmm-0.6.5/fastlmm/pyplink/snpreader/
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpreader/Bed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpreader/Dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpreader/Hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpreader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.477541 fastlmm-0.6.5/fastlmm/pyplink/snpset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpset/AllSnps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpset/PositionRange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpset/RandomSnpSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpset/SnpIndexList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpset/SnpSetAndName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpset/SnpsFromFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/snpset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/pyplink/vcfpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.481542 fastlmm-0.6.5/fastlmm/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/NearBronze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/VertexCut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/_example_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/computePC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/compute_auto_pcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/est_h2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/fastlmm.hashdown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/genphen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/gensnp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.481542 fastlmm-0.6.5/fastlmm/util/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/matrix/mmultfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/mingrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/pickle_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/run_fastlmmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.481542 fastlmm-0.6.5/fastlmm/util/standardizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/standardizer/Beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/standardizer/Unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/standardizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.481542 fastlmm-0.6.5/fastlmm/util/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/stats/chi2mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29437 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/stats/plotp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21384 2023-05-02 22:07:17.000000 fastlmm-0.6.5/fastlmm/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.429536 fastlmm-0.6.5/fastlmm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-02 22:08:51.000000 fastlmm-0.6.5/fastlmm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-02 22:08:51.000000 fastlmm-0.6.5/fastlmm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:08:51.000000 fastlmm-0.6.5/fastlmm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-02 22:08:51.000000 fastlmm-0.6.5/fastlmm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-02 22:08:51.000000 fastlmm-0.6.5/fastlmm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-02 22:07:17.000000 fastlmm-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 22:08:51.481542 fastlmm-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-02 22:07:17.000000 fastlmm-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:08:51.481542 fastlmm-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-05-02 22:07:17.000000 fastlmm-0.6.5/tests/test.py
```

### Comparing `fastlmm-0.6.4/LICENSE.md` & `fastlmm-0.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/PKG-INFO` & `fastlmm-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlmm
-Version: 0.6.4
+Version: 0.6.5
 Summary: Fast GWAS
 Home-page: https://fastlmm.github.io/
 Author: FaST-LMM Team
 Author-email: fastlmm-dev@python.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/fastlmm/FaST-LMM/issues
 Project-URL: Documentation, http://fastlmm.github.io/FaST-LMM
```

### Comparing `fastlmm-0.6.4/README.md` & `fastlmm-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/__init__.py` & `fastlmm-0.6.5/fastlmm/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/FastLmmSet.py` & `fastlmm-0.6.5/fastlmm/association/FastLmmSet.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/FastLmmSetLOOC.py` & `fastlmm-0.6.5/fastlmm/association/FastLmmSetLOOC.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf` & `fastlmm-0.6.5/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe` & `fastlmm-0.6.5/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/Fastlmm_autoselect/fastlmmc` & `fastlmm-0.6.5/fastlmm/association/Fastlmm_autoselect/fastlmmc`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll` & `fastlmm-0.6.5/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/LeaveOneChromosomeOut.py` & `fastlmm-0.6.5/fastlmm/association/LeaveOneChromosomeOut.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/LocoGwas.py` & `fastlmm-0.6.5/fastlmm/association/LocoGwas.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/PairResult.py` & `fastlmm-0.6.5/fastlmm/association/PairResult.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/PrecomputeLocoPcs.py` & `fastlmm-0.6.5/fastlmm/association/PrecomputeLocoPcs.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/Result.py` & `fastlmm-0.6.5/fastlmm/association/Result.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/__init__.py` & `fastlmm-0.6.5/fastlmm/association/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/_matchscript.py` & `fastlmm-0.6.5/fastlmm/association/_matchscript.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/_pipelines.py` & `fastlmm-0.6.5/fastlmm/association/_pipelines.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/altset_list/__init__.py` & `fastlmm-0.6.5/fastlmm/association/altset_list/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/altset_list/consecutive.py` & `fastlmm-0.6.5/fastlmm/association/altset_list/consecutive.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/altset_list/minmaxsetsize.py` & `fastlmm-0.6.5/fastlmm/association/altset_list/minmaxsetsize.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/altset_list/snpandsetnamecollection.py` & `fastlmm-0.6.5/fastlmm/association/altset_list/snpandsetnamecollection.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/altset_list/subset.py` & `fastlmm-0.6.5/fastlmm/association/altset_list/subset.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/epistasis.py` & `fastlmm-0.6.5/fastlmm/association/epistasis.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/fixed.py` & `fastlmm-0.6.5/fastlmm/association/fixed.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/gwas.py` & `fastlmm-0.6.5/fastlmm/association/gwas.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/gwas_eval.py` & `fastlmm-0.6.5/fastlmm/association/gwas_eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     LOD2 = sp.median(stats.chi2.isf(pv,1))
     L = (LOD2/0.456)
     return (L)
 
 
 def cut_snps_close_to_causals(p_values, pos, causal_idx, mindist, plot=False):
 
-    i_causal_all = np.zeros(len(p_values), dtype=np.bool)
+    i_causal_all = np.zeros(len(p_values), dtype=bool)
     i_causal_all[causal_idx] = True
         
     # cut out snps in LD to causal snps
     pos_all = np.array(pos)
     pos_causal = np.array(pos)[causal_idx]
 
     close_to_causals_mask = excludeinds(pos_all, pos_causal, mindist=mindist, idist=2)
@@ -431,12 +431,12 @@
 
     pylab.show()
 
 
 if __name__ == "__main__":
     num = 700000 * 500
     pv = X = np.random.random((num))
-    i_causal = X = np.ones((num), dtype=np.bool)
+    i_causal = X = np.ones((num), dtype=bool)
     
     t0 = time.time()
     compute_power_data(pv, i_causal)
     print(("time taken:", time.time() - t0))
```

### Comparing `fastlmm-0.6.4/fastlmm/association/heritability_spatial_correction.py` & `fastlmm-0.6.5/fastlmm/association/heritability_spatial_correction.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/lrt.py` & `fastlmm-0.6.5/fastlmm/association/lrt.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/meta_analysis.py` & `fastlmm-0.6.5/fastlmm/association/meta_analysis.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/score.py` & `fastlmm-0.6.5/fastlmm/association/score.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/single_snp.py` & `fastlmm-0.6.5/fastlmm/association/single_snp.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/single_snp_all_plus_select.py` & `fastlmm-0.6.5/fastlmm/association/single_snp_all_plus_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/single_snp_linreg.py` & `fastlmm-0.6.5/fastlmm/association/single_snp_linreg.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/single_snp_scale.py` & `fastlmm-0.6.5/fastlmm/association/single_snp_scale.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/single_snp_select.py` & `fastlmm-0.6.5/fastlmm/association/single_snp_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/snp_set.py` & `fastlmm-0.6.5/fastlmm/association/snp_set.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/testCV.py` & `fastlmm-0.6.5/fastlmm/association/testCV.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/Cv.py` & `fastlmm-0.6.5/fastlmm/association/tests/Cv.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/LRT_up.py` & `fastlmm-0.6.5/fastlmm/association/tests/LRT_up.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/Lrt.py` & `fastlmm-0.6.5/fastlmm/association/tests/Lrt.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/Sc.py` & `fastlmm-0.6.5/fastlmm/association/tests/Sc.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/__init__.py` & `fastlmm-0.6.5/fastlmm/association/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/test_gpu_perf.py` & `fastlmm-0.6.5/fastlmm/association/tests/test_gpu_perf.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/test_gwas.py` & `fastlmm-0.6.5/fastlmm/association/tests/test_gwas.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/test_heritability_spatial_correction.py` & `fastlmm-0.6.5/fastlmm/association/tests/test_heritability_spatial_correction.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/test_single_snp.py` & `fastlmm-0.6.5/fastlmm/association/tests/test_single_snp.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/test_single_snp_all_plus_select.py` & `fastlmm-0.6.5/fastlmm/association/tests/test_single_snp_all_plus_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/test_single_snp_linreg.py` & `fastlmm-0.6.5/fastlmm/association/tests/test_single_snp_linreg.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/test_single_snp_scale.py` & `fastlmm-0.6.5/fastlmm/association/tests/test_single_snp_scale.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/test_single_snp_select.py` & `fastlmm-0.6.5/fastlmm/association/tests/test_single_snp_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/test_snp_set.py` & `fastlmm-0.6.5/fastlmm/association/tests/test_snp_set.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/testepistasis.py` & `fastlmm-0.6.5/fastlmm/association/tests/testepistasis.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/tests/tests_util.py` & `fastlmm-0.6.5/fastlmm/association/tests/tests_util.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/varcomp_test.py` & `fastlmm-0.6.5/fastlmm/association/varcomp_test.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/association/windowing_gwas.py` & `fastlmm-0.6.5/fastlmm/association/windowing_gwas.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/external/pca.py` & `fastlmm-0.6.5/fastlmm/external/pca.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/external/util/math.py` & `fastlmm-0.6.5/fastlmm/external/util/math.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import
+from __future__ import absolute_import
 import numpy as np
 import scipy as sp
 
 def mvnormpdf(b, mean, cov, precision=False):
     k = b.shape[0]
     part1 = np.exp(-0.5*k*np.log(2.0*np.pi))
     dev = b-mean
@@ -43,22 +43,22 @@
         return (d*mtx.T).T
     else:
         return d*mtx
 
 def check_definite_positiveness(A):
     B = np.empty_like(A)
     B[:] = A
-    B[np.diag_indices_from(B)] += np.sqrt(np.finfo(np.float).eps)
+    B[np.diag_indices_from(B)] += np.sqrt(np.finfo(float).eps)
     try:
         np.linalg.cholesky(B)
     except np.linalg.LinAlgError:
         return False
     return True
 
 def check_symmetry(A):
-    return abs(A-A.T).max() < np.sqrt(np.finfo(np.float).eps)
+    return abs(A-A.T).max() < np.sqrt(np.finfo(float).eps)
 
 def kl_divergence(p,q):
     return np.sum(np.log(p/q)*p)
 
 stl = lambda a, b : sp.linalg.solve_triangular(a, b, lower=True, check_finite=False)
 stu = lambda a, b : sp.linalg.solve_triangular(a, b, lower=False, check_finite=False)
```

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/PerformSelectionDistributable.py` & `fastlmm-0.6.5/fastlmm/feature_selection/PerformSelectionDistributable.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import numpy as np
 import pandas as pd
 import sys
 
 # sklearn
 from sklearn.linear_model import RidgeCV, Ridge
 from sklearn.model_selection import KFold, LeaveOneOut, ShuffleSplit
-from sklearn.datasets import load_boston, load_diabetes
 from sklearn.metrics import mean_squared_error
 from sklearn.feature_selection import f_regression
 from sklearn import model_selection
 from sklearn.decomposition import PCA
 
 # project
 import fastlmm.pyplink.plink as plink
```

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.5chrom.bed` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.5chrom.bed`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.5chrom.bim` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.5chrom.bim`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.5chrom.fam` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.5chrom.fam`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.cov` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.cov`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.map` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.map`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.phe` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/toydata.shufflePlus.phe` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/toydata.shufflePlus.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/toydataTest.phe` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/toydataTest.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/examples/toydataTrain.phe` & `fastlmm-0.6.5/fastlmm/feature_selection/examples/toydataTrain.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/feature_selection_cv.py` & `fastlmm-0.6.5/fastlmm/feature_selection/feature_selection_cv.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import scipy as sp
 import numpy as np
 import pandas as pd
 
 # sklearn
 from sklearn.linear_model import RidgeCV, Ridge
 from sklearn.model_selection import KFold, LeaveOneOut, ShuffleSplit
-from sklearn.datasets import load_boston, load_diabetes
 from sklearn.metrics import mean_squared_error
 from sklearn.feature_selection import f_regression
 from sklearn import model_selection
 from sklearn.decomposition import KernelPCA
 
 # project
 from pysnptools.snpreader import Bed
```

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/feature_selection_example.py` & `fastlmm-0.6.5/fastlmm/feature_selection/feature_selection_example.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/feature_selection_two_kernel.py` & `fastlmm-0.6.5/fastlmm/feature_selection/feature_selection_two_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,16 +204,16 @@
                         lmm = fastLMM(X=cov_train, Y=y_train[:,np.newaxis], G=G_bg_train)
                     else:
                         lmm = fastLMM(X=cov_train, Y=y_train[:,np.newaxis], K=K_bg_train)
 
                     W = G_fs_train.copy()
                     UGup,UUGup = lmm.rotate(W)
                 
-                    i_up = np.zeros((G_fs_train.shape[1]), dtype=np.bool)
-                    i_G1 = np.ones((G_fs_train.shape[1]), dtype=np.bool)
+                    i_up = np.zeros((G_fs_train.shape[1]), dtype=bool)
+                    i_G1 = np.ones((G_fs_train.shape[1]), dtype=bool)
                     t0 = time.time()
                     res = lmm.findH2_2K(nGridH2=10, minH2=0.0, maxH2=0.99999, i_up=i_up, i_G1=i_G1, UW=UGup, UUW=UUGup)
                     logging.info("time taken for k=%i: %s" % (max_k, str(time.time()-t0)))
                 
                     # recover a2 from alternate parameterization
                     a2 = res["h2_1"] / float(res["h2"] + res["h2_1"])
                     h2 = res["h2"] + res["h2_1"]
```

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/kernel_ridge_cv.py` & `fastlmm-0.6.5/fastlmm/feature_selection/kernel_ridge_cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import absolute_import
 from __future__ import print_function
 import time
 import os
 import sys
 
 import scipy as SP
+import numpy as np
 import sklearn.metrics as SKM
 
 import sklearn.feature_selection as SKFS
 import sklearn.model_selection as SKCV 
 import sklearn.metrics as SKM
 
 from pysnptools.util.mapreduce1.distributable import *
@@ -172,13 +173,13 @@
         """precomputes the kernel
         """
         print("loading data...")
         G, self.X, self.y = load_snp_data(self.bed_fn, self.pheno_fn, cov_fn=self.cov_fn,offset=self.offset)
         print("done.")
         print("precomputing kernel... ")
         nSnps = G.shape[1]
-        self.K = 1./nSnps * SP.dot(G,G.T)
+        self.K = 1./nSnps * np.dot(G,G.T)
         print("done.")
         del G
```

### Comparing `fastlmm-0.6.4/fastlmm/feature_selection/test.py` & `fastlmm-0.6.5/fastlmm/feature_selection/test.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/inference/__init__.py` & `fastlmm-0.6.5/fastlmm/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/inference/ep.py` & `fastlmm-0.6.5/fastlmm/inference/ep.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/inference/fastlmm_predictor.py` & `fastlmm-0.6.5/fastlmm/inference/fastlmm_predictor.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/inference/glmm.py` & `fastlmm-0.6.5/fastlmm/inference/glmm.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/inference/laplace.py` & `fastlmm-0.6.5/fastlmm/inference/laplace.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/inference/likelihood.py` & `fastlmm-0.6.5/fastlmm/inference/likelihood.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/inference/linear_regression.py` & `fastlmm-0.6.5/fastlmm/inference/linear_regression.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/inference/lmm.py` & `fastlmm-0.6.5/fastlmm/inference/lmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import scipy as SP
 import numpy as NP
+import numpy as np
 import scipy.linalg as LA
 import scipy.optimize as opt
 import scipy.stats as ST
 import scipy.special as SS
 from fastlmm.util.mingrid import *
 from fastlmm.util.util import *
 import time
@@ -135,15 +136,15 @@
             if a2 == 0.0:
                 logging.info("a2=0.0, only using G0")
                 self.G = G0
             elif a2 == 1.0:
                 self.G = G1
                 logging.info("a2=1.0, only using G1")
             else:
-                self.G = SP.concatenate((SP.sqrt(1.0-a2) * G0, SP.sqrt(a2) * G1),1)
+                self.G = np.concatenate((np.sqrt(1.0-a2) * G0, np.sqrt(a2) * G1),1)
             
         else:
             self.G=None
 
         if self.G is not None:
             N = self.G.shape[0]
             k = self.G.shape[1]
@@ -164,15 +165,15 @@
                     logging.warning("Got SVD exception, trying eigenvalue decomposition of square of G. Note that this is a little bit less accurate")
                     [S_,V_] = LA.eigh(self.G.T.dot(self.G))
                     if np.any(S_ < -0.1):
                         logging.warning("kernel contains a negative Eigenvalue")
                     S_nonz=(S_>0)
                     self.S = S_[S_nonz]
                     self.S*=(N/self.S.sum())
-                    self.U=self.G.dot(V_[:,S_nonz]/SP.sqrt(self.S))
+                    self.U=self.G.dot(V_[:,S_nonz]/np.sqrt(self.S))
             else:
                 if K0 is None:
                     K0=self.G0.dot(self.G0.T);
                 self.K0=K0
                 if (self.G1 is not None) and (K1 is None):
                     K1=self.G1.dot(self.G1.T);
                 self.setK(K0=K0, K1=K1, a2=a2)
@@ -382,42 +383,42 @@
         D=self.UX.shape[1]
         
         #if REML == True:
         #    # this needs to be fixed, please see test_gwas.py for details
         #    raise NotImplementedError("REML in lmm object not supported, please use lmm_cov.py instead")
 
         if logdelta is not None:
-            delta = SP.exp(logdelta)
+            delta = np.exp(logdelta)
 
         if delta is not None:
             Sd = (self.S+delta)*scale
         else:
             Sd = (h2*self.S + (1.0-h2))*scale
 
         UXS = self.UX / NP.lib.stride_tricks.as_strided(Sd, (Sd.size,self.UX.shape[1]), (Sd.itemsize,0))
         UyS = self.Uy / Sd
 
         XKX = UXS.T.dot(self.UX)
         XKy = UXS.T.dot(self.Uy)
         yKy = UyS.T.dot(self.Uy)
 
-        logdetK = SP.log(Sd).sum()
+        logdetK = np.log(Sd).sum()
                 
         if (k<N):#low rank part
         
             # determine normalization factor
             if delta is not None:
                 denom = (delta*scale)
             else:
                 denom = ((1.0-h2)*scale)
             
             XKX += self.UUX.T.dot(self.UUX)/(denom)
             XKy += self.UUX.T.dot(self.UUy)/(denom)
             yKy += self.UUy.T.dot(self.UUy)/(denom)      
-            logdetK+=(N-k) * SP.log(denom)
+            logdetK+=(N-k) * np.log(denom)
  
         # proximal contamination (see Supplement Note 2: An Efficient Algorithm for Avoiding Proximal Contamination)
         # available at: http://www.nature.com/nmeth/journal/v9/n6/extref/nmeth.2037-S1.pdf
         # exclude SNPs from the RRM in the likelihood evaluation
         
 
         if len(self.exclude_idx) > 0:          
@@ -456,15 +457,15 @@
             assert UWy.shape == (num_exclude,)
             
             # compute S_WW^{-1} * UWX
             WX = UWX / NP.lib.stride_tricks.as_strided(S_WW, (S_WW.size,UWX.shape[1]), (S_WW.itemsize,0))
             # compute S_WW^{-1} * UWy
             Wy = UWy / S_WW
             # determinant update
-            logdetK += SP.log(S_WW).sum()
+            logdetK += np.log(S_WW).sum()
             assert WX.shape == (num_exclude, D)
             assert Wy.shape == (num_exclude,)
             
             # perform updates (instantiations for a and b in Equation (1.5) of Supplement)
             yKy += UWy.T.dot(Wy)
             XKy += UWX.T.dot(Wy)
             XKX += UWX.T.dot(WX)
@@ -481,22 +482,22 @@
 
         r2 = yKy-XKy.dot(beta)
 
         if dof is None:#Use the Multivariate Gaussian
             if REML:
                 XX = self.X.T.dot(self.X)
                 [Sxx,Uxx]= LA.eigh(XX)
-                logdetXX  = SP.log(Sxx).sum()
-                logdetXKX = SP.log(SxKx).sum()
+                logdetXX  = np.log(Sxx).sum()
+                logdetXKX = np.log(SxKx).sum()
                 sigma2 = r2 / (N - D)
-                nLL =  0.5 * ( logdetK + logdetXKX - logdetXX + (N-D) * ( SP.log(2.0*SP.pi*sigma2) + 1 ) )
+                nLL =  0.5 * ( logdetK + logdetXKX - logdetXX + (N-D) * ( np.log(2.0*SP.pi*sigma2) + 1 ) )
                 variance_beta = None
             else:
                 sigma2 = r2 / (N)
-                nLL =  0.5 * ( logdetK + N * ( SP.log(2.0*SP.pi*sigma2) + 1 ) )
+                nLL =  0.5 * ( logdetK + N * ( np.log(2.0*SP.pi*sigma2) + 1 ) )
                 if delta is not None:
                     h2 = 1.0/(delta+1)
                 # This is a faster version of h2 * sigma2 * np.diag(LA.inv(XKX))
                 # where h2*sigma2 is sigma2_g
                 variance_beta = h2 * sigma2 * (UxKx[:,i_pos]/SxKx[i_pos] * UxKx[:,i_pos]).sum(-1)
             result = {
                   'nLL':nLL,
@@ -508,33 +509,33 @@
                   'a2':self.a2,
                   'scale':scale
                   }
         else:#Use multivariate student-t
             if REML:
                 XX = self.X.T.dot(self.X)
                 [Sxx,Uxx]= LA.eigh(XX)
-                logdetXX  = SP.log(Sxx).sum()
-                logdetXKX = SP.log(SxKx).sum()
+                logdetXX  = np.log(Sxx).sum()
+                logdetXKX = np.log(SxKx).sum()
 
-                nLL =  0.5 * ( logdetK + logdetXKX - logdetXX + (dof + (N-D)) * SP.log(1.0+r2/dof) )
-                nLL += 0.5 * (N-D)*SP.log( dof*SP.pi ) + SS.gammaln( 0.5*dof ) - SS.gammaln( 0.5* (dof + (N-D) ))
+                nLL =  0.5 * ( logdetK + logdetXKX - logdetXX + (dof + (N-D)) * np.log(1.0+r2/dof) )
+                nLL += 0.5 * (N-D)*np.log( dof*SP.pi ) + SS.gammaln( 0.5*dof ) - SS.gammaln( 0.5* (dof + (N-D) ))
             else:
-                nLL =   0.5 * ( logdetK + (dof + N) * SP.log(1.0+r2/dof) )
-                nLL +=  0.5 * N*SP.log( dof*SP.pi ) + SS.gammaln( 0.5*dof ) - SS.gammaln( 0.5* (dof + N ))
+                nLL =   0.5 * ( logdetK + (dof + N) * np.log(1.0+r2/dof) )
+                nLL +=  0.5 * N*np.log( dof*SP.pi ) + SS.gammaln( 0.5*dof ) - SS.gammaln( 0.5* (dof + N ))
             result = {
                   'nLL':nLL,
                   'dof':dof,
                   'beta':beta,
                   'variance_beta': None,
                   'h2':h2,
                   'REML':REML,
                   'a2':self.a2,
                   'scale':scale
                   }      
-        assert SP.all(SP.isreal(nLL)), "nLL has an imaginary component, possibly due to constant covariates"
+        assert np.all(np.isreal(nLL)), "nLL has an imaginary component, possibly due to constant covariates"
         if result['variance_beta'] is None:
             del result['variance_beta']
         return result
 
 
     def getPosteriorWeights(self,beta,h2=0.0,logdelta=None,delta=None,scale=1.0):
         '''
@@ -555,34 +556,34 @@
         weights           : [k0+k1] 1-dimensional array of predicted phenotype values
         --------------------------------------------------------------------------
         '''
         k=self.S.shape[0]
         N=self.y.shape[0]
 
         if logdelta is not None:
-            delta = SP.exp(logdelta)
+            delta = np.exp(logdelta)
         if delta is not None:
             Sd = (self.S+delta)*scale
         else:
             Sd = (h2*self.S + (1.0-h2))*scale
 
-        yres = self.y - SP.dot(self.X,beta)
-        Uyres = SP.dot(self.U.T,yres)
-        UG = SP.dot(self.U.T, self.G)
-        weights = SP.dot(UG.T , Uyres/Sd)
+        yres = self.y - np.dot(self.X,beta)
+        Uyres = np.dot(self.U.T,yres)
+        UG = np.dot(self.U.T, self.G)
+        weights = np.dot(UG.T , Uyres/Sd)
 
         if k < N: # low-rank part
             # determine normalization factor
             if delta is not None:
                 denom = (delta*scale)
             else:
                 denom = ((1.0-h2)*scale)
                   
-            UUG = self.G - SP.dot(self.U, UG)
-            UUyres = yres - SP.dot(self.U,Uyres)
+            UUG = self.G - np.dot(self.U, UG)
+            UUyres = yres - np.dot(self.U,Uyres)
             weights += UUG.T.dot(UUyres)/(denom)
 
         return weights
 
 
     def setTestData(self,Xstar,K0star=None,K1star=None,G0star=None,G1star=None):
         '''
@@ -606,32 +607,32 @@
             if self.a2 == 0.0:
                 logging.info("a2=0.0, only using G0")
                 self.Gstar = G0star
             elif self.a2 == 1.0:
                 self.Gstar = G1star
                 logging.info("a2=1.0, only using G1")
             else:
-                self.Gstar=SP.concatenate((SP.sqrt(1.0-self.a2) * G0star, SP.sqrt(self.a2) * G1star),1)
+                self.Gstar=np.concatenate((np.sqrt(1.0-self.a2) * G0star, np.sqrt(self.a2) * G1star),1)
    
         if K0star is not None:
             if K1star is None:
                 self.Kstar = K0star
             else:
                 self.Kstar = (1.0-self.a2)*K0star + self.a2*K1star
         else:
-            self.Kstar = SP.dot(self.Gstar,self.G.T)
+            self.Kstar = np.dot(self.Gstar,self.G.T)
 
-        self.UKstar = SP.dot(self.U.T,self.Kstar.T)
+        self.UKstar = np.dot(self.U.T,self.Kstar.T)
 
         if self.G is not None:
             k = self.G.shape[1]
             N = self.G.shape[0]
             if k<N:
                 # see e.g. Equation 3.17 in Supplement of FaST LMM paper
-                self.UUKstar = self.Kstar.T - SP.dot(self.U, self.UKstar)
+                self.UUKstar = self.Kstar.T - np.dot(self.U, self.UKstar)
    
     def setTestData2(self,Xstar,K0star=None,K1star=None):
         '''
         a version of setTestData that doesn't assume that Eigenvalue decomposition has been done.
         '''
         
         self.Xstar = Xstar
@@ -669,50 +670,50 @@
             return SP.nan * SP.ones(M)
 
         k=self.S.shape[0]
         N=self.y.shape[0]
         #D=self.UX.shape[1]
        
         if logdelta is not None:
-            delta = SP.exp(logdelta)
+            delta = np.exp(logdelta)
 
         #delta = (1-h2) / h2
         if delta is not None:
             Sd = (self.S+delta)*scale
         else:
             assert False, "not implemented (UKstar needs to be scaled by h2)"
             Sd = (h2*self.S + (1.0-h2))*scale
 
         if len(self.exclude_idx) > 0:
             # cut out
             num_exclude = len(self.exclude_idx)
             # consider only excluded SNPs
             Gstar_exclude = self.Gstar[:,self.exclude_idx]
             #G_exclude = self.G[:,self.exclude_idx]
-            UKstar = self.UKstar - SP.dot(self.UW,Gstar_exclude.T)
+            UKstar = self.UKstar - np.dot(self.UW,Gstar_exclude.T)
             if k<N:
-                UUKstar = self.UUKstar - SP.dot(self.UUW,Gstar_exclude.T)
+                UUKstar = self.UUKstar - np.dot(self.UUW,Gstar_exclude.T)
         else:
             UKstar = self.UKstar 
             UUKstar = self.UUKstar 
 
-        yfixed = SP.dot(self.Xstar,beta)
-        yres = self.y - SP.dot(self.X,beta)
-        Uyres = self.Uy - SP.dot(self.UX,beta)
+        yfixed = np.dot(self.Xstar,beta)
+        yres = self.y - np.dot(self.X,beta)
+        Uyres = self.Uy - np.dot(self.UX,beta)
         Sdi = 1./Sd
-        yrandom = SP.dot(Sdi*UKstar.T,Uyres)
+        yrandom = np.dot(Sdi*UKstar.T,Uyres)
         
         if k < N: # low-rank part
             # determine normalization factor
             if delta is not None:
                 denom = (delta*scale)
             else:
                 denom = ((1.0-h2)*scale)
-            UUyres = yres - SP.dot(self.U,Uyres)
-            yrandom += SP.dot(UUKstar.T,UUyres)/denom
+            UUyres = yres - np.dot(self.U,Uyres)
+            yrandom += np.dot(UUKstar.T,UUyres)/denom
 
         # proximal contamination (see Supplement Note 2: An Efficient Algorithm for Avoiding Proximal Contamination)
         # available at: http://www.nature.com/nmeth/journal/v9/n6/extref/nmeth.2037-S1.pdf
         # exclude SNPs from the RRM in the likelihood evaluation
         if len(self.exclude_idx) > 0:
             UWS = self.UW / NP.lib.stride_tricks.as_strided(Sd, (Sd.size,num_exclude), (Sd.itemsize,0))
             assert UWS.shape == (k, num_exclude)
@@ -760,15 +761,15 @@
         else:
             K = np.dot(np.dot(lmm.U,np.eye(len(lmm.U)) * lmm.S),lmm.U.T) #Re-compose the Eigen value decomposition #!!!later do this more efficiently
         V = varg * K + vare * np.eye(len(K))
         Vinv = LA.inv(V)
 
         a = np.dot(varg * lmm.Kstar, Vinv)
 
-        y_star = np.dot(lmm.Xstar,beta) + np.dot(a, lmm.y-SP.dot(lmm.X,beta)) #!!!later shouldn't the 2nd dot be precomputed?
+        y_star = np.dot(lmm.Xstar,beta) + np.dot(a, lmm.y-np.dot(lmm.X,beta)) #!!!later shouldn't the 2nd dot be precomputed?
         y_star = y_star.reshape(-1,1) #Make 2-d
 
         var_star = (varg * Kstar_star + 
                     vare * np.eye(len(Kstar_star)) -
                     np.dot(a,
                             (varg * lmm.Kstar.T)))
         return y_star, var_star
@@ -809,15 +810,15 @@
         k = self.S.shape[0]
         N = self.y.shape[0]
         #D = self.UX.shape[1]
 
         #print "k, N, D", k, N, D
 
         if logdelta is not None:
-            delta = SP.exp(logdelta)
+            delta = np.exp(logdelta)
 
         if delta is not None:
             #Sd = (self.S+delta)*sigma2
             Sd = (self.S+delta)
         else:
             #Sd = (h2*self.S + (1.0-h2))*sigma2
             Sd = (h2*self.S + (1.0-h2))
@@ -828,15 +829,15 @@
         
         # part 1 from c-code
         #TODO: handle h2 parameterization
         #TODO: make more efficient (add_diag)
 
         if Kstar_star is None:
             N_test = self.Gstar.shape[0]
-            Kstar_star = SP.dot(self.Gstar, self.Gstar.T)
+            Kstar_star = np.dot(self.Gstar, self.Gstar.T)
         else:
             Kstar_star = Kstar_star.copy()
 
         N_test = Kstar_star.shape[0]
         assert N_test == Kstar_star.shape[1]
 
         part1 = Kstar_star
@@ -844,18 +845,18 @@
         part1 *= sigma2
         
         #print "part1", part1[0,0]
         #print "delta", delta, "sigma2", sigma2
         
         # part 2 from c-code
         # (U1^T a)^T (S_1 + delta*I)^{-1} (U1^T a)
-        SUKstarTUkStar = SP.dot(Sdi*self.UKstar.T, self.UKstar)
+        SUKstarTUkStar = np.dot(Sdi*self.UKstar.T, self.UKstar)
         
         #UXS = self.UKstar / NP.lib.stride_tricks.as_strided(Sd, (Sd.size,self.UKstar.shape[1]), (Sd.itemsize,0))
-        #NP.testing.assert_array_almost_equal(SUKstarTUkStar, SP.dot(UXS.T, self.UKstar), decimal=4)
+        #NP.testing.assert_array_almost_equal(SUKstarTUkStar, np.dot(UXS.T, self.UKstar), decimal=4)
 
         SUKstarTUkStar *= sigma2
 
         #print "UKstar[0,0]", self.UKstar[0,0]
         #print "UKstarS[0,0]", UXS[0,0]
         #print "SUK", SUKstarTUkStar[0,0]
         
@@ -865,15 +866,15 @@
             if delta is not None:
                 denom = (delta*sigma2)
             else:
                 denom = ((1.0-h2)*sigma2)
        
             # see Equation 3.17 in Supplement of FaST LMM paper:
             # 1 / delta * (((I_n - U1U1^T)a)^T (I_n - U1U1^T)a), a=K(XS,X)
-            SUKstarTUkStar += SP.dot(self.UUKstar.T, self.UUKstar)/denom
+            SUKstarTUkStar += np.dot(self.UUKstar.T, self.UUKstar)/denom
         
         # see Carl Rasmussen's book on GPs, Equation 2.24
         # or Equation 5 in Lasso-LMM paper
         Var_star = part1 - SUKstarTUkStar
         
         return Var_star
 
@@ -914,25 +915,25 @@
             S_nonz=(S_>1E-9)
         assert sum(S_nonz) > 0, "Some eigenvalues should be nonzero"
         S = S_[S_nonz]
         U = U_[:, S_nonz]
         Sdi = 1 / S
 
         res_sig = res.T.dot(Sdi * U).dot(U.T)
-        logdetK = SP.log(S).sum()
+        logdetK = np.log(S).sum()
 
         # some sanity checks
         if False:
             res_sig3 = SP.linalg.pinv(sigma).dot(res)
             NP.testing.assert_array_almost_equal(res_sig, res_sig3, decimal=2)
 
         # see Carl Rasmussen's book on GPs, equation 5.10, or 
         term1 = -0.5 * logdetK
-        term2 = -0.5 * SP.dot(res_sig.reshape(-1).T, res.reshape(-1)) #Change the inputs to the functions so that these are vectors, not 1xn,nx1
-        term3 = -0.5 * len(res) * SP.log(2 * SP.pi)
+        term2 = -0.5 * np.dot(res_sig.reshape(-1).T, res.reshape(-1)) #Change the inputs to the functions so that these are vectors, not 1xn,nx1
+        term3 = -0.5 * len(res) * np.log(2 * SP.pi)
 
         if term2 < -10000:
             logging.warning("looks like nLLeval_test is running into numerical difficulties")
 
             SC = S.copy()
             SC.sort()
```

### Comparing `fastlmm-0.6.4/fastlmm/inference/lmm2k.py` & `fastlmm-0.6.5/fastlmm/inference/lmm2k.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import absolute_import
 from __future__ import print_function
 import scipy as SP
 import numpy as NP
+import numpy as np
 import scipy.linalg as LA
 import scipy.optimize as opt
 import scipy.stats as ST
 import scipy.special as SS
 from fastlmm.util.mingrid import *
 from fastlmm.util.util import *
 import time
@@ -432,27 +433,27 @@
         UXS = dotDiag(self.UX, Sd, minVal = 0.0, symmetric = False, exponent = -1.0)
         UYS = dotDiag(self.UY, Sd, minVal = 0.0, symmetric = False, exponent = -1.0)
 
         XKX = UXS.T.dot(self.UX)
         XKy = UXS.T.dot(self.Uy)
         yKy = UyS.T.dot(self.Uy)
 
-        logdetK = SP.log(Sd).sum()
+        logdetK = np.log(Sd).sum()
 
 
         if (k<N):#low rank part
         
             # determine normalization factor
             denom = (1.0*scale)
             
 
             XKX += self.UUX.T.dot(self.UUX)/(denom)
             XKy += self.UUX.T.dot(self.UUy)/(denom)
             yKy += self.UUy.T.dot(self.UUy)/(denom)      
-            logdetK+=(N-k) * SP.log(denom)
+            logdetK+=(N-k) * np.log(denom)
  
         # proximal contamination (see Supplement Note 2: An Efficient Algorithm for Avoiding Proximal Contamination)
         # available at: http://www.nature.com/nmeth/journal/v9/n6/extref/nmeth.2037-S1.pdf
         # exclude SNPs from the RRM in the likelihood evaluation
         
 
         if len(self.exclude_idx) > 0:
@@ -492,65 +493,65 @@
             assert UWy.shape == (num_exclude,)
             
             # compute S_WW^{-1} * UWX
             WX = UWX / NP.lib.stride_tricks.as_strided(S_WW, (S_WW.size,UWX.shape[1]), (S_WW.itemsize,0))
             # compute S_WW^{-1} * UWy
             Wy = UWy / S_WW
             # determinant update
-            logdetK += SP.log(S_WW).sum()
+            logdetK += np.log(S_WW).sum()
             assert WX.shape == (num_exclude, D)
             assert Wy.shape == (num_exclude,)
             
             # perform updates (instantiations for a and b in Equation (1.5) of Supplement)
             yKy += UWy.T.dot(Wy)
             XKy += UWX.T.dot(Wy)
             XKX += UWX.T.dot(WX)
             
 
         #######
 
         [SxKx,UxKx]= LA.eigh(XKX)
         i_pos = SxKx>1E-10
-        beta = SP.dot(UxKx[:,i_pos],(SP.dot(UxKx[:,i_pos].T,XKy)/SxKx[i_pos]))
+        beta = np.dot(UxKx[:,i_pos],(np.dot(UxKx[:,i_pos].T,XKy)/SxKx[i_pos]))
 
         r2 = yKy-XKy.dot(beta)
 
         if dof is None:#Use the Multivariate Gaussian
             if REML:
                 XX = self.X.T.dot(self.X)
                 [Sxx,Uxx]= LA.eigh(XX)
-                logdetXX  = SP.log(Sxx).sum()
-                logdetXKX = SP.log(SxKx).sum()
+                logdetXX  = np.log(Sxx).sum()
+                logdetXKX = np.log(SxKx).sum()
                 sigma2 = r2 / (N - D)
-                nLL =  0.5 * ( logdetK + logdetXKX - logdetXX + (N-D) * ( SP.log(2.0*SP.pi*sigma2) + 1 ) )
+                nLL =  0.5 * ( logdetK + logdetXKX - logdetXX + (N-D) * ( np.log(2.0*SP.pi*sigma2) + 1 ) )
             else:
                 sigma2 = r2 / (N)
-                nLL =  0.5 * ( logdetK + N * ( SP.log(2.0*SP.pi*sigma2) + 1 ) )
+                nLL =  0.5 * ( logdetK + N * ( np.log(2.0*SP.pi*sigma2) + 1 ) )
             result = {
                   'nLL':nLL,
                   'sigma2':sigma2,
                   'beta':beta,
                   'gamma1':gamma1,
                   'REML':REML,
                   'gamma0':self.gamma0,
                   'delta':self.delta,
                   'scale':scale
                   }
         else:#Use multivariate student-t
             if REML:
                 XX = self.X.T.dot(self.X)
                 [Sxx,Uxx]= LA.eigh(XX)
-                logdetXX  = SP.log(Sxx).sum()
-                logdetXKX = SP.log(SxKx).sum()
+                logdetXX  = np.log(Sxx).sum()
+                logdetXKX = np.log(SxKx).sum()
 
-                nLL =  0.5 * ( logdetK + logdetXKX - logdetXX + (dof + (N-D)) * SP.log(1.0+r2/dof) )
-                nLL += 0.5 * (N-D)*SP.log( dof*SP.pi ) + SS.gammaln( 0.5*dof ) - SS.gammaln( 0.5* (dof + (N-D) ))
+                nLL =  0.5 * ( logdetK + logdetXKX - logdetXX + (dof + (N-D)) * np.log(1.0+r2/dof) )
+                nLL += 0.5 * (N-D)*np.log( dof*SP.pi ) + SS.gammaln( 0.5*dof ) - SS.gammaln( 0.5* (dof + (N-D) ))
             else:
-                nLL =   0.5 * ( logdetK + (dof + N) * SP.log(1.0+r2/dof) )
-                nLL +=  0.5 * N*SP.log( dof*SP.pi ) + SS.gammaln( 0.5*dof ) - SS.gammaln( 0.5* (dof + N ))
+                nLL =   0.5 * ( logdetK + (dof + N) * np.log(1.0+r2/dof) )
+                nLL +=  0.5 * N*np.log( dof*SP.pi ) + SS.gammaln( 0.5*dof ) - SS.gammaln( 0.5* (dof + N ))
             result = {
                   'nLL':nLL,
                   'dof':dof,
                   'sigma2':sigma2,
                   'beta':beta,
                   'gamma1':gamma1,
                   'REML':REML,
```

### Comparing `fastlmm-0.6.4/fastlmm/inference/lmm_cov.py` & `fastlmm-0.6.5/fastlmm/inference/lmm_cov.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # flake8: noqa: E501
 
 import numpy as np
+import warnings
 import scipy.optimize as opt
 import scipy.stats as st
 import scipy.special as ss
 from fastlmm.util.mingrid import *
 from fastlmm.util.util import *
 import time
 import pysnptools.util as pstutil
@@ -1031,15 +1032,17 @@
             logdetK += np.log(np.absolute(S_WW)).sum()
 
             ########
 
         if Usnps is not None:
             penalty_ = penalty or 0.0
             assert penalty_ >= 0.0, "penalty has to be non-negative"
-            beta = snpsKY / (snpsKsnps + penalty_)
+            with warnings.catch_warnings():
+                warnings.filterwarnings('ignore', category=RuntimeWarning, message='invalid value encountered in divide')
+                beta = snpsKY / (snpsKsnps + penalty_)
             if np.isnan(beta.min()):
                 logging.debug(
                     "NaN beta value seen, may be due to an SNC (a constant SNP)"
                 )
                 beta[snpsKY == 0] = 0.0
             variance_explained_beta = snpsKY * beta
             r2 = YKY[np.newaxis, :] - variance_explained_beta
@@ -1050,15 +1053,17 @@
                     * (snpsKsnps / ((snpsKsnps + penalty_) * (snpsKsnps + penalty_)))
                 )  # note that we assume the loss in DOF is 1 here, even though it is less, so the
                 # variance estimate is conservative, due to N-1 for penalty case
                 variance_explained_beta *= (snpsKsnps / (snpsKsnps + penalty_)) * (
                     snpsKsnps / (snpsKsnps + penalty_)
                 )
             else:
-                variance_beta = r2 / (N - 1.0) / snpsKsnps
+                with warnings.catch_warnings():
+                    warnings.filterwarnings('ignore', category=RuntimeWarning, message='divide by zero encountered in divide')
+                    variance_beta = r2 / (N - 1.0) / snpsKsnps
                 fraction_variance_explained_beta = (
                     variance_explained_beta / YKY[np.newaxis, :]
                 )  # variance explained by beta over total variance
         else:
             r2 = YKY
             beta = None
             variance_beta = None
```

### Comparing `fastlmm-0.6.4/fastlmm/inference/tests/test.py` & `fastlmm-0.6.5/fastlmm/inference/tests/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import absolute_import
 import numpy as NP
+import numpy as np
 import scipy as SP
 import scipy.io as SIO
 import scipy.linalg as LA
 from fastlmm.inference.laplace import LaplaceGLMM_N3K1, LaplaceGLMM_N1K3
 from fastlmm.inference.ep import EPGLMM_N3K1, EPGLMM_N1K3
 from fastlmm.inference import getLMM
 import unittest
@@ -20,15 +21,15 @@
         self._N = 50
         self._D = 1
         self._M = 2
         self._k0 = 5
         self._k1 = 10
         self._a2 = 0.4
         self._logdelta = +1
-        self._beta = SP.array([1.2])
+        self._beta = np.array([1.2])
 
         from numpy.random import RandomState
 
         randomstate = RandomState(621360)
         self._X = randomstate.randn(self._N, self._D)
         self._G0 = randomstate.randn(self._N, self._k0)
         self._G1 = randomstate.randn(self._N, self._k1)
@@ -43,29 +44,29 @@
         model.setG(G0=self._G0, G1=self._G1, a2=self._a2)
         model.setX(self._X)
         model.sety(self._y)
 
         # logdelta space
         model.setTestData(Xstar=self._Xstar, G0star=self._G0star, G1star=self._G1star)
         ystar = model.predictMean(self._beta, logdelta=self._logdelta)
-        Gstar = SP.concatenate(
-            (SP.sqrt(1.0 - self._a2) * self._G0star, SP.sqrt(self._a2) * self._G1star),
+        Gstar = np.concatenate(
+            (np.sqrt(1.0 - self._a2) * self._G0star, np.sqrt(self._a2) * self._G1star),
             1,
         )
         weights = model.getPosteriorWeights(beta=self._beta, logdelta=self._logdelta)
-        ystar2 = SP.dot(self._Xstar, self._beta) + SP.dot(Gstar, weights)
+        ystar2 = np.dot(self._Xstar, self._beta) + np.dot(Gstar, weights)
         self.assertAlmostEqual(ystar[0], ystar2[0])
         self.assertAlmostEqual(ystar[1], ystar2[1])
 
         # h2 space
         # TODO: this passes on the above toy data but fails on realistic data, fix!
         # h2 = 0.5
         # ystar = model.predictMean(self._beta,h2=h2)
         # weights = model.getPosteriorWeights(beta=self._beta,h2=h2)
-        # ystar2 = SP.dot(self._Xstar,self._beta) + SP.dot(Gstar,weights)
+        # ystar2 = np.dot(self._Xstar,self._beta) + np.dot(Gstar,weights)
         # self.assertAlmostEqual(ystar[0],ystar2[0])
         # self.assertAlmostEqual(ystar[1],ystar2[1])
 
     def test_nLLeval_1(self):
         """
         small regression test to check negative log likelihood function
```

### Comparing `fastlmm-0.6.4/fastlmm/inference/tests/test_fastlmm_predictor.py` & `fastlmm-0.6.5/fastlmm/inference/tests/test_fastlmm_predictor.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/inference/tests/test_linear_regression.py` & `fastlmm-0.6.5/fastlmm/inference/tests/test_linear_regression.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/altset_list/Consecutive.py` & `fastlmm-0.6.5/fastlmm/pyplink/altset_list/Consecutive.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/altset_list/MinMaxSetSize.py` & `fastlmm-0.6.5/fastlmm/pyplink/altset_list/MinMaxSetSize.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py` & `fastlmm-0.6.5/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/altset_list/Subset.py` & `fastlmm-0.6.5/fastlmm/pyplink/altset_list/Subset.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/altset_list/__init__.py` & `fastlmm-0.6.5/fastlmm/pyplink/altset_list/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/plink.py` & `fastlmm-0.6.5/fastlmm/pyplink/plink.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/setup.py` & `fastlmm-0.6.5/fastlmm/pyplink/setup.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpreader/Bed.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpreader/Bed.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpreader/Dat.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpreader/Dat.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpreader/Hdf5.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpreader/Hdf5.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpset/AllSnps.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpset/AllSnps.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpset/PositionRange.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpset/PositionRange.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpset/RandomSnpSet.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpset/RandomSnpSet.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpset/SnpIndexList.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpset/SnpIndexList.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpset/SnpSetAndName.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpset/SnpSetAndName.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpset/SnpsFromFile.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpset/SnpsFromFile.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/snpset/__init__.py` & `fastlmm-0.6.5/fastlmm/pyplink/snpset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/test.py` & `fastlmm-0.6.5/fastlmm/pyplink/test.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/pyplink/vcfpy.py` & `fastlmm-0.6.5/fastlmm/pyplink/vcfpy.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/NearBronze.py` & `fastlmm-0.6.5/fastlmm/util/NearBronze.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/VertexCut.py` & `fastlmm-0.6.5/fastlmm/util/VertexCut.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/_example_file.py` & `fastlmm-0.6.5/fastlmm/util/_example_file.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/computePC.py` & `fastlmm-0.6.5/fastlmm/util/computePC.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/compute_auto_pcs.py` & `fastlmm-0.6.5/fastlmm/util/compute_auto_pcs.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/est_h2.py` & `fastlmm-0.6.5/fastlmm/util/est_h2.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/fastlmm.hashdown.json` & `fastlmm-0.6.5/fastlmm/util/fastlmm.hashdown.json`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/genphen.py` & `fastlmm-0.6.5/fastlmm/util/genphen.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/gensnp.py` & `fastlmm-0.6.5/fastlmm/util/gensnp.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/matrix/mmultfile.py` & `fastlmm-0.6.5/fastlmm/util/matrix/mmultfile.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/mingrid.py` & `fastlmm-0.6.5/fastlmm/util/mingrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import absolute_import
 from __future__ import print_function
 import scipy as SP
+import numpy as np
 import scipy.optimize as opt
 from six.moves import range
 
 
 def minimize1D(f, evalgrid = None, nGrid=10, minval=0.0, maxval = 0.99999, verbose=False, brent=True,check_boundaries = True, resultgrid=None, return_grid=False):
     '''
     minimize a function f(x) in the grid between minval and maxval.
@@ -92,16 +93,16 @@
     else:
         resultgrid = SP.ones(evalgrid.shape[0])*9999999999999.0
     for i in range(evalgrid.shape[0]):        
         fevalgrid = f(evalgrid[i])
 
         is_real=False
         try:
-            is_real = SP.isreal(fevalgrid).all()
+            is_real = np.isreal(fevalgrid).all()
         except:
-            is_real = SP.isreal(fevalgrid)
+            is_real = np.isreal(fevalgrid)
         assert is_real,"function returned imaginary value"
 
         resultgrid[i] = fevalgrid
     return (evalgrid,resultgrid)
```

### Comparing `fastlmm-0.6.4/fastlmm/util/pickle_io.py` & `fastlmm-0.6.5/fastlmm/util/pickle_io.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/preprocess.py` & `fastlmm-0.6.5/fastlmm/util/preprocess.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/run_fastlmmc.py` & `fastlmm-0.6.5/fastlmm/util/run_fastlmmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     eigenOut    save the spectral decomposition object to the directory name
     maxThreads  suggests the level of parallelism to use
     simOut      specifies that genetic similarities are to be written to this file
     topKbyLinRegdirects AutoSelect to use only the top <int> SNPs, as determined by linear regression, while selecting SNPs
     for more information, we refer to the user-manual of fast-lmm
     '''
     os.environ["FastLmmUseAnyMklLib"] = "1"
-    logging.info('Run FAST-LMM')   
+    logging.info('Run FAST-LMM')
 
     osname = sys.platform
     if (osname.find("win") >= 0):    #         was loaded, if it was loaded from a file
         fastlmmpath = os.path.join(fastlmm_path, "fastlmmc.exe")
     elif (osname.find("linux") >= 0):
         fastlmmpath = os.path.join(fastlmm_path, "fastlmmc")
         import stat
@@ -180,14 +180,13 @@
         cmd += ' -bfileSim %s'%bfileSim
     if topKbyLinReg!=None:
         cmd += ' -topKbyLinReg %d'%topKbyLinReg
     logging.info(cmd)
     
     output = ""
     try:
-        output = subprocess.check_output(cmd,shell=True,stderr=subprocess.STDOUT)
+        output = subprocess.check_output(cmd, shell=True, stderr=subprocess.STDOUT)
     except Exception as e:
         print(e)
     print(output)
-    #LG.info(output)
-    #return output
-
+    # LG.info(output)
+    # return output
```

### Comparing `fastlmm-0.6.4/fastlmm/util/standardizer/Beta.py` & `fastlmm-0.6.5/fastlmm/util/standardizer/Beta.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/standardizer/Unit.py` & `fastlmm-0.6.5/fastlmm/util/standardizer/Unit.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/standardizer/__init__.py` & `fastlmm-0.6.5/fastlmm/util/standardizer/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/stats/__init__.py` & `fastlmm-0.6.5/fastlmm/util/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/stats/chi2mixture.py` & `fastlmm-0.6.5/fastlmm/util/stats/chi2mixture.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/stats/plotp.py` & `fastlmm-0.6.5/fastlmm/util/stats/plotp.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/test.py` & `fastlmm-0.6.5/fastlmm/util/test.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm/util/util.py` & `fastlmm-0.6.5/fastlmm/util/util.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.4/fastlmm.egg-info/PKG-INFO` & `fastlmm-0.6.5/fastlmm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlmm
-Version: 0.6.4
+Version: 0.6.5
 Summary: Fast GWAS
 Home-page: https://fastlmm.github.io/
 Author: FaST-LMM Team
 Author-email: fastlmm-dev@python.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/fastlmm/FaST-LMM/issues
 Project-URL: Documentation, http://fastlmm.github.io/FaST-LMM
```

### Comparing `fastlmm-0.6.4/fastlmm.egg-info/SOURCES.txt` & `fastlmm-0.6.5/fastlmm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -141,8 +141,9 @@
 fastlmm/util/matrix/__init__.py
 fastlmm/util/matrix/mmultfile.py
 fastlmm/util/standardizer/Beta.py
 fastlmm/util/standardizer/Unit.py
 fastlmm/util/standardizer/__init__.py
 fastlmm/util/stats/__init__.py
 fastlmm/util/stats/chi2mixture.py
-fastlmm/util/stats/plotp.py
+fastlmm/util/stats/plotp.py
+tests/test.py
```

### Comparing `fastlmm-0.6.4/setup.py` & `fastlmm-0.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Work around https://github.com/pypa/pip/issues/7953
 import site
 import sys
 
 site.ENABLE_USER_SITE = "--user" in sys.argv[1:]
 
 # Version number
-version = "0.6.4"
+version = "0.6.5"
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
```

