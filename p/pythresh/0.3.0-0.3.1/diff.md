# Comparing `tmp/pythresh-0.3.0.tar.gz` & `tmp/pythresh-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythresh-0.3.0.tar", last modified: Tue Mar 21 17:03:37 2023, max compression
+gzip compressed data, was "pythresh-0.3.1.tar", last modified: Wed May  3 17:06:44 2023, max compression
```

## Comparing `pythresh-0.3.0.tar` & `pythresh-0.3.1.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-03-21 17:03:37.785266 pythresh-0.3.0/
--rw-r--r--   0 denmark   (1000) denmark   (1000)     1317 2022-06-16 06:55:08.000000 pythresh-0.3.0/LICENSE
--rw-r--r--   0 denmark   (1000) denmark   (1000)      269 2023-03-20 18:17:50.000000 pythresh-0.3.0/MANIFEST.in
--rw-r--r--   0 denmark   (1000) denmark   (1000)    28555 2023-03-21 17:03:37.785266 pythresh-0.3.0/PKG-INFO
--rw-r--r--   0 denmark   (1000) denmark   (1000)    27460 2023-03-21 16:59:30.000000 pythresh-0.3.0/README.rst
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-03-21 17:03:37.758599 pythresh-0.3.0/pythresh/
--rw-r--r--   0 denmark   (1000) denmark   (1000)      114 2022-11-22 17:00:48.000000 pythresh-0.3.0/pythresh/__init__.py
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-03-21 17:03:37.761932 pythresh-0.3.0/pythresh/models/
--rw-r--r--   0 denmark   (1000) denmark   (1000)   141564 2022-11-06 09:53:23.000000 pythresh-0.3.0/pythresh/models/meta_model_GNB.pkl
--rw-r--r--   0 denmark   (1000) denmark   (1000)   141284 2022-12-31 13:15:02.000000 pythresh-0.3.0/pythresh/models/meta_model_GNBC.pkl
--rw-r--r--   0 denmark   (1000) denmark   (1000)   165531 2023-03-16 17:01:32.000000 pythresh-0.3.0/pythresh/models/meta_model_GNBM.pkl
--rw-r--r--   0 denmark   (1000) denmark   (1000)  3181480 2022-11-06 09:53:21.000000 pythresh-0.3.0/pythresh/models/meta_model_LIN.pkl
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-03-21 17:03:37.785266 pythresh-0.3.0/pythresh/thresholds/
--rw-r--r--   0 denmark   (1000) denmark   (1000)       24 2022-06-16 06:55:08.000000 pythresh-0.3.0/pythresh/thresholds/__init__.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     5535 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/all.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3320 2023-02-16 20:23:31.000000 pythresh-0.3.0/pythresh/thresholds/aucp.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     1088 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/base.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3382 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/boot.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3509 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/chau.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2922 2023-03-19 06:25:35.000000 pythresh-0.3.0/pythresh/thresholds/clf.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)    10113 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/clust.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4295 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/comb.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2789 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/cpd.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3583 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/decomp.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)    10502 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/dsn.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3427 2023-03-19 06:11:00.000000 pythresh-0.3.0/pythresh/thresholds/eb.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2513 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/fgd.py
--rwxr-xr-x   0 denmark   (1000) denmark   (1000)     4999 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/filter.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2327 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/fwfm.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4104 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/gesd.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     9319 2022-12-17 20:04:47.000000 pythresh-0.3.0/pythresh/thresholds/hist.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2332 2023-02-16 20:23:31.000000 pythresh-0.3.0/pythresh/thresholds/iqr.py
--rwxr-xr-x   0 denmark   (1000) denmark   (1000)     3516 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/karch.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2119 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/mad.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4942 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/mcst.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     5305 2023-03-20 18:55:49.000000 pythresh-0.3.0/pythresh/thresholds/meta.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4721 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/moll.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     5517 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/mtt.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     7197 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/ocsvm.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3940 2023-02-16 20:23:43.000000 pythresh-0.3.0/pythresh/thresholds/qmcd.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3491 2023-02-16 20:23:31.000000 pythresh-0.3.0/pythresh/thresholds/regr.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)      806 2022-11-22 16:06:32.000000 pythresh-0.3.0/pythresh/thresholds/thresh_utility.py
--rwxr-xr-x   0 denmark   (1000) denmark   (1000)    10072 2023-02-16 20:23:31.000000 pythresh-0.3.0/pythresh/thresholds/vae.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     4787 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/wind.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     3261 2023-02-16 20:23:30.000000 pythresh-0.3.0/pythresh/thresholds/yj.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2079 2022-11-24 16:57:56.000000 pythresh-0.3.0/pythresh/thresholds/zscore.py
--rw-r--r--   0 denmark   (1000) denmark   (1000)      172 2023-03-21 17:00:10.000000 pythresh-0.3.0/pythresh/version.py
-drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-03-21 17:03:37.758599 pythresh-0.3.0/pythresh.egg-info/
--rw-r--r--   0 denmark   (1000) denmark   (1000)    28555 2023-03-21 17:03:37.000000 pythresh-0.3.0/pythresh.egg-info/PKG-INFO
--rw-r--r--   0 denmark   (1000) denmark   (1000)     1342 2023-03-21 17:03:37.000000 pythresh-0.3.0/pythresh.egg-info/SOURCES.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)        1 2023-03-21 17:03:37.000000 pythresh-0.3.0/pythresh.egg-info/dependency_links.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)       79 2023-03-21 17:03:37.000000 pythresh-0.3.0/pythresh.egg-info/requires.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)        9 2023-03-21 17:03:37.000000 pythresh-0.3.0/pythresh.egg-info/top_level.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)       79 2022-12-21 18:33:59.000000 pythresh-0.3.0/requirements.txt
--rw-r--r--   0 denmark   (1000) denmark   (1000)       80 2023-03-21 17:03:37.785266 pythresh-0.3.0/setup.cfg
--rw-r--r--   0 denmark   (1000) denmark   (1000)     2236 2023-02-16 20:23:29.000000 pythresh-0.3.0/setup.py
+drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.131144 pythresh-0.3.1/
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     1317 2022-06-16 06:55:08.000000 pythresh-0.3.1/LICENSE
+-rw-r--r--   0 denmark   (1000) denmark   (1000)      269 2023-03-20 18:17:50.000000 pythresh-0.3.1/MANIFEST.in
+-rw-r--r--   0 denmark   (1000) denmark   (1000)    28480 2023-05-03 17:06:44.131144 pythresh-0.3.1/PKG-INFO
+-rw-r--r--   0 denmark   (1000) denmark   (1000)    27334 2023-05-03 17:00:01.000000 pythresh-0.3.1/README.rst
+drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.107810 pythresh-0.3.1/pythresh/
+-rw-r--r--   0 denmark   (1000) denmark   (1000)       89 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/__init__.py
+drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.111144 pythresh-0.3.1/pythresh/models/
+-rw-r--r--   0 denmark   (1000) denmark   (1000)   141564 2022-11-06 09:53:23.000000 pythresh-0.3.1/pythresh/models/meta_model_GNB.pkl
+-rw-r--r--   0 denmark   (1000) denmark   (1000)   141284 2022-12-31 13:15:02.000000 pythresh-0.3.1/pythresh/models/meta_model_GNBC.pkl
+-rw-r--r--   0 denmark   (1000) denmark   (1000)   165531 2023-03-16 17:01:32.000000 pythresh-0.3.1/pythresh/models/meta_model_GNBM.pkl
+-rw-r--r--   0 denmark   (1000) denmark   (1000)  3181480 2022-11-06 09:53:21.000000 pythresh-0.3.1/pythresh/models/meta_model_LIN.pkl
+drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.131144 pythresh-0.3.1/pythresh/thresholds/
+-rw-r--r--   0 denmark   (1000) denmark   (1000)        0 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/__init__.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     3320 2023-04-13 18:25:51.000000 pythresh-0.3.1/pythresh/thresholds/aucp.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     1008 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/base.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     3378 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/boot.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     3499 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/chau.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     2905 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/clf.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)    10087 2023-04-23 15:04:42.000000 pythresh-0.3.1/pythresh/thresholds/clust.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     4293 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/comb.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     2782 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/cpd.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     3996 2023-04-27 08:02:52.000000 pythresh-0.3.1/pythresh/thresholds/decomp.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)    10503 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/dsn.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     3427 2023-04-13 18:25:51.000000 pythresh-0.3.1/pythresh/thresholds/eb.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     2512 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/fgd.py
+-rwxr-xr-x   0 denmark   (1000) denmark   (1000)     4900 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/filter.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     2316 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/fwfm.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     4104 2023-04-13 18:25:50.000000 pythresh-0.3.1/pythresh/thresholds/gesd.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     9327 2023-04-15 13:25:28.000000 pythresh-0.3.1/pythresh/thresholds/hist.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     2323 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/iqr.py
+-rwxr-xr-x   0 denmark   (1000) denmark   (1000)     3516 2023-04-13 18:25:51.000000 pythresh-0.3.1/pythresh/thresholds/karch.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     2110 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/mad.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     4938 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/mcst.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     5266 2023-04-13 19:04:48.000000 pythresh-0.3.1/pythresh/thresholds/meta.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     4721 2023-04-13 18:25:51.000000 pythresh-0.3.1/pythresh/thresholds/moll.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     5518 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/mtt.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     7163 2023-04-15 13:29:48.000000 pythresh-0.3.1/pythresh/thresholds/ocsvm.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     3928 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/qmcd.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     3476 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/regr.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)      806 2023-04-13 17:36:34.000000 pythresh-0.3.1/pythresh/thresholds/thresh_utility.py
+-rwxr-xr-x   0 denmark   (1000) denmark   (1000)    10067 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/vae.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     4774 2023-04-13 19:25:40.000000 pythresh-0.3.1/pythresh/thresholds/wind.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     3253 2023-04-13 19:04:50.000000 pythresh-0.3.1/pythresh/thresholds/yj.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     2067 2023-05-02 19:25:21.000000 pythresh-0.3.1/pythresh/thresholds/zscore.py
+-rw-r--r--   0 denmark   (1000) denmark   (1000)      171 2023-05-03 16:02:26.000000 pythresh-0.3.1/pythresh/version.py
+drwxr-xr-x   0 denmark   (1000) denmark   (1000)        0 2023-05-03 17:06:44.111144 pythresh-0.3.1/pythresh.egg-info/
+-rw-r--r--   0 denmark   (1000) denmark   (1000)    28480 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/PKG-INFO
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     1315 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/SOURCES.txt
+-rw-r--r--   0 denmark   (1000) denmark   (1000)        1 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/dependency_links.txt
+-rw-r--r--   0 denmark   (1000) denmark   (1000)       66 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/requires.txt
+-rw-r--r--   0 denmark   (1000) denmark   (1000)        9 2023-05-03 17:06:43.000000 pythresh-0.3.1/pythresh.egg-info/top_level.txt
+-rw-r--r--   0 denmark   (1000) denmark   (1000)       66 2023-05-02 18:44:48.000000 pythresh-0.3.1/requirements.txt
+-rw-r--r--   0 denmark   (1000) denmark   (1000)       80 2023-05-03 17:06:44.131144 pythresh-0.3.1/setup.cfg
+-rw-r--r--   0 denmark   (1000) denmark   (1000)     2266 2023-05-02 17:41:56.000000 pythresh-0.3.1/setup.py
```

### Comparing `pythresh-0.3.0/LICENSE` & `pythresh-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/PKG-INFO` & `pythresh-0.3.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,22 @@
-Metadata-Version: 2.1
-Name: pythresh
-Version: 0.3.0
-Summary: A Python Toolbox for Outlier Detection Thresholding
-Home-page: https://github.com/KulikDM/pythresh
-Author: D Kulik
-License: UNKNOWN
-Download-URL: https://github.com/KulikDM/pythresh/archive/master.zip
-Project-URL: Documentation, https://pythresh.readthedocs.io/en/latest/
-Keywords: outlier detection,anomaly detection,thresholding,cutoff,contamintion level,data science,machine learning
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ##################################################
  Python Outlier Detection Thresholding (PyThresh)
 ##################################################
 
 **Deployment, Stats, & License**
 
 .. image:: https://img.shields.io/pypi/v/pythresh.svg?color=brightgreen&logo=pypi&logoColor=white
    :target: https://pypi.org/project/pythresh/
    :alt: PyPI version
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/pythresh?color=brightgreen&logo=conda-forge&logoColor=white
    :target: https://anaconda.org/conda-forge/pythresh
    :alt: Anaconda version
 
