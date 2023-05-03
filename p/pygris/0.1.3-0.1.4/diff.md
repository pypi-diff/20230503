# Comparing `tmp/pygris-0.1.3.tar.gz` & `tmp/pygris-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygris-0.1.3.tar", last modified: Thu Feb  9 20:03:32 2023, max compression
+gzip compressed data, was "pygris-0.1.4.tar", last modified: Wed May  3 14:35:19 2023, max compression
```

## Comparing `pygris-0.1.3.tar` & `pygris-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-02-09 20:03:32.385918 pygris-0.1.3/
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     1050 2022-10-05 14:20:47.000000 pygris-0.1.3/LICENSE
--rw-rw-r--   0 kyle      (1001) kyle      (1001)       55 2022-11-25 16:28:53.000000 pygris-0.1.3/MANIFEST.in
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     2137 2023-02-09 20:03:32.385918 pygris-0.1.3/PKG-INFO
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     1543 2022-11-25 15:22:17.000000 pygris-0.1.3/README.md
-drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-02-09 20:03:32.381918 pygris-0.1.3/pygris/
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      229 2023-02-09 19:50:41.000000 pygris-0.1.3/pygris/__init__.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     8749 2022-11-21 12:48:35.000000 pygris-0.1.3/pygris/data.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    37601 2022-11-20 21:03:28.000000 pygris-0.1.3/pygris/enumeration_units.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    11872 2022-11-21 12:13:43.000000 pygris-0.1.3/pygris/geocode.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     5448 2022-12-31 13:21:40.000000 pygris-0.1.3/pygris/helpers.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      180 2022-10-19 14:24:10.000000 pygris-0.1.3/pygris/internal_data.py
-drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-02-09 20:03:32.385918 pygris-0.1.3/pygris/internals/
--rw-rw-r--   0 kyle      (1001) kyle      (1001)        0 2022-10-13 19:22:43.000000 pygris-0.1.3/pygris/internals/__init__.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)   111585 2022-07-29 23:53:00.000000 pygris-0.1.3/pygris/internals/fips_codes.csv
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    12451 2022-11-20 21:07:11.000000 pygris-0.1.3/pygris/legislative.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    10168 2022-11-20 21:06:27.000000 pygris-0.1.3/pygris/metro_areas.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     3955 2022-10-20 20:36:10.000000 pygris-0.1.3/pygris/national.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    12253 2022-11-20 21:04:25.000000 pygris-0.1.3/pygris/native.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    12451 2022-11-20 21:05:17.000000 pygris-0.1.3/pygris/transportation.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    13836 2023-02-09 19:50:41.000000 pygris-0.1.3/pygris/utils.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     7163 2022-11-20 21:05:52.000000 pygris-0.1.3/pygris/water.py
-drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-02-09 20:03:32.385918 pygris-0.1.3/pygris.egg-info/
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     2137 2023-02-09 20:03:32.000000 pygris-0.1.3/pygris.egg-info/PKG-INFO
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      530 2023-02-09 20:03:32.000000 pygris-0.1.3/pygris.egg-info/SOURCES.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)        1 2023-02-09 20:03:32.000000 pygris-0.1.3/pygris.egg-info/dependency_links.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      110 2023-02-09 20:03:32.000000 pygris-0.1.3/pygris.egg-info/requires.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)       28 2023-02-09 20:03:32.000000 pygris-0.1.3/pygris.egg-info/top_level.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      953 2023-02-09 19:50:41.000000 pygris-0.1.3/pyproject.toml
--rw-rw-r--   0 kyle      (1001) kyle      (1001)       68 2022-11-21 15:16:13.000000 pygris-0.1.3/requirements.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)       38 2023-02-09 20:03:32.385918 pygris-0.1.3/setup.cfg
+drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-03 14:35:19.573255 pygris-0.1.4/
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     1050 2022-10-05 14:20:47.000000 pygris-0.1.4/LICENSE
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)       55 2022-11-25 16:28:53.000000 pygris-0.1.4/MANIFEST.in
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     2137 2023-05-03 14:35:19.573255 pygris-0.1.4/PKG-INFO
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     1543 2022-11-25 15:22:17.000000 pygris-0.1.4/README.md
+drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-03 14:35:19.573255 pygris-0.1.4/pygris/
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      229 2023-04-06 13:28:03.000000 pygris-0.1.4/pygris/__init__.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    10047 2023-05-03 14:21:45.000000 pygris-0.1.4/pygris/data.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    37601 2022-11-20 21:03:28.000000 pygris-0.1.4/pygris/enumeration_units.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    11872 2022-11-21 12:13:43.000000 pygris-0.1.4/pygris/geocode.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     5448 2022-12-31 13:21:40.000000 pygris-0.1.4/pygris/helpers.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      180 2022-10-19 14:24:10.000000 pygris-0.1.4/pygris/internal_data.py
+drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-03 14:35:19.573255 pygris-0.1.4/pygris/internals/
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)        0 2022-10-13 19:22:43.000000 pygris-0.1.4/pygris/internals/__init__.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)   111585 2022-07-29 23:53:00.000000 pygris-0.1.4/pygris/internals/fips_codes.csv
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    12451 2022-11-20 21:07:11.000000 pygris-0.1.4/pygris/legislative.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    10168 2022-11-20 21:06:27.000000 pygris-0.1.4/pygris/metro_areas.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     3955 2022-10-20 20:36:10.000000 pygris-0.1.4/pygris/national.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    12253 2022-11-20 21:04:25.000000 pygris-0.1.4/pygris/native.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    12451 2022-11-20 21:05:17.000000 pygris-0.1.4/pygris/transportation.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    13836 2023-05-01 18:04:49.000000 pygris-0.1.4/pygris/utils.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     7163 2022-11-20 21:05:52.000000 pygris-0.1.4/pygris/water.py
+drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-03 14:35:19.573255 pygris-0.1.4/pygris.egg-info/
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     2137 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/PKG-INFO
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      530 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)        1 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      110 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/requires.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)       28 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/top_level.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      953 2023-04-06 13:32:23.000000 pygris-0.1.4/pyproject.toml
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)       68 2022-11-21 15:16:13.000000 pygris-0.1.4/requirements.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)       38 2023-05-03 14:35:19.573255 pygris-0.1.4/setup.cfg
```

### Comparing `pygris-0.1.3/LICENSE` & `pygris-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/PKG-INFO` & `pygris-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygris
-Version: 0.1.3
+Version: 0.1.4
 Summary: Download and use US Census Bureau TIGER/Line Shapefiles and other data resources in Python
 Author-email: Kyle Walker <kyle@walker-data.com>
 License: MIT
 Project-URL: Homepage, https://github.com/walkerke/pygris
 Project-URL: Bug Tracker, https://github.com/walkerke/pygris/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygris-0.1.3/README.md` & `pygris-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/data.py` & `pygris-0.1.4/pygris/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import pandas as pd
 import appdirs
 import os
