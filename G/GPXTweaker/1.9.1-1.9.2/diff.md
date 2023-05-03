# Comparing `tmp/GPXTweaker-1.9.1.tar.gz` & `tmp/GPXTweaker-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPXTweaker-1.9.1.tar", last modified: Wed Mar 30 16:27:02 2022, max compression
+gzip compressed data, was "GPXTweaker-1.9.2.tar", last modified: Wed Apr 27 19:26:39 2022, max compression
```

## Comparing `GPXTweaker-1.9.1.tar` & `GPXTweaker-1.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-03-30 16:27:02.807201 GPXTweaker-1.9.1/
--rw-rw-rw-   0        0        0    35149 2022-03-09 11:48:36.000000 GPXTweaker-1.9.1/LICENSE
--rw-rw-rw-   0        0        0    15017 2022-03-30 16:27:02.807201 GPXTweaker-1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0    14097 2022-03-09 11:48:36.000000 GPXTweaker-1.9.1/README.md
--rw-rw-rw-   0        0        0      108 2022-02-05 21:10:24.000000 GPXTweaker-1.9.1/pyproject.toml
--rw-rw-rw-   0        0        0      963 2022-03-30 16:27:02.807201 GPXTweaker-1.9.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-03-30 16:27:02.781558 GPXTweaker-1.9.1/src/
-drwxrwxrwx   0        0        0        0 2022-03-30 16:27:02.791560 GPXTweaker-1.9.1/src/GPXTweaker/
--rw-rw-rw-   0        0        0     6327 2022-03-22 22:42:24.000000 GPXTweaker-1.9.1/src/GPXTweaker/GPXTweaker.cfg
--rw-rw-rw-   0        0        0   734563 2022-03-30 09:49:10.000000 GPXTweaker-1.9.1/src/GPXTweaker/GPXTweaker.py
--rw-rw-rw-   0        0        0    14097 2022-03-19 09:48:40.000000 GPXTweaker-1.9.1/src/GPXTweaker/README.md
--rw-rw-rw-   0        0        0        0 2022-02-05 21:03:43.000000 GPXTweaker-1.9.1/src/GPXTweaker/__init__.py
--rwxrwxrwx   0        0        0      135 2021-04-19 23:17:36.000000 GPXTweaker-1.9.1/src/GPXTweaker/jpegtran.bat
--rw-rw-rw-   0        0        0     8680 2022-03-19 09:48:40.000000 GPXTweaker-1.9.1/src/GPXTweaker/test.py
-drwxrwxrwx   0        0        0        0 2022-03-30 16:27:02.807201 GPXTweaker-1.9.1/src/GPXTweaker.egg-info/
--rw-rw-rw-   0        0        0    15017 2022-03-30 16:27:02.000000 GPXTweaker-1.9.1/src/GPXTweaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2022-03-30 16:27:02.000000 GPXTweaker-1.9.1/src/GPXTweaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-30 16:27:02.000000 GPXTweaker-1.9.1/src/GPXTweaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-03-30 16:27:02.000000 GPXTweaker-1.9.1/src/GPXTweaker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-04-27 19:26:39.793652 GPXTweaker-1.9.2/
+-rw-rw-rw-   0        0        0    35149 2022-03-09 11:48:36.000000 GPXTweaker-1.9.2/LICENSE
+-rw-rw-rw-   0        0        0    15017 2022-04-27 19:26:39.793652 GPXTweaker-1.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14097 2022-04-15 08:27:16.000000 GPXTweaker-1.9.2/README.md
+-rw-rw-rw-   0        0        0      108 2022-02-05 21:10:24.000000 GPXTweaker-1.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0      963 2022-04-27 19:26:39.793652 GPXTweaker-1.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-04-27 19:26:39.767957 GPXTweaker-1.9.2/src/
+drwxrwxrwx   0        0        0        0 2022-04-27 19:26:39.777992 GPXTweaker-1.9.2/src/GPXTweaker/
+-rw-rw-rw-   0        0        0     6327 2022-04-15 08:27:16.000000 GPXTweaker-1.9.2/src/GPXTweaker/GPXTweaker.cfg
+-rw-rw-rw-   0        0        0   736335 2022-04-27 19:19:30.000000 GPXTweaker-1.9.2/src/GPXTweaker/GPXTweaker.py
+-rw-rw-rw-   0        0        0    14097 2022-03-19 09:48:40.000000 GPXTweaker-1.9.2/src/GPXTweaker/README.md
+-rw-rw-rw-   0        0        0        0 2022-02-05 21:03:43.000000 GPXTweaker-1.9.2/src/GPXTweaker/__init__.py
+-rwxrwxrwx   0        0        0      135 2021-04-19 23:17:36.000000 GPXTweaker-1.9.2/src/GPXTweaker/jpegtran.bat
+-rw-rw-rw-   0        0        0     8680 2022-03-19 09:48:40.000000 GPXTweaker-1.9.2/src/GPXTweaker/test.py
+drwxrwxrwx   0        0        0        0 2022-04-27 19:26:39.793652 GPXTweaker-1.9.2/src/GPXTweaker.egg-info/
+-rw-rw-rw-   0        0        0    15017 2022-04-27 19:26:39.000000 GPXTweaker-1.9.2/src/GPXTweaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2022-04-27 19:26:39.000000 GPXTweaker-1.9.2/src/GPXTweaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-27 19:26:39.000000 GPXTweaker-1.9.2/src/GPXTweaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2022-04-27 19:26:39.000000 GPXTweaker-1.9.2/src/GPXTweaker.egg-info/top_level.txt
```

### Comparing `GPXTweaker-1.9.1/LICENSE` & `GPXTweaker-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GPXTweaker-1.9.1/PKG-INFO` & `GPXTweaker-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPXTweaker
-Version: 1.9.1
+Version: 1.9.2
 Summary: A script in Python 3 to visualize, in 2D and 3D, and edit GPX tracks
 Home-page: https://github.com/PCigales/GPXTweaker
 Author: PCigales
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/PCigales/GPXTweaker/issues
 Keywords: gpx,gis,wms,wmts,3d,wgs84,mercator,geotag
 Platform: win64
