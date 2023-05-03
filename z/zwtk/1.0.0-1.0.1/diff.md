# Comparing `tmp/zwtk-1.0.0-py3-none-any.whl.zip` & `tmp/zwtk-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 16179 bytes, number of entries: 19
+Zip file size: 16395 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat        0 b- defN 20-Jul-16 08:16 zwtk/__init__.py
--rw-rw-rw-  2.0 fat      288 b- defN 23-May-02 11:47 zwtk/__version__.py
+-rw-rw-rw-  2.0 fat      286 b- defN 23-May-03 04:30 zwtk/__version__.py
 -rw-rw-rw-  2.0 fat     1159 b- defN 23-May-02 02:51 zwtk/comm.py
 -rw-rw-rw-  2.0 fat     1453 b- defN 23-Feb-08 05:36 zwtk/config.py
 -rw-rw-rw-  2.0 fat     9392 b- defN 23-Feb-15 13:39 zwtk/dlso.py
--rw-rw-rw-  2.0 fat     7118 b- defN 23-May-02 03:06 zwtk/fileutils.py
+-rw-rw-rw-  2.0 fat     7478 b- defN 23-May-03 04:18 zwtk/fileutils.py
 -rw-rw-rw-  2.0 fat     1728 b- defN 23-May-02 11:44 zwtk/geoutils.py
--rw-rw-rw-  2.0 fat      800 b- defN 23-May-02 07:47 zwtk/mprocessing.py
+-rw-rw-rw-  2.0 fat      897 b- defN 23-May-03 04:20 zwtk/mprocessing.py
 -rw-rw-rw-  2.0 fat     2269 b- defN 21-Jul-27 09:50 zwtk/mthreading.py
--rw-rw-rw-  2.0 fat      656 b- defN 23-May-02 06:58 zwtk/osutils.py
+-rw-rw-rw-  2.0 fat      815 b- defN 23-May-03 04:29 zwtk/osutils.py
 -rw-rw-rw-  2.0 fat      261 b- defN 22-Mar-22 06:05 zwtk/rand.py
 -rw-rw-rw-  2.0 fat     1217 b- defN 23-May-02 11:44 zwtk/reutils.py
 -rw-rw-rw-  2.0 fat     4850 b- defN 22-May-23 04:27 zwtk/textutils.py
 -rw-rw-rw-  2.0 fat     6638 b- defN 23-Feb-08 05:36 zwtk/urlutils.py
--rw-rw-rw-  2.0 fat     1068 b- defN 23-May-02 11:47 zwtk-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      527 b- defN 23-May-02 11:47 zwtk-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 11:47 zwtk-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-02 11:47 zwtk-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1378 b- defN 23-May-02 11:47 zwtk-1.0.0.dist-info/RECORD
-19 files, 40899 bytes uncompressed, 13989 bytes compressed:  65.8%
+-rw-rw-rw-  2.0 fat     1068 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      527 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1378 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/RECORD
+19 files, 41513 bytes uncompressed, 14205 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: zwtk/textutils.py
 Comment: 
 
 Filename: zwtk/urlutils.py
 Comment: 
 
-Filename: zwtk-1.0.0.dist-info/LICENSE
+Filename: zwtk-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: zwtk-1.0.0.dist-info/METADATA
+Filename: zwtk-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: zwtk-1.0.0.dist-info/WHEEL
+Filename: zwtk-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: zwtk-1.0.0.dist-info/top_level.txt
+Filename: zwtk-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: zwtk-1.0.0.dist-info/RECORD
+Filename: zwtk-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zwtk/__version__.py

```diff
@@ -1,10 +1,8 @@
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 __title__ = 'zwtk'
 __description__ = 'Personal Python Utilities'
 __url__ = 'https://github.com/njzhaowei/zwtk'
 __author__ = 'Zhao Wei'
 __author_email__ = 'yewberry@163.com'
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2023 Zhao Wei. All rights reserved.'
-
-
```

## zwtk/fileutils.py

