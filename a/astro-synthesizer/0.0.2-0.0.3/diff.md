# Comparing `tmp/astro-synthesizer-0.0.2.tar.gz` & `tmp/astro-synthesizer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-synthesizer-0.0.2.tar", last modified: Sun Apr  2 17:47:19 2023, max compression
+gzip compressed data, was "astro-synthesizer-0.0.3.tar", last modified: Wed May  3 10:41:09 2023, max compression
```

## Comparing `astro-synthesizer-0.0.2.tar` & `astro-synthesizer-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-04-02 17:47:19.158745 astro-synthesizer-0.0.2/
--rw-rw-r--   0 jz        (1000) jz        (1000)    35149 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/LICENSE
--rw-rw-r--   0 jz        (1000) jz        (1000)    43841 2023-04-02 17:47:19.154744 astro-synthesizer-0.0.2/PKG-INFO
--rw-rw-r--   0 jz        (1000) jz        (1000)     2796 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/README.md
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-04-02 17:47:19.154744 astro-synthesizer-0.0.2/astro_synthesizer.egg-info/
--rw-rw-r--   0 jz        (1000) jz        (1000)    43841 2023-04-02 17:47:19.000000 astro-synthesizer-0.0.2/astro_synthesizer.egg-info/PKG-INFO
--rw-rw-r--   0 jz        (1000) jz        (1000)     1191 2023-04-02 17:47:19.000000 astro-synthesizer-0.0.2/astro_synthesizer.egg-info/SOURCES.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)        1 2023-04-02 17:47:19.000000 astro-synthesizer-0.0.2/astro_synthesizer.egg-info/dependency_links.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)       63 2023-04-02 17:47:19.000000 astro-synthesizer-0.0.2/astro_synthesizer.egg-info/entry_points.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)       78 2023-04-02 17:47:19.000000 astro-synthesizer-0.0.2/astro_synthesizer.egg-info/requires.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)       12 2023-04-02 17:47:19.000000 astro-synthesizer-0.0.2/astro_synthesizer.egg-info/top_level.txt
--rw-rw-r--   0 jz        (1000) jz        (1000)      864 2023-04-02 17:46:41.000000 astro-synthesizer-0.0.2/pyproject.toml
--rw-rw-r--   0 jz        (1000) jz        (1000)       38 2023-04-02 17:47:19.158745 astro-synthesizer-0.0.2/setup.cfg
--rw-rw-r--   0 jz        (1000) jz        (1000)       38 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/setup.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-04-02 17:47:19.154744 astro-synthesizer-0.0.2/synthesizer/
--rw-rw-r--   0 jz        (1000) jz        (1000)      919 2023-04-02 17:47:04.000000 astro-synthesizer-0.0.2/synthesizer/__main__.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-04-02 17:47:19.154744 astro-synthesizer-0.0.2/synthesizer/dustmixer/
--rw-rw-r--   0 jz        (1000) jz        (1000)       28 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/dustmixer/__init__.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     4887 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/dustmixer/bhcoat.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     5773 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/dustmixer/bhmie.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    34437 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/dustmixer/dustmixer.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-04-02 17:47:19.154744 astro-synthesizer-0.0.2/synthesizer/gridder/
--rw-rw-r--   0 jz        (1000) jz        (1000)      165 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/gridder/__init__.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     4610 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/gridder/amr_reader.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    17922 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/gridder/analytical.py
--rw-rw-r--   0 jz        (1000) jz        (1000)      819 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/gridder/custom_model.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    23722 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/gridder/gridder.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     7619 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/gridder/models.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    10315 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/gridder/sph_reader.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     3922 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/gridder/vector_field.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    13914 2023-04-02 17:46:49.000000 astro-synthesizer-0.0.2/synthesizer/parser.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    43241 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/pipeline.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-04-02 17:47:19.154744 astro-synthesizer-0.0.2/synthesizer/raytrace/
--rw-rw-r--   0 jz        (1000) jz        (1000)       29 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/raytrace/__init__.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    15204 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/raytrace/radmc3d.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-04-02 17:47:19.154744 astro-synthesizer-0.0.2/synthesizer/synobs/
--rw-rw-r--   0 jz        (1000) jz        (1000)       66 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/synobs/__init__.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    19644 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/synobs/scripter.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     2861 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/synobs/syn_imager.py
-drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-04-02 17:47:19.154744 astro-synthesizer-0.0.2/synthesizer/synobs/templates/
--rw-rw-r--   0 jz        (1000) jz        (1000)     1519 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/synobs/templates/alma_1.3mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1698 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/synobs/templates/alma_1.3mm_pol.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1692 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/synobs/templates/alma_3mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1619 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/synobs/templates/vla_18mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1588 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/synobs/templates/vla_7mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)     1597 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/synobs/templates/vla_9mm.py
--rw-rw-r--   0 jz        (1000) jz        (1000)    27401 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.2/synthesizer/utils.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.895515 astro-synthesizer-0.0.3/
+-rw-rw-r--   0 jz        (1000) jz        (1000)    35149 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/LICENSE
+-rw-rw-r--   0 jz        (1000) jz        (1000)    43841 2023-05-03 10:41:09.895515 astro-synthesizer-0.0.3/PKG-INFO
+-rw-rw-r--   0 jz        (1000) jz        (1000)     2796 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/README.md
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.887515 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/
+-rw-rw-r--   0 jz        (1000) jz        (1000)    43841 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/PKG-INFO
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1191 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)        1 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)       63 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/entry_points.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)       78 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/requires.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)       12 2023-05-03 10:41:09.000000 astro-synthesizer-0.0.3/astro_synthesizer.egg-info/top_level.txt
+-rw-rw-r--   0 jz        (1000) jz        (1000)      864 2023-05-03 10:39:54.000000 astro-synthesizer-0.0.3/pyproject.toml
+-rw-rw-r--   0 jz        (1000) jz        (1000)       38 2023-05-03 10:41:09.895515 astro-synthesizer-0.0.3/setup.cfg
+-rw-rw-r--   0 jz        (1000) jz        (1000)       38 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/setup.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.887515 astro-synthesizer-0.0.3/synthesizer/
+-rw-rw-r--   0 jz        (1000) jz        (1000)      919 2023-05-03 10:40:23.000000 astro-synthesizer-0.0.3/synthesizer/__main__.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.887515 astro-synthesizer-0.0.3/synthesizer/dustmixer/
+-rw-rw-r--   0 jz        (1000) jz        (1000)       28 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/dustmixer/__init__.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     4887 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/dustmixer/bhcoat.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     5773 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/dustmixer/bhmie.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    34563 2023-04-26 10:11:51.000000 astro-synthesizer-0.0.3/synthesizer/dustmixer/dustmixer.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.891515 astro-synthesizer-0.0.3/synthesizer/gridder/
+-rw-rw-r--   0 jz        (1000) jz        (1000)      165 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/gridder/__init__.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     5170 2023-04-13 15:55:46.000000 astro-synthesizer-0.0.3/synthesizer/gridder/amr_reader.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    20285 2023-04-14 07:03:56.000000 astro-synthesizer-0.0.3/synthesizer/gridder/analytical.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)      819 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/gridder/custom_model.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    26881 2023-05-03 10:40:33.000000 astro-synthesizer-0.0.3/synthesizer/gridder/gridder.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    13982 2023-04-14 08:05:22.000000 astro-synthesizer-0.0.3/synthesizer/gridder/models.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    12533 2023-04-08 22:10:38.000000 astro-synthesizer-0.0.3/synthesizer/gridder/sph_reader.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     3922 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/gridder/vector_field.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    14290 2023-05-03 10:40:10.000000 astro-synthesizer-0.0.3/synthesizer/parser.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    44280 2023-05-03 10:40:31.000000 astro-synthesizer-0.0.3/synthesizer/pipeline.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.891515 astro-synthesizer-0.0.3/synthesizer/raytrace/
+-rw-rw-r--   0 jz        (1000) jz        (1000)       29 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/raytrace/__init__.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    15204 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/raytrace/radmc3d.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.891515 astro-synthesizer-0.0.3/synthesizer/synobs/
+-rw-rw-r--   0 jz        (1000) jz        (1000)       66 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/__init__.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    19644 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/scripter.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     2861 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/syn_imager.py
+drwxrwxr-x   0 jz        (1000) jz        (1000)        0 2023-05-03 10:41:09.895515 astro-synthesizer-0.0.3/synthesizer/synobs/templates/
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1519 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_1.3mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1698 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_1.3mm_pol.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1692 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_3mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1619 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_18mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1588 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_7mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)     1597 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_9mm.py
+-rw-rw-r--   0 jz        (1000) jz        (1000)    27401 2023-04-02 17:43:02.000000 astro-synthesizer-0.0.3/synthesizer/utils.py
```

### Comparing `astro-synthesizer-0.0.2/LICENSE` & `astro-synthesizer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/PKG-INFO` & `astro-synthesizer-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-synthesizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate astronomical synthetic observations from the command-line 
 Author-email: Joaquin Zamponi <jzamponi@mpe.mpg.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `astro-synthesizer-0.0.2/README.md` & `astro-synthesizer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/astro_synthesizer.egg-info/PKG-INFO` & `astro-synthesizer-0.0.3/astro_synthesizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-synthesizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate astronomical synthetic observations from the command-line 
 Author-email: Joaquin Zamponi <jzamponi@mpe.mpg.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `astro-synthesizer-0.0.2/astro_synthesizer.egg-info/SOURCES.txt` & `astro-synthesizer-0.0.3/astro_synthesizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/pyproject.toml` & `astro-synthesizer-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astro-synthesizer"
