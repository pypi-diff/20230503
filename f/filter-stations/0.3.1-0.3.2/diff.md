# Comparing `tmp/filter_stations-0.3.1.tar.gz` & `tmp/filter_stations-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_stations-0.3.1.tar", last modified: Mon May  1 20:36:30 2023, max compression
+gzip compressed data, was "filter_stations-0.3.2.tar", last modified: Wed May  3 06:56:42 2023, max compression
```

## Comparing `filter_stations-0.3.1.tar` & `filter_stations-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 20:36:30.372008 filter_stations-0.3.1/
--rw-rw-rw-   0        0        0    39900 2023-05-01 20:36:30.369020 filter_stations-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    39594 2023-05-01 20:35:50.000000 filter_stations-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 20:36:30.267863 filter_stations-0.3.1/filter_stations/
--rw-rw-rw-   0        0        0    33665 2023-05-01 19:30:40.000000 filter_stations-0.3.1/filter_stations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:36:30.357811 filter_stations-0.3.1/filter_stations.egg-info/
--rw-rw-rw-   0        0        0    39900 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-01 20:36:29.000000 filter_stations-0.3.1/filter_stations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 20:36:30.373007 filter_stations-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-05-01 20:36:19.000000 filter_stations-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:56:42.947232 filter_stations-0.3.2/
+-rw-rw-rw-   0        0        0    39900 2023-05-03 06:56:42.946220 filter_stations-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    39594 2023-05-01 20:35:50.000000 filter_stations-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 06:56:42.907290 filter_stations-0.3.2/filter_stations/
+-rw-rw-rw-   0        0        0    36141 2023-05-03 06:56:15.000000 filter_stations-0.3.2/filter_stations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:56:42.944069 filter_stations-0.3.2/filter_stations.egg-info/
+-rw-rw-rw-   0        0        0    39900 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-03 06:56:42.000000 filter_stations-0.3.2/filter_stations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 06:56:42.948217 filter_stations-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-05-03 06:53:56.000000 filter_stations-0.3.2/setup.py
```

### Comparing `filter_stations-0.3.1/PKG-INFO` & `filter_stations-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filter_stations
-Version: 0.3.1
+Version: 0.3.2
 Summary: Making it easier to navigate and clean station data
 Home-page: https://github.com/kaburia/Packaging/tree/main/filter_stations
 Author: Austin Kaburia
 Author-email: kaburiaaustin1@gmail.com
 Description-Content-Type: text/markdown
 
 <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: filter_stations Version: 0.3.1 Summary: Making it
+Metadata-Version: 2.1 Name: filter_stations Version: 0.3.2 Summary: Making it
 easier to navigate and clean station data Home-page: https://github.com/
 kaburia/Packaging/tree/main/filter_stations Author: Austin Kaburia Author-
 email: kaburiaaustin1@gmail.com Description-Content-Type: text/markdown
                                                                                    index
                                                                                       c:
 __init__ \users\austin\desktop\agent\packages\filter_stations\filter_stations\__init__.py
