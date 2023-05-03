# Comparing `tmp/init_service-0.7.0.tar.gz` & `tmp/init_service-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "init_service-0.7.0.tar", max compression
+gzip compressed data, was "init_service-0.8.0.tar", max compression
```

## Comparing `init_service-0.7.0.tar` & `init_service-0.8.0.tar`

### file list

```diff
@@ -1,42 +1,48 @@
--rw-r--r--   0        0        0    11357 2023-04-13 16:06:56.962055 init_service-0.7.0/LICENSE
--rw-r--r--   0        0        0      683 2023-04-13 16:06:56.962055 init_service-0.7.0/init_service/__init__.py
--rw-r--r--   0        0        0    10586 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/init_service.py
--rw-r--r--   0        0        0    50425 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/pyratemp.py
--rw-r--r--   0        0        0      353 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/.gitignore
--rw-r--r--   0        0        0      299 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/build.sbt
--rw-r--r--   0        0        0      308 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/project/LibDependencies.scala
--rw-r--r--   0        0        0       28 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/project/build.properties
--rw-r--r--   0        0        0      369 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/project/plugins.sbt
--rw-r--r--   0        0        0       82 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/src/main/scala/uk/gov/hmrc/hello/HelloWorld.scala
--rw-r--r--   0        0        0      275 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/library/src/test/scala/uk/gov/hmrc/hello/HelloWorldSpec.scala
--rw-r--r--   0        0        0      353 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/.gitignore
--rw-r--r--   0        0        0       41 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/assets/stylesheets/application.scss
--rw-r--r--   0        0        0      447 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/config/AppConfig.scala
--rw-r--r--   0        0        0      626 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/config/ErrorHandler.scala
--rw-r--r--   0        0        0      221 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/config/Module.scala
--rw-r--r--   0        0        0      620 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/controllers/HelloWorldController.scala
--rw-r--r--   0        0        0      503 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/controllers/MicroserviceHelloWorldController.scala
--rw-r--r--   0        0        0      374 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/views/ErrorTemplate.scala.html
--rw-r--r--   0        0        0      260 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/views/HelloWorldPage.scala.html
--rw-r--r--   0        0        0      454 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/app/views/Layout.scala.html
--rw-r--r--   0        0        0      855 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/build.sbt
--rw-r--r--   0        0        0      472 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/app.routes
--rw-r--r--   0        0        0      300 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/application-json-logger.xml
--rw-r--r--   0        0        0     3070 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/application.conf
--rw-r--r--   0        0        0     2337 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/logback.xml
--rw-r--r--   0        0        0       68 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/messages
--rw-r--r--   0        0        0       69 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/messages.cy
--rw-r--r--   0        0        0      247 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/prod.routes
--rw-r--r--   0        0        0     1098 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/conf/testOnlyDoNotUseInAppConf.routes
--rw-r--r--   0        0        0     1024 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/it/HealthEndpointIntegrationSpec.scala
--rw-r--r--   0        0        0     1239 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/project/AppDependencies.scala
--rw-r--r--   0        0        0      566 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/project/CodeCoverageSettings.scala
--rw-r--r--   0        0        0       28 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/project/build.properties
--rw-r--r--   0        0        0      770 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/project/plugins.sbt
--rw-r--r--   0        0        0      232 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/template/BACKEND.delete
--rw-r--r--   0        0        0      115 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/template/FRONTEND.delete
--rw-r--r--   0        0        0      914 2023-04-13 16:06:56.966055 init_service-0.7.0/init_service/templates/service/test/config/ErrorHandlerSpec.scala
--rw-r--r--   0        0        0     1119 2023-04-13 16:06:56.970055 init_service-0.7.0/init_service/templates/service/test/controllers/HelloWorldControllerSpec.scala
--rw-r--r--   0        0        0      623 2023-04-13 16:06:56.970055 init_service-0.7.0/init_service/templates/service/test/controllers/MicroserviceHelloWorldControllerSpec.scala
--rw-r--r--   0        0        0      902 2023-04-13 16:06:56.970055 init_service-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 init_service-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-03 15:11:14.374194 init_service-0.8.0/LICENSE
+-rw-r--r--   0        0        0      683 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/__init__.py
+-rw-r--r--   0        0        0    10535 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/init_service.py
+-rw-r--r--   0        0        0    50425 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/pyratemp.py
+-rw-r--r--   0        0        0      353 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/library/.gitignore
+-rw-r--r--   0        0        0      299 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/library/build.sbt
+-rw-r--r--   0        0        0      308 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/library/project/LibDependencies.scala
+-rw-r--r--   0        0        0       28 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/library/project/build.properties
+-rw-r--r--   0        0        0      369 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/library/project/plugins.sbt
+-rw-r--r--   0        0        0       82 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/library/src/main/scala/uk/gov/hmrc/hello/HelloWorld.scala
+-rw-r--r--   0        0        0      275 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/library/src/test/scala/uk/gov/hmrc/hello/HelloWorldSpec.scala
+-rw-r--r--   0        0        0      353 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/.gitignore
+-rw-r--r--   0        0        0       41 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/assets/stylesheets/application.scss
+-rw-r--r--   0        0        0      447 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/config/AppConfig.scala
+-rw-r--r--   0        0        0      626 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/config/ErrorHandler.scala
+-rw-r--r--   0        0        0      221 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/config/Module.scala
+-rw-r--r--   0        0        0      609 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/controllers/DocumentationController.scala
+-rw-r--r--   0        0        0      620 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/controllers/HelloWorldController.scala
+-rw-r--r--   0        0        0      503 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/controllers/MicroserviceHelloWorldController.scala
+-rw-r--r--   0        0        0      374 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/views/ErrorTemplate.scala.html
+-rw-r--r--   0        0        0      260 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/views/HelloWorldPage.scala.html
+-rw-r--r--   0        0        0      454 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/app/views/Layout.scala.html
+-rw-r--r--   0        0        0      994 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/build.sbt
+-rw-r--r--   0        0        0      472 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/conf/app.routes
+-rw-r--r--   0        0        0      300 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/conf/application-json-logger.xml
+-rw-r--r--   0        0        0     3081 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/conf/application.conf
+-rw-r--r--   0        0        0      266 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/conf/definition.routes
+-rw-r--r--   0        0        0     2337 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/conf/logback.xml
+-rw-r--r--   0        0        0       68 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/conf/messages
+-rw-r--r--   0        0        0       69 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/conf/messages.cy
+-rw-r--r--   0        0        0      511 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/conf/prod.routes
+-rw-r--r--   0        0        0     1098 2023-05-03 15:11:14.378194 init_service-0.8.0/init_service/templates/service/conf/testOnlyDoNotUseInAppConf.routes
+-rw-r--r--   0        0        0     1024 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/it/HealthEndpointIntegrationSpec.scala
+-rw-r--r--   0        0        0     1239 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/project/AppDependencies.scala
+-rw-r--r--   0        0        0      566 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/project/CodeCoverageSettings.scala
+-rw-r--r--   0        0        0       28 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/project/build.properties
+-rw-r--r--   0        0        0      770 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/project/plugins.sbt
+-rw-r--r--   0        0        0     1048 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/resources/conf/1.0/application.yaml
+-rw-r--r--   0        0        0       72 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/resources/conf/common/overview.md
+-rw-r--r--   0        0        0      361 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/resources/definition.json
+-rw-r--r--   0        0        0      232 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/template/API.delete
+-rw-r--r--   0        0        0      311 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/template/BACKEND.delete
+-rw-r--r--   0        0        0      194 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/template/FRONTEND.delete
+-rw-r--r--   0        0        0      914 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/test/config/ErrorHandlerSpec.scala
+-rw-r--r--   0        0        0     1119 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/test/controllers/HelloWorldControllerSpec.scala
+-rw-r--r--   0        0        0      623 2023-05-03 15:11:14.382195 init_service-0.8.0/init_service/templates/service/test/controllers/MicroserviceHelloWorldControllerSpec.scala
+-rw-r--r--   0        0        0      902 2023-05-03 15:11:14.382195 init_service-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 init_service-0.8.0/PKG-INFO
```

### Comparing `init_service-0.7.0/LICENSE` & `init_service-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/__init__.py` & `init_service-0.8.0/init_service/__init__.py`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/init_service.py` & `init_service-0.8.0/init_service/init_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         scala_version = "2.13.8"
         scala_binary_version = re.sub(r"\.(\d)*$", "", scala_version)
         print(f"scala_binary_version={scala_binary_version}")
         if self.type == "FRONTEND":
             bootstrap_play_version = self.get_latest_library_version(
                 "uk.gov.hmrc", "bootstrap-frontend-play-28", scala_binary_version
             )
-        elif self.type == "BACKEND":
+        elif self.type in ["BACKEND", "API"]:
             bootstrap_play_version = self.get_latest_library_version(
                 "uk.gov.hmrc", "bootstrap-backend-play-28", scala_binary_version
             )
         else:
             bootstrap_play_version = ""  # template won't use this
 
         play_frontend_hmrc_version = self.get_latest_library_version(
@@ -144,26 +144,24 @@
             command, shell=False, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
         ps_command.wait()
         return ps_command
 
     def create_project(self):
         if self.type == "LIBRARY":
-            template_dir = os.path.normpath(
-                os.path.join(os.path.abspath(__file__), "../templates/library")
-            )
+            template_location = "../templates/library"
             repository_type = "library"
-        elif self.type in ["FRONTEND", "BACKEND"]:
-            template_dir = os.path.normpath(
-                os.path.join(os.path.abspath(__file__), "../templates/service")
-            )
+        elif self.type in ["FRONTEND", "BACKEND", "API"]:
+            template_location = "../templates/service"
             repository_type = "service"
         else:
             raise Exception(f"ERROR: Invalid type '{self.type}'")
 
+        template_dir = os.path.normpath(os.path.join(os.path.abspath(__file__), template_location))
+
         print(f"project name: {self.repository}")
 
         if not self.dry_run:
             print(f"Cloning repo '{self.repository}'.")
             self.clone_repo()
 
         print(f"Creating new {repository_type}: {self.repository}, this could take a few moments")
```

