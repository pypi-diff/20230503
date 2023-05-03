# Comparing `tmp/tflwrapper-1.1.7.tar.gz` & `tmp/tflwrapper-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tflwrapper-1.1.7.tar", last modified: Mon Apr 11 17:48:25 2022, max compression
+gzip compressed data, was "tflwrapper-1.1.8.tar", last modified: Wed May  3 16:52:48 2023, max compression
```

## Comparing `tflwrapper-1.1.7.tar` & `tflwrapper-1.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-04-11 17:48:25.753705 tflwrapper-1.1.7/
--rw-rw-rw-   0        0        0     1100 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     1768 2022-04-11 17:48:25.752731 tflwrapper-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1419 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/README.md
--rw-rw-rw-   0        0        0       42 2022-04-11 17:48:25.753705 tflwrapper-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      583 2022-04-11 17:48:04.000000 tflwrapper-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-11 17:48:25.739060 tflwrapper-1.1.7/tflwrapper/
--rw-rw-rw-   0        0        0      663 2022-04-11 17:47:46.000000 tflwrapper-1.1.7/tflwrapper/__init__.py
--rw-rw-rw-   0        0        0      431 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/accidentStats.py
--rw-rw-rw-   0        0        0      322 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/airQuality.py
--rw-rw-rw-   0        0        0      658 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/bikePoint.py
--rw-rw-rw-   0        0        0     1069 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/crowding.py
--rw-rw-rw-   0        0        0      343 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/disruptions.py
--rw-rw-rw-   0        0        0     5682 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/line.py
--rw-rw-rw-   0        0        0      732 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/mode.py
--rw-rw-rw-   0        0        0     1518 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/occupancy.py
--rw-rw-rw-   0        0        0     2534 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/road.py
--rw-rw-rw-   0        0        0     8848 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/stopPoint.py
--rw-rw-rw-   0        0        0     1867 2022-04-11 17:40:46.000000 tflwrapper-1.1.7/tflwrapper/tfl.py
--rw-rw-rw-   0        0        0     1630 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/trackerNet.py
--rw-rw-rw-   0        0        0     1274 2022-03-01 22:46:06.000000 tflwrapper-1.1.7/tflwrapper/travelTimes.py
-drwxrwxrwx   0        0        0        0 2022-04-11 17:48:25.751756 tflwrapper-1.1.7/tflwrapper.egg-info/
--rw-rw-rw-   0        0        0     1768 2022-04-11 17:48:25.000000 tflwrapper-1.1.7/tflwrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2022-04-11 17:48:25.000000 tflwrapper-1.1.7/tflwrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-11 17:48:25.000000 tflwrapper-1.1.7/tflwrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-04-11 17:48:25.000000 tflwrapper-1.1.7/tflwrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-04-11 17:48:25.000000 tflwrapper-1.1.7/tflwrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 16:52:48.276549 tflwrapper-1.1.8/
+-rw-rw-rw-   0        0        0     1100 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1745 2023-05-03 16:52:48.275553 tflwrapper-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1419 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 16:52:48.276549 tflwrapper-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-05-03 16:49:36.000000 tflwrapper-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:52:48.268063 tflwrapper-1.1.8/tflwrapper/
+-rw-rw-rw-   0        0        0      663 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/__init__.py
+-rw-rw-rw-   0        0        0      505 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/accidentStats.py
+-rw-rw-rw-   0        0        0      318 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/airQuality.py
+-rw-rw-rw-   0        0        0      812 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/bikePoint.py
+-rw-rw-rw-   0        0        0     1090 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/crowding.py
+-rw-rw-rw-   0        0        0      339 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/disruptions.py
+-rw-rw-rw-   0        0        0     6410 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/line.py
+-rw-rw-rw-   0        0        0      758 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/mode.py
+-rw-rw-rw-   0        0        0     1553 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/occupancy.py
+-rw-rw-rw-   0        0        0     2570 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/road.py
+-rw-rw-rw-   0        0        0     9358 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/stopPoint.py
+-rw-rw-rw-   0        0        0     2105 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/tfl.py
+-rw-rw-rw-   0        0        0     1915 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/trackerNet.py
+-rw-rw-rw-   0        0        0     1282 2023-05-03 16:43:06.000000 tflwrapper-1.1.8/tflwrapper/travelTimes.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:52:48.274550 tflwrapper-1.1.8/tflwrapper.egg-info/
+-rw-rw-rw-   0        0        0     1745 2023-05-03 16:52:48.000000 tflwrapper-1.1.8/tflwrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-03 16:52:48.000000 tflwrapper-1.1.8/tflwrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 16:52:48.000000 tflwrapper-1.1.8/tflwrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 16:52:48.000000 tflwrapper-1.1.8/tflwrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 16:52:48.000000 tflwrapper-1.1.8/tflwrapper.egg-info/top_level.txt
```

### Comparing `tflwrapper-1.1.7/LICENSE` & `tflwrapper-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tflwrapper-1.1.7/PKG-INFO` & `tflwrapper-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tflwrapper
-Version: 1.1.7
+Version: 1.1.8
 Summary: A wrapper for the Transport for London Unified API and TrackerNet
 Home-page: https://github.com/you/tfl-api-wrapper-py
 Author: zackaryh8
 Author-email: zackary12389@yahoo.co.uk
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img width="200" src="https://blog.tfl.gov.uk/wp-content/uploads/2018/05/cropped-logo_roundel-2.png" alt="TfL Logo">
     <h1 align="center">TfL API Wrapper</h1>
     <p align="center">An API wrapper for the TfL Unified API, made with Python.</p>