+from pygris.enumeration_units import states, counties, tracts, block_groups, blocks
 
 def get_census(dataset, variables, year = None, params = {}, 
                return_geoid = False, guess_dtypes = False):
     """
     Make a request to a US Census Bureau API endpoint
 
     Parameters
@@ -112,41 +113,48 @@
         # to NaN. Users who want to keep the codes should keep as object and handle
         # themselves.
         out[num_list] = out[num_list].where(out[num_list] > -999999)
 
     return out
 
 
-def get_lodes(state, year, lodes_type = "od", part = "main", 
-              job_type = "JT00", segment = "S000", cache = False):
+def get_lodes(state, year, version = "LODES8", lodes_type = "od", part = "main", 
+              job_type = "JT00", segment = "S000", agg_level = "block", cache = False):
 
     """
     Get synthetic block-level data on workplace, residence, and origin-destination flows characteristics from the 
     LEHD Origin-Destination Employment Statistics (LODES) dataset
 
     Parameters
     --------------
     state : str
         The state postal code of your requested data. Please note that not all states are available 
         in all years.
     year : int
         The year of your requested data. LODES data go back to 2002, but not all datasets are available 
         for all years / for all states.  
+    version : str
+        The LODES version to use.  Version 8 (the default, use "LODES8") is enumerated at 2020 Census blocks.
+        "LODES7" is enumerated at 2010 Census blocks, but ends in 2019; "LODES5" is enumerated at 2000 Census
+        blocks, but ends in 2009.  
     lodes_type : str
         One of "od" (the default) for origin-destination flows, "wac" for workplace area characteristics, 
         or "rac" for residence area characteristics.  
     part : str
         Only relevant for the "od" file.  "main" gives information on within-state residence to workplace flows.
         "aux" gives information for residence to workplace flows from outside a given state.
     job_type : str
         The available job type breakdown; defaults to "JT00" for all jobs. Please review the LODES technical
         documentation for a description of other options.
     segment : str
         The workforce segment, relevant when lodes_type is "wac" or "rac". Defaults to "S000" for total jobs;
         review the LODES technical documentation for a description of other options.
