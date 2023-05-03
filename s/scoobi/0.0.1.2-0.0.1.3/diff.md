# Comparing `tmp/scoobi-0.0.1.2.tar.gz` & `tmp/scoobi-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoobi-0.0.1.2.tar", last modified: Wed May  3 12:01:45 2023, max compression
+gzip compressed data, was "scoobi-0.0.1.3.tar", last modified: Wed May  3 15:27:04 2023, max compression
```

## Comparing `scoobi-0.0.1.2.tar` & `scoobi-0.0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:01:45.870963 scoobi-0.0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-03 12:01:45.870963 scoobi-0.0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-03 12:01:45.870963 scoobi-0.0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:01:45.866963 scoobi-0.0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:01:45.866963 scoobi-0.0.1.2/src/scoobi/
--rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/src/scoobi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/src/scoobi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:01:45.870963 scoobi-0.0.1.2/src/scoobi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:27:04.861273 scoobi-0.0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-03 15:26:50.000000 scoobi-0.0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-03 15:27:04.861273 scoobi-0.0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-03 15:26:50.000000 scoobi-0.0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-03 15:27:04.861273 scoobi-0.0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 15:26:50.000000 scoobi-0.0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:27:04.857273 scoobi-0.0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:27:04.861273 scoobi-0.0.1.3/src/scoobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-05-03 15:26:50.000000 scoobi-0.0.1.3/src/scoobi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-03 15:26:50.000000 scoobi-0.0.1.3/src/scoobi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:27:04.861273 scoobi-0.0.1.3/src/scoobi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-03 15:27:04.000000 scoobi-0.0.1.3/src/scoobi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 15:27:04.000000 scoobi-0.0.1.3/src/scoobi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:27:04.000000 scoobi-0.0.1.3/src/scoobi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:27:04.000000 scoobi-0.0.1.3/src/scoobi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:27:04.000000 scoobi-0.0.1.3/src/scoobi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 15:27:04.000000 scoobi-0.0.1.3/src/scoobi.egg-info/top_level.txt
```

### Comparing `scoobi-0.0.1.2/LICENSE` & `scoobi-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.2/PKG-INFO` & `scoobi-0.0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `scoobi-0.0.1.2/README.md` & `scoobi-0.0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.2/setup.py` & `scoobi-0.0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as rdme:
     desc = rdme.read()
 
 setup(
     name = 'scoobi',
-    version = '0.0.1.2',
+    version = '0.0.1.3',
     url='https://github.com/avialxee/scoobi',
     author='Avinash Kumar',
     author_email='avialxee@gmail.com',
     description='Solar Conventionality-based Organizing Observation data ( SCOOBI )',
     py_modules = ["scoobi"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
```

### Comparing `scoobi-0.0.1.2/src/scoobi/__init__.py` & `scoobi-0.0.1.3/src/scoobi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,50 +86,31 @@
         Ex. S-2022-11-01T02:02:20.001-HA.fits
 
     :destfolder: 
         (str) (Optional) (Default:None) (Superseeds final)
 
         The destination folder name where all the files will get saved.
 
-    :final: 
-        (boolean) (Optional) (Default:False)
-        
-        If the destination folder is Not defined and final=True then, all the files will save inside final_datafinal.
-
-    :rootfolder: 
-        (str) (Optional) (Default: "/data/solar_data/raw/Year2012/")
-        
-        This is the root folder inside which the destination folder is located For 
-        Ex. rootfolder="/data/solar_data/raw/Year2012/"
-
     *Return*
     
         (str) folder name for the fits file.
 
     """
-    params={'destfolder': 'processed/', 'final':False,
-     'rootfolder':'/data/Solar_data/Avinash_codes/april/'}
+    params={'destfolder': 'processed/',
+    }
     params.update(kwargs)
-    if Path(params["rootfolder"]).exists():
-        if params['destfolder'] is None:
-            if params['final']:
-                params['destfolder']='final_data/'
-            else:
-                params['destfolder']='processed/'
-        dcf=fitsname.split('-')
-        dcf_date=dcf[3].split('T')[0]
-        #currentfolder=f'{params["rootfolder"]}{params["destfolder"]}{dcf[1]}/{dcf[1]}{dcf[2]}{dcf_date}/'
-        currentfolder=f'{params["rootfolder"]}{params["destfolder"]}{dcf[1]}/{dcf[2]}/{dcf_date}/'
-        if not Path(currentfolder).exists():
-            Path(currentfolder).mkdir(parents=True,exist_ok=True)
-        return f'{currentfolder}{fitsname}'
         
-    else:
-        raise Exception('Please check rootfolder path')
-
+    dcf=fitsname.split('-')
+    dcf_date=dcf[3].split('T')[0]
+    #currentfolder=f'{params["rootfolder"]}{params["destfolder"]}{dcf[1]}/{dcf[1]}{dcf[2]}{dcf_date}/'
+    currentfolder=f'{params["destfolder"]}{dcf[1]}/{dcf[2]}/{dcf_date}/'
+    if not Path(currentfolder).exists():
+        Path(currentfolder).mkdir(parents=True,exist_ok=True)
+    return f'{currentfolder}{fitsname}'
+        
 def tif_to_fits(tiffile, magick=True, header=None, **kwargs):
     """
     *Parameters*
     
     :tiffile:
         (str) (Required)
 