@@ -47,9 +46,7 @@
 
 print(arrivals)
 ```
 
 ## Disclaimer
 
 This repository is not affiliated, associated, authorized, endorsed by, or in any way officially connected with Transport for London (TfL) or it's parent organisation Greater London Authority (GLA)
-
-
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: tflwrapper Version: 1.1.7 Summary: A wrapper for
+Metadata-Version: 2.1 Name: tflwrapper Version: 1.1.8 Summary: A wrapper for
 the Transport for London Unified API and TrackerNet Home-page: https://
 github.com/you/tfl-api-wrapper-py Author: zackaryh8 Author-email:
-zackary12389@yahoo.co.uk License: MIT Platform: UNKNOWN Description-Content-
-Type: text/markdown License-File: LICENSE
+zackary12389@yahoo.co.uk License: MIT Description-Content-Type: text/markdown
+License-File: LICENSE
                                   [TfL Logo]
                          ****** TfL API Wrapper ******
            An API wrapper for the TfL Unified API, made with Python.
                             Read the Documentation
 [![Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg)](https://github.com/psf/black) [![](https://img.shields.io/github/
 issues/ZackaryH8/tfl-api-wrapper-py)](https://github.com/ZackaryH8/tfl-api-
```

### Comparing `tflwrapper-1.1.7/README.md` & `tflwrapper-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tflwrapper-1.1.7/setup.py` & `tflwrapper-1.1.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
 setup(
     name="tflwrapper",
-    version="1.1.7",
+    version="1.1.8",
     description="A wrapper for the Transport for London Unified API and TrackerNet",
     long_description=(HERE / "README.md").read_text(),
     long_description_content_type="text/markdown",
     author="zackaryh8",
     license="MIT",
     author_email="zackary12389@yahoo.co.uk",
     url="https://github.com/you/tfl-api-wrapper-py",
```

### Comparing `tflwrapper-1.1.7/tflwrapper/__init__.py` & `tflwrapper-1.1.8/tflwrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `tflwrapper-1.1.7/tflwrapper/bikePoint.py` & `tflwrapper-1.1.8/tflwrapper/bikePoint.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,31 @@
 
 class bikePoint(tflAPI):
     """Bike point from Unified API"""
 
     def getAll(self):
         """Gets all bike point locations"""
         return super(bikePoint, self).sendRequestUnified(
-            "/BikePoint", {}
+            "/BikePoint"
         )
 
     def getByID(self, ID):
-        """Gets the bike point by the given id"""
+        """
+        Gets the bike point by the given id
+
+        Args:
+            ID: The ID of the bike point
+        """
         return super(bikePoint, self).sendRequestUnified(
-            f"/BikePoint/{ID}", {}
+            f"/BikePoint/{ID}"
         )
 
     def getByName(self, name):
-        """Search for bike points by their name"""
+        """
+        Search for bike points by their name
+
+        Args:
+            name: The name of the bike point
+        """
         return super(bikePoint, self).sendRequestUnified(
             f"/BikePoint/Search", {'query': name}
         )
```

### Comparing `tflwrapper-1.1.7/tflwrapper/crowding.py` & `tflwrapper-1.1.8/tflwrapper/crowding.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,31 +3,37 @@
 
 class crowding(tflAPI):
     """Crowding from Unified API"""
 
     def getAllByNaptan(self, id):
         """
         Get crowding information for Naptan
-        :param id: naptanID ID of the stop (eg. 940GZZLUASL)
+
+        Args:
+            id: NaPTAN ID of the stop (eg. 940GZZLUASL)
         """
         return super(crowding, self).sendRequestUnified(
-            f"/Crowding/{id}", {}
+            f"/Crowding/{id}"
         )
 
     def getByNaptanDay(self, id, day):
         """
         Get crowding information for Naptan for a specified day of week
-        :param id: naptanID ID of the stop (eg. 940GZZLUASL)
-        :param day: The day of which you would like data to return (eg. MON, TUE)
+
+        Args:
+            id: NaPTAN ID of the stop (eg. 940GZZLUASL)
+            day: The day of which you would like data to return (eg. MON, TUE)
         """
         return super(crowding, self).sendRequestUnified(
-            f"/Crowding/{id}/{day}", {}
+            f"/Crowding/{id}/{day}"
         )
 
     def getLiveByNaptan(self, id):
         """
         Get crowding information for Naptan for a specified day of week
-        :param id: naptanID ID of the stop (eg. 940GZZLUASL)
+
+        Args:
+            id: NaPTAN ID of the stop (eg. 940GZZLUASL)
         """
         return super(crowding, self).sendRequestUnified(
-            f"/Crowding/{id}/Live", {}
+            f"/Crowding/{id}/Live"
         )
```

### Comparing `tflwrapper-1.1.7/tflwrapper/mode.py` & `tflwrapper-1.1.8/tflwrapper/mode.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 class mode(tflAPI):
     """Mode API, /mode"""
 
     def getActiveServiceTypes(self):
         """Returns the service type active for a mode, currently only supports tube"""
 
         return super(mode, self).sendRequestUnified(
-            "/Mode/ActiveServiceTypes", {}
+            "/Mode/ActiveServiceTypes"
         )
 
     def getAllArrivalPredictions(self, modes: str, count: str):
         """
         Returns arrival predictions for all stops
 
-        :param modes: A mode name e.g. tube, dlr
-        :param count: A number of arrivals to return for each stop, -1 to return all available
+        Args:
+            modes: The modes for which to return predictions e.g. tube, dlr
+            count: The number of predictions to return, -1 to return all available
         """
 
         return super(mode, self).sendRequestUnified(
             f"/Mode/{modes}/Arrivals", {'count': count}
         )
```

### Comparing `tflwrapper-1.1.7/tflwrapper/occupancy.py` & `tflwrapper-1.1.8/tflwrapper/occupancy.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,48 +4,51 @@
 class occupancy(tflAPI):
     """Occupancy from Unified API"""
 
     def getBikePointByIDs(self, ids):
         """
         Gets the occupancy data for bike points
 
-        :param ids: Bike Point ID (Eg. BikePoints_208)
+        Args:
+            ids: List of bike point IDs (Eg. ['BikePoints_208', 'BikePoints_209'])
         """
         return super(occupancy, self).sendRequestUnified(
-            f"/Occupancy/BikePoints/{self.arrayToCSV(ids)}", {}
+            f"/Occupancy/BikePoints/{self.arrayToCSV(ids)}"
         )
 
     def getCarParkByID(self, id):
         """
         Gets the occupancy for a car park with a given id
-        
-        :param id: Car Park ID (Eg. CarParks_800468)
+
+        Args:
+            id: Car park ID (Eg. 'CarParks_800468')
         """
         
         return super(occupancy, self).sendRequestUnified(
-            f"/Occupancy/CarPark/{id}", {}
+            f"/Occupancy/CarPark/{id}"
         )
 
     def getChargeConnectorByID(self, id):
         """
         Gets the occupancy for a charge connectors with a given id
-        
-        :param id: Charge Connector ID (Eg. ChargePointESB-UT06NW-1)
+
+        Args:
+            id: Charge connector ID (Eg. 'ChargePointESB-UT06NW-1')
         """
         
         return super(occupancy, self).sendRequestUnified(
-            f"/Occupancy/ChargeConnector/{id}", {}
+            f"/Occupancy/ChargeConnector/{id}"
         )
 
     def getAllCarParks(self):
         """Gets the occupancy for all car parks that have occupancy data"""
         
         return super(occupancy, self).sendRequestUnified(
-            f"/Occupancy/CarPark", {}
+            f"/Occupancy/CarPark"
         )
 
     def getAllChargeConnectors(self):
         """Gets the occupancy for all charge connectors"""
         
         return super(occupancy, self).sendRequestUnified(
-            f"/Occupancy/ChargeConnector", {}
+            f"/Occupancy/ChargeConnector"
         )
```

### Comparing `tflwrapper-1.1.7/tflwrapper/road.py` & `tflwrapper-1.1.8/tflwrapper/road.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,59 +20,61 @@
             {}
         )
 
     def getAll(self):
         """Get all roads managed by TfL"""
 
         return super(road, self).sendRequestUnified(
-            '/Road', {}
+            '/Road'
         )
 
     def getByID(self, ids):
         """
         Get the road with the specified ID (Eg. A1)
-
-        :param ids: ID(s) of the road(s). Eg. ['A1']
+        Args:
+            ids: ID(s) of the road(s). Eg. ['A1']
         """
 
         return super(road, self).sendRequestUnified(
-            f'/Road/{self.arrayToCSV(ids)}', {}
+            f'/Road/{self.arrayToCSV(ids)}'
         )
 
     def getStatusByID(self, ids, startDate, endDate):
         """
         Gets the specified roads with the status aggregated over the date range specified, or now until the end of today if no dates are passed.
-
-        :param ids: ID(s) of the road(s). Eg. ['A1']
-        :param startDate:
-        :param endDate:
+        Args:
+            ids: ID(s) of the road(s). Eg. ['A1']
+            startDate: Optional, the start time to filter on
+            endDate: Optional, the end time to filter on
         """
 
         return super(road, self).sendRequestUnified(
             f'/Road/{self.arrayToCSV(ids)}', {'startDate': self.getRFC3339(
                 startDate), 'endDate': self.getRFC3339(endDate)}
         )
 
     def getAllStreetDisruption(self, startDate, endDate):
         """
         Gets a list of disrupted streets
 
-        :param startDate: Optional, the start time to filter on
-        :param endDate: Optional, the end time to filter on
+        Args:
+            startDate: Optional, the start time to filter on
+            endDate: Optional, the end time to filter on
         """
         return super(road, self).sendRequestUnified(
             '/Road/all/Street/Disruption',
             {'startDate': self.getRFC3339(
                 startDate), 'endDate': self.getRFC3339(endDate)}
         )
 
