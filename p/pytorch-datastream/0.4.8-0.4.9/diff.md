# Comparing `tmp/pytorch_datastream-0.4.8.tar.gz` & `tmp/pytorch_datastream-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_datastream-0.4.8.tar", max compression
+gzip compressed data, was "pytorch_datastream-0.4.9.tar", max compression
```

## Comparing `pytorch_datastream-0.4.8.tar` & `pytorch_datastream-0.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    90835 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/LICENSE
--rw-r--r--   0        0        0     3233 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/README.rst
--rw-r--r--   0        0        0      259 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/__init__.py
--rw-r--r--   0        0        0    27423 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/dataset.py
--rw-r--r--   0        0        0    17306 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/datastream.py
--rw-r--r--   0        0        0      368 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/samplers/__init__.py
--rw-r--r--   0        0        0     2977 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/samplers/merge_sampler.py
--rw-r--r--   0        0        0     2551 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/samplers/multi_sampler.py
--rw-r--r--   0        0        0     1705 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/samplers/repeat_sampler.py
--rw-r--r--   0        0        0      672 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/samplers/sequential_sampler.py
--rw-r--r--   0        0        0     1729 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/samplers/standard_sampler.py
--rw-r--r--   0        0        0     2442 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/samplers/zip_sampler.py
--rw-r--r--   0        0        0      454 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/tools/__init__.py
--rw-r--r--   0        0        0      980 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/tools/numpy_seed.py
--rw-r--r--   0        0        0      323 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/tools/repeat_map_chain.py
--rw-r--r--   0        0        0     7479 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/tools/split_dataframes.py
--rw-r--r--   0        0        0      181 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/tools/star.py
--rw-r--r--   0        0        0     1363 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/tools/starcompose.py
--rw-r--r--   0        0        0     1332 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/tools/stratified_split.py
--rw-r--r--   0        0        0      706 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/tools/unstratified_split.py
--rw-r--r--   0        0        0     1286 2022-10-25 20:03:51.238277 pytorch_datastream-0.4.8/datastream/tools/verify_split.py
--rw-r--r--   0        0        0     1675 2022-10-25 20:05:05.623324 pytorch_datastream-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     4137 1970-01-01 00:00:00.000000 pytorch_datastream-0.4.8/setup.py
--rw-r--r--   0        0        0     4709 1970-01-01 00:00:00.000000 pytorch_datastream-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    90835 2023-05-03 14:48:12.183126 pytorch_datastream-0.4.9/LICENSE
+-rw-r--r--   0        0        0     3233 2023-05-03 14:48:12.183126 pytorch_datastream-0.4.9/README.rst
+-rw-r--r--   0        0        0      259 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/__init__.py
+-rw-r--r--   0        0        0    27423 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/dataset.py
+-rw-r--r--   0        0        0    17306 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/datastream.py
+-rw-r--r--   0        0        0      368 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/samplers/__init__.py
+-rw-r--r--   0        0        0     2977 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/samplers/merge_sampler.py
+-rw-r--r--   0        0        0     2551 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/samplers/multi_sampler.py
+-rw-r--r--   0        0        0     1705 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/samplers/repeat_sampler.py
+-rw-r--r--   0        0        0      672 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/samplers/sequential_sampler.py
+-rw-r--r--   0        0        0     1729 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/samplers/standard_sampler.py
+-rw-r--r--   0        0        0     2442 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/samplers/zip_sampler.py
+-rw-r--r--   0        0        0      454 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/tools/__init__.py
+-rw-r--r--   0        0        0      980 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/tools/numpy_seed.py
+-rw-r--r--   0        0        0      323 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/tools/repeat_map_chain.py
+-rw-r--r--   0        0        0     7479 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/tools/split_dataframes.py
+-rw-r--r--   0        0        0      181 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/tools/star.py
+-rw-r--r--   0        0        0     1363 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/tools/starcompose.py
+-rw-r--r--   0        0        0     1332 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/tools/stratified_split.py
+-rw-r--r--   0        0        0      706 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/tools/unstratified_split.py
+-rw-r--r--   0        0        0     1286 2023-05-03 14:48:12.187126 pytorch_datastream-0.4.9/datastream/tools/verify_split.py
+-rw-r--r--   0        0        0     1675 2023-05-03 14:51:00.203599 pytorch_datastream-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 pytorch_datastream-0.4.9/setup.py
+-rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 pytorch_datastream-0.4.9/PKG-INFO
```

### Comparing `pytorch_datastream-0.4.8/LICENSE` & `pytorch_datastream-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/README.rst` & `pytorch_datastream-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/dataset.py` & `pytorch_datastream-0.4.9/datastream/dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/datastream.py` & `pytorch_datastream-0.4.9/datastream/datastream.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/samplers/merge_sampler.py` & `pytorch_datastream-0.4.9/datastream/samplers/merge_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/samplers/multi_sampler.py` & `pytorch_datastream-0.4.9/datastream/samplers/multi_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/samplers/repeat_sampler.py` & `pytorch_datastream-0.4.9/datastream/samplers/repeat_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/samplers/sequential_sampler.py` & `pytorch_datastream-0.4.9/datastream/samplers/sequential_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/samplers/standard_sampler.py` & `pytorch_datastream-0.4.9/datastream/samplers/standard_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/samplers/zip_sampler.py` & `pytorch_datastream-0.4.9/datastream/samplers/zip_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/tools/numpy_seed.py` & `pytorch_datastream-0.4.9/datastream/tools/numpy_seed.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/tools/split_dataframes.py` & `pytorch_datastream-0.4.9/datastream/tools/split_dataframes.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/tools/starcompose.py` & `pytorch_datastream-0.4.9/datastream/tools/starcompose.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/tools/stratified_split.py` & `pytorch_datastream-0.4.9/datastream/tools/stratified_split.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/tools/unstratified_split.py` & `pytorch_datastream-0.4.9/datastream/tools/unstratified_split.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/datastream/tools/verify_split.py` & `pytorch_datastream-0.4.9/datastream/tools/verify_split.py`

 * *Files identical despite different names*

### Comparing `pytorch_datastream-0.4.8/pyproject.toml` & `pytorch_datastream-0.4.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytorch-datastream"
-version = "v0.4.8"
+version = "v0.4.9"
 description = "Simple dataset to dataloader library for pytorch"
 authors = ["NextML"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/nextml-code/pytorch-datastream"
 documentation = "https://pytorch-datastream.readthedocs.io"
 keywords = [
@@ -31,24 +31,24 @@
 ]
 packages = [
     { include = "datastream" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-torch = "^1.4.0"
+torch = ">=1.4.0"
 numpy = "^1.17.0"
 pandas = "^1.0.5"
 pydantic = "^1.5.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.6.0"
 flake8 = "^3.8.4"
 pytest = "^6.1.2"
-black = "^22.10.0"
+black = "^23.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `pytorch_datastream-0.4.8/setup.py` & `pytorch_datastream-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.17.0,<2.0.0',
  'pandas>=1.0.5,<2.0.0',
  'pydantic>=1.5.0,<2.0.0',
- 'torch>=1.4.0,<2.0.0']
+ 'torch>=1.4.0']
 
 setup_kwargs = {
     'name': 'pytorch-datastream',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'Simple dataset to dataloader library for pytorch',
     'long_description': "==================\nPytorch Datastream\n==================\n\n.. image:: https://badge.fury.io/py/pytorch-datastream.svg\n       :target: https://badge.fury.io/py/pytorch-datastream\n\n.. image:: https://img.shields.io/pypi/pyversions/pytorch-datastream.svg\n       :target: https://pypi.python.org/pypi/pytorch-datastream\n\n.. image:: https://readthedocs.org/projects/pytorch-datastream/badge/?version=latest\n       :target: https://pytorch-datastream.readthedocs.io/en/latest/?badge=latest\n\n.. image:: https://img.shields.io/pypi/l/pytorch-datastream.svg\n       :target: https://pypi.python.org/pypi/pytorch-datastream\n\n\n\nThis is a simple library for creating readable dataset pipelines and\nreusing best practices for issues such as imbalanced datasets. There are\njust two components to keep track of: ``Dataset`` and ``Datastream``.\n\n``Dataset`` is a simple mapping between an index and an example. It provides \npipelining of functions in a readable syntax originally adapted from\ntensorflow 2's ``tf.data.Dataset``.\n\n``Datastream`` combines a ``Dataset`` and a sampler into a stream of examples.\nIt provides a simple solution to oversampling / stratification, weighted\nsampling, and finally converting to a ``torch.utils.data.DataLoader``.\n\nInstall\n=======\n\n.. code-block::\n\n    poetry add pytorch-datastream\n\nOr, for the old-timers:\n\n.. code-block::\n\n    pip install pytorch-datastream\n\nUsage\n=====\n\nThe list below is meant to showcase functions that are useful in most standard\nand non-standard cases. It is not meant to be an exhaustive list. See the \n`documentation <https://pytorch-datastream.readthedocs.io/en/latest/>`_ for \na more extensive list on API and usage.\n\n.. code-block:: python\n\n    Dataset.from_subscriptable\n    Dataset.from_dataframe\n    Dataset\n        .map\n        .subset\n        .split\n        .cache\n        .with_columns\n\n    Datastream.merge\n    Datastream.zip\n    Datastream\n        .map\n        .data_loader\n        .zip_index\n        .update_weights_\n        .update_example_weight_\n        .weight\n        .state_dict\n        .load_state_dict\n\nMerge / stratify / oversample datastreams\n-----------------------------------------\nThe fruit datastreams given below repeatedly yields the string of its fruit\ntype.\n\n.. code-block:: python\n\n    >>> datastream = Datastream.merge([\n    ...     (apple_datastream, 2),\n    ...     (pear_datastream, 1),\n    ...     (banana_datastream, 1),\n    ... ])\n    >>> next(iter(datastream.data_loader(batch_size=8)))\n    ['apple', 'apple', 'pear', 'banana', 'apple', 'apple', 'pear', 'banana']\n\nZip independently sampled datastreams\n-------------------------------------\nThe fruit datastreams given below repeatedly yields the string of its fruit\ntype.\n\n.. code-block:: python\n\n    >>> datastream = Datastream.zip([\n    ...     apple_datastream,\n    ...     Datastream.merge([pear_datastream, banana_datastream]),\n    ... ])\n    >>> next(iter(datastream.data_loader(batch_size=4)))\n    [('apple', 'pear'), ('apple', 'banana'), ('apple', 'pear'), ('apple', 'banana')]\n\nMore usage examples\n-------------------\nSee the `documentation <https://pytorch-datastream.readthedocs.io/en/latest/>`_\nfor more usage examples.\n\nInstall from source\n===================\n\n.. pip install -e .\n",
     'author': 'NextML',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nextml-code/pytorch-datastream',
```

### Comparing `pytorch_datastream-0.4.8/PKG-INFO` & `pytorch_datastream-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-datastream
-Version: 0.4.8
+Version: 0.4.9
 Summary: Simple dataset to dataloader library for pytorch
 Home-page: https://github.com/nextml-code/pytorch-datastream
 License: Apache-2.0
 Keywords: pytorch,machine,learning,dataset,pipeline,dataloader
 Author: NextML
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -22,15 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: numpy (>=1.17.0,<2.0.0)
 Requires-Dist: pandas (>=1.0.5,<2.0.0)
 Requires-Dist: pydantic (>=1.5.0,<2.0.0)
-Requires-Dist: torch (>=1.4.0,<2.0.0)
+Requires-Dist: torch (>=1.4.0)
 Project-URL: Documentation, https://pytorch-datastream.readthedocs.io
 Project-URL: Repository, https://github.com/nextml-code/pytorch-datastream
 Description-Content-Type: text/x-rst
 
 ==================
 Pytorch Datastream
 ==================
```

