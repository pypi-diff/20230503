# Comparing `tmp/satellite_weather_downloader-1.8.2.tar.gz` & `tmp/satellite_weather_downloader-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellite_weather_downloader-1.8.2.tar", max compression
+gzip compressed data, was "satellite_weather_downloader-1.8.3.tar", max compression
```

## Comparing `satellite_weather_downloader-1.8.2.tar` & `satellite_weather_downloader-1.8.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-04-14 17:09:47.313802 satellite_weather_downloader-1.8.2/LICENSE
--rw-r--r--   0        0        0     3072 2023-04-14 17:09:47.313802 satellite_weather_downloader-1.8.2/README.md
--rw-r--r--   0        0        0     1862 2023-04-14 17:11:54.347297 satellite_weather_downloader-1.8.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/__init__.py
--rw-r--r--   0        0        0      190 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/__init__.py
--rw-r--r--   0        0        0     9715 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/extract_reanalysis.py
--rw-r--r--   0        0        0       52 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/__init__.py
--rw-r--r--   0        0        0    12112 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/api_vars.py
--rw-r--r--   0        0        0    16153 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/prompt.py
--rw-r--r--   0        0        0     2924 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/request.py
--rw-r--r--   0        0        0      296 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/__init__.py
--rw-r--r--   0        0        0       20 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/__init__.py
--rw-r--r--   0        0        0     1360 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas.py
--rw-r--r--   0        0        0       11 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.cst
--rw-r--r--   0        0        0     9413 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.dbf
--rw-r--r--   0        0        0      417 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.prj
--rw-r--r--   0        0        0 11174984 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.shp
--rw-r--r--   0        0        0      372 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.shx
--rw-r--r--   0        0        0       77 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/__init__.py
--rw-r--r--   0        0        0     4119 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/extract_coordinates.py
--rw-r--r--   0        0        0     1351 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/extract_latlons.py
--rw-r--r--   0        0        0  1175429 2023-04-14 17:09:47.393805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/municipios.json
--rw-r--r--   0        0        0       40 2023-04-14 17:09:47.393805 satellite_weather_downloader-1.8.2/satellite/weather/utils/__init__.py
--rw-r--r--   0        0        0     4871 2023-04-14 17:09:47.393805 satellite_weather_downloader-1.8.2/satellite/weather/utils/episem.py
--rw-r--r--   0        0        0    13631 2023-04-14 17:09:47.393805 satellite_weather_downloader-1.8.2/satellite/weather/xr_extensions.py
--rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-03 18:11:19.813823 satellite_weather_downloader-1.8.3/LICENSE
+-rw-r--r--   0        0        0     3072 2023-05-03 18:11:19.813823 satellite_weather_downloader-1.8.3/README.md
+-rw-r--r--   0        0        0     1862 2023-05-03 18:14:17.198639 satellite_weather_downloader-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/__init__.py
+-rw-r--r--   0        0        0     9715 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/extract_reanalysis.py
+-rw-r--r--   0        0        0       52 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/__init__.py
+-rw-r--r--   0        0        0    12112 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/api_vars.py
+-rw-r--r--   0        0        0    16153 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/prompt.py
+-rw-r--r--   0        0        0     2924 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/request.py
+-rw-r--r--   0        0        0      296 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/__init__.py
+-rw-r--r--   0        0        0       20 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/__init__.py
+-rw-r--r--   0        0        0     1360 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas.py
+-rw-r--r--   0        0        0       11 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.cst
+-rw-r--r--   0        0        0     9413 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.dbf
+-rw-r--r--   0        0        0      417 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.prj
+-rw-r--r--   0        0        0 11174984 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.shp
+-rw-r--r--   0        0        0      372 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.shx
+-rw-r--r--   0        0        0       77 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/__init__.py
+-rw-r--r--   0        0        0     4119 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/extract_coordinates.py
+-rw-r--r--   0        0        0     1351 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/extract_latlons.py
+-rw-r--r--   0        0        0  1175429 2023-05-03 18:11:19.901824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/municipios.json
+-rw-r--r--   0        0        0       40 2023-05-03 18:11:19.901824 satellite_weather_downloader-1.8.3/satellite/weather/utils/__init__.py
+-rw-r--r--   0        0        0     4871 2023-05-03 18:11:19.901824 satellite_weather_downloader-1.8.3/satellite/weather/utils/episem.py
+-rw-r--r--   0        0        0    13565 2023-05-03 18:11:19.901824 satellite_weather_downloader-1.8.3/satellite/weather/xr_extensions.py
+-rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.8.3/PKG-INFO
```

### Comparing `satellite_weather_downloader-1.8.2/LICENSE` & `satellite_weather_downloader-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/README.md` & `satellite_weather_downloader-1.8.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,36 +21,36 @@
 
 Version 1.X includes only methods for Brazil's data format and cities.
 
 ## Create requests via Interactive shell
 Since SWT version 1.5, it is possible to create dynamic requests using the interactive
 python shell or via method call:
 ```python
-from satellite_downloader import request
+from satellite.downloader import request
 
 file = request.ERA5_reanalysis(
     filename = 'my_dataset_file'
     # Any ERA5 Reanalysis option can be passed in the method
 )
 ```
 ```
 NOTE: This feature is still in experimental versions, please submit an issue if you find any bug.
 ```
 
 ## Extract Brazil NetCDF4 file from a date range
 ``` python
-import satellite_downloader
+from satellite import downloader
 
-file = satellite_downloader.download_br_netcdf('2023-01-01', '2023-01-07')
+file = downloader.download_br_netcdf('2023-01-01', '2023-01-07')
 
 ```
 
 ## Load the dataset
 ``` python
-import satellite_weather as sat
+from satellite import weather as sat
 br_dataset = sat.load_dataset(file)
 
 ```
 
 ## Usage of `copebr` extension
 ``` python
 rio_geocode = 3304557 # Rio de Janeiro's geocode (IBGE)
```