```

### Comparing `GPXTweaker-1.9.1/README.md` & `GPXTweaker-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `GPXTweaker-1.9.1/setup.cfg` & `GPXTweaker-1.9.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2047 5058 5477 6561 6b65 720d 0a76   = GPXTweaker..v
-00000020: 6572 7369 6f6e 203d 2031 2e39 2e31 0d0a  ersion = 1.9.1..
+00000020: 6572 7369 6f6e 203d 2031 2e39 2e32 0d0a  ersion = 1.9.2..
 00000030: 6175 7468 6f72 203d 2050 4369 6761 6c65  author = PCigale
 00000040: 730d 0a6c 6963 656e 7365 203d 2047 4e55  s..license = GNU
 00000050: 2047 504c 7633 0d0a 6465 7363 7269 7074   GPLv3..descript
 00000060: 696f 6e20 3d20 4120 7363 7269 7074 2069  ion = A script i
 00000070: 6e20 5079 7468 6f6e 2033 2074 6f20 7669  n Python 3 to vi
 00000080: 7375 616c 697a 652c 2069 6e20 3244 2061  sualize, in 2D a
 00000090: 6e64 2033 442c 2061 6e64 2065 6469 7420  nd 3D, and edit
```

### Comparing `GPXTweaker-1.9.1/src/GPXTweaker/GPXTweaker.cfg` & `GPXTweaker-1.9.2/src/GPXTweaker/GPXTweaker.cfg`

 * *Files identical despite different names*

### Comparing `GPXTweaker-1.9.1/src/GPXTweaker/GPXTweaker.py` & `GPXTweaker-1.9.2/src/GPXTweaker/GPXTweaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# GPXTweaker v1.9.1 (https://github.com/PCigales/GPXTweaker)
+# GPXTweaker v1.9.2 (https://github.com/PCigales/GPXTweaker)
 # Copyright © 2022 PCigales
 # This program is licensed under the GNU GPLv3 copyleft license (see https://www.gnu.org/licenses)
 
 from functools import partial
 import urllib.parse
 import socket
 import selectors