-    def getAllDisruptionsByID(self, ids, stripContent: bool):
+    def getAllDisruptionsByID(self, ids, stripContent: bool = False):
         """
         Gets a list of disrupted streets
 
-        :param ids: ID(s) of the road(s). Eg. ['A1']
-        :param stripContent: When true, removes every property/node except for id, point, severity, severityDescription,  startDate, endDate, corridor details, location and comments.
+        Args:
+            ids: ID(s) of the road(s). Eg. ['A1']
+            stripContent: Optional, if true, the content of the disruption will be stripped from the response
         """
         return super(road, self).sendRequestUnified(
             f'/Road/all/Disruption/{self.arrayToCSV(ids)}',
             {'stripContent': stripContent}
         )
```

### Comparing `tflwrapper-1.1.7/tflwrapper/stopPoint.py` & `tflwrapper-1.1.8/tflwrapper/stopPoint.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,159 +3,168 @@
 
 class stopPoint(tflAPI):
     """Stop Point from Unified API"""
 
     def getCategories(self):
         """Gets the list of available StopPoint additional information categories"""
         return super(stopPoint, self).sendRequestUnified(
-            "/StopPoint/Meta/Categories", {}
+            "/StopPoint/Meta/Categories"
         )
 
     def getTypes(self):
         """Gets the list of available StopPoint types"""
 
         return super(stopPoint, self).sendRequestUnified(
-            "/StopPoint/Meta/StopTypes", {}
+            "/StopPoint/Meta/StopTypes"
         )
 
     def getModes(self):
         """Gets the list of available StopPoint modes"""
 
         return super(stopPoint, self).sendRequestUnified(
-            "/StopPoint/Meta/Modes", {}
+            "/StopPoint/Meta/Modes"
         )
 
     def getByIDs(self, ids, includeCrowdingData: bool):
         """
         Gets a list of StopPoints corresponding to the given list of stop ids
 
-        :param ids: A list of stop point ids (station naptan code e.g. 940GZZLUASL).
-        :param includeCrowdingData: Include the crowding data (static). To Filter further use: /StopPoint/{ids}/Crowding/{line}
+        Args:
+            ids: A list of StopPoint ids (station naptan code e.g. 940GZZLUAS)
+            includeCrowdingData: Specify true to return crowding data (static) for each stop point
         """
 
         return super(stopPoint, self).sendRequestUnified(
-            f"/StopPoint/{','.join(ids)}", {includeCrowdingData}
+            f"/StopPoint/{','.join(ids)}", {'includeCrowdingData': includeCrowdingData}
         )
 
     def getAllByStopType(self, array):
         """
         Gets all stop points of a given type
 
-        :param array: A list of valid stop types can be obtained from the StopPoint/meta/stoptypes endpoint
+        Args:
+            array: An array of stop point types e.g. ['NaptanPublicBusCoachTram']
         """
 
         return super(stopPoint, self).sendRequestUnified(
-            f"/StopPoint/{super(stopPoint, self).arrayToCSV(array)}", {}
+            f"/StopPoint/{super(stopPoint, self).arrayToCSV(array)}"
         )
 
     def getServiceTypesByID(self, stopPointID: str, lineIds, modes):
         """
         Gets the service types for a given Stop Point
 
-        :param stopPointID:
-        :param lineIds:
-        :param modes:
+        Args:
+            stopPointID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
+            lineIds: A list of Line ids (e.g. victoria)
+            modes: An array of modes e.g. ['tube', 'dlr']
         """
 
         return super(stopPoint, self).sendRequestUnified(
             f"/StopPoint/ServiceTypes",
             {"id": stopPointID, "lineIds": lineIds, "modes": modes},
         )
 
     def search(self, name: str, modes):
         """
         Search StopPoints by their common name. Will not return a valid NaPTAN for HUB
 
-        :param name: Name of station
-        :param modes: Eg. ['tflwrapper', 'dlr']
+        Args:
+            name: The name of station to search for
+            modes: An array of modes e.g. ['tube', 'dlr']
         """
 
         return super(stopPoint, self).sendRequestUnified(
             f"/StopPoint/Search/${name}",
             {"modes": super(stopPoint, self).arrayToCSV(modes)},
         )
 
     def getStationArrivals(self, naptanID: str):
         """
         Get all service arrivals
 
-        :param naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
+        Args:
+            naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
         """
 
         return super(stopPoint, self).sendRequestUnified(
-            f"/StopPoint/{naptanID}/Arrivals", {}
+            f"/StopPoint/{naptanID}/Arrivals"
         )
 
     # def getArrivalsDepartures(self, naptanID: str, lineIds):
     #     """
     #     Get all service arrivals and departures
 
     #     :param naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
     #     :param lineIds: List of line ids e.g. ['tflwrapper-rail', 'london-overground', 'thameslink']
     #     """
 
     #     return super(stopPoint, self).sendRequestUnified(
