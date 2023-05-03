# Comparing `tmp/bluetooth_auto_recovery-1.0.3.tar.gz` & `tmp/bluetooth_auto_recovery-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_auto_recovery-1.0.3.tar", max compression
+gzip compressed data, was "bluetooth_auto_recovery-1.1.0.tar", max compression
```

## Comparing `bluetooth_auto_recovery-1.0.3.tar` & `bluetooth_auto_recovery-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1072 2022-12-15 23:20:37.717899 bluetooth_auto_recovery-1.0.3/LICENSE
--rw-r--r--   0        0        0     3840 2022-12-15 23:20:37.717899 bluetooth_auto_recovery-1.0.3/README.md
--rw-r--r--   0        0        0     2490 2022-12-15 23:20:38.485895 bluetooth_auto_recovery-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       91 2022-12-15 23:20:38.441896 bluetooth_auto_recovery-1.0.3/src/bluetooth_auto_recovery/__init__.py
--rw-r--r--   0        0        0        0 2022-12-15 23:20:37.717899 bluetooth_auto_recovery-1.0.3/src/bluetooth_auto_recovery/py.typed
--rw-r--r--   0        0        0    18824 2022-12-15 23:20:37.717899 bluetooth_auto_recovery-1.0.3/src/bluetooth_auto_recovery/recover.py
--rw-r--r--   0        0        0     4918 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.0.3/setup.py
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-03 15:00:11.880923 bluetooth_auto_recovery-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3840 2023-05-03 15:00:11.880923 bluetooth_auto_recovery-1.1.0/README.md
+-rw-r--r--   0        0        0     2490 2023-05-03 15:00:12.700922 bluetooth_auto_recovery-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-05-03 15:00:12.664922 bluetooth_auto_recovery-1.1.0/src/bluetooth_auto_recovery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:00:11.880923 bluetooth_auto_recovery-1.1.0/src/bluetooth_auto_recovery/py.typed
+-rw-r--r--   0        0        0    20595 2023-05-03 15:00:11.880923 bluetooth_auto_recovery-1.1.0/src/bluetooth_auto_recovery/recover.py
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.1.0/PKG-INFO
```

### Comparing `bluetooth_auto_recovery-1.0.3/LICENSE` & `bluetooth_auto_recovery-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.0.3/README.md` & `bluetooth_auto_recovery-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.0.3/pyproject.toml` & `bluetooth_auto_recovery-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-auto-recovery"
-version = "1.0.3"
+version = "1.1.0"
 description = "Recover bluetooth adapters that are in an stuck state"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bluetooth-auto-recovery"
 documentation = "https://bluetooth-auto-recovery.readthedocs.io"
 classifiers = [
```

### Comparing `bluetooth_auto_recovery-1.0.3/src/bluetooth_auto_recovery/recover.py` & `bluetooth_auto_recovery-1.1.0/src/bluetooth_auto_recovery/recover.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 """Automatic recovery for bluetooth adapters."""
 from __future__ import annotations
 
+import array
 import asyncio
 import logging
 import socket
+import struct
 from contextlib import asynccontextmanager
 from dataclasses import dataclass
+from fcntl import ioctl
 from typing import Any, AsyncIterator, cast
 
 import async_timeout
 import pyric.net.wireless.rfkill_h as rfkh
 import pyric.utils.rfkill as rfkill
 from btsocket import btmgmt_protocol, btmgmt_socket
+from btsocket.btmgmt_socket import AF_BLUETOOTH, BTPROTO_HCI
 from usb_devices import BluetoothDevice, NotAUSBDeviceError
 
 _LOGGER = logging.getLogger(__name__)
 
 POWER_OFF_TIME = 2
 POWER_ON_TIME = 3
 MAX_RFKILL_TIME = 3
 DBUS_REGISTER_TIME = 1.5
 
 MGMT_PROTOCOL_TIMEOUT = 5
 
+# https://git.kernel.org/pub/scm/bluetooth/bluez.git/tree/lib/hci.h
+HCIDEVUP = 0x400448C9  # 201
+HCIDEVDOWN = 0x400448CA  # 202
+
 
 @dataclass
 class RFKillInfo:
     """RFKill info."""
 
     soft_block: bool | None
     hard_block: bool | None
@@ -467,14 +475,35 @@
     except Exception as ex:  # pylint: disable=broad-except
         _LOGGER.exception(
             "Unexpected error while attempting USB reset of hci%s: %s", hci, ex
         )
         return False
 
 
+async def _bounce_adapter_interface(adapter: MGMTBluetoothCtl) -> None:
+    """Bounce the adapter ex. hciconfig down/up."""
+    loop = asyncio.get_running_loop()
+    socket = await loop.run_in_executor(None, raw_open, adapter.idx)
+    try:
+        _LOGGER.debug("Bouncing Bluetooth adapter hci%i", adapter.idx)
+        req_str = struct.pack("H", adapter.idx)
+        request = array.array("b", req_str)
+        _LOGGER.debug("Setting hci%i down", adapter.idx)
+        await loop.run_in_executor(None, ioctl, socket.fileno(), HCIDEVDOWN, request[0])
+        await asyncio.sleep(0.5)
+        req_str = struct.pack("H", adapter.idx)
+        request = array.array("b", req_str)
+        _LOGGER.debug("Setting hci%i up", adapter.idx)
+        await loop.run_in_executor(None, ioctl, socket.fileno(), HCIDEVUP, request[0])
+        await asyncio.sleep(0.5)
+        _LOGGER.debug("Finished bouncing hci%i", adapter.idx)
+    finally:
+        await loop.run_in_executor(None, raw_close, socket)
+
+
 async def _execute_reset(adapter: MGMTBluetoothCtl) -> bool:
     """Execute the reset."""
     name = f"hci{adapter.idx} [{adapter.mac}]"
     if adapter.idx is None:
         _LOGGER.error(
             "%s seems not to exist (anymore), check BT interface mac address in your settings; "
             "Available adapters: %s ",
@@ -487,15 +516,14 @@
         pstate_before = await adapter.get_powered()
     except AttributeError as ex:
         _LOGGER.warning(
             "Could not determine the power state of the Bluetooth adapter %s: %s",
             name,
             ex,
         )
-        return False
 
     if pstate_before is True:
         _LOGGER.debug("Current power state of bluetooth adapter is ON.")
         try:
             await adapter.set_powered(False)
         except AttributeError as ex:
             _LOGGER.warning(
@@ -509,14 +537,19 @@
             name,
         )
     else:
         _LOGGER.debug("Power state of bluetooth adapter could not be determined")
         return False
 
     try:
+        await _bounce_adapter_interface(adapter)
+    except Exception as ex:  # pylint: disable=broad-except
+        _LOGGER.warning("Could not cycle the Bluetooth adapter %s: %s", name, ex)
+
+    try:
         await adapter.set_powered(True)
     except AttributeError as ex:
         _LOGGER.warning(
             "Could not re-enable power after cycle of the Bluetooth adapter %s: %s",
             name,
             ex,
         )
@@ -541,7 +574,20 @@
         return False
 
     _LOGGER.debug(
         "Power state of bluetooth adapter %s could not be determined after power cycle",
         name,
     )
     return False
+
+
+def raw_open(adapter_idx: int) -> socket.socket:
+    """Create a bluetooth socket for a specific adapter."""
+    sock = socket.socket(AF_BLUETOOTH, socket.SOCK_RAW, BTPROTO_HCI)
+    sock.bind((adapter_idx,))
+    return sock
+
+
+def raw_close(bt_socket: socket.socket) -> None:
+    """Close the bluetooth socket."""
+    fd = bt_socket.detach()
+    socket.close(fd)
```

### Comparing `bluetooth_auto_recovery-1.0.3/setup.py` & `bluetooth_auto_recovery-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,97 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bluetooth-auto-recovery
+Version: 1.1.0
+Summary: Recover bluetooth adapters that are in an stuck state
+Home-page: https://github.com/bluetooth-devices/bluetooth-auto-recovery
+License: MIT
+Author: J. Nick Koston
+Author-email: nick@koston.org
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: docs
+Requires-Dist: PyRIC (>=0.1.6.3)
+Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
+Requires-Dist: async-timeout (>=4.0.1)
+Requires-Dist: btsocket (>=0.2.0)
+Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
+Requires-Dist: usb-devices (>=0.4.1)
+Project-URL: Bug Tracker, https://github.com/bluetooth-devices/bluetooth-auto-recovery/issues
+Project-URL: Changelog, https://github.com/bluetooth-devices/bluetooth-auto-recovery/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://bluetooth-auto-recovery.readthedocs.io
+Project-URL: Repository, https://github.com/bluetooth-devices/bluetooth-auto-recovery
+Description-Content-Type: text/markdown
+
+# Bluetooth Auto Recovery
+
+<p align="center">
+  <a href="https://github.com/bluetooth-devices/bluetooth-auto-recovery/actions?query=workflow%3ACI">
+    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/bluetooth-auto-recovery/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >
+  </a>
+  <a href="https://bluetooth-auto-recovery.readthedocs.io">
+    <img src="https://img.shields.io/readthedocs/bluetooth-auto-recovery.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
+  </a>
+  <a href="https://codecov.io/gh/bluetooth-devices/bluetooth-auto-recovery">
+    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/bluetooth-auto-recovery.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  </a>
+</p>
+<p align="center">
+  <a href="https://python-poetry.org/">
+    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
+  </a>
+  <a href="https://github.com/ambv/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  </a>
+  <a href="https://github.com/pre-commit/pre-commit">
+    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
+  </a>
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/bluetooth-auto-recovery/">
+    <img src="https://img.shields.io/pypi/v/bluetooth-auto-recovery.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/bluetooth-auto-recovery.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/bluetooth-auto-recovery.svg?style=flat-square" alt="License">
+</p>
+
+Recover bluetooth adapters that are in an stuck state
+
+## Credits
+
+The code in this repo originates from https://github.com/custom-components/ble_monitor/blob/master/custom_components/ble_monitor/bt_helpers.py
+
+## Installation
+
+Install this via pip (or your favourite package manager):
+
+`pip install bluetooth-auto-recovery`
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- prettier-ignore-start -->
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- markdownlint-disable -->
+<!-- markdownlint-enable -->
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+<!-- prettier-ignore-end -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Credits
+
+This package was created with
+[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
+[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)
+project template.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['bluetooth_auto_recovery']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyRIC>=0.1.6.3',
- 'async-timeout>=4.0.1',
- 'btsocket>=0.2.0',
- 'usb-devices>=0.4.1']
-
-extras_require = \
-{'docs': ['Sphinx>=5.0,<6.0',
-          'sphinx-rtd-theme>=1.0,<2.0',
-          'myst-parser>=0.18,<0.19']}
-
-setup_kwargs = {
-    'name': 'bluetooth-auto-recovery',
-    'version': '1.0.3',
-    'description': 'Recover bluetooth adapters that are in an stuck state',
-    'long_description': '# Bluetooth Auto Recovery\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/bluetooth-auto-recovery/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/bluetooth-auto-recovery/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://bluetooth-auto-recovery.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/bluetooth-auto-recovery.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/bluetooth-auto-recovery">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/bluetooth-auto-recovery.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/bluetooth-auto-recovery/">\n    <img src="https://img.shields.io/pypi/v/bluetooth-auto-recovery.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/bluetooth-auto-recovery.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/bluetooth-auto-recovery.svg?style=flat-square" alt="License">\n</p>\n\nRecover bluetooth adapters that are in an stuck state\n\n## Credits\n\nThe code in this repo originates from https://github.com/custom-components/ble_monitor/blob/master/custom_components/ble_monitor/bt_helpers.py\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install bluetooth-auto-recovery`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
-    'author': 'J. Nick Koston',
-    'author_email': 'nick@koston.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/bluetooth-devices/bluetooth-auto-recovery',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,31 +1,35 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['bluetooth_auto_recovery'] package_data = \ {'': ['*']}
-install_requires = \ ['PyRIC>=0.1.6.3', 'async-timeout>=4.0.1',
-'btsocket>=0.2.0', 'usb-devices>=0.4.1'] extras_require = \ {'docs':
-['Sphinx>=5.0,<6.0', 'sphinx-rtd-theme>=1.0,<2.0', 'myst-parser>=0.18,<0.19']}
-setup_kwargs = { 'name': 'bluetooth-auto-recovery', 'version': '1.0.3',
-'description': 'Recover bluetooth adapters that are in an stuck state',
-'long_description': '# Bluetooth Auto Recovery\n\n
-     \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
-                                percentage]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-      \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
-\n\nRecover bluetooth adapters that are in an stuck state\n\n## Credits\n\nThe
-code in this repo originates from https://github.com/custom-components/
-ble_monitor/blob/master/custom_components/ble_monitor/bt_helpers.py\n\n##
-Installation\n\nInstall this via pip (or your favourite package manager):
-\n\n`pip install bluetooth-auto-recovery`\n\n## Contributors â¨\n\nThanks goes
-to these wonderful people ([emoji key](https://allcontributors.org/docs/en/
-emoji-key)):\n\n\n\n\n\n\n\n\nThis project follows the [all-contributors]
-(https://github.com/all-contributors/all-contributors) specification.
-Contributions of any kind welcome!\n\n## Credits\n\nThis package was created
-with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n
-[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/
-cookiecutter-pypackage)\nproject template.\n', 'author': 'J. Nick Koston',
-'author_email': 'nick@koston.org', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/bluetooth-devices/bluetooth-auto-recovery',
-'package_dir': package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.1.0 Summary:
+Recover bluetooth adapters that are in an stuck state Home-page: https://
+github.com/bluetooth-devices/bluetooth-auto-recovery License: MIT Author: J.
+Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Software Development :: Libraries Provides-Extra: docs Requires-Dist: PyRIC
+(>=0.1.6.3) Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs" Requires-Dist:
+async-timeout (>=4.0.1) Requires-Dist: btsocket (>=0.2.0) Requires-Dist: myst-
+parser (>=0.18,<0.19) ; extra == "docs" Requires-Dist: sphinx-rtd-theme
+(>=1.0,<2.0) ; extra == "docs" Requires-Dist: usb-devices (>=0.4.1) Project-
+URL: Bug Tracker, https://github.com/bluetooth-devices/bluetooth-auto-recovery/
+issues Project-URL: Changelog, https://github.com/bluetooth-devices/bluetooth-
+auto-recovery/blob/main/CHANGELOG.md Project-URL: Documentation, https://
+bluetooth-auto-recovery.readthedocs.io Project-URL: Repository, https://
+github.com/bluetooth-devices/bluetooth-auto-recovery Description-Content-Type:
+text/markdown # Bluetooth Auto Recovery
+         [CI_Status] [Documentation_Status] [Test_coverage_percentage]
+                         [Poetry] [black] [pre-commit]
+             [PyPI_Version] [Supported Python versions] [License]
+Recover bluetooth adapters that are in an stuck state ## Credits The code in
+this repo originates from https://github.com/custom-components/ble_monitor/
+blob/master/custom_components/ble_monitor/bt_helpers.py ## Installation Install
+this via pip (or your favourite package manager): `pip install bluetooth-auto-
+recovery` ## Contributors â¨ Thanks goes to these wonderful people ([emoji
+key](https://allcontributors.org/docs/en/emoji-key)):       This project
+follows the [all-contributors](https://github.com/all-contributors/all-
+contributors) specification. Contributions of any kind welcome! ## Credits This
+package was created with [Cookiecutter](https://github.com/audreyr/
+cookiecutter) and the [browniebroke/cookiecutter-pypackage](https://github.com/
+browniebroke/cookiecutter-pypackage) project template.
```

