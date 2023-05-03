# Comparing `tmp/cygnsslib-1.2.3.tar.gz` & `tmp/cygnsslib-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cygnsslib-1.2.3.tar", last modified: Sat Jan 28 08:21:07 2023, max compression
+gzip compressed data, was "cygnsslib-1.3.0.tar", last modified: Wed May  3 02:18:58 2023, max compression
```

## Comparing `cygnsslib-1.2.3.tar` & `cygnsslib-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/
--rw-rw-rw-   0 root         (0) root         (0)    15976 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13126 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/src/cygnsslib/
--rw-rw-rw-   0 root         (0) root         (0)    14486 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/CygDdmId.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    64581 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/cyg.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/src/cygnsslib/cygnss_download/
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/cygnss_download/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/src/cygnsslib/data_downloader/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/data_downloader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/data_downloader/cyg_ant_ptrn.py
--rw-rw-rw-   0 root         (0) root         (0)    12672 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/data_downloader/download_cyg_rawif.py
--rw-rw-rw-   0 root         (0) root         (0)    24921 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/data_downloader/download_cygnss.py
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/data_downloader/download_cygnss_sftp.py
--rw-rw-rw-   0 root         (0) root         (0)    13468 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/data_downloader/download_srtm.py
--rw-rw-rw-   0 root         (0) root         (0)     7427 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/data_downloader/pass_core.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/istarmap.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/plotting.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/src/cygnsslib/srtm_download/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/srtm_download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9286 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/cygnsslib/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/src/cygnsslib.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    15976 2023-01-28 08:21:07.000000 cygnsslib-1.2.3/src/cygnsslib.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1008 2023-01-28 08:21:07.000000 cygnsslib-1.2.3/src/cygnsslib.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-28 08:21:07.000000 cygnsslib-1.2.3/src/cygnsslib.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-01-28 08:21:07.000000 cygnsslib-1.2.3/src/cygnsslib.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-01-28 08:21:07.000000 cygnsslib-1.2.3/src/cygnsslib.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-28 08:21:07.705688 cygnsslib-1.2.3/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/tests/list_loc2kml.py
--rw-rw-rw-   0 root         (0) root         (0)     1583 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/tests/test_download_cyg_data.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/tests/test_download_srtm.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/tests/test_find_land_prod_from_cvs.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/tests/test_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/tests/test_search_within_circle.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2023-01-28 08:20:56.000000 cygnsslib-1.2.3/src/tests/test_write_sp_within_radius.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 02:18:58.137295 cygnsslib-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    15896 2023-05-03 02:18:58.137295 cygnsslib-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13006 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-03 02:18:58.137295 cygnsslib-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 02:18:58.133295 cygnsslib-1.3.0/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 02:18:58.133295 cygnsslib-1.3.0/src/cygnsslib/
+-rw-rw-rw-   0 root         (0) root         (0)    14486 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/CygDdmId.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    63464 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/cyg.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 02:18:58.137295 cygnsslib-1.3.0/src/cygnsslib/cygnss_download/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/cygnss_download/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 02:18:58.137295 cygnsslib-1.3.0/src/cygnsslib/data_downloader/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/data_downloader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/data_downloader/cyg_ant_ptrn.py
+-rw-rw-rw-   0 root         (0) root         (0)     5663 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/data_downloader/download_cyg_rawif.py
+-rw-rw-rw-   0 root         (0) root         (0)    19211 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/data_downloader/download_cygnss.py
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/data_downloader/download_cygnss_sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)    13187 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/data_downloader/download_srtm.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/istarmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     4926 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/plotting.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 02:18:58.137295 cygnsslib-1.3.0/src/cygnsslib/srtm_download/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/srtm_download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9205 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/cygnsslib/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 02:18:58.137295 cygnsslib-1.3.0/src/cygnsslib.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    15896 2023-05-03 02:18:58.000000 cygnsslib-1.3.0/src/cygnsslib.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-03 02:18:58.000000 cygnsslib-1.3.0/src/cygnsslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-03 02:18:58.000000 cygnsslib-1.3.0/src/cygnsslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-03 02:18:58.000000 cygnsslib-1.3.0/src/cygnsslib.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-03 02:18:58.000000 cygnsslib-1.3.0/src/cygnsslib.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 02:18:58.137295 cygnsslib-1.3.0/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/tests/list_loc2kml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/tests/test_download_cyg_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/tests/test_download_srtm.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/tests/test_find_land_prod_from_cvs.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/tests/test_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/tests/test_search_within_circle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2023-05-03 02:18:46.000000 cygnsslib-1.3.0/src/tests/test_write_sp_within_radius.py
```

### Comparing `cygnsslib-1.2.3/PKG-INFO` & `cygnsslib-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cygnsslib
-Version: 1.2.3
+Version: 1.3.0
 Summary: Toolset for working with CYGNSS data and downloading CYGNSS data from PODAAC
 Home-page: https://bitbucket.org/usc_mixil/cygnsslib
 Author: Amer Melebari and James D. Campbell
 Author-email: amelebar@usc.edu
 License: UNKNOWN
 Description: # CYGNSS Library
         
