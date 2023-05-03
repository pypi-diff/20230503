# Comparing `tmp/lockss_turtles-0.4.0.dev2.tar.gz` & `tmp/lockss_turtles-0.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockss_turtles-0.4.0.dev2.tar", max compression
+gzip compressed data, was "lockss_turtles-0.4.0.dev3.tar", max compression
```

## Comparing `lockss_turtles-0.4.0.dev2.tar` & `lockss_turtles-0.4.0.dev3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3158 2023-04-07 16:33:57.473442 lockss_turtles-0.4.0.dev2/CHANGELOG.rst
--rw-r--r--   0        0        0     1506 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/LICENSE
--rw-r--r--   0        0        0    38149 2023-05-02 19:16:12.800240 lockss_turtles-0.4.0.dev2/README.rst
--rw-r--r--   0        0        0     1001 2023-05-02 19:16:18.990341 lockss_turtles-0.4.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     3201 2023-05-02 19:17:04.874415 lockss_turtles-0.4.0.dev2/src/lockss/turtles/__init__.py
--rw-r--r--   0        0        0     1633 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/__main__.py
--rw-r--r--   0        0        0     9074 2023-03-28 03:37:09.141564 lockss_turtles-0.4.0.dev2/src/lockss/turtles/app.py
--rw-r--r--   0        0        0    22480 2023-04-07 16:33:57.473442 lockss_turtles-0.4.0.dev2/src/lockss/turtles/cli.py
--rw-r--r--   0        0        0     4312 2023-03-28 04:09:36.841384 lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin.py
--rw-r--r--   0        0        0     9445 2023-03-28 04:13:05.571566 lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin_registry.py
--rw-r--r--   0        0        0    10486 2023-03-28 03:40:12.508020 lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin_set.py
--rw-r--r--   0        0        0     1579 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/__init__.py
--rw-r--r--   0        0        0      685 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-registry-catalog-schema.json
--rw-r--r--   0        0        0     2766 2023-03-28 04:02:43.557727 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-registry-schema.json
--rw-r--r--   0        0        0      650 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-set-catalog-schema.json
--rw-r--r--   0        0        0     2338 2023-03-04 21:54:35.657031 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-set-schema.json
--rw-r--r--   0        0        0      753 2023-03-06 06:11:17.982107 lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-signing-credentials-schema.json
--rw-r--r--   0        0        0     2430 2023-03-04 08:36:28.933873 lockss_turtles-0.4.0.dev2/src/lockss/turtles/util.py
--rw-r--r--   0        0        0    39406 1970-01-01 00:00:00.000000 lockss_turtles-0.4.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0     3158 2023-04-06 06:42:02.921705 lockss_turtles-0.4.0.dev3/CHANGELOG.rst
+-rw-r--r--   0        0        0     1506 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev3/LICENSE
+-rw-r--r--   0        0        0    38149 2023-05-03 16:01:32.089503 lockss_turtles-0.4.0.dev3/README.rst
+-rw-r--r--   0        0        0     1001 2023-05-03 16:01:38.442972 lockss_turtles-0.4.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     3201 2023-05-03 16:02:06.153555 lockss_turtles-0.4.0.dev3/src/lockss/turtles/__init__.py
+-rw-r--r--   0        0        0     1633 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev3/src/lockss/turtles/__main__.py
+-rw-r--r--   0        0        0     9074 2023-04-06 06:32:04.687811 lockss_turtles-0.4.0.dev3/src/lockss/turtles/app.py
+-rw-r--r--   0        0        0    22476 2023-05-03 15:57:35.377335 lockss_turtles-0.4.0.dev3/src/lockss/turtles/cli.py
+-rw-r--r--   0        0        0     4312 2023-04-06 06:32:04.691144 lockss_turtles-0.4.0.dev3/src/lockss/turtles/plugin.py
+-rw-r--r--   0        0        0     9445 2023-04-06 06:32:04.691144 lockss_turtles-0.4.0.dev3/src/lockss/turtles/plugin_registry.py
+-rw-r--r--   0        0        0    10486 2023-04-06 06:32:04.691144 lockss_turtles-0.4.0.dev3/src/lockss/turtles/plugin_set.py
+-rw-r--r--   0        0        0     1579 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/__init__.py
+-rw-r--r--   0        0        0      685 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-registry-catalog-schema.json
+-rw-r--r--   0        0        0     2766 2023-04-06 06:32:04.691144 lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-registry-schema.json
+-rw-r--r--   0        0        0      650 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-set-catalog-schema.json
+-rw-r--r--   0        0        0     2338 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-set-schema.json
+-rw-r--r--   0        0        0      753 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-signing-credentials-schema.json
+-rw-r--r--   0        0        0     2430 2023-03-07 22:41:03.875719 lockss_turtles-0.4.0.dev3/src/lockss/turtles/util.py
+-rw-r--r--   0        0        0    39406 1970-01-01 00:00:00.000000 lockss_turtles-0.4.0.dev3/PKG-INFO
```

### Comparing `lockss_turtles-0.4.0.dev2/CHANGELOG.rst` & `lockss_turtles-0.4.0.dev3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/LICENSE` & `lockss_turtles-0.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/README.rst` & `lockss_turtles-0.4.0.dev3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =======
 Turtles
 =======
 