@@ -156,26 +137,14 @@
         If not provided will build name according to the timestamp in the TIFF header.
         Ex. S-2022-11-01T02:02:20.001-HA.fits
 
     :destfolder: 
         (str) (Optional) (Default:None)
 
         The destination folder name where all the files will get saved.
-
-    :final: 
-        (boolean) (Optional) (Default:False)
-        
-        If the destination folder is Not defined and final=True then, all the files will save inside final_datafinal.
-
-    :rootfolder: 
-        (str) (Optional) (Default: "/data/archived_data_solar/")
-        
-        This is the root folder inside which the destination folder is located For 
-        Ex. rootfolder="/data/archived_data_solar"
-
     """
     params={'fitsname':None, 'telescope':'HA'}
     params.update(kwargs)
     tifpath = Path(tiffile)
     if header is None:
         header=header_dictfromtiff(tiffile)
     else:
@@ -219,30 +188,31 @@
     """
     takes input as list of string tiff folder paths and executes tif to fits using for loop to each folder path.
     see *tif_to_fits()* for the list of parameters.
     If tif to fits conversion fails, the file is saved in "corrupt/" (can be changed from call) folder at the tiff source folder.
     """
     params={'failed_folder':'corrupt/'}
     params.update(kwargs)
-    if 'tiff_folder' in params.keys(): params['failed_folder']=f"{params['tiff_folder']}/{params['failed_folder']}"
         
     if isinstance(tiffolderlist,list):
         for tifffolder in tiffolderlist:
             listtiff=search_file(tifffolder,'.tif', recursive=True)
             for f in listtiff:
-                try:
-                    tif_to_fits(f, **kwargs)
-                except:
+                if not 'corrupt' in f:
+                    params['failed_folder']=f"{Path(f).parent}/corrupt/"
                     try:
-                        # if Path(f).stat().st_size <= desiredsize:
-                        Path(params['failed_folder']).mkdir(parents=True,exist_ok=True)
-                        shutil.copy(str(f), str(f"{params['failed_folder']}/{Path(f).name}"))
+                        tif_to_fits(f, **kwargs)
                     except:
-                        with open('failed.scoobi','a') as sf:
-                            sf.write(f)
+                        try:
+                            # if Path(f).stat().st_size <= desiredsize:
+                            Path(params['failed_folder']).mkdir(parents=True,exist_ok=True)
+                            shutil.copy(str(f), str(f"{params['failed_folder']}/{Path(f).name}"))
+                        except:
+                            with open('failed.scoobi','+a') as sf:
+                                sf.write(f"{f}\n")
     else:
         raise Exception(f'Is "{tiffolderlist}" a list?')
         
 #log generation
 def compare_datetime(**kwargs):
     params={
         'fits_folder':'/home/avi/archived_data_solar/processed_data/2012/',
```

### Comparing `scoobi-0.0.1.2/src/scoobi/cli.py` & `scoobi-0.0.1.3/src/scoobi/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,14 @@
     if args.ct and not args.no_datedfolder: compare_datetime(**params)
     if args.no_datedfolder and args.ct: compare_datetime_nofolder(**params)
     if args.rc: print(read_configfile(configfile))
     if args.cc: print(create_config(params,configfile))
     if args.rt: print(str(read_tif(params['tiff_folder'])['Image DateTime'].values))
     if args.do: 
         if '.tif' not in params['tiff_folder']: 
-            print(tif2fits_bulk(params['tiff_folder'].split(','), rootfolder=params['fits_folder']))
+            print(tif2fits_bulk(params['tiff_folder'].split(','), destfolder=params['fits_folder']))
         else:
-            print(tif_to_fits(params['tiff_folder'], rootfolder=params['fits_folder']))
+            print(tif_to_fits(params['tiff_folder'], destfolder=params['fits_folder']))
     if args.th: thumb_gen(params['fits_folder'])
         
 if __name__=='__main__':
     cli()
```

### Comparing `scoobi-0.0.1.2/src/scoobi.egg-info/PKG-INFO` & `scoobi-0.0.1.3/src/scoobi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

