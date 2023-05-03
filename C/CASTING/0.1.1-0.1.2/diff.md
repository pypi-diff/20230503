# Comparing `tmp/CASTING-0.1.1.tar.gz` & `tmp/CASTING-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CASTING-0.1.1.tar", last modified: Wed Jan 18 05:25:43 2023, max compression
+gzip compressed data, was "CASTING-0.1.2.tar", last modified: Wed May  3 07:32:16 2023, max compression
```

## Comparing `CASTING-0.1.1.tar` & `CASTING-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,69 @@
-drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-01-18 05:25:43.553677 CASTING-0.1.1/
-drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-01-18 05:25:43.550251 CASTING-0.1.1/CASTING/
--rw-rw----   0 sbanik   (92023) m3560    (91515)     5482 2023-01-18 05:25:00.000000 CASTING-0.1.1/CASTING/MCTS.py
--rw-rw----   0 sbanik   (92023) m3560    (91515)       46 2023-01-18 05:25:00.000000 CASTING-0.1.1/CASTING/__init__.py
--rw-rw----   0 sbanik   (92023) m3560    (91515)     6001 2023-01-18 05:25:00.000000 CASTING-0.1.1/CASTING/clusterfun.py
--rw-rw----   0 sbanik   (92023) m3560    (91515)     2609 2023-01-18 05:25:00.000000 CASTING-0.1.1/CASTING/lammpsEvaluate.py
--rw-rw----   0 sbanik   (92023) m3560    (91515)      873 2023-01-18 05:25:00.000000 CASTING-0.1.1/CASTING/perturb.py
--rw-rw----   0 sbanik   (92023) m3560    (91515)     1890 2023-01-18 05:25:00.000000 CASTING-0.1.1/CASTING/utilis.py
--rw-rw----   0 sbanik   (92023) m3560    (91515)     2774 2023-01-18 05:25:00.000000 CASTING-0.1.1/CASTING/writer.py
-drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-01-18 05:25:43.552793 CASTING-0.1.1/CASTING.egg-info/
--rw-rw----   0 sbanik   (92023) m3560    (91515)     8587 2023-01-18 05:25:43.550895 CASTING-0.1.1/CASTING.egg-info/PKG-INFO
--rw-rw----   0 sbanik   (92023) m3560    (91515)      334 2023-01-18 05:25:43.551390 CASTING-0.1.1/CASTING.egg-info/SOURCES.txt
--rw-rw----   0 sbanik   (92023) m3560    (91515)        1 2023-01-18 05:25:43.551833 CASTING-0.1.1/CASTING.egg-info/dependency_links.txt
--rw-rw----   0 sbanik   (92023) m3560    (91515)      100 2023-01-18 05:25:43.552419 CASTING-0.1.1/CASTING.egg-info/requires.txt
--rw-rw----   0 sbanik   (92023) m3560    (91515)        8 2023-01-18 05:25:43.552912 CASTING-0.1.1/CASTING.egg-info/top_level.txt
--rw-rw----   0 sbanik   (92023) m3560    (91515)     1067 2023-01-18 05:25:00.000000 CASTING-0.1.1/LICENSE
--rw-rw----   0 sbanik   (92023) m3560    (91515)     8587 2023-01-18 05:25:43.553327 CASTING-0.1.1/PKG-INFO
--rw-rw----   0 sbanik   (92023) m3560    (91515)     8120 2023-01-18 05:25:00.000000 CASTING-0.1.1/README.md
--rw-rw----   0 sbanik   (92023) m3560    (91515)      700 2023-01-18 05:25:00.000000 CASTING-0.1.1/pyproject.toml
--rw-rw----   0 sbanik   (92023) m3560    (91515)       38 2023-01-18 05:25:43.553793 CASTING-0.1.1/setup.cfg
--rw-rw----   0 sbanik   (92023) m3560    (91515)     1140 2023-01-18 05:25:00.000000 CASTING-0.1.1/setup.py
+drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 07:32:16.174963 CASTING-0.1.2/
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1799 2023-05-03 04:35:48.000000 CASTING-0.1.2/.gitignore
+drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 07:32:16.135962 CASTING-0.1.2/CASTING/
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     5482 2023-05-03 04:35:48.000000 CASTING-0.1.2/CASTING/MCTS.py
+-rw-rw----   0 sbanik   (92023) m3560    (91515)       46 2023-05-03 07:29:07.000000 CASTING-0.1.2/CASTING/__init__.py
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     2079 2023-05-03 07:09:39.000000 CASTING-0.1.2/CASTING/aseEamEvaluate.py
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     6001 2023-05-03 04:35:48.000000 CASTING-0.1.2/CASTING/clusterfun.py
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     2609 2023-05-03 04:35:48.000000 CASTING-0.1.2/CASTING/lammpsEvaluate.py
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      873 2023-05-03 04:35:48.000000 CASTING-0.1.2/CASTING/perturb.py
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1890 2023-05-03 04:35:48.000000 CASTING-0.1.2/CASTING/utilis.py
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     2774 2023-05-03 04:35:48.000000 CASTING-0.1.2/CASTING/writer.py
+drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 07:32:16.138443 CASTING-0.1.2/CASTING.egg-info/
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     8622 2023-05-03 07:32:15.000000 CASTING-0.1.2/CASTING.egg-info/PKG-INFO
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1206 2023-05-03 07:32:16.137111 CASTING-0.1.2/CASTING.egg-info/SOURCES.txt
+-rw-rw----   0 sbanik   (92023) m3560    (91515)        1 2023-05-03 07:32:15.000000 CASTING-0.1.2/CASTING.egg-info/dependency_links.txt
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      100 2023-05-03 07:32:15.000000 CASTING-0.1.2/CASTING.egg-info/requires.txt
+-rw-rw----   0 sbanik   (92023) m3560    (91515)        8 2023-05-03 07:32:15.000000 CASTING-0.1.2/CASTING.egg-info/top_level.txt
+drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 07:32:16.139453 CASTING-0.1.2/C_dataset/
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     3103 2023-05-03 04:35:48.000000 CASTING-0.1.2/C_dataset/info.csv
+-rw-rw----   0 sbanik   (92023) m3560    (91515)    19899 2023-05-03 04:35:48.000000 CASTING-0.1.2/C_dataset/poscars.zip
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1067 2023-05-03 04:35:48.000000 CASTING-0.1.2/LICENSE
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     8622 2023-05-03 07:32:16.174480 CASTING-0.1.2/PKG-INFO
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     8155 2023-05-03 04:35:48.000000 CASTING-0.1.2/README.md
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      386 2023-05-03 04:35:48.000000 CASTING-0.1.2/citations.bib
+drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 07:32:16.145004 CASTING-0.1.2/docs/
+-rw-rw----   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/.nojekyll
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      962 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/Example1.md
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      441 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/Example2.md
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      629 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/Installation.md
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1935 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/README.md
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      239 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/_coverpage.md
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      198 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/_sidebar.md
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      533 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/citation.md
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      895 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/index.html
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      272 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/prerequisites.md
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     3314 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/puzzle.png
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     2973 2023-05-03 04:35:48.000000 CASTING-0.1.2/docs/running-the-code.md
+drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 07:32:16.156309 CASTING-0.1.2/example/
+-rw-rw----   0 sbanik   (92023) m3560    (91515)  1790882 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/Au.eam
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1422 2023-05-03 07:09:45.000000 CASTING-0.1.2/example/RunOPt.py
+-rw-rw----   0 sbanik   (92023) m3560    (91515)   157328 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/dumpfile.dat
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      215 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/energy.dat
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      313 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/extract.py
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      660 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/in.data
+-rw-rw----   0 sbanik   (92023) m3560    (91515)   959482 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/log.lammps
+-rw-rw----   0 sbanik   (92023) m3560    (91515)   909312 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/log.screen
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1148 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/min.geo
+drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 07:32:16.166187 CASTING-0.1.2/example/structures/
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/0.POSCAR
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/1.POSCAR
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/2.POSCAR
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/3.POSCAR
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/4.POSCAR
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/5.POSCAR
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/6.POSCAR
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/7.POSCAR
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/8.POSCAR
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1117 2023-05-03 04:35:48.000000 CASTING-0.1.2/example/structures/9.POSCAR
+drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 07:32:16.169275 CASTING-0.1.2/figs/
+-rw-rw----   0 sbanik   (92023) m3560    (91515)   348649 2023-05-03 04:35:48.000000 CASTING-0.1.2/figs/MCTS.png
+-rw-rw----   0 sbanik   (92023) m3560    (91515)   532150 2023-05-03 04:35:48.000000 CASTING-0.1.2/figs/MetastableC.png
+-rw-rw----   0 sbanik   (92023) m3560    (91515)   175208 2023-05-03 04:35:48.000000 CASTING-0.1.2/figs/sutton_chen.gif
+drwxrws---   0 sbanik   (92023) m3560    (91515)        0 2023-05-03 07:32:16.173545 CASTING-0.1.2/notebooks/
+-rw-rw----   0 sbanik   (92023) m3560    (91515)  1790882 2023-05-03 07:10:20.000000 CASTING-0.1.2/notebooks/Au.eam
+-rw-rw----   0 sbanik   (92023) m3560    (91515)    18924 2023-05-03 07:23:55.000000 CASTING-0.1.2/notebooks/Au_example_Ase.ipynb
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      700 2023-05-03 07:29:19.000000 CASTING-0.1.2/pyproject.toml
+-rw-rw----   0 sbanik   (92023) m3560    (91515)      101 2023-05-03 04:35:48.000000 CASTING-0.1.2/requirements.txt
+-rw-rw----   0 sbanik   (92023) m3560    (91515)       38 2023-05-03 07:32:16.175109 CASTING-0.1.2/setup.cfg
+-rw-rw----   0 sbanik   (92023) m3560    (91515)     1140 2023-05-03 07:29:32.000000 CASTING-0.1.2/setup.py
```

### Comparing `CASTING-0.1.1/CASTING/MCTS.py` & `CASTING-0.1.2/CASTING/MCTS.py`

 * *Files identical despite different names*

### Comparing `CASTING-0.1.1/CASTING/clusterfun.py` & `CASTING-0.1.2/CASTING/clusterfun.py`

 * *Files identical despite different names*

### Comparing `CASTING-0.1.1/CASTING/lammpsEvaluate.py` & `CASTING-0.1.2/CASTING/lammpsEvaluate.py`

 * *Files identical despite different names*

### Comparing `CASTING-0.1.1/CASTING/perturb.py` & `CASTING-0.1.2/CASTING/perturb.py`

 * *Files identical despite different names*

### Comparing `CASTING-0.1.1/CASTING/utilis.py` & `CASTING-0.1.2/CASTING/utilis.py`

 * *Files identical despite different names*

### Comparing `CASTING-0.1.1/CASTING/writer.py` & `CASTING-0.1.2/CASTING/writer.py`

 * *Files identical despite different names*

### Comparing `CASTING-0.1.1/CASTING.egg-info/PKG-INFO` & `CASTING-0.1.2/CASTING.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CASTING
-Version: 0.1.1
+Version: 0.1.2
 Summary: A continuous action space tree search for inverse design (CASTING)
 Home-page: https://github.com/sbanik2/CASTING
 Author: Suvo Banik
 Author-email: Suvo Banik <sbanik2@uic.edu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,16 +17,17 @@
 <a name="readme-top"></a>
 
 
 ![Release][release-shield]
 [![License][license-shield]][license-url]
 ![Commit][commit-shield]
 ![Size][size-shield]