### Comparing `satellite_weather_downloader-1.8.2/pyproject.toml` & `satellite_weather_downloader-1.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "satellite-weather-downloader"
-version = "1.8.2"  # changed by semantic-release
+version = "1.8.3"  # changed by semantic-release
 description = "The modules available in this package are designed to capture and proccess satellite data from Copernicus"
 readme = "README.md"
 authors = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 maintainers = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/osl-incubator/satellite-weather-downloader"
 homepage = "https://github.com/osl-incubator/satellite-weather-downloader"
```

### Comparing `satellite_weather_downloader-1.8.2/satellite/downloader/extract_reanalysis.py` & `satellite_weather_downloader-1.8.3/satellite/downloader/extract_reanalysis.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/api_vars.py` & `satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/api_vars.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/prompt.py` & `satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/prompt.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/downloader/request.py` & `satellite_weather_downloader-1.8.3/satellite/downloader/request.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas.py` & `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.dbf` & `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.dbf`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.shp` & `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.shp`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/extract_coordinates.py` & `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/extract_latlons.py` & `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/extract_latlons.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/municipios.json` & `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/municipios.json`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/weather/utils/episem.py` & `satellite_weather_downloader-1.8.3/satellite/weather/utils/episem.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.2/satellite/weather/xr_extensions.py` & `satellite_weather_downloader-1.8.3/satellite/weather/xr_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy as np
 import xarray as xr
 from loguru import logger
 from matplotlib.path import Path
 from metpy.units import units
 from shapely.geometry.polygon import Polygon
 from sqlalchemy import create_engine
+from sqlalchemy.engine import Connectable
 
 from . import _brazil
 
 xr.set_options(keep_attrs=True)
 
 
 @xr.register_dataset_accessor('copebr')
@@ -72,30 +73,30 @@
         return pool.submit(
             asyncio.run, self._final_dataframe(geocodes=geocodes, raw=raw)
         ).result()
 
     def to_sql(
         self,
         geocodes: Union[list, int],
-        sql_uri: str,
+        con: Connectable,
         tablename: str,
         schema: str,
         raw: bool = False,
     ) -> None:
         """ 
         Reads the data for each geocode and insert the rows into the
         database one by one, created by sqlalchemy engine with the URI.
         This method is convenient to prevent the memory overhead when
         executing with a large amount of geocodes.
         """
         geocodes = [geocodes] if isinstance(geocodes, int) else geocodes
         for geocode in geocodes:
             self._geocode_to_sql(
                 geocode=geocode,
-                sql_uri=sql_uri,
+                con=con,
                 schema=schema,
                 tablename=tablename,
                 raw=raw,
             )
         logger.debug(
             f'{len(geocodes)} geocodes updated on {schema}.{tablename}'
         )
@@ -147,15 +148,15 @@
         df = df.assign(geocodigo=da.from_array(geocode))
 
         return df
 
     def _geocode_to_sql(
         self,
         geocode: int,
-        sql_uri: str,
+        con: Connectable,
         schema: str,
         tablename: str,
         raw: bool,
     ):
         ds = asyncio.run(self._geocode_ds(geocode, raw))
         df = ds.to_dataframe()
         del ds
@@ -163,23 +164,21 @@
         df = df.assign(geocodigo=geocodes)
         df = df.reset_index(drop=False)
         if raw:
             df = df.rename(columns={'time': 'datetime'})
         else:
             df = df.rename(columns={'time': 'date'})
 
-        engine = create_engine(sql_uri)
-        with engine.connect() as conn:
-            df.to_sql(
-                name=tablename,
-                schema=schema,
-                con=conn,
-                if_exists='append',
-                index=False,
-            )
+        df.to_sql(
+            name=tablename,
+            schema=schema,
+            con=con,
+            if_exists='append',
+            index=False,
+        )
 
     async def _geocode_ds(self, geocode: int, raw=False):
         """
         This is the most important method of the extension. It will
         slice the dataset according to the geocode provided, do the
         math and the parse of the units to Br's format, and reduce by
         min, mean and max by day, if the `raw` is false.
```

