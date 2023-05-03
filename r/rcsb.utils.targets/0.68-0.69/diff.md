# Comparing `tmp/rcsb.utils.targets-0.68.tar.gz` & `tmp/rcsb.utils.targets-0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.targets-0.68.tar", last modified: Thu Apr 27 16:15:26 2023, max compression
+gzip compressed data, was "rcsb.utils.targets-0.69.tar", last modified: Wed May  3 20:18:38 2023, max compression
```

## Comparing `rcsb.utils.targets-0.68.tar` & `rcsb.utils.targets-0.69.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.446173 rcsb.utils.targets-0.68/
--rw-r--r--   0 vsts      (1001) docker     (122)     5820 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-04-27 16:15:26.446173 rcsb.utils.targets-0.68/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      952 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.442173 rcsb.utils.targets-0.68/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.442173 rcsb.utils.targets-0.68/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.446173 rcsb.utils.targets-0.68/rcsb/utils/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10157 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetOntologyProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/DrugBankTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/IMGTTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/IMGTTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8841 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/SAbDabTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.442173 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-27 16:03:25.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-04-27 16:15:26.446173 rcsb.utils.targets-0.68/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.238499 rcsb.utils.targets-0.69/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5885 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-05-03 20:18:38.238499 rcsb.utils.targets-0.69/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      952 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.234499 rcsb.utils.targets-0.69/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.234499 rcsb.utils.targets-0.69/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.238499 rcsb.utils.targets-0.69/rcsb/utils/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetOntologyProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/DrugBankTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/IMGTTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/IMGTTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8841 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/SAbDabTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/rcsb/utils/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 20:18:38.234499 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-03 20:03:55.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-03 20:18:38.000000 rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-05-03 20:18:38.238499 rcsb.utils.targets-0.69/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-05-03 20:02:44.000000 rcsb.utils.targets-0.69/setup.py
```

### Comparing `rcsb.utils.targets-0.68/HISTORY.txt` & `rcsb.utils.targets-0.69/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,7 +54,8 @@
   27-Feb-2023  - V0.62 Fix PharosTargetProvider mysql loading issue
    3-Mar-2023  - V0.63 Fix typo and handle missing activityType in PharosTargetCofactorProvider()
   13-Mar-2023  - V0.64 Add CARDTargetAnnotationProvider (to replace CARDTargetFeatureProvider)
   22-Mar-2023  - V0.65 Add timeout to IMGT data file fetch, and update py-rcsb_exdb_assets locators
   24-Mar-2023  - V0.66 In PharosTargetProvider(), download sql file to separate dir
   11-Apr-2023  - V0.67 Fix issue with CARD lineage tree building--handle cases with two parents at same depth; Add treeNodeList building and exporting
   27-Apr-2023  - V0.68 Update CARD treeNodeList building
+   2-May-2023  - V0.69 Remove depth field from CARD lineage tree
```

### Comparing `rcsb.utils.targets-0.68/LICENSE` & `rcsb.utils.targets-0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/PKG-INFO` & `rcsb.utils.targets-0.69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.68
+Version: 0.69
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.68/README.md` & `rcsb.utils.targets-0.69/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetAnnotationProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetFeatureProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetOntologyProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/CARDTargetProvider.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,254 +1,238 @@
 ##
-#  File:           CARDTargetOntologyProvider.py
-#  Date:           14-Mar-2023 dwp
+#  File:           CARDTargetProvider.py
+#  Date:           27-Nov-2020 jdw
 #
 #  Updates:
-#   11-Apr-2023 dwp  Fix issue with lineage tree building--handle cases with two parents at same depth;
-#                    Add treeNodeList building and exporting
-#   27-Apr-2023 dwp  Update tree node list generation
+#   14-Mar-2023 dwp  Add filterForHomologs() method to filter CARD data for only protein homolog models;
+#                    Remove unused getTargetDataPath() and getCofactorDataPath() methods
 ##
 """
-Accessors for CARD ontologies.
+Accessors for CARD target assignments.
 
 """
 
 import datetime
 import logging
 import os.path
 import time
 
 from rcsb.utils.io.FileUtil import FileUtil
 from rcsb.utils.io.MarshalUtil import MarshalUtil
 
 logger = logging.getLogger(__name__)
 
 
-class CARDTargetOntologyProvider:
-    """Accessors for CARD ontologies."""
+class CARDTargetProvider:
+    """Accessors for CARD target assignments."""
 
     def __init__(self, **kwargs):
         #
         self.__cachePath = kwargs.get("cachePath", ".")
-        self.__dirPath = os.path.join(self.__cachePath, "CARD-ontology")
+        self.__dirPath = os.path.join(self.__cachePath, "CARD-targets")
         #
         self.__mU = MarshalUtil(workPath=self.__dirPath)
-        self.__oD, self.__tnL, self.__version = self.__reload(self.__dirPath, **kwargs)
+        self.__oD, self.__version = self.__reload(self.__dirPath, **kwargs)
         #
 
-    def testCache(self, minCount=500):
+    def testCache(self, minCount=3000):
         if self.__oD and len(self.__oD) > minCount:
             return True
         else:
             return False
 
-    def getAssignmentVersion(self):
-        return self.__version
+    def hasModel(self, modelId):
+        return modelId in self.__oD
 
