# Comparing `tmp/mogptk-0.3.3.tar.gz` & `tmp/mogptk-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mogptk-0.3.3.tar", last modified: Fri Apr 14 14:08:24 2023, max compression
+gzip compressed data, was "mogptk-0.3.4.tar", last modified: Wed May  3 14:38:50 2023, max compression
```

## Comparing `mogptk-0.3.3.tar` & `mogptk-0.3.4.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.656745 mogptk-0.3.3/
--rw-r--r--   0 taco      (1000) users      (100)      115 2022-04-24 22:51:10.000000 mogptk-0.3.3/.gitignore
--rw-r--r--   0 taco      (1000) users      (100)     1052 2019-08-30 20:58:49.000000 mogptk-0.3.3/LICENSE
--rw-r--r--   0 taco      (1000) users      (100)       26 2022-04-24 02:23:55.000000 mogptk-0.3.3/MANIFEST.in
--rw-r--r--   0 taco      (1000) users      (100)    10833 2023-04-14 14:08:24.656745 mogptk-0.3.3/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)    10432 2023-03-31 14:19:49.000000 mogptk-0.3.3/README.md
--rwxr-xr-x   0 taco      (1000) users      (100)       99 2022-06-01 13:42:52.000000 mogptk-0.3.3/build.sh
--rwxr-xr-x   0 taco      (1000) users      (100)     1083 2022-07-14 17:48:19.000000 mogptk-0.3.3/build_docs.sh
--rw-r--r--   0 taco      (1000) users      (100)     2101 2020-02-07 16:46:12.000000 mogptk-0.3.3/config.mako
--rw-r--r--   0 taco      (1000) users      (100)       66 2020-02-06 15:45:19.000000 mogptk-0.3.3/head.mako
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.653412 mogptk-0.3.3/mogptk/
--rw-r--r--   0 taco      (1000) users      (100)      360 2022-06-28 22:19:05.000000 mogptk-0.3.3/mogptk/__init__.py
--rw-r--r--   0 taco      (1000) users      (100)    56121 2022-06-28 23:33:16.000000 mogptk-0.3.3/mogptk/data.py
--rw-r--r--   0 taco      (1000) users      (100)    29065 2022-05-26 18:32:31.000000 mogptk-0.3.3/mogptk/dataset.py
--rw-r--r--   0 taco      (1000) users      (100)     7226 2022-05-12 16:46:24.000000 mogptk-0.3.3/mogptk/documentation.md
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.656745 mogptk-0.3.3/mogptk/gpr/
--rw-r--r--   0 taco      (1000) users      (100)      260 2022-04-20 16:31:55.000000 mogptk-0.3.3/mogptk/gpr/__init__.py
--rw-r--r--   0 taco      (1000) users      (100)     2738 2022-05-10 02:07:17.000000 mogptk-0.3.3/mogptk/gpr/config.py
--rw-r--r--   0 taco      (1000) users      (100)    16624 2022-06-28 22:03:02.000000 mogptk-0.3.3/mogptk/gpr/kernel.py
--rw-r--r--   0 taco      (1000) users      (100)    26313 2022-06-14 15:18:49.000000 mogptk-0.3.3/mogptk/gpr/likelihood.py
--rw-r--r--   0 taco      (1000) users      (100)     3119 2022-08-02 19:14:49.000000 mogptk-0.3.3/mogptk/gpr/mean.py
--rw-r--r--   0 taco      (1000) users      (100)    38753 2023-03-22 02:23:05.000000 mogptk-0.3.3/mogptk/gpr/model.py
--rw-r--r--   0 taco      (1000) users      (100)    29785 2022-12-29 15:57:38.000000 mogptk-0.3.3/mogptk/gpr/multioutput.py
--rw-r--r--   0 taco      (1000) users      (100)    10377 2022-05-21 17:05:07.000000 mogptk-0.3.3/mogptk/gpr/parameter.py
--rw-r--r--   0 taco      (1000) users      (100)     1209 2023-03-22 02:14:00.000000 mogptk-0.3.3/mogptk/gpr/plot.py
--rw-r--r--   0 taco      (1000) users      (100)    29625 2022-06-28 22:33:08.000000 mogptk-0.3.3/mogptk/gpr/singleoutput.py
--rw-r--r--   0 taco      (1000) users      (100)     2451 2022-05-09 21:37:57.000000 mogptk-0.3.3/mogptk/gpr/util.py
--rw-r--r--   0 taco      (1000) users      (100)     5701 2023-03-22 02:04:42.000000 mogptk-0.3.3/mogptk/init.py
--rw-r--r--   0 taco      (1000) users      (100)    41046 2023-03-28 15:50:48.000000 mogptk-0.3.3/mogptk/model.py
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.656745 mogptk-0.3.3/mogptk/models/
--rw-r--r--   0 taco      (1000) users      (100)        0 2022-03-01 22:37:51.000000 mogptk-0.3.3/mogptk/models/__init__.py
--rw-r--r--   0 taco      (1000) users      (100)     4693 2022-12-29 15:58:20.000000 mogptk-0.3.3/mogptk/models/conv.py
--rw-r--r--   0 taco      (1000) users      (100)     5113 2022-12-29 15:58:44.000000 mogptk-0.3.3/mogptk/models/csm.py
--rw-r--r--   0 taco      (1000) users      (100)     7226 2022-12-29 15:58:53.000000 mogptk-0.3.3/mogptk/models/mohsm.py
--rw-r--r--   0 taco      (1000) users      (100)    12081 2022-12-29 15:59:00.000000 mogptk-0.3.3/mogptk/models/mosm.py
--rw-r--r--   0 taco      (1000) users      (100)     7516 2022-12-29 15:59:17.000000 mogptk-0.3.3/mogptk/models/sm.py
--rw-r--r--   0 taco      (1000) users      (100)     5551 2022-12-29 15:59:09.000000 mogptk-0.3.3/mogptk/models/sm_lmc.py
--rw-r--r--   0 taco      (1000) users      (100)     4715 2022-05-25 17:06:55.000000 mogptk-0.3.3/mogptk/transformer.py
--rw-r--r--   0 taco      (1000) users      (100)    10128 2022-05-31 15:51:52.000000 mogptk-0.3.3/mogptk/util.py
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-04-14 14:08:24.653412 mogptk-0.3.3/mogptk.egg-info/
--rw-r--r--   0 taco      (1000) users      (100)    10833 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)      810 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/SOURCES.txt
--rw-r--r--   0 taco      (1000) users      (100)        1 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/dependency_links.txt
--rw-r--r--   0 taco      (1000) users      (100)       74 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/requires.txt
--rw-r--r--   0 taco      (1000) users      (100)        7 2023-04-14 14:08:24.000000 mogptk-0.3.3/mogptk.egg-info/top_level.txt
--rwxr-xr-x   0 taco      (1000) users      (100)       36 2020-01-27 19:27:01.000000 mogptk-0.3.3/publish.sh
--rw-r--r--   0 taco      (1000) users      (100)       79 2023-04-14 14:08:24.656745 mogptk-0.3.3/setup.cfg
--rw-r--r--   0 taco      (1000) users      (100)      944 2023-04-14 14:07:40.000000 mogptk-0.3.3/setup.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-03 14:38:50.047685 mogptk-0.3.4/
+-rw-r--r--   0 taco      (1000) users      (100)      115 2022-04-24 22:51:10.000000 mogptk-0.3.4/.gitignore
+-rw-r--r--   0 taco      (1000) users      (100)     1052 2019-08-30 20:58:49.000000 mogptk-0.3.4/LICENSE
+-rw-r--r--   0 taco      (1000) users      (100)       26 2022-04-24 02:23:55.000000 mogptk-0.3.4/MANIFEST.in
+-rw-r--r--   0 taco      (1000) users      (100)    11080 2023-05-03 14:38:50.047685 mogptk-0.3.4/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)    10679 2023-05-03 14:36:55.000000 mogptk-0.3.4/README.md
+-rwxr-xr-x   0 taco      (1000) users      (100)       99 2022-06-01 13:42:52.000000 mogptk-0.3.4/build.sh
+-rwxr-xr-x   0 taco      (1000) users      (100)     1083 2022-07-14 17:48:19.000000 mogptk-0.3.4/build_docs.sh
+-rw-r--r--   0 taco      (1000) users      (100)     2101 2020-02-07 16:46:12.000000 mogptk-0.3.4/config.mako
+-rw-r--r--   0 taco      (1000) users      (100)       66 2020-02-06 15:45:19.000000 mogptk-0.3.4/head.mako
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-03 14:38:50.044351 mogptk-0.3.4/mogptk/
+-rw-r--r--   0 taco      (1000) users      (100)      360 2022-06-28 22:19:05.000000 mogptk-0.3.4/mogptk/__init__.py
+-rw-r--r--   0 taco      (1000) users      (100)    56121 2022-06-28 23:33:16.000000 mogptk-0.3.4/mogptk/data.py
+-rw-r--r--   0 taco      (1000) users      (100)    29065 2022-05-26 18:32:31.000000 mogptk-0.3.4/mogptk/dataset.py
+-rw-r--r--   0 taco      (1000) users      (100)     7226 2022-05-12 16:46:24.000000 mogptk-0.3.4/mogptk/documentation.md
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-03 14:38:50.044351 mogptk-0.3.4/mogptk/gpr/
+-rw-r--r--   0 taco      (1000) users      (100)      260 2022-04-20 16:31:55.000000 mogptk-0.3.4/mogptk/gpr/__init__.py
+-rw-r--r--   0 taco      (1000) users      (100)     2738 2022-05-10 02:07:17.000000 mogptk-0.3.4/mogptk/gpr/config.py
+-rw-r--r--   0 taco      (1000) users      (100)    16638 2023-04-16 21:56:38.000000 mogptk-0.3.4/mogptk/gpr/kernel.py
+-rw-r--r--   0 taco      (1000) users      (100)    26313 2022-06-14 15:18:49.000000 mogptk-0.3.4/mogptk/gpr/likelihood.py
+-rw-r--r--   0 taco      (1000) users      (100)     3119 2022-08-02 19:14:49.000000 mogptk-0.3.4/mogptk/gpr/mean.py
+-rw-r--r--   0 taco      (1000) users      (100)    38761 2023-05-03 13:44:32.000000 mogptk-0.3.4/mogptk/gpr/model.py
+-rw-r--r--   0 taco      (1000) users      (100)    29785 2022-12-29 15:57:38.000000 mogptk-0.3.4/mogptk/gpr/multioutput.py
+-rw-r--r--   0 taco      (1000) users      (100)    10377 2022-05-21 17:05:07.000000 mogptk-0.3.4/mogptk/gpr/parameter.py
+-rw-r--r--   0 taco      (1000) users      (100)     1209 2023-03-22 02:14:00.000000 mogptk-0.3.4/mogptk/gpr/plot.py
+-rw-r--r--   0 taco      (1000) users      (100)    29625 2022-06-28 22:33:08.000000 mogptk-0.3.4/mogptk/gpr/singleoutput.py
+-rw-r--r--   0 taco      (1000) users      (100)     2451 2022-05-09 21:37:57.000000 mogptk-0.3.4/mogptk/gpr/util.py
+-rw-r--r--   0 taco      (1000) users      (100)     5701 2023-03-22 02:04:42.000000 mogptk-0.3.4/mogptk/init.py
+-rw-r--r--   0 taco      (1000) users      (100)    41095 2023-05-03 14:03:21.000000 mogptk-0.3.4/mogptk/model.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-03 14:38:50.047685 mogptk-0.3.4/mogptk/models/
+-rw-r--r--   0 taco      (1000) users      (100)        0 2022-03-01 22:37:51.000000 mogptk-0.3.4/mogptk/models/__init__.py
+-rw-r--r--   0 taco      (1000) users      (100)     4693 2022-12-29 15:58:20.000000 mogptk-0.3.4/mogptk/models/conv.py
+-rw-r--r--   0 taco      (1000) users      (100)     5113 2022-12-29 15:58:44.000000 mogptk-0.3.4/mogptk/models/csm.py
+-rw-r--r--   0 taco      (1000) users      (100)     7226 2022-12-29 15:58:53.000000 mogptk-0.3.4/mogptk/models/mohsm.py
+-rw-r--r--   0 taco      (1000) users      (100)    12081 2022-12-29 15:59:00.000000 mogptk-0.3.4/mogptk/models/mosm.py
+-rw-r--r--   0 taco      (1000) users      (100)     7516 2022-12-29 15:59:17.000000 mogptk-0.3.4/mogptk/models/sm.py
+-rw-r--r--   0 taco      (1000) users      (100)     5551 2022-12-29 15:59:09.000000 mogptk-0.3.4/mogptk/models/sm_lmc.py
+-rw-r--r--   0 taco      (1000) users      (100)     4715 2022-05-25 17:06:55.000000 mogptk-0.3.4/mogptk/transformer.py
+-rw-r--r--   0 taco      (1000) users      (100)    10128 2022-05-31 15:51:52.000000 mogptk-0.3.4/mogptk/util.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-03 14:38:50.044351 mogptk-0.3.4/mogptk.egg-info/
+-rw-r--r--   0 taco      (1000) users      (100)    11080 2023-05-03 14:38:49.000000 mogptk-0.3.4/mogptk.egg-info/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)      832 2023-05-03 14:38:50.000000 mogptk-0.3.4/mogptk.egg-info/SOURCES.txt
+-rw-r--r--   0 taco      (1000) users      (100)        1 2023-05-03 14:38:49.000000 mogptk-0.3.4/mogptk.egg-info/dependency_links.txt
+-rw-r--r--   0 taco      (1000) users      (100)       74 2023-05-03 14:38:49.000000 mogptk-0.3.4/mogptk.egg-info/requires.txt
+-rw-r--r--   0 taco      (1000) users      (100)        7 2023-05-03 14:38:49.000000 mogptk-0.3.4/mogptk.egg-info/top_level.txt
+-rwxr-xr-x   0 taco      (1000) users      (100)       36 2020-01-27 19:27:01.000000 mogptk-0.3.4/publish.sh
+-rw-r--r--   0 taco      (1000) users      (100)       79 2023-05-03 14:38:50.047685 mogptk-0.3.4/setup.cfg
+-rw-r--r--   0 taco      (1000) users      (100)      944 2023-05-03 14:35:09.000000 mogptk-0.3.4/setup.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-05-03 14:38:50.047685 mogptk-0.3.4/tests/
+-rw-r--r--   0 taco      (1000) users      (100)     2156 2022-05-14 03:11:31.000000 mogptk-0.3.4/tests/test_kernels.py
```

### Comparing `mogptk-0.3.3/LICENSE` & `mogptk-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/PKG-INFO` & `mogptk-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mogptk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Multi-Output Gaussian Process ToolKit
 Home-page: https://github.com/GAMES-UChile/mogptk
 Author: Taco de Wolff, Alejandro Cuevas, Felipe Tobar
 Author-email: tacodewolff@gmail.com
 License: MIT
 Keywords: MOGP,MOSM,GP,Gaussian Process,Multi-Output,Tobar,Parra
 Requires-Python: >=3.6