-    #         f"StopPoint/${naptanID}/ArrivalsDepartures", {lineIds}
+    #         f"StopPoint/${naptanID}/ArrivalsDepartures", {'lineIds': lineIds}
     #     )
 
     def getDisruptionsByID(
         self,
         ids,
         getFamily: bool,
         includeRouteBlockedStops: bool,
         flattenResponse: bool,
     ):
         """
         Gets all disruptions for the specified StopPointId, plus disruptions for any child Naptan records it may have
 
-        :param ids: A list of StopPoint ids (station naptan code e.g. 940GZZLUAS)
-        :param getFamily: Specify true to return disruptions for entire family, or false to return disruptions for just this stop point. Defaults to false.
-        :param includeRouteBlockedStops:
-        :param flattenResponse: Specify true to associate all disruptions with parent stop point. (Only applicable when getFamily is true)
+        Args:
+            ids: A list of StopPoint ids (station naptan code e.g. 940GZZLUAS)
+            getFamily: Specify true to return disruptions for entire family, or false to return disruptions for just this stop point. Defaults to false.
+            includeRouteBlockedStops: Specify true to return disruptions for route blocked stops, or false to return disruptions for all stops. Defaults to false.
+            flattenResponse: Specify true to return a flattened response, or false to return a nested response. Defaults to false.
         """
 
         return super(stopPoint, self).sendRequestUnified(
             f"/StopPoint/{super(stopPoint, self).arrayToCSV(ids)}/Disruption",
-            {getFamily, includeRouteBlockedStops, flattenResponse},
+            {'getFamily': getFamily, 'includeRouteBlockedStops': includeRouteBlockedStops, 'flattenResponse': flattenResponse},
         )
 
     def getDisruptionsByMode(self, modes, includeRouteBlockedStops: bool):
         """
         Gets a distinct list of disrupted stop points for the given modes
 
-        :param modes: An array of modes e.g. ['tube', 'dlr']
-        :param includeRouteBlockedStops:
+        Args:
+            modes: An array of modes e.g. ['tube', 'dlr']
+            includeRouteBlockedStops: Specify true to return disruptions for route blocked stops, or false to return disruptions for all stops. Defaults to false.
         """
         return super(stopPoint, self).sendRequestUnified(
             f"/StopPoint/Mode/{super(stopPoint, self).arrayToCSV(modes)}/Disruption",
-            {includeRouteBlockedStops},
+            {'includeRouteBlockedStops': includeRouteBlockedStops},
         )
 
     def getReachableStationsByID(self, naptanID: str, lineID: str, serviceTypes=None):
         """
         Gets Stop points that are reachable from a station/line combination
 
-        :param naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
-        :param lineID: Line id of the line to filter by (e.g. victoria)
-        :param serviceTypes: List of service types to filter on. Supported values: Regular, Night.
+        Args:
+            naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
+            lineID: A Line id (e.g. victoria)
+            serviceTypes: An array of service types. Supported values: Regular, Night. Defaults to Regular.
         """
 
         if serviceTypes is None:
             serviceTypes = ["Regular"]
         return super(stopPoint, self).sendRequestUnified(
             f"/StopPoint/{naptanID}/CanReachOnLine/{lineID}",
             {"serviceTypes": super(stopPoint, self).arrayToCSV(serviceTypes)},
         )
 
     def getRouteSectionByID(self, naptanID: str, serviceTypes):
         """
         Get the route sections for all the lines that service the given stop point id#
 
-        :param naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
-        :param serviceTypes: List of service types to filter on. Supported values: Regular, Night.
+        Args:
+            naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
+            serviceTypes: An array of service types. Supported values: Regular, Night.
         """
 
         return super(stopPoint, self).sendRequestUnified(
             f"/StopPoint/{naptanID}/Route",
             {"serviceTypes": super(stopPoint, self).arrayToCSV(serviceTypes)},
         )
 