```diff
@@ -5,127 +5,132 @@
 import csv
 import hashlib
 import subprocess
 from pathlib import Path
 import shutil
 
 def rmfile(pth):
+    ''' Remove file(and only file) if exists'''
     if os.path.isfile(str(pth)):
         os.remove(str(pth))
 
 def rmdir(pth):
+    ''' Remove directory empty or not, ignore any error.'''
     shutil.rmtree(str(pth), ignore_errors=True)
 
 def move(src, dst):
+    ''' Move file or directory'''
     shutil.move(src, dst)
 
 def writefile(path, txt, enc='utf-8'):
-    """Write string to file and create parent dirs automatically.
-    """
+    '''Write string to file and create parent dirs automatically.
+    '''
     if not isinstance(txt, str):
         txt = str(txt)
     if not Path(path).parent.exists():
         Path(path).parent.mkdir(parents=True, exist_ok=True)
     with codecs.open(str(path), 'w', enc) as fp:
         fp.write(txt)
         fp.flush()
 
 def readfile(path, enc='utf-8', default=None):
-    """Read string from file with default value.
-    """
+    '''Read string from file with default value.
+    '''
     rtn = None
     if not Path(path).exists() and default is not None:
         return default
     with codecs.open(str(path), 'r', enc) as fp:
         rtn = fp.read()
     if enc=='utf-8' and rtn.startswith('\ufeff'):# BOM
         rtn = rtn[1:]
     return rtn
 
 def writebin(path, dat):
-    """Write binary data to file and create parent dirs automatically.
-    """
+    '''Write binary data to file and create parent dirs automatically.
+    '''
     if not Path(path).parent.exists():
         Path(path).parent.mkdir(parents=True, exist_ok=True)
     with open(str(path), 'wb') as fp:
         fp.write(dat)
         fp.flush()
 
 def readbin(path, default=None):
-    """Read binary data from file with default value.
-    """
+    '''Read binary data from file with default value.
+    '''
     rtn = None
     if not Path(path).exists() and default is not None:
         return default
     with open(str(path), 'rb') as fp:
         rtn = fp.read()
     return rtn
 
 def writejson(path, o, enc='utf-8'):
-    """Write json data to file and create parent dirs automatically.
-    """
+    '''Write json data to file and create parent dirs automatically.
+    '''
     if not Path(path).parent.exists():
         Path(path).parent.mkdir(parents=True, exist_ok=True)
     with codecs.open(str(path), 'w', enc) as fp:
         json.dump(o, fp, ensure_ascii=False)
 
 def readjson(path, enc='utf-8', default=None):
-    """Read json data from file with default value.
-    """
+    '''Read json data from file with default value.
+    '''
     rtn = None
     if not Path(path).exists() and default is not None:
         return default
     with codecs.open(str(path), 'r',enc) as fp:
         rtn = json.load(fp)
     return rtn
 
 def writecsv(path, array2d, delimiter=',', enc='utf-8'):
-    """Write csv data to file and create parent dirs automatically.
-    """
+    '''Write csv data to file and create parent dirs automatically.
+    '''
     if not Path(path).parent.exists():
         Path(path).parent.mkdir(parents=True, exist_ok=True)
     with codecs.open(str(path), 'w', enc) as fp:
         writer = csv.writer(fp, delimiter=delimiter)
         writer.writerows(array2d)
 
 def readcsv(path, enc='utf-8', default=None):
-    """Read csv data from file with default value.
-    """
+    '''Read csv data from file with default value.
+    '''
     rtn = None
     if not Path(path).exists() and default is not None:
         return default
     with codecs.open(str(path), 'r', enc) as fp:
         reader = csv.reader(fp)
         rtn = list(reader)
     return rtn
 
 def file_encode_convert(src, dst, src_encode='utf-8', dst_encode='gbk'):
+    '''Change file encode'''
     src_encode = src_encode.lower()
     dst_encode = dst_encode.lower()
     with codecs.open(src, 'r', src_encode) as fp:
         new_content = fp.read()
     with codecs.open(src, 'w', dst_encode) as fp:
         fp.write(new_content)
         fp.flush()
 
 def md5(fp):
+    '''md5 file'''
     hash_md5 = hashlib.md5()
     with open(fp, 'rb') as f:
         for chunk in iter(lambda: f.read(4096), b''):
             hash_md5.update(chunk)
     return hash_md5.hexdigest()
 
 def zip(srcpth, destpth=None, pwd=None, pth7z=None):
-    """Use 7z.exe or zip command to zip file or dir
+    '''Use 7z.exe(Win, 7z.exe should in path) or zip command(Linux) to zip file or dir
     :param srcpth: ./dir/file => file in zip, dir/file => dir/file in zip
     :param destpth: zip in srcpth if None
     :param pwd: no password if not set
     :param pth7z: 7z.exe in ./bin in win by default, zip command in linux
 
-    """
+    '''
     iswin = True if sys.platform == 'win32' else False
     spath = Path(srcpth)
     sname = '%s.zip'%spath.stem if spath.is_file() else '%s.zip'%spath.name
     destpth = destpth or str(spath.parent / sname)
     cmd = pth7z or ( './bin/7z.exe' if iswin else 'zip' )
     cmds = [str(cmd)]
     if iswin:
@@ -138,14 +143,16 @@
             cmds.append('-P %s'%pwd)
     cmds.extend([str(destpth), str(srcpth)])
     subprocess.run(cmds)
     destfile = Path(destpth)
     return destfile.exists()
 
 def unzip(srcpth, destpth=None, pwd=None, pth7z=None):
+    '''Unzip file use 7z.exe(Win, 7z.exe should in path) or unzip command(Linux)
+    '''
     iswin = True if sys.platform == 'win32' else False
     cmd = pth7z or ( './bin/7z.exe' if iswin else 'unzip' )    
     cmds = [str(cmd)]
     destfile = Path(destpth)
     destfile.parent.mkdir(parents=True, exist_ok=True)
     if iswin:
         cmds.extend(['x', str(srcpth), '-y', '-aoa', '-o%s'%destpth])
@@ -155,14 +162,15 @@
         cmds.extend([srcpth, '-d', destpth])
         if pwd:
             cmds.append('-P %s'%pwd)
     subprocess.run(cmds)
     return destfile.exists()
 
 def dirsize(pth):
+    '''Calc directory size in byte'''
     size = 0
     for root, dirs, files in os.walk(pth):
         size += sum([os.path.getsize(os.path.join(root, file)) for file in files])
     return size
 
 # def tar(pth, outpath=None, flag='w:gz'):
 #     p = Path(pth)
```

