# Comparing `tmp/geosdemo-haoyu-0.0.1.tar.gz` & `tmp/geosdemo-haoyu-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosdemo-haoyu-0.0.1.tar", last modified: Tue Apr 25 20:48:26 2023, max compression
+gzip compressed data, was "geosdemo-haoyu-0.1.0.tar", last modified: Wed May  3 19:41:03 2023, max compression
```

## Comparing `geosdemo-haoyu-0.0.1.tar` & `geosdemo-haoyu-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 20:48:26.550764 geosdemo-haoyu-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-04-25 20:29:12.000000 geosdemo-haoyu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-25 20:29:12.000000 geosdemo-haoyu-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1185 2023-04-25 20:48:26.551764 geosdemo-haoyu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-04-25 20:29:12.000000 geosdemo-haoyu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 20:48:26.544245 geosdemo-haoyu-0.0.1/geosdemo_haoyu/
--rw-rw-rw-   0        0        0      129 2023-04-25 20:29:12.000000 geosdemo-haoyu-0.0.1/geosdemo_haoyu/__init__.py
--rw-rw-rw-   0        0        0      194 2023-04-25 20:29:12.000000 geosdemo-haoyu-0.0.1/geosdemo_haoyu/common.py
--rw-rw-rw-   0        0        0       20 2023-04-25 20:29:12.000000 geosdemo-haoyu-0.0.1/geosdemo_haoyu/geosdemo_haoyu.py
-drwxrwxrwx   0        0        0        0 2023-04-25 20:48:26.549750 geosdemo-haoyu-0.0.1/geosdemo_haoyu.egg-info/
--rw-rw-rw-   0        0        0     1185 2023-04-25 20:48:26.000000 geosdemo-haoyu-0.0.1/geosdemo_haoyu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-25 20:48:26.000000 geosdemo-haoyu-0.0.1/geosdemo_haoyu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 20:48:26.000000 geosdemo-haoyu-0.0.1/geosdemo_haoyu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-25 20:48:26.000000 geosdemo-haoyu-0.0.1/geosdemo_haoyu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-04-25 20:48:26.000000 geosdemo-haoyu-0.0.1/geosdemo_haoyu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-25 20:29:12.000000 geosdemo-haoyu-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      422 2023-04-25 20:48:26.552754 geosdemo-haoyu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1777 2023-04-25 20:29:12.000000 geosdemo-haoyu-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:41:03.955147 geosdemo-haoyu-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 19:40:47.000000 geosdemo-haoyu-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-03 19:40:47.000000 geosdemo-haoyu-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-03 19:41:03.955147 geosdemo-haoyu-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-03 19:40:47.000000 geosdemo-haoyu-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:41:03.955147 geosdemo-haoyu-0.1.0/geosdemo_haoyu/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 19:40:47.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 19:40:47.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-03 19:40:47.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-03 19:40:47.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu/geosdemo_haoyu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:41:03.955147 geosdemo-haoyu-0.1.0/geosdemo_haoyu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-03 19:41:03.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 19:41:03.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 19:41:03.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:41:03.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 19:41:03.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 19:41:03.000000 geosdemo-haoyu-0.1.0/geosdemo_haoyu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 19:40:47.000000 geosdemo-haoyu-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-03 19:41:03.955147 geosdemo-haoyu-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-03 19:40:47.000000 geosdemo-haoyu-0.1.0/setup.py
```

### Comparing `geosdemo-haoyu-0.0.1/LICENSE` & `geosdemo-haoyu-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Haoyu Niu
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Haoyu Niu
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `geosdemo-haoyu-0.0.1/PKG-INFO` & `geosdemo-haoyu-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: geosdemo-haoyu
-Version: 0.0.1
-Summary: A python package for interactive mapping.
-Home-page: https://github.com/hniu-tamu/geosdemo-haoyu
-Author: Haoyu Niu
-Author-email: hniu@tamu.edu
-License: MIT license
-Keywords: geosdemo_haoyu
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# geosdemo-haoyu
-
-
-[![image](https://img.shields.io/pypi/v/geosdemo-haoyu.svg)](https://pypi.python.org/pypi/geosdemo-haoyu)
-[![image](https://img.shields.io/conda/vn/conda-forge/geosdemo-haoyu.svg)](https://anaconda.org/conda-forge/geosdemo-haoyu)
-
-
-**A python package for interactive mapping.**
-
-
--   Free software: MIT license
--   Documentation: https://hniu-tamu.github.io/geosdemo-haoyu
-    
-
-## Features
-
--   TODO
+Metadata-Version: 2.1
+Name: geosdemo-haoyu
+Version: 0.1.0
+Summary: A python package for interactive mapping.
+Home-page: https://github.com/hniu-tamu/geosdemo-haoyu
+Author: Haoyu Niu
+Author-email: hniu@tamu.edu
+License: MIT license
+Keywords: geosdemo_haoyu
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# geosdemo-haoyu
+
+
+[![image](https://img.shields.io/pypi/v/geosdemo-haoyu.svg)](https://pypi.python.org/pypi/geosdemo-haoyu)
+[![image](https://img.shields.io/conda/vn/conda-forge/geosdemo-haoyu.svg)](https://anaconda.org/conda-forge/geosdemo-haoyu)
+
+
+**A python package for interactive mapping.**
+
+
+-   Free software: MIT license
+-   Documentation: https://hniu-tamu.github.io/geosdemo-haoyu
+    
+
+## Features
+
+-   TODO
```

