# Comparing `tmp/fold_core-0.1.7.tar.gz` & `tmp/fold_core-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fold_core-0.1.7.tar", max compression
+gzip compressed data, was "fold_core-0.1.8.tar", max compression
```

## Comparing `fold_core-0.1.7.tar` & `fold_core-0.1.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3870 2023-05-02 13:09:22.050625 fold_core-0.1.7/LICENSE
--rw-r--r--   0        0        0    10102 2023-05-02 13:09:22.050625 fold_core-0.1.7/README.md
--rw-r--r--   0        0        0     3820 2023-05-02 13:09:22.086625 fold_core-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      474 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/__init__.py
--rw-r--r--   0        0        0     6200 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/base.py
--rw-r--r--   0        0        0      570 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/__init__.py
--rw-r--r--   0        0        0    10261 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/columns.py
--rw-r--r--   0        0        0     1577 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/common.py
--rw-r--r--   0        0        0     6272 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/concat.py
--rw-r--r--   0        0        0     2226 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6384 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     2857 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/optimize.py
--rw-r--r--   0        0        0     4785 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/residual.py
--rw-r--r--   0        0        0     3261 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/sample.py
--rw-r--r--   0        0        0     2231 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/select.py
--rw-r--r--   0        0        0     4632 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/composites/target.py
--rw-r--r--   0        0        0      345 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/__init__.py
--rw-r--r--   0        0        0      975 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     1687 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1439 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0     3198 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/backtesting.py
--rw-r--r--   0        0        0     1264 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/checks.py
--rw-r--r--   0        0        0    11552 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/common.py
--rw-r--r--   0        0        0     7138 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/encase.py
--rw-r--r--   0        0        0     2886 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/global.py
--rw-r--r--   0        0        0      852 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/inference.py
--rw-r--r--   0        0        0     2993 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/memory.py
--rw-r--r--   0        0        0     6387 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/training.py
--rw-r--r--   0        0        0     1845 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/types.py
--rw-r--r--   0        0        0      756 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/update.py
--rw-r--r--   0        0        0     2243 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/loop/wrap.py
--rw-r--r--   0        0        0      381 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/__init__.py
--rw-r--r--   0        0        0     3219 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/base.py
--rw-r--r--   0        0        0     1926 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/baseline.py
--rw-r--r--   0        0        0     4349 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/dummy.py
--rw-r--r--   0        0        0     2187 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/random.py
--rw-r--r--   0        0        0     5169 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/models/sklearn.py
--rw-r--r--   0        0        0        0 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/py.typed
--rw-r--r--   0        0        0     6724 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/splitters.py
--rw-r--r--   0        0        0     1003 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/__init__.py
--rw-r--r--   0        0        0     6034 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/columns.py
--rw-r--r--   0        0        0     8593 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/date.py
--rw-r--r--   0        0        0     4775 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/dev.py
--rw-r--r--   0        0        0     5393 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/difference.py
--rw-r--r--   0        0        0      798 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/function.py
--rw-r--r--   0        0        0     6569 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/holidays.py
--rw-r--r--   0        0        0     6557 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/lags.py
--rw-r--r--   0        0        0     8858 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/math.py
--rw-r--r--   0        0        0     3836 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/scaling.py
--rw-r--r--   0        0        0     4808 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      887 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/update.py
--rw-r--r--   0        0        0     4414 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/transformations/window.py
--rw-r--r--   0        0        0     2216 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/checks.py
--rw-r--r--   0        0        0      638 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/dataframe.py
--rw-r--r--   0        0        0     2240 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/dataset.py
--rw-r--r--   0        0        0     1591 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/list.py
--rw-r--r--   0        0        0     4496 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/tests.py
--rw-r--r--   0        0        0     1716 2023-05-02 13:09:22.086625 fold_core-0.1.7/src/fold/utils/trim.py
--rw-r--r--   0        0        0    12899 1970-01-01 00:00:00.000000 fold_core-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3870 2023-05-03 13:32:34.739451 fold_core-0.1.8/LICENSE
+-rw-r--r--   0        0        0    10102 2023-05-03 13:32:34.739451 fold_core-0.1.8/README.md
+-rw-r--r--   0        0        0     3957 2023-05-03 13:32:34.771452 fold_core-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/__init__.py
+-rw-r--r--   0        0        0     6351 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/base.py
+-rw-r--r--   0        0        0      570 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10456 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/columns.py
+-rw-r--r--   0        0        0     1577 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/common.py
+-rw-r--r--   0        0        0     6402 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/concat.py
+-rw-r--r--   0        0        0     2291 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6449 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     3419 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/optimize.py
+-rw-r--r--   0        0        0     4850 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/residual.py
+-rw-r--r--   0        0        0     3326 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/sample.py
+-rw-r--r--   0        0        0     2231 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/select.py
+-rw-r--r--   0        0        0     5056 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/target.py
+-rw-r--r--   0        0        0      345 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/__init__.py
+-rw-r--r--   0        0        0      975 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     1687 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1439 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0     3198 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/backtesting.py
+-rw-r--r--   0        0        0     1264 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/checks.py
+-rw-r--r--   0        0        0    11691 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/common.py
+-rw-r--r--   0        0        0     7138 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/encase.py
+-rw-r--r--   0        0        0     2886 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/global.py
+-rw-r--r--   0        0        0      852 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/inference.py
+-rw-r--r--   0        0        0     2993 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/memory.py
+-rw-r--r--   0        0        0     6387 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/training.py
+-rw-r--r--   0        0        0     1845 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/types.py
+-rw-r--r--   0        0        0      756 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/update.py
+-rw-r--r--   0        0        0     2243 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/wrap.py
+-rw-r--r--   0        0        0      381 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/__init__.py
+-rw-r--r--   0        0        0     3219 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/base.py
+-rw-r--r--   0        0        0     1926 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/baseline.py
+-rw-r--r--   0        0        0     4349 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/dummy.py
+-rw-r--r--   0        0        0     2187 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/random.py
+-rw-r--r--   0        0        0     5346 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/sklearn.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/py.typed
+-rw-r--r--   0        0        0     6724 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/splitters.py
+-rw-r--r--   0        0        0     1003 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     6213 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8689 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/date.py
+-rw-r--r--   0        0        0     4879 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/dev.py
+-rw-r--r--   0        0        0     5479 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/difference.py
+-rw-r--r--   0        0        0      798 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/function.py
+-rw-r--r--   0        0        0     6765 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     5866 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/lags.py
+-rw-r--r--   0        0        0     8447 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/math.py
+-rw-r--r--   0        0        0     3836 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/scaling.py
+-rw-r--r--   0        0        0     5013 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      887 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/update.py
+-rw-r--r--   0        0        0     4530 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/window.py
+-rw-r--r--   0        0        0     2216 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/checks.py
+-rw-r--r--   0        0        0      638 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/dataframe.py
+-rw-r--r--   0        0        0     2240 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/dataset.py
+-rw-r--r--   0        0        0     1591 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/list.py
+-rw-r--r--   0        0        0     4783 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/tests.py
+-rw-r--r--   0        0        0     1716 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/trim.py
+-rw-r--r--   0        0        0    12990 1970-01-01 00:00:00.000000 fold_core-0.1.8/PKG-INFO
```

### Comparing `fold_core-0.1.7/LICENSE` & `fold_core-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/README.md` & `fold_core-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/pyproject.toml` & `fold_core-0.1.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fold-core"
 packages = [
     { include="fold", from="./src" },
 ]