## zwtk/mprocessing.py

```diff
@@ -1,21 +1,23 @@
 import subprocess
 from concurrent.futures import ProcessPoolExecutor, as_completed
 
 def multiprocess_cmd(cmds, max_workers=3):
+    '''Run multi processes for commands'''
     rtn = []
     with ProcessPoolExecutor(max_workers=max_workers) as executor:
         cmds = list(cmds)
         futures = [executor.submit(subprocess.run, cmd, shell=True) for cmd in cmds]
         for future in as_completed(futures):
             r = future.result()
             rtn.append(r)
     return rtn
 
 def multiprocess_run(cbfunc, args, max_workers=3):
+    '''Run multi processes for callback function'''
     rtn = []
     with ProcessPoolExecutor(max_workers=max_workers) as executor:
         args = list(args)
         futures = [executor.submit(cbfunc, *arg) for arg in args]
         for future in as_completed(futures):
             r = future.result()
             rtn.append(r)
```

## zwtk/osutils.py

```diff
@@ -18,11 +18,16 @@
     pid = os.getpid()
     pth = Path(dir) / ('%s.pid'%pid)
     Path(pth).parent.mkdir(parents=True, exist_ok=True)
     writefile(pth, pid)
     return pth
 
 def run_shell(cmd, *args):
+    '''Run command and get result text. Try decoded by utf-8 and gbk.'''
     cmds = [cmd]
     cmds.extend(list(args))
-    r = subprocess.run(cmds, stdout=subprocess.PIPE).stdout.decode('utf-8')
+    out = subprocess.run(cmds, stdout=subprocess.PIPE, shell=True).stdout
+    try:
+        r = out.decode('utf-8')
+    except:
+        r = out.decode('gbk')
     return r
```