@@ -169,22 +178,23 @@
         returnLines: bool,
         latitude: int,
         longitude: int,
     ):
         """
         Gets a list of StopPoints within {radius} by the specified criteria
 
-        :param stopTypes: A list of stopTypes that should be returned
-        :param radius: The radius of the bounding circle in metres (default : 200)
-        :param useStopPointHierarchy: Re-arrange the output into a parent/child hierarchy.
-        :param modes: modes The list of modes to search eg. ['tube', 'dlr']
-        :param categories: an optional list of comma separated property categories to return in the StopPoint's property bag. If null or empty, all categories of property are returned. Pass the keyword "none" to return no properties.Pass the keyword "none" to return no properties.
-        :param returnLines: True to return the lines that each stop point serves as a nested resource.
-        :param latitude:
-        :param longitude:
+        Args:
+            stopTypes: An array of stop point types e.g. ['NaptanPublicBusCoachTram']
+            radius: The radius in metres. Defaults to 200.
+            useStopPointHierarchy: Specify true to return stop points in the hierarchy, or false to return stop points at the specified radius. Defaults to false.
+            modes: An array of modes e.g. ['tube', 'dlr']
+            categories: An array of categories e.g. ['tram', 'bus']
+            returnLines: Specify true to return the lines that service the stop point, or false to return the stop point itself. Defaults to false.
+            latitude: The latitude of the location to search from.
+            longitude: The longitude of the location to search from.
         """
 
         return super(stopPoint, self).sendRequestUnified(
             "/StopPoint",
             {
                 "stopTypes": super(stopPoint, self).arrayToCSV(stopTypes),
                 "radius": radius,
@@ -196,37 +206,40 @@
                 "longitude": longitude,
             },
         )
 
     def getBySMSCode(self, smsID: str, output: str):
         """
         Gets a StopPoint for a given sms code
-
-        :param smsID: A 5-digit Countdown Bus Stop Code e.g. 73241, 50435, 56334.
-        # :param output: If set to "web", a 302 redirect to relevant website bus stop page is returned. All other values are ignored.
+        
+        Args:
+            smsID: A 5-digit sms code e.g. 73241, 50435, 5633.
+            output: If set to "web", a 302 redirect to relevant website bus stop page is returned. All other values are ignored.
         """
 
         return super(stopPoint, self).sendRequestUnified(
-            f"/StopPoint/Sms/{smsID}", {output}
+            f"/StopPoint/Sms/{smsID}", {'output': output}
         )
 
     def getTaxiRanksByID(self, naptanID: str):
         """
         Gets a list of taxi ranks corresponding to the given stop point id
 
-        :param naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
+        Args:
+            naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
         """
 
         return super(stopPoint, self).sendRequestUnified(
-            f"/StopPoint/{naptanID}/TaxiRanks", {}
+            f"/StopPoint/{naptanID}/TaxiRanks"
         )
 
     def getCarParksByID(self, naptanID: str):
         """
         Get car parks corresponding to the given stop point id
 
-        :param naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
+        Args:
+            naptanID: A StopPoint id (station naptan code e.g. 940GZZLUAS)
         """
 
         return super(stopPoint, self).sendRequestUnified(
-            f"/StopPoint/{naptanID}/CarParks", {}
+            f"/StopPoint/{naptanID}/CarParks"
         )
