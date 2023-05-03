# Comparing `tmp/pymodaq_plugin_manager-1.0.0.tar.gz` & `tmp/pymodaq_plugin_manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugin_manager-1.0.0.tar", last modified: Tue Apr 25 16:22:57 2023, max compression
+gzip compressed data, was "pymodaq_plugin_manager-1.0.1.tar", last modified: Wed May  3 12:12:54 2023, max compression
```

## Comparing `pymodaq_plugin_manager-1.0.0.tar` & `pymodaq_plugin_manager-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    47137 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    74359 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.711697 pymodaq_plugin_manager-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/PluginList.json
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/plugin_list.schema
--rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-04-25 16:22:45.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:57.715698 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 16:22:57.000000 pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:12:54.247058 pymodaq_plugin_manager-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-03 12:12:54.243058 pymodaq_plugin_manager-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    47137 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    74359 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:12:54.247058 pymodaq_plugin_manager-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:12:54.235057 pymodaq_plugin_manager-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:12:54.243058 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:12:54.243058 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/data/PluginList.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/data/plugin_list.schema
+-rw-r--r--   0 runner    (1001) docker     (123)    16589 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-05-03 12:12:37.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:12:54.243058 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-03 12:12:54.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-03 12:12:54.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:12:54.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 12:12:54.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 12:12:54.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 12:12:54.000000 pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager.egg-info/top_level.txt
```

### Comparing `pymodaq_plugin_manager-1.0.0/LICENSE` & `pymodaq_plugin_manager-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugin_manager-1.0.0/PKG-INFO` & `pymodaq_plugin_manager-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugin_manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: Manager and interface to list, install or remove PyMoDAQ's plugins
 Home-page: 
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugin_manager-1.0.0/README.md` & `pymodaq_plugin_manager-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pymodaq_plugin_manager-1.0.0/icon.ico` & `pymodaq_plugin_manager-1.0.1/icon.ico`

 * *Files identical despite different names*

### Comparing `pymodaq_plugin_manager-1.0.0/setup.py` & `pymodaq_plugin_manager-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/PluginList.json` & `pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/data/PluginList.json`

 * *Files identical despite different names*

### Comparing `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/data/plugin_list.schema` & `pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/data/plugin_list.schema`

 * *Files identical despite different names*

### Comparing `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/manager.py` & `pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 
 import numpy as np
 from qtpy import QtWidgets, QtCore
 from qtpy.QtCore import Qt, Slot, Signal
 from qtpy.QtGui import QTextCursor
 from readme_renderer.rst import render
 
-from pymodaq_plugin_manager.validate import validate_json_plugin_list, get_plugins, get_plugin, get_check_repo,\
-    find_dict_in_list_from_key_val
+from pymodaq_plugin_manager.validate import get_plugins
 from pymodaq_plugin_manager.validate import get_pypi_pymodaq
 from pymodaq_plugin_manager import __version__ as version
 from pymodaq_plugin_manager.utils import QVariant, TableModel, TableView, SpinBoxDelegate, get_pymodaq_version
 
 logger = logging.getLogger(__name__)
-# logger.addHandler(logging.NullHandler())
+logger.addHandler(logging.StreamHandler())
 
 
 class TableModel(TableModel):
-
+    """Specific Model to display plugins info in a TableView"""
     def __init__(self, *args, plugins=[], **kwargs):
         super().__init__(*args, **kwargs)
         self._selected = [False for ind in range(len(self._data))]
         self.plugins = plugins
 
     @property
     def selected(self):
@@ -68,15 +67,15 @@
                     self._selected[index.row()] = value == Qt.Checked
                     self.dataChanged.emit(index, index, [role])
                     return True
         return False
 
 
 class FilterProxy(QtCore.QSortFilterProxyModel):
-
+    """Utility to filter the View"""
     def __init__(self, parent=None):
         super().__init__(parent)
 
         self.textRegExp = QtCore.QRegExp()
         self.textRegExp.setCaseSensitivity(QtCore.Qt.CaseInsensitive)
         self.textRegExp.setPatternSyntax(QtCore.QRegExp.Wildcard)
 
@@ -98,15 +97,18 @@
 
     def setTextFilter(self, regexp):
         self.textRegExp.setPattern(regexp)
         self.invalidateFilter()
 
 
 class PluginManager(QtCore.QObject):
