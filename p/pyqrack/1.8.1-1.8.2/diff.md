# Comparing `tmp/pyqrack-1.8.1.tar.gz` & `tmp/pyqrack-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqrack-1.8.1.tar", last modified: Mon May  1 22:57:38 2023, max compression
+gzip compressed data, was "pyqrack-1.8.2.tar", last modified: Tue May  2 16:37:04 2023, max compression
```

## Comparing `pyqrack-1.8.1.tar` & `pyqrack-1.8.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:57:38.086257 pyqrack-1.8.1/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2021-12-27 16:00:58.000000 pyqrack-1.8.1/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-01 22:57:38.086257 pyqrack-1.8.1/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2767 2023-05-01 22:57:30.000000 pyqrack-1.8.1/README.md
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      104 2021-12-27 16:00:58.000000 pyqrack-1.8.1/pyproject.toml
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:57:38.086257 pyqrack-1.8.1/pyqrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      492 2023-05-01 22:27:13.000000 pyqrack-1.8.1/pyqrack/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      594 2023-05-01 22:49:53.000000 pyqrack-1.8.1/pyqrack/neuron_activation_fn.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      654 2022-06-18 20:18:56.000000 pyqrack-1.8.1/pyqrack/pauli.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     8677 2023-05-01 22:27:13.000000 pyqrack-1.8.1/pyqrack/qrack_neuron.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    83208 2023-04-30 17:06:05.000000 pyqrack-1.8.1/pyqrack/qrack_simulator.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:57:38.086257 pyqrack-1.8.1/pyqrack/qrack_system/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      334 2021-12-27 16:00:58.000000 pyqrack-1.8.1/pyqrack/qrack_system/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    27647 2023-05-01 22:57:30.000000 pyqrack-1.8.1/pyqrack/qrack_system/qrack_system.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:57:38.086257 pyqrack-1.8.1/pyqrack/util/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      333 2022-06-18 20:18:56.000000 pyqrack-1.8.1/pyqrack/util/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2065 2022-06-18 20:18:56.000000 pyqrack-1.8.1/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:57:38.086257 pyqrack-1.8.1/pyqrack.egg-info/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-01 22:57:38.000000 pyqrack-1.8.1/pyqrack.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      468 2023-05-01 22:57:38.000000 pyqrack-1.8.1/pyqrack.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-01 22:57:38.000000 pyqrack-1.8.1/pyqrack.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-01 22:57:37.000000 pyqrack-1.8.1/pyqrack.egg-info/not-zip-safe
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        8 2023-05-01 22:57:38.000000 pyqrack-1.8.1/pyqrack.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-05-01 22:57:38.086257 pyqrack-1.8.1/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1559 2023-05-01 22:56:52.000000 pyqrack-1.8.1/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-02 16:37:04.885659 pyqrack-1.8.2/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2021-12-27 16:00:58.000000 pyqrack-1.8.2/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-02 16:37:04.885659 pyqrack-1.8.2/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2767 2023-05-02 16:36:51.000000 pyqrack-1.8.2/README.md
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      104 2021-12-27 16:00:58.000000 pyqrack-1.8.2/pyproject.toml
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-02 16:37:04.885659 pyqrack-1.8.2/pyqrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      492 2023-05-01 22:27:13.000000 pyqrack-1.8.2/pyqrack/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      594 2023-05-01 22:49:53.000000 pyqrack-1.8.2/pyqrack/neuron_activation_fn.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      654 2022-06-18 20:18:56.000000 pyqrack-1.8.2/pyqrack/pauli.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     8677 2023-05-01 22:27:13.000000 pyqrack-1.8.2/pyqrack/qrack_neuron.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    83208 2023-04-30 17:06:05.000000 pyqrack-1.8.2/pyqrack/qrack_simulator.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-02 16:37:04.885659 pyqrack-1.8.2/pyqrack/qrack_system/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      334 2021-12-27 16:00:58.000000 pyqrack-1.8.2/pyqrack/qrack_system/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    27647 2023-05-02 16:36:51.000000 pyqrack-1.8.2/pyqrack/qrack_system/qrack_system.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-02 16:37:04.885659 pyqrack-1.8.2/pyqrack/util/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      333 2022-06-18 20:18:56.000000 pyqrack-1.8.2/pyqrack/util/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2065 2022-06-18 20:18:56.000000 pyqrack-1.8.2/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-02 16:37:04.885659 pyqrack-1.8.2/pyqrack.egg-info/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-02 16:37:04.000000 pyqrack-1.8.2/pyqrack.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      468 2023-05-02 16:37:04.000000 pyqrack-1.8.2/pyqrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-02 16:37:04.000000 pyqrack-1.8.2/pyqrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-02 16:37:04.000000 pyqrack-1.8.2/pyqrack.egg-info/not-zip-safe
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        8 2023-05-02 16:37:04.000000 pyqrack-1.8.2/pyqrack.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-05-02 16:37:04.885659 pyqrack-1.8.2/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1559 2023-05-02 16:36:37.000000 pyqrack-1.8.2/setup.py
```

### Comparing `pyqrack-1.8.1/LICENSE` & `pyqrack-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrack-1.8.1/PKG-INFO` & `pyqrack-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrack
-Version: 1.8.1
+Version: 1.8.2
 Summary: pyqrack - Pure Python vm6502q/qrack Wrapper
 Home-page: https://github.com/vm6502q/pyqrack
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: MIT
 Keywords: pyqrack qrack simulator quantum gpu
 Classifier: Environment :: Console
```

### Comparing `pyqrack-1.8.1/README.md` & `pyqrack-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pyqrack-1.8.1/pyqrack/neuron_activation_fn.py` & `pyqrack-1.8.2/pyqrack/neuron_activation_fn.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.8.1/pyqrack/pauli.py` & `pyqrack-1.8.2/pyqrack/pauli.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.8.1/pyqrack/qrack_neuron.py` & `pyqrack-1.8.2/pyqrack/qrack_neuron.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.8.1/pyqrack/qrack_simulator.py` & `pyqrack-1.8.2/pyqrack/qrack_simulator.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.8.1/pyqrack/qrack_system/qrack_system.py` & `pyqrack-1.8.2/pyqrack/qrack_system/qrack_system.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.8.1/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py` & `pyqrack-1.8.2/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.8.1/pyqrack.egg-info/PKG-INFO` & `pyqrack-1.8.2/pyqrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrack
-Version: 1.8.1
+Version: 1.8.2
 Summary: pyqrack - Pure Python vm6502q/qrack Wrapper
 Home-page: https://github.com/vm6502q/pyqrack
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: MIT
 Keywords: pyqrack qrack simulator quantum gpu
 Classifier: Environment :: Console
```

### Comparing `pyqrack-1.8.1/setup.py` & `pyqrack-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from setuptools import setup
 
 
 requirements = []
 
-VERSION = "1.8.1"
+VERSION = "1.8.2"
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md')
 with open(README_PATH) as readme_file:
     README = readme_file.read()
 
 setup(
```

