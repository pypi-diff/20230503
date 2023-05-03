# Comparing `tmp/tunnelvision-0.3.2-py3-none-manylinux1_x86_64.whl.zip` & `tmp/tunnelvision-0.3.3-py3-none-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,24 @@
-Zip file size: 25313 bytes, number of entries: 17
--rw-rw-r--  2.0 unx      189 b- defN 23-Apr-25 21:54 tunnelvision/__init__.py
+Zip file size: 3393277 bytes, number of entries: 22
+-rw-rw-r--  2.0 unx      189 b- defN 23-May-03 16:47 tunnelvision/__init__.py
 -rw-rw-r--  2.0 unx     1472 b- defN 23-Apr-25 04:54 tunnelvision/config.py
 -rw-rw-r--  2.0 unx       89 b- defN 23-Apr-14 22:07 tunnelvision/definitions.py
 -rw-rw-r--  2.0 unx      638 b- defN 23-Apr-25 04:54 tunnelvision/logger.py
--rw-rw-r--  2.0 unx     5935 b- defN 23-Apr-25 04:54 tunnelvision/plot.py
+-rw-rw-r--  2.0 unx     5942 b- defN 23-May-03 16:47 tunnelvision/plot.py
 -rw-rw-r--  2.0 unx     1356 b- defN 23-Apr-25 04:54 tunnelvision/utils.py
+-rwxrwxr-x  2.0 unx 10182432 b- defN 23-May-03 16:49 tunnelvision/bin/tunnelvision-server
 -rw-rw-r--  2.0 unx     1021 b- defN 23-Apr-25 21:54 tunnelvision/bin/dist/index.html
+-rw-rw-r--  2.0 unx   192210 b- defN 23-Apr-25 04:54 tunnelvision/bin/dist/assets/bridge.78d53f15.js
+-rw-rw-r--  2.0 unx   393740 b- defN 23-Apr-25 21:54 tunnelvision/bin/dist/assets/index.58d42c0b.js
+-rw-rw-r--  2.0 unx     4240 b- defN 23-Apr-25 21:54 tunnelvision/bin/dist/assets/index.73b74798.css
+-rw-rw-r--  2.0 unx  1589244 b- defN 23-Apr-25 04:54 tunnelvision/bin/dist/assets/tv.b4f81926.wasm
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-14 22:07 tunnelvision/experimental/__init__.py
 -rw-rw-r--  2.0 unx     5399 b- defN 23-Apr-15 02:40 tunnelvision/experimental/plot.py
 -rw-rw-r--  2.0 unx      231 b- defN 23-Apr-25 04:54 tunnelvision/server/__init__.py
 -rw-rw-r--  2.0 unx     6323 b- defN 23-Apr-25 04:54 tunnelvision/server/server.py
 -rw-rw-r--  2.0 unx     1119 b- defN 23-Apr-25 04:54 tunnelvision/server/state.py
--rw-rw-r--  2.0 unx    34523 b- defN 23-Apr-25 22:15 tunnelvision-0.3.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3149 b- defN 23-Apr-25 22:15 tunnelvision-0.3.2.dist-info/METADATA
--rw-rw-r--  2.0 unx      106 b- defN 23-Apr-25 22:15 tunnelvision-0.3.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 23-Apr-25 22:15 tunnelvision-0.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1415 b- defN 23-Apr-25 22:15 tunnelvision-0.3.2.dist-info/RECORD
-17 files, 62978 bytes uncompressed, 22979 bytes compressed:  63.5%
+-rw-rw-r--  2.0 unx    34523 b- defN 23-May-03 16:50 tunnelvision-0.3.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3149 b- defN 23-May-03 16:50 tunnelvision-0.3.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx      106 b- defN 23-May-03 16:50 tunnelvision-0.3.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 23-May-03 16:50 tunnelvision-0.3.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1932 b- defN 23-May-03 16:50 tunnelvision-0.3.3.dist-info/RECORD
+22 files, 12425368 bytes uncompressed, 3390121 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -12,17 +12,32 @@
 
 Filename: tunnelvision/plot.py
 Comment: 
 
 Filename: tunnelvision/utils.py
 Comment: 
 
+Filename: tunnelvision/bin/tunnelvision-server
+Comment: 
+
 Filename: tunnelvision/bin/dist/index.html
 Comment: 
 
+Filename: tunnelvision/bin/dist/assets/bridge.78d53f15.js
+Comment: 
+
+Filename: tunnelvision/bin/dist/assets/index.58d42c0b.js
+Comment: 
+
+Filename: tunnelvision/bin/dist/assets/index.73b74798.css
+Comment: 
+
+Filename: tunnelvision/bin/dist/assets/tv.b4f81926.wasm
+Comment: 
+
 Filename: tunnelvision/experimental/__init__.py
 Comment: 
 
 Filename: tunnelvision/experimental/plot.py
 Comment: 
 
 Filename: tunnelvision/server/__init__.py
@@ -30,23 +45,23 @@
 
 Filename: tunnelvision/server/server.py
 Comment: 
 
 Filename: tunnelvision/server/state.py
 Comment: 
 
-Filename: tunnelvision-0.3.2.dist-info/LICENSE
+Filename: tunnelvision-0.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: tunnelvision-0.3.2.dist-info/METADATA
+Filename: tunnelvision-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: tunnelvision-0.3.2.dist-info/WHEEL
+Filename: tunnelvision-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: tunnelvision-0.3.2.dist-info/top_level.txt
+Filename: tunnelvision-0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: tunnelvision-0.3.2.dist-info/RECORD
+Filename: tunnelvision-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tunnelvision/__init__.py