@@ -304,14 +304,15 @@
     'jvfov': 'Champ de vue vertical:',
     'jheight': 'Hauteur de vue:',
     'start': 'démarrage',
     'close': 'fermeture'
   },
   'parser': {
     'license': 'Ce programme est sous licence copyleft GNU GPLv3 (voir https://www.gnu.org/licenses)',
+    'help': 'affichage du message d\'aide et interruption du script',
     'uri': 'chemin d\'accès à la trace ou argument pas mentionné pour démarrer avec l\'explorateur de traces',
     'conf': 'chemin d\'accès au fichier de configuration [même répertoire que le script par défaut]',
     'trk': 'indice de la trace (commençant à 0) [0 par défaut]',
     'map': 'chemin d\'accès complet à la carte ou nom du fournisseur de carte ou vide pour utiliser le premier founisseur de carte configuré, ou option pas mentionnée pour utiliser les fournisseurs de tuiles configurés [par défaut]',
     'emap': 'chemin d\'accès complet à la carte d\'altitudes ou nom du fournisseur de carte d\'altitudes ou vide pour utiliser le premier fournisseur de carte d\'altitudes configuré, ou option pas mentionnée pour utiliser les fournisseurs de tuiles et données d\'altitudes configurés [par défaut]',
     'box': '"minlat, maxlat, minlon, maxlon" (latitudes minimale et maximale, longitudes minimale et maximale, avec les "" ) de la carte à charger / à retourner (pour l\'utilisation d\'une carte / d\'un fournisseur de carte) [lu dans les métadonnées gpxtweaker de la carte / déterminé à partir de la trace par défaut]',
     'size': '"height, width" (hauteur et largeur, avec les "") de la carte à charger / "maxheight, maxwidth" (hauteur et largeur maximales, avec les "") de la carte à retourner (pour l\'utilisation d\'une carte / d\'un fournisseur de carte) [lu dans les métadonnées gpxtweaker de la carte / "2000, 4000" par défaut]',
@@ -590,14 +591,15 @@
     'jvfov': 'Vertical field of view:',
     'jheight': 'Height of view:',
     'start': 'start-up',
     'close': 'shutdown'
   },
   'parser': {
     'license': 'This program is licensed under the GNU GPLv3 copyleft license (see https://www.gnu.org/licenses)',
+    'help': 'display of the help message and interruption of the script',
     'uri': 'path to the track or argument not mentioned to start with the explorer of tracks',
     'conf': 'full path to the configuration file [same folder as the script by default]',
     'trk': 'index of the track (starting at 0) [0 by default]',
     'map': 'full path to the map or name of the map provider or blank to use the first map provider configured, or option not mentioned to use the tiles providers configured [by default]',
     'emap': 'path to the elevations map or name of the elevations map provider or blank to use the first elevations map configured, or option not mentioned to use the elevations tiles and data providers configured [by default]',
     'box': '"minlat, maxlat, minlon, maxlon" (minimum and maximum latitudes, minimum and maximum longitudes, with the "") of the map to be loaded / retrieved (for the use of a map / of a map provider) [read from the gpxtweaker metadata of the map / determined from the track by default]',
     'size': '"height, width" (height and width, with the "") of the map to be loaded / "maxheight, maxwidth" (maximum height and width, with the "") of the map to be retrieved (for the use of a map / of a map provider) [read from the gpxtweaker metadata of the map / "2000, 4000" by default]',
@@ -607,15 +609,15 @@
     'gpx': 'only .gpx files are supported',
     'open': 'Open the url %s',
     'keyboard': 'Press "S" to exit'
    }
 }
 LSTRINGS = EN_STRINGS
 try:
-  if locale.getdefaultlocale()[0][:2].lower() == 'fr':
+  if locale.getlocale()[0][:2].lower() == 'fr':
     LSTRINGS = FR_STRINGS
 except:
   pass
 
 VERBOSITY = 0
 def log(kmod, level, kmsg, *var):
   if level <= VERBOSITY:
@@ -671,15 +673,15 @@
 class HTTPMessage():
 
   @staticmethod
   def _read_headers(msg, http_message):
     if not msg:
       return False
     a = None