+    """Main UI to display a list of plugins and install/uninstall them
 
+    Attempts to display plugins only compatible with the currently installed version of pymodaq
+    """
     quit_signal = Signal()
     restart_signal = Signal()
 
     def __init__(self, parent, standalone=False):
         super().__init__()
         self.parent = parent
         self.parent.setLayout(QtWidgets.QVBoxLayout())
@@ -325,22 +327,19 @@
         elif plugin_choice == 'Installed':
             model_proxy.setSourceModel(self.model_installed)
             self.action_button.setText('Remove')
         self.search_edit.textChanged.connect(model_proxy.setTextFilter)
         self.table_view.setModel(model_proxy)
         self.item_clicked(model_proxy.index(0, 0))
 
-
     def item_clicked(self, index):
         if index.isValid():
             self.display_info(index)
             self.action_button.setEnabled(bool(np.any(index.model().sourceModel().selected)))
 
-
-
     def display_info(self, index):
         self.info_widget.clear()
         if index.isValid():
             if self.plugin_choice.currentText() == 'Available':
                 plugin = self.plugins_available[index.model().mapToSource(index).row()]
             elif self.plugin_choice.currentText() == 'Update':
                 plugin = self.plugins_update[index.model().mapToSource(index).row()]
```

### Comparing `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/utils.py` & `pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager/validate.py` & `pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager/validate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import logging
 from typing import List, Union
 
 from hashlib import sha256
 from packaging import version
 from packaging.version import Version
-from packaging.requirements import Requirement, SpecifierSet, Specifier
+from packaging.requirements import Requirement
+from packaging.specifiers import SpecifierSet
 import pkg_resources
 from jsonschema import validate
 import json
 from distlib.index import PackageIndex
 from pathlib import Path
 #using pip directly https://pip.pypa.io/en/latest/reference/pip_install/#git
 from pytablewriter import MarkdownTableWriter
 from yawrap import Doc
 import requests
 from lxml import html
 from copy import deepcopy
 import re
 
 logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