+[![Downloads][download-shield]][download-url]
 [![Doi][DOI-shield]][DOI-url]
-<!-- ![Downloads][download-shield] -->
+
 
 
 
 
 # CASTING 
 
 <p align="justify"> A Continuous Action Space Tree search for INverse desiGn (CASTING) Framework and Materials Discovery</p>
@@ -250,14 +251,15 @@
     
 <!--LINKS -->
 
 
 [release-shield]: https://img.shields.io/github/v/release/sbanik2/CASTING
 [license-shield]: https://img.shields.io/github/license/sbanik2/CASTING
 [license-url]: https://github.com/sbanik2/CASTING/blob/main/LICENSE
-[download-shield]: https://img.shields.io/github/downloads/sbanik2/CASTING/total
+[download-shield]: https://static.pepy.tech/badge/casting
+[download-url]: https://pepy.tech/project/casting
 [commit-shield]:https://img.shields.io/github/last-commit/sbanik2/CASTING
 [size-shield]: https://img.shields.io/github/languages/code-size/sbanik2/CASTING
 [DOI-shield]: https://img.shields.io/badge/DOI-doi.org/10.48550/arXiv.2212.12106-red
 [DOI-url]: https://doi.org/10.48550/arXiv.2212.12106
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: CASTING Version: 0.1.1 Summary: A continuous action
+Metadata-Version: 2.1 Name: CASTING Version: 0.1.2 Summary: A continuous action
 space tree search for inverse design (CASTING) Home-page: https://github.com/
 sbanik2/CASTING Author: Suvo Banik Author-email: Suvo Banik
 uic.edu> Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE  ![Release][release-shield] [![License][license-shield]][license-url] !
