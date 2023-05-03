# Comparing `tmp/supylib-0.21.tar.gz` & `tmp/supylib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ak/projects/supylib/dist/tmppx96s8tp/supylib-0.21.tar", last modified: Wed Nov  2 18:26:47 2022, max compression
+gzip compressed data, was "/home/ak/projects/supylib/dist/tmph3vqsvnl/supylib-0.3.tar", last modified: Wed May  3 16:52:39 2023, max compression
```

## Comparing `supylib-0.21.tar` & `supylib-0.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2022-11-02 18:26:47.000000 supylib-0.21/
--rw-rw-r--   0 ak        (1000) ak        (1000)     1118 2022-03-09 09:38:11.000000 supylib-0.21/LICENSE
--rw-r--r--   0 ak        (1000) ak        (1000)     1180 2022-11-02 18:12:13.000000 supylib-0.21/README.md
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2022-11-02 18:26:47.000000 supylib-0.21/python/
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2022-11-02 18:26:47.000000 supylib-0.21/python/supylib.egg-info/
--rw-rw-r--   0 ak        (1000) ak        (1000)        5 2022-11-02 18:26:47.000000 supylib-0.21/python/supylib.egg-info/top_level.txt
--rw-rw-r--   0 ak        (1000) ak        (1000)        1 2022-11-02 18:26:47.000000 supylib-0.21/python/supylib.egg-info/dependency_links.txt
--rw-rw-r--   0 ak        (1000) ak        (1000)      649 2022-11-02 18:26:47.000000 supylib-0.21/python/supylib.egg-info/SOURCES.txt
--rw-rw-r--   0 ak        (1000) ak        (1000)     1775 2022-11-02 18:26:47.000000 supylib-0.21/python/supylib.egg-info/PKG-INFO
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2022-11-02 18:26:47.000000 supylib-0.21/python/supy/
--rw-r--r--   0 ak        (1000) ak        (1000)    12807 2019-02-28 09:55:09.000000 supylib-0.21/python/supy/forms.py
--rw-r--r--   0 ak        (1000) ak        (1000)     6868 2022-09-08 14:57:35.000000 supylib-0.21/python/supy/guimaker3.py
--rw-r--r--   0 ak        (1000) ak        (1000)    40317 2022-03-09 08:59:15.000000 supylib-0.21/python/supy/sqltableeditor.py
--rw-r--r--   0 ak        (1000) ak        (1000)     7965 2022-03-09 08:57:33.000000 supylib-0.21/python/supy/multibase.py
--rw-r--r--   0 ak        (1000) ak        (1000)     6871 2019-02-28 09:56:23.000000 supylib-0.21/python/supy/guimaker.py
--rw-r--r--   0 ak        (1000) ak        (1000)    17745 2022-03-09 08:58:19.000000 supylib-0.21/python/supy/sqldatabase_inputmask.py
--rw-r--r--   0 ak        (1000) ak        (1000)    20272 2022-03-09 08:54:20.000000 supylib-0.21/python/supy/database_inputmask3.py
--rw-r--r--   0 ak        (1000) ak        (1000)    20266 2022-03-09 08:55:21.000000 supylib-0.21/python/supy/database_inputmask.py
--rw-r--r--   0 ak        (1000) ak        (1000)    19500 2022-03-09 08:55:47.000000 supylib-0.21/python/supy/database.py
--rw-r--r--   0 ak        (1000) ak        (1000)    31946 2022-03-09 09:01:33.000000 supylib-0.21/python/supy/widgets.py
--rw-r--r--   0 ak        (1000) ak        (1000)     5419 2022-03-09 08:57:58.000000 supylib-0.21/python/supy/serialize.py
--rw-r--r--   0 ak        (1000) ak        (1000)   106175 2022-03-09 09:00:49.000000 supylib-0.21/python/supy/sqlforms.py
--rw-r--r--   0 ak        (1000) ak        (1000)    42485 2022-03-09 08:56:45.000000 supylib-0.21/python/supy/forms3.py
--rw-rw-r--   0 ak        (1000) ak        (1000)       22 2022-11-02 18:18:03.000000 supylib-0.21/python/supy/__init__.py
--rw-r--r--   0 ak        (1000) ak        (1000)    30059 2022-03-09 08:58:51.000000 supylib-0.21/python/supy/sqldatabase.py
--rw-r--r--   0 ak        (1000) ak        (1000)     5226 2022-03-09 09:01:13.000000 supylib-0.21/python/supy/utilities.py
--rw-r--r--   0 ak        (1000) ak        (1000)    76510 2022-09-12 07:20:03.000000 supylib-0.21/python/supy/computervision.py
--rw-rw-r--   0 ak        (1000) ak        (1000)      689 2022-11-02 18:26:47.000000 supylib-0.21/setup.cfg
--rw-rw-r--   0 ak        (1000) ak        (1000)      104 2022-03-09 09:36:04.000000 supylib-0.21/pyproject.toml
--rw-rw-r--   0 ak        (1000) ak        (1000)     1775 2022-11-02 18:26:47.000000 supylib-0.21/PKG-INFO
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 16:52:39.000000 supylib-0.3/
+-rw-rw-r--   0 ak        (1000) ak        (1000)     1118 2022-03-09 09:38:11.000000 supylib-0.3/LICENSE
+-rw-r--r--   0 ak        (1000) ak        (1000)     1210 2023-05-03 15:06:47.000000 supylib-0.3/README.md
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 16:52:39.000000 supylib-0.3/python/
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/
+-rw-rw-r--   0 ak        (1000) ak        (1000)        5 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/top_level.txt
+-rw-rw-r--   0 ak        (1000) ak        (1000)        1 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/dependency_links.txt
+-rw-rw-r--   0 ak        (1000) ak        (1000)      671 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/SOURCES.txt
+-rw-rw-r--   0 ak        (1000) ak        (1000)     1823 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/PKG-INFO
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 16:52:39.000000 supylib-0.3/python/supy/
+-rw-r--r--   0 ak        (1000) ak        (1000)    12807 2019-02-28 09:55:09.000000 supylib-0.3/python/supy/forms.py
+-rw-rw-r--   0 ak        (1000) ak        (1000)   170861 2023-05-03 16:18:00.000000 supylib-0.3/python/supy/signal.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     6868 2022-09-08 14:57:35.000000 supylib-0.3/python/supy/guimaker3.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    40317 2022-03-09 08:59:15.000000 supylib-0.3/python/supy/sqltableeditor.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     7965 2022-03-09 08:57:33.000000 supylib-0.3/python/supy/multibase.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     6871 2019-02-28 09:56:23.000000 supylib-0.3/python/supy/guimaker.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    17745 2022-03-09 08:58:19.000000 supylib-0.3/python/supy/sqldatabase_inputmask.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    20272 2022-03-09 08:54:20.000000 supylib-0.3/python/supy/database_inputmask3.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    20266 2022-03-09 08:55:21.000000 supylib-0.3/python/supy/database_inputmask.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    19500 2022-03-09 08:55:47.000000 supylib-0.3/python/supy/database.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    31946 2022-03-09 09:01:33.000000 supylib-0.3/python/supy/widgets.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     5419 2022-03-09 08:57:58.000000 supylib-0.3/python/supy/serialize.py
+-rw-r--r--   0 ak        (1000) ak        (1000)   106175 2022-03-09 09:00:49.000000 supylib-0.3/python/supy/sqlforms.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    42485 2022-03-09 08:56:45.000000 supylib-0.3/python/supy/forms3.py
+-rw-rw-r--   0 ak        (1000) ak        (1000)       22 2022-11-02 18:18:03.000000 supylib-0.3/python/supy/__init__.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    30059 2022-03-09 08:58:51.000000 supylib-0.3/python/supy/sqldatabase.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     5226 2022-03-09 09:01:13.000000 supylib-0.3/python/supy/utilities.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    76826 2023-04-14 09:28:16.000000 supylib-0.3/python/supy/computervision.py
+-rw-rw-r--   0 ak        (1000) ak        (1000)      707 2023-05-03 16:52:39.000000 supylib-0.3/setup.cfg
+-rw-rw-r--   0 ak        (1000) ak        (1000)      104 2022-03-09 09:36:04.000000 supylib-0.3/pyproject.toml
+-rw-rw-r--   0 ak        (1000) ak        (1000)     1823 2023-05-03 16:52:39.000000 supylib-0.3/PKG-INFO
```

### Comparing `supylib-0.21/LICENSE` & `supylib-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `supylib-0.21/README.md` & `supylib-0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-supylib 0.21
+supylib 0.3
 -------------------------
-Eine Python-basierte Utility-Bibliothek für Datenbanken, Computer Vision und Machine Learning
-(c) Andreas Knoblauch, HS Albstadt-Sigmaringen
+Eine Python-basierte Utility-Bibliothek für Datenbanken, Computer Vision, Signalverarbeitung und Machine Learning
+(c) Andreas Knoblauch, HS Albstadt-Sigmaringen, 2015-2023
 
 Aktivierung/Sichtbarkeit
 -------------------------
 Der folgende Shell-Befehl macht das suplib/python Verzeichnis global sichtbar,
 indem vorne in PYTHONPATH und PATH gestellt wird (ggf. in .bashrc einfügen...):
 
 source /home/ak/projects/supylib/python/BashSrc
```