```diff
@@ -1,8 +1,8 @@
 """Tunnelvision"""
 
 from tunnelvision.plot import Axes, imshow, show  # noqa: F401
 
 __all__ = ["plot", "Axes", "show", "imshow"]
 
 # This line will be read by setup.py
-__version__ = "0.3.2"
+__version__ = "0.3.3"
```

## tunnelvision/plot.py

```diff
@@ -167,15 +167,16 @@
     Args:
         x (np.ndarray): The array to display.
         ax: The Axes object to use.
     """
     if ax is None:
         ax = Axes()
 
-    return ax.imshow(x=x, **kwargs)
+    ax.imshow(x=x, **kwargs)
+    return ax
 
 
 def show(x: np.generic, ax: Axes = None, **kwargs):
     """Display a multi-dimensional array.
 
     Args:
         x (np.generic): The array to display.
```

## Comparing `tunnelvision-0.3.2.dist-info/LICENSE` & `tunnelvision-0.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tunnelvision-0.3.2.dist-info/METADATA` & `tunnelvision-0.3.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tunnelvision
-Version: 0.3.2
+Version: 0.3.3
 Summary: Experimental tensor viewer for IPython built on top of Voxel
 Home-page: https://github.com/sluijs/tunnelvision
 Author: Rogier van der Sluijs
 License: GNU
 Project-URL: Documentation, https://tunnelvision.readthedocs.io/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `tunnelvision-0.3.2.dist-info/RECORD` & `tunnelvision-0.3.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-tunnelvision/__init__.py,sha256=TA0n4J4iQ-40C1ICux2EG7YAIQ-shIT-Uf27Y9b155A,189
+tunnelvision/__init__.py,sha256=kliLClsCGps1N6PEm5syq7h7tu18BX-ghUzt0WMlYsc,189
 tunnelvision/config.py,sha256=7nSzwOLwfskrnRcQBlI3kr5USCyrfJoiksq7SszXagI,1472
 tunnelvision/definitions.py,sha256=jVkGpbx4_hiTW0TiN9WEGPtTXRJkVob26NTVnaf5r9g,89
 tunnelvision/logger.py,sha256=bECJ--zHo3QPj0cSQK1AX26BHE_UP0qcPQ3DNm2gBRA,638
-tunnelvision/plot.py,sha256=rm7Rel6lQnX_eZp0_Da3Xuzkwz4PI4CmZCDVwe1QWCA,5935
+tunnelvision/plot.py,sha256=icjyreyRJCd79M0fWGJjXFbD95npIBrpp7BGHMKW-IY,5942
 tunnelvision/utils.py,sha256=bhgF9nR5KP7QlkFEnnE2N-kf0PesVMZqV3ypbsllQKs,1356
+tunnelvision/bin/tunnelvision-server,sha256=ygAJJuizfIp01wqj0sKTzCHamkOGrVesbmemLd6DDRM,10182432
 tunnelvision/bin/dist/index.html,sha256=bXjz2DbHn-G88UcQIx1IvfZ6-PgYJH5n3bdhJwlhJTQ,1021
+tunnelvision/bin/dist/assets/bridge.78d53f15.js,sha256=ApGZ3Jkb-SlLr5jjpSHaEwG63uNk7iFmv3T-h8UdX3w,192210
+tunnelvision/bin/dist/assets/index.58d42c0b.js,sha256=VAmyZwhsNuDJg1V5Dw4QoB3iWSEGVS-vZkGH7fUImYY,393740
+tunnelvision/bin/dist/assets/index.73b74798.css,sha256=c7dHmMo3Sp1m6G1ZCJfirOs5hqiceFxOaeogDN_xd7Q,4240
+tunnelvision/bin/dist/assets/tv.b4f81926.wasm,sha256=tPgZJtZjjnu5TKQjJqT1_EMvTm3eaCncPYHRW4hw-WM,1589244
 tunnelvision/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tunnelvision/experimental/plot.py,sha256=cN8oQhdLX-3CgTBLm8NSLGt_H2wmx3tUlWjHl3dODQ8,5399
 tunnelvision/server/__init__.py,sha256=Rr-J8ZnpwDuDQhJgp55pYnAPoSMYIp4X6JOVvpW8cvc,231
 tunnelvision/server/server.py,sha256=1XkGXISq9lbXXvlkd1DTj25wVIC-bs5VEVO6mbXKoj8,6323
 tunnelvision/server/state.py,sha256=-BlvLfuJsuSbVaTIUGlJdT1COZa8-wRLw-VSJ02b8fM,1119
-tunnelvision-0.3.2.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-tunnelvision-0.3.2.dist-info/METADATA,sha256=fyL9lxr31Y9L7wkX2xLCR4xE9XSC9AzyRm8rcF0qQUk,3149
-tunnelvision-0.3.2.dist-info/WHEEL,sha256=-kQi_VMfvRQozZJT7HUPMfY-5vLo0LVTmAylNJ3Ft98,106
-tunnelvision-0.3.2.dist-info/top_level.txt,sha256=XUh4ZBFbjHxVS8ULjfgvL1v1gVEk1C6TSx-ZTVwVWVg,13
-tunnelvision-0.3.2.dist-info/RECORD,,
+tunnelvision-0.3.3.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+tunnelvision-0.3.3.dist-info/METADATA,sha256=t1wucYodRY7i4hpeBbxxN5U6OHIGxzXegYjwv4qkBXk,3149
+tunnelvision-0.3.3.dist-info/WHEEL,sha256=-kQi_VMfvRQozZJT7HUPMfY-5vLo0LVTmAylNJ3Ft98,106
+tunnelvision-0.3.3.dist-info/top_level.txt,sha256=XUh4ZBFbjHxVS8ULjfgvL1v1gVEk1C6TSx-ZTVwVWVg,13
+tunnelvision-0.3.3.dist-info/RECORD,,
```

