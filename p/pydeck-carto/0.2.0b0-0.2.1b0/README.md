# Comparing `tmp/pydeck-carto-0.2.0b0.tar.gz` & `tmp/pydeck-carto-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeck-carto-0.2.0b0.tar", last modified: Wed Apr 24 19:39:07 2024, max compression
+gzip compressed data, was "pydeck-carto-0.2.1b0.tar", last modified: Thu May  9 20:01:16 2024, max compression
```

## Comparing `pydeck-carto-0.2.0b0.tar` & `pydeck-carto-0.2.1b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 donmccurdy   (501) staff       (20)        0 2024-04-24 19:39:07.868241 pydeck-carto-0.2.0b0/
--rw-r--r--   0 donmccurdy   (501) staff       (20)     1512 2023-11-13 16:22:18.000000 pydeck-carto-0.2.0b0/LICENSE
--rw-r--r--   0 donmccurdy   (501) staff       (20)     3035 2024-04-24 19:39:07.868318 pydeck-carto-0.2.0b0/PKG-INFO
--rw-r--r--   0 donmccurdy   (501) staff       (20)     2021 2024-04-24 19:12:23.000000 pydeck-carto-0.2.0b0/README.md
-drwxr-xr-x   0 donmccurdy   (501) staff       (20)        0 2024-04-24 19:39:07.867193 pydeck-carto-0.2.0b0/pydeck_carto/
--rw-r--r--   0 donmccurdy   (501) staff       (20)      198 2024-04-24 19:12:23.000000 pydeck-carto-0.2.0b0/pydeck_carto/__init__.py
--rw-r--r--   0 donmccurdy   (501) staff       (20)       24 2024-04-24 19:12:23.000000 pydeck-carto-0.2.0b0/pydeck_carto/_version.py
--rw-r--r--   0 donmccurdy   (501) staff       (20)     2108 2024-04-24 19:12:23.000000 pydeck-carto-0.2.0b0/pydeck_carto/layer.py
--rw-r--r--   0 donmccurdy   (501) staff       (20)     7713 2024-04-24 19:12:23.000000 pydeck-carto-0.2.0b0/pydeck_carto/sources.py
--rw-r--r--   0 donmccurdy   (501) staff       (20)     3286 2023-11-13 16:22:18.000000 pydeck-carto-0.2.0b0/pydeck_carto/styles.py
-drwxr-xr-x   0 donmccurdy   (501) staff       (20)        0 2024-04-24 19:39:07.868121 pydeck-carto-0.2.0b0/pydeck_carto.egg-info/
--rw-r--r--   0 donmccurdy   (501) staff       (20)     3035 2024-04-24 19:39:07.000000 pydeck-carto-0.2.0b0/pydeck_carto.egg-info/PKG-INFO
--rw-r--r--   0 donmccurdy   (501) staff       (20)      369 2024-04-24 19:39:07.000000 pydeck-carto-0.2.0b0/pydeck_carto.egg-info/SOURCES.txt
--rw-r--r--   0 donmccurdy   (501) staff       (20)        1 2024-04-24 19:39:07.000000 pydeck-carto-0.2.0b0/pydeck_carto.egg-info/dependency_links.txt
--rw-r--r--   0 donmccurdy   (501) staff       (20)        1 2024-04-24 19:39:07.000000 pydeck-carto-0.2.0b0/pydeck_carto.egg-info/not-zip-safe
--rw-r--r--   0 donmccurdy   (501) staff       (20)       57 2024-04-24 19:39:07.000000 pydeck-carto-0.2.0b0/pydeck_carto.egg-info/requires.txt
--rw-r--r--   0 donmccurdy   (501) staff       (20)       13 2024-04-24 19:39:07.000000 pydeck-carto-0.2.0b0/pydeck_carto.egg-info/top_level.txt
--rw-r--r--   0 donmccurdy   (501) staff       (20)       69 2024-04-24 19:39:07.868579 pydeck-carto-0.2.0b0/setup.cfg
--rw-r--r--   0 donmccurdy   (501) staff       (20)     1507 2024-04-24 19:12:23.000000 pydeck-carto-0.2.0b0/setup.py
+drwxr-xr-x   0 donmccurdy   (501) staff       (20)        0 2024-05-09 20:01:16.816053 pydeck-carto-0.2.1b0/
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     1512 2023-11-13 16:22:18.000000 pydeck-carto-0.2.1b0/LICENSE
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     3063 2024-05-09 20:01:16.816146 pydeck-carto-0.2.1b0/PKG-INFO
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     2049 2024-04-29 17:55:15.000000 pydeck-carto-0.2.1b0/README.md
+drwxr-xr-x   0 donmccurdy   (501) staff       (20)        0 2024-05-09 20:01:16.814929 pydeck-carto-0.2.1b0/pydeck_carto/
+-rw-r--r--   0 donmccurdy   (501) staff       (20)      198 2024-04-29 17:55:12.000000 pydeck-carto-0.2.1b0/pydeck_carto/__init__.py
+-rw-r--r--   0 donmccurdy   (501) staff       (20)       24 2024-05-09 19:59:31.000000 pydeck-carto-0.2.1b0/pydeck_carto/_version.py
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     2108 2024-05-09 19:56:28.000000 pydeck-carto-0.2.1b0/pydeck_carto/layer.py
+-rw-r--r--   0 donmccurdy   (501) staff       (20)    13368 2024-04-29 17:55:15.000000 pydeck-carto-0.2.1b0/pydeck_carto/sources.py
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     3286 2023-11-13 16:22:18.000000 pydeck-carto-0.2.1b0/pydeck_carto/styles.py
+drwxr-xr-x   0 donmccurdy   (501) staff       (20)        0 2024-05-09 20:01:16.815930 pydeck-carto-0.2.1b0/pydeck_carto.egg-info/
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     3063 2024-05-09 20:01:16.000000 pydeck-carto-0.2.1b0/pydeck_carto.egg-info/PKG-INFO
+-rw-r--r--   0 donmccurdy   (501) staff       (20)      369 2024-05-09 20:01:16.000000 pydeck-carto-0.2.1b0/pydeck_carto.egg-info/SOURCES.txt
+-rw-r--r--   0 donmccurdy   (501) staff       (20)        1 2024-05-09 20:01:16.000000 pydeck-carto-0.2.1b0/pydeck_carto.egg-info/dependency_links.txt
+-rw-r--r--   0 donmccurdy   (501) staff       (20)        1 2024-05-09 20:01:16.000000 pydeck-carto-0.2.1b0/pydeck_carto.egg-info/not-zip-safe
+-rw-r--r--   0 donmccurdy   (501) staff       (20)       57 2024-05-09 20:01:16.000000 pydeck-carto-0.2.1b0/pydeck_carto.egg-info/requires.txt
+-rw-r--r--   0 donmccurdy   (501) staff       (20)       13 2024-05-09 20:01:16.000000 pydeck-carto-0.2.1b0/pydeck_carto.egg-info/top_level.txt
+-rw-r--r--   0 donmccurdy   (501) staff       (20)       69 2024-05-09 20:01:16.816356 pydeck-carto-0.2.1b0/setup.cfg
+-rw-r--r--   0 donmccurdy   (501) staff       (20)     1507 2024-05-08 15:38:35.000000 pydeck-carto-0.2.1b0/setup.py
```

### Comparing `pydeck-carto-0.2.0b0/LICENSE` & `pydeck-carto-0.2.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeck-carto-0.2.0b0/PKG-INFO` & `pydeck-carto-0.2.1b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeck-carto
-Version: 0.2.0b0
+Version: 0.2.1b0
 Summary: Pydeck wrapper for use with CARTO
 Home-page: https://github.com/visgl/deck.gl/tree/master/bindings/pydeck-carto
 Author: CARTO
 Author-email: jarroyo@carto.com
 License: BSD 3-Clause
 Keywords: pydeck,carto,visualization,graphics,GIS,maps
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,21 +56,23 @@
 
 # Authentication with CARTO
 carto_auth = CartoAuth.from_oauth()
 
 # Register new layer types in pydeck
 pdkc.register_layers()
 
