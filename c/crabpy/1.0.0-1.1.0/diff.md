# Comparing `tmp/crabpy-1.0.0.tar.gz` & `tmp/crabpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy-1.0.0.tar", last modified: Thu Apr 13 12:57:59 2023, max compression
+gzip compressed data, was "crabpy-1.1.0.tar", last modified: Wed May  3 12:29:20 2023, max compression
```

## Comparing `crabpy-1.0.0.tar` & `crabpy-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6333 2023-04-13 12:57:29.000000 crabpy-1.0.0/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.0.0/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.0.0/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7984 2023-04-13 12:57:59.740497 crabpy-1.0.0/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.0.0/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/crabpy/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7372 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/client.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/crabpy/data/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   118599 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/data/deelgemeenten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      478 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/data/gewesten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      753 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/data/provincies.json
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/crabpy/gateway/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    31167 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/gateway/exception.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/wsa.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.0.0/crabpy/wsse.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:59.740497 crabpy-1.0.0/crabpy.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7984 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      551 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-04-13 12:57:59.000000 crabpy-1.0.0/crabpy.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-04-13 12:57:59.740497 crabpy-1.0.0/setup.cfg
--rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-04-13 12:57:29.000000 crabpy-1.0.0/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-03 12:29:20.234536 crabpy-1.1.0/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6413 2023-05-03 12:29:06.000000 crabpy-1.1.0/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.1.0/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.1.0/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8064 2023-05-03 12:29:20.234536 crabpy-1.1.0/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.1.0/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-03 12:29:20.234536 crabpy-1.1.0/crabpy/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.1.0/crabpy/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7372 2023-04-13 12:57:29.000000 crabpy-1.1.0/crabpy/client.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-03 12:29:20.234536 crabpy-1.1.0/crabpy/data/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   238209 2023-05-03 12:29:06.000000 crabpy-1.1.0/crabpy/data/deelgemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   167480 2023-05-03 12:29:06.000000 crabpy-1.1.0/crabpy/data/gemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      547 2023-05-03 12:29:06.000000 crabpy-1.1.0/crabpy/data/gewesten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      753 2023-04-13 12:57:29.000000 crabpy-1.1.0/crabpy/data/provincies.json
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-03 12:29:20.234536 crabpy-1.1.0/crabpy/gateway/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.1.0/crabpy/gateway/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    29924 2023-05-03 12:29:06.000000 crabpy-1.1.0/crabpy/gateway/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.1.0/crabpy/gateway/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.1.0/crabpy/gateway/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.1.0/crabpy/gateway/exception.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.1.0/crabpy/wsa.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.1.0/crabpy/wsse.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-03 12:29:20.234536 crabpy-1.1.0/crabpy.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8064 2023-05-03 12:29:20.000000 crabpy-1.1.0/crabpy.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      578 2023-05-03 12:29:20.000000 crabpy-1.1.0/crabpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-03 12:29:20.000000 crabpy-1.1.0/crabpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-05-03 12:29:20.000000 crabpy-1.1.0/crabpy.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.1.0/crabpy.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-05-03 12:29:20.000000 crabpy-1.1.0/crabpy.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-05-03 12:29:20.000000 crabpy-1.1.0/crabpy.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-05-03 12:29:20.234536 crabpy-1.1.0/setup.cfg
+-rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-05-03 12:29:06.000000 crabpy-1.1.0/setup.py
```

### Comparing `crabpy-1.0.0/CHANGES.rst` & `crabpy-1.1.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.1.0 (03-05-2023)
+------------------
+
+- Lijst gemeenten statisch maken (#203)
+
 1.0.0 (13-04-2023)
 ------------------
 
 - Naar v2 van adressenregister (#185)
 - File wordt niet geclosed (#133)
 - black, flake8, python2 weg en pre-commit (#195)
 - Uitbreidingen aan adressenregister model (#192)
```

### Comparing `crabpy-1.0.0/LICENSE` & `crabpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy-1.0.0/PKG-INFO` & `crabpy-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.1.0 (03-05-2023)
+------------------
+
+- Lijst gemeenten statisch maken (#203)
+
 1.0.0 (13-04-2023)
 ------------------
 
 - Naar v2 van adressenregister (#185)
 - File wordt niet geclosed (#133)
 - black, flake8, python2 weg en pre-commit (#195)
 - Uitbreidingen aan adressenregister model (#192)
```

### Comparing `crabpy-1.0.0/README.rst` & `crabpy-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy-1.0.0/crabpy/client.py` & `crabpy-1.1.0/crabpy/client.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.0.0/crabpy/data/provincies.json` & `crabpy-1.1.0/crabpy/data/provincies.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.0.0/crabpy/gateway/adressenregister.py` & `crabpy-1.1.0/crabpy/gateway/adressenregister.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,18 +115,27 @@
             return Deelgemeente(
                 id_=data["id"],
                 naam=data["naam"],
                 gemeente_niscode=data["gemeente_niscode"],
                 gateway=self,
             )
 
+        def gemeente_from_json_data(data):
+            return Gemeente(
+                niscode=data["niscode"],
+                provincie_niscode=data["provincie"],
+                namen=data["namen"],
+                gateway=self,
+            )
+
         def gewest_from_json_data(data):
             return Gewest(
                 id_=data["id"],
                 naam=data["naam"],
+                niscode=data["niscode"],
                 centroid=data["centroid"],
                 bounding_box=data["bounding_box"],
                 gateway=self,
             )
 
         def provincie_from_json_data(data):
             return Provincie(
@@ -139,14 +148,16 @@
         data_dir = os.path.join(os.path.dirname(__file__), "..", "data")
         with open(os.path.join(data_dir, "deelgemeenten.json"), encoding="utf-8") as f:
             self.deelgemeenten = json.load(f, object_hook=deelgemeente_from_json_data)
         with open(os.path.join(data_dir, "gewesten.json"), encoding="utf-8") as f:
             self.gewesten = json.load(f, object_hook=gewest_from_json_data)
         with open(os.path.join(data_dir, "provincies.json"), encoding="utf-8") as f:
             self.provincies = json.load(f, object_hook=provincie_from_json_data)
+        with open(os.path.join(data_dir, "gemeenten.json"), encoding="utf-8") as f:
+            self.gemeenten = [gemeente_from_json_data(data) for data in json.load(f)]
 
         setup_cache(cache_settings)
 
     def list_gewesten(self):
         return self.gewesten
 
     def get_gewest_by_id(self, id_):
@@ -180,71 +191,68 @@
         """
         niscode = str(niscode)
         for provincie in self.provincies:
             if provincie.niscode == niscode:
                 return provincie
         return None
 
-    @LONG_CACHE.cache_on_arguments()
     def list_gemeenten_by_provincie(self, provincie):
         """
         List all `gemeenten` in a `provincie`.
 
         :param provincie: The :class:`Provincie` for which the \
             `gemeenten` are wanted.
         :rtype: A :class:`list` of :class:`Gemeente`.
         """
         if not isinstance(provincie, Provincie):
             provincie = self.get_provincie_by_id(provincie)
-        first_niscode_digit = str(provincie.niscode)[0]
+        provincie_niscode = str(provincie.niscode)
         return [
-            Gemeente.from_list_response(gemeente, self)
-            for gemeente in self.client.get_gemeenten()
-            if gemeente["identificator"]["objectId"][0] == first_niscode_digit
+            gemeente
+            for gemeente in self.gemeenten
+            if gemeente.provincie_niscode == provincie_niscode
         ]
 
-    @LONG_CACHE.cache_on_arguments()
     def list_gemeenten(self, gewest=2):
         """
         List all `gemeenten` in a `gewest`.
 
         :param gewest: The :class:`Gewest` for which the \
             `gemeenten` are wanted.
         :rtype: A :class:`list` of :class:`Gemeente`.
         """
-        first_niscode_digits = [
-            provincie.niscode[0]
+        # Brussel is a special case, because it has no provinces
+        if str(gewest) == "1":
+            return [
+                gemeente
+                for gemeente in self.gemeenten
+                if gemeente.niscode.startswith("21")
+            ]
+        provincie_niscodes = [
+            provincie.niscode
             for provincie in self.list_provincies(gewest=gewest)
-            if provincie.gewest == gewest or gewest is None
+            if provincie.gewest == gewest
         ]
         return [
-            Gemeente.from_list_response(gemeente, self)
-            for gemeente in self.client.get_gemeenten()
-            if gemeente["identificator"]["objectId"][0] in first_niscode_digits
+            gemeente
+            for gemeente in self.gemeenten
+            if gemeente.provincie_niscode in provincie_niscodes
         ]
 
-    @LONG_CACHE.cache_on_arguments()
-    def get_gemeente_by_id(self, gemeente_id):
-        """
-        Retrieve a `gemeente` by the crab id.
-
-        :param integer gemeente_id: The niscode of the gemeente.
-        :rtype: :class:`Gemeente`
-        """
-        return Gemeente.from_get_response(self.client.get_gemeente(gemeente_id), self)
-
-    @LONG_CACHE.cache_on_arguments()
     def get_gemeente_by_niscode(self, niscode):
         """
         Retrieve a `gemeente` by the NIScode.
 
         :param integer niscode: The NIScode of the gemeente.
         :rtype: :class:`Gemeente`
         """
-        return Gemeente.from_get_response(self.client.get_gemeente(niscode), self)
+        return next(
+            (gemeente for gemeente in self.gemeenten if gemeente.niscode == str(niscode)),
+            None,
+        )
 
     @LONG_CACHE.cache_on_arguments()
     def get_postinfo_by_gemeentenaam(self, gemeente_naam):
         """
         Retrieve a `postinfo` by gemeentenaam.
 
         :param string gemeente_naam: The name of the municipality.
@@ -261,15 +269,14 @@
         Retrieve a `postinfo` by crab id.
 
         :param integer gemeente_id: The crab id of the municipality.
         :rtype: :class:`Postinfo`
         """
         return Postinfo.from_get_response(self.client.get_postinfo(postcode), self)
 
-    @LONG_CACHE.cache_on_arguments()
     def list_deelgemeenten(self, gewest=2):
         """
         List all `deelgemeenten` in a `gewest`.
 
         :param gewest: The :class:`Gewest` for which the \
             `deelgemeenten` are wanted. Currently only Flanders is supported.
         :rtype: A :class:`list` of :class:`Deelgemeente`.
@@ -281,15 +288,14 @@
         ]
         return [
             deelgemeente
             for deelgemeente in self.deelgemeenten
             if deelgemeente.id[0] in first_niscode_digits
         ]
 
-    @LONG_CACHE.cache_on_arguments()
     def list_deelgemeenten_by_gemeente(self, gemeente):
         """
         List all `deelgemeenten` in a `gemeente`.
 
         :param gemeente: The :class:`Gemeente` for which the \
             `deelgemeenten` are wanted. Currently only Flanders is supported.
         :rtype: A :class:`list` of :class:`Deelgemeente`.
@@ -298,15 +304,14 @@
             gemeente = self.get_gemeente_by_niscode(gemeente)
         return [
             deelgemeente
             for deelgemeente in self.deelgemeenten
             if deelgemeente.gemeente_niscode == gemeente.niscode
         ]
 
-    @LONG_CACHE.cache_on_arguments()
     def get_deelgemeente_by_id(self, deelgemeente_id):
         """
         Retrieve a `deelgemeente` by the id.
 
         :param string deelgemeente_id: The id of the deelgemeente.
         :rtype: :class:`Deelgemeente`
         """
@@ -478,18 +483,19 @@
     """
     A large administrative unit in Belgium.
 
     Belgium consists of 3 `gewesten`. Together they form the entire territory
     of the country.
     """
 
-    def __init__(self, id_, naam, centroid, bounding_box, gateway=None):
+    def __init__(self, id_, niscode, naam, centroid, bounding_box, gateway=None):
         super().__init__(gateway=gateway)
         self.id = int(id_)
         self.naam = naam
+        self.niscode = niscode
         self.centroid = centroid
         self.bounding_box = bounding_box
 
     @LazyProperty
     def provincies(self):
         return self.gateway.list_provincies(gewest=self.id)
 
@@ -532,92 +538,51 @@
 
 
 class Gemeente(GatewayObject):
     """
     The smallest administrative unit in Belgium.
     """
 
-    def __init__(self, niscode, gateway, naam=AUTO, taal=AUTO, status=AUTO, uri=AUTO):
+    def __init__(self, niscode, gateway, provincie_niscode=None, namen=None, naam=None):
         super().__init__(gateway)
         self.niscode = niscode
-        if naam is not AUTO:
+        self.provincie_niscode = provincie_niscode
+        if not (namen or naam):
+            raise ValueError("Either namen or naam must be given")
+        if namen is not None:
+            self.namen = namen
+        if naam is not None:
             if isinstance(naam, str):
                 naam = CallableString(naam)
             if not callable(naam):
                 raise ValueError("naam must be a callable")
             self.naam = naam
-        if taal is not AUTO:
-            self.taal = taal
-        if status is not AUTO:
-            self.status = status
-        if uri is not AUTO:
-            self.uri = uri
-
-    @classmethod
-    def from_list_response(cls, gemeente, gateway):
-        return Gemeente(
-            naam=gemeente["gemeentenaam"]["geografischeNaam"]["spelling"],
-            niscode=gemeente["identificator"]["objectId"],
-            status=gemeente["gemeenteStatus"],
-            uri=gemeente["identificator"]["id"],
-            gateway=gateway,
-        )
-
-    @classmethod
-    def from_get_response(cls, gemeente, gateway):
-        res = Gemeente(niscode=gemeente["identificator"]["objectId"], gateway=gateway)
-        res._source_json = gemeente
-        return res
-
-    @LazyProperty
-    def uri(self):
-        return self._source_json["identificator"]["id"]
-
-    @LazyProperty
-    def taal(self):
-        return self._source_json["officieleTalen"][0]
 
     def naam(self, taal="nl"):
-        for _taal in [taal, self.taal]:
-            naam = next(
-                (
-                    gemeentenaam["spelling"]
-                    for gemeentenaam in self._source_json["gemeentenamen"]
-                    if gemeentenaam["taal"] == _taal
-                ),
-                None,
-            )
-            if naam:
-                return naam
-
-        return self._source_json["gemeentenamen"][0]["spelling"]
-
-    @LazyProperty
-    def status(self):
-        return self._source_json["gemeenteStatus"]
+        return next(
+            (naam["naam"] for naam in self.namen if naam["taal"] == taal),
+            self.namen[0]["naam"],
+        )
 
     @LazyProperty
     def straten(self):
         return self.gateway.list_straten(self)
 
     @LazyProperty
     def postinfo(self):
         gemeente_naam = self.naam() if not isinstance(self.naam, str) else self.naam
         return self.gateway.get_postinfo_by_gemeentenaam(gemeente_naam)
 
     @LazyProperty
     def provincie(self):
-        for p in self.gateway.provincies:
-            if self.niscode[0] == p.niscode[0]:
-                return p
+        return self.gateway.get_provincie_by_id(self.provincie_niscode)
 
     @LazyProperty
-    @SHORT_CACHE.cache_on_arguments(function_key_generator=cache_on_attribute("niscode"))
-    def _source_json(self):
-        return self.gateway.client.get_gemeente(self.niscode)
+    def gewest(self):
+        return self.gateway.get_gewest_by_id(self.provincie.gewest)
 
     def __str__(self):
         return f"{self.naam} ({self.niscode})"
 
     def __repr__(self):
         return f"Gemeente(niscode={self.niscode})"
 
@@ -633,15 +598,15 @@
         super().__init__(gateway)
         self.id = id_
         self.naam = naam
         self.gemeente_niscode = gemeente_niscode
 
     @LazyProperty
     def gemeente(self):
-        return Gemeente(niscode=self.gemeente_niscode, gateway=self.gateway)
+        return self.gateway.get_gemeente_by_niscode(self.gemeente_niscode)
 
     def __str__(self):
         return f"{self.naam} ({self.id})"
 
     def __repr__(self):
         return f"Deelgemeente(id={self.id}"
 
@@ -705,17 +670,16 @@
 
     @LazyProperty
     def status(self):
         return self._source_json["straatnaamStatus"]
 
     @LazyProperty
     def gemeente(self):
-        return Gemeente(
-            niscode=self._source_json["gemeente"]["objectId"], gateway=self.gateway
-        )
+        gemeente_niscode = self._source_json["gemeente"]["objectId"]
+        return self.gateway.get_gemeente_by_niscode(gemeente_niscode)
 
     @LazyProperty
     def adressen(self):
         return self.gateway.list_adressen_by_straat(self)
 
     @LazyProperty
     @SHORT_CACHE.cache_on_arguments(function_key_generator=cache_on_attribute("id"))
@@ -823,17 +787,16 @@
 
     @LazyProperty
     def busnummer(self):
         return self._source_json.get("busnummer", "")
 
     @LazyProperty
     def gemeente(self):
-        return Gemeente(
-            niscode=self._source_json["gemeente"]["objectId"], gateway=self.gateway
-        )
+        gemeente_niscode = self._source_json["gemeente"]["objectId"]
+        return self.gateway.get_gemeente_by_niscode(gemeente_niscode)
 
     @LazyProperty
     @SHORT_CACHE.cache_on_arguments(function_key_generator=cache_on_attribute("id"))
     def _source_json(self):
         return self.gateway.client.get_adres(self.id)
 
     def __str__(self):
@@ -994,21 +957,16 @@
 
     @LazyProperty
     def status(self):
         return self._source_json["postInfoStatus"]
 
     @LazyProperty
     def gemeente(self):
-        return Gemeente(
-            niscode=self._source_json["gemeente"]["objectId"],
-            gateway=self.gateway,
-            naam=self._source_json["gemeente"]["gemeentenaam"]["geografischeNaam"][
-                "spelling"
-            ],
-        )
+        niscode = self._source_json["gemeente"]["objectId"]
+        return self.gateway.get_gemeente_by_niscode(niscode)
 
     def namen(self, taal="nl"):
         namen = [
             postnaam["geografischeNaam"]["spelling"]
             for postnaam in self._source_json["postnamen"]
             if postnaam["geografischeNaam"]["taal"] == taal
         ]
```

### Comparing `crabpy-1.0.0/crabpy/gateway/capakey.py` & `crabpy-1.1.0/crabpy/gateway/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.0.0/crabpy/gateway/crab.py` & `crabpy-1.1.0/crabpy/gateway/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.0.0/crabpy/gateway/exception.py` & `crabpy-1.1.0/crabpy/gateway/exception.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.0.0/crabpy/wsa.py` & `crabpy-1.1.0/crabpy/wsa.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.0.0/crabpy/wsse.py` & `crabpy-1.1.0/crabpy/wsse.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.0.0/crabpy.egg-info/PKG-INFO` & `crabpy-1.1.0/crabpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.1.0 (03-05-2023)
+------------------
+
+- Lijst gemeenten statisch maken (#203)
+
 1.0.0 (13-04-2023)
 ------------------
 
 - Naar v2 van adressenregister (#185)
 - File wordt niet geclosed (#133)
 - black, flake8, python2 weg en pre-commit (#195)
 - Uitbreidingen aan adressenregister model (#192)
```

### Comparing `crabpy-1.0.0/crabpy.egg-info/SOURCES.txt` & `crabpy-1.1.0/crabpy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 crabpy.egg-info/SOURCES.txt
 crabpy.egg-info/dependency_links.txt
 crabpy.egg-info/entry_points.txt
 crabpy.egg-info/not-zip-safe
 crabpy.egg-info/requires.txt
 crabpy.egg-info/top_level.txt
 crabpy/data/deelgemeenten.json
+crabpy/data/gemeenten.json
 crabpy/data/gewesten.json
 crabpy/data/provincies.json
 crabpy/gateway/__init__.py
 crabpy/gateway/adressenregister.py
 crabpy/gateway/capakey.py
 crabpy/gateway/crab.py
 crabpy/gateway/exception.py
```

### Comparing `crabpy-1.0.0/setup.py` & `crabpy-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "crabpy",
 ]
 
 requires = ["suds-py3>=1.4.4.1", "dogpile.cache", "requests"]
 
 setup(
     name="crabpy",
-    version="1.0.0",
+    version="1.1.0",
     description="Interact with geographical webservices by Informatie Vlaanderen.",
     long_description=open("README.rst").read() + "\n\n" + open("CHANGES.rst").read(),
     author="Onroerend Erfgoed",
     author_email="ict@onroerenderfgoed.be",
     url="http://github.com/onroerenderfgoed/crabpy",
     packages=find_packages(exclude=["tests*"]),
     package_data={"": ["LICENSE"]},
```

