# Comparing `tmp/pyfem-0.0.1.tar.gz` & `tmp/pyfem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.0.1.tar", last modified: Thu Apr 13 08:03:30 2023, max compression
+gzip compressed data, was "pyfem-0.0.2.tar", last modified: Wed May  3 10:38:13 2023, max compression
```

## Comparing `pyfem-0.0.1.tar` & `pyfem-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 08:03:30.384678 pyfem-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-04-13 07:21:12.000000 pyfem-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      570 2023-04-13 08:03:30.384678 pyfem-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-04-13 07:21:12.000000 pyfem-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 08:03:30.384678 pyfem-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-04-13 08:02:19.000000 pyfem-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:03:30.376701 pyfem-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 08:03:30.380678 pyfem-0.0.1/src/pyfem/
--rw-rw-rw-   0        0        0        0 2022-08-16 03:54:46.000000 pyfem-0.0.1/src/pyfem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:03:30.383678 pyfem-0.0.1/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0      570 2023-04-13 08:03:30.000000 pyfem-0.0.1/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-04-13 08:03:30.000000 pyfem-0.0.1/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 08:03:30.000000 pyfem-0.0.1/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 08:03:30.000000 pyfem-0.0.1/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.860701 pyfem-0.0.2/
+-rw-rw-rw-   0        0        0    11524 2023-05-03 09:58:16.000000 pyfem-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      535 2023-05-03 10:38:13.860206 pyfem-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-05-03 09:58:16.000000 pyfem-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 10:38:13.860701 pyfem-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-05-03 10:37:50.000000 pyfem-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.821477 pyfem-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.836397 pyfem-0.0.2/src/pyfem/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-03 10:34:48.000000 pyfem-0.0.2/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.846813 pyfem-0.0.2/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.848301 pyfem-0.0.2/src/pyfem/elements/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.849789 pyfem-0.0.2/src/pyfem/fem/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/fem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.851774 pyfem-0.0.2/src/pyfem/io/
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:26:23.000000 pyfem-0.0.2/src/pyfem/io/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.853263 pyfem-0.0.2/src/pyfem/materials/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/materials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.855247 pyfem-0.0.2/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.856735 pyfem-0.0.2/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/solvers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.858222 pyfem-0.0.2/src/pyfem/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.2/src/pyfem/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:38:13.845325 pyfem-0.0.2/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-03 10:38:13.000000 pyfem-0.0.2/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.0.1/LICENSE` & `pyfem-0.0.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-                                 Apache License
+Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
 
@@ -194,8 +194,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `pyfem-0.0.1/PKG-INFO` & `pyfem-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.1
+Version: 0.0.2
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfem
-A finite element package in python.
+
```

### Comparing `pyfem-0.0.1/setup.py` & `pyfem-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.0.1",
+    version="0.0.2",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
@@ -18,9 +18,14 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.10",
+    python_requires=">=3.9",
+    entry_points={
+        'console_scripts': [
+            'pyfem=pyfem.__main__:main'
+        ]
+    }
 )
```

### Comparing `pyfem-0.0.1/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.0.2/src/pyfem.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.1
+Version: 0.0.2
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfem
-A finite element package in python.
+
```