-# Render CARTO layer in pydeck
+# Create CARTO data source
 data = pdkc.sources.vector_query_source(
     access_token=carto_auth.get_access_token(),
     api_base_url=carto_auth.get_api_base_url(),
     connection_name="carto_dw",
     sql_query="SELECT geom, name FROM carto-demo-data.demo_tables.world_airports",
 )
+
+# Render CARTO layer in pydeck
 layer = pdk.Layer(
     "VectorTileLayer",
     data=data,
     get_fill_color=[238, 77, 90],
     point_radius_min_pixels=2.5,
     pickable=True,
 )
```

### Comparing `pydeck-carto-0.2.0b0/README.md` & `pydeck-carto-0.2.1b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 
 # Authentication with CARTO
 carto_auth = CartoAuth.from_oauth()
 
 # Register new layer types in pydeck
 pdkc.register_layers()
 
-# Render CARTO layer in pydeck
+# Create CARTO data source
 data = pdkc.sources.vector_query_source(
     access_token=carto_auth.get_access_token(),
     api_base_url=carto_auth.get_api_base_url(),
     connection_name="carto_dw",
     sql_query="SELECT geom, name FROM carto-demo-data.demo_tables.world_airports",
 )
+
+# Render CARTO layer in pydeck
 layer = pdk.Layer(
     "VectorTileLayer",
     data=data,
     get_fill_color=[238, 77, 90],
     point_radius_min_pixels=2.5,
     pickable=True,
 )