@@ -95,14 +95,16 @@
 
 **[05 - Error Metrics](https://games-uchile.github.io/mogptk/examples.html?q=05_Error_Metrics)** Obtain different metrics in order to compare models.
 
 **[06 - Custom Kernels and Mean Functions](https://games-uchile.github.io/mogptk/examples.html?q=06_Custom_Kernels_and_Mean_Functions)** Use or create custom kernels as well as training custom mean functions.
 
 **[07 - Sparse Multi Input](https://games-uchile.github.io/mogptk/examples.html?q=07_Sparse_Multi_Input)** Use 8 input dimensions to train the Abalone data set using sparse GPs.
 
+**[08 - Multi Likelihood Classification](https://games-uchile.github.io/mogptk/examples.html?q=08_Multi_Likelihood_Classification)** Use a different likelihood for each channel, one Bernoulli for classification and one StudentT's for regression.
+
 ## Examples
 
 **[Airline passengers](https://games-uchile.github.io/mogptk/examples.html?q=example_airline_passengers)**: Regression using a single output spectral mixture on the yearly number of passengers of an airline.
 
 **[Seasonal CO2 of Mauna-Loa](https://games-uchile.github.io/mogptk/examples.html?q=example_mauna_loa)**: Regression using a single output spectral mixture on the CO2 concentration at Mauna-Loa throughout many years.
 
 **[Currency Exchange](https://games-uchile.github.io/mogptk/examples.html?q=example_currency_exchange)**: Model training, interpretation and comparison on a dataset of 11 currency exchange rates (against the dollar) from 2017 and 2018. These 11 channels are fitted with the MOSM, SM-LMC, CSM, and CONV kernels and their results are compared and interpreted.
```

### Comparing `mogptk-0.3.3/README.md` & `mogptk-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 
 **[05 - Error Metrics](https://games-uchile.github.io/mogptk/examples.html?q=05_Error_Metrics)** Obtain different metrics in order to compare models.
 
 **[06 - Custom Kernels and Mean Functions](https://games-uchile.github.io/mogptk/examples.html?q=06_Custom_Kernels_and_Mean_Functions)** Use or create custom kernels as well as training custom mean functions.
 
 **[07 - Sparse Multi Input](https://games-uchile.github.io/mogptk/examples.html?q=07_Sparse_Multi_Input)** Use 8 input dimensions to train the Abalone data set using sparse GPs.
 
+**[08 - Multi Likelihood Classification](https://games-uchile.github.io/mogptk/examples.html?q=08_Multi_Likelihood_Classification)** Use a different likelihood for each channel, one Bernoulli for classification and one StudentT's for regression.
+
 ## Examples
 
 **[Airline passengers](https://games-uchile.github.io/mogptk/examples.html?q=example_airline_passengers)**: Regression using a single output spectral mixture on the yearly number of passengers of an airline.
 
 **[Seasonal CO2 of Mauna-Loa](https://games-uchile.github.io/mogptk/examples.html?q=example_mauna_loa)**: Regression using a single output spectral mixture on the CO2 concentration at Mauna-Loa throughout many years.
 
 **[Currency Exchange](https://games-uchile.github.io/mogptk/examples.html?q=example_currency_exchange)**: Model training, interpretation and comparison on a dataset of 11 currency exchange rates (against the dollar) from 2017 and 2018. These 11 channels are fitted with the MOSM, SM-LMC, CSM, and CONV kernels and their results are compared and interpreted.
```

### Comparing `mogptk-0.3.3/build_docs.sh` & `mogptk-0.3.4/build_docs.sh`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/config.mako` & `mogptk-0.3.4/config.mako`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/data.py` & `mogptk-0.3.4/mogptk/data.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/dataset.py` & `mogptk-0.3.4/mogptk/dataset.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/documentation.md` & `mogptk-0.3.4/mogptk/documentation.md`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/gpr/config.py` & `mogptk-0.3.4/mogptk/gpr/config.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/gpr/kernel.py` & `mogptk-0.3.4/mogptk/gpr/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 X2 = torch.index_select(X2, dim=1, index=self.active_dims)
         return X1, X2
 
     def _check_input(self, X1, X2=None):
         if not torch.is_tensor(X1):
             X1 = torch.tensor(X1, device=config.device, dtype=config.dtype)
         elif X1.device != config.device or X1.dtype != config.dtype:
-            X1 = X1.to(device, dtype)
+            X1 = X1.to(config.device, config.dtype)
         if X1.ndim != 2:
             raise ValueError("X should have two dimensions (data_points,input_dims)")
         if X1.shape[0] == 0 or X1.shape[1] == 0:
             raise ValueError("X must not be empty")
         if X2 is not None:
             if not torch.is_tensor(X2):
                 X2 = torch.tensor(X2, device=config.device, dtype=config.dtype)
```

### Comparing `mogptk-0.3.3/mogptk/gpr/likelihood.py` & `mogptk-0.3.4/mogptk/gpr/likelihood.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/gpr/mean.py` & `mogptk-0.3.4/mogptk/gpr/mean.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/gpr/model.py` & `mogptk-0.3.4/mogptk/gpr/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -888,8 +888,8 @@
         mean (mogptk.gpr.mean.Mean): Mean.
         name (str): Name of the model.
 
     [1] J. Hensman, et al., "Scalable Variational Gaussian Process Classification", 2015
     """
     def __init__(self, kernel, X, y, likelihood=GaussianLikelihood(1.0), jitter=1e-8,
                  mean=None, name="Hensman"):
-        super().__init__(kernel, X, y, None, likelihood, jitter, mean, name)
+        super().__init__(kernel, X, y, None, 'grid', likelihood, jitter, mean, name)
```

### Comparing `mogptk-0.3.3/mogptk/gpr/multioutput.py` & `mogptk-0.3.4/mogptk/gpr/multioutput.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/gpr/parameter.py` & `mogptk-0.3.4/mogptk/gpr/parameter.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/gpr/plot.py` & `mogptk-0.3.4/mogptk/gpr/plot.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/gpr/singleoutput.py` & `mogptk-0.3.4/mogptk/gpr/singleoutput.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/gpr/util.py` & `mogptk-0.3.4/mogptk/gpr/util.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/init.py` & `mogptk-0.3.4/mogptk/init.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/model.py` & `mogptk-0.3.4/mogptk/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,51 +459,52 @@
             method = 'SGD'
         elif method.lower() == 'adagrad':
             method = 'AdaGrad'
         else:
             raise ValueError('optimizer must be LBFGS, Adam, SGD, or AdaGrad')
 
         if verbose:
-            print('\nStarting optimization using', method)
+            print('Starting optimization using', method)
             if self.name is not None:
                 print('‣ Model: %s' % self.name)
             print('‣ Channels: %d' % len(self.dataset))
             print('‣ Parameters: %d' % self.num_parameters())
             print('‣ Training points: %d' % self.num_training_points())
-            print('‣ Initial loss: %6g' % self.loss())
-            if error is not None:
-                print('‣ Initial error: %6g' % self.error(error, error_use_all_data))
+            print('‣ Iterations: %d' % iters)
 
         iter_offset = 0
         times = np.zeros((iters+1,))
         losses = np.zeros((iters+1,))
         errors = np.zeros((iters+1,))
         if self.times.shape[0] != 0:
             iter_offset = self.times.shape[0]-1
             times = np.concatenate((self.times[:-1],times))
             losses = np.concatenate((self.losses[:-1],losses))
             errors = np.concatenate((self.errors[:-1],errors))
         initial_time = time.time()
+        progress_time = 0.0
 
         iters_len = int(math.log10(iter_offset+iters)) + 1
-        def progress(i, loss):
+        def progress(i, loss, last=False):
+            nonlocal progress_time
+
             elapsed_time = time.time() - initial_time
-            write = verbose and i % max(1,iters/100) == 0
+            write = verbose and (i == 0 or last or 10.0 <= elapsed_time-progress_time)
             i += iter_offset
             times[i] = elapsed_time
             losses[i] = loss
             if error is not None:
                 errors[i] = float(self.error(error, error_use_all_data))
                 if write:
                     print("  %*d/%*d %s  loss=%12g  error=%12g" % (iters_len, i, iters_len, iter_offset+iters, _format_time(elapsed_time), losses[i], errors[i]))
+                    progress_time = elapsed_time
             elif write:
                 print("  %*d/%*d %s  loss=%12g" % (iters_len, i, iters_len, iter_offset+iters, _format_time(elapsed_time), losses[i]))
+                progress_time = elapsed_time
 
-        if verbose:
-            print("\nStart %s:" % (method,))
         if method == 'LBFGS':
             if not 'max_iter' in kwargs:
                 kwargs['max_iter'] = iters
             else:
                 iters = kwargs['max_iter']
             optimizer = torch.optim.LBFGS(self.gpr.parameters(), **kwargs)
 
@@ -521,24 +522,19 @@
                 optimizer = torch.optim.SGD(self.gpr.parameters(), **kwargs)
             elif method == 'AdaGrad':
                 optimizer = torch.optim.Adagrad(self.gpr.parameters(), **kwargs)
 
             for i in range(iters):
                 progress(i, self.loss())
                 optimizer.step()
-        progress(iters, self.loss())
+        progress(iters, self.loss(), last=True)
 
         if verbose:
             elapsed_time = time.time() - initial_time
-            print("Finished")
-            print('\nOptimization finished in %s' % _format_duration(elapsed_time))
-            print('‣ Iterations: %d' % iters)
-            print('‣ Final loss: %6g'% losses[iter_offset+iters])
-            if error is not None:
-                print('‣ Final error: %6g' % errors[iter_offset+iters])
+            print('Optimization finished in %s' % _format_duration(elapsed_time))
 
         self.iters = iter_offset+iters
         self.times = times[:iter_offset+iters+1]
         self.losses = losses[:iter_offset+iters+1]
         if error is not None:
             self.errors = errors[:iter_offset+iters+1]
         if plot:
@@ -579,18 +575,18 @@
         Args:
             X (list, dict): Array of shape (data_points,), (data_points,input_dims), or [(data_points,)] * input_dims per channel with prediction X values. If a dictionary is passed, the index is the channel index or name.
             sigma (float): Number of standard deviations to display upwards and downwards.
             predict_y (boolean): Predict data values instead of function values.
             transformed (boolean): Return transformed data as used for training.
 
         Returns:
-            numpy.ndarray: X prediction of shape (n,) for each channel.
-            numpy.ndarray: Y mean prediction of shape (n,) for each channel.
-            numpy.ndarray: Y lower prediction of uncertainty interval of shape (n,) for each channel.
-            numpy.ndarray: Y upper prediction of uncertainty interval of shape (n,) for each channel.
+            numpy.ndarray: X prediction of shape (data_points,input_dims) for each channel.
+            numpy.ndarray: Y mean prediction of shape (data_points,) for each channel.
+            numpy.ndarray: Y lower prediction of uncertainty interval of shape (data_points,) for each channel.
+            numpy.ndarray: Y upper prediction of uncertainty interval of shape (data_points,) for each channel.
 
         Examples:
             >>> model.predict(X)
         """
         if X is None:
             X = self.dataset.get_prediction_data()
         else:
@@ -629,15 +625,15 @@
         Evaluate the kernel at K(X1,X2).
 
         Args:
             X1 (list, dict): Array of shape (data_points,), (data_points,input_dims), or [(data_points,)] * input_dims per channel with prediction X values. If a dictionary is passed, the index is the channel index or name.
             X2 (list, dict): Same as X1 if None.
 
         Returns:
-            numpy.ndarray: kernel evaluated at X1 and X2 of shape (n1,n2).
+            numpy.ndarray: kernel evaluated at X1 and X2 of shape (data_points1,data_points2).
 
         Examples:
             >>> channel0 = np.array(['1987-05-20', '1987-05-21'])
             >>> channel1 = np.array([[2.5, 534.6], [3.5, 898.22], [4.5, 566.98]])
             >>> model.K([channel0,channel1])
         """
         X1 = self.dataset._format_X(X1)
@@ -740,14 +736,15 @@
         return fig, ax
 
     def plot_prediction(self, X=None, title=None, figsize=None, legend=True, errorbars=True, sigma=2, predict_y=True, transformed=False):
         """
         Plot the data including removed observations, latent function, and predictions of this model for each channel.
 
         Args:
+            X (list, dict): Array of shape (data_points,), (data_points,input_dims), or [(data_points,)] * input_dims per channel with prediction X values. If a dictionary is passed, the index is the channel index or name.
             title (str): Set the title of the plot.
             figsize (tuple): Set the figure size.
             legend (boolean): Disable legend.
             errorbars (boolean): Plot data error bars if available.
             sigma (float): Number of standard deviations to display upwards and downwards.
             predict_y (boolean): Predict data values instead of function values.
             transformed (boolean): Display transformed Y data as used for training.
```

### Comparing `mogptk-0.3.3/mogptk/models/conv.py` & `mogptk-0.3.4/mogptk/models/conv.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/models/csm.py` & `mogptk-0.3.4/mogptk/models/csm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/models/mohsm.py` & `mogptk-0.3.4/mogptk/models/mohsm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/models/mosm.py` & `mogptk-0.3.4/mogptk/models/mosm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/models/sm.py` & `mogptk-0.3.4/mogptk/models/sm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/models/sm_lmc.py` & `mogptk-0.3.4/mogptk/models/sm_lmc.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/transformer.py` & `mogptk-0.3.4/mogptk/transformer.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk/util.py` & `mogptk-0.3.4/mogptk/util.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.3.3/mogptk.egg-info/PKG-INFO` & `mogptk-0.3.4/mogptk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mogptk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Multi-Output Gaussian Process ToolKit
 Home-page: https://github.com/GAMES-UChile/mogptk
 Author: Taco de Wolff, Alejandro Cuevas, Felipe Tobar
 Author-email: tacodewolff@gmail.com
 License: MIT
 Keywords: MOGP,MOSM,GP,Gaussian Process,Multi-Output,Tobar,Parra
 Requires-Python: >=3.6
@@ -95,14 +95,16 @@
 
 **[05 - Error Metrics](https://games-uchile.github.io/mogptk/examples.html?q=05_Error_Metrics)** Obtain different metrics in order to compare models.
 
 **[06 - Custom Kernels and Mean Functions](https://games-uchile.github.io/mogptk/examples.html?q=06_Custom_Kernels_and_Mean_Functions)** Use or create custom kernels as well as training custom mean functions.
 
 **[07 - Sparse Multi Input](https://games-uchile.github.io/mogptk/examples.html?q=07_Sparse_Multi_Input)** Use 8 input dimensions to train the Abalone data set using sparse GPs.
 
+**[08 - Multi Likelihood Classification](https://games-uchile.github.io/mogptk/examples.html?q=08_Multi_Likelihood_Classification)** Use a different likelihood for each channel, one Bernoulli for classification and one StudentT's for regression.
+
 ## Examples
 
 **[Airline passengers](https://games-uchile.github.io/mogptk/examples.html?q=example_airline_passengers)**: Regression using a single output spectral mixture on the yearly number of passengers of an airline.
 
 **[Seasonal CO2 of Mauna-Loa](https://games-uchile.github.io/mogptk/examples.html?q=example_mauna_loa)**: Regression using a single output spectral mixture on the CO2 concentration at Mauna-Loa throughout many years.
 
 **[Currency Exchange](https://games-uchile.github.io/mogptk/examples.html?q=example_currency_exchange)**: Model training, interpretation and comparison on a dataset of 11 currency exchange rates (against the dollar) from 2017 and 2018. These 11 channels are fitted with the MOSM, SM-LMC, CSM, and CONV kernels and their results are compared and interpreted.
```

### Comparing `mogptk-0.3.3/mogptk.egg-info/SOURCES.txt` & `mogptk-0.3.4/mogptk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,8 +35,9 @@
 mogptk/gpr/util.py
 mogptk/models/__init__.py
 mogptk/models/conv.py
 mogptk/models/csm.py
 mogptk/models/mohsm.py
 mogptk/models/mosm.py
 mogptk/models/sm.py
-mogptk/models/sm_lmc.py
+mogptk/models/sm_lmc.py
+tests/test_kernels.py
```

### Comparing `mogptk-0.3.3/setup.py` & `mogptk-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='mogptk',
-      version='0.3.3',
+      version='0.3.4',
       description='Multi-Output Gaussian Process ToolKit',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/GAMES-UChile/mogptk',
       author='Taco de Wolff, Alejandro Cuevas, Felipe Tobar',
       author_email='tacodewolff@gmail.com',
       license='MIT',
```