### Comparing `geosdemo-haoyu-0.0.1/geosdemo_haoyu.egg-info/PKG-INFO` & `geosdemo-haoyu-0.1.0/geosdemo_haoyu.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: geosdemo-haoyu
-Version: 0.0.1
-Summary: A python package for interactive mapping.
-Home-page: https://github.com/hniu-tamu/geosdemo-haoyu
-Author: Haoyu Niu
-Author-email: hniu@tamu.edu
-License: MIT license
-Keywords: geosdemo_haoyu
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# geosdemo-haoyu
-
-
-[![image](https://img.shields.io/pypi/v/geosdemo-haoyu.svg)](https://pypi.python.org/pypi/geosdemo-haoyu)
-[![image](https://img.shields.io/conda/vn/conda-forge/geosdemo-haoyu.svg)](https://anaconda.org/conda-forge/geosdemo-haoyu)
-
-
-**A python package for interactive mapping.**
-
-
--   Free software: MIT license
--   Documentation: https://hniu-tamu.github.io/geosdemo-haoyu
-    
-
-## Features
-
--   TODO
+Metadata-Version: 2.1
+Name: geosdemo-haoyu
+Version: 0.1.0
+Summary: A python package for interactive mapping.
+Home-page: https://github.com/hniu-tamu/geosdemo-haoyu
+Author: Haoyu Niu
+Author-email: hniu@tamu.edu
+License: MIT license
+Keywords: geosdemo_haoyu
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# geosdemo-haoyu
+
+
+[![image](https://img.shields.io/pypi/v/geosdemo-haoyu.svg)](https://pypi.python.org/pypi/geosdemo-haoyu)
+[![image](https://img.shields.io/conda/vn/conda-forge/geosdemo-haoyu.svg)](https://anaconda.org/conda-forge/geosdemo-haoyu)
+
+
+**A python package for interactive mapping.**
+
+
+-   Free software: MIT license
+-   Documentation: https://hniu-tamu.github.io/geosdemo-haoyu
+    
+
+## Features
+
+-   TODO
```

### Comparing `geosdemo-haoyu-0.0.1/setup.py` & `geosdemo-haoyu-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = [ ]
-
-test_requirements = [ ]
-
-setup(
-    author="Haoyu Niu",
-    author_email='hniu@tamu.edu',
-    python_requires='>=3.8',
-    classifiers=[
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
-    description="A python package for interactive mapping.",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='geosdemo_haoyu',
-    name='geosdemo-haoyu',
-    packages=find_packages(include=['geosdemo_haoyu', 'geosdemo_haoyu.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/hniu-tamu/geosdemo-haoyu',
-    version='0.0.1',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = [ ]
+
+test_requirements = [ ]
+
+setup(
+    author="Haoyu Niu",
+    author_email='hniu@tamu.edu',
+    python_requires='>=3.8',
+    classifiers=[
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ],
+    description="A python package for interactive mapping.",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='geosdemo_haoyu',
+    name='geosdemo-haoyu',
+    packages=find_packages(include=['geosdemo_haoyu', 'geosdemo_haoyu.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/hniu-tamu/geosdemo-haoyu',
+    version='0.1.0',
+    zip_safe=False,
+)
```

