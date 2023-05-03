# Comparing `tmp/scoobi-0.0.1.1.tar.gz` & `tmp/scoobi-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoobi-0.0.1.1.tar", last modified: Tue Apr 25 15:54:27 2023, max compression
+gzip compressed data, was "scoobi-0.0.1.2.tar", last modified: Wed May  3 12:01:45 2023, max compression
```

## Comparing `scoobi-0.0.1.1.tar` & `scoobi-0.0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:54:27.318221 scoobi-0.0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-25 15:54:27.318221 scoobi-0.0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-25 15:54:27.318221 scoobi-0.0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:54:27.314221 scoobi-0.0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:54:27.314221 scoobi-0.0.1.1/src/scoobi/
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/src/scoobi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/src/scoobi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:54:27.318221 scoobi-0.0.1.1/src/scoobi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:01:45.870963 scoobi-0.0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-03 12:01:45.870963 scoobi-0.0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-03 12:01:45.870963 scoobi-0.0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:01:45.866963 scoobi-0.0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:01:45.866963 scoobi-0.0.1.2/src/scoobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/src/scoobi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-03 12:01:22.000000 scoobi-0.0.1.2/src/scoobi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:01:45.870963 scoobi-0.0.1.2/src/scoobi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 12:01:45.000000 scoobi-0.0.1.2/src/scoobi.egg-info/top_level.txt
```

### Comparing `scoobi-0.0.1.1/LICENSE` & `scoobi-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.1/PKG-INFO` & `scoobi-0.0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `scoobi-0.0.1.1/README.md` & `scoobi-0.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.1/setup.py` & `scoobi-0.0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as rdme:
     desc = rdme.read()
 
 setup(
     name = 'scoobi',
-    version = '0.0.1.1',
+    version = '0.0.1.2',
     url='https://github.com/avialxee/scoobi',
     author='Avinash Kumar',
     author_email='avialxee@gmail.com',
     description='Solar Conventionality-based Organizing Observation data ( SCOOBI )',
     py_modules = ["scoobi"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
@@ -26,12 +26,12 @@
                       ],
     extras_require = {
         "dev" : ["pytest>=3.7",
         ]
     },
      entry_points={ 
         "console_scripts": [
-            "scoobi=scoobi.cli:cli",
+            "scoobi=scoobi.cli:cli"
         ],
     },
 
 )
```

### Comparing `scoobi-0.0.1.1/src/scoobi/__init__.py` & `scoobi-0.0.1.2/src/scoobi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from astropy.io import fits
 from astropy.time import Time
 import astropy.units as u
 from collections import defaultdict
 import csv
 import datetime
+import shutil
 
 
 class SCOOBI():
     def __init__():
         pass
 
 # Helper
@@ -101,23 +102,23 @@
         Ex. rootfolder="/data/solar_data/raw/Year2012/"
 
     *Return*
     
         (str) folder name for the fits file.
 
     """
-    params={'destfolder': '/processed/', 'final':False,
+    params={'destfolder': 'processed/', 'final':False,
      'rootfolder':'/data/Solar_data/Avinash_codes/april/'}
     params.update(kwargs)
     if Path(params["rootfolder"]).exists():
         if params['destfolder'] is None:
             if params['final']:
                 params['destfolder']='final_data/'
             else:
-                params['destfolder']='processed_data/'
+                params['destfolder']='processed/'
         dcf=fitsname.split('-')
         dcf_date=dcf[3].split('T')[0]
         #currentfolder=f'{params["rootfolder"]}{params["destfolder"]}{dcf[1]}/{dcf[1]}{dcf[2]}{dcf_date}/'
         currentfolder=f'{params["rootfolder"]}{params["destfolder"]}{dcf[1]}/{dcf[2]}/{dcf_date}/'
         if not Path(currentfolder).exists():
             Path(currentfolder).mkdir(parents=True,exist_ok=True)
         return f'{currentfolder}{fitsname}'
@@ -179,41 +180,69 @@
         header=header_dictfromtiff(tiffile)
     else:
         header.update(header_dictfromtiff(tiffile))
     if params['fitsname'] is None:
         # name convention : *S + DATETIME + TELESCOPE*
         fitsfile=f'S-{header["DATE-OBS"]}-{params["telescope"]}.fits'
         fitsfile=build_foldername(fitsfile, **kwargs)
-        
     
     if magick:
-        print(tiffile)
+        #print(tiffile)
         subprocess.run(['convert', str(tiffile), fitsfile])
         print(f'created {fitsfile}')
     else:
         pass
     with fits.open(fitsfile, 'update') as f:
         for hdu in f:
             hdu.header.update(header)
             hdu.header['TELESCOP']=params['telescope']
             hdu.header['FILENAME']=tifpath.name
             hdu.header['HISTORY']=f'{tiffile}'
             hdu.header['HISTORY']=f'scoobi'
 
+def thumb_gen(fits_folder, out_folder=None, thumb_folder="Thumbnails", force=False):
+    """
+    Creates thumbnails for the fits file provided in the fits_folder path.
+    """
+    if fits_folder:
+        allfile=search_file(f"{fits_folder}/",'.fits', recursive=True)
+        
+        for fitsfile in allfile:
+            if not out_folder:out_folder=Path(fitsfile).parent
+            jpgfolder=f"{out_folder}/{thumb_folder}"
+            jpgfile=f"{jpgfolder}/{Path(fitsfile).stem}.jpg"
+            
+            if not Path(jpgfolder).exists(): Path(jpgfolder).mkdir(parents=True,exist_ok=True)
+            if not Path(jpgfile).exists() or force: subprocess.run(["convert", fitsfile,"-linear-stretch","1x1","-resize", "56%", jpgfile ])
+            
 
 def tif2fits_bulk(tiffolderlist, **kwargs):
     """
     takes input as list of string tiff folder paths and executes tif to fits using for loop to each folder path.
     see *tif_to_fits()* for the list of parameters.