```

### Comparing `filter_stations-0.3.1/README.md` & `filter_stations-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `filter_stations-0.3.1/filter_stations/__init__.py` & `filter_stations-0.3.2/filter_stations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,33 @@
         # Calculate distances to all other stations and sort by distance
         infostations = self.get_stations_info()
         infostations['distance'] = infostations.apply(lambda row: hs.haversine((lat, lon), (row['location.latitude'], row['location.longitude'])), axis=1)
         infostations = infostations.sort_values('distance')
         
         # Create dictionary of nearest neighbouring stations and their distances
         return dict(infostations[['code', 'distance']].head(number).values[1:])
+    
+    # trained models in stored in mongoDB
+    def trained_models(self, columns=None):
+        """
+        Retrieves trained models from the MongoDB.
+
+        Args:
+            columns (list of str, optional): List of column names to include in the returned DataFrame. 
+                If None, all columns are included. Defaults to None.
+
+        Returns:
+            pandas.DataFrame: DataFrame containing trained models with the specified columns.
+        """
+        reqUrl = "https://tahmorqctest.eu-de.mybluemix.net/api/models" # endpoint
+        response = self.__request(reqUrl, {})
+        if columns:
+            return pd.DataFrame(response.json())[columns]
+        else:
+            return pd.DataFrame(response.json())
 
     
     def aggregate_variables(self, dataframe):
         """
         Aggregates a pandas DataFrame of weather variables by summing values across each day.
 
         Args:
@@ -172,31 +191,36 @@
         # Group by date and sum values
         return dataframe.groupby(pd.Grouper(key='Date', axis=0, freq='1D')).sum()
 
     
     # Get the variables only
     def get_measurements(self, station, startDate=None, endDate=None, variables=None, dataset='controlled', aggregate=False):
             """
-            Get measurements for a specified station and time period.
+            Get measurements from a station.
 
-            :param station: The station ID for which to retrieve measurements.
-            :type station: str
-            :param startDate: The start date of the time period for which to retrieve measurements.
-            :type startDate: datetime or str, optional
-            :param endDate: The end date of the time period for which to retrieve measurements.
-            :type endDate: datetime or str, optional
-            :param variables: A list of variable shortcodes to retrieve measurements for. If None, all variables are retrieved.
-            :type variables: list or None, optional
-            :param dataset: The dataset to retrieve measurements from. Default is 'controlled'.
-            :type dataset: str, optional
-            :param aggregate: Whether to aggregate variables by sensor ID. Default is False.
-            :type aggregate: bool, optional
-            :return: A Pandas DataFrame containing the requested measurements.
-            :rtype: pandas.DataFrame
-            """
+            Parameters:
+            -----------
+            station: str
+                The station ID.
+            startDate: str, optional
+                The start date of the measurement period in the format 'YYYY-MM-DD'.
+            endDate: str, optional
+                The end date of the measurement period in the format 'YYYY-MM-DD'.
+            variables: list, optional
+                The variables to retrieve measurements for. If None, all variables are retrieved.
+            dataset: str, optional
+                The dataset to retrieve measurements from. Default is 'controlled'.
+            aggregate: bool, optional
+                Whether to aggregate the measurements by variable. Default is False.
+
+            Returns:
+            --------
+            pd.DataFrame
+                A DataFrame containing the measurements.
+            """            
             #print('Get measurements', station, startDate, endDate, variables)
             endpoint = 'services/measurements/v2/stations/%s/measurements/%s' % (station, dataset)
 
             dateSplit = self.__splitDateRange(startDate, endDate)
             series = []
             seriesHolder = {}
 
@@ -362,15 +386,15 @@
     def __init__(self, apiKey, apiSecret):
         super().__init__(apiKey, apiSecret)
     
     def get_stations_info(self, station=None, multipleStations=[], countrycode=None):
         return super().get_stations_info(station, multipleStations, countrycode)
         
     # Get the centre point of the address
-    def getLocation(self, address):
+    def centre_point(self, address):
         """
         This method retrieves the latitude and longitude coordinates of a given address using the Nominatim API.
         
         Parameters:
         -----------
         address : str
             The address of the location you want to retrieve the coordinates for.
@@ -382,21 +406,27 @@
         """
         url = 'https://nominatim.openstreetmap.org/search/' + urllib.parse.quote(address) +'?format=json'
         return requests.get(url).json()[0]['lat'], requests.get(url).json()[0]['lon']
 
     # Get the new radius of the address
     def calculate_new_point(self, lat, lon, distance, bearing):
         """
-        Calculate a new point given a starting point, distance, and bearing.
-        
-        :param lat: starting latitude in degrees
-        :param lon: starting longitude in degrees
-        :param distance: distance to move in meters
-        :param bearing: bearing to move in degrees (0 is north)
-        :return: tuple containing the new latitude and longitude in degrees
+        Calculates a new geographic point based on the given latitude, longitude,
+        distance and bearing.
+
+        Parameters:
+            lat (float): The latitude of the starting point in decimal degrees.
+            lon (float): The longitude of the starting point in decimal degrees.
+            distance (float): The distance in kilometers from the starting point to the new point.
+            bearing (float): The bearing in degrees from the starting point to the new point,
+                measured clockwise from true north.
+
+        Returns:
+            Tuple[float, float]: A tuple containing the latitude and longitude of the new point,
+            respectively, in decimal degrees.
         """
         distance = distance * 1000
         # Convert degrees to radians
         lat = math.radians(lat)
         lon = math.radians(lon)
         bearing = math.radians(bearing)
         
@@ -439,29 +469,29 @@
         g2 = [max(p[0] for p in points), max(p[1] for p in points)]
         # print(g1, '\n', g2)
         return g1[0], g1[1], g2[0], g2[1]
 
     # Get the minimum and maximum latitude and longitude of the address
 
 
-    def filterStations(self, address, distance, startDate=None, endDate=None, csvfile='KEcheck3.csv'):
+    def filter_stations(self, address, distance, startDate=None, endDate=None, csvfile='KEcheck3.csv'):
         """
         This method filters weather station data within a certain distance from a given address.
         
         Parameters:
         address (str): Address to center the bounding box around.
         distance (float): The distance (in kilometers) from the center to the edge of the bounding box.
         startDate (str): The start date for filtering the weather station data in the format 'YYYY-MM-DD'.
         endDate (str): The end date for filtering the weather station data in the format 'YYYY-MM-DD'.
         csvfile (str): The name of the csv file containing the weather station data.
         
         Returns:
         pandas.DataFrame: The filtered weather station data within the bounding box.
         """     
-        lat, lon = self.getLocation(address)
+        lat, lon = self.centre_point(address)
         min_lat, min_lon, max_lat, max_lon = self.compute_filter(float(lat), float(lon), distance)
         stations = super().get_stations_info()
         bounds = list(stations['code'][(stations['location.longitude'] >= min_lon)
                                         & (stations['location.longitude'] <= max_lon)
                                         & (stations['location.latitude'] >= min_lat)
                                             & (stations['location.latitude'] <= max_lat)])
         
@@ -482,26 +512,26 @@
             return ke_chec[[col for bbox in bounds for col in ke_chec if bbox in col]]
         else:
             ke_chec = ke_chec.set_index('Date')
             return ke_chec[[col for bbox in bounds for col in ke_chec if bbox in col]]
 
 
     # A list of filtered stations
-    def filterStationsList(self, address, distance=100):
+    def filter_stations_list(self, address, distance=100):
         """
         Filters stations based on their proximity to a given address and returns a list of station codes that fall within the specified distance.
         
         Args:
             address (str): Address to filter stations by.
             distance (float, optional): Maximum distance (in kilometers) between the stations and the address. Default is 100 km.
         
         Returns:
             List of station codes that fall within the specified distance from the given address.
         """
-        return list(set([i.split('_')[0] for i in self.filterStations(f'{address}', distance).columns if i.split('_')[-1] != 'clogFlag']))
+        return list(set([i.split('_')[0] for i in self.filter_stations(f'{address}', distance).columns if i.split('_')[-1] != 'clogFlag']))
 
     
 
 # A different class for visualisations
 class Interactive_maps(retreive_data):
     # inherit from retrieve_data class
     def __init__(self, apiKey, apiSecret):
@@ -531,53 +561,90 @@
         marker_locations = [[row['location.latitude'], row['location.longitude']] for _, row in stations.iterrows()]
         my_map.fit_bounds(marker_locations)
 
         # display the map
         return my_map
 
 
-    def create_animation(self, data, valid_sensors, day=100, T=10, interval=500):
+    def animation_image(self, sensors,  start_date, end_date, day=100, T=10, interval=500, data=None):
         '''
         Creates an animation of pollutant levels for a given range of days and valid sensors.
 
         Parameters:
         data (DataFrame): A pandas DataFrame containing pollution data.
-        valid_sensors (list): A list of valid sensor names.
+        sensors (list): A list of valid sensor names.
         day (int): The starting day of the animation (default is 100).
         T (int): The range of days for the animation (default is 10).
         interval (int): The interval between frames in milliseconds (default is 500).
 
         Returns:
         HTML: An HTML object containing the animation.
         '''
+        if not data:
+            data = pd.read_csv('KEcheck3.csv')
+            data['Date'] = pd.to_datetime(data['Date'])
+            data = data.loc[(data['Date'] >= start_date) & (data['Date'] <= end_date)]
+
         
-        data1 = np.array(data[valid_sensors].iloc[day:day+1]).T
+        data1 = np.array(data[sensors].iloc[day:day+1]).T
         data1 /= np.max(data1)
         # Create figure and axis
         fig, ax = plt.subplots()
 
         # Define function to update matrix data
         def update(i):
             # Generate new data
-            new_data =  np.array(data[valid_sensors].iloc[int(day):int(day+1+i)]).T
+            new_data =  np.array(data[sensors].iloc[int(day):int(day+1+i)]).T
             new_data /= np.max(new_data)
 
             # Update matrix data
             im.set_array(new_data)
 
             return [im]
 
         # Create matrix plot
         im = ax.imshow(data1, aspect='auto', interpolation=None)
 
         # Create animation
         ani = animation.FuncAnimation(fig, update, frames=range(T), interval=interval, blit=False)
+
         plt.close()
 
         return HTML(ani.to_jshtml())
+    
+    # create animation grid
+    def animation_grid(self, mu_pred, xi, xj, valid_station_df, clogged_station_df, T=10):
+        """
+        Creates an animation of the predicted data on a grid over time.
+
+        Parameters:
+        mu_pred (ndarray): The predicted data on a grid over time.
+        xi (ndarray): The x-coordinates of the grid.
+        xj (ndarray): The y-coordinates of the grid.
+        valid_station_df (DataFrame): A DataFrame containing the information of the valid stations.
+        clogged_station_df (DataFrame): A DataFrame containing the information of the clogged stations.
+        T (int): The number of time steps.
+
+        Returns:
+        HTML: The animation as an HTML object.
+        """
+        fig, ax = plt.subplots()
+
+        def animate(t):
+            ax.clear()
+            ax.set_title('Time step {}'.format(t))
+            ax.pcolor(xi, xj, mu_pred[:, t:t+1].reshape(xi.shape), shading='auto')
+            ax.plot(valid_station_df['Longitude'], valid_station_df['Latitude'], '.')
+            ax.plot(clogged_station_df['Longitude'], clogged_station_df['Latitude'], 'r.')
+
+        ani = animation.FuncAnimation(fig, animate, frames=T, interval=500, blit=False)
+        plt.close()
+        
+        return HTML(ani.to_jshtml())
+
 
 
     def plot_station(self, ws, df_rainfall):
         """
         Plot the rainfall data for a specific weather station.
 
         Args:
@@ -642,15 +709,15 @@
             image_data = base64.b64encode(buf.read()).decode('utf-8')
             return '<img src="data:image/png;base64,{}">'.format(image_data)
         else:
             return 'No data available for station {}'.format(ws)
 
 
 
-    def get_map(self, subset_list, start_date=None, end_date=None, data_values=False, csv_file='KEcheck3.csv', min_zoom=8, max_zoom=11, width=850, height=850, png_resolution=300):
+    def get_map(self, subset_list, start_date=None, end_date=None, data_values=False, csv_file='KEcheck3.csv', min_zoom=8, max_zoom=11, width=2000, height=2000, png_resolution=300):
         """
         Creates a Folium map showing the locations of the weather stations in the given subsets.
 
         Parameters:
         -----------
         subset_list : list of lists of str
             List of subsets of weather stations, where each subset is a list of station codes.
@@ -711,15 +778,15 @@
         color_markers = ['blue', 'red', 'green', 'purple', 'orange', 'black', 'beige', 'yellow', 'violet', 'brown']
         for _, row in stations.iterrows():
             # loop throught the list subsets and create markers for each subset
             for num, subs in enumerate(subset_list):
                 if row['code'] in subs:
                     # Create an IFrame object with the image as the content
                     if data_values:
-                        popup_iframe = folium.IFrame(html=f"{self.encode_image(row['code'], df_rainfall)}", width=width//2, height=height//2)
+                        popup_iframe = folium.IFrame(html=f"{self.encode_image(row['code'], df_rainfall)}", width=width//8, height=height//8)
                         folium.Marker([row['location.latitude'], row['location.longitude']], popup=folium.Popup(popup_iframe),  
                                     tooltip=row['code'], icon=folium.Icon(color=color_markers[num])).add_to(my_map)
                     else:
                         folium.Marker([row['location.latitude'], row['location.longitude']], 
                                     tooltip=row['code'], icon=folium.Icon(color=color_markers[num])).add_to(my_map)
         
         # display the map
@@ -733,8 +800,8 @@
 
     return parser.parse_args()
 
 if __name__ == '__main__':
     args = parse_args()
     
     if args.address or args.csvfile:
-        filter.filterStations(address=args.address, csvfile=args.csvfile)
+        filter.filter_stations(address=args.address, csvfile=args.csvfile)
```