-version = "0.1.7"
+version = "0.1.8"
 authors = ["Mark Aron Szulyovszky", "Daniel Szemerey" ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -50,14 +50,16 @@
 mkdocs-include-markdown-plugin = {version = ">=4.0", optional = true}
 mkdocs-autorefs = {version = ">=0.4", optional = true}
 mkdocs-jupyter = {version = ">=0.22", optional = true}
 image = {version = ">=1.5.33", optional = true}
 mkdocs-gallery = {version = ">=0.7", optional = true}
 mkdocs-glightbox = {version = "<=0.3.2", optional = true}
 ray = {version = ">=1.4", optional = true}
+fold-models = {version = "~=0.1.2", optional = true}
+fold-wrappers = {version = "~=0.1", optional = true}
 
 [project.urls]
 Documentation = "https://dream-faster.github.io/fold"
 Issues = "https://github.com/dream-faster/fold/issues"
 Source = "https://github.com/dream-faster/fold"
 
 [tool.poetry.extras]
@@ -80,18 +82,20 @@
   "mkdocs-autorefs",
   "mkdocs-jupyter",
   "image",
   "mkdocs-gallery",
   "mkdocs-glightbox"
 ]
 ray = ["ray"]
-extras = [
+all = [
   "ray",
   "holidays",
   "krisi",
+  "fold-core",
+  "fold-wrappers",
 ]
 
 [tool.hatch.envs.quality]
 dependencies = [
   ".[quality]"
 ]
 detached = true
@@ -124,15 +128,15 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.7"
+current_version = "0.1.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_core-0.1.7/src/fold/base.py` & `fold_core-0.1.8/src/fold/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,17 +172,19 @@
 
 
 class Tunable(ABC):
     @abstractmethod
     def get_params(self) -> dict:
         raise NotImplementedError
 
-    @abstractmethod
-    def set_params(self, **parameters):
-        raise NotImplementedError
+    def clone_with_params(self, **parameters) -> Tunable:
+        """
+        The default implementation only works for Transformations, when parameters and the init parameters match 100%.
+        """
+        return self.__class__(**parameters)
 
 
 class FeatureSelector(Transformation):
     selected_features: List[str]
 
 
 Transformations = Union[
```

### Comparing `fold_core-0.1.7/src/fold/composites/__init__.py` & `fold_core-0.1.8/src/fold/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/composites/columns.py` & `fold_core-0.1.8/src/fold/composites/columns.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,18 +68,20 @@
     ) -> pd.DataFrame:
         return postprocess_results(results, self.name)
 
     def get_child_transformations_primary(self) -> Pipelines:
         return self.pipelines
 
     def clone(self, clone_child_transformations: Callable) -> EnsembleEachColumn:
-        return EnsembleEachColumn.from_cloned_instance(
+        clone = EnsembleEachColumn.from_cloned_instance(
             pipeline=clone_child_transformations(self.pipelines),
             pipelines_already_cloned=self.pipelines_already_cloned,
         )
+        clone.properties = self.properties
+        return clone
 
 
 class TransformEachColumn(Composite):
     """
     Apply a single pipeline to each column, separately.
 
     Parameters
@@ -145,18 +147,20 @@
     ) -> pd.DataFrame:
         return pd.concat(results, axis="columns")
 
     def get_child_transformations_primary(self) -> Pipelines:
         return self.pipeline
 
     def clone(self, clone_child_transformations: Callable) -> TransformEachColumn:
-        return TransformEachColumn.from_cloned_instance(
+        clone = TransformEachColumn.from_cloned_instance(
             pipeline=clone_child_transformations(self.pipeline),
             pipeline_already_cloned=self.pipeline_already_cloned,
         )
+        clone.properties = self.properties
+        return clone
 
 
 class SkipNA(Composite):
     """
     Skips rows with NaN values in the input data.
     In the output, rows with NaNs are returned as is, all other rows transformed.
 
@@ -207,17 +211,19 @@
         results = [result.reindex(self.original_index) for result in results]
         return pd.concat(results, axis="columns")
 
     def get_child_transformations_primary(self) -> Pipelines:
         return self.pipeline
 
     def clone(self, clone_child_transformations: Callable) -> SkipNA:
-        return SkipNA(
+        clone = SkipNA(
             pipeline=clone_child_transformations(self.pipeline),
         )
+        clone.properties = self.properties
+        return clone
 
 
 def postprocess_results(
     results: List[pd.DataFrame],
     name: str,
 ) -> pd.DataFrame:
     if all_have_probabilities(results):
```

### Comparing `fold_core-0.1.7/src/fold/composites/common.py` & `fold_core-0.1.8/src/fold/composites/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/composites/concat.py` & `fold_core-0.1.8/src/fold/composites/concat.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,18 +122,20 @@
         else:
             return pd.concat(results, axis="columns")
 
     def get_child_transformations_primary(self) -> Pipelines:
         return self.pipelines
 
     def clone(self, clone_child_transformations: Callable) -> Concat:
-        return Concat(
+        clone = Concat(
             pipelines=clone_child_transformations(self.pipelines),
             if_duplicate_keep=self.if_duplicate_keep,
         )
+        clone.properties = self.properties
+        return clone
 
 
 class Pipeline(Composite):
     """
     An optional wrappers that is equivalent to using a single array for the transformations.
     It executes the transformations sequentially, in the order they are provided.
 
@@ -159,15 +161,17 @@
     ) -> pd.DataFrame:
         return results[0]
 
     def get_child_transformations_primary(self) -> Pipelines:
         return self.pipeline
 
     def clone(self, clone_child_transformations: Callable) -> Pipeline:
-        return Pipeline(pipeline=clone_child_transformations(self.pipeline))
+        clone = Pipeline(pipeline=clone_child_transformations(self.pipeline))
+        clone.properties = self.properties
+        return clone
 
 
 def TransformColumn(
     columns: Union[List[str], str], pipeline: Transformations
 ) -> Composite:
     """
     Transforms a single or multiple columns using the given pipeline.
```

### Comparing `fold_core-0.1.7/src/fold/composites/ensemble.py` & `fold_core-0.1.8/src/fold/composites/ensemble.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,10 +56,12 @@
     ) -> pd.DataFrame:
         return postprocess_results(results, self.name)
 
     def get_child_transformations_primary(self) -> Pipelines:
         return self.pipelines
 
     def clone(self, clone_child_transformations: Callable) -> Ensemble:
-        return Ensemble(
+        clone = Ensemble(
             pipelines=clone_child_transformations(self.pipelines),
         )
+        clone.properties = self.properties
+        return clone
```

### Comparing `fold_core-0.1.7/src/fold/composites/metalabeling.py` & `fold_core-0.1.8/src/fold/composites/metalabeling.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,20 +153,22 @@
 
     def get_child_transformations_secondary(
         self,
     ) -> Optional[Pipelines]:
         return self.meta
 
     def clone(self, clone_child_transformations: Callable) -> MetaLabeling:
-        return MetaLabeling(
+        clone = MetaLabeling(
             primary=clone_child_transformations(self.primary),
             meta=clone_child_transformations(self.meta),
             positive_class=self.positive_class,
             primary_output_included=self.primary_output_included,
         )
+        clone.properties = self.properties
+        return clone
 
 
 def get_int_class(input: str) -> int:
     if input.endswith(".0"):
         return int(float(input[:-2]))
     elif input == "True":
         return 1
```

### Comparing `fold_core-0.1.7/src/fold/composites/optimize.py` & `fold_core-0.1.8/src/fold/composites/optimize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from __future__ import annotations
 
-from copy import deepcopy
 from typing import Callable, Iterable, List, Optional
 
 import pandas as pd
 from sklearn.model_selection import ParameterGrid
 
 from fold.utils.list import wrap_in_list
 
-from ..base import Composite, Optimizer, Tunable
+from ..base import Optimizer, Tunable
 from .common import get_concatenated_names
 
 
 class OptimizeGridSearch(Optimizer):
-    properties = Composite.Properties(primary_requires_predictions=True)
-    selected_params: Optional[dict] = None
+    candidates: Optional[List[Tunable]] = None
+    selected_params_: Optional[dict] = None
+    selected_model_: Optional[Tunable] = None
+    scores_: Optional[List[float]] = None
     param_permutations: List[dict]
 
     def __init__(
         self,
         model: Tunable,
         param_grid: dict,
         scorer: Callable,
@@ -37,47 +38,58 @@
     @classmethod
     def from_cloned_instance(
         cls,
         model: Tunable,
         param_grid: dict,
         scorer: Callable,
         is_scorer_loss: bool,
-        selected_params: Optional[dict],
+        candidates: Optional[List[Tunable]],
+        selected_params_: Optional[dict],
+        selected_model_: Optional[Tunable],
+        scores_: Optional[List[float]],
     ) -> OptimizeGridSearch:
         instance = cls(model, param_grid, scorer, is_scorer_loss)
-        instance.selected_params = selected_params
+        instance.candidates = candidates
+        instance.selected_params_ = selected_params_
+        instance.selected_model_ = selected_model_
+        instance.scores_ = scores_
         return instance
 
     def get_candidates(self) -> Iterable[Tunable]:
-        models = [deepcopy(self.model[0]) for _ in self.param_permutations]
-
-        for model, params in zip(models, self.param_permutations):
-            model.set_params(**params)
-
-        return models
+        if self.candidates is None:
+            self.candidates = [
+                self.model[0].clone_with_params(
+                    **{**self.model[0].get_params(), **params}
+                )
+                for params in self.param_permutations
+            ]
+        return self.candidates
 
     def get_optimized_pipeline(self) -> Optional[Tunable]:
-        if self.selected_params is None:
-            return None
-        self.model[0].set_params(**self.selected_params)
-        return self.model[0]
+        return self.selected_model_
 
     def process_candidate_results(self, results: List[pd.DataFrame], y: pd.Series):
-        if self.selected_params is not None:
+        if self.selected_params_ is not None:
             raise ValueError("Optimizer is already fitted.")
 
-        scores = [self.scorer(y, result) for result in results]
+        scores = [self.scorer(y[-len(result) :], result) for result in results]
         selected_index = (
             scores.index(min(scores))
             if self.is_scorer_loss
             else scores.index(max(scores))
         )
-        self.selected_params = self.param_permutations[selected_index]
+        self.selected_params_ = self.param_permutations[selected_index]
+        self.selected_model_ = self.candidates[selected_index]
+        # TODO: need to store the params for each score as well
+        self.scores_ = scores
 
     def clone(self, clone_child_transformations: Callable) -> OptimizeGridSearch:
         return OptimizeGridSearch.from_cloned_instance(
             model=clone_child_transformations(self.model),
             param_grid=self.param_grid,
             scorer=self.scorer,
             is_scorer_loss=self.is_scorer_loss,
-            selected_params=self.selected_params,
+            candidates=self.candidates,
+            selected_params_=self.selected_params_,
+            selected_model_=self.selected_model_,
+            scores_=self.scores_,
         )
```

### Comparing `fold_core-0.1.7/src/fold/composites/residual.py` & `fold_core-0.1.8/src/fold/composites/residual.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,12 +128,14 @@
 
     def get_child_transformations_secondary(
         self,
     ) -> Optional[Pipelines]:
         return self.meta
 
     def clone(self, clone_child_transformations: Callable) -> ModelResiduals:
-        return ModelResiduals(
+        clone = ModelResiduals(
             primary=clone_child_transformations(self.primary),
             meta=clone_child_transformations(self.meta),
             primary_output_included=self.primary_output_included,
         )
+        clone.properties = self.properties
+        return clone
```

### Comparing `fold_core-0.1.7/src/fold/composites/sample.py` & `fold_core-0.1.8/src/fold/composites/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,11 +84,13 @@
     ) -> pd.DataFrame:
         return results[0]
 
     def get_child_transformations_primary(self) -> Pipelines:
         return self.pipeline
 
     def clone(self, clone_child_transformations: Callable) -> Sample:
-        return Sample(
+        clone = Sample(
             sampler=self.sampler,
             pipeline=clone_child_transformations(self.pipeline),
         )
+        clone.properties = self.properties
+        return clone
```

### Comparing `fold_core-0.1.7/src/fold/composites/select.py` & `fold_core-0.1.8/src/fold/composites/select.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/composites/target.py` & `fold_core-0.1.8/src/fold/composites/target.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 
     Parameters
     ----------
     wrapped_pipeline: Pipeline
         Pipeline, which will be applied to the input data, where the target (`y`) is already transformed.
     y_pipeline: Union[List[InvertibleTransformation], InvertibleTransformation]
         InvertibleTransformations, which will be applied to the target (`y`)
+    invert_wrapped_output: bool, default=True
+        Apply the inverse transformation of `y_pipeline` to the output of `wrapped_pipeline`. default is `True`.
+
 
     Examples
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.composites import ModelResiduals
@@ -56,20 +59,22 @@
         secondary_only_single_pipeline=True,
     )
 
     def __init__(
         self,
         wrapped_pipeline: Pipeline,
         y_pipeline: Union[List[InvertibleTransformation], InvertibleTransformation],
+        invert_wrapped_output: bool = True,
     ) -> None:
         self.wrapped_pipeline = wrap_in_double_list_if_needed(wrapped_pipeline)
         self.y_pipeline = wrap_in_double_list_if_needed(y_pipeline)
         self.name = "TransformTarget-" + get_concatenated_names(
             self.wrapped_pipeline + self.y_pipeline
         )
+        self.invert_wrapped_output = invert_wrapped_output
 
     def preprocess_primary(
         self, X: pd.DataFrame, index: int, y: T, fit: bool
     ) -> Tuple[pd.DataFrame, T]:
         # TransformTarget's primary transformation transforms `y`, not `X`.
         if y is None:
             return (
@@ -97,29 +102,32 @@
     def postprocess_result_secondary(
         self,
         primary_results: List[pd.DataFrame],
         secondary_results: List[pd.DataFrame],
         y: Optional[pd.Series],
         in_sample: bool,
     ) -> pd.DataFrame:
+        if self.invert_wrapped_output is False:
+            return secondary_results[0]
         predictions = get_prediction_column(secondary_results[0])
         for transformation in reversed(self.y_pipeline[0]):
             predictions = transformation.inverse_transform(predictions, in_sample)
-        orignal_results = secondary_results[0]
-        orignal_results[get_prediction_column_name(orignal_results)] = to_series(
-            predictions
-        )
-        return orignal_results
+        results = secondary_results[0]
+        results[get_prediction_column_name(results)] = to_series(predictions)
+        return results
 
     def get_child_transformations_primary(self) -> Pipelines:
         return self.y_pipeline
 
     def get_child_transformations_secondary(
         self,
     ) -> Optional[Pipelines]:
         return self.wrapped_pipeline
 
     def clone(self, clone_child_transformations: Callable) -> TransformTarget:
-        return TransformTarget(
+        clone = TransformTarget(
             wrapped_pipeline=clone_child_transformations(self.wrapped_pipeline),
             y_pipeline=clone_child_transformations(self.y_pipeline),
+            invert_wrapped_output=self.invert_wrapped_output,
         )
+        clone.properties = self.properties
+        return clone
```

### Comparing `fold_core-0.1.7/src/fold/loop/backend/__init__.py` & `fold_core-0.1.8/src/fold/loop/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/backend/ray.py` & `fold_core-0.1.8/src/fold/loop/backend/ray.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/backend/sequential.py` & `fold_core-0.1.8/src/fold/loop/backend/sequential.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/backtesting.py` & `fold_core-0.1.8/src/fold/loop/backtesting.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/checks.py` & `fold_core-0.1.8/src/fold/loop/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/common.py` & `fold_core-0.1.8/src/fold/loop/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import List, Optional
 
 import pandas as pd
 
 from ..base import Composite, Optimizer, Transformation, Transformations
 from ..models.base import Model
 from ..utils.checks import is_prediction, is_X_available
-from ..utils.trim import trim_initial_nans
+from ..utils.trim import trim_initial_nans, trim_initial_nans_single
 from .backend import get_backend_dependent_functions
 from .memory import postprocess_X_y_into_memory, preprocess_X_y_with_memory
 from .types import Backend, Stage
 
 
 def recursively_transform(
     X: pd.DataFrame,
@@ -168,14 +168,17 @@
             X,
             y,
             sample_weights,
             stage,
             backend,
             None,
         )
+        results_primary = [
+            trim_initial_nans_single(result) for result in results_primary
+        ]
         optimizer.process_candidate_results(results_primary, y)
 
     optimized_pipeline = optimizer.get_optimized_pipeline()
     return recursively_transform(
         X, y, sample_weights, optimized_pipeline, stage, backend
     )
```

### Comparing `fold_core-0.1.7/src/fold/loop/encase.py` & `fold_core-0.1.8/src/fold/loop/encase.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/global.py` & `fold_core-0.1.8/src/fold/loop/global.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/inference.py` & `fold_core-0.1.8/src/fold/loop/inference.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/memory.py` & `fold_core-0.1.8/src/fold/loop/memory.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/training.py` & `fold_core-0.1.8/src/fold/loop/training.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/types.py` & `fold_core-0.1.8/src/fold/loop/types.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/update.py` & `fold_core-0.1.8/src/fold/loop/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/loop/wrap.py` & `fold_core-0.1.8/src/fold/loop/wrap.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/models/base.py` & `fold_core-0.1.8/src/fold/models/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/models/baseline.py` & `fold_core-0.1.8/src/fold/models/baseline.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/models/dummy.py` & `fold_core-0.1.8/src/fold/models/dummy.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/models/random.py` & `fold_core-0.1.8/src/fold/models/random.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/models/sklearn.py` & `fold_core-0.1.8/src/fold/models/sklearn.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,16 +66,18 @@
         return pd.concat([predictions, probabilities], axis="columns")
 
     predict_in_sample = predict
 
     def get_params(self) -> dict:
         return self.model.get_params()
 
-    def set_params(self, **params) -> None:
-        self.model.set_params(**params)
+    def clone_with_params(self, **parameters) -> Tunable:
+        return WrapSKLearnClassifier(
+            model_class=self.model.__class__, init_args=parameters
+        )
 
 
 class WrapSKLearnRegressor(Model, Tunable):
     """
     Wraps an SKLearn regressor model.
     There's no need to use it directly, `fold` automatically wraps all sklearn regressors into this class.
     """
@@ -122,16 +124,18 @@
         ).to_frame()
 
     predict_in_sample = predict
 
     def get_params(self) -> dict:
         return self.model.get_params()
 
-    def set_params(self, **params) -> None:
-        self.model.set_params(**params)
+    def clone_with_params(self, **parameters) -> Tunable:
+        return WrapSKLearnRegressor(
+            model_class=self.model.__class__, init_args=parameters
+        )
 
 
 class WrapSKLearnPipeline(Model):
     """
     Wraps an scikit-learn Pipeline.
     It's usage is discouraged, as it's not possible to update an scikit-learn Pipeline with new data.
     Fold has all the primitives that scikit-learn Pipelines provide, just wrap your Transformations into an array.
```

### Comparing `fold_core-0.1.7/src/fold/splitters.py` & `fold_core-0.1.8/src/fold/splitters.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/transformations/__init__.py` & `fold_core-0.1.8/src/fold/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/transformations/columns.py` & `fold_core-0.1.8/src/fold/transformations/columns.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 from __future__ import annotations
 
 from typing import List, Union
 
 import pandas as pd
 
-from ..base import Transformation, fit_noop
+from ..base import Transformation, Tunable, fit_noop
 from ..utils.checks import check_get_columns
 from ..utils.list import wrap_in_list
 
 
-class SelectColumns(Transformation):
+class SelectColumns(Transformation, Tunable):
     """
     Selects a single or multiple columns, drops the rest.
 
     Parameters
     ----------
 
     columns : Union[List[str], str]
@@ -33,16 +33,19 @@
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         return X[self.columns]
 
     fit = fit_noop
     update = fit
 
+    def get_params(self) -> dict:
+        return {"columns": self.columns}
 
-class DropColumns(Transformation):
+
+class DropColumns(Transformation, Tunable):
     """
     Drops a single or multiple columns.
 
     Parameters
     ----------
 
     columns : List[str], str
@@ -58,14 +61,17 @@
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         return X.drop(columns=check_get_columns(self.columns, X))
 
     fit = fit_noop
     update = fit
 
+    def get_params(self) -> dict:
+        return {"columns": self.columns}
+
 
 class RenameColumns(Transformation):
     """
     Renames columns.
 
     Parameters
     ----------
```

### Comparing `fold_core-0.1.7/src/fold/transformations/date.py` & `fold_core-0.1.8/src/fold/transformations/date.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import Callable, List, Union
 
 import pandas as pd
 
-from ..base import SingleFunctionTransformation, Transformation, fit_noop
+from ..base import SingleFunctionTransformation, Transformation, Tunable, fit_noop
 from ..utils.list import wrap_in_list
 
 
 class DateTimeFeature(Enum):
     second = "second"
     minute = "minute"
     hour = "hour"
@@ -32,15 +32,15 @@
         for strategy in DateTimeFeature:
             if strategy.value == value:
                 return strategy
         else:
             raise ValueError(f"Unknown DateTimeFeature: {value}")
 
 
-class AddDateTimeFeatures(Transformation):
+class AddDateTimeFeatures(Transformation, Tunable):
     """
     Adds (potentially multiple) date/time features to the input, as additional columns.
     The name of the new column will be the name of the DateTimeFeature passed in.
     Values are returned as integers, so the 59th minute of the hour will be `59`, and year 2022 will be `2022`.
 
     Parameters
     ----------
@@ -110,14 +110,17 @@
             else:
                 raise ValueError(f"Unsupported feature: {feature}")
         return pd.concat([X, X_datetime], axis="columns")
 
     fit = fit_noop
     update = fit_noop
 
+    def get_params(self) -> dict:
+        return {"features": self.features}
+
 
 class AddSecond(SingleFunctionTransformation):
     """
     Adds "second" features to the input, as an additional column.
 
     Examples
     --------
```

### Comparing `fold_core-0.1.7/src/fold/transformations/dev.py` & `fold_core-0.1.8/src/fold/transformations/dev.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,22 +47,24 @@
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         if self.stop_at_transform:
             breakpoint()
         return X
 
 
-class Identity(Transformation):
+class Identity(InvertibleTransformation):
     properties = Transformation.Properties(requires_X=False)
-
     name = "Identity"
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         return X
 
+    def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
+        return X
+
     fit = fit_noop
     update = fit
 
 
 class Test(InvertibleTransformation):
     properties = InvertibleTransformation.Properties(requires_X=False)
     __test__ = False
```

### Comparing `fold_core-0.1.7/src/fold/transformations/difference.py` & `fold_core-0.1.8/src/fold/transformations/difference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from typing import Optional, Union
 
 import pandas as pd
 
-from ..base import InvertibleTransformation, Transformation
+from ..base import InvertibleTransformation, Transformation, Tunable
 from ..utils.dataframe import to_series
 
 
-class Difference(InvertibleTransformation):
+class Difference(InvertibleTransformation, Tunable):
     """
     Performs differencing.
     Sesonal differencing can be achieved by setting `lag` to the seasonality of the data.
     To achieve second-order differencing, simply chain multiple `Difference` transformations.
 
     Parameters
     ----------
@@ -99,14 +99,17 @@
             return X
         else:
             X = pd.concat([to_series(self.last_values_X), X], axis="index")
             for i in range(self.lag):
                 X.iloc[i :: self.lag] = X.iloc[i :: self.lag].cumsum()
             return X.iloc[self.lag :]
 
+    def get_params(self) -> dict:
+        return {"lag": self.lag}
+
 
 class TakeReturns(Transformation):
     """
     Takes the returns (percentage change between the current and a prior element).
 
     Examples
     --------
```

### Comparing `fold_core-0.1.7/src/fold/transformations/function.py` & `fold_core-0.1.8/src/fold/transformations/function.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/transformations/holidays.py` & `fold_core-0.1.8/src/fold/transformations/holidays.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from datetime import date
 from enum import Enum
 from typing import List, Union
 
 import pandas as pd
 
-from ..base import Transformation, fit_noop
+from ..base import Transformation, Tunable, fit_noop
 from ..utils.list import swap_tuples, wrap_in_list
 
 
 class LabelingMethod(Enum):
     """
     Parameters
     ----------
@@ -44,15 +44,15 @@
         for strategy in LabelingMethod:
             if strategy.value == value:
                 return strategy
         else:
             raise ValueError(f"Unknown HolidayType: {value}")
 
 
-class AddHolidayFeatures(Transformation):
+class AddHolidayFeatures(Transformation, Tunable):
     """
     Adds holiday features for given region(s) as new column(s).
     It uses the pattern "holiday_{country_code}" for naming the columns.
 
 
     Parameters
     ----------
@@ -74,15 +74,15 @@
         country_codes: Union[List[str], str],
         labeling: Union[str, LabelingMethod] = LabelingMethod.weekday_weekend_holiday,
     ) -> None:
         self.country_codes = [
             country_code.upper() for country_code in wrap_in_list(country_codes)
         ]
         self.name = f"AddHolidayFeatures-{self.country_codes}"
-        self.type = LabelingMethod.from_str(labeling)
+        self.labeling = LabelingMethod.from_str(labeling)
         from holidays import country_holidays, list_supported_countries
 
         all_supported_countries = list_supported_countries()
 
         assert all(
             [
                 country_code in all_supported_countries
@@ -107,55 +107,61 @@
                     )
                 )
             )
             for country_code in self.country_codes
         ]
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        if self.type == LabelingMethod.holiday_binary:
+        if self.labeling == LabelingMethod.holiday_binary:
             holidays = _get_holidays(
                 X.index, self.country_codes, self.holiday_to_int_maps, encode=True
             )
             holidays[holidays != 0] = 1
 
             return pd.concat([X, holidays], axis="columns")
-        elif self.type == LabelingMethod.weekday_weekend_holiday:
+        elif self.labeling == LabelingMethod.weekday_weekend_holiday:
             holidays = _get_holidays(
                 X.index, self.country_codes, self.holiday_to_int_maps, encode=True
             )
 
             # All values that are (bigger than 0 or a string) are holidays, but we don't want to differentiate between them
             holidays[holidays != 0] = 2
 
             holidays[holidays == 0] = holidays[holidays == 0].add(
                 _get_weekends(X.index), axis="index"
             )
             return pd.concat([X, holidays], axis="columns")
         elif (
-            self.type == LabelingMethod.weekday_weekend_uniqueholiday
-            or self.type == LabelingMethod.weekday_weekend_uniqueholiday_string
+            self.labeling == LabelingMethod.weekday_weekend_uniqueholiday
+            or self.labeling == LabelingMethod.weekday_weekend_uniqueholiday_string
         ):
             holidays = _get_holidays(
                 X.index,
                 self.country_codes,
                 self.holiday_to_int_maps,
-                encode=self.type == LabelingMethod.weekday_weekend_uniqueholiday,
+                encode=self.labeling == LabelingMethod.weekday_weekend_uniqueholiday,
             )
 
             weekends = _get_weekends(X.index)
             holidays[holidays == 0] = holidays[holidays == 0].add(
                 weekends, axis="index"
             )
             return pd.concat([X, holidays], axis="columns")
         else:
-            raise ValueError(f"Unknown HolidayType: {self.type}")
+            raise ValueError(f"Unknown HolidayType: {self.labeling}")
 
     fit = fit_noop
     update = fit_noop
 
+    def get_params(self) -> dict:
+        return {
+            "country_codes": self.country_codes,
+            "labeling": self.labeling,
+        }
+
 
 def _get_weekends(dates: pd.DatetimeIndex) -> pd.Series:
     return pd.Series((dates.weekday > 4).astype(int), index=dates)
 
 
 def _get_holidays(
     dates: pd.DatetimeIndex,
```

### Comparing `fold_core-0.1.7/src/fold/transformations/lags.py` & `fold_core-0.1.8/src/fold/transformations/lags.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,24 +73,14 @@
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
         return {"lags": self.lags}
 
-    def set_params(self, **parameters):
-        for parameter, value in parameters.items():
-            setattr(self, parameter, value)
-        self.properties = Transformation.Properties(
-            requires_X=False,
-            mode=Transformation.Properties.Mode.online,
-            memory_size=max(self.lags),
-            _internal_supports_minibatch_backtesting=True,
-        )
-
 
 class AddLagsX(Transformation, Tunable):
     """
     Adds past values of `X` for the desired column(s).
 
     Parameters
     ----------
@@ -164,15 +154,7 @@
         return pd.concat([X, X_lagged], axis="columns")
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
         return {"columns_and_lags": self.columns_and_lags}
-
-    def set_params(self, **parameters):
-        for parameter, value in parameters.items():
-            setattr(self, parameter, value)
-        self.properties = Transformation.Properties(
-            requires_X=True,
-            memory_size=max(flatten([l for _, l in self.columns_and_lags])),
-        )
```

### Comparing `fold_core-0.1.7/src/fold/transformations/math.py` & `fold_core-0.1.8/src/fold/transformations/math.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,18 +81,14 @@
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
         return {"base": self.base}
 
-    def set_params(self, **parameters):
-        for parameter, value in parameters.items():
-            setattr(self, parameter, value)
-
 
 class AddConstant(InvertibleTransformation, Tunable):
 
     """
     Adds a constant to the data.
 
     Parameters
@@ -164,18 +160,14 @@
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
         return {"constant": self.constant}
 
-    def set_params(self, **parameters):
-        for parameter, value in parameters.items():
-            setattr(self, parameter, value)
-
 
 class TurnPositive(InvertibleTransformation):
     """
     Adds a constant to the data, varying by column, so that all values are positive.
     It identifies the constant during training, and applies it during inference (and backtesting).
     Therefore there's no guarantee that the data will be positive during inference (and backtesting).
 
@@ -255,11 +247,7 @@
         return X / self.constant
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
         return {"constant": self.constant}
-
-    def set_params(self, **parameters):
-        for parameter, value in parameters.items():
-            setattr(self, parameter, value)
```

### Comparing `fold_core-0.1.7/src/fold/transformations/scaling.py` & `fold_core-0.1.8/src/fold/transformations/scaling.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/transformations/sklearn.py` & `fold_core-0.1.8/src/fold/transformations/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,18 @@
             return self.transformation.transform(X)
         else:
             return pd.DataFrame(self.transformation.transform(X), columns=X.columns)
 
     def get_params(self) -> dict:
         return self.transformation.get_params()
 
-    def set_params(self, **params) -> None:
-        self.transformation.set_params(**params)
+    def clone_with_params(self, **parameters) -> Tunable:
+        return WrapSKLearnTransformation(
+            transformation_class=self.transformation.__class__, init_args=parameters
+        )
 
 
 class WrapInvertibleSKLearnTransformation(
     WrapSKLearnTransformation, InvertibleTransformation
 ):
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         return pd.Series(self.transformation.inverse_transform(X), index=X.index)
@@ -129,11 +131,13 @@
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         return X[self.selected_features]
 
     def get_params(self) -> dict:
         return self.transformation.get_params()
 
-    def set_params(self, **params) -> None:
-        self.transformation.set_params(**params)
+    def clone_with_params(self, **parameters) -> Tunable:
+        return WrapSKLearnFeatureSelector(
+            transformation_class=self.transformation.__class__, init_args=parameters
+        )
 
     update = fit_noop
```

### Comparing `fold_core-0.1.7/src/fold/transformations/update.py` & `fold_core-0.1.8/src/fold/transformations/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/transformations/window.py` & `fold_core-0.1.8/src/fold/transformations/window.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import Callable, List, Tuple, Union
 
 import pandas as pd
 
-from ..base import Transformation, fit_noop
+from ..base import Transformation, Tunable, fit_noop
 from ..utils.list import wrap_in_list
 
 
 class PredefinedFunction(Enum):
     mean = "mean"
     sum = "sum"
     median = "median"
@@ -38,15 +38,15 @@
 
 
 ColumnOrColumns = Union[str, List[str]]
 FunctionOrPredefined = Union[Callable, PredefinedFunction, str]
 ColumnWindowFunction = Tuple[ColumnOrColumns, int, FunctionOrPredefined]
 
 
-class AddWindowFeatures(Transformation):
+class AddWindowFeatures(Transformation, Tunable):
 
     """
     Creates rolling window features on the specified columns.
     Equivalent to adding a new column by running: `df[column].rolling(window).function()`.
 
 
     Parameters
@@ -121,7 +121,10 @@
                     X_function_applied[f"{col}_{window}_{function_name}"] = function(
                         X[col].rolling(window)
                     )
         return pd.concat([X, X_function_applied], axis="columns")
 
     fit = fit_noop
     update = fit
+
+    def get_params(self) -> dict:
+        return {"column_window_func": self.column_window_func}
```

### Comparing `fold_core-0.1.7/src/fold/utils/checks.py` & `fold_core-0.1.8/src/fold/utils/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/utils/dataframe.py` & `fold_core-0.1.8/src/fold/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/utils/dataset.py` & `fold_core-0.1.8/src/fold/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/utils/list.py` & `fold_core-0.1.8/src/fold/utils/list.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/src/fold/utils/tests.py` & `fold_core-0.1.8/src/fold/utils/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     instance: Transformation,
     different_params: dict,
     init_function: Optional[Callable] = None,
     classification: bool = False,
     tolerance: Optional[float] = None,
 ):
     """
-    Used to test the general structure and implementation of get_params() and set_params() methods.
+    Used to test the general structure and implementation of get_params() and clone_with_params() methods.
     the kwargs are used to set the parameters of the transformation, which should be different to the init parameters of the `instance`.
     """
     assert isinstance(instance, Tunable)
 
     params = instance.get_params()
     different_instance = (
         instance.__class__(**different_params)
@@ -128,17 +128,22 @@
         generate_zeros_and_ones(length=500)
         if classification
         else generate_sine_wave_data(length=500)
     )
     splitter = SingleWindowSplitter(train_window=0.5)
     preds_orig, _ = train_backtest(instance, X, y, splitter)
     preds_different, _ = train_backtest(different_instance, X, y, splitter)
-    assert not preds_orig.equals(preds_different)
+    assert not preds_orig.equals(
+        preds_different
+    ), "The output of the two instances with different parameters should be different"
 
-    reconstructed_instance = different_instance
-    reconstructed_instance.set_params(**params)
+    reconstructed_instance = different_instance.clone_with_params(**params)
 
     preds_reconstructed, _ = train_backtest(reconstructed_instance, X, y, splitter)
     if tolerance is None:
-        assert preds_orig.equals(preds_reconstructed)
+        assert preds_orig.equals(
+            preds_reconstructed
+        ), "The output of the two instances with different parameters should be the same"
     else:
-        assert np.isclose(preds_orig, preds_reconstructed, atol=tolerance).all()
+        assert np.isclose(
+            preds_orig, preds_reconstructed, atol=tolerance
+        ).all(), "The output of the two instances with different parameters should be the close"
```

### Comparing `fold_core-0.1.7/src/fold/utils/trim.py` & `fold_core-0.1.8/src/fold/utils/trim.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.7/PKG-INFO` & `fold_core-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
 License: Proprietary
 Keywords: time-series,machine-learning,forecasting,forecast,nowcast,models,time-series-regression,time-series-classification,financial-machine-learning
 Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
@@ -19,41 +19,43 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Provides-Extra: all
 Provides-Extra: docs
-Provides-Extra: extras
 Provides-Extra: quality
 Provides-Extra: ray
 Provides-Extra: tests
 Requires-Dist: black (>=22.12.0,<22.13.0) ; extra == "quality"
 Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality"
-Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "extras"
+Requires-Dist: fold-models (>=0.1.2,<0.2.0)
+Requires-Dist: fold-wrappers (>=0.1,<1.0) ; extra == "all"
+Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "all"
 Requires-Dist: image (>=1.5.33) ; extra == "docs"
 Requires-Dist: imbalanced-learn (>=0.7.0) ; extra == "tests"
 Requires-Dist: isort (>=5.10.1,<5.11.0) ; extra == "quality"
 Requires-Dist: iteration_utilities (>=0.11)
-Requires-Dist: krisi (>=0.0.8,<0.1.0) ; extra == "extras"
+Requires-Dist: krisi (>=0.0.8,<0.1.0) ; extra == "all"
 Requires-Dist: mkdocs (>=1.2)
 Requires-Dist: mkdocs-autorefs (>=0.4) ; extra == "docs"
 Requires-Dist: mkdocs-gallery (>=0.7) ; extra == "docs"
 Requires-Dist: mkdocs-glightbox (<=0.3.2) ; extra == "docs"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs"
 Requires-Dist: mkdocs-jupyter (>=0.22) ; extra == "docs"
 Requires-Dist: mkdocs-material (>=9.0.0) ; extra == "docs"
 Requires-Dist: mkdocstrings-python (>=0.9.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.16)
 Requires-Dist: pandas (>=1.2)
 Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra == "quality"
 Requires-Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests"
 Requires-Dist: pytest-cov (>=4.0) ; extra == "tests"
-Requires-Dist: ray (>=1.4) ; extra == "ray" or extra == "extras"
+Requires-Dist: ray (>=1.4) ; extra == "ray" or extra == "all"
 Requires-Dist: scikit-learn (>=0.22)
 Requires-Dist: tqdm (>=4.0)
 Description-Content-Type: text/markdown
 
 <!-- # fold -->
 
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.1.7 Summary: A Time Series
+Metadata-Version: 2.1 Name: fold-core Version: 0.1.8 Summary: A Time Series
 Cross-Validation library that lets you build, deploy and update composite
 models easily. An order of magnitude speed-up, combined with flexibility and
 rigour. License: Proprietary Keywords: time-series,machine-
 learning,forecasting,forecast,nowcast,models,time-series-regression,time-
 series-classification,financial-machine-learning Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: Other/Proprietary License Classifier: Operating
@@ -12,33 +12,35 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Provides-Extra: docs Provides-Extra: extras Provides-Extra: quality Provides-
+Provides-Extra: all Provides-Extra: docs Provides-Extra: quality Provides-
 Extra: ray Provides-Extra: tests Requires-Dist: black (>=22.12.0,<22.13.0) ;
 extra == "quality" Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality"
-Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "extras"
-Requires-Dist: image (>=1.5.33) ; extra == "docs" Requires-Dist: imbalanced-
-learn (>=0.7.0) ; extra == "tests" Requires-Dist: isort (>=5.10.1,<5.11.0) ;
-extra == "quality" Requires-Dist: iteration_utilities (>=0.11) Requires-Dist:
-krisi (>=0.0.8,<0.1.0) ; extra == "extras" Requires-Dist: mkdocs (>=1.2)
-Requires-Dist: mkdocs-autorefs (>=0.4) ; extra == "docs" Requires-Dist: mkdocs-
-gallery (>=0.7) ; extra == "docs" Requires-Dist: mkdocs-glightbox (<=0.3.2) ;
-extra == "docs" Requires-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra
-== "docs" Requires-Dist: mkdocs-jupyter (>=0.22) ; extra == "docs" Requires-
-Dist: mkdocs-material (>=9.0.0) ; extra == "docs" Requires-Dist: mkdocstrings-
-python (>=0.9.0) ; extra == "docs" Requires-Dist: numpy (>=1.16) Requires-Dist:
-pandas (>=1.2) Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra ==
-"quality" Requires-Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests" Requires-
-Dist: pytest-cov (>=4.0) ; extra == "tests" Requires-Dist: ray (>=1.4) ; extra
-== "ray" or extra == "extras" Requires-Dist: scikit-learn (>=0.22) Requires-
-Dist: tqdm (>=4.0) Description-Content-Type: text/markdown
+Requires-Dist: fold-models (>=0.1.2,<0.2.0) Requires-Dist: fold-wrappers
+(>=0.1,<1.0) ; extra == "all" Requires-Dist: holidays (>=0.10) ; extra ==
+"tests" or extra == "all" Requires-Dist: image (>=1.5.33) ; extra == "docs"
+Requires-Dist: imbalanced-learn (>=0.7.0) ; extra == "tests" Requires-Dist:
+isort (>=5.10.1,<5.11.0) ; extra == "quality" Requires-Dist:
+iteration_utilities (>=0.11) Requires-Dist: krisi (>=0.0.8,<0.1.0) ; extra ==
+"all" Requires-Dist: mkdocs (>=1.2) Requires-Dist: mkdocs-autorefs (>=0.4) ;
+extra == "docs" Requires-Dist: mkdocs-gallery (>=0.7) ; extra == "docs"
+Requires-Dist: mkdocs-glightbox (<=0.3.2) ; extra == "docs" Requires-Dist:
+mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs" Requires-Dist: mkdocs-
+jupyter (>=0.22) ; extra == "docs" Requires-Dist: mkdocs-material (>=9.0.0) ;
+extra == "docs" Requires-Dist: mkdocstrings-python (>=0.9.0) ; extra == "docs"
+Requires-Dist: numpy (>=1.16) Requires-Dist: pandas (>=1.2) Requires-Dist: pre-
+commit (>=2.20.0,<2.21.0) ; extra == "quality" Requires-Dist: pytest
+(>=7.1.2,<7.2.0) ; extra == "tests" Requires-Dist: pytest-cov (>=4.0) ; extra
+== "tests" Requires-Dist: ray (>=1.4) ; extra == "ray" or extra == "all"
+Requires-Dist: scikit-learn (>=0.22) Requires-Dist: tqdm (>=4.0) Description-
+Content-Type: text/markdown
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
                                       ****
                      Fast Adaptive Time Series ML Engine
```