-    for msg_line in msg.splitlines()[:-1]:
+    for msg_line in msg.replace('\r\n', '\n').split('\n')[:-2]:
       if a is None:
         try:
           a, b, c = msg_line.strip().split(None, 2)
         except:
           try:
             a, b, c = *msg_line.strip().split(None, 2), ''
           except:
@@ -3463,55 +3465,55 @@
             b = self._XMLNewNode('color', self.GPXSTYLE_NAMESPACE)
             a.appendChild(b)
           t = XMLText(msgp[1].lstrip('#'))
           while b.hasChildNodes():
             b.removeChild(b.firstChild).unlink()
           b.appendChild(t)
         elif msgp[0][-4:] == 'name':
-          self._XMLUpdateChildNodeText(trk, 'name', trkns, trkp, msgp[1], None, True)
+          self._XMLUpdateChildNodeText(trk, 'name', trkns, trkp, ' '.join(msgp[1].splitlines()), None, True)
         else:
           raise
         if not self.ProcessGPX('e'):
           raise
       else:
         msgp = msg.split('=\r\n')
-        nmsg = msgp[0].splitlines()
-        wpmsg = msgp[1].splitlines()
+        nmsg = msgp[0].split('\r\n')[:-1]
+        wpmsg = msgp[1].split('\r\n')[:-1]
         smsg = msgp[2].split('-\r\n')[1:]
         wpts = r.removeChildren('wpt')
         segs = trk.removeChildren('trkseg')
         pts = list(pt for seg in segs for pt in seg.removeChildren('trkpt'))
-        self._XMLUpdateChildNodeText(trk, 'name', trkns, trkp, (nmsg or [''])[0], None, True)
+        self._XMLUpdateChildNodeText(trk, 'name', trkns, trkp, ' '.join((nmsg or [''])[0].splitlines()), None, True)
         wpn = []
         for wp in wpmsg:
           if '&' in wp:
             v = wp.split('&')
             if int(v[0]) < len(wpts):
               nwp = wpts[int(v[0])]
               wpts[int(v[0])] = None
             else:
               nwp = self._XMLNewNode('wpt', trkns, trkp)
             self._XMLUpdateAttribute(nwp, 'lat', v[1])
             self._XMLUpdateAttribute(nwp, 'lon', v[2])
             self._XMLUpdateChildNodeText(nwp, 'ele', trkns, trkp, v[3], None)
             self._XMLUpdateChildNodeText(nwp, 'time', trkns, trkp, urllib.parse.unquote(v[4]), ('ele',))
-            self._XMLUpdateChildNodeText(nwp, 'name', trkns, trkp, urllib.parse.unquote(v[5]), ('geoidheight', 'magvar', 'time', 'ele') , True)
+            self._XMLUpdateChildNodeText(nwp, 'name', trkns, trkp, ' '.join(urllib.parse.unquote(v[5]).splitlines()), ('geoidheight', 'magvar', 'time', 'ele') , True)
           else:
             nwp = wpts[int(wp)]
             wpts[int(wp)] = None
           wpn.append(nwp)
         r.insertAfter(wpn, (r.getChildren('metadata') or [None])[-1])
         for wp in wpts:
           if wp is not None:
             wp.unlink()
         for s in segs:
           s.unlink()
         for s in smsg:
           ns = self._XMLNewNode('trkseg', trkns, trkp)
-          pmsg = s.splitlines()
+          pmsg = s.split('\r\n')[:-1]
           for p in pmsg:
             if '&' in p:
               v = p.split('&')
               if int(v[0]) < len(pts):
                 np = pts[int(v[0])]
                 pts[int(v[0])] = None
               else:
@@ -3735,22 +3737,26 @@
     else:
       return None
 
 
 class GeotaggedMedia():
 
   MP4_EPOCH = 2082844800
