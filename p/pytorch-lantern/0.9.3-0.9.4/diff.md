# Comparing `tmp/pytorch-lantern-0.9.3.tar.gz` & `tmp/pytorch-lantern-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-lantern-0.9.3.tar", last modified: Wed Dec 23 17:37:51 2020, max compression
+gzip compressed data, was "pytorch-lantern-0.9.4.tar", last modified: Thu Jan 28 12:24:22 2021, max compression
```

## Comparing `pytorch-lantern-0.9.3.tar` & `pytorch-lantern-0.9.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    90835 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/LICENSE
--rw-r--r--   0        0        0     2085 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/README.rst
--rw-r--r--   0        0        0     1206 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/__init__.py
--rw-r--r--   0        0        0     1241 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/early_stopping.py
--rw-r--r--   0        0        0      203 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/epochs.py
--rw-r--r--   0        0        0      735 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/evaluate.py
--rw-r--r--   0        0        0      155 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/functional/__init__.py
--rw-r--r--   0        0        0      101 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/functional/star.py
--rw-r--r--   0        0        0     1273 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/functional/starcompose.py
--rw-r--r--   0        0        0      328 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/functional/structure_map.py
--rw-r--r--   0        0        0      936 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/functional_base.py
--rw-r--r--   0        0        0      827 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/metric.py
--rw-r--r--   0        0        0     1934 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/metrics.py
--rw-r--r--   0        0        0     4670 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/module_compose.py
--rw-r--r--   0        0        0       71 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/module_device.py
--rw-r--r--   0        0        0      747 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/module_train.py
--rw-r--r--   0        0        0      106 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/numpy/__init__.py
--rw-r--r--   0        0        0      318 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/numpy/figure_to_numpy.py
--rw-r--r--   0        0        0      980 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/numpy/numpy_seed.py
--rw-r--r--   0        0        0      375 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/progress_bar.py
--rw-r--r--   0        0        0     3361 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/requires_grad.py
--rw-r--r--   0        0        0      188 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/set_learning_rate.py
--rw-r--r--   0        0        0      261 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/set_seeds.py
--rw-r--r--   0        0        0      676 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/step.py
--rw-r--r--   0        0        0     2136 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/tensor.py
--rw-r--r--   0        0        0      833 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/to_device.py
--rw-r--r--   0        0        0      538 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/to_shapes.py
--rw-r--r--   0        0        0      802 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/train.py
--rw-r--r--   0        0        0      429 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/update_cpu_model.py
--rw-r--r--   0        0        0      188 2020-12-23 17:35:57.509296 pytorch-lantern-0.9.3/lantern/worker_init.py
--rw-r--r--   0        0        0     1737 2020-12-23 17:37:50.798707 pytorch-lantern-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     3013 2020-12-23 17:37:51.468813 pytorch-lantern-0.9.3/setup.py
--rw-r--r--   0        0        0     3591 2020-12-23 17:37:51.469230 pytorch-lantern-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    90835 2021-01-28 12:22:38.483768 pytorch-lantern-0.9.4/LICENSE
+-rw-r--r--   0        0        0     2085 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/README.rst
+-rw-r--r--   0        0        0     1206 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/__init__.py
+-rw-r--r--   0        0        0     1241 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/early_stopping.py
+-rw-r--r--   0        0        0      206 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/epochs.py
+-rw-r--r--   0        0        0      735 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/evaluate.py
+-rw-r--r--   0        0        0      155 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/functional/__init__.py
+-rw-r--r--   0        0        0      101 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/functional/star.py
+-rw-r--r--   0        0        0     1273 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/functional/starcompose.py
+-rw-r--r--   0        0        0      328 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/functional/structure_map.py
+-rw-r--r--   0        0        0      972 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/functional_base.py
+-rw-r--r--   0        0        0      827 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/metric.py
+-rw-r--r--   0        0        0     1934 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/metrics.py
+-rw-r--r--   0        0        0     4670 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/module_compose.py
+-rw-r--r--   0        0        0       71 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/module_device.py
+-rw-r--r--   0        0        0      747 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/module_train.py
+-rw-r--r--   0        0        0      106 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/numpy/__init__.py
+-rw-r--r--   0        0        0      318 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/numpy/figure_to_numpy.py
+-rw-r--r--   0        0        0      980 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/numpy/numpy_seed.py
+-rw-r--r--   0        0        0      375 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/progress_bar.py
+-rw-r--r--   0        0        0     3361 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/requires_grad.py
+-rw-r--r--   0        0        0      188 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/set_learning_rate.py
+-rw-r--r--   0        0        0      261 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/set_seeds.py
+-rw-r--r--   0        0        0      676 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/step.py
+-rw-r--r--   0        0        0     2136 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/tensor.py
+-rw-r--r--   0        0        0      833 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/to_device.py
+-rw-r--r--   0        0        0      538 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/to_shapes.py
+-rw-r--r--   0        0        0      802 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/train.py
+-rw-r--r--   0        0        0      429 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/update_cpu_model.py
+-rw-r--r--   0        0        0      188 2021-01-28 12:22:38.487769 pytorch-lantern-0.9.4/lantern/worker_init.py
+-rw-r--r--   0        0        0     1737 2021-01-28 12:24:21.598907 pytorch-lantern-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3013 2021-01-28 12:24:22.209721 pytorch-lantern-0.9.4/setup.py
+-rw-r--r--   0        0        0     3591 2021-01-28 12:24:22.210128 pytorch-lantern-0.9.4/PKG-INFO
```

### Comparing `pytorch-lantern-0.9.3/LICENSE` & `pytorch-lantern-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/README.rst` & `pytorch-lantern-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/__init__.py` & `pytorch-lantern-0.9.4/lantern/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/early_stopping.py` & `pytorch-lantern-0.9.4/lantern/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/evaluate.py` & `pytorch-lantern-0.9.4/lantern/evaluate.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/functional/starcompose.py` & `pytorch-lantern-0.9.4/lantern/functional/starcompose.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/functional_base.py` & `pytorch-lantern-0.9.4/lantern/functional_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from pydantic import BaseModel
+from pydantic import BaseModel, Extra
 
 
 class FunctionalBase(BaseModel):
     class Config:
         allow_mutation = False
