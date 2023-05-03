# Comparing `tmp/geomulticorr-0.0.1.tar.gz` & `tmp/geomulticorr-0.0.2.tar.gz`

## Comparing `geomulticorr-0.0.1.tar` & `geomulticorr-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/src/__init__.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/src/geomorph.py
--rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/src/pair.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/src/pzone.py
--rw-r--r--   0        0        0    20060 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/src/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/src/spine.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/src/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/src/xzone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/tests/test_geomorph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/tests/test_pair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/tests/test_pzone.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/tests/test_session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/tests/test_xzone.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/LICENSE.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 geomulticorr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20056 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/src/geomulticorr/xzone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/tests/test_geomorph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/tests/test_pair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/tests/test_pzone.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/tests/test_session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/tests/test_xzone.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 geomulticorr-0.0.2/PKG-INFO
```

### Comparing `geomulticorr-0.0.1/src/geomorph.py` & `geomulticorr-0.0.2/src/geomulticorr/geomorph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-#%%
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
 import geopandas as gpd
 from telenvi import raster_tools as rt
 
-import geomulticorr.src.spine
+import src.geomulticorr.spine
 
 class Geomorph:
         
     def __init__(self, session, ge_id):
         
         # Check existence and unique
         assert ge_id in session._geomorphs.ge_frogi_id.values, 'key not found in Geomorphs layer'
@@ -74,15 +73,15 @@
             row['V'] = row.D/abs(row.L-row.R)        
             disps.append(row)
         return pd.DataFrame(disps)
     
     def get_spines(self):
         all_spines = self.session._spines
         ge_spines  = all_spines[all_spines.sp_ge_id == self.ge_id]
-        return [geomulticorr.src.spine.Spine(self.session, spine.sp_id) for spine in ge_spines.iloc]
+        return [src.geomulticorr.spine.Spine(self.session, spine.sp_id) for spine in ge_spines.iloc]
 
     def show_mean_velocities(self, savepath=None, bounds=None):
         fig, ax = plt.subplots(figsize=(10,6.5))
         disps = self.get_disp_overview()
         for pair in disps.iloc:
             ya = pair.L
             yb = pair.R
@@ -95,9 +94,8 @@
             ax.plot([int(ya), int(yb)],[meters, meters], 'bo', color=color, alpha=0.7)
 
         if bounds != None:
             ax.set_ybound(lower=bounds[0], upper=bounds[1])
         ax.set_xticks(np.arange(2001,2023,2))
         ax.set_title(f"Vitesses annuelles moyennes sur {self.ge_id}")
         if savepath != None:
-            fig.savefig(savepath)
-# %%
+            fig.savefig(savepath)
```

### Comparing `geomulticorr-0.0.1/src/pair.py` & `geomulticorr-0.0.2/src/geomulticorr/pair.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from telenvi import raster_tools as rt
 
-import geomulticorr.src.thumb
+import src.geomulticorr.thumb
 
 ROOT_OUTPUTS  = Path(__file__).parent.with_name('temp')
 ROOT_TEMPLATE = Path(__file__).parent.with_name('template')
 
 class Pair:
 
     def __init__(self, session=None, target_path=None, left=None, right=None):
@@ -37,16 +37,16 @@
 
             # Reconstruct their path
             thumbs_pzone_path = Path(session.p_raster_data, pz_name, 'opticals')
             left_path = Path (thumbs_pzone_path, left_key)
             right_path = Path(thumbs_pzone_path, right_key)
 
             # Make Thumbs from them
-            left  = geomulticorr.src.thumb.Thumb(left_path)
-            right = geomulticorr.src.thumb.Thumb(right_path)
+            left  = src.geomulticorr.thumb.Thumb(left_path)
+            right = src.geomulticorr.thumb.Thumb(right_path)
 
         # Construction from two thumbs
         assert left.th_pz_name == right.th_pz_name, 'left and right have not the same pzone'
         assert left.th_path != right.th_path, 'left thumb is right thumb'
 
         # Metadata
         self.pa_pz_name = left.th_pz_name
```

### Comparing `geomulticorr-0.0.1/src/pzone.py` & `geomulticorr-0.0.2/src/geomulticorr/pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.1/src/session.py` & `geomulticorr-0.0.2/src/geomulticorr/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import tqdm
 import pandas as pd
 
 from osgeo import gdal
 import geopandas as gpd
 from telenvi import raster_tools as rt
 
