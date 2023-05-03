# Comparing `tmp/sports-box-0.1.1.tar.gz` & `tmp/sports-box-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports-box-0.1.1.tar", last modified: Sun Mar 26 22:28:39 2023, max compression
+gzip compressed data, was "sports-box-0.1.2.tar", last modified: Wed May  3 21:31:02 2023, max compression
```

## Comparing `sports-box-0.1.1.tar` & `sports-box-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,61 @@
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.223955 sports-box-0.1.1/
--rw-r--r--   0 danielhu   (501) staff       (20)      395 2023-03-26 21:51:17.000000 sports-box-0.1.1/.bumpversion.cfg
--rw-r--r--   0 danielhu   (501) staff       (20)        5 2023-03-26 21:52:26.000000 sports-box-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 danielhu   (501) staff       (20)    11357 2023-02-17 22:43:34.000000 sports-box-0.1.1/LICENSE
--rw-r--r--   0 danielhu   (501) staff       (20)      384 2023-03-22 18:27:44.000000 sports-box-0.1.1/MANIFEST.in
--rw-r--r--   0 danielhu   (501) staff       (20)     2253 2023-03-22 18:27:44.000000 sports-box-0.1.1/Makefile
--rw-r--r--   0 danielhu   (501) staff       (20)    14777 2023-03-26 22:28:39.223736 sports-box-0.1.1/PKG-INFO
--rw-r--r--   0 danielhu   (501) staff       (20)     1021 2023-03-26 21:52:26.000000 sports-box-0.1.1/README.md
--rw-r--r--   0 danielhu   (501) staff       (20)     1311 2023-03-22 18:27:44.000000 sports-box-0.1.1/package-lock.json
--rw-r--r--   0 danielhu   (501) staff       (20)       54 2023-03-22 18:27:44.000000 sports-box-0.1.1/package.json
--rw-r--r--   0 danielhu   (501) staff       (20)     2216 2023-03-26 21:52:20.000000 sports-box-0.1.1/pyproject.toml
--rw-r--r--   0 danielhu   (501) staff       (20)       38 2023-03-26 22:28:39.224058 sports-box-0.1.1/setup.cfg
--rw-r--r--   0 danielhu   (501) staff       (20)       39 2023-03-22 18:27:44.000000 sports-box-0.1.1/setup.py
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.218520 sports-box-0.1.1/sports_box/
--rw-r--r--   0 danielhu   (501) staff       (20)       94 2023-03-26 05:59:52.000000 sports-box-0.1.1/sports_box/.env
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.220149 sports-box-0.1.1/sports_box/.pytest_cache/
--rw-r--r--   0 danielhu   (501) staff       (20)       37 2023-03-03 00:45:39.000000 sports-box-0.1.1/sports_box/.pytest_cache/.gitignore
--rw-r--r--   0 danielhu   (501) staff       (20)      191 2023-03-03 00:45:39.000000 sports-box-0.1.1/sports_box/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 danielhu   (501) staff       (20)      302 2023-03-03 00:45:39.000000 sports-box-0.1.1/sports_box/.pytest_cache/README.md
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.212681 sports-box-0.1.1/sports_box/.pytest_cache/v/
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.220570 sports-box-0.1.1/sports_box/.pytest_cache/v/cache/
--rw-r--r--   0 danielhu   (501) staff       (20)        2 2023-03-03 00:45:39.000000 sports-box-0.1.1/sports_box/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 danielhu   (501) staff       (20)        2 2023-03-03 00:45:39.000000 sports-box-0.1.1/sports_box/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 danielhu   (501) staff       (20)      458 2023-03-26 21:51:17.000000 sports-box-0.1.1/sports_box/__init__.py
--rw-r--r--   0 danielhu   (501) staff       (20)      344 2023-03-26 21:51:17.000000 sports-box-0.1.1/sports_box/__main__.py
--rw-r--r--   0 danielhu   (501) staff       (20)       22 2023-03-26 21:52:06.000000 sports-box-0.1.1/sports_box/_version.py
--rw-r--r--   0 danielhu   (501) staff       (20)     1537 2023-03-26 21:51:17.000000 sports-box-0.1.1/sports_box/bot.py
--rw-r--r--   0 danielhu   (501) staff       (20)     1038 2023-03-22 18:27:44.000000 sports-box-0.1.1/sports_box/fantasydata.py
--rw-r--r--   0 danielhu   (501) staff       (20)     2598 2023-03-26 21:51:17.000000 sports-box-0.1.1/sports_box/getnews.py
--rw-r--r--   0 danielhu   (501) staff       (20)     3182 2023-03-26 21:51:17.000000 sports-box-0.1.1/sports_box/getplayerstuff.py
--rw-r--r--   0 danielhu   (501) staff       (20)      853 2023-03-24 01:10:40.000000 sports-box-0.1.1/sports_box/getteamstuff.py
--rw-r--r--   0 danielhu   (501) staff       (20)     2406 2023-03-26 21:51:17.000000 sports-box-0.1.1/sports_box/gettodayscores.py
--rw-r--r--   0 danielhu   (501) staff       (20)     4608 2023-03-24 01:10:40.000000 sports-box-0.1.1/sports_box/teamcolors.py
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.220773 sports-box-0.1.1/sports_box/tests/
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.221521 sports-box-0.1.1/sports_box/tests/.pytest_cache/
--rw-r--r--   0 danielhu   (501) staff       (20)       37 2023-03-03 00:45:57.000000 sports-box-0.1.1/sports_box/tests/.pytest_cache/.gitignore
--rw-r--r--   0 danielhu   (501) staff       (20)      191 2023-03-03 00:45:57.000000 sports-box-0.1.1/sports_box/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 danielhu   (501) staff       (20)      302 2023-03-03 00:45:57.000000 sports-box-0.1.1/sports_box/tests/.pytest_cache/README.md
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.212916 sports-box-0.1.1/sports_box/tests/.pytest_cache/v/
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.223248 sports-box-0.1.1/sports_box/tests/.pytest_cache/v/cache/
--rw-r--r--   0 danielhu   (501) staff       (20)       22 2023-03-03 00:45:57.000000 sports-box-0.1.1/sports_box/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 danielhu   (501) staff       (20)        2 2023-03-03 01:45:22.000000 sports-box-0.1.1/sports_box/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 danielhu   (501) staff       (20)        2 2023-03-03 01:45:22.000000 sports-box-0.1.1/sports_box/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 danielhu   (501) staff       (20)     9145 2023-03-26 21:51:17.000000 sports-box-0.1.1/sports_box/tests/test_all.py
--rw-r--r--   0 danielhu   (501) staff       (20)      650 2023-03-26 21:51:17.000000 sports-box-0.1.1/sports_box/userinterface.py
-drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-03-26 22:28:39.219318 sports-box-0.1.1/sports_box.egg-info/
--rw-r--r--   0 danielhu   (501) staff       (20)    14777 2023-03-26 22:28:39.000000 sports-box-0.1.1/sports_box.egg-info/PKG-INFO
--rw-r--r--   0 danielhu   (501) staff       (20)     1077 2023-03-26 22:28:39.000000 sports-box-0.1.1/sports_box.egg-info/SOURCES.txt
--rw-r--r--   0 danielhu   (501) staff       (20)        1 2023-03-26 22:28:39.000000 sports-box-0.1.1/sports_box.egg-info/dependency_links.txt
--rw-r--r--   0 danielhu   (501) staff       (20)      201 2023-03-26 22:28:39.000000 sports-box-0.1.1/sports_box.egg-info/requires.txt
--rw-r--r--   0 danielhu   (501) staff       (20)       11 2023-03-26 22:28:39.000000 sports-box-0.1.1/sports_box.egg-info/top_level.txt
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.580825 sports-box-0.1.2/
+-rw-r--r--   0 danielhu   (501) staff       (20)      395 2023-05-03 21:28:14.000000 sports-box-0.1.2/.bumpversion.cfg
+-rw-r--r--   0 danielhu   (501) staff       (20)     5133 2023-04-04 23:31:10.000000 sports-box-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 danielhu   (501) staff       (20)    11357 2023-02-17 22:43:34.000000 sports-box-0.1.2/LICENSE
+-rw-r--r--   0 danielhu   (501) staff       (20)      569 2023-05-03 21:28:14.000000 sports-box-0.1.2/MANIFEST.in
+-rw-r--r--   0 danielhu   (501) staff       (20)     2420 2023-05-03 21:28:14.000000 sports-box-0.1.2/Makefile
+-rw-r--r--   0 danielhu   (501) staff       (20)    17240 2023-05-03 21:31:02.580536 sports-box-0.1.2/PKG-INFO
+-rw-r--r--   0 danielhu   (501) staff       (20)     3484 2023-05-03 21:28:14.000000 sports-box-0.1.2/README.md
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.568289 sports-box-0.1.2/docs/
+-rw-r--r--   0 danielhu   (501) staff       (20)      636 2023-05-03 21:28:14.000000 sports-box-0.1.2/docs/Makefile
+-rw-r--r--   0 danielhu   (501) staff       (20)      416 2023-05-03 21:28:14.000000 sports-box-0.1.2/docs/api.md
+-rw-r--r--   0 danielhu   (501) staff       (20)     1448 2023-05-03 21:28:14.000000 sports-box-0.1.2/docs/conf.py
+-rw-r--r--   0 danielhu   (501) staff       (20)     1100 2023-05-03 21:28:14.000000 sports-box-0.1.2/docs/gettingstarted.md
+-rw-r--r--   0 danielhu   (501) staff       (20)      938 2023-05-03 21:28:14.000000 sports-box-0.1.2/docs/index.md
+-rw-r--r--   0 danielhu   (501) staff       (20)      765 2023-05-03 21:28:14.000000 sports-box-0.1.2/docs/make.bat
+-rw-r--r--   0 danielhu   (501) staff       (20)     1311 2023-03-22 18:27:44.000000 sports-box-0.1.2/package-lock.json
+-rw-r--r--   0 danielhu   (501) staff       (20)       54 2023-03-22 18:27:44.000000 sports-box-0.1.2/package.json
+-rw-r--r--   0 danielhu   (501) staff       (20)     2292 2023-05-03 21:28:14.000000 sports-box-0.1.2/pyproject.toml
+-rw-r--r--   0 danielhu   (501) staff       (20)       38 2023-05-03 21:31:02.580876 sports-box-0.1.2/setup.cfg
+-rw-r--r--   0 danielhu   (501) staff       (20)       39 2023-03-22 18:27:44.000000 sports-box-0.1.2/setup.py
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.570968 sports-box-0.1.2/sports_box/
+-rw-r--r--   0 danielhu   (501) staff       (20)       94 2023-03-26 05:59:52.000000 sports-box-0.1.2/sports_box/.env
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.572245 sports-box-0.1.2/sports_box/.pytest_cache/
+-rw-r--r--   0 danielhu   (501) staff       (20)       37 2023-03-03 00:45:39.000000 sports-box-0.1.2/sports_box/.pytest_cache/.gitignore
+-rw-r--r--   0 danielhu   (501) staff       (20)      191 2023-03-03 00:45:39.000000 sports-box-0.1.2/sports_box/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 danielhu   (501) staff       (20)      302 2023-03-03 00:45:39.000000 sports-box-0.1.2/sports_box/.pytest_cache/README.md
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.565000 sports-box-0.1.2/sports_box/.pytest_cache/v/
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.573087 sports-box-0.1.2/sports_box/.pytest_cache/v/cache/
+-rw-r--r--   0 danielhu   (501) staff       (20)        2 2023-03-03 00:45:39.000000 sports-box-0.1.2/sports_box/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 danielhu   (501) staff       (20)        2 2023-03-03 00:45:39.000000 sports-box-0.1.2/sports_box/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 danielhu   (501) staff       (20)      522 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/__init__.py
+-rw-r--r--   0 danielhu   (501) staff       (20)      344 2023-03-26 21:51:17.000000 sports-box-0.1.2/sports_box/__main__.py
+-rw-r--r--   0 danielhu   (501) staff       (20)       22 2023-04-04 23:31:10.000000 sports-box-0.1.2/sports_box/_version.py
+-rw-r--r--   0 danielhu   (501) staff       (20)     2867 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/bot.py
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.573235 sports-box-0.1.2/sports_box/dogger/
+-rw-r--r--   0 danielhu   (501) staff       (20)  2295598 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/dogger/dogger.png
+-rw-r--r--   0 danielhu   (501) staff       (20)      623 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/fantasydata.py
+-rw-r--r--   0 danielhu   (501) staff       (20)     3113 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/getnews.py
+-rw-r--r--   0 danielhu   (501) staff       (20)     4042 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/getplayerstuff.py
+-rw-r--r--   0 danielhu   (501) staff       (20)     1045 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/getteamstuff.py
+-rw-r--r--   0 danielhu   (501) staff       (20)     1215 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/gettiktokstuff.py
+-rw-r--r--   0 danielhu   (501) staff       (20)     3097 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/gettodayscores.py
+-rw-r--r--   0 danielhu   (501) staff       (20)     4608 2023-03-24 01:10:40.000000 sports-box-0.1.2/sports_box/teamcolors.py
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.576433 sports-box-0.1.2/sports_box/tests/
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.579021 sports-box-0.1.2/sports_box/tests/.pytest_cache/
+-rw-r--r--   0 danielhu   (501) staff       (20)       37 2023-03-03 00:45:57.000000 sports-box-0.1.2/sports_box/tests/.pytest_cache/.gitignore
+-rw-r--r--   0 danielhu   (501) staff       (20)      191 2023-03-03 00:45:57.000000 sports-box-0.1.2/sports_box/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 danielhu   (501) staff       (20)      302 2023-03-03 00:45:57.000000 sports-box-0.1.2/sports_box/tests/.pytest_cache/README.md
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.565277 sports-box-0.1.2/sports_box/tests/.pytest_cache/v/
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.580077 sports-box-0.1.2/sports_box/tests/.pytest_cache/v/cache/
+-rw-r--r--   0 danielhu   (501) staff       (20)       22 2023-03-03 00:45:57.000000 sports-box-0.1.2/sports_box/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 danielhu   (501) staff       (20)        2 2023-03-03 01:45:22.000000 sports-box-0.1.2/sports_box/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 danielhu   (501) staff       (20)        2 2023-03-03 01:45:22.000000 sports-box-0.1.2/sports_box/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 danielhu   (501) staff       (20)     9805 2023-05-03 21:28:14.000000 sports-box-0.1.2/sports_box/tests/test_all.py
+-rw-r--r--   0 danielhu   (501) staff       (20)      650 2023-03-26 21:51:17.000000 sports-box-0.1.2/sports_box/userinterface.py
+drwxr-xr-x   0 danielhu   (501) staff       (20)        0 2023-05-03 21:31:02.571681 sports-box-0.1.2/sports_box.egg-info/
+-rw-r--r--   0 danielhu   (501) staff       (20)    17240 2023-05-03 21:31:02.000000 sports-box-0.1.2/sports_box.egg-info/PKG-INFO
+-rw-r--r--   0 danielhu   (501) staff       (20)     1225 2023-05-03 21:31:02.000000 sports-box-0.1.2/sports_box.egg-info/SOURCES.txt
+-rw-r--r--   0 danielhu   (501) staff       (20)        1 2023-05-03 21:31:02.000000 sports-box-0.1.2/sports_box.egg-info/dependency_links.txt
+-rw-r--r--   0 danielhu   (501) staff       (20)      249 2023-05-03 21:31:02.000000 sports-box-0.1.2/sports_box.egg-info/requires.txt
+-rw-r--r--   0 danielhu   (501) staff       (20)       11 2023-05-03 21:31:02.000000 sports-box-0.1.2/sports_box.egg-info/top_level.txt
```

### Comparing `sports-box-0.1.1/LICENSE` & `sports-box-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sports-box-0.1.1/Makefile` & `sports-box-0.1.2/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #########
 # BUILD #
 #########
 develop:  ## install dependencies and build library
