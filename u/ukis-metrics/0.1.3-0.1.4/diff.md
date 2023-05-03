# Comparing `tmp/ukis_metrics-0.1.3.tar.gz` & `tmp/ukis_metrics-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukis_metrics-0.1.3.tar", max compression
+gzip compressed data, was "ukis_metrics-0.1.4.tar", max compression
```

## Comparing `ukis_metrics-0.1.3.tar` & `ukis_metrics-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11438 2021-10-11 11:32:18.604217 ukis_metrics-0.1.3/LICENSE
--rw-r--r--   0        0        0     5762 2021-10-11 11:32:18.604217 ukis_metrics-0.1.3/README.md
--rw-r--r--   0        0        0      587 2021-10-11 11:32:18.616217 ukis_metrics-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       22 2021-10-11 11:32:18.616217 ukis_metrics-0.1.3/ukis_metrics/__init__.py
--rw-r--r--   0        0        0     4157 2021-10-11 11:32:18.616217 ukis_metrics-0.1.3/ukis_metrics/seg_metrics.py
--rw-r--r--   0        0        0     6620 2021-10-11 11:32:28.211187 ukis_metrics-0.1.3/setup.py
--rw-r--r--   0        0        0     6532 2021-10-11 11:32:28.211584 ukis_metrics-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11438 2023-05-03 13:51:46.173094 ukis_metrics-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5868 2023-05-03 13:51:46.173094 ukis_metrics-0.1.4/README.md
+-rw-r--r--   0        0        0      603 2023-05-03 13:51:46.185094 ukis_metrics-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-03 13:51:46.185094 ukis_metrics-0.1.4/ukis_metrics/__init__.py
+-rw-r--r--   0        0        0     4157 2023-05-03 13:51:46.185094 ukis_metrics-0.1.4/ukis_metrics/seg_metrics.py
+-rw-r--r--   0        0        0     6639 1970-01-01 00:00:00.000000 ukis_metrics-0.1.4/PKG-INFO
```

### Comparing `ukis_metrics-0.1.3/LICENSE` & `ukis_metrics-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ukis_metrics-0.1.3/README.md` & `ukis_metrics-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ![ukis-metrics](https://github.com/dlr-eoc/ukis-metrics/workflows/ukis-metrics/badge.svg)
 [![codecov](https://codecov.io/gh/dlr-eoc/ukis-metrics/branch/main/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-metrics)
 ![Upload Python Package](https://github.com/dlr-eoc/ukis-metrics/workflows/Upload%20Python%20Package/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ukis-metrics)](https://pypi.python.org/pypi/ukis-metrics/)
 [![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5561771.svg)](https://doi.org/10.5281/zenodo.5561771)
 
 A pure Numpy-based implementation of the most common performance metrics for semantic image segmentation. 
 
 ## Installation
 ```shell
 pip install ukis_metrics
 ```
```

### Comparing `ukis_metrics-0.1.3/ukis_metrics/seg_metrics.py` & `ukis_metrics-0.1.4/ukis_metrics/seg_metrics.py`

 * *Files identical despite different names*

### Comparing `ukis_metrics-0.1.3/setup.py` & `ukis_metrics-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,140 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ukis-metrics
+Version: 0.1.4
+Summary: Numpy-based implementation of common performance metrics for semantic image segmentation
+Home-page: https://github.com/dlr-eoc/ukis-metrics
+License: Apache 2.0
+Author: German Aerospace Center (DLR)
+Author-email: ukis-helpdesk@dlr.de
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Project-URL: Repository, https://github.com/dlr-eoc/ukis-metrics
+Description-Content-Type: text/markdown
+
+# [![UKIS](img/ukis-logo.png)](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) ukis-metrics
+
+![ukis-metrics](https://github.com/dlr-eoc/ukis-metrics/workflows/ukis-metrics/badge.svg)
+[![codecov](https://codecov.io/gh/dlr-eoc/ukis-metrics/branch/main/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-metrics)
+![Upload Python Package](https://github.com/dlr-eoc/ukis-metrics/workflows/Upload%20Python%20Package/badge.svg)
+[![PyPI version](https://img.shields.io/pypi/v/ukis-metrics)](https://pypi.python.org/pypi/ukis-metrics/)
+[![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5561771.svg)](https://doi.org/10.5281/zenodo.5561771)
+
+A pure Numpy-based implementation of the most common performance metrics for semantic image segmentation. 
+
+## Installation
+```shell
+pip install ukis_metrics
+```
+
+```shell
+>>> import ukis_metrics
+>>> ukis_metrics.__version__
+'0.1.3'
+```
+
+## Why?
+Simply because we wanted a lightweight and fast alternative to scikit learn for tracking during training. 
+
+[execution_time.py](https://github.com/dlr-eoc/ukis-metrics/blob/main/performance/execution_time.py)
+compares the execution time of ukis-metrics with sklearn. Here's an example output:
+```
+Shape of array: (256, 256, 2)
+
+                                        ### Metrics execution time [s] ###
+
+                ukis-metrics                            sklearn metrics         speed gain
+acc             0.001900                                0.007627                4.01
+rec             0.001716                                0.024509                14.28
+pre             0.001815                                0.025021                13.79
+f1              0.001798                                0.024770                13.78
+iou             0.001797                                0.024247                13.49
+kap             0.001824                                0.034577                18.96
+```
+
+## Workings and included metrics
+In a first step the **true positives** *tp*, **true negatives** *tn*, **false positives** *fp*, **false negatives** *fn*
+and the number of valid pixels **n_valid_pixels** are computed. These values are then used to compute the following 
+metrics:
+- Accuracy [1]:   
+  ```math
+  acc = \frac{tp + tn}{tp + fn + fp + tn}
+  ```
+- Recall [1]:
+  ```math
+  rec = \frac{tp}{tp + fn}
+  ```
+- Precision [1]:
+  ```math
+  prec = \frac{tp}{tp + fp}
+  ```
+- F1-score [2]:
+  ```math
+  F1 = \frac{2 * prec * rec}{prec + rec}
+  ```
+- IoU [3]:
+  ```math
+  IoU = \frac{tp}{tp + fp + fn}
+  ```  
+- Kappa: The computation of the Kappa-score incorporates several steps. Please refer to [4] for the full 
+  documentation
+
+## How to use
+Simply pass a Numpy ndarray to get a dict containing the `tpfptnfn` and pass the dict to `segmentation_metrics(tpfptnfn)`:
+```python 
+import ukis_metrics.seg_metrics as segm
+import numpy as np
+# ndarray containing the reference data, e.g.
+shape = (256, 256, 1)
+y_true = np.ones(shape)
+# ndarray containing the model predicions, e.g.
+y_pred = np.ones(shape)
+# get tp, fp, tn, fn an n_valid_pixel
+tpfptnfn = segm.tpfptnfn(y_true, y_pred, None)
+metrics = segm.segmentation_metrics(tpfptnfn)
+```
+So far these metrics were only used for binary classification, although one should be able to use them for 
+multiclass segmentation too, if the slices for a given class are provided individually.
+
+There is a [jupyter notebook](https://github.com/dlr-eoc/ukis-metrics/tree/main/examples) showing how ukis-metrics can be used and how it could be extended for multiclass problems.
+
+## References
+- [1] [Sokolova and Lapalme 2009: A systematic analysis of performance measures for classification tasks](https://www.researchgate.net/publication/222674734_A_systematic_analysis_of_performance_measures_for_classification_tasks)
+- [2] [scikit-learn](https://scikit-learn.org/stable/modules/model_evaluation.html)
+- [3] [Berman et al. 2018: The Lovász-Softmax loss: A tractable surrogate for the optimization of 
+  the intersection-over-union measure in neural networks](https://arxiv.org/pdf/1705.08790.pdf)
+- [4] [Tang et al. 2015: Kappa coefficient: a popular measure of rater agreement](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4372765/) 
+
+
+## Contributors
+The UKIS team creates and adapts libraries which simplify the usage of satellite data. Our team includes (in alphabetical order):
+* Fichtner, Florian
+* Helleis, Max
+* Martinis, Sandro
+* Wieland, Marc
+
+German Aerospace Center (DLR)
+
+## Licenses
+This software is licensed under the [Apache 2.0 License](https://github.com/dlr-eoc/ukis-metrics/blob/main/LICENSE).
+
+Copyright (c) 2021 German Aerospace Center (DLR) * German Remote Sensing Data Center * Department: Geo-Risks and Civil Security
+
+## Changelog
+See [changelog](https://github.com/dlr-eoc/ukis-metrics/blob/main/CHANGELOG.md).
 
-packages = \
-['ukis_metrics']
 
-package_data = \
-{'': ['*']}
+## What is UKIS?
+The DLR project Environmental and Crisis Information System (the German abbreviation is UKIS, standing for [Umwelt- und Kriseninformationssysteme](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) aims at harmonizing the development of information systems at the German Remote Sensing Data Center (DFD) and setting up a framework of modularized and generalized software components.
 
-install_requires = \
-['numpy>=1.20.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'ukis-metrics',
-    'version': '0.1.3',
-    'description': 'Numpy-based implementation of common performance metrics for semantic image segmentation',
-    'long_description': "# [![UKIS](img/ukis-logo.png)](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) ukis-metrics\n\n![ukis-metrics](https://github.com/dlr-eoc/ukis-metrics/workflows/ukis-metrics/badge.svg)\n[![codecov](https://codecov.io/gh/dlr-eoc/ukis-metrics/branch/main/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-metrics)\n![Upload Python Package](https://github.com/dlr-eoc/ukis-metrics/workflows/Upload%20Python%20Package/badge.svg)\n[![PyPI version](https://img.shields.io/pypi/v/ukis-metrics)](https://pypi.python.org/pypi/ukis-metrics/)\n[![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)\n[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)\n\nA pure Numpy-based implementation of the most common performance metrics for semantic image segmentation. \n\n## Installation\n```shell\npip install ukis_metrics\n```\n\n```shell\n>>> import ukis_metrics\n>>> ukis_metrics.__version__\n'0.1.3'\n```\n\n## Why?\nSimply because we wanted a lightweight and fast alternative to scikit learn for tracking during training. \n\n[execution_time.py](https://github.com/dlr-eoc/ukis-metrics/blob/main/performance/execution_time.py)\ncompares the execution time of ukis-metrics with sklearn. Here's an example output:\n```\nShape of array: (256, 256, 2)\n\n                                        ### Metrics execution time [s] ###\n\n                ukis-metrics                            sklearn metrics         speed gain\nacc             0.001900                                0.007627                4.01\nrec             0.001716                                0.024509                14.28\npre             0.001815                                0.025021                13.79\nf1              0.001798                                0.024770                13.78\niou             0.001797                                0.024247                13.49\nkap             0.001824                                0.034577                18.96\n```\n\n## Workings and included metrics\nIn a first step the **true positives** *tp*, **true negatives** *tn*, **false positives** *fp*, **false negatives** *fn*\nand the number of valid pixels **n_valid_pixels** are computed. These values are then used to compute the following \nmetrics:\n- Accuracy [1]:   \n  ```math\n  acc = \\frac{tp + tn}{tp + fn + fp + tn}\n  ```\n- Recall [1]:\n  ```math\n  rec = \\frac{tp}{tp + fn}\n  ```\n- Precision [1]:\n  ```math\n  prec = \\frac{tp}{tp + fp}\n  ```\n- F1-score [2]:\n  ```math\n  F1 = \\frac{2 * prec * rec}{prec + rec}\n  ```\n- IoU [3]:\n  ```math\n  IoU = \\frac{tp}{tp + fp + fn}\n  ```  \n- Kappa: The computation of the Kappa-score incorporates several steps. Please refer to [4] for the full \n  documentation\n\n## How to use\nSimply pass a Numpy ndarray to get a dict containing the `tpfptnfn` and pass the dict to `segmentation_metrics(tpfptnfn)`:\n```python \nimport ukis_metrics.seg_metrics as segm\nimport numpy as np\n# ndarray containing the reference data, e.g.\nshape = (256, 256, 1)\ny_true = np.ones(shape)\n# ndarray containing the model predicions, e.g.\ny_pred = np.ones(shape)\n# get tp, fp, tn, fn an n_valid_pixel\ntpfptnfn = segm.tpfptnfn(y_true, y_pred, None)\nmetrics = segm.segmentation_metrics(tpfptnfn)\n```\nSo far these metrics were only used for binary classification, although one should be able to use them for \nmulticlass segmentation too, if the slices for a given class are provided individually.\n\nThere is a [jupyter notebook](https://github.com/dlr-eoc/ukis-metrics/tree/main/examples) showing how ukis-metrics can be used and how it could be extended for multiclass problems.\n\n## References\n- [1] [Sokolova and Lapalme 2009: A systematic analysis of performance measures for classification tasks](https://www.researchgate.net/publication/222674734_A_systematic_analysis_of_performance_measures_for_classification_tasks)\n- [2] [scikit-learn](https://scikit-learn.org/stable/modules/model_evaluation.html)\n- [3] [Berman et al. 2018: The Lovász-Softmax loss: A tractable surrogate for the optimization of \n  the intersection-over-union measure in neural networks](https://arxiv.org/pdf/1705.08790.pdf)\n- [4] [Tang et al. 2015: Kappa coefficient: a popular measure of rater agreement](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4372765/) \n\n\n## Contributors\nThe UKIS team creates and adapts libraries which simplify the usage of satellite data. Our team includes (in alphabetical order):\n* Fichtner, Florian\n* Helleis, Max\n* Martinis, Sandro\n* Wieland, Marc\n\nGerman Aerospace Center (DLR)\n\n## Licenses\nThis software is licensed under the [Apache 2.0 License](https://github.com/dlr-eoc/ukis-metrics/blob/main/LICENSE).\n\nCopyright (c) 2021 German Aerospace Center (DLR) * German Remote Sensing Data Center * Department: Geo-Risks and Civil Security\n\n## Changelog\nSee [changelog](https://github.com/dlr-eoc/ukis-metrics/blob/main/CHANGELOG.md).\n\n\n## What is UKIS?\nThe DLR project Environmental and Crisis Information System (the German abbreviation is UKIS, standing for [Umwelt- und Kriseninformationssysteme](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) aims at harmonizing the development of information systems at the German Remote Sensing Data Center (DFD) and setting up a framework of modularized and generalized software components.\n\nUKIS is intended to ease and standardize the process of setting up specific information systems and thus bridging the gap from EO product generation and information fusion to the delivery of products and information to end users.\n\nFurthermore, the intention is to save and broaden know-how that was and is invested and earned in the development of information systems and components in several ongoing and future DFD projects.\n",
-    'author': 'German Aerospace Center (DLR)',
-    'author_email': 'ukis-helpdesk@dlr.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/dlr-eoc/ukis-metrics',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+UKIS is intended to ease and standardize the process of setting up specific information systems and thus bridging the gap from EO product generation and information fusion to the delivery of products and information to end users.
 
+Furthermore, the intention is to save and broaden know-how that was and is invested and earned in the development of information systems and components in several ongoing and future DFD projects.
 
-setup(**setup_kwargs)
```

