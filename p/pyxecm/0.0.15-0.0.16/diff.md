# Comparing `tmp/pyxecm-0.0.15.tar.gz` & `tmp/pyxecm-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.0.15.tar", last modified: Tue May  2 21:23:18 2023, max compression
+gzip compressed data, was "pyxecm-0.0.16.tar", last modified: Wed May  3 09:45:46 2023, max compression
```

## Comparing `pyxecm-0.0.15.tar` & `pyxecm-0.0.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:23:18.970272 pyxecm-0.0.15/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-02 21:23:02.000000 pyxecm-0.0.15/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-02 21:23:18.969272 pyxecm-0.0.15/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      729 2023-05-02 21:23:02.000000 pyxecm-0.0.15/README.md
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-05-02 21:23:08.000000 pyxecm-0.0.15/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:23:18.968272 pyxecm-0.0.15/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30519 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)    69124 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/m365.py
--rw-rw-rw-   0 root         (0) root         (0)    49946 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/main.py
--rw-rw-rw-   0 root         (0) root         (0)     7463 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   216194 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   113213 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10224 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)   226245 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/payload.py
--rw-rw-rw-   0 root         (0) root         (0)     5987 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/sap.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/translate.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:23:18.969272 pyxecm-0.0.15/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      394 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 21:23:18.970272 pyxecm-0.0.15/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-02 21:23:02.000000 pyxecm-0.0.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:45:46.248448 pyxecm-0.0.16/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-03 09:45:22.000000 pyxecm-0.0.16/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-03 09:45:46.248448 pyxecm-0.0.16/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-05-03 09:45:22.000000 pyxecm-0.0.16/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-05-03 09:45:33.000000 pyxecm-0.0.16/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:45:46.246448 pyxecm-0.0.16/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30481 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)    69124 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/m365.py
+-rw-rw-rw-   0 root         (0) root         (0)    49947 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   216194 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   113213 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10224 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)   226245 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/payload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5987 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/sap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/translate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2023-05-03 09:45:22.000000 pyxecm-0.0.16/pyxecm/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:45:46.248448 pyxecm-0.0.16/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      394 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 09:45:46.000000 pyxecm-0.0.16/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 09:45:46.248448 pyxecm-0.0.16/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-03 09:45:22.000000 pyxecm-0.0.16/setup.py
```

### Comparing `pyxecm-0.0.15/LICENSE` & `pyxecm-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/PKG-INFO` & `pyxecm-0.0.16/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.15
+Version: 0.0.16
 Summary: A library to connect to Opentext Extended ECM
 Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyxecm-0.0.15/README.md` & `pyxecm-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyproject.toml` & `pyxecm-0.0.16/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
   dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36", "suds"]
   description = "A library to connect to Opentext Extended ECM"
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.0.15"
+  version = "0.0.16"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
```

### Comparing `pyxecm-0.0.15/pyxecm/k8s.py` & `pyxecm-0.0.16/pyxecm/k8s.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
         return response
 
     # end method definition
 
     def findConfigMap(self, config_map_name: str):
         try:
             response = self.listConfigMaps(
-                fieldSelector="metadata.name={}".format(config_map_name)
+                field_selector="metadata.name={}".format(config_map_name)
             )
         except ApiException as e:
             logger.error(
                 "Failed to find Config Map -> {}; error -> {}".format(
                     config_map_name, str(e)
                 )
             )
@@ -531,15 +531,15 @@
         Args:
             sts_name (string): name of the Kubernetes stateful set in the current namespace
         Return: response of the Kubernetes patch command or None if the call fails
         """
 
         try:
             response = self.patchStatefulSet(
-                sts_name, stsBody={"spec": {"replicas": scale}}
+                sts_name, sts_body={"spec": {"replicas": scale}}
             )
         except ApiException as e:
             logger.error(
                 "Failed to scale Stateful Set -> {} to -> {} replicas; error -> {}".format(
                     sts_name, scale, str(e)
                 )
             )
@@ -691,34 +691,34 @@
                     "http": {
                         "paths": [
                             {
                                 "path": "/",
                                 "pathType": "Prefix",
                                 "backend": {
                                     "service": {
-                                        "name": <serviceName>,
+                                        "name": <service_name>,
                                         "port": {
                                             "name": None,
-                                            "number": <servicePort>,
+                                            "number": <service_port>,
                                         },
                                     },
                                 },
                             }
                         ]
                     },
                 }
             ]
         }
 
         Args:
-            ingressName (string): name of the Kubernetes Ingress in the current namespace
+            ingress_name (string): name of the Kubernetes Ingress in the current namespace
             hostname (string): hostname that should get an updated backend service / port
-            serviceName (string): new backend service name
-            servicePort (int): new backend service port
-        Return: Object of <class 'kubernetes.client.models.v1_ingress.V1Ingress'> or None if the call fails
+            service_name (string): new backend service name
+            service_port (integer): new backend service port
+        Return: V1Ingress Object or None if the call fails
                 This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
         """
 
         ingress = self.getIngress(ingress_name)
         if not ingress:
             return None
```

### Comparing `pyxecm-0.0.15/pyxecm/m365.py` & `pyxecm-0.0.16/pyxecm/m365.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm/main.py` & `pyxecm-0.0.16/pyxecm/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -837,15 +837,15 @@
         if result:
             logger.info("Successfully updated AppWorks Solution YAML.")
         else:
             logger.error("Failed to update AppWorks Solution YAML.")
         logger.debug("Solution YAML for AppWorks -> {}".format(solution))
 
     logger.info("Scale AppWorks Kubernetes Stateful Set to 1...")
-    k8s_object.scaleStatefulSet(stsName=OTAWP_K8S_STATEFUL_SET, scale=1)
+    k8s_object.scaleStatefulSet(sts_name=OTAWP_K8S_STATEFUL_SET, scale=1)
 
     # Add the OTCS Admin user to the AppWorks Access Role in OTDS
     otds_object.addUserToAccessRole(
         "Access to " + OTAWP_RESOURCE_NAME, "otadmin@otds.admin"
     )
 
     # Loop to wait for OTCS to create its OTDS user partition:
```

### Comparing `pyxecm-0.0.15/pyxecm/otac.py` & `pyxecm-0.0.16/pyxecm/otac.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm/otcs.py` & `pyxecm-0.0.16/pyxecm/otcs.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm/otds.py` & `pyxecm-0.0.16/pyxecm/otds.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm/otiv.py` & `pyxecm-0.0.16/pyxecm/otiv.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm/otpd.py` & `pyxecm-0.0.16/pyxecm/otpd.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm/payload.py` & `pyxecm-0.0.16/pyxecm/payload.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm/sap.py` & `pyxecm-0.0.16/pyxecm/sap.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm/translate.py` & `pyxecm-0.0.16/pyxecm/translate.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm/web.py` & `pyxecm-0.0.16/pyxecm/web.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.15/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.0.16/pyxecm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.15
+Version: 0.0.16
 Summary: A library to connect to Opentext Extended ECM
 Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