-    def getLineage(self, aroId):
-        """Return the lineage (all parents + the requested aroId) of the given aroId.
-
-        Args:
-            aroId (str): ARO ID in the form of "ARO:3001059"
-
-        Returns:
-            list: list of dictionaries containing the "id" and "name" of each parent
-        """
-        return self.__oD.get(aroId, [])
+    def getModelValue(self, modelId, key):
+        try:
+            return self.__oD[modelId][key]
+        except Exception:
+            return None
 
-    def getTreeNodeList(self):
-        return self.__tnL
+    def getAssignmentVersion(self):
+        return self.__version
 
     def __reload(self, dirPath, **kwargs):
         oD = None
         version = None
         startTime = time.time()
         useCache = kwargs.get("useCache", True)
         #
         ok = False
         fU = FileUtil()
         #
-        ontologyDumpUrl = kwargs.get("OntologyDumpUrl", "https://card.mcmaster.ca/latest/ontology")
-        ontologyDumpFileName = "card-ontology.tar.bz2"
-        ontologyDumpPath = os.path.join(dirPath, ontologyDumpFileName)
-        ontologyDumpDirPath = os.path.join(dirPath, "dump-ontology")
+        # CARDDumpUrl = kwargs.get("CARDDumpUrl", "https://card.mcmaster.ca/latest/data/broadstreet-v3.1.0.tar.bz2")
+        cardDumpUrl = kwargs.get("CARDDumpUrl", "https://card.mcmaster.ca/latest/data")
+        cardDumpFileName = "card-data.tar.bz2"
+        cardDumpPath = os.path.join(dirPath, cardDumpFileName)
+        cardDumpDirPath = os.path.join(dirPath, "dump-targets")
         #
         fU.mkdir(dirPath)
-        ontologyDataPath = os.path.join(dirPath, "card-ontology-data.json")
+        cardDataPath = os.path.join(dirPath, "card-select-data.json")
         #
         # ---
-        # Load Ontology data
-        logger.info("useCache %r ontologyDumpPath %r", useCache, ontologyDumpPath)
-        if useCache and self.__mU.exists(ontologyDataPath):
-            qD = self.__mU.doImport(ontologyDataPath, fmt="json")
+        # Load CARD data
+        logger.info("useCache %r CARDDumpPath %r", useCache, cardDumpPath)
+        if useCache and self.__mU.exists(cardDataPath):
+            qD = self.__mU.doImport(cardDataPath, fmt="json")
             version = qD["version"]
             oD = qD["data"]
         else:
-            logger.info("Fetching url %s path %s", ontologyDumpUrl, ontologyDumpPath)
-            ok = fU.get(ontologyDumpUrl, ontologyDumpPath)
-            fU.mkdir(ontologyDumpDirPath)
-            fU.uncompress(ontologyDumpPath, outputDir=ontologyDumpDirPath)
-            fU.unbundleTarfile(os.path.join(ontologyDumpDirPath, ontologyDumpFileName[:-4]), dirPath=ontologyDumpDirPath)
+            logger.info("Fetching url %s path %s", cardDumpUrl, cardDumpPath)
+            ok = fU.get(cardDumpUrl, cardDumpPath)
+            fU.mkdir(cardDumpDirPath)
+            fU.uncompress(cardDumpPath, outputDir=cardDumpDirPath)
+            fU.unbundleTarfile(os.path.join(cardDumpDirPath, cardDumpFileName[:-4]), dirPath=cardDumpDirPath)
             logger.info("Completed fetch (%r) at %s (%.4f seconds)", ok, time.strftime("%Y %m %d %H:%M:%S", time.localtime()), time.time() - startTime)
-            oD, tnL, version = self.__parseOntologyData(os.path.join(ontologyDumpDirPath, "aro.obo"))
+            oD, version = self.__parseCardData(os.path.join(cardDumpDirPath, "card.json"))
+            #
+            # Filter for only protein homolog models (this can be removed if/when we decide to include all types of models)
+            oD = self.__filterForHomologs(os.path.join(cardDumpDirPath, "protein_fasta_protein_homolog_model.fasta"), oD)
             #
             tS = datetime.datetime.now().isoformat()
             qD = {"version": version, "created": tS, "data": oD}
             oD = qD["data"]
-            ok = self.__mU.doExport(ontologyDataPath, qD, fmt="json", indent=3)
-            logger.info("Export CARD ontology data (%d) status %r", len(oD), ok)
+            ok = self.__mU.doExport(cardDataPath, qD, fmt="json", indent=3)
+            logger.info("Export CARD data (%d) status %r", len(oD), ok)
+        # ---
+        return oD, version
 
-        return oD, tnL, version
+    def exportCardFasta(self, fastaPath, taxonPath):
+        ok = self.__exportCardFasta(fastaPath, taxonPath, self.__oD)
+        return ok
 
-    def __parseOntologyData(self, filePath):
-        """Parse CARD ontology data
+    def __exportCardFasta(self, fastaPath, taxonPath, cardD):
+        """Export a CARD sequence target fasta file
 
         Args:
-            filePath (str): card ontology data file (aro.obo)
+            fastaPath (str): fasta output file path
+            cardD (dict): card selected data dictionary
 
         Returns:
-            (dict, string): dictionary of all ARO IDs and their ancestor lineages, ontology version string
+            (bool): True for success or False otherwise
         """
+        sD = {}
+        taxonL = []
         try:
-            cpD, tnL = None, None
-            version = None
-            parentChildList = []
-            idNameD = {}
-
-            with open(filePath, "r", encoding="utf-8") as f:
-                data = f.read()
+            for modelId, tD in cardD.items():
+                modelBitScore = None
+                # aroAcc = tD["accession"]
+                aroId = tD["cvTermId"]
+                if "sequences" not in tD:
+                    continue
+                modelBitScore = tD["modelBitScore"] if "modelBitScore" in tD else None
+                for qD in tD["sequences"]:
+                    sId = qD["seqId"]
+                    seq = qD["sequence"]
+                    taxId = qD["taxId"]
+                    cD = {"sequence": seq, "modelId": modelId, "aroId": aroId, "seqId": sId, "taxId": taxId}
+                    cD["bitScore"] = modelBitScore if modelBitScore else "-1.0"
+                    #
+                    cId = ""
+                    cL = []
+                    for k, v in cD.items():
+                        if k in ["sequence"]:
+                            continue
+                        cL.append(str(v))
+                        cL.append(str(k))
+                    cId = "|".join(cL)
+                    sD[cId] = cD
+                    taxonL.append("%s\t%s" % (cId, taxId))
+
+            ok = self.__mU.doExport(fastaPath, sD, fmt="fasta", makeComment=True)
+            logger.info("Export CARD fasta (%d) status %r", len(sD), ok)
+            ok = self.__mU.doExport(taxonPath, taxonL, fmt="list")
+            logger.info("Export Taxon (%d) status %r", len(taxonL), ok)
+        except Exception as e:
+            logger.exception("Failing for model %r tD %r with %s", modelId, tD, str(e))
+        return ok
 
-            dL = data.split("[Term]")
+    def __parseCardData(self, filePath):
+        """Parse CARD target data
 
-            version = dL.pop(0).split("\n")[0].split("format-version: ")[1]
-
-            for tS in dL:
-                tsL = tS.strip().split("\n")
-                childId, parentId, childName = None, None, None
-                for item in tsL:
-                    if item.startswith("id: "):
-                        childId = item.split('id: ')[1]
-                    if item.startswith("is_a: "):
-                        parentId = item.split('is_a: ')[1].split(" !")[0]
-                    if item.startswith("name: "):
-                        childName = item.split('name: ')[1]
-                    if parentId and childId and (parentId, childId) not in parentChildList:
-                        parentChildList.append((parentId, childId))
-                    if childName and childId not in idNameD:
-                        idNameD[childId] = childName
-                    if item.startswith("[Typedef]"):
-                        break
+        Args:
+            filePath (str): card json data file
 
-            logger.info("Ontology parent-child pair count (%d)", len(parentChildList))
+        Returns:
+            (dict, string): card selected data dictionary, card version string
+        """
+        try:
+            oD = {}
+            version = None
+            cD = self.__mU.doImport(filePath, fmt="json")
+            logger.info("CARD model count (%d)", len(cD))
+            for modelId, mD in cD.items():
+                if modelId.startswith("_"):
+                    if modelId == "_version":
+                        version = mD
+                    continue
+                oD[modelId] = {}  # modelId = '1028'
+                for kTup in [
+                    ("ARO_accession", "accession"),  # 'ARO_accession', '3001059'
+                    ("ARO_id", "cvTermId"),  # 'ARO_id', '37439'
+                    ("ARO_name", "name"),  # 'ARO_name', 'SHV-1'
+                    ("ARO_description", "descr"),  # 'SHV-1 is a broad-spectrum beta-lactamase...
+                    ("model_name", "modelName"),  # 'model_name', 'SHV-1'
+                    ("model_type", "modelType"),  # 'model_type', 'protein homolog model'
+                ]:
+                    if kTup[0] in mD:
+                        oD[modelId][kTup[1]] = mD[kTup[0]]
+                # Add in category details (Family, Drug Class(es), and Resistance mechanism)
+                acD = {}
+                if "ARO_category" in mD:
+                    aroCategoryD = mD["ARO_category"]  # 'ARO_category', large dict containing each type of 'category_aro_class_name' ("AMR Gene Family", "Drug Class", ...)
+                    for cvId, catD in aroCategoryD.items():
+                        if all([k in catD for k in ["category_aro_class_name", "category_aro_accession", "category_aro_name", "category_aro_description"]]):
+                            if catD["category_aro_class_name"] == "AMR Gene Family":
+                                acD["familyCvTermId"] = cvId
+                                acD["familyAccession"] = catD["category_aro_accession"]
+                                acD["familyName"] = catD["category_aro_name"]
+                                acD["familyDescription"] = catD["category_aro_description"]
+                            if catD["category_aro_class_name"] == "Drug Class":
+                                acD.setdefault("drugClasses", []).append(catD["category_aro_name"])
+                            if catD["category_aro_class_name"] == "Resistance Mechanism":
+                                acD["resistanceMechanism"] = catD["category_aro_name"]
+                oD[modelId].update(acD)
+                #
+                try:
+                    if "model_sequences" in mD:
+                        for seqId, tD in mD["model_sequences"]["sequence"].items():
+                            oD[modelId].setdefault("sequences", []).append(
+                                {"seqId": seqId, "sequence": tD["protein_sequence"]["sequence"], "taxId": tD["NCBI_taxonomy"]["NCBI_taxonomy_id"]}
+                            )
+                except Exception as e:
+                    logger.exception("Failing with %s", str(e))
+
+                try:
+                    if "model_param" in mD and "blastp_bit_score" in mD["model_param"] and "param_value" in mD["model_param"]["blastp_bit_score"]:
+                        oD[modelId]["modelBitScore"] = mD["model_param"]["blastp_bit_score"]["param_value"]
 
-            cpD, tnL = self.__buildLineageTree(parentChildList, idNameD)
+                except Exception as e:
+                    logger.exception("Failing with %s", str(e))
 
         except Exception as e:
             logger.exception("Failing with %s", str(e))
-        return cpD, tnL, version
+        return oD, version
 
-    def __buildLineageTree(self, parentChildTupleList, idNameMapD):
-        """Build a lineage tree containing all children as keys and a list of all possible parents as the values.
+    def __filterForHomologs(self, filePath, targetD):
+        """Filter the CARD target data to select only for protein homologs
 
         Args:
-            parentChildTupleList (list): list of (parent, child) tuples (e.g., [('ARO:1000003', 'ARO:0000000'), ('ARO:1000003', 'ARO:0000001')])
-            idNameMapD (dict): dictionary mapping of ARO IDs to their corresponding name
+            filePath (str): path to CARD fasta protein homolog model file (protein_fasta_protein_homolog_model.fasta; from source)
+            targetD (dict): dictionary generated from __parseCardData (i.e., oD)
 
         Returns:
-            dict: dictionary containing all children as keys and all possible parents as values
-                  (including the child itself, but excluding the top-level parent 'ARO:1000001')
-            list: list of all nodes (as dicts) in the tree with their immediate parents only (for building tree in browser)
+            (dict): filtered card selected data dictionary
         """