-  if locale.getdefaultlocale()[0][:2].lower() == 'fr':
-    DATETIME_FORMAT = '%d/%m/%Y %H:%M:%S'
-    @staticmethod
-    def DATETIME_CONVERT(dt):
-      dtc = dt.split()
-      dtc[0] = '/'.join(dtc[0].split(':')[::-1])
-      return ' '.join(dtc)
-  else:
+  DATETIME_FORMAT = ''
+  try:
+    if locale.getlocale()[0][:2].lower() == 'fr':
+      DATETIME_FORMAT = '%d/%m/%Y %H:%M:%S'
+      @staticmethod
+      def DATETIME_CONVERT(dt):
+        dtc = dt.split()
+        dtc[0] = '/'.join(dtc[0].split(':')[::-1])
+        return ' '.join(dtc)
+  except:
+    pass
+  if not DATETIME_FORMAT:
     DATETIME_FORMAT = '%Y/%m/%d %H:%M:%S'
     @staticmethod
     def DATETIME_CONVERT(dt):
       return dt.replace(':', '/', 2)
   
   def __init__(self, folders, photos=True, videos=True, box=None):
     self.Folders = folders
@@ -9066,26 +9072,30 @@
   '      var mousey = null;\r\n' \
   '      var viewpane = document.getElementById("view");\r\n' \
   '      var handle = document.getElementById("handle");\r\n' \
   '      var hand = null;\r\n' \
   '      var hand_m = false;\r\n' \
   '      var mouse_out = null;\r\n' \
   '      var pointer_e = null;\r\n' \
+  '      var mouse_ocm = null;\r\n' \
   '      function pointer_down(e) {\r\n' \
   '        pointer_e = e.pointerId;\r\n' \
   '      }\r\n' \
   '      function mouse_down(e) {\r\n' \
   '        if (e.button != 0 && e.button != 2) {return;}\r\n' \
   '        mousex = e.pageX;\r\n' \
   '        mousey = e.pageY;\r\n' \
   '        e.stopPropagation();\r\n' \
   '        e.preventDefault();\r\n' \
   '        document.onmousemove = mouse_move;\r\n' \
   '        document.onmouseup = mouse_up;\r\n' \
-  '        document.oncontextmenu = mouse_click;\r\n' \
+  '        if (e.button == 2) {\r\n' \
+  '          if (mouse_ocm) {clearTimeout(mouse_ocm); mouse_ocm=null;}\r\n' \
+  '          document.oncontextmenu = mouse_click;\r\n' \
+  '        }\r\n' \
   '        scrollmode_ex = scrollmode;\r\n' \
   '        scrollmode = 0;\r\n' \
   '        let elt = e.target;\r\n' \
   '        if (! elt) {return;}\r\n' \
   '        if (e.button == 0) {\r\n' \
   '          if (elt.id == "view") {\r\n' \
   '            hand = elt;\r\n' \
@@ -9177,39 +9187,48 @@
   '            graph_point();\r\n' \
   '          } else {\r\n' \
   '            viewpane.style.cursor = "";\r\n' \
   '            viewpane.releasePointerCapture(pointer_e);\r\n' \
   '          }\r\n' \
   '          hand = null;\r\n' \
   '          pointer_e = null;\r\n' \
+  '          if (e.button == 2) {\r\n' \
+  '            mouse_ocm = setTimeout(function() {if (mouse_ocm) {document.oncontextmenu=null; mouse_ocm=null;};}, 100);\r\n' \
+  '          }\r\n' \
   '          return;\r\n' \
   '        }\r\n' \
   '        let elt = e.target;\r\n' \
-  '        if (! elt) {return;}\r\n' \
+  '        if (! (elt?elt.id:elt)) {\r\n' \
+  '          mouse_ocm = setTimeout(function() {console.log(mouse_ocm);if (mouse_ocm) {document.oncontextmenu=null; mouse_ocm=null;};}, 100);\r\n' \
+  '          return;\r\n' \
+  '        }\r\n' \
   '        if (e.button == 2) {\r\n' \
   '          if (elt.id.indexOf("dot") >= 0) {\r\n' \
   '            let cb = document.getElementById(elt.id.replace("dot", "point"));\r\n' \
   '            cb.checked = ! cb.checked;\r\n' \
   '            point_checkbox(cb);\r\n' \
   '            cb.scrollIntoView({block:"nearest"});\r\n' \
   '          } else if (elt.id.substring(0, 4) == "path") {\r\n' \
   '            let cb = document.getElementById(elt.id.replace("path", "segment"));\r\n' \
   '            cb.checked = ! cb.checked;\r\n' \
   '            segment_checkbox(cb);\r\n' \
   '            cb.scrollIntoView({block:"nearest"});\r\n' \
   '          }\r\n' \