### Comparing `supylib-0.21/python/supylib.egg-info/SOURCES.txt` & `supylib-0.3/python/supylib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 python/supy/database_inputmask3.py
 python/supy/forms.py
 python/supy/forms3.py
 python/supy/guimaker.py
 python/supy/guimaker3.py
 python/supy/multibase.py
 python/supy/serialize.py
+python/supy/signal.py
 python/supy/sqldatabase.py
 python/supy/sqldatabase_inputmask.py
 python/supy/sqlforms.py
 python/supy/sqltableeditor.py
 python/supy/utilities.py
 python/supy/widgets.py
 python/supylib.egg-info/PKG-INFO
```

### Comparing `supylib-0.21/python/supylib.egg-info/PKG-INFO` & `supylib-0.3/python/supylib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: supylib
-Version: 0.21
-Summary: A Python-based utility library for databases, computer vision, and machine learning
+Version: 0.3
+Summary: A Python-based utility library for databases, computer vision, signal processing, and machine learning
 Home-page: https://github.com/aknoblauch/supylib
 Author: Andreas Knoblauch
 Author-email: knoblauch@hs-albsig.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aknoblauch/supylib/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-supylib 0.21
+supylib 0.3
 -------------------------
-Eine Python-basierte Utility-Bibliothek für Datenbanken, Computer Vision und Machine Learning
-(c) Andreas Knoblauch, HS Albstadt-Sigmaringen
+Eine Python-basierte Utility-Bibliothek für Datenbanken, Computer Vision, Signalverarbeitung und Machine Learning
+(c) Andreas Knoblauch, HS Albstadt-Sigmaringen, 2015-2023
 
 Aktivierung/Sichtbarkeit
 -------------------------
 Der folgende Shell-Befehl macht das suplib/python Verzeichnis global sichtbar,
 indem vorne in PYTHONPATH und PATH gestellt wird (ggf. in .bashrc einfügen...):
 
 source /home/ak/projects/supylib/python/BashSrc