-.. |RELEASE| replace:: 0.4.0-dev2
+.. |RELEASE| replace:: 0.4.0-dev3
 .. |RELEASE_DATE| replace:: ?
 
 .. |HELP| replace:: ``--help/-h``
 .. |IDENTIFIER| replace:: ``--identifier/-i``
 .. |IDENTIFIERS| replace:: ``--identifiers/-I``
 .. |JAR| replace:: ``--jar/-j``
 .. |JARS| replace:: ``--jars/-J``
```

### Comparing `lockss_turtles-0.4.0.dev2/pyproject.toml` & `lockss_turtles-0.4.0.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lockss-turtles"
-version = "0.4.0-dev2"
+version = "0.4.0-dev3"
 description = "Tool to manage LOCKSS plugin sets and LOCKSS plugin registries"
 license = "BSD-3-Clause"
 authors = [
     "Thib Guicherd-Callin <thib@cs.stanford.edu>"
 ]
 readme = "README.rst"
 homepage = "https://www.lockss.org/"
```

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/__init__.py` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '0.4.0-dev2'
+__version__ = '0.4.0-dev3'
 
 __copyright__ = '''
 Copyright (c) 2000-2023, Board of Trustees of Leland Stanford Jr. University
 '''.strip()
 
 __license__ = __copyright__ + '\n\n' + '''
 Redistribution and use in source and binary forms, with or without
```

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/__main__.py` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/__main__.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/app.py` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/app.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/cli.py` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                                 headers=['Plugin JAR', 'Plugin identifier', 'Plugin version', 'Plugin registry', 'Plugin registry layer', 'Deployed JAR'],
                                 tablefmt=self._args.output_format))
 
     def _get_identifiers(self):
         if self._identifiers is None:
             self._identifiers = list()
             self._identifiers.extend(self._args.remainder)
-            self._identifiers.extend(self._args.get_identifier)
+            self._identifiers.extend(self._args.identifier)
             for path in self._args.identifiers:
                 self._identifiers.extend(_file_lines(path))
             if len(self._identifiers) == 0:
                 self._parser.error('list of plugin identifiers to build is empty')
         return self._identifiers
 
     def _get_jars(self):
```

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin.py` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/plugin.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin_registry.py` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/plugin_set.py` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/plugin_set.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/__init__.py` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-registry-catalog-schema.json` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-registry-catalog-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-registry-schema.json` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-registry-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-set-catalog-schema.json` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-set-catalog-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-set-schema.json` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-set-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/resources/plugin-signing-credentials-schema.json` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/resources/plugin-signing-credentials-schema.json`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/src/lockss/turtles/util.py` & `lockss_turtles-0.4.0.dev3/src/lockss/turtles/util.py`

 * *Files identical despite different names*

### Comparing `lockss_turtles-0.4.0.dev2/PKG-INFO` & `lockss_turtles-0.4.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockss-turtles
-Version: 0.4.0.dev2
+Version: 0.4.0.dev3
 Summary: Tool to manage LOCKSS plugin sets and LOCKSS plugin registries
 Home-page: https://www.lockss.org/
 License: BSD-3-Clause
 Author: Thib Guicherd-Callin
 Author-email: thib@cs.stanford.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,15 +29,15 @@
 Project-URL: Repository, https://github.com/lockss/lockss-turtles
 Description-Content-Type: text/x-rst
 
 =======
 Turtles
 =======
 
-.. |RELEASE| replace:: 0.4.0-dev2
+.. |RELEASE| replace:: 0.4.0-dev3
 .. |RELEASE_DATE| replace:: ?
 
 .. |HELP| replace:: ``--help/-h``
 .. |IDENTIFIER| replace:: ``--identifier/-i``
 .. |IDENTIFIERS| replace:: ``--identifiers/-I``
 .. |JAR| replace:: ``--jar/-j``
 .. |JARS| replace:: ``--jars/-J``
```