### Comparing `init_service-0.7.0/init_service/pyratemp.py` & `init_service-0.8.0/init_service/pyratemp.py`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/app/config/ErrorHandler.scala` & `init_service-0.8.0/init_service/templates/service/app/config/ErrorHandler.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/app/controllers/HelloWorldController.scala` & `init_service-0.8.0/init_service/templates/service/app/controllers/HelloWorldController.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/conf/application.conf` & `init_service-0.8.0/init_service/templates/service/conf/application.conf`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # gtm.container property below to be one of a, b, c, d, e, f or sdes
 #tracking-consent-frontend {
 #  gtm.container = "<INSERT YOUR GTM CONTAINER LETTER HERE>"
 #}
 
 <!--(end)-->
 
-<!--(if type=="BACKEND")-->
+<!--(if type in ["BACKEND", "API"])-->
 include "backend.conf"
 
 # This is the main configuration file for the application.
 # ~~~~~
 
 appName = $!APP_NAME!$
```

### Comparing `init_service-0.7.0/init_service/templates/service/conf/logback.xml` & `init_service-0.8.0/init_service/templates/service/conf/logback.xml`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/conf/testOnlyDoNotUseInAppConf.routes` & `init_service-0.8.0/init_service/templates/service/conf/testOnlyDoNotUseInAppConf.routes`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/it/HealthEndpointIntegrationSpec.scala` & `init_service-0.8.0/init_service/templates/service/it/HealthEndpointIntegrationSpec.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/project/AppDependencies.scala` & `init_service-0.8.0/init_service/templates/service/project/AppDependencies.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/project/CodeCoverageSettings.scala` & `init_service-0.8.0/init_service/templates/service/project/CodeCoverageSettings.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/project/plugins.sbt` & `init_service-0.8.0/init_service/templates/service/project/plugins.sbt`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/test/config/ErrorHandlerSpec.scala` & `init_service-0.8.0/init_service/templates/service/test/config/ErrorHandlerSpec.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/test/controllers/HelloWorldControllerSpec.scala` & `init_service-0.8.0/init_service/templates/service/test/controllers/HelloWorldControllerSpec.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/init_service/templates/service/test/controllers/MicroserviceHelloWorldControllerSpec.scala` & `init_service-0.8.0/init_service/templates/service/test/controllers/MicroserviceHelloWorldControllerSpec.scala`

 * *Files identical despite different names*

### Comparing `init_service-0.7.0/pyproject.toml` & `init_service-0.8.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "init-service"
-version = "0.7.0"
+version = "0.8.0"
 description = "A templating tool for HMRC MDTP repositories"
 authors = ["Your Name <you@example.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
```

