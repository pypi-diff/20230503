# Comparing `tmp/fastapi-listing-0.0.4.tar.gz` & `tmp/fastapi-listing-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-listing-0.0.4.tar", last modified: Sun Apr 30 13:27:15 2023, max compression
+gzip compressed data, was "fastapi-listing-0.0.5.tar", last modified: Wed May  3 18:30:26 2023, max compression
```

## Comparing `fastapi-listing-0.0.4.tar` & `fastapi-listing-0.0.5.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.470801 fastapi-listing-0.0.4/fastapi_listing/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/base_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/abstracts/sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/dao/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/dao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/dao/generic_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/factory/_generic_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/factory/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/factory/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/filters/generic_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/interface/listing_meta_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/mechanics/iterative_filter_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/mechanics/singleton_sorter_mechanics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/paginator/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/paginator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/paginator/naive_page_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/service/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/service/listing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/sorter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/sorter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/sorter/naive_page_sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/fastapi_listing/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/strategies/query_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/fastapi_listing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:27:15.470801 fastapi-listing-0.0.4/fastapi_listing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 13:27:15.000000 fastapi-listing-0.0.4/fastapi_listing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 13:27:15.474802 fastapi-listing-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-30 13:27:04.000000 fastapi-listing-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.161166 fastapi-listing-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-03 18:30:26.161166 fastapi-listing-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.149164 fastapi-listing-0.0.5/fastapi_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.153164 fastapi-listing-0.0.5/fastapi_listing/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/base_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/abstracts/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.153164 fastapi-listing-0.0.5/fastapi_listing/dao/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/dao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/dao/generic_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.153164 fastapi-listing-0.0.5/fastapi_listing/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/factory/_generic_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/factory/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/factory/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.153164 fastapi-listing-0.0.5/fastapi_listing/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/filters/generic_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/interface/listing_meta_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/mechanics/iterative_filter_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/mechanics/singleton_sorter_mechanics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/paginator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/paginator/naive_page_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/service/listing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.157165 fastapi-listing-0.0.5/fastapi_listing/sorter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/sorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/sorter/naive_page_sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.161166 fastapi-listing-0.0.5/fastapi_listing/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/strategies/query_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/fastapi_listing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:30:26.149164 fastapi-listing-0.0.5/fastapi_listing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 18:30:26.000000 fastapi-listing-0.0.5/fastapi_listing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:30:26.161166 fastapi-listing-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-03 18:30:15.000000 fastapi-listing-0.0.5/setup.py
```

### Comparing `fastapi-listing-0.0.4/PKG-INFO` & `fastapi-listing-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi-listing
-Version: 0.0.4
-Summary: Data Listing Library for FastAPI
+Version: 0.0.5
+Summary: Advaned Data Listing Library for FastAPI
 Home-page: https://github.com/danielhasan1/fastapi-listing
 Author: Danish Hasan
 Author-email: dh813030@gmail.com
 Keywords: starlette,fastapi,starlite,pydantic
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `fastapi-listing-0.0.4/fastapi_listing/__init__.py` & `fastapi-listing-0.0.5/fastapi_listing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fastapi_listing.factory import strategy_factory
 from fastapi_listing.strategies import NaiveQueryStrategy, NaivePaginationStrategy, SortingOrderStrategy
 from fastapi_listing.service.listing_main import ListingService, FastapiListing
 from fastapi_listing.mechanics import IterativeFilterMechanics, SingletonSorterMechanics
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 strategy_factory.register_strategy("naive_paginator", NaivePaginationStrategy)
 strategy_factory.register_strategy("naive_sorter", SortingOrderStrategy)
 strategy_factory.register_strategy("naive_query", NaiveQueryStrategy)
 strategy_factory.register_strategy("iterative_filter_mechanics", IterativeFilterMechanics)
 strategy_factory.register_strategy("singleton_sorter_mechanics", SingletonSorterMechanics)
```

### Comparing `fastapi-listing-0.0.4/fastapi_listing/abstracts/dao.py` & `fastapi-listing-0.0.5/fastapi_listing/abstracts/dao.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from abc import ABCMeta, abstractmethod
 
 from fastapi_listing.typing import SqlAlchemyModel
 
 
 class DaoAbstract(metaclass=ABCMeta):
 
