# Comparing `tmp/mepe-0.1.3.tar.gz` & `tmp/mepe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mepe-0.1.3.tar", max compression
+gzip compressed data, was "mepe-0.1.4.tar", max compression
```

## Comparing `mepe-0.1.3.tar` & `mepe-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2022-12-06 07:19:37.310016 mepe-0.1.3/LICENSE
--rw-r--r--   0        0        0      328 2022-12-08 08:51:15.430875 mepe-0.1.3/README.md
--rw-r--r--   0        0        0       18 2022-12-09 03:18:31.720436 mepe-0.1.3/mepe/__init__.py
--rw-r--r--   0        0        0     1306 2022-12-09 02:32:15.270943 mepe-0.1.3/mepe/display.py
--rw-r--r--   0        0        0      117 2022-12-08 03:15:44.638716 mepe-0.1.3/mepe/exceptions.py
--rw-r--r--   0        0        0      919 2022-12-08 03:43:11.838238 mepe-0.1.3/mepe/main.py
--rw-r--r--   0        0        0     1336 2022-12-09 02:40:22.614563 mepe-0.1.3/mepe/scrape.py
--rw-r--r--   0        0        0      480 2022-12-09 03:18:31.721339 mepe-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 mepe-0.1.3/setup.py
--rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 mepe-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-12-06 07:19:37.310016 mepe-0.1.4/LICENSE
+-rw-r--r--   0        0        0      328 2022-12-08 08:51:15.430875 mepe-0.1.4/README.md
+-rw-r--r--   0        0        0       18 2023-05-03 04:25:16.806429 mepe-0.1.4/mepe/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-03 04:24:35.716166 mepe-0.1.4/mepe/display.py
+-rw-r--r--   0        0        0      117 2022-12-08 03:15:44.638716 mepe-0.1.4/mepe/exceptions.py
+-rw-r--r--   0        0        0      919 2022-12-08 03:43:11.838238 mepe-0.1.4/mepe/main.py
+-rw-r--r--   0        0        0     1336 2022-12-09 02:40:22.614563 mepe-0.1.4/mepe/scrape.py
+-rw-r--r--   0        0        0      480 2023-05-03 04:25:16.807521 mepe-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 mepe-0.1.4/setup.py
+-rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 mepe-0.1.4/PKG-INFO
```

### Comparing `mepe-0.1.3/LICENSE` & `mepe-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mepe-0.1.3/mepe/display.py` & `mepe-0.1.4/mepe/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from rich.text import Text
 
 console = Console()
 logger = logging.getLogger(__name__)
 
 
 def display(metrics: List["prometheus_client.metrics_core.Metric"]) -> None:
+    metrics = sorted(metrics, key=lambda m: m.name)
+
     for metric in metrics:
         display_metric(metric)
 
 
 def display_metric(metric: "prometheus_client.metrics_core.Metric") -> None:
     name = Text(metric.name)
     # bold the common prefix which indicates the metrics group
```

### Comparing `mepe-0.1.3/mepe/main.py` & `mepe-0.1.4/mepe/main.py`

 * *Files identical despite different names*

### Comparing `mepe-0.1.3/mepe/scrape.py` & `mepe-0.1.4/mepe/scrape.py`

 * *Files identical despite different names*

### Comparing `mepe-0.1.3/setup.py` & `mepe-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'rich>=12.6.0,<13.0.0']
 
 entry_points = \
 {'console_scripts': ['mepe = mepe.main:main']}
 
 setup_kwargs = {
     'name': 'mepe',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': '# Prometheus Metrics Explorer\n\nCli Prometheus metrics viewer.\n\nSummaries metrics, useful when you configure a new Grafana dashboard for a new component, and want to check what metrics does it have.\n\n## Installation\n\n```shell\npip install mepe\n```\n\n## Usage\n\n```shell\nmepe http://127.0.0.1:9100/metrics\n```\n\n\n![](./docs/mepe.png)\n',
     'author': 'laixintao',
     'author_email': 'laixintaoo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mepe-0.1.3/PKG-INFO` & `mepe-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mepe
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: laixintao
 Author-email: laixintaoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