```

### Comparing `supylib-0.21/python/supy/forms.py` & `supylib-0.3/python/supy/forms.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/guimaker3.py` & `supylib-0.3/python/supy/guimaker3.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/sqltableeditor.py` & `supylib-0.3/python/supy/sqltableeditor.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/multibase.py` & `supylib-0.3/python/supy/multibase.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/guimaker.py` & `supylib-0.3/python/supy/guimaker.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/sqldatabase_inputmask.py` & `supylib-0.3/python/supy/sqldatabase_inputmask.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/database_inputmask3.py` & `supylib-0.3/python/supy/database_inputmask3.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/database_inputmask.py` & `supylib-0.3/python/supy/database_inputmask.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/database.py` & `supylib-0.3/python/supy/database.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/widgets.py` & `supylib-0.3/python/supy/widgets.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/serialize.py` & `supylib-0.3/python/supy/serialize.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/sqlforms.py` & `supylib-0.3/python/supy/sqlforms.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/forms3.py` & `supylib-0.3/python/supy/forms3.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/sqldatabase.py` & `supylib-0.3/python/supy/sqldatabase.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/utilities.py` & `supylib-0.3/python/supy/utilities.py`

 * *Files identical despite different names*

### Comparing `supylib-0.21/python/supy/computervision.py` & `supylib-0.3/python/supy/computervision.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 #  - def limitPosNegValsByMedians(im,fac_med_pos,fac_med_neg=None)
 #  - def getBWImage_locally_darkest(img,sz_kernel,p_darkest)
 #  - def getBWImage_darkest(img,p_darkest)
 #  - def getBWImage_opened_closed(img,open_and_closes)
 #  - def getBWImage(img,th_lo,th_hi, flagMorph,krn_close,krn_open, flagCanny,canny_th1,canny_th2,canny_aperturesize)
 # 
 # Part III) Kernel Operations