+    agg_level : str
+        The level at which to aggregate the data.  Defaults to the Census block; other options include 
+        "state", "county", "tract", and "block group".  
     cache : bool
         If True, downloads the requested LODES data to a cache directory on your computer and reads from
         that directory if the file exists. Defaults to False, which will download the data by default. 
 
     Returns
     ---------------
     A Pandas DataFrame of LODES data.
@@ -166,30 +174,21 @@
 
     if lodes_type not in ['od', 'wac', 'rac']:
         raise ValueError("lodes_type must be one of 'od', 'rac', or 'wac'.")
     
     state = state.lower()
 
     if lodes_type == "od":
-        url = f"https://lehd.ces.census.gov/data/lodes/LODES7/{state}/od/{state}_od_{part}_{job_type}_{year}.csv.gz"
+        url = f"https://lehd.ces.census.gov/data/lodes/{version}/{state}/od/{state}_od_{part}_{job_type}_{year}.csv.gz"
     else:
-        url = f"https://lehd.ces.census.gov/data/lodes/LODES7/{state}/{lodes_type}/{state}_{lodes_type}_{segment}_{job_type}_{year}.csv.gz"
+        url = f"https://lehd.ces.census.gov/data/lodes/{version}/{state}/{lodes_type}/{state}_{lodes_type}_{segment}_{job_type}_{year}.csv.gz"
     
     if not cache:
         lodes_data = pd.read_csv(url)
         
-        if lodes_type == "od":
-            lodes_data['w_geocode'] = lodes_data['w_geocode'].astype(str).str.zfill(15)
-            lodes_data['h_geocode'] = lodes_data['h_geocode'].astype(str).str.zfill(15)
-        elif lodes_type == "rac":
-            lodes_data['h_geocode'] = lodes_data['h_geocode'].astype(str).str.zfill(15)
-        else:
-            lodes_data['w_geocode'] = lodes_data['w_geocode'].astype(str).str.zfill(15)        
-
-        return lodes_data
     else:
         cache_dir = appdirs.user_cache_dir("pygris")
 
         if not os.path.isdir(cache_dir):
             os.mkdir(cache_dir) 
 
         basename = os.path.basename(url)
@@ -203,16 +202,51 @@
 
             with open(out_file, 'wb') as fd:
                 fd.write(req.content)
         
         # Now, read in the file from the cache directory
         lodes_data = pd.read_csv(out_file)
 