+  '          mouse_ocm = setTimeout(function() {console.log(mouse_ocm);if (mouse_ocm) {document.oncontextmenu=null; mouse_ocm=null;};}, 100);\r\n' \
   '        }\r\n' \
   '      }\r\n' \
   '      function mouse_click(e) {\r\n' \
   '        e.stopPropagation();\r\n' \
   '        e.preventDefault();\r\n' \
   '        document.oncontextmenu = null;\r\n' \
+  '        if (mouse_ocm) {clearTimeout(mouse_ocm); mouse_ocm=null;}\r\n' \
+  '        mouse_ocm = null;\r\n' \
   '        let elt = e.target;\r\n' \
   '        if (! elt) {return;}\r\n' \
-  '        if (elt.id.substring(0, 4) == "path") {\r\n' \
+  '        if (e.button == 0 && elt.id.substring(0, 4) == "path") {\r\n' \
   '          let seg = document.getElementById(elt.id.replace("path", "segment") + "desc");\r\n' \
   '          element_click(null, seg);\r\n' \
   '        }\r\n' \
   '      }\r\n' \
   '      function mouse_outside() {\r\n' \
   '        if (mouse_out == null) {return;}\r\n' \
   '        let dx = 0;\r\n' \
@@ -12430,27 +12449,31 @@
   '      var mousex = null;\r\n' \
   '      var mousey = null;\r\n' \
   '      var viewpane = document.getElementById("view");\r\n' \
   '      var handle = document.getElementById("handle");\r\n' \
   '      var hand = null;\r\n' \
   '      var mouse_out = null;\r\n' \
   '      var pointer_e = null;\r\n' \
+  '      var mouse_ocm = null;\r\n' \
   '      function pointer_down(e) {\r\n' \
   '        pointer_e = e.pointerId;\r\n' \
   '      }\r\n' \
   '      function mouse_down(e) {\r\n' \
   '        if (e.button != 0 && e.button != 2) {return;}\r\n' \
   '        document.getElementById("tracksfilter").blur();\r\n' \
   '        mousex = e.pageX;\r\n' \
   '        mousey = e.pageY;\r\n' \
   '        e.stopPropagation();\r\n' \
   '        e.preventDefault();\r\n' \
   '        document.onmousemove = mouse_move;\r\n' \
   '        document.onmouseup = mouse_up;\r\n' \
-  '        document.oncontextmenu = mouse_click;\r\n' \
+  '        if (e.button == 2) {\r\n' \
+  '          if (mouse_ocm) {clearTimeout(mouse_ocm); mouse_ocm=null;}\r\n' \
+  '          document.oncontextmenu = mouse_click;\r\n' \
+  '        }\r\n' \
   '        scrollmode_ex = scrollmode;\r\n' \
   '        scrollmode = 0;\r\n' \
   '        if (e.target && e.button == 0) {\r\n' \
   '          if (e.target.id == "view") {\r\n' \
   '            hand = e.target;\r\n' \
   '            viewpane.style.cursor = "all-scroll";\r\n' \
   '            viewpane.setPointerCapture(pointer_e);\r\n' \
@@ -12471,25 +12494,29 @@
   '          if (mouse_out != null) {\r\n' \
   '            window.clearInterval(mouse_out);\r\n' \
   '            mouse_out = null;\r\n' \
   '          }\r\n' \
   '          hand = null;\r\n' \
   '          viewpane.style.cursor = "";\r\n' \
   '          viewpane.releasePointerCapture(pointer_e);\r\n' \
+  '          pointer_e = null;\r\n' \
   '          if (media_ex_visible) {\r\n' \
   '            show_media();\r\n' \
   '            media_ex_visible = false;\r\n' \
   '          }\r\n' \
