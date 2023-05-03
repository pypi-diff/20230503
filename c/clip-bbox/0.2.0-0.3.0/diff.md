# Comparing `tmp/clip_bbox-0.2.0.tar.gz` & `tmp/clip_bbox-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clip_bbox-0.2.0.tar", last modified: Wed Apr  5 04:03:49 2023, max compression
+gzip compressed data, was "clip_bbox-0.3.0.tar", last modified: Wed May  3 15:13:05 2023, max compression
```

## Comparing `clip_bbox-0.2.0.tar` & `clip_bbox-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,50 @@
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-04-05 04:03:49.189372 clip_bbox-0.2.0/
--rw-rw----   0 gsu      (20682) gsu      (24121)      528 2023-04-05 03:55:30.000000 clip_bbox-0.2.0/.bumpversion.cfg
--rw-rw----   0 gsu      (20682) gsu      (24121)     1804 2023-04-05 02:04:28.000000 clip_bbox-0.2.0/CONTRIBUTING.md
--rw-rw----   0 gsu      (20682) gsu      (24121)    11357 2023-04-05 01:37:03.000000 clip_bbox-0.2.0/LICENSE
--rw-rw----   0 gsu      (20682) gsu      (24121)      679 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/MANIFEST.in
--rw-rw----   0 gsu      (20682) gsu      (24121)     2620 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/Makefile
--rw-rw----   0 gsu      (20682) gsu      (24121)    15738 2023-04-05 04:03:49.189372 clip_bbox-0.2.0/PKG-INFO
--rw-rw----   0 gsu      (20682) gsu      (24121)     1911 2023-04-05 02:04:28.000000 clip_bbox-0.2.0/README.md
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-04-05 04:03:49.185372 clip_bbox-0.2.0/clip_bbox/
--rw-rw----   0 gsu      (20682) gsu      (24121)       47 2023-04-05 03:55:30.000000 clip_bbox-0.2.0/clip_bbox/__init__.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     6873 2023-04-05 02:04:28.000000 clip_bbox-0.2.0/clip_bbox/bbox_utils.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     9320 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/clip_bbox/clip.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     2484 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/clip_bbox/clip_model_setup.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     3231 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/clip_bbox/clipbbox.py
--rw-rw----   0 gsu      (20682) gsu      (24121)    18740 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/clip_bbox/model.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     1239 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/clip_bbox/newpad.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     3002 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/clip_bbox/preprocess.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     4740 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/clip_bbox/simple_tokenizer.py
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-04-05 04:03:49.185372 clip_bbox-0.2.0/clip_bbox/tests/
--rw-rw----   0 gsu      (20682) gsu      (24121)      541 2023-04-05 03:35:06.000000 clip_bbox-0.2.0/clip_bbox/tests/test_all.py
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-04-05 04:03:49.185372 clip_bbox-0.2.0/clip_bbox.egg-info/
--rw-rw----   0 gsu      (20682) gsu      (24121)    15738 2023-04-05 04:03:49.000000 clip_bbox-0.2.0/clip_bbox.egg-info/PKG-INFO
--rw-rw----   0 gsu      (20682) gsu      (24121)      678 2023-04-05 04:03:49.000000 clip_bbox-0.2.0/clip_bbox.egg-info/SOURCES.txt
--rw-rw----   0 gsu      (20682) gsu      (24121)        1 2023-04-05 04:03:49.000000 clip_bbox-0.2.0/clip_bbox.egg-info/dependency_links.txt
--rw-rw----   0 gsu      (20682) gsu      (24121)      229 2023-04-05 04:03:49.000000 clip_bbox-0.2.0/clip_bbox.egg-info/requires.txt
--rw-rw----   0 gsu      (20682) gsu      (24121)       10 2023-04-05 04:03:49.000000 clip_bbox-0.2.0/clip_bbox.egg-info/top_level.txt
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-04-05 04:03:49.185372 clip_bbox-0.2.0/docs/
--rw-rw----   0 gsu      (20682) gsu      (24121)      638 2023-04-05 02:04:28.000000 clip_bbox-0.2.0/docs/Makefile
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-04-05 04:03:49.185372 clip_bbox-0.2.0/docs/images/
--rw-rw----   0 gsu      (20682) gsu      (24121)   330320 2023-04-05 02:04:28.000000 clip_bbox-0.2.0/docs/images/example_output.png
--rw-rw----   0 gsu      (20682) gsu      (24121)      840 2023-04-05 03:41:23.000000 clip_bbox-0.2.0/docs/index.md
--rw-rw----   0 gsu      (20682) gsu      (24121)      804 2023-04-05 02:04:28.000000 clip_bbox-0.2.0/docs/make.bat
--rw-rw----   0 gsu      (20682) gsu      (24121)      100 2023-04-05 03:55:30.000000 clip_bbox-0.2.0/docs/requirements.txt
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-04-05 04:03:49.189372 clip_bbox-0.2.0/docs/source/
--rw-rw----   0 gsu      (20682) gsu      (24121)      327 2023-04-05 03:41:23.000000 clip_bbox-0.2.0/docs/source/clip_bbox.rst
--rw-rw----   0 gsu      (20682) gsu      (24121)     1476 2023-04-05 03:55:30.000000 clip_bbox-0.2.0/docs/source/conf.py
--rw-rw----   0 gsu      (20682) gsu      (24121)       66 2023-04-05 03:41:23.000000 clip_bbox-0.2.0/docs/source/modules.rst
--rw-rw----   0 gsu      (20682) gsu      (24121)     2421 2023-04-05 03:55:30.000000 clip_bbox-0.2.0/pyproject.toml
--rw-rw----   0 gsu      (20682) gsu      (24121)      106 2023-04-05 02:04:28.000000 clip_bbox-0.2.0/requirements.txt
--rw-rw----   0 gsu      (20682) gsu      (24121)       38 2023-04-05 04:03:49.189372 clip_bbox-0.2.0/setup.cfg
--rw-rw----   0 gsu      (20682) gsu      (24121)       39 2023-04-05 01:37:03.000000 clip_bbox-0.2.0/setup.py
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.323311 clip_bbox-0.3.0/
+-rw-rw----   0 gsu      (20682) gsu      (24121)      528 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/.bumpversion.cfg
+-rw-rw----   0 gsu      (20682) gsu      (24121)      123 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/.coveragerc
+-rw-rw----   0 gsu      (20682) gsu      (24121)     1804 2023-04-05 02:04:28.000000 clip_bbox-0.3.0/CONTRIBUTING.md
+-rw-rw----   0 gsu      (20682) gsu      (24121)    11357 2023-04-05 01:37:03.000000 clip_bbox-0.3.0/LICENSE
+-rw-rw----   0 gsu      (20682) gsu      (24121)      681 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/MANIFEST.in
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2402 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/Makefile
+-rw-rw----   0 gsu      (20682) gsu      (24121)    16565 2023-05-03 15:13:05.323311 clip_bbox-0.3.0/PKG-INFO
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2738 2023-05-02 21:26:04.000000 clip_bbox-0.3.0/README.md
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.295311 clip_bbox-0.3.0/clip_bbox/
+-rw-rw----   0 gsu      (20682) gsu      (24121)       47 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/clip_bbox/__init__.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)      638 2023-05-02 21:26:04.000000 clip_bbox-0.3.0/clip_bbox/__main__.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     6884 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/bbox_utils.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     9375 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/clip.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2600 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/clip_model_setup.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     3526 2023-05-02 21:26:04.000000 clip_bbox-0.3.0/clip_bbox/clipbbox.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)    18878 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/model.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     1239 2023-04-05 03:35:06.000000 clip_bbox-0.3.0/clip_bbox/newpad.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2601 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/clip_bbox/preprocess.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     4740 2023-04-05 03:35:06.000000 clip_bbox-0.3.0/clip_bbox/simple_tokenizer.py
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.299311 clip_bbox-0.3.0/clip_bbox/tests/
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.315311 clip_bbox-0.3.0/clip_bbox/tests/assets/
+-rw-rw----   0 gsu      (20682) gsu      (24121)     3784 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/tests/assets/heat.npz
+-rw-rw----   0 gsu      (20682) gsu      (24121) 11059328 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/tests/assets/rocket.npy
+-rw-rw----   0 gsu      (20682) gsu      (24121)   302557 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/tests/assets/rocket.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)   342530 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/tests/assets/test_all-gt_output.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)     3740 2023-05-02 21:26:04.000000 clip_bbox-0.3.0/clip_bbox/tests/test_all.py
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.299311 clip_bbox-0.3.0/clip_bbox.egg-info/
+-rw-rw----   0 gsu      (20682) gsu      (24121)    16565 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/PKG-INFO
+-rw-rw----   0 gsu      (20682) gsu      (24121)      930 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/SOURCES.txt
+-rw-rw----   0 gsu      (20682) gsu      (24121)        1 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/dependency_links.txt
+-rw-rw----   0 gsu      (20682) gsu      (24121)      278 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/requires.txt
+-rw-rw----   0 gsu      (20682) gsu      (24121)       10 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/top_level.txt
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.319311 clip_bbox-0.3.0/docs/
+-rw-rw----   0 gsu      (20682) gsu      (24121)      638 2023-04-05 02:04:28.000000 clip_bbox-0.3.0/docs/Makefile
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.319311 clip_bbox-0.3.0/docs/images/
+-rw-rw----   0 gsu      (20682) gsu      (24121)   833138 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/docs/images/command_line_usage.gif
+-rw-rw----   0 gsu      (20682) gsu      (24121)   330320 2023-04-05 02:04:28.000000 clip_bbox-0.3.0/docs/images/example_output.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)   341790 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/docs/images/rocket_result.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)      804 2023-04-05 02:04:28.000000 clip_bbox-0.3.0/docs/make.bat
+-rw-rw----   0 gsu      (20682) gsu      (24121)      122 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/docs/requirements.txt
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.323311 clip_bbox-0.3.0/docs/source/
+-rw-rw----   0 gsu      (20682) gsu      (24121)      728 2023-04-09 16:57:10.000000 clip_bbox-0.3.0/docs/source/clip_bbox.rst
+-rw-rw----   0 gsu      (20682) gsu      (24121)     1478 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/docs/source/conf.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     1678 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/docs/source/index.md
+-rw-rw----   0 gsu      (20682) gsu      (24121)       66 2023-04-05 03:41:23.000000 clip_bbox-0.3.0/docs/source/modules.rst
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2509 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/pyproject.toml
+-rw-rw----   0 gsu      (20682) gsu      (24121)      150 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/requirements.txt
+-rw-rw----   0 gsu      (20682) gsu      (24121)       38 2023-05-03 15:13:05.323311 clip_bbox-0.3.0/setup.cfg
+-rw-rw----   0 gsu      (20682) gsu      (24121)       39 2023-04-05 01:37:03.000000 clip_bbox-0.3.0/setup.py
```

### Comparing `clip_bbox-0.2.0/.bumpversion.cfg` & `clip_bbox-0.3.0/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.3.0
 commit = True
 tag = True
 
 [bumpversion:file:clip_bbox/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
@@ -12,9 +12,9 @@
 replace = version = "{new_version}"
 
 [bumpversion:file:docs/source/conf.py]
 search = release = "{current_version}"
 replace = release = "{new_version}"
 
 [bumpversion:file:docs/requirements.txt]
-search = clip_bbox=={current_version}
-replace = clip_bbox=={new_version}
+search = clip-bbox=={current_version}
+replace = clip-bbox=={new_version}
```

### Comparing `clip_bbox-0.2.0/CONTRIBUTING.md` & `clip_bbox-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.2.0/LICENSE` & `clip_bbox-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.2.0/MANIFEST.in` & `clip_bbox-0.3.0/MANIFEST.in`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 include *.md
 
 include .bumpversion.cfg
 include .readthedocs.yml
 include pyproject.toml
 include Makefile
 include requirements.txt
-include docs/images/example_output.png
-
+include docs/images/*
+include .coveragerc
 
 recursive-include docs *.bat
 recursive-include docs *.md
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
```

### Comparing `clip_bbox-0.2.0/Makefile` & `clip_bbox-0.3.0/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 annotate:  ## run type checking
 	python -m mypy ./clip_bbox
 
 #########
 # TESTS #
 #########
 test: ## clean and run unit tests
-	python -m pytest -v clip_bbox/tests
+	python -m pytest -v clip_bbox/tests --disable-warnings
 
 coverage:  ## clean and run unit tests with coverage
-	python -m pytest -v clip_bbox/tests --cov=clip_bbox --cov-branch --cov-fail-under=50 --cov-report term-missing
+	python -m pytest -v clip_bbox/tests --cov=clip_bbox --cov-branch --cov-fail-under=50 --cov-report term-missing --disable-warnings
 
 # Alias
 tests: test
 
 ###########
 # VERSION #
 ###########
@@ -70,49 +70,40 @@
 
 dist-check:
 	python -m twine check dist/*
 
 dist: clean build dist-build dist-check  ## Build dists
 
 publish:  # Upload python assets
-	echo "would usually run python -m twine upload dist/* --skip-existing"
+	python -m twine upload dist/* --skip-existing
 
 
 #########
 # CLEAN #
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
 clean: ## clean the repository
 	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache .mypy_cache
+	$(MAKE) -C docs/ clean
 
 ########
 # DOCS #
 ########
 TMPREPO=/tmp/docs/clip_bbox
 
 docs:
 	$(MAKE) -C docs/ clean
 	$(MAKE) -C docs/ html
 
-pages: 
-	rm -rf $(TMPREPO)
-	git clone -b gh-pages https://github.com/graceduansu/clip_bbox.git $(TMPREPO)
-	rm -rf $(TMPREPO)/*
-	cp -r docs/_build/html/* $(TMPREPO)
-	cd $(TMPREPO);\
-	git add -A ;\
-	git commit -a -m 'auto-updating docs' ;\
-	git push
-
 ############################################################################################
 
 # Thanks to Francoise at marmelab.com for this
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
-.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean docs pages help
+.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean docs help
```

### Comparing `clip_bbox-0.2.0/PKG-INFO` & `clip_bbox-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip_bbox
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python library for detecting image objects with natural language text labels
 Author-email: Grace Su <grace.duansu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,45 +225,62 @@
 
 `CLIP_BBox` is a Python library for detecting image objects with natural language text labels. 
 
 [![Build Status](https://github.com/graceduansu/clip_bbox/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/graceduansu/clip_bbox/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/graceduansu/clip_bbox/branch/main/graph/badge.svg)](https://codecov.io/gh/graceduansu/clip_bbox)
 [![GitHub](https://img.shields.io/github/license/graceduansu/clip_bbox)](./LICENSE)
 ![GitHub issues](https://img.shields.io/github/issues/graceduansu/clip_bbox)
+[![PyPI](https://img.shields.io/pypi/v/clip-bbox)](https://pypi.org/project/clip-bbox/)
+[![Documentation Status](https://readthedocs.org/projects/clip-bbox/badge/?version=latest)](https://clip-bbox.readthedocs.io/en/latest/?badge=latest)
+
 
 ## Overview
 
 [CLIP](https://github.com/openai/CLIP) is a neural network, pretrained on image-text pairs, that can predict the most relevant text snippet for a given image. 
 
 Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw a bounding box around the image region with the highest image-text correspondence. 
 
+## Note
+The files for building the CLIP model (`clip.py`, `model.py`, `newpad.py`, `simple_tokenizer.py`) are third-party code from the [CLIP repo](https://github.com/openai/CLIP). They are not included in test coverage.
+
 ### Features
 
-The library will provide functions for the following operations:
+The library provides functions for the following operations:
 * Getting and appropriately reshaping an image's spatial embedding from the CLIP model before it performs attention-pooling
-* Getting a text snippet's embedding from the CLIP model
-* Computing the similarity heatmap between a pair of spatial and text embeddings from CLIP
-* Drawing bounding boxes on an image, given a similarity heatmap and a similarity threshold
+* Getting a text snippet's embedding from CLIP
+* Computing the similarity heatmap between an image's spatial and text embeddings from CLIP
+* Drawing bounding boxes on an image, given a similarity heatmap
 
 ## Install
 
 Use pip to install clip_bbox as a Python package:
 
-    $ pip install clip_bbox
+    $ pip install clip-bbox
+
+## Usage Examples
 
-## Example Usage
+### Command Line Script
+```
+usage: python -m clip_bbox [-h] imgpath caption outpath
+
+positional arguments:
+  imgpath     path to input image
+  caption     caption of input image
+  outpath     path to output image displaying bounding boxes
 
-### Use As a Command Line Script
+optional arguments:
+  -h, --help  show this help message and exit
+```
 
-To draw bounding boxes on an image, run
+To draw bounding boxes on an image based on its caption, run
 
-    $ python clip_bbox.py --img "path/to/img.png" 
+    $ python -m clip_bbox "path/to/img.png" "caption of your image" "path/to/output_path.png"
 
-### Use As a Python Module
+### Python Module
 
-To draw bounding boxes on an image, do the following:
+To draw bounding boxes on an image based on its caption, do the following:
 
 ```python
 from clip_bbox import run_clip_bbox
 
-run_clip_bbox('path/to/img.png')
+run_clip_bbox("path/to/img.png", "caption of your image", "path/to/output_path.png")
 ```
```

### Comparing `clip_bbox-0.2.0/README.md` & `clip_bbox-0.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -3,45 +3,62 @@
 
 `CLIP_BBox` is a Python library for detecting image objects with natural language text labels. 
 
 [![Build Status](https://github.com/graceduansu/clip_bbox/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/graceduansu/clip_bbox/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/graceduansu/clip_bbox/branch/main/graph/badge.svg)](https://codecov.io/gh/graceduansu/clip_bbox)
 [![GitHub](https://img.shields.io/github/license/graceduansu/clip_bbox)](./LICENSE)
 ![GitHub issues](https://img.shields.io/github/issues/graceduansu/clip_bbox)
+[![PyPI](https://img.shields.io/pypi/v/clip-bbox)](https://pypi.org/project/clip-bbox/)
+[![Documentation Status](https://readthedocs.org/projects/clip-bbox/badge/?version=latest)](https://clip-bbox.readthedocs.io/en/latest/?badge=latest)
+
 
 ## Overview
 
 [CLIP](https://github.com/openai/CLIP) is a neural network, pretrained on image-text pairs, that can predict the most relevant text snippet for a given image. 
 
 Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw a bounding box around the image region with the highest image-text correspondence. 
 
+## Note
+The files for building the CLIP model (`clip.py`, `model.py`, `newpad.py`, `simple_tokenizer.py`) are third-party code from the [CLIP repo](https://github.com/openai/CLIP). They are not included in test coverage.
+
 ### Features
 
-The library will provide functions for the following operations:
+The library provides functions for the following operations:
 * Getting and appropriately reshaping an image's spatial embedding from the CLIP model before it performs attention-pooling
-* Getting a text snippet's embedding from the CLIP model
-* Computing the similarity heatmap between a pair of spatial and text embeddings from CLIP
-* Drawing bounding boxes on an image, given a similarity heatmap and a similarity threshold
+* Getting a text snippet's embedding from CLIP
+* Computing the similarity heatmap between an image's spatial and text embeddings from CLIP
+* Drawing bounding boxes on an image, given a similarity heatmap
 
 ## Install
 
 Use pip to install clip_bbox as a Python package:
 
-    $ pip install clip_bbox
+    $ pip install clip-bbox
+
+## Usage Examples
 
-## Example Usage
+### Command Line Script
+```
+usage: python -m clip_bbox [-h] imgpath caption outpath
+
+positional arguments:
+  imgpath     path to input image
+  caption     caption of input image
+  outpath     path to output image displaying bounding boxes
 
-### Use As a Command Line Script
+optional arguments:
+  -h, --help  show this help message and exit
+```
 
-To draw bounding boxes on an image, run
+To draw bounding boxes on an image based on its caption, run
 
-    $ python clip_bbox.py --img "path/to/img.png" 
+    $ python -m clip_bbox "path/to/img.png" "caption of your image" "path/to/output_path.png"
 
-### Use As a Python Module
+### Python Module
 
-To draw bounding boxes on an image, do the following:
+To draw bounding boxes on an image based on its caption, do the following:
 
 ```python
 from clip_bbox import run_clip_bbox
 
-run_clip_bbox('path/to/img.png')
+run_clip_bbox("path/to/img.png", "caption of your image", "path/to/output_path.png")
 ```
```

### Comparing `clip_bbox-0.2.0/clip_bbox/bbox_utils.py` & `clip_bbox-0.3.0/clip_bbox/bbox_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     cmap="viridis",
     cbar="False",
     dot_max=False,
     bboxes=[],
     order=None,
 ):
     """Draw bounding boxes on image and overlay the
-    corresponding heatmap.
+    corresponding heatmap. Saves result to save_path.
 
     Args:
         image (numpy array): Image stored in RGB format
         heat_map (numpy array): 2D heatmap of values
         save_path (str): Save path for generated figure
         title (str): Title on generated figure
         en_name (str): Text inside figure
@@ -131,14 +131,15 @@
         order (str): The order of coordinates used for bboxes
 
     Returns:
         Matplotlib figure
 
     """
 
+    # np.save("rocket.npy", image)
     H, W = image.shape[0:2]
     # resize heat map
     heat_map_resized = cv2.resize(heat_map, (W, H))
     # display
     fig = plt.figure(figsize=(15, 15))
     fig.suptitle(title, size=15)
     ax = plt.subplot(1, 3, 1)
@@ -164,15 +165,15 @@
                 x_min, x_max, y_min, y_max = (
                     int(bbox_norm[0] * W),
                     int(bbox_norm[2] * W),
                     int(bbox_norm[1] * H),
                     int(bbox_norm[3] * H),
                 )
             x_length, y_length = x_max - x_min, y_max - y_min
-            print(x_min, y_min, x_length, y_length)
+
             box = plt.Rectangle(
                 (x_min, y_min),
                 x_length,
                 y_length,
                 edgecolor="r",
                 linewidth=3,
                 fill=False,
```

### Comparing `clip_bbox-0.2.0/clip_bbox/clip.py` & `clip_bbox-0.3.0/clip_bbox/clip.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 from pkg_resources import packaging
 
 import torch
 from PIL import Image
 from torchvision.transforms import Compose, Resize, CenterCrop, ToTensor, Normalize
 from tqdm import tqdm
 
-from model import build_model
-from simple_tokenizer import SimpleTokenizer as _Tokenizer
+from .model import build_model
+
+# from .simple_tokenizer import SimpleTokenizer as _Tokenizer
 
 try:
     from torchvision.transforms import InterpolationMode
 
     BICUBIC = InterpolationMode.BICUBIC
 except ImportError:
     BICUBIC = Image.BICUBIC
 
 
 if packaging.version.parse(torch.__version__) < packaging.version.parse("1.7.1"):
     warnings.warn("PyTorch version 1.7.1 or higher is recommended")
 
 
-__all__ = ["available_models", "load", "tokenize"]
-_tokenizer = _Tokenizer()
+__all__ = ["available_models", "load"]
+# _tokenizer = _Tokenizer()
 
 _MODELS = {
     "RN50": (
         "https://openaipublic.azureedge.net/clip/models/"
         "afeb0e10f9e5a86da6080e35cf09123aca3b358a0c3e3b6c78a7b63bc04b6762/RN50.pt"
     ),
     "RN101": (
@@ -235,44 +236,44 @@
         patch_float(model.encode_text)
 
         model.float()
 
     return model, _transform(model.input_resolution.item())
 
 
-def tokenize(texts: Union[str, List[str]], context_length: int = 77, truncate: bool = False) -> torch.LongTensor:
-    """
-    Returns the tokenized representation of given input string(s)
-
-    Parameters
-    ----------
-    texts : Union[str, List[str]]
-        An input string or a list of input strings to tokenize
-
-    context_length : int
-        The context length to use; all CLIP models use 77 as the context length
-
-    truncate: bool
-        Whether to truncate the text in case its encoding is longer than the context length
-
-    Returns
-    -------
-    A two-dimensional tensor containing the resulting tokens, shape = [number of input strings, context_length]
-    """
-    if isinstance(texts, str):
-        texts = [texts]
-
-    sot_token = _tokenizer.encoder["<|startoftext|>"]
-    eot_token = _tokenizer.encoder["<|endoftext|>"]
-    all_tokens = [[sot_token] + _tokenizer.encode(text) + [eot_token] for text in texts]
-    result = torch.zeros(len(all_tokens), context_length, dtype=torch.long)
-
-    for i, tokens in enumerate(all_tokens):
-        if len(tokens) > context_length:
-            if truncate:
-                tokens = tokens[:context_length]
-                tokens[-1] = eot_token
-            else:
-                raise RuntimeError(f"Input {texts[i]} is too long for context length {context_length}")
-        result[i, : len(tokens)] = torch.tensor(tokens)
+# def tokenize(texts: Union[str, List[str]], context_length: int = 77, truncate: bool = False) -> torch.LongTensor:
+#     """
+#     Returns the tokenized representation of given input string(s)
+
+#     Parameters
+#     ----------
+#     texts : Union[str, List[str]]
+#         An input string or a list of input strings to tokenize
+
+#     context_length : int
+#         The context length to use; all CLIP models use 77 as the context length
+
+#     truncate: bool
+#         Whether to truncate the text in case its encoding is longer than the context length
+
+#     Returns
+#     -------
+#     A two-dimensional tensor containing the resulting tokens, shape = [number of input strings, context_length]
+#     """
+#     if isinstance(texts, str):
+#         texts = [texts]
+
+#     sot_token = _tokenizer.encoder["<|startoftext|>"]
+#     eot_token = _tokenizer.encoder["<|endoftext|>"]
+#     all_tokens = [[sot_token] + _tokenizer.encode(text) + [eot_token] for text in texts]
+#     result = torch.zeros(len(all_tokens), context_length, dtype=torch.long)
+
+#     for i, tokens in enumerate(all_tokens):
+#         if len(tokens) > context_length:
+#             if truncate:
+#                 tokens = tokens[:context_length]
+#                 tokens[-1] = eot_token
+#             else:
+#                 raise RuntimeError(f"Input {texts[i]} is too long for context length {context_length}")
+#         result[i, : len(tokens)] = torch.tensor(tokens)
 
-    return result
+#     return result
```

### Comparing `clip_bbox-0.2.0/clip_bbox/clip_model_setup.py` & `clip_bbox-0.3.0/clip_bbox/clip_model_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 import torch
-from model import build_model
+import os
+from .model import build_model
+from .clip import load
 
 # os.path.abspath(os.path.dirname(__file__))
 
 MODELS = {
     "RN50": (
         "https://openaipublic.azureedge.net/clip/models/"
         "afeb0e10f9e5a86da6080e35cf09123aca3b358a0c3e3b6c78a7b63bc04b6762"
@@ -24,52 +26,54 @@
         "https://openaipublic.azureedge.net/clip/models/"
         "40d365715913c9da98579312b702a82c18be219cc2a73407c4526f58eba950af/"
         "ViT-B-32.pt"
     ),
 }
 
 
-def get_clip_model(model_name="RN50", input_res=(720, 1280)):
+def get_clip_model(device, model_name="RN50", input_res=(720, 1280)):
     """Downloads pre-trained CLIP model and adjusts model to accept
     desired input resolution.
 
     Args:
         model_name (str): Description of arg1
         input_res (tuple[int]): Input resolution represented as (height, width)
 
     Returns:
         Modified Torch model accepting the desired input resolution
 
     """
     print("Torch version:", torch.__version__)
 
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    print(device)
-
     input_resolution = input_res
-    # os.system("wget {} -O model.pt".format(MODELS[model_name]))
 
-    clip_model = torch.jit.load("model.pt").cuda().eval()
-    context_length = clip_model.context_length.item()
-    vocab_size = clip_model.vocab_size.item()
+    if not os.path.exists("model.pt"):
+        os.system("wget -q {} -O model.pt".format(MODELS[model_name]))
+
+    clip_model, _ = load("model.pt", device, jit=False, download_root='./')
+    clip_model = clip_model.eval()
+    # clip_model = torch.load("model.pt", map_location=device).eval()
+    context_length = clip_model.context_length
+    # context_length = clip_model.context_length.item()
+    vocab_size = clip_model.vocab_size
+    # vocab_size = clip_model.vocab_size.item()
+    # print("model location: ", clip_model.device)
 
     print(
         "Model parameters:",
         f"{np.sum([int(np.prod(p.shape)) for p in clip_model.parameters()]):,}",
     )
     print("Input resolution:", input_resolution)
     print("Context length:", context_length)
     print("Vocab size:", vocab_size)
 
     clip_model.state_dict()["input_resolution"] = torch.tensor(input_res)
     # print("Model's state_dict:")
     for param_tensor in clip_model.state_dict():
         # print(param_tensor + '            ' + str(clip_model.state_dict()[param_tensor].size()))
-        clip_model.state_dict()[param_tensor] = clip_model.state_dict()[param_tensor].cuda()
+        clip_model.state_dict()[param_tensor] = clip_model.state_dict()[param_tensor].to(device)
 
     model_modded = build_model(clip_model.state_dict())
 
-    print("check model cuda: {}".format(next(model_modded.parameters()).is_cuda))
     model_modded.to(device)
-    print("device count: {}".format(torch.cuda.device_count()))
 
     return model_modded
```

### Comparing `clip_bbox-0.2.0/clip_bbox/clipbbox.py` & `clip_bbox-0.3.0/clip_bbox/clipbbox.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 #!/usr/bin/env python3
 
 import torch
 
-import clip_model_setup
-import bbox_utils
-import preprocess
+from . import clip_model_setup
+from . import bbox_utils
+from . import preprocess
 
-# TODO: arg parser for bbox params
 
-
-def run_clip_bbox(input_res):
+def run_clip_bbox(img_path, caption, out_path):
     """Draws bounding boxes on an input image.
 
     Args:
-        input_res (tuple[int]): Input resolution represented as (height, width)
+        img_path (str): path to input image
+        caption (str): caption of input image
+        out_path (str): path to output image displaying bounding boxes
 
     Returns:
         None
 
     """
+    device = torch.device("cpu")
+
+    print('torch device:', device)
 
-    # TODO: add argument for image path
+    input_resolution = (720, 1280)
+    images, image_input = preprocess.preprocess_imgs([img_path], device, input_resolution=input_resolution)
 
-    input_resolution = input_res
-    model_modded = clip_model_setup.get_clip_model()
+    # TODO: make img_fts_to_heatmap accept all resolutions
+    # input_resolution = images[0].size()[1:]
 
-    images, image_input = preprocess.preprocess_imgs()
-    text_input = preprocess.preprocess_texts(model_modded.context_length)
+    model_modded = clip_model_setup.get_clip_model(device, input_res=input_resolution)
+    text_input = preprocess.preprocess_texts([caption], model_modded.context_length, device)
 
     with torch.no_grad():
         image_features = model_modded.encode_image(image_input).float()
         text_features = model_modded.encode_text(text_input).float()
 
     # get bbox results
     img_fts = image_features[1:]
     # print("fts size: ", img_fts.size())
+    # torch.save(img_fts, "rocket_img_fts.pt")
+    # torch.save(text_features, "rocket_txt_fts.pt")
 
     heatmap_list = img_fts_to_heatmap(img_fts, text_features)
     pred_bboxes = []
     for h in range(len(heatmap_list)):
-        title = "Image " + str(h)
         heat = heatmap_list[h]
+        # np.savez("heat.npz", heat)
         bboxes = bbox_utils.heat2bbox(heat, input_resolution)
         pred_bboxes.append([torch.tensor(b["bbox_normalized"]).unsqueeze(0) for b in bboxes])
-        save_path = "img_{}_bbox.png".format(h)
         bbox_utils.img_heat_bbox_disp(
             images[h].permute(1, 2, 0).cpu(),
             heat,
-            save_path,
-            title=title,
+            out_path,
             bboxes=bboxes,
             order="xyxy",
         )
 
 
 def img_fts_to_heatmap(img_fts, txt_fts):
     """Computes the similarity heatmap between a pair of
@@ -69,39 +73,35 @@
     """
 
     # dot product with normalization
     img_norm = img_fts / img_fts.norm(dim=-1, keepdim=True)
     txt_norm = txt_fts / txt_fts.norm(dim=-1, keepdim=True)
 
     batch_size = len(txt_norm)
-    print(batch_size)
+    # print(batch_size)
 
     # img_norm = F.interpolate(img_norm.permute(2,1,0), size=int(input_resolution[0]*input_resolution[1]/64),
     #      mode='nearest').permute(2,1,0)
     # resize = torch.flatten(img_norm).size()[0] / batch_size / img_fts.size()[0]
     # resize = int(math.sqrt(resize))
     img_reshape = torch.reshape(img_norm, (22, 40, batch_size, img_fts.size()[2]))
     # img_reshape = torch.reshape(img_norm, (7, 7, batch_size, 1024))
     # img_reshape = torch.reshape(img_norm, (resize, resize, batch_size, img_fts.size()[0]))
-    print(img_reshape.shape)
-    print(txt_norm.shape)
+    # print(img_reshape.shape)
+    # print(txt_norm.shape)
 
     img_reshape = img_reshape.cpu()
 
     heatmap_norm = img_reshape.cpu().numpy() @ txt_norm.cpu().numpy().T
 
     # heatmap_list = [-1.0 * heatmap_norm[:,:,h,h] + heatmap_norm[:,:,h,h].min() for h in range(batch_size)]
 
     # my loop
     heatmap_list = []
     for h in range(batch_size):
-        maxi = heatmap_norm[:, :, h, h].max()
-        print(maxi)
+        # maxi = heatmap_norm[:, :, h, h].max()
+        # print(maxi)
         hm = -1.0 * heatmap_norm[:, :, h, h] + heatmap_norm[:, :, h, h].max()
         # hm = hm / np.linalg.norm(hm)
         heatmap_list.append(hm)
 
     return heatmap_list
-
-
-if __name__ == "__main__":
-    run_clip_bbox(input_res=(720, 1280))
```

### Comparing `clip_bbox-0.2.0/clip_bbox/model.py` & `clip_bbox-0.3.0/clip_bbox/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,16 @@
         self.num_heads = num_heads
 
     def forward(self, x):
         x = x.reshape(x.shape[0], x.shape[1], x.shape[2] * x.shape[3]).permute(2, 0, 1)  # NCHW -> (HW)NC
         x = torch.cat([x.mean(dim=0, keepdim=True), x], dim=0)  # (HW+1)NC
         # x = x + self.positional_embedding[:, None, :].to(x.dtype)  # (HW+1)NC
         temp = self.positional_embedding[:, None, :].to(x.dtype)
+
+        # TODO: Document these modifications
         temp = temp.permute(2, 1, 0)
         temp = F.interpolate(temp, size=x.shape[0], mode="linear").permute(2, 1, 0)
 
         x = x + temp
         x, _ = F.multi_head_attention_forward(
             query=x,
             key=x,
@@ -111,14 +113,15 @@
             out_proj_weight=self.c_proj.weight,
             out_proj_bias=self.c_proj.bias,
             use_separate_proj_weight=True,
             training=self.training,
             need_weights=False,
         )
 
+        # return x.squeeze(0)
         return x
 
 
 class ModifiedResNet(nn.Module):
     """
     A ResNet class that is similar to torchvision's but contains the following changes:
     - There are now 3 "stem" convolutions as opposed to 1, with an average pool instead of a max pool.
@@ -158,32 +161,34 @@
         for _ in range(1, blocks):
             layers.append(Bottleneck(self._inplanes, planes))
 
         return nn.Sequential(*layers)
 
     def forward(self, x):
         def stem(x):
+            device = x.device
+
             for conv, bn in [
                 (self.conv1, self.bn1),
                 (self.conv2, self.bn2),
                 (self.conv3, self.bn3),
             ]:
-                x = x.cuda()
+                x = x.to(device)
                 x = self.relu(bn(conv(x)))
             x = self.avgpool(x)
             return x
 
         x = x.type(self.conv1.weight.dtype)
         x = stem(x)
         x = self.layer1(x)
         x = self.layer2(x)
         x = self.layer3(x)
         x = self.layer4(x)
         x = self.attnpool(x)
-        print("output size: ", x.size())
+        # print("output size: ", x.size())
 
         return x
 
 
 class LayerNorm(nn.LayerNorm):
     """Subclass torch's LayerNorm to handle fp16."""
 
@@ -400,15 +405,15 @@
 
     def encode_image(self, image):
         # self = MyDataParallel(self, device_ids=[0,1,2,3])
         return self.visual(image.type(self.dtype))
 
     def encode_text(self, text):
         # self = MyDataParallel(self, device_ids=[0,1,2,3])
-        x = self.token_embedding(text).type(self.dtype)  # [batch_size, n_ctx, d_model]
+        x = self.token_embedding(text.type(torch.LongTensor)).type(self.dtype)  # [batch_size, n_ctx, d_model]
 
         x = x + self.positional_embedding.type(self.dtype)
         x = x.permute(1, 0, 2)  # NLD -> LND
         x = self.transformer(x)
         x = x.permute(1, 0, 2)  # LND -> NLD
         x = self.ln_final(x).type(self.dtype)
 
@@ -506,10 +511,10 @@
         transformer_layers,
     )
 
     for key in ["input_resolution", "context_length", "vocab_size"]:
         if key in state_dict:
             del state_dict[key]
 
-    convert_weights(model)
+    # convert_weights(model)
     model.load_state_dict(state_dict)
     return model.eval()
```

### Comparing `clip_bbox-0.2.0/clip_bbox/newpad.py` & `clip_bbox-0.3.0/clip_bbox/newpad.py`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.2.0/clip_bbox/simple_tokenizer.py` & `clip_bbox-0.3.0/clip_bbox/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.2.0/clip_bbox.egg-info/PKG-INFO` & `clip_bbox-0.3.0/clip_bbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip-bbox
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python library for detecting image objects with natural language text labels
 Author-email: Grace Su <grace.duansu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,45 +225,62 @@
 
 `CLIP_BBox` is a Python library for detecting image objects with natural language text labels. 
 
 [![Build Status](https://github.com/graceduansu/clip_bbox/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/graceduansu/clip_bbox/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/graceduansu/clip_bbox/branch/main/graph/badge.svg)](https://codecov.io/gh/graceduansu/clip_bbox)
 [![GitHub](https://img.shields.io/github/license/graceduansu/clip_bbox)](./LICENSE)
 ![GitHub issues](https://img.shields.io/github/issues/graceduansu/clip_bbox)
+[![PyPI](https://img.shields.io/pypi/v/clip-bbox)](https://pypi.org/project/clip-bbox/)
+[![Documentation Status](https://readthedocs.org/projects/clip-bbox/badge/?version=latest)](https://clip-bbox.readthedocs.io/en/latest/?badge=latest)
+
 
 ## Overview
 
 [CLIP](https://github.com/openai/CLIP) is a neural network, pretrained on image-text pairs, that can predict the most relevant text snippet for a given image. 
 
 Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw a bounding box around the image region with the highest image-text correspondence. 
 
+## Note
+The files for building the CLIP model (`clip.py`, `model.py`, `newpad.py`, `simple_tokenizer.py`) are third-party code from the [CLIP repo](https://github.com/openai/CLIP). They are not included in test coverage.
+
 ### Features
 
-The library will provide functions for the following operations:
+The library provides functions for the following operations:
 * Getting and appropriately reshaping an image's spatial embedding from the CLIP model before it performs attention-pooling
-* Getting a text snippet's embedding from the CLIP model
-* Computing the similarity heatmap between a pair of spatial and text embeddings from CLIP
-* Drawing bounding boxes on an image, given a similarity heatmap and a similarity threshold
+* Getting a text snippet's embedding from CLIP
+* Computing the similarity heatmap between an image's spatial and text embeddings from CLIP
+* Drawing bounding boxes on an image, given a similarity heatmap
 
 ## Install
 
 Use pip to install clip_bbox as a Python package:
 
-    $ pip install clip_bbox
+    $ pip install clip-bbox
+
+## Usage Examples
 
-## Example Usage
+### Command Line Script
+```
+usage: python -m clip_bbox [-h] imgpath caption outpath
+
+positional arguments:
+  imgpath     path to input image
+  caption     caption of input image
+  outpath     path to output image displaying bounding boxes
 
-### Use As a Command Line Script
+optional arguments:
+  -h, --help  show this help message and exit
+```
 
-To draw bounding boxes on an image, run
+To draw bounding boxes on an image based on its caption, run
 
-    $ python clip_bbox.py --img "path/to/img.png" 
+    $ python -m clip_bbox "path/to/img.png" "caption of your image" "path/to/output_path.png"
 
-### Use As a Python Module
+### Python Module
 
-To draw bounding boxes on an image, do the following:
+To draw bounding boxes on an image based on its caption, do the following:
 
 ```python
 from clip_bbox import run_clip_bbox
 
-run_clip_bbox('path/to/img.png')
+run_clip_bbox("path/to/img.png", "caption of your image", "path/to/output_path.png")
 ```
```

### Comparing `clip_bbox-0.2.0/clip_bbox.egg-info/SOURCES.txt` & `clip_bbox-0.3.0/clip_bbox.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 .bumpversion.cfg
+.coveragerc
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 clip_bbox/__init__.py
+clip_bbox/__main__.py
 clip_bbox/bbox_utils.py
 clip_bbox/clip.py
 clip_bbox/clip_model_setup.py
 clip_bbox/clipbbox.py
 clip_bbox/model.py
 clip_bbox/newpad.py
 clip_bbox/preprocess.py
 clip_bbox/simple_tokenizer.py
 clip_bbox.egg-info/PKG-INFO
 clip_bbox.egg-info/SOURCES.txt
 clip_bbox.egg-info/dependency_links.txt
 clip_bbox.egg-info/requires.txt
 clip_bbox.egg-info/top_level.txt
 clip_bbox/tests/test_all.py
+clip_bbox/tests/assets/heat.npz
+clip_bbox/tests/assets/rocket.npy
+clip_bbox/tests/assets/rocket.png
+clip_bbox/tests/assets/test_all-gt_output.png
 docs/Makefile
-docs/index.md
 docs/make.bat
 docs/requirements.txt
+docs/images/command_line_usage.gif
 docs/images/example_output.png
+docs/images/rocket_result.png
 docs/source/clip_bbox.rst
 docs/source/conf.py
+docs/source/index.md
 docs/source/modules.rst
```

### Comparing `clip_bbox-0.2.0/docs/Makefile` & `clip_bbox-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.2.0/docs/images/example_output.png` & `clip_bbox-0.3.0/docs/images/example_output.png`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.2.0/docs/make.bat` & `clip_bbox-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.2.0/docs/source/conf.py` & `clip_bbox-0.3.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 import sphinx_rtd_theme
 from recommonmark.transform import AutoStructify
 import os
 import sys
 
 # Path for autodocs
-sys.path.insert(0, os.path.abspath('../'))
+sys.path.insert(0, os.path.abspath('../..'))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'clip_bbox'
 copyright = '2023, Grace Su'
 author = 'Grace Su'
-release = "0.2.0"
+release = "0.3.0"
 
 master_doc = 'index'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['recommonmark', 'sphinx.ext.autodoc', 'sphinx.ext.githubpages', 'sphinx.ext.napoleon']
```

### Comparing `clip_bbox-0.2.0/pyproject.toml` & `clip_bbox-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,18 +7,28 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "clip_bbox"
 authors = [{name = "Grace Su", email = "grace.duansu@gmail.com"}]
 description="Python library for detecting image objects with natural language text labels"
 readme = "README.md"
-version = "0.2.0"
+version = "0.3.0"
 requires-python = ">=3.7"
 
-dependencies = ["torch==1.7.1", "torchvision", "ftfy", "regex"]
+dependencies = [
+    "torch==1.7.1", 
+    "torchvision", 
+    "ftfy", 
+    "regex", 
+    "opencv-python", 
+    "matplotlib", 
+    "scikit-image",
+    "scipy",
+    "tqdm"
+    ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
@@ -94,12 +104,11 @@
 # warn_unused_configs = true
 # disallow_subclassing_any = true
 # disallow_incomplete_defs = true
 # disallow_untyped_decorators = true
 # disallow_untyped_calls = true
 
 [tool.pytest.ini_options]
-asyncio_mode = 'strict'
 testpaths = 'clip_bbox/tests'
 pythonpath = [
   ".", "clip_bbox"
 ]
```