+        extra = Extra.forbid
 
     def map(self, fn, *args, **kwargs):
         return fn(self, *args, **kwargs)
 
     def replace(self, **kwargs):
         new_dict = self.dict()
         new_dict.update(**kwargs)
```

### Comparing `pytorch-lantern-0.9.3/lantern/metric.py` & `pytorch-lantern-0.9.4/lantern/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/metrics.py` & `pytorch-lantern-0.9.4/lantern/metrics.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/module_compose.py` & `pytorch-lantern-0.9.4/lantern/module_compose.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/module_train.py` & `pytorch-lantern-0.9.4/lantern/module_train.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/numpy/numpy_seed.py` & `pytorch-lantern-0.9.4/lantern/numpy/numpy_seed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/requires_grad.py` & `pytorch-lantern-0.9.4/lantern/requires_grad.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/step.py` & `pytorch-lantern-0.9.4/lantern/step.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/tensor.py` & `pytorch-lantern-0.9.4/lantern/tensor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/to_device.py` & `pytorch-lantern-0.9.4/lantern/to_device.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/to_shapes.py` & `pytorch-lantern-0.9.4/lantern/to_shapes.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/lantern/train.py` & `pytorch-lantern-0.9.4/lantern/train.py`

 * *Files identical despite different names*

### Comparing `pytorch-lantern-0.9.3/pyproject.toml` & `pytorch-lantern-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytorch-lantern"
-version = "v0.9.3"
+version = "v0.9.4"
 description = "Pytorch project template and related tools"
 authors = ["Aiwizo"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/Aiwizo/pytorch-lantern"
 documentation = "https://pytorch-lantern.readthedocs.io"
 keywords = [
```

### Comparing `pytorch-lantern-0.9.3/setup.py` & `pytorch-lantern-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pytorch-datastream>=0.4.0,<0.5.0',
  'tensorboard>=2.2.0,<3.0.0',
  'torch>=1.6.0,<2.0.0',
  'tqdm>=4.51.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'pytorch-lantern',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Pytorch project template and related tools',
     'long_description': '================\nPytorch Lantern\n================\n\n.. image:: https://badge.fury.io/py/pytorch-lantern.svg\n       :target: https://badge.fury.io/py/pytorch-lantern\n\n.. image:: https://img.shields.io/pypi/pyversions/pytorch-lantern.svg\n       :target: https://pypi.python.org/pypi/pytorch-lantern\n\n.. image:: https://readthedocs.org/projects/pytorch-lantern/badge/?version=latest\n       :target: https://pytorch-lantern.readthedocs.io/en/latest/?badge=latest\n\n.. image:: https://img.shields.io/pypi/l/pytorch-lantern.svg\n       :target: https://pypi.python.org/pypi/pytorch-lantern\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n\nLantern contains our process of bringing a project to fruition as\nefficiently as possible. This is subject to change as we iterate and improve.\nThis package implements tools and missing features to help bridge the gap\nbetween frameworks and libraries that we utilize.\n\nThe main packages and tools that we build around are:\n\n- `pytorch <https://pytorch.org>`_\n- `pytorch-datastream <https://github.com/Aiwizo/pytorch-datastream>`_\n- `guild <https://guild.ai>`_\n\n\nSee the `documentation <https://pytorch-lantern.readthedocs.io/en/latest/>`_\nfor more information.\n\nCreate new project with template\n================================\n\nInstall `cookiecutter <https://github.com/cookiecutter/cookiecutter>`_\nand `poetry <https://github.com/python-poetry/poetry>`_:\n\n.. code-block::\n\n    pip install cookiecutter\n    curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python\n\nSetup project:\n\n.. code-block::\n\n    cookiecutter https://github.com/aiwizo/pytorch-lantern-template.git\n    cd <new-project>\n    poetry install\n\nYou can now train the placeholder model and inspect the results:\n\n.. code-block::\n\n    guild run prepare\n    guild run train\n    guild tensorboard\n\nUse lantern without templates\n==============================\n\nInstall lantern from pypi using pip or poetry:\n\n.. code-block::\n\n    poetry add pytorch-lantern\n    # pip install pytorch-lantern\n',
     'author': 'Aiwizo',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Aiwizo/pytorch-lantern',
```

### Comparing `pytorch-lantern-0.9.3/PKG-INFO` & `pytorch-lantern-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-lantern
-Version: 0.9.3
+Version: 0.9.4
 Summary: Pytorch project template and related tools
 Home-page: https://github.com/Aiwizo/pytorch-lantern
 License: Apache-2.0
 Keywords: pytorch,machine,learning
 Author: Aiwizo
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