## Comparing `zwtk-1.0.0.dist-info/LICENSE` & `zwtk-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zwtk-1.0.0.dist-info/METADATA` & `zwtk-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zwtk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Personal Python Utilities
 Home-page: https://github.com/njzhaowei/zwtk
 Author: Zhao Wei
 Author-email: yewberry@163.com
 License: Apache 2.0
 Platform: all
 Classifier: Programming Language :: Python :: 3
```

## Comparing `zwtk-1.0.0.dist-info/RECORD` & `zwtk-1.0.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 zwtk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-zwtk/__version__.py,sha256=uWnYv2PuiUk2_QgYkceBnWTcF4qW8c5w6NiggjUOw-M,288
+zwtk/__version__.py,sha256=xosNaqiDX_35hEBr8wJ1-ARhVHh6CheDxnaWC6WJeQo,286
 zwtk/comm.py,sha256=OycFwe4kcxvSESh0EHsjuG6raipj_rfXqOn8-YpmGh8,1159
 zwtk/config.py,sha256=lFeXOV4SNoiofGN48ssAATA5yal_hWbE5xUd-AZNdyI,1453
 zwtk/dlso.py,sha256=ZP70mx88H6hMJxBlLxhFjU4cuyTc_QFyj-vZlJcKFoI,9392
-zwtk/fileutils.py,sha256=5D9e2ncf2joAaaf9cDIfcHv4ydXQHNeGIHE23Mu-Vr4,7118
+zwtk/fileutils.py,sha256=pBPFJg_hc6noGACbTQoEpWnic0i-rpTrqdyea0q5rvk,7478
 zwtk/geoutils.py,sha256=8ve3fz_7zgjNgcLLKC4DTxob9mmJLNsr4-i-U2amaCs,1728
-zwtk/mprocessing.py,sha256=Cmy7BFAm-bBnaiaX6-NZgpBfk7UW0kr19Uf4sXVcc3I,800
+zwtk/mprocessing.py,sha256=-5IGrK87WKCgjp9-cqcu2cOL8_pOQRWPYdTf1gq1jec,897
 zwtk/mthreading.py,sha256=YDzai3v9Ne8NglFY4RvI-mDsMwgk1t-IxJx_YFwA9MA,2269
-zwtk/osutils.py,sha256=Us4rfuisk1SX5bpJDRw_TEXMh9-YHO-fKFtWVerbALs,656
+zwtk/osutils.py,sha256=R62uDBTw_kQhQgkxG8V2Bu-OvX65418HrleM7Bgx24s,815
 zwtk/rand.py,sha256=NF97IN2QAcd5azH1I0CbdEAvou4QeCK510-zjvrawGo,261
 zwtk/reutils.py,sha256=fjw6A_MGI2EY10TuiEat4wpG6DfpwQVRbFFu0GmgDME,1217
 zwtk/textutils.py,sha256=ua6uxxB-wsIqRZHrdHbz7F391utpUHvzfF0pkHITPIw,4850
 zwtk/urlutils.py,sha256=TgXKbJhrSFMJAOd9K7c91L4LC1obzbfHdhnoehi1st8,6638
-zwtk-1.0.0.dist-info/LICENSE,sha256=u-k3pdS046rxrlusCu-PdSHHdF5pgn1GgR1IU0CfoyI,1068
-zwtk-1.0.0.dist-info/METADATA,sha256=XKN6R_v5DwjVtresYtulISdP50S98kKZUHPbCTL_nhE,527
-zwtk-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-zwtk-1.0.0.dist-info/top_level.txt,sha256=sZshqvNUx_xBkWVO93H3Nu-ACwaM6HhRtvErJtzxUTQ,5
-zwtk-1.0.0.dist-info/RECORD,,
+zwtk-1.0.1.dist-info/LICENSE,sha256=u-k3pdS046rxrlusCu-PdSHHdF5pgn1GgR1IU0CfoyI,1068
+zwtk-1.0.1.dist-info/METADATA,sha256=lgP3itQW9Aq_DSgWtbKCUQ5TkHCFlQoY3PQBXx6OQYQ,527
+zwtk-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+zwtk-1.0.1.dist-info/top_level.txt,sha256=sZshqvNUx_xBkWVO93H3Nu-ACwaM6HhRtvErJtzxUTQ,5
+zwtk-1.0.1.dist-info/RECORD,,
```