+logger.addHandler(logging.StreamHandler())
+logger.setLevel('INFO')
 
 pypi_index = PackageIndex()
 
 
 def find_dict_in_list_from_key_val(dicts, key, value):
     """ lookup within a list of dicts. Look for the dict within the list which has the correct key, value pair
 
@@ -41,32 +43,40 @@
     for dict in dicts:
         if key in dict:
             if dict[key] == value:
                 return dict
     return None
 
 
-def get_pypi_package_list(match_name=None):
+def get_pypi_package_list(match_name: str = None) -> List[str]:
+    """Connect to the "simple" pypi url to get the list of all packages matching all or part of
+    the given name
+
+    Parameters
+    ----------
+    match_name: str
+        The package name to be (partially) matched
+
+    Examples
+    --------
+    get_pypi_package_list('pymodaq_plugins') will retrieve the names of all packages having 'pymodaq_plugins'
+    in their name
+    """
     status = 'Connecting to the pypi repository, may take some time to retrieve the list'
-    if logging:
-        logger.info(status)
-    else:
-        print(status)
+    logger.info(status)
     simple_package = requests.get('https://pypi.org/simple/')
     if simple_package.status_code == 503:
         info = 'The service from pypi is currently unavailable, please retry later or install your plugins manually'
-        if logging:
-            logger.info(info)
-        else:
-            print(info)
+        logger.info(info)
     tree = html.fromstring(simple_package.text)
     packages = []
     for child in tree.body:
         if match_name is None or match_name in child.text:
             packages.append(child.text)
+            logger.info(f'Got package {child.text}')
     return packages
 
 
 def get_pymodaq_specifier(requirements: List[str]) -> SpecifierSet:
     """Get specifiers for pymodaq version from a list of requirements"""
     specifier = SpecifierSet('>3.0,<4.0')
     if requirements is not None:
@@ -74,25 +84,40 @@
             req = Requirement(package)
             if req.name == 'pymodaq':
                 specifier = req.specifier
                 break
     return specifier
 
 
-def get_package_metadata(name: str, version: Union[str, Version] = None):
+def get_package_metadata(name: str, version: Union[str, Version] = None) -> dict:
+    """Retrieve the metadata of a given package on pypi matching or not a specific version
+
+    Parameters
+    ----------
+    name: str
+        package name
+    version: Union[str, Version]
+        package version specifier
+
+
+    Returns
+    -------
+    dict of metadata
+    """
     if version is None:
         url = f'https://pypi.python.org/pypi/{name}/json'
     else:
         url = f'https://pypi.python.org/pypi/{name}/{str(version)}/json'
     rep = requests.get(url)
     if rep.status_code != 404:
         return rep.json()
 
 
 def get_metadata_from_json(json_as_dict: dict) -> dict:
+    """Transform dict of metadata from pypi to a simpler dict"""
     try:
         if json_as_dict is not None:
             metadata = dict([])
             metadata['author'] = json_as_dict['info']['author']
             metadata['description'] = json_as_dict['info']['description']
             metadata['project_url'] = json_as_dict['info']['project_url']
             metadata['version'] = json_as_dict['info']['version']
@@ -130,21 +155,32 @@
                         return
                     if pymodaq_version in specifier:
                         return get_metadata_from_json(versioned)
         else:
             return get_metadata_from_json(latest)
 
 
-def get_pypi_plugins(browse_pypi=False, pymodaq_version: Version = None):
+def get_pypi_plugins(browse_pypi=True, pymodaq_version: Union[Version, str] = None) -> List[dict]:
+    """Fetch the list of plugins (for a given version) of pymodaq
+
+    Parameters
+    ----------
+    browse_pypi: bool
+        If True get the list from pypi server, if False from the builtin json (deprecated, should be True)
+    pymodaq_version: Union[str, Version]
+        a given pymodaq version (or the latest if None)
+
+    Returns
+    -------
+    list of dictionaries giving info on plugins
+    """
     plugins = []
-    if browse_pypi:
-        packages = get_pypi_package_list('pymodaq-plugins')
-    else:
-        packages = [plug['plugin-name'] for plug in get_plugins_from_json()]
+    packages = get_pypi_package_list('pymodaq-plugins')
     for package in packages:
+        logger.info(f'Fetching metadata for package {package}')
         metadata = get_pypi_pymodaq(package, pymodaq_version)
         if metadata is not None:
             title = metadata['description'].split('\n')[0]
             if '(' in title and ')' in title:
                 display_name = re.search(r'\((.*?)\)', title).group(1)
             else:
                 display_name = title
@@ -154,57 +190,44 @@
                       'instruments': '', 'authors': [metadata['author']], 'contributors': [],
                       'homepage': metadata['project_url']}
             plugins.append(plugin)
     return plugins
 
 
 def get_plugin_sourcefile_id(filename):
+    """Get the SHA identifier of a vien file"""
     h = sha256()
     b = bytearray(128*1024)
     mv = memoryview(b)
     with open(filename, 'rb', buffering=0) as f:
         for n in iter(lambda: f.readinto(mv), 0):
             h.update(mv[:n])
     return h.hexdigest()
 
 
-def get_plugins_from_json():
-    return validate_json_plugin_list()['pymodaq-plugins']
-
-
-def get_plugin(name, entry='display-name'):
-    plugins = get_plugins_from_json()
-    d = find_dict_in_list_from_key_val(plugins, entry, name)
-    return d
-
-
 def get_check_repo(plugin_dict):
+    """Unused"""
     try:
         response = requests.get(plugin_dict["repository"])
     except requests.exceptions.RequestException as e:
-        if logging:
-            logger.exception(str(e))
-            return str(e)
+        logger.exception(str(e))
+        return str(e)
 
     if response.status_code != 200:
         rep = f'{plugin_dict["display-name"]}: failed to download plugin. Returned code {response.status_code}'
-        if logging:
-            logger.error(rep)
-        return rep
+        logger.error(rep)
 
     # Hash it and make sure its what is expected
     hash = sha256(response.content).hexdigest()
     if plugin_dict["id"].lower() != hash.lower():
         rep = f'{plugin_dict["display-name"]}: Invalid hash. Got {hash.lower()} but expected {plugin_dict["id"]}'
-        if logging:
-            logger.error(rep)
+        logger.error(rep)
         return rep
     else:
-        if logging:
-            logger.info(f'SHA256 is Ok')
+        logger.info(f'SHA256 is Ok')
 
 
 def get_plugins(from_json=False, browse_pypi=True, pymodaq_version: Version = None):
     """get PyMoDAQ plugins
 
     Parameters
     ----------
