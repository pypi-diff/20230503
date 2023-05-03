# Comparing `tmp/landingzone_organization-0.2.0.tar.gz` & `tmp/landingzone_organization-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingzone_organization-0.2.0.tar", max compression
+gzip compressed data, was "landingzone_organization-0.2.1.tar", max compression
```

## Comparing `landingzone_organization-0.2.0.tar` & `landingzone_organization-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4206 2023-05-02 11:58:11.001978 landingzone_organization-0.2.0/README.md
--rw-r--r--   0        0        0      390 2023-05-02 11:58:11.930060 landingzone_organization-0.2.0/landingzone_organization/__init__.py
--rw-r--r--   0        0        0      395 2023-05-02 11:58:11.001978 landingzone_organization-0.2.0/landingzone_organization/account.py
--rw-r--r--   0        0        0       75 2023-05-02 11:58:11.001978 landingzone_organization-0.2.0/landingzone_organization/adapters/__init__.py
--rw-r--r--   0        0        0     3248 2023-05-02 11:58:11.001978 landingzone_organization-0.2.0/landingzone_organization/adapters/aws_organization.py
--rw-r--r--   0        0        0      509 2023-05-02 11:58:11.001978 landingzone_organization-0.2.0/landingzone_organization/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 11:58:11.001978 landingzone_organization-0.2.0/landingzone_organization/cli/commands/__init__.py
--rw-r--r--   0        0        0      598 2023-05-02 11:58:11.001978 landingzone_organization-0.2.0/landingzone_organization/cli/commands/account.py
--rw-r--r--   0        0        0      558 2023-05-02 11:58:11.001978 landingzone_organization-0.2.0/landingzone_organization/cli/commands/organization.py
--rw-r--r--   0        0        0      707 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/cli/commands/workload.py
--rw-r--r--   0        0        0     1517 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/cli/context.py
--rw-r--r--   0        0        0      744 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/cli/handler.py
--rw-r--r--   0        0        0      666 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/filtering.py
--rw-r--r--   0        0        0     1035 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/group.py
--rw-r--r--   0        0        0      929 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/groups.py
--rw-r--r--   0        0        0     2537 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/organization.py
--rw-r--r--   0        0        0      938 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/organization_unit.py
--rw-r--r--   0        0        0      887 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/workload.py
--rw-r--r--   0        0        0     1559 2023-05-02 11:58:11.005979 landingzone_organization-0.2.0/landingzone_organization/workloads.py
--rw-r--r--   0        0        0     1233 2023-05-02 11:58:11.930060 landingzone_organization-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 landingzone_organization-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      408 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/README.md
+-rw-r--r--   0        0        0      390 2023-05-03 12:09:03.600784 landingzone_organization-0.2.1/landingzone_organization/__init__.py
+-rw-r--r--   0        0        0      395 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/account.py
+-rw-r--r--   0        0        0       75 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/adapters/__init__.py
+-rw-r--r--   0        0        0     3248 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/adapters/aws_organization.py
+-rw-r--r--   0        0        0      509 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/cli/commands/__init__.py
+-rw-r--r--   0        0        0      598 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/cli/commands/account.py
+-rw-r--r--   0        0        0      558 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/cli/commands/organization.py
+-rw-r--r--   0        0        0      707 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/cli/commands/workload.py
+-rw-r--r--   0        0        0     1517 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/cli/context.py
+-rw-r--r--   0        0        0      744 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/cli/handler.py
+-rw-r--r--   0        0        0      666 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/filtering.py
+-rw-r--r--   0        0        0     1035 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/group.py
+-rw-r--r--   0        0        0      929 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/groups.py
+-rw-r--r--   0        0        0     2537 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/organization.py
+-rw-r--r--   0        0        0      938 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/organization_unit.py
+-rw-r--r--   0        0        0      887 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/workload.py
+-rw-r--r--   0        0        0     1559 2023-05-03 12:09:02.920777 landingzone_organization-0.2.1/landingzone_organization/workloads.py
+-rw-r--r--   0        0        0     1391 2023-05-03 12:09:03.600784 landingzone_organization-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 landingzone_organization-0.2.1/PKG-INFO
```

### Comparing `landingzone_organization-0.2.0/landingzone_organization/adapters/aws_organization.py` & `landingzone_organization-0.2.1/landingzone_organization/adapters/aws_organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/cli/commands/account.py` & `landingzone_organization-0.2.1/landingzone_organization/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/cli/commands/organization.py` & `landingzone_organization-0.2.1/landingzone_organization/cli/commands/organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/cli/commands/workload.py` & `landingzone_organization-0.2.1/landingzone_organization/cli/commands/workload.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/cli/context.py` & `landingzone_organization-0.2.1/landingzone_organization/cli/context.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/cli/handler.py` & `landingzone_organization-0.2.1/landingzone_organization/cli/handler.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/filtering.py` & `landingzone_organization-0.2.1/landingzone_organization/filtering.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/group.py` & `landingzone_organization-0.2.1/landingzone_organization/group.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/groups.py` & `landingzone_organization-0.2.1/landingzone_organization/groups.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/organization.py` & `landingzone_organization-0.2.1/landingzone_organization/organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/organization_unit.py` & `landingzone_organization-0.2.1/landingzone_organization/organization_unit.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/workload.py` & `landingzone_organization-0.2.1/landingzone_organization/workload.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/landingzone_organization/workloads.py` & `landingzone_organization-0.2.1/landingzone_organization/workloads.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.2.0/pyproject.toml` & `landingzone_organization-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [tool.poetry]
 name = "landingzone-organization"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 readme = "README.md"
 repository = "https://github.com/binxio/landingzone-organization"
 packages = [{include = "landingzone_organization"}]
 
+[project.urls]
+"Homepage" = "https://binxio.github.io/landingzone-organization/"
+"Bug Tracker" = "https://github.com/binxio/landingzone-organization/issues"
+
 [tool.semantic_release]
 version_variable = [
     "landingzone_organization/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "main"
 upload_to_pypi = true
```