-.. image:: https://readthedocs.org/projects/pythresh/badge/?version=latest
+.. image:: https://img.shields.io/readthedocs/pythresh.svg?version=latest&logo=read-the-docs&logoColor=white
    :target: http://pythresh.readthedocs.io/?badge=latest
    :alt: Documentation status
 
 .. image:: https://github.com/KulikDM/pythresh/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/KulikDM/pythresh/actions/workflows/python-package.yml
    :alt: testing
 
@@ -61,14 +36,18 @@
    :target: https://pypi.org/project/pythresh/
    :alt: Python versions
 
 .. image:: https://img.shields.io/github/license/KulikDM/pythresh.svg
    :target: https://github.com/KulikDM/pythresh/blob/master/LICENSE
    :alt: License
 
+.. image:: https://zenodo.org/badge/497683169.svg
+   :target: https://zenodo.org/badge/latestdoi/497683169
+   :alt: Zenodo DOI
+
 ----
 
 PyThresh is a comprehensive and scalable **Python toolkit** for
 **thresholding outlier detection scores** in univariate/multivariate
 data. It has been writen to work in tandem with PyOD and has similar
 syntax and data structures. However, it is not limited to this single
 library. PyThresh is meant to threshold scores generated by an outlier
@@ -82,20 +61,25 @@
 All threshold functions return a binary array where inliers and outliers
 are represented by a 0 and 1 respectively.
 
 PyThresh includes more than 30 thresholding algorithms. These algorithms
 range from using simple statistical analysis like the Z-score to more
 complex mathematical methods that involve graph theory and topology.
 
-***************
- Documentation
-***************
+************************
+ Documentation & Citing
+************************
+
+Visit `PyThresh Docs
+<https://pythresh.readthedocs.io/en/latest/?badge=latest>`_ for full
+documentation or see below for a quickstart installation and usage
+example.
 
-Visit `PyThresh Docs <https://pythresh.readthedocs.io/en/latest/?badge=latest>`_
-for full documentation or see below for a quickstart installation and usage example
+To cite this work you can visit `PyThresh Citation
+<https://zenodo.org/badge/latestdoi/497683169>`_
 
 ----
 
 **Outlier Detection Thresholding with 7 Lines of Code**:
 
 .. code:: python
 
@@ -143,22 +127,22 @@
 
    pip install https://github.com/KulikDM/pythresh/archive/main.zip
 
 **Required Dependencies**:
 
 -  matplotlib
 -  numpy>=1.13
--  pyclustering
 -  pyod
 -  scipy>=1.3.1
 -  scikit_learn>=0.20.0
 -  six
 
 **Optional Dependencies**:
 
+-  pyclustering (used in the CLUST thresholder)
 -  ruptures (used in the CPD thresholder)
 -  geomstats (used in the KARCH thresholder)
 -  scikit-lego (used in the META thresholder)
 -  joblib>=0.14.1 (used in the META thresholder)
 -  pandas (used in the META thresholder)
 -  torch (used in the VAE thresholder)
 -  tqdm (used in the VAE thresholder)