-#  - def getDoGKernel(r,sigx1,sigy1=None,sigx2=0,sigy2=None,phi=0.0,weight1=1.0,weight2=1.0,mu_x=0.0,mu_y=0.0,box=None,mu_x_target=0.0,mu_y_target=0.0,flagCircularMask=1,norm=0)
+#  - def getDoGKernel(r,sigx1,sigy1=None,sigx2=0,sigy2=None,phi=0.0,weight1=1.0,weight2=1.0,mu_x=0.0,mu_y=0.0,box=None,mu_x_target=0.0,mu_y_target=0.0,flagCircularMask=1,norm=0,ry=None)
 #  - def getGaborWaveletKernel(r, lmbda, theta, psi, sigma, gamma)
 #  - def getLineKernel(l,b,phi,eps=1e-6,r=None)
 #  - def getBlockKernel(r,x1,y1,l,w,phi=0,norm=1)
 #  - def getDoBKernel(r,l,alpha,beta,wIn,wOut,phi,offset=[0,0],flagReturnPosNegMasks=0)
 # 
 # Part IV) Region- and Kernel-based operations
 #  - def applyKernelOnImagePos(img,kernel,i,j,op='+',w=1.0,flagInplace=0)
@@ -544,15 +544,15 @@
         img_edges = cv2.Canny(img,canny_th1,canny_th2,canny_aperturesize)
     return img_bw,img_bw_hi,img_bw_lo,img_bw_closed,img_bw_opened,img_edges
 
 # ***************************************************************************************
 # Part III) Kernel Operations
 # ***************************************************************************************
 
-def getDoGKernel(r,sigx1,sigy1=None,sigx2=0,sigy2=None,phi=0.0,weight1=1.0,weight2=1.0,mu_x=0.0,mu_y=0.0,box=None,mu_x_target=0.0,mu_y_target=0.0,flagCircularMask=1,norm=0):
+def getDoGKernel(r,sigx1,sigy1=None,sigx2=0,sigy2=None,phi=0.0,weight1=1.0,weight2=1.0,mu_x=0.0,mu_y=0.0,box=None,mu_x_target=0.0,mu_y_target=0.0,flagCircularMask=1,norm=0,ry=None):
     """
     generate DifferenceOfGaussian kernel
     that is normalized and oriented
     :param r: kernel radius (i.e., size = 2*r+1) 
     :param sigx1,sigy1: s.d. in x and y direction of the inner unorientated gaussian (sigy defaults to sigx)
     :param sigx2,sigy2: s.d. in x and y direction of the outer unorientated gaussian (sigy defaults to sigx); if 0 then just take first Gaussian (default)!
     :param phi: rotation in rad (default: 0 rad)
@@ -561,26 +561,27 @@
     :param mu_x: offset of Gauss center relative to midpoint in x-direction (before rotation)
     :param mu_y: offset of Gauss center relative to midpoint in y-direction (before rotation)
     :param box: integer list [x1 y1 x2 y2] defining a rectangle that will be cut out (default: whole kernel region [-r -r r r])
     :param mu_x_target: offset of Gauss center relative to midpoint in x-direction (target after rotation)
     :param mu_y_target: offset of Gauss center relative to midpoint in y-direction (target after rotation)
     :param flagCircularMask: if set then apply a circular mask; otherwise full size rectangular
     :param norm: if >0 then the final kernel is normalized to Euklidean length 1
+    :param ry: if not None then use ry as radius in y-direction (if None, then r is radius for both x- and y-direction)  
     :returns kernel: resulting kernel  
-
     """
     if sigy1==None: sigy1=sigx1   # default: sigy1 = sigx1
     if sigy2==None: sigy2=sigx2   # default: sigy2 = sigx2