### Comparing `satellite_weather_downloader-1.8.2/PKG-INFO` & `satellite_weather_downloader-1.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satellite-weather-downloader
-Version: 1.8.2
+Version: 1.8.3
 Summary: The modules available in this package are designed to capture and proccess satellite data from Copernicus
 Home-page: https://github.com/osl-incubator/satellite-weather-downloader
 License: GNU GPL v3.0
 Author: Luã Bida Vacaro
 Author-email: luabidaa@gmail.com
 Maintainer: Luã Bida Vacaro
 Maintainer-email: luabidaa@gmail.com
@@ -62,36 +62,36 @@
 
 Version 1.X includes only methods for Brazil's data format and cities.
 
 ## Create requests via Interactive shell
 Since SWT version 1.5, it is possible to create dynamic requests using the interactive
 python shell or via method call:
 ```python
-from satellite_downloader import request
+from satellite.downloader import request
 
 file = request.ERA5_reanalysis(
     filename = 'my_dataset_file'
     # Any ERA5 Reanalysis option can be passed in the method
 )
 ```
 ```
 NOTE: This feature is still in experimental versions, please submit an issue if you find any bug.
 ```
 
 ## Extract Brazil NetCDF4 file from a date range
 ``` python
-import satellite_downloader
+from satellite import downloader
 
-file = satellite_downloader.download_br_netcdf('2023-01-01', '2023-01-07')
+file = downloader.download_br_netcdf('2023-01-01', '2023-01-07')
 
 ```
 
 ## Load the dataset
 ``` python
-import satellite_weather as sat
+from satellite import weather as sat
 br_dataset = sat.load_dataset(file)
 
 ```
 
 ## Usage of `copebr` extension
 ``` python
 rio_geocode = 3304557 # Rio de Janeiro's geocode (IBGE)
```