@@ -255,32 +239,31 @@
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | WIND      | Topological Winding Number                | [#wind1]_          | `pythresh.thresholds.wind module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.wind>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | YJ        | Yeo-Johnson Transformation                | [#yj1]_            | `pythresh.thresholds.yj module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.yj>`_                    |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | ZSCORE    | Z-score                                   | [#zscore1]_        | `pythresh.thresholds.zscore module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.zscore>`_            |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
-| ALL       | All Thresholders Combined                 | None               | `pythresh.thresholds.all module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.all>`_                  |
-+-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | COMB      | Thresholder Combination                   | None               | `pythresh.thresholds.comb module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.comb>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 
 ******************************
  Implementations & Benchmarks
 ******************************
 
 **The comparison among implemented models and general implementation**
 is made available below
 
-Additional `benchmarking <https://pythresh.readthedocs.io/en/latest/benchmark.html>`_ 
-has been done on all the thresholders and it was
-found that the ``META`` thresholder performed best while the ``CLF`` 
-thresholder provided the smallest uncertainty about its mean and is the 
-most robust (best least accurate prediction). However, for interpretability 
-and general performance the ``FILTER`` thresholder is a good fit.
+Additional `benchmarking
+<https://pythresh.readthedocs.io/en/latest/benchmark.html>`_ has been
+done on all the thresholders and it was found that the ``META``
+thresholder performed best while the ``CLF`` thresholder provided the
+smallest uncertainty about its mean and is the most robust (best least
+accurate prediction). However, for interpretability and general
+performance the ``FILTER`` thresholder is a good fit.
 
 ----
 
 For Jupyter Notebooks, please navigate to `notebooks
 <https://github.com/KulikDM/pythresh/tree/main/notebooks>`_.
 
 A quick look at all the thresholders performance can be found at
@@ -288,40 +271,43 @@
 
 .. image:: https://raw.githubusercontent.com/KulikDM/pythresh/main/imgs/All.png
    :target: https://raw.githubusercontent.com/KulikDM/pythresh/main/imgs/All.png
    :alt: Comparision_of_All
 
 ----
 
-
 **************
  Contributing
 **************
 
 Anyone is welcome to contribute to PyThresh:
 
-* Please share your ideas and ask questions by opening an issue.
+-  Please share your ideas and ask questions by opening an issue.
 
-* To contribute, first check the Issue list for the "help wanted" tag and comment 
-  on the one that you are interested in. The issue will then be assigned to you.
+-  To contribute, first check the Issue list for the "help wanted" tag
+   and comment on the one that you are interested in. The issue will
+   then be assigned to you.
 
-* If the bug, feature, or documentation change is novel (not in the Issue list),
-  you can either log a new issue or create a pull request for the new changes.
+-  If the bug, feature, or documentation change is novel (not in the
+   Issue list), you can either log a new issue or create a pull request
+   for the new changes.
 
-* To start, fork the main branch and add your improvement/modification/fix.
+-  To start, fork the main branch and add your
+   improvement/modification/fix.
 
-* To make sure the code has the same style and standard, please refer to qmcd.py for 
-  example.
+-  To make sure the code has the same style and standard, please refer
+   to qmcd.py for example.
 
-* Create a pull request to the **main branch** and follow the pull request template 
-  `PR template <https://github.com/KulikDM/pythresh/blob/main/.github/PULL_REQUEST_TEMPLATE.md>`_
+-  Create a pull request to the **main branch** and follow the pull
+   request template `PR template
+   <https://github.com/KulikDM/pythresh/blob/main/.github/PULL_REQUEST_TEMPLATE.md>`_
 
-* Please make sure that all code changes are accompanied with proper new/updated test 
-  functions. Automatic tests will be triggered. Before the pull request can be merged, 
-  make sure that all the tests pass.
+-  Please make sure that all code changes are accompanied with proper
+   new/updated test functions. Automatic tests will be triggered. Before
+   the pull request can be merged, make sure that all the tests pass.
 
 ----
 
 ************
  References
 ************
 
@@ -477,9 +463,7 @@
    `Transforming variables to central normality
    <https://arxiv.org/abs/2005.07946>`_
 
 .. [#zscore1]
 
    `Multiple outlier detection tests for parametric models
    <https://arxiv.org/abs/1910.10426>`_
-
-
```

### Comparing `pythresh-0.3.0/README.rst` & `pythresh-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,48 @@
+Metadata-Version: 2.1
+Name: pythresh
+Version: 0.3.1
+Summary: A Python Toolbox for Outlier Detection Thresholding
+Home-page: https://github.com/KulikDM/pythresh
+Author: D Kulik
+License: UNKNOWN
+Download-URL: https://github.com/KulikDM/pythresh/archive/master.zip
+Project-URL: Documentation, https://pythresh.readthedocs.io/en/latest/
+Keywords: outlier detection,anomaly detection,thresholding,cutoff,contamintion level,data science,machine learning
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ##################################################
  Python Outlier Detection Thresholding (PyThresh)
 ##################################################
 
 **Deployment, Stats, & License**
 
 .. image:: https://img.shields.io/pypi/v/pythresh.svg?color=brightgreen&logo=pypi&logoColor=white
    :target: https://pypi.org/project/pythresh/
    :alt: PyPI version
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/pythresh?color=brightgreen&logo=conda-forge&logoColor=white
    :target: https://anaconda.org/conda-forge/pythresh
    :alt: Anaconda version
 
-.. image:: https://readthedocs.org/projects/pythresh/badge/?version=latest
+.. image:: https://img.shields.io/readthedocs/pythresh.svg?version=latest&logo=read-the-docs&logoColor=white
    :target: http://pythresh.readthedocs.io/?badge=latest
    :alt: Documentation status
 
 .. image:: https://github.com/KulikDM/pythresh/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/KulikDM/pythresh/actions/workflows/python-package.yml
    :alt: testing
 
@@ -36,14 +62,18 @@
    :target: https://pypi.org/project/pythresh/
    :alt: Python versions
 
 .. image:: https://img.shields.io/github/license/KulikDM/pythresh.svg
    :target: https://github.com/KulikDM/pythresh/blob/master/LICENSE
    :alt: License
 
+.. image:: https://zenodo.org/badge/497683169.svg
+   :target: https://zenodo.org/badge/latestdoi/497683169
+   :alt: Zenodo DOI
+
 ----
 
 PyThresh is a comprehensive and scalable **Python toolkit** for
 **thresholding outlier detection scores** in univariate/multivariate
 data. It has been writen to work in tandem with PyOD and has similar
 syntax and data structures. However, it is not limited to this single
 library. PyThresh is meant to threshold scores generated by an outlier
@@ -57,20 +87,25 @@
 All threshold functions return a binary array where inliers and outliers
 are represented by a 0 and 1 respectively.
 
 PyThresh includes more than 30 thresholding algorithms. These algorithms
 range from using simple statistical analysis like the Z-score to more
 complex mathematical methods that involve graph theory and topology.
 
-***************
- Documentation
-***************
+************************
+ Documentation & Citing
+************************
+
+Visit `PyThresh Docs
+<https://pythresh.readthedocs.io/en/latest/?badge=latest>`_ for full
+documentation or see below for a quickstart installation and usage
+example.
 
-Visit `PyThresh Docs <https://pythresh.readthedocs.io/en/latest/?badge=latest>`_
-for full documentation or see below for a quickstart installation and usage example
+To cite this work you can visit `PyThresh Citation
+<https://zenodo.org/badge/latestdoi/497683169>`_
 
 ----
 
 **Outlier Detection Thresholding with 7 Lines of Code**:
 
 .. code:: python
 
@@ -118,22 +153,22 @@
 
    pip install https://github.com/KulikDM/pythresh/archive/main.zip
 
 **Required Dependencies**:
 
 -  matplotlib
 -  numpy>=1.13
--  pyclustering
 -  pyod
 -  scipy>=1.3.1
 -  scikit_learn>=0.20.0
 -  six
 
 **Optional Dependencies**:
 
+-  pyclustering (used in the CLUST thresholder)
 -  ruptures (used in the CPD thresholder)
 -  geomstats (used in the KARCH thresholder)
 -  scikit-lego (used in the META thresholder)
 -  joblib>=0.14.1 (used in the META thresholder)
 -  pandas (used in the META thresholder)
 -  torch (used in the VAE thresholder)
 -  tqdm (used in the VAE thresholder)
@@ -230,32 +265,31 @@
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | WIND      | Topological Winding Number                | [#wind1]_          | `pythresh.thresholds.wind module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.wind>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | YJ        | Yeo-Johnson Transformation                | [#yj1]_            | `pythresh.thresholds.yj module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.yj>`_                    |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | ZSCORE    | Z-score                                   | [#zscore1]_        | `pythresh.thresholds.zscore module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.zscore>`_            |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
-| ALL       | All Thresholders Combined                 | None               | `pythresh.thresholds.all module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.all>`_                  |
-+-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | COMB      | Thresholder Combination                   | None               | `pythresh.thresholds.comb module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.comb>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 
 ******************************
  Implementations & Benchmarks
 ******************************
 
 **The comparison among implemented models and general implementation**
 is made available below
 
-Additional `benchmarking <https://pythresh.readthedocs.io/en/latest/benchmark.html>`_ 
-has been done on all the thresholders and it was
-found that the ``META`` thresholder performed best while the ``CLF`` 
-thresholder provided the smallest uncertainty about its mean and is the 
-most robust (best least accurate prediction). However, for interpretability 
-and general performance the ``FILTER`` thresholder is a good fit.
+Additional `benchmarking
+<https://pythresh.readthedocs.io/en/latest/benchmark.html>`_ has been
+done on all the thresholders and it was found that the ``META``
+thresholder performed best while the ``CLF`` thresholder provided the
+smallest uncertainty about its mean and is the most robust (best least
+accurate prediction). However, for interpretability and general
+performance the ``FILTER`` thresholder is a good fit.
 
 ----
 
 For Jupyter Notebooks, please navigate to `notebooks
 <https://github.com/KulikDM/pythresh/tree/main/notebooks>`_.
 
 A quick look at all the thresholders performance can be found at
@@ -263,40 +297,43 @@
 
 .. image:: https://raw.githubusercontent.com/KulikDM/pythresh/main/imgs/All.png
    :target: https://raw.githubusercontent.com/KulikDM/pythresh/main/imgs/All.png
    :alt: Comparision_of_All
 
 ----
 
-
 **************
  Contributing
 **************
 
 Anyone is welcome to contribute to PyThresh:
 
-* Please share your ideas and ask questions by opening an issue.
+-  Please share your ideas and ask questions by opening an issue.
 
-* To contribute, first check the Issue list for the "help wanted" tag and comment 
-  on the one that you are interested in. The issue will then be assigned to you.
+-  To contribute, first check the Issue list for the "help wanted" tag
+   and comment on the one that you are interested in. The issue will
+   then be assigned to you.
 
-* If the bug, feature, or documentation change is novel (not in the Issue list),
-  you can either log a new issue or create a pull request for the new changes.
+-  If the bug, feature, or documentation change is novel (not in the
+   Issue list), you can either log a new issue or create a pull request
+   for the new changes.
 
-* To start, fork the main branch and add your improvement/modification/fix.
+-  To start, fork the main branch and add your
+   improvement/modification/fix.
 
-* To make sure the code has the same style and standard, please refer to qmcd.py for 
-  example.
+-  To make sure the code has the same style and standard, please refer
+   to qmcd.py for example.
 
-* Create a pull request to the **main branch** and follow the pull request template 
-  `PR template <https://github.com/KulikDM/pythresh/blob/main/.github/PULL_REQUEST_TEMPLATE.md>`_
+-  Create a pull request to the **main branch** and follow the pull
+   request template `PR template
+   <https://github.com/KulikDM/pythresh/blob/main/.github/PULL_REQUEST_TEMPLATE.md>`_
 
-* Please make sure that all code changes are accompanied with proper new/updated test 
-  functions. Automatic tests will be triggered. Before the pull request can be merged, 
-  make sure that all the tests pass.
+-  Please make sure that all code changes are accompanied with proper
+   new/updated test functions. Automatic tests will be triggered. Before
+   the pull request can be merged, make sure that all the tests pass.
 
 ----
 
 ************
  References
 ************
 
@@ -452,7 +489,9 @@
    `Transforming variables to central normality
    <https://arxiv.org/abs/2005.07946>`_
 
 .. [#zscore1]
 
    `Multiple outlier detection tests for parametric models
    <https://arxiv.org/abs/1910.10426>`_
+
+
```

### Comparing `pythresh-0.3.0/pythresh/models/meta_model_GNB.pkl` & `pythresh-0.3.1/pythresh/models/meta_model_GNB.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/models/meta_model_GNBC.pkl` & `pythresh-0.3.1/pythresh/models/meta_model_GNBC.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/models/meta_model_GNBM.pkl` & `pythresh-0.3.1/pythresh/models/meta_model_GNBM.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/models/meta_model_LIN.pkl` & `pythresh-0.3.1/pythresh/models/meta_model_LIN.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/thresholds/all.py` & `pythresh-0.3.1/pythresh/thresholds/mcst.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,95 @@
-import warnings
-
 import numpy as np
 import scipy.stats as stats
 from sklearn.utils import check_array
 
-from .aucp import AUCP
 from .base import BaseThresholder
-from .boot import BOOT
-from .chau import CHAU
-from .clf import CLF
-from .clust import CLUST
-from .decomp import DECOMP
-from .dsn import DSN
-from .eb import EB
-from .fgd import FGD
-from .filter import FILTER
-from .fwfm import FWFM
-from .gesd import GESD
-from .hist import HIST
-from .iqr import IQR
-from .mad import MAD
-from .mcst import MCST
-from .moll import MOLL
-from .mtt import MTT
-from .ocsvm import OCSVM
-from .qmcd import QMCD
-from .regr import REGR
 from .thresh_utility import cut, normalize
-from .wind import WIND
-from .yj import YJ
-from .zscore import ZSCORE
 
 
-class ALL(BaseThresholder):
-    """ALL class for Combined thresholder.
-
-       Use the multiple thresholders as a non-parametric means
-       to threshold scores generated by the decision_scores where outliers
-       are set to any value beyond the (mean, median, or mode) of the
-       contamination from all the combined thresholders.
+class MCST(BaseThresholder):
+    r"""MCST class for Monte Carlo Shapiro Tests thresholder.
+
+       Use uniform random sampling and statistical testing to evaluate a
+       non-parametric means to threshold scores generated by the decision_scores
+       where outliers are set to any value beyond the minimum value left after
+       iterative Shapiro-Wilk tests have occurred. Note** accuracy decreases with
+       array size. For good results the should be array<1000. However still this
+       threshold method may fail at any array size.
+       See :cite:`coin2008mcst` for details.
 
        Parameters
        ----------
 
-       thresholders : list, optional (default='all')
-            List of instantiated thresholders, e.g. [DSN()]
-
-       max_contam : float, optional (default=0.5)
-            Maximum contamination allowed for each threshold output. Thresholded scores
-            above the maximum contamination will not be included in the final combined
-            threshold
-
-       method : {'mean', 'median', 'mode'}, optional (default='mean')
-           statistic to apply to contamination levels
-
-           - 'mean':   calculate the mean combined threshold
-           - 'median': calculate the median combined threshold
-           - 'mode':  calculate the majority vote or mode of the thresholded labels
-
        random_state : int, optional (default=1234)
-            Random seed for the random number generators of the thresholders. Can also
-            be set to None.
-
+            Random seed for the uniform distribution. Can also be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
-       confidence_interval_ : lower and upper confidence interval of the contamination level
+       Notes
+       -----
 
-    """
+       The Shapiro-Wilk test is a frequentist statistical test for normality.
+       It is used to test the null-hypothesis that the decision scores came
+       from a normal distribution. This test statistic is defined as:
+
+       .. math::
+
+          W = \frac{\left(\sum_{i=1}^n a_i x_{(i)} \right)^2}{\sum_{i=1}^n \left(x_i - \bar{x} \right)^2} \mathrm{,}
+
+       where :math:`\bar{x}` is the mean of the scores and :math:`x_{(i)}`
+       is the ith-smallest number in the sample (kth order statistic). The
+       coefficients :math:`a_i` is given by:
+
+       .. math::
+
+          (a_1,...,a_n) = \frac{m^{\top}V^{-1}}{\sqrt{m^{\top}V^{-1}V^{-1}m}} \mathrm{,}
+
+       where the vector :math:`m=\lvert(m_1,...,m_n \rvert)^{\top}` and :math:`V`
+       is the covariance matrix of the order statistics.
+
+       The threshold is set by first calculating an initial Shapiro-Wilk test
+       p-value on the decision scores. Using Monte Carlo simulations, random values
+       between 0-1 are inserted into the normalized decision scores and p-values are
+       calculated. if the p-value is higher than the initial p-value, the initial p-value
+       is set to this value and the random value is stored. The minimum stored random
+       value is set as the threshold as it is the minimum found outlier.
+
+       Examples
+       --------
+       The effects of randomness can affect the thresholder's output perfomance
+       signicantly. Therefore, to alleviate the effects of randomness on the
+       thresholder a combined model can be used with different random_state values.
+       E.g.
 
-    def __init__(self, thresholders='all', max_contam=0.5, method='mean', random_state=1234):
+       .. code:: python
 
-        warnings.warn('''The ALL thresholder will be depreciated by version 0.3.1.
-                      Use the COMB thresholder instead''',
-                      category=DeprecationWarning, stacklevel=2)
-
-        self.thresholders = thresholders
-        self.max_contam = max_contam
-        stat = {'mean': np.mean, 'median': np.median, 'mode': stats.mode}
-        self.method = method
-        self.method_func = stat[method]
+            # train the KNN detector
+            from pyod.models.knn import KNN
+            from pythresh.thresholds.comb import COMB
+            from pythresh.thresholds.mcst import MCST
+
+            clf = KNN()
+            clf.fit(X_train)
+
+            # get outlier scores
+            decision_scores = clf.decision_scores_  # raw outlier scores
+
+            # get outlier labels with combined model
+            thres = COMB(thresholders = [MCST(random_state=1234),
+            MCST(random_state=42), MCST(random_state=9685),
+            MCST(random_state=111222)])
+            labels = thres.eval(decision_scores)
+
+    """
+
+    def __init__(self, random_state=1234):
         self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
@@ -100,64 +103,36 @@
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
         decision = check_array(decision, ensure_2d=False)
 
-        decision = np.sort(normalize(decision))
-
-        # Initialize thresholders
-        if self.thresholders == 'all':
-            self.thresholders = [IQR(), MAD(), FWFM(), YJ(), ZSCORE(), AUCP(), QMCD(),
-                                 FGD(), DSN(random_state=self.random_state), CLF(),
-                                 FILTER(), WIND(random_state=self.random_state), EB(),
-                                 REGR(random_state=self.random_state),
-                                 BOOT(random_state=self.random_state),
-                                 MCST(random_state=self.random_state), HIST(),
-                                 MOLL(), CHAU(), GESD(), MTT(),
-                                 OCSVM(random_state=self.random_state),
-                                 CLUST(random_state=self.random_state),
-                                 DECOMP(random_state=self.random_state)]
-
-        # Apply each thresholder
-        contam = []
-        ratio = []
-        counts = len(decision)
-
-        for thresholder in self.thresholders:
-
-            labels = thresholder.eval(decision)
-            outlier_ratio = np.sum(labels)/counts
-
-            if outlier_ratio < self.max_contam:
-
-                contam.append(labels)
-                ratio.append(outlier_ratio)
-
-        contam = np.array(contam)
-        ratio = np.array(ratio)
+        decision = normalize(decision)
 
-        # Get lower and upper confidence interval
-        low, high = stats.bootstrap(ratio.reshape(1, -1),
-                                    np.mean, paired=True,
-                                    random_state=self.random_state).confidence_interval
-        self.confidence_interval_ = [low, high]
+        # Get Baseline Shapiro-Wilk test p-value
+        p_std = stats.shapiro(decision).pvalue
 
-        # Get [mean, median, or mode] of inliers
-        if self.method == 'mode':
+        # Create random dataset to insert and test p-values
+        rnd = stats.uniform.rvs(loc=0, scale=1, size=len(
+            decision), random_state=self.random_state)
+        rnd = normalize(rnd)
+        povr = []
 
-            self.thresh_ = None
-            lbls = self.method_func(contam, axis=0)
+        # Iterate and add a new random variable
+        # Perform a Shapiro-Wilk test and see if the new
+        # distribution has a lower or higher p-value
+        # If higher record these potential outlier values
+        for i in range(len(rnd)):
 
-            return np.squeeze(lbls[0])
+            arr = np.append(decision, rnd[i])
+            p_check = stats.shapiro(arr).pvalue
 
-        else:
+            if p_check > p_std:
 
-            contam = np.sum(contam, axis=1)/contam.shape[1]
-            inlier_ratio = 1-self.method_func(contam)
+                p_std = p_check
+                povr.append(rnd[i])
 
-            idx = int(counts*inlier_ratio)
-            limit = decision[idx] if idx < counts else 1.0
-            self.thresh_ = limit
+        limit = np.min(povr) if povr else 1.1
+        self.thresh_ = limit
 
-            return cut(decision, limit)
+        return cut(decision, limit)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/aucp.py` & `pythresh-0.3.1/pythresh/thresholds/aucp.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/thresholds/base.py` & `pythresh-0.3.1/pythresh/thresholds/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-from __future__ import division, print_function
-
 import abc
 
-import six
-
 
-@six.add_metaclass(abc.ABCMeta)
-class BaseThresholder(object):
+class BaseThresholder(metaclass=abc.ABCMeta):
     """Abstract class for all outlier detection thresholding algorithms.
 
-
        Parameters
        ----------
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
-
     """
 
     @abc.abstractmethod
     def __init__(self):
 
         self.thresh_ = None
         self.confidence_interval_ = None
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/boot.py` & `pythresh-0.3.1/pythresh/thresholds/boot.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
        The returned upper and lower confidence intervals are used to threshold
        the decision scores. Outliers are set to any value above the mean of the
        upper and lower confidence intervals.
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance 
-       signicantly. Therefore, to alleviate the effects of randomness on the 
+       The effects of randomness can affect the thresholder's output perfomance
+       signicantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -54,16 +54,16 @@
             clf = KNN()
             clf.fit(X_train)
 
             # get outlier scores
             decision_scores = clf.decision_scores_  # raw outlier scores
 
             # get outlier labels with combined model
-            thres = COMB(thresholders = [BOOT(random_state=1234), 
-            BOOT(random_state=42), BOOT(random_state=9685), 
+            thres = COMB(thresholders = [BOOT(random_state=1234),
+            BOOT(random_state=42), BOOT(random_state=9685),
             BOOT(random_state=111222)])
             labels = thres.eval(decision_scores)
 
     """
 
     def __init__(self, random_state=1234):
         self.random_state = random_state
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/chau.py` & `pythresh-0.3.1/pythresh/thresholds/chau.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
        Any z-score greater than the Chauvenet's criterion is considered an outlier.
 
 
     """
 
     def __init__(self, method='mean'):
 
-        super(CHAU, self).__init__()
+        super().__init__()
         stat = {'mean': np.mean, 'median': np.median, 'gmean': stats.gmean}
         self.method = stat[method]
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/clf.py` & `pythresh-0.3.1/pythresh/thresholds/clf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
        Parameters
        ----------
 
        method : {'simple', 'complex'}, optional (default='complex')
             Type of linear model
 
-            - 'simple':  Uses only the scores 
+            - 'simple':  Uses only the scores
             - 'complex': Uses the scores, log of the scores, and the scores' PDF
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
@@ -37,17 +37,17 @@
        and the contaminations and random states were randomized each iterative step.
 
 
     """
 
     def __init__(self, method='complex'):
 
-        if method=='complex':
+        if method == 'complex':
 
-            self.m1 = 7.115947536708103  
+            self.m1 = 7.115947536708103
             self.m2 = -5.934885742167458
             self.m3 = -3.416078337348704
             self.c = 2.5731351150980992
 
         else:
 
             self.m = 4.0581548062264075
@@ -74,23 +74,23 @@
 
         decision = check_array(decision, ensure_2d=False)
 
         decision = normalize(decision)
 
         # Calculate expected y
         if self.method == 'complex':
-            
+
             kde = gaussian_kde(decision)
             pdf = normalize(kde.pdf(decision))
             pdf = normalize(pdf**(1/10))
             log = normalize(np.log(decision + 1))
 
             pred = self.m1*decision + self.m2*log + self.m3*pdf + self.c
 
-        else:    
+        else:
             pred = self.m*decision + self.c
 
         # Determine labels
         pred[pred > 0] = 1
         pred[pred <= 0] = 0
 
         self.thresh_ = None
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/clust.py` & `pythresh-0.3.1/pythresh/thresholds/clust.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,16 +59,16 @@
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance 
-       signicantly. Therefore, to alleviate the effects of randomness on the 
+       The effects of randomness can affect the thresholder's output perfomance
+       signicantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -78,25 +78,24 @@
             clf = KNN()
             clf.fit(X_train)
 
             # get outlier scores
             decision_scores = clf.decision_scores_  # raw outlier scores
 
             # get outlier labels with combined model
-            thres = COMB(thresholders = [CLUST(method='bgm', random_state=1234), 
-            CLUST(method='bgm', random_state=42), 
-            CLUST(method='bgm', random_state=9685), 
+            thres = COMB(thresholders = [CLUST(method='bgm', random_state=1234),
+            CLUST(method='bgm', random_state=42),
+            CLUST(method='bgm', random_state=9685),
             CLUST(method='bgm', random_state=111222)])
             labels = thres.eval(decision_scores)
-
     """
 
     def __init__(self, method='spec', random_state=1234):
 
-        super(CLUST, self).__init__()
+        super().__init__()
         self.method = method
         self.method_funcs = {'agg': self._AGG_clust, 'birch': self._BIRCH_clust,
                              'bang': self._BANG_clust, 'bgm': self._BGM_clust,
                              'bsas': self._BSAS_clust, 'dbscan': self._DBSCAN_clust,
                              'ema': self._EMA_clust, 'kmeans': self._KMEANS_clust,
                              'mbsas': self._MBSAS_clust, 'mshift': self._MSHIFT_clust,
                              'optics': self._OPTICS_clust, 'somsc': self._SOMSC_clust,
@@ -127,131 +126,132 @@
         labels = self.method_funcs[str(self.method)](decision)
 
         self.thresh_ = None
 
         return labels
 
     def _pyclust_eval(self, cl, decision):
-        """ Evaluate cluster labels from pyclustering methods """
+        """Evaluate cluster labels from pyclustering methods."""
 
         cl.process()
 
         pred = np.squeeze(np.array(cl.get_clusters(), dtype=object))
 
-        if type(pred[0]) == list:
-            pred = np.array(pred[0])
+        pred = np.array(pred[0]) if type(pred[0]) == list else pred
 
         labels = np.ones(len(decision))
         labels[pred.astype(int)] = 0
 
         # Flip if outliers were clustered
-        if sum(labels) > np.ceil(len(decision)/2):
-            labels = 1-labels
+        labels = 1-labels if sum(labels) > np.ceil(len(decision)/2) else labels
 
         return labels
 
     def _sklearn_eval(self, cl, decision):
-        """ Evaluate cluster labels from sklearn methods """
+        """Evaluate cluster labels from sklearn methods."""
 
         cl.fit(decision)
         labels = cl.labels_
 
         # Flip if outliers were clustered
-        if sum(labels) > np.ceil(len(decision)/2):
-            labels = 1-labels
+        labels = 1-labels if sum(labels) > np.ceil(len(decision)/2) else labels
 
         return labels
 
     def _AGG_clust(self, decision):
-        """ Agglomerative algorithm for cluster analysis """
+        """Agglomerative algorithm for cluster analysis."""
 
         cl = agglomerative(data=decision, number_clusters=2,
                            link=2, ccore=True)
 
         return self._pyclust_eval(cl, decision)
 
     def _BIRCH_clust(self, decision):
-        """ BIRCH (Balanced Iterative Reducing and Clustering using
+        """BIRCH (Balanced Iterative Reducing and Clustering using.
+
             Hierarchies) algorithm for cluster analysis
         """
 
         cl = Birch(n_clusters=2, threshold=np.std(decision)/np.sqrt(2))
 
         return self._sklearn_eval(cl, decision)
 
     def _BANG_clust(self, decision):
-        """ BANG clustering algorithm for cluster analysis """
+        """BANG clustering algorithm for cluster analysis."""
 
         cl = bang(data=decision, levels=8, ccore=True)
 
         return self._pyclust_eval(cl, decision)
 
     def _BGM_clust(self, decision):
-        """ Bayesian Gaussian Mixture algorithm for cluster analysis """
+        """Bayesian Gaussian Mixture algorithm for cluster analysis."""
 
         cl = BayesianGaussianMixture(n_components=2,
                                      covariance_type='tied',
                                      random_state=self.random_state).fit(decision)
 
         labels = cl.predict(decision)
 
         # Flip if outliers were clustered
-        if sum(labels) > np.ceil(len(decision)/2):
-            labels = 1-labels
+        labels = 1-labels if sum(labels) > np.ceil(len(decision)/2) else labels
 
         return labels
 
     def _BSAS_clust(self, decision):
-        """ BSAS (Basic Sequential Algorithmic Scheme)
+        """BSAS (Basic Sequential Algorithmic Scheme).
+
             algorithm for cluster analysis
         """
 
         cl = bsas(data=decision, maximum_clusters=2,
                   threshold=np.std(decision), ccore=True)
 
         return self._pyclust_eval(cl, decision)
 
     def _DBSCAN_clust(self, decision):
-        """ DBSCAN (Density-based spatial clustering of applications with
+        """DBSCAN (Density-based spatial clustering of applications with.
+
             noise) algorithm for cluster analysis
         """
 
         cl = dbscan(data=decision, eps=np.std(decision) /
                     np.sqrt(2), neighbors=len(decision) // 2, ccore=True)
 
         return self._pyclust_eval(cl, decision)
 
     def _EMA_clust(self, decision):
-        """ Expectation-Maximization clustering algorithm for Gaussian
+        """Expectation-Maximization clustering algorithm for Gaussian.
+
             Mixture Models
         """
 
         cl = ema(data=decision, amount_clusters=2)
 
         return self._pyclust_eval(cl, decision)
 
     def _KMEANS_clust(self, decision):
-        """ K-means algorithm for cluster analysis """
+        """K-means algorithm for cluster analysis."""
 
         cl = KMeans(n_clusters=2)
 
         return self._sklearn_eval(cl, decision)
 
     def _MBSAS_clust(self, decision):
-        """ MBSAS (Modified Basic Sequential Algorithmic Scheme)
+        """MBSAS (Modified Basic Sequential Algorithmic Scheme).
+
             algorithm for cluster analysis
         """
 
         cl = mbsas(data=decision, maximum_clusters=2,
                    threshold=np.std(decision), ccore=True)
 
         return self._pyclust_eval(cl, decision)
 
     def _MSHIFT_clust(self, decision):
-        """ Mean shift algorithm for cluster analysis"""
+        """Mean shift algorithm for cluster analysis."""
 
         # Get quantile value for bandwidth estimation
         dat = np.squeeze(decision)
         q = cityblock(dat, np.sort(dat))/np.sum(dat)
 
         q = max(0.25, min(q, 1.0))
 
@@ -265,36 +265,37 @@
         mode = np.bincount(lbls).argmax()
         labels = np.ones(len(lbls))
         labels[lbls == mode] = 0
 
         return labels
 
     def _OPTICS_clust(self, decision):
-        """ OPTICS (Ordering Points To Identify Clustering Structure)
+        """OPTICS (Ordering Points To Identify Clustering Structure).
+
             algorithm for cluster analysis
         """
 
         cl = optics(sample=decision, eps=np.std(decision) / np.sqrt(2),
                     minpts=len(decision) // 2, amount_clusters=1, ccore=True)
 
         return self._pyclust_eval(cl, decision)
 
     def _SOMSC_clust(self, decision):
-        """ Self-organized feature map algorithm for cluster analysis """
+        """Self-organized feature map algorithm for cluster analysis."""
 
         cl = somsc(data=decision, amount_clusters=2, ccore=True)
 
         return self._pyclust_eval(cl, decision)
 
     def _SPEC_clust(self, decision):
-        """ Clustering to a projection of the normalized Laplacian """
+        """Clustering to a projection of the normalized Laplacian."""
 
         cl = SpectralClustering(n_clusters=2)
 
         return self._sklearn_eval(cl, decision)
 
     def _XMEANS_clust(self, decision):
-        """ X-means algorithm for cluster analysis """
+        """X-means algorithm for cluster analysis."""
 
         cl = xmeans(data=decision, kmax=2, ccore=True)
 
         return self._pyclust_eval(cl, decision)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/comb.py` & `pythresh-0.3.1/pythresh/thresholds/comb.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,22 +32,20 @@
            - 'median': calculate the median combined threshold
            - 'mode':  calculate the majority vote or mode of the thresholded labels
 
        random_state : int, optional (default=1234)
             Random seed for the random number generators of the thresholders. Can also
             be set to None.
 
-
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        confidence_interval_ : lower and upper confidence interval of the contamination level
-
     """
 
     def __init__(self, thresholders='default', max_contam=0.5, method='mean', random_state=1234):
 
         self.thresholders = thresholders
         self.max_contam = max_contam
         stat = {'mean': np.mean, 'median': np.median, 'mode': stats.mode}
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/cpd.py` & `pythresh-0.3.1/pythresh/thresholds/cpd.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
             - 'cdf': Use the cumulative distribution function
             - 'kde': Use the kernel density estimation
 
        Attributes
        ----------
 
-       thres_ : threshold value that seperates inliers from outliers       
+       thres_ : threshold value that seperates inliers from outliers
 
     """
 
     def __init__(self, method='Dynp', transform='cdf'):
 
         self.method = method
         self.transform = transform
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/decomp.py` & `pythresh-0.3.1/pythresh/thresholds/decomp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import numpy as np
 from sklearn.decomposition import NMF, PCA
+from sklearn.random_projection import (
+    GaussianRandomProjection,
+    SparseRandomProjection
+)
 from sklearn.utils import check_array
 
 from .base import BaseThresholder
 from .thresh_utility import cut, gen_cdf, normalize
 
 
 class DECOMP(BaseThresholder):
@@ -15,32 +19,34 @@
        matrix that results from decomposing the cumulative distribution
        function of the decision scores.
        See :cite:`boente2002decomp` for details
 
        Parameters
        ----------
 
-       method: {'NMF', 'PCA'}, optional (default='PCA')
+       method : {'NMF', 'PCA', 'GRP', 'SRP'}, optional (default='PCA')
             Method to use for decomposition
 
             - 'NMF':  Non-Negative Matrix Factorization
-            - 'PCA':  Principal component analysis
+            - 'PCA':  Principal Component Analysis
+            - 'GRP':  Gaussian Random Projection
+            - 'SRP':  Sparse Random Projection
 
        random_state : int, optional (default=1234)
             Random seed for the decomposition algorithm. Can also be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance 
-       signicantly. Therefore, to alleviate the effects of randomness on the 
+       The effects of randomness can affect the thresholder's output perfomance
+       signicantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -50,28 +56,29 @@
             clf = KNN()
             clf.fit(X_train)
 
             # get outlier scores
             decision_scores = clf.decision_scores_  # raw outlier scores
 
             # get outlier labels with combined model
-            thres = COMB(thresholders = [DECOMP(random_state=1234), 
-            DECOMP(random_state=42), DECOMP(random_state=9685), 
+            thres = COMB(thresholders = [DECOMP(random_state=1234),
+            DECOMP(random_state=42), DECOMP(random_state=9685),
             DECOMP(random_state=111222)])
             labels = thres.eval(decision_scores)
-
     """
 
     def __init__(self, method='PCA', random_state=1234):
 
         self.method = method
         self.method_funcs = {'NMF': NMF(random_state=random_state),
-                             'PCA': PCA(random_state=random_state)}
-        # make available as property for consistency with other thresholders
-        self.random_state = random_state
+                             'PCA': PCA(random_state=random_state),
+                             'GRP': GaussianRandomProjection(n_components=2,
+                                                             random_state=random_state),
+                             'SRP': SparseRandomProjection(n_components=3,
+                                                           random_state=random_state)}
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
@@ -96,13 +103,12 @@
 
         # Apply decomposition
         dec = self.method_funcs[str(self.method)].fit_transform(
             val.reshape(-1, 1))
 
         # Set limit to max value from decomposition matrix
         limit = np.max(dec)
-        if limit > 0.5:
-            limit = 1-limit
+        limit = 1-limit if limit > 0.5 else limit
 
         self.thresh_ = limit
 
         return cut(decision, limit)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/dsn.py` & `pythresh-0.3.1/pythresh/thresholds/dsn.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,16 @@
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance 
-       signicantly. Therefore, to alleviate the effects of randomness on the 
+       The effects of randomness can affect the thresholder's output perfomance
+       signicantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -67,24 +67,23 @@
             clf = KNN()
             clf.fit(X_train)
 
             # get outlier scores
             decision_scores = clf.decision_scores_  # raw outlier scores
 
             # get outlier labels with combined model
-            thres = COMB(thresholders = [DSN(random_state=1234), 
-            DSN(random_state=42), DSN(random_state=9685), 
+            thres = COMB(thresholders = [DSN(random_state=1234),
+            DSN(random_state=42), DSN(random_state=9685),
             DSN(random_state=111222)])
             labels = thres.eval(decision_scores)
-
     """
 
     def __init__(self, metric='MAH', random_state=1234):
 
-        super(DSN, self).__init__()
+        super().__init__()
         self.metric = metric
         self.metric_funcs = {'JS': self._JS_metric, 'WS': self._WS_metric,
                              'ENG': self._ENG_metric, 'BHT': self._BHT_metric,
                              'HLL': self._HLL_metric, 'HI': self._HI_metric,
                              'LK': self._LK_metric, 'LP': self._LP_metric,
                              'MAH': self._MAH_metric, 'TMT': self._TMT_metric,
                              'RES': self._RES_metric, 'KS': self._KS_metric,
@@ -140,55 +139,55 @@
         limit = self.metric_funcs[str(self.metric)]()
 
         self.thresh_ = limit
 
         return cut(decision, limit)
 
     def _JS_metric(self):
-        """Calculate the Jensen-Shannon distance"""
+        """Calculate the Jensen-Shannon distance."""
 
         return 1-distance.jensenshannon(self.val_data, self.val_norm)
 
     def _WS_metric(self):
-        """Calculate the Wasserstein or Earth Movers distance"""
+        """Calculate the Wasserstein or Earth Movers distance."""
 
         return stats.wasserstein_distance(self.val_data, self.val_norm)
 
     def _ENG_metric(self):
-        """Calculate the Energy distance"""
+        """Calculate the Energy distance."""
 
         return stats.energy_distance(self.val_data, self.val_norm)
 
     def _BHT_metric(self):
-        """Calculate the Bhattacharyya distance"""
+        """Calculate the Bhattacharyya distance."""
 
         bht = simpson(np.sqrt(self.val_data*self.val_norm),
                       dx=1/len(self.val_data))
 
         return np.log1p(bht)
 
     def _HLL_metric(self):
-        """Calculate the Hellinger distance"""
+        """Calculate the Hellinger distance."""
 
         val_data = self.val_data/np.sum(self.val_data)
         val_norm = self.val_norm/np.sum(self.val_norm)
 
         return (distance.euclidean(np.sqrt(val_data), np.sqrt(val_norm))
                 / np.sqrt(2))
 
     def _HI_metric(self):
-        """Calculate the Histogram intersection distance"""
+        """Calculate the Histogram intersection distance."""
 
         val_data = self.val_data/np.sum(self.val_data)
         val_norm = self.val_norm/np.sum(self.val_norm)
 
         return 1-np.sum(np.minimum(val_data, val_norm))
 
     def _LK_metric(self):
-        """Calculate the Lukaszyk-Karmowski metric for normal distributions"""
+        """Calculate the Lukaszyk-Karmowski metric for normal distributions."""
 
         # Get expected values for both distributions
         rng = np.linspace(0, 1, len(self.val_data))
         exp_data = (rng*self.val_data).sum()/self.val_data.sum()
         exp_norm = (rng*self.val_norm).sum()/self.val_norm.sum()
 
         nu_xy = np.abs(exp_data-exp_norm)
@@ -197,48 +196,48 @@
         std = np.std(rng)
 
         # Get the LK distance
         return (nu_xy + 2*std/np.sqrt(np.pi)*np.exp(-nu_xy**2/(4*std**2))
                 - nu_xy*special.erfc(nu_xy/(2*std)))
 
     def _LP_metric(self):
-        """Calculate the Levy-Prokhorov metric"""
+        """Calculate the Levy-Prokhorov metric."""
 
         # Get the edges for the complete graphs of the datasets
         f1 = np.array(list(combinations(self.val_data.tolist(), 2)))
         f2 = np.array(list(combinations(self.val_norm.tolist(), 2)))
 
         return (distance.directed_hausdorff(f1, f2)[0] /
                 distance.correlation(self.val_data, self.val_norm))
 
     def _MAH_metric(self):
-        """Calculate the Mahalanobis distance"""
+        """Calculate the Mahalanobis distance."""
 
         # fit a Minimum Covariance Determinant (MCD) robust estimator to data
         robust_cov = MinCovDet().fit(np.array([self.val_norm]).T)
 
         # Get the Mahalanobis distance
         dist = robust_cov.mahalanobis(np.array([self.val_data]).T)
 
         return 1-np.mean(dist)/np.max(dist)
 
     def _TMT_metric(self):
-        """Calculate the Tanimoto distance"""
+        """Calculate the Tanimoto distance."""
 
         val_data = self.val_data/np.sum(self.val_data)
         val_norm = self.val_norm/np.sum(self.val_norm)
 
         p = np.sum(val_data)
         q = np.sum(val_norm)
         m = np.sum(np.minimum(val_data, val_norm))
 
         return (p+q-2*m)/(p+q-m)
 
     def _RES_metric(self):
-        """Calculate the studentized residual distance"""
+        """Calculate the studentized residual distance."""
 
         mean_X = np.mean(self.val_data)
         mean_Y = np.mean(self.val_norm)
         n = len(self.val_data)
 
         diff_mean_sqr = np.dot((self.val_data - mean_X),
                                (self.val_data - mean_X))
@@ -257,20 +256,20 @@
 
         SE_regression = Var_e*((1-h_ii) ** 0.5)
         studentized_residuals = residuals/SE_regression
 
         return np.abs(np.sum(studentized_residuals))
 
     def _KS_metric(self):
-        """Calculate the Kolmogorov-Smirnov distance"""
+        """Calculate the Kolmogorov-Smirnov distance."""
 
         return np.max(np.abs(self.val_data-self.val_norm))
 
     def _INTER_metric(self):
-        """Calculate the weighted spline interpolation distance"""
+        """Calculate the weighted spline interpolation distance."""
 
         # Get splines
         data_spl = self._interp(self.data_range, self.val_data)
         norm_spl = self._interp(self.norm_range, self.val_norm)
 
         # Get distance of new weight shifted spline
         dist = []
@@ -280,28 +279,28 @@
             spline = (data_spl[0]*(1.0-weight) +
                       norm_spl[0]*weight)
             dist.append(np.max(spline))
 
         return np.mean(dist)-np.mean(self.norm)
 
     def _interp(self, x, y):
-        """Spline interpolation"""
+        """Spline interpolation."""
 
         # Smooth approximating B-spline coefficients
         tck, _ = interpolate.splprep([x, y], s=0)
 
         # Resample points
         points = np.arange(0.0, 1.0, 1e-2)
 
         # Generate spline
         spline = interpolate.splev(points, tck)
 
         return np.array(spline)
 
     def _MMD_metric(self):
-        """Calculate the Maximum Mean Discrepancy distance using a linear kernel"""
+        """Calculate the Maximum Mean Discrepancy distance using a linear kernel."""
 
         delta = self.val_data - self.val_norm
         delta = normalize(delta)
         delta = delta.dot(delta.T)
 
         return delta/np.sum(self.data_range)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/eb.py` & `pythresh-0.3.1/pythresh/thresholds/eb.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/thresholds/fgd.py` & `pythresh-0.3.1/pythresh/thresholds/fgd.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
        -----
 
        A probability distribution of the decision scores is generated using
        kernel density estimation. The first derivative of the pdf is
        calculated, and the threshold is set as the middle point between the
        first and second inflection points starting from the left side of the
        data range.
-
     """
 
     def __init__(self):
 
         pass
 
     def eval(self, decision):
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/filter.py` & `pythresh-0.3.1/pythresh/thresholds/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
             - 'hilbert':  use the hilbert based filter
             - 'wiener':   use the wiener based filter
             - 'medfilt:   use a median based filter
             - 'decimate': use a decimate based filter
             - 'detrend':  use a detrend based filter
             - 'resample': use a resampling based filter
 
-
        sigma : int, optional (default='auto')
             Variable specific to each filter type, default sets sigma to len(scores)*np.std(scores)
 
             - 'gaussian': standard deviation for Gaussian kernel
             - 'savgol':   savgol filter window size
             - 'hilbert':  number of Fourier components
             - 'medfilt:   kernel size
@@ -42,20 +41,19 @@
             - 'detrend':  number of break points
             - 'resample': resampling window size
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
-
     """
 
     def __init__(self, method='savgol', sigma='auto'):
 
-        super(FILTER, self).__init__()
+        super().__init__()
         self.method = method
         self.method_funcs = {'gaussian': self._GAU_fltr, 'savgol': self._SAV_fltr,
                              'hilbert': self._HIL_fltr, 'wiener': self._WIE_fltr,
                              'medfilt': self._MED_fltr, 'decimate': self._DEC_fltr,
                              'detrend': self._DET_fltr, 'resample': self._RES_fltr}
 
         self.sigma = sigma
@@ -78,75 +76,70 @@
         """
 
         decision = check_array(decision, ensure_2d=False)
 
         decision = normalize(decision)
 
         # Get sigma variables for various applications for each filter
-        sig = self.sigma
-        if self.sigma == 'auto':
-            sig = len(decision)*np.std(decision)
+        sig = (len(decision)*np.std(decision) if self.sigma == 'auto'
+               else self.sigma)
 
         # Filter scores
         fltr = self.method_funcs[str(self.method)](decision, sig)
         limit = np.max(fltr)
 
         self.thresh_ = limit
 
         return cut(decision, limit)
 
     def _GAU_fltr(self, decision, sig):
-        """Gaussian filter scores"""
+        """Gaussian filter scores."""
 
         return gaussian_filter(decision, sigma=sig)
 
     def _SAV_fltr(self, decision, sig):
-        """Savgol filter scores"""
+        """Savgol filter scores."""
 
-        if self.sigma == 'auto':
-            sig = round(0.5*sig)
+        sig = round(0.5*sig) if self.sigma == 'auto' else sig
 
-        if sig % 2 == 0:
-            sig += 1
+        sig = sig+1 if sig % 2 == 0 else sig
 
         return signal.savgol_filter(decision, window_length=round(sig),
                                     polyorder=1)
 
     def _HIL_fltr(self, decision, sig):
-        """Hilbert filter scores"""
+        """Hilbert filter scores."""
 
         return signal.hilbert(decision, N=round(sig))
 
     def _WIE_fltr(self, decision, sig):
-        """Wiener filter scores"""
+        """Wiener filter scores."""
 
         return signal.wiener(decision, mysize=len(decision))
 
     def _MED_fltr(self, decision, sig):
-        """Medfilt filter scores"""
+        """Medfilt filter scores."""
 
         sig = round(sig)
 
-        if sig % 2 == 0:
-            sig += 1
+        sig = sig+1 if sig % 2 == 0 else sig
 
         return signal.medfilt(decision, kernel_size=[sig])
 
     def _DEC_fltr(self, decision, sig):
-        """Decimate filter scores"""
+        """Decimate filter scores."""
 
         return signal.decimate(decision, q=round(sig), ftype='fir')
 
     def _DET_fltr(self, decision, sig):
-        """Detrend filter scores"""
+        """Detrend filter scores."""
 
-        return signal.detrend(decision, bp=np.linspace(0, len(decision)-1, round(sig)).astype(int))
+        return signal.detrend(decision, bp=np.linspace(0, len(decision)-1,
+                                                       round(sig)).astype(int))
 
     def _RES_fltr(self, decision, sig):
-        """Resampling filter scores"""
+        """Resampling filter scores."""
+
+        sig = np.sqrt(sig) if self.sigma == 'auto' else sig
 
-        if self.sigma == 'auto':
-            return signal.resample(decision, num=round(np.sqrt(len(decision))),
-                                   window=round(np.sqrt(sig)))
-        else:
-            return signal.resample(decision, num=round(np.sqrt(len(decision))),
-                                   window=round(sig))
+        return signal.resample(decision, num=round(np.sqrt(len(decision))),
+                               window=round(sig))
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/fwfm.py` & `pythresh-0.3.1/pythresh/thresholds/fwfm.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,19 @@
        -----
 
        The outlier detection scores are assumed to be a mixture of Gaussian
        distributions. The probability density function of this Gaussian mixture
        is approximated using kernel density estimation. The highest peak within the
        PDF is used to find the base width of the mixture and the threshold is set
        to the base width divided by the number of scores.
-
     """
 
     def __init__(self):
 
-        super(FWFM, self).__init__()
+        super().__init__()
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/gesd.py` & `pythresh-0.3.1/pythresh/thresholds/gesd.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/thresholds/hist.py` & `pythresh-0.3.1/pythresh/thresholds/hist.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,25 +29,23 @@
             - 'otsu':     OTSU's method for filtering
             - 'yen':      Yen's method for filtering
             - 'isodata':  Ridler-Calvard or inter-means method for filtering
             - 'li':       Li's iterative Minimum Cross Entropy method for filtering
             - 'minimum':  Minimum between two maxima via smoothing method for filtering
             - 'triangle': Triangle algorithm method for filtering
 
-
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
-
     """
 
     def __init__(self, method='triangle', nbins='auto'):
 
-        super(HIST, self).__init__()
+        super().__init__()
         self.nbins = nbins
         self.method = method
         self.method_funcs = {'otsu': self._OTSU_thres, 'yen': self._YEN_thres,
                              'isodata': self._ISODATA_thres, 'li': self._LI_thres,
                              'minimum': self._Minimum_thres,
                              'triangle': self._Triangle_thres}
 
@@ -94,23 +92,23 @@
         scores[outliers] = 1
 
         self.thresh_ = threshold
 
         return scores
 
     def _histogram(self, decision, nbins):
-        """Generate histograms and get bin centers"""
+        """Generate histograms and get bin centers."""
 
         counts, bin_edges = np.histogram(decision, bins=nbins, range=(0, 1))
         bin_centers = (bin_edges[:-1] + bin_edges[1:])/2.
 
         return bin_centers, counts
 
     def _find_local_maxima_idx(self, hist):
-        """Find the local maxima in histogram"""
+        """Find the local maxima in histogram."""
 
         maximum_idxs = []
         direction = 1
 
         for i in range(hist.shape[0] - 1):
             if direction > 0:
                 if hist[i + 1] < hist[i]:
@@ -118,15 +116,15 @@
                     maximum_idxs.append(i)
             elif hist[i + 1] > hist[i]:
                 direction = 1
 
         return maximum_idxs
 
     def _OTSU_thres(self, bin_centers, counts):
-        """Otsu's method for histogram based thresholding"""
+        """Otsu's method for histogram based thresholding."""
 
         counts = counts.astype(float)
 
         # class probabilities for all possible thresholds
         weight1 = np.cumsum(counts)
         weight2 = np.cumsum(counts[::-1])[::-1]
 
@@ -138,15 +136,15 @@
         variance12 = weight1[:-1] * weight2[1:] * (mean1[:-1] - mean2[1:])**2
 
         idx = np.argmax(variance12)
 
         return bin_centers[idx]
 
     def _YEN_thres(self, bin_centers, counts):
-        """Yen's method for histogram based thresholding"""
+        """Yen's method for histogram based thresholding."""
 
         # Calculate probability mass function
         pmf = counts.astype(np.float32) / counts.sum()
         P1 = np.cumsum(pmf)
         P1_sq = np.cumsum(pmf ** 2)
 
         # Get cumsum calculated from end of squared array:
@@ -155,15 +153,15 @@
         # Get critical value
         crit = np.log(((P1_sq[:-1] * P2_sq[1:]) ** -1) *
                       (P1[:-1] * (1.0 - P1[:-1])) ** 2)
 
         return bin_centers[crit.argmax()]
 
     def _ISODATA_thres(self, bin_centers, counts):
-        """ISODATA method for histogram based thresholding"""
+        """ISODATA method for histogram based thresholding."""
 
         counts = counts.astype(np.float32)
 
         # csuml and csumh contain the count of pixels in that bin or lower, and
         # in all bins strictly higher than that bin, respectively
         csuml = np.cumsum(counts)
         csumh = csuml[-1] - csuml
@@ -183,16 +181,18 @@
 
         # Look only at thresholds that are below the actual all_mean value
         distances = all_mean - bin_centers[:-1]
 
         return bin_centers[:-1][(distances >= 0) & (distances < bin_width)][0]
 
     def _LI_thres(self, decision, bin_centers, counts):
-        """Li's iterative Minimum Cross Entropy method for histogram
-        based thresholing"""
+        """Li's iterative Minimum Cross Entropy method for histogram.
+
+        based thresholing
+        """
 
         counts = counts.astype(float)
 
         tolerance = np.min(np.diff(np.unique(decision)))/2
         t_next = np.mean(decision)  # initial new guess for iteration
         t_curr = -2 * tolerance  # initial old guess for iteration
 
@@ -212,15 +212,15 @@
 
             t_next = ((mean_in - mean_out)
                       / (np.log(mean_in) - np.log(mean_out)))
 
         return t_next
 
     def _Minimum_thres(self, bin_centers, counts):
-        """Minimum method for histogram based thresholding"""
+        """Minimum method for histogram based thresholding."""
 
         smooth_hist = counts.astype(np.float64, copy=False)
 
         for _ in range(10000):
             smooth_hist = ndi.uniform_filter1d(smooth_hist, 3)
             maximum_idxs = self._find_local_maxima_idx(smooth_hist)
             if len(maximum_idxs) < 3:
@@ -229,15 +229,15 @@
         # Find lowest point between the maxima
         threshold_idx = np.argmin(
             smooth_hist[maximum_idxs[0]:maximum_idxs[1] + 1])
 
         return bin_centers[maximum_idxs[0] + threshold_idx]
 
     def _Triangle_thres(self, bin_centers, counts):
-        """Triangle algorithm for histogram based thresholding"""
+        """Triangle algorithm for histogram based thresholding."""
 
         nbins = len(counts)
 
         # Find peak, lowest and highest score levels.
         arg_peak_height = np.argmax(counts)
         peak_height = counts[arg_peak_height]
         arg_low_level, arg_high_level = np.where(counts > 0)[0][[0, -1]]
@@ -259,11 +259,10 @@
         peak_height /= norm
         width /= norm
 
         # Maximize the length.
         length = peak_height * x1 - width * y1
         arg_level = np.argmax(length) + arg_low_level
 
-        if flip:
-            arg_level = nbins - arg_level - 1
+        arg_level = nbins - arg_level - 1 if flip else arg_level
 
         return bin_centers[arg_level]
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/iqr.py` & `pythresh-0.3.1/pythresh/thresholds/iqr.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
            t = Q_3 + 1.5 IQR
 
     """
 
     def __init__(self):
 
-        super(IQR, self).__init__()
+        super().__init__()
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/karch.py` & `pythresh-0.3.1/pythresh/thresholds/karch.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/thresholds/mad.py` & `pythresh-0.3.1/pythresh/thresholds/mad.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
        where :math:`\bar{x}` and :math:`\sigma` are the mean and
        standard deviation of the scores respectively
 
     """
 
     def __init__(self):
 
-        super(MAD, self).__init__()
+        super().__init__()
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/mcst.py` & `pythresh-0.3.1/pythresh/thresholds/wind.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,137 @@
 import numpy as np
-import scipy.stats as stats
+from scipy import integrate, stats
 from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import cut, gen_kde, normalize
 
 
-class MCST(BaseThresholder):
-    r"""MCST class for Monte Carlo Shapiro Tests thresholder.
+class WIND(BaseThresholder):
+    r"""WIND class for topological Winding number thresholder.
 
-       Use uniform random sampling and statistical testing to evaluate a
-       non-parametric means to threshold scores generated by the decision_scores
-       where outliers are set to any value beyond the minimum value left after
-       iterative Shapiro-Wilk tests have occurred. Note** accuracy decreases with
-       array size. For good results the should be array<1000. However still this
-       threshold method may fail at any array size.
-       See :cite:`coin2008mcst` for details.
+       Use the topological winding number (with respect to the origin) to
+       evaluate a non-parametric means to threshold scores generated by
+       the decision_scores where outliers are set to any value beyond the
+       mean intersection point calculated from the winding number.
+       See :cite:`jacobson2013wind` for details.
 
        Parameters
        ----------
 
        random_state : int, optional (default=1234)
-            Random seed for the uniform distribution. Can also be set to None.
+            Random seed for the normal distribution. Can also be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Notes
        -----
 
-       The Shapiro-Wilk test is a frequentist statistical test for normality.
-       It is used to test the null-hypothesis that the decision scores came
-       from a normal distribution. This test statistic is defined as:
+       The topological winding number or the degree of a continuous mapping. It is an
+       integer sum of the number of completed/closed counterclockwise rotations in a plane
+       around a point. And is given by,
 
        .. math::
 
-          W = \frac{\left(\sum_{i=1}^n a_i x_{(i)} \right)^2}{\sum_{i=1}^n \left(x_i - \bar{x} \right)^2} \mathrm{,}
+           \mathrm{d}\theta = \frac{1}{r^2} \left(x\mathrm{d}y - y\mathrm{d}x \right) \mathrm{,}
 
-       where :math:`\bar{x}` is the mean of the scores and :math:`x_{(i)}`
-       is the ith-smallest number in the sample (kth order statistic). The
-       coefficients :math:`a_i` is given by:
+       where :math:`r^2 = x^2 + y^2`
 
        .. math::
 
-          (a_1,...,a_n) = \frac{m^{\top}V^{-1}}{\sqrt{m^{\top}V^{-1}V^{-1}m}} \mathrm{,}
+           wind(\gamma,0) = \frac{1}{2\pi} \oint_\gamma \mathrm{d}\theta
 
-       where the vector :math:`m=\lvert(m_1,...,m_n \rvert)^{\top}` and :math:`V`
-       is the covariance matrix of the order statistics.
-
-       The threshold is set by first calculating an initial Shapiro-Wilk test
-       p-value on the decision scores. Using Monte Carlo simulations, random values
-       between 0-1 are inserted into the normalized decision scores and p-values are
-       calculated. if the p-value is higher than the initial p-value, the initial p-value
-       is set to this value and the random value is stored. The minimum stored random
-       value is set as the threshold as it is the minimum found outlier.
+       The winding number intuitively captures self-intersections/contours, with a change in the
+       distribution of the dataset or shift from inliers to outliers relating to these intersections.
+       With this, it is assumed that if an intersection exists, then adjacent/incident regions
+       must have different region labels. Since multiple intersection regions may exist. The
+       threshold between inliers and outliers is taken as the mean intersection point.
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance 
-       signicantly. Therefore, to alleviate the effects of randomness on the 
+       The effects of randomness can affect the thresholder's output perfomance
+       signicantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
             from pythresh.thresholds.comb import COMB
-            from pythresh.thresholds.mcst import MCST
+            from pythresh.thresholds.wind import WIND
 
             clf = KNN()
             clf.fit(X_train)
 
             # get outlier scores
             decision_scores = clf.decision_scores_  # raw outlier scores
 
             # get outlier labels with combined model
-            thres = COMB(thresholders = [MCST(random_state=1234), 
-            MCST(random_state=42), MCST(random_state=9685), 
-            MCST(random_state=111222)])
+            thres = COMB(thresholders = [WIND(random_state=1234),
+            WIND(random_state=42), WIND(random_state=9685),
+            WIND(random_state=111222)])
             labels = thres.eval(decision_scores)
 
     """
 
     def __init__(self, random_state=1234):
+        super().__init__()
         self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
-        decision : np.array or list of shape (n_samples)
-                   which are the decision scores from a
-                   outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
         decision = check_array(decision, ensure_2d=False)
 
         decision = normalize(decision)
 
-        # Get Baseline Shapiro-Wilk test p-value
-        p_std = stats.shapiro(decision).pvalue
-
-        # Create random dataset to insert and test p-values
-        rnd = stats.uniform.rvs(loc=0, scale=1, size=len(
-            decision), random_state=self.random_state)
-        rnd = normalize(rnd)
-        povr = []
-
-        # Iterate and add a new random variable
-        # Perform a Shapiro-Wilk test and see if the new
-        # distribution has a lower or higher p-value
-        # If higher record these potential outlier values
-        for i in range(len(rnd)):
-
-            arr = np.append(decision, rnd[i])
-            p_check = stats.shapiro(arr).pvalue
+        # Create a normal distribution and normalize
+        size = min(len(decision), 1500)
+        norm = stats.norm.rvs(size=size, loc=0.0, scale=1.0,
+                              random_state=self.random_state)
+        norm = normalize(norm)
+
+        # Create a KDE of the labels and the normal distribution
+        # Generate KDE
+        val_data, dat_range = gen_kde(decision, 0, 1, len(decision)*3)
+        val_norm, _ = gen_kde(norm, 0, 1, len(decision)*3)
+
+        # Get the rsquared value
+        r2 = val_data**2 + val_norm**2
+
+        val_data = val_data/np.max(val_data)
+        val_norm = val_norm/np.max(val_norm)
+
+        # Find the first derivatives of the decision and norm kdes
+        # with respect to the decision scores
+        deriv_data = np.gradient(val_data, dat_range[1]-dat_range[0])
+        deriv_norm = np.gradient(val_norm, dat_range[1]-dat_range[0])
+
+        # Compute integrand
+        integrand = self._dtheta(
+            val_data, val_norm, deriv_data, deriv_norm, r2)
 
-            if p_check > p_std:
+        # Integrate to find winding numbers mean intersection point
+        limit = integrate.simpson(integrand)/np.sum((val_data+val_norm)/2)
 
-                p_std = p_check
-                povr.append(rnd[i])
-
-        limit = np.min(povr) if povr else 1.1
         self.thresh_ = limit
 
         return cut(decision, limit)
+
+    def _dtheta(self, x, y, dx, dy, r2):
+        """Calculate dtheta for the integrand."""
+        return (x*dy - y*dx)/r2
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/meta.py` & `pythresh-0.3.1/pythresh/thresholds/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,18 @@
        that contains only the explanatory variables (X), yet no response
        variable (y), it can still be predicted by using a meta-model. This
        is done by modelling datasets with known response variables that
        are similar to the dataset that is missing the response variable.
 
        The META thresholder was trained using the ``PyOD`` outlier
        detection methods ``LODA, QMCD, CD, MCD, GMM, KNN, KDE, PCA, Sampling`` and ``IForest``
-       on the AD benchmark datasets: ``ALOI, annthyroid, breastw, campaign, cardio, 
-       Cardiotocography, fault, glass, Hepatitis, Ionosphere, landsat, letter, Lymphography, 
-       magic.gamma, mammography, mnist, musk, optdigits, PageBlocks, pendigits, Pima, 
-       satellite, satimage-2, shuttle, smtp, SpamBase, speech, Stamps, thyroid, vertebral, 
+       on the AD benchmark datasets: ``ALOI, annthyroid, breastw, campaign, cardio,
+       Cardiotocography, fault, glass, Hepatitis, Ionosphere, landsat, letter, Lymphography,
+       magic.gamma, mammography, mnist, musk, optdigits, PageBlocks, pendigits, Pima,
+       satellite, satimage-2, shuttle, smtp, SpamBase, speech, Stamps, thyroid, vertebral,
        vowels, Waveform,  WBC, WDBC, Wilt, wine, WPBC, yeast`` available at
        `ADBench dataset <https://github.com/Minqi824/ADBench/tree/main/datasets/Classical>`_.
        META uses a majority vote of all the trained models to determine the
        inlier/outlier labels.
 
     """
 
@@ -97,22 +97,22 @@
         counts = len(decision)
         parent = up(up(__file__))
         model = joblib.load(os.path.join(parent, 'models', clf))
 
         if self.method == 'GNBM':
 
             scaler = MinMaxScaler()
-            norm = scaler.fit_transform(decision.reshape(-1,1))
+            norm = scaler.fit_transform(decision.reshape(-1, 1))
             norm = (norm/(norm.max(axis=0, keepdims=True)
-                            + np.spacing(0)))
+                          + np.spacing(0)))
 
             qmcd = self._wrap_around_discrepancy(norm)
-            
+
             qmcd = normalize(qmcd)
-            if len(qmcd[qmcd>0.5]) > 0.5*len(qmcd):
+            if len(qmcd[qmcd > 0.5]) > 0.5*len(qmcd):
                 qmcd = 1 - qmcd
 
             kde = stats.gaussian_kde(decision)
             pdf = normalize(kde.pdf(decision))
 
         for i in range(380):
 
@@ -152,12 +152,12 @@
         for i in prange(n):
             dc = 0.0
             for j in prange(n):
                 prod = 1.0
                 for k in prange(d):
                     x_kikj = abs(data[i, k] - data[j, k])
                     prod *= 3.0 / 2.0 - x_kikj + x_kikj ** 2
-                        
+
                 dc += prod
             disc[i] = dc
 
         return - (4.0 / 3.0) ** d + 1.0 / (n ** 2) * disc
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/moll.py` & `pythresh-0.3.1/pythresh/thresholds/moll.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/thresholds/mtt.py` & `pythresh-0.3.1/pythresh/thresholds/mtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 break
 
         self.thresh_ = limit
 
         return cut(decision, limit)
 
     def _get_T_critical_value(self, n, strictness):
-        """Get the value from the t-Student distribution for the given n"""
+        """Get the value from the t-Student distribution for the given n."""
 
         mapping = {
             1: [{1: 3.078, 2: 1.886, 3: 1.638, 4: 1.533, 5: 1.476, 6: 1.440, 7: 1.415, 8: 1.397, 9: 1.383, 10: 1.372, 11: 1.363, 12: 1.356,
                  13: 1.350, 14: 1.345, 15: 1.341, 16: 1.337, 17: 1.333, 18: 1.330, 19: 1.328, 20: 1.325, 21: 1.323, 22: 1.321, 23: 1.319,
                  24: 1.318, 25: 1.316, 26: 1.315, 27: 1.314, 28: 1.313, 29: 1.311, 30: 1.310, 40: 1.303, 50: 1.299, 60: 1.296, 80: 1.292,
                  100: 1.290, 120: 1.289}, 1.282],
             2: [{1: 6.314, 2: 2.920, 3: 2.353, 4: 2.132, 5: 2.015, 6: 1.943, 7: 1.895, 8: 1.860, 9: 1.833, 10: 1.812, 11: 1.796, 12: 1.782,
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/ocsvm.py` & `pythresh-0.3.1/pythresh/thresholds/ocsvm.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance 
-       signicantly. Therefore, to alleviate the effects of randomness on the 
+       The effects of randomness can affect the thresholder's output perfomance
+       signicantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -78,19 +78,18 @@
             clf = KNN()
             clf.fit(X_train)
 
             # get outlier scores
             decision_scores = clf.decision_scores_  # raw outlier scores
 
             # get outlier labels with combined model
-            thres = COMB(thresholders = [OCSVM(random_state=1234), 
-            OCSVM(random_state=42), OCSVM(random_state=9685), 
+            thres = COMB(thresholders = [OCSVM(random_state=1234),
+            OCSVM(random_state=42), OCSVM(random_state=9685),
             OCSVM(random_state=111222)])
             labels = thres.eval(decision_scores)
-
     """
 
     def __init__(self, model='sgd', degree='auto', gamma='auto',
                  criterion='bic', nu='auto', tol=1e-3, random_state=1234):
 
         self.model = model
         self.degree = degree
@@ -126,16 +125,16 @@
             np.seterr(divide='ignore')
             gmean = stats.gmean(decision)
             mean = np.mean(decision)
             med = np.median(decision)
 
             self.nu = len(decision[decision <= med +
                           abs(mean-gmean)])/len(decision)
-            if self.nu == 1.0:
-                self.nu = 0.5  # use sklearn default
+
+        self.nu = 0.5 if self.nu == 1.0 else self.nu
 
         # Get auto degree calculation
         if (self.degree == 'auto') & (self.model == 'poly'):
 
             self.degree = self._auto_crit(decision)
 
         decision = decision.reshape(-1, 1)
@@ -163,15 +162,15 @@
         res[mask] = 0
 
         self.thresh_ = None
 
         return res
 
     def _auto_crit(self, decision):
-        '''Decide polynomial degree using criterion'''
+        """Decide polynomial degree using criterion."""
 
         # Generate kde
         kde, dat_range = gen_kde(decision, 0, 1, len(decision))
 
         # Set polynomial degrees to test
         polys = [2, 3, 4, 5, 6, 7, 8, 9, 10]
         n = len(decision)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/qmcd.py` & `pythresh-0.3.1/pythresh/thresholds/qmcd.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
        lim : {'Q', 'P'}, optional (default='P')
             Filtering method to threshold scores using 1 - discrepancy
 
             - 'Q': Use quantile limiting
             - 'P': Use percentile limiting
 
-
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Notes
        -----
@@ -54,20 +53,19 @@
        space.
 
        The QMCD method utilizes the discrepancy value by assuming that when it is at its lowest
        value (0) the "quasi-random" generated sequences and the decision scores are equally
        equidistributed across :math:`M`. Outliers are assumed to solely raise the discrepancy
        value. And therefore, the contamination of the dataset can be set as one minus the
        discrepancy.
-
     """
 
     def __init__(self, method='WD', lim='P'):
 
-        super(QMCD, self).__init__()
+        super().__init__()
         self.method = method
         self.lim = lim
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/regr.py` & `pythresh-0.3.1/pythresh/thresholds/regr.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance 
-       signicantly. Therefore, to alleviate the effects of randomness on the 
+       The effects of randomness can affect the thresholder's output perfomance
+       signicantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -48,24 +48,23 @@
             clf = KNN()
             clf.fit(X_train)
 
             # get outlier scores
             decision_scores = clf.decision_scores_  # raw outlier scores
 
             # get outlier labels with combined model
-            thres = COMB(thresholders = [REGR(random_state=1234), 
-            REGR(random_state=42), REGR(random_state=9685), 
+            thres = COMB(thresholders = [REGR(random_state=1234),
+            REGR(random_state=42), REGR(random_state=9685),
             REGR(random_state=111222)])
             labels = thres.eval(decision_scores)
-
     """
 
     def __init__(self, method='siegel', random_state=1234):
 
-        super(REGR, self).__init__()
+        super().__init__()
         self.method = method
         self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/thresh_utility.py` & `pythresh-0.3.1/pythresh/thresholds/thresh_utility.py`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.0/pythresh/thresholds/vae.py` & `pythresh-0.3.1/pythresh/thresholds/vae.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance 
-       signicantly. Therefore, to alleviate the effects of randomness on the 
+       The effects of randomness can affect the thresholder's output perfomance
+       signicantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -72,16 +72,16 @@
             clf = KNN()
             clf.fit(X_train)
 
             # get outlier scores
             decision_scores = clf.decision_scores_  # raw outlier scores
 
             # get outlier labels with combined model
-            thres = COMB(thresholders = [VAE(random_state=1234), 
-            VAE(random_state=42), VAE(random_state=9685), 
+            thres = COMB(thresholders = [VAE(random_state=1234),
+            VAE(random_state=42), VAE(random_state=9685),
             VAE(random_state=111222)])
             labels = thres.eval(decision_scores)
 
     """
 
     def __init__(self, verbose=False, device='cpu', latent_dims='auto',
                  random_state=1234, epochs=100, batch_size=64, loss='kl'):
@@ -138,15 +138,15 @@
 
         limit = np.max(z)-np.min(z)
         self.thresh_ = limit
 
         return cut(scores, limit)
 
     def _autodim(self, vals):
-        ''' Estimate the latent dimension size using the method of Zhu and Ghodsi (2006) '''
+        """Estimate the latent dimension size using the method of Zhu and Ghodsi (2006)."""
 
         vals = np.sort(vals)[::-1]
         m = len(vals)
         profile_lik = []
 
         for i in range(1, m):
 
@@ -169,15 +169,15 @@
         optimizer = torch.optim.Adam(self.model.parameters(),
                                      weight_decay=1e-4,
                                      lr=1e-2)
 
         scheduler = opt.lr_scheduler.ExponentialLR(optimizer,
                                                    gamma=0.95)
 
-        for _ in (tqdm(range(self.epochs), ascii=True, desc="Training")
+        for _ in (tqdm(range(self.epochs), ascii=True, desc='Training')
                   if self.verbose else range(self.epochs)):
 
             for x in self.data:
 
                 x = x.to(self.device)
                 optimizer.zero_grad()
                 _ = self.model.forward(x)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/yj.py` & `pythresh-0.3.1/pythresh/thresholds/yj.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
        to a normal distribution originally the smaller the probability this
        threshold will be able to identify outliers.
 
     """
 
     def __init__(self):
 
-        super(YJ, self).__init__()
+        super().__init__()
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
```

### Comparing `pythresh-0.3.0/pythresh/thresholds/zscore.py` & `pythresh-0.3.1/pythresh/thresholds/zscore.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
        is set that any value beyond an absolute z-score of 1 is considered
        and outlier.
 
     """
 
     def __init__(self):
 
-        super(ZSCORE, self).__init__()
+        super().__init__()
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
```

### Comparing `pythresh-0.3.0/pythresh.egg-info/PKG-INFO` & `pythresh-0.3.1/pythresh.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythresh
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python Toolbox for Outlier Detection Thresholding
 Home-page: https://github.com/KulikDM/pythresh
 Author: D Kulik
 License: UNKNOWN
 Download-URL: https://github.com/KulikDM/pythresh/archive/master.zip
 Project-URL: Documentation, https://pythresh.readthedocs.io/en/latest/
 Keywords: outlier detection,anomaly detection,thresholding,cutoff,contamintion level,data science,machine learning
@@ -16,14 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ##################################################
  Python Outlier Detection Thresholding (PyThresh)
 ##################################################
 
@@ -33,15 +34,15 @@
    :target: https://pypi.org/project/pythresh/
    :alt: PyPI version
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/pythresh?color=brightgreen&logo=conda-forge&logoColor=white
    :target: https://anaconda.org/conda-forge/pythresh
    :alt: Anaconda version
 
-.. image:: https://readthedocs.org/projects/pythresh/badge/?version=latest
+.. image:: https://img.shields.io/readthedocs/pythresh.svg?version=latest&logo=read-the-docs&logoColor=white
    :target: http://pythresh.readthedocs.io/?badge=latest
    :alt: Documentation status
 
 .. image:: https://github.com/KulikDM/pythresh/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/KulikDM/pythresh/actions/workflows/python-package.yml
    :alt: testing
 
@@ -61,14 +62,18 @@
    :target: https://pypi.org/project/pythresh/
    :alt: Python versions
 
 .. image:: https://img.shields.io/github/license/KulikDM/pythresh.svg
    :target: https://github.com/KulikDM/pythresh/blob/master/LICENSE
    :alt: License
 
+.. image:: https://zenodo.org/badge/497683169.svg
+   :target: https://zenodo.org/badge/latestdoi/497683169
+   :alt: Zenodo DOI
+
 ----
 
 PyThresh is a comprehensive and scalable **Python toolkit** for
 **thresholding outlier detection scores** in univariate/multivariate
 data. It has been writen to work in tandem with PyOD and has similar
 syntax and data structures. However, it is not limited to this single
 library. PyThresh is meant to threshold scores generated by an outlier
@@ -82,20 +87,25 @@
 All threshold functions return a binary array where inliers and outliers
 are represented by a 0 and 1 respectively.
 
 PyThresh includes more than 30 thresholding algorithms. These algorithms
 range from using simple statistical analysis like the Z-score to more
 complex mathematical methods that involve graph theory and topology.
 
-***************
- Documentation
-***************
+************************
+ Documentation & Citing
+************************
+
+Visit `PyThresh Docs
+<https://pythresh.readthedocs.io/en/latest/?badge=latest>`_ for full
+documentation or see below for a quickstart installation and usage
+example.
 
-Visit `PyThresh Docs <https://pythresh.readthedocs.io/en/latest/?badge=latest>`_
-for full documentation or see below for a quickstart installation and usage example
+To cite this work you can visit `PyThresh Citation
+<https://zenodo.org/badge/latestdoi/497683169>`_
 
 ----
 
 **Outlier Detection Thresholding with 7 Lines of Code**:
 
 .. code:: python
 
@@ -143,22 +153,22 @@
 
    pip install https://github.com/KulikDM/pythresh/archive/main.zip
 
 **Required Dependencies**:
 
 -  matplotlib
 -  numpy>=1.13
--  pyclustering
 -  pyod
 -  scipy>=1.3.1
 -  scikit_learn>=0.20.0
 -  six
 
 **Optional Dependencies**:
 
+-  pyclustering (used in the CLUST thresholder)
 -  ruptures (used in the CPD thresholder)
 -  geomstats (used in the KARCH thresholder)
 -  scikit-lego (used in the META thresholder)
 -  joblib>=0.14.1 (used in the META thresholder)
 -  pandas (used in the META thresholder)
 -  torch (used in the VAE thresholder)
 -  tqdm (used in the VAE thresholder)
@@ -255,32 +265,31 @@
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | WIND      | Topological Winding Number                | [#wind1]_          | `pythresh.thresholds.wind module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.wind>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | YJ        | Yeo-Johnson Transformation                | [#yj1]_            | `pythresh.thresholds.yj module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.yj>`_                    |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | ZSCORE    | Z-score                                   | [#zscore1]_        | `pythresh.thresholds.zscore module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.zscore>`_            |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
-| ALL       | All Thresholders Combined                 | None               | `pythresh.thresholds.all module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.all>`_                  |
-+-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | COMB      | Thresholder Combination                   | None               | `pythresh.thresholds.comb module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.comb>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 
 ******************************
  Implementations & Benchmarks
 ******************************
 
 **The comparison among implemented models and general implementation**
 is made available below
 
-Additional `benchmarking <https://pythresh.readthedocs.io/en/latest/benchmark.html>`_ 
-has been done on all the thresholders and it was
-found that the ``META`` thresholder performed best while the ``CLF`` 
-thresholder provided the smallest uncertainty about its mean and is the 
-most robust (best least accurate prediction). However, for interpretability 
-and general performance the ``FILTER`` thresholder is a good fit.
+Additional `benchmarking
+<https://pythresh.readthedocs.io/en/latest/benchmark.html>`_ has been
+done on all the thresholders and it was found that the ``META``
+thresholder performed best while the ``CLF`` thresholder provided the
+smallest uncertainty about its mean and is the most robust (best least
+accurate prediction). However, for interpretability and general
+performance the ``FILTER`` thresholder is a good fit.
 
 ----
 
 For Jupyter Notebooks, please navigate to `notebooks
 <https://github.com/KulikDM/pythresh/tree/main/notebooks>`_.
 
 A quick look at all the thresholders performance can be found at
@@ -288,40 +297,43 @@
 
 .. image:: https://raw.githubusercontent.com/KulikDM/pythresh/main/imgs/All.png
    :target: https://raw.githubusercontent.com/KulikDM/pythresh/main/imgs/All.png
    :alt: Comparision_of_All
 
 ----
 
-
 **************
  Contributing
 **************
 
 Anyone is welcome to contribute to PyThresh:
 
-* Please share your ideas and ask questions by opening an issue.
+-  Please share your ideas and ask questions by opening an issue.
 
-* To contribute, first check the Issue list for the "help wanted" tag and comment 
-  on the one that you are interested in. The issue will then be assigned to you.
+-  To contribute, first check the Issue list for the "help wanted" tag
+   and comment on the one that you are interested in. The issue will
+   then be assigned to you.
 
-* If the bug, feature, or documentation change is novel (not in the Issue list),
-  you can either log a new issue or create a pull request for the new changes.
+-  If the bug, feature, or documentation change is novel (not in the
+   Issue list), you can either log a new issue or create a pull request
+   for the new changes.
 
-* To start, fork the main branch and add your improvement/modification/fix.
+-  To start, fork the main branch and add your
+   improvement/modification/fix.
 
-* To make sure the code has the same style and standard, please refer to qmcd.py for 
-  example.
+-  To make sure the code has the same style and standard, please refer
+   to qmcd.py for example.
 
-* Create a pull request to the **main branch** and follow the pull request template 
-  `PR template <https://github.com/KulikDM/pythresh/blob/main/.github/PULL_REQUEST_TEMPLATE.md>`_
+-  Create a pull request to the **main branch** and follow the pull
+   request template `PR template
+   <https://github.com/KulikDM/pythresh/blob/main/.github/PULL_REQUEST_TEMPLATE.md>`_
 
-* Please make sure that all code changes are accompanied with proper new/updated test 
-  functions. Automatic tests will be triggered. Before the pull request can be merged, 
-  make sure that all the tests pass.
+-  Please make sure that all code changes are accompanied with proper
+   new/updated test functions. Automatic tests will be triggered. Before
+   the pull request can be merged, make sure that all the tests pass.
 
 ----
 
 ************
  References
 ************
```

### Comparing `pythresh-0.3.0/pythresh.egg-info/SOURCES.txt` & `pythresh-0.3.1/pythresh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 pythresh.egg-info/requires.txt
 pythresh.egg-info/top_level.txt
 pythresh/models/meta_model_GNB.pkl
 pythresh/models/meta_model_GNBC.pkl
 pythresh/models/meta_model_GNBM.pkl
 pythresh/models/meta_model_LIN.pkl
 pythresh/thresholds/__init__.py
-pythresh/thresholds/all.py
 pythresh/thresholds/aucp.py
 pythresh/thresholds/base.py
 pythresh/thresholds/boot.py
 pythresh/thresholds/chau.py
 pythresh/thresholds/clf.py
 pythresh/thresholds/clust.py
 pythresh/thresholds/comb.py
```

### Comparing `pythresh-0.3.0/setup.py` & `pythresh-0.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import re
 import sys
-from io import open
 # read the contents of README file
 from os import path
 
 from setuptools import find_packages, setup
 
 # get __version__ from version.py
 try:
     verpath = path.join('pythresh', 'version.py')
     with open(verpath) as version_file:
         __version__ = str(re.findall(
             r'\b\d+(?:\.\d+)+', version_file.read())[0])
 except Exception as error:
-    __version__ = "0.0.1"
+    __version__ = '0.0.1'
     sys.stderr.write("Warning: Could not open '%s' due %s\n" %
                      (verpath, error))
 
 
 this_directory = path.abspath(path.dirname(__file__))
 
 
@@ -40,15 +39,15 @@
     long_description_content_type='text/x-rst',
     author='D Kulik',
     url='https://github.com/KulikDM/pythresh',
     download_url='https://github.com/KulikDM/pythresh/archive/master.zip',
     keywords=['outlier detection', 'anomaly detection', 'thresholding', 'cutoff',
               'contamintion level', 'data science', 'machine learning'],
     project_urls={
-        "Documentation": 'https://pythresh.readthedocs.io/en/latest/'},
+        'Documentation': 'https://pythresh.readthedocs.io/en/latest/'},
     packages=find_packages(exclude=['test']),
     include_package_data=True,
     install_requires=requirements,
     setup_requires=['setuptools>=38.6.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Education',
@@ -57,9 +56,10 @@
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