-    sz=2*r+1                      # kernel size
-    kernel1 = np.zeros((sz,sz))   # allocate kernel
-    
-    x = np.array([np.arange(-r,r+1) for i in range(sz)],'float')       # x values relative to kernel mid point (=origin)
-    y = np.array([np.arange(r,-r-1,-1) for i in range(sz)],'float').T  # y values relative to kernel mid point (=origin)
+    sz_x=2*r+1                    # kernel size
+    if ry is None: ry,sz_y=r,sz_x # size in y direction same as in x direction?
+    else: sz_y=2*ry+1             # size in y direction differs from size in x-direction
+    x = np.array([np.arange(-r,r+1) for i in range(sz_y)],'float')           # x values relative to kernel mid point (=origin)
+    y = np.array([np.arange(ry,-ry-1,-1) for i in range(sz_x)],'float').T    # y values relative to kernel mid point (=origin)
+    kernel1 = np.zeros((sz_y,sz_x))  # allocate kernel
     h = np.sqrt(np.multiply(x,x)+np.multiply(y,y)) # distance of P(x,y) from origin
-    mask = np.ones((sz,sz))                        # initialize mask with ones
+    mask = np.ones(kernel1.shape)                  # initialize mask with ones
     if flagCircularMask>0: mask[h>r]=0             # set all points outside circle with radius r to zero ?
     x_rot = (x-mu_x_target)*np.cos(-phi)-(y-mu_y_target)*np.sin(-phi)-mu_x   # rotate back to coordinates of the Gauss template function
     y_rot = (y-mu_y_target)*np.cos(-phi)+(x-mu_x_target)*np.sin(-phi)-mu_y   # rotate back to coordinates of the Gauss template function
     x_rot2=np.multiply(x_rot,x_rot)                # x_rot squared
     y_rot2=np.multiply(y_rot,y_rot)                # y_rot squared
     varx1,vary1 = sigx1*sigx1, sigy1*sigy1         # variances for inner Gaussian
     varx2,vary2 = sigx2*sigx2, sigy2*sigy2         # variances for outer Gaussian
```

### Comparing `supylib-0.21/setup.cfg` & `supylib-0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = supylib
-version = 0.21
+version = 0.3
 author = Andreas Knoblauch
 author_email = knoblauch@hs-albsig.de
-description = A Python-based utility library for databases, computer vision, and machine learning
+description = A Python-based utility library for databases, computer vision, signal processing, and machine learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aknoblauch/supylib
 project_urls = 
 	Bug Tracker = https://github.com/aknoblauch/supylib/issues
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `supylib-0.21/PKG-INFO` & `supylib-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: supylib
-Version: 0.21
-Summary: A Python-based utility library for databases, computer vision, and machine learning
+Version: 0.3
+Summary: A Python-based utility library for databases, computer vision, signal processing, and machine learning
 Home-page: https://github.com/aknoblauch/supylib
 Author: Andreas Knoblauch
 Author-email: knoblauch@hs-albsig.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aknoblauch/supylib/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-supylib 0.21
+supylib 0.3
 -------------------------
-Eine Python-basierte Utility-Bibliothek für Datenbanken, Computer Vision und Machine Learning
-(c) Andreas Knoblauch, HS Albstadt-Sigmaringen
+Eine Python-basierte Utility-Bibliothek für Datenbanken, Computer Vision, Signalverarbeitung und Machine Learning
+(c) Andreas Knoblauch, HS Albstadt-Sigmaringen, 2015-2023
 
 Aktivierung/Sichtbarkeit
 -------------------------
 Der folgende Shell-Befehl macht das suplib/python Verzeichnis global sichtbar,
 indem vorne in PYTHONPATH und PATH gestellt wird (ggf. in .bashrc einfügen...):
 
 source /home/ak/projects/supylib/python/BashSrc
```