-version = "0.0.2"
+version = "0.0.3"
 description = "Generate astronomical synthetic observations from the command-line "
 readme = "README.md"
 authors = [{ name = "Joaquin Zamponi", email = "jzamponi@mpe.mpg.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `astro-synthesizer-0.0.2/synthesizer/__main__.py` & `astro-synthesizer-0.0.3/synthesizer/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,11 +21,11 @@
                     python3-matplotlib, python3-astropy, python3-mayavi,
                     python3-radmc3dPy
 
 """
 
 from synthesizer import parser
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 if __name__ == "__main__":
     parser.parser()
```

### Comparing `astro-synthesizer-0.0.2/synthesizer/dustmixer/bhcoat.py` & `astro-synthesizer-0.0.3/synthesizer/dustmixer/bhcoat.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/dustmixer/bhmie.py` & `astro-synthesizer-0.0.3/synthesizer/dustmixer/bhmie.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/dustmixer/dustmixer.py` & `astro-synthesizer-0.0.3/synthesizer/dustmixer/dustmixer.py`

 * *Files 1% similar despite different names*

```diff
@@ -656,19 +656,21 @@
 
         utils.print_(f'Writing out radmc3d opacity file: {outfile}')
         with open(outfile, 'w+') as f:
             # Write a comment with info
             f.write(f'# Opacity table generated by Dustmixer\n')
             f.write(f'# Material = {self.name}\n')
             f.write(f'# Density = {self.dens} g/cm3\n')
-            f.write(f'# Minimum grain size = {np.round(self.amin*1e4, 1)}um\n')
-            f.write(f'# Maximum grain size = {np.round(self.amax*1e4, 1)}um\n')
+            f.write(f'# Minimum grain size = {np.round(self.amin*1e4, 3)}um\n')
+            f.write(f'# Maximum grain size = {np.round(self.amax*1e4, 3)}um\n')
             f.write(f'# Number of sizes = {self.na}\n')
             f.write(f'# Distribution slope = {self.q}\n')
             f.write(f'# Number of scattering angles: {self.nang}\n')
+            f.write(f'# Columns are: wavelength (microns), k_abs (cm2/g), ')
+            f.write(f'k_sca (cm2/g), g_sca\n')
 
             # Write file header
             f.write('1\n' if self.scatmatrix else '3\n')
             f.write(f'{self.l.size}\n')
             if self.scatmatrix:
                 f.write(f'{self.nang}\n')
             
@@ -787,15 +789,15 @@
 
         p.semilogx(self.l*u.cm.to(u.micron), self.gsca, ls='-', c='black')
         p.text(0.55, 0.90, r'$g=\int_{-1}^1 p(\mu)\mu d\mu,\,\,\mu=\cos \theta$',
             fontsize=18, transform=p.transAxes)
         p.set_xlabel('Wavelength (microns)')
         p.set_ylabel(r'$g_{\rm sca}$')
         p.set_ylim(-1, 1)
-        p.set_xlim(1e-1, 3e4)
+        #p.set_xlim(1e-1, 3e4)
         plt.tight_layout()
         return utils.plot_checkout(fig, show, savefig)
 
     def plot_opacities(self, show=True, savefig=None):
         """ Plot the extinction, scattering & absorption eficiencies.  """
 
         if self.kext is None or self.ksca is None: 
@@ -810,15 +812,15 @@
         p.loglog(self.l*u.cm.to(u.micron), self.ksca, ls=':', c='black')
         p.loglog(self.l*u.cm.to(u.micron), self.kabs, ls='--', c='black')
         p.legend([r'$k_{\rm ext}$', r'$k_{\rm sca}$', r'$k_{\rm abs}$'])
         p.text(0.05, 0.95, self.name, fontsize=13, transform=p.transAxes)
         p.set_xlabel('Wavelength (microns)')
         p.set_ylabel(r'Dust opacity $k$ (cm$^2$ g$^{-1}$)')
         p.set_ylim(1e-2, 1e4)
-        p.set_xlim(1e-1, 3e4)
+        #p.set_xlim(1e-1, 3e4)
         plt.tight_layout()
 
         return utils.plot_checkout(fig, show, savefig)
 
     def _get_kappa_at_lam(self, lam):
         """ Return the extinction dust opacity at a given wavelength """
```

### Comparing `astro-synthesizer-0.0.2/synthesizer/gridder/amr_reader.py` & `astro-synthesizer-0.0.3/synthesizer/gridder/amr_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 import h5py
 import numpy as np
+import astropy.units as u
+import astropy.constants as c
 
 from synthesizer import utils
 
 class Athena:
-    """ Object designed to read in spatial and physical quantities from 
+    """ 
+        Object designed to read in spatial and physical quantities from 
         Athena++ snapshots.
     """
     def __init__(self):
         utils.not_implemented()
 
 class Flash:
-    """ Object designed to read in spatial and physical quantities from 
+    """ 
+        Object designed to read in spatial and physical quantities from 
         FLASH snapshots.
     """
     def __init__(self):
         utils.not_implemented()
 
 class Enzo:
-    """ Object designed to read in spatial and physical quantities from 
+    """ 
+        Object designed to read in spatial and physical quantities from 
         ENZO snapshots.
     """
     def __init__(self):
         utils.not_implemented()
 
 class Ramses:
-    """ Object designed to read in spatial and physical quantities from 
+    """ 
+        Object designed to read in spatial and physical quantities from 
         RAMSES snapshots.
     """
     def __init__(self):
         utils.not_implemented()
 
 class ZeusTW:
-    """ This object is an adapted copy of Zeus2Polaris._read_data()
+    """ 
+        This object is an adapted copy of Zeus2Polaris._read_data()
         src: https://github.com/jzamponi/zeus2polaris
     """ 
+    def __init__(self):
+        self.rho = None
+        self.rho = None
+        self.Br  = None
+        self.Bth = None
+        self.Bph = None
+        self.Vr  = None
+        self.Vth = None
+        self.Vph = None
+        self.cordsystem = 150
+
     def read(self, filename, coord=False):
         """ Read the binary files from zeusTW.
             Reshape to 3D only if it is a physical quantity and not a coordinate
         """
         # Load binary file
         with open(filename, "rb") as binfile:
             data = np.fromfile(file=binfile, dtype=np.double, count=-1)
@@ -49,21 +67,27 @@
             shape = (self.r.size, self.th.size, self.ph.size)
             return data.reshape(shape, order='F')
 
     def generate_coords(self, r, th, ph):
         self.r = self.read(r, coord=True)
         self.th = self.read(th, coord=True)
         self.ph = self.read(ph, coord=True)
+        self.x = self.r
+        self.y = self.th
+        self.z = self.ph
 
     def trim_ghost_cells(self, field_type, ng=3):
         if field_type == 'coords':
             # Trim ghost zones for the coordinate fields
             self.r = self.r[ng:-ng]
             self.th = self.th[ng:-ng]
             self.ph = self.ph[ng:-ng]
+            self.x = self.x[ng:-ng]
+            self.y = self.y[ng:-ng]
+            self.z = self.z[ng:-ng]
 
         elif field_type == 'scalar':
             # Trim ghost cells for scalar fields
             self.rho = self.rho[ng:-ng, ng:-ng, ng:-ng]
 
         elif field_type == 'vector':
             # Trim ghost cells for vector fields
@@ -96,15 +120,18 @@
 
     def LH_to_Gaussian(self):
         self.Br *= np.sqrt(4 * np.pi)
         self.Bth *= np.sqrt(4 * np.pi)
         self.Bph *= np.sqrt(4 * np.pi)
     
     def generate_cartesian(self):
-        """ Convert spherical coordinates and vector components to cartesian. """
+        """ Convert spherical coordinates and vector components to cartesian """
+
+        self.cordsystem = 1 
+
         # Create a coordinate grid.
         r, th, ph = np.meshgrid(self.r, self.th, self.ph, indexing='ij')
 
         # Convert coordinates to cartesian
         self.x = r * np.cos(ph) * np.sin(th)
         self.y = r * np.sin(ph) * np.sin(th)
         self.z = r * np.cos(th)
```

### Comparing `astro-synthesizer-0.0.2/synthesizer/gridder/analytical.py` & `astro-synthesizer-0.0.3/synthesizer/gridder/analytical.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,36 +104,101 @@
             utils.not_implemented(f'Model: {self.model}')
             model = models.SpiralDisk(x, y, z, field)
 
         # Gas filament 
         elif self.model == 'filament':
             utils.not_implemented(f'Model: {self.model}')
             model = models.Filament(x, y, z, field)
+
+        # PPDisk: HL Tau
+        elif self.model == 'hltau':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.HLTau(x, y, z, field)
     
+        # PPDisk: TW Hya
+        elif self.model == 'twhya':
+            #utils.not_implemented(f'Model: {self.model}')
+            model = models.TWHya(x, y, z, field)
+    
+        # PPDisk: HD 163296
+        elif self.model == 'hd16293':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.HD16293(x, y, z, field)
+
+        # PPDisk: IM Lup
+        elif self.model == 'imlup':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.IMLup(x, y, z, field)
+
+        # PPDisk: WaOph 6
+        elif self.model == 'waoph6':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.WaOph6(x, y, z, field)
+
+        # PPDisk: Elias 27
+        elif self.model == 'elias27':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.Elias27(x, y, z, field)
+
+        # PPDisk: Elias 26
+        elif self.model == 'elias26':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.Elias26(x, y, z, field)
+
+        # PPDisk: AS 209
+        elif self.model == 'as209':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.AS209(x, y, z, field)
+
+        # PPDisk: GW Lup
+        elif self.model == 'gwlup':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.GWLup(x, y, z, field)
+
+        # PPDisk: HD 143006
+        elif self.model == 'hd143006':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.HD143006(x, y, z, field)
+
+        # PPDisk: HT Lup
+        elif self.model == 'htlup':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.htlup(x, y, z, field)
+
+        # PPDisk: AS 205
+        elif self.model == 'as205':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.AS205(x, y, z, field)
+
+        # PPDisk: HH 212
+        elif self.model == 'hh212':
+            utils.not_implemented(f'Model: {self.model}')
+            model = models.HH212(x, y, z, field)
+
         else:
             raise ValueError(
                 f'{utils.color.red}' +\
                 f'Model: {self.model} cannot be found.' +\
                 f'{utils.color.none}')
 
         # Copy the model density and temperature to the current obj (anaytical)
         self.dens = model.dens / self.g2d
         if self.add_temp: self.temp = model.temp
         if self.vfield is not None: self.vfield = model.vfield                
         if model.plotmin is not None: self.plotmin = model.plotmin
         if model.plotmax is not None: self.plotmax = model.plotmax
 
 
-    def write_grid_file(self):
+    def write_grid_file(self, regular=True):
         """ Write the regular cartesian grid file """
         with open('amr_grid.inp','w+') as f:
             # iformat
             f.write('1\n')
             # Regular grid
-            f.write('0\n')
+            f.write('0\n' if regular else '1\n')
             # Coordinate system: cartesian
             f.write('1\n')
             # Gridinfo
             f.write('0\n')
             # Number of cells
             f.write('1 1 1\n')
             # Size of the grid
@@ -414,15 +479,15 @@
                 utils.print_('Adding optical depth surface at tau = 1')
                 dl = bbox * u.au.to(u.cm) * 2 / data.shape[0]
                 kappa = 1
                 tau1 = np.cumsum(data * kappa * dl, axis=0).T
 
                 if tau1.max() < 1:
                     utils.print_(
-                        'The highest optical depth is tau = {tau1.max()}. ' +
+                        f'The highest optical depth is tau = {tau1.max()}. ' +
                         'No tau = 1 surface will be displayed.')
                 else:
                     tausurf = mlab.contour3d(
                         tau1, contours=[1], opacity=0.5, color=(0, 0, 1))
 
             utils.print_('HINT: If you wanna play with the figure, press '+\
                 'the nice icon in the upper left corner.', blue=True)
@@ -457,14 +522,18 @@
         if not dust_density and not dust_temperature:
             subprocess.run('radmc3d vtk_grid'.split())
 
         self.radmc3d_banner()
 
     def render(self, state=None, dust_density=False, dust_temperature=True):
         """ Render the new grid in 3D using ParaView """
+
+        # Make sure ParaView is installed and callable
+        utils.which('paraview')
+    
         if isinstance(state, str):
             subprocess.run(f'paraview --state {state} 2>/dev/null'.split())
         else:
             try:
                 if dust_density:
                     subprocess.run(
                     f'paraview model_dust_density.vtk 2>/dev/null'.split())
```

### Comparing `astro-synthesizer-0.0.2/synthesizer/gridder/custom_model.py` & `astro-synthesizer-0.0.3/synthesizer/gridder/custom_model.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/gridder/gridder.py` & `astro-synthesizer-0.0.3/synthesizer/gridder/gridder.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,24 @@
 from scipy.interpolate import griddata
 
 from synthesizer.gridder.vector_field import VectorField
 from synthesizer.gridder.sph_reader  import *
 from synthesizer.gridder.amr_reader  import *
 from synthesizer import utils
 
-class CartesianGrid():
+
+class Grid():
+    """ 
+        Base class for different grid geometries.
+    """
+    pass
+
+class CartesianGrid(Grid):
     def __init__(self, ncells, bbox=None, rout=None, nspec=1, csubl=0, 
-            sootline=300, g2d=100, temp=False):
+            sootline=300, g2d=100, temp=False, vfield=None):
         """ 
         Create a cartesian grid from a set of 3D points.
 
         The input SPH particle coordinates should be given as cartesian 
         coordinates in units of cm.
 
         The box can be trimmed to a given size calling self.trim_box. The 
@@ -30,21 +37,30 @@
 
         """
 
         self.cordsystem = 1
         self.fx = 1
         self.fy = 1
         self.fz = 1
-        self.dens = np.zeros((ncells, ncells, ncells))
-        self.temp = np.zeros((ncells, ncells, ncells))
-        self.interp_dens = None
-        self.interp_temp = None
-        self.vfield = None
-        self.add_temp = temp
+        self.nx = ncells
+        self.ny = ncells
+        self.nz = ncells
         self.ncells = ncells
+        self.dens = np.zeros((self.nx, self.ny, self.nz))
+        self.temp = np.zeros((self.nx, self.ny, self.nz))
+        self.vx = np.zeros((self.nx, self.ny, self.nz))
+        self.vy = np.zeros((self.nx, self.ny, self.nz))
+        self.vz = np.zeros((self.nx, self.ny, self.nz))
+        self.grid_dens = None
+        self.grid_temp = None
+        self.grid_vx = None
+        self.grid_vy = None
+        self.grid_vz = None
+        self.vfield = vfield
+        self.add_temp = temp
         self.bbox = bbox
         self.rout = rout
         self.g2d = g2d
         self.nspec = nspec
         self.csubl = csubl
         self.sootline = sootline
         self.carbon = 0.375
@@ -61,31 +77,31 @@
         utils.print_(
             f'Reading data from: {filename} | Format: {source.upper()}', end='')
         if not os.path.exists(filename): 
             raise FileNotFoundError(f'{utils.color.red}' +\
                 f'Input SPH file does not exist{utils.color.none}')
 
         if source.lower() == 'sphng':
-            self.sph = SPHng(filename, temp=self.add_temp)
+            self.sph = SPHng(filename, self.add_temp, self.vfield)
 
         elif source.lower() == 'gizmo':
-            self.sph = Gizmo(filename, temp=self.add_temp)
+            self.sph = Gizmo(filename, self.add_temp, self.vfield)
 
         elif source.lower() == 'gadget':
-            self.sph = Gadget(filename, temp=self.add_temp)
+            self.sph = Gadget(filename, self.add_temp, self.vfield)
 
         elif source.lower() == 'arepo':
-            self.sph = Arepo(filename, temp=self.add_temp)
+            self.sph = Arepo(filename, self.add_temp, self.vfield)
 
         elif source.lower() == 'phantom':
             utils.not_implemented()
-            self.sph = Phantom(filename, temp=self.add_temp)
+            self.sph = Phantom(filename, self.add_temp, self.vfield)
 
         elif source.lower() == 'nbody6':
-            self.sph = Nbody6(filename, temp=self.add_temp)
+            self.sph = Nbody6(filename, self.add_temp, self.vfield)
 
         else:
             print('')
             raise ValueError(f'Source = {source} is currently not supported')
             
         self.x = self.sph.x
         self.y = self.sph.y
@@ -94,56 +110,76 @@
         self.npoints = len(self.dens)
         print(f' | Particles: {self.npoints}')
 
         if self.add_temp:
             self.temp = self.sph.temp
         else:
             self.temp = np.zeros(self.dens.shape)
+        
+        if self.vfield:
+            self.vx = self.sph.vx
+            self.vy = self.sph.vy
+            self.vz = self.sph.vz
 
-    def read_amr(self, filename, sourle='athena++'):
+    def read_amr(self, filename, source='athena++'):
         """ Read AMR data """
 
+        source = source.lower()
+
         utils.print_(f'Reading data from: {filename} | Format: {source}')
         if not os.path.exists(filename): 
-            raise FileNotFoundError('Input AMR file does not exist')
-
-        if source.lower() == 'athena++':
-            utils.not_implemented()
+            if source != 'zeustw':
+                utils.file_exists(filename,
+                    msg='Input AMR file does not exist')
 
-        elif source.lower() == 'zeustw':
+        if source == 'athena++':
             utils.not_implemented()
 
+        elif source == 'zeustw':
             # Generate a Data instance
             data = ZeusTW()
 
+            # Set the coordinate system
+            self.cordsystem = data.cordsystem
+
             # Read coordinates: x?a are cell edges and x?b are cell centers
             data.generate_coords(r="z_x1ap", th="z_x2ap", ph="z_x3ap")
 
             frame = str(filename).zfill(5)
             data.rho = data.read(f"o_d__{frame}")
-            data.trim_ghost_cells(field_type='coords')
-            data.trim_ghost_cells(field_type='scalar')
-            data.trim_ghost_cells(field_type='vector')
+            data.Br = data.read(f"o_b1_{frame}")
+            data.Bth = data.read(f"o_b2_{frame}")
+            data.Bph = data.read(f"o_b3_{frame}")
+            data.Vr = data.read(f"o_v1_{frame}")
+            data.Vth = data.read(f"o_v2_{frame}")
+            data.Vph = data.read(f"o_v3_{frame}")
+
+            data.trim_ghost_cells(field_type='coords', ng=3)
+            data.trim_ghost_cells(field_type='scalar', ng=3)
+            data.trim_ghost_cells(field_type='vector', ng=3)
             data.LH_to_Gaussian()
             data.generate_temperature()
-            data.generate_cartesian()
+            #data.generate_cartesian()
 
-            self.xw = data.x
-            self.yw = data.y
-            self.zw = data.z
-            self.dens = data.rho
-            self.temp = data.temp
+            self.xc = data.x
+            self.yc = data.y
+            self.zc = data.z
+            self.nx = data.x.size
+            self.ny = data.y.size
+            self.nz = data.z.size
+            self.grid_dens = data.rho * self.g2d
+            self.grid_temp = data.temp
 
-        elif source.lower() == 'flash':
+        elif source == 'flash':
             utils.not_implemented()
 
-        elif source.lower() == 'enzo':
+        elif source == 'enzo':
             utils.not_implemented()
             
-        elif source.lower() == 'ramses':
+        elif source == 'ramses':
             utils.not_implemented()
             
         else:
             raise ValueError(f'Source = {source} is currently not supported')
 
     def trim_box(self):
         """ 
@@ -185,17 +221,46 @@
 
         # Remove the particles from each quantity
         self.x = np.delete(self.x, to_remove)
         self.y = np.delete(self.y, to_remove)
         self.z = np.delete(self.z, to_remove)
         self.dens = np.delete(self.dens, to_remove)
         self.temp = np.delete(self.temp, to_remove)
+
+        if self.vfield:
+            self.vx = np.delete(self.vx, to_remove)
+            self.vy = np.delete(self.vy, to_remove)
+            self.vz = np.delete(self.vz, to_remove)
+
         utils.print_(f'Particles included: {self.x.size} | ' +
             f'Particles excluded: {self.npoints - self.x.size} ')
 
+        if self.x.size == 0:
+            raise ValueError(
+                utils.color.red +
+                'All particles were removed. Try increasing --bbox or --rout' +
+                utils.color.none
+            )
+
+    def plot_particles(self):
+        """ 
+            Render the locations of the 3D points weighted by the 
+            normalized density 
+        """
+
+        from mayavi import mlab
+
+        utils.print_('Rendering particles in 3D weighted by density')
+
+        fig = mlab.figure(
+            size=(1100, 1000),  bgcolor=(1, 1, 1),  fgcolor=(0.2, 0.2, 0.2)
+        )
+        mlab.points3d(self.x, self.y, self.z, self.dens)
+        mlab.show()
+
     def find_resolution(self):
         """
         Find the minimum distance between points. 
         If particles are too many, it uses only those that are 
         closer to the geometrical center than the mean distance.
         """
         
@@ -220,89 +285,125 @@
                 f'is larger than the minimum particle separation '+\
                 f'{self.resolution*u.cm.to(u.au):.1}au. ', blue=True)
             utils.print_('You may want to increase ncells or use a bbox', 
                 blue=True)
 
         return dmin
 
-    def interpolate_points(self, field, method='linear', fill='min'):
+    def interpolate(self, field, method='linear', fill='min'):
         """
             Interpolate a set of points in cartesian coordinates along with their
             values into a rectangular grid.
         """
 
         # Construct the rectangular grid
         rmin = np.min([self.x.min(), self.y.min(), self.z.min()])
         rmax = np.max([self.x.max(), self.y.max(), self.z.max()])
         self.bbox = (rmax - rmin) / 2
         self.cellsize = self.bbox / self.ncells
-        #self.resolution = self.find_resolution()
+        # self.resolution = self.find_resolution()
 
-        self.xc = np.linspace(rmin, rmax, self.ncells)
-        self.yc = np.linspace(rmin, rmax, self.ncells)
-        self.zc = np.linspace(rmin, rmax, self.ncells)
+        self.xc = np.linspace(rmin, rmax, self.nx)
+        self.yc = np.linspace(rmin, rmax, self.ny)
+        self.zc = np.linspace(rmin, rmax, self.nz)
         self.X, self.Y, self.Z = np.meshgrid(self.xc, self.yc, self.zc)
 
-        utils.print_(f'Creating a box of size [{rmin*u.cm.to(u.au):.1f} au, ' +\
-            f'{rmax*u.cm.to(u.au):.1f} au] with {self.ncells} cells per side.')
+        if field == 'dens':
+            utils.print_(
+                f'Creating a box of size [{rmin*u.cm.to(u.au):.1f} au, ' +
+                f'{rmax*u.cm.to(u.au):.1f} au] with {self.ncells} cells ' +
+                f'per side.'
+            )
 
         # Determine which quantity is to be interpolated
         if field == 'dens':
-            utils.print_(f'Interpolating density values onto the grid')
+            utils.print_(
+                f'Interpolating density values onto the grid')
             values = self.dens
         elif field == 'temp':
-            utils.print_(f'Interpolating temperature values onto the grid')
+            utils.print_(
+                f'Interpolating temperature values onto the grid')
             values = self.temp
+        elif field == 'vx':
+            utils.print_(
+                f'Interpolating X vector field components onto the grid')
+            values = self.vx
+        elif field == 'vy':
+            utils.print_(
+                f'Interpolating Y vector field components onto the grid')
+            values = self.vy
+        elif field == 'vz':
+            utils.print_(
+                f'Interpolating Z vector field components onto the grid')
+            values = self.vz
         else:
-            raise ValueError('field must be "dens" or "temp".')
+            raise ValueError('field must be "dens", "temp", "vx", "vy" or "vz"')
+
+        # Set a number or key to fill the values outside the interpol. range
+        fill = {
+            'min': np.min(values), 
+            'max': np.max(values), 
+            'mean': np.mean(values), 
+        }.get(fill, fill)
 
         # Interpolate the point values at the grid points
         interp = griddata(
             points=np.vstack([self.x, self.y, self.z]).T, 
             values=values, 
             xi=(self.X, self.Y, self.Z), 
             method=method, 
-            fill_value=np.min(values) if fill == 'min' else fill,
+            fill_value=fill,
         )
  
         # Store the interpolated field
         if field == 'dens':
-            self.interp_dens = interp
+            self.grid_dens = interp
         elif field == 'temp':
-            self.interp_temp = interp
+            self.grid_temp = interp
+        elif field == 'vx':
+            self.grid_vx = interp
+        elif field == 'vy':
+            self.grid_vy = interp
+        elif field == 'vz':
+            self.grid_vz = interp
 
 
-    def write_grid_file(self):
+    def write_grid_file(self, regular=True):
         """ Write the regular cartesian grid file """
         with open('amr_grid.inp','w+') as f:
             # iformat
             f.write('1\n')                     
             # Regular grid
             f.write('0\n')                      
             # Coordinate system
             f.write(f'{self.cordsystem}\n')                     
             # Gridinfo
             f.write('0\n')                       
             # Number of cells
             f.write('1 1 1\n')                   
             # Size of the grid
-            f.write(f'{self.ncells:d} {self.ncells:d} {self.ncells:d}\n')
+            f.write(f'{self.nx:d} {self.ny:d} {self.nz:d}\n')
 
             # Shift the cell centers right to set the cell walls
-            dx = np.diff(self.xc)[0]
-            dy = np.diff(self.yc)[0]
-            dz = np.diff(self.zc)[0]
-            self.xw = self.xc + dx
-            self.yw = self.yc + dy
-            self.zw = self.zc + dz
-
-            # Add the missing wall at the beginning of each axis
-            self.xw = np.insert(self.xw, 0, self.xc[0])
-            self.yw = np.insert(self.yw, 0, self.yc[0])
-            self.zw = np.insert(self.zw, 0, self.zc[0])
+            if regular:
+                dx = np.diff(self.xc)[0]
+                dy = np.diff(self.yc)[0]
+                dz = np.diff(self.zc)[0]
+                self.xw = self.xc + dx
+                self.yw = self.yc + dy
+                self.zw = self.zc + dz
+
+                # Add the missing wall at the beginning of each axis
+                self.xw = np.insert(self.xw, 0, self.xc[0])
+                self.yw = np.insert(self.yw, 0, self.yc[0])
+                self.zw = np.insert(self.zw, 0, self.zc[0])
+            else:
+                self.xw = self.xc
+                self.yw = self.yc
+                self.zw = self.zc
 
             # Write the cell walls
             for i in self.xw:
                 f.write(f'{i:13.6e}\n')      
             for j in self.yw:
                 f.write(f'{j:13.6e}\n')      
             for k in self.zw:
@@ -310,29 +411,29 @@
 
 
     def write_density_file(self):
         """ Write the density file """
         utils.print_('Writing dust density file')
 
         # Flatten the array into a 1D fortran-style indexing
-        density = self.interp_dens.ravel(order='F')
+        density = self.grid_dens.ravel(order='F')
         with open('dust_density.inp','w+') as f:
             f.write('1\n')                      
             f.write(f'{density.size:d}\n')
             f.write(f'{self.nspec}\n')                
 
             if self.nspec == 1:
                 # Write a single dust species
                 for d in density:
                     f.write(f'{d:13.6e}\n')
             else:
                 utils.print_(f'Writing two density species ...')
                 # Write two densities: 
                 # one with original value outside the sootline and zero within 
-                temp1d = self.interp_temp.ravel(order='F')
+                temp1d = self.grid_temp.ravel(order='F')
                 for i, d in enumerate(density):
                     if temp1d[i] < self.sootline:
                         f.write(f'{d:13.6e}\n')
                     else:
                         f.write('0\n')
 
                 # one with zero outside the sootline and reduced density within
@@ -342,15 +443,15 @@
                     else:
                         f.write(f'{(d * self.subl_mfrac):13.6e}\n')
 
     def write_temperature_file(self):
         """ Write the temperature file """
         utils.print_('Writing dust temperature file')
         
-        temperature = self.interp_temp.ravel(order='F')
+        temperature = self.grid_temp.ravel(order='F')
         with open('dust_temperature.dat','w+') as f:
             f.write('1\n')                      
             f.write(f'{temperature.size:d}\n')
             f.write(f'{self.nspec}\n')                
 
             # Write the temperature Nspec times for Nspec dust species
             for i in range(self.nspec):
@@ -358,23 +459,26 @@
                     f.write(f'{t:13.6e}\n')
 
     def write_vector_field(self, morphology):
         """ Create a vector field for dust alignment """
  
         utils.print_('Writing grain alignment direction file')
  
-        if self.vfield is None:
+        if self.vfield:
             self.vfield = VectorField(self.X, self.Y, self.Z, morphology)
+            self.vfield.vx = self.grid_vx 
+            self.vfield.vy = self.grid_vy 
+            self.vfield.vz = self.grid_vz 
  
         with open('grainalign_dir.inp','w+') as f:
             f.write('1\n')
-            f.write(f'{int(self.ncells**3)}\n')
-            for iz in range(self.ncells):
-                for iy in range(self.ncells):
-                    for ix in range(self.ncells):
+            f.write(f'{int(self.nx * self.ny * self.nz)}\n')
+            for iz in range(self.nx):
+                for iy in range(self.ny):
+                    for ix in range(self.nz):
                         f.write(f'{self.vfield.vx[ix, iy, iz]:13.6e} ' +\
                                 f'{self.vfield.vy[ix, iy, iz]:13.6e} ' +\
                                 f'{self.vfield.vz[ix, iy, iz]:13.6e}\n')
 
     def plot_midplane(self, field, data=None):
         """ Plot the density midplane at z=0 using Matplotlib """
         try:
@@ -387,16 +491,16 @@
             plt.rcParams['xtick.minor.visible'] = True
             plt.rcParams['ytick.minor.visible'] = True
             plt.close('all')
 
             # Detect what field to use
             if data is None:
                 data = {
-                    'density': self.interp_dens, 
-                    'temperature': self.interp_temp
+                    'density': self.grid_dens, 
+                    'temperature': self.grid_temp
                 }[field]
             else:
                 data = data.T
             
             # Set the plot title for the right field
             title = {
                 'density': r'Dust Density (g cm$^{-3}$)', 
@@ -444,15 +548,15 @@
             p[1].set_title('Midplane XZ')
             p[0].set_ylabel('Y (AU)')
             p[1].set_ylabel('Z (AU)')
             p[0].set_xticklabels([])
             p[1].set_xticklabels([])
 
             try:
-                if self.vfield is not None and field == 'density':
+                if self.vfield and field == 'density':
                     p[0].streamplot(
                         np.linspace(-bbox, bbox, self.ncells), 
                         np.linspace(-bbox, bbox, self.ncells), 
                         self.vfield.vx[..., plane], 
                         self.vfield.vy[..., plane],
                         linewidth=0.5,
                         color='k', 
@@ -487,16 +591,16 @@
             from mayavi.modules.text3d import Text3D
             from mayavi.modules.grid_plane import GridPlane
 
             utils.print_('Visualizing the interpolated field ...')
 
             if data is None:
                 data = {
-                    'density': self.interp_dens, 
-                    'temperature': self.interp_temp
+                    'density': self.grid_dens, 
+                    'temperature': self.grid_temp
                 }[field]
             
             title = {
                 'density': r'Dust Density (g cm$^{-3}$)', 
                 'temperature': r'Gas Temperature (g cm$^{-3}$)',
             }[field]
 
@@ -513,15 +617,15 @@
             # Add a colorbar
             cbar = mlab.colorbar(plot, orientation='vertical', title=title)
 
             # Add a bounding box frame             
             bbox = int(np.round(self.bbox * u.cm.to(u.au), 1))
             mlab.outline(
                 figure=fig, 
-                extent=[0, self.ncells] * 3, 
+                extent=[0, self.nx, 0, self.ny, 0, self.nz], 
             )
             mlab.axes(
                 ranges=[-bbox, bbox] * 3,
                 xlabel='AU', ylabel='AU', zlabel='AU', nb_labels=3
             )
         
             # Handle figure items
@@ -557,15 +661,15 @@
                 utils.print_('Adding optical depth surface at tau = 1')
                 dl = bbox * u.au.to(u.cm) * 2 / data.shape[0]
                 kappa = 1
                 tau1 = np.cumsum(data * kappa * dl, axis=0).T
 
                 if tau1.max() < 1:
                     utils.print_(
-                        'The highest optical depth is tau = {tau1.max()}. ' +
+                        f'The highest optical depth is tau = {tau1.max()}. ' +
                         'No tau = 1 surface will be displayed.')
                 else:
                     tausurf = mlab.contour3d(
                         tau1, contours=[1], opacity=0.5, color=(0, 0, 1))
 
             utils.print_('HINT: If you wanna play with the figure, press '+\
                 'the nice icon in the upper left corner.', blue=True)
@@ -579,51 +683,50 @@
             mlab.show()
 
         except Exception as e:
             utils.print_('Unable to show the 3D grid.',  red=True)
             utils.print_(e, bold=True)
 
 
-    def create_vtk(self, dust_density=False, dust_temperature=True, rename=False):
+    def create_vtk(self, dust_density=False, dust_temperature=False, rename=False):
         """ Call radmc3d to create a VTK file of the grid """
-        self.radmc3d_banner()
 
         if dust_density:
             subprocess.run('radmc3d vtk_dust_density 1'.split())
             if rename:
                 subprocess.run('mv model.vtk model_dust_density.vtk'.split())
 
         if dust_temperature:
             subprocess.run('radmc3d vtk_dust_temperature 1'.split())
             if rename:
                 subprocess.run('mv model.vtk model_dust_temperature.vtk'.split())
 
         if not dust_density and not dust_temperature:
             subprocess.run('radmc3d vtk_grid'.split())
 
-        self.radmc3d_banner()
 
-    def render(self, state=None, dust_density=False, dust_temperature=True):
+    def render(self, dust_density=False, dust_temperature=False):
         """ Render the new grid in 3D using ParaView """
-        if isinstance(state, str):
-            subprocess.run(f'paraview --state {state} 2>/dev/null'.split())
-        else:
-            try:
-                if dust_density:
-                    subprocess.run(
-                    f'paraview model_dust_density.vtk 2>/dev/null'.split())
-                elif dust_temperature:
-                    subprocess.run(
-                    f'paraview model_dust_temperature.vtk 2>/dev/null'.split())
-            except Exception as e:
-                utils.print_('Unable to render using ParaView.',  red=True)
-                utils.print_(e, bold=True)
+    
+        # Make sure ParaView is installed and callable
+        utils.which('paraview')
+    
+        try:
+            if dust_density:
+                subprocess.run(
+                f'paraview model_dust_density.vtk 2>/dev/null'.split())
+            elif dust_temperature:
+                subprocess.run(
+                f'paraview model_dust_temperature.vtk 2>/dev/null'.split())
+        except Exception as e:
+            utils.print_('Unable to render using ParaView.',  red=True)
+            utils.print_(e, bold=True)
 
 
-class SphericalGrid():
+class SphericalGrid(Grid):
     def __init__(self):
         """ This is yet to be implemented.
             It will be translated from old scripts and from the very own
             radmc3d's implementation.
             src:https://github.com/dullemond/radmc3d-2.0/blob/master/python/
                 radmc3d_tools/sph_to_sphergrid.py
          """
```

### Comparing `astro-synthesizer-0.0.2/synthesizer/gridder/sph_reader.py` & `astro-synthesizer-0.0.3/synthesizer/gridder/sph_reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,19 +27,42 @@
 
         if temp.shape != dens.shape:
             raise ValueError(f'Array shape of temp must be equal to dens.' +\
                 f'{temp.shape = }   {self._dens.shape = }')
 
         self._temp = temp
 
+    @property
+    def vx(self):
+        return self._vx
+    
+    @property
+    def vy(self):
+        return self._vy
+
+    @property
+    def vz(self):
+        return self._vz
+
+    @vx.setter
+    def vx(self, vx):
+        self._vx = vx
+
+    @vy.setter
+    def vy(self, vy):
+        self._vy = vy
+
+    @vz.setter
+    def vz(self, vz):
+        self._vz = vz
 
 
 class SPHng(SPHCode):
     """ Handle binary snapshots from the SPHng code. """
-    def __init__(self, filename, temp=False, remove_sink=True):
+    def __init__(self, filename, temp=False, vfield=False, remove_sink=True):
         """
             Notes:
 
             This reader assumes your file is binary and formatted 
             with a header stating the quantities, assumed to be 
             f4 floats. May not be widely applicable.
 
@@ -55,14 +78,15 @@
             T = particle temperature [K]
             u = particle internal energy [ignore]
             
             There's an outlier (probably a sink particle) with index = 31330
         """
         
         self.add_temp = temp
+        self.vfield = vfield
 
         # Read file in binary format
         try:
             with open(filename, "rb") as f:
                 names = f.readline()[1:].split()
                 self.data = np.frombuffer(f.read()).reshape(-1, len(names))
                 self.data = self.data.astype("f4")
@@ -88,64 +112,93 @@
             self.data[sink_id, 11] = 900
         
         self.x = self.data[:, 2]
         self.y = self.data[:, 3]
         self.z = self.data[:, 4]
 
     @property
-    def rho_g(self):
-        return self.data[:, 10]
+    def rho_g(self): return self.data[:, 10]
 
     @property
     def temp(self):
-        if self.add_temp:
-            return self.data[:, 11]
+        if self.add_temp: return self.data[:, 11]
+
+    @property
+    def vx(self):
+        if self.vfield: return self.data[:, 5]
+
+    @property
+    def vy(self):
+        if self.vfield: return self.data[:, 6]
+
+    @property
+    def vz(self):
+        if self.vfield: return self.data[:, 7]
 
 
 class Gizmo(SPHCode):
     """ Handle HDF5 snapshots from the GIZMO code. """
-    def __init__(self, filename):
+    def __init__(self, filename, temp=False, vfield=False):
 
         # Read in particle coordinates and density
         self.data = h5py.File(filename, 'r')['PartType0']
         coords = np.array(self.data['Coordinates'])
         self.x = coords[:, 0] * u.pc.to(u.cm)
         self.y = coords[:, 1] * u.pc.to(u.cm)
         self.z = coords[:, 2] * u.pc.to(u.cm)
 
         # Recenter the particles based on the center of mass
         self.x -= np.average(self.x, weights=self.rho_g)
         self.y -= np.average(self.y, weights=self.rho_g)
         self.z -= np.average(self.z, weights=self.rho_g)
 
+        self.add_temp = temp
+        self.vfield = vfield
+
     @property
     def rho_g(self):
         return np.array(self.data['Density']) * 1.3816327e-23
 
     @property
     def temp(self):
         # Read in temperature if available
         if 'Temperature' in self.data:
             return np.array(self.data['Temperature'])
+
         # Or maybe the krome temperature, when coupled with KROME
         elif 'KromeTemperature' in self.data:
             return np.array(self.data['KromeTemperature'])
         
         # Or derive from a barotropic equation of state
-        elif 'InternalEnergy' in self.data.keys() and 'Pressure' in self.data.keys():
+        elif 'InternalEnergy' in self.data.keys() and \
+            'Pressure' in self.data.keys():
             return self.data['InternalEnergy'] / np.array(self.data['Pressure'])
 
         else:
             return np.zeros(self.rho_g.shape)
 
+    @property
+    def vx(self):
+        if self.vfield: return self.data['MagneticField'][:, 0]
+
+    @property
+    def vy(self):
+        if self.vfield: return self.data['MagneticField'][:, 1]
+
+    @property
+    def vz(self):
+        if self.vfield: return self.data['MagneticField'][:, 2]
+
+
 class Gadget(SPHCode):
     """ Handle snapshots from the Gadget code. """
-    def __init__(self, filename, temp=False):
+    def __init__(self, filename, temp=False, vfield=False):
     
         self.add_temp = temp
+        self.vfield = vfield 
 
         # Read in particle coordinates and density
         self.data = h5py.File(filename, 'r')['PartType0']
         coords = np.array(self.data['Coordinates'])
         self.x = coords[:, 0] * u.au.to(u.cm)
         self.y = coords[:, 1] * u.au.to(u.cm)
         self.z = coords[:, 2] * u.au.to(u.cm) 
@@ -172,19 +225,33 @@
                 kB = c.k_B.cgs.value
                 mu = 2.3 * (c.m_e + c.m_p).cgs.value
                 return (mu / kB) * np.array(self.data['Pressure']) / self.rho_g
 
             else:
                 return np.zeros(self.rho_g.shape)
 
+    @property
+    def vx(self):
+        if self.vfield: return self.data['MagneticField'][:, 0]
+
+    @property
+    def vy(self):
+        if self.vfield: return self.data['MagneticField'][:, 1]
+
+    @property
+    def vz(self):
+        if self.vfield: return self.data['MagneticField'][:, 2]
+
+
 class Arepo(SPHCode):
     """ Handle snapshots from the AREPO code. """
-    def __init__(self, filename, temp=False):
+    def __init__(self, filename, temp=False, vfield=False):
 
         self.add_temp = temp
+        self.vfield = vfield
 
         # Read in particle coordinates and density
         self.data = h5py.File(filename, 'r')['PartType0']
         coords = np.array(self.data.get('Coordinates'))
         mass = np.array(self.data.get('Masses'))
         press = np.array(self.data.get('Pressure'))
         energy = np.array(self.data.get('InternalEnergy'))
@@ -236,62 +303,104 @@
                 )
 
                 return T2
 
             else:
                 return np.zeros(self.rho_g.shape)
 
+    @property
+    def vx(self):
+        if self.vfield: return self.data['MagneticField'][:, 0]
+
+    @property
+    def vy(self):
+        if self.vfield: return self.data['MagneticField'][:, 1]
+
+    @property
+    def vz(self):
+        if self.vfield: return self.data['MagneticField'][:, 2]
+
+
 class Phantom(SPHCode):
     """ Handle snapshots from the PHANTOM code. """
-    def __init__(self, filename, temp=False):
+    def __init__(self, filename, temp=False, vfield=False):
+
+        utils.not_implemented('PHANTOM Interface')
         
         # Read in particle coordinates and density
         self.data = h5py.File(filename, 'r')['particles']
         coords = self.data['xyz'].value
+
         # Derive density from the particle mass / h**3
         # src: https://github.com/dmentipl/plonk/blob/main/src/plonk/snap/readers/phantom.py
     
         self.add_temp = temp
+        self.vfield = vfield
+
         self.x = coords[:, 0] * u.au.to(u.cm)
         self.y = coords[:, 1] * u.au.to(u.cm)
         self.z = coords[:, 2] * u.au.to(u.cm)
 
     @property
     def rho_g(self):
         dens = np.array(self.data['Density'])
         return dens * 1e-10 * (u.Msun / u.au**3).to(u.g/u.cm**3)
 
     @property
     def temp(self):
         return np.zeros(self.rho_g.shape)
 
+    @property
+    def vx(self):
+        if self.vfield: return self.data['bfield'][:, 0]
+
+    @property
+    def vy(self):
+        if self.vfield: return self.data['bfield'][:, 1]
+
+    @property
+    def vz(self):
+        if self.vfield: return self.data['bfield'][:, 2]
+
+
 class Nbody6(SPHCode):
     """ Handle snapshots from the Nbody6 code. """
-    def __init__(self, filename, temp=False):
+    def __init__(self, filename, temp=False, vfield=False):
 
         self.add_temp = temp
+        self.vfield = vfield
         
         # Read in data from HDF5 file
         if filename.endswith(('h5', 'hdf5')):
             utils.not_implemented('Nbody6-HDF5')
             self.data = h5py.File(filename, 'r')
 
         # Read in data from ASCII table
         else:
             self.data = np.loadtxt(filename)
             self.mass = self.data[:, 0] * u.Msun.to(u.g)
             self.radius = self.data[:, 1] * u.Rsun.to(u.cm)
             self.x = self.data[:, 3] * u.pc.to(u.cm)
             self.y = self.data[:, 4] * u.pc.to(u.cm)
             self.z = self.data[:, 5] * u.pc.to(u.cm)
-            self.vx = self.data[:, 6] * (u.km/u.s).to(u.cm/u.s)
-            self.vy = self.data[:, 7] * (u.km/u.s).to(u.cm/u.s)
-            self.vz = self.data[:, 8] * (u.km/u.s).to(u.cm/u.s)
             self.id = self.data[:, 10]
 
     @property
     def rho_g(self):
         return self.data[:, 2] * (u.Msun/u.Rsun**3).to(u.g/u.cm**3)
 
     @property
     def temp(self):
         return self.data[:, 9] 
+
+    @property
+    def vx(self):
+        if self.vfield: return self.data[:, 6] * (u.km/u.s).to(u.cm/u.s)
+
+    @property
+    def vy(self):
+        if self.vfield: return self.data[:, 7] * (u.km/u.s).to(u.cm/u.s)
+
+    @property
+    def vz(self):
+        if self.vfield: return self.data[:, 8] * (u.km/u.s).to(u.cm/u.s)
+
```

### Comparing `astro-synthesizer-0.0.2/synthesizer/gridder/vector_field.py` & `astro-synthesizer-0.0.3/synthesizer/gridder/vector_field.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/parser.py` & `astro-synthesizer-0.0.3/synthesizer/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,17 @@
         choices=['x', 'y', 'z', 'toroidal', 'radial', 'hourglass', 
         'helicoidal', 'dipole', 'quadrupole', 'custom'], 
         help='Create a vectory field for alignment of elongated grains.')
 
     parser.add_argument('--temperature', action='store_true', default=False, 
         help='Write the dust temperature from the model.')
 
+    parser.add_argument('--show-particles', action='store_true', default=False,  
+        help='Render the SPH particle positions weighted by density')
+
     parser.add_argument('--show-grid-2d', action='store_true', default=False,  
         help='Plot the midplane of the newly created grid')
 
     parser.add_argument('--show-grid-3d', action='store_true', default=False, 
         help='Render the new cartesian grid in 3D')
 
     parser.add_argument('--vtk', action='store_true', default=False, 
@@ -145,14 +148,17 @@
 
     parser.add_argument('--npix', action='store', type=int, default=300,
         help='Number of pixels per side of new image')
 
     parser.add_argument('--incl', action='store', type=float, default=0,
         help='Inclination angle of the grid in degrees')
 
+    parser.add_argument('--phi', action='store', type=float, default=0,
+        help='Inclination angle over a second axis in degrees')
+
     parser.add_argument('--sizeau', action='store', type=int, default=None,
         help='Physical size of the image in AU')
 
     parser.add_argument('--distance', action='store', type=float, default=141,
         help='Physical distance in pc, used to convert fluxes into Jy/pixel.')
 
     parser.add_argument('--star', action='store', default=None, nargs=6,
@@ -231,15 +237,15 @@
 
     parser.add_argument('-ow', '--overwrite', action='store_true', 
         default=False, help='Overwrite opacities, RADMC3D and CASA input files')
 
     parser.add_argument('--quiet', action='store_true', default=False,
         help='Disable verbosity. Do not output anything.')
 
-    parser.add_argument('--version', action='version', version='%(prog)s 0.0.2')
+    parser.add_argument('--version', action='version', version='%(prog)s 0.0.3')
 
 
 
     # Store the command-line given arguments
     cli = parser.parse_args()
 
     # Initialize the pipeline
@@ -256,15 +262,16 @@
     if cli.grid:
         pipeline.create_grid(
             sphfile=cli.sphfile, amrfile=cli.amrfile, 
             source=cli.source, model=cli.model, ncells=cli.ncells, g2d=cli.g2d, 
             bbox=cli.bbox, rout=cli.rout, temperature=cli.temperature, 
             render=cli.render, vtk=cli.vtk, show_2d=cli.show_grid_2d, 
             show_3d=cli.show_grid_3d, vector_field=cli.vector_field, 
-            tau=cli.tau,
+            tau=cli.tau, show_particles=cli.show_particles, 
+            alignment=cli.alignment,
         )
 
     # Generate the dust opacity tables
     if cli.opacity:
         pipeline.dustmixer(
             show_nk=cli.show_nk, show_opac=cli.show_opacity, pb=not cli.nopb
         )
@@ -272,15 +279,15 @@
     # Run a thermal Monte-Carlo
     if cli.monte_carlo:
         pipeline.monte_carlo(nphot=cli.nphot, radmc3d_cmds=cli.radmc3d)
 
     # Run a ray-tracing on the new grid and generate an image
     if cli.raytrace:
         pipeline.raytrace(
-            incl=cli.incl, npix=cli.npix, distance=cli.distance,
+            incl=cli.incl, phi=cli.phi, npix=cli.npix, distance=cli.distance,
             sizeau=cli.sizeau, show=cli.show_rt, noscat=cli.noscat, tau=cli.tau,
             tau_surf=cli.tau_surf, show_tau_surf=cli.show_tau_surf, 
             radmc3d_cmds=cli.radmc3d
         )
 
     # Run a synthetic observation of the new image by calling CASA
     if cli.synobs:
```

### Comparing `astro-synthesizer-0.0.2/synthesizer/pipeline.py` & `astro-synthesizer-0.0.3/synthesizer/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         self.q = q
         self.nang = nang
         self.material = material
         self.nphot = int(nphot)
         self.nthreads = int(nthreads)
         self.npix = None
         self.incl = None
+        self.phi = None
         self.sizeau = None
         self.polarization = polarization
         self.alignment = alignment
         if polarization:
             self.scatmode = 5
             self.inputstyle = 10
         else:
@@ -93,18 +94,21 @@
             self.tstar = star[5]
 
         self.bbox = bbox
         self.overwrite = overwrite
         self.verbose = verbose
 
     @utils.elapsed_time
-    def create_grid(self, model=None, sphfile=None, amrfile=None, 
+    def create_grid(
+            self, model=None, sphfile=None, amrfile=None, 
             source='sphng', bbox=None, rout=None, ncells=None, tau=False, 
             vector_field=None, show_2d=False, show_3d=False, vtk=False, 
-            render=False, g2d=100, temperature=True):
+            render=False, g2d=100, temperature=True, show_particles=False, 
+            alignment=False,
+        ):
         """ Initial step in the pipeline: creates an input grid for RADMC3D """
 
         self.model = model
         self.sphfile = sphfile
         self.amrfile = amrfile
         self.ncells = ncells
         self.bbox = bbox * u.au.to(u.cm) if bbox is not None else bbox
@@ -122,54 +126,70 @@
 
         # Create a grid instance
         print('')
         utils.print_('Creating model grid ...\n', bold=True)
     
         # Create a grid using an analytical model
         if model is not None:
+            regular = True
+
             self.grid = gridder.AnalyticalModel(
                 model=self.model,
                 bbox=self.bbox, 
                 ncells=self.ncells, 
                 g2d=self.g2d,
                 nspec=self.nspec,
                 temp=temperature, 
             )
             
             # Create a model density grid 
             self.grid.create_model()
 
         # Create a grid from SPH particles
         elif sphfile is not None:
+            regular = True
+
             self.grid = gridder.CartesianGrid(
                 ncells=self.ncells, 
                 bbox=self.bbox, 
                 rout=self.rout,
                 csubl=self.csubl, 
                 nspec=self.nspec, 
                 sootline=self.sootline, 
                 g2d=self.g2d, 
                 temp=temperature,
+                vfield=alignment,
             )
 
             # Read the SPH data
             self.grid.read_sph(self.sphfile, source=source)
 
             # Set a bounding box or radius to trim particles outside of it
             if self.bbox is not None or self.rout is not None:
                 self.grid.trim_box()
+
+            # Render SPH particles in 3D space before interpolation
+            if show_particles:
+                self.grid.plot_particles()
     
             # Interpolate the SPH points onto a regular cartesian grid
-            self.grid.interpolate_points('dens', 'linear', fill='min')
+            self.grid.interpolate('dens', 'linear', fill='min')
 
             if temperature:
-                self.grid.interpolate_points('temp', 'linear', fill='min')
+                self.grid.interpolate('temp', 'linear', fill='min')
+
+            if alignment:
+                self.grid.interpolate('vx', 'linear', fill=0)
+                self.grid.interpolate('vy', 'linear', fill=0)
+                self.grid.interpolate('vz', 'linear', fill=0)
 
         # Create a grid from an AMR grid
         elif amrfile is not None:
+            regular = False    
+
             self.grid = gridder.CartesianGrid(
                 ncells=self.ncells, 
                 bbox=self.bbox, 
                 rout=self.rout,
                 csubl=self.csubl, 
                 nspec=self.nspec, 
                 sootline=self.sootline, 
@@ -177,29 +197,31 @@
                 temp=temperature,
             )
             
             # Read the AMR data
             self.grid.read_amr(self.amrfile, source=source)
         
         else:
-            raise ValueError(f'{utils.color.red}When --grid is set, either --'+\
-                f'model, --sphfile or --amrfile must be given{utils.color.none}')
+            raise ValueError(
+                f'{utils.color.red}When --grid is set, either --model, ' +\
+                f'--sphfile or --amrfile must be given{utils.color.none}'
+            )
 
         self.bbox = self.grid.bbox
 
         # Write the new cartesian grid to radmc3d file format
-        self.grid.write_grid_file()
+        self.grid.write_grid_file(regular=regular)
 
         # Write the dust density distribution to radmc3d file format
         self.grid.write_density_file()
         
         if temperature:
             self.grid.write_temperature_file()
 
-        if vector_field is not None:
+        if vector_field is not None or alignment:
             self.grid.write_vector_field(morphology=vector_field)
 
         # Plot the density midplane
         if show_2d:
             self.grid.plot_midplane('density')
 
         # Plot the temperature midplane
@@ -212,20 +234,25 @@
 
         # Render the temperature volume in 3D using Mayavi
         if show_3d and temperature:
             self.grid.plot_3d('temperature')
         
         # Call RADMC3D to read the grid file and generate a VTK representation
         if vtk:
-            self.grid.create_vtk(
-                dust_density=False, dust_temperature=True, rename=True)
+            self.grid.create_vtk(dust_density=True, rename=True)
+
+            if temperature:
+                self.grid.create_vtk(dust_temperature=True, rename=True)
         
         # Visualize the VTK grid file using ParaView
         if render:
-            self.grid.render()
+            self.grid.render(dust_density=True)
+
+            if temperature:
+                self.grid.render(dust_temperature=True)
 
         # Register the pipeline step 
         self.steps.append('create_grid')
 
 
     @utils.elapsed_time
     def dustmixer(self, show_nk=False, pb=True, show_opac=False, savefig=None):
@@ -545,17 +572,17 @@
         
         self._catch_radmc3d_error()
 
         # Register the pipeline step 
         self.steps.append('monte_carlo')
 
     @utils.elapsed_time
-    def raytrace(self, lam=None, incl=None, npix=None, sizeau=None, show=True, 
+    def raytrace(self, lam=None, incl=None, phi=None, npix=None, sizeau=None, 
             distance=141, tau=False, tau_surf=None, show_tau_surf=False, 
-            noscat=False, radmc3d_cmds=''):
+            noscat=False, radmc3d_cmds='', show=True):
         """ 
             Call radmc3d to raytrace the newly created grid and plot an image 
         """
 
         print('')
         utils.print_("Ray-tracing the model density and temperature ...\n", 
             bold=True)
@@ -627,14 +654,16 @@
 
         if lam is not None:
             self.lam = lam
         if npix is not None:
             self.npix = npix
         if incl is not None:
             self.incl = incl
+        if phi is not None:
+            self.phi = phi
         if sizeau is not None:
             self.sizeau = sizeau 
         else:
             self.sizeau = int(2 * self._get_bbox() * u.cm.to(u.au))
 
         # Explicitly the model rotate by 180.
         # Only for the current model. This line should be later removed.
@@ -650,14 +679,15 @@
         # Set the RADMC3D command by concatenating options
         cmd = f'radmc3d image '
         cmd += f'lambda {self.lam} '
         cmd += f'sizeau {self.sizeau} '
         cmd += f'noscat ' if noscat else ' '
         cmd += f'stokes ' if self.polarization else ' '
         cmd += f'incl {self.incl} ' if self.incl is not None else ' '
+        cmd += f'phi {self.phi} ' if self.phi is not None else ' '
         cmd += f'npix {self.npix} ' if self.npix is not None else ' '
         cmd += f'{" ".join(radmc3d_cmds)} '
         
 
         # Call RADMC3D and pipe the output also to radmc3d.out
         try:
             utils.print_(f'Executing command: {cmd}')
@@ -683,14 +713,15 @@
         for st in ['I', 'Q', 'U'] if self.polarization else ['I']:
             stfile = fitsfile.replace('I', st)
             utils.radmc3d_casafits(stfile, stokes=st, dpc=distance)
             utils.edit_header(stfile, 'NPHOT', f'{self.nphot:e}')
             utils.edit_header(stfile, 'OPACITY', self.kappa)
             utils.edit_header(stfile, 'MATERIAL', self.material)
             utils.edit_header(stfile, 'INCL', self.incl)
+            utils.edit_header(stfile, 'PHI', self.phi)
             utils.edit_header(stfile, 'CSUBL', self.csubl)
             utils.edit_header(stfile, 'NSPEC', self.nspec)
 
         # Plot the new image in Jy/pixel
         if show:
             self.plot_rt()
 
@@ -1132,21 +1163,22 @@
             if --grid was given. Otherwise read from the grid file.
         """
 
         if self.bbox is not None:
             return self.bbox
         else:
             gridid = int(np.loadtxt('amr_grid.inp', skiprows=1, max_rows=1))
-            ncells = int(np.loadtxt('amr_grid.inp', skiprows=5, max_rows=1)[0])
+            ncells = np.loadtxt('amr_grid.inp', skiprows=5, max_rows=1)
+            nx, ny, nz = int(ncells[0]), int(ncells[1]), int(ncells[2])
 
             # Number of lines to skip from grid style (0: reg, 1: oct, 10: amr)
             skip = {0: 6, 1: 7, 10: 7}[gridid]
 
             # Number of lines to read
-            nlines = ncells * 3 + 3 
+            nlines = nx * ny * nz + 3 
 
             # Read in the grid
             g = np.loadtxt('amr_grid.inp', skiprows=skip, max_rows=nlines)
 
             # Return bbox as the difference between the first and last vertex
             return (g[-1] - g[0]) / 2
```

### Comparing `astro-synthesizer-0.0.2/synthesizer/raytrace/radmc3d.py` & `astro-synthesizer-0.0.3/synthesizer/raytrace/radmc3d.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/synobs/scripter.py` & `astro-synthesizer-0.0.3/synthesizer/synobs/scripter.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/synobs/syn_imager.py` & `astro-synthesizer-0.0.3/synthesizer/synobs/syn_imager.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/synobs/templates/alma_1.3mm.py` & `astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_1.3mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/synobs/templates/alma_1.3mm_pol.py` & `astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_1.3mm_pol.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/synobs/templates/alma_3mm.py` & `astro-synthesizer-0.0.3/synthesizer/synobs/templates/alma_3mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/synobs/templates/vla_18mm.py` & `astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_18mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/synobs/templates/vla_7mm.py` & `astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_7mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/synobs/templates/vla_9mm.py` & `astro-synthesizer-0.0.3/synthesizer/synobs/templates/vla_9mm.py`

 * *Files identical despite different names*

### Comparing `astro-synthesizer-0.0.2/synthesizer/utils.py` & `astro-synthesizer-0.0.3/synthesizer/utils.py`

 * *Files identical despite different names*

