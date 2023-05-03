# Comparing `tmp/krisi-0.1.1.tar.gz` & `tmp/krisi-0.1.2.tar.gz`

## Comparing `krisi-0.1.1.tar` & `krisi-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,50 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-0.1.1/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.1.1/.isort.cfg
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 krisi-0.1.1/mkdocs.yaml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.1.1/.vscode/launch.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/assertions.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/compare.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/dataset.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/group.py
--rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/metric.py
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/score.py
--rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/scorecard.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/type.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/__init__.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/default_metrics_classification.py
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/default_metrics_regression.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/diagrams.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/metric_wrappers.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/__init__.py
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/console.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/interactive.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/pdf.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/report.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/type.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/vizualise.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/console/diagrams.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/pdf_layouts/default/template.css
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/pdf_layouts/default/template.html
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.css
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/console_plot.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/data.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/environment.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/io.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/iterable_helpers.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/printing.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/devutils/timing.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-0.1.1/.gitignore
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.1.1/LICENSE
--rw-r--r--   0        0        0    27691 2020-02-02 00:00:00.000000 krisi-0.1.1/README.md
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 krisi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    32385 2020-02-02 00:00:00.000000 krisi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-0.1.2/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.1.2/.isort.cfg
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 krisi-0.1.2/mkdocs.yaml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.1.2/.vscode/launch.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/analyse/__init__.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/analyse/correlations.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/analyse/dataset.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/analyse/utils.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/assertions.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/compare.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/group.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/metric.py
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/score.py
+-rw-r--r--   0        0        0    20417 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/scorecard.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/type.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/__init__.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/default_metrics_classification.py
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/default_metrics_regression.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/diagrams.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/metric_wrappers.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/__init__.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/console.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/graph.py
+-rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/interactive.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/pdf.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/report.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/type.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/vizualise.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/console/diagrams.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/pdf_layouts/default/template.css
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/pdf_layouts/default/template.html
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/pdf_layouts/scorecard/report.css
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/pdf_layouts/scorecard/report.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/console_plot.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/data.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/environment.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/io.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/iterable_helpers.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/printing.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/devutils/timing.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-0.1.2/.gitignore
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.1.2/LICENSE
+-rw-r--r--   0        0        0    27691 2020-02-02 00:00:00.000000 krisi-0.1.2/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 krisi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    32477 2020-02-02 00:00:00.000000 krisi-0.1.2/PKG-INFO
```

### Comparing `krisi-0.1.1/mkdocs.yaml` & `krisi-0.1.2/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/.vscode/settings.json` & `krisi-0.1.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/assertions.py` & `krisi-0.1.2/src/krisi/evaluate/assertions.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/compare.py` & `krisi-0.1.2/src/krisi/evaluate/compare.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/dataset.py` & `krisi-0.1.2/src/krisi/analyse/dataset.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/group.py` & `krisi-0.1.2/src/krisi/evaluate/group.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/metric.py` & `krisi-0.1.2/src/krisi/evaluate/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     def __getitem__(self, key: str) -> Any:
         return getattr(self, key, "Unknown Field")
 
     def __str__(self) -> str:
         return print_metric(self)
 
     def __repr__(self) -> str:
-        return print_metric(self, repr=True)
+        print(print_metric(self, repr=True))
+        return super().__repr__()
 
     def _evaluation(self, *args) -> "Metric":
         try:
             result = self.func(*args, **self.parameters)
         except Exception as e:
             result = e
         self.__safe_set(result, key="result")
```

### Comparing `krisi-0.1.1/src/krisi/evaluate/score.py` & `krisi-0.1.2/src/krisi/evaluate/score.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/scorecard.py` & `krisi-0.1.2/src/krisi/evaluate/scorecard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import datetime
 from copy import deepcopy
-from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from IPython.display import display
 from rich import print