### Comparing `filter_stations-0.3.1/filter_stations.egg-info/PKG-INFO` & `filter_stations-0.3.2/filter_stations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filter-stations
-Version: 0.3.1
+Version: 0.3.2
 Summary: Making it easier to navigate and clean station data
 Home-page: https://github.com/kaburia/Packaging/tree/main/filter_stations
 Author: Austin Kaburia
 Author-email: kaburiaaustin1@gmail.com
 Description-Content-Type: text/markdown
 
 <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: filter-stations Version: 0.3.1 Summary: Making it
+Metadata-Version: 2.1 Name: filter-stations Version: 0.3.2 Summary: Making it
 easier to navigate and clean station data Home-page: https://github.com/
 kaburia/Packaging/tree/main/filter_stations Author: Austin Kaburia Author-
 email: kaburiaaustin1@gmail.com Description-Content-Type: text/markdown
                                                                                    index
                                                                                       c:
 __init__ \users\austin\desktop\agent\packages\filter_stations\filter_stations\__init__.py
```

### Comparing `filter_stations-0.3.1/setup.py` & `filter_stations-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='filter_stations',
-    version='0.3.1',
+    version='0.3.2',
     packages=find_packages(),
     include_package_data=True,
     description='Making it easier to navigate and clean station data',
     author='Austin Kaburia',
     author_email='kaburiaaustin1@gmail.com',
     url='https://github.com/kaburia/Packaging/tree/main/filter_stations',
     install_requires=[
```