+    @property
+    @abstractmethod
+    def model(self):
+        pass
+
     @abstractmethod
     def create(self, values: dict[str, str | int]) -> SqlAlchemyModel:
         pass
 
     @abstractmethod
     def update(self, identifier: dict[str, str | int | list], values: dict) -> bool:
         pass
```

### Comparing `fastapi-listing-0.0.4/fastapi_listing/abstracts/listing.py` & `fastapi-listing-0.0.5/fastapi_listing/abstracts/listing.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/dao/generic_dao.py` & `fastapi-listing-0.0.5/fastapi_listing/dao/generic_dao.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fastapi_listing.abstracts import DaoAbstract
 from sqlalchemy.orm import Session
 
 from fastapi_listing.typing import SqlAlchemyModel
 
 
-class GenericDao(DaoAbstract):
+class GenericDao(DaoAbstract):  # type:ignore # noqa
     """
     Dao stands for data access object.
     This layers encapsulates all logic that a user may write
     in order to interact with databases.
     Dao has only one responsibility that is to communicate with
     database, all logic regarding data manipulation should live at
     service layer. This also acts as a gateway to database
@@ -26,46 +26,61 @@
     objects context here that one dao object should only have one primary model
     but one dao object can talk to multiple models with having first primary model.
 
     Note - no data validation should happen at this layer. That should be prior to pushing
     at this layer.
     """
 
-    model_kls: SqlAlchemyModel = None
+    # model: SqlAlchemyModel = None to be defined at model dao level
 
-    def __init__(self, **kwargs):
+    def __init__(self, read_db=None, write_db=None):
         # considering that we are dealing with separate read and write dbs.
         # we must have two sessions one for read replica and one for master or write replica
         # we should define our reusable attributes here that we will use in each dao method definition
-        self._read_db: Session = kwargs.get("read_db")
-        self._write_db: Session = kwargs.get("write_db")
-        if self.model_kls is None:
-            raise ValueError("model class is not set!")
-        self.model = self.model_kls
+        # even if we are using single db still having two references for the same session won't hurt
+        # for future expansion once we decide to move on to read/write replica architecure
+        # we already have groundwork done and only need to push different connections
+        # from request lifecycle layer.
+        self._read_db: Session = read_db #kwargs.get("read_db")
+        self._write_db: Session = write_db #kwargs.get("write_db")
+        # if self.model is None:
+        #     raise ValueError("model class is not set!")
+
+    # def __setattr__(cls, name, value):
+    #     if name == "model":
+    #         raise AttributeError("Cannot modify .model")
+    #     else:
+    #         return type.__setattr__(cls, name, value)
+    #
+    # def __delattr__(cls, name):
+    #     if name == "model":
+    #         raise AttributeError("Cannot delete .model")
+    #     else:
+    #         return type.__delattr__(cls, name)
 
     def create(self, values: dict[str, str | int]) -> SqlAlchemyModel:
         """
         A light method that enters values in primary model table.
         single value at a time receives a dict implementation could map the dict with model values and
         insert that mapping or single row into the table.
         :param values: dict of values where keys are columns of table and value should be row values
         :return: created object i.e., instrumented row object.
         """
-        pass
+        raise NotImplementedError
 
     def update(self, identifier: dict[str, str | int | list], values: dict) -> bool:
         """
         Similar to create method this receives an identifier
         :param identifier:
         :param values:
         :return:
         """
-        pass
+        raise NotImplementedError
 
     def read(self, identifier: dict[str, str | int | list], fields: list | str = "__all__") -> SqlAlchemyModel:
-        pass
+        raise NotImplementedError
 
     def delete(self, ids: list[int]) -> bool:
-        pass
+        raise NotImplementedError
 
     def get_naive_read(self, fields_to_read: list):
         return self._read_db.query(*fields_to_read)
```

### Comparing `fastapi-listing-0.0.4/fastapi_listing/factory/_generic_factory.py` & `fastapi-listing-0.0.5/fastapi_listing/factory/_generic_factory.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/factory/strategy.py` & `fastapi-listing-0.0.5/fastapi_listing/factory/strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/filters/generic_filters.py` & `fastapi-listing-0.0.5/fastapi_listing/filters/generic_filters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,140 +1,154 @@
 from datetime import datetime
 
 from fastapi_listing.abstracts import FilterAbstract
