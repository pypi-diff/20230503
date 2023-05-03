# Comparing `tmp/libtado-3.5.1.tar.gz` & `tmp/libtado-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libtado-3.5.1.tar", last modified: Tue Oct  4 13:09:56 2022, max compression
+gzip compressed data, was "dist/libtado-3.6.0.tar", last modified: Wed May  3 06:54:09 2023, max compression
```

## Comparing `libtado-3.5.1.tar` & `libtado-3.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 13:09:56.000000 libtado-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-10-04 13:09:56.000000 libtado-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2622 2022-10-04 13:09:46.000000 libtado-3.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 13:09:56.000000 libtado-3.5.1/libtado/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 13:09:46.000000 libtado-3.5.1/libtado/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17509 2022-10-04 13:09:46.000000 libtado-3.5.1/libtado/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    46255 2022-10-04 13:09:46.000000 libtado-3.5.1/libtado/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 13:09:56.000000 libtado-3.5.1/libtado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-10-04 13:09:56.000000 libtado-3.5.1/libtado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-10-04 13:09:56.000000 libtado-3.5.1/libtado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 13:09:56.000000 libtado-3.5.1/libtado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-04 13:09:56.000000 libtado-3.5.1/libtado.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-04 13:09:56.000000 libtado-3.5.1/libtado.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-04 13:09:56.000000 libtado-3.5.1/libtado.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-10-04 13:09:47.000000 libtado-3.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-04 13:09:56.000000 libtado-3.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-04 13:09:47.000000 libtado-3.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 13:09:56.000000 libtado-3.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 13:09:46.000000 libtado-3.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 13:09:46.000000 libtado-3.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:54:09.000000 libtado-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-03 06:54:09.000000 libtado-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-03 06:53:53.000000 libtado-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:53:53.000000 libtado-3.6.0/libtado/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18009 2023-05-03 06:53:53.000000 libtado-3.6.0/libtado/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46255 2023-05-03 06:53:53.000000 libtado-3.6.0/libtado/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-03 06:53:54.000000 libtado-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 06:54:09.000000 libtado-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 06:53:54.000000 libtado-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:54:09.000000 libtado-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:53:53.000000 libtado-3.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:53:53.000000 libtado-3.6.0/tests/conftest.py
```

### Comparing `libtado-3.5.1/README.md` & `libtado-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `libtado-3.5.1/libtado/__main__.py` & `libtado-3.6.0/libtado/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,22 @@
       # V2 smart radiator thermostat
       click.echo('Serial: %s' % d['serialNo'])
       click.echo('Type: %s' % d['deviceType'])
       click.echo('Firmware: %s' % d['currentFwVersion'])
       click.echo('Connection: %s (%s)' % (d['connectionState']['value'], d['connectionState']['timestamp']))
       click.echo('Mounted: %s (%s)' % (d['mountingState']['value'], d['mountingState']['timestamp']))
       click.echo('Battery State: %s' % d['batteryState'])
+    elif d['deviceType'] == 'VA02E':
+      # V2 smart radiator thermostat Basic
+      click.echo('Serial: %s' % d['serialNo'])
+      click.echo('Type: %s' % d['deviceType'])
+      click.echo('Firmware: %s' % d['currentFwVersion'])
+      click.echo('Connection: %s (%s)' % (d['connectionState']['value'], d['connectionState']['timestamp']))
+      click.echo('Mounted: %s (%s)' % (d['mountingState']['value'], d['mountingState']['timestamp']))
+      click.echo('Battery State: %s' % d['batteryState'])
     elif d['deviceType'] == 'RU02':
       # V2 smart wall theromstat
       click.echo('Serial: %s' % d['serialNo'])
       click.echo('Type: %s' % d['deviceType'])
       click.echo('Firmware: %s' % d['currentFwVersion'])
       click.echo('Connection: %s (%s)' % (d['connectionState']['value'], d['connectionState']['timestamp']))
       click.echo('Battery State: %s' % d['batteryState'])
```

### Comparing `libtado-3.5.1/libtado/api.py` & `libtado-3.6.0/libtado/api.py`

 * *Files identical despite different names*

### Comparing `libtado-3.5.1/pyproject.toml` & `libtado-3.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libtado"
-version = "3.5.1",
+version = "3.6.0",
 authors = [
   { name="Germain Lefebvre", email="germainlefebvre4@gmail.com" },
 ]
 description = "A library (and a command line client) to control your Tado Smart Thermostat."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `libtado-3.5.1/setup.py` & `libtado-3.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name='libtado',
-  version='3.5.1',
+  version='3.6.0',
   author='Germain Lefebvre',
   author_email='germainlefebvre4@gmail.com',
   description='A library (and a command line client) to control your Tado Smart Thermostat.',
   url='https://github.com/germainlefebvre4/libtado',
   license='GPLv3+',
   packages=find_packages(),
   classifiers=[
```

