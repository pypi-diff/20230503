# Comparing `tmp/skylab-0.1.1.tar.gz` & `tmp/skylab-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skylab-0.1.1.tar", max compression
+gzip compressed data, was "skylab-0.1.2.tar", max compression
```

## Comparing `skylab-0.1.1.tar` & `skylab-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1090 2023-04-23 21:28:56.735383 skylab-0.1.1/LICENSE
--rw-r--r--   0        0        0      831 2023-04-25 12:00:39.422608 skylab-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      857 2023-04-24 19:11:31.739686 skylab-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-21 22:27:55.460381 skylab-0.1.1/skylab/__init__.py
--rw-r--r--   0        0        0      236 2023-04-23 22:12:51.429163 skylab-0.1.1/skylab/__main__.py
--rw-r--r--   0        0        0     1112 2023-04-24 19:15:43.017845 skylab-0.1.1/skylab/api.py
--rw-r--r--   0        0        0      424 2023-04-24 13:45:07.205633 skylab-0.1.1/skylab/css/styles.css
--rw-r--r--   0        0        0     1668 2023-04-24 19:11:57.443257 skylab-0.1.1/skylab/models.py
--rw-r--r--   0        0        0     5100 2023-04-24 14:45:36.607699 skylab-0.1.1/skylab/skylab.py
--rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 skylab-0.1.1/setup.py
--rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 skylab-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-23 21:28:56.735383 skylab-0.1.2/LICENSE
+-rw-r--r--   0        0        0      831 2023-05-03 21:42:11.409035 skylab-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      857 2023-05-03 19:11:19.310742 skylab-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 22:27:55.460381 skylab-0.1.2/skylab/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-23 22:12:51.429163 skylab-0.1.2/skylab/__main__.py
+-rw-r--r--   0        0        0     1471 2023-05-03 21:07:31.551740 skylab-0.1.2/skylab/api.py
+-rw-r--r--   0        0        0      424 2023-04-24 13:45:07.205633 skylab-0.1.2/skylab/css/styles.css
+-rw-r--r--   0        0        0     1668 2023-04-25 20:23:37.949077 skylab-0.1.2/skylab/models.py
+-rw-r--r--   0        0        0     5206 2023-05-03 21:04:54.108267 skylab-0.1.2/skylab/skylab.py
+-rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 skylab-0.1.2/setup.py
+-rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 skylab-0.1.2/PKG-INFO
```

### Comparing `skylab-0.1.1/LICENSE` & `skylab-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skylab-0.1.1/pyproject.toml` & `skylab-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skylab"
-version = "0.1.1"
+version = "0.1.2"
 description = "A TUI for showing latest upcoming rocket launches."
 authors = ["SerhiiStets <stets.serhii@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository="https://github.com/SerhiiStets/skylab"
 
 [tool.poetry.dependencies]
```

### Comparing `skylab-0.1.1/README.md` & `skylab-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `skylab-0.1.1/skylab/api.py` & `skylab-0.1.2/skylab/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 """Api module for receiving data from thespacedevs."""
+import datetime
 
 import requests
 
 from skylab.models import Launch
 
-GET_UPCOMING_LAUNCHES = "https://lldev.thespacedevs.com/2.2.0/launch/upcoming/"
+GET_UPCOMING_LAUNCHES = "https://ll.thespacedevs.com/2.2.0/launch/upcoming/"
 
 
 def get_upcoming_laucnhes(url: str, timeout: float = 5.0) -> dict:
     """Get request for upcoming launches."""
-    response = requests.get(url, timeout=timeout)
-    response.raise_for_status()
-    return response.json()
+    try:
+        response = requests.get(url, timeout=timeout)
+        response.raise_for_status()
+        return response.json()
+    except requests.exceptions.RequestException as ex:
+        raise ValueError(f"Failed to retrieve upcoming launches: {ex}.")
 
 
 def launch_factory() -> list[Launch]:
     """Makes a request for upcoming launches, modifies and validates them."""
     results = get_upcoming_laucnhes(GET_UPCOMING_LAUNCHES)["results"]
     launches = []
     for launch_dict in results:
+        # checking if the launch date is not expired
+        net = datetime.datetime.fromisoformat(launch_dict["net"][:-1])
+        if net < datetime.datetime.now():
+            continue
+
         # removing "configuration" nested layer from given data
         rocket_config = launch_dict["rocket"].pop("configuration")
         launch_dict["rocket"].update(rocket_config)
 
         # getting address name from "location" json
         launch_pad_address = launch_dict["pad"].pop("location")["name"]
         launch_dict["pad"]["address"] = launch_pad_address
```

### Comparing `skylab-0.1.1/skylab/models.py` & `skylab-0.1.2/skylab/models.py`

 * *Files identical despite different names*

### Comparing `skylab-0.1.1/skylab/skylab.py` & `skylab-0.1.2/skylab/skylab.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,18 @@
         )
 
 
 class SkylabApp(App):
     """Skylab TUI app."""
 
     TITLE = "skylab"
-    BINDINGS = [("d", "exit", "Exit skylab.")]
+    BINDINGS = [
+        ("d", "exit", "Exit skylab."),
+        ("?", "", "SpaceDev API is free but allows no more than 15 requests per hour"),
+    ]
     CSS_PATH = os.path.join(CURR_DIR, "css/styles.css")
 
     def __init__(self, *args, **kwargs):
         """Initialize SkylabApp."""
         super().__init__(*args, **kwargs)
         self.launch_widget_list = [
             LaunchWidget(launch=launch) for launch in skylab.api.launch_factory()
```

### Comparing `skylab-0.1.1/setup.py` & `skylab-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'tzlocal>=4.3,<5.0']
 
 entry_points = \
 {'console_scripts': ['skylab = skylab.__main__:main']}
 
 setup_kwargs = {
     'name': 'skylab',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A TUI for showing latest upcoming rocket launches.',
     'long_description': '# Skylab\n\nSkylab is a text user interface (TUI) tool that displays upcoming space launches in a user-friendly way.\n\n## Instalation\n\nTo install Skylab using pip, run the following command:\n\n```\n$ pip install skylab\n```\n\n## Usage\n\nTo use Skylab, simply enter the following command in your terminal:\n\n```\n$ skylab\n```\n\n## Contributing\n\nHelp in testing, development, documentation and other tasks is\nhighly appreciated and useful to the project.\n\nTo get started with developing skylab, see [CONTRIBUTING.md](CONTRIBUTING.md).\n\n## Acknowledgments\n\nThis project makes use of the [The Space Devs API](https://thespacedevs.com/) to retrieve data about upcoming space launches. We would like to thank the creators of this API for providing this valuable service.\n\n## License\n\nSkylab is released under the [MIT License](LICENSE.md).\n',
     'author': 'SerhiiStets',
     'author_email': 'stets.serhii@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SerhiiStets/skylab',
```

### Comparing `skylab-0.1.1/PKG-INFO` & `skylab-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skylab
-Version: 0.1.1
+Version: 0.1.2
 Summary: A TUI for showing latest upcoming rocket launches.
 Home-page: https://github.com/SerhiiStets/skylab
 License: MIT
 Author: SerhiiStets
 Author-email: stets.serhii@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