```

### Comparing `tflwrapper-1.1.7/tflwrapper/tfl.py` & `tflwrapper-1.1.8/tflwrapper/tfl.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,56 +8,71 @@
 
 class tflAPI(object):
     """TFL API"""
 
     def __init__(self, app_key):
         self.app_key = app_key
 
-    def sendRequestUnified(self, uri: str, params):
+    def sendRequestUnified(self, uri: str, params = {}):
         """
         Send a HTTP GET request to the TFL Unified API using your API Key
 
-        :param uri: The url which will be prepended to unifiedAPI
-        :param params: An object containg any extra parameters
-        :returns: API Data from TfL Unified API
+        Args:
+            uri: The URI to send the request to
+            params: The parameters to send with the request
+        
+        Returns:
+            The response from the TFL Unified API
         """
         fullURL = f"https://api.tfl.gov.uk:443{uri}?{urllib.parse.urlencode({'app_key': self.app_key})}"
 
+        # If params is specified then convert it to a url encoded string
         if params:
             fullURL += f"&{urllib.parse.urlencode(params)}"
 
+        # Send the request
         resource = urllib.request.urlopen(fullURL)
+        
         return json.loads(
             resource.read().decode(resource.headers.get_content_charset())
         )
 
     @staticmethod
     def sendRequestTrackerNet(uri: str):
         """
         Send a HTTP GET request to the TrackerNet API
 
-        :param uri: The url which will be prepended to trackerNetAPI
-        :returns: API Data from TfL Unified API
+        Args:
+            uri: The URI to send the request to
+        
+        Returns:
+            The response from the TrackerNet API
         """
 
         data = urllib.request.urlopen(
             f"http://cloud.tfl.gov.uk/TrackerNet{uri}").read()
 
     @staticmethod
     def arrayToCSV(array):
         """
         Convert array to a comma-separated string
-
-        :param array: Array to convert to a comma-separated string
-        :returns: A comma-separated string
+        
+        Args:
+            array: The array to convert to a comma-separated string
+        
+        returns:
+            The comma-separated string
         """
         return ",".join(array)
 
     @staticmethod
     def getRFC3339(date_object):
         """
         Convert date object to RFC3339 standard
-
-        :param date_object: A date object to convert to RFC3339 standard
-        :returns: A RFC3339 formatted string
+        
+        Args:
+            date_object: The date object to convert
+        
+        Returns:
+            The RFC3339 formatted string
         """
         return date_object.isoformat("T") + "Z"