-        if lodes_type == "od":
-            lodes_data['w_geocode'] = lodes_data['w_geocode'].astype(str).str.zfill(15)
-            lodes_data['h_geocode'] = lodes_data['h_geocode'].astype(str).str.zfill(15)
+    # Drop the 'createdate' column
+    lodes_data = lodes_data.drop('createdate', axis = 1)
+
+    if lodes_type == "od":
+        lodes_data['w_geocode'] = lodes_data['w_geocode'].astype(str).str.zfill(15)
+        lodes_data['h_geocode'] = lodes_data['h_geocode'].astype(str).str.zfill(15)
+    elif lodes_type == "rac":
+        lodes_data['h_geocode'] = lodes_data['h_geocode'].astype(str).str.zfill(15)
+    else:
+        lodes_data['w_geocode'] = lodes_data['w_geocode'].astype(str).str.zfill(15)
+
+    # Handle aggregation logic
+    if agg_level != "block":
+        if agg_level == "state":
+            end = 2
+        elif agg_level == "county":
+            end = 5
+        elif agg_level == "tract":
+            end = 11
+        elif agg_level == "block group":
+            end = 12
+        else: 
+            raise ValueError("Invalid agg_level; choose one of 'state', 'county', 'tract', or 'block group'.")
+        
+        if lodes_type == "wac":
+            lodes_data['w_geocode'] = lodes_data['w_geocode'].str.slice(stop = end)
+
+            lodes_data = lodes_data.groupby('w_geocode').agg("sum")
         elif lodes_type == "rac":
-            lodes_data['h_geocode'] = lodes_data['h_geocode'].astype(str).str.zfill(15)
-        else:
-            lodes_data['w_geocode'] = lodes_data['w_geocode'].astype(str).str.zfill(15)
+            lodes_data['h_geocode'] = lodes_data['h_geocode'].str.slice(stop = end)
+
+            lodes_data = lodes_data.groupby('h_geocode').agg("sum")
+        elif lodes_type == "od":
+            lodes_data['h_geocode'] = lodes_data['h_geocode'].str.slice(stop = end)
+            lodes_data['w_geocode'] = lodes_data['w_geocode'].str.slice(stop = end)
+
+            lodes_data = lodes_data.groupby(['h_geocode', 'w_geocode']).agg("sum")  
+
+        return lodes_data.reset_index()          
+    
+
+
 
-        return lodes_data          
+
```

### Comparing `pygris-0.1.3/pygris/enumeration_units.py` & `pygris-0.1.4/pygris/enumeration_units.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/geocode.py` & `pygris-0.1.4/pygris/geocode.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/helpers.py` & `pygris-0.1.4/pygris/helpers.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/internals/fips_codes.csv` & `pygris-0.1.4/pygris/internals/fips_codes.csv`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/legislative.py` & `pygris-0.1.4/pygris/legislative.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/metro_areas.py` & `pygris-0.1.4/pygris/metro_areas.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/national.py` & `pygris-0.1.4/pygris/national.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/native.py` & `pygris-0.1.4/pygris/native.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/transportation.py` & `pygris-0.1.4/pygris/transportation.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/utils.py` & `pygris-0.1.4/pygris/utils.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris/water.py` & `pygris-0.1.4/pygris/water.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pygris.egg-info/PKG-INFO` & `pygris-0.1.4/pygris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygris
-Version: 0.1.3
+Version: 0.1.4
 Summary: Download and use US Census Bureau TIGER/Line Shapefiles and other data resources in Python
 Author-email: Kyle Walker <kyle@walker-data.com>
 License: MIT
 Project-URL: Homepage, https://github.com/walkerke/pygris
 Project-URL: Bug Tracker, https://github.com/walkerke/pygris/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygris-0.1.3/pygris.egg-info/SOURCES.txt` & `pygris-0.1.4/pygris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygris-0.1.3/pyproject.toml` & `pygris-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygris"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Kyle Walker", email="kyle@walker-data.com" },
 ]
 license = {text = "MIT"}
 description = "Download and use US Census Bureau TIGER/Line Shapefiles and other data resources in Python"
 readme = "README.md"
 requires-python = ">=3.7"
```

