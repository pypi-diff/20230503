# Comparing `tmp/hardeneks-0.9.1.tar.gz` & `tmp/hardeneks-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardeneks-0.9.1.tar", max compression
+gzip compressed data, was "hardeneks-0.9.2.tar", max compression
```

## Comparing `hardeneks-0.9.1.tar` & `hardeneks-0.9.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      927 2023-04-28 16:06:51.608430 hardeneks-0.9.1/LICENSE
--rw-r--r--   0        0        0     6610 2023-04-28 16:06:51.608430 hardeneks-0.9.1/README.md
--rw-r--r--   0        0        0     7046 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/cluster_autoscaling/__init__.py
--rw-r--r--   0        0        0     9687 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py
--rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/reliability/__init__.py
--rw-r--r--   0        0        0     1525 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/reliability/applications.py
--rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/scalability/__init__.py
--rw-r--r--   0        0        0     2112 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/scalability/control_plane.py
--rw-r--r--   0        0        0      551 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/scalability/skipped.json
--rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/__init__.py
--rw-r--r--   0        0        0      874 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/detective_controls.py
--rw-r--r--   0        0        0     3161 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/encryption_secrets.py
--rw-r--r--   0        0        0     5409 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/iam.py
--rw-r--r--   0        0        0     1009 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/image_security.py
--rw-r--r--   0        0        0     2374 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/infrastructure_security.py
--rw-r--r--   0        0        0      760 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/multi_tenancy.py
--rw-r--r--   0        0        0     2558 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/network_security.py
--rw-r--r--   0        0        0     1222 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/pod_security.py
--rw-r--r--   0        0        0     2731 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/config.yaml
--rw-r--r--   0        0        0      728 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/harden.py
--rw-r--r--   0        0        0      544 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/helpers.py
--rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/reliability/__init__.py
--rw-r--r--   0        0        0     5859 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/reliability/applications.py
--rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/__init__.py
--rw-r--r--   0        0        0     1305 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/encryption_secrets.py
--rw-r--r--   0        0        0     8011 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/iam.py
--rw-r--r--   0        0        0     1370 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/network_security.py
--rw-r--r--   0        0        0     5259 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/pod_security.py
--rw-r--r--   0        0        0     1685 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/runtime_security.py
--rw-r--r--   0        0        0     2289 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/resources.py
--rw-r--r--   0        0        0     1412 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/rules.py
--rw-r--r--   0        0        0     1005 2023-04-28 16:06:51.616430 hardeneks-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 hardeneks-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      927 2023-05-03 18:18:58.610709 hardeneks-0.9.2/LICENSE
+-rw-r--r--   0        0        0     6610 2023-05-03 18:18:58.610709 hardeneks-0.9.2/README.md
+-rw-r--r--   0        0        0     7046 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/cluster_autoscaling/__init__.py
+-rw-r--r--   0        0        0     9687 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py
+-rw-r--r--   0        0        0        0 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/reliability/__init__.py
+-rw-r--r--   0        0        0     1525 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/reliability/applications.py
+-rw-r--r--   0        0        0        0 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/scalability/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/scalability/control_plane.py
+-rw-r--r--   0        0        0      551 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/scalability/skipped.json
+-rw-r--r--   0        0        0        0 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/security/__init__.py
+-rw-r--r--   0        0        0      874 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/security/detective_controls.py
+-rw-r--r--   0        0        0     3161 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/security/encryption_secrets.py
+-rw-r--r--   0        0        0     5560 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/security/iam.py
+-rw-r--r--   0        0        0     1009 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/security/image_security.py
+-rw-r--r--   0        0        0     2374 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/security/infrastructure_security.py
+-rw-r--r--   0        0        0      760 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/security/multi_tenancy.py
+-rw-r--r--   0        0        0     2558 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/security/network_security.py
+-rw-r--r--   0        0        0     1222 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/cluster_wide/security/pod_security.py
+-rw-r--r--   0        0        0     2731 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/config.yaml
+-rw-r--r--   0        0        0      728 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/harden.py
+-rw-r--r--   0        0        0      544 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/namespace_based/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/namespace_based/reliability/__init__.py
+-rw-r--r--   0        0        0     5859 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/namespace_based/reliability/applications.py
+-rw-r--r--   0        0        0        0 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/namespace_based/security/__init__.py
+-rw-r--r--   0        0        0     1305 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/namespace_based/security/encryption_secrets.py
+-rw-r--r--   0        0        0     8011 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/namespace_based/security/iam.py
+-rw-r--r--   0        0        0     1370 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/namespace_based/security/network_security.py
+-rw-r--r--   0        0        0     5259 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/namespace_based/security/pod_security.py
+-rw-r--r--   0        0        0     1685 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/namespace_based/security/runtime_security.py
+-rw-r--r--   0        0        0     2289 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/resources.py
+-rw-r--r--   0        0        0     1412 2023-05-03 18:18:58.622710 hardeneks-0.9.2/hardeneks/rules.py
+-rw-r--r--   0        0        0     1005 2023-05-03 18:18:58.622710 hardeneks-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 hardeneks-0.9.2/PKG-INFO
```

### Comparing `hardeneks-0.9.1/LICENSE` & `hardeneks-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/README.md` & `hardeneks-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/__init__.py` & `hardeneks-0.9.2/hardeneks/__init__.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/reliability/applications.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/reliability/applications.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/scalability/control_plane.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/scalability/control_plane.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/scalability/skipped.json` & `hardeneks-0.9.2/hardeneks/cluster_wide/scalability/skipped.json`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/security/detective_controls.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/security/detective_controls.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/security/encryption_secrets.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/security/encryption_secrets.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/security/iam.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/security/iam.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,16 +127,21 @@
     section = "iam"
     message = "Don't bind clusterroles to anonymous/unauthenticated groups."
     url = "https://aws.github.io/aws-eks-best-practices/security/docs/iam/#review-and-revoke-unnecessary-anonymous-access"
 
     def check(self, resources: Resources):
         offenders = []
 
+        ignored = ["system:public-info-viewer"]
+
         for cluster_role_binding in resources.cluster_role_bindings:
-            if cluster_role_binding.subjects:
+            if (
+                cluster_role_binding.subjects
+                and cluster_role_binding.metadata.name not in ignored
+            ):
                 for subject in cluster_role_binding.subjects:
                     if (
                         subject.name == "system:unauthenticated"
                         or subject.name == "system:anonymous"
                     ):
                         offenders.append(cluster_role_binding)
```

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/security/image_security.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/security/image_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/security/infrastructure_security.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/security/infrastructure_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/security/multi_tenancy.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/security/multi_tenancy.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/security/network_security.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/security/network_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/cluster_wide/security/pod_security.py` & `hardeneks-0.9.2/hardeneks/cluster_wide/security/pod_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/config.yaml` & `hardeneks-0.9.2/hardeneks/config.yaml`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/harden.py` & `hardeneks-0.9.2/hardeneks/harden.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/helpers.py` & `hardeneks-0.9.2/hardeneks/helpers.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/namespace_based/reliability/applications.py` & `hardeneks-0.9.2/hardeneks/namespace_based/reliability/applications.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/namespace_based/security/encryption_secrets.py` & `hardeneks-0.9.2/hardeneks/namespace_based/security/encryption_secrets.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/namespace_based/security/iam.py` & `hardeneks-0.9.2/hardeneks/namespace_based/security/iam.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/namespace_based/security/network_security.py` & `hardeneks-0.9.2/hardeneks/namespace_based/security/network_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/namespace_based/security/pod_security.py` & `hardeneks-0.9.2/hardeneks/namespace_based/security/pod_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/namespace_based/security/runtime_security.py` & `hardeneks-0.9.2/hardeneks/namespace_based/security/runtime_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/resources.py` & `hardeneks-0.9.2/hardeneks/resources.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/hardeneks/rules.py` & `hardeneks-0.9.2/hardeneks/rules.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.1/pyproject.toml` & `hardeneks-0.9.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hardeneks"
-version = "0.9.1"
+version = "0.9.2"
 description = ""
 authors = ["Doruk Ozturk <dozturk@amazon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 typer = {extras = ["all"], version = "^0.6.1"}
@@ -37,15 +37,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.9.1"
+version = "0.9.2"
 version_files = [
   "pyproject.toml:[tool.commitizen]\nversion",
   "pyproject.toml:[tool.poetry]\nname = \"commitizen\"\nversion",
   "pyproject.toml:^version"
 ]
 tag_format = "v$version"
 [build-system]
```

### Comparing `hardeneks-0.9.1/PKG-INFO` & `hardeneks-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardeneks
-Version: 0.9.1
+Version: 0.9.2
 Summary: 
 Author: Doruk Ozturk
 Author-email: dozturk@amazon.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