```

### Comparing `tflwrapper-1.1.7/tflwrapper/trackerNet.py` & `tflwrapper-1.1.8/tflwrapper/trackerNet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 from .tfl import tflAPI
 
 
 class trackerNet(tflAPI):
     """TrackerNet API"""
 
     def getPredictionSummary(self, line: str):
-        """Get detailed train prediction information for a nominated station on a nominated line within 100 minute range"""
+        """
+        Get detailed train prediction information for a nominated station on a nominated line within 100 minute range
+        
+        Args:
+            line: The line code for the line (eg. C)
+        """
 
         return super(trackerNet, self).sendRequestTrackerNet(
             f"/PredictionSummary/{line}"
         )
 
     def getPredictionDetailed(self, line: str, stationCode: str):
-        """Get detailed train prediction information for a nominated station on a nominated line within 100 minute range"""
+        """
+        Get detailed train prediction information for a nominated station on a nominated line within 100 minute range
+        
+        Args:
+            line: The line code for the line (eg. C)
+            stationCode: The station code for the station (eg. BNK)
+        """
 
         return super(trackerNet, self).sendRequestTrackerNet(
             f"/PredictionDetailed/{line}/{stationCode}"
         )
 
     def getAllLinesStatus(self, incidentsOnly: bool):
         """
         Get the status of all lines on the network indicating any delays, disruptions or suspensions on the lines.
 
-        :param incidentsOnly: Get station status information for stations with incidents only
+        Args:
+            incidentsOnly: Get line status information for lines with incidents only
         """
 
         incidentsOnlyCheck = '/IncidentsOnly' if incidentsOnly else ''
         return super(trackerNet, self).sendRequestTrackerNet(
             f"/LineStatus{incidentsOnlyCheck}"
         )
 
     def getAllStationStatus(self, incidentsOnly: bool):
         """
         Get station status information for all stations
 
-        :param incidentsOnly: Get station status information for stations with incidents only
+        Args:
+            incidentsOnly: Get station status information for stations with incidents only
         """
 
         incidentsOnlyCheck = '/IncidentsOnly' if incidentsOnly else ''
         return super(trackerNet, self).sendRequestTrackerNet(
             f"/StationStatus{incidentsOnlyCheck}"
         )