+    If tif to fits conversion fails, the file is saved in "corrupt/" (can be changed from call) folder at the tiff source folder.
     """
+    params={'failed_folder':'corrupt/'}
+    params.update(kwargs)
+    if 'tiff_folder' in params.keys(): params['failed_folder']=f"{params['tiff_folder']}/{params['failed_folder']}"
+        
     if isinstance(tiffolderlist,list):
         for tifffolder in tiffolderlist:
             listtiff=search_file(tifffolder,'.tif', recursive=True)
             for f in listtiff:
-                tif_to_fits(f, **kwargs)
+                try:
+                    tif_to_fits(f, **kwargs)
+                except:
+                    try:
+                        # if Path(f).stat().st_size <= desiredsize:
+                        Path(params['failed_folder']).mkdir(parents=True,exist_ok=True)
+                        shutil.copy(str(f), str(f"{params['failed_folder']}/{Path(f).name}"))
+                    except:
+                        with open('failed.scoobi','a') as sf:
+                            sf.write(f)
     else:
         raise Exception(f'Is "{tiffolderlist}" a list?')
         
 #log generation
 def compare_datetime(**kwargs):
     params={
         'fits_folder':'/home/avi/archived_data_solar/processed_data/2012/',
```

### Comparing `scoobi-0.0.1.1/src/scoobi/cli.py` & `scoobi-0.0.1.2/src/scoobi/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from scoobi import compare_datetime, read_tif, Time, tif2fits_bulk, tif_to_fits, compare_datetime_nofolder
+from scoobi import compare_datetime, read_tif, Time, tif2fits_bulk, tif_to_fits, compare_datetime_nofolder, thumb_gen
 from collections import defaultdict
 from pathlib import Path
 
 def read_configfile(filepath):
     with open(filepath,'r') as f:
         params = defaultdict(list)
         pr=f.read().splitlines()
@@ -35,15 +35,14 @@
                 o.write(f'{k}={",".join(v)}\n')
             elif isinstance(v, range):
                 o.write(f'{k}={v.start},{v.stop}\n')
             else:
                 o.write(f'{k}={v}\n')
     return f'configfile:{out}'
 
-
 parser = argparse.ArgumentParser('scoobi',description="""
 Solar Conventionality-based Organizing Observation data ( SCOOBI )""", formatter_class=argparse.RawDescriptionHelpFormatter)
 
 # pa = parser.add_subparsers(help='compare datetimes') # subparser is used like $pip "install"
 
 parser.add_argument('-f','--fits_folder', help='source') #positionals
 parser.add_argument('-t','--tiff_folder', help='tiff folder path')
@@ -63,14 +62,15 @@
 
 parser.add_argument('--no-datedfolder', action='store_true', dest='no_datedfolder',help='if not needed to create dated folder') 
 parser.add_argument('-rt','--read-time', action='store_true', dest='rt',help='reads time from a tiff file') 
 parser.add_argument('-ct','--compare-time', action='store_true', dest='ct',help='compares time from a fits file to a tiff file') 
 parser.add_argument('-rc','--read-config',action='store_true',dest='rc', help=" read config, bool")
 parser.add_argument('-cc','--create-config',action='store_true',dest='cc', help=" create config, if called with rc would modify from and to the CONFIG_FILE path")
 parser.add_argument('-do','--do-conversion',action='store_true',dest='do', help=" create fits from tiff file and take care of the folder structure. Requires tiff_folder path")
+parser.add_argument('-th','--thumbnail', action='store_true', dest='th',help='True/False for creating thumbnails; The fits folder path is required but should be more specific e.g atleaset including the /processed; should not be used with -do')
 
 args=parser.parse_args()
 def cli():
     params=default_params()
     header = defaultdict(list)
     if args.fits_folder: params['fits_folder']=args.fits_folder
     if args.output_file: params['csv_file']=args.output_file
@@ -108,10 +108,11 @@
     if args.cc: print(create_config(params,configfile))
     if args.rt: print(str(read_tif(params['tiff_folder'])['Image DateTime'].values))
     if args.do: 
         if '.tif' not in params['tiff_folder']: 
             print(tif2fits_bulk(params['tiff_folder'].split(','), rootfolder=params['fits_folder']))
         else:
             print(tif_to_fits(params['tiff_folder'], rootfolder=params['fits_folder']))
-    
+    if args.th: thumb_gen(params['fits_folder'])
+        
 if __name__=='__main__':
     cli()
```

### Comparing `scoobi-0.0.1.1/src/scoobi.egg-info/PKG-INFO` & `scoobi-0.0.1.2/src/scoobi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