+from fastapi_listing.typing import SqlAlchemyQuery, AnySqlAlchemyColumn
 
 
 class CommonFilterImpl(FilterAbstract):
 
     def __init__(self, dao=None, request=None, extra_context=None):
         self.dao = dao
         self.request = request
         self.extra_context = extra_context
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
+    def extract_field(self, field: str) -> AnySqlAlchemyColumn:
+        return getattr(self.dao.model, field.split(".")[-1])
+
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
         raise NotImplementedError("To be implemented in child class!")
 
 
 class EqualityFilter(CommonFilterImpl):
 
-    def filter(self, *, field=None, value=None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-
-        query = query.filter(inst_field == value.get("search"))
+    def filter(self, *, field=None, value=None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field == value.get("search"))
         return query
 
 
 class InEqualityFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
         if value:
             query = query.filter(inst_field != value.get("search"))
         return query
 
 
 class InDataFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field.in_(value.get("list")))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field.in_(value.get("list")))
         return query
 
 
-class BetweenDateFilter(CommonFilterImpl):
+class BetweenUnixMilliSecDateFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field.between(datetime.fromtimestamp(int(value.get('start')) / 1000),
-                                                datetime.fromtimestamp(int(value.get('end')) / 1000)))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field.between(datetime.fromtimestamp(int(value.get('start')) / 1000),
+                                                    datetime.fromtimestamp(int(value.get('end')) / 1000)))
         return query
 
 
 class StringStartsWithFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field.startswith(value.get("search")))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field.startswith(value.get("search")))
         return query
 
 
 class StringEndsWithFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field.endswith(value.get("search")))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field.endswith(value.get("search")))
         return query
 
 
 class StringContainsFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field.contains(value.get("search")))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field.contains(value.get("search")))
         return query
 
 
 class StringLikeFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field.like(value.get("search")))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field.like(value.get("search")))
         return query
 
 
 class DataGreaterThanFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field > value.get("search"))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field > value.get("search"))
         return query
 
 
 class DataGreaterThanEqualToFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field >= value.get("search"))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field >= value.get("search"))
         return query
 
 
 class DataLessThanFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field < value.get("search"))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field < value.get("search"))
         return query
 
 
 class DataLessThanEqualToFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
-        query = query.filter(inst_field <= value.get("search"))
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field <= value.get("search"))
         return query
 
 
 class DataGropByElementFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
         query = query.group_by(inst_field)
         return query
 
 
 class DataDistinctByElementFilter(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
         query = query.distinct(inst_field)
         return query
 
 
 class HasFieldValue(CommonFilterImpl):
 
-    def filter(self, *, field: str = None, value: dict = None, query=None):
-        inst_field = getattr(self.dao.model, field.split(".")[1])
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
         if value.get("search"):
             query = query.filter(inst_field.is_not(None))
         else:
             query = query.filter(inst_field.is_(None))
         return query
```

### Comparing `fastapi-listing-0.0.4/fastapi_listing/interface/listing_meta_info.py` & `fastapi-listing-0.0.5/fastapi_listing/interface/listing_meta_info.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/loader.py` & `fastapi-listing-0.0.5/fastapi_listing/loader.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/mechanics/iterative_filter_mechanics.py` & `fastapi-listing-0.0.5/fastapi_listing/mechanics/iterative_filter_mechanics.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/mechanics/singleton_sorter_mechanics.py` & `fastapi-listing-0.0.5/fastapi_listing/mechanics/singleton_sorter_mechanics.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/paginator/naive_page_builder.py` & `fastapi-listing-0.0.5/fastapi_listing/paginator/naive_page_builder.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/service/listing_main.py` & `fastapi-listing-0.0.5/fastapi_listing/service/listing_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from fastapi_listing.abstracts import TableDataPaginatingStrategy
 from fastapi_listing.typing import ListingResponseType
 from fastapi_listing.abstracts import ListingBase, ListingServiceBase
 from fastapi_listing.factory import strategy_factory
 from fastapi_listing.errors import ListingFilterError, ListingSorterError
 from fastapi_listing.dao.generic_dao import GenericDao
 from fastapi_listing.interface.listing_meta_info import ListingMetaInfo
-from fastapi_listing.factory import _generic_factory
+from fastapi_listing import constants
+import os
 
 try:
     from pydantic import BaseModel
 
     HAS_PYDANTIC = True
 except ImportError:
     HAS_PYDANTIC = False
@@ -118,15 +119,17 @@
         page = paginate_strategy.paginate(query, self.request, extra_context)
         return page
 
     def _prepare_query(self, listing_meta_info: ListingMetaInfo) -> Query:
         base_query: Query = listing_meta_info.query_strategy.get_query(request=self.request,
                                                                        dao=self.dao,
                                                                        extra_context=listing_meta_info.extra_context)
-        fltr_query: Query = self._apply_filters(base_query, listing_meta_info)
+        if base_query is None or not base_query:
+            raise ValueError("query strategy returned nothing Query object is expected!")
+        fltr_query: Query = self._apply_filters(base_query, listing_meta_info) # expects a query but none returned when custom strategy return none etc
         srtd_query: Query = self._apply_sorting(fltr_query, listing_meta_info)
         return srtd_query
 
     @staticmethod
     def _set_vals_in_extra_context(extra_context: dict, **kwargs):
         extra_context.update(kwargs)
 
@@ -137,20 +140,20 @@
                                         )
         fnl_query: Query = self._prepare_query(listing_meta_info)
         response: ListingResponseType = self._paginate(fnl_query, listing_meta_info.paginating_strategy,
                                                        listing_meta_info.extra_context)
         return response
 
 