@@ -218,18 +241,15 @@
     Returns
     -------
     plugins_available: list of available plugins for installation
     plugins_installed: list of already installed plugins
     plugins_update: list of plugins with existing update
     """
     logger.info('Fetching plugin list')
-    if from_json:
-        plugins_available = get_plugins_from_json()
-    else:
-        plugins_available = get_pypi_plugins(browse_pypi=browse_pypi, pymodaq_version=pymodaq_version)
+    plugins_available = get_pypi_plugins(browse_pypi=browse_pypi, pymodaq_version=pymodaq_version)
 
     plugins = deepcopy(plugins_available)
     plugins_installed_init = [{'plugin-name': entry.module_name,
                           'version': entry.dist.version} for entry in pkg_resources.iter_entry_points('pymodaq.plugins')]
     plugins_installed = []
     for plug in plugins_installed_init:
         d = find_dict_in_list_from_key_val(plugins_available, 'plugin-name', plug['plugin-name'])
@@ -243,70 +263,16 @@
         d = find_dict_in_list_from_key_val(plugins, 'plugin-name', plug['plugin-name'])
         if version.parse(d['version']) > version.parse(plug['version']):
             plugins_update.append(d)
 
     return plugins_available, plugins_installed, plugins_update
 
 
-def validate_json_plugin_list():
-    base_path = Path(__file__).parent.joinpath('data')
-    with open(str(base_path.joinpath('plugin_list.schema'))) as f:
-        schema = json.load(f)
-    with open(str(base_path.joinpath('PluginList.json'))) as f:
-        plugins = json.load(f)
-    validate(instance=plugins, schema=schema)
-    return plugins
-
-
 def post_error(message):
-    if logging:
-        logger.error(message)
-
-
-def check_plugin_entries():
-    displaynames = []
-    repositories = []
-    for plugin in get_plugins_from_json():
-        if logging:
-            logger.info(f'Checking info on plugin: {plugin["display-name"]}')
-
-        try:
-            response = requests.get(plugin["repository"])
-        except requests.exceptions.RequestException as e:
-            post_error(str(e))
-            continue
-
-        if response.status_code != 200:
-            post_error(f'{plugin["display-name"]}: failed to download plugin. Returned code {response.status_code}')
-            continue
-
-        # Hash it and make sure its what is expected
-        hash = sha256(response.content).hexdigest()
-        if plugin["id"].lower() != hash.lower():
-            post_error(f'{plugin["display-name"]}: Invalid hash. Got {hash.lower()} but expected {plugin["id"]}')
-        else:
-            if logging:
-                logger.info(f'SHA256 is Ok')
-
-        # check uniqueness of json display-name and repository
-        found = False
-        for name in displaynames:
-            if plugin["display-name"] == name:
-                post_error(f'{plugin["display-name"]}: non unique display-name entry')
-                found = True
-        if not found:
-            displaynames.append(plugin["display-name"])
-
-        found = False
-        for repo in repositories:
-            if plugin["repository"] == repo:
-                post_error(f'{plugin["repository"]}: non unique repository entry')
-                found = True
-        if not found:
-            repositories.append(plugin["repository"])
+    logger.error(message)
 
 
 def extract_authors_from_description(description):
     """returns the authors as a list from the plugin package description (it should follow the template structure)
 
     Parameters
     ----------
@@ -321,14 +287,15 @@
     posc = description.find('\n\nContributors')
     posi = description.find('\n\nInstruments')
     authors_raw = description[posa:posc if posc != -1 else posi]
     return authors_raw.split('\n* ')[1:]
 
 
 def write_plugin_doc():
+    """Update the README from info of all available plugins"""
     plugins = get_pypi_plugins(browse_pypi=True)
     base_path = Path(__file__).parent
 
     header_keys = ['display-name', 'authors', 'version', 'description']
     header = ['Repo Name', 'Authors', 'Version plugin', 'Instruments']
     plugins_tmp = []
 
@@ -399,14 +366,14 @@
         content = f.read()
         content += '\r\n'
 
     with open(base_path.parent.parent.joinpath('README.md'), 'w') as f:
         content += writer.dumps()
         f.write(content)
 
+
 if __name__ == '__main__':
-    #check_plugin_entries()
     write_plugin_doc()
     # versions = get_pypi_pymodaq()
     # from pymodaq_plugin_manager import __version__ as version
     # print(version)
     #print(get_pypi_package_list('pymodaq-plugins'))
```

### Comparing `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/PKG-INFO` & `pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugin-manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: Manager and interface to list, install or remove PyMoDAQ's plugins
 Home-page: 
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugin_manager-1.0.0/src/pymodaq_plugin_manager.egg-info/SOURCES.txt` & `pymodaq_plugin_manager-1.0.1/src/pymodaq_plugin_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