-  '          return;\r\n' \
+  '        }\r\n' \
+  '        if (e.button == 2) {\r\n' \
+  '          mouse_ocm = setTimeout(function() {if (mouse_ocm) {document.oncontextmenu=null; mouse_ocm=null;};}, 100);\r\n' \
   '        }\r\n' \
   '      }\r\n' \
   '      function mouse_click(e) {\r\n' \
   '        e.stopPropagation();\r\n' \
   '        e.preventDefault();\r\n' \
   '        document.oncontextmenu = null;\r\n' \
+  '        if (mouse_ocm) {clearTimeout(mouse_ocm); mouse_ocm=null;}\r\n' \
   '        let elt = e.target;\r\n' \
   '        if (! elt) {return;}\r\n' \
   '        if (e.button == 2) {\r\n' \
   '          if (elt.id.substring(0, 4) == "path") {\r\n' \
   '            let cb = document.getElementById(elt.id.replace("path", "track") + "visible");\r\n' \
   '            cb.checked = false;\r\n' \
   '            track_checkbox(cb);\r\n' \
@@ -13869,20 +13896,21 @@
         del trck.Track
       self.HTML = self.HTMLExp = self.HTML3D = self.HTML3DData = None
     with self.Media.DLock:
       self.Media.Data = None
 
 
 if __name__ == '__main__':
-  print('GPXTweaker v1.9.1 (https://github.com/PCigales/GPXTweaker)    Copyright © 2022 PCigales')
+  print('GPXTweaker v1.9.2 (https://github.com/PCigales/GPXTweaker)    Copyright © 2022 PCigales')
   print(LSTRINGS['parser']['license'])
   print('');
   formatter = lambda prog: argparse.HelpFormatter(prog, max_help_position=50, width=119)
-  CustomArgumentParser = partial(argparse.ArgumentParser, formatter_class=formatter)
+  CustomArgumentParser = partial(argparse.ArgumentParser, formatter_class=formatter, add_help=False)
   parser = CustomArgumentParser()
+  parser.add_argument('--help', '-h', action='help', default=argparse.SUPPRESS, help=LSTRINGS['parser']['help'])
   parser.add_argument('uri', metavar='URI', help=LSTRINGS['parser']['uri'], nargs='?', default=None)
   parser.add_argument('--conf', '-c', metavar='CONF', help=LSTRINGS['parser']['conf'], default='')
   parser.add_argument('--trk', '-t', metavar='TRK', help=LSTRINGS['parser']['trk'], type=int, default=None)
   parser.add_argument('--map', '-m', metavar='MAP', help=LSTRINGS['parser']['map'], nargs ='?', const=' ', default='')
   parser.add_argument('--emap', '-e', metavar='EMAP', help=LSTRINGS['parser']['emap'], nargs ='?', const=' ', default='')
   parser.add_argument('--box', '-b', metavar='BOX', help=LSTRINGS['parser']['box'], type=(lambda b: (list((p,q,r,s) for [p,q,r,s] in (map(float, map(str.strip, b.split(','))),))[0]) if b != '' else (None, ) * 4), default='')
   parser.add_argument('--size', '-s', metavar='SIZE', help=LSTRINGS['parser']['size'], type=(lambda s: (list((p,q) for [p,q] in (map(int, map(str.strip, s.split(','))),))[0]) if s != '' else (None, ) * 2), default='')
```

### Comparing `GPXTweaker-1.9.1/src/GPXTweaker/README.md` & `GPXTweaker-1.9.2/src/GPXTweaker/README.md`

 * *Files identical despite different names*

### Comparing `GPXTweaker-1.9.1/src/GPXTweaker/test.py` & `GPXTweaker-1.9.2/src/GPXTweaker/test.py`

 * *Files identical despite different names*

### Comparing `GPXTweaker-1.9.1/src/GPXTweaker.egg-info/PKG-INFO` & `GPXTweaker-1.9.2/src/GPXTweaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPXTweaker
-Version: 1.9.1
+Version: 1.9.2
 Summary: A script in Python 3 to visualize, in 2D and 3D, and edit GPX tracks
 Home-page: https://github.com/PCigales/GPXTweaker
 Author: PCigales
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/PCigales/GPXTweaker/issues
 Keywords: gpx,gis,wms,wmts,3d,wgs84,mercator,geotag
 Platform: win64
```

