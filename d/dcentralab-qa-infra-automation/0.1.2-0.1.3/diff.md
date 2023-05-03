# Comparing `tmp/dcentralab_qa_infra_automation-0.1.2.tar.gz` & `tmp/dcentralab_qa_infra_automation-0.1.3.tar.gz`

## Comparing `dcentralab_qa_infra_automation-0.1.2.tar` & `dcentralab_qa_infra_automation-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-0.1.2/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.1.3/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `dcentralab_qa_infra_automation-0.1.2/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.1.3/.idea/workspace.xml`

```diff
@@ -7,15 +7,15 @@
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/Loggers.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/Loggers.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/seleniumPythonFramework_VeriSoft/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -38,15 +38,15 @@
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
-    "last_opened_file_path": "C:/Users/Efrat Cohen/Desktop/projects/packaging/src/dcentralab_qa_infra_automation/fixtures"
+    "last_opened_file_path": "C:/Users/Efrat Cohen/Desktop/projects/Dcentralab-pip/auto-qa-pip"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging\src\dcentralab_qa_infra_automation\fixtures"/>
       <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging\src\dcentralab_qa_infra_automation\drivers"/>
       <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging\src\seleniumPythonFramework_VeriSoft"/>
```

### Comparing `dcentralab_qa_infra_automation-0.1.2/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-0.1.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/LICENSE` & `dcentralab_qa_infra_automation-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.2/pyproject.toml` & `dcentralab_qa_infra_automation-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-0.1.2/PKG-INFO` & `dcentralab_qa_infra_automation-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 0.1.2
+Version: 0.1.3
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