-import geomulticorr.src.geomorph
-import geomulticorr.src.pzone
-import geomulticorr.src.pair
-import geomulticorr.src.spine
-import geomulticorr.src.thumb
-import geomulticorr.src.xzone
+import src.geomulticorr.geomorph
+import src.geomulticorr.pzone
+import src.geomulticorr.pair
+import src.geomulticorr.spine
+import src.geomulticorr.thumb
+import src.geomulticorr.xzone
 
-project_template_location = Path(Path(__file__).parent.parent, 'resources/project_template')
+project_template_location = Path(Path(__file__).parent, 'resources', 'project_template')
 
 def is_conform_to_gmc_template(target_root_path):
     """
     check the 3 conditions to be sure than the target root path is leading to a folder conform to the geomulticorr project data architecture
     """
 
     target_root_path = Path(target_root_path)
@@ -126,66 +126,66 @@
 
     def get_thumbs_overview(self, criterias=''):
         """Send a dataframe with informations about each thumb raster file meeting the criterias.
            If there's no criterias, send informations about all the thumbs of the project """
         return self._search_engine('Thumbs', criterias)
 
     def get_thumbs(self, criterias=''):
-        """Send a list of geomulticorr.src.thumb.Thumb objects meeting the criterias"""
+        """Send a list of src.geomulticorr.thumb.Thumb objects meeting the criterias"""
         selected_thumbs = self.get_thumbs_overview(criterias)
-        return [geomulticorr.src.thumb.Thumb(x.th_path) for x in selected_thumbs.iloc]
+        return [src.geomulticorr.thumb.Thumb(x.th_path) for x in selected_thumbs.iloc]
 
     def get_pairs_overview(self, criterias=''):
         """Send a dataframe with each possible Pair according to the Thumbs"""
         return self._search_engine('Pairs', criterias)
     
     def get_pairs(self, criterias=''):
-        """Send a list of geomulticorr.src.pair.Pairs objects meeting the criterias"""
+        """Send a list of src.geomulticorr.pair.Pairs objects meeting the criterias"""
         selected_pairs = self.get_pairs_overview(criterias)
-        return [geomulticorr.src.pair.Pair(self, target_path = x.pa_path) for x in selected_pairs.iloc]
+        return [src.geomulticorr.pair.Pair(self, target_path = x.pa_path) for x in selected_pairs.iloc]
 
     def get_pzones_overview(self, pz_name=''):
         """Send a dataframe with each pzone"""
         return self._search_engine('Pzones', pz_name)
 
     def get_pzones(self, pz_name=''):
-        """Send a list of geomulticorr.src.pzone.Pzones objects"""
+        """Send a list of src.geomulticorr.pzone.Pzones objects"""
         selected_pzones = self.get_pzones_overview(pz_name)
-        return [geomulticorr.src.pzone.Pzone(x.pz_name, self) for x in selected_pzones.iloc]
+        return [src.geomulticorr.pzone.Pzone(x.pz_name, self) for x in selected_pzones.iloc]
 
     def get_geomorphs_overview(self, criterias=''):
         """Send a dataframe with each geomorph"""
         return self._search_engine('Geomorphs', criterias)
 
     def get_geomorphs(self, criterias=''):
-        """Send a list of geomulticorr.src.geomorph.Geomorphs objects"""
+        """Send a list of src.geomulticorr.geomorph.Geomorphs objects"""
         selected_geomorphs = self.get_geomorphs_overview(criterias)
-        return [geomulticorr.src.geomorph.Geomorph(self, x.ge_frogi_id) for x in selected_geomorphs.iloc]
+        return [src.geomulticorr.geomorph.Geomorph(self, x.ge_frogi_id) for x in selected_geomorphs.iloc]
 
     def get_xzone(self, xz_id):
-        """Send a geomulticorr.src.xzones.Xzones object"""
-        return geomulticorr.src.xzones.Xzones(self, xz_id)
+        """Send a src.geomulticorr.xzones.Xzones object"""
+        return src.geomulticorr.xzones.Xzones(self, xz_id)
 
     def get_pairs_overview_on_period(self, ymin, ymax, criterias=''):
         """Retourne un tableau des paires completement incluses dans la période [yMin;yMax]"""
         pairs = self.get_pairs_overview(criterias)
         pairs['chrono_min'] = pairs.apply(lambda row: min(int(row.pa_left_date.split('-')[0]), int(row.pa_right_date.split('-')[0])), axis=1)
         pairs['chrono_max'] = pairs.apply(lambda row: max(int(row.pa_left_date.split('-')[0]), int(row.pa_right_date.split('-')[0])), axis=1)
         pairs = pairs[(pairs.chrono_min>=ymin)&(pairs.chrono_max<=ymax)]
         return pairs
 
     def get_pairs_on_period(self, ymin, ymax, criterias=''):
         """Retourne les paires completement incluses dans la période [yMin;yMax]"""
         board = self.get_pairs_overview_on_period(ymin, ymax, criterias)