```

### Comparing `pydeck-carto-0.2.0b0/pydeck_carto/layer.py` & `pydeck-carto-0.2.1b0/pydeck_carto/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pydeck as pdk
 
 H3_VERSION = "~4.1.*"
-DECKGL_VERSION = "~9.0.*"
+DECKGL_VERSION = "9.0.13"
 
 LIBRARIES_TO_INCLUDE = [
     f"npm/h3-js@{H3_VERSION}/dist/h3-js.umd.js",
     f"npm/@deck.gl/extensions@{DECKGL_VERSION}/dist.min.js",
     f"npm/@deck.gl/carto@{DECKGL_VERSION}/dist.min.js",
 ]
 SELECTED_LIBRARIES = ",".join(LIBRARIES_TO_INCLUDE)
```

### Comparing `pydeck-carto-0.2.0b0/pydeck_carto/styles.py` & `pydeck-carto-0.2.1b0/pydeck_carto/styles.py`

 * *Files identical despite different names*

### Comparing `pydeck-carto-0.2.0b0/pydeck_carto.egg-info/PKG-INFO` & `pydeck-carto-0.2.1b0/pydeck_carto.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeck-carto
-Version: 0.2.0b0
+Version: 0.2.1b0
 Summary: Pydeck wrapper for use with CARTO
 Home-page: https://github.com/visgl/deck.gl/tree/master/bindings/pydeck-carto
 Author: CARTO
 Author-email: jarroyo@carto.com
 License: BSD 3-Clause
 Keywords: pydeck,carto,visualization,graphics,GIS,maps
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,21 +56,23 @@
 
 # Authentication with CARTO
 carto_auth = CartoAuth.from_oauth()
 
 # Register new layer types in pydeck
 pdkc.register_layers()
 
-# Render CARTO layer in pydeck
+# Create CARTO data source
 data = pdkc.sources.vector_query_source(
     access_token=carto_auth.get_access_token(),
     api_base_url=carto_auth.get_api_base_url(),
     connection_name="carto_dw",
     sql_query="SELECT geom, name FROM carto-demo-data.demo_tables.world_airports",
 )
+
+# Render CARTO layer in pydeck
 layer = pdk.Layer(
     "VectorTileLayer",
     data=data,
     get_fill_color=[238, 77, 90],
     point_radius_min_pixels=2.5,
     pickable=True,
 )
```

### Comparing `pydeck-carto-0.2.0b0/setup.py` & `pydeck-carto-0.2.1b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     author="CARTO",
     author_email="jarroyo@carto.com",
     url="https://github.com/visgl/deck.gl/tree/master/bindings/pydeck-carto",
     license="BSD 3-Clause",
     packages=find_packages(exclude=["examples", "tests"]),
     python_requires=">=3.8",
     install_requires=[
-        "pydeck>=0.8.0",
+        "pydeck>=0.9.0",
         "carto-auth>=0.2.0",
         "typing-extensions>=4.0.0",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Jupyter",
         "Intended Audience :: Developers",
```

