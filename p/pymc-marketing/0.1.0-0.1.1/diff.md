# Comparing `tmp/pymc-marketing-0.1.0.tar.gz` & `tmp/pymc-marketing-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-marketing-0.1.0.tar", last modified: Thu Apr  6 12:34:13 2023, max compression
+gzip compressed data, was "pymc-marketing-0.1.1.tar", last modified: Wed May  3 10:22:24 2023, max compression
```

## Comparing `pymc-marketing-0.1.0.tar` & `pymc-marketing-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:34:13.707226 pymc-marketing-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20911 2023-04-06 12:34:13.707226 pymc-marketing-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:34:13.707226 pymc-marketing-0.1.0/pymc_marketing/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:34:13.707226 pymc-marketing-0.1.0/pymc_marketing/clv/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/clv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/clv/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:34:13.707226 pymc-marketing-0.1.0/pymc_marketing/clv/models/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/clv/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/clv/models/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/clv/models/beta_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/clv/models/gamma_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/clv/models/shifted_beta_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/clv/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/clv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:34:13.707226 pymc-marketing-0.1.0/pymc_marketing/mmm/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/mmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/mmm/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/mmm/delayed_saturated_mmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/mmm/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/mmm/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/mmm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/mmm/validating.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pymc_marketing/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:34:13.707226 pymc-marketing-0.1.0/pymc_marketing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20911 2023-04-06 12:34:13.000000 pymc-marketing-0.1.0/pymc_marketing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-06 12:34:13.000000 pymc-marketing-0.1.0/pymc_marketing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 12:34:13.000000 pymc-marketing-0.1.0/pymc_marketing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-06 12:34:13.000000 pymc-marketing-0.1.0/pymc_marketing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-06 12:34:13.000000 pymc-marketing-0.1.0/pymc_marketing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-06 12:34:03.000000 pymc-marketing-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 12:34:13.707226 pymc-marketing-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20972 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.160673 pymc-marketing-0.1.1/pymc_marketing/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.160673 pymc-marketing-0.1.1/pymc_marketing/clv/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/pymc_marketing/clv/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/beta_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/gamma_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/models/shifted_beta_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/clv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/pymc_marketing/mmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20190 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/delayed_saturated_mmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/mmm/validating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pymc_marketing/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:22:24.160673 pymc-marketing-0.1.1/pymc_marketing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20972 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 10:22:24.000000 pymc-marketing-0.1.1/pymc_marketing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-03 10:22:15.000000 pymc-marketing-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:22:24.164673 pymc-marketing-0.1.1/setup.cfg
```

### Comparing `pymc-marketing-0.1.0/LICENSE` & `pymc-marketing-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.0/PKG-INFO` & `pymc-marketing-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-marketing
-Version: 0.1.0
+Version: 0.1.1
 Summary: Marketing Statistical Models in PyMC
 Maintainer-email: PyMC Labs <info@pymc-labs.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,45 +209,43 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
