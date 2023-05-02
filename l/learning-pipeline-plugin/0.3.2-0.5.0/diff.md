# Comparing `tmp/learning_pipeline_plugin-0.3.2.tar.gz` & `tmp/learning_pipeline_plugin-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learning_pipeline_plugin-0.3.2.tar", max compression
+gzip compressed data, was "learning_pipeline_plugin-0.5.0.tar", max compression
```

## Comparing `learning_pipeline_plugin-0.3.2.tar` & `learning_pipeline_plugin-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2538 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/README.md
--rw-r--r--   0        0        0      164 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/__init__.py
--rw-r--r--   0        0        0     2242 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/actfw_utils.py
--rw-r--r--   0        0        0       90 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/__init__.py
--rw-r--r--   0        0        0     5857 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/stream_al.py
--rw-r--r--   0        0        0    10929 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/submodular_diversity.py
--rw-r--r--   0        0        0     2405 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/submodular_utils.py
--rw-r--r--   0        0        0      802 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/type_helper.py
--rw-r--r--   0        0        0     2250 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/uncertainty.py
--rw-r--r--   0        0        0     3006 2023-03-02 06:00:36.919585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/collect_pipe.py
--rw-r--r--   0        0        0      881 2023-03-02 06:00:36.923585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/notifier.py
--rw-r--r--   0        0        0     3986 2023-03-02 06:00:36.923585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/select_task.py
--rw-r--r--   0        0        0     7007 2023-03-02 06:00:36.923585 learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/sender_task.py
--rw-r--r--   0        0        0      671 2023-03-02 06:00:36.923585 learning_pipeline_plugin-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3177 1970-01-01 00:00:00.000000 learning_pipeline_plugin-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2538 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/README.md
+-rw-r--r--   0        0        0      164 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/__init__.py
+-rw-r--r--   0        0        0     2242 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/actfw_utils.py
+-rw-r--r--   0        0        0       90 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/__init__.py
+-rw-r--r--   0        0        0     5857 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/stream_al.py
+-rw-r--r--   0        0        0    10929 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/submodular_diversity.py
+-rw-r--r--   0        0        0     2405 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/submodular_utils.py
+-rw-r--r--   0        0        0      802 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/type_helper.py
+-rw-r--r--   0        0        0     2250 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/uncertainty.py
+-rw-r--r--   0        0        0     3118 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/collect_pipe.py
+-rw-r--r--   0        0        0      881 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/notifier.py
+-rw-r--r--   0        0        0     3986 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/select_task.py
+-rw-r--r--   0        0        0     7764 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/sender_task.py
+-rw-r--r--   0        0        0      707 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 learning_pipeline_plugin-0.5.0/PKG-INFO
```

### Comparing `learning_pipeline_plugin-0.3.2/README.md` & `learning_pipeline_plugin-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/actfw_utils.py` & `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/actfw_utils.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/stream_al.py` & `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/stream_al.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/submodular_diversity.py` & `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/submodular_diversity.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/submodular_utils.py` & `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/submodular_utils.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/type_helper.py` & `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/type_helper.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/algorithms/uncertainty.py` & `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/uncertainty.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/collect_pipe.py` & `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/collect_pipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,32 +18,35 @@
         app: Application,
         sender_task: AbstractSenderTask,
         uncertainty: AbstractUncertainty,
         collect_frequency: int,
         batch_size: int,
         sspp_eps: float = 0.05,
         uncertainty_rate_lambda: float = 0.91,
-        notifier: AbstractNotifier = Notifier(),
+        notifier: Optional[AbstractNotifier] = None
     ):
         """CollectPipeBase sends the selected image to the API Server.
         - app(Application): instance of actfw_core.Application
         - sender_task(AbstractSenderTask): instance of SenderTask
         - uncertainty(AbstractUncertainty): function to evaluate the uncertainty of an image
         - collect_frequency(int): frequency of sending data to the server. Unit is minutes.
         - batch_size(int): parameter for how many images to collect per send.
         - sspp_eps(float): trade-off parameter between accuracy and computational complexity.
                         The smaller the parameter, the higher the accuracy, but the increased computational complexity.
         - uncertainty_rate_lambda(float): weighting parameter to balance uncertainty/diversity
                         (diversity only if 0, uncertainty only if 1)
         - notifier(AbstractNotifier): message formatter to notify sending success/failure to Actcast
         """
         super().__init__()
-        self.notifier = notifier
+        if notifier is None:
+            self.notifier: AbstractNotifier = Notifier()
+        else:
+            self.notifier = notifier
 
-        sender_task.set_notifier(notifier)
+        sender_task.set_notifier(self.notifier)
         app.register_task(sender_task)
 
         self.select_task = SelectTask(
             uncertainty,
             sspp_eps,
             batch_size,
             sender_task,
```

### Comparing `learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/notifier.py` & `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/notifier.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.3.2/learning_pipeline_plugin/select_task.py` & `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/select_task.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.3.2/PKG-INFO` & `learning_pipeline_plugin-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: learning-pipeline-plugin
-Version: 0.3.2
+Version: 0.5.0
 Summary: 
 Home-page: https://github.com/Idein/learning-pipeline-plugin
 License: MIT
 Author: Idein Inc.
 Requires-Python: >=3.7.0,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: actfw-core (>=2.2.0,<3.0.0)
 Requires-Dist: numpy (>=1,<2)
+Requires-Dist: pillow (<6)
 Requires-Dist: requests[socks] (>=2.28.1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Repository, https://github.com/Idein/learning-pipeline-plugin
 Description-Content-Type: text/markdown
 
 # learning-pipeline-plugin
```