-class ListingService(ListingServiceBase):
+class ListingService(ListingServiceBase): # noqa
     filter_mapper: dict = {}
     sort_mapper: dict = {}
     # here resource creation should be based on factory and not inline as we are separating creation from usage.
     # factory should deliver sorting resource
-    DEFAULT_SRT_ON: str = "created_at"
+    # DEFAULT_SRT_ON: str = "created_at" # to be taken by user at child class level
     DEFAULT_SRT_ORD: str = "dsc"
     PAGINATE_STRATEGY: str = "naive_paginator"
     QUERY_STRATEGY: str = "naive_query"
     SORTING_STRATEGY: str = "naive_sorter"
     SORT_MECHA: str = "singleton_sorter_mechanics"
     FILTER_MECHA: str = "iterative_filter_mechanics"
     dao_kls: GenericDao = GenericDao
@@ -158,22 +161,33 @@
     # pydantic_serializer: Type[BaseModel] = None
     # allowed_pydantic_custom_fields: bool = False
     # it is possible to have more than one serializer for particular endpoint depending upon
     # user or a query/path param condition we could switch json schema so allowing this
     # flexibility for the user to be able to switch between schema Fastapilisting object
     # should get initialized at user level and not implicit.
 
-    def __init__(self, request, **kwargs) -> None:
-        self.dao = self.dao_kls(**kwargs)
+    def __init__(self, request: Request, read_db=None, write_db=None, **kwargs) -> None:
+        # self.dao = self.dao_kls(**kwargs)
         # pop out db sessions as they are concrete property of data access layer and not service layer.
-        # once injected to dao popping out here
-        kwargs.pop("read_db", None)
-        kwargs.pop("write_db", None)
         self.request = request
         self.extra_context = kwargs
+        # ideally dao shouldn't have anything to do with extra_context i.e., kwargs
+        # but in case someone could find any use of it we pushed prepare_dap below
+        # so user could hack prepare_dao hook to do unwanted things.
+        self._prepare_dao(read_db, write_db)
+
+    def _prepare_dao(self, read_db, write_db):
+
+        self.dao = self.dao_kls(read_db=read_db, write_db=write_db)
+        # once dao is prepared and linked with listing service
+        # we don't need it's dependent params anymore.
+        # to only allowing db access on a single layer i.e. dao (data access object layer)
+        # in case user has only one db for read/write
+        # they can send read_db = write_db = db
+        # both variable will still refer to same session
 
     def get_listing(self):
         """
         implement at child class level.
 
         FastapiListing(self.request, self.dao, pydantic_serializer=some_pydantic_model_class,
          custom_fields=True/False).get_response(self.MetaInfo(self))
@@ -216,22 +230,14 @@
             self.sorter_mechanic = outer_instance.SORT_MECHA
             self.filter_mechanic = outer_instance.FILTER_MECHA
             self.extra_context = outer_instance.extra_context
 
     def meta_info_generator(self) -> ListingMetaInfo:
         return ListingService.MetaInfo(self)  # type:ignore # noqa # some issue is coming in pycharm for return types
 
-    @classmethod
-    def get_aliased_filter_mapper(cls) -> dict[str, str]:
-        return {key: key for key, val in cls.filter_mapper.items()}
-
-    @classmethod
-    def get_aliased_sort_mapper(cls) -> dict[str, str]:
-        return {key: key for key, val in cls.sort_mapper.items()}
-
     # @staticmethod
     # def get_sort_mecha_plugin_path() -> str:
     #     """
     #     hook to provide sort mecha plugin module path as py import path
     #     overwrite allowed to provide custom path.
     #     :return: import path as string ex. fastapi_listing.mechanics.sorter_mechanics.
     #     """
