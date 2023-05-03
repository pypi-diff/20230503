# Comparing `tmp/strangeworks_qaoa-0.1.3.tar.gz` & `tmp/strangeworks_qaoa-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qaoa-0.1.3.tar", max compression
+gzip compressed data, was "strangeworks_qaoa-0.1.4.tar", max compression
```

## Comparing `strangeworks_qaoa-0.1.3.tar` & `strangeworks_qaoa-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-26 15:00:04.025123 strangeworks_qaoa-0.1.3/LICENSE
--rw-r--r--   0        0        0      576 2023-04-26 15:00:04.025123 strangeworks_qaoa-0.1.3/README.md
--rw-r--r--   0        0        0      791 2023-04-26 15:00:22.529517 strangeworks_qaoa-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      128 2023-04-26 15:00:04.029123 strangeworks_qaoa-0.1.3/strangeworks_qaoa/__init__.py
--rw-r--r--   0        0        0    16000 2023-04-26 15:00:04.029123 strangeworks_qaoa-0.1.3/strangeworks_qaoa/sdk.py
--rw-r--r--   0        0        0      691 2023-04-26 15:00:04.029123 strangeworks_qaoa-0.1.3/strangeworks_qaoa/serializer.py
--rw-r--r--   0        0        0    10892 2023-04-26 15:00:04.029123 strangeworks_qaoa-0.1.3/strangeworks_qaoa/utils.py
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-03 11:03:36.401419 strangeworks_qaoa-0.1.4/LICENSE
+-rw-r--r--   0        0        0      576 2023-05-03 11:03:36.401419 strangeworks_qaoa-0.1.4/README.md
+-rw-r--r--   0        0        0      791 2023-05-03 11:03:54.857458 strangeworks_qaoa-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-05-03 11:03:36.405420 strangeworks_qaoa-0.1.4/strangeworks_qaoa/__init__.py
+-rw-r--r--   0        0        0    16028 2023-05-03 11:03:36.405420 strangeworks_qaoa-0.1.4/strangeworks_qaoa/sdk.py
+-rw-r--r--   0        0        0      691 2023-05-03 11:03:36.405420 strangeworks_qaoa-0.1.4/strangeworks_qaoa/serializer.py
+-rw-r--r--   0        0        0    12428 2023-05-03 11:03:36.405420 strangeworks_qaoa-0.1.4/strangeworks_qaoa/utils.py
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.4/PKG-INFO
```

### Comparing `strangeworks_qaoa-0.1.3/LICENSE` & `strangeworks_qaoa-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.3/README.md` & `strangeworks_qaoa-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.3/pyproject.toml` & `strangeworks_qaoa-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-qaoa"
-version = "0.1.3"
+version = "0.1.4"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qaoa"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `strangeworks_qaoa-0.1.3/strangeworks_qaoa/sdk.py` & `strangeworks_qaoa-0.1.4/strangeworks_qaoa/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import dimod
 import networkx as nx
 import numpy as np
 import qiskit
 import strangeworks
 from strangeworks.core.errors.error import StrangeworksError
 
-import strangeworks_qaoa.serializer as serializer
 import strangeworks_qaoa.utils as utils
 
 
 class StrangeworksQAOA:
     """Strangeworks client object."""
 
     def __init__(self, resource_slug: Optional[str] = " ") -> None:
@@ -24,16 +23,18 @@
                 if rsc_list[rr].product.slug == "qaoa":
                     self.rsc = rsc_list[rr]
 
         self.backend_list = " "
 
     def backends(self):
         """
-        To-Do: Add cross check as to which backends the current user actually has access to.
-                Currently, this just lists all backends that could work with the qaoa service.
+        To-Do: Add cross check as to which backends the current user actually has
+          access to.
+                Currently, this just lists all backends that could work with the qaoa
+                  service.
         """
 
         all_backends = strangeworks.backends(backend_type_slugs=["sw-qaoa"])
 
         aws_backends = []
         aws_sim_backends = []
         ibmq_backends = []
@@ -60,15 +61,15 @@
                         backend_temp = {
                             "name": all_backends[bb].name,
                             "provider": "AWS",
                             "remote_status": all_backends[bb].remote_status,
                             "arn": all_backends[bb].remote_backend_id,
                         }
                         aws_backends.append(backend_temp)
-            except:
+            except AttributeError:
                 None
 
             try:
                 ibm_str = all_backends[bb].name[0:3]
                 id_str = all_backends[bb].remote_backend_id[0:3]
                 if ibm_str == "ibm":
                     if id_str == "ibm":
@@ -100,15 +101,15 @@
                     prov = "IBM_Simulator"
                     backend_temp = {
                         "backend_name": all_backends[bb].name,
                         "provider": prov,
                         "remote_status": all_backends[bb].remote_status,
                     }
                     ibm_sim_backends.append(backend_temp)
-            except:
+            except AttributeError:
                 None
 
         self.backend_list = {
             "AWS": aws_backends,
             "AWS_Sim": aws_sim_backends,
             "IBMQ": ibmq_backends,
             "IBM_Cloud": ibm_cloud_backends,
@@ -238,15 +239,14 @@
                 variable_order=problem.get("variable_order")
             )
             H = utils.get_Ham_from_QUBO(QUBO)
         else:
             raise StrangeworksError("Problem not in currently supported format")
 
         problem_params["H"] = json.dumps(H)
-        problem_params["nqubits"] = len(H[0][1])
         problem_params["ising"] = (
             json.dumps(problem_params["ising"])
             if problem_params.get("ising")
             else json.dumps(False)
         )
 
         if aws is True:
@@ -314,22 +314,23 @@
         if calculate_exact_sol:
             inputs_url = strangeworks.execute(
                 self.rsc, {"payload": {"job_slug": job_slug}}, "get_inputs_url"
             )
             inputs = strangeworks.download_job_files([inputs_url])[0]
 
             H = json.loads(inputs["H"])
+            nqubits = int(inputs["nqubits"])
 
             try:
                 En_exact = utils.get_exact_en(
-                    utils.get_graph_from_Ham(H),
-                    len(H[0][1]),
+                    utils.get_graph_from_Ham(H, nqubits),
+                    nqubits,
                     ising=json.loads(inputs["ising"]) if inputs.get("ising") else False,
                 )
-            except:
+            except Exception:
                 En_exact = "!!problem too big for exact solution!!"
             result_file["En_exact"] = En_exact
         else:
             result_file["En_exact"] = None
 
         if display_results:
             sol = result_file["sol"]
@@ -360,15 +361,15 @@
                 if job_list[jj].status != "COMPLETED" and update_status is True:
                     try:
                         status = strangeworks.execute(
                             self.rsc,
                             {"payload": {"job_slug": job_list[jj].slug}},
                             "status",
                         )
-                    except:
+                    except Exception:
                         status = job_list[jj].status
                 else:
                     status = job_list[jj].status
 
                 temp = {
                     "slug": job_list[jj].slug,
                     "Status": status,
```

### Comparing `strangeworks_qaoa-0.1.3/strangeworks_qaoa/serializer.py` & `strangeworks_qaoa-0.1.4/strangeworks_qaoa/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.3/PKG-INFO` & `strangeworks_qaoa-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-qaoa
-Version: 0.1.3
+Version: 0.1.4
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

