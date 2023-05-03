# Comparing `tmp/krisi-0.1.2.tar.gz` & `tmp/krisi-0.1.3.tar.gz`

## Comparing `krisi-0.1.2.tar` & `krisi-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,48 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-0.1.2/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.1.2/.isort.cfg
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 krisi-0.1.2/mkdocs.yaml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.1.2/.vscode/launch.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/analyse/__init__.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/analyse/correlations.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/analyse/dataset.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/analyse/utils.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/assertions.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/compare.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/group.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/metric.py
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/score.py
--rw-r--r--   0        0        0    20417 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/scorecard.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/type.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/__init__.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/default_metrics_classification.py
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/default_metrics_regression.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/diagrams.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/evaluate/library/metric_wrappers.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/__init__.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/console.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/graph.py
--rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/interactive.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/pdf.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/report.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/type.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/vizualise.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/console/diagrams.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/pdf_layouts/default/template.css
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/pdf_layouts/default/template.html
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/pdf_layouts/scorecard/report.css
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/report/library/pdf_layouts/scorecard/report.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/console_plot.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/data.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/environment.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/io.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/iterable_helpers.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/printing.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-0.1.2/src/krisi/utils/devutils/timing.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-0.1.2/.gitignore
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.1.2/LICENSE
--rw-r--r--   0        0        0    27691 2020-02-02 00:00:00.000000 krisi-0.1.2/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 krisi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    32477 2020-02-02 00:00:00.000000 krisi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-0.1.3/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.1.3/.isort.cfg
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 krisi-0.1.3/mkdocs.yaml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.1.3/.vscode/launch.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/analyse/__init__.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/analyse/correlations.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/analyse/dataset.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/analyse/utils.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/assertions.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/compare.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/group.py
+-rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/metric.py
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/score.py
+-rw-r--r--   0        0        0    21175 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/scorecard.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/type.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/__init__.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/default_metrics_classification.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/default_metrics_regression.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/diagrams.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/metric_wrappers.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/__init__.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/console.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/graph.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/interactive.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/pdf.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/report.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/type.py
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/vizualise.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/library/console/diagrams.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/library/pdf_layouts/scorecard/report.css
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/library/pdf_layouts/scorecard/report.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/console_plot.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/data.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/environment.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/io.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/iterable_helpers.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/printing.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/devutils/timing.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-0.1.3/.gitignore
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.1.3/LICENSE
+-rw-r--r--   0        0        0    27691 2020-02-02 00:00:00.000000 krisi-0.1.3/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 krisi-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    32477 2020-02-02 00:00:00.000000 krisi-0.1.3/PKG-INFO
```

### Comparing `krisi-0.1.2/mkdocs.yaml` & `krisi-0.1.3/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/.vscode/settings.json` & `krisi-0.1.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/analyse/correlations.py` & `krisi-0.1.3/src/krisi/analyse/correlations.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/analyse/dataset.py` & `krisi-0.1.3/src/krisi/analyse/dataset.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/evaluate/assertions.py` & `krisi-0.1.3/src/krisi/evaluate/assertions.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/evaluate/compare.py` & `krisi-0.1.3/src/krisi/evaluate/compare.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/evaluate/group.py` & `krisi-0.1.3/src/krisi/evaluate/group.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/evaluate/metric.py` & `krisi-0.1.3/src/krisi/evaluate/metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from dataclasses import dataclass, field
-from typing import Any, Generic, List, Optional, Union
+from typing import Any, Dict, Generic, List, Optional, Tuple, Union
 
 import pandas as pd
 
 from krisi.evaluate.type import (
     ComputationalComplexity,
     MetricCategories,
     MetricFunction,
@@ -60,16 +60,16 @@
     name: str
     key: str = ""
     category: Optional[MetricCategories] = None
     result: Optional[Union[Exception, MetricResult, List[MetricResult]]] = None
     result_rolling: Optional[Union[Exception, MetricResult, List[MetricResult]]] = None
     parameters: dict = field(default_factory=dict)
     func: Optional[MetricFunction] = None
-    plot_funcs: Optional[List[PlotFunction]] = None
-    plot_func_rolling: Optional[PlotFunction] = None
+    plot_funcs: Optional[List[Tuple[PlotFunction, Optional[Dict[str, Any]]]]] = None
+    plot_func_rolling: Optional[Tuple[PlotFunction, Optional[Dict[str, Any]]]] = None
     info: str = ""
     restrict_to_sample: Optional[SampleTypes] = None
     comp_complexity: Optional[ComputationalComplexity] = None
     disable_rolling: bool = False
 
     def __post_init__(self):
         if self.key == "":
@@ -167,34 +167,47 @@
         logging.info("No plot_func_rolling (Plotting Function Rolling) specified")
         return None
     elif isinstance(obj.result_rolling, Exception) or obj.result_rolling is None:
         return None
     elif isiterable(obj.result_rolling):
         return [
             InteractiveFigure(
-                f"{obj.key}_{obj.plot_func_rolling.__name__}",
+                f"{obj.key}_{obj.plot_func_rolling[0].__name__}",
                 get_figure=plotly_interactive(
-                    obj.plot_func_rolling, obj.result_rolling, title=obj.name
+                    obj.plot_func_rolling[0], obj.result_rolling, title=obj.name
                 ),
+                title=f"{obj.name} - {obj.plot_func_rolling[0].__name__}",
                 category=obj.category,
+                plot_args=merge_default_dict(obj.plot_func_rolling[1]),
             )
         ]
     else:
         return None
 
 
+def merge_default_dict(
+    new_dict: Optional[Dict[str, Any]] = None,
+    default_dict: Dict[str, Any] = dict(width=900.0, height=600.0),
+) -> Dict[str, Any]:
+    if new_dict is None:
+        return default_dict
+    else:
+        return {**default_dict, **new_dict}
+
+
 def create_diagram(obj: Metric) -> Optional[List[InteractiveFigure]]:
     if obj.plot_funcs is None:
         logging.info("No plot_func (Plotting Function) specified")
         return None
     elif isinstance(obj.result, Exception) or obj.result is None:
         return None
     else:
         return [
             InteractiveFigure(
                 f"{obj.key}_{plot_func.__name__}",
                 get_figure=plotly_interactive(plot_func, obj.result, title=obj.name),
                 title=f"{obj.name} - {plot_func.__name__}",
                 category=obj.category,
+                plot_args=merge_default_dict(plot_args),
             )
-            for plot_func in obj.plot_funcs
+            for plot_func, plot_args in obj.plot_funcs
         ]
```

### Comparing `krisi-0.1.2/src/krisi/evaluate/score.py` & `krisi-0.1.3/src/krisi/evaluate/score.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     project_name: Optional[str] = None,
     default_metrics: Optional[List[Metric]] = None,
     custom_metrics: Optional[List[Metric]] = None,
     classification: Optional[bool] = None,
     sample_type: SampleTypes = SampleTypes.outofsample,
     calculation: Union[Calculation, str] = Calculation.single,
     rolling_args: Optional[Dict[str, Any]] = None,
+    **kwargs,
 ) -> ScoreCard:
     """
     Creates a ScoreCard based on the passed in arguments, evaluates and then returns the ScoreCard.
 
     Parameters
     ----------
     y: Targets
@@ -80,14 +81,15 @@
         dataset_name=dataset_name,
         project_name=project_name,
         sample_type=sample_type,
         classification=classification,
         default_metrics=default_metrics,
         custom_metrics=custom_metrics,
         rolling_args=rolling_args,
+        **kwargs,
     )
 
     if calculation == Calculation.single or calculation == Calculation.single.value:
         sc.evaluate()
     elif calculation == Calculation.rolling or calculation == Calculation.rolling.value:
         sc.evaluate_over_time()
     elif calculation == Calculation.both or calculation == Calculation.both.value:
```

### Comparing `krisi-0.1.2/src/krisi/evaluate/scorecard.py` & `krisi-0.1.3/src/krisi/evaluate/scorecard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import os
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from IPython.display import display
@@ -33,19 +34,20 @@
     get_large_metric_summary,
     get_minimal_summary,
     get_summary,
 )
 from krisi.report.report import create_report_from_scorecard
 from krisi.report.type import DisplayModes, InteractiveFigure
 from krisi.utils.environment import is_notebook
-from krisi.utils.io import save_console, save_minimal_summary, save_object
+from krisi.utils.io import ensure_path, save_console, save_minimal_summary, save_object
 from krisi.utils.iterable_helpers import (
     flatten,
     map_newdict_on_olddict,
     remove_nans,
+    replace_if_None,
     strip_builtin_functions,
     wrap_in_list,
 )
 
 
 def convert_to_series(
     data: Union[List[float], List[int], pd.Series, np.ndarray], name: str
@@ -126,14 +128,15 @@
     predictions: Predictions
     sample_type: SampleTypes
     default_metrics_keys: List[str]
     custom_metrics_keys: List[str]
     classification: bool  # TODO: Support multilabel classification
     metadata: ScoreCardMetadata
     rolling_args: Dict[str, Any]
+    save_path: Path
 
     def __init__(
         self,
         y: Targets,
         predictions: Predictions,
         model_name: Optional[str] = None,
         model_description: str = "",
@@ -189,14 +192,24 @@
 
         for metric in default_metrics:
             self.__dict__[metric.key] = deepcopy(metric)
 
         for metric in custom_metrics:
             self.__dict__[metric.key] = deepcopy(metric)
 
+        self.__dict__["save_path"] = Path(
+            os.path.join(
+                PathConst.default_eval_output_path,
+                replace_if_None(
+                    self.metadata.project_name,
+                    f"{datetime.datetime.now().strftime('%d-%m')}_{self.metadata.model_name}_{self.metadata.dataset_name}",
+                ),
+            )
+        )
+
     def __setitem__(self, key: str, item: Any) -> None:
         self.__setattr__(key, item)
 
     def __getitem__(self, key: Union[str, List[str]]) -> Union["ScoreCard", Metric]:
         if isinstance(key, List):
             scorecard_copy = deepcopy(self)
             all_keys = list(scorecard_copy.__dict__.keys())
@@ -483,37 +496,31 @@
             if isinstance(to_display, (pd.DataFrame, pd.Series)) and is_notebook():
                 display(to_display)
             else:
                 print(to_display)
 
     def save(
         self,
-        path: Path = PathConst.default_eval_output_path,
         with_info: bool = False,
         save_modes: List[Union[SaveModes, str]] = [
             SaveModes.minimal,
             SaveModes.obj,
             SaveModes.text,
         ],
+        override_base_path: Optional[Path] = None,
+        timestamping: bool = True,
     ) -> "ScoreCard":
-        import os
-
-        if self.metadata.project_name:
-            path = Path(os.path.join(path, Path(f"{self.metadata.project_name}")))
-        path = Path(
+        path = replace_if_None(
+            override_base_path,
             os.path.join(
-                path,
-                Path(
-                    f"{datetime.datetime.now().strftime('%H-%M-%S')}_{self.metadata.model_name}_{self.metadata.dataset_name}"
-                ),
-            )
+                self.save_path,
+                f"scorecards/{datetime.datetime.now().strftime('%H-%M-%S-%f') if timestamping else 'scorecard'}",
+            ),
         )
-
-        if not os.path.exists(path):
-            os.makedirs(path)
+        ensure_path(path)
 
         if SaveModes.minimal in save_modes or SaveModes.minimal.value in save_modes:
             save_minimal_summary(self, path)
         if SaveModes.obj in save_modes or SaveModes.obj.value in save_modes:
             save_object(self, path)
         save_console(self, path, with_info, save_modes)
 
@@ -530,21 +537,33 @@
         self,
         display_modes: Union[str, List[str], DisplayModes, List[DisplayModes]] = [
             DisplayModes.interactive
         ],
         html_template_url: Path = PathConst.html_report_template_url,
         css_template_url: Path = PathConst.css_report_template_url,
         author: str = "",
+        report_title: Optional[str] = None,
+        override_base_path: Optional[Path] = None,
     ) -> None:
+        save_path = replace_if_None(override_base_path, self.save_path)
+        ensure_path(save_path)
+
+        display_modes = [
+            DisplayModes.from_str(mode) for mode in wrap_in_list(display_modes)
+        ]
         report = create_report_from_scorecard(
             self,
             display_modes,
             html_template_url,
             css_template_url,
             author=author,
+            report_title=replace_if_None(
+                report_title, f"Report on {self.metadata.project_name}"
+            ),
+            save_path=save_path,
         )
         report.generate_launch()
 
 
 def get_rolling_diagrams(obj: "ScoreCard") -> List[List[InteractiveFigure]]:
     return [
         diagram
```

### Comparing `krisi-0.1.2/src/krisi/evaluate/type.py` & `krisi-0.1.3/src/krisi/evaluate/type.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/evaluate/utils.py` & `krisi-0.1.3/src/krisi/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/evaluate/library/default_metrics_classification.py` & `krisi-0.1.3/src/krisi/evaluate/library/default_metrics_classification.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,59 +12,59 @@
 
 accuracy = Metric[float](
     name="Accuracy",
     key="accuracy",
     category=MetricCategories.class_err,
     info="In multilabel classification, this function computes subset accuracy: the set of labels predicted for a sample must exactly match the corresponding set of labels in y_true. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.accuracy_score.html",
     func=accuracy_score,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=500.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 recall = Metric[float](
     name="Recall",
     key="recall",
     category=MetricCategories.class_err,
     info="The recall is the ratio tp / (tp + fn) where tp is the number of true positives and fn the number of false negatives. The recall is intuitively the ability of the classifier to find all the positive samples.\nThe best value is 1 and the worst value is 0. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.recall_score.html",
     parameters={"average": "binary"},
     func=recall_score,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=500.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """~"""
 precision = Metric[float](
     name="Precision",
     key="precision",
     category=MetricCategories.class_err,
     info="The precision is the ratio tp / (tp + fp) where tp is the number of true positives and fp the number of false positives. The precision is intuitively the ability of the classifier not to label as positive a sample that is negative.\nThe best value is 1 and the worst value is 0. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html",
     parameters={"average": "binary"},
     func=precision_score,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=500.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """~"""
 f_one_score = Metric[float](
     name="F1 Score",
     key="f_one_score",
     category=MetricCategories.class_err,
     info="The F1 score can be interpreted as a harmonic mean of the precision and recall, where an F1 score reaches its best value at 1 and worst score at 0. The relative contribution of precision and recall to the F1 score are equal. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html",
     parameters={"average": "macro"},
     func=f1_score,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=500.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """~"""
 matthew_corr = Metric[float](
     name="Matthew Correlation Coefficient",
     key="matthew_corr",
     category=MetricCategories.class_err,
     info="The Matthews correlation coefficient is used in machine learning as a measure of the quality of binary and multiclass classifications. It takes into account true and false positives and negatives and is generally regarded as a balanced measure which can be used even if the classes are of very different sizes. The MCC is in essence a correlation coefficient value between -1 and +1. A coefficient of +1 represents a perfect prediction, 0 an average random prediction and -1 an inverse prediction. The statistic is also known as the phi coefficient.",
     func=matthews_corrcoef,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=500.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """~"""
 all_classification_metrics = [accuracy, recall, precision, f_one_score, matthew_corr]
 """~"""
 minimal_classification_metrics = [accuracy, f_one_score]
 """~"""
```

### Comparing `krisi-0.1.2/src/krisi/evaluate/library/default_metrics_regression.py` & `krisi-0.1.3/src/krisi/evaluate/library/default_metrics_regression.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,114 +23,118 @@
 
 mae = Metric[float](
     name="Mean Absolute Error",
     key="mae",
     category=MetricCategories.reg_err,
     info="(Mean absolute error) represents the difference between the original and predicted values extracted by averaged the absolute difference over the data set.",
     func=mean_absolute_error,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=900.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 mape = Metric[float](
     name="Mean Absolute Percentage Error",
     key="mape",
     category=MetricCategories.reg_err,
     func=mean_absolute_percentage_error,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=900.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 smape = Metric[float](
     name="Symmetric Mean Absolute Percentage Error",
     key="smape",
     category=MetricCategories.reg_err,
     func=lambda y_true, y_pred: np.mean(
         np.abs(y_pred - y_true) / (np.abs(y_true) + np.abs(y_pred)), axis=0
     ),
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=900.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 mse = Metric[float](
     name="Mean Squared Error",
     key="mse",
     category=MetricCategories.reg_err,
     info="(Mean Squared Error) represents the difference between the original and predicted values extracted by squared the average difference over the data set.",
     parameters={"squared": True},
     func=mean_squared_error,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=900.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 rmse = Metric[float](
     name="Root Mean Squared Error",
     key="rmse",
     category=MetricCategories.reg_err,
     info="(Root Mean Squared Error) is the error rate by the square root of Mean Squared Error.",
     parameters={"squared": False},
     func=mean_squared_error,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=900.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 rmsle = Metric[float](
     name="Root Mean Squared Log Error",
     key="rmsle",
     category=MetricCategories.reg_err,
     parameters={"squared": False},
     func=mean_squared_log_error,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=900.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 r_two = Metric[float](
     name="R-squared",
     key="r_two",
     category=MetricCategories.reg_err,
     info="(Coefficient of determination) represents the coefficient of how well the values fit compared to the original values. The value from 0 to 1 interpreted as percentages. The higher the value is, the better the model is.",
     func=r2_score,
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=900.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 residuals = Metric[List[float]](
     name="Residuals",
     key="residuals",
     category=MetricCategories.residual,
     func=lambda y, pred: y - pred,
-    plot_funcs=[display_acf_plot, display_density_plot, display_time_series],
+    plot_funcs=[
+        (display_acf_plot, dict(width=1500.0)),
+        (display_density_plot, dict(width=1500.0)),
+        (display_time_series, dict(width=1500.0)),
+    ],
     disable_rolling=True,
 )
 """ ~ """
 
 residuals_mean = Metric[float](
     name="Mean of the Residuals",
     key="residuals_mean",
     category=MetricCategories.residual,
     func=lambda res: res.mean(),
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=900.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 residuals_std = Metric[float](
     name="Standard Deviation of the Residuals",
     key="residuals_std",
     category=MetricCategories.residual,
     func=lambda res: res.std(),
-    plot_funcs=[display_single_value],
-    plot_func_rolling=display_time_series,
+    plot_funcs=[(display_single_value, dict(width=900.0))],
+    plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 ljung_box_statistics = Metric[pd.DataFrame](
     name="Ljung Box Statistics",
     key="ljung_box_statistics",
     category=MetricCategories.residual,
```

### Comparing `krisi-0.1.2/src/krisi/evaluate/library/diagrams.py` & `krisi-0.1.3/src/krisi/evaluate/library/diagrams.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         y=lower_y,
         mode="lines",
         fillcolor="rgba(32, 146, 230,0.3)",
         fill="tonexty",
         line_color="rgba(255,255,255,0)",
     )
     fig.update_traces(showlegend=False)
-    fig.update_xaxes(range=[-1, 42])
+    fig.update_xaxes(range=[-1, len(corr_array[0]) + 2])
     fig.update_yaxes(zerolinecolor="#000000")
 
     fig.update_layout(title=title)
     return fig
 
 
 def display_density_plot(
```

### Comparing `krisi-0.1.2/src/krisi/report/console.py` & `krisi-0.1.3/src/krisi/report/console.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/report/graph.py` & `krisi-0.1.3/src/krisi/report/graph.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/report/interactive.py` & `krisi-0.1.3/src/krisi/report/interactive.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,19 @@
         className="flex flex-row flex-wrap",
     )
 
 
 def figure_with_controller(figure: InteractiveFigure):
     if len(figure.inputs) > 0 or len(figure.global_input_ids) > 0:
         return block(
-            graph=dcc.Graph(id=figure.id, className="h-full flex align-center w-1/2"),
+            graph=dcc.Graph(
+                id=figure.id,
+                figure=figure.get_figure(width=figure.plot_args["width"] - 216.0),
+                className="h-full flex align-center",
+            ),
             title=None,
             controllers=html.Div(
                 className="h-full flex align-center",
                 children=[
                     input_.type(
                         className="h-full min-w-[150px] flex justify-center align-center",
                         id=input_.id,
@@ -41,17 +45,17 @@
                     for input_ in figure.inputs
                 ],
             ),
         )
 
     else:
         return dcc.Graph(
-            className="h-full flex align-center w-1/2",
+            className="h-full flex align-center",
             id=figure.id,
-            figure=figure.get_figure(),
+            figure=figure.get_figure(width=figure.plot_args["width"] - 216.0),
             style={"display": "inline-block"},
         )
 
 
 def category_block(category: str, figures: List[InteractiveFigure]) -> "html.Div":
     return html.Div(
         className="flex flex-col shadow-lg mb-4",
@@ -125,23 +129,29 @@
     title: str = "",
     description: str = "",
     scorecard_metadata: Optional[ScoreCardMetadata] = None,
 ) -> None:
     import sys
 
     from dash import Dash, Input, Output, dcc, html
+    from jupyter_dash import JupyterDash
+
+    isnotebook = is_notebook()
 
     sys.modules[__name__].html = html
     sys.modules[__name__].dcc = dcc
 
-    app = Dash(__name__, external_scripts=external_script)
+    if isnotebook:
+        app = JupyterDash(__name__, external_scripts=external_script)
+    else:
+        app = Dash(__name__, external_scripts=external_script)
     app.scripts.config.serve_locally = True
 
     app.layout = html.Div(
-        className="p-24",
+        className="p-24 w-full h-full flex flex-col",
         children=[
             html.H1(
                 title,
                 className="flex-auto text-3xl font-semibold text-yellow-400 p-2",
             ),
             create_description_component(scorecard_metadata),
             html.Div(
@@ -167,11 +177,11 @@
         if len(component.inputs) > 0 or len(component.global_input_ids) > 0:
             app.callback(
                 Output(component.id, "figure"),
                 [Input(input_.id, input_.value_name) for input_ in component.inputs]
                 + [Input(input_id, "value") for input_id in component.global_input_ids],
             )(component.get_figure)
 
-    if is_notebook():
-        app.run(mode="inline", debug=False, threaded=True)
+    if isnotebook:
+        app.run_server(mode="inline", debug=True, threaded=True)
     else:
-        app.run(debug=False, threaded=True)
+        app.run(debug=True, threaded=True)
```

### Comparing `krisi-0.1.2/src/krisi/report/pdf.py` & `krisi-0.1.3/src/krisi/report/pdf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 from typing import TYPE_CHECKING, Dict, List
 
+from krisi.utils.io import ensure_path
+
 if TYPE_CHECKING:
     import plotly.graph_objects as go
 
 from pathlib import Path
 
-from krisi.report.type import InteractiveFigure, PathConst
+from krisi.report.type import InteractiveFigure
 
 
 def __figure_to_html(figure: "go.Figure") -> str:
     import base64
 
-    image = str(base64.b64encode(figure.to_image(format="png", scale=5)))[2:-1]
+    image = str(base64.b64encode(figure.to_image(format="svg")))[2:-1]
     return f'<img style="max-width:100%; max-height:100%;" src="data:image/png;base64,{image}"/>'
 
 
+def convert_figure_to_html(figure: "go.Figure") -> str:
+    return "<br>" + __figure_to_html(figure)
+
+
+def convert_figures_to_html(figures: List["go.Figure"]) -> str:
+    return "<br>".join([__figure_to_html(figure) for figure in figures])
+
+
+def convert_figures_to_side_by_side_html(figures: List["go.Figure"]) -> str:
+    return (
+        '<div class="flex flex-row">'
+        + "".join([f"<div>{__figure_to_html(figure)}</div>" for figure in figures])
+        + "</div>"
+    )
+
+
 def __create_html_report(
     template_file: Path, html_elements_to_inject: Dict[str, str]
 ) -> str:
     import pkgutil
 
     template_html = pkgutil.get_data(__name__, str(template_file))
     template_html = template_html.decode()
@@ -27,40 +45,43 @@
         template_html = template_html.replace(f"{{ {key} }}", value)
     return template_html
 
 
 def __convert_html_to_pdf(
     source_html: Path, output_path: Path, report_name: str, css_template_url: Path
 ) -> None:
-    import os
-    import pkgutil
+    pass
 
-    from weasyprint import CSS, HTML
+    # import pkgutil
+    import logging
 
-    if not os.path.exists(output_path):
-        os.makedirs(output_path)
+    from weasyprint import CSS, HTML
 
-    css_string = pkgutil.get_data(__name__, str(css_template_url))
-    css_string = css_string.decode()
+    logging.getLogger("weasyprint").setLevel(100)
 
-    css = CSS(string=css_string)
-    pdf = HTML(string=source_html).write_pdf(stylesheets=[css])
+    ensure_path(output_path)
 
-    open(f"{output_path}/{report_name}", "wb").write(pdf)
+    # css_string = pkgutil.get_data(__name__, str(css_template_url))
+    # css_string = css_string.decode()
 
+    # css = CSS(string=css_string)
+    pdf = HTML(string=source_html).write_pdf(
+        stylesheets=[
+            CSS("https://cdn.jsdelivr.net/npm/tailwindcss/dist/tailwind.min.css")
+        ]
+    )
 
-def convert_figures_to_html(figures: List["go.Figure"]) -> str:
-    return "<br>".join([__figure_to_html(figure) for figure in figures])
+    open(f"{output_path}/{report_name}", "wb").write(pdf)
 
 
 def create_pdf_report(
-    path: Path = PathConst.default_save_path,
-    title: str = "Time Series Report",
-    html_template_url: Path = PathConst.html_template_url,
-    css_template_url: Path = PathConst.css_template_url,
+    path: Path,
+    title: str,
+    html_template_url: Path,
+    css_template_url: Path,
     html_elements_to_inject: Dict[str, str] = dict(),
 ):
     html_elements_to_inject["title"] = title
     report_html = __create_html_report(html_template_url, html_elements_to_inject)
     __convert_html_to_pdf(report_html, path, f"{title}.pdf", css_template_url)
 
 
@@ -71,11 +92,11 @@
         residuals_display_acf_plot=(750.0, 750.0),
         residuals_display_density_plot=(350.0, 350.0),
         residuals_display_time_series=(1500.0, 750.0),
     )
 
     for key, value in size_dict.items():
         if key in diagram_dict.keys():
-            diagram_dict[key].width = value[0]
+            # diagram_dict[key].width = value[0]
             diagram_dict[key].height = value[1]
 
     return diagram_dict
```

### Comparing `krisi-0.1.2/src/krisi/report/type.py` & `krisi-0.1.3/src/krisi/report/type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import dataclass, field
 from enum import Enum
-from pathlib import Path
-from typing import TYPE_CHECKING, Callable, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 import pandas as pd
 from typing_extensions import Literal
 
 if TYPE_CHECKING:
     import plotly.graph_objects as go
 
@@ -34,33 +33,40 @@
     get_figure: Callable
     inputs: List[PlotlyInput] = field(default_factory=list)
     global_input_ids: List[str] = field(default_factory=list)
     title: Optional[str] = ""
     width: Optional[float] = 900.0
     height: Optional[float] = 600.0
     category: Optional[MetricCategories] = None
+    plot_args: Dict[str, Any] = field(default_factory=dict)
 
 
 class DisplayModes(Enum):
     interactive = "interactive"
     pdf = "pdf"
     direct = "direct"
+    direct_save = "direct_save"
+    direct_one_subplot = "direct_one_subplot"
 
-
-class PathConst:
-    default_save_path: Path = Path("output/report/")
-    html_template_url: Path = Path("libary/default/template.html")
-    css_template_url: Path = Path("libary/default/template.css")
+    @staticmethod
+    def from_str(value: Union[str, "DisplayModes"]) -> "DisplayModes":
+        if isinstance(value, DisplayModes):
+            return value
+        for strategy in DisplayModes:
+            if strategy.value == value:
+                return strategy
+        else:
+            raise ValueError(f"Unknown DisplayModes: {value}")
 
 
 def plotly_interactive(
     plot_function: PlotFunction,
     data_source: Union[pd.DataFrame, pd.Series],
     *args,
-    **kwargs
+    **kwargs,
 ) -> Callable:
     # default_args = args
     default_kwargs = kwargs
 
     def wrapper(*args, **kwargs) -> "go.Figure":
         width = kwargs.pop("width", None)
         height = kwargs.pop("height", None)
```

### Comparing `krisi-0.1.2/src/krisi/report/vizualise.py` & `krisi-0.1.3/src/krisi/report/vizualise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import pkgutil
 from enum import Enum
-from typing import List, Optional, Union
+from typing import TYPE_CHECKING, List, Optional, Union
 
 import pandas as pd
 
+from krisi.report.type import InteractiveFigure
 from krisi.utils.iterable_helpers import wrap_in_list
 
+if TYPE_CHECKING:
+    import plotly.graph_objects as go
+
 
 class VizualisationMethod(Enum):
     overlap = "overlap"
     seperate = "seperate"
 
     @staticmethod
     def from_str(value: Union[str, "VizualisationMethod"]) -> "VizualisationMethod":
@@ -98,50 +102,50 @@
             line_color=plt.colors.DEFAULT_PLOTLY_COLORS[i],
         )
         for i, column in enumerate(df.columns)
     ]
 
     if y_separate:
         y_trace.showlegend = False
-        fig.append_trace(
+        fig.add_trace(
             y_trace,
             row=1,
             col=1,
         )
 
     for mode in modes:
         if mode == VizualisationMethod.seperate:
             for i, column in enumerate(df.columns):
-                fig.append_trace(
+                fig.add_trace(
                     traces[i],
                     row=i + (2 if y_separate else 1),
                     col=1,
                 )
                 if not y_separate:
                     if i == 0:
                         y_trace.showlegend = True
                     else:
                         y_trace.showlegend = False
-                    fig.append_trace(
+                    fig.add_trace(
                         y_trace,
                         row=i + 1,
                         col=1,
                     )
 
         if mode == VizualisationMethod.overlap:
             if not y_separate:
                 if num_plots == 1:
                     y_trace.showlegend = True
-                fig.append_trace(
+                fig.add_trace(
                     y_trace,
                     row=num_plots,
                     col=1,
                 )
             for i, column in enumerate(df.columns):
-                fig.append_trace(
+                fig.add_trace(
                     traces[i],
                     row=num_plots,
                     col=1,
                 )
 
     for row in range(num_plots):
         fig.update_xaxes(title_text=x_name, row=row + 1, col=1)
@@ -189,7 +193,30 @@
             joint_plot_name=joint_plot_name,
             target_plot_name=target_plot_name,
         )
     else:
         raise AssertionError(
             "`Plotly` is not installed. Install Plotly by running `pip install plotly` or unlock all reporting capability by `pip install krisi[plotting]`."
         )
+
+
+def create_subplots_from_mutiple_plots(
+    interactive_figures: List[InteractiveFigure], title: str
+) -> "go.Figure":
+    from plotly.subplots import make_subplots
+
+    figures = [figure.get_figure(**figure.plot_args) for figure in interactive_figures]
+
+    fig = make_subplots(
+        rows=len(figures),
+        cols=1,
+        subplot_titles=[figure.title for figure in interactive_figures],
+        row_heights=[500 for _ in range(len(figures))],
+        specs=[[{"type": fig_.data[0].type}] for fig_ in figures],
+    )
+
+    for i, figure in enumerate(figures):
+        fig.add_trace(figure.data[0], row=1 + i, col=1)
+
+    fig.update_layout(height=500 * len(figures), title_text=title)
+
+    return fig
```

### Comparing `krisi-0.1.2/src/krisi/report/library/console/diagrams.py` & `krisi-0.1.3/src/krisi/report/library/console/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/report/library/pdf_layouts/scorecard/report.css` & `krisi-0.1.3/src/krisi/report/library/pdf_layouts/scorecard/report.css`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/utils/console_plot.py` & `krisi-0.1.3/src/krisi/utils/console_plot.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/utils/data.py` & `krisi-0.1.3/src/krisi/utils/data.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/utils/environment.py` & `krisi-0.1.3/src/krisi/utils/environment.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/utils/io.py` & `krisi-0.1.3/src/krisi/utils/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,18 +69,33 @@
 ) -> List["ScoreCard"]:
     import os
     import pickle
 
     if isinstance(path, str):
         path = Path(path)
 
-    path = Path(os.path.join(path, Path(f"{project_name}")))
-    files = os.listdir(path)
+    path = Path(os.path.join(path, Path(f"{project_name}/scorecards")))
+    project_files = os.listdir(path)
+
+    scorecard_dirs = [
+        directory
+        for directory in project_files
+        if os.path.isdir(os.path.join(path, directory))
+    ]
 
     loaded_scorecards = []
-    for file in files:
-        with open(
-            Path(os.path.join(path, Path(f"{file}/scorecard.pickle"))), "rb"
-        ) as f:
-            loaded_scorecards.append(pickle.load(f))
+    for scorecard_dir in scorecard_dirs:
+        files = os.listdir(os.path.join(path, scorecard_dir))
+        for file in files:
+            if file.split(".")[-1] != "pickle":
+                continue
+            with open(
+                Path(os.path.join(path, Path(f"{scorecard_dir}/{file}"))), "rb"
+            ) as f:
+                loaded_scorecards.append(pickle.load(f))
 
     return loaded_scorecards
+
+
+def ensure_path(path: Union[str, Path]) -> None:
+    if not os.path.exists(path):
+        os.makedirs(path)
```

### Comparing `krisi-0.1.2/src/krisi/utils/iterable_helpers.py` & `krisi-0.1.3/src/krisi/utils/iterable_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,7 +101,11 @@
 
 
 T = TypeVar("T")
 
 
 def wrap_in_list(input: Union[T, List[T]]) -> List[T]:
     return input if isinstance(input, List) else [input]
+
+
+def replace_if_None(input: Any, replacement: Any) -> Any:
+    return replacement if input is None else input
```

### Comparing `krisi-0.1.2/src/krisi/utils/printing.py` & `krisi-0.1.3/src/krisi/utils/printing.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/src/krisi/utils/devutils/timing.py` & `krisi-0.1.3/src/krisi/utils/devutils/timing.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/.gitignore` & `krisi-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/LICENSE` & `krisi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/README.md` & `krisi-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `krisi-0.1.2/pyproject.toml` & `krisi-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krisi"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Mark Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 description = "Testing and Reporting framework for Time Series Analysis"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -135,15 +135,15 @@
   "src",
   ".",
 ]
 testpaths = ["tests"] 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `krisi-0.1.2/PKG-INFO` & `krisi-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krisi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Testing and Reporting framework for Time Series Analysis
 Project-URL: Documentation, https://dream-faster.github.io/krisi
 Project-URL: Issues, https://github.com/dream-faster/krisi/issues
 Project-URL: Source, https://github.com/dream-faster/krisi
 Author-email: Mark Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
```

