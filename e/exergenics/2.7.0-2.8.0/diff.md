# Comparing `tmp/exergenics-2.7.0.tar.gz` & `tmp/exergenics-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-2.7.0.tar", last modified: Tue May  2 08:58:06 2023, max compression
+gzip compressed data, was "exergenics-2.8.0.tar", last modified: Wed May  3 02:26:44 2023, max compression
```

## Comparing `exergenics-2.7.0.tar` & `exergenics-2.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:58:06.951701 exergenics-2.7.0/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-02 08:58:06.951701 exergenics-2.7.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:58:06.951701 exergenics-2.7.0/exergenics/
--rw-rw-r--   0 root         (0) root         (0)       37 2023-05-02 08:56:50.000000 exergenics-2.7.0/exergenics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    60098 2023-05-02 08:56:50.000000 exergenics-2.7.0/exergenics/exergenics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:58:06.951701 exergenics-2.7.0/exergenics.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      225 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 08:58:06.951701 exergenics-2.7.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      672 2023-05-02 08:58:04.000000 exergenics-2.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:26:44.858461 exergenics-2.8.0/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-03 02:26:44.858461 exergenics-2.8.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:26:44.858461 exergenics-2.8.0/exergenics/
+-rw-rw-r--   0 root         (0) root         (0)       37 2023-05-03 02:25:28.000000 exergenics-2.8.0/exergenics/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    62080 2023-05-03 02:25:28.000000 exergenics-2.8.0/exergenics/exergenics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:26:44.858461 exergenics-2.8.0/exergenics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-03 02:26:44.000000 exergenics-2.8.0/exergenics.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 02:26:44.858461 exergenics-2.8.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      672 2023-05-03 02:26:42.000000 exergenics-2.8.0/setup.py
```

### Comparing `exergenics-2.7.0/exergenics/exergenics.py` & `exergenics-2.8.0/exergenics/exergenics.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,20 +542,19 @@
             region_name='ap-southeast-2',
             aws_access_key_id=AWS_ACCESS_KEY_ID,
             aws_secret_access_key=AWS_SECRET_ACCESS_KEY
         )
         today = date.today()
 
         extraArgs = {'ContentType': contentType}
-        if contentType == "text/html" or contentType == "html":
+        if localFile.endswith(".html") or contentType == "text/html" or contentType == "html":
             extraArgs = {
                 'ContentType': 'text/html',
                 'ContentDisposition': 'inline'
             }
-
         saveAs = "{}/{}/{}/{}__{}".format(today.year, today.month,
                                           today.day, uuid.uuid4().hex, localFile)
         client.upload_file(Filename=localFile, Bucket=self.aws_bucketName, Key=saveAs,
                            ExtraArgs=extraArgs)
         return "{}{}".format(self.aws_bucketRoot, saveAs)
 
     def getJobs(self, stage, status="completed"):
@@ -1178,14 +1177,47 @@
                                                   outputType, backgroundColor, chartWidth, chartHeight, fontSize,
                                                   fontFamily,
                                                   fontColor, legendFamily, legendSize, legendColor, legendBg, titleFont,
                                                   titleColor)
         self.putFile(plantCode, urlToChart, portalCategory,
                      chartName, equipCode, jobId)
         return urlToChart
+    
+    def portalChart_generalised3D(self, plantCode, chartName, portalCategory, dataJSON,
+                                      xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle", zAxisTitle="zAxisTitle",
+                                      fileName="fileName", backgroundColor="white", fontSize=16, fontFamily="Verdana",
+                                      fontColor="black", legendFamily="Verdana", legendSize=15, legendColor="black",
+                                      legendBg="LightSteelBlue", equipCode="", jobId=""):
+        urlToChart = self.plotlyGeneralised3D(dataJSON, xAxisTitle, yAxisTitle, zAxisTitle, fileName,
+                                                  backgroundColor, fontSize, fontFamily, fontColor, legendFamily,
+                                                  legendSize, legendColor, legendBg)
+        self.putFile(plantCode, urlToChart, portalCategory,
+                     chartName, equipCode, jobId)
+        return urlToChart
+
+    def plotlyGeneralised3D(self, dataJSON, xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle", zAxisTitle="zAxisTitle",
+                                fileName="fileName", backgroundColor="white", fontSize=16, fontFamily="Verdana",
+                                fontColor="black", legendFamily="Verdana", legendSize=15, legendColor="black",
+                                legendBg="LightSteelBlue"):
+
+        return self.plotlyRequest("generalised3D", {
+            "dataJSON": dataJSON,
+            "xAxisTitle": xAxisTitle,
+            "yAxisTitle": yAxisTitle,
+            "zAxisTitle": zAxisTitle,
+            "fileName": fileName,
+            "backgroundColor": backgroundColor,
+            "fontSize": fontSize,
+            "fontFamily": fontFamily,
+            "fontColor": fontColor,
+            "legendFamily": legendFamily,
+            "legendSize": legendSize,
+            "legendColor": legendColor,
+            "legendBg": legendBg,
+        }, "urlToGeneralised3D")
 
 
 '''
 *****************************
 ExergenicsLogger.class.py
 *****************************
```

### Comparing `exergenics-2.7.0/setup.py` & `exergenics-2.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='exergenics',
-    version='2.7.0',
+    version='2.8.0',
     author="John Christian",
     author_email='john.christian@exergenics.com',
     packages=['exergenics'],
     long_description="",
     long_description_content_type="text/markdown",
     # package_dir={'': 'src'},
     url='https://github.com/Exergenics/internal-portal-api',
```

