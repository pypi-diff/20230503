# Comparing `tmp/helium_positioning_api-0.0.2.dev1678370622.tar.gz` & `tmp/helium_positioning_api-0.0.2.dev1683125793.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helium_positioning_api-0.0.2.dev1678370622.tar", max compression
+gzip compressed data, was "helium_positioning_api-0.0.2.dev1683125793.tar", max compression
```

## Comparing `helium_positioning_api-0.0.2.dev1678370622.tar` & `helium_positioning_api-0.0.2.dev1683125793.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1080 2023-03-09 14:03:19.987660 helium_positioning_api-0.0.2.dev1678370622/LICENSE
--rw-r--r--   0        0        0     6541 2023-03-09 14:03:19.987660 helium_positioning_api-0.0.2.dev1678370622/README.md
--rw-r--r--   0        0        0     2257 2023-03-09 14:03:43.419869 helium_positioning_api-0.0.2.dev1678370622/pyproject.toml
--rw-r--r--   0        0        0      723 2023-03-09 14:03:19.991660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/DataObjects.py
--rw-r--r--   0        0        0       30 2023-03-09 14:03:19.991660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/__init__.py
--rw-r--r--   0        0        0     2198 2023-03-09 14:03:19.991660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/__main__.py
--rw-r--r--   0        0        0     2455 2023-03-09 14:03:19.995660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/api.py
--rw-r--r--   0        0        0     7215 2023-03-09 14:03:19.995660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/auxilary.py
--rw-r--r--   0        0        0     1106 2023-03-09 14:03:19.995660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/distance_prediction.py
--rw-r--r--   0        0        0     1189 2023-03-09 14:03:19.995660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/midpoint.py
--rw-r--r--   0        0        0      834 2023-03-09 14:03:19.995660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/nearest_neighbor.py
--rw-r--r--   0        0        0        0 2023-03-09 14:03:19.995660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/py.typed
--rw-r--r--   0        0        0    12994 2023-03-09 14:03:19.995660 helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/trilateration.py
--rw-r--r--   0        0        0     7768 1970-01-01 00:00:00.000000 helium_positioning_api-0.0.2.dev1678370622/setup.py
--rw-r--r--   0        0        0     7979 1970-01-01 00:00:00.000000 helium_positioning_api-0.0.2.dev1678370622/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-03 14:56:16.940494 helium_positioning_api-0.0.2.dev1683125793/LICENSE
+-rw-r--r--   0        0        0     6819 2023-05-03 14:56:16.940494 helium_positioning_api-0.0.2.dev1683125793/README.md
+-rw-r--r--   0        0        0     2257 2023-05-03 14:56:34.300801 helium_positioning_api-0.0.2.dev1683125793/pyproject.toml
+-rw-r--r--   0        0        0      723 2023-05-03 14:56:16.944494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/DataObjects.py
+-rw-r--r--   0        0        0       30 2023-05-03 14:56:16.944494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/__init__.py
+-rw-r--r--   0        0        0     2198 2023-05-03 14:56:16.944494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/__main__.py
+-rw-r--r--   0        0        0     2455 2023-05-03 14:56:16.944494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/api.py
+-rw-r--r--   0        0        0     7215 2023-05-03 14:56:16.944494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/auxilary.py
+-rw-r--r--   0        0        0     1106 2023-05-03 14:56:16.944494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/distance_prediction.py
+-rw-r--r--   0        0        0     1189 2023-05-03 14:56:16.944494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/midpoint.py
+-rw-r--r--   0        0        0      834 2023-05-03 14:56:16.944494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/nearest_neighbor.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:56:16.944494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/py.typed
+-rw-r--r--   0        0        0    12994 2023-05-03 14:56:16.948494 helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/trilateration.py
+-rw-r--r--   0        0        0     8054 1970-01-01 00:00:00.000000 helium_positioning_api-0.0.2.dev1683125793/setup.py
+-rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 helium_positioning_api-0.0.2.dev1683125793/PKG-INFO
```

### Comparing `helium_positioning_api-0.0.2.dev1678370622/LICENSE` & `helium_positioning_api-0.0.2.dev1683125793/LICENSE`

 * *Files identical despite different names*

### Comparing `helium_positioning_api-0.0.2.dev1678370622/README.md` & `helium_positioning_api-0.0.2.dev1683125793/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 [black]: https://github.com/psf/black
 
 ## Features
 
 Prediction of the location of devices belonging to an organization in the [Helium Console](https://console.helium.com/). 
 Several different methods and models are available.
 
+## Docker
+
+The easiest way to run the positioning-API is to prepare an `.env` file (see below for further instructions what should be in it) and run it as docker-container:
+
+```
+docker run -p 8000:8000 --env-file=.env ghcr.io/emergotechnologies/helium-positioning-api:main
+```
+
 ## Installation
 
 ### Developer install
 
 The following allows a user to create a developer install of the positioning api.
 
 ```console
```

### Comparing `helium_positioning_api-0.0.2.dev1678370622/pyproject.toml` & `helium_positioning_api-0.0.2.dev1683125793/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "helium-positioning-api"
-version = "0.0.2.dev.1678370622"
+version = "0.0.2.dev.1683125793"
 description = "Helium Positioning API"
 authors = ["Lukas Huber <lukas.huber@fh-kufstein.ac.at>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/emergotechnologies/helium-positioning-api"
 repository = "https://github.com/emergotechnologies/helium-positioning-api"
 documentation = "https://helium-positioning-api.readthedocs.io"
```

### Comparing `helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/DataObjects.py` & `helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/DataObjects.py`

 * *Files identical despite different names*

### Comparing `helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/__main__.py` & `helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/__main__.py`

 * *Files identical despite different names*

### Comparing `helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/api.py` & `helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/api.py`

 * *Files identical despite different names*

### Comparing `helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/auxilary.py` & `helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/auxilary.py`

 * *Files identical despite different names*

### Comparing `helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/distance_prediction.py` & `helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/distance_prediction.py`

 * *Files identical despite different names*

### Comparing `helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/midpoint.py` & `helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/midpoint.py`

 * *Files identical despite different names*

### Comparing `helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/nearest_neighbor.py` & `helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `helium_positioning_api-0.0.2.dev1678370622/src/helium_positioning_api/trilateration.py` & `helium_positioning_api-0.0.2.dev1683125793/src/helium_positioning_api/trilateration.py`

 * *Files identical despite different names*

### Comparing `helium_positioning_api-0.0.2.dev1678370622/setup.py` & `helium_positioning_api-0.0.2.dev1683125793/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
  'python-dotenv>=0.21.1,<0.22.0',
  'scikit-learn==1.0.2',
  'utm>=0.7.0,<0.8.0',
  'uvicorn>=0.19.0,<0.20.0']
 
 setup_kwargs = {
     'name': 'helium-positioning-api',
-    'version': '0.0.2.dev1678370622',
+    'version': '0.0.2.dev1683125793',
     'description': 'Helium Positioning API',
-    'long_description': '# Helium Positioning API\n\n[![PyPI](https://img.shields.io/pypi/v/helium-positioning-api.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/helium-positioning-api.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/helium-positioning-api)][python version]\n[![License](https://img.shields.io/pypi/l/helium-positioning-api)][license]\n\n[![Read the documentation at https://helium-positioning-api.readthedocs.io/](https://img.shields.io/readthedocs/helium-positioning-api-api-api-api-api-api/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/emergotechnologies/helium-positioning-api/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/emergotechnologies/helium-positioning-api/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/helium-positioning-api/\n[status]: https://pypi.org/project/helium-positioning-api/\n[python version]: https://pypi.org/project/helium-positioning-api\n[read the docs]: https://helium-positioning-api.readthedocs.io/\n[tests]: https://github.com/emergotechnologies/helium-positioning-api/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/emergotechnologies/helium-positioning-api\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\nPrediction of the location of devices belonging to an organization in the [Helium Console](https://console.helium.com/). \nSeveral different methods and models are available.\n\n## Installation\n\n### Developer install\n\nThe following allows a user to create a developer install of the positioning api.\n\n```console\npip install -r requirements.txt\npoetry install\npoetry shell\npip install git+https://github.com/emergotechnologies/helium-api-wrapper\n```\n\n## Prerequisites\n\nBefore use, ensure that there is an `.env` file in the root directory of the repository where the `API_KEY` variable is entered (see `.env.sample`). You can generate and copy the `API_KEY` at https://console.helium.com/profile.\n\n## Usage\n\nThe service allows usage via **command line interface** or locally hosted **REST interface**.\n\n### CLI\n\n**Get Device Position**\n\n```\npython -m helium_positioning_api predict --uuid 92f23793-6647-40aa-b255-fa1d4baec75d\n```\n\nCurrently defaults to the "nearest_neighbor" model.\n\n**Advanced Requests**\n\nThe location prediction command is\n\n```\npython -m helium_positioning_api predict --uuid \'your uuid\' --model \'your model selection\'\n```\n\nSee the table below for a list of currently available models.\n\n| **Model**                         | **Position estimation explanation**                                 | **Suggested use**                                                                                                                                                             |\n| --------------------------------- | ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| nearest_neighbor                  | Location of hotspot with the best signal                            | Purchase of at most one packet from a device (see [Packet Configurations](https://docs.helium.com/use-the-network/console/multi-packets/) for more details)                   |\n| midpoint                          | Point of equal distance from the two hotspots with the best signals | Purchase of at least two packets from a device (see [Packet Configurations](https://docs.helium.com/use-the-network/console/multi-packets/) for more details)                 |\n| linear_regression (experimental)  | Trilateration with an linear regression distance estimator          | Experimental. Purchase of at least three packets from a device (see [Packet Configurations](https://docs.helium.com/use-the-network/console/multi-packets/) for more details) |\n| gradient_boosting (experimental)  | Trilateration with a gradient boosted regression distance estimator | Experimental. Purchase of at least three packets from a device (see [Packet Configurations](https://docs.helium.com/use-the-network/console/multi-packets/) for more details) |\n\n### REST-API\n\n1. Start local REST-API (default)\n   ```\n   python -m helium_positioning_api serve\n   ```\n2. Open Browser and navigate to `127.0.0.1:8000/docs`\n3. Click on `predict_tf` path to drop down the endpoint details\n4. Click on the `Try it out` button.\n5. Fill in the `uuid` of your device and click on the button `Execute` to get an estimation using the `nearest_neighbor` model\n6. You can see the location prediction response in the `Responses` section below.\n\nThe mapping of available models to paths can be seen in the table below.\n\n| **model**         | **path**                                                            |\n| ----------------- | ------------------------------------------------------------------- |\n| nearest_neighbor  | predict_tf                                                          |\n| midpoint          | predict_mp                                                          |\n| linear_regression | predict_tl_lin                                                      |\n| gradient_boosting | predict_tl_grad                                                     |\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Helium Positioning API_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/emergotechnologies/helium-positioning-api/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/emergotechnologies/helium-positioning-api/blob/main/LICENSE\n[contributor guide]: https://github.com/emergotechnologies/helium-positioning-api/blob/main/CONTRIBUTING.md\n[command-line reference]: https://helium-positioning-api.readthedocs.io/en/latest/usage.html\n',
+    'long_description': '# Helium Positioning API\n\n[![PyPI](https://img.shields.io/pypi/v/helium-positioning-api.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/helium-positioning-api.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/helium-positioning-api)][python version]\n[![License](https://img.shields.io/pypi/l/helium-positioning-api)][license]\n\n[![Read the documentation at https://helium-positioning-api.readthedocs.io/](https://img.shields.io/readthedocs/helium-positioning-api-api-api-api-api-api/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/emergotechnologies/helium-positioning-api/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/emergotechnologies/helium-positioning-api/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/helium-positioning-api/\n[status]: https://pypi.org/project/helium-positioning-api/\n[python version]: https://pypi.org/project/helium-positioning-api\n[read the docs]: https://helium-positioning-api.readthedocs.io/\n[tests]: https://github.com/emergotechnologies/helium-positioning-api/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/emergotechnologies/helium-positioning-api\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\nPrediction of the location of devices belonging to an organization in the [Helium Console](https://console.helium.com/). \nSeveral different methods and models are available.\n\n## Docker\n\nThe easiest way to run the positioning-API is to prepare an `.env` file (see below for further instructions what should be in it) and run it as docker-container:\n\n```\ndocker run -p 8000:8000 --env-file=.env ghcr.io/emergotechnologies/helium-positioning-api:main\n```\n\n## Installation\n\n### Developer install\n\nThe following allows a user to create a developer install of the positioning api.\n\n```console\npip install -r requirements.txt\npoetry install\npoetry shell\npip install git+https://github.com/emergotechnologies/helium-api-wrapper\n```\n\n## Prerequisites\n\nBefore use, ensure that there is an `.env` file in the root directory of the repository where the `API_KEY` variable is entered (see `.env.sample`). You can generate and copy the `API_KEY` at https://console.helium.com/profile.\n\n## Usage\n\nThe service allows usage via **command line interface** or locally hosted **REST interface**.\n\n### CLI\n\n**Get Device Position**\n\n```\npython -m helium_positioning_api predict --uuid 92f23793-6647-40aa-b255-fa1d4baec75d\n```\n\nCurrently defaults to the "nearest_neighbor" model.\n\n**Advanced Requests**\n\nThe location prediction command is\n\n```\npython -m helium_positioning_api predict --uuid \'your uuid\' --model \'your model selection\'\n```\n\nSee the table below for a list of currently available models.\n\n| **Model**                         | **Position estimation explanation**                                 | **Suggested use**                                                                                                                                                             |\n| --------------------------------- | ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| nearest_neighbor                  | Location of hotspot with the best signal                            | Purchase of at most one packet from a device (see [Packet Configurations](https://docs.helium.com/use-the-network/console/multi-packets/) for more details)                   |\n| midpoint                          | Point of equal distance from the two hotspots with the best signals | Purchase of at least two packets from a device (see [Packet Configurations](https://docs.helium.com/use-the-network/console/multi-packets/) for more details)                 |\n| linear_regression (experimental)  | Trilateration with an linear regression distance estimator          | Experimental. Purchase of at least three packets from a device (see [Packet Configurations](https://docs.helium.com/use-the-network/console/multi-packets/) for more details) |\n| gradient_boosting (experimental)  | Trilateration with a gradient boosted regression distance estimator | Experimental. Purchase of at least three packets from a device (see [Packet Configurations](https://docs.helium.com/use-the-network/console/multi-packets/) for more details) |\n\n### REST-API\n\n1. Start local REST-API (default)\n   ```\n   python -m helium_positioning_api serve\n   ```\n2. Open Browser and navigate to `127.0.0.1:8000/docs`\n3. Click on `predict_tf` path to drop down the endpoint details\n4. Click on the `Try it out` button.\n5. Fill in the `uuid` of your device and click on the button `Execute` to get an estimation using the `nearest_neighbor` model\n6. You can see the location prediction response in the `Responses` section below.\n\nThe mapping of available models to paths can be seen in the table below.\n\n| **model**         | **path**                                                            |\n| ----------------- | ------------------------------------------------------------------- |\n| nearest_neighbor  | predict_tf                                                          |\n| midpoint          | predict_mp                                                          |\n| linear_regression | predict_tl_lin                                                      |\n| gradient_boosting | predict_tl_grad                                                     |\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Helium Positioning API_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/emergotechnologies/helium-positioning-api/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/emergotechnologies/helium-positioning-api/blob/main/LICENSE\n[contributor guide]: https://github.com/emergotechnologies/helium-positioning-api/blob/main/CONTRIBUTING.md\n[command-line reference]: https://helium-positioning-api.readthedocs.io/en/latest/usage.html\n',
     'author': 'Lukas Huber',
     'author_email': 'lukas.huber@fh-kufstein.ac.at',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/emergotechnologies/helium-positioning-api',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `helium_positioning_api-0.0.2.dev1678370622/PKG-INFO` & `helium_positioning_api-0.0.2.dev1683125793/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helium-positioning-api
-Version: 0.0.2.dev1678370622
+Version: 0.0.2.dev1683125793
 Summary: Helium Positioning API
 Home-page: https://github.com/emergotechnologies/helium-positioning-api
 License: MIT
 Author: Lukas Huber
 Author-email: lukas.huber@fh-kufstein.ac.at
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -55,14 +55,22 @@
 [black]: https://github.com/psf/black
 
 ## Features
 
 Prediction of the location of devices belonging to an organization in the [Helium Console](https://console.helium.com/). 
 Several different methods and models are available.
 
+## Docker
+
+The easiest way to run the positioning-API is to prepare an `.env` file (see below for further instructions what should be in it) and run it as docker-container:
+
+```
+docker run -p 8000:8000 --env-file=.env ghcr.io/emergotechnologies/helium-positioning-api:main
+```
+
 ## Installation
 
 ### Developer install
 
 The following allows a user to create a developer install of the positioning api.
 
 ```console
```

