# Comparing `tmp/wombatoo-0.0.1.tar.gz` & `tmp/wombatoo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Prashant\Desktop\wombato\dist\.tmp-p3d4avns\wombatoo-0.0.1.tar", last modified: Wed May  3 03:54:35 2023, max compression
+gzip compressed data, was "C:\Users\Prashant\Desktop\wombato\dist\.tmp-hk2i6lxh\wombatoo-0.0.2.tar", last modified: Wed May  3 04:23:59 2023, max compression
```

## Comparing `wombatoo-0.0.1.tar` & `wombatoo-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:54:35.000000 wombatoo-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      320 2023-05-03 03:54:35.000000 wombatoo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombatoo-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 03:54:35.000000 wombatoo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      887 2023-05-03 03:54:10.000000 wombatoo-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:54:35.000000 wombatoo-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombatoo-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     9597 2023-05-03 03:53:25.000000 wombatoo-0.0.1/src/wombatoo.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:54:35.000000 wombatoo-0.0.1/wombatoo.egg-info/
--rw-rw-rw-   0        0        0      320 2023-05-03 03:54:35.000000 wombatoo-0.0.1/wombatoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-05-03 03:54:35.000000 wombatoo-0.0.1/wombatoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:54:35.000000 wombatoo-0.0.1/wombatoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-03 03:54:35.000000 wombatoo-0.0.1/wombatoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-03 03:54:35.000000 wombatoo-0.0.1/wombatoo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 04:23:59.000000 wombatoo-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0      320 2023-05-03 04:23:59.000000 wombatoo-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombatoo-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 04:23:59.000000 wombatoo-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      887 2023-05-03 04:22:22.000000 wombatoo-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 04:23:59.000000 wombatoo-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombatoo-0.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     9597 2023-05-03 03:53:25.000000 wombatoo-0.0.2/src/wombatoo.py
+drwxrwxrwx   0        0        0        0 2023-05-03 04:23:59.000000 wombatoo-0.0.2/wombatoo.egg-info/
+-rw-rw-rw-   0        0        0      320 2023-05-03 04:23:58.000000 wombatoo-0.0.2/wombatoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-05-03 04:23:58.000000 wombatoo-0.0.2/wombatoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 04:23:58.000000 wombatoo-0.0.2/wombatoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-03 04:23:58.000000 wombatoo-0.0.2/wombatoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-03 04:23:58.000000 wombatoo-0.0.2/wombatoo.egg-info/top_level.txt
```

### Comparing `wombatoo-0.0.1/LICENSE.md` & `wombatoo-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wombatoo-0.0.1/setup.py` & `wombatoo-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 
 setup(
     name="wombatoo",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(exclude=["tests", "examples", "docs"]),
     include_package_data=True,
     description="A Data-Ops tool for devs",
     long_description="Please refer to: README",
     long_description_content_type="text/markdown",
     url="https://github.com/prashdash112/wombat",
     author="Prashant Singh",
     # classifiers=[
     #     "Programming Language :: Python :: 3 :: Only",
     #     "Programming Language :: Python :: 3.8",
     #     "Programming Language :: Python :: 3.9"
     # ],
     license="Please refer to the readme",
-    python_requires=">=3.8",
+    python_requires=">=3.6",
     install_requires=["numpy==1.23.5",
                       "pandas==1.5.2",
                       "pyhtml2pdf==0.0.6",
                       "ydata-profiling==4.1.1"]
                       )
```

### Comparing `wombatoo-0.0.1/src/wombatoo.py` & `wombatoo-0.0.2/src/wombatoo.py`

 * *Files identical despite different names*