-        # create a dictionary to store the parents of each child
-        childToParentD = {}
-        for parent, child in parentChildTupleList:
-            if child not in childToParentD and child != "ARO:1000001":
-                childToParentD[child] = []
-            if parent != "ARO:1000001":  # Exclude the top-level "ARO:1000001"
-                childToParentD[child].append(parent)
-
-        # depthD = self.__createDepthDict(parentChildTupleList)
-        treeNodeL = self.__exportTreeNodeList(childToParentD, idNameMapD)
-
-        # create a dictionary to store the ancestors of each child
-        lineageD = {}
-        for child in childToParentD:
-            lineageD[child] = [{"id": child, "name": idNameMapD[child], "depth": 0}]  # Add the child to its own ancestry list
-            stack = [child]
-            depth = -1
-            while stack:
-                node = stack.pop()
-                if node in childToParentD:
-                    for parent in childToParentD[node]:
-                        if parent not in [d["id"] for d in lineageD[child]]:
-                            lineageD[child].append({"id": parent, "name": idNameMapD[parent], "depth": depth})
-                            stack.append(parent)
-                    depthLevels = set(i["depth"] for i in lineageD[child])
-                    depth = min(depthLevels) - 1
-            numDepthLevels = len(set(i["depth"] for i in lineageD[child]))
-            #
-            # Flip the depth numbering so that oldest ancestor has depth=1 and youngest/most-specific child has depth=n
-            nL = []
-            for aD in lineageD[child]:
-                aD["depth"] += numDepthLevels
-                nL.append(aD)
-            snL = sorted(nL, key=lambda x: x["depth"])  # List oldest/broadest ancestor first (depth=1), youngest/most-specific child last (depth=n)
-            lineageD[child] = snL
-
-        return lineageD, treeNodeL
-
-    def __exportTreeNodeList(self, childToParentD, idNameMapD):
-        """Create tree node list in the format of:
-
-        {'id': 'ARO:1000003', 'name': 'antibiotic molecule'}
-        {'id': 'ARO:0000041', 'name': 'bacitracin', 'parents': ['ARO:3000053', 'ARO:3000707']}
-        {'id': 'ARO:0000039', 'name': 'spectinomycin', 'parents': ['ARO:0000016']}
-        """
-        #
-        dL = []
-        for child, parentL in childToParentD.items():
-            if parentL:
-                tD = {"id": child, "name": idNameMapD[child], "parents": parentL}
-            else:
-                tD = {"id": child, "name": idNameMapD[child]}
-            dL.append(tD)
-
-        return dL
-
-    # def __createDepthDict(self, parentChildTupleList):
-    #     # Create an adjacency list to represent the graph
-    #     graph = {}
-    #     for parent, child in parentChildTupleList:
-    #         if parent not in graph:
-    #             graph[parent] = set()
-    #         graph[parent].add(child)
-    #     #
-    #     # Initialize the depth dictionary and visited set
-    #     depthD = {}
-    #     visited = set()
-    #     #
-    #     # Define a helper function to traverse the graph
-    #     def traverse(node, depth, cycleNodes):
-    #         # If we have already visited this node, return
-    #         if node in visited:
-    #             return
-    #         #
-    #         # Add the node to the visited set
-    #         visited.add(node)
-    #         #
-    #         # Add the node to the depth dictionary
-    #         if node in depthD:
-    #             depthD[node].extend(cycleNodes + [depth])
-    #         else:
-    #             depthD[node] = cycleNodes + [depth]
-    #         #
-    #         # Traverse the children of the node
-    #         if node in graph:
-    #             for child in graph[node]:
-    #                 traverse(child, depth+1, cycleNodes)
-    #     #
-    #     # Traverse the graph from each node to handle cycles
-    #     for node in graph:
-    #         traverse(node, 0, [])
-    #     #
-    #     # Return the completed depth dictionary
-    #     return depthD
+
+        with open(filePath, "r", encoding="utf-8") as f:
+            data = f.readlines()
+
+        aroL = [i.split("|")[2].strip("ARO:") for i in data if i.startswith(">")]
+
+        filteredD = {}
+        for k, v in targetD.items():
+            if v["accession"] in aroL:
+                filteredD.update({k: v})
+
+        return filteredD
```

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetActivityProvider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,238 +1,236 @@
 ##
-#  File:           CARDTargetProvider.py
-#  Date:           27-Nov-2020 jdw
+#  File:           PharosTargetActivityProvider.py
+#  Date:           17-Jun-2021 jdw
+#
+#  Updated:
+#  3-Mar-2023 aae fix method typo
 #
-#  Updates:
-#   14-Mar-2023 dwp  Add filterForHomologs() method to filter CARD data for only protein homolog models;
-#                    Remove unused getTargetDataPath() and getCofactorDataPath() methods
 ##
 """
-Accessors for CARD target assignments.
+Accessors for Pharos target activity data.
 
 """
 
 import datetime
 import logging
 import os.path
 import time
 
+from rcsb.utils.chemref.PharosProvider import PharosProvider
 from rcsb.utils.io.FileUtil import FileUtil
 from rcsb.utils.io.MarshalUtil import MarshalUtil
+from rcsb.utils.io.StashableBase import StashableBase
+
 
 logger = logging.getLogger(__name__)
 
 
-class CARDTargetProvider:
-    """Accessors for CARD target assignments."""
+class PharosTargetActivityProvider(StashableBase):
+    """Accessors for Pharos target activity data."""
 
-    def __init__(self, **kwargs):
+    def __init__(self, cachePath, useCache):
         #
-        self.__cachePath = kwargs.get("cachePath", ".")
-        self.__dirPath = os.path.join(self.__cachePath, "CARD-targets")
-        #
-        self.__mU = MarshalUtil(workPath=self.__dirPath)
-        self.__oD, self.__version = self.__reload(self.__dirPath, **kwargs)
+        self.__cachePath = cachePath
+        self.__dirName = "Pharos-target-activity"
+        super(PharosTargetActivityProvider, self).__init__(self.__cachePath, [self.__dirName])
+        self.__dirPath = os.path.join(self.__cachePath, self.__dirName)
+        self.__mU = MarshalUtil(workPath=self.__cachePath)
         #
+        self.__aD, self.__tD, self.__version = self.__reload(self.__dirPath, useCache)
 
-    def testCache(self, minCount=3000):
-        if self.__oD and len(self.__oD) > minCount:
+    def testCache(self, minCount=0):
+        if minCount == 0:
             return True
-        else:
-            return False
-
-    def hasModel(self, modelId):
-        return modelId in self.__oD
-
-    def getModelValue(self, modelId, key):
-        try:
-            return self.__oD[modelId][key]
-        except Exception:
-            return None
+        if self.__aD and (len(self.__aD) > minCount):
+            logger.info("Cached Pharos activity data for (%d) targets", len(self.__aD))
+            return True
+        return False
 
     def getAssignmentVersion(self):
         return self.__version
 
-    def __reload(self, dirPath, **kwargs):
-        oD = None
-        version = None
+    def getTargetActivityDataPath(self):
+        return os.path.join(self.__dirPath, "pharos-target-activity-data.json")
+
+    def __reload(self, dirPath, useCache):
         startTime = time.time()
-        useCache = kwargs.get("useCache", True)
-        #
-        ok = False
+        aD = {}
+        tD = {}
+        version = None
         fU = FileUtil()
+        fU.mkdir(dirPath)
+        targetActivityFilePath = self.getTargetActivityDataPath()
         #
-        # CARDDumpUrl = kwargs.get("CARDDumpUrl", "https://card.mcmaster.ca/latest/data/broadstreet-v3.1.0.tar.bz2")
-        cardDumpUrl = kwargs.get("CARDDumpUrl", "https://card.mcmaster.ca/latest/data")
-        cardDumpFileName = "card-data.tar.bz2"
-        cardDumpPath = os.path.join(dirPath, cardDumpFileName)
-        cardDumpDirPath = os.path.join(dirPath, "dump-targets")
+        if useCache and fU.exists(targetActivityFilePath):
+            logger.info("useCache %r using %r", useCache, targetActivityFilePath)
+            qD = self.__mU.doImport(targetActivityFilePath, fmt="json")
+            aD = qD["activity"] if "activity" in qD else {}
+            tD = qD["targets"] if "targets" in qD else {}
+            version = qD["version"] if "version" in qD else None
         #
-        fU.mkdir(dirPath)
-        cardDataPath = os.path.join(dirPath, "card-select-data.json")
+        logger.info("Completed reload of (%d) activity records at %s (%.4f seconds)", len(aD), time.strftime("%Y %m %d %H:%M:%S", time.localtime()), time.time() - startTime)
         #
-        # ---
-        # Load CARD data
-        logger.info("useCache %r CARDDumpPath %r", useCache, cardDumpPath)
-        if useCache and self.__mU.exists(cardDataPath):
-            qD = self.__mU.doImport(cardDataPath, fmt="json")
-            version = qD["version"]
-            oD = qD["data"]
-        else:
-            logger.info("Fetching url %s path %s", cardDumpUrl, cardDumpPath)
-            ok = fU.get(cardDumpUrl, cardDumpPath)
-            fU.mkdir(cardDumpDirPath)
-            fU.uncompress(cardDumpPath, outputDir=cardDumpDirPath)
-            fU.unbundleTarfile(os.path.join(cardDumpDirPath, cardDumpFileName[:-4]), dirPath=cardDumpDirPath)
-            logger.info("Completed fetch (%r) at %s (%.4f seconds)", ok, time.strftime("%Y %m %d %H:%M:%S", time.localtime()), time.time() - startTime)
-            oD, version = self.__parseCardData(os.path.join(cardDumpDirPath, "card.json"))
-            #
-            # Filter for only protein homolog models (this can be removed if/when we decide to include all types of models)
-            oD = self.__filterForHomologs(os.path.join(cardDumpDirPath, "protein_fasta_protein_homolog_model.fasta"), oD)
-            #
-            tS = datetime.datetime.now().isoformat()
-            qD = {"version": version, "created": tS, "data": oD}
-            oD = qD["data"]
-            ok = self.__mU.doExport(cardDataPath, qD, fmt="json", indent=3)
-            logger.info("Export CARD data (%d) status %r", len(oD), ok)
-        # ---
-        return oD, version
+        return aD, tD, version
 
-    def exportCardFasta(self, fastaPath, taxonPath):
-        ok = self.__exportCardFasta(fastaPath, taxonPath, self.__oD)
-        return ok
+    def getTargetActivity(self, pharosTargetId):
+        try:
+            return self.__aD[pharosTargetId] if pharosTargetId in self.__aD else []
+        except Exception:
+            return []
 
-    def __exportCardFasta(self, fastaPath, taxonPath, cardD):
-        """Export a CARD sequence target fasta file
+    def hasTargetActivity(self, pharosTargetId):
+        try:
+            return pharosTargetId in self.__aD
+        except Exception:
+            return False
 
-        Args:
-            fastaPath (str): fasta output file path
-            cardD (dict): card selected data dictionary
+    def hasTargetInfo(self, pharosTargetId):
+        try:
+            return pharosTargetId in self.__tD
+        except Exception:
+            return False
 
-        Returns:
-            (bool): True for success or False otherwise
-        """
-        sD = {}
-        taxonL = []
+    def getTargetInfo(self, pharosTargetId, ky):
         try:
-            for modelId, tD in cardD.items():
-                modelBitScore = None
-                # aroAcc = tD["accession"]
-                aroId = tD["cvTermId"]
-                if "sequences" not in tD:
-                    continue
-                modelBitScore = tD["modelBitScore"] if "modelBitScore" in tD else None
-                for qD in tD["sequences"]:
-                    sId = qD["seqId"]
-                    seq = qD["sequence"]
-                    taxId = qD["taxId"]
-                    cD = {"sequence": seq, "modelId": modelId, "aroId": aroId, "seqId": sId, "taxId": taxId}
-                    cD["bitScore"] = modelBitScore if modelBitScore else "-1.0"
-                    #
-                    cId = ""
-                    cL = []
-                    for k, v in cD.items():
-                        if k in ["sequence"]:
-                            continue
-                        cL.append(str(v))
-                        cL.append(str(k))
-                    cId = "|".join(cL)
-                    sD[cId] = cD
-                    taxonL.append("%s\t%s" % (cId, taxId))
-
-            ok = self.__mU.doExport(fastaPath, sD, fmt="fasta", makeComment=True)
-            logger.info("Export CARD fasta (%d) status %r", len(sD), ok)
-            ok = self.__mU.doExport(taxonPath, taxonL, fmt="list")
-            logger.info("Export Taxon (%d) status %r", len(taxonL), ok)
-        except Exception as e:
-            logger.exception("Failing for model %r tD %r with %s", modelId, tD, str(e))
+            return self.__tD[pharosTargetId][ky]
+        except Exception:
+            return None
+
+    def fetchTargetActivityData(self):
+        targetD = {}
+        cofactorFilePath = os.path.join(self.__cachePath, "Pharos-targets", "drug_activity.tdd")
+        cfDL = self.__mU.doImport(cofactorFilePath, fmt="tdd", rowFormat="dict")
+        targetD = self.__extractCofactorData(cfDL)
+        drgIdS = self.__extractDrugIdentifiers(cfDL)
+        #
+        cofactorFilePath = os.path.join(self.__cachePath, "Pharos-targets", "cmpd_activity.tdd")
+        cfDL = self.__mU.doImport(cofactorFilePath, fmt="tdd", rowFormat="dict")
+        targetD.update(self.__extractCofactorData(cfDL))
+        cmpIdS = self.__extractCompoundIdentifiers(cfDL)
+        chemblIdList = list(cmpIdS.union(drgIdS))
+        phP = PharosProvider(cachePath=self.__cachePath, useCache=False)
+        phP.load(chemblIdList, "identifiers", fmt="json", indent=0)
+        #
+        targetFilePath = os.path.join(self.__cachePath, "Pharos-targets", "protein.tdd")
+        tDL = self.__mU.doImport(targetFilePath, fmt="tdd", rowFormat="dict")
+        targetDetailsD = self.__getTargetDetails(tDL)
+        #
+        pharosReadmePath = os.path.join(self.__cachePath, "Pharos-targets", "pharos-readme.txt")
+        readmeLines = self.__mU.doImport(pharosReadmePath, fmt="list")
+        self.__version = readmeLines[0].split(" ")[1][1:] if readmeLines else "6"
+        #
+        tS = datetime.datetime.now().isoformat()
+        # vS = datetime.datetime.now().strftime("%Y-%m-%d")
+        vS = self.__version
+        ok = self.__mU.doExport(self.getTargetActivityDataPath(), {"version": vS, "created": tS, "activity": targetD, "targets": targetDetailsD}, fmt="json", indent=3)
         return ok
 
-    def __parseCardData(self, filePath):
-        """Parse CARD target data
+    def fetchCompoundIdentifiers(self):
+        cofactorFilePath = os.path.join(self.__cachePath, "Pharos-targets", "drug_activity.tdd")
+        cfDL = self.__mU.doImport(cofactorFilePath, fmt="tdd", rowFormat="dict")
+        drgIdS = self.__extractDrugIdentifiers(cfDL)
+        #
+        cofactorFilePath = os.path.join(self.__cachePath, "Pharos-targets", "cmpd_activity.tdd")
+        cfDL = self.__mU.doImport(cofactorFilePath, fmt="tdd", rowFormat="dict")
+        cmpIdS = self.__extractCompoundIdentifiers(cfDL)
+        chemblIdList = list(cmpIdS.union(drgIdS))
+        return chemblIdList
+
+    def __extractCompoundIdentifiers(self, cfDL):
+        chemblIdS = set()
+        for cfD in cfDL:
+            if cfD["catype"].upper() == "CHEMBL":
+                chemblIdS.add(cfD["cmpd_id_in_src"])
+        return chemblIdS
+
+    def __extractDrugIdentifiers(self, cfDL):
+        chemblIdS = set()
+        for cfD in cfDL:
+            if cfD["cmpd_chemblid"] and cfD["cmpd_chemblid"].startswith("CHEM"):
+                chemblIdS.add(cfD["cmpd_chemblid"])
+        return chemblIdS
+
+    def __extractCofactorData(self, cfDL):
+        """Extract ids, activity and moa data for drugs and cofactors from the Pharos schema dump files.
 
         Args:
-            filePath (str): card json data file
+            cfDL (list): list of dictionaries of containing pharos exported db data.
 
         Returns:
-            (dict, string): card selected data dictionary, card version string
+            dict: dictionary of extracted cofactor data
         """
         try:
-            oD = {}
-            version = None
-            cD = self.__mU.doImport(filePath, fmt="json")
-            logger.info("CARD model count (%d)", len(cD))
-            for modelId, mD in cD.items():
-                if modelId.startswith("_"):
-                    if modelId == "_version":
-                        version = mD
-                    continue
-                oD[modelId] = {}  # modelId = '1028'
-                for kTup in [
-                    ("ARO_accession", "accession"),  # 'ARO_accession', '3001059'
-                    ("ARO_id", "cvTermId"),  # 'ARO_id', '37439'
-                    ("ARO_name", "name"),  # 'ARO_name', 'SHV-1'
-                    ("ARO_description", "descr"),  # 'SHV-1 is a broad-spectrum beta-lactamase...
-                    ("model_name", "modelName"),  # 'model_name', 'SHV-1'
-                    ("model_type", "modelType"),  # 'model_type', 'protein homolog model'
-                ]:
-                    if kTup[0] in mD:
-                        oD[modelId][kTup[1]] = mD[kTup[0]]
-                # Add in category details (Family, Drug Class(es), and Resistance mechanism)
-                acD = {}
-                if "ARO_category" in mD:
-                    aroCategoryD = mD["ARO_category"]  # 'ARO_category', large dict containing each type of 'category_aro_class_name' ("AMR Gene Family", "Drug Class", ...)
-                    for cvId, catD in aroCategoryD.items():
-                        if all([k in catD for k in ["category_aro_class_name", "category_aro_accession", "category_aro_name", "category_aro_description"]]):
-                            if catD["category_aro_class_name"] == "AMR Gene Family":
-                                acD["familyCvTermId"] = cvId
-                                acD["familyAccession"] = catD["category_aro_accession"]
-                                acD["familyName"] = catD["category_aro_name"]
-                                acD["familyDescription"] = catD["category_aro_description"]
-                            if catD["category_aro_class_name"] == "Drug Class":
-                                acD.setdefault("drugClasses", []).append(catD["category_aro_name"])
-                            if catD["category_aro_class_name"] == "Resistance Mechanism":
-                                acD["resistanceMechanism"] = catD["category_aro_name"]
-                oD[modelId].update(acD)
+            qD = {}
+            targetD = {}
+            dupD = {}
+            for cfD in cfDL:
+                tId = cfD["target_id"]
+                qD = {}
+                qD["smiles"] = cfD["smiles"] if "smiles" in cfD and cfD["smiles"] not in ["N", "NULL"] else None
+                qD["chemblId"] = cfD["cmpd_chemblid"] if "cmpd_chemblid" in cfD else None
+                qD["chemblId"] = cfD["cmpd_id_in_src"] if "catype" in cfD and cfD["catype"].upper() == "CHEMBL" else qD["chemblId"]
+                qD["chemblId"] = qD["chemblId"] if qD["chemblId"] not in ["N", "NULL"] else None
+                qD["pubChemId"] = cfD["cmpd_pubchem_cid"] if "cmpd_pubchem_cid" in cfD and cfD["cmpd_pubchem_cid"] not in ["NULL"] else None
+                #
+                qD["activity"] = cfD["act_value"] if "act_value" in cfD and cfD["act_value"] != "NULL" else None
+                qD["activityType"] = cfD["act_type"] if "act_type" in cfD and cfD["act_type"] != "NULL" else None
+                if qD["activity"] is not None:
+                    qD["activity"] = float(qD["activity"])
+                    # qD["activityUnits"] = "nM"
+                #
+                qD["action"] = cfD["action"] if "action" in cfD and cfD["moa"] == "1" else None
+                qD["pharmacology"] = cfD["nlm_drug_info"] if "nlm_drug_info" in cfD else None
+                tS = cfD["drug"] if "drug" in cfD else None
+                tS = cfD["cmpd_name_in_src"] if "cmpd_name_in_src" in cfD and cfD["cmpd_name_in_src"] != "NULL" else tS
+                #
+                if tS and tS.startswith("US"):
+                    tSL = tS.split(",")
+                    qD["patents"] = [t for t in tSL if t.startswith("US")]
+                elif tS:
+                    # handle the double colon :: separators
+                    tSL = tS.split("::")
+                    if not tSL:
+                        qD["molecule_name"] = tS
+                    else:
+                        for tS in tSL:
+                            if tS.startswith("CHEMBL"):
+                                continue
+                            elif tS.startswith("US"):
+                                ttL = tS.split(",")
+                                qD.setdefault("patents", []).append(ttL[0])
+                            else:
+                                qD["molecule_name"] = tS
+
+                #
+                pmId = None
+                tS = cfD["reference"] if "reference" in cfD else None
+                if tS and "pubmed" in tS:
+                    pmId = tS.split("/")[-1]
+                tS = cfD["pubmed_ids"].split(",")[0] if "pubmed_ids" in cfD and cfD["pubmed_ids"] else pmId
+                qD["pubmedId"] = tS if tS and tS not in ["NULL"] else None
                 #
-                try:
-                    if "model_sequences" in mD:
-                        for seqId, tD in mD["model_sequences"]["sequence"].items():
-                            oD[modelId].setdefault("sequences", []).append(
-                                {"seqId": seqId, "sequence": tD["protein_sequence"]["sequence"], "taxId": tD["NCBI_taxonomy"]["NCBI_taxonomy_id"]}
-                            )
-                except Exception as e:
-                    logger.exception("Failing with %s", str(e))
-
-                try:
-                    if "model_param" in mD and "blastp_bit_score" in mD["model_param"] and "param_value" in mD["model_param"]["blastp_bit_score"]:
-                        oD[modelId]["modelBitScore"] = mD["model_param"]["blastp_bit_score"]["param_value"]
+                if qD["activity"] and qD["chemblId"] and (qD["chemblId"], qD["activityType"], qD["action"]) not in dupD:
+                    dupD[(qD["chemblId"], qD["activityType"], qD["action"])] = True
+                    targetD.setdefault(tId, []).append({ky: qD[ky] for ky in qD if qD[ky] is not None})
 
-                except Exception as e:
-                    logger.exception("Failing with %s", str(e))
+            #
+        except Exception as e:
+            logger.exception("Failing with %r %s", qD, str(e))
+        return targetD
 
+    def __getTargetDetails(self, targetDL):
+        # Pharos protein target - protein.tdd
+        # id	name	description	uniprot	up_version	geneid	sym	family	chr	seq	dtoid	stringid	dtoclass
+        rD = {}
+        try:
+            for targetD in targetDL:
+                proteinId = targetD["id"]
+                unpId = targetD["uniprot"] if "uniprot" in targetD and targetD["uniprot"] != "NULL" else None
+                descr = targetD["description"] if "description" in targetD and targetD["description"] != "NULL" else None
+                geneId = targetD["geneid"] if "geneid" in targetD and targetD["geneid"] != "NULL" else None
+                dtoId = targetD["dtoid"] if "dtoid" in targetD and targetD["dtoid"] != "NULL" else None
+                dtoClass = targetD["dtoclass"] if "dtoclass" in targetD and targetD["dtoclass"] != "NULL" else None
+                rD[proteinId] = {"unpId": unpId, "name": descr, "geneId": geneId, "dtoId": dtoId, "dtoClass": dtoClass}
         except Exception as e:
             logger.exception("Failing with %s", str(e))
-        return oD, version
-
-    def __filterForHomologs(self, filePath, targetD):
-        """Filter the CARD target data to select only for protein homologs
-
-        Args:
-            filePath (str): path to CARD fasta protein homolog model file (protein_fasta_protein_homolog_model.fasta; from source)
-            targetD (dict): dictionary generated from __parseCardData (i.e., oD)
-
-        Returns:
-            (dict): filtered card selected data dictionary
-        """
-
-        with open(filePath, "r", encoding="utf-8") as f:
-            data = f.readlines()
-
-        aroL = [i.split("|")[2].strip("ARO:") for i in data if i.startswith(">")]
-
-        filteredD = {}
-        for k, v in targetD.items():
-            if v["accession"] in aroL:
-                filteredD.update({k: v})
-
-        return filteredD
+        return rD
```

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetActivityProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/ChEMBLTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/DrugBankTargetCofactorProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/DrugBankTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/DrugBankTargetProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/DrugBankTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/IMGTTargetFeatureProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/IMGTTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/IMGTTargetProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/IMGTTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetCofactorProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/PharosTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/SAbDabTargetFeatureProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/SAbDabTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb/utils/targets/SAbDabTargetProvider.py` & `rcsb.utils.targets-0.69/rcsb/utils/targets/SAbDabTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/PKG-INFO` & `rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.68
+Version: 0.69
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/SOURCES.txt` & `rcsb.utils.targets-0.69/rcsb.utils.targets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.68/setup.py` & `rcsb.utils.targets-0.69/setup.py`

 * *Files identical despite different names*