-from rich.pretty import Pretty
 
 from krisi.evaluate.assertions import (
     check_valid_pred_target,
     is_dataset_classification_like,
 )
 from krisi.evaluate.group import Group
 from krisi.evaluate.library.default_metrics_classification import (
@@ -65,15 +63,14 @@
         The converted data.
     """
     if isinstance(data, pd.Series):
         return data.rename(name)
     return pd.Series(data, name=name)
 
 
-@dataclass
 class ScoreCard:
     """
     ScoreCard Object.
 
     Krisi's main object holding and evaluating metrics.
     Stores, evaluates and generates vizualisations of predefined
     and custom metrics for regression and classification.
@@ -151,17 +148,15 @@
         rolling_args: Optional[Dict[str, Any]] = None,
     ) -> None:
         check_valid_pred_target(y, predictions)
         self.__dict__["y"] = convert_to_series(y, "y")
         self.__dict__["predictions"] = convert_to_series(predictions, "predictions")
         self.__dict__["sample_type"] = sample_type
         self.__dict__["rolling_args"] = (
-            rolling_args
-            if rolling_args is not None
-            else dict(window=len(y) // 100, step=len(y) // 100)
+            rolling_args if rolling_args is not None else dict(window=len(y) // 100)
         )
         self.__dict__["classification"] = (
             is_dataset_classification_like(y)
             if classification is None
             else classification
         )
         model_name_, dataset_name_, project_name_ = handle_unnamed(
@@ -213,16 +208,20 @@
             return scorecard_copy
         elif isinstance(key, str):
             return getattr(self, key, Metric("Unknown Metric"))
 
     def __delitem__(self, key: str) -> None:
         del self[key]
 
+    def __repr__(self) -> str:
+        self.print(mode=PrintMode.minimal)
+        return super().__repr__()
+
     def __str__(self) -> str:
-        print(Pretty(self.__dict__))
+        self.print(mode=PrintMode.minimal)
         return ""
 
     def __setattr__(self, key: str, item: Any) -> None:
         """
         Defines Dictionary like behaviour and ensures that a Metric can be
         added as a:
```

### Comparing `krisi-0.1.1/src/krisi/evaluate/type.py` & `krisi-0.1.2/src/krisi/evaluate/type.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/utils.py` & `krisi-0.1.2/src/krisi/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/library/default_metrics_classification.py` & `krisi-0.1.2/src/krisi/evaluate/library/default_metrics_classification.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/library/default_metrics_regression.py` & `krisi-0.1.2/src/krisi/evaluate/library/default_metrics_regression.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/evaluate/library/diagrams.py` & `krisi-0.1.2/src/krisi/evaluate/library/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/report/console.py` & `krisi-0.1.2/src/krisi/report/console.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     from krisi.evaluate.metric import Metric
     from krisi.evaluate.scorecard import ScoreCard
 
 from krisi.utils.printing import bold
 
 
 def print_metric(obj: "Metric", repr: bool = False) -> str:
+    if repr:
+        return f"{obj.result} | {obj.name}"
     hyperparams = ""
     if obj.parameters is not None:
         hyperparams += "".join(
             [f"{key} - {value}" for key, value in obj.parameters.items()]
         )
     if (
         obj.result is None
```

### Comparing `krisi-0.1.1/src/krisi/report/interactive.py` & `krisi-0.1.2/src/krisi/report/interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from krisi.evaluate.type import ScoreCardMetadata
 from krisi.report.type import InteractiveFigure, PlotlyInput
+from krisi.utils.environment import is_notebook
 from krisi.utils.iterable_helpers import flatten
 
 if TYPE_CHECKING:
     from dash import dcc, html
 
 
 external_script = ["https://tailwindcss.com/", {"src": "https://cdn.tailwindcss.com"}]
@@ -166,8 +167,11 @@
         if len(component.inputs) > 0 or len(component.global_input_ids) > 0:
             app.callback(
                 Output(component.id, "figure"),
                 [Input(input_.id, input_.value_name) for input_ in component.inputs]
                 + [Input(input_id, "value") for input_id in component.global_input_ids],
             )(component.get_figure)
 
-    app.run(debug=True, threaded=True)
+    if is_notebook():
+        app.run(mode="inline", debug=False, threaded=True)
+    else:
+        app.run(debug=False, threaded=True)
```

### Comparing `krisi-0.1.1/src/krisi/report/pdf.py` & `krisi-0.1.2/src/krisi/report/pdf.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/report/report.py` & `krisi-0.1.2/src/krisi/report/report.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/report/type.py` & `krisi-0.1.2/src/krisi/report/type.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/report/vizualise.py` & `krisi-0.1.2/src/krisi/report/vizualise.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/report/library/console/diagrams.py` & `krisi-0.1.2/src/krisi/report/library/console/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/report/library/pdf_layouts/default/template.html` & `krisi-0.1.2/src/krisi/report/library/pdf_layouts/default/template.html`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.css` & `krisi-0.1.2/src/krisi/report/library/pdf_layouts/scorecard/report.css`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.html` & `krisi-0.1.2/src/krisi/report/library/pdf_layouts/scorecard/report.html`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/utils/console_plot.py` & `krisi-0.1.2/src/krisi/utils/console_plot.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/utils/data.py` & `krisi-0.1.2/src/krisi/utils/data.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/utils/environment.py` & `krisi-0.1.2/src/krisi/utils/environment.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/utils/io.py` & `krisi-0.1.2/src/krisi/utils/io.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/utils/iterable_helpers.py` & `krisi-0.1.2/src/krisi/utils/iterable_helpers.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/utils/printing.py` & `krisi-0.1.2/src/krisi/utils/printing.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/src/krisi/utils/devutils/timing.py` & `krisi-0.1.2/src/krisi/utils/devutils/timing.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/.gitignore` & `krisi-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/LICENSE` & `krisi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/README.md` & `krisi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `krisi-0.1.1/pyproject.toml` & `krisi-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krisi"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Mark Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 description = "Testing and Reporting framework for Time Series Analysis"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -79,15 +79,17 @@
 ]
 plotting = [
   "plotly",
   "dash",
   "jupyter_dash",
   "weasyprint",
   "kaleido",
-  "pangocffi"
+  "pangocffi",
+  "matplotlib",
+  "networkx"
 ]
 
 [tool.hatch.envs.quality]
 dependencies = [
   "krisi[quality]"
 ]
 detached = true
@@ -133,15 +135,15 @@
   "src",
   ".",
 ]
 testpaths = ["tests"] 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `krisi-0.1.1/PKG-INFO` & `krisi-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krisi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Testing and Reporting framework for Time Series Analysis
 Project-URL: Documentation, https://dream-faster.github.io/krisi
 Project-URL: Issues, https://github.com/dream-faster/krisi/issues
 Project-URL: Source, https://github.com/dream-faster/krisi
 Author-email: Mark Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
         
@@ -73,14 +73,16 @@
 Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: plotting
 Requires-Dist: dash; extra == 'plotting'
 Requires-Dist: jupyter-dash; extra == 'plotting'
 Requires-Dist: kaleido; extra == 'plotting'
+Requires-Dist: matplotlib; extra == 'plotting'
+Requires-Dist: networkx; extra == 'plotting'
 Requires-Dist: pangocffi; extra == 'plotting'
 Requires-Dist: plotly; extra == 'plotting'
 Requires-Dist: weasyprint; extra == 'plotting'
 Provides-Extra: quality
 Requires-Dist: black~=22.10.0; extra == 'quality'
 Requires-Dist: flake8~=4.0.1; extra == 'quality'
 Requires-Dist: isort~=5.10.1; extra == 'quality'
```

