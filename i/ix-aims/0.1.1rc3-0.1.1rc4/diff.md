# Comparing `tmp/ix_aims-0.1.1rc3.tar.gz` & `tmp/ix_aims-0.1.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ix_aims-0.1.1rc3.tar", max compression
+gzip compressed data, was "ix_aims-0.1.1rc4.tar", max compression
```

## Comparing `ix_aims-0.1.1rc3.tar` & `ix_aims-0.1.1rc4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.1rc3/README.md
--rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.1rc3/ix_aims/__init__.py
--rw-r--r--   0        0        0      123 2023-05-02 21:37:07.078194 ix_aims-0.1.1rc3/ix_aims/cli.py
--rw-r--r--   0        0        0      230 2023-05-02 21:58:44.236538 ix_aims-0.1.1rc3/ix_aims/imgs/__init__.py
--rw-r--r--   0        0        0      322 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc3/ix_aims/imgs/plusTab.png
--rw-r--r--   0        0        0     3615 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc3/ix_aims/imgs/processesBtn.png
--rw-r--r--   0        0        0     2201 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc3/ix_aims/imgs/yesBtn.png
--rw-r--r--   0        0        0     3649 2023-05-02 22:06:44.488732 ix_aims-0.1.1rc3/ix_aims/lib.py
--rw-r--r--   0        0        0      630 2023-05-02 22:06:53.460738 ix_aims-0.1.1rc3/pyproject.toml
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc3/setup.py
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc3/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.1rc4/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.1rc4/ix_aims/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-02 21:37:07.078194 ix_aims-0.1.1rc4/ix_aims/cli.py
+-rw-r--r--   0        0        0      230 2023-05-02 21:58:44.236538 ix_aims-0.1.1rc4/ix_aims/imgs/__init__.py
+-rw-r--r--   0        0        0      322 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc4/ix_aims/imgs/plusTab.png
+-rw-r--r--   0        0        0     3615 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc4/ix_aims/imgs/processesBtn.png
+-rw-r--r--   0        0        0     2201 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc4/ix_aims/imgs/yesBtn.png
+-rw-r--r--   0        0        0     3662 2023-05-02 22:08:47.556814 ix_aims-0.1.1rc4/ix_aims/lib.py
+-rw-r--r--   0        0        0      630 2023-05-02 22:08:55.024819 ix_aims-0.1.1rc4/pyproject.toml
+-rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc4/setup.py
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc4/PKG-INFO
```

### Comparing `ix_aims-0.1.1rc3/ix_aims/imgs/processesBtn.png` & `ix_aims-0.1.1rc4/ix_aims/imgs/processesBtn.png`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.1rc3/ix_aims/imgs/yesBtn.png` & `ix_aims-0.1.1rc4/ix_aims/imgs/yesBtn.png`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.1rc3/ix_aims/lib.py` & `ix_aims-0.1.1rc4/ix_aims/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 
     # Open iXCapture
     # Use this if working in RDP client to activate the write window
     # g.click(1000, 1000)
     open_ix_capture()
     sleep(10)
     go_to_processes_tab()
+    sleep(2)
     click_yes()
 
     for flight in flights:
         date = arrow.get(flight['acq_date'])
         sess = flight['sess_num']
         year = date.format('YYYY')
         doy = date.format('DDD')
```

### Comparing `ix_aims-0.1.1rc3/pyproject.toml` & `ix_aims-0.1.1rc4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ix-aims"
-version = "0.1.1rc3"
+version = "0.1.1rc4"
 description = "iX Capture automation with AIMS data"
 authors = ["Taylor Denouden <taylor.denouden@hakai.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ix_aims"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ix_aims-0.1.1rc3/setup.py` & `ix_aims-0.1.1rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['autoix = ix_aims.cli:main']}
 
 setup_kwargs = {
     'name': 'ix-aims',
-    'version': '0.1.1rc3',
+    'version': '0.1.1rc4',
     'description': 'iX Capture automation with AIMS data',
     'long_description': '# auto-ix-capture\n',
     'author': 'Taylor Denouden',
     'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ix_aims-0.1.1rc3/PKG-INFO` & `ix_aims-0.1.1rc4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ix-aims
-Version: 0.1.1rc3
+Version: 0.1.1rc4
 Summary: iX Capture automation with AIMS data
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

