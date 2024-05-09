# Comparing `tmp/fmi-weather-client-0.2.1.tar.gz` & `tmp/fmi-weather-client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmi-weather-client-0.2.1.tar", last modified: Tue Feb 27 18:21:18 2024, max compression
+gzip compressed data, was "fmi-weather-client-0.2.2.tar", last modified: Thu May  9 19:59:30 2024, max compression
```

## Comparing `fmi-weather-client-0.2.1.tar` & `fmi-weather-client-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-02-27 18:21:18.115006 fmi-weather-client-0.2.1/
--rw-r--r--   0 mika       (501) staff       (20)    35149 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/LICENSE
--rw-r--r--   0 mika       (501) staff       (20)     5722 2024-02-27 18:21:18.114839 fmi-weather-client-0.2.1/PKG-INFO
--rw-r--r--   0 mika       (501) staff       (20)     4118 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/README.md
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-02-27 18:21:18.113054 fmi-weather-client-0.2.1/fmi_weather_client/
--rw-r--r--   0 mika       (501) staff       (20)     3776 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/fmi_weather_client/__init__.py
--rw-r--r--   0 mika       (501) staff       (20)      507 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/fmi_weather_client/errors.py
--rw-r--r--   0 mika       (501) staff       (20)     5064 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/fmi_weather_client/http.py
--rw-r--r--   0 mika       (501) staff       (20)     2027 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/fmi_weather_client/models.py
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-02-27 18:21:18.113978 fmi-weather-client-0.2.1/fmi_weather_client/parsers/
--rw-r--r--   0 mika       (501) staff       (20)        0 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/fmi_weather_client/parsers/__init__.py
--rw-r--r--   0 mika       (501) staff       (20)     8290 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/fmi_weather_client/parsers/forecast.py
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-02-27 18:21:18.113718 fmi-weather-client-0.2.1/fmi_weather_client.egg-info/
--rw-r--r--   0 mika       (501) staff       (20)     5722 2024-02-27 18:21:18.000000 fmi-weather-client-0.2.1/fmi_weather_client.egg-info/PKG-INFO
--rw-r--r--   0 mika       (501) staff       (20)      515 2024-02-27 18:21:18.000000 fmi-weather-client-0.2.1/fmi_weather_client.egg-info/SOURCES.txt
--rw-r--r--   0 mika       (501) staff       (20)        1 2024-02-27 18:21:18.000000 fmi-weather-client-0.2.1/fmi_weather_client.egg-info/dependency_links.txt
--rw-r--r--   0 mika       (501) staff       (20)       35 2024-02-27 18:21:18.000000 fmi-weather-client-0.2.1/fmi_weather_client.egg-info/requires.txt
--rw-r--r--   0 mika       (501) staff       (20)       19 2024-02-27 18:21:18.000000 fmi-weather-client-0.2.1/fmi_weather_client.egg-info/top_level.txt
--rw-r--r--   0 mika       (501) staff       (20)       38 2024-02-27 18:21:18.115064 fmi-weather-client-0.2.1/setup.cfg
--rw-r--r--   0 mika       (501) staff       (20)      907 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/setup.py
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-02-27 18:21:18.114582 fmi-weather-client-0.2.1/test/
--rw-r--r--   0 mika       (501) staff       (20)     1161 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/test/test_http.py
--rw-r--r--   0 mika       (501) staff       (20)     7694 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/test/test_init.py
--rw-r--r--   0 mika       (501) staff       (20)      694 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/test/test_models.py
--rw-r--r--   0 mika       (501) staff       (20)     2044 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.1/test/test_parsers_forecast.py
+drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.329298 fmi-weather-client-0.2.2/
+-rw-r--r--   0 mika       (501) staff       (20)    35149 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/LICENSE
+-rw-r--r--   0 mika       (501) staff       (20)     5722 2024-05-09 19:59:30.329121 fmi-weather-client-0.2.2/PKG-INFO
+-rw-r--r--   0 mika       (501) staff       (20)     4118 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/README.md
+drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.327027 fmi-weather-client-0.2.2/fmi_weather_client/
+-rw-r--r--   0 mika       (501) staff       (20)     3776 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/__init__.py
+-rw-r--r--   0 mika       (501) staff       (20)      507 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/errors.py
+-rw-r--r--   0 mika       (501) staff       (20)     5064 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/http.py
+-rw-r--r--   0 mika       (501) staff       (20)     2027 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/models.py
+drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.328115 fmi-weather-client-0.2.2/fmi_weather_client/parsers/
+-rw-r--r--   0 mika       (501) staff       (20)        0 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/parsers/__init__.py
+-rw-r--r--   0 mika       (501) staff       (20)     8290 2024-05-09 19:56:15.000000 fmi-weather-client-0.2.2/fmi_weather_client/parsers/forecast.py
+drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.327823 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/
+-rw-r--r--   0 mika       (501) staff       (20)     5722 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/PKG-INFO
+-rw-r--r--   0 mika       (501) staff       (20)      515 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mika       (501) staff       (20)        1 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mika       (501) staff       (20)       35 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/requires.txt
+-rw-r--r--   0 mika       (501) staff       (20)       19 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/top_level.txt
+-rw-r--r--   0 mika       (501) staff       (20)       38 2024-05-09 19:59:30.329359 fmi-weather-client-0.2.2/setup.cfg
+-rw-r--r--   0 mika       (501) staff       (20)      907 2024-05-09 19:56:15.000000 fmi-weather-client-0.2.2/setup.py
+drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.328817 fmi-weather-client-0.2.2/test/
+-rw-r--r--   0 mika       (501) staff       (20)     1161 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/test/test_http.py
+-rw-r--r--   0 mika       (501) staff       (20)     7694 2024-05-09 19:56:15.000000 fmi-weather-client-0.2.2/test/test_init.py
+-rw-r--r--   0 mika       (501) staff       (20)      694 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/test/test_models.py
+-rw-r--r--   0 mika       (501) staff       (20)     2044 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/test/test_parsers_forecast.py
```

### Comparing `fmi-weather-client-0.2.1/LICENSE` & `fmi-weather-client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.1/PKG-INFO` & `fmi-weather-client-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmi-weather-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library for fetching weather information from Finnish Meteorological Institute (FMI)
 Home-page: https://github.com/saaste/fmi-weather-client
 Author: Mika Hiltunen
 Author-email: saaste@gmail.com
 License: UNKNOWN
 Description: ![Test](https://github.com/saaste/fmi-weather-client/workflows/tests/badge.svg?branch=master)
         ![Last commit](https://img.shields.io/github/last-commit/saaste/fmi-weather-client)
```

### Comparing `fmi-weather-client-0.2.1/README.md` & `fmi-weather-client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.1/fmi_weather_client/__init__.py` & `fmi-weather-client-0.2.2/fmi_weather_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.1/fmi_weather_client/http.py` & `fmi-weather-client-0.2.2/fmi_weather_client/http.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.1/fmi_weather_client/models.py` & `fmi-weather-client-0.2.2/fmi_weather_client/models.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.1/fmi_weather_client/parsers/forecast.py` & `fmi-weather-client-0.2.2/fmi_weather_client/parsers/forecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 
 def _get_place(data: Dict[str, Any]) -> FMIPlace:
     place_data = (data['wfs:FeatureCollection']['wfs:member']['omso:GridSeriesObservation']
                       ['om:featureOfInterest']['sams:SF_SpatialSamplingFeature']['sams:shape']
                       ['gml:MultiPoint']['gml:pointMembers']['gml:Point'])
 
     coordinates = place_data['gml:pos'].split(' ', 1)
-    lon = float(coordinates[0])
-    lat = float(coordinates[1])
+    lat = float(coordinates[0])
+    lon = float(coordinates[1])
 
     return FMIPlace(place_data['gml:name'], lat, lon)
 
 
 def _get_datetimes(data: Dict[str, Any]) -> List[datetime]:
     result = []
     forecast_datetimes = (data['wfs:FeatureCollection']['wfs:member']['omso:GridSeriesObservation']
```

### Comparing `fmi-weather-client-0.2.1/fmi_weather_client.egg-info/PKG-INFO` & `fmi-weather-client-0.2.2/fmi_weather_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmi-weather-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library for fetching weather information from Finnish Meteorological Institute (FMI)
 Home-page: https://github.com/saaste/fmi-weather-client
 Author: Mika Hiltunen
 Author-email: saaste@gmail.com
 License: UNKNOWN
 Description: ![Test](https://github.com/saaste/fmi-weather-client/workflows/tests/badge.svg?branch=master)
         ![Last commit](https://img.shields.io/github/last-commit/saaste/fmi-weather-client)
```

### Comparing `fmi-weather-client-0.2.1/fmi_weather_client.egg-info/SOURCES.txt` & `fmi-weather-client-0.2.2/fmi_weather_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.1/setup.py` & `fmi-weather-client-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fmi-weather-client",
-    version="0.2.1",
+    version="0.2.2",
     author="Mika Hiltunen",
     author_email="saaste@gmail.com",
     description="Library for fetching weather information from Finnish Meteorological Institute (FMI)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/saaste/fmi-weather-client",
     packages=setuptools.find_packages(exclude=["*test", "*test.*"]),
```

### Comparing `fmi-weather-client-0.2.1/test/test_http.py` & `fmi-weather-client-0.2.2/test/test_http.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.1/test/test_init.py` & `fmi-weather-client-0.2.2/test/test_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def test_get_forecast_by_coordinates(self, mock_get):
         forecast = fmi_weather_client.forecast_by_coordinates(29.742731, 67.583988)
         self.assert_coordinate_forecast(forecast)
 
     @mock.patch('requests.get', side_effect=test_data.mock_coordinate_forecast_response)
     def test_async_get_forecast_by_coordinates(self, mock_get):
         loop = asyncio.get_event_loop()
-        forecast = loop.run_until_complete(fmi_weather_client.async_forecast_by_coordinates(29.742731, 67.583988))
+        forecast = loop.run_until_complete(fmi_weather_client.async_forecast_by_coordinates(67.583988, 29.742731))
         self.assert_coordinate_forecast(forecast)
 
     # CORNER CASES
     @mock.patch('requests.get', side_effect=test_data.mock_nan_response)
     def test_nil_weather_response(self, mock_get):
         weather_coord = fmi_weather_client.weather_by_coordinates(25.46816, 65.01236)
         weather_name = fmi_weather_client.weather_by_place_name('Oulu')
@@ -124,25 +124,25 @@
         self.assertEqual(weather.place, 'Sauoiva')
         self.assertEqual(weather.data.time.timestamp(), 1663585800.0)
         self.assertEqual(weather.data.temperature.value, 6.6)
         self.assertEqual(weather.data.wind_speed.value, 4.79)
 
     def assert_name_forecast(self, forecast):
         self.assertEqual(forecast.place, 'Iisalmi')
-        self.assertEqual(forecast.lat, 27.19067)
-        self.assertEqual(forecast.lon, 63.55915)
+        self.assertEqual(forecast.lat, 63.55915)
+        self.assertEqual(forecast.lon, 27.19067)
         self.assertEqual(len(forecast.forecasts), 12)
         self.assertEqual(forecast.forecasts[0].temperature.value, 12.3)
         self.assertEqual(forecast.forecasts[1].pressure.value, 1000.6)
         self.assertEqual(forecast.forecasts[4].humidity.value, 80.7)
 
     def assert_coordinate_forecast(self, forecast):
         self.assertEqual(forecast.place, 'Sauoiva')
-        self.assertEqual(forecast.lat, 29.74273)
-        self.assertEqual(forecast.lon, 67.58399)
+        self.assertEqual(forecast.lat, 67.58399)
+        self.assertEqual(forecast.lon, 29.74273)
         self.assertEqual(len(forecast.forecasts), 12)
         self.assertEqual(forecast.forecasts[0].temperature.value, 6.8)
         self.assertEqual(forecast.forecasts[1].pressure.value, 1005.8)
         self.assertEqual(forecast.forecasts[4].humidity.value, 97.9)
 
 
 if __name__ == '__main__':
```

### Comparing `fmi-weather-client-0.2.1/test/test_models.py` & `fmi-weather-client-0.2.2/test/test_models.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.1/test/test_parsers_forecast.py` & `fmi-weather-client-0.2.2/test/test_parsers_forecast.py`

 * *Files identical despite different names*

