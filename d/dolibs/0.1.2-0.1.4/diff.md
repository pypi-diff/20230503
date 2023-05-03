# Comparing `tmp/dolibs-0.1.2.tar.gz` & `tmp/dolibs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibs-0.1.2.tar", last modified: Tue May  2 16:20:27 2023, max compression
+gzip compressed data, was "dolibs-0.1.4.tar", last modified: Wed May  3 12:12:16 2023, max compression
```

## Comparing `dolibs-0.1.2.tar` & `dolibs-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-02 16:20:27.421991 dolibs-0.1.2/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-05-02 16:20:27.421847 dolibs-0.1.2/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      628 2023-05-02 14:40:08.000000 dolibs-0.1.2/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-02 16:20:27.420807 dolibs-0.1.2/dolibs/
--rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.1.2/dolibs/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)     4602 2023-05-02 15:47:01.000000 dolibs-0.1.2/dolibs/skintemp.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-02 16:20:27.421628 dolibs-0.1.2/dolibs.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      205 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       47 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)        7 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-02 16:20:27.422044 dolibs-0.1.2/setup.cfg
--rw-r--r--   0 leandro    (501) staff       (20)      569 2023-05-02 16:20:02.000000 dolibs-0.1.2/setup.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-03 12:12:16.182770 dolibs-0.1.4/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-05-03 12:12:16.182634 dolibs-0.1.4/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     1152 2023-05-03 10:26:07.000000 dolibs-0.1.4/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-03 12:12:16.181216 dolibs-0.1.4/dolibs/
+-rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.1.4/dolibs/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4591 2023-05-03 09:47:15.000000 dolibs-0.1.4/dolibs/skintemp.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-03 12:12:16.182170 dolibs-0.1.4/dolibs.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-05-03 12:12:16.000000 dolibs-0.1.4/dolibs.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      205 2023-05-03 12:12:16.000000 dolibs-0.1.4/dolibs.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-03 12:12:16.000000 dolibs-0.1.4/dolibs.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       71 2023-05-03 12:12:16.000000 dolibs-0.1.4/dolibs.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        7 2023-05-03 12:12:16.000000 dolibs-0.1.4/dolibs.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-03 12:12:16.182835 dolibs-0.1.4/setup.cfg
+-rw-r--r--   0 leandro    (501) staff       (20)      599 2023-05-03 12:12:13.000000 dolibs-0.1.4/setup.py
```

### Comparing `dolibs-0.1.2/dolibs/skintemp.py` & `dolibs-0.1.4/dolibs/skintemp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #skin temperature image functions for Drought Observatory platform
 # input: year, month and day of the image to be retrieved from ERA5 CDS.
 # output: return code - 0 OK
 import cdsapi 
+import rioxarray
 import numpy as np
 import xarray as xr
 import requests
 import os
 import sqlalchemy as db
 import logging
 
@@ -37,68 +38,64 @@
                 '18:00', '19:00', '20:00',
                 '21:00', '22:00', '23:00',
                         ],
                     'area': [
                         70, -13, 20, 40,
                         ],  
             },
-            basepath+'/skintemp_'+str(year_in)+'_'+str(month_in)+'.nc')
-        
+            basepath+'/skintemp_'+str(year_in)+'_'+str(month_in)+'.nc')    
         
         print('open nc file')
         nc_file = basepath+'/skintemp_'+str(year_in)+'_'+str(month_in)+'.nc'
         print('Loading dataset')
         ds = xr.open_dataset(nc_file).load()
 
         print('Calculate daily temperature and transform in Celsius')
         daily_data = ds.resample(time='d').mean()
         daily_data_celsius = daily_data.skt - 273.15
 
         print('Start cube elaboration')
         #always skip last retrieved day cause it could be incomplete
         for i in range((len(daily_data_celsius) - 1)):
             dout = daily_data_celsius[i,:,:]
-            dout.rio.write_crs("EPSG:4326", inplace=True).rio.to_raster(nc_file.title()+'_out_'+str((i+1))+'.tiff')
+            dout.rio.write_crs("EPSG:4326", inplace=True).rio.to_raster(nc_file+'_out_'+str((i+1))+'.tiff')
             #set file and form data for post call
 
             files_in = {
-                'file': (nc_file.title()+'_out_'+str((i+1))+'.tiff', open(nc_file.title()+'_out_'+str((i+1))+'.tiff', 'rb'),'multipart/form-data'),
+                'file': (nc_file+'_out_'+str((i+1))+'.tiff', open(nc_file+'_out_'+str((i+1))+'.tiff', 'rb'),'multipart/form-data'),
                 'year': str(year_in),
                 'month': str(month_in),
                 'day': str((i+1))
             }
         
             #call rest api
             response = requests.post(myurl, files=files_in)
         
             print(response.content)
             dout.close()
             #delete tiff image
-            print("remove "+nc_file.title()+'_out_'+str((i+1))+'.tiff')
-            os.remove(nc_file.title()+'_out_'+str((i+1))+'.tiff')
+            print("remove "+nc_file+'_out_'+str((i+1))+'.tiff')
+            os.remove(nc_file+'_out_'+str((i+1))+'.tiff')
         daily_data_celsius.close()
         daily_data.close()
             
         ds.close()
       
-    
-
-
         #delete nc file
         print("remove "+nc_file)
         os.remove(nc_file)
         return 0
     except Exception as e:
         logging.error(e)
         return 1
     
 
 def get_last_day(connect_str: str) -> int:
     retval = -1
-    engine = db.create_engine(connect_str)
+    engine = db.create_engine(connect_str,future=True)
     connection = engine.connect()
     metadata = db.MetaData()
     try:
         sql = db.text("select max(dtime) from postgis.acquisizioni inner join postgis.skin_temperature using (id_acquisizione)")
 
         ResultProxy = connection.execute(sql).fetchall()
         
@@ -110,15 +107,15 @@
     except:
         connection.close()
         return -1
     
 def del_image(connect_str: str, dtime_from: str, dtime_to: str) -> int:
     retval = -1
     print(connect_str)
-    engine = db.create_engine(connect_str)
+    engine = db.create_engine(connect_str,future=True)
     connection = engine.connect()
     metadata = db.MetaData()
     try:
      
 
         sql = db.text("delete from postgis.skin_temperature where id_acquisizione in (select id_acquisizione from postgis.acquisizioni inner join postgis.imgtypes using (id_imgtype) where imgtype = 'SKINTEMP' and dtime between '"+dtime_from+"'::timestamp and '"+dtime_to+"'::timestamp)")
```

### Comparing `dolibs-0.1.2/setup.py` & `dolibs-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 setup(
     name='dolibs',
     packages=find_packages(include=['dolibs']),
-    version='0.1.2',
+    version='0.1.4',
     url='https://github.com/n3tmaster/ERA5_procedures',
     description='Library for importing ERA5 Copernicus data into Drought Observatory platform',
     author='Leandro Rocchi - CNR',
     author_email='leandro.rocchi@cnr.it',
     license='MIT',
-    install_requires=['cdsapi','numpy','xarray','sqlalchemy','psycopg2-binary'],
+    install_requires=['cdsapi','scipy','netcdf4','rioxarray','numpy','xarray','sqlalchemy','psycopg2-binary'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest==4.4.1'],
     test_suite='tests',
 )
```