@@ -30,40 +30,42 @@
         You can then remove the local copy if you wish. Alternatively, if you wish to be able to make changes to your local copy without having to reinstall the package for the changes to take effect (e.g., for development purposes), you can use the following instead:
         ```console
         pip uninstall cygnsslib
         ```
         ### Required packages
         Here the required Python packages:
         ```console
-        gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pbkdf2 pycrypto pyproj pysftp requests setuptools tqdm paramiko
+        gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pysftp requests tqdm
         ```
         Note: `gdal` can be installed using conda   
         ```console
         conda install -c conda-forge gdal  
         ```
         or using [this method](https://mothergeo-py.readthedocs.io/en/latest/development/how-to/gdal-ubuntu-pkg.html) in Ubuntu  
-        ## How to Use The Package
+        Also, you need the modified data-subscriber package from [https://github.com/MiXIL/data-subscriber](https://github.com/MiXIL/data-subscriber)  
+        
+        ## How to Use The Package  
         The cygnsslib has several modules:  
         1. Identify CYGNSS DDMs within a specific region  
         2. Group DDMs within a specific distance  
         3. Download CYGNSS antenna pattern  
         4. CygDdmId Class, which work as CYGNSS DDM ID  
         5. Download CYGNSS data from PO.DAAC  
-        6. Download SRTM data from NASA Earth Data
+        6. Download SRTM data from NASA Earth Data  
         7. Other functionality related to CYGNSS data  
           
-        For most of the library, you need to set the environment variable ``CYGNSS_L1_PATH`` to the path of the CYGNSS L1 data. i.e.
-        ```console 
-        CYGNSS_L1_PATH=/cygnss_data/L1/v3.0
-        ```
-        Note the folder needs to be named as the version (e.g. `v3.0`)name in PODAAC, and the parent folder need to be `L1`
-        You can set the environment variable for the session in python as follows:
-        ```python
+        For most of the library, you need to set the environment variable ``CYGNSS_L1_PATH`` to the path of the CYGNSS L1 data. i.e.  
+        ```console  
+        CYGNSS_L1_PATH=/cygnss_data/L1/v3.1
+        ```   
+        Note the folder needs to be named as the version (e.g. `v3.1`)name in PODAAC, and the parent folder need to be `L1`
+        You can set the environment variable for the session in python as follows:  
+        ```python  
         import os
-        os.environ['CYGNSS_L1_PATH'] = '/cygnss_data/L1/v3.0'
+        os.environ['CYGNSS_L1_PATH'] = '/cygnss_data/L1/v3.1'
         ```
         
         For SRTM you can specify the main path by specifying the environment variable ``SRTM_PATH``. The files will be saved in `SRTM_PATH\hgt`
         ### Identify CYGNSS DDMs within a specific region
         
         There are several ways to find the DDM within a region.  
         1. find all the DDMs that their SP location within a specific distance from a specific location.  
@@ -72,15 +74,16 @@
         Below an example of the usage:
         
         ```python
         import cygnsslib
         import numpy as np
         import datetime as dt
         
-        cygnss_l1_path = None  # this will make the strip get the path from os.environ["CYGNSS_L1_PATH"]
+        # this will make the strip get the path from os.environ["CYGNSS_L1_PATH"]
+        cygnss_l1_path = None  
         year = 2019
         days_list = np.arange(1, 100)
         ref_pos = (37.1906, -105.9921)  # (lat,long)
         radius = 10e3  # [m]
         thesh_ddm_snr = 3.0  # split DDMs into above thesh_ddm_snr and below thesh_ddm_snr. Above this value the DDM image will be saved
         thesh_noise = 1  # noise threshold, each pixel in the DDM below this value will be replaced by this value
         kml_out_tag = f'my_data'  # tag for all the output files, ex: my_data_above_thresh.kml
@@ -89,17 +92,18 @@
         options = {'save_cvs': False,
                    'save_ddm_img': True,
                    'plt_tag': '',
                    'title_img_inc_ddm_time': False,
                    'img_save_type': ['png'],
                    'sheet_type': 'xls'}
         
-        cygnsslib.write_sp_within_radius(cygnss_l1_path, year=2019, daylist=days_list, ref_pos=ref_pos, radius=radius, out_folder_path=f'', 
-                                         out_file_tag=kml_out_tag, thresh_ddm_snr=thesh_ddm_snr, plt_thresh_noise=thesh_noise, download_cygnss_data=True, 
-                                         out_options=options, save_podaac_pass=save_podaac_pass)
+        out_folder_path = 'my_ddms'
+        cygnsslib.write_sp_within_radius(cygnss_l1_path, year, days_list, ref_pos, radius, 
+                                         out_folder_path, kml_out_tag, thesh_ddm_snr, thesh_noise, 
+                                         download_cygnss_data=True, out_options=options)
         
         start_date = dt.date(year=2019, month=1, day=1)
         end_date = dt.date(year=2019, month=6, day=10)  # the end date included in the search
         cygnsslib.write_sp_within_radius_between_dates(cygnss_l1_path, start_date, end_date, ref_pos=ref_pos,
                                                        radius=radius, out_folder_path=f'', out_file_tag=kml_out_tag, thresh_ddm_snr=thesh_ddm_snr,
                                                        plt_thresh_noise=thesh_noise, download_cygnss_data=True,
                                                        out_options=options, save_podaac_pass=save_podaac_pass)
@@ -196,39 +200,39 @@
         ### Download CYGNSS data from PO.DAAC
         
         You can download both the standard DDMs and the rawif data. You can choose to download data between two dates or a list of days in the year.  
         If a file exists, the code will not re-download it.  
         Note if you select `check_md5_exist_file=True`, then the code will do an md5 check for existing files. This will ensure existing files are good. However, this will make it very slow.
         
         Below an example of downloading DDMs and the rawif files. The files will be organized as they're in PODAAC.
+        
         ```python
         from cygnsslib import cygnss_download
         import datetime as dt
         import numpy as np
         
         # Download data in the same year and range of days
         days_list = np.arange(5, 10)
         data_year = 2020
         # list_sc_num = [3]
         list_sc_num = None  # Will download all the 8 spacecrafts 
-        cyg_data_ver = f'v3.0'
-        cygnss_download.download_cyg_files(data_year, days_list, list_sc_num=list_sc_num, cyg_data_ver=cyg_data_ver, 
-                                           check_md5_exist_file=False, cyg_data_lvl=f'L1', save_podaac_pass=True)
+        cyg_data_ver = f'v3.1'
+        cygnss_download.download_cyg_files(data_year, days_list, list_sc_num, cyg_data_ver, cyg_data_lvl=f'L1', checksum_exist_file=False)
         # Downloading data between two dates (including end date)
         st_date = dt.date(year=2019, month=1, day=12)
         end_date = dt.date(year=2020, month=1, day=3)
         
-        cygnss_download.download_cyg_files_between_date(st_date, end_date, list_sc_num=list_sc_num, cyg_data_ver=cyg_data_ver, 
-                                                        check_md5_exist_file=False, cyg_data_lvl=f'L1', save_podaac_pass=True)
+        cygnss_download.download_cyg_files_between_date(st_date, end_date, list_sc_num, cyg_data_ver=cyg_data_ver, cyg_data_lvl=f'L1',
+                                                        checksum_exist_file=False)
         
         # Downloading rawif data 
         download_l1_data = True  # This will download the corresponding L1 data
-        cygnss_download.download_cyg_rawif_files(data_year,days_list, list_sc_num, save_podaac_pass=True, 
+        cygnss_download.download_cyg_rawif_files(data_year, days_list, list_sc_num, save_podaac_pass=True,
                                                  download_l1_data=download_l1_data)
-        cygnss_download.download_rawif_cyg_files_between_date(st_date,end_date, list_sc_num, save_podaac_pass=True, 
+        cygnss_download.download_rawif_cyg_files_between_date(st_date, end_date, list_sc_num, save_podaac_pass=True,
                                                               download_l1_data=download_l1_data)
         
         ```
         #### PODAAC user/pass related notes
         You can get the PO.DAAC Drive API Credentials from https://podaac-tools.jpl.nasa.gov/drive/  
         If you entered the wrong PODAAC user/pass, you'll be asked to re-enter them again. However, you need to re-start the code after that so the saved user/pass are loaded again.  
         
@@ -252,19 +256,20 @@
         files_lat = [21, 22, 20]
         files_lon = [29, 30]
         srtm_download.download_srtm_ght_files(files_lat, files_lon, save_pass=True, unzipfile=False, remove_zippedfile=True)  
         
         
         ```
         #### EarthData username and pass related notes  
-        You can reset your EarthData user/pass and enter new user/pass using the following code. Note when you run the code, you'll be asked to enter the new user/pass  
+        You can reset your EarthData user/pass and enter new user/pass using the following code. Note when you run the code, you'll be asked to enter the new user/pass
+        
         ```python
         from cygnsslib import srtm_download
         
-        srtm_download.get_earthdata_cred(save_pass=True, reset_pass=True) 
+        srtm_download.get_earthdata_cred() 
         ```
         ### Other functionality related to CYGNSS data   
         
         Create a circle or a square on the ground and export it to kml file  
         ```python
         import cygnsslib
         ref_pos = [37.1906, -105.9921] #  [lat,long]
```

### Comparing `cygnsslib-1.2.3/README.md` & `cygnsslib-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,40 +22,42 @@
 You can then remove the local copy if you wish. Alternatively, if you wish to be able to make changes to your local copy without having to reinstall the package for the changes to take effect (e.g., for development purposes), you can use the following instead:
 ```console
 pip uninstall cygnsslib
 ```
 ### Required packages
 Here the required Python packages:
 ```console
-gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pbkdf2 pycrypto pyproj pysftp requests setuptools tqdm paramiko
+gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pysftp requests tqdm
 ```
 Note: `gdal` can be installed using conda   
 ```console
 conda install -c conda-forge gdal  
 ```
 or using [this method](https://mothergeo-py.readthedocs.io/en/latest/development/how-to/gdal-ubuntu-pkg.html) in Ubuntu  
-## How to Use The Package
+Also, you need the modified data-subscriber package from [https://github.com/MiXIL/data-subscriber](https://github.com/MiXIL/data-subscriber)  
+
+## How to Use The Package  
 The cygnsslib has several modules:  
 1. Identify CYGNSS DDMs within a specific region  
 2. Group DDMs within a specific distance  
 3. Download CYGNSS antenna pattern  
 4. CygDdmId Class, which work as CYGNSS DDM ID  
 5. Download CYGNSS data from PO.DAAC  
-6. Download SRTM data from NASA Earth Data
+6. Download SRTM data from NASA Earth Data  
 7. Other functionality related to CYGNSS data  
   
-For most of the library, you need to set the environment variable ``CYGNSS_L1_PATH`` to the path of the CYGNSS L1 data. i.e.
-```console 
-CYGNSS_L1_PATH=/cygnss_data/L1/v3.0
-```
-Note the folder needs to be named as the version (e.g. `v3.0`)name in PODAAC, and the parent folder need to be `L1`
-You can set the environment variable for the session in python as follows:
-```python
+For most of the library, you need to set the environment variable ``CYGNSS_L1_PATH`` to the path of the CYGNSS L1 data. i.e.  
+```console  
+CYGNSS_L1_PATH=/cygnss_data/L1/v3.1
+```   
+Note the folder needs to be named as the version (e.g. `v3.1`)name in PODAAC, and the parent folder need to be `L1`
+You can set the environment variable for the session in python as follows:  
+```python  
 import os
-os.environ['CYGNSS_L1_PATH'] = '/cygnss_data/L1/v3.0'
+os.environ['CYGNSS_L1_PATH'] = '/cygnss_data/L1/v3.1'
 ```
 
 For SRTM you can specify the main path by specifying the environment variable ``SRTM_PATH``. The files will be saved in `SRTM_PATH\hgt`
 ### Identify CYGNSS DDMs within a specific region
 
 There are several ways to find the DDM within a region.  
 1. find all the DDMs that their SP location within a specific distance from a specific location.  
@@ -64,15 +66,16 @@
 Below an example of the usage:
 
 ```python
 import cygnsslib
 import numpy as np
 import datetime as dt
 
-cygnss_l1_path = None  # this will make the strip get the path from os.environ["CYGNSS_L1_PATH"]
+# this will make the strip get the path from os.environ["CYGNSS_L1_PATH"]
+cygnss_l1_path = None  
 year = 2019
 days_list = np.arange(1, 100)
 ref_pos = (37.1906, -105.9921)  # (lat,long)
 radius = 10e3  # [m]
 thesh_ddm_snr = 3.0  # split DDMs into above thesh_ddm_snr and below thesh_ddm_snr. Above this value the DDM image will be saved
 thesh_noise = 1  # noise threshold, each pixel in the DDM below this value will be replaced by this value
 kml_out_tag = f'my_data'  # tag for all the output files, ex: my_data_above_thresh.kml
@@ -81,17 +84,18 @@
 options = {'save_cvs': False,
            'save_ddm_img': True,
            'plt_tag': '',
            'title_img_inc_ddm_time': False,
            'img_save_type': ['png'],
            'sheet_type': 'xls'}
 
-cygnsslib.write_sp_within_radius(cygnss_l1_path, year=2019, daylist=days_list, ref_pos=ref_pos, radius=radius, out_folder_path=f'', 
-                                 out_file_tag=kml_out_tag, thresh_ddm_snr=thesh_ddm_snr, plt_thresh_noise=thesh_noise, download_cygnss_data=True, 
-                                 out_options=options, save_podaac_pass=save_podaac_pass)
+out_folder_path = 'my_ddms'
+cygnsslib.write_sp_within_radius(cygnss_l1_path, year, days_list, ref_pos, radius, 
+                                 out_folder_path, kml_out_tag, thesh_ddm_snr, thesh_noise, 
+                                 download_cygnss_data=True, out_options=options)
 
 start_date = dt.date(year=2019, month=1, day=1)
 end_date = dt.date(year=2019, month=6, day=10)  # the end date included in the search
 cygnsslib.write_sp_within_radius_between_dates(cygnss_l1_path, start_date, end_date, ref_pos=ref_pos,
                                                radius=radius, out_folder_path=f'', out_file_tag=kml_out_tag, thresh_ddm_snr=thesh_ddm_snr,
                                                plt_thresh_noise=thesh_noise, download_cygnss_data=True,
                                                out_options=options, save_podaac_pass=save_podaac_pass)
@@ -188,39 +192,39 @@
 ### Download CYGNSS data from PO.DAAC
 
 You can download both the standard DDMs and the rawif data. You can choose to download data between two dates or a list of days in the year.  
 If a file exists, the code will not re-download it.  
 Note if you select `check_md5_exist_file=True`, then the code will do an md5 check for existing files. This will ensure existing files are good. However, this will make it very slow.
 
 Below an example of downloading DDMs and the rawif files. The files will be organized as they're in PODAAC.
+
 ```python
 from cygnsslib import cygnss_download
 import datetime as dt
 import numpy as np
 
 # Download data in the same year and range of days
 days_list = np.arange(5, 10)
 data_year = 2020
 # list_sc_num = [3]
 list_sc_num = None  # Will download all the 8 spacecrafts 
-cyg_data_ver = f'v3.0'
-cygnss_download.download_cyg_files(data_year, days_list, list_sc_num=list_sc_num, cyg_data_ver=cyg_data_ver, 
-                                   check_md5_exist_file=False, cyg_data_lvl=f'L1', save_podaac_pass=True)
+cyg_data_ver = f'v3.1'
+cygnss_download.download_cyg_files(data_year, days_list, list_sc_num, cyg_data_ver, cyg_data_lvl=f'L1', checksum_exist_file=False)
 # Downloading data between two dates (including end date)
 st_date = dt.date(year=2019, month=1, day=12)
 end_date = dt.date(year=2020, month=1, day=3)
 
-cygnss_download.download_cyg_files_between_date(st_date, end_date, list_sc_num=list_sc_num, cyg_data_ver=cyg_data_ver, 
-                                                check_md5_exist_file=False, cyg_data_lvl=f'L1', save_podaac_pass=True)
+cygnss_download.download_cyg_files_between_date(st_date, end_date, list_sc_num, cyg_data_ver=cyg_data_ver, cyg_data_lvl=f'L1',
+                                                checksum_exist_file=False)
 
 # Downloading rawif data 
 download_l1_data = True  # This will download the corresponding L1 data
-cygnss_download.download_cyg_rawif_files(data_year,days_list, list_sc_num, save_podaac_pass=True, 
+cygnss_download.download_cyg_rawif_files(data_year, days_list, list_sc_num, save_podaac_pass=True,
                                          download_l1_data=download_l1_data)
-cygnss_download.download_rawif_cyg_files_between_date(st_date,end_date, list_sc_num, save_podaac_pass=True, 
+cygnss_download.download_rawif_cyg_files_between_date(st_date, end_date, list_sc_num, save_podaac_pass=True,
                                                       download_l1_data=download_l1_data)
 
 ```
 #### PODAAC user/pass related notes
 You can get the PO.DAAC Drive API Credentials from https://podaac-tools.jpl.nasa.gov/drive/  
 If you entered the wrong PODAAC user/pass, you'll be asked to re-enter them again. However, you need to re-start the code after that so the saved user/pass are loaded again.  
 
@@ -244,19 +248,20 @@
 files_lat = [21, 22, 20]
 files_lon = [29, 30]
 srtm_download.download_srtm_ght_files(files_lat, files_lon, save_pass=True, unzipfile=False, remove_zippedfile=True)  
 
 
 ```
 #### EarthData username and pass related notes  
-You can reset your EarthData user/pass and enter new user/pass using the following code. Note when you run the code, you'll be asked to enter the new user/pass  
+You can reset your EarthData user/pass and enter new user/pass using the following code. Note when you run the code, you'll be asked to enter the new user/pass
+
 ```python
 from cygnsslib import srtm_download
 
-srtm_download.get_earthdata_cred(save_pass=True, reset_pass=True) 
+srtm_download.get_earthdata_cred() 
 ```
 ### Other functionality related to CYGNSS data   
 
 Create a circle or a square on the ground and export it to kml file  
 ```python
 import cygnsslib
 ref_pos = [37.1906, -105.9921] #  [lat,long]
```

### Comparing `cygnsslib-1.2.3/setup.py` & `cygnsslib-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as fh:
     req = fh.read()
 
 setup(
     name='cygnsslib',
-    version='1.2.3',
+    version='1.3.0',
     author='Amer Melebari and James D. Campbell',
     author_email='amelebar@usc.edu',
     description='Toolset for working with CYGNSS data and downloading CYGNSS data from PODAAC',
     long_description=long_description,
     install_requires=req.split(),
     long_description_content_type="text/markdown",
     url='https://bitbucket.org/usc_mixil/cygnsslib',
```

### Comparing `cygnsslib-1.2.3/src/cygnsslib/CygDdmId.py` & `cygnsslib-1.3.0/src/cygnsslib/CygDdmId.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         original_l1_path = os.environ.get("CYGNSS_L1_PATH")
     dist_cygnss_l1_path = os.path.join(os.environ.get("CYGNSS_PATH"), 'L1', new_version)
     in_cygddmid.fill_file_name(cygnss_l1_path=original_l1_path)
     cygnss_original_ver_file = os.path.join(original_l1_path, f'{in_cygddmid.year:04d}', f'{in_cygddmid.day:03d}', in_cygddmid.file_name)
     ds_cyg = Dataset(cygnss_original_ver_file, 'r')
     ds_cyg.set_auto_maskandscale(False)
     tcs = pd.Timestamp(ds_cyg.time_coverage_start)
-    tcs_in_sec = (tcs - copy.deepcopy(tcs).replace(hour=0, minute=0, second=0, microsecond=0, nanosecond=0)).delta * 1e-9
+    tcs_in_sec = (tcs - copy.deepcopy(tcs).replace(hour=0, minute=0, second=0, microsecond=0, nanosecond=0)).value * 1e-9
 
     # Number of seconds relative to the beginning of the day [sec]. resolution is nano second
     sel_sample_time_sec = ds_cyg.variables['ddm_timestamp_utc'][in_cygddmid.samp_id] + tcs_in_sec
     ds_cyg.close()  # close the file
 
     # open the land file
     cyg_dis_ver_file_name = find_cygnss_file(data_year=in_cygddmid.year, data_day=in_cygddmid.day, sc_num=in_cygddmid.sc_num,
@@ -143,15 +143,15 @@
     :return: L1 sample id (zero-based)
     :type: int
     """
     ds_cyg = Dataset(cyg_full_file, 'r')
     ds_cyg.set_auto_maskandscale(False)
 
     tcs = pd.Timestamp(ds_cyg.time_coverage_start)
-    tcs_in_sec = (tcs - copy.deepcopy(tcs).replace(hour=0, minute=0, second=0, microsecond=0, nanosecond=0)).delta * 1e-9
+    tcs_in_sec = (tcs - copy.deepcopy(tcs).replace(hour=0, minute=0, second=0, microsecond=0, nanosecond=0)).value * 1e-9
 
     sample_time = np.array(ds_cyg.variables['ddm_timestamp_utc']) + tcs_in_sec  # Number of seconds relative to the beginning of the day [sec]
     # resolution is nano second
     ds_cyg.close()
 
     sel_ddm_tf = np.isclose(sample_time, sel_sample_time, rtol=0, atol=1e-6)  # set atol=1e-9 as the resolution in nano second
     if sel_ddm_tf.sum() > 1:  # if we have two samples with the same time tamp
```

### Comparing `cygnsslib-1.2.3/src/cygnsslib/__init__.py` & `cygnsslib-1.3.0/src/cygnsslib/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,12 +8,9 @@
 # from cygnsslib import srtm_download
 # CygDdmID class
 from cygnsslib import CygDdmId
 
 # land products
 from cygnsslib.util import find_land_prod_sample_id_from_excel, get_ant_pattern_for_diff_versions
 
-# pass manager
-from cygnsslib.data_downloader import pass_core as MixilKeys
-
 # Antenna Patterns
 from cygnsslib.data_downloader.cyg_ant_ptrn import download_cyg_antenna_patterns
```

### Comparing `cygnsslib-1.2.3/src/cygnsslib/cyg.py` & `cygnsslib-1.3.0/src/cygnsslib/cyg.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,16 +103,15 @@
     if sp_rx_gain <= 0.0:
         qflags_msg_list.append('negative_sp_rx_gain')
     return qflags_msg_list, land_flag, our_flags
 
 
 def write_sp_within_radius(cygnss_l1_dir: Optional[str], year: int, daylist: Union[list[int], np.ndarray, int], ref_pos: tuple[float, float],
                            radius: float, out_folder_path: str, out_file_tag: str, thresh_ddm_snr: float = -9999.0, plt_thresh_noise: float = 1.0,
-                           download_cygnss_data: bool = True, out_options: Optional[dict] = None,
-                           save_podaac_pass: bool = True) -> tuple[str, str, str]:
+                           download_cygnss_data: bool = True, out_options: Optional[dict] = None) -> tuple[str, str, str]:
     """
         This  search for all CYGNSS DDMs within radius from the ref_pos in the daylist time period. It exports the plots of the DDMs with SNR above
         thesh_ddm_snr
     Note: The structure of the folders/files of  CYGNSS date need to be the same as the POO.DAC
 
     :param cygnss_l1_dir: the path of the main folder of CYGNSS L1 data (after the versions) (if None it uses os.environ.get("CYGNSS_L1_PATH"))
     :param year: year number in 4 digits (ex. 2020) (you can't select multiple years for now
@@ -122,15 +121,14 @@
     :param out_folder_path: output folder path
     :param out_file_tag: tag for all the output files, ex: "out_root"_above_thresh.kml
     :param out_options: currently we only implemented save_csv and save_ddm_img
     :param thresh_ddm_snr: DDM SNR threshold, above this value the DDM map image will be saved
     :param plt_thresh_noise: noise threshold, each pixel in the DDM below this value will be replaced by this value
     :param download_cygnss_data: download CYGNSS L1 data if they're not available ?
     :param out_options: currently we only implemented save_csv and save_ddm_img
-    :param save_podaac_pass: save PO DAAC username/password? ignored if download_cygnss_data = False
     :return: high SNR, low SNR, reference kml files paths
 
     """
     geod = Geodesic.WGS84
     geo_shape = ogr.Geometry(ogr.wkbLinearRing)
 
     for angle in np.arange(0, 361, 1):
@@ -146,22 +144,21 @@
     if np.size(daylist) == 1:
         daylist = [int(daylist)]
     date_list = np.zeros(len(daylist), dtype=dt.date)
     for idx, iday in enumerate(daylist):
         date_list[idx] = dt.date(year, month=1, day=1) + dt.timedelta(days=int(iday) - 1)
     out_root = os.path.join(out_folder_path, out_file_tag)
     return _write_sp_from_poly_or_circle(cygnss_l1_dir, date_list, ref_pos, radius, thresh_ddm_snr, plt_thresh_noise, out_root, poly, tf_poly,
-                                         download_cygnss_data, out_options, save_podaac_pass)
+                                         download_cygnss_data, out_options)
 
 
 def write_sp_within_box_between_dates(st_date: dt.date, end_date: dt.date, lat_lim: Union[list[float], np.ndarray],
                                       lon_lim: Union[list[float], np.ndarray], out_folder_path: str, out_file_tag: str,
                                       thresh_ddm_snr: float = -9999.0, plt_thresh_noise: float = 1.0, download_cygnss_data: bool = True,
-                                      out_options: Optional[dict] = None, save_podaac_pass: bool = True,
-                                      cygnss_l1_dir: Optional[str] = None) -> tuple[str, str, str]:
+                                      out_options: Optional[dict] = None, cygnss_l1_dir: Optional[str] = None) -> tuple[str, str, str]:
     geo_shape = ogr.Geometry(ogr.wkbLinearRing)
     lat_lim = np.sort(lat_lim)
     lon_lim = np.sort(lon_lim)
 
     geo_shape.AddPoint(lon_lim[0], lat_lim[0])
     geo_shape.AddPoint(lon_lim[1], lat_lim[0])
     geo_shape.AddPoint(lon_lim[1], lat_lim[1])
@@ -178,22 +175,21 @@
 
     num_days = (end_date - st_date).days + 1
     date_list = np.zeros(num_days, dtype=dt.date)
     for iday in range(0, num_days):
         date_list[iday] = st_date + dt.timedelta(days=iday)
     out_root = os.path.join(out_folder_path, out_file_tag)
     return _write_sp_from_poly_or_circle(cygnss_l1_dir, date_list, ref_pos, radius, thresh_ddm_snr, plt_thresh_noise, out_root, poly, tf_poly,
-                                         download_cygnss_data, out_options, save_podaac_pass)
+                                         download_cygnss_data, out_options)
 
 
 def write_sp_within_box(year: int, daylist: Union[list[int], np.ndarray, int], lat_lim: Union[list[float], np.ndarray],
                         lon_lim: Union[list[float], np.ndarray], out_folder_path: str, out_file_tag: str,
                         thresh_ddm_snr: float = -9999.0, plt_thresh_noise: float = 1.0, download_cygnss_data: bool = True,
-                        out_options: Optional[dict] = None, save_podaac_pass: bool = True,
-                        cygnss_l1_dir: Optional[str] = None) -> tuple[str, str, str]:
+                        out_options: Optional[dict] = None, cygnss_l1_dir: Optional[str] = None) -> tuple[str, str, str]:
     geo_shape = ogr.Geometry(ogr.wkbLinearRing)
     lat_lim = np.sort(lat_lim)
     lon_lim = np.sort(lon_lim)
 
     geo_shape.AddPoint(lon_lim[0], lat_lim[0])
     geo_shape.AddPoint(lon_lim[1], lat_lim[0])
     geo_shape.AddPoint(lon_lim[1], lat_lim[1])
@@ -212,21 +208,21 @@
     if np.size(daylist) == 1:
         daylist = [int(daylist)]
     date_list = np.zeros(len(daylist), dtype=dt.date)
     for idx, iday in enumerate(daylist):
         date_list[idx] = dt.date(year, month=1, day=1) + dt.timedelta(days=int(iday) - 1)
     out_root = os.path.join(out_folder_path, out_file_tag)
     return _write_sp_from_poly_or_circle(cygnss_l1_dir, date_list, ref_pos, radius, thresh_ddm_snr, plt_thresh_noise, out_root, poly, tf_poly,
-                                         download_cygnss_data, out_options, save_podaac_pass)
+                                         download_cygnss_data, out_options)
 
 
 def write_sp_within_radius_between_dates(cygnss_l1_dir: Optional[str], st_date: dt.date, end_date: dt.date, ref_pos: tuple[float, float],
                                          radius: float, out_folder_path: str, out_file_tag: str, thresh_ddm_snr: float = -9999.0,
-                                         plt_thresh_noise: float = 1.0, download_cygnss_data: bool = True, out_options: Optional[dict] = None,
-                                         save_podaac_pass: bool = True) -> tuple[str, str, str]:
+                                         plt_thresh_noise: float = 1.0, download_cygnss_data: bool = True,
+                                         out_options: Optional[dict] = None) -> tuple[str, str, str]:
     """
         This search for all CYGNSS DDMs within radius from the ref_pos from st_date to end_date. It exports the plots of the DDMs with SNR above
         thesh_ddm_snr
     Note: The structure of the folders/files of  CYGNSS date need to be the same as the POO.DAC
 
     :param cygnss_l1_dir: the path of the main folder of CYGNSS L1 data (after the versions) (if None it uses os.environ.get("CYGNSS_L1_PATH"))
     :param st_date: start date
@@ -236,15 +232,14 @@
     :param out_folder_path: output folder path
     :param out_file_tag: tag for all the output files, ex: "out_root"_above_thresh.kml
     :param out_options: currently we only implemented save_csv and save_ddm_img
     :param thresh_ddm_snr: DDM SNR threshold, above this value the DDM map image will be saved
     :param plt_thresh_noise: noise threshold, each pixel in the DDM below this value will be replaced by this value
     :param download_cygnss_data: download CYGNSS L1 data if they're not available ?
     :param out_options: currently we only implemented save_csv and save_ddm_img
-    :param save_podaac_pass: save PO DAAC username/password? ignored if download_cygnss_data = False
     :return: high SNR, low SNR, reference kml files paths
     """
     geod = Geodesic.WGS84
     geo_shape = ogr.Geometry(ogr.wkbLinearRing)
 
     for angle in np.arange(0, 361, 1):
         poly_point = geod.Direct(ref_pos[0], ref_pos[1], angle, radius)
@@ -258,20 +253,20 @@
     num_days = (end_date - st_date).days + 1
     date_list = np.zeros(num_days, dtype=dt.date)
     for iday in range(0, num_days):
         date_list[iday] = st_date + dt.timedelta(days=iday)
     out_root = os.path.join(out_folder_path, out_file_tag)
 
     return _write_sp_from_poly_or_circle(cygnss_l1_dir, date_list, ref_pos, radius, thresh_ddm_snr, plt_thresh_noise, out_root, poly, tf_poly,
-                                         download_cygnss_data, out_options, save_podaac_pass)
+                                         download_cygnss_data, out_options)
 
 
 def write_sp_from_kml(cygnss_l1_dir: Optional[str], year: int, daylist: Union[list[int], np.ndarray], in_kml: str, out_folder_path: str,
                       out_file_tag: str, thresh_ddm_snr: float = -9999.0, plt_thresh_noise: float = 1.0, download_cygnss_data: bool = True,
-                      out_options: Optional[dict] = None, save_podaac_pass: bool = True) -> tuple[str, str, str]:
+                      out_options: Optional[dict] = None) -> tuple[str, str, str]:
     """
     This  search for all CYGNSS DDMs within the polygon in the in_kml within the daylist time period. It exports the plots of the DDMs with SNR above
     thesh_ddm_snr
     Note: The structure of the folders/files of  CYGNSS date need to be the same as the POO.DAC
 
     :param cygnss_l1_dir: the path of the main folder of CYGNSS L1 data (after the versions) (if None it uses os.environ.get("CYGNSS_L1_PATH"))
     :type cygnss_l1_dir: str or None
@@ -287,16 +282,14 @@
     :type thresh_ddm_snr: float
     :param plt_thresh_noise: noise threshold, each pixel in the DDM below this value will be replaced by this value
     :type plt_thresh_noise: float
     :param download_cygnss_data: download CYGNSS L1 data if they're not available ?
     :type download_cygnss_data: bool
     :param out_options: currently we only implemented save_csv and save_ddm_img
     :type out_options: dict or None
-    :param save_podaac_pass: save PO DAAC username/password? ignored if download_cygnss_data = False
-    :type save_podaac_pass: bool
     :return: high SNR, low SNR, reference kml files paths
     """
     # Read polygon from input file and make longitude positive
     poly = get_poly(in_kml)
     # Find specular points inside polygon and write them to output
     ref_pos = [0.0, 0.0]
     ref_pos[1], ref_pos[0], *_ = poly.Centroid().GetPoint()
@@ -307,21 +300,20 @@
         daylist = [int(daylist)]
     date_list = np.zeros(len(daylist), dtype=dt.date)
     for idx, iday in enumerate(daylist):
         date_list[idx] = dt.date(year, month=1, day=1) + dt.timedelta(days=int(iday) - 1)
     out_root = os.path.join(out_folder_path, out_file_tag)
 
     return _write_sp_from_poly_or_circle(cygnss_l1_dir, date_list, ref_pos, radius, thresh_ddm_snr, plt_thresh_noise, out_root, poly, tf_poly,
-                                         download_cygnss_data, out_options, save_podaac_pass)
+                                         download_cygnss_data, out_options)
 
 
 def write_sp_from_kml_between_dates(cygnss_l1_dir: Optional[str], st_date: dt.date, end_date: dt.date, in_kml: str, out_folder_path: str,
                                     out_file_tag: str, thresh_ddm_snr: float = -9999.0, plt_thresh_noise: float = 1.0,
-                                    download_cygnss_data: bool = True, out_options: Optional[dict] = None,
-                                    save_podaac_pass: bool = True) -> tuple[str, str, str]:
+                                    download_cygnss_data: bool = True, out_options: Optional[dict] = None) -> tuple[str, str, str]:
     """
     This  search for all CYGNSS DDMs within the polygon in the in_kml within the daylist time period. It exports the plots of the DDMs with SNR above
     thesh_ddm_snr
     Note: The structure of the folders/files of  CYGNSS date need to be the same as the POO.DAC
 
     :param cygnss_l1_dir: the path of the main folder of CYGNSS L1 data (after the versions) (if None it uses os.environ.get("CYGNSS_L1_PATH"))
     :param st_date: start date
@@ -329,15 +321,14 @@
     :param in_kml: name of the kml file that have the poly
     :param out_folder_path: output folder path
     :param out_file_tag: tag for all the output files, ex: "out_root"_above_thresh.kml
     :param thresh_ddm_snr: DDM SNR threshold, above this value the DDM map image will be saved
     :param plt_thresh_noise: noise threshold, each pixel in the DDM below this value will be replaced by this value
     :param download_cygnss_data: download CYGNSS L1 data if they're not available ?
     :param out_options: currently we only implemented save_csv and save_ddm_img
-    :param save_podaac_pass: save PO DAAC username/password? ignored if download_cygnss_data = False
     :return: high SNR, low SNR, reference kml files paths
 
     """
     # Read polygon from input file and make longitude positive
     poly = get_poly(in_kml)
     # Find specular points inside polygon and write them to output
     ref_pos = [0.0, 0.0]
@@ -347,15 +338,15 @@
     num_days = (end_date - st_date).days + 1
     date_list = np.zeros(num_days, dtype=dt.date)
     for iday in range(num_days):
         date_list[iday] = st_date + dt.timedelta(days=iday)
     out_root = os.path.join(out_folder_path, out_file_tag)
 
     return _write_sp_from_poly_or_circle(cygnss_l1_dir, date_list, ref_pos, radius, thresh_ddm_snr, plt_thresh_noise, out_root, poly, tf_poly,
-                                         download_cygnss_data, out_options, save_podaac_pass)
+                                         download_cygnss_data, out_options)
 
 
 def get_poly(in_kml):
     """
     get the polygon from the kml file and return a geometry class
 
     :param in_kml: kml file name
@@ -380,31 +371,29 @@
     poly.AddGeometry(ring)
     ds_in = None
     return poly
 
 
 def _write_sp_from_poly_or_circle(cygnss_l1_path: Optional[str], date_list: Union[list[dt.date], np.ndarray],
                                   ref_pos: Union[tuple[float, float], list[float]], radius: float, thresh_ddm_snr: float, plt_thresh_noise: float,
-                                  out_root: str, poly, tf_poly: bool, download_cygnss_data: bool = True, out_options: Optional[dict] = None,
-                                  save_podaac_pass: bool = True) -> tuple[str, str, str]:
+                                  out_root: str, poly, tf_poly: bool, download_cygnss_data: bool = True, out_options: Optional[dict] = None) -> tuple[str, str, str]:
     """
 
     :param cygnss_l1_path: the path of the main folder of CYGNSS L1 data (after the versions) (if None it uses os.environ.get("CYGNSS_L1_PATH"))
     :param date_list: list of dates
     :type date_list: list of dt.date or np.array of dt.date
     :param ref_pos: (lat,long)
     :param radius: radius of search in m
     :param thresh_ddm_snr: DDM SNR threshold, above this value the DDM image will be saved
     :param plt_thresh_noise: noise threshold, each pixel in the DDM below this value will be replaced by this value
     :param out_root: tag for all the output files, ex: "out_root"_above_thresh.kml
     :param poly: Geometry class with the poly to search within
     :type poly: Geometry
     :param download_cygnss_data: download CYGNSS L1 data if they're not available ?
     :param out_options: currently we only implemented save_csv and save_ddm_img
-    :param save_podaac_pass: save PO DAAC username/password? ignored if download_cygnss_data = False
     :return: high SNR, low SNR, reference kml files paths
     """
 
     if out_options is None:
         out_options = dict()
 
     save_csv = out_options["save_csv"] if ("save_csv" in out_options) else False
@@ -497,15 +486,15 @@
         pbar = None
         gdal.UseExceptions()
         pnt_list_high = list()
         pnt_list_low = list()
 
         with Pool() as pool:
             args = ((cygnss_l1_path, i_date, download_cygnss_data, thresh_ddm_snr, ddm_quality_filter, bbox, poly, tf_poly,
-                     ref_pos, radius, save_podaac_pass, tf_print_screen, save_ddm_img, img_save_type,
+                     ref_pos, radius, tf_print_screen, save_ddm_img, img_save_type,
                      plt_tag, plt_thresh_noise, title_img_inc_ddm_time, out_folder, plt_reflectivity) for i_date in date_list)
             if pbar_tf:
                 for day_pnt_list_high, day_pnt_list_low in tqdm(pool.istarmap(_find_sp_in_day, args), total=len(date_list),
                                                                 desc='Searching CYGNSS files', unit='day'):
                     if day_pnt_list_high:
                         pnt_list_high += day_pnt_list_high
                     if day_pnt_list_low:
@@ -519,15 +508,15 @@
         del args, day_pnt_list_high, day_pnt_list_low
     else:
         pbar = tqdm(total=len(date_list) * 8, desc='Searching CYGNSS files', unit='file') if pbar_tf else None
         pnt_list_high = list()
         pnt_list_low = list()
         for i_date in date_list:
             day_pnt_list_high, day_pnt_list_low = _find_sp_in_day(cygnss_l1_path, i_date, download_cygnss_data, thresh_ddm_snr, ddm_quality_filter,
-                                                                  bbox, poly, tf_poly, ref_pos, radius, save_podaac_pass, tf_print_screen,
+                                                                  bbox, poly, tf_poly, ref_pos, radius, tf_print_screen,
                                                                   save_ddm_img, img_save_type, plt_tag, plt_thresh_noise, title_img_inc_ddm_time,
                                                                   out_folder, plt_reflectivity, pbar)
             if day_pnt_list_high:
                 pnt_list_high += day_pnt_list_high
             if day_pnt_list_low:
                 pnt_list_low += day_pnt_list_low
     if pbar is not None:
@@ -605,28 +594,28 @@
 
         df_data = pd.DataFrame(out_dic)
 
     return df_data
 
 
 def _find_sp_in_day(cygnss_l1_path: str, i_date: datetime.date, download_cygnss_data: bool, thresh_ddm_snr: float, ddm_quality_filter: int,
-                    bbox: list, poly: ogr.Geometry, tf_poly: bool, ref_pos: Union[list, np.ndarray], radius: float, save_podaac_pass: bool,
+                    bbox: list, poly: ogr.Geometry, tf_poly: bool, ref_pos: Union[list, np.ndarray], radius: float,
                     tf_print_screen: bool, save_ddm_img: bool, img_save_type: Union[list, np.ndarray], plt_tag: str, plt_thresh_noise: float,
                     title_img_inc_ddm_time: str, out_folder: str, plt_reflectivity: bool = False, pbar: Optional[tqdm] = None) -> tuple[list, list]:
     geod = Geodesic.WGS84
     day_pnt_list_high = list()
     day_pnt_list_low = list()
     day = i_date.timetuple().tm_yday
     cyg_day_folder = os.path.join(cygnss_l1_path, f'{i_date.year:04d}', f'{day:03d}')
     for sc_num in np.arange(1, 9):
         if pbar is not None:
             pbar.update()
         filename = get_cyg_file(cyg_day_folder, sc_num)
         if filename is None and download_cygnss_data:
-            file_name = download_cyg_files(i_date.year, day, sc_num, cygnss_l1_path=cygnss_l1_path, save_podaac_pass=save_podaac_pass)
+            file_name = download_cyg_files(i_date.year, day, sc_num, cygnss_l1_path=cygnss_l1_path)
             filename = None if (not file_name) else file_name[0]
 
         if filename is None:
             continue
         if tf_print_screen:
             print(filename)
         fullfile = os.path.join(cyg_day_folder, filename)
```

### Comparing `cygnsslib-1.2.3/src/cygnsslib/data_downloader/cyg_ant_ptrn.py` & `cygnsslib-1.3.0/src/cygnsslib/data_downloader/cyg_ant_ptrn.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.2.3/src/cygnsslib/data_downloader/download_cygnss_sftp.py` & `cygnsslib-1.3.0/src/cygnsslib/data_downloader/download_cygnss_sftp.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.2.3/src/cygnsslib/data_downloader/download_srtm.py` & `cygnsslib-1.3.0/src/cygnsslib/data_downloader/download_srtm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,27 @@
           See <https://bitbucket.org/usc_mixil/cygnss-library>
 
           This Tool download SRTM .hgt data
 
  AUTHOR   Amer Melebari
           Microwave Systems, Sensors and Imaging Lab (MiXiL)
           University of Southern California
- EMAIL    jamesdca@usc.edu
+ EMAIL    amelebar@usc.edu
  CREATED  2020-08-16
- Updated  2020-06-22
+ Updated  2023-05-02
 
 
 part of the download_file() is from the following codes:
 https://git.earthdata.nasa.gov/projects/LPDUR/repos/daac_data_download_python/
 https://github.com/DHI-GRAS/earthdata-download/tree/master/earthdata_download
 
   Copyright 2020 University of Southern California
 """
-from cygnsslib.data_downloader.pass_core import MixilKeys
-from getpass import getpass
+import logging
+import netrc
 from time import sleep
 from tqdm.auto import tqdm
 import numpy as np
 import os
 import requests
 import shutil
 import zipfile
@@ -61,15 +61,15 @@
 
 
 def _cyg_data_auth_err_handling():
     print('Error in the Earthdata Credentials, try to enter them again.')
     print('Note: you need to re-start the code after this download as the new user/pass need to be re-loaded')
     save_pass_str = input('Do you want to save the new user/pass? (if yes, the old user/pass will be deleted) [Yes, No]')
     save_pass = True if (save_pass_str.lower() in ['y', 'yes']) else False
-    podaac_usr, podaac_pass = get_earthdata_cred(pass_folder=None, save_pass=save_pass)
+    podaac_usr, podaac_pass = get_earthdata_cred()
     return podaac_usr, podaac_pass
 
 
 def _download_file_earthdata(file_url, output_folder, auth):
     """
     download the file with url into folder output_folder
 
@@ -86,14 +86,17 @@
     out_file = os.path.join(output_folder, file_name)
 
     out_file_temp = f'{out_file:s}.incomplete'
     for i_try in np.arange(MAX_CONNECTIONS_TRIES):
         try:
             with EarthdataSession(username=auth[0], password=auth[1]) as session:
                 with session.get(file_url, stream=True) as response:
+                    if response.status_code == 404:
+                        print(f'SRTM download Error: {file_url} is not Found')
+                        return None
                     response.raise_for_status()
                     response.raw.decode_content = True
                     with tqdm.wrapattr(open(out_file_temp, "wb"), "write", miniters=1, total=int(response.headers.get('content-length', 0)),
                                        desc=out_file_temp) as target_file:
                         for chunk in response.iter_content(chunk_size=CHUNK_SIZE):
                             target_file.write(chunk)
 
@@ -203,35 +206,30 @@
     :type zipped_filename: str
     :return: unzipped SRTM file name
     :rtype: str
     """
     return '{:s}.hgt'.format(zipped_filename.split('.')[0])
 
 
-def get_earthdata_cred(pass_folder=None, save_pass=True, reset_pass=False):
+def get_earthdata_cred():
     """
     import EarthData username and pass from the system, if not found it ask you to enter them
 
     :return:
     """
-    if reset_pass:
-        mixil_keys = MixilKeys(pass_folder=pass_folder)
-        mixil_keys.remove('lpdaac_usr')
-        mixil_keys.remove('lpdaac_pass')
-        del mixil_keys
-
-    if save_pass:
-        mixil_keys = MixilKeys(pass_folder=pass_folder)
-        mixil_keys.require('lpdaac_usr', msg='Get NASA Earthdata Credentials from: https://urs.earthdata.nasa.gov/home \nNASA Earthdata Username: ')
-        mixil_keys.require('lpdaac_pass', msg='NASA Earthdata Password: ')
-        earthdata_usr = mixil_keys.retrieve('lpdaac_usr')
-        earthdata_pass = mixil_keys.retrieve('lpdaac_pass')
-    else:
-        earthdata_usr = getpass('NASA Earthdata Username: ')
-        earthdata_pass = getpass('NASA Earthdata Password: ')
+    edl = "urs.earthdata.nasa.gov"
+    earthdata_usr = ''
+    earthdata_pass = ''
+    try:
+        earthdata_usr, _, earthdata_pass = netrc.netrc().authenticators(edl)
+    except (FileNotFoundError, TypeError):
+        # FileNotFound = There's no .netrc file
+        # TypeError = The endpoint isn't in the netrc file,
+        #  causing the above to try unpacking None
+        logging.warning("There's no .netrc file or the The endpoint isn't in the netrc file")
 
     return earthdata_usr, earthdata_pass
 
 
 def download_srtm_ght_files(list_lat, list_lon, out_folder=None, earthdata_usr_pass=None, save_pass=True, unzipfile=False, remove_zippedfile=True,
                             silent_run=False):
     """
@@ -269,15 +267,15 @@
     except TypeError:
         list_lon = [int(list_lon)]
 
     if out_folder is None:
         out_folder = os.path.join(os.environ['SRTM_PATH'], 'hgt')
         os.makedirs(out_folder, exist_ok=True)
     if earthdata_usr_pass is None:
-        earthdata_usr_pass = get_earthdata_cred(save_pass=save_pass)
+        earthdata_usr_pass = get_earthdata_cred()
 
     d_file_paths = list()
     for lat in list_lat:
         for lon in list_lon:
             d_file_paths.append(download_srtm_ght_single_file(lat, lon, out_folder=out_folder, earthdata_usr_pass=earthdata_usr_pass,
                                                               save_pass=save_pass, unzipfile=unzipfile, remove_zipedfile=remove_zippedfile,
                                                               silent_run=silent_run))
@@ -326,15 +324,15 @@
         return unzipped_file_path
     if os.path.exists(file_path):
         if not silent_run:
             print(f'{file_path:s} file exist')
         return file_path
 
     if earthdata_usr_pass is None:
-        earthdata_usr_pass = get_earthdata_cred(save_pass=save_pass)
+        earthdata_usr_pass = get_earthdata_cred()
     file_url = f'{SRTM_USGS_URL:s}{file_name:s}'
     saved_zip_file = _download_file_earthdata(file_url, out_folder, auth=earthdata_usr_pass)
     if not unzipfile:
         return saved_zip_file
 
     extract_srtm_zipfile(saved_zip_file, out_folder)
     unzipped_file = os.path.join(out_folder, get_srtm_unzipped_file_name(file_name))
```

### Comparing `cygnsslib-1.2.3/src/cygnsslib/istarmap.py` & `cygnsslib-1.3.0/src/cygnsslib/istarmap.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.2.3/src/cygnsslib/plotting.py` & `cygnsslib-1.3.0/src/cygnsslib/plotting.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.2.3/src/cygnsslib/util.py` & `cygnsslib-1.3.0/src/cygnsslib/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
     if xls_out is None:
         inxls_list = xls_in.split('.')
         xls_out = f'{inxls_list[0]:s}_land_prod.xlsx'  # car read xlsx and xls but write only to xls
 
     if not os.path.exists(xls_in):
         raise FileExistsError(f"Input Excel file doesn't exist, {xls_in:s}")
-    df = pd.read_excel(xls_in)
+    df: pd.DataFrame = pd.read_excel(xls_in)
 
     land_samp_list = []
     for i_ddm in df.itertuples():
         try:
             ddm_id = CygDdmId(None, i_ddm.year, i_ddm.day, i_ddm.flight_model, i_ddm.channel, i_ddm.sample_zero_based)
         except AttributeError:
             ddm_id = CygDdmId(None, i_ddm[start_col + 1], i_ddm[start_col + 2], i_ddm[start_col + 3], i_ddm[start_col + 4], i_ddm[start_col + 5])
@@ -159,11 +159,10 @@
 if __name__ == '__main__':
     # xls_in = 'SLV_Z4_thawed_2019.xlsx'
     # find_land_prod_sample_id_from_excel(xls_in, xls_out=None, start_col=1, out_sheet_suffix='', timestamp_col=0)
     # xls_in = 'SLV_Z1_thawed_2019.xlsx'
     # find_land_prod_sample_id_from_excel(xls_in, xls_out=None, st_row=1, start_col=1, out_sheet_suffix='', timestamp_col=0)
     kml_file_path = 'z1_test_v3_samples.xlsx'
     ant_comp_xls = 'z1_test_v3_samples_antt.xlsx'
-    get_ant_pattern_for_diff_versions(kml_file_path, kml_cyg_ver='v3.0', cyg_ver_list=['v2.1'], out_xls=ant_comp_xls)
-    kml_file_path = '/media/amer/myfiles/cygnss/kml_files/Z1/z1_yr19_aft_aug_above_thresh.kml'
+    get_ant_pattern_for_diff_versions(kml_file_path, kml_cyg_ver='v3.1', cyg_ver_list=['v2.1'], out_xls=ant_comp_xls)
     ant_comp_xls = 'v2v3_ant_com.xlsx'
-    get_ant_pattern_for_diff_versions(kml_file_path, kml_cyg_ver='v3.0', cyg_ver_list=['v2.1'], out_xls=ant_comp_xls)
+    get_ant_pattern_for_diff_versions(kml_file_path, kml_cyg_ver='v3.1', cyg_ver_list=['v2.1'], out_xls=ant_comp_xls)
```

### Comparing `cygnsslib-1.2.3/src/cygnsslib.egg-info/PKG-INFO` & `cygnsslib-1.3.0/src/cygnsslib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cygnsslib
-Version: 1.2.3
+Version: 1.3.0
 Summary: Toolset for working with CYGNSS data and downloading CYGNSS data from PODAAC
 Home-page: https://bitbucket.org/usc_mixil/cygnsslib
 Author: Amer Melebari and James D. Campbell
 Author-email: amelebar@usc.edu
 License: UNKNOWN
 Description: # CYGNSS Library
         
@@ -30,40 +30,42 @@
         You can then remove the local copy if you wish. Alternatively, if you wish to be able to make changes to your local copy without having to reinstall the package for the changes to take effect (e.g., for development purposes), you can use the following instead:
         ```console
         pip uninstall cygnsslib
         ```
         ### Required packages
         Here the required Python packages:
         ```console
-        gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pbkdf2 pycrypto pyproj pysftp requests setuptools tqdm paramiko
+        gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pysftp requests tqdm
         ```
         Note: `gdal` can be installed using conda   
         ```console
         conda install -c conda-forge gdal  
         ```
         or using [this method](https://mothergeo-py.readthedocs.io/en/latest/development/how-to/gdal-ubuntu-pkg.html) in Ubuntu  
-        ## How to Use The Package
+        Also, you need the modified data-subscriber package from [https://github.com/MiXIL/data-subscriber](https://github.com/MiXIL/data-subscriber)  
+        
+        ## How to Use The Package  
         The cygnsslib has several modules:  
         1. Identify CYGNSS DDMs within a specific region  
         2. Group DDMs within a specific distance  
         3. Download CYGNSS antenna pattern  
         4. CygDdmId Class, which work as CYGNSS DDM ID  
         5. Download CYGNSS data from PO.DAAC  
-        6. Download SRTM data from NASA Earth Data
+        6. Download SRTM data from NASA Earth Data  
         7. Other functionality related to CYGNSS data  
           
-        For most of the library, you need to set the environment variable ``CYGNSS_L1_PATH`` to the path of the CYGNSS L1 data. i.e.
-        ```console 
-        CYGNSS_L1_PATH=/cygnss_data/L1/v3.0
-        ```
-        Note the folder needs to be named as the version (e.g. `v3.0`)name in PODAAC, and the parent folder need to be `L1`
-        You can set the environment variable for the session in python as follows:
-        ```python
+        For most of the library, you need to set the environment variable ``CYGNSS_L1_PATH`` to the path of the CYGNSS L1 data. i.e.  
+        ```console  
+        CYGNSS_L1_PATH=/cygnss_data/L1/v3.1
+        ```   
+        Note the folder needs to be named as the version (e.g. `v3.1`)name in PODAAC, and the parent folder need to be `L1`
+        You can set the environment variable for the session in python as follows:  
+        ```python  
         import os
-        os.environ['CYGNSS_L1_PATH'] = '/cygnss_data/L1/v3.0'
+        os.environ['CYGNSS_L1_PATH'] = '/cygnss_data/L1/v3.1'
         ```
         
         For SRTM you can specify the main path by specifying the environment variable ``SRTM_PATH``. The files will be saved in `SRTM_PATH\hgt`
         ### Identify CYGNSS DDMs within a specific region
         
         There are several ways to find the DDM within a region.  
         1. find all the DDMs that their SP location within a specific distance from a specific location.  
@@ -72,15 +74,16 @@
         Below an example of the usage:
         
         ```python
         import cygnsslib
         import numpy as np
         import datetime as dt
         
-        cygnss_l1_path = None  # this will make the strip get the path from os.environ["CYGNSS_L1_PATH"]
+        # this will make the strip get the path from os.environ["CYGNSS_L1_PATH"]
+        cygnss_l1_path = None  
         year = 2019
         days_list = np.arange(1, 100)
         ref_pos = (37.1906, -105.9921)  # (lat,long)
         radius = 10e3  # [m]
         thesh_ddm_snr = 3.0  # split DDMs into above thesh_ddm_snr and below thesh_ddm_snr. Above this value the DDM image will be saved
         thesh_noise = 1  # noise threshold, each pixel in the DDM below this value will be replaced by this value
         kml_out_tag = f'my_data'  # tag for all the output files, ex: my_data_above_thresh.kml
@@ -89,17 +92,18 @@
         options = {'save_cvs': False,
                    'save_ddm_img': True,
                    'plt_tag': '',
                    'title_img_inc_ddm_time': False,
                    'img_save_type': ['png'],
                    'sheet_type': 'xls'}
         
-        cygnsslib.write_sp_within_radius(cygnss_l1_path, year=2019, daylist=days_list, ref_pos=ref_pos, radius=radius, out_folder_path=f'', 
-                                         out_file_tag=kml_out_tag, thresh_ddm_snr=thesh_ddm_snr, plt_thresh_noise=thesh_noise, download_cygnss_data=True, 
-                                         out_options=options, save_podaac_pass=save_podaac_pass)
+        out_folder_path = 'my_ddms'
+        cygnsslib.write_sp_within_radius(cygnss_l1_path, year, days_list, ref_pos, radius, 
+                                         out_folder_path, kml_out_tag, thesh_ddm_snr, thesh_noise, 
+                                         download_cygnss_data=True, out_options=options)
         
         start_date = dt.date(year=2019, month=1, day=1)
         end_date = dt.date(year=2019, month=6, day=10)  # the end date included in the search
         cygnsslib.write_sp_within_radius_between_dates(cygnss_l1_path, start_date, end_date, ref_pos=ref_pos,
                                                        radius=radius, out_folder_path=f'', out_file_tag=kml_out_tag, thresh_ddm_snr=thesh_ddm_snr,
                                                        plt_thresh_noise=thesh_noise, download_cygnss_data=True,
                                                        out_options=options, save_podaac_pass=save_podaac_pass)
@@ -196,39 +200,39 @@
         ### Download CYGNSS data from PO.DAAC
         
         You can download both the standard DDMs and the rawif data. You can choose to download data between two dates or a list of days in the year.  
         If a file exists, the code will not re-download it.  
         Note if you select `check_md5_exist_file=True`, then the code will do an md5 check for existing files. This will ensure existing files are good. However, this will make it very slow.
         
         Below an example of downloading DDMs and the rawif files. The files will be organized as they're in PODAAC.
+        
         ```python
         from cygnsslib import cygnss_download
         import datetime as dt
         import numpy as np
         
         # Download data in the same year and range of days
         days_list = np.arange(5, 10)
         data_year = 2020
         # list_sc_num = [3]
         list_sc_num = None  # Will download all the 8 spacecrafts 
-        cyg_data_ver = f'v3.0'
-        cygnss_download.download_cyg_files(data_year, days_list, list_sc_num=list_sc_num, cyg_data_ver=cyg_data_ver, 
-                                           check_md5_exist_file=False, cyg_data_lvl=f'L1', save_podaac_pass=True)
+        cyg_data_ver = f'v3.1'
+        cygnss_download.download_cyg_files(data_year, days_list, list_sc_num, cyg_data_ver, cyg_data_lvl=f'L1', checksum_exist_file=False)
         # Downloading data between two dates (including end date)
         st_date = dt.date(year=2019, month=1, day=12)
         end_date = dt.date(year=2020, month=1, day=3)
         
-        cygnss_download.download_cyg_files_between_date(st_date, end_date, list_sc_num=list_sc_num, cyg_data_ver=cyg_data_ver, 
-                                                        check_md5_exist_file=False, cyg_data_lvl=f'L1', save_podaac_pass=True)
+        cygnss_download.download_cyg_files_between_date(st_date, end_date, list_sc_num, cyg_data_ver=cyg_data_ver, cyg_data_lvl=f'L1',
+                                                        checksum_exist_file=False)
         
         # Downloading rawif data 
         download_l1_data = True  # This will download the corresponding L1 data
-        cygnss_download.download_cyg_rawif_files(data_year,days_list, list_sc_num, save_podaac_pass=True, 
+        cygnss_download.download_cyg_rawif_files(data_year, days_list, list_sc_num, save_podaac_pass=True,
                                                  download_l1_data=download_l1_data)
-        cygnss_download.download_rawif_cyg_files_between_date(st_date,end_date, list_sc_num, save_podaac_pass=True, 
+        cygnss_download.download_rawif_cyg_files_between_date(st_date, end_date, list_sc_num, save_podaac_pass=True,
                                                               download_l1_data=download_l1_data)
         
         ```
         #### PODAAC user/pass related notes
         You can get the PO.DAAC Drive API Credentials from https://podaac-tools.jpl.nasa.gov/drive/  
         If you entered the wrong PODAAC user/pass, you'll be asked to re-enter them again. However, you need to re-start the code after that so the saved user/pass are loaded again.  
         
@@ -252,19 +256,20 @@
         files_lat = [21, 22, 20]
         files_lon = [29, 30]
         srtm_download.download_srtm_ght_files(files_lat, files_lon, save_pass=True, unzipfile=False, remove_zippedfile=True)  
         
         
         ```
         #### EarthData username and pass related notes  
-        You can reset your EarthData user/pass and enter new user/pass using the following code. Note when you run the code, you'll be asked to enter the new user/pass  
+        You can reset your EarthData user/pass and enter new user/pass using the following code. Note when you run the code, you'll be asked to enter the new user/pass
+        
         ```python
         from cygnsslib import srtm_download
         
-        srtm_download.get_earthdata_cred(save_pass=True, reset_pass=True) 
+        srtm_download.get_earthdata_cred() 
         ```
         ### Other functionality related to CYGNSS data   
         
         Create a circle or a square on the ground and export it to kml file  
         ```python
         import cygnsslib
         ref_pos = [37.1906, -105.9921] #  [lat,long]
```

### Comparing `cygnsslib-1.2.3/src/cygnsslib.egg-info/SOURCES.txt` & `cygnsslib-1.3.0/src/cygnsslib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 src/cygnsslib/cygnss_download/__init__.py
 src/cygnsslib/data_downloader/__init__.py
 src/cygnsslib/data_downloader/cyg_ant_ptrn.py
 src/cygnsslib/data_downloader/download_cyg_rawif.py
 src/cygnsslib/data_downloader/download_cygnss.py
 src/cygnsslib/data_downloader/download_cygnss_sftp.py
 src/cygnsslib/data_downloader/download_srtm.py
-src/cygnsslib/data_downloader/pass_core.py
 src/cygnsslib/srtm_download/__init__.py
 src/tests/list_loc2kml.py
 src/tests/test_download_cyg_data.py
 src/tests/test_download_srtm.py
 src/tests/test_find_land_prod_from_cvs.py
 src/tests/test_functions.py
 src/tests/test_search_within_circle.py
```

### Comparing `cygnsslib-1.2.3/src/tests/list_loc2kml.py` & `cygnsslib-1.3.0/src/tests/list_loc2kml.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.2.3/src/tests/test_download_cyg_data.py` & `cygnsslib-1.3.0/src/tests/test_download_cyg_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     # sc_num = None
     check_md5_exist_file = False
     cyg_data_ver = 'v3.1'
     cygnss_l1_path = os.environ["CYGNSS_L1_PATH"]
     data_day = 24
     sc_num = 3
     cygnss_download.download_cyg_files(data_year, data_day, list_sc_num=sc_num, cyg_data_ver=cyg_data_ver, cyg_data_lvl='L1',
-                                       cygnss_l1_path=cygnss_l1_path, check_md5_exist_file=check_md5_exist_file)
+                                       cygnss_l1_path=cygnss_l1_path, checksum_exist_file=check_md5_exist_file)
     st_date = dt.date(year=2019, month=1, day=12)
     end_date = dt.date(year=2020, month=1, day=3)
 
     cygnss_download.download_cyg_files_between_date(st_date, end_date, list_sc_num=sc_num, cyg_data_ver=cyg_data_ver, cyg_data_lvl='L1',
-                                                    cygnss_l1_path=cygnss_l1_path, check_md5_exist_file=check_md5_exist_file)
+                                                    cygnss_l1_path=cygnss_l1_path, checksum_exist_file=check_md5_exist_file)
 
     cygnsslib.data_downloader.download_cyg_rawif.download_cyg_rawif_files(data_year=2020, list_data_day=227)
 
     st_date = dt.date(year=2020, month=8, day=4)
     end_date = dt.date(year=2020, month=8, day=4)
     cygnsslib.data_downloader.download_cyg_rawif.download_rawif_cyg_files_between_date(st_date, end_date, download_l1_data=True)
```

### Comparing `cygnsslib-1.2.3/src/tests/test_functions.py` & `cygnsslib-1.3.0/src/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.2.3/src/tests/test_search_within_circle.py` & `cygnsslib-1.3.0/src/tests/test_search_within_circle.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.2.3/src/tests/test_write_sp_within_radius.py` & `cygnsslib-1.3.0/src/tests/test_write_sp_within_radius.py`

 * *Files identical despite different names*