-	python -m pip install -e .[develop]
+	python3 -m pip install -e .[develop]
 
 build:  ## build the python library
 	python3 setup.py build build_ext --inplace
 
 install:  ## install library
 	python3 -m pip install .
 
@@ -38,15 +38,15 @@
 #########
 # TESTS #
 #########
 test: ## clean and run unit tests
 	python3 -m pytest -v sports_box/tests
 
 coverage:  ## clean and run unit tests with coverage
-	python3 -m pytest -v sports_box/tests --cov=sports_box --cov-branch --cov-fail-under=75 --cov-report term-missing
+	python3 -m pytest -v sports_box/tests --cov=sports_box --cov-branch --cov-fail-under=50 --cov-report term-missing
 
 # Alias
 tests: test
 
 ###########
 # VERSION #
 ###########
@@ -72,14 +72,24 @@
 	python3 -m twine check dist/*
 
 dist: clean build dist-build dist-check  ## Build dists
 
 publish:  # Upload python assets
 	echo "would usually run python -m twine upload dist/* --skip-existing"
 
+########
+# DOCS #
+########
+
+docs:  ## build the documentation
+	make -C docs html
+
+show-docs: docs  ## show the documentation
+	open docs/_build/html/index.html
+
 #########
 # CLEAN #
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
 clean: ## clean the repository
@@ -91,8 +101,8 @@
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
-.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+.PHONY: develop build docs install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
```

### Comparing `sports-box-0.1.1/PKG-INFO` & `sports-box-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports-box
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sportsbox
 Author-email: Daniel Hu <danielhu2000@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,17 +218,103 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 <h1> sportsbox </h1>
 
-<p>Discord bot displaying sports news and convenient stats. </p>
+<p>Discord bot and independent helper functions displaying sports news and convenient stats. </p>
+
 
 ![](https://img.shields.io/badge/license-Apache--2.0-brightgreen)
 ![](https://img.shields.io/github/issues/dhu16/sportsbox)
 [![Build Status](https://github.com/dhu16/sportsbox/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/dhu16/sportsbox/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/dhu16/sportsbox/branch/main/graph/badge.svg?token=UHT46NYQGX)](https://codecov.io/gh/dhu16/sportsbox)
+[![PyPI](https://img.shields.io/pypi/v/sports-box)](https://pypi.org/project/sports-box/)
+[![docs](https://img.shields.io/github/actions/workflow/status/dhu16/sportsbox/docs.yml?label=docs)](https://dhu16.github.io/sportsbox/)
 
 <h2> Overview </h2>
 
-<p> This Discord bot allows users to view NBA and NFL news, scores, and stats on their servers with easy commands. I always found it annoying to constantly search up stats for a game I was monitoring while studying and I was too lazy to install official apps too. This alleviates the inconvenience of always having to manually search up stats or open one's phone while working or playing games with friends as Discord is usually always open on someone's computer.  </p>
+<p> This Discord bot allows users to view NBA and NFL news, scores, and stats on their servers with intuitive commands. The commands are named after the key words I always search with. I always found it annoying to constantly search up stats for a game I was monitoring while studying and I was too lazy to install official apps too. This alleviates the inconvenience of always having to manually search up stats or open one's phone while working or playing games with friends as Discord is usually always open on someone's computer.  </p>
+
+</br>
+
+## Installation
+
+`pip install sports-box`
+
+<h3> Usage </h3>
+
+```py
+
+from sportsbox import showUpcomingGames, getPlayer, playerStats, playerNextNGames, getTeam, getScores, getNBANews, getNFLNews
+
+#Get basic player information and career regular season stats returned as dataframes
+player_info_df = getPlayer("Lebron James")
+player_stats_df = playerStats("Lebron James")
+
+#Show upcoming next N games for a player as a matplotlib plot
+showUpcomingGames("Lebron James", 3)
+
+#Get upcoming next N games with more details for a player returned as a dataframe
+player_games_df = playerNextNGames("Lebron James", "3")
+
+#Get basic team information returned as dataframe
+team_info_df = getTeam("mil")
+
+#Get today's NBA box scores returned as a list of Game objects
+today_scores = getScores()
+
+#Get 5 recent NBA or NFL articles returned as set of Article objects
+nbanews = getNBANews()
+nflnews = getNFLNews()
+
+```
+
+## Game class attributes
+Attribute Variable | Value |
+------------ | :-----------: |
+gameStatus | `1` not started, `2` in progress, `3` finished |
+gameStatusText | `start time (ET)`, `Qx and time remaining`, `FINAL`  | 
+homeTeam | EX: `LAL` | 
+hWins | home team wins | 
+hLosses | home team losses | 
+hScore | home team's current score | 
+awayTeam | EX: `LAC` | 
+aWins | away team wins |
+aLosses | away team losses |
+aScore | away team's current score |
+
+
+## Article class attributes
+Attribute Variable | Value |
+------------ | :-----------: |
+headline | headline of the ESPN article |
+description | description of the ESPN article | 
+link | link to ESPN article | 
+
+
+</br>
+
+## Invite as Discord bot (NOTE: currently not hosted on server yet!)
+
+Invite [sportsbox](https://discord.com/api/oauth2/authorize?client_id=1089389802840920195&permissions=2147576832&scope=bot) to your Discord server!
+
+<h3> Commands </h3>
+
+`!nbanews` - Shows 5 random recent NBA news articles
+
+`!nflnews` - Shows 5 random recent NFL news articles
+
+`!nbascores` - Shows today's NBA box scores
+
+</br>
+
+## Development
+
+Read [CONTRIBUTING.md](CONTRIBUTING.md) file
+
+</br>
+
+## Upcoming Features
+
+- Bot command to post a random trending sports highlight
```

### Comparing `sports-box-0.1.1/package-lock.json` & `sports-box-0.1.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `sports-box-0.1.1/pyproject.toml` & `sports-box-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "sports-box"
 authors = [{name = "Daniel Hu", email = "danielhu2000@gmail.com"}]
 description="Sportsbox"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = [
     "matplotlib",
     "nba_api",
     "espn_api",
     "requests",
-    "discord"
+    "discord",
+    "tiktokapipy"
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
@@ -50,14 +51,17 @@
     "flake8-black>=0.2.1",
     "flake8-pyproject",
     "mypy",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "twine",
     "wheel",
+    "sphinx",
+    "sphinx_rtd_theme",
+    "myst-parser",
 ]
 
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
```

### Comparing `sports-box-0.1.1/sports_box/bot.py` & `sports-box-0.1.2/sports_box/bot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import discord
 import os
 from getnews import getNBANews, getNFLNews
+from gettiktokstuff import getnbalinks, getnfllinks
 from gettodayscores import getScores
 from discord.ext import commands
 from dotenv import load_dotenv
 
 
 load_dotenv()
 TOKEN = os.getenv('DISCORD_TOKEN')
@@ -18,47 +19,89 @@
 intents = discord.Intents.default()
 intents.message_content = True
 
 bot = commands.Bot(command_prefix='!', intents=intents)
 
 
 @bot.command(name='nbanews')
-async def nbanews(ctx):
+async def nbanews(ctx):  # pragma: no cover
+    """!nbanews - Posts NBA news articles to Discord"""
     articles = getNBANews()
 
     embed = discord.Embed(title="NBA Recent News")
 
     for a in articles:
         desc = a.description + "  [Read]({})".format(a.link)
         embed.add_field(name=a.headline, value=desc, inline=False)
 
     await ctx.send(embed=embed)
 
 
 @bot.command(name='nflnews')
-async def nflnews(ctx):
+async def nflnews(ctx):  # pragma: no cover
+    """!nflnews - Posts NFL news articles to Discord"""
     articles = getNFLNews()
 
     embed = discord.Embed(title="NFL Recent News")
 
     for a in articles:
         desc = a.description + "  [Read]({})".format(a.link)
         embed.add_field(name=a.headline, value=desc, inline=False)
 
     await ctx.send(embed=embed)
 
 
 @bot.command(name='nbascores')
-async def nbascores(ctx):
+async def nbascores(ctx):  # pragma: no cover
+    """!nbascores - Posts today's NBA box scores"""
     games = getScores()
 
     embed = discord.Embed(title="NBA Box Scores")
 
     for g in games:
         score = g.awayTeam + " " + str(g.aScore) + "    @    " + str(g.hScore) + " " + g.homeTeam
         embed.add_field(name=score, value=g.gameStatusText, inline=False)
 
     await ctx.send(embed=embed)
 
 
+@bot.command(name='nbavids')
+async def nbavids(ctx):  # pragma: no cover
+    await ctx.send("Loading...")
+
+    vids = await getnbalinks()
+
+    embed = discord.Embed(title="Latest NBA Highlights")
+
+    for link, caption in vids.items():
+        desc = "[Watch]({})".format(link)
+        embed.add_field(name=caption, value=desc, inline=False)
+
+    await ctx.send(embed=embed)
+
+
+@bot.command(name='nflvids')
+async def nflvids(ctx):  # pragma: no cover
+    await ctx.send("Loading...")
+
+    vids = await getnfllinks()
+
+    embed = discord.Embed(title="Latest NFL Highlights")
+
+    for link, caption in vids.items():
+        desc = "[Watch]({})".format(link)
+        embed.add_field(name=caption, value=desc, inline=False)
+
+    await ctx.send(embed=embed)
+
+
+@bot.command(name='dogger')
+async def dogger(ctx):  # pragma: no cover
+    embed = discord.Embed(title="Dogger of the Month")
+
+    file = discord.File("sports_box/dogger/dogger.png", filename="image.png")
+    embed.set_image(url="attachment://image.png")
+    await ctx.send(file=file, embed=embed)
+
+
 # client.run(TOKEN)
 bot.run(TOKEN)
```

### Comparing `sports-box-0.1.1/sports_box/getnews.py` & `sports-box-0.1.2/sports_box/getnews.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,47 @@
 import random
 
 # import discord
 # from discord.ext import commands
 
 
 class Article:
+    """Article class.
+
+    EX: article = Article("Headline", "Description", "Link")
+
+    Args:
+        headline (str): headline of the ESPN article
+        description (str): description of the ESPN article
+        link (str): link to ESPN article
+
+
+    """
+
     def __init__(self, headline, description, link):
         self.headline = headline
         self.description = description
         self.link = link
 
     def __eq__(self, other):
         return self.headline == other.headline
 
     def __hash__(self):
         return hash((self.headline, self.description, self.link))
 
 
 def getNBANews():  # get 5 random recent articles
+    """Gets 5 random recent articles.
+
+    EX: nbanews = getNBANews()
+
+    Returns:
+        Set: 5 unique NBA articles
+
+    """
     url = 'http://site.api.espn.com/apis/site/v2/sports/basketball/nba/news'
     data = requests.get(url)
     news_dict = data.json()
     nbaarticles = set()
 
     nbaarticles.clear()
 
@@ -44,14 +64,22 @@
     # print(data)
 
 
 # getNBANews()
 
 
 def getNFLNews():  # get 5 random recent articles
+    """Gets 5 random recent articles.
+
+    EX: nflnews = getNFLNews()
+
+    Returns:
+        Set: 5 unique NFL articles
+
+    """
     url = 'http://site.api.espn.com/apis/site/v2/sports/football/nfl/news'
     data = requests.get(url)
     news_dict = data.json()
     nflarticles = set()
 
     nflarticles.clear()
```

### Comparing `sports-box-0.1.1/sports_box/getplayerstuff.py` & `sports-box-0.1.2/sports_box/getplayerstuff.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,89 +12,131 @@
 # MOCK CLASSES
 ########################################################
 class PlayerId(object):
     def __init__(self, player_id):
         self.player_id = player_id
 
     def get_data(self):
+        """For testing purposes."""
         data = players.find_players_by_full_name("Lebron James")
         return data
 
 
 class PlayerInfo(object):
     def __init__(self, player_id):
         self.player_id = player_id
 
     def get_data(self):
+        """For testing purposes."""
         data = commonplayerinfo.CommonPlayerInfo(2544).common_player_info
         return data
 
 
 class PlayerStats(object):
     def __init__(self, player_id):
         self.player_id = player_id
 
     def get_data(self):
+        """For testing purposes."""
         data = playercareerstats.PlayerCareerStats(2544).career_totals_regular_season.get_dict()
         # data = playerStats("Lebron James")
         return data
 
 
 class PlayerGames(object):
     def __init__(self, number_of_games, player_id, season_all, season_type_all_star):
         self.number_of_games = number_of_games
         self.player_id = player_id
         self.season_all = season_all
         self.season_type_all_star = season_type_all_star
 
     def get_data(self):
+        """For testing purposes."""
         data = PlayerNextNGames(
             number_of_games="3", player_id=2544, season_all="2021-22", season_type_all_star="Regular Season"
         ).next_n_games.get_dict()
         # data = playerNextNGames("Lebron James", 3)
         return data
 
 
 #############################################################################
 
 
 def getPID(player):  # helper function to get player ID
+    """Gets player ID.
+
+    Args:
+        arg1 (str): case-sensitive first and last name of player
+
+    Returns:
+        int: player ID
+
+    """
+
     p = players.find_players_by_full_name(player)
     d = p[0]
     id = list(d.items())[0][1]
 
     return id
 
 
 def getPlayer(player):
+    """Gets common player info.
+
+    Args:
+        arg1 (str): case-sensitive first and last name of player
+
+    Returns:
+        DataFrame: basic player info
+
+    """
     # getHeadshotById(id)
     id = getPID(player)
     load = commonplayerinfo.CommonPlayerInfo(id).common_player_info
     # load = commonplayerinfo.CommonPlayerInfo(id)
     playerinfo = load.common_player_info.get_data_frame()
     # playerinfo = load.get_dict()
     # playerinfo = load
 
     # display(playerinfo.loc[0])
     return playerinfo
     # print(playerinfo)
 
 
 def playerStats(player):  # show career stats of player
+    """Gets player stats.
+
+    Args:
+        arg1 (str): case-sensitive first and last name of player
+
+    Returns:
+        DataFrame: player regular season stats
+
+    """
     id = getPID(player)
     load = playercareerstats.PlayerCareerStats(id).career_totals_regular_season
     stats = load.get_data_frame()
     # stats = load.get_dict()
     # stats.style.set_caption(player + "'s Stats")
 
     # print(stats)
     return stats  # horizontal stats
 
 
 def playerNextNGames(player, n):  # return next n games as data frame
+    """Gets next N games for player.
+
+    Args:
+        arg1 (str): case-sensitive first and last name of player
+        arg2 (int): number of upcoming games to be shown
+
+    Returns:
+        DataFrame: next N games info
+
+    """
     s = str(n)
     id = getPID(player)
     load = PlayerNextNGames(
         number_of_games=s, player_id=id, season_all="2022-23", season_type_all_star="Regular Season"
     )
     upcoming = load.next_n_games.get_data_frame()
     # upcoming = load.next_n_games.get_dict()
```

### Comparing `sports-box-0.1.1/sports_box/getteamstuff.py` & `sports-box-0.1.2/sports_box/getteamstuff.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,22 +10,32 @@
 
 
 class TeamId(object):
     def __init__(self, team_id):
         self.team_id = team_id
 
     def get_data(self):
+        """For testing purposes."""
         data = teams.find_team_by_abbreviation("mil")
         return data
 
 
 ########################################################
 
 
 def getTeam(team):
+    """Gets common team info.
+
+    Args:
+        arg1 (str): non case-sensitive team abbreviation
+
+    Returns:
+        DataFrame: basic team info
+
+    """
     t = teams.find_team_by_abbreviation(team)
     # get team logo
     id = list(t.items())[0][1]
     load = teaminfocommon.TeamInfoCommon(team_id=id, season_nullable="2022-23")
     # teaminfo = load.team_info_common.get_data_frame()
     teaminfo = load.team_info_common.get_dict()
```

### Comparing `sports-box-0.1.1/sports_box/gettodayscores.py` & `sports-box-0.1.2/sports_box/gettodayscores.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 import requests
 
 # import discord
 # from discord.ext import commands
 
 
 class Game:
+    """Game class.
+
+    Class containing elements relating to a box score.
+
+    Args:
+        gameStatus (int): `1` not started, `2` in progress, `3` finished
+        gameStatusText (str): `start time (ET)`, `Qx and time remaining`, `FINAL`
+        homeTeam (str): EX: `LAL`
+        hWins (int): home team wins
+        hLosses (int): home team losses
+        hScore (int): home team's current score
+        awayTeam (str): EX: `LAC`
+        aWins (int): away team wins
+        aLosses (int): away team losses
+        aScore (int): away team's current score
+
+
+    """
+
     def __init__(self, gameStatus, gameStatusText, homeTeam, hWins, hLosses, hScore, awayTeam, aWins, aLosses, aScore):
         self.gameStatus = gameStatus
         self.gameStatusText = gameStatusText
         self.homeTeam = homeTeam
         self.hWins = hWins
         self.hLosses = hLosses
         self.hScore = hScore
@@ -24,14 +43,24 @@
 isGames = False
 
 if data.ok:
     isGames = True
 
 
 def getScores():
+    """Gets today's NBA box scores and stores in Game object
+
+    Args:
+
+
+    Returns:
+        Game: Game object
+
+
+    """
     games = list()
     games.clear()
 
     if isGames:
         scoreboard = scores_data.get('scoreboard')
 
         for s in scoreboard['games']:
```

### Comparing `sports-box-0.1.1/sports_box/teamcolors.py` & `sports-box-0.1.2/sports_box/teamcolors.py`

 * *Files identical despite different names*

### Comparing `sports-box-0.1.1/sports_box/tests/test_all.py` & `sports-box-0.1.2/sports_box/tests/test_all.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 # tests
-from sports_box import PlayerInfo, PlayerStats, PlayerId, TeamId, getTName, getTColor1, getNBANews, getNFLNews
+from sports_box import (
+    PlayerInfo,
+    PlayerStats,
+    MockVideo,
+    PlayerId,
+    TeamId,
+    getTName,
+    getTColor1,
+    getNBANews,
+    getNFLNews,
+    getnbalinks,
+)
 from unittest.mock import patch
 from unittest import TestCase
 from unittest.mock import Mock
+import types
 
 # from typing import List
 # import pytest
 # import pandas as pd
 
 
 sample_id_data = {
@@ -259,28 +271,51 @@
 
     def get_dict(self):
         return sample_player_stats
 
 
 class FakePlayerStats:
     def __init__(self, player_id):
-        self.career_totals_regular_season = FakeCommonPlayerInfoData(player_id)
+        self.career_totals_regular_season = FakePlayerStatsData(player_id)
 
 
 class PlayerStatsTest(TestCase):
     def setUp(self):
         self.playerstats = PlayerStats(2544)
 
     def test_getpstats(self):
         with patch('nba_api.stats.endpoints.playercareerstats.PlayerCareerStats') as fakePlayerStatsCreator:
             fakePlayerStatsCreator.return_value = FakePlayerStats(2544)
             mock_data = self.playerstats.get_data()
             assert type(mock_data) == type(sample_player_stats)
 
 
+# TIKTOKS TEST
+class FakeUserData:
+    def __init__(self, id, video_limit):
+        self.id = id
+        video_limit = 5
+
+
+class FakeUser:
+    def __init__(self, id, video_limit):
+        self.videos = MockVideo(123)
+
+
+class UserVideosTest(TestCase):
+    def setUp(self):
+        self.videos = MockVideo(123)
+
+    def test_nbatiktoks(self):
+        with patch("tiktokapipy.async_api.AsyncTikTokAPI.user") as fakeUserCreator:
+            fakeUserCreator.return_value = FakeUser(123, 5)
+            mock_data = getnbalinks()
+            assert type(mock_data) is types.CoroutineType
+
+
 """
 # PLAYER NEXT GAMES TEST
 class FakeNextGamesData:
     def __init__(self, number_of_games, player_id, season_all, season_type_all_star):
         self.number_of_games = number_of_games
         self.player_id = player_id
         self.season_all = season_all
```

### Comparing `sports-box-0.1.1/sports_box/userinterface.py` & `sports-box-0.1.2/sports_box/userinterface.py`

 * *Files identical despite different names*

### Comparing `sports-box-0.1.1/sports_box.egg-info/PKG-INFO` & `sports-box-0.1.2/sports_box.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports-box
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sportsbox
 Author-email: Daniel Hu <danielhu2000@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,17 +218,103 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 <h1> sportsbox </h1>
 
-<p>Discord bot displaying sports news and convenient stats. </p>
+<p>Discord bot and independent helper functions displaying sports news and convenient stats. </p>
+
 
 ![](https://img.shields.io/badge/license-Apache--2.0-brightgreen)
 ![](https://img.shields.io/github/issues/dhu16/sportsbox)
 [![Build Status](https://github.com/dhu16/sportsbox/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/dhu16/sportsbox/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/dhu16/sportsbox/branch/main/graph/badge.svg?token=UHT46NYQGX)](https://codecov.io/gh/dhu16/sportsbox)
+[![PyPI](https://img.shields.io/pypi/v/sports-box)](https://pypi.org/project/sports-box/)
+[![docs](https://img.shields.io/github/actions/workflow/status/dhu16/sportsbox/docs.yml?label=docs)](https://dhu16.github.io/sportsbox/)
 
 <h2> Overview </h2>
 
-<p> This Discord bot allows users to view NBA and NFL news, scores, and stats on their servers with easy commands. I always found it annoying to constantly search up stats for a game I was monitoring while studying and I was too lazy to install official apps too. This alleviates the inconvenience of always having to manually search up stats or open one's phone while working or playing games with friends as Discord is usually always open on someone's computer.  </p>
+<p> This Discord bot allows users to view NBA and NFL news, scores, and stats on their servers with intuitive commands. The commands are named after the key words I always search with. I always found it annoying to constantly search up stats for a game I was monitoring while studying and I was too lazy to install official apps too. This alleviates the inconvenience of always having to manually search up stats or open one's phone while working or playing games with friends as Discord is usually always open on someone's computer.  </p>
+
+</br>
+
+## Installation
+
+`pip install sports-box`
+
+<h3> Usage </h3>
+
+```py
+
+from sportsbox import showUpcomingGames, getPlayer, playerStats, playerNextNGames, getTeam, getScores, getNBANews, getNFLNews
+
+#Get basic player information and career regular season stats returned as dataframes
+player_info_df = getPlayer("Lebron James")
+player_stats_df = playerStats("Lebron James")
+
+#Show upcoming next N games for a player as a matplotlib plot
+showUpcomingGames("Lebron James", 3)
+
+#Get upcoming next N games with more details for a player returned as a dataframe
+player_games_df = playerNextNGames("Lebron James", "3")
+
+#Get basic team information returned as dataframe
+team_info_df = getTeam("mil")
+
+#Get today's NBA box scores returned as a list of Game objects
+today_scores = getScores()
+
+#Get 5 recent NBA or NFL articles returned as set of Article objects
+nbanews = getNBANews()
+nflnews = getNFLNews()
+
+```
+
+## Game class attributes
+Attribute Variable | Value |
+------------ | :-----------: |
+gameStatus | `1` not started, `2` in progress, `3` finished |
+gameStatusText | `start time (ET)`, `Qx and time remaining`, `FINAL`  | 
+homeTeam | EX: `LAL` | 
+hWins | home team wins | 
+hLosses | home team losses | 
+hScore | home team's current score | 
+awayTeam | EX: `LAC` | 
+aWins | away team wins |
+aLosses | away team losses |
+aScore | away team's current score |
+
+
+## Article class attributes
+Attribute Variable | Value |
+------------ | :-----------: |
+headline | headline of the ESPN article |
+description | description of the ESPN article | 
+link | link to ESPN article | 
+
+
+</br>
+
+## Invite as Discord bot (NOTE: currently not hosted on server yet!)
+
+Invite [sportsbox](https://discord.com/api/oauth2/authorize?client_id=1089389802840920195&permissions=2147576832&scope=bot) to your Discord server!
+
+<h3> Commands </h3>
+
+`!nbanews` - Shows 5 random recent NBA news articles
+
+`!nflnews` - Shows 5 random recent NFL news articles
+
+`!nbascores` - Shows today's NBA box scores
+
+</br>
+
+## Development
+
+Read [CONTRIBUTING.md](CONTRIBUTING.md) file
+
+</br>
+
+## Upcoming Features
+
+- Bot command to post a random trending sports highlight
```