-# PyMC-Marketing
+<div align="center">
+  <a href="https://github.com/pymc-labs/pymc-marketing"><img height="240px" src="docs/source/_static/marketing-logo-light.jpg"></a>
+</div>
+
+----
 
 ![Build](https://github.com/pymc-labs/pymc-marketing/workflows/ci/badge.svg)
 [![codecov](https://codecov.io/gh/pymc-labs/pymc-marketing/branch/main/graph/badge.svg?token=OBV3BS5TYE)](https://codecov.io/gh/pymc-labs/pymc-marketing)
 [![docs](https://readthedocs.org/projects/pymc-marketing/badge/?version=latest)](https://docs.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI Version](https://img.shields.io/pypi/v/pymc-marketing.svg)](https://pypi.python.org/pypi/pymc-marketing)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-**Unlock the power of marketing analytics with PyMC-Marketing – the open source solution for smarter decision-making.** Media mix modeling and customer lifetime value modules allow businesses to make data-driven decisions about their marketing campaigns. Optimize your marketing strategy and unlock the full potential of your customer data.
+# PyMC-Marketing
 
----
+**Unlock the power of marketing analytics with PyMC-Marketing – the open source solution for smarter decision-making.** Media mix modeling and customer lifetime value modules allow businesses to make data-driven decisions about their marketing campaigns. Optimize your marketing strategy and unlock the full potential of your customer data.
 
 ## Installation
 
-Start by setting up an environment (e.g. `marketing_env`) with PyMC. It may look something like the following:
+Install and activate an environment (e.g. `marketing_env`) with the `pymc-marketing` package from [conda-forge](https://conda-forge.org). It may look something like the following:
 
 ```bash
-mamba create -c conda-forge -n marketing_env python "pymc>=5"
+mamba create -c conda-forge -n marketing_env pymc-marketing
 mamba activate marketing_env
 ```
 
 See the official [PyMC installation guide](https://www.pymc.io/projects/docs/en/latest/installation.html) if more detail is needed.
 
-Assuming you have an environment set up then install PyMC-Marketing with the following command. This will give you the latest version of the library from PyPI.
-
-```bash
-pip install pymc-marketing
-```
-
-Alternatively you can install from GitHub directly:
+For testing purposes, if you wish to install the `main` branch directly from GitHub:
 
 ```bash
 pip install git+https://github.com/pymc-labs/pymc-marketing.git
 ```
 
 ## Bayesian Media Mix Models (MMMs) in PyMC
```

### Comparing `pymc-marketing-0.1.0/README.md` & `pymc-marketing-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,473 +1,477 @@
-00000000: 2320 5079 4d43 2d4d 6172 6b65 7469 6e67  # PyMC-Marketing
-00000010: 0a0a 215b 4275 696c 645d 2868 7474 7073  ..![Build](https
-00000020: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-00000030: 6d63 2d6c 6162 732f 7079 6d63 2d6d 6172  mc-labs/pymc-mar
-00000040: 6b65 7469 6e67 2f77 6f72 6b66 6c6f 7773  keting/workflows
-00000050: 2f63 692f 6261 6467 652e 7376 6729 0a5b  /ci/badge.svg).[
-00000060: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
-00000070: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000080: 2f70 796d 632d 6c61 6273 2f70 796d 632d  /pymc-labs/pymc-
-00000090: 6d61 726b 6574 696e 672f 6272 616e 6368  marketing/branch
-000000a0: 2f6d 6169 6e2f 6772 6170 682f 6261 6467  /main/graph/badg
-000000b0: 652e 7376 673f 746f 6b65 6e3d 4f42 5633  e.svg?token=OBV3
-000000c0: 4253 3554 5945 295d 2868 7474 7073 3a2f  BS5TYE)](https:/
-000000d0: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f70  /codecov.io/gh/p
-000000e0: 796d 632d 6c61 6273 2f70 796d 632d 6d61  ymc-labs/pymc-ma
-000000f0: 726b 6574 696e 6729 0a5b 215b 646f 6373  rketing).[![docs
-00000100: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
-00000110: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
-00000120: 7473 2f70 796d 632d 6d61 726b 6574 696e  ts/pymc-marketin
-00000130: 672f 6261 6467 652f 3f76 6572 7369 6f6e  g/badge/?version
-00000140: 3d6c 6174 6573 7429 5d28 6874 7470 733a  =latest)](https:
-00000150: 2f2f 646f 6373 2e72 6561 6474 6865 646f  //docs.readthedo
-00000160: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00000170: 290a 5b21 5b43 6f64 6520 7374 796c 653a  ).[![Code style:
-00000180: 2062 6c61 636b 5d28 6874 7470 733a 2f2f   black](https://
-00000190: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-000001a0: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
-000001b0: 652d 626c 6163 6b2d 3030 3030 3030 2e73  e-black-000000.s
-000001c0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-000001d0: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
-000001e0: 6b29 0a5b 215b 5079 5049 2056 6572 7369  k).[![PyPI Versi
-000001f0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-00000200: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000210: 762f 7079 6d63 2d6d 6172 6b65 7469 6e67  v/pymc-marketing
-00000220: 2e73 7667 295d 2868 7474 7073 3a2f 2f70  .svg)](https://p
-00000230: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
-00000240: 7970 692f 7079 6d63 2d6d 6172 6b65 7469  ypi/pymc-marketi
-00000250: 6e67 290a 5b21 5b4c 6963 656e 7365 5d28  ng).[![License](
-00000260: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000270: 6c64 732e 696f 2f62 6164 6765 2f4c 6963  lds.io/badge/Lic
-00000280: 656e 7365 2d41 7061 6368 655f 322e 302d  ense-Apache_2.0-
-00000290: 626c 7565 2e73 7667 295d 2868 7474 7073  blue.svg)](https
-000002a0: 3a2f 2f6f 7065 6e73 6f75 7263 652e 6f72  ://opensource.or
-000002b0: 672f 6c69 6365 6e73 6573 2f41 7061 6368  g/licenses/Apach
-000002c0: 652d 322e 3029 0a0a 2a2a 556e 6c6f 636b  e-2.0)..**Unlock
-000002d0: 2074 6865 2070 6f77 6572 206f 6620 6d61   the power of ma
-000002e0: 726b 6574 696e 6720 616e 616c 7974 6963  rketing analytic
-000002f0: 7320 7769 7468 2050 794d 432d 4d61 726b  s with PyMC-Mark
-00000300: 6574 696e 6720 e280 9320 7468 6520 6f70  eting ... the op
-00000310: 656e 2073 6f75 7263 6520 736f 6c75 7469  en source soluti
-00000320: 6f6e 2066 6f72 2073 6d61 7274 6572 2064  on for smarter d
-00000330: 6563 6973 696f 6e2d 6d61 6b69 6e67 2e2a  ecision-making.*
-00000340: 2a20 4d65 6469 6120 6d69 7820 6d6f 6465  * Media mix mode
-00000350: 6c69 6e67 2061 6e64 2063 7573 746f 6d65  ling and custome
-00000360: 7220 6c69 6665 7469 6d65 2076 616c 7565  r lifetime value
-00000370: 206d 6f64 756c 6573 2061 6c6c 6f77 2062   modules allow b
-00000380: 7573 696e 6573 7365 7320 746f 206d 616b  usinesses to mak
-00000390: 6520 6461 7461 2d64 7269 7665 6e20 6465  e data-driven de
-000003a0: 6369 7369 6f6e 7320 6162 6f75 7420 7468  cisions about th
-000003b0: 6569 7220 6d61 726b 6574 696e 6720 6361  eir marketing ca
-000003c0: 6d70 6169 676e 732e 204f 7074 696d 697a  mpaigns. Optimiz
-000003d0: 6520 796f 7572 206d 6172 6b65 7469 6e67  e your marketing
-000003e0: 2073 7472 6174 6567 7920 616e 6420 756e   strategy and un
-000003f0: 6c6f 636b 2074 6865 2066 756c 6c20 706f  lock the full po
-00000400: 7465 6e74 6961 6c20 6f66 2079 6f75 7220  tential of your 
-00000410: 6375 7374 6f6d 6572 2064 6174 612e 0a0a  customer data...
-00000420: 2d2d 2d0a 0a23 2320 496e 7374 616c 6c61  ---..## Installa
-00000430: 7469 6f6e 0a0a 5374 6172 7420 6279 2073  tion..Start by s
-00000440: 6574 7469 6e67 2075 7020 616e 2065 6e76  etting up an env
-00000450: 6972 6f6e 6d65 6e74 2028 652e 672e 2060  ironment (e.g. `
-00000460: 6d61 726b 6574 696e 675f 656e 7660 2920  marketing_env`) 
-00000470: 7769 7468 2050 794d 432e 2049 7420 6d61  with PyMC. It ma
-00000480: 7920 6c6f 6f6b 2073 6f6d 6574 6869 6e67  y look something
-00000490: 206c 696b 6520 7468 6520 666f 6c6c 6f77   like the follow
-000004a0: 696e 673a 0a0a 6060 6062 6173 680a 6d61  ing:..```bash.ma
-000004b0: 6d62 6120 6372 6561 7465 202d 6320 636f  mba create -c co
-000004c0: 6e64 612d 666f 7267 6520 2d6e 206d 6172  nda-forge -n mar
-000004d0: 6b65 7469 6e67 5f65 6e76 2070 7974 686f  keting_env pytho
-000004e0: 6e20 2270 796d 633e 3d35 220a 6d61 6d62  n "pymc>=5".mamb
-000004f0: 6120 6163 7469 7661 7465 206d 6172 6b65  a activate marke
-00000500: 7469 6e67 5f65 6e76 0a60 6060 0a0a 5365  ting_env.```..Se
-00000510: 6520 7468 6520 6f66 6669 6369 616c 205b  e the official [
-00000520: 5079 4d43 2069 6e73 7461 6c6c 6174 696f  PyMC installatio
-00000530: 6e20 6775 6964 655d 2868 7474 7073 3a2f  n guide](https:/
-00000540: 2f77 7777 2e70 796d 632e 696f 2f70 726f  /www.pymc.io/pro
-00000550: 6a65 6374 732f 646f 6373 2f65 6e2f 6c61  jects/docs/en/la
-00000560: 7465 7374 2f69 6e73 7461 6c6c 6174 696f  test/installatio
-00000570: 6e2e 6874 6d6c 2920 6966 206d 6f72 6520  n.html) if more 
-00000580: 6465 7461 696c 2069 7320 6e65 6564 6564  detail is needed
-00000590: 2e0a 0a41 7373 756d 696e 6720 796f 7520  ...Assuming you 
-000005a0: 6861 7665 2061 6e20 656e 7669 726f 6e6d  have an environm
-000005b0: 656e 7420 7365 7420 7570 2074 6865 6e20  ent set up then 
-000005c0: 696e 7374 616c 6c20 5079 4d43 2d4d 6172  install PyMC-Mar
-000005d0: 6b65 7469 6e67 2077 6974 6820 7468 6520  keting with the 
-000005e0: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-000005f0: 642e 2054 6869 7320 7769 6c6c 2067 6976  d. This will giv
-00000600: 6520 796f 7520 7468 6520 6c61 7465 7374  e you the latest
-00000610: 2076 6572 7369 6f6e 206f 6620 7468 6520   version of the 
-00000620: 6c69 6272 6172 7920 6672 6f6d 2050 7950  library from PyP
-00000630: 492e 0a0a 6060 6062 6173 680a 7069 7020  I...```bash.pip 
-00000640: 696e 7374 616c 6c20 7079 6d63 2d6d 6172  install pymc-mar
-00000650: 6b65 7469 6e67 0a60 6060 0a0a 416c 7465  keting.```..Alte
-00000660: 726e 6174 6976 656c 7920 796f 7520 6361  rnatively you ca
-00000670: 6e20 696e 7374 616c 6c20 6672 6f6d 2047  n install from G
-00000680: 6974 4875 6220 6469 7265 6374 6c79 3a0a  itHub directly:.
-00000690: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
-000006a0: 7461 6c6c 2067 6974 2b68 7474 7073 3a2f  tall git+https:/
-000006b0: 2f67 6974 6875 622e 636f 6d2f 7079 6d63  /github.com/pymc
-000006c0: 2d6c 6162 732f 7079 6d63 2d6d 6172 6b65  -labs/pymc-marke
-000006d0: 7469 6e67 2e67 6974 0a60 6060 0a0a 2323  ting.git.```..##
-000006e0: 2042 6179 6573 6961 6e20 4d65 6469 6120   Bayesian Media 
-000006f0: 4d69 7820 4d6f 6465 6c73 2028 4d4d 4d73  Mix Models (MMMs
-00000700: 2920 696e 2050 794d 430a 0a49 6e20 7468  ) in PyMC..In th
-00000710: 6973 2070 6163 6b61 6765 2077 6520 7072  is package we pr
-00000720: 6f76 6964 6520 616e 2041 5049 2066 6f72  ovide an API for
-00000730: 2061 2042 6179 6573 6961 6e20 6d65 6469   a Bayesian medi
-00000740: 6120 6d69 7820 6d6f 6465 6c20 284d 4d4d  a mix model (MMM
-00000750: 2920 7370 6563 6966 6963 6174 696f 6e20  ) specification 
-00000760: 666f 6c6c 6f77 696e 6720 5b4a 696e 2c20  following [Jin, 
-00000770: 5975 7875 652c 2065 7420 616c 2e20 e280  Yuxue, et al. ..
-00000780: 9c42 6179 6573 6961 6e20 6d65 7468 6f64  .Bayesian method
-00000790: 7320 666f 7220 6d65 6469 6120 6d69 7820  s for media mix 
-000007a0: 6d6f 6465 6c69 6e67 2077 6974 6820 6361  modeling with ca
-000007b0: 7272 796f 7665 7220 616e 6420 7368 6170  rryover and shap
-000007c0: 6520 6566 6665 6374 732e e280 9d20 2832  e effects.... (2
-000007d0: 3031 3729 2e5d 2868 7474 7073 3a2f 2f72  017).](https://r
-000007e0: 6573 6561 7263 682e 676f 6f67 6c65 2f70  esearch.google/p
-000007f0: 7562 732f 7075 6234 3630 3031 2f29 2043  ubs/pub46001/) C
-00000800: 6f6e 6372 6574 656c 792c 2067 6976 656e  oncretely, given
-00000810: 2061 2074 696d 6520 7365 7269 6573 2074   a time series t
-00000820: 6172 6765 7420 7661 7269 6162 6c65 2024  arget variable $
-00000830: 795f 7b74 7d24 2028 652e 672e 2073 616c  y_{t}$ (e.g. sal
-00000840: 6573 206f 6e20 636f 6e76 6572 7369 6f6e  es on conversion
-00000850: 7329 2c20 6d65 6469 6120 7661 7269 6162  s), media variab
-00000860: 6c65 7320 2478 5f7b 6d2c 2074 7d24 2028  les $x_{m, t}$ (
-00000870: 652e 672e 2069 6d70 7265 7373 696f 6e73  e.g. impressions
-00000880: 2c20 636c 6963 6b73 206f 7220 636f 7374  , clicks or cost
-00000890: 7329 2061 6e64 2061 2073 6574 206f 6620  s) and a set of 
-000008a0: 636f 6e74 726f 6c20 636f 7661 7269 6174  control covariat
-000008b0: 6573 2024 7a5f 7b63 2c20 747d 2420 2865  es $z_{c, t}$ (e
-000008c0: 2e67 2e20 686f 6c69 6461 7973 2c20 7370  .g. holidays, sp
-000008d0: 6563 6961 6c20 6576 656e 7473 2920 7765  ecial events) we
-000008e0: 2063 6f6e 7369 6465 7220 6120 6c69 6e65   consider a line
-000008f0: 6172 206d 6f64 656c 206f 6620 7468 6520  ar model of the 
-00000900: 666f 726d 0a0a 2424 0a79 5f7b 747d 203d  form..$$.y_{t} =
-00000910: 205c 616c 7068 6120 2b20 5c73 756d 5f7b   \alpha + \sum_{
-00000920: 6d3d 317d 5e7b 4d7d 5c62 6574 615f 7b6d  m=1}^{M}\beta_{m
-00000930: 7d66 2878 5f7b 6d2c 2074 7d29 202b 2020  }f(x_{m, t}) +  
-00000940: 5c73 756d 5f7b 633d 317d 5e7b 437d 5c67  \sum_{c=1}^{C}\g
-00000950: 616d 6d61 5f7b 637d 7a5f 7b63 2c20 747d  amma_{c}z_{c, t}
-00000960: 202b 205c 7661 7265 7073 696c 6f6e 5f7b   + \varepsilon_{
-00000970: 747d 2c0a 2424 0a0a 7768 6572 6520 245c  t},.$$..where $\
-00000980: 616c 7068 6124 2069 7320 7468 6520 696e  alpha$ is the in
-00000990: 7465 7263 6570 742c 2024 6624 2069 7320  tercept, $f$ is 
-000009a0: 6120 6d65 6469 6120 7472 616e 7366 6f72  a media transfor
-000009b0: 6d61 7469 6f6e 2066 756e 6374 696f 6e20  mation function 
-000009c0: 616e 6420 245c 7661 7265 7073 696c 6f6e  and $\varepsilon
-000009d0: 5f7b 747d 2420 6973 2074 6865 2065 7272  _{t}$ is the err
-000009e0: 6f72 2074 6865 726d 2077 6869 6368 2077  or therm which w
-000009f0: 6520 6173 7375 6d65 2069 7320 6e6f 726d  e assume is norm
-00000a00: 616c 6c79 2064 6973 7472 6962 7574 6564  ally distributed
-00000a10: 2e20 5468 6520 6675 6e63 7469 6f6e 2024  . The function $
-00000a20: 6624 2065 6e63 6f64 6573 2074 6865 2063  f$ encodes the c
-00000a30: 6f6e 7472 6962 7574 696f 6e20 6f66 206d  ontribution of m
-00000a40: 6564 6961 206f 6e20 7468 6520 7461 7267  edia on the targ
-00000a50: 6574 2076 6172 6961 626c 652e 2054 7970  et variable. Typ
-00000a60: 6963 616c 6c79 2077 6520 636f 6e73 6964  ically we consid
-00000a70: 6572 2074 776f 2074 7970 6573 206f 6620  er two types of 
-00000a80: 7472 616e 7366 6f72 6d61 7469 6f6e 3a20  transformation: 
-00000a90: 6164 7374 6f63 6b20 2863 6172 7279 2d6f  adstock (carry-o
-00000aa0: 7665 7229 2061 6e64 2073 6174 7572 6174  ver) and saturat
-00000ab0: 696f 6e20 6566 6665 6374 732e 0a0a 5b48  ion effects...[H
-00000ac0: 6572 655d 2868 7474 7073 3a2f 2f70 796d  ere](https://pym
-00000ad0: 632d 6d61 726b 6574 696e 672e 7265 6164  c-marketing.read
-00000ae0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-00000af0: 6162 6c65 2f6e 6f74 6562 6f6f 6b73 2f6d  able/notebooks/m
-00000b00: 6d6d 2f6d 6d6d 5f65 7861 6d70 6c65 2e68  mm/mmm_example.h
-00000b10: 746d 6c29 2079 6f75 2063 616e 2066 696e  tml) you can fin
-00000b20: 6420 6120 7369 6d75 6c61 7465 6420 6578  d a simulated ex
-00000b30: 616d 706c 653a 0a0a 312e 2046 6972 7374  ample:..1. First
-00000b40: 2c20 7765 2064 6573 6372 6962 6520 7468  , we describe th
-00000b50: 6520 6461 7461 2067 656e 6172 6174 696f  e data genaratio
-00000b60: 6e20 7072 6f63 6573 7320 6f66 2061 2073  n process of a s
-00000b70: 696d 756c 6174 6564 2064 6174 6173 6574  imulated dataset
-00000b80: 2e0a 322e 204e 6578 742c 2077 6520 6465  ..2. Next, we de
-00000b90: 7363 7269 6265 2068 6f77 2074 6f20 7370  scribe how to sp
-00000ba0: 6563 6966 7920 616e 6420 6669 7420 6120  ecify and fit a 
-00000bb0: 6d65 6469 6120 6d69 7820 6d6f 6465 6c20  media mix model 
-00000bc0: 2861 7320 6465 7363 7269 6265 6420 6162  (as described ab
-00000bd0: 6f76 6529 2075 7369 6e67 2074 6865 2060  ove) using the `
-00000be0: 7079 6d63 2d6d 6172 6b65 7469 6e67 6020  pymc-marketing` 
-00000bf0: 4d4d 4d27 7320 4150 492e 0a33 2e20 4669  MMM's API..3. Fi
-00000c00: 6e61 6c6c 792c 2077 6520 6465 7363 7269  nally, we descri
-00000c10: 6265 2074 6865 206d 6f64 656c 2072 6573  be the model res
-00000c20: 756c 7473 3a20 6368 616e 6e65 6c20 636f  ults: channel co
-00000c30: 6e73 7472 6962 7574 696f 6e20 616e 6420  nstribution and 
-00000c40: 524f 4153 2065 7374 696d 6174 696f 6e2e  ROAS estimation.
-00000c50: 2057 6520 616c 736f 2073 686f 7720 686f   We also show ho
-00000c60: 7720 7468 6520 6d6f 6465 6c20 7265 636f  w the model reco
-00000c70: 7665 7273 2074 6865 2070 6172 616d 6574  vers the paramet
-00000c80: 6572 7320 6672 6f6d 2074 6865 2064 6174  ers from the dat
-00000c90: 6120 6765 6e65 7261 7469 6f6e 2070 726f  a generation pro
-00000ca0: 6365 7373 2073 7465 702e 0a0a 2323 2320  cess step...### 
-00000cb0: 5265 6665 7265 6e63 6573 3a0a 0a2d 205b  References:..- [
-00000cc0: 4a69 6e2c 2059 7578 7565 2c20 6574 2061  Jin, Yuxue, et a
-00000cd0: 6c2e 20e2 809c 4261 7965 7369 616e 206d  l. ...Bayesian m
-00000ce0: 6574 686f 6473 2066 6f72 206d 6564 6961  ethods for media
-00000cf0: 206d 6978 206d 6f64 656c 696e 6720 7769   mix modeling wi
-00000d00: 7468 2063 6172 7279 6f76 6572 2061 6e64  th carryover and
-00000d10: 2073 6861 7065 2065 6666 6563 7473 2ee2   shape effects..
-00000d20: 809d 2028 3230 3137 292e 5d28 6874 7470  .. (2017).](http
-00000d30: 733a 2f2f 7265 7365 6172 6368 2e67 6f6f  s://research.goo
-00000d40: 676c 652f 7075 6273 2f70 7562 3436 3030  gle/pubs/pub4600
-00000d50: 312f 290a 2d20 5079 4d43 204c 6162 7320  1/).- PyMC Labs 
-00000d60: 426c 6f67 3a0a 2020 2d20 5b42 6179 6573  Blog:.  - [Bayes
-00000d70: 6961 6e20 4d65 6469 6120 4d69 7820 4d6f  ian Media Mix Mo
-00000d80: 6465 6c69 6e67 2066 6f72 204d 6172 6b65  deling for Marke
-00000d90: 7469 6e67 204f 7074 696d 697a 6174 696f  ting Optimizatio
-00000da0: 6e5d 2868 7474 7073 3a2f 2f77 7777 2e70  n](https://www.p
-00000db0: 796d 632d 6c61 6273 2e69 6f2f 626c 6f67  ymc-labs.io/blog
-00000dc0: 2d70 6f73 7473 2f62 6179 6573 6961 6e2d  -posts/bayesian-
-00000dd0: 6d65 6469 612d 6d69 782d 6d6f 6465 6c69  media-mix-modeli
-00000de0: 6e67 2d66 6f72 2d6d 6172 6b65 7469 6e67  ng-for-marketing
-00000df0: 2d6f 7074 696d 697a 6174 696f 6e2f 290a  -optimization/).
-00000e00: 2020 2d20 5b49 6d70 726f 7669 6e67 2074    - [Improving t
-00000e10: 6865 2053 7065 6564 2061 6e64 2041 6363  he Speed and Acc
-00000e20: 7572 6163 7920 6f66 2042 6179 6573 6961  uracy of Bayesia
-00000e30: 6e20 4d65 6469 6120 4d69 7820 4d6f 6465  n Media Mix Mode
-00000e40: 6c73 5d28 6874 7470 733a 2f2f 7777 772e  ls](https://www.
-00000e50: 7079 6d63 2d6c 6162 732e 696f 2f62 6c6f  pymc-labs.io/blo
-00000e60: 672d 706f 7374 732f 7265 6475 6369 6e67  g-posts/reducing
-00000e70: 2d63 7573 746f 6d65 722d 6163 7175 6973  -customer-acquis
-00000e80: 6974 696f 6e2d 636f 7374 732d 686f 772d  ition-costs-how-
-00000e90: 7765 2d68 656c 7065 642d 6f70 7469 6d69  we-helped-optimi
-00000ea0: 7a69 6e67 2d68 656c 6c6f 6672 6573 6873  zing-hellofreshs
-00000eb0: 2d6d 6172 6b65 7469 6e67 2d62 7564 6765  -marketing-budge
-00000ec0: 742f 290a 2d20 5b4a 6f68 6e73 2c20 4d69  t/).- [Johns, Mi
-00000ed0: 6368 6165 6c20 616e 6420 5761 6e67 2c20  chael and Wang, 
-00000ee0: 205a 6865 6e79 752e 2022 4120 4261 7965   Zhenyu. "A Baye
-00000ef0: 7369 616e 2041 7070 726f 6163 6820 746f  sian Approach to
-00000f00: 204d 6564 6961 204d 6978 204d 6f64 656c   Media Mix Model
-00000f10: 696e 6722 5d28 6874 7470 733a 2f2f 7777  ing"](https://ww
-00000f20: 772e 796f 7574 7562 652e 636f 6d2f 7761  w.youtube.com/wa
-00000f30: 7463 683f 763d 557a 6e4d 5f2d 5f37 3630  tch?v=UznM_-_760
-00000f40: 5929 0a2d 205b 4f72 6475 7a2c 204a 7561  Y).- [Orduz, Jua
-00000f50: 6e2e 2022 4d65 6469 6120 4566 6665 6374  n. "Media Effect
-00000f60: 2045 7374 696d 6174 696f 6e20 7769 7468   Estimation with
-00000f70: 2050 794d 433a 2041 6473 746f 636b 2c20   PyMC: Adstock, 
-00000f80: 5361 7475 7261 7469 6f6e 2026 2044 696d  Saturation & Dim
-00000f90: 696e 6973 6869 6e67 2052 6574 7572 6e73  inishing Returns
-00000fa0: 225d 2868 7474 7073 3a2f 2f6a 7561 6e69  "](https://juani
-00000fb0: 746f 7264 757a 2e67 6974 6875 622e 696f  torduz.github.io
-00000fc0: 2f70 796d 635f 6d6d 6d2f 290a 0a2d 2d2d  /pymc_mmm/)..---
-00000fd0: 0a0a 2323 2042 6179 6573 6961 6e20 434c  ..## Bayesian CL
-00000fe0: 5673 2069 6e20 5079 4d43 0a5b 4375 7374  Vs in PyMC.[Cust
-00000ff0: 6f6d 6572 204c 6966 6574 696d 6520 5661  omer Lifetime Va
-00001000: 6c75 655d 2868 7474 7073 3a2f 2f65 6e2e  lue](https://en.
-00001010: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-00001020: 6b69 2f43 7573 746f 6d65 725f 6c69 6665  ki/Customer_life
-00001030: 7469 6d65 5f76 616c 7565 2920 2843 4c56  time_value) (CLV
-00001040: 2920 6d6f 6465 6c73 2061 7265 2061 6e6f  ) models are ano
-00001050: 7468 6572 2069 6d70 6f72 7461 6e74 2063  ther important c
-00001060: 6c61 7373 206f 6620 6d6f 6465 6c73 2e20  lass of models. 
-00001070: 5468 6572 6520 6172 6520 6d61 6e79 2064  There are many d
-00001080: 6966 6665 7265 6e74 2074 7970 6573 206f  ifferent types o
-00001090: 6620 434c 5620 6d6f 6465 6c73 2061 6e64  f CLV models and
-000010a0: 2069 7420 6361 6e20 6265 2068 656c 7066   it can be helpf
-000010b0: 756c 2074 6f20 636f 6e63 6570 7475 616c  ul to conceptual
-000010c0: 6973 6520 7468 656d 2061 7320 6669 7474  ise them as fitt
-000010d0: 696e 6720 696e 2061 2032 2d64 696d 656e  ing in a 2-dimen
-000010e0: 7369 6f6e 616c 2067 7269 6420 6173 2062  sional grid as b
-000010f0: 656c 6f77 2e20 416e 2065 7863 656c 6c65  elow. An excelle
-00001100: 6e74 2073 6574 206f 6620 696e 7472 6f64  nt set of introd
-00001110: 7563 7469 6f6e 2073 6c69 6465 7320 746f  uction slides to
-00001120: 2043 4c56 2773 2069 7320 7072 6f76 6964   CLV's is provid
-00001130: 6564 2069 6e20 5b50 726f 6261 6269 6c69  ed in [Probabili
-00001140: 7479 204d 6f64 656c 7320 666f 7220 4375  ty Models for Cu
-00001150: 7374 6f6d 6572 2d42 6173 6520 416e 616c  stomer-Base Anal
-00001160: 7973 6973 5d28 6874 7470 733a 2f2f 7777  ysis](https://ww
-00001170: 772e 6272 7563 6568 6172 6469 652e 636f  w.brucehardie.co
-00001180: 6d2f 7461 6c6b 732f 686f 5f63 6261 5f74  m/talks/ho_cba_t
-00001190: 7574 5f61 7274 5f30 392e 7064 6629 2062  ut_art_09.pdf) b
-000011a0: 7920 4661 6465 7220 2620 4861 7264 6965  y Fader & Hardie
-000011b0: 2028 3230 3039 292e 0a0a 2323 2320 4578   (2009)...### Ex
-000011c0: 616d 706c 6573 0a0a 7c20 2020 2020 2020  amples..|       
-000011d0: 2020 2020 2020 2020 207c 202a 2a4e 6f6e           | **Non
-000011e0: 2d63 6f6e 7472 6163 7475 616c 2a2a 207c  -contractual** |
-000011f0: 202a 2a43 6f6e 7472 6163 7475 616c 2a2a   **Contractual**
-00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001210: 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.|------------
-00001220: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
-00001230: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-00001240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
-00001260: 2a2a 436f 6e74 696e 756f 7573 2a2a 207c  **Continuous** |
-00001270: 2042 7579 696e 6720 6772 6f63 6572 6965   Buying grocerie
-00001280: 7320 2020 207c 2041 7564 6962 6c65 2020  s    | Audible  
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 2020 2020 2020 207c 0a7c 202a 2a44 6973         |.| **Dis
-000012b0: 6372 6574 652a 2a20 2020 7c20 4369 6e65  crete**   | Cine
-000012c0: 6d61 2074 6963 6b65 7420 2020 2020 2020  ma ticket       
-000012d0: 7c20 4d6f 6e74 686c 7920 6f72 2079 6561  | Monthly or yea
-000012e0: 726c 7920 7375 6273 6372 6970 7469 6f6e  rly subscription
-000012f0: 7320 7c0a 0a54 6f20 6578 706c 6169 6e20  s |..To explain 
-00001300: 6675 7274 6865 723a 0a2d 202a 2a43 6f6e  further:.- **Con
-00001310: 7472 6163 7475 616c 3a2a 2a20 496e 2063  tractual:** In c
-00001320: 6f6e 7472 6163 7475 616c 2073 6574 7469  ontractual setti
-00001330: 6e67 732c 2061 2063 7573 746f 6d65 7220  ngs, a customer 
-00001340: 6861 7320 6120 636f 6e74 7261 6374 2077  has a contract w
-00001350: 6869 6368 2063 6f6e 7469 6e75 6573 2074  hich continues t
-00001360: 6f20 6265 2061 6374 6976 6520 756e 7469  o be active unti
-00001370: 6c20 6974 2069 7320 6578 706c 6963 6974  l it is explicit
-00001380: 6c79 2063 616e 6365 6c6c 6564 2e20 5468  ly cancelled. Th
-00001390: 6572 6566 6f72 652c 2063 7573 746f 6d65  erefore, custome
-000013a0: 7220 6368 7572 6e20 6576 656e 7473 2061  r churn events a
-000013b0: 7265 206f 6273 6572 7665 642e 0a0a 2d20  re observed...- 
-000013c0: 2a2a 4e6f 6e2d 636f 6e74 7261 6374 7561  **Non-contractua
-000013d0: 6c3a 2a2a 2049 6e20 6e6f 6e2d 636f 6e74  l:** In non-cont
-000013e0: 7261 6374 7561 6c20 7365 7474 696e 6773  ractual settings
-000013f0: 2c20 7468 6572 6520 6973 206e 6f20 6f6e  , there is no on
-00001400: 676f 696e 6720 636f 6e74 7261 6374 2074  going contract t
-00001410: 6861 7420 6120 6375 7374 6f6d 6572 2068  hat a customer h
-00001420: 6173 2077 6974 6820 6120 636f 6d70 616e  as with a compan
-00001430: 792e 2049 6e73 7465 6164 2c20 7075 7263  y. Instead, purc
-00001440: 6861 7365 7320 6361 6e20 6265 2061 6420  hases can be ad 
-00001450: 686f 6320 616e 6420 6368 7572 6e20 6576  hoc and churn ev
-00001460: 656e 7473 2061 7265 2075 6e6f 6273 6572  ents are unobser
-00001470: 7665 642e 0a0a 2d20 2a2a 4469 7363 7265  ved...- **Discre
-00001480: 7465 3a2a 2a20 4865 7265 2c20 7075 7263  te:** Here, purc
-00001490: 6861 7365 7320 6172 6520 6d61 6465 2061  hases are made a
-000014a0: 7420 6469 7363 7265 7465 2070 6f69 6e74  t discrete point
-000014b0: 7320 696e 2074 696d 652e 2054 6869 7320  s in time. This 
-000014c0: 6f62 7669 6f75 736c 7920 6465 7065 6e64  obviously depend
-000014d0: 7320 7570 6f6e 2074 6865 2074 696d 6573  s upon the times
-000014e0: 6361 6c65 2074 6861 7420 7765 2061 7265  cale that we are
-000014f0: 2077 6f72 6b69 6e67 206f 6e2c 2062 7574   working on, but
-00001500: 2074 7970 6963 616c 6c79 2061 2072 656c   typically a rel
-00001510: 6576 616e 7420 7469 6d65 2070 6572 696f  evant time perio
-00001520: 6420 776f 756c 6420 6265 2061 206d 6f6e  d would be a mon
-00001530: 7468 206f 7220 7965 6172 2e20 486f 7765  th or year. Howe
-00001540: 7665 7220 6974 2063 6f75 6c64 2062 6520  ver it could be 
-00001550: 6d6f 7265 2067 7261 6e75 616c 6172 2074  more granualar t
-00001560: 6861 6e20 7468 6973 202d 2074 6869 6e6b  han this - think
-00001570: 206f 6620 7461 6b69 6e67 2074 6865 2032   of taking the 2
-00001580: 6e64 206f 6620 3420 696e 7465 722d 6369  nd of 4 inter-ci
-00001590: 7479 2074 7261 696e 206a 6f75 726e 6579  ty train journey
-000015a0: 7320 6f66 6665 7265 6420 7065 7220 6461  s offered per da
-000015b0: 792e 0a0a 2d20 2a2a 436f 6e74 696e 756f  y...- **Continuo
-000015c0: 7573 3a2a 2a20 496e 2074 6865 2063 6f6e  us:** In the con
-000015d0: 7469 6e75 6f75 732d 7469 6d65 2064 6f6d  tinuous-time dom
-000015e0: 6169 6e2c 2070 7572 6368 6173 6573 2063  ain, purchases c
-000015f0: 616e 2062 6520 6d61 6465 2061 7420 616e  an be made at an
-00001600: 7920 706f 696e 7420 7769 7468 696e 2061  y point within a
-00001610: 2066 6972 6d73 206f 7065 6e69 6e67 2068   firms opening h
-00001620: 6f75 7273 2e20 466f 7220 6f6e 6c69 6e65  ours. For online
-00001630: 206f 7264 6572 696e 672c 2074 6869 7320   ordering, this 
-00001640: 636f 756c 6420 6265 2061 6e79 2070 6f69  could be any poi
-00001650: 6e74 2077 6974 6869 6e20 6120 3234 2068  nt within a 24 h
-00001660: 6f75 7220 6379 636c 652c 206f 7220 7075  our cycle, or pu
-00001670: 7263 6861 7365 7320 696e 2070 6879 7369  rchases in physi
-00001680: 6361 6c20 7374 6f72 6573 2063 6f75 6c64  cal stores could
-00001690: 2062 6520 6d61 6465 2061 7420 616e 7920   be made at any 
-000016a0: 706f 696e 7420 6475 7269 6e67 2074 6865  point during the
-000016b0: 2074 7261 6469 6e67 2064 6179 2e0a 0a49   trading day...I
-000016c0: 6e20 7468 6520 646f 6375 6d65 6e74 6174  n the documentat
-000016d0: 696f 6e2c 2077 6520 7072 6f76 6964 6520  ion, we provide 
-000016e0: 736f 6d65 2065 7861 6d70 6c65 7320 6f6e  some examples on
-000016f0: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
-00001700: 434c 5620 4150 492e 2057 6520 7573 6520  CLV API. We use 
-00001710: 7468 6520 6461 7461 2066 726f 6d20 7468  the data from th
-00001720: 6520 5b60 6c69 6665 7469 6d65 7360 5d28  e [`lifetimes`](
-00001730: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001740: 6f6d 2f43 616d 4461 7669 6473 6f6e 5069  om/CamDavidsonPi
-00001750: 6c6f 6e2f 6c69 6665 7469 6d65 7329 2070  lon/lifetimes) p
-00001760: 6163 6b61 6765 2074 6f20 696c 6c75 7374  ackage to illust
-00001770: 7261 7465 2074 6865 206d 6f64 656c 732e  rate the models.
-00001780: 0a0a 2d20 5b43 4c56 2051 7569 636b 7374  ..- [CLV Quickst
-00001790: 6172 745d 2868 7474 7073 3a2f 2f70 796d  art](https://pym
-000017a0: 632d 6d61 726b 6574 696e 672e 7265 6164  c-marketing.read
-000017b0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-000017c0: 6162 6c65 2f6e 6f74 6562 6f6f 6b73 2f63  able/notebooks/c
-000017d0: 6c76 2f63 6c76 5f71 7569 636b 7374 6172  lv/clv_quickstar
-000017e0: 742e 6874 6d6c 290a 2d20 5b42 472f 4e42  t.html).- [BG/NB
-000017f0: 4420 6d6f 6465 6c5d 2868 7474 7073 3a2f  D model](https:/
-00001800: 2f70 796d 632d 6d61 726b 6574 696e 672e  /pymc-marketing.
-00001810: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00001820: 6e2f 7374 6162 6c65 2f6e 6f74 6562 6f6f  n/stable/noteboo
-00001830: 6b73 2f63 6c76 2f62 675f 6e62 642e 6874  ks/clv/bg_nbd.ht
-00001840: 6d6c 290a 2d20 5b47 616d 6d61 2d47 616d  ml).- [Gamma-Gam
-00001850: 6d61 206d 6f64 656c 5d28 6874 7470 733a  ma model](https:
-00001860: 2f2f 7079 6d63 2d6d 6172 6b65 7469 6e67  //pymc-marketing
-00001870: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00001880: 656e 2f73 7461 626c 652f 6e6f 7465 626f  en/stable/notebo
-00001890: 6f6b 732f 636c 762f 6761 6d6d 615f 6761  oks/clv/gamma_ga
-000018a0: 6d6d 612e 6874 6d6c 290a 0a2d 2d2d 0a0a  mma.html)..---..
-000018b0: 2323 20f0 9f93 9e20 5363 6865 6475 6c65  ## .... Schedule
-000018c0: 2061 2043 6f6e 7375 6c74 6174 696f 6e0a   a Consultation.
-000018d0: 556e 6c6f 636b 2079 6f75 7220 706f 7465  Unlock your pote
-000018e0: 6e74 6961 6c20 7769 7468 2061 2066 7265  ntial with a fre
-000018f0: 6520 3330 2d6d 696e 7574 6520 7374 7261  e 30-minute stra
-00001900: 7465 6779 2073 6573 7369 6f6e 2077 6974  tegy session wit
-00001910: 6820 6f75 7220 5079 4d43 2065 7870 6572  h our PyMC exper
-00001920: 7473 2e20 4469 7363 6f76 6572 2068 6f77  ts. Discover how
-00001930: 206f 7065 6e20 736f 7572 6365 2073 6f6c   open source sol
-00001940: 7574 696f 6e73 2061 6e64 2070 796d 632d  utions and pymc-
-00001950: 6d61 726b 6574 696e 6720 6361 6e20 656c  marketing can el
-00001960: 6576 6174 6520 796f 7572 206d 6564 6961  evate your media
-00001970: 2d6d 6978 206d 6f64 656c 7320 616e 6420  -mix models and 
-00001980: 6375 7374 6f6d 6572 206c 6966 6574 696d  customer lifetim
-00001990: 6520 7661 6c75 6520 616e 616c 7973 6573  e value analyses
-000019a0: 2e20 426f 6f73 7420 796f 7572 2063 6172  . Boost your car
-000019b0: 6565 7220 616e 6420 6f72 6761 6e69 7a61  eer and organiza
-000019c0: 7469 6f6e 2062 7920 6d61 6b69 6e67 2073  tion by making s
-000019d0: 6d61 7274 6572 2c20 6461 7461 2d64 7269  marter, data-dri
-000019e0: 7665 6e20 6465 6369 7369 6f6e 732e 2044  ven decisions. D
-000019f0: 6f6e 2774 2077 6169 74e2 8094 5b63 6c61  on't wait...[cla
-00001a00: 696d 2079 6f75 7220 636f 6d70 6c69 6d65  im your complime
-00001a10: 6e74 6172 7920 7365 7373 696f 6e5d 2868  ntary session](h
-00001a20: 7474 7073 3a2f 2f63 616c 656e 646c 792e  ttps://calendly.
-00001a30: 636f 6d2f 6265 6e6a 616d 696e 2d76 696e  com/benjamin-vin
-00001a40: 6365 6e74 2f70 796d 632d 6d61 726b 6574  cent/pymc-market
-00001a50: 696e 6729 2074 6f64 6179 2061 6e64 206c  ing) today and l
-00001a60: 6561 6420 7468 6520 7761 7920 696e 206d  ead the way in m
-00001a70: 6172 6b65 7469 6e67 2061 6e64 2064 6174  arketing and dat
-00001a80: 6120 7363 6965 6e63 6520 696e 6e6f 7661  a science innova
-00001a90: 7469 6f6e 2e0a 0a23 2320 5573 696e 6720  tion...## Using 
-00001aa0: 5079 4d43 2d4d 6172 6b65 7469 6e67 2061  PyMC-Marketing a
-00001ab0: 6e64 2068 6f77 2050 794d 4320 4c61 6273  nd how PyMC Labs
-00001ac0: 2063 616e 2068 656c 7020 796f 750a 5079   can help you.Py
-00001ad0: 4d43 2d4d 6172 6b65 7469 6e67 2075 7365  MC-Marketing use
-00001ae0: 7320 7468 6520 5b41 7061 6368 6520 322e  s the [Apache 2.
-00001af0: 3020 6c69 6365 6e63 655d 284c 4943 454e  0 licence](LICEN
-00001b00: 5345 2920 7768 6963 6820 7065 726d 6974  SE) which permit
-00001b10: 7320 636f 6d6d 6572 6369 616c 2075 7365  s commercial use
-00001b20: 2c20 616d 6f6e 6773 7420 6f74 6865 7220  , amongst other 
-00001b30: 7468 696e 6773 2e0a 0a49 6620 796f 7520  things...If you 
-00001b40: 7761 6e74 2074 6f20 6275 696c 6420 7570  want to build up
-00001b50: 6f6e 2074 6865 2070 6163 6b61 6765 2c20  on the package, 
-00001b60: 706c 6561 7365 2066 6565 6c20 6672 6565  please feel free
-00001b70: 2074 6f20 666f 726b 2074 6865 2072 6570   to fork the rep
-00001b80: 6f20 616e 6420 7375 626d 6974 2061 2070  o and submit a p
-00001b90: 756c 6c20 7265 7175 6573 742e 2049 6620  ull request. If 
-00001ba0: 696e 2064 6f75 6274 2c20 706c 6561 7365  in doubt, please
-00001bb0: 206f 7065 6e20 616e 2069 7373 7565 2e0a   open an issue..
-00001bc0: 0a46 6f72 2063 6f6d 7061 6e69 6573 2074  .For companies t
-00001bd0: 6861 7420 7761 6e74 2074 6f20 7573 6520  hat want to use 
-00001be0: 5079 4d43 2d4d 6172 6b65 7469 6e67 2069  PyMC-Marketing i
-00001bf0: 6e20 7072 6f64 7563 7469 6f6e 2c20 5b50  n production, [P
-00001c00: 794d 4320 4c61 6273 5d28 6874 7470 733a  yMC Labs](https:
-00001c10: 2f2f 7777 772e 7079 6d63 2d6c 6162 732e  //www.pymc-labs.
-00001c20: 696f 2920 6973 2061 7661 696c 6162 6c65  io) is available
-00001c30: 2066 6f72 2063 6f6e 7375 6c74 696e 6720   for consulting 
-00001c40: 616e 6420 7472 6169 6e69 6e67 2e20 5765  and training. We
-00001c50: 2063 616e 2068 656c 7020 796f 7520 6275   can help you bu
-00001c60: 696c 6420 616e 6420 6465 706c 6f79 2079  ild and deploy y
-00001c70: 6f75 7220 6d6f 6465 6c73 2069 6e20 7072  our models in pr
-00001c80: 6f64 7563 7469 6f6e 2e20 5765 2068 6176  oduction. We hav
-00001c90: 6520 6578 7065 7269 656e 6365 2077 6974  e experience wit
-00001ca0: 6820 6375 7474 696e 6720 6564 6765 2042  h cutting edge B
-00001cb0: 6179 6573 6961 6e20 6d6f 6465 6c6c 696e  ayesian modellin
-00001cc0: 6720 7465 6368 6e69 7175 6573 2069 6e20  g techniques in 
-00001cd0: 6765 6e65 7261 6c2c 2061 6e64 2069 6e20  general, and in 
-00001ce0: 7061 7274 6963 756c 6172 2077 6974 6820  particular with 
-00001cf0: 4d4d 4d73 2061 6e64 2043 4c56 732e 2046  MMMs and CLVs. F
-00001d00: 6f72 2065 7861 6d70 6c65 2c20 7365 6520  or example, see 
-00001d10: 6f75 7220 7669 6465 6f20 6f6e 205b 4261  our video on [Ba
-00001d20: 7965 7369 616e 204d 6172 6b65 7469 6e67  yesian Marketing
-00001d30: 204d 6978 204d 6f64 656c 733a 2053 7461   Mix Models: Sta
-00001d40: 7465 206f 6620 7468 6520 4172 7420 616e  te of the Art an
-00001d50: 6420 7468 6569 7220 4675 7475 7265 5d28  d their Future](
-00001d60: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
-00001d70: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
-00001d80: 7856 7839 3170 7243 3831 6729 2e0a       xVx91prC81g)..
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a20 203c 6120 6872 6566 3d22  er">.  <a href="
+00000020: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000030: 6f6d 2f70 796d 632d 6c61 6273 2f70 796d  om/pymc-labs/pym
+00000040: 632d 6d61 726b 6574 696e 6722 3e3c 696d  c-marketing"><im
+00000050: 6720 6865 6967 6874 3d22 3234 3070 7822  g height="240px"
+00000060: 2073 7263 3d22 646f 6373 2f73 6f75 7263   src="docs/sourc
+00000070: 652f 5f73 7461 7469 632f 6d61 726b 6574  e/_static/market
+00000080: 696e 672d 6c6f 676f 2d6c 6967 6874 2e6a  ing-logo-light.j
+00000090: 7067 223e 3c2f 613e 0a3c 2f64 6976 3e0a  pg"></a>.</div>.
+000000a0: 0a2d 2d2d 2d0a 0a21 5b42 7569 6c64 5d28  .----..![Build](
+000000b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000c0: 6f6d 2f70 796d 632d 6c61 6273 2f70 796d  om/pymc-labs/pym
+000000d0: 632d 6d61 726b 6574 696e 672f 776f 726b  c-marketing/work
+000000e0: 666c 6f77 732f 6369 2f62 6164 6765 2e73  flows/ci/badge.s
+000000f0: 7667 290a 5b21 5b63 6f64 6563 6f76 5d28  vg).[![codecov](
+00000100: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00000110: 696f 2f67 682f 7079 6d63 2d6c 6162 732f  io/gh/pymc-labs/
+00000120: 7079 6d63 2d6d 6172 6b65 7469 6e67 2f62  pymc-marketing/b
+00000130: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
+00000140: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+00000150: 3d4f 4256 3342 5335 5459 4529 5d28 6874  =OBV3BS5TYE)](ht
+00000160: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000170: 2f67 682f 7079 6d63 2d6c 6162 732f 7079  /gh/pymc-labs/py
+00000180: 6d63 2d6d 6172 6b65 7469 6e67 290a 5b21  mc-marketing).[!
+00000190: 5b64 6f63 735d 2868 7474 7073 3a2f 2f72  [docs](https://r
+000001a0: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
+000001b0: 726f 6a65 6374 732f 7079 6d63 2d6d 6172  rojects/pymc-mar
+000001c0: 6b65 7469 6e67 2f62 6164 6765 2f3f 7665  keting/badge/?ve
+000001d0: 7273 696f 6e3d 6c61 7465 7374 295d 2868  rsion=latest)](h
+000001e0: 7474 7073 3a2f 2f64 6f63 732e 7265 6164  ttps://docs.read
+000001f0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000200: 7465 7374 2f29 0a5b 215b 436f 6465 2073  test/).[![Code s
+00000210: 7479 6c65 3a20 626c 6163 6b5d 2868 7474  tyle: black](htt
+00000220: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000230: 2e69 6f2f 6261 6467 652f 636f 6465 2532  .io/badge/code%2
+00000240: 3073 7479 6c65 2d62 6c61 636b 2d30 3030  0style-black-000
+00000250: 3030 302e 7376 6729 5d28 6874 7470 733a  000.svg)](https:
+00000260: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
+00000270: 2f62 6c61 636b 290a 5b21 5b50 7950 4920  /black).[![PyPI 
+00000280: 5665 7273 696f 6e5d 2868 7474 7073 3a2f  Version](https:/
+00000290: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000002a0: 7079 7069 2f76 2f70 796d 632d 6d61 726b  pypi/v/pymc-mark
+000002b0: 6574 696e 672e 7376 6729 5d28 6874 7470  eting.svg)](http
+000002c0: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+000002d0: 6f72 672f 7079 7069 2f70 796d 632d 6d61  org/pypi/pymc-ma
+000002e0: 726b 6574 696e 6729 0a5b 215b 4c69 6365  rketing).[![Lice
+000002f0: 6e73 655d 2868 7474 7073 3a2f 2f69 6d67  nse](https://img
+00000300: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000310: 652f 4c69 6365 6e73 652d 4170 6163 6865  e/License-Apache
+00000320: 5f32 2e30 2d62 6c75 652e 7376 6729 5d28  _2.0-blue.svg)](
+00000330: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00000340: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
+00000350: 4170 6163 6865 2d32 2e30 290a 0a23 2050  Apache-2.0)..# P
+00000360: 794d 432d 4d61 726b 6574 696e 670a 0a2a  yMC-Marketing..*
+00000370: 2a55 6e6c 6f63 6b20 7468 6520 706f 7765  *Unlock the powe
+00000380: 7220 6f66 206d 6172 6b65 7469 6e67 2061  r of marketing a
+00000390: 6e61 6c79 7469 6373 2077 6974 6820 5079  nalytics with Py
+000003a0: 4d43 2d4d 6172 6b65 7469 6e67 20e2 8093  MC-Marketing ...
+000003b0: 2074 6865 206f 7065 6e20 736f 7572 6365   the open source
+000003c0: 2073 6f6c 7574 696f 6e20 666f 7220 736d   solution for sm
+000003d0: 6172 7465 7220 6465 6369 7369 6f6e 2d6d  arter decision-m
+000003e0: 616b 696e 672e 2a2a 204d 6564 6961 206d  aking.** Media m
+000003f0: 6978 206d 6f64 656c 696e 6720 616e 6420  ix modeling and 
+00000400: 6375 7374 6f6d 6572 206c 6966 6574 696d  customer lifetim
+00000410: 6520 7661 6c75 6520 6d6f 6475 6c65 7320  e value modules 
+00000420: 616c 6c6f 7720 6275 7369 6e65 7373 6573  allow businesses
+00000430: 2074 6f20 6d61 6b65 2064 6174 612d 6472   to make data-dr
+00000440: 6976 656e 2064 6563 6973 696f 6e73 2061  iven decisions a
+00000450: 626f 7574 2074 6865 6972 206d 6172 6b65  bout their marke
+00000460: 7469 6e67 2063 616d 7061 6967 6e73 2e20  ting campaigns. 
+00000470: 4f70 7469 6d69 7a65 2079 6f75 7220 6d61  Optimize your ma
+00000480: 726b 6574 696e 6720 7374 7261 7465 6779  rketing strategy
+00000490: 2061 6e64 2075 6e6c 6f63 6b20 7468 6520   and unlock the 
+000004a0: 6675 6c6c 2070 6f74 656e 7469 616c 206f  full potential o
+000004b0: 6620 796f 7572 2063 7573 746f 6d65 7220  f your customer 
+000004c0: 6461 7461 2e0a 0a23 2320 496e 7374 616c  data...## Instal
+000004d0: 6c61 7469 6f6e 0a0a 496e 7374 616c 6c20  lation..Install 
+000004e0: 616e 6420 6163 7469 7661 7465 2061 6e20  and activate an 
+000004f0: 656e 7669 726f 6e6d 656e 7420 2865 2e67  environment (e.g
+00000500: 2e20 606d 6172 6b65 7469 6e67 5f65 6e76  . `marketing_env
+00000510: 6029 2077 6974 6820 7468 6520 6070 796d  `) with the `pym
+00000520: 632d 6d61 726b 6574 696e 6760 2070 6163  c-marketing` pac
+00000530: 6b61 6765 2066 726f 6d20 5b63 6f6e 6461  kage from [conda
+00000540: 2d66 6f72 6765 5d28 6874 7470 733a 2f2f  -forge](https://
+00000550: 636f 6e64 612d 666f 7267 652e 6f72 6729  conda-forge.org)
+00000560: 2e20 4974 206d 6179 206c 6f6f 6b20 736f  . It may look so
+00000570: 6d65 7468 696e 6720 6c69 6b65 2074 6865  mething like the
+00000580: 2066 6f6c 6c6f 7769 6e67 3a0a 0a60 6060   following:..```
+00000590: 6261 7368 0a6d 616d 6261 2063 7265 6174  bash.mamba creat
+000005a0: 6520 2d63 2063 6f6e 6461 2d66 6f72 6765  e -c conda-forge
+000005b0: 202d 6e20 6d61 726b 6574 696e 675f 656e   -n marketing_en
+000005c0: 7620 7079 6d63 2d6d 6172 6b65 7469 6e67  v pymc-marketing
+000005d0: 0a6d 616d 6261 2061 6374 6976 6174 6520  .mamba activate 
+000005e0: 6d61 726b 6574 696e 675f 656e 760a 6060  marketing_env.``
+000005f0: 600a 0a53 6565 2074 6865 206f 6666 6963  `..See the offic
+00000600: 6961 6c20 5b50 794d 4320 696e 7374 616c  ial [PyMC instal
+00000610: 6c61 7469 6f6e 2067 7569 6465 5d28 6874  lation guide](ht
+00000620: 7470 733a 2f2f 7777 772e 7079 6d63 2e69  tps://www.pymc.i
+00000630: 6f2f 7072 6f6a 6563 7473 2f64 6f63 732f  o/projects/docs/
+00000640: 656e 2f6c 6174 6573 742f 696e 7374 616c  en/latest/instal
+00000650: 6c61 7469 6f6e 2e68 746d 6c29 2069 6620  lation.html) if 
+00000660: 6d6f 7265 2064 6574 6169 6c20 6973 206e  more detail is n
+00000670: 6565 6465 642e 0a0a 466f 7220 7465 7374  eeded...For test
+00000680: 696e 6720 7075 7270 6f73 6573 2c20 6966  ing purposes, if
+00000690: 2079 6f75 2077 6973 6820 746f 2069 6e73   you wish to ins
+000006a0: 7461 6c6c 2074 6865 2060 6d61 696e 6020  tall the `main` 
+000006b0: 6272 616e 6368 2064 6972 6563 746c 7920  branch directly 
+000006c0: 6672 6f6d 2047 6974 4875 623a 0a0a 6060  from GitHub:..``
+000006d0: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+000006e0: 6c20 6769 742b 6874 7470 733a 2f2f 6769  l git+https://gi
+000006f0: 7468 7562 2e63 6f6d 2f70 796d 632d 6c61  thub.com/pymc-la
+00000700: 6273 2f70 796d 632d 6d61 726b 6574 696e  bs/pymc-marketin
+00000710: 672e 6769 740a 6060 600a 0a23 2320 4261  g.git.```..## Ba
+00000720: 7965 7369 616e 204d 6564 6961 204d 6978  yesian Media Mix
+00000730: 204d 6f64 656c 7320 284d 4d4d 7329 2069   Models (MMMs) i
+00000740: 6e20 5079 4d43 0a0a 496e 2074 6869 7320  n PyMC..In this 
+00000750: 7061 636b 6167 6520 7765 2070 726f 7669  package we provi
+00000760: 6465 2061 6e20 4150 4920 666f 7220 6120  de an API for a 
+00000770: 4261 7965 7369 616e 206d 6564 6961 206d  Bayesian media m
+00000780: 6978 206d 6f64 656c 2028 4d4d 4d29 2073  ix model (MMM) s
+00000790: 7065 6369 6669 6361 7469 6f6e 2066 6f6c  pecification fol
+000007a0: 6c6f 7769 6e67 205b 4a69 6e2c 2059 7578  lowing [Jin, Yux
+000007b0: 7565 2c20 6574 2061 6c2e 20e2 809c 4261  ue, et al. ...Ba
+000007c0: 7965 7369 616e 206d 6574 686f 6473 2066  yesian methods f
+000007d0: 6f72 206d 6564 6961 206d 6978 206d 6f64  or media mix mod
+000007e0: 656c 696e 6720 7769 7468 2063 6172 7279  eling with carry
+000007f0: 6f76 6572 2061 6e64 2073 6861 7065 2065  over and shape e
+00000800: 6666 6563 7473 2ee2 809d 2028 3230 3137  ffects.... (2017
+00000810: 292e 5d28 6874 7470 733a 2f2f 7265 7365  ).](https://rese
+00000820: 6172 6368 2e67 6f6f 676c 652f 7075 6273  arch.google/pubs
+00000830: 2f70 7562 3436 3030 312f 2920 436f 6e63  /pub46001/) Conc
+00000840: 7265 7465 6c79 2c20 6769 7665 6e20 6120  retely, given a 
+00000850: 7469 6d65 2073 6572 6965 7320 7461 7267  time series targ
+00000860: 6574 2076 6172 6961 626c 6520 2479 5f7b  et variable $y_{
+00000870: 747d 2420 2865 2e67 2e20 7361 6c65 7320  t}$ (e.g. sales 
+00000880: 6f6e 2063 6f6e 7665 7273 696f 6e73 292c  on conversions),
+00000890: 206d 6564 6961 2076 6172 6961 626c 6573   media variables
+000008a0: 2024 785f 7b6d 2c20 747d 2420 2865 2e67   $x_{m, t}$ (e.g
+000008b0: 2e20 696d 7072 6573 7369 6f6e 732c 2063  . impressions, c
+000008c0: 6c69 636b 7320 6f72 2063 6f73 7473 2920  licks or costs) 
+000008d0: 616e 6420 6120 7365 7420 6f66 2063 6f6e  and a set of con
+000008e0: 7472 6f6c 2063 6f76 6172 6961 7465 7320  trol covariates 
+000008f0: 247a 5f7b 632c 2074 7d24 2028 652e 672e  $z_{c, t}$ (e.g.
+00000900: 2068 6f6c 6964 6179 732c 2073 7065 6369   holidays, speci
+00000910: 616c 2065 7665 6e74 7329 2077 6520 636f  al events) we co
+00000920: 6e73 6964 6572 2061 206c 696e 6561 7220  nsider a linear 
+00000930: 6d6f 6465 6c20 6f66 2074 6865 2066 6f72  model of the for
+00000940: 6d0a 0a24 240a 795f 7b74 7d20 3d20 5c61  m..$$.y_{t} = \a
+00000950: 6c70 6861 202b 205c 7375 6d5f 7b6d 3d31  lpha + \sum_{m=1
+00000960: 7d5e 7b4d 7d5c 6265 7461 5f7b 6d7d 6628  }^{M}\beta_{m}f(
+00000970: 785f 7b6d 2c20 747d 2920 2b20 205c 7375  x_{m, t}) +  \su
+00000980: 6d5f 7b63 3d31 7d5e 7b43 7d5c 6761 6d6d  m_{c=1}^{C}\gamm
+00000990: 615f 7b63 7d7a 5f7b 632c 2074 7d20 2b20  a_{c}z_{c, t} + 
+000009a0: 5c76 6172 6570 7369 6c6f 6e5f 7b74 7d2c  \varepsilon_{t},
+000009b0: 0a24 240a 0a77 6865 7265 2024 5c61 6c70  .$$..where $\alp
+000009c0: 6861 2420 6973 2074 6865 2069 6e74 6572  ha$ is the inter
+000009d0: 6365 7074 2c20 2466 2420 6973 2061 206d  cept, $f$ is a m
+000009e0: 6564 6961 2074 7261 6e73 666f 726d 6174  edia transformat
+000009f0: 696f 6e20 6675 6e63 7469 6f6e 2061 6e64  ion function and
+00000a00: 2024 5c76 6172 6570 7369 6c6f 6e5f 7b74   $\varepsilon_{t
+00000a10: 7d24 2069 7320 7468 6520 6572 726f 7220  }$ is the error 
+00000a20: 7468 6572 6d20 7768 6963 6820 7765 2061  therm which we a
+00000a30: 7373 756d 6520 6973 206e 6f72 6d61 6c6c  ssume is normall
+00000a40: 7920 6469 7374 7269 6275 7465 642e 2054  y distributed. T
+00000a50: 6865 2066 756e 6374 696f 6e20 2466 2420  he function $f$ 
+00000a60: 656e 636f 6465 7320 7468 6520 636f 6e74  encodes the cont
+00000a70: 7269 6275 7469 6f6e 206f 6620 6d65 6469  ribution of medi
+00000a80: 6120 6f6e 2074 6865 2074 6172 6765 7420  a on the target 
+00000a90: 7661 7269 6162 6c65 2e20 5479 7069 6361  variable. Typica
+00000aa0: 6c6c 7920 7765 2063 6f6e 7369 6465 7220  lly we consider 
+00000ab0: 7477 6f20 7479 7065 7320 6f66 2074 7261  two types of tra
+00000ac0: 6e73 666f 726d 6174 696f 6e3a 2061 6473  nsformation: ads
+00000ad0: 746f 636b 2028 6361 7272 792d 6f76 6572  tock (carry-over
+00000ae0: 2920 616e 6420 7361 7475 7261 7469 6f6e  ) and saturation
+00000af0: 2065 6666 6563 7473 2e0a 0a5b 4865 7265   effects...[Here
+00000b00: 5d28 6874 7470 733a 2f2f 7079 6d63 2d6d  ](https://pymc-m
+00000b10: 6172 6b65 7469 6e67 2e72 6561 6474 6865  arketing.readthe
+00000b20: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+00000b30: 652f 6e6f 7465 626f 6f6b 732f 6d6d 6d2f  e/notebooks/mmm/
+00000b40: 6d6d 6d5f 6578 616d 706c 652e 6874 6d6c  mmm_example.html
+00000b50: 2920 796f 7520 6361 6e20 6669 6e64 2061  ) you can find a
+00000b60: 2073 696d 756c 6174 6564 2065 7861 6d70   simulated examp
+00000b70: 6c65 3a0a 0a31 2e20 4669 7273 742c 2077  le:..1. First, w
+00000b80: 6520 6465 7363 7269 6265 2074 6865 2064  e describe the d
+00000b90: 6174 6120 6765 6e61 7261 7469 6f6e 2070  ata genaration p
+00000ba0: 726f 6365 7373 206f 6620 6120 7369 6d75  rocess of a simu
+00000bb0: 6c61 7465 6420 6461 7461 7365 742e 0a32  lated dataset..2
+00000bc0: 2e20 4e65 7874 2c20 7765 2064 6573 6372  . Next, we descr
+00000bd0: 6962 6520 686f 7720 746f 2073 7065 6369  ibe how to speci
+00000be0: 6679 2061 6e64 2066 6974 2061 206d 6564  fy and fit a med
+00000bf0: 6961 206d 6978 206d 6f64 656c 2028 6173  ia mix model (as
+00000c00: 2064 6573 6372 6962 6564 2061 626f 7665   described above
+00000c10: 2920 7573 696e 6720 7468 6520 6070 796d  ) using the `pym
+00000c20: 632d 6d61 726b 6574 696e 6760 204d 4d4d  c-marketing` MMM
+00000c30: 2773 2041 5049 2e0a 332e 2046 696e 616c  's API..3. Final
+00000c40: 6c79 2c20 7765 2064 6573 6372 6962 6520  ly, we describe 
+00000c50: 7468 6520 6d6f 6465 6c20 7265 7375 6c74  the model result
+00000c60: 733a 2063 6861 6e6e 656c 2063 6f6e 7374  s: channel const
+00000c70: 7269 6275 7469 6f6e 2061 6e64 2052 4f41  ribution and ROA
+00000c80: 5320 6573 7469 6d61 7469 6f6e 2e20 5765  S estimation. We
+00000c90: 2061 6c73 6f20 7368 6f77 2068 6f77 2074   also show how t
+00000ca0: 6865 206d 6f64 656c 2072 6563 6f76 6572  he model recover
+00000cb0: 7320 7468 6520 7061 7261 6d65 7465 7273  s the parameters
+00000cc0: 2066 726f 6d20 7468 6520 6461 7461 2067   from the data g
+00000cd0: 656e 6572 6174 696f 6e20 7072 6f63 6573  eneration proces
+00000ce0: 7320 7374 6570 2e0a 0a23 2323 2052 6566  s step...### Ref
+00000cf0: 6572 656e 6365 733a 0a0a 2d20 5b4a 696e  erences:..- [Jin
+00000d00: 2c20 5975 7875 652c 2065 7420 616c 2e20  , Yuxue, et al. 
+00000d10: e280 9c42 6179 6573 6961 6e20 6d65 7468  ...Bayesian meth
+00000d20: 6f64 7320 666f 7220 6d65 6469 6120 6d69  ods for media mi
+00000d30: 7820 6d6f 6465 6c69 6e67 2077 6974 6820  x modeling with 
+00000d40: 6361 7272 796f 7665 7220 616e 6420 7368  carryover and sh
+00000d50: 6170 6520 6566 6665 6374 732e e280 9d20  ape effects.... 
+00000d60: 2832 3031 3729 2e5d 2868 7474 7073 3a2f  (2017).](https:/
+00000d70: 2f72 6573 6561 7263 682e 676f 6f67 6c65  /research.google
+00000d80: 2f70 7562 732f 7075 6234 3630 3031 2f29  /pubs/pub46001/)
+00000d90: 0a2d 2050 794d 4320 4c61 6273 2042 6c6f  .- PyMC Labs Blo
+00000da0: 673a 0a20 202d 205b 4261 7965 7369 616e  g:.  - [Bayesian
+00000db0: 204d 6564 6961 204d 6978 204d 6f64 656c   Media Mix Model
+00000dc0: 696e 6720 666f 7220 4d61 726b 6574 696e  ing for Marketin
+00000dd0: 6720 4f70 7469 6d69 7a61 7469 6f6e 5d28  g Optimization](
+00000de0: 6874 7470 733a 2f2f 7777 772e 7079 6d63  https://www.pymc
+00000df0: 2d6c 6162 732e 696f 2f62 6c6f 672d 706f  -labs.io/blog-po
+00000e00: 7374 732f 6261 7965 7369 616e 2d6d 6564  sts/bayesian-med
+00000e10: 6961 2d6d 6978 2d6d 6f64 656c 696e 672d  ia-mix-modeling-
+00000e20: 666f 722d 6d61 726b 6574 696e 672d 6f70  for-marketing-op
+00000e30: 7469 6d69 7a61 7469 6f6e 2f29 0a20 202d  timization/).  -
+00000e40: 205b 496d 7072 6f76 696e 6720 7468 6520   [Improving the 
+00000e50: 5370 6565 6420 616e 6420 4163 6375 7261  Speed and Accura
+00000e60: 6379 206f 6620 4261 7965 7369 616e 204d  cy of Bayesian M
+00000e70: 6564 6961 204d 6978 204d 6f64 656c 735d  edia Mix Models]
+00000e80: 2868 7474 7073 3a2f 2f77 7777 2e70 796d  (https://www.pym
+00000e90: 632d 6c61 6273 2e69 6f2f 626c 6f67 2d70  c-labs.io/blog-p
+00000ea0: 6f73 7473 2f72 6564 7563 696e 672d 6375  osts/reducing-cu
+00000eb0: 7374 6f6d 6572 2d61 6371 7569 7369 7469  stomer-acquisiti
+00000ec0: 6f6e 2d63 6f73 7473 2d68 6f77 2d77 652d  on-costs-how-we-
+00000ed0: 6865 6c70 6564 2d6f 7074 696d 697a 696e  helped-optimizin
+00000ee0: 672d 6865 6c6c 6f66 7265 7368 732d 6d61  g-hellofreshs-ma
+00000ef0: 726b 6574 696e 672d 6275 6467 6574 2f29  rketing-budget/)
+00000f00: 0a2d 205b 4a6f 686e 732c 204d 6963 6861  .- [Johns, Micha
+00000f10: 656c 2061 6e64 2057 616e 672c 2020 5a68  el and Wang,  Zh
+00000f20: 656e 7975 2e20 2241 2042 6179 6573 6961  enyu. "A Bayesia
+00000f30: 6e20 4170 7072 6f61 6368 2074 6f20 4d65  n Approach to Me
+00000f40: 6469 6120 4d69 7820 4d6f 6465 6c69 6e67  dia Mix Modeling
+00000f50: 225d 2868 7474 7073 3a2f 2f77 7777 2e79  "](https://www.y
+00000f60: 6f75 7475 6265 2e63 6f6d 2f77 6174 6368  outube.com/watch
+00000f70: 3f76 3d55 7a6e 4d5f 2d5f 3736 3059 290a  ?v=UznM_-_760Y).
+00000f80: 2d20 5b4f 7264 757a 2c20 4a75 616e 2e20  - [Orduz, Juan. 
+00000f90: 224d 6564 6961 2045 6666 6563 7420 4573  "Media Effect Es
+00000fa0: 7469 6d61 7469 6f6e 2077 6974 6820 5079  timation with Py
+00000fb0: 4d43 3a20 4164 7374 6f63 6b2c 2053 6174  MC: Adstock, Sat
+00000fc0: 7572 6174 696f 6e20 2620 4469 6d69 6e69  uration & Dimini
+00000fd0: 7368 696e 6720 5265 7475 726e 7322 5d28  shing Returns"](
+00000fe0: 6874 7470 733a 2f2f 6a75 616e 6974 6f72  https://juanitor
+00000ff0: 6475 7a2e 6769 7468 7562 2e69 6f2f 7079  duz.github.io/py
+00001000: 6d63 5f6d 6d6d 2f29 0a0a 2d2d 2d0a 0a23  mc_mmm/)..---..#
+00001010: 2320 4261 7965 7369 616e 2043 4c56 7320  # Bayesian CLVs 
+00001020: 696e 2050 794d 430a 5b43 7573 746f 6d65  in PyMC.[Custome
+00001030: 7220 4c69 6665 7469 6d65 2056 616c 7565  r Lifetime Value
+00001040: 5d28 6874 7470 733a 2f2f 656e 2e77 696b  ](https://en.wik
+00001050: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00001060: 4375 7374 6f6d 6572 5f6c 6966 6574 696d  Customer_lifetim
+00001070: 655f 7661 6c75 6529 2028 434c 5629 206d  e_value) (CLV) m
+00001080: 6f64 656c 7320 6172 6520 616e 6f74 6865  odels are anothe
+00001090: 7220 696d 706f 7274 616e 7420 636c 6173  r important clas
+000010a0: 7320 6f66 206d 6f64 656c 732e 2054 6865  s of models. The
+000010b0: 7265 2061 7265 206d 616e 7920 6469 6666  re are many diff
+000010c0: 6572 656e 7420 7479 7065 7320 6f66 2043  erent types of C
+000010d0: 4c56 206d 6f64 656c 7320 616e 6420 6974  LV models and it
+000010e0: 2063 616e 2062 6520 6865 6c70 6675 6c20   can be helpful 
+000010f0: 746f 2063 6f6e 6365 7074 7561 6c69 7365  to conceptualise
+00001100: 2074 6865 6d20 6173 2066 6974 7469 6e67   them as fitting
+00001110: 2069 6e20 6120 322d 6469 6d65 6e73 696f   in a 2-dimensio
+00001120: 6e61 6c20 6772 6964 2061 7320 6265 6c6f  nal grid as belo
+00001130: 772e 2041 6e20 6578 6365 6c6c 656e 7420  w. An excellent 
+00001140: 7365 7420 6f66 2069 6e74 726f 6475 6374  set of introduct
+00001150: 696f 6e20 736c 6964 6573 2074 6f20 434c  ion slides to CL
+00001160: 5627 7320 6973 2070 726f 7669 6465 6420  V's is provided 
+00001170: 696e 205b 5072 6f62 6162 696c 6974 7920  in [Probability 
+00001180: 4d6f 6465 6c73 2066 6f72 2043 7573 746f  Models for Custo
+00001190: 6d65 722d 4261 7365 2041 6e61 6c79 7369  mer-Base Analysi
+000011a0: 735d 2868 7474 7073 3a2f 2f77 7777 2e62  s](https://www.b
+000011b0: 7275 6365 6861 7264 6965 2e63 6f6d 2f74  rucehardie.com/t
+000011c0: 616c 6b73 2f68 6f5f 6362 615f 7475 745f  alks/ho_cba_tut_
+000011d0: 6172 745f 3039 2e70 6466 2920 6279 2046  art_09.pdf) by F
+000011e0: 6164 6572 2026 2048 6172 6469 6520 2832  ader & Hardie (2
+000011f0: 3030 3929 2e0a 0a23 2323 2045 7861 6d70  009)...### Examp
+00001200: 6c65 730a 0a7c 2020 2020 2020 2020 2020  les..|          
+00001210: 2020 2020 2020 7c20 2a2a 4e6f 6e2d 636f        | **Non-co
+00001220: 6e74 7261 6374 7561 6c2a 2a20 7c20 2a2a  ntractual** | **
+00001230: 436f 6e74 7261 6374 7561 6c2a 2a20 2020  Contractual**   
+00001240: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001250: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00001260: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00001270: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00001280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001290: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 202a 2a43  ---------|.| **C
+000012a0: 6f6e 7469 6e75 6f75 732a 2a20 7c20 4275  ontinuous** | Bu
+000012b0: 7969 6e67 2067 726f 6365 7269 6573 2020  ying groceries  
+000012c0: 2020 7c20 4175 6469 626c 6520 2020 2020    | Audible     
+000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012e0: 2020 2020 7c0a 7c20 2a2a 4469 7363 7265      |.| **Discre
+000012f0: 7465 2a2a 2020 207c 2043 696e 656d 6120  te**   | Cinema 
+00001300: 7469 636b 6574 2020 2020 2020 207c 204d  ticket       | M
+00001310: 6f6e 7468 6c79 206f 7220 7965 6172 6c79  onthly or yearly
+00001320: 2073 7562 7363 7269 7074 696f 6e73 207c   subscriptions |
+00001330: 0a0a 546f 2065 7870 6c61 696e 2066 7572  ..To explain fur
+00001340: 7468 6572 3a0a 2d20 2a2a 436f 6e74 7261  ther:.- **Contra
+00001350: 6374 7561 6c3a 2a2a 2049 6e20 636f 6e74  ctual:** In cont
+00001360: 7261 6374 7561 6c20 7365 7474 696e 6773  ractual settings
+00001370: 2c20 6120 6375 7374 6f6d 6572 2068 6173  , a customer has
+00001380: 2061 2063 6f6e 7472 6163 7420 7768 6963   a contract whic
+00001390: 6820 636f 6e74 696e 7565 7320 746f 2062  h continues to b
+000013a0: 6520 6163 7469 7665 2075 6e74 696c 2069  e active until i
+000013b0: 7420 6973 2065 7870 6c69 6369 746c 7920  t is explicitly 
+000013c0: 6361 6e63 656c 6c65 642e 2054 6865 7265  cancelled. There
+000013d0: 666f 7265 2c20 6375 7374 6f6d 6572 2063  fore, customer c
+000013e0: 6875 726e 2065 7665 6e74 7320 6172 6520  hurn events are 
+000013f0: 6f62 7365 7276 6564 2e0a 0a2d 202a 2a4e  observed...- **N
+00001400: 6f6e 2d63 6f6e 7472 6163 7475 616c 3a2a  on-contractual:*
+00001410: 2a20 496e 206e 6f6e 2d63 6f6e 7472 6163  * In non-contrac
+00001420: 7475 616c 2073 6574 7469 6e67 732c 2074  tual settings, t
+00001430: 6865 7265 2069 7320 6e6f 206f 6e67 6f69  here is no ongoi
+00001440: 6e67 2063 6f6e 7472 6163 7420 7468 6174  ng contract that
+00001450: 2061 2063 7573 746f 6d65 7220 6861 7320   a customer has 
+00001460: 7769 7468 2061 2063 6f6d 7061 6e79 2e20  with a company. 
+00001470: 496e 7374 6561 642c 2070 7572 6368 6173  Instead, purchas
+00001480: 6573 2063 616e 2062 6520 6164 2068 6f63  es can be ad hoc
+00001490: 2061 6e64 2063 6875 726e 2065 7665 6e74   and churn event
+000014a0: 7320 6172 6520 756e 6f62 7365 7276 6564  s are unobserved
+000014b0: 2e0a 0a2d 202a 2a44 6973 6372 6574 653a  ...- **Discrete:
+000014c0: 2a2a 2048 6572 652c 2070 7572 6368 6173  ** Here, purchas
+000014d0: 6573 2061 7265 206d 6164 6520 6174 2064  es are made at d
+000014e0: 6973 6372 6574 6520 706f 696e 7473 2069  iscrete points i
+000014f0: 6e20 7469 6d65 2e20 5468 6973 206f 6276  n time. This obv
+00001500: 696f 7573 6c79 2064 6570 656e 6473 2075  iously depends u
+00001510: 706f 6e20 7468 6520 7469 6d65 7363 616c  pon the timescal
+00001520: 6520 7468 6174 2077 6520 6172 6520 776f  e that we are wo
+00001530: 726b 696e 6720 6f6e 2c20 6275 7420 7479  rking on, but ty
+00001540: 7069 6361 6c6c 7920 6120 7265 6c65 7661  pically a releva
+00001550: 6e74 2074 696d 6520 7065 7269 6f64 2077  nt time period w
+00001560: 6f75 6c64 2062 6520 6120 6d6f 6e74 6820  ould be a month 
+00001570: 6f72 2079 6561 722e 2048 6f77 6576 6572  or year. However
+00001580: 2069 7420 636f 756c 6420 6265 206d 6f72   it could be mor
+00001590: 6520 6772 616e 7561 6c61 7220 7468 616e  e granualar than
+000015a0: 2074 6869 7320 2d20 7468 696e 6b20 6f66   this - think of
+000015b0: 2074 616b 696e 6720 7468 6520 326e 6420   taking the 2nd 
+000015c0: 6f66 2034 2069 6e74 6572 2d63 6974 7920  of 4 inter-city 
+000015d0: 7472 6169 6e20 6a6f 7572 6e65 7973 206f  train journeys o
+000015e0: 6666 6572 6564 2070 6572 2064 6179 2e0a  ffered per day..
+000015f0: 0a2d 202a 2a43 6f6e 7469 6e75 6f75 733a  .- **Continuous:
+00001600: 2a2a 2049 6e20 7468 6520 636f 6e74 696e  ** In the contin
+00001610: 756f 7573 2d74 696d 6520 646f 6d61 696e  uous-time domain
+00001620: 2c20 7075 7263 6861 7365 7320 6361 6e20  , purchases can 
+00001630: 6265 206d 6164 6520 6174 2061 6e79 2070  be made at any p
+00001640: 6f69 6e74 2077 6974 6869 6e20 6120 6669  oint within a fi
+00001650: 726d 7320 6f70 656e 696e 6720 686f 7572  rms opening hour
+00001660: 732e 2046 6f72 206f 6e6c 696e 6520 6f72  s. For online or
+00001670: 6465 7269 6e67 2c20 7468 6973 2063 6f75  dering, this cou
+00001680: 6c64 2062 6520 616e 7920 706f 696e 7420  ld be any point 
+00001690: 7769 7468 696e 2061 2032 3420 686f 7572  within a 24 hour
+000016a0: 2063 7963 6c65 2c20 6f72 2070 7572 6368   cycle, or purch
+000016b0: 6173 6573 2069 6e20 7068 7973 6963 616c  ases in physical
+000016c0: 2073 746f 7265 7320 636f 756c 6420 6265   stores could be
+000016d0: 206d 6164 6520 6174 2061 6e79 2070 6f69   made at any poi
+000016e0: 6e74 2064 7572 696e 6720 7468 6520 7472  nt during the tr
+000016f0: 6164 696e 6720 6461 792e 0a0a 496e 2074  ading day...In t
+00001700: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00001710: 2c20 7765 2070 726f 7669 6465 2073 6f6d  , we provide som
+00001720: 6520 6578 616d 706c 6573 206f 6e20 686f  e examples on ho
+00001730: 7720 746f 2075 7365 2074 6865 2043 4c56  w to use the CLV
+00001740: 2041 5049 2e20 5765 2075 7365 2074 6865   API. We use the
+00001750: 2064 6174 6120 6672 6f6d 2074 6865 205b   data from the [
+00001760: 606c 6966 6574 696d 6573 605d 2868 7474  `lifetimes`](htt
+00001770: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001780: 4361 6d44 6176 6964 736f 6e50 696c 6f6e  CamDavidsonPilon
+00001790: 2f6c 6966 6574 696d 6573 2920 7061 636b  /lifetimes) pack
+000017a0: 6167 6520 746f 2069 6c6c 7573 7472 6174  age to illustrat
+000017b0: 6520 7468 6520 6d6f 6465 6c73 2e0a 0a2d  e the models...-
+000017c0: 205b 434c 5620 5175 6963 6b73 7461 7274   [CLV Quickstart
+000017d0: 5d28 6874 7470 733a 2f2f 7079 6d63 2d6d  ](https://pymc-m
+000017e0: 6172 6b65 7469 6e67 2e72 6561 6474 6865  arketing.readthe
+000017f0: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+00001800: 652f 6e6f 7465 626f 6f6b 732f 636c 762f  e/notebooks/clv/
+00001810: 636c 765f 7175 6963 6b73 7461 7274 2e68  clv_quickstart.h
+00001820: 746d 6c29 0a2d 205b 4247 2f4e 4244 206d  tml).- [BG/NBD m
+00001830: 6f64 656c 5d28 6874 7470 733a 2f2f 7079  odel](https://py
+00001840: 6d63 2d6d 6172 6b65 7469 6e67 2e72 6561  mc-marketing.rea
+00001850: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+00001860: 7461 626c 652f 6e6f 7465 626f 6f6b 732f  table/notebooks/
+00001870: 636c 762f 6267 5f6e 6264 2e68 746d 6c29  clv/bg_nbd.html)
+00001880: 0a2d 205b 4761 6d6d 612d 4761 6d6d 6120  .- [Gamma-Gamma 
+00001890: 6d6f 6465 6c5d 2868 7474 7073 3a2f 2f70  model](https://p
+000018a0: 796d 632d 6d61 726b 6574 696e 672e 7265  ymc-marketing.re
+000018b0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000018c0: 7374 6162 6c65 2f6e 6f74 6562 6f6f 6b73  stable/notebooks
+000018d0: 2f63 6c76 2f67 616d 6d61 5f67 616d 6d61  /clv/gamma_gamma
+000018e0: 2e68 746d 6c29 0a0a 2d2d 2d0a 0a23 2320  .html)..---..## 
+000018f0: f09f 939e 2053 6368 6564 756c 6520 6120  .... Schedule a 
+00001900: 436f 6e73 756c 7461 7469 6f6e 0a55 6e6c  Consultation.Unl
+00001910: 6f63 6b20 796f 7572 2070 6f74 656e 7469  ock your potenti
+00001920: 616c 2077 6974 6820 6120 6672 6565 2033  al with a free 3
+00001930: 302d 6d69 6e75 7465 2073 7472 6174 6567  0-minute strateg
+00001940: 7920 7365 7373 696f 6e20 7769 7468 206f  y session with o
+00001950: 7572 2050 794d 4320 6578 7065 7274 732e  ur PyMC experts.
+00001960: 2044 6973 636f 7665 7220 686f 7720 6f70   Discover how op
+00001970: 656e 2073 6f75 7263 6520 736f 6c75 7469  en source soluti
+00001980: 6f6e 7320 616e 6420 7079 6d63 2d6d 6172  ons and pymc-mar
+00001990: 6b65 7469 6e67 2063 616e 2065 6c65 7661  keting can eleva
+000019a0: 7465 2079 6f75 7220 6d65 6469 612d 6d69  te your media-mi
+000019b0: 7820 6d6f 6465 6c73 2061 6e64 2063 7573  x models and cus
+000019c0: 746f 6d65 7220 6c69 6665 7469 6d65 2076  tomer lifetime v
+000019d0: 616c 7565 2061 6e61 6c79 7365 732e 2042  alue analyses. B
+000019e0: 6f6f 7374 2079 6f75 7220 6361 7265 6572  oost your career
+000019f0: 2061 6e64 206f 7267 616e 697a 6174 696f   and organizatio
+00001a00: 6e20 6279 206d 616b 696e 6720 736d 6172  n by making smar
+00001a10: 7465 722c 2064 6174 612d 6472 6976 656e  ter, data-driven
+00001a20: 2064 6563 6973 696f 6e73 2e20 446f 6e27   decisions. Don'
+00001a30: 7420 7761 6974 e280 945b 636c 6169 6d20  t wait...[claim 
+00001a40: 796f 7572 2063 6f6d 706c 696d 656e 7461  your complimenta
+00001a50: 7279 2073 6573 7369 6f6e 5d28 6874 7470  ry session](http
+00001a60: 733a 2f2f 6361 6c65 6e64 6c79 2e63 6f6d  s://calendly.com
+00001a70: 2f62 656e 6a61 6d69 6e2d 7669 6e63 656e  /benjamin-vincen
+00001a80: 742f 7079 6d63 2d6d 6172 6b65 7469 6e67  t/pymc-marketing
+00001a90: 2920 746f 6461 7920 616e 6420 6c65 6164  ) today and lead
+00001aa0: 2074 6865 2077 6179 2069 6e20 6d61 726b   the way in mark
+00001ab0: 6574 696e 6720 616e 6420 6461 7461 2073  eting and data s
+00001ac0: 6369 656e 6365 2069 6e6e 6f76 6174 696f  cience innovatio
+00001ad0: 6e2e 0a0a 2323 2055 7369 6e67 2050 794d  n...## Using PyM
+00001ae0: 432d 4d61 726b 6574 696e 6720 616e 6420  C-Marketing and 
+00001af0: 686f 7720 5079 4d43 204c 6162 7320 6361  how PyMC Labs ca
+00001b00: 6e20 6865 6c70 2079 6f75 0a50 794d 432d  n help you.PyMC-
+00001b10: 4d61 726b 6574 696e 6720 7573 6573 2074  Marketing uses t
+00001b20: 6865 205b 4170 6163 6865 2032 2e30 206c  he [Apache 2.0 l
+00001b30: 6963 656e 6365 5d28 4c49 4345 4e53 4529  icence](LICENSE)
+00001b40: 2077 6869 6368 2070 6572 6d69 7473 2063   which permits c
+00001b50: 6f6d 6d65 7263 6961 6c20 7573 652c 2061  ommercial use, a
+00001b60: 6d6f 6e67 7374 206f 7468 6572 2074 6869  mongst other thi
+00001b70: 6e67 732e 0a0a 4966 2079 6f75 2077 616e  ngs...If you wan
+00001b80: 7420 746f 2062 7569 6c64 2075 706f 6e20  t to build upon 
+00001b90: 7468 6520 7061 636b 6167 652c 2070 6c65  the package, ple
+00001ba0: 6173 6520 6665 656c 2066 7265 6520 746f  ase feel free to
+00001bb0: 2066 6f72 6b20 7468 6520 7265 706f 2061   fork the repo a
+00001bc0: 6e64 2073 7562 6d69 7420 6120 7075 6c6c  nd submit a pull
+00001bd0: 2072 6571 7565 7374 2e20 4966 2069 6e20   request. If in 
+00001be0: 646f 7562 742c 2070 6c65 6173 6520 6f70  doubt, please op
+00001bf0: 656e 2061 6e20 6973 7375 652e 0a0a 466f  en an issue...Fo
+00001c00: 7220 636f 6d70 616e 6965 7320 7468 6174  r companies that
+00001c10: 2077 616e 7420 746f 2075 7365 2050 794d   want to use PyM
+00001c20: 432d 4d61 726b 6574 696e 6720 696e 2070  C-Marketing in p
+00001c30: 726f 6475 6374 696f 6e2c 205b 5079 4d43  roduction, [PyMC
+00001c40: 204c 6162 735d 2868 7474 7073 3a2f 2f77   Labs](https://w
+00001c50: 7777 2e70 796d 632d 6c61 6273 2e69 6f29  ww.pymc-labs.io)
+00001c60: 2069 7320 6176 6169 6c61 626c 6520 666f   is available fo
+00001c70: 7220 636f 6e73 756c 7469 6e67 2061 6e64  r consulting and
+00001c80: 2074 7261 696e 696e 672e 2057 6520 6361   training. We ca
+00001c90: 6e20 6865 6c70 2079 6f75 2062 7569 6c64  n help you build
+00001ca0: 2061 6e64 2064 6570 6c6f 7920 796f 7572   and deploy your
+00001cb0: 206d 6f64 656c 7320 696e 2070 726f 6475   models in produ
+00001cc0: 6374 696f 6e2e 2057 6520 6861 7665 2065  ction. We have e
+00001cd0: 7870 6572 6965 6e63 6520 7769 7468 2063  xperience with c
+00001ce0: 7574 7469 6e67 2065 6467 6520 4261 7965  utting edge Baye
+00001cf0: 7369 616e 206d 6f64 656c 6c69 6e67 2074  sian modelling t
+00001d00: 6563 686e 6971 7565 7320 696e 2067 656e  echniques in gen
+00001d10: 6572 616c 2c20 616e 6420 696e 2070 6172  eral, and in par
+00001d20: 7469 6375 6c61 7220 7769 7468 204d 4d4d  ticular with MMM
+00001d30: 7320 616e 6420 434c 5673 2e20 466f 7220  s and CLVs. For 
+00001d40: 6578 616d 706c 652c 2073 6565 206f 7572  example, see our
+00001d50: 2076 6964 656f 206f 6e20 5b42 6179 6573   video on [Bayes
+00001d60: 6961 6e20 4d61 726b 6574 696e 6720 4d69  ian Marketing Mi
+00001d70: 7820 4d6f 6465 6c73 3a20 5374 6174 6520  x Models: State 
+00001d80: 6f66 2074 6865 2041 7274 2061 6e64 2074  of the Art and t
+00001d90: 6865 6972 2046 7574 7572 655d 2868 7474  heir Future](htt
+00001da0: 7073 3a2f 2f77 7777 2e79 6f75 7475 6265  ps://www.youtube
+00001db0: 2e63 6f6d 2f77 6174 6368 3f76 3d78 5678  .com/watch?v=xVx
+00001dc0: 3931 7072 4338 3167 292e 0a              91prC81g)..
```

### Comparing `pymc-marketing-0.1.0/pymc_marketing/clv/__init__.py` & `pymc-marketing-0.1.1/pymc_marketing/clv/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.0/pymc_marketing/clv/distributions.py` & `pymc-marketing-0.1.1/pymc_marketing/clv/distributions.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.0/pymc_marketing/clv/models/basic.py` & `pymc-marketing-0.1.1/pymc_marketing/clv/models/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     def _check_prior_ndim(prior, ndim=0):
         if prior.ndim != ndim:
             raise ValueError(
                 f"Prior variable {prior} must be have {ndim} ndims, but it has {prior.ndim} ndims."
             )
 
     @staticmethod
-    def _process_priors(*priors: TensorVariable) -> Tuple[TensorVariable]:
+    def _process_priors(*priors: TensorVariable) -> Tuple[TensorVariable, ...]:
         """Check that each prior variable is unique and attach `str_repr` method."""
         if len(priors) != len(set(priors)):
             raise ValueError("Prior variables must be unique")
 
         # Related to https://github.com/pymc-devs/pymc/issues/6311
         for prior in priors:
-            prior.str_repr = types.MethodType(str_for_dist, prior)
+            prior.str_repr = types.MethodType(str_for_dist, prior)  # type: ignore
         return priors
 
     def fit(self, fit_method="mcmc", **kwargs):
         """Infer model posterior
 
         Parameters
         ----------
```

### Comparing `pymc-marketing-0.1.0/pymc_marketing/clv/models/beta_geo.py` & `pymc-marketing-0.1.1/pymc_marketing/clv/models/beta_geo.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.0/pymc_marketing/clv/models/gamma_gamma.py` & `pymc-marketing-0.1.1/pymc_marketing/clv/models/gamma_gamma.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytensor.tensor as pt
 import xarray
+from pymc.util import RandomState
 from pytensor.tensor import TensorVariable
 
 from pymc_marketing.clv.models.basic import CLVModel
 from pymc_marketing.clv.utils import customer_lifetime_value, to_xarray
 
 
 class BaseGammaGammaModel(CLVModel):
@@ -29,15 +30,15 @@
         return super()._process_priors(p_prior, q_prior, v_prior)
 
     def distribution_customer_spend(
         self,
         customer_id: Union[np.ndarray, pd.Series],
         mean_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
         frequency: Union[np.ndarray, pd.Series, TensorVariable],
-        random_seed=None,
+        random_seed: Optional[RandomState] = None,
     ) -> xarray.DataArray:
         """Posterior distribution of transaction value per customer"""
 
         x = frequency
         z_mean = mean_transaction_value
 
         coords = {"customer_id": np.unique(customer_id)}
@@ -126,15 +127,18 @@
         frequency: Union[np.ndarray, pd.Series],
         recency: Union[np.ndarray, pd.Series],
         T: Union[np.ndarray, pd.Series],
         time: int = 12,
         discount_rate: float = 0.01,
         freq: str = "D",
     ) -> xarray.DataArray:
-        """Expected customer lifetime value."""
+        """Expected customer lifetime value.
+
+        See clv.utils.customer_lifetime_value for details on the meaning of each parameter
+        """
 
         # Use the Gamma-Gamma estimates for the monetary_values
         adjusted_monetary_value = self.expected_customer_spend(
             customer_id=customer_id,
             mean_transaction_value=mean_transaction_value,
             frequency=frequency,
         )
@@ -377,19 +381,19 @@
         )
         customer_id = gdf.index
         x = gdf["count"]
         z_mean = gdf["mean"]
 
         return customer_id, z_mean, x
 
-    def distribution_customer_spend(
+    def distribution_customer_spend(  # type: ignore [override]
         self,
         customer_id: Union[np.ndarray, pd.Series],
         individual_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
-        random_seed=None,
+        random_seed: Optional[RandomState] = None,
     ) -> xarray.DataArray:
         """Return distribution of transaction value per customer"""
 
         customer_id, z_mean, x = self._summarize_mean_data(
             customer_id, individual_transaction_value
         )
 
@@ -400,41 +404,44 @@
             random_seed=random_seed,
         )
 
     def expected_customer_spend(
         self,
         customer_id: Union[np.ndarray, pd.Series],
         individual_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
-        random_seed=None,
+        random_seed: Optional[RandomState] = None,
     ) -> xarray.DataArray:
         """Return expected transaction value per customer"""
 
         customer_id, z_mean, x = self._summarize_mean_data(
             customer_id, individual_transaction_value
         )
 
         return super().expected_customer_spend(
             customer_id=customer_id,
             mean_transaction_value=z_mean,
             frequency=x,
-            random_seed=random_seed,
+            random_seed=random_seed,  # type: ignore [call-arg]
         )
 
-    def expected_customer_lifetime_value(
+    def expected_customer_lifetime_value(  # type: ignore [override]
         self,
         transaction_model: CLVModel,
         customer_id: Union[np.ndarray, pd.Series],
         individual_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
         recency: Union[np.ndarray, pd.Series],
         T: Union[np.ndarray, pd.Series],
         time: int = 12,
         discount_rate: float = 0.01,
         freq: str = "D",
     ) -> xarray.DataArray:
-        """Return expected customer lifetime value."""
+        """Return expected customer lifetime value.
+
+        See clv.utils.customer_lifetime_value for details on the meaning of each parameter
+        """
 
         customer_id, z_mean, x = self._summarize_mean_data(
             customer_id, individual_transaction_value
         )
 
         return super().expected_customer_lifetime_value(
             transaction_model=transaction_model,
```

### Comparing `pymc-marketing-0.1.0/pymc_marketing/clv/models/shifted_beta_geo.py` & `pymc-marketing-0.1.1/pymc_marketing/clv/models/shifted_beta_geo.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.0/pymc_marketing/clv/plotting.py` & `pymc-marketing-0.1.1/pymc_marketing/clv/plotting.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.0/pymc_marketing/clv/utils.py` & `pymc-marketing-0.1.1/pymc_marketing/clv/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Union
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import xarray
 
 __all__ = ["to_xarray", "customer_lifetime_value", "clv_summary"]
 
@@ -13,17 +13,15 @@
     dims = (dim,)
     coords = {dim: np.asarray(customer_id)}
 
     res = tuple(
         xarray.DataArray(data=array, coords=coords, dims=dims) for array in arrays
     )
 
-    if len(arrays) == 1:
-        return res[0]
-    return res
+    return res[0] if len(arrays) == 1 else res
 
 
 def customer_lifetime_value(
     transaction_model,
     customer_id: Union[pd.Series, np.ndarray],
     frequency: Union[pd.Series, np.ndarray],
     recency: Union[pd.Series, np.ndarray],
@@ -54,20 +52,20 @@
     T: array_like
         The vector of customers' age (time since first purchase)
     monetary_value: array_like
         The monetary value vector of customer's purchases (denoted m in literature).
     time: int, optional
         The lifetime expected for the user in months. Default: 12
     discount_rate: float, optional
-        The monthly adjusted discount rate. Default: 1
+        The monthly adjusted discount rate. Default: 0.01
     freq: string, optional
-        Frequency of discrete time steps used to estimate the customer lifetime value.
-        Defaults to "D" for daily. Other options are "W" (weekly), "M" (monthly), and "H" (hourly).
-        Smaller time frames estimate better the effects of discounting rate, at the cost of more
-        evaluations.
+        Unit of time of the purchase history. Defaults to "D" for daily.
+        Other options are "W" (weekly), "M" (monthly), and "H" (hourly).
+        Example: If your dataset contains information about weekly purchases,
+        you should use "W".
 
     Returns
     -------
     xarray
         DataArray with the estimated customer lifetime values
     """
 
@@ -121,17 +119,17 @@
     return clv
 
 
 def _find_first_transactions(
     transactions: pd.DataFrame,
     customer_id_col: str,
     datetime_col: str,
-    monetary_value_col: str = None,
-    datetime_format: str = None,
-    observation_period_end: Union[str, pd.Period, datetime] = None,
+    monetary_value_col: Optional[str] = None,
+    datetime_format: Optional[str] = None,
+    observation_period_end: Optional[Union[str, pd.Period, datetime]] = None,
     time_unit: str = "D",
 ) -> pd.DataFrame:
     """
     Return dataframe with first transactions.
 
     This takes a DataFrame of transaction data of the form:
         customer_id, datetime [, monetary_value]
@@ -148,44 +146,50 @@
     customer_id_col: string
         Column in the transactions DataFrame that denotes the customer_id.
     datetime_col:  string
         Column in the transactions DataFrame that denotes the datetime the purchase was made.
     monetary_value_col: string, optional
         Column in the transactions DataFrame that denotes the monetary value of the transaction.
         Optional; only needed for spend estimation models like the Gamma-Gamma model.
-    observation_period_end: :obj: datetime
-        A string or datetime to denote the final date of the study.
-        Events after this date are truncated. If not given, defaults to the max 'datetime_col'.
     datetime_format: string, optional
         A string that represents the timestamp format. Useful if Pandas can't understand
         the provided format.
+    observation_period_end: Union[str, pd.Period, datetime], optional
+        A string or datetime to denote the final date of the study.
+        Events after this date are truncated. If not given, defaults to the max 'datetime_col'.
     time_unit: string, optional
         Time granularity for study.
         Default: 'D' for days. Possible values listed here:
         https://numpy.org/devdocs/reference/arrays.datetime.html#datetime-units
     """
 
     select_columns = [customer_id_col, datetime_col]
 
+    if observation_period_end is None:
+        observation_period_end = transactions[datetime_col].max()
+
+    if isinstance(observation_period_end, pd.Period):
+        observation_period_end = observation_period_end.to_timestamp()
+
     if monetary_value_col:
         select_columns.append(monetary_value_col)
 
     transactions = transactions[select_columns].sort_values(select_columns).copy()
 
     # convert date column into a DateTimeIndex for time-wise grouping and truncating
     transactions[datetime_col] = pd.to_datetime(
         transactions[datetime_col], format=datetime_format
     )
     transactions = (
         transactions.set_index(datetime_col).to_period(time_unit).to_timestamp()
     )
 
-    transactions = transactions.loc[
-        (transactions.index <= observation_period_end)
-    ].reset_index()
+    mask = pd.DatetimeIndex(transactions.index) <= observation_period_end
+
+    transactions = transactions.loc[mask].reset_index()
 
     period_groupby = transactions.groupby(
         [datetime_col, customer_id_col], sort=False, as_index=False
     )
 
     if monetary_value_col:
         # when processing a monetary column, make sure to sum together transactions made in the same period
@@ -204,28 +208,28 @@
         .head(1)
         .index
     )
     # flag first transactions as True
     period_transactions.loc[first_transactions, "first"] = True
     select_columns.append("first")
     # reset datetime_col to period
-    period_transactions.loc[:, datetime_col] = pd.Index(
-        period_transactions[datetime_col]
-    ).to_period(time_unit)
+    period_transactions.loc[:, datetime_col] = period_transactions[
+        datetime_col
+    ].dt.to_period(time_unit)
 
     return period_transactions[select_columns]
 
 
 def clv_summary(
     transactions: pd.DataFrame,
     customer_id_col: str,
     datetime_col: str,
-    monetary_value_col: str = None,
-    datetime_format: str = None,
-    observation_period_end: Union[str, pd.Period, datetime] = None,
+    monetary_value_col: Optional[str] = None,
+    datetime_format: Optional[str] = None,
+    observation_period_end: Optional[Union[str, pd.Period, datetime]] = None,
     time_unit: str = "D",
     time_scaler: float = 1,
 ) -> pd.DataFrame:
     """
     Summarize transaction data for modeling.
 
     This transforms a DataFrame of transaction data of the form:
@@ -243,17 +247,17 @@
     customer_id_col: string
         Column in the transactions DataFrame that denotes the customer_id.
     datetime_col:  string
         Column in the transactions DataFrame that denotes the datetime the purchase was made.
     monetary_value_col: string, optional
         Column in the transactions DataFrame that denotes the monetary value of the transaction.
         Optional; only needed for spend estimation models like the Gamma-Gamma model.
-    observation_period_end: datetime, optional
-         A string or datetime to denote the final date of the study.
-         Events after this date are truncated. If not given, defaults to the max 'datetime_col'.
+    observation_period_end: Union[str, pd.Period, datetime], optional
+        A string or datetime to denote the final date of the study.
+        Events after this date are truncated. If not given, defaults to the max 'datetime_col'.
     datetime_format: string, optional
         A string that represents the timestamp format. Useful if Pandas can't understand
         the provided format.
     time_unit: string, optional
         Time granularity for study.
         Default: 'D' for days. Possible values listed here:
         https://numpy.org/devdocs/reference/arrays.datetime.html#datetime-units
@@ -267,56 +271,58 @@
     Returns
     -------
     :obj: DataFrame:
         customer_id, frequency, recency, T [, monetary_value]
     """
 
     if observation_period_end is None:
-        observation_period_end = (
+        observation_period_end_ts = (
             pd.to_datetime(transactions[datetime_col].max(), format=datetime_format)
             .to_period(time_unit)
             .to_timestamp()
         )
+    elif isinstance(observation_period_end, pd.Period):
+        observation_period_end_ts = observation_period_end.to_timestamp()
     else:
-        observation_period_end = (
+        observation_period_end_ts = (
             pd.to_datetime(observation_period_end, format=datetime_format)
             .to_period(time_unit)
             .to_timestamp()
         )
 
     # label repeated transactions
     repeated_transactions = _find_first_transactions(
         transactions,
         customer_id_col,
         datetime_col,
         monetary_value_col,
         datetime_format,
-        observation_period_end,
+        observation_period_end_ts,
         time_unit,
     )
     # reset datetime_col to timestamp
-    repeated_transactions[datetime_col] = pd.Index(
-        repeated_transactions[datetime_col]
-    ).to_timestamp()
+    repeated_transactions[datetime_col] = repeated_transactions[
+        datetime_col
+    ].dt.to_timestamp()
 
     # count all orders by customer
     customers = repeated_transactions.groupby(customer_id_col, sort=False)[
         datetime_col
     ].agg(["min", "max", "count"])
 
     # subtract 1 from count for non-repeat customers
     customers["frequency"] = customers["count"] - 1
 
     customers["T"] = (
-        (observation_period_end - customers["min"])
+        (observation_period_end_ts - customers["min"])
         / np.timedelta64(1, time_unit)
         / time_scaler
     )
     customers["recency"] = (
-        (customers["max"] - customers["min"])
+        (pd.to_datetime(customers["max"]) - pd.to_datetime(customers["min"]))
         / np.timedelta64(1, time_unit)
         / time_scaler
     )
 
     summary_columns = ["frequency", "recency", "T"]
 
     if monetary_value_col:
```

### Comparing `pymc-marketing-0.1.0/pymc_marketing/mmm/preprocessing.py` & `pymc-marketing-0.1.1/pymc_marketing/mmm/preprocessing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from typing import Any, Callable, List, Tuple, Union
 
 import pandas as pd
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import MaxAbsScaler, StandardScaler
 
 __all__ = [
     "preprocessing_method",
@@ -10,46 +10,53 @@
     "MaxAbsScaleChannels",
     "StandardizeControls",
 ]
 
 
 def preprocessing_method(method: Callable) -> Callable:
     if not hasattr(method, "_tags"):
-        method._tags = {}
-    method._tags["preprocessing"] = True
+        method._tags = {}  # type: ignore
+    method._tags["preprocessing"] = True  # type: ignore
     return method
 
 
 class MaxAbsScaleTarget:
+    target_column: str
+    target_transformer: Pipeline
+
     @preprocessing_method
     def max_abs_scale_target_data(self, data: pd.DataFrame) -> pd.DataFrame:
         target_vector = data[self.target_column].to_numpy().reshape(-1, 1)
         transformers = [("scaler", MaxAbsScaler())]
         pipeline = Pipeline(steps=transformers)
         self.target_transformer: Pipeline = pipeline.fit(X=target_vector)
         data[self.target_column] = self.target_transformer.transform(
             X=target_vector
         ).flatten()
         return data
 
 
 class MaxAbsScaleChannels:
+    channel_columns: Union[List[str], Tuple[str]]
+
     @preprocessing_method
     def max_abs_scale_channel_data(self, data: pd.DataFrame) -> pd.DataFrame:
-        channel_data: pd.DataFrame = data[self.channel_columns]
+        channel_data: Union[pd.DataFrame, pd.Series[Any]] = data[self.channel_columns]
         transformers = [("scaler", MaxAbsScaler())]
         pipeline: Pipeline = Pipeline(steps=transformers)
         self.channel_transformer: Pipeline = pipeline.fit(X=channel_data.to_numpy())
         data[self.channel_columns] = self.channel_transformer.transform(
             channel_data.to_numpy()
         )
         return data
 
 
 class StandardizeControls:
+    control_columns: List[str]  # TODO: Handle Optional[List[str]]
+
     @preprocessing_method
     def standardize_control_data(self, data: pd.DataFrame) -> pd.DataFrame:
         control_data: pd.DataFrame = data[self.control_columns]
         transformers = [("scaler", StandardScaler())]
         pipeline: Pipeline = Pipeline(steps=transformers)
         self.control_transformer: Pipeline = pipeline.fit(X=control_data.to_numpy())
         data[self.control_columns] = self.control_transformer.transform(
```

### Comparing `pymc-marketing-0.1.0/pymc_marketing/mmm/transformers.py` & `pymc-marketing-0.1.1/pymc_marketing/mmm/transformers.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.0/pymc_marketing/mmm/utils.py` & `pymc-marketing-0.1.1/pymc_marketing/mmm/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.0/pymc_marketing/mmm/validating.py` & `pymc-marketing-0.1.1/pymc_marketing/mmm/validating.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-from typing import Callable
+from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
 __all__ = [
     "validation_method",
     "ValidateControlColumns",
     "ValidateTargetColumn",
     "ValidateDateColumn",
     "ValidateChannelColumns",
 ]
 
 
 def validation_method(method: Callable) -> Callable:
     if not hasattr(method, "_tags"):
-        method._tags = {}
-    method._tags["validation"] = True
+        method._tags = {}  # type: ignore
+    method._tags["validation"] = True  # type: ignore
     return method
 
 
 class ValidateTargetColumn:
+    target_column: str
+
     @validation_method
     def validate_target(self, data: pd.DataFrame) -> None:
         if self.target_column not in data.columns:
             raise ValueError(f"target {self.target_column} not in data")
 
 
 class ValidateDateColumn:
+    date_column: str
+
     @validation_method
     def validate_date_col(self, data: pd.DataFrame) -> None:
         if self.date_column not in data.columns:
             raise ValueError(f"date_col {self.date_column} not in data")
         if not data[self.date_column].is_unique:
             raise ValueError(f"date_col {self.date_column} has repeated values")
 
 
 class ValidateChannelColumns:
+    channel_columns: Union[List[str], Tuple[str]]
+
     @validation_method
     def validate_channel_columns(self, data: pd.DataFrame) -> None:
         if not isinstance(self.channel_columns, (list, tuple)):
             raise ValueError("channel_columns must be a list or tuple")
         if len(self.channel_columns) == 0:
             raise ValueError("channel_columns must not be empty")
         if not set(self.channel_columns).issubset(data.columns):
             raise ValueError(f"channel_columns {self.channel_columns} not in data")
         if len(set(self.channel_columns)) != len(self.channel_columns):
             raise ValueError(
                 f"channel_columns {self.channel_columns} contains duplicates"
             )
-        if (data[self.channel_columns] < 0).any().any():
+        if (data.filter(list(self.channel_columns)) < 0).any().any():
             raise ValueError(
                 f"channel_columns {self.channel_columns} contains negative values"
             )
 
 
 class ValidateControlColumns:
+    control_columns: Optional[List[str]]
+
     @validation_method
     def validate_control_columns(self, data: pd.DataFrame) -> None:
         if self.control_columns is None:
             return None
         if not isinstance(self.control_columns, (list, tuple)):
             raise ValueError("control_columns must be None, a list or tuple")
         if len(self.control_columns) == 0:
```

### Comparing `pymc-marketing-0.1.0/pymc_marketing.egg-info/PKG-INFO` & `pymc-marketing-0.1.1/pymc_marketing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-marketing
-Version: 0.1.0
+Version: 0.1.1
 Summary: Marketing Statistical Models in PyMC
 Maintainer-email: PyMC Labs <info@pymc-labs.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,45 +209,43 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
-# PyMC-Marketing
+<div align="center">
+  <a href="https://github.com/pymc-labs/pymc-marketing"><img height="240px" src="docs/source/_static/marketing-logo-light.jpg"></a>
+</div>
+
+----
 
 ![Build](https://github.com/pymc-labs/pymc-marketing/workflows/ci/badge.svg)
 [![codecov](https://codecov.io/gh/pymc-labs/pymc-marketing/branch/main/graph/badge.svg?token=OBV3BS5TYE)](https://codecov.io/gh/pymc-labs/pymc-marketing)
 [![docs](https://readthedocs.org/projects/pymc-marketing/badge/?version=latest)](https://docs.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI Version](https://img.shields.io/pypi/v/pymc-marketing.svg)](https://pypi.python.org/pypi/pymc-marketing)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-**Unlock the power of marketing analytics with PyMC-Marketing – the open source solution for smarter decision-making.** Media mix modeling and customer lifetime value modules allow businesses to make data-driven decisions about their marketing campaigns. Optimize your marketing strategy and unlock the full potential of your customer data.
+# PyMC-Marketing
 
----
+**Unlock the power of marketing analytics with PyMC-Marketing – the open source solution for smarter decision-making.** Media mix modeling and customer lifetime value modules allow businesses to make data-driven decisions about their marketing campaigns. Optimize your marketing strategy and unlock the full potential of your customer data.
 
 ## Installation
 
-Start by setting up an environment (e.g. `marketing_env`) with PyMC. It may look something like the following:
+Install and activate an environment (e.g. `marketing_env`) with the `pymc-marketing` package from [conda-forge](https://conda-forge.org). It may look something like the following:
 
 ```bash
-mamba create -c conda-forge -n marketing_env python "pymc>=5"
+mamba create -c conda-forge -n marketing_env pymc-marketing
 mamba activate marketing_env
 ```
 
 See the official [PyMC installation guide](https://www.pymc.io/projects/docs/en/latest/installation.html) if more detail is needed.
 
-Assuming you have an environment set up then install PyMC-Marketing with the following command. This will give you the latest version of the library from PyPI.
-
-```bash
-pip install pymc-marketing
-```
-
-Alternatively you can install from GitHub directly:
+For testing purposes, if you wish to install the `main` branch directly from GitHub:
 
 ```bash
 pip install git+https://github.com/pymc-labs/pymc-marketing.git
 ```
 
 ## Bayesian Media Mix Models (MMMs) in PyMC
```

### Comparing `pymc-marketing-0.1.0/pymc_marketing.egg-info/SOURCES.txt` & `pymc-marketing-0.1.1/pymc_marketing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.1.0/pyproject.toml` & `pymc-marketing-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 maintainers = [{ name = "PyMC Labs", email = "info@pymc-labs.io" }]
 
 dependencies = [
     "arviz>=0.13.0",
     "matplotlib>=3.5.1",
     "numpy>=1.17",
     "pandas",
-    "pymc>=5.1.2",
+    # NOTE: Keep minimum pymc version in sync with ci.yml `OLDEST_PYMC_VERSION`
+    "pymc>=5.3.0",
     "scikit-learn>=1.1.1",
     "seaborn>=0.12.2",
     "xarray"
 ]
 
 [project.optional-dependencies]
 docs = [
@@ -35,14 +36,16 @@
     "sphinx-notfound-page",
     "sphinx-design"
 ]
 lint = [
     "black>=22.3.0",
     "flake8>=4.0.1",
     "isort>=5.10.1",
+    "mypy",
+    "pandas-stubs",
     "pre-commit>=2.19.0",
     "pylint"
 ]
 test = [
     "lifetimes==0.11.3",
     "pytest==7.0.1",
     "pytest-cov==3.0.0"
@@ -72,9 +75,10 @@
 [tool.pytest.ini_options]
 addopts = [
     "-v",
     "--strict-markers",
     "--strict-config",
     "--cov=pymc_marketing",
     "--cov-report=term-missing",
+    "--color=yes",
 ]
 testpaths = "tests"
```