```

### Comparing `tflwrapper-1.1.7/tflwrapper.egg-info/PKG-INFO` & `tflwrapper-1.1.8/tflwrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tflwrapper
-Version: 1.1.7
+Version: 1.1.8
 Summary: A wrapper for the Transport for London Unified API and TrackerNet
 Home-page: https://github.com/you/tfl-api-wrapper-py
 Author: zackaryh8
 Author-email: zackary12389@yahoo.co.uk
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img width="200" src="https://blog.tfl.gov.uk/wp-content/uploads/2018/05/cropped-logo_roundel-2.png" alt="TfL Logo">
     <h1 align="center">TfL API Wrapper</h1>
     <p align="center">An API wrapper for the TfL Unified API, made with Python.</p>
@@ -47,9 +46,7 @@
 
 print(arrivals)
 ```
 
 ## Disclaimer
 
 This repository is not affiliated, associated, authorized, endorsed by, or in any way officially connected with Transport for London (TfL) or it's parent organisation Greater London Authority (GLA)
-
-
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: tflwrapper Version: 1.1.7 Summary: A wrapper for
+Metadata-Version: 2.1 Name: tflwrapper Version: 1.1.8 Summary: A wrapper for
 the Transport for London Unified API and TrackerNet Home-page: https://
 github.com/you/tfl-api-wrapper-py Author: zackaryh8 Author-email:
-zackary12389@yahoo.co.uk License: MIT Platform: UNKNOWN Description-Content-
-Type: text/markdown License-File: LICENSE
+zackary12389@yahoo.co.uk License: MIT Description-Content-Type: text/markdown
+License-File: LICENSE
                                   [TfL Logo]
                          ****** TfL API Wrapper ******
            An API wrapper for the TfL Unified API, made with Python.
                             Read the Documentation
 [![Code style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg)](https://github.com/psf/black) [![](https://img.shields.io/github/
 issues/ZackaryH8/tfl-api-wrapper-py)](https://github.com/ZackaryH8/tfl-api-
```

### Comparing `tflwrapper-1.1.7/tflwrapper.egg-info/SOURCES.txt` & `tflwrapper-1.1.8/tflwrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