```

### Comparing `fastapi-listing-0.0.4/fastapi_listing/sorter/naive_page_sorter.py` & `fastapi-listing-0.0.5/fastapi_listing/sorter/naive_page_sorter.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/strategies/query_strategy.py` & `fastapi-listing-0.0.5/fastapi_listing/strategies/query_strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.4/fastapi_listing/typing.py` & `fastapi-listing-0.0.5/fastapi_listing/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 # will support future imports as well like pymongo and other orm tools
 
 try:
     from sqlalchemy.orm.decl_api import DeclarativeMeta
     from sqlalchemy.orm import Query
     from sqlalchemy.orm import Session
     from sqlalchemy.sql.sqltypes import TypeEngine
+    from sqlalchemy.sql.schema import Column
 except ImportError:
     DeclarativeMeta = None
     Query = None
     Session = None
-    TypeEngine = None
+    Column = None
 
 
 class ListingResponseType(TypedDict):
     data: List[Dict[str, int | str | list | dict]]
     currentPageNumber: int
     currentPageSize: int
     totalCount: int
     hasNext: bool
 
 
 SqlAlchemyQuery = TypeVar("SqlAlchemyQuery", bound=Query)
 SqlAlchemySession = TypeVar("SqlAlchemySession", bound=Session)
 FastapiRequest = TypeVar("FastapiRequest", bound=Request)
-AnySqlAlchemyColumn = TypeVar("AnySqlAlchemyColumn", bound=TypeEngine)
+AnySqlAlchemyColumn = TypeVar("AnySqlAlchemyColumn", bound=Column)
 SqlAlchemyModel = TypeVar("SqlAlchemyModel", bound=DeclarativeMeta)
```

### Comparing `fastapi-listing-0.0.4/fastapi_listing.egg-info/PKG-INFO` & `fastapi-listing-0.0.5/fastapi_listing.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi-listing
-Version: 0.0.4
-Summary: Data Listing Library for FastAPI
+Version: 0.0.5
+Summary: Advaned Data Listing Library for FastAPI
 Home-page: https://github.com/danielhasan1/fastapi-listing
 Author: Danish Hasan
 Author-email: dh813030@gmail.com
 Keywords: starlette,fastapi,starlite,pydantic
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `fastapi-listing-0.0.4/fastapi_listing.egg-info/SOURCES.txt` & `fastapi-listing-0.0.5/fastapi_listing.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 fastapi_listing/__init__.py
+fastapi_listing/constants.py
 fastapi_listing/errors.py
 fastapi_listing/loader.py
 fastapi_listing/py.typed
 fastapi_listing/typing.py
 fastapi_listing/utils.py
 fastapi_listing.egg-info/PKG-INFO
 fastapi_listing.egg-info/SOURCES.txt
```

### Comparing `fastapi-listing-0.0.4/setup.py` & `fastapi-listing-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
 
 setuptools.setup(
     name="fastapi-listing",
     version=get_version(),
     author="Danish Hasan",
     author_email="dh813030@gmail.com",
-    description="Data Listing Library for FastAPI",
+    description="Advaned Data Listing Library for FastAPI",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/danielhasan1/fastapi-listing",
     packages=setuptools.find_packages(exclude=["tests.*"]),
     package_data={"fastapi_listing": ["py.typed"]},
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
```