-        pairs = [geomulticorr.src.pair.Pair(self, p.pa_path) for p in board.iloc]
+        pairs = [src.geomulticorr.pair.Pair(self, p.pa_path) for p in board.iloc]
         return pairs
 
     def get_spine(self, sp_id):
-        """Send a geomulticorr.src.spine.Spine object"""
-        return geomulticorr.src.spine.Spine(self, sp_id)
+        """Send a src.geomulticorr.spine.Spine object"""
+        return src.geomulticorr.spine.Spine(self, sp_id)
 
     def get_protomap(self, rawpath, extensions=['tif', 'jp2']):
         """make a vector layer with the extents of all the rasters stored under the rawpath
            and write metadata in hte layer attribute table"""
 
         # check the validity of the rawpath
         rawpath = Path(rawpath)
@@ -273,15 +273,15 @@
 
         # Copy the geodatabase before the transaction
         assert self.copy_geodb()
 
         # Get 2 version of the Thumbs layer
         opt_root = Path(self.p_raster_data)
         old = self._thumbs
-        new = gpd.GeoDataFrame([geomulticorr.src.thumb.Thumb(target_path).to_pdserie() for target_path in filter(lambda x: geomulticorr.src.thumb.THUMBNAME_PATTERN.match(x.name), list(opt_root.glob(pattern='**/opticals/*.tif')))])
+        new = gpd.GeoDataFrame([src.geomulticorr.thumb.Thumb(target_path).to_pdserie() for target_path in filter(lambda x: src.geomulticorr.thumb.THUMBNAME_PATTERN.match(x.name), list(opt_root.glob(pattern='**/opticals/*.tif')))])
 
         # Comparison
         common = new.merge(old, on=['th_path'])
         stables = old[old.th_path.isin(common.th_path)]
         addeds = new[~new.th_path.isin(common.th_path)]
 
         # Push it into the geodatabase
```

### Comparing `geomulticorr-0.0.1/src/spine.py` & `geomulticorr-0.0.2/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.1/src/thumb.py` & `geomulticorr-0.0.2/src/geomulticorr/thumb.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import pandas as pd
 
 from osgeo import gdal
 from telenvi import raster_tools as rt
 
-import geomulticorr.src.pair
+import src.geomulticorr.pair
 
 THUMBNAME_PATTERN = re.compile('^([a-z]|[A-Z]|-)+_[0-9]{4}(-[0-9]{2}){2}_.*.(tif|TIF)$')
 
 class Thumb:
 
     def __init__(self, target_path):
         target_path = Path(target_path)
@@ -34,15 +34,15 @@
             'th_sensor':self.th_sensor,
             'th_date':self.th_date ,
             'th_year':self.th_year,
             'th_valid':self.th_valid,
             'geometry':self.geometry})
 
     def __add__(self, right):
-        return geomulticorr.src.pair.GMC_Pair(left=self, right=right)
+        return src.geomulticorr.pair.GMC_Pair(left=self, right=right)
 
     def __repr__(self):
         return f"""---------
 type   : GMC_Thumb
 pzone  : {self.th_pz_name}
 date   : {self.th_date}
 sensor : {self.th_sensor}
```

### Comparing `geomulticorr-0.0.1/src/xzone.py` & `geomulticorr-0.0.2/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.1/tests/test_session.py` & `geomulticorr-0.0.2/tests/test_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import unittest
-import geomulticorr.src.session
+import src.geomulticorr.session
 
 path_to_test_session = '/media/duvanelt/TD002/sandbox_gmc/vanoise'
 pzone_name = 'iseran'
 
 class TestSession(unittest.TestCase):
 
     def setUp(self):
-        self.test_session = geomulticorr.src.session.open(path_to_test_session)
+        self.test_session = src.geomulticorr.session.open(path_to_test_session)
 
     def test_is_session(self):
-        self.assertIsInstance(self.test_session, geomulticorr.src.session.Session)
+        self.assertIsInstance(self.test_session, src.geomulticorr.session.Session)
 
     def test_get_thumbs(self):
         self.assertIsInstance(self.test_session.get_thumbs(), list)
         self.assertIsInstance(self.test_session.get_thumbs(pzone_name), list)
 
     def test_get_pairs(self):
         self.assertIsInstance(self.test_session.get_pairs(), list)
```

### Comparing `geomulticorr-0.0.1/LICENSE.md` & `geomulticorr-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.0.1/pyproject.toml` & `geomulticorr-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.0.1/PKG-INFO` & `geomulticorr-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