-[Commit][commit-shield] ![Size][size-shield] [![Doi][DOI-shield]][DOI-url]  #
-CASTING
+[Commit][commit-shield] ![Size][size-shield] [![Downloads][download-shield]]
+[download-url] [![Doi][DOI-shield]][DOI-url] # CASTING
 A Continuous Action Space Tree search for INverse desiGn (CASTING) Framework
 and Materials Discovery
 ## Table of Contents - [Introduction](#Introduction) - [Prerequisites]
 (#prerequisites) - [Installation](#installation) - [Running the code](#running-
 the-code) - [Optimization of Gold nanocluster](#optimization-of-Gold-
 nanocluster) - [Carbon metastable polymorphs](#carbon-metastable-polymorphs) -
 [Citation](#citation) - [License](#license) ## Introduction A pseudocode
@@ -99,12 +99,13 @@
 year={2022} } ```
                                                                   (back_to_top)
 ## License CASTING is distributed under MIT License. See `LICENSE` for details.
                                                                   (back_to_top)
  [release-shield]: https://img.shields.io/github/v/release/sbanik2/CASTING
 [license-shield]: https://img.shields.io/github/license/sbanik2/CASTING
 [license-url]: https://github.com/sbanik2/CASTING/blob/main/LICENSE [download-
-shield]: https://img.shields.io/github/downloads/sbanik2/CASTING/total [commit-
-shield]:https://img.shields.io/github/last-commit/sbanik2/CASTING [size-
-shield]: https://img.shields.io/github/languages/code-size/sbanik2/CASTING
-[DOI-shield]: https://img.shields.io/badge/DOI-doi.org/10.48550/
-arXiv.2212.12106-red [DOI-url]: https://doi.org/10.48550/arXiv.2212.12106
+shield]: https://static.pepy.tech/badge/casting [download-url]: https://
+pepy.tech/project/casting [commit-shield]:https://img.shields.io/github/last-
+commit/sbanik2/CASTING [size-shield]: https://img.shields.io/github/languages/
+code-size/sbanik2/CASTING [DOI-shield]: https://img.shields.io/badge/DOI-
+doi.org/10.48550/arXiv.2212.12106-red [DOI-url]: https://doi.org/10.48550/
+arXiv.2212.12106
```

### Comparing `CASTING-0.1.1/LICENSE` & `CASTING-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CASTING-0.1.1/PKG-INFO` & `CASTING-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CASTING
-Version: 0.1.1
+Version: 0.1.2
 Summary: A continuous action space tree search for inverse design (CASTING)
 Home-page: https://github.com/sbanik2/CASTING
 Author: Suvo Banik
 Author-email: Suvo Banik <sbanik2@uic.edu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,16 +17,17 @@
 <a name="readme-top"></a>
 
 
 ![Release][release-shield]
 [![License][license-shield]][license-url]
 ![Commit][commit-shield]
 ![Size][size-shield]
+[![Downloads][download-shield]][download-url]
 [![Doi][DOI-shield]][DOI-url]
-<!-- ![Downloads][download-shield] -->
+
 
 
 
 
 # CASTING 
 
 <p align="justify"> A Continuous Action Space Tree search for INverse desiGn (CASTING) Framework and Materials Discovery</p>
@@ -250,14 +251,15 @@
     
 <!--LINKS -->
 
 
 [release-shield]: https://img.shields.io/github/v/release/sbanik2/CASTING
 [license-shield]: https://img.shields.io/github/license/sbanik2/CASTING
 [license-url]: https://github.com/sbanik2/CASTING/blob/main/LICENSE
-[download-shield]: https://img.shields.io/github/downloads/sbanik2/CASTING/total
+[download-shield]: https://static.pepy.tech/badge/casting
+[download-url]: https://pepy.tech/project/casting
 [commit-shield]:https://img.shields.io/github/last-commit/sbanik2/CASTING
 [size-shield]: https://img.shields.io/github/languages/code-size/sbanik2/CASTING
 [DOI-shield]: https://img.shields.io/badge/DOI-doi.org/10.48550/arXiv.2212.12106-red
 [DOI-url]: https://doi.org/10.48550/arXiv.2212.12106
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: CASTING Version: 0.1.1 Summary: A continuous action
+Metadata-Version: 2.1 Name: CASTING Version: 0.1.2 Summary: A continuous action
 space tree search for inverse design (CASTING) Home-page: https://github.com/
 sbanik2/CASTING Author: Suvo Banik Author-email: Suvo Banik
 uic.edu> Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE  ![Release][release-shield] [![License][license-shield]][license-url] !
-[Commit][commit-shield] ![Size][size-shield] [![Doi][DOI-shield]][DOI-url]  #
-CASTING
+[Commit][commit-shield] ![Size][size-shield] [![Downloads][download-shield]]
+[download-url] [![Doi][DOI-shield]][DOI-url] # CASTING
 A Continuous Action Space Tree search for INverse desiGn (CASTING) Framework
 and Materials Discovery
 ## Table of Contents - [Introduction](#Introduction) - [Prerequisites]
 (#prerequisites) - [Installation](#installation) - [Running the code](#running-
 the-code) - [Optimization of Gold nanocluster](#optimization-of-Gold-
 nanocluster) - [Carbon metastable polymorphs](#carbon-metastable-polymorphs) -
 [Citation](#citation) - [License](#license) ## Introduction A pseudocode
@@ -99,12 +99,13 @@
 year={2022} } ```
                                                                   (back_to_top)
 ## License CASTING is distributed under MIT License. See `LICENSE` for details.
                                                                   (back_to_top)
  [release-shield]: https://img.shields.io/github/v/release/sbanik2/CASTING
 [license-shield]: https://img.shields.io/github/license/sbanik2/CASTING
 [license-url]: https://github.com/sbanik2/CASTING/blob/main/LICENSE [download-
-shield]: https://img.shields.io/github/downloads/sbanik2/CASTING/total [commit-
-shield]:https://img.shields.io/github/last-commit/sbanik2/CASTING [size-
-shield]: https://img.shields.io/github/languages/code-size/sbanik2/CASTING
-[DOI-shield]: https://img.shields.io/badge/DOI-doi.org/10.48550/
-arXiv.2212.12106-red [DOI-url]: https://doi.org/10.48550/arXiv.2212.12106
+shield]: https://static.pepy.tech/badge/casting [download-url]: https://
+pepy.tech/project/casting [commit-shield]:https://img.shields.io/github/last-
+commit/sbanik2/CASTING [size-shield]: https://img.shields.io/github/languages/
+code-size/sbanik2/CASTING [DOI-shield]: https://img.shields.io/badge/DOI-
+doi.org/10.48550/arXiv.2212.12106-red [DOI-url]: https://doi.org/10.48550/
+arXiv.2212.12106
```

### Comparing `CASTING-0.1.1/README.md` & `CASTING-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 <a name="readme-top"></a>
 
 
 ![Release][release-shield]
 [![License][license-shield]][license-url]
 ![Commit][commit-shield]
 ![Size][size-shield]
+[![Downloads][download-shield]][download-url]
 [![Doi][DOI-shield]][DOI-url]
-<!-- ![Downloads][download-shield] -->
+
 
 
 
 
 # CASTING 
 
 <p align="justify"> A Continuous Action Space Tree search for INverse desiGn (CASTING) Framework and Materials Discovery</p>
@@ -236,14 +237,15 @@
     
 <!--LINKS -->
 
 
 [release-shield]: https://img.shields.io/github/v/release/sbanik2/CASTING
 [license-shield]: https://img.shields.io/github/license/sbanik2/CASTING
 [license-url]: https://github.com/sbanik2/CASTING/blob/main/LICENSE
-[download-shield]: https://img.shields.io/github/downloads/sbanik2/CASTING/total
+[download-shield]: https://static.pepy.tech/badge/casting
+[download-url]: https://pepy.tech/project/casting
 [commit-shield]:https://img.shields.io/github/last-commit/sbanik2/CASTING
 [size-shield]: https://img.shields.io/github/languages/code-size/sbanik2/CASTING
 [DOI-shield]: https://img.shields.io/badge/DOI-doi.org/10.48550/arXiv.2212.12106-red
 [DOI-url]: https://doi.org/10.48550/arXiv.2212.12106
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
   ![Release][release-shield] [![License][license-shield]][license-url] !
-[Commit][commit-shield] ![Size][size-shield] [![Doi][DOI-shield]][DOI-url]  #
-CASTING
+[Commit][commit-shield] ![Size][size-shield] [![Downloads][download-shield]]
+[download-url] [![Doi][DOI-shield]][DOI-url] # CASTING
 A Continuous Action Space Tree search for INverse desiGn (CASTING) Framework
 and Materials Discovery
 ## Table of Contents - [Introduction](#Introduction) - [Prerequisites]
 (#prerequisites) - [Installation](#installation) - [Running the code](#running-
 the-code) - [Optimization of Gold nanocluster](#optimization-of-Gold-
 nanocluster) - [Carbon metastable polymorphs](#carbon-metastable-polymorphs) -
 [Citation](#citation) - [License](#license) ## Introduction A pseudocode
@@ -93,12 +93,13 @@
 year={2022} } ```
                                                                   (back_to_top)
 ## License CASTING is distributed under MIT License. See `LICENSE` for details.
                                                                   (back_to_top)
  [release-shield]: https://img.shields.io/github/v/release/sbanik2/CASTING
 [license-shield]: https://img.shields.io/github/license/sbanik2/CASTING
 [license-url]: https://github.com/sbanik2/CASTING/blob/main/LICENSE [download-
-shield]: https://img.shields.io/github/downloads/sbanik2/CASTING/total [commit-
-shield]:https://img.shields.io/github/last-commit/sbanik2/CASTING [size-
-shield]: https://img.shields.io/github/languages/code-size/sbanik2/CASTING
-[DOI-shield]: https://img.shields.io/badge/DOI-doi.org/10.48550/
-arXiv.2212.12106-red [DOI-url]: https://doi.org/10.48550/arXiv.2212.12106
+shield]: https://static.pepy.tech/badge/casting [download-url]: https://
+pepy.tech/project/casting [commit-shield]:https://img.shields.io/github/last-
+commit/sbanik2/CASTING [size-shield]: https://img.shields.io/github/languages/
+code-size/sbanik2/CASTING [DOI-shield]: https://img.shields.io/badge/DOI-
+doi.org/10.48550/arXiv.2212.12106-red [DOI-url]: https://doi.org/10.48550/
+arXiv.2212.12106
```

### Comparing `CASTING-0.1.1/pyproject.toml` & `CASTING-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CASTING"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Suvo Banik", email="sbanik2@uic.edu" },
 ]
 dependencies = [
             "ase>=3.21.1",
             "networkx>=2.0",
             "numpy>=1.23.1",
```

### Comparing `CASTING-0.1.1/setup.py` & `CASTING-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="CASTING",
-    version="0.1.1",  
+    version="0.1.2",  
     description="A continuous action spce tree search for inverse design",
     author="Suvo Banik",
     author_email="sbanik2@uic.edu", 
     install_requires=[
             "ase>=3.21.1",
             "networkx>=2.0",
             "numpy>=1.23.1",
```

