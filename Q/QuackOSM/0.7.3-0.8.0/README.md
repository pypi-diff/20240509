# Comparing `tmp/quackosm-0.7.3.tar.gz` & `tmp/quackosm-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quackosm-0.7.3.tar", last modified: Tue May  7 15:07:10 2024, max compression
+gzip compressed data, was "quackosm-0.8.0.tar", last modified: Thu May  9 08:31:35 2024, max compression
```

## Comparing `quackosm-0.7.3.tar` & `quackosm-0.8.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11339 2024-05-07 15:06:41.640138 quackosm-0.7.3/LICENSE
--rw-r--r--   0        0        0    27879 2024-05-07 15:06:41.640138 quackosm-0.7.3/README.md
--rw-r--r--   0        0        0     4378 2024-05-07 15:07:10.152255 quackosm-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      560 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/__init__.py
--rw-r--r--   0        0        0      464 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/__main__.py
--rw-r--r--   0        0        0      127 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_constants.py
--rw-r--r--   0        0        0      181 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_exceptions.py
--rw-r--r--   0        0        0     6497 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_osm_tags_filters.py
--rw-r--r--   0        0        0     1188 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_osm_way_polygon_features.py
--rw-r--r--   0        0        0    12674 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_rich_progress.py
--rw-r--r--   0        0        0      717 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_typing.py
--rw-r--r--   0        0        0    24446 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/cli.py
--rw-r--r--   0        0        0     2031 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/conftest.py
--rw-r--r--   0        0        0    53246 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/functions.py
--rw-r--r--   0        0        0    19193 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/__init__.py
--rw-r--r--   0        0        0     2320 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/_poly_parser.py
--rw-r--r--   0        0        0     2941 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/bbbike.py
--rw-r--r--   0        0        0      251 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/extract.py
--rw-r--r--   0        0        0     1709 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/geofabrik.py
--rw-r--r--   0        0        0     4376 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/osm_fr.py
--rw-r--r--   0        0        0     3362 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_way_polygon_features.json
--rw-r--r--   0        0        0   110453 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/pbf_file_reader.py
--rw-r--r--   0        0        0       33 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/__init__.py
--rw-r--r--   0        0        0       38 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/__init__.py
--rw-r--r--   0        0        0      746 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/conftest.py
--rw-r--r--   0        0        0    24831 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/test_cli.py
--rw-r--r--   0        0        0     5422 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/test_osm_extracts.py
--rw-r--r--   0        0        0    29285 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/test_osm_tags_filtering.py
--rw-r--r--   0        0        0    36528 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/test_pbf_file_reader.py
--rw-r--r--   0        0        0       43 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/benchmark/__init__.py
--rw-r--r--   0        0        0      945 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/benchmark/test_big_file.py
--rw-r--r--   0        0        0      238 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/conftest.py
--rw-r--r--   0        0        0     1472 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/optional_imports/test_optional_cli_dependency.py
--rw-r--r--   0        0        0      342 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-05-07 15:06:41.656138 quackosm-0.7.3/tests/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0    91717 2024-05-07 15:06:41.656138 quackosm-0.7.3/tests/test_files/monaco_boundary.geojson
--rw-r--r--   0        0        0      112 2024-05-07 15:06:41.656138 quackosm-0.7.3/tests/test_files/osm_tags_filter.json
--rw-r--r--   0        0        0    29715 1970-01-01 00:00:00.000000 quackosm-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-05-09 08:31:06.335242 quackosm-0.8.0/LICENSE
+-rw-r--r--   0        0        0    27910 2024-05-09 08:31:06.335242 quackosm-0.8.0/README.md
+-rw-r--r--   0        0        0     4538 2024-05-09 08:31:35.423438 quackosm-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      560 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/__main__.py
+-rw-r--r--   0        0        0      127 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_constants.py
+-rw-r--r--   0        0        0      181 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_exceptions.py
+-rw-r--r--   0        0        0     6497 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_osm_tags_filters.py
+-rw-r--r--   0        0        0     1188 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_osm_way_polygon_features.py
+-rw-r--r--   0        0        0    11246 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_rich_progress.py
+-rw-r--r--   0        0        0      717 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_typing.py
+-rw-r--r--   0        0        0    24503 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/cli.py
+-rw-r--r--   0        0        0     2031 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/conftest.py
+-rw-r--r--   0        0        0    54717 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/functions.py
+-rw-r--r--   0        0        0    19193 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/__init__.py
+-rw-r--r--   0        0        0     2320 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/_poly_parser.py
+-rw-r--r--   0        0        0     2941 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/bbbike.py
+-rw-r--r--   0        0        0      251 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/extract.py
+-rw-r--r--   0        0        0     1709 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/geofabrik.py
+-rw-r--r--   0        0        0     4376 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/osm_fr.py
+-rw-r--r--   0        0        0     3362 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_way_polygon_features.json
+-rw-r--r--   0        0        0   112604 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/pbf_file_reader.py
+-rw-r--r--   0        0        0       33 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/__init__.py
+-rw-r--r--   0        0        0      746 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/conftest.py
+-rw-r--r--   0        0        0    24603 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/test_cli.py
+-rw-r--r--   0        0        0     5422 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/test_osm_extracts.py
+-rw-r--r--   0        0        0    29285 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/test_osm_tags_filtering.py
+-rw-r--r--   0        0        0    37132 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/test_pbf_file_reader.py
+-rw-r--r--   0        0        0       43 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/benchmark/__init__.py
+-rw-r--r--   0        0        0      945 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/benchmark/test_big_file.py
+-rw-r--r--   0        0        0      238 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     1456 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/optional_imports/test_optional_cli_dependency.py
+-rw-r--r--   0        0        0      342 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0    91717 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/monaco_boundary.geojson
+-rw-r--r--   0        0        0      112 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/osm_tags_filter.json
+-rw-r--r--   0        0        0    29811 1970-01-01 00:00:00.000000 quackosm-0.8.0/PKG-INFO
```

### Comparing `quackosm-0.7.3/LICENSE` & `quackosm-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/README.md` & `quackosm-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,50 +68,50 @@
 
 ### Dependencies
 
 Required:
 
 - `duckdb (>=0.10.2)`: For all DuckDB operations on PBF files
 
-- `pyarrow (>=13.0.0)`: For parquet files wrangling
+- `pyarrow (>=14.0.0)`: For parquet files wrangling
 
 - `pyarrow-ops`: For easy removal of duplicated features in parquet files
 
 - `geoarrow-pyarrow (>=0.1.2)`: For GeoParquet IO operations
 
-- `geopandas`: For returning GeoDataFrames and reading Geo files
+- `geopandas (>=0.6)`: For returning GeoDataFrames and reading Geo files
 
 - `shapely (>=2.0)`: For parsing WKT and GeoJSON strings and fixing geometries
 
-- `typeguard`: For internal validation of types
+- `polars (>=0.19.4)`: For faster OSM ways grouping operation
 
-- `psutil`: For automatic scaling of parameters based on available resources
+- `typeguard (>=3.0)`: For internal validation of types
 
-- `pooch`: For downloading `*.osm.pbf` files
+- `psutil (>=5.6.2)`: For automatic scaling of parameters based on available resources
 
-- `tqdm`: For showing progress bars
+- `pooch (>=1.6.0)`: For downloading `*.osm.pbf` files
+
+- `rich (>=10.11.0)` & `tqdm (>=4.42.0)`: For showing progress bars
 
 - `requests`: For iterating OSM PBF files services
 
 - `beautifulsoup4`: For parsing HTML files and scraping required information
 
 
 Optional:
 
 - `typer[all] (>=0.9.0)` (click, colorama, rich, shellingham): For CLI
 
-- `osmnx`: For geocoding of strings in CLI
+- `osmnx (>=1.3.0)`: For geocoding of strings in CLI
 
 - `h3 (>=4.0.0b1)`: For reading H3 strings in CLI
 
-- `h3ronpy (>=0.18.0)`: For transforming H3 indexes into geometries
-
-- `s2`: For transforming S2 indexes into geometries
+- `s2 (>=0.1.9)`: For transforming S2 indexes into geometries
 
-- `python-geohash`: For transforming GeoHash indexes into geometries
+- `python-geohash (>=0.8)`: For transforming GeoHash indexes into geometries
 
 ## Usage
 
 ### If you already have downloaded the PBF file 📁🗺️
 
 #### Load data as a GeoDataFrame
 
@@ -137,15 +137,15 @@
 
 #### Just convert PBF to GeoParquet
 
 ```python
 >>> import quackosm as qosm
 >>> gpq_path = qosm.convert_pbf_to_gpq(monaco_pbf_path)
 >>> gpq_path.as_posix()
-'files/monaco_nofilter_noclip_compact.geoparquet'
+'files/monaco_nofilter_noclip_compact.parquet'
 ```
 
 #### Inspect the file with duckdb
 
 ```python
 >>> import duckdb
 >>> duckdb.load_extension('spatial')
@@ -223,15 +223,15 @@
 ⠋ [27.2/32] Saving relations outer parts - invalid geometries • 0:00:00
 ⠋ [  28/32] Saving relations outer parts with holes • 0:00:00
 ⠋ [  29/32] Saving relations outer parts without holes • 0:00:00
 ⠙ [  30/32] Saving filtered relations with geometries • 0:00:00
 ⠹ [31.1/32] Saving valid features • 0:00:00
 ⠋ [  32/32] Saving final geoparquet file • 0:00:00
 Finished operation in 0:00:06
-files/monaco_nofilter_noclip_compact.geoparquet
+files/monaco_nofilter_noclip_compact.parquet
 ```
 
 ### Let the QuackOSM automatically download the required OSM PBF files for you 🔎🌍
 
 #### Load data as a GeoDataFrame
 
 ```python
@@ -262,15 +262,15 @@
 >>> import quackosm as qosm
 >>> from shapely import from_wkt
 >>> geometry = from_wkt(
 ...     "POLYGON ((14.4861 35.9107, 14.4861 35.8811, 14.5331 35.8811, 14.5331 35.9107, 14.4861 35.9107))"
 ... )
 >>> gpq_path = qosm.convert_geometry_to_gpq(geometry)
 >>> gpq_path.as_posix()
-'files/4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.geoparquet'
+'files/4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.parquet'
 ```
 
 #### Inspect the file with duckdb
 
 ```python
 >>> import duckdb
 >>> duckdb.load_extension('spatial')
@@ -349,15 +349,15 @@
 ⠋ [27.2/32] Saving relations outer parts - invalid geometries • 0:00:00
 ⠋ [  28/32] Saving relations outer parts with holes • 0:00:00
 ⠋ [  29/32] Saving relations outer parts without holes • 0:00:00
 ⠙ [  30/32] Saving filtered relations with geometries • 0:00:00
 ⠸ [31.1/32] Saving valid features • 0:00:00
 ⠋ [  32/32] Saving final geoparquet file • 0:00:00
 Finished operation in 0:00:39
-files/9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.geoparquet
+files/9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.parquet
 ```
 
 CLI Help output (`QuackOSM -h`):
 ![CLI Help output](https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/cli_help.png)
 
 You can find full API + more examples in the [docs](https://kraina-ai.github.io/quackosm/).
 
@@ -407,34 +407,34 @@
 
 Library utilizes caching system to reduce repeatable computations.
 
 By default, the library is saving results in the `files` directory created in the working directory. Result file name is generated based on the original `*.osm.pbf` file name.
 
 Original file name to be converted: `example.osm.pbf`.
 
-Default output without any filtering: `example_nofilter_noclip_compact.geoparquet`.
+Default output without any filtering: `example_nofilter_noclip_compact.parquet`.
 
 The nofilter part can be replaced by the hash of OSM tags provided for filtering.
-`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.geoparquet`
+`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.parquet`
 
 The noclip part can be replaced by the hash of geometry used for filtering.
-`example_nofilter_430020b6b1ba7bef8ea919b2fb4472dab2972c70a2abae253760a56c29f449c4_compact.geoparquet`
+`example_nofilter_430020b6b1ba7bef8ea919b2fb4472dab2972c70a2abae253760a56c29f449c4_compact.parquet`
 
 The `compact` part can also take the form of `exploded`, it represents the form of OSM tags - either kept together in a single dictionary or split into columns.
 
 When filtering by selecting individual features IDs, an additional hash based on those IDs is appended to the file.
-`example_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.geoparquet`
+`example_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.parquet`
 
 When the `keep_all_tags` parameter is passed while filtering by OSM tags, and additional `alltags` component is added after the osm filter hash part.
-`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.geoparquet`
+`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.parquet`
 
 General schema of multiple segments that are concatenated together:
-`pbf_file_name`\_(`osm_filter_tags_hash_part`/`nofilter`)(\_`alltags`)\_(`clipping_geometry_hash_part`/`noclip`)\_(`compact`/`exploded`)(\_`filter_osm_ids_hash_part`).geoparquet
+`pbf_file_name`\_(`osm_filter_tags_hash_part`/`nofilter`)(\_`alltags`)\_(`clipping_geometry_hash_part`/`noclip`)\_(`compact`/`exploded`)(\_`filter_osm_ids_hash_part`).parquet
 
-> If the WKT mode is turned on, then the result file will be saved with a `parquet` extension and a `_wkt` suffix.
+> If the WKT mode is turned on, then the result file will be saved with a `_wkt` suffix.
 
 ### Memory usage
 
 DuckDB queries requiring `JOIN`, `GROUP` and `ORDER BY` operations are very memory intensive. Because of that, some steps are divided into chunks (groups) with a set number of rows per chunk.
 
 QuackOSM has been roughly tuned to different workloads. The `rows_per_group` variable is set based on an available memory in the system:
 
@@ -443,20 +443,20 @@
 |     < 8 GB |        100 000 |
 |  8 - 16 GB |        500 000 |
 | 16 - 24 GB |      1 000 000 |
 |    > 24 GB |      5 000 000 |
 
 > WSL usage: sometimes code can break since DuckDB is trying to use all available memory, that can be occupied by Windows.
 
-### Disk usage
+### Resources usage
 
 The algorithm depends on saving intermediate `.parquet` files between queries.
 As a rule of thumb, when parsing a full file without filtering, you should have at least 10x more free space on disk than the base file size (100MB pbf file -> 1GB free space to parse it).
 
-Below you can see the chart of disk usage during operation. Generated on a machine with AMD Ryzen 7 5800X CPU (16 threads, 3.8 GHz clock speed) and 24 GB of RAM.
+Below you can see the chart of resources usage during operation. Generated on a Github Actions Ubuntu virtual machine with 4 threads and 16 GB of memory.
 
 #### Monaco
 
 PBF file size: 525 KB
 
 [Geofabrik link](https://download.geofabrik.de/europe/monaco.html)
```

#### html2text {}

```diff
@@ -17,48 +17,49 @@
 as Python module as well as a beautiful CLI based on `Typer`[^4]. [^1]: [DuckDB
 Website](https://duckdb.org/) [^2]: [DuckDB Spatial extension repository]
 (https://github.com/duckdb/duckdb_spatial) [^3]: [GeoParquet data format]
 (https://geoparquet.org/) [^4]: [Typer docs](https://typer.tiangolo.com/) ##
 Installing ### As pure Python module ``` pip install quackosm ``` ### With
 beautiful CLI ``` pip install quackosm[cli] ``` ### Required Python version?
 QuackOSM supports **Python >= 3.9** ### Dependencies Required: - `duckdb
-(>=0.10.2)`: For all DuckDB operations on PBF files - `pyarrow (>=13.0.0)`: For
+(>=0.10.2)`: For all DuckDB operations on PBF files - `pyarrow (>=14.0.0)`: For
 parquet files wrangling - `pyarrow-ops`: For easy removal of duplicated
 features in parquet files - `geoarrow-pyarrow (>=0.1.2)`: For GeoParquet IO
-operations - `geopandas`: For returning GeoDataFrames and reading Geo files -
-`shapely (>=2.0)`: For parsing WKT and GeoJSON strings and fixing geometries -
-`typeguard`: For internal validation of types - `psutil`: For automatic scaling
-of parameters based on available resources - `pooch`: For downloading
-`*.osm.pbf` files - `tqdm`: For showing progress bars - `requests`: For
-iterating OSM PBF files services - `beautifulsoup4`: For parsing HTML files and
-scraping required information Optional: - `typer[all] (>=0.9.0)` (click,
-colorama, rich, shellingham): For CLI - `osmnx`: For geocoding of strings in
-CLI - `h3 (>=4.0.0b1)`: For reading H3 strings in CLI - `h3ronpy (>=0.18.0)`:
-For transforming H3 indexes into geometries - `s2`: For transforming S2 indexes
-into geometries - `python-geohash`: For transforming GeoHash indexes into
-geometries ## Usage ### If you already have downloaded the PBF file ððºï¸
-#### Load data as a GeoDataFrame ```python >>> import quackosm as qosm >>>
-qosm.get_features_gdf(monaco_pbf_path) tags geometry feature_id node/
-10005045289 {'shop': 'bakery'} POINT (7.42245 43.73105) node/10020887517
-{'leisure': 'swimming_pool', ... POINT (7.41316 43.73384) node/10021298117
-{'leisure': 'swimming_pool', ... POINT (7.42777 43.74277) node/10021298717
-{'leisure': 'swimming_pool', ... POINT (7.42630 43.74097) node/10025656383
-{'ferry': 'yes', 'name': 'Qua... POINT (7.42550 43.73690) ... ... ... way/
-990669427 {'amenity': 'shelter', 'shelt... POLYGON ((7.41461 43.7338... way/
-990669428 {'highway': 'secondary', 'jun... LINESTRING (7.41366 43.73... way/
-990669429 {'highway': 'secondary', 'jun... LINESTRING (7.41376 43.73... way/
-990848785 {'addr:city': 'Monaco', 'addr... POLYGON ((7.41426 43.7339... way/
-993121275 {'building': 'yes', 'name': ... POLYGON ((7.43214 43.7481... [7906
-rows x 2 columns] ``` #### Just convert PBF to GeoParquet ```python >>> import
-quackosm as qosm >>> gpq_path = qosm.convert_pbf_to_gpq(monaco_pbf_path) >>>
-gpq_path.as_posix() 'files/monaco_nofilter_noclip_compact.geoparquet' ``` ####
-Inspect the file with duckdb ```python >>> import duckdb >>>
-duckdb.load_extension('spatial') >>> duckdb.read_parquet(str(gpq_path)).project
-( ... "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)" ... ).order
-("feature_id")
+operations - `geopandas (>=0.6)`: For returning GeoDataFrames and reading Geo
+files - `shapely (>=2.0)`: For parsing WKT and GeoJSON strings and fixing
+geometries - `polars (>=0.19.4)`: For faster OSM ways grouping operation -
+`typeguard (>=3.0)`: For internal validation of types - `psutil (>=5.6.2)`: For
+automatic scaling of parameters based on available resources - `pooch
+(>=1.6.0)`: For downloading `*.osm.pbf` files - `rich (>=10.11.0)` & `tqdm
+(>=4.42.0)`: For showing progress bars - `requests`: For iterating OSM PBF
+files services - `beautifulsoup4`: For parsing HTML files and scraping required
+information Optional: - `typer[all] (>=0.9.0)` (click, colorama, rich,
+shellingham): For CLI - `osmnx (>=1.3.0)`: For geocoding of strings in CLI -
+`h3 (>=4.0.0b1)`: For reading H3 strings in CLI - `s2 (>=0.1.9)`: For
+transforming S2 indexes into geometries - `python-geohash (>=0.8)`: For
+transforming GeoHash indexes into geometries ## Usage ### If you already have
+downloaded the PBF file ððºï¸ #### Load data as a GeoDataFrame ```python
+>>> import quackosm as qosm >>> qosm.get_features_gdf(monaco_pbf_path) tags
+geometry feature_id node/10005045289 {'shop': 'bakery'} POINT (7.42245
+43.73105) node/10020887517 {'leisure': 'swimming_pool', ... POINT (7.41316
+43.73384) node/10021298117 {'leisure': 'swimming_pool', ... POINT (7.42777
+43.74277) node/10021298717 {'leisure': 'swimming_pool', ... POINT (7.42630
+43.74097) node/10025656383 {'ferry': 'yes', 'name': 'Qua... POINT (7.42550
+43.73690) ... ... ... way/990669427 {'amenity': 'shelter', 'shelt... POLYGON (
+(7.41461 43.7338... way/990669428 {'highway': 'secondary', 'jun... LINESTRING
+(7.41366 43.73... way/990669429 {'highway': 'secondary', 'jun... LINESTRING
+(7.41376 43.73... way/990848785 {'addr:city': 'Monaco', 'addr... POLYGON (
+(7.41426 43.7339... way/993121275 {'building': 'yes', 'name': ... POLYGON (
+(7.43214 43.7481... [7906 rows x 2 columns] ``` #### Just convert PBF to
+GeoParquet ```python >>> import quackosm as qosm >>> gpq_path =
+qosm.convert_pbf_to_gpq(monaco_pbf_path) >>> gpq_path.as_posix() 'files/
+monaco_nofilter_noclip_compact.parquet' ``` #### Inspect the file with duckdb
+```python >>> import duckdb >>> duckdb.load_extension('spatial') >>>
+duckdb.read_parquet(str(gpq_path)).project( ... "* REPLACE (ST_GeomFromWKB
+(geometry) AS geometry)" ... ).order("feature_id")
 ââââââââââââââââââââ¬âââââââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââ
 â feature_id â tags â geometry â â varchar â map(varchar, varchâ¦
 â geometry â
 ââââââââââââââââââââ¼âââââââââââââââââââââââ¼âââââââââââââââââââââââââââââââââââââââââââââââ¤
 â node/10005045289 â {shop=bakery} â POINT (7.4224498 43.7310532) â â
 node/10020887517 â {leisure=swimming_â¦ â POINT (7.4131561 43.7338391) â
 â node/10021298117 â {leisure=swimming_â¦ â POINT (7.4277743 43.7427669)
@@ -117,35 +118,35 @@
 Saving relations inner parts - invalid geometries â¢ 0:00:00 â  [27.1/32]
 Saving relations outer parts - valid geometries â¢ 0:00:00 â  [27.2/32]
 Saving relations outer parts - invalid geometries â¢ 0:00:00 â  [ 28/32]
 Saving relations outer parts with holes â¢ 0:00:00 â  [ 29/32] Saving
 relations outer parts without holes â¢ 0:00:00 â  [ 30/32] Saving filtered
 relations with geometries â¢ 0:00:00 â ¹ [31.1/32] Saving valid features â¢
 0:00:00 â  [ 32/32] Saving final geoparquet file â¢ 0:00:00 Finished
-operation in 0:00:06 files/monaco_nofilter_noclip_compact.geoparquet ``` ###
-Let the QuackOSM automatically download the required OSM PBF files for you
-ðð #### Load data as a GeoDataFrame ```python >>> import quackosm as qosm
->>> import osmnx as ox >>> geometry = ox.geocode_to_gdf("Vatican
-City").unary_union >>> qosm.get_features_gdf_from_geometry(geometry) tags
-geometry feature_id node/10253371713 {'crossing': 'uncontrolled',... POINT
-(12.45603 41.90454) node/10253371714 {'highway': 'stop'} POINT (12.45705
-41.90400) node/10253371715 {'highway': 'stop'} POINT (12.45242 41.90164) node/
-10253371720 {'artwork_type': 'statue',... POINT (12.45147 41.90484) node/
-10253371738 {'natural': 'tree'} POINT (12.45595 41.90609) ... ... ... way/
-983015528 {'barrier': 'hedge', 'height'... POLYGON ((12.45027 41.901... way/
-983015529 {'barrier': 'hedge', 'height'... POLYGON ((12.45028 41.901... way/
-983015530 {'barrier': 'hedge', 'height'... POLYGON ((12.45023 41.901... way/
-998561138 {'barrier': 'bollard', 'bicyc... LINESTRING (12.45821 41.9... way/
-998561139 {'barrier': 'bollard', 'bicyc... LINESTRING (12.45828 41.9... [3286
-rows x 2 columns] ``` #### Just convert geometry to GeoParquet ```python >>>
-import quackosm as qosm >>> from shapely import from_wkt >>> geometry =
-from_wkt( ... "POLYGON ((14.4861 35.9107, 14.4861 35.8811, 14.5331 35.8811,
-14.5331 35.9107, 14.4861 35.9107))" ... ) >>> gpq_path =
-qosm.convert_geometry_to_gpq(geometry) >>> gpq_path.as_posix() 'files/
-4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.geoparquet'
+operation in 0:00:06 files/monaco_nofilter_noclip_compact.parquet ``` ### Let
+the QuackOSM automatically download the required OSM PBF files for you ðð
+#### Load data as a GeoDataFrame ```python >>> import quackosm as qosm >>>
+import osmnx as ox >>> geometry = ox.geocode_to_gdf("Vatican City").unary_union
+>>> qosm.get_features_gdf_from_geometry(geometry) tags geometry feature_id
+node/10253371713 {'crossing': 'uncontrolled',... POINT (12.45603 41.90454)
+node/10253371714 {'highway': 'stop'} POINT (12.45705 41.90400) node/10253371715
+{'highway': 'stop'} POINT (12.45242 41.90164) node/10253371720 {'artwork_type':
+'statue',... POINT (12.45147 41.90484) node/10253371738 {'natural': 'tree'}
+POINT (12.45595 41.90609) ... ... ... way/983015528 {'barrier': 'hedge',
+'height'... POLYGON ((12.45027 41.901... way/983015529 {'barrier': 'hedge',
+'height'... POLYGON ((12.45028 41.901... way/983015530 {'barrier': 'hedge',
+'height'... POLYGON ((12.45023 41.901... way/998561138 {'barrier': 'bollard',
+'bicyc... LINESTRING (12.45821 41.9... way/998561139 {'barrier': 'bollard',
+'bicyc... LINESTRING (12.45828 41.9... [3286 rows x 2 columns] ``` #### Just
+convert geometry to GeoParquet ```python >>> import quackosm as qosm >>> from
+shapely import from_wkt >>> geometry = from_wkt( ... "POLYGON ((14.4861
+35.9107, 14.4861 35.8811, 14.5331 35.8811, 14.5331 35.9107, 14.4861 35.9107))"
+... ) >>> gpq_path = qosm.convert_geometry_to_gpq(geometry) >>>
+gpq_path.as_posix() 'files/
+4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.parquet'
 ``` #### Inspect the file with duckdb ```python >>> import duckdb >>>
 duckdb.load_extension('spatial') >>> duckdb.read_parquet(str(gpq_path)).project
 ( ... "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)" ... ).order
 ("feature_id")
 ââââââââââââââââââââ¬âââââââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââ
 â feature_id â tags â geometry â â varchar â map(varchar, varchâ¦
 â geometry â
@@ -212,15 +213,15 @@
 Saving relations outer parts - valid geometries â¢ 0:00:00 â  [27.2/32]
 Saving relations outer parts - invalid geometries â¢ 0:00:00 â  [ 28/32]
 Saving relations outer parts with holes â¢ 0:00:00 â  [ 29/32] Saving
 relations outer parts without holes â¢ 0:00:00 â  [ 30/32] Saving filtered
 relations with geometries â¢ 0:00:00 â ¸ [31.1/32] Saving valid features â¢
 0:00:00 â  [ 32/32] Saving final geoparquet file â¢ 0:00:00 Finished
 operation in 0:00:39 files/
-9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.geoparquet
+9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.parquet
 ``` CLI Help output (`QuackOSM -h`): ![CLI Help output](https://
 raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
 cli_help.png) You can find full API + more examples in the [docs](https://
 kraina-ai.github.io/quackosm/). ## How does it work? ### Basic logic QuackOSM
 utilizes `ST_ReadOSM` function from `DuckDB`'s `Spatial` extension to read raw
 data from the PBF file: - **Nodes** with coordinates and tags; - **Ways** with
 nodes refs and tags; - **Relations** with nodes and ways refs, ref roles and
@@ -249,52 +250,51 @@
 with weird artifacts by `GDAL`. You can inspect the comparison algorithm in the
 `test_gdal_parity` function from `tests/base/test_pbf_file_reader.py` file. ###
 Caching Library utilizes caching system to reduce repeatable computations. By
 default, the library is saving results in the `files` directory created in the
 working directory. Result file name is generated based on the original
 `*.osm.pbf` file name. Original file name to be converted: `example.osm.pbf`.
 Default output without any filtering:
-`example_nofilter_noclip_compact.geoparquet`. The nofilter part can be replaced
-by the hash of OSM tags provided for filtering.
-`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.geoparquet`
+`example_nofilter_noclip_compact.parquet`. The nofilter part can be replaced by
+the hash of OSM tags provided for filtering.
+`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.parquet`
 The noclip part can be replaced by the hash of geometry used for filtering.
-`example_nofilter_430020b6b1ba7bef8ea919b2fb4472dab2972c70a2abae253760a56c29f449c4_compact.geoparquet`
+`example_nofilter_430020b6b1ba7bef8ea919b2fb4472dab2972c70a2abae253760a56c29f449c4_compact.parquet`
 The `compact` part can also take the form of `exploded`, it represents the form
 of OSM tags - either kept together in a single dictionary or split into
 columns. When filtering by selecting individual features IDs, an additional
 hash based on those IDs is appended to the file.
-`example_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.geoparquet`
+`example_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.parquet`
 When the `keep_all_tags` parameter is passed while filtering by OSM tags, and
 additional `alltags` component is added after the osm filter hash part.
-`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.geoparquet`
+`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.parquet`
 General schema of multiple segments that are concatenated together:
 `pbf_file_name`\_(`osm_filter_tags_hash_part`/`nofilter`)(\_`alltags`)\_
 (`clipping_geometry_hash_part`/`noclip`)\_(`compact`/`exploded`)
-(\_`filter_osm_ids_hash_part`).geoparquet > If the WKT mode is turned on, then
-the result file will be saved with a `parquet` extension and a `_wkt` suffix.
-### Memory usage DuckDB queries requiring `JOIN`, `GROUP` and `ORDER BY`
-operations are very memory intensive. Because of that, some steps are divided
-into chunks (groups) with a set number of rows per chunk. QuackOSM has been
-roughly tuned to different workloads. The `rows_per_group` variable is set
-based on an available memory in the system: | Memory | Rows per group | | -----
-----: | -------------: | | < 8 GB | 100 000 | | 8 - 16 GB | 500 000 | | 16 - 24
-GB | 1 000 000 | | > 24 GB | 5 000 000 | > WSL usage: sometimes code can break
-since DuckDB is trying to use all available memory, that can be occupied by
-Windows. ### Disk usage The algorithm depends on saving intermediate `.parquet`
-files between queries. As a rule of thumb, when parsing a full file without
-filtering, you should have at least 10x more free space on disk than the base
-file size (100MB pbf file -> 1GB free space to parse it). Below you can see the
-chart of disk usage during operation. Generated on a machine with AMD Ryzen 7
-5800X CPU (16 threads, 3.8 GHz clock speed) and 24 GB of RAM. #### Monaco PBF
-file size: 525 KB [Geofabrik link](https://download.geofabrik.de/europe/
-monaco.html) ![Monaco PBF file result](https://raw.githubusercontent.com/
-kraina-ai/quackosm/main/docs/assets/images/monaco_disk_spillage.png) ####
-Estonia PBF file size: 100 MB [Geofabrik link](https://download.geofabrik.de/
-europe/estonia.html) ![Estonia PBF file result](https://
+(\_`filter_osm_ids_hash_part`).parquet > If the WKT mode is turned on, then the
+result file will be saved with a `_wkt` suffix. ### Memory usage DuckDB queries
+requiring `JOIN`, `GROUP` and `ORDER BY` operations are very memory intensive.
+Because of that, some steps are divided into chunks (groups) with a set number
+of rows per chunk. QuackOSM has been roughly tuned to different workloads. The
+`rows_per_group` variable is set based on an available memory in the system: |
+Memory | Rows per group | | ---------: | -------------: | | < 8 GB | 100 000 |
+| 8 - 16 GB | 500 000 | | 16 - 24 GB | 1 000 000 | | > 24 GB | 5 000 000 | >
+WSL usage: sometimes code can break since DuckDB is trying to use all available
+memory, that can be occupied by Windows. ### Resources usage The algorithm
+depends on saving intermediate `.parquet` files between queries. As a rule of
+thumb, when parsing a full file without filtering, you should have at least 10x
+more free space on disk than the base file size (100MB pbf file -> 1GB free
+space to parse it). Below you can see the chart of resources usage during
+operation. Generated on a Github Actions Ubuntu virtual machine with 4 threads
+and 16 GB of memory. #### Monaco PBF file size: 525 KB [Geofabrik link](https:/
+/download.geofabrik.de/europe/monaco.html) ![Monaco PBF file result](https://
 raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
+monaco_disk_spillage.png) #### Estonia PBF file size: 100 MB [Geofabrik link]
+(https://download.geofabrik.de/europe/estonia.html) ![Estonia PBF file result]
+(https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
 estonia_disk_spillage.png) #### Poland PBF file size: 1.7 GB [Geofabrik link]
 (https://download.geofabrik.de/europe/poland.html) ![Poland PBF file result]
 (https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
 poland_disk_spillage.png) ## License The library is distributed under Apache-
 2.0 License. The free [OpenStreetMap](https://www.openstreetmap.org/) data,
 which is used for the development of QuackOSM, is licensed under the [Open Data
 Commons Open Database License](https://opendatacommons.org/licenses/odbl/)
```

### Comparing `quackosm-0.7.3/pyproject.toml` & `quackosm-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [project]
 name = "QuackOSM"
-version = "0.7.3"
+version = "0.8.0"
 description = "An open-source tool for reading OpenStreetMap PBF files using DuckDB"
 authors = [
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
 ]
 dependencies = [
-    "geopandas",
+    "geopandas>=0.6",
     "shapely>=2",
-    "pyarrow>=13.0.0",
+    "pyarrow>=14.0.0",
     "duckdb>=0.10.2",
     "geoarrow-pyarrow>=0.1.2",
-    "typeguard",
-    "psutil",
-    "pooch",
-    "tqdm",
+    "typeguard>=3.0.0",
+    "psutil>=5.6.2",
+    "pooch>=1.6.0",
+    "tqdm>=4.42.0",
     "beautifulsoup4",
     "pyarrow-ops",
     "requests",
+    "polars>=0.19.4",
+    "rich>=10.11.0",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -46,19 +48,18 @@
 Repository = "https://github.com/kraina-ai/quackosm"
 Documentation = "https://kraina-ai.github.io/quackosm"
 Changelog = "https://github.com/kraina-ai/quackosm/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 cli = [
     "typer[all]>=0.9.0",
-    "osmnx",
+    "osmnx>=1.3.0",
     "h3>=4.0.0b1",
-    "h3ronpy>=0.18.0",
-    "s2",
-    "python-geohash",
+    "s2>=0.1.9",
+    "python-geohash>=0.8",
 ]
 
 [project.scripts]
 quackosm = "quackosm.__main__:main"
 QuackOSM = "quackosm.__main__:main"
 
 [build-system]
@@ -67,51 +68,53 @@
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "bumpver",
     "types-requests",
+    "setuptools>=45.0.0",
 ]
 lint = [
     "pre-commit",
-    "mypy",
+    "mypy>=1",
     "docformatter[tomli]",
-    "ruff",
+    "ruff>=0.1.0",
 ]
 test = [
-    "pytest",
+    "pytest>=7.0.0",
     "tox-pdm",
-    "pytest-mock",
+    "pytest-mock>=3.3.0",
     "requests-mock",
     "pytest-check",
     "pytest-parametrization",
-    "pytest-xdist",
+    "pytest-xdist>=3.4.0",
     "pytest-doctestplus",
     "srai>=0.6.2",
 ]
 docs = [
     "mkdocs",
     "mkdocs-material",
     "mkdocs-mermaid2-plugin",
     "mkdocstrings[python]",
     "mkdocs-jupyter",
     "ipykernel",
     "mkdocs-gen-files",
     "mkdocs-awesome-pages-plugin",
-    "mike<2",
+    "mike>=1,<2",
     "black",
     "jupyter",
     "nbconvert",
     "nbformat",
     "notebook",
     "osmnx",
     "matplotlib",
-    "seaborn",
+    "seaborn>=0.10.0",
     "py-cpuinfo",
+    "adjustText",
 ]
 license = [
     "licensecheck",
 ]
 cli-dev = [
     "ipywidgets",
     "folium",
@@ -185,15 +188,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.7.3"
+current_version = "0.8.0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `quackosm-0.7.3/quackosm/__init__.py` & `quackosm-0.8.0/quackosm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     convert_pbf_to_gpq,
     get_features_gdf,
     get_features_gdf_from_geometry,
 )
 from quackosm.pbf_file_reader import PbfFileReader
 
 __app_name__ = "QuackOSM"
-__version__ = "0.7.3"
+__version__ = "0.8.0"
 
 __all__ = [
     "PbfFileReader",
     "convert_pbf_to_gpq",
     "convert_geometry_to_gpq",
     "get_features_gdf",
     "get_features_gdf_from_geometry",
```

### Comparing `quackosm-0.7.3/quackosm/_osm_tags_filters.py` & `quackosm-0.8.0/quackosm/_osm_tags_filters.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/_osm_way_polygon_features.py` & `quackosm-0.8.0/quackosm/_osm_way_polygon_features.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/_rich_progress.py` & `quackosm-0.8.0/quackosm/_rich_progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,83 @@
 # type: ignore
 """Wrapper over Rich progress bar."""
 
+import json
 import os
 import time
 from collections.abc import Iterable
-from contextlib import suppress
 from datetime import timedelta
-from typing import Any, Literal, Optional
+from types import TracebackType
+from typing import Any, Literal, Optional, Union
+
+from rich import print as rprint
+from rich.progress import (
+    BarColumn,
+    Console,
+    Live,
+    MofNCompleteColumn,
+    Progress,
+    ProgressColumn,
+    SpinnerColumn,
+    Task,
+    Text,
+    TextColumn,
+    TimeElapsedColumn,
+    TimeRemainingColumn,
+)
 
 __all__ = ["TaskProgressSpinner", "TaskProgressBar"]
 
 TOTAL_STEPS = 32
 
 
 def log_message(message: str) -> None:
-    try:  # pragma: no cover
-        from rich import print as rprint
-
-        rprint(message)
-    except ImportError:
-        print(message)
+    rprint(message)
 
 
 def show_total_elapsed_time(elapsed_seconds: float) -> None:
-    with suppress(ImportError):  # pragma: no cover
-        from rich import print as rprint
+    elapsed_time_formatted = str(timedelta(seconds=int(elapsed_seconds)))
+    rprint(f"Finished operation in [progress.elapsed]{elapsed_time_formatted}")
+
+
+class SpeedColumn(ProgressColumn):
+    def render(self, task: "Task") -> Text:
+        if task.speed is None:
+            return Text("")
+        elif task.speed >= 1:
+            return Text(f"{task.speed:.2f} it/s")
+        else:
+            return Text(f"{1/task.speed:.2f} s/it")  # noqa: FURB126
+
+
+class TransientProgress(Progress):
+    def __init__(self, *columns: Union[str, ProgressColumn], live_obj: Live, **kwargs) -> None:
+        super().__init__(*columns, **kwargs)
+        self.live = live_obj
+        self.live._get_renderable = self.get_renderable
 
-        elapsed_time_formatted = str(timedelta(seconds=int(elapsed_seconds)))
-        rprint(f"Finished operation in [progress.elapsed]{elapsed_time_formatted}")
+    def start(self) -> None:
+        if not self.live.transient:
+            super().start()
+
+    def stop(self) -> None:
+        if not self.live.transient:
+            super().stop()
+
+    def __enter__(self) -> Progress:
+        self.start()
+        return self
+
+    def __exit__(
+        self,
+        exc_type: Optional[type[BaseException]],
+        exc_val: Optional[BaseException],
+        exc_tb: Optional[TracebackType],
+    ) -> None:
+        self.stop()
 
 
 class TaskProgressSpinner:
     def __init__(
         self,
         step_name: str,
         step_number: str,
@@ -47,42 +93,36 @@
         self.transient_mode = transient_mode
         self.skip_step_number = skip_step_number
         self.progress = None
         self.progress_cls = progress_cls
         self.live_obj = live_obj
 
     def __enter__(self):
-        try:  # pragma: no cover
-            if self.silent_mode:
-                self.progress = None
-            else:
-                from rich.progress import SpinnerColumn, TextColumn, TimeElapsedColumn
-
-                columns = [
-                    SpinnerColumn(),
-                    TextColumn(self.step_number),
-                    TextColumn("[progress.description]{task.description}"),
-                    TextColumn("•"),
-                    TimeElapsedColumn(),
-                ]
-
-                if self.skip_step_number:
-                    columns.pop(1)
-
-                self.progress = self.progress_cls(
-                    *columns,
-                    live_obj=self.live_obj,
-                    transient=self.transient_mode,
-                )
-
-                self.progress.__enter__()
-                self.progress.add_task(description=self.step_name, total=None)
-
-        except ImportError:
+        if self.silent_mode:
             self.progress = None
+        else:
+            columns = [
+                SpinnerColumn(),
+                TextColumn(self.step_number),
+                TextColumn("[progress.description]{task.description}"),
+                TextColumn("•"),
+                TimeElapsedColumn(),
+            ]
+
+            if self.skip_step_number:
+                columns.pop(1)
+
+            self.progress = self.progress_cls(
+                *columns,
+                live_obj=self.live_obj,
+                transient=self.transient_mode,
+            )
+
+            self.progress.__enter__()
+            self.progress.add_task(description=self.step_name, total=None)
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         if self.progress:
             self.progress.__exit__(exc_type, exc_value, exc_tb)
 
         self.progress = None
 
@@ -104,70 +144,46 @@
         self.transient_mode = transient_mode
         self.skip_step_number = skip_step_number
         self.progress = None
         self.progress_cls = progress_cls
         self.live_obj = live_obj
 
     def __enter__(self):
-        try:  # pragma: no cover
-            if self.silent_mode:
-                self.progress = None
-            else:
-                from rich.progress import (
-                    BarColumn,
-                    MofNCompleteColumn,
-                    ProgressColumn,
-                    SpinnerColumn,
-                    Task,
-                    Text,
-                    TextColumn,
-                    TimeElapsedColumn,
-                    TimeRemainingColumn,
-                )
-
-                class SpeedColumn(ProgressColumn):
-                    def render(self, task: "Task") -> Text:
-                        if task.speed is None:
-                            return Text("")
-                        elif task.speed >= 1:
-                            return Text(f"{task.speed:.2f} it/s")
-                        else:
-                            return Text(f"{1/task.speed:.2f} s/it")  # noqa: FURB126
-
-                columns = [
-                    SpinnerColumn(),
-                    TextColumn(self.step_number),
-                    TextColumn(
-                        "[progress.description]{task.description}"
-                        " [progress.percentage]{task.percentage:>3.0f}%"
-                    ),
-                    BarColumn(),
-                    MofNCompleteColumn(),
-                    TextColumn("•"),
-                    TimeElapsedColumn(),
-                    TextColumn("<"),
-                    TimeRemainingColumn(),
-                    TextColumn("•"),
-                    SpeedColumn(),
-                ]
-
-                if self.skip_step_number:
-                    columns.pop(1)
-
-                self.progress = self.progress_cls(
-                    *columns,
-                    live_obj=self.live_obj,
-                    transient=self.transient_mode,
-                    speed_estimate_period=1800,
-                )
+        if self.silent_mode:
+            self.progress = None
+        else:
 
-                self.progress.__enter__()
+            columns = [
+                SpinnerColumn(),
+                TextColumn(self.step_number),
+                TextColumn(
+                    "[progress.description]{task.description}"
+                    " [progress.percentage]{task.percentage:>3.0f}%"
+                ),
+                BarColumn(),
+                MofNCompleteColumn(),
+                TextColumn("•"),
+                TimeElapsedColumn(),
+                TextColumn("<"),
+                TimeRemainingColumn(),
+                TextColumn("•"),
+                SpeedColumn(),
+            ]
+
+            if self.skip_step_number:
+                columns.pop(1)
+
+            self.progress = self.progress_cls(
+                *columns,
+                live_obj=self.live_obj,
+                transient=self.transient_mode,
+                speed_estimate_period=1800,
+            )
 
-        except ImportError:
-            self.progress = None
+            self.progress.__enter__()
 
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         if self.progress:
             self.progress.__exit__(exc_type, exc_value, exc_tb)
 
@@ -184,75 +200,43 @@
 
 class TaskProgressTracker:
     def __init__(
         self,
         verbosity_mode: Literal["silent", "transient", "verbose"] = "verbose",
         total_major_steps: int = 1,
         current_major_step: int = 1,
+        debug: bool = False,
     ):
         self.verbosity_mode = verbosity_mode
         self.major_step_number: int = 0
         self.minor_step_number: Optional[int] = None
         self.total_major_steps = total_major_steps
         self.current_major_step = current_major_step
         self.transient_progress_cls = None
         self.live = None
         self.console = None
+        self.debug = debug
+        self.steps_times = {}
+        self.start_time = time.time()
 
         if total_major_steps > 1:
             number_width = len(str(total_major_steps))
             self.major_steps_prefix = f"[{current_major_step: >{number_width}}/{total_major_steps}]"
         else:
             self.major_steps_prefix = ""
 
         if not self.verbosity_mode == "silent":
-            with suppress(ImportError):  # pragma: no cover
-                from types import TracebackType
-                from typing import Union
-
-                from rich.progress import Console, Live, Progress, ProgressColumn
-
-                self.force_terminal = os.getenv("FORCE_TERMINAL_MODE", "false").lower() == "true"
-
-                class TransientProgress(Progress):
-                    def __init__(
-                        self, *columns: Union[str, ProgressColumn], live_obj: Live, **kwargs
-                    ) -> None:
-                        super().__init__(*columns, **kwargs)
-                        self.live = live_obj
-                        self.live._get_renderable = self.get_renderable
-
-                    def start(self) -> None:
-                        if not self.live.transient:
-                            super().start()
-
-                    def stop(self) -> None:
-                        if not self.live.transient:
-                            super().stop()
-
-                    def __enter__(self) -> Progress:
-                        self.start()
-                        return self
-
-                    def __exit__(
-                        self,
-                        exc_type: Optional[type[BaseException]],
-                        exc_val: Optional[BaseException],
-                        exc_tb: Optional[TracebackType],
-                    ) -> None:
-                        self.stop()
-
-                self.console = Console(
-                    force_interactive=False if self.force_terminal else None,
-                    force_jupyter=False if self.force_terminal else None,
-                    force_terminal=True if self.force_terminal else None,
-                )
-                self.transient_progress_cls = TransientProgress
+            self.force_terminal = os.getenv("FORCE_TERMINAL_MODE", "false").lower() == "true"
 
-            self.start_time = time.time()
+            self.console = Console(
+                force_interactive=False if self.force_terminal else None,
+                force_jupyter=False if self.force_terminal else None,
+                force_terminal=True if self.force_terminal else None,
+            )
+            self.transient_progress_cls = TransientProgress
 
     def reset_steps(self, current_major_step):
         self.major_step_number: int = 0
         self.minor_step_number: Optional[int] = None
 
         self.current_major_step = current_major_step
         if self.total_major_steps > 1:
@@ -273,31 +257,30 @@
             self.console.print()
 
         if not self.verbosity_mode == "silent":
             end_time = time.time()
             elapsed_seconds = end_time - self.start_time
             show_total_elapsed_time(elapsed_seconds)
 
+        if self.debug:
+            rprint(f"Steps times: {json.dumps(self.steps_times)}")
+
     def _check_live_obj(self):
         if self.verbosity_mode == "silent":
             return
-
-        with suppress(ImportError):  # pragma: no cover
-            if not self.live or not self.live._started:
-                from rich.progress import Live
-
-                self.live = Live(
-                    console=self.console,
-                    auto_refresh=True,
-                    refresh_per_second=1,
-                    transient=self.verbosity_mode == "transient",
-                    redirect_stdout=True,
-                    redirect_stderr=True,
-                )
-                self.live.start(refresh=True)
+        if not self.live or not self.live._started:
+            self.live = Live(
+                console=self.console,
+                auto_refresh=True,
+                refresh_per_second=1,
+                transient=self.verbosity_mode == "transient",
+                redirect_stdout=True,
+                redirect_stderr=True,
+            )
+            self.live.start(refresh=True)
 
     def get_spinner(
         self,
         step_name: str,
         next_step: Literal["major", "minor"] = "major",
         with_minor_step: bool = False,
     ) -> TaskProgressSpinner:
@@ -366,8 +349,11 @@
 
         step_number = (
             str(self.major_step_number)
             if not self.minor_step_number
             else f"{self.major_step_number}.{self.minor_step_number}"
         )
 
+        if self.debug:
+            self.steps_times[step_number] = round(time.time(), 2)
+
         self.current_step_number = f"{self.major_steps_prefix}[{step_number: >4}/{TOTAL_STEPS}]"
```

### Comparing `quackosm-0.7.3/quackosm/_typing.py` & `quackosm-0.8.0/quackosm/_typing.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/cli.py` & `quackosm-0.8.0/quackosm/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import geopandas as gpd
 import h3
 import osmnx as ox
 import typer
 from click import Argument
 from click.exceptions import MissingParameter
 from geohash import bbox as geohash_bbox
-from h3ronpy.arrow.vector import cells_to_wkb_polygons
 from s2 import s2
 from shapely import from_geojson, from_wkt
 from shapely.geometry import Polygon, box
 
 from quackosm import __app_name__, __version__
 from quackosm._osm_tags_filters import GroupedOsmTagsFilter, OsmTagsFilter
 from quackosm._typing import is_expected_type
@@ -141,18 +140,22 @@
 
     def convert(self, value, param=None, ctx=None):  # type: ignore
         """Convert parameter value."""
         if not value:
             return None
 
         try:
-            h3_int_indexes = [h3.str_to_int(h3_cell.strip()) for h3_cell in value.split(",")]
-            return gpd.GeoSeries.from_wkb(cells_to_wkb_polygons(h3_int_indexes)).unary_union
-        except Exception:
-            raise typer.BadParameter(f"Cannot parse provided H3 values: {value}") from None
+            geometries = []  # noqa: FURB138
+            for h3_cell in value.split(","):
+                geometries.append(
+                    Polygon([coords[::-1] for coords in h3.cell_to_boundary(h3_cell.strip())])
+                )
+            return gpd.GeoSeries(geometries).unary_union
+        except Exception as ex:
+            raise typer.BadParameter(f"Cannot parse provided H3 values: {value}") from ex
 
 
 class S2GeometryParser(click.ParamType):  # type: ignore
     """Parser for geometry in string Nominatim query form."""
 
     name = "TEXT (S2)"
```

### Comparing `quackosm-0.7.3/quackosm/conftest.py` & `quackosm-0.8.0/quackosm/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/functions.py` & `quackosm-0.8.0/quackosm/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     save_as_wkt: bool = False,
     verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
-    debug: bool = False,
+    debug_memory: bool = False,
+    debug_times: bool = False,
 ) -> Path:
     """
     Convert PBF file to GeoParquet file.
 
     Args:
         pbf_path (Union[str, Path]): Pbf file to be parsed to GeoParquet.
         tags_filter (Union[OsmTagsFilter, GroupedOsmTagsFilter], optional): A dictionary
@@ -74,28 +75,31 @@
         save_as_wkt (bool): Whether to save the file with geometry in the WKT form instead of WKB.
             If `True`, it will be saved as a `.parquet` file, because it won't be in the GeoParquet
             standard. Defaults to `False`.
         verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
             verbosity mode. Can be one of: silent, transient and verbose. Silent disables
             output completely. Transient tracks progress, but removes output after finished.
             Verbose leaves all progress outputs in the stdout. Defaults to "transient".
-        debug (bool, optional): If turned on, will keep all temporary files after operation
+        debug_memory (bool, optional): If turned on, will keep all temporary files after operation
             for debugging. Defaults to `False`.
+        debug_times (bool, optional): If turned on, will report timestamps at which second each
+            step has been executed. Defaults to `False`.
 
     Returns:
         Path: Path to the generated GeoParquet file.
 
     Examples:
         Get OSM data from a PBF file.
 
         Tags will be kept in a single column.
         >>> import quackosm as qosm
         >>> gpq_path = qosm.convert_pbf_to_gpq(monaco_pbf_path)
+        Finished operation in ...
         >>> gpq_path.as_posix()
-        'files/monaco_nofilter_noclip_compact.geoparquet'
+        'files/monaco_nofilter_noclip_compact.parquet'
 
         Inspect the file with duckdb
         >>> import duckdb
         >>> duckdb.load_extension('spatial')
         >>> duckdb.read_parquet(str(gpq_path)).project(
         ...     "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)"
         ... ).order("feature_id") # doctest: +SKIP
@@ -133,16 +137,17 @@
         Get only buildings, amenities and highways from a PBF file.
 
         Tags will be split into separate columns because of applying the filter.
         >>> gpq_path = qosm.convert_pbf_to_gpq(
         ...     monaco_pbf_path,
         ...     tags_filter={"building": True, "amenity": True, "highway": True}
         ... )
+        Finished operation in ...
         >>> gpq_path.as_posix()
-        'files/monaco_6593ca69098459d039054bc5fe0a87c56681e29a5f59d38ce3485c03cb0e9374_noclip_exploded.geoparquet'
+        'files/monaco_6593ca69098459d039054bc5fe0a87c56681e29a5f59d38ce3485c03cb0e9374_noclip_exploded.parquet'
 
         Inspect the file with duckdb
         >>> duckdb.read_parquet(str(gpq_path)).project(
         ...     "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)"
         ... ).order("feature_id") # doctest: +SKIP
         ┌──────────────────┬──────────┬────────────┬─────────────┬───────────────────────────────┐
         │    feature_id    │ building │  amenity   │   highway   │           geometry            │
@@ -184,16 +189,17 @@
         ...     geometry_filter=box(
         ...         minx=73.4975872,
         ...         miny=4.1663240,
         ...         maxx=73.5215528,
         ...         maxy=4.1818121
         ...     )
         ... )
+        Finished operation in ...
         >>> gpq_path.as_posix()
-        'files/maldives_nofilter_4eeabb20ccd8aefeaa80b9a46a202ab985fd454760823b7012cc7778498a085b_compact.geoparquet'
+        'files/maldives_nofilter_4eeabb20ccd8aefeaa80b9a46a202ab985fd454760823b7012cc7778498a085b_compact.parquet'
 
         Inspect the file with duckdb
         >>> duckdb.read_parquet(str(gpq_path)).project(
         ...     "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)"
         ... ).order("feature_id") # doctest: +SKIP
         ┌──────────────────┬──────────────────────┬──────────────────────────────────────────────┐
         │    feature_id    │         tags         │                   geometry                   │
@@ -228,15 +234,16 @@
     """
     return PbfFileReader(
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         verbosity_mode=verbosity_mode,
-        debug=debug,
+        debug_memory=debug_memory,
+        debug_times=debug_times,
     ).convert_pbf_to_gpq(
         pbf_path=pbf_path,
         result_file_path=result_file_path,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
@@ -254,15 +261,16 @@
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     save_as_wkt: bool = False,
     verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
     allow_uncovered_geometry: bool = False,
-    debug: bool = False,
+    debug_memory: bool = False,
+    debug_times: bool = False,
 ) -> Path:
     """
     Get a GeoParquet file with OpenStreetMap features within given geometry.
 
     Automatically downloads matching OSM extracts from different sources and returns a single file
     as a result.
 
@@ -309,32 +317,35 @@
         verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
             verbosity mode. Can be one of: silent, transient and verbose. Silent disables
             output completely. Transient tracks progress, but removes output after finished.
             Verbose leaves all progress outputs in the stdout. Defaults to "transient".
         allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
             by any OSM extract. Works only when PbfFileReader is asked to download OSM extracts
             automatically. Defaults to `False`.
-        debug (bool, optional): If turned on, will keep all temporary files after operation
+        debug_memory (bool, optional): If turned on, will keep all temporary files after operation
             for debugging. Defaults to `False`.
+        debug_times (bool, optional): If turned on, will report timestamps at which second each
+            step has been executed. Defaults to `False`.
 
     Returns:
         Path: Path to the generated GeoParquet file.
 
     Examples:
         Get OSM data from the center of Monaco.
 
         >>> import quackosm as qosm
         >>> from shapely import from_wkt
         >>> wkt = (
         ...     "POLYGON ((7.41644 43.73598, 7.41644 43.73142, 7.42378 43.73142,"
         ...     " 7.42378 43.73598, 7.41644 43.73598))"
         ... )
         >>> gpq_path = qosm.convert_geometry_to_gpq(from_wkt(wkt))
+        Finished operation in ...
         >>> gpq_path.as_posix()
-        'files/bf4b33debfd6d3e605555340606df6ce7eea934958c1f3477aca0ccf79e7929f_nofilter_compact.geoparquet'
+        'files/bf4b33debfd6d3e605555340606df6ce7eea934958c1f3477aca0ccf79e7929f_nofilter_compact.parquet'
 
         Inspect the file with duckdb
         >>> import duckdb
         >>> duckdb.load_extension('spatial')
         >>> duckdb.read_parquet(str(gpq_path)).project(
         ...     "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)"
         ... ).order("feature_id") # doctest: +SKIP
@@ -371,16 +382,17 @@
 
         Making sure that you are using specific OSM extract source - here Geofabrik.
 
         >>> gpq_path = qosm.convert_geometry_to_gpq(
         ...     from_wkt(wkt),
         ...     osm_extract_source='Geofabrik',
         ... )
+        Finished operation in ...
         >>> gpq_path.as_posix()
-        'files/bf4b33debfd6d3e605555340606df6ce7eea934958c1f3477aca0ccf79e7929f_nofilter_compact.geoparquet'
+        'files/bf4b33debfd6d3e605555340606df6ce7eea934958c1f3477aca0ccf79e7929f_nofilter_compact.parquet'
 
         Inspect the file with duckdb
         >>> duckdb.read_parquet(str(gpq_path)).project(
         ...     "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)"
         ... ).order("feature_id") # doctest: +SKIP
         ┌──────────────────┬──────────────────────┬──────────────────────────────────────────────┐
         │    feature_id    │         tags         │                   geometry                   │
@@ -417,15 +429,16 @@
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         osm_extract_source=osm_extract_source,
         verbosity_mode=verbosity_mode,
         allow_uncovered_geometry=allow_uncovered_geometry,
-        debug=debug,
+        debug_memory=debug_memory,
+        debug_times=debug_times,
     ).convert_geometry_filter_to_gpq(
         result_file_path=result_file_path,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
         save_as_wkt=save_as_wkt,
@@ -439,15 +452,16 @@
     keep_all_tags: bool = False,
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
-    debug: bool = False,
+    debug_memory: bool = False,
+    debug_times: bool = False,
 ) -> gpd.GeoDataFrame:
     """
     Get features GeoDataFrame from a PBF file or list of PBF files.
 
     Function can parse multiple PBF files and returns a single GeoDataFrame with loaded
     OSM objects.
 
@@ -485,26 +499,30 @@
             Config used to determine which closed way features are polygons.
             Modifications to this config left are left for experienced OSM users.
             Defaults to predefined "osm_way_polygon_features.json".
         verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
             verbosity mode. Can be one of: silent, transient and verbose. Silent disables
             output completely. Transient tracks progress, but removes output after finished.
             Verbose leaves all progress outputs in the stdout. Defaults to "transient".
-        debug (bool, optional): If turned on, will keep all temporary files after operation
+        debug_memory (bool, optional): If turned on, will keep all temporary files after operation
             for debugging. Defaults to `False`.
+        debug_times (bool, optional): If turned on, will report timestamps at which second each
+            step has been executed. Defaults to `False`.
 
     Returns:
         gpd.GeoDataFrame: GeoDataFrame with OSM features.
 
     Examples:
         Get OSM data from a PBF file.
 
         Tags will be kept in a single column.
         >>> import quackosm as qosm
-        >>> qosm.get_features_gdf(monaco_pbf_path).sort_index()
+        >>> gdf = qosm.get_features_gdf(monaco_pbf_path)
+        Finished operation in ...
+        >>> gdf.sort_index()
                                                       tags                      geometry
         feature_id
         node/10005045289                {'shop': 'bakery'}      POINT (7.42245 43.73105)
         node/10020887517  {'leisure': 'swimming_pool', ...      POINT (7.41316 43.73384)
         node/10021298117  {'leisure': 'swimming_pool', ...      POINT (7.42777 43.74277)
         node/10021298717  {'leisure': 'swimming_pool', ...      POINT (7.42630 43.74097)
         node/10025656383  {'ferry': 'yes', 'name': 'Qua...      POINT (7.42550 43.73690)
@@ -516,17 +534,19 @@
         way/993121275      {'building': 'yes', 'name': ...  POLYGON ((7.43214 43.7481...
         <BLANKLINE>
         [7906 rows x 2 columns]
 
         Get only buildings from a PBF file.
 
         Tags will be split into separate columns because of applying the filter.
-        >>> qosm.get_features_gdf(
+        >>> gdf = qosm.get_features_gdf(
         ...     monaco_pbf_path, tags_filter={"building": True}
-        ... ).sort_index()
+        ... )
+        Finished operation in ...
+        >>> gdf.sort_index()
                               building                                           geometry
         feature_id
         relation/11384697          yes  POLYGON ((7.42749 43.73125, 7.42672 43.73063, ...
         relation/11484092        hotel  POLYGON ((7.41790 43.72483, 7.41783 43.72486, ...
         relation/11484093   apartments  POLYGON ((7.41815 43.72561, 7.41836 43.72547, ...
         relation/11484094  residential  POLYGON ((7.41753 43.72583, 7.41753 43.72563, ...
         relation/11485520   apartments  POLYGON ((7.42071 43.73260, 7.42125 43.73260, ...
@@ -539,23 +559,25 @@
         <BLANKLINE>
         [1283 rows x 2 columns]
 
         Get features for Malé - the capital city of Maldives
 
         Tags will be kept in a single column.
         >>> from shapely.geometry import box
-        >>> qosm.get_features_gdf(
+        >>> gdf = qosm.get_features_gdf(
         ...     maldives_pbf_path,
         ...     geometry_filter=box(
         ...         minx=73.4975872,
         ...         miny=4.1663240,
         ...         maxx=73.5215528,
         ...         maxy=4.1818121
         ...     )
-        ... ).sort_index()
+        ... )
+        Finished operation in ...
+        >>> gdf.sort_index()
                                                    tags                                     geometry
         feature_id
         node/10010180778  {'brand': 'Ooredoo', 'bran...                     POINT (73.51790 4.17521)
         node/10062500171  {'contact:facebook': 'http...                     POINT (73.50958 4.17245)
         node/10078084764  {'addr:city': 'Male'', 'ad...                     POINT (73.50480 4.17267)
         node/10078086040  {'addr:city': 'Malé', 'add...                     POINT (73.50317 4.17596)
         node/10158825718  {'addr:postcode': '20175',...                     POINT (73.50832 4.17301)
@@ -569,29 +591,31 @@
         [2140 rows x 2 columns]
 
 
         Get features grouped into catgegories for Christmas Island
 
         Even though we apply the filter, the tags will be kept in a single column
         because of manual `explode_tags` value setting.
-        >>> qosm.get_features_gdf(
+        >>> gdf = qosm.get_features_gdf(
         ...     kiribati_pbf_path,
         ...     tags_filter={
         ...         "highway": {"highway": True},
         ...         "tree": {"natural": "tree"},
         ...         "building": {"building": True},
         ...     },
         ...     geometry_filter=box(
         ...         minx=-157.6046004,
         ...         miny=1.6724409,
         ...         maxx=-157.1379507,
         ...         maxy=2.075240
         ...     ),
         ...     explode_tags=False,
-        ... ).sort_index()
+        ... )
+        Finished operation in ...
+        >>> gdf.sort_index()
                                                   tags                                      geometry
         feature_id
         node/2377661784  {'building': 'building=ruin'}                    POINT (-157.18826 1.75186)
         node/4150479646       {'tree': 'natural=tree'}                    POINT (-157.36152 1.98363)
         node/4396875565       {'tree': 'natural=tree'}                    POINT (-157.36143 1.98364)
         node/4396875566       {'tree': 'natural=tree'}                    POINT (-157.36135 1.98364)
         node/4396875567       {'tree': 'natural=tree'}                    POINT (-157.36141 1.98371)
@@ -606,15 +630,16 @@
     """
     return PbfFileReader(
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         verbosity_mode=verbosity_mode,
-        debug=debug,
+        debug_memory=debug_memory,
+        debug_times=debug_times,
     ).get_features_gdf(
         file_paths=file_paths,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
     )
@@ -628,15 +653,16 @@
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
     allow_uncovered_geometry: bool = False,
-    debug: bool = False,
+    debug_memory: bool = False,
+    debug_times: bool = False,
 ) -> gpd.GeoDataFrame:
     """
     Get a GeoParquet file with OpenStreetMap features within given geometry.
 
     Automatically downloads matching OSM extracts from different sources and returns a single file
     as a result.
 
@@ -677,30 +703,34 @@
         verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
             verbosity mode. Can be one of: silent, transient and verbose. Silent disables
             output completely. Transient tracks progress, but removes output after finished.
             Verbose leaves all progress outputs in the stdout. Defaults to "transient".
         allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
             by any OSM extract. Works only when PbfFileReader is asked to download OSM extracts
             automatically. Defaults to `False`.
-        debug (bool, optional): If turned on, will keep all temporary files after operation
+        debug_memory (bool, optional): If turned on, will keep all temporary files after operation
             for debugging. Defaults to `False`.
+        debug_times (bool, optional): If turned on, will report timestamps at which second each
+            step has been executed. Defaults to `False`.
 
     Returns:
         gpd.GeoDataFrame: GeoDataFrame with OSM features.
 
     Examples:
         Get OSM data from the center of Monaco.
 
         >>> import quackosm as qosm
         >>> from shapely import from_wkt
         >>> wkt = (
         ...     "POLYGON ((7.41644 43.73598, 7.41644 43.73142, 7.42378 43.73142,"
         ...     " 7.42378 43.73598, 7.41644 43.73598))"
         ... )
-        >>> qosm.get_features_gdf_from_geometry(from_wkt(wkt)).sort_index()
+        >>> gdf = qosm.get_features_gdf_from_geometry(from_wkt(wkt))
+        Finished operation in ...
+        >>> gdf.sort_index()
                                                   tags                                      geometry
         feature_id
         node/10068880335     {'amenity': 'bench', '...                      POINT (7.41869 43.73215)
         node/10196648824  {'contact:city': 'Monaco'...                      POINT (7.41938 43.73375)
         node/10601158089  {'addr:city': 'Monaco', '...                      POINT (7.42131 43.73362)
         node/10672624925  {'addr:city': 'Monaco', '...                      POINT (7.42157 43.73517)
         node/10674256605         {'amenity': 'bar',...                      POINT (7.42136 43.73363)
@@ -711,18 +741,20 @@
         way/952419572     {'highway': 'primary', 'j...  LINESTRING (7.41731 43.73168, 7.41728 43....
         way/952419573     {'highway': 'primary', 'j...  LINESTRING (7.41739 43.73164, 7.41737 43....
         <BLANKLINE>
         [1384 rows x 2 columns]
 
         Making sure that you are using specific OSM extract source - here Geofabrik.
 
-        >>> qosm.get_features_gdf_from_geometry(
+        >>> gdf = qosm.get_features_gdf_from_geometry(
         ...     from_wkt(wkt),
         ...     osm_extract_source='Geofabrik',
-        ... ).sort_index()
+        ... )
+        Finished operation in ...
+        >>> gdf.sort_index()
                                                   tags                                      geometry
         feature_id
         node/10068880335       {'amenity': 'bench',...                      POINT (7.41869 43.73215)
         node/10196648824  {'contact:city': 'Monaco'...                      POINT (7.41938 43.73375)
         node/10601158089    {'addr:city': 'Monaco',...                      POINT (7.42131 43.73362)
         node/10672624925    {'addr:city': 'Monaco',...                      POINT (7.42157 43.73517)
         node/10674256605         {'amenity': 'bar',...                      POINT (7.42136 43.73363)
@@ -739,14 +771,15 @@
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         osm_extract_source=osm_extract_source,
         verbosity_mode=verbosity_mode,
         allow_uncovered_geometry=allow_uncovered_geometry,
-        debug=debug,
+        debug_memory=debug_memory,
+        debug_times=debug_times,
     ).get_features_gdf_from_geometry(
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
     )
```

### Comparing `quackosm-0.7.3/quackosm/osm_extracts/__init__.py` & `quackosm-0.8.0/quackosm/osm_extracts/__init__.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/osm_extracts/_poly_parser.py` & `quackosm-0.8.0/quackosm/osm_extracts/_poly_parser.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/osm_extracts/bbbike.py` & `quackosm-0.8.0/quackosm/osm_extracts/bbbike.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/osm_extracts/geofabrik.py` & `quackosm-0.8.0/quackosm/osm_extracts/geofabrik.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/osm_extracts/osm_fr.py` & `quackosm-0.8.0/quackosm/osm_extracts/osm_fr.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/osm_way_polygon_features.json` & `quackosm-0.8.0/quackosm/osm_way_polygon_features.json`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/quackosm/pbf_file_reader.py` & `quackosm-0.8.0/quackosm/pbf_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pathlib import Path
 from time import sleep
 from typing import Any, Literal, NamedTuple, Optional, Union, cast
 
 import duckdb
 import geoarrow.pyarrow as ga
 import geopandas as gpd
+import polars as pl
 import psutil
 import pyarrow as pa
 import pyarrow.parquet as pq
 import shapely.wkt as wktlib
 from geoarrow.pyarrow import io
 from pyarrow_ops import drop_duplicates
 from shapely.geometry import LinearRing, Polygon
@@ -106,15 +107,16 @@
         osm_way_polygon_features_config: Optional[
             Union[OsmWayPolygonConfig, dict[str, Any]]
         ] = None,
         parquet_compression: str = "snappy",
         osm_extract_source: Union[OsmExtractSource, str] = OsmExtractSource.geofabrik,
         verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
         allow_uncovered_geometry: bool = False,
-        debug: bool = False,
+        debug_memory: bool = False,
+        debug_times: bool = False,
     ) -> None:
         """
         Initialize PbfFileReader.
 
         Args:
             tags_filter (Union[OsmTagsFilter, GroupedOsmTagsFilter], optional): A dictionary
                 specifying which tags to download.
@@ -142,16 +144,18 @@
                 Defaults to `geofabrik`.
             verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
                 verbosity mode. Can be one of: silent, transient and verbose. Silent disables
                 output completely. Transient tracks progress, but removes output after finished.
                 Verbose leaves all progress outputs in the stdout. Defaults to "transient".
             allow_uncovered_geometry (bool, optional): Suppress an error if some geometry parts
                 aren't covered by any OSM extract. Defaults to `False`.
-            debug (bool, optional): If turned on, will keep all temporary files after operation
-                for debugging. Defaults to `False`.
+            debug_memory (bool, optional): If turned on, will keep all temporary files after
+                operation for debugging. Defaults to `False`.
+            debug_times (bool, optional): If turned on, will report timestamps at which second each
+                step has been executed. Defaults to `False`.
 
         Raises:
             InvalidGeometryFilter: When provided geometry filter has parts without area.
         """
         self.geometry_filter = geometry_filter
         self._check_if_valid_geometry_filter()
 
@@ -167,15 +171,16 @@
         self.allow_uncovered_geometry = allow_uncovered_geometry
         self.osm_extract_source = osm_extract_source
         self.working_directory = Path(working_directory)
         self.working_directory.mkdir(parents=True, exist_ok=True)
         self.connection: duckdb.DuckDBPyConnection = None
         self.encountered_query_exception = False
         self.verbosity_mode = verbosity_mode
-        self.debug = debug
+        self.debug_memory = debug_memory
+        self.debug_times = debug_times
         self.task_progress_tracker: TaskProgressTracker = None
 
         self.rows_per_group = PbfFileReader.ROWS_PER_GROUP_MEMORY_CONFIG[0]
         actual_memory = psutil.virtual_memory()
         # If more than 8 / 16 / 24 GB total memory, increase the number of rows per group
         for memory_gb, rows_per_group in PbfFileReader.ROWS_PER_GROUP_MEMORY_CONFIG.items():
             if actual_memory.total >= (memory_gb * MEMORY_1GB):
@@ -236,28 +241,30 @@
 
         Returns:
             Path: Path to the generated GeoParquet file.
         """
         created_task_progress_tracker = False
         if self.task_progress_tracker is None or not self.task_progress_tracker.is_new():
             created_task_progress_tracker = True
-            self.task_progress_tracker = TaskProgressTracker(verbosity_mode=self.verbosity_mode)
+            self.task_progress_tracker = TaskProgressTracker(
+                verbosity_mode=self.verbosity_mode, debug=self.debug_times
+            )
 
         if filter_osm_ids is None:
             filter_osm_ids = []
 
         if explode_tags is None:
             explode_tags = (
                 self.tags_filter is not None and self.is_tags_filter_positive and not keep_all_tags
             )
 
         with tempfile.TemporaryDirectory(dir=self.working_directory.resolve()) as self.tmp_dir_name:
             self.tmp_dir_path = Path(self.tmp_dir_name)
 
-            if self.debug:
+            if self.debug_memory:
                 self.tmp_dir_path = self._prepare_debug_directory()
 
             try:
                 self.encountered_query_exception = False
                 self.connection = _set_up_duckdb_connection(tmp_dir_path=self.tmp_dir_path)
                 result_file_path = result_file_path or self._generate_result_file_path(
                     pbf_path,
@@ -361,22 +368,36 @@
                 keep_all_tags=keep_all_tags,
                 explode_tags=explode_tags,
                 ignore_cache=ignore_cache,
                 filter_osm_ids=filter_osm_ids,
                 save_as_wkt=save_as_wkt,
             )
         else:
+            if result_file_path.with_suffix(".geoparquet").exists() and not ignore_cache:
+                warnings.warn(
+                    (
+                        "Found existing result file with `.geoparquet` extension."
+                        " Users are enouraged to change the extension manually"
+                        " to `.parquet` for old files. Files with `.geoparquet`"
+                        " extension will be backwards supported, but reusing them"
+                        " will result in this warning."
+                    ),
+                    DeprecationWarning,
+                    stacklevel=0,
+                )
+                return result_file_path.with_suffix(".geoparquet")
             if not result_file_path.exists() or ignore_cache:
                 pbf_files = download_extracts_pbf_files(matching_extracts, self.working_directory)
 
                 parsed_geoparquet_files = []
                 total_files = len(pbf_files)
                 self.task_progress_tracker = TaskProgressTracker(
                     verbosity_mode=self.verbosity_mode,
                     total_major_steps=total_files,
+                    debug=self.debug_times,
                 )
                 for file_idx, file_path in enumerate(pbf_files):
                     self.task_progress_tracker.reset_steps(file_idx + 1)
                     parsed_geoparquet_file = self.convert_pbf_to_gpq(
                         file_path,
                         keep_all_tags=keep_all_tags,
                         explode_tags=explode_tags,
@@ -386,15 +407,15 @@
                     )
                     parsed_geoparquet_files.append(parsed_geoparquet_file)
 
                 if parsed_geoparquet_files:
                     with tempfile.TemporaryDirectory(
                         dir=self.working_directory.resolve()
                     ) as tmp_dir_name:
-                        if self.debug:
+                        if self.debug_memory:
                             tmp_dir_name = self._prepare_debug_directory()  # type: ignore[assignment] # noqa: PLW2901
 
                         try:
                             joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
                                 parsed_geoparquet_files
                             )
                         except pa.ArrowInvalid:
@@ -485,29 +506,30 @@
             )
 
         parsed_geoparquet_files = []
         total_files = len(list(file_paths))
         self.task_progress_tracker = TaskProgressTracker(
             verbosity_mode=self.verbosity_mode,
             total_major_steps=total_files,
+            debug=self.debug_memory,
         )
         for file_idx, file_path in enumerate(file_paths):
             self.task_progress_tracker.reset_steps(file_idx + 1)
             parsed_geoparquet_file = self.convert_pbf_to_gpq(
                 file_path,
                 keep_all_tags=keep_all_tags,
                 explode_tags=explode_tags,
                 ignore_cache=ignore_cache,
                 filter_osm_ids=filter_osm_ids,
             )
             parsed_geoparquet_files.append(parsed_geoparquet_file)
 
         if parsed_geoparquet_files:
             with tempfile.TemporaryDirectory(dir=self.working_directory.resolve()) as tmp_dir_name:
-                if self.debug:
+                if self.debug_memory:
                     tmp_dir_name = self._prepare_debug_directory()  # type: ignore[assignment] # noqa: PLW2901
 
                 try:
                     joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
                         parsed_geoparquet_files
                     )
                 except pa.ArrowInvalid:
@@ -630,15 +652,15 @@
                 ) TO '{output_file_name}' (
                     FORMAT 'parquet',
                     PER_THREAD_OUTPUT true,
                     ROW_GROUP_SIZE 25000,
                     COMPRESSION '{self.parquet_compression}'
                 )
             """
-            if self.debug:
+            if self.debug_memory:
                 log_message(f"Saved to directory: {output_file_name}")
             self._run_query(query, run_in_separate_process=True, tmp_dir_path=tmp_dir_path)
             return pq.read_table(output_file_name)
 
     def _drop_duplicated_features_in_joined_table_one_by_one(
         self, parsed_geoparquet_files: list[Path], tmp_dir_path: Path
     ) -> pa.Table:
@@ -667,15 +689,15 @@
                     ) TO '{filtered_result_parquet_file}' (
                         FORMAT 'parquet',
                         PER_THREAD_OUTPUT true,
                         ROW_GROUP_SIZE 25000,
                         COMPRESSION '{self.parquet_compression}'
                     )
                 """
-                if self.debug:
+                if self.debug_memory:
                     log_message(f"Saved to directory: {filtered_result_parquet_file}")
                 connection.sql(query)
                 result_parquet_files.extend(filtered_result_parquet_file.glob("*.parquet"))
         return pq.read_table(result_parquet_files)
 
     def _parse_pbf_file(
         self,
@@ -683,14 +705,28 @@
         result_file_path: Path,
         filter_osm_ids: list[str],
         keep_all_tags: bool = False,
         explode_tags: bool = True,
         ignore_cache: bool = False,
         save_as_wkt: bool = False,
     ) -> Path:
+        if result_file_path.with_suffix(".geoparquet").exists() and not ignore_cache:
+            warnings.warn(
+                (
+                    "Found existing result file with `.geoparquet` extension."
+                    " Users are enouraged to change the extension manually"
+                    " to `.parquet` for old files. Files with `.geoparquet`"
+                    " extension will be backwards supported, but reusing them"
+                    " will result in this warning."
+                ),
+                DeprecationWarning,
+                stacklevel=0,
+            )
+            return result_file_path.with_suffix(".geoparquet")
+
         if not result_file_path.exists() or ignore_cache:
 
             elements = self.connection.sql(f"SELECT * FROM ST_READOSM('{Path(pbf_path)}');")
 
             if self.tags_filter is None:
                 self.expanded_tags_filter = None
                 self.merged_tags_filter = None
@@ -819,15 +855,15 @@
             result_file_name = (
                 f"{pbf_file_name}_{osm_filter_tags_hash_part}"
                 f"_{clipping_geometry_hash_part}_{exploded_tags_part}{filter_osm_ids_hash_part}_wkt.parquet"
             )
         else:
             result_file_name = (
                 f"{pbf_file_name}_{osm_filter_tags_hash_part}"
-                f"_{clipping_geometry_hash_part}_{exploded_tags_part}{filter_osm_ids_hash_part}.geoparquet"
+                f"_{clipping_geometry_hash_part}_{exploded_tags_part}{filter_osm_ids_hash_part}.parquet"
             )
         return Path(self.working_directory) / result_file_name
 
     def _generate_result_file_path_from_geometry(
         self, keep_all_tags: bool, explode_tags: bool, filter_osm_ids: list[str], save_as_wkt: bool
     ) -> Path:
         osm_filter_tags_hash_part = "nofilter"
@@ -851,15 +887,15 @@
             result_file_name = (
                 f"{clipping_geometry_hash_part}_{osm_filter_tags_hash_part}"
                 f"_{exploded_tags_part}{filter_osm_ids_hash_part}_wkt.parquet"
             )
         else:
             result_file_name = (
                 f"{clipping_geometry_hash_part}_{osm_filter_tags_hash_part}"
-                f"_{exploded_tags_part}{filter_osm_ids_hash_part}.geoparquet"
+                f"_{exploded_tags_part}{filter_osm_ids_hash_part}.parquet"
             )
         return Path(self.working_directory) / result_file_name
 
     def _check_if_valid_geometry_filter(self) -> None:
         if self.geometry_filter is None:
             return
 
@@ -1299,15 +1335,15 @@
             relations_with_unnested_way_refs=relations_with_unnested_way_refs,
             relations_filtered_ids=relations_filtered_ids,
         )
 
     def _delete_directories(
         self, directories: Union[str, Path, list[Union[str, Path]]], override_debug: bool = False
     ) -> None:
-        if self.debug and not override_debug:
+        if self.debug_memory and not override_debug:
             return
 
         _directories = []
         if isinstance(directories, (str, Path)):
             _directories = [directories]
         else:
             _directories = directories
@@ -1324,15 +1360,15 @@
                     if tries == 0:
                         raise ex
                     sleep(0.5)
                 finally:
                     tries -= 1
 
     def _prepare_debug_directory(self) -> Path:
-        if self.debug:
+        if self.debug_memory:
             dir_path = Path(self.working_directory) / "debug" / secrets.token_hex(16)
             self._delete_directories(dir_path, override_debug=True)
             dir_path.mkdir(exist_ok=True, parents=True)
             return dir_path
         raise RuntimeError("Cannot prepare debug directory when debug mode is not activated.")
 
     def _generate_osm_tags_sql_filter(self) -> str:
@@ -1449,15 +1485,15 @@
                 FORMAT 'parquet',
                 PER_THREAD_OUTPUT true,
                 ROW_GROUP_SIZE 25000,
                 COMPRESSION '{self.parquet_compression}'
             )
         """
         self._run_query(query, run_in_separate_process)
-        if self.debug:
+        if self.debug_memory:
             log_message(f"Saved to directory: {file_path}")
         return self.connection.sql(f"SELECT * FROM read_parquet('{file_path}/**')")
 
     def _run_query(
         self,
         sql_queries: Union[str, list[str]],
         run_in_separate_process: bool = False,
@@ -1512,15 +1548,15 @@
                 FORMAT 'parquet',
                 PER_THREAD_OUTPUT true,
                 ROW_GROUP_SIZE 25000,
                 COMPRESSION '{self.parquet_compression}'
             )
             """
         )
-        if self.debug:
+        if self.debug_memory:
             log_message(f"Saved to directory: {result_path}")
 
         return self.connection.sql(f"SELECT * FROM read_parquet('{result_path}/**')")
 
     def _get_filtered_nodes_with_geometry(
         self,
         osm_parquet_files: ConvertedOSMParquetFiles,
@@ -1607,14 +1643,15 @@
         destination_dir_path: Path,
         grouped_ways_tmp_path: Path,
         grouped_ways_path: Path,
     ) -> "duckdb.DuckDBPyRelation":
         finished_operation = False
 
         while not finished_operation:
+            reset_steps = 1
             try:
                 if not self.encountered_query_exception:
                     groups = self._group_ways(
                         ways_ids=ways_ids,
                         mode=mode,
                         osm_parquet_files=osm_parquet_files,
                         destination_dir_path=destination_dir_path,
@@ -1628,14 +1665,15 @@
                         mode=mode,
                         osm_parquet_files=osm_parquet_files,
                         destination_dir_path=destination_dir_path,
                         grouped_ways_tmp_path=grouped_ways_tmp_path,
                         grouped_ways_path=grouped_ways_path,
                         group_all_at_once=False,
                     )
+                reset_steps += 1
 
                 self._delete_directories(grouped_ways_tmp_path)
 
                 with self.task_progress_tracker.get_bar(
                     f"Saving {mode} ways with linestrings"
                 ) as bar:
                     self._construct_ways_linestrings(
@@ -1644,15 +1682,15 @@
                         destination_dir_path=destination_dir_path,
                         grouped_ways_path=grouped_ways_path,
                     )
 
                 finished_operation = True
             except (duckdb.OutOfMemoryException, MemoryError, TimeoutError) as ex:
                 self.encountered_query_exception = True
-                self.task_progress_tracker.major_step_number -= 1
+                self.task_progress_tracker.major_step_number -= reset_steps
                 if self.rows_per_group > PbfFileReader.ROWS_PER_GROUP_MEMORY_CONFIG[0]:
                     self._delete_directories(
                         [destination_dir_path, grouped_ways_tmp_path, grouped_ways_path]
                     )
                     smaller_rows_per_group = 0
                     for rows_per_group in PbfFileReader.ROWS_PER_GROUP_MEMORY_CONFIG.values():
                         if rows_per_group < self.rows_per_group:
@@ -1806,58 +1844,52 @@
                     FORMAT 'parquet',
                     PARTITION_BY ("group"),
                     ROW_GROUP_SIZE 25000,
                     COMPRESSION '{self.parquet_compression}'
                 )
                 """
             )
-            if self.debug:
+            if self.debug_memory:
                 log_message(f"Saved to directory: {grouped_ways_path}")
 
         return groups
 
     def _construct_ways_linestrings(
         self,
         bar: TaskProgressBar,
         groups: int,
         destination_dir_path: Path,
         grouped_ways_path: Path,
     ) -> None:
         for group in bar.track(range(groups + 1)):
             current_ways_group_path = grouped_ways_path / f"group={group}"
-            current_destination_path = destination_dir_path / f"group={group}"
+            current_destination_path = destination_dir_path / f"group={group}" / "data.parquet"
+            current_destination_path.parent.mkdir(parents=True, exist_ok=True)
 
-            temp_table_name = f"tbl{secrets.token_hex(16)}"
-            create_temp_table_query = f"""
-                CREATE OR REPLACE TEMP TABLE {temp_table_name} AS
-                FROM read_parquet('{current_ways_group_path}/**')
-            """
-            group_ways_query = f"""
-                COPY (
-                    SELECT id, list(point ORDER BY ref_idx ASC)::LINESTRING_2D linestring
-                    FROM {temp_table_name}
-                    GROUP BY id
-                ) TO '{current_destination_path}' (
-                    FORMAT 'parquet',
-                    PER_THREAD_OUTPUT true,
-                    ROW_GROUP_SIZE 25000,
-                    COMPRESSION '{self.parquet_compression}'
+            with Pool() as pool:
+                r = pool.apply_async(
+                    _group_ways_with_polars,
+                    args=(current_ways_group_path, current_destination_path),
                 )
-            """
-            drop_table_query = f"DROP TABLE {temp_table_name}"
-            queries = [create_temp_table_query, group_ways_query, drop_table_query]
+                actual_memory = psutil.virtual_memory()
+                percentage_threshold = 95
+                if (actual_memory.total * 0.05) > MEMORY_1GB:
+                    percentage_threshold = (
+                        100 * (actual_memory.total - MEMORY_1GB) / actual_memory.total
+                    )
+                while not r.ready():
+                    actual_memory = psutil.virtual_memory()
+                    if actual_memory.percent > percentage_threshold:
+                        raise MemoryError()
 
-            self._run_query(
-                queries,
-                run_in_separate_process=(
-                    self.rows_per_group > PbfFileReader.ROWS_PER_GROUP_MEMORY_CONFIG[0]
-                ),
-            )
-            if self.debug:
-                log_message(f"Saved to directory: {current_destination_path}")
+                    sleep(0.5)
+                r.get()
+
+            if self.debug_memory:
+                log_message(f"Saved to file: {current_destination_path}")
 
             self._delete_directories(current_ways_group_path)
 
     def _get_filtered_ways_with_proper_geometry(
         self,
         osm_parquet_files: ConvertedOSMParquetFiles,
         required_ways_with_linestrings: "duckdb.DuckDBPyRelation",
@@ -2111,15 +2143,15 @@
                     FORMAT 'parquet',
                     PER_THREAD_OUTPUT true,
                     ROW_GROUP_SIZE 25000,
                     COMPRESSION '{self.parquet_compression}'
                 )
                 """
             )
-            if self.debug:
+            if self.debug_memory:
                 log_message(f"Saved to directory: {file_path}")
 
         return self.connection.sql(
             f"""
             SELECT * EXCLUDE (geometry_wkb), ST_GeomFromWKB(geometry_wkb) geometry
             FROM read_parquet('{file_path}/**')
             """
@@ -2475,26 +2507,43 @@
     )
     connection.sql("SET enable_progress_bar = false;")
     connection.sql("SET enable_progress_bar_print = false;")
     for extension_name in ("parquet", "spatial"):
         connection.install_extension(extension_name)
         connection.load_extension(extension_name)
 
-    connection.sql("""
+    connection.sql(
+        """
         CREATE OR REPLACE MACRO linestring_to_linestring_geometry(ls) AS
         ls::struct(x DECIMAL(10, 7), y DECIMAL(10, 7))[]::LINESTRING_2D::GEOMETRY;
-    """)
-    connection.sql("""
+    """
+    )
+    connection.sql(
+        """
         CREATE OR REPLACE MACRO linestring_to_polygon_geometry(ls) AS
         [ls::struct(x DECIMAL(10, 7), y DECIMAL(10, 7))[]]::POLYGON_2D::GEOMETRY;
-    """)
+    """
+    )
 
     return connection
 
 
 def _run_query(sql_queries: Union[str, list[str]], tmp_dir_path: Path) -> None:
     if isinstance(sql_queries, str):
         sql_queries = [sql_queries]
     conn = _set_up_duckdb_connection(tmp_dir_path=tmp_dir_path, is_main_connection=False)
     for sql_query in sql_queries:
         conn.sql(sql_query)
     conn.close()
+
+
+def _group_ways_with_polars(current_ways_group_path: Path, current_destination_path: Path) -> None:
+    pl.scan_parquet(
+        source=f"{current_ways_group_path}/*.parquet",
+        hive_partitioning=False,
+    ).group_by("id").agg(pl.col("point").sort_by(pl.col("ref_idx"))).rename(
+        {"point": "linestring"}
+    ).collect(
+        streaming=True
+    ).write_parquet(
+        current_destination_path
+    )
```

### Comparing `quackosm-0.7.3/tests/base/conftest.py` & `quackosm-0.8.0/tests/base/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/tests/base/test_cli.py` & `quackosm-0.8.0/tests/base/test_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,206 +53,206 @@
 
 
 def test_basic_run(monaco_pbf_file_path: str) -> None:
     """Test if runs properly without options."""
     result = runner.invoke(cli.app, [monaco_pbf_file_path])
 
     assert result.exit_code == 0
-    assert str(Path("files/monaco_nofilter_noclip_compact.geoparquet")) in result.stdout
+    assert str(Path("files/monaco_nofilter_noclip_compact.parquet")) in result.stdout
 
 
 def test_silent_mode(monaco_pbf_file_path: str) -> None:
     """Test if runs properly without reporting status."""
     result = runner.invoke(cli.app, [monaco_pbf_file_path, "--ignore-cache", "--silent"])
 
     assert result.exit_code == 0
-    assert str(Path("files/monaco_nofilter_noclip_compact.geoparquet")) == result.stdout.strip()
+    assert str(Path("files/monaco_nofilter_noclip_compact.parquet")) == result.stdout.strip()
 
 
 def test_transient_mode(monaco_pbf_file_path: str) -> None:
     """Test if runs properly without reporting status."""
     result = runner.invoke(cli.app, [monaco_pbf_file_path, "--ignore-cache", "--transient"])
     output_lines = result.stdout.strip().split("\n")
     assert result.exit_code == 0
     assert len(result.stdout.strip().split("\n")) == 2
     assert "Finished operation in" in output_lines[0]
-    assert str(Path("files/monaco_nofilter_noclip_compact.geoparquet")) == output_lines[1]
+    assert str(Path("files/monaco_nofilter_noclip_compact.parquet")) == output_lines[1]
 
 
 @P.parameters("args", "expected_result")  # type: ignore
 @P.case(
     "Explode",
     ["--explode-tags"],
-    "files/monaco_nofilter_noclip_exploded.geoparquet",
+    "files/monaco_nofilter_noclip_exploded.parquet",
 )  # type: ignore
-@P.case("Explode short", ["--explode"], "files/monaco_nofilter_noclip_exploded.geoparquet")  # type: ignore
-@P.case("Compact", ["--compact-tags"], "files/monaco_nofilter_noclip_compact.geoparquet")  # type: ignore
-@P.case("Compact short", ["--compact"], "files/monaco_nofilter_noclip_compact.geoparquet")  # type: ignore
+@P.case("Explode short", ["--explode"], "files/monaco_nofilter_noclip_exploded.parquet")  # type: ignore
+@P.case("Compact", ["--compact-tags"], "files/monaco_nofilter_noclip_compact.parquet")  # type: ignore
+@P.case("Compact short", ["--compact"], "files/monaco_nofilter_noclip_compact.parquet")  # type: ignore
 @P.case(
     "Working directory",
     ["--working-directory", "files/workdir"],
-    "files/workdir/monaco_nofilter_noclip_compact.geoparquet",
+    "files/workdir/monaco_nofilter_noclip_compact.parquet",
 )  # type: ignore
-@P.case("Ignore cache", ["--ignore-cache"], "files/monaco_nofilter_noclip_compact.geoparquet")  # type: ignore
-@P.case("Ignore cache short", ["--no-cache"], "files/monaco_nofilter_noclip_compact.geoparquet")  # type: ignore
-@P.case("Output", ["--output", "files/monaco_output.geoparquet"], "files/monaco_output.geoparquet")  # type: ignore
-@P.case("Output short", ["-o", "files/monaco_output.geoparquet"], "files/monaco_output.geoparquet")  # type: ignore
-@P.case("Silent", ["--silent"], "files/monaco_nofilter_noclip_compact.geoparquet")  # type: ignore
-@P.case("Transient", ["--transient"], "files/monaco_nofilter_noclip_compact.geoparquet")  # type: ignore
+@P.case("Ignore cache", ["--ignore-cache"], "files/monaco_nofilter_noclip_compact.parquet")  # type: ignore
+@P.case("Ignore cache short", ["--no-cache"], "files/monaco_nofilter_noclip_compact.parquet")  # type: ignore
+@P.case("Output", ["--output", "files/monaco_output.parquet"], "files/monaco_output.parquet")  # type: ignore
+@P.case("Output short", ["-o", "files/monaco_output.parquet"], "files/monaco_output.parquet")  # type: ignore
+@P.case("Silent", ["--silent"], "files/monaco_nofilter_noclip_compact.parquet")  # type: ignore
+@P.case("Transient", ["--transient"], "files/monaco_nofilter_noclip_compact.parquet")  # type: ignore
 @P.case(
     "Output with working directory",
-    ["--working-directory", "files/workdir", "-o", "files/monaco_output.geoparquet"],
-    "files/monaco_output.geoparquet",
+    ["--working-directory", "files/workdir", "-o", "files/monaco_output.parquet"],
+    "files/monaco_output.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter",
     [
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
     ],
-    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.geoparquet",
+    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter compact",
     [
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
         "--compact",
     ],
-    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_compact.geoparquet",
+    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter file",
     [
         "--osm-tags-filter-file",
         osm_tags_filter_file_path(),
     ],
-    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.geoparquet",
+    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter file compact",
     [
         "--osm-tags-filter-file",
         osm_tags_filter_file_path(),
         "--compact",
     ],
-    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_compact.geoparquet",
+    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter grouped",
     [
         "--osm-tags-filter",
         '{"group": {"building": true, "highway": ["primary", "secondary"], "amenity": "bench"} }',
     ],
-    "files/monaco_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_noclip_exploded.geoparquet",
+    "files/monaco_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_noclip_exploded.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter grouped compact",
     [
         "--osm-tags-filter",
         '{"group": {"building": true, "highway": ["primary", "secondary"], "amenity": "bench"} }',
         "--compact",
     ],
-    "files/monaco_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_noclip_compact.geoparquet",
+    "files/monaco_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_noclip_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry WKT filter",
     ["--geom-filter-wkt", geometry_wkt()],
-    "files/monaco_nofilter_09c3fc0471538594b784be7c52782837c7a26753c2b26097b780581fa0a6bfc6_compact.geoparquet",
+    "files/monaco_nofilter_09c3fc0471538594b784be7c52782837c7a26753c2b26097b780581fa0a6bfc6_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry GeoJSON filter",
     ["--geom-filter-geojson", geometry_geojson()],
-    "files/monaco_nofilter_82c0fdfa2d5654818a03540644834d70c353e3f82f9d8f201c37420aeb35118e_compact.geoparquet",
+    "files/monaco_nofilter_82c0fdfa2d5654818a03540644834d70c353e3f82f9d8f201c37420aeb35118e_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry file filter",
     ["--geom-filter-file", geometry_boundary_file_path()],
-    "files/monaco_nofilter_6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_compact.geoparquet",
+    "files/monaco_nofilter_6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry geocode filter",
     ["--geom-filter-geocode", "Monaco-Ville, Monaco"],
-    "files/monaco_nofilter_e7f0b78a0fdc16c4db31c9767fa4e639eadaa8e83a9b90e07b521f4925cdf4b3_compact.geoparquet",
+    "files/monaco_nofilter_e7f0b78a0fdc16c4db31c9767fa4e639eadaa8e83a9b90e07b521f4925cdf4b3_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry Geohash filter",
     ["--geom-filter-index-geohash", "spv2bc"],
-    "files/monaco_nofilter_c08889e81575260e7ea2bc9764ddaa7c5e1141270a890b022799689d39dfe4d5_compact.geoparquet",
+    "files/monaco_nofilter_c08889e81575260e7ea2bc9764ddaa7c5e1141270a890b022799689d39dfe4d5_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry Geohash filter multiple",
     ["--geom-filter-index-geohash", "spv2bc,spv2bfr"],
-    "files/monaco_nofilter_1bd33e0afc3cd0efcb4740185b8a05ecaf1bac916d571403768939b82844b43e_compact.geoparquet",
+    "files/monaco_nofilter_1bd33e0afc3cd0efcb4740185b8a05ecaf1bac916d571403768939b82844b43e_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry H3 filter",
     ["--geom-filter-index-h3", "8a3969a40ac7fff"],
-    "files/monaco_nofilter_a2f8d5114760394646aa999a1204adaa48ad686b3fcadb0b25fd02322c16dff4_compact.geoparquet",
+    "files/monaco_nofilter_a2f8d5114760394646aa999a1204adaa48ad686b3fcadb0b25fd02322c16dff4_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry H3 filter multiple",
     ["--geom-filter-index-h3", "8a3969a40ac7fff,893969a4037ffff"],
-    "files/monaco_nofilter_e50e6489d4faba664a3c7f9729b7a3bedafb7a396ae826521f32b556d0b554f1_compact.geoparquet",
+    "files/monaco_nofilter_e50e6489d4faba664a3c7f9729b7a3bedafb7a396ae826521f32b556d0b554f1_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry S2 filter",
     ["--geom-filter-index-s2", "12cdc28bc"],
-    "files/monaco_nofilter_5c3d61eb108819e543a1a59fe6c67658f817c0453d728b5aa007f227453d5bf6_compact.geoparquet",
+    "files/monaco_nofilter_5c3d61eb108819e543a1a59fe6c67658f817c0453d728b5aa007f227453d5bf6_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry S2 filter multiple",
     ["--geom-filter-index-s2", "12cdc28bc,12cdc28f"],
-    "files/monaco_nofilter_cda5d65e169e3ff04970e66e80b021937a5ae141ed72428cc0d9a3764bf076db_compact.geoparquet",
+    "files/monaco_nofilter_cda5d65e169e3ff04970e66e80b021937a5ae141ed72428cc0d9a3764bf076db_compact.parquet",
 )  # type: ignore
 @P.case(
     "Filter OSM features IDs",
     ["--filter-osm-ids", "way/94399646,node/3617982224,relation/36990"],
-    "files/monaco_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.geoparquet",
+    "files/monaco_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.parquet",
 )  # type: ignore
 @P.case(
     "Keep all tags",
     [
         "--keep-all-tags",
     ],
-    "files/monaco_nofilter_noclip_compact.geoparquet",
+    "files/monaco_nofilter_noclip_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter with keep all tags",
     [
         "--keep-all-tags",
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
     ],
-    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.geoparquet",
+    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter with keep all tags compact",
     [
         "--keep-all-tags",
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
         "--compact",
     ],
-    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.geoparquet",
+    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter with keep all tags exploded",
     [
         "--keep-all-tags",
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
         "--explode",
     ],
-    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_exploded.geoparquet",
+    "files/monaco_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_exploded.parquet",
 )  # type: ignore
 @P.case(
     "OSM way polygon config",
     ["--osm-way-polygon-config", osm_way_config_file_path()],
-    "files/monaco_nofilter_noclip_compact.geoparquet",
+    "files/monaco_nofilter_noclip_compact.parquet",
 )  # type: ignore
 @P.case("WKT", ["--wkt-result"], "files/monaco_nofilter_noclip_compact_wkt.parquet")  # type: ignore
 @P.case("WKT short", ["--wkt"], "files/monaco_nofilter_noclip_compact_wkt.parquet")  # type: ignore
 def test_proper_args_with_pbf(
     monaco_pbf_file_path: str, args: list[str], expected_result: str
 ) -> None:
     """Test if runs properly with options."""
@@ -263,262 +263,262 @@
     assert str(Path(expected_result)) in result.stdout
 
 
 @P.parameters("args", "expected_result")  # type: ignore
 @P.case(
     "Geometry WKT filter",
     ["--geom-filter-wkt", geometry_wkt()],
-    "files/09c3fc0471538594b784be7c52782837c7a26753c2b26097b780581fa0a6bfc6_nofilter_compact.geoparquet",
+    "files/09c3fc0471538594b784be7c52782837c7a26753c2b26097b780581fa0a6bfc6_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry GeoJSON filter",
     ["--geom-filter-geojson", geometry_geojson()],
-    "files/82c0fdfa2d5654818a03540644834d70c353e3f82f9d8f201c37420aeb35118e_nofilter_compact.geoparquet",
+    "files/82c0fdfa2d5654818a03540644834d70c353e3f82f9d8f201c37420aeb35118e_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry geocode filter",
     ["--geom-filter-geocode", "Monaco-Ville, Monaco"],
-    "files/e7f0b78a0fdc16c4db31c9767fa4e639eadaa8e83a9b90e07b521f4925cdf4b3_nofilter_compact.geoparquet",
+    "files/e7f0b78a0fdc16c4db31c9767fa4e639eadaa8e83a9b90e07b521f4925cdf4b3_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry Geohash filter",
     ["--geom-filter-index-geohash", "spv2bc"],
-    "files/c08889e81575260e7ea2bc9764ddaa7c5e1141270a890b022799689d39dfe4d5_nofilter_compact.geoparquet",
+    "files/c08889e81575260e7ea2bc9764ddaa7c5e1141270a890b022799689d39dfe4d5_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry Geohash filter multiple",
     ["--geom-filter-index-geohash", "spv2bc,spv2bfr"],
-    "files/1bd33e0afc3cd0efcb4740185b8a05ecaf1bac916d571403768939b82844b43e_nofilter_compact.geoparquet",
+    "files/1bd33e0afc3cd0efcb4740185b8a05ecaf1bac916d571403768939b82844b43e_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry H3 filter",
     ["--geom-filter-index-h3", "8a3969a40ac7fff"],
-    "files/a2f8d5114760394646aa999a1204adaa48ad686b3fcadb0b25fd02322c16dff4_nofilter_compact.geoparquet",
+    "files/a2f8d5114760394646aa999a1204adaa48ad686b3fcadb0b25fd02322c16dff4_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry H3 filter multiple",
     ["--geom-filter-index-h3", "8a3969a40ac7fff,893969a4037ffff"],
-    "files/e50e6489d4faba664a3c7f9729b7a3bedafb7a396ae826521f32b556d0b554f1_nofilter_compact.geoparquet",
+    "files/e50e6489d4faba664a3c7f9729b7a3bedafb7a396ae826521f32b556d0b554f1_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry S2 filter",
     ["--geom-filter-index-s2", "12cdc28bc"],
-    "files/5c3d61eb108819e543a1a59fe6c67658f817c0453d728b5aa007f227453d5bf6_nofilter_compact.geoparquet",
+    "files/5c3d61eb108819e543a1a59fe6c67658f817c0453d728b5aa007f227453d5bf6_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry S2 filter multiple",
     ["--geom-filter-index-s2", "12cdc28bc,12cdc28f"],
-    "files/cda5d65e169e3ff04970e66e80b021937a5ae141ed72428cc0d9a3764bf076db_nofilter_compact.geoparquet",
+    "files/cda5d65e169e3ff04970e66e80b021937a5ae141ed72428cc0d9a3764bf076db_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Geometry file filter with different OSM source",
     ["--geom-filter-file", geometry_boundary_file_path(), "--osm-extract-source", "OSMfr"],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Explode",
     ["--geom-filter-file", geometry_boundary_file_path(), "--explode-tags"],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_exploded.parquet",
 )  # type: ignore
 @P.case(
     "Explode short",
     ["--geom-filter-file", geometry_boundary_file_path(), "--explode"],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_exploded.parquet",
 )  # type: ignore
 @P.case(
     "Compact",
     ["--geom-filter-file", geometry_boundary_file_path(), "--compact-tags"],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Compact short",
     ["--geom-filter-file", geometry_boundary_file_path(), "--compact"],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Working directory",
     ["--geom-filter-file", geometry_boundary_file_path(), "--working-directory", "files/workdir"],
-    "files/workdir/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
+    "files/workdir/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Ignore cache",
     ["--geom-filter-file", geometry_boundary_file_path(), "--ignore-cache"],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Ignore cache short",
     ["--geom-filter-file", geometry_boundary_file_path(), "--no-cache"],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Output",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--output",
-        "files/monaco_output.geoparquet",
+        "files/monaco_output.parquet",
     ],
-    "files/monaco_output.geoparquet",
+    "files/monaco_output.parquet",
 )  # type: ignore
 @P.case(
     "Output short",
-    ["--geom-filter-file", geometry_boundary_file_path(), "-o", "files/monaco_output.geoparquet"],
-    "files/monaco_output.geoparquet",
+    ["--geom-filter-file", geometry_boundary_file_path(), "-o", "files/monaco_output.parquet"],
+    "files/monaco_output.parquet",
 )  # type: ignore
 @P.case(
     "Output with working directory",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--working-directory",
         "files/workdir",
         "-o",
-        "files/monaco_output.geoparquet",
+        "files/monaco_output.parquet",
     ],
-    "files/monaco_output.geoparquet",
+    "files/monaco_output.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_exploded.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter compact",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
         "--compact",
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter file",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter-file",
         osm_tags_filter_file_path(),
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_exploded.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter file compact",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter-file",
         osm_tags_filter_file_path(),
         "--compact",
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter grouped",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter",
         '{"group": {"building": true, "highway": ["primary", "secondary"], "amenity": "bench"} }',
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_exploded.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter grouped compact",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-tags-filter",
         '{"group": {"building": true, "highway": ["primary", "secondary"], "amenity": "bench"} }',
         "--compact",
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_654daac5550b95c8c0e3c57a75a1e16dfa638946461e0977af8f9ca98039db06_compact.parquet",
 )  # type: ignore
 @P.case(
     "Filter OSM features IDs",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--filter-osm-ids",
         "way/94399646,node/3617982224,relation/36990",
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.parquet",
 )  # type: ignore
 @P.case(
     "Keep all tags",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--keep-all-tags",
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter with keep all tags",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--keep-all-tags",
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter with keep all tags compact",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--keep-all-tags",
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
         "--compact",
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_compact.parquet",
 )  # type: ignore
 @P.case(
     "OSM tags filter with keep all tags exploded",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--keep-all-tags",
         "--osm-tags-filter",
         '{"building": true, "highway": ["primary", "secondary"], "amenity": "bench"}',
         "--explode",
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_exploded.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_exploded.parquet",
 )  # type: ignore
 @P.case(
     "OSM way polygon config",
     [
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-way-polygon-config",
         osm_way_config_file_path(),
     ],
-    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.geoparquet",
+    "files/6a869bcfa1a49ade8b76569e48e4142bce29098815bf37e57155a18204f2bbbc_nofilter_compact.parquet",
 )  # type: ignore
 @P.case(
     "Allow not covered geometry",
     [
         "--geom-filter-wkt",
         (
             "POLYGON ((-43.064 29.673, -43.064 29.644, -43.017 29.644,"
             " -43.017 29.673, -43.064 29.673))"
         ),
         "--allow-uncovered-geometry",
         "--ignore-cache",
     ],
-    "files/fa44926c5f128cd438ecbe06d29644849a9de323703076b8ac62ffd7a0747e50_nofilter_compact.geoparquet",
+    "files/fa44926c5f128cd438ecbe06d29644849a9de323703076b8ac62ffd7a0747e50_nofilter_compact.parquet",
 )  # type: ignore
 def test_proper_args_without_pbf(args: list[str], expected_result: str) -> None:
     """Test if runs properly with options."""
     result = runner.invoke(cli.app, [*args, "--osm-extract-source", "any"])
     print(result.stdout)
 
     assert result.exit_code == 0
```

### Comparing `quackosm-0.7.3/tests/base/test_osm_extracts.py` & `quackosm-0.8.0/tests/base/test_osm_extracts.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/tests/base/test_osm_tags_filtering.py` & `quackosm-0.8.0/tests/base/test_osm_tags_filtering.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/tests/base/test_pbf_file_reader.py` & `quackosm-0.8.0/tests/base/test_pbf_file_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 )
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
 from srai.geometry import remove_interiors
 from srai.loaders.download import download_file
 from srai.loaders.osm_loaders.filters import GEOFABRIK_LAYERS, HEX2VEC_FILTER
 
-from quackosm import convert_geometry_to_gpq, get_features_gdf
+from quackosm import convert_geometry_to_gpq, convert_pbf_to_gpq, get_features_gdf
 from quackosm._constants import FEATURES_INDEX, WGS84_CRS
 from quackosm._exceptions import (
     GeometryNotCoveredError,
     GeometryNotCoveredWarning,
     InvalidGeometryFilter,
 )
 from quackosm._osm_tags_filters import GroupedOsmTagsFilter, OsmTagsFilter
@@ -181,15 +181,15 @@
         result_gdf = get_features_gdf(
             file_paths=[
                 monaco_file_path,
                 monaco_file_path,
             ],
             ignore_cache=True,
         )
-        single_result_gdf = PbfFileReader(debug=True).get_features_gdf(
+        single_result_gdf = PbfFileReader(debug_memory=True, debug_times=True).get_features_gdf(
             file_paths=[monaco_file_path], ignore_cache=True
         )
 
         assert result_gdf.index.is_unique
         assert len(result_gdf.index) == len(single_result_gdf.index)
     elif operation_mode == "gpq":
         result = convert_geometry_to_gpq(
@@ -323,14 +323,29 @@
 )
 def test_invalid_geometries(geometry: BaseGeometry):
     """Test if invalid geometry filters raise errors."""
     with pytest.raises(InvalidGeometryFilter):
         PbfFileReader(geometry_filter=geometry)
 
 
+def test_geoparquet_deprecation_warning() -> None:
+    """Test if warning is properly displayed."""
+    monaco_file_path = Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf"
+    convert_pbf_to_gpq(
+        monaco_file_path,
+        ignore_cache=True,
+        result_file_path="files/monaco_nofilter_noclip_compact.geoparquet",
+    )
+    with pytest.warns(DeprecationWarning):
+        convert_pbf_to_gpq(monaco_file_path, ignore_cache=False)
+
+    with pytest.warns(DeprecationWarning):
+        get_features_gdf(monaco_file_path, ignore_cache=False)
+
+
 @pytest.mark.parametrize(  # type: ignore
     "geometry",
     [
         box(
             minx=7.416486207767861,
             miny=43.7310867041912,
             maxx=7.421931388477276,
@@ -537,15 +552,15 @@
     Test downloads prepared pbf files and parsed geoparquet using GDAL from kraina-ai/srai-test-
     files repository.
     """
     pbf_file_download_url = LFS_DIRECTORY_URL + f"{extract_name}-latest.osm.pbf"
     pbf_file_path = Path(__file__).parent.parent / "files" / f"{extract_name}.osm.pbf"
     download_file(pbf_file_download_url, str(pbf_file_path), force_download=True)
     gpq_file_download_url = LFS_DIRECTORY_URL + f"{extract_name}-latest.geoparquet"
-    gpq_file_path = Path(__file__).parent.parent / "files" / f"{extract_name}.geoparquet"
+    gpq_file_path = Path(__file__).parent.parent / "files" / f"{extract_name}.parquet"
     download_file(gpq_file_download_url, str(gpq_file_path), force_download=True)
 
     reader = PbfFileReader()
     duckdb_gdf = reader.get_features_gdf([pbf_file_path], explode_tags=False, ignore_cache=True)
     gdal_gdf = gpd.read_parquet(gpq_file_path)
     gdal_gdf["tags"] = gdal_gdf["tags"].apply(json.loads)
```

### Comparing `quackosm-0.7.3/tests/benchmark/test_big_file.py` & `quackosm-0.8.0/tests/benchmark/test_big_file.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/tests/optional_imports/test_optional_cli_dependency.py` & `quackosm-0.8.0/tests/optional_imports/test_optional_cli_dependency.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 @pytest.fixture  # type: ignore
 def optional_packages() -> list[str]:
     """Get a list with optional packages."""
     return [
         "typer",
         "click",
-        "rich",
         "osmnx",
         "h3",
         "h3ronpy",
         "s2",
         "geohash",
     ]
```

### Comparing `quackosm-0.7.3/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `quackosm-0.8.0/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `quackosm-0.8.0/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `quackosm-0.8.0/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/tests/test_files/monaco.osm.pbf` & `quackosm-0.8.0/tests/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/tests/test_files/monaco_boundary.geojson` & `quackosm-0.8.0/tests/test_files/monaco_boundary.geojson`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.3/PKG-INFO` & `quackosm-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuackOSM
-Version: 0.7.3
+Version: 0.8.0
 Summary: An open-source tool for reading OpenStreetMap PBF files using DuckDB
 Author-Email: Kamil Raczycki <kraczycki@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -19,32 +19,33 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Project-URL: Homepage, https://kraina-ai.github.io/quackosm
 Project-URL: Repository, https://github.com/kraina-ai/quackosm
 Project-URL: Documentation, https://kraina-ai.github.io/quackosm
 Project-URL: Changelog, https://github.com/kraina-ai/quackosm/blob/main/CHANGELOG.md
 Requires-Python: >=3.9
-Requires-Dist: geopandas
+Requires-Dist: geopandas>=0.6
 Requires-Dist: shapely>=2
-Requires-Dist: pyarrow>=13.0.0
+Requires-Dist: pyarrow>=14.0.0
 Requires-Dist: duckdb>=0.10.2
 Requires-Dist: geoarrow-pyarrow>=0.1.2
-Requires-Dist: typeguard
-Requires-Dist: psutil
-Requires-Dist: pooch
-Requires-Dist: tqdm
+Requires-Dist: typeguard>=3.0.0
+Requires-Dist: psutil>=5.6.2
+Requires-Dist: pooch>=1.6.0
+Requires-Dist: tqdm>=4.42.0
 Requires-Dist: beautifulsoup4
 Requires-Dist: pyarrow-ops
 Requires-Dist: requests
+Requires-Dist: polars>=0.19.4
+Requires-Dist: rich>=10.11.0
 Requires-Dist: typer[all]>=0.9.0; extra == "cli"
-Requires-Dist: osmnx; extra == "cli"
+Requires-Dist: osmnx>=1.3.0; extra == "cli"
 Requires-Dist: h3>=4.0.0b1; extra == "cli"
-Requires-Dist: h3ronpy>=0.18.0; extra == "cli"
-Requires-Dist: s2; extra == "cli"
-Requires-Dist: python-geohash; extra == "cli"
+Requires-Dist: s2>=0.1.9; extra == "cli"
+Requires-Dist: python-geohash>=0.8; extra == "cli"
 Provides-Extra: cli
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img width="300" src="https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/logos/quackosm_logo.png"><br/>
   <small>Generated using DALL·E 3 model with this prompt: A logo for a python library with White background, high quality, 8k. Cute duck and globe with cartography elements. Library for reading OpenStreetMap data using DuckDB.</small>
 </p>
@@ -114,50 +115,50 @@
 
 ### Dependencies
 
 Required:
 
 - `duckdb (>=0.10.2)`: For all DuckDB operations on PBF files
 
-- `pyarrow (>=13.0.0)`: For parquet files wrangling
+- `pyarrow (>=14.0.0)`: For parquet files wrangling
 
 - `pyarrow-ops`: For easy removal of duplicated features in parquet files
 
 - `geoarrow-pyarrow (>=0.1.2)`: For GeoParquet IO operations
 
-- `geopandas`: For returning GeoDataFrames and reading Geo files
+- `geopandas (>=0.6)`: For returning GeoDataFrames and reading Geo files
 
 - `shapely (>=2.0)`: For parsing WKT and GeoJSON strings and fixing geometries
 
-- `typeguard`: For internal validation of types
+- `polars (>=0.19.4)`: For faster OSM ways grouping operation
 
-- `psutil`: For automatic scaling of parameters based on available resources
+- `typeguard (>=3.0)`: For internal validation of types
 
-- `pooch`: For downloading `*.osm.pbf` files
+- `psutil (>=5.6.2)`: For automatic scaling of parameters based on available resources
 
-- `tqdm`: For showing progress bars
+- `pooch (>=1.6.0)`: For downloading `*.osm.pbf` files
+
+- `rich (>=10.11.0)` & `tqdm (>=4.42.0)`: For showing progress bars
 
 - `requests`: For iterating OSM PBF files services
 
 - `beautifulsoup4`: For parsing HTML files and scraping required information
 
 
 Optional:
 
 - `typer[all] (>=0.9.0)` (click, colorama, rich, shellingham): For CLI
 
-- `osmnx`: For geocoding of strings in CLI
+- `osmnx (>=1.3.0)`: For geocoding of strings in CLI
 
 - `h3 (>=4.0.0b1)`: For reading H3 strings in CLI
 
-- `h3ronpy (>=0.18.0)`: For transforming H3 indexes into geometries
-
-- `s2`: For transforming S2 indexes into geometries
+- `s2 (>=0.1.9)`: For transforming S2 indexes into geometries
 
-- `python-geohash`: For transforming GeoHash indexes into geometries
+- `python-geohash (>=0.8)`: For transforming GeoHash indexes into geometries
 
 ## Usage
 
 ### If you already have downloaded the PBF file 📁🗺️
 
 #### Load data as a GeoDataFrame
 
@@ -183,15 +184,15 @@
 
 #### Just convert PBF to GeoParquet
 
 ```python
 >>> import quackosm as qosm
 >>> gpq_path = qosm.convert_pbf_to_gpq(monaco_pbf_path)
 >>> gpq_path.as_posix()
-'files/monaco_nofilter_noclip_compact.geoparquet'
+'files/monaco_nofilter_noclip_compact.parquet'
 ```
 
 #### Inspect the file with duckdb
 
 ```python
 >>> import duckdb
 >>> duckdb.load_extension('spatial')
@@ -269,15 +270,15 @@
 ⠋ [27.2/32] Saving relations outer parts - invalid geometries • 0:00:00
 ⠋ [  28/32] Saving relations outer parts with holes • 0:00:00
 ⠋ [  29/32] Saving relations outer parts without holes • 0:00:00
 ⠙ [  30/32] Saving filtered relations with geometries • 0:00:00
 ⠹ [31.1/32] Saving valid features • 0:00:00
 ⠋ [  32/32] Saving final geoparquet file • 0:00:00
 Finished operation in 0:00:06
-files/monaco_nofilter_noclip_compact.geoparquet
+files/monaco_nofilter_noclip_compact.parquet
 ```
 
 ### Let the QuackOSM automatically download the required OSM PBF files for you 🔎🌍
 
 #### Load data as a GeoDataFrame
 
 ```python
@@ -308,15 +309,15 @@
 >>> import quackosm as qosm
 >>> from shapely import from_wkt
 >>> geometry = from_wkt(
 ...     "POLYGON ((14.4861 35.9107, 14.4861 35.8811, 14.5331 35.8811, 14.5331 35.9107, 14.4861 35.9107))"
 ... )
 >>> gpq_path = qosm.convert_geometry_to_gpq(geometry)
 >>> gpq_path.as_posix()
-'files/4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.geoparquet'
+'files/4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.parquet'
 ```
 
 #### Inspect the file with duckdb
 
 ```python
 >>> import duckdb
 >>> duckdb.load_extension('spatial')
@@ -395,15 +396,15 @@
 ⠋ [27.2/32] Saving relations outer parts - invalid geometries • 0:00:00
 ⠋ [  28/32] Saving relations outer parts with holes • 0:00:00
 ⠋ [  29/32] Saving relations outer parts without holes • 0:00:00
 ⠙ [  30/32] Saving filtered relations with geometries • 0:00:00
 ⠸ [31.1/32] Saving valid features • 0:00:00
 ⠋ [  32/32] Saving final geoparquet file • 0:00:00
 Finished operation in 0:00:39
-files/9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.geoparquet
+files/9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.parquet
 ```
 
 CLI Help output (`QuackOSM -h`):
 ![CLI Help output](https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/cli_help.png)
 
 You can find full API + more examples in the [docs](https://kraina-ai.github.io/quackosm/).
 
@@ -453,34 +454,34 @@
 
 Library utilizes caching system to reduce repeatable computations.
 
 By default, the library is saving results in the `files` directory created in the working directory. Result file name is generated based on the original `*.osm.pbf` file name.
 
 Original file name to be converted: `example.osm.pbf`.
 
-Default output without any filtering: `example_nofilter_noclip_compact.geoparquet`.
+Default output without any filtering: `example_nofilter_noclip_compact.parquet`.
 
 The nofilter part can be replaced by the hash of OSM tags provided for filtering.
-`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.geoparquet`
+`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.parquet`
 
 The noclip part can be replaced by the hash of geometry used for filtering.
-`example_nofilter_430020b6b1ba7bef8ea919b2fb4472dab2972c70a2abae253760a56c29f449c4_compact.geoparquet`
+`example_nofilter_430020b6b1ba7bef8ea919b2fb4472dab2972c70a2abae253760a56c29f449c4_compact.parquet`
 
 The `compact` part can also take the form of `exploded`, it represents the form of OSM tags - either kept together in a single dictionary or split into columns.
 
 When filtering by selecting individual features IDs, an additional hash based on those IDs is appended to the file.
-`example_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.geoparquet`
+`example_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.parquet`
 
 When the `keep_all_tags` parameter is passed while filtering by OSM tags, and additional `alltags` component is added after the osm filter hash part.
-`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.geoparquet`
+`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.parquet`
 
 General schema of multiple segments that are concatenated together:
-`pbf_file_name`\_(`osm_filter_tags_hash_part`/`nofilter`)(\_`alltags`)\_(`clipping_geometry_hash_part`/`noclip`)\_(`compact`/`exploded`)(\_`filter_osm_ids_hash_part`).geoparquet
+`pbf_file_name`\_(`osm_filter_tags_hash_part`/`nofilter`)(\_`alltags`)\_(`clipping_geometry_hash_part`/`noclip`)\_(`compact`/`exploded`)(\_`filter_osm_ids_hash_part`).parquet
 
-> If the WKT mode is turned on, then the result file will be saved with a `parquet` extension and a `_wkt` suffix.
+> If the WKT mode is turned on, then the result file will be saved with a `_wkt` suffix.
 
 ### Memory usage
 
 DuckDB queries requiring `JOIN`, `GROUP` and `ORDER BY` operations are very memory intensive. Because of that, some steps are divided into chunks (groups) with a set number of rows per chunk.
 
 QuackOSM has been roughly tuned to different workloads. The `rows_per_group` variable is set based on an available memory in the system:
 
@@ -489,20 +490,20 @@
 |     < 8 GB |        100 000 |
 |  8 - 16 GB |        500 000 |
 | 16 - 24 GB |      1 000 000 |
 |    > 24 GB |      5 000 000 |
 
 > WSL usage: sometimes code can break since DuckDB is trying to use all available memory, that can be occupied by Windows.
 
-### Disk usage
+### Resources usage
 
 The algorithm depends on saving intermediate `.parquet` files between queries.
 As a rule of thumb, when parsing a full file without filtering, you should have at least 10x more free space on disk than the base file size (100MB pbf file -> 1GB free space to parse it).
 
-Below you can see the chart of disk usage during operation. Generated on a machine with AMD Ryzen 7 5800X CPU (16 threads, 3.8 GHz clock speed) and 24 GB of RAM.
+Below you can see the chart of resources usage during operation. Generated on a Github Actions Ubuntu virtual machine with 4 threads and 16 GB of memory.
 
 #### Monaco
 
 PBF file size: 525 KB
 
 [Geofabrik link](https://download.geofabrik.de/europe/monaco.html)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: QuackOSM Version: 0.7.3 Summary: An open-source
+Metadata-Version: 2.1 Name: QuackOSM Version: 0.8.0 Summary: An open-source
 tool for reading OpenStreetMap PBF files using DuckDB Author-Email: Kamil
 Raczycki
 kraina.ai> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
@@ -10,23 +10,24 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Operating System :: Unix Classifier: Operating System :: MacOS Classifier:
 Operating System :: Microsoft :: Windows Project-URL: Homepage, https://kraina-
 ai.github.io/quackosm Project-URL: Repository, https://github.com/kraina-ai/
 quackosm Project-URL: Documentation, https://kraina-ai.github.io/quackosm
 Project-URL: Changelog, https://github.com/kraina-ai/quackosm/blob/main/
-CHANGELOG.md Requires-Python: >=3.9 Requires-Dist: geopandas Requires-Dist:
-shapely>=2 Requires-Dist: pyarrow>=13.0.0 Requires-Dist: duckdb>=0.10.2
-Requires-Dist: geoarrow-pyarrow>=0.1.2 Requires-Dist: typeguard Requires-Dist:
-psutil Requires-Dist: pooch Requires-Dist: tqdm Requires-Dist: beautifulsoup4
-Requires-Dist: pyarrow-ops Requires-Dist: requests Requires-Dist: typer
-[all]>=0.9.0; extra == "cli" Requires-Dist: osmnx; extra == "cli" Requires-
-Dist: h3>=4.0.0b1; extra == "cli" Requires-Dist: h3ronpy>=0.18.0; extra ==
-"cli" Requires-Dist: s2; extra == "cli" Requires-Dist: python-geohash; extra ==
-"cli" Provides-Extra: cli Description-Content-Type: text/markdown
+CHANGELOG.md Requires-Python: >=3.9 Requires-Dist: geopandas>=0.6 Requires-
+Dist: shapely>=2 Requires-Dist: pyarrow>=14.0.0 Requires-Dist: duckdb>=0.10.2
+Requires-Dist: geoarrow-pyarrow>=0.1.2 Requires-Dist: typeguard>=3.0.0
+Requires-Dist: psutil>=5.6.2 Requires-Dist: pooch>=1.6.0 Requires-Dist:
+tqdm>=4.42.0 Requires-Dist: beautifulsoup4 Requires-Dist: pyarrow-ops Requires-
+Dist: requests Requires-Dist: polars>=0.19.4 Requires-Dist: rich>=10.11.0
+Requires-Dist: typer[all]>=0.9.0; extra == "cli" Requires-Dist: osmnx>=1.3.0;
+extra == "cli" Requires-Dist: h3>=4.0.0b1; extra == "cli" Requires-Dist:
+s2>=0.1.9; extra == "cli" Requires-Dist: python-geohash>=0.8; extra == "cli"
+Provides-Extra: cli Description-Content-Type: text/markdown
  [https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/logos/
                               quackosm_logo.png]
  Generated using DALLÂ·E 3 model with this prompt: A logo for a python library
  with White background, high quality, 8k. Cute duck and globe with cartography
         elements. Library for reading OpenStreetMap data using DuckDB.
  [GitHub][Checks]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _-_ _D_E_V_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _-_ _P_R_O_D_]
  _[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]_[_C_o_d_e_F_a_c_t_o_r_ _G_r_a_d_e_]_[_C_o_d_e_c_o_v_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d
@@ -42,48 +43,49 @@
 as Python module as well as a beautiful CLI based on `Typer`[^4]. [^1]: [DuckDB
 Website](https://duckdb.org/) [^2]: [DuckDB Spatial extension repository]
 (https://github.com/duckdb/duckdb_spatial) [^3]: [GeoParquet data format]
 (https://geoparquet.org/) [^4]: [Typer docs](https://typer.tiangolo.com/) ##
 Installing ### As pure Python module ``` pip install quackosm ``` ### With
 beautiful CLI ``` pip install quackosm[cli] ``` ### Required Python version?
 QuackOSM supports **Python >= 3.9** ### Dependencies Required: - `duckdb
-(>=0.10.2)`: For all DuckDB operations on PBF files - `pyarrow (>=13.0.0)`: For
+(>=0.10.2)`: For all DuckDB operations on PBF files - `pyarrow (>=14.0.0)`: For
 parquet files wrangling - `pyarrow-ops`: For easy removal of duplicated
 features in parquet files - `geoarrow-pyarrow (>=0.1.2)`: For GeoParquet IO
-operations - `geopandas`: For returning GeoDataFrames and reading Geo files -
-`shapely (>=2.0)`: For parsing WKT and GeoJSON strings and fixing geometries -
-`typeguard`: For internal validation of types - `psutil`: For automatic scaling
-of parameters based on available resources - `pooch`: For downloading
-`*.osm.pbf` files - `tqdm`: For showing progress bars - `requests`: For
-iterating OSM PBF files services - `beautifulsoup4`: For parsing HTML files and
-scraping required information Optional: - `typer[all] (>=0.9.0)` (click,
-colorama, rich, shellingham): For CLI - `osmnx`: For geocoding of strings in
-CLI - `h3 (>=4.0.0b1)`: For reading H3 strings in CLI - `h3ronpy (>=0.18.0)`:
-For transforming H3 indexes into geometries - `s2`: For transforming S2 indexes
-into geometries - `python-geohash`: For transforming GeoHash indexes into
-geometries ## Usage ### If you already have downloaded the PBF file ððºï¸
-#### Load data as a GeoDataFrame ```python >>> import quackosm as qosm >>>
-qosm.get_features_gdf(monaco_pbf_path) tags geometry feature_id node/
-10005045289 {'shop': 'bakery'} POINT (7.42245 43.73105) node/10020887517
-{'leisure': 'swimming_pool', ... POINT (7.41316 43.73384) node/10021298117
-{'leisure': 'swimming_pool', ... POINT (7.42777 43.74277) node/10021298717
-{'leisure': 'swimming_pool', ... POINT (7.42630 43.74097) node/10025656383
-{'ferry': 'yes', 'name': 'Qua... POINT (7.42550 43.73690) ... ... ... way/
-990669427 {'amenity': 'shelter', 'shelt... POLYGON ((7.41461 43.7338... way/
-990669428 {'highway': 'secondary', 'jun... LINESTRING (7.41366 43.73... way/
-990669429 {'highway': 'secondary', 'jun... LINESTRING (7.41376 43.73... way/
-990848785 {'addr:city': 'Monaco', 'addr... POLYGON ((7.41426 43.7339... way/
-993121275 {'building': 'yes', 'name': ... POLYGON ((7.43214 43.7481... [7906
-rows x 2 columns] ``` #### Just convert PBF to GeoParquet ```python >>> import
-quackosm as qosm >>> gpq_path = qosm.convert_pbf_to_gpq(monaco_pbf_path) >>>
-gpq_path.as_posix() 'files/monaco_nofilter_noclip_compact.geoparquet' ``` ####
-Inspect the file with duckdb ```python >>> import duckdb >>>
-duckdb.load_extension('spatial') >>> duckdb.read_parquet(str(gpq_path)).project
-( ... "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)" ... ).order
-("feature_id")
+operations - `geopandas (>=0.6)`: For returning GeoDataFrames and reading Geo
+files - `shapely (>=2.0)`: For parsing WKT and GeoJSON strings and fixing
+geometries - `polars (>=0.19.4)`: For faster OSM ways grouping operation -
+`typeguard (>=3.0)`: For internal validation of types - `psutil (>=5.6.2)`: For
+automatic scaling of parameters based on available resources - `pooch
+(>=1.6.0)`: For downloading `*.osm.pbf` files - `rich (>=10.11.0)` & `tqdm
+(>=4.42.0)`: For showing progress bars - `requests`: For iterating OSM PBF
+files services - `beautifulsoup4`: For parsing HTML files and scraping required
+information Optional: - `typer[all] (>=0.9.0)` (click, colorama, rich,
+shellingham): For CLI - `osmnx (>=1.3.0)`: For geocoding of strings in CLI -
+`h3 (>=4.0.0b1)`: For reading H3 strings in CLI - `s2 (>=0.1.9)`: For
+transforming S2 indexes into geometries - `python-geohash (>=0.8)`: For
+transforming GeoHash indexes into geometries ## Usage ### If you already have
+downloaded the PBF file ððºï¸ #### Load data as a GeoDataFrame ```python
+>>> import quackosm as qosm >>> qosm.get_features_gdf(monaco_pbf_path) tags
+geometry feature_id node/10005045289 {'shop': 'bakery'} POINT (7.42245
+43.73105) node/10020887517 {'leisure': 'swimming_pool', ... POINT (7.41316
+43.73384) node/10021298117 {'leisure': 'swimming_pool', ... POINT (7.42777
+43.74277) node/10021298717 {'leisure': 'swimming_pool', ... POINT (7.42630
+43.74097) node/10025656383 {'ferry': 'yes', 'name': 'Qua... POINT (7.42550
+43.73690) ... ... ... way/990669427 {'amenity': 'shelter', 'shelt... POLYGON (
+(7.41461 43.7338... way/990669428 {'highway': 'secondary', 'jun... LINESTRING
+(7.41366 43.73... way/990669429 {'highway': 'secondary', 'jun... LINESTRING
+(7.41376 43.73... way/990848785 {'addr:city': 'Monaco', 'addr... POLYGON (
+(7.41426 43.7339... way/993121275 {'building': 'yes', 'name': ... POLYGON (
+(7.43214 43.7481... [7906 rows x 2 columns] ``` #### Just convert PBF to
+GeoParquet ```python >>> import quackosm as qosm >>> gpq_path =
+qosm.convert_pbf_to_gpq(monaco_pbf_path) >>> gpq_path.as_posix() 'files/
+monaco_nofilter_noclip_compact.parquet' ``` #### Inspect the file with duckdb
+```python >>> import duckdb >>> duckdb.load_extension('spatial') >>>
+duckdb.read_parquet(str(gpq_path)).project( ... "* REPLACE (ST_GeomFromWKB
+(geometry) AS geometry)" ... ).order("feature_id")
 ââââââââââââââââââââ¬âââââââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââ
 â feature_id â tags â geometry â â varchar â map(varchar, varchâ¦
 â geometry â
 ââââââââââââââââââââ¼âââââââââââââââââââââââ¼âââââââââââââââââââââââââââââââââââââââââââââââ¤
 â node/10005045289 â {shop=bakery} â POINT (7.4224498 43.7310532) â â
 node/10020887517 â {leisure=swimming_â¦ â POINT (7.4131561 43.7338391) â
 â node/10021298117 â {leisure=swimming_â¦ â POINT (7.4277743 43.7427669)
@@ -142,35 +144,35 @@
 Saving relations inner parts - invalid geometries â¢ 0:00:00 â  [27.1/32]
 Saving relations outer parts - valid geometries â¢ 0:00:00 â  [27.2/32]
 Saving relations outer parts - invalid geometries â¢ 0:00:00 â  [ 28/32]
 Saving relations outer parts with holes â¢ 0:00:00 â  [ 29/32] Saving
 relations outer parts without holes â¢ 0:00:00 â  [ 30/32] Saving filtered
 relations with geometries â¢ 0:00:00 â ¹ [31.1/32] Saving valid features â¢
 0:00:00 â  [ 32/32] Saving final geoparquet file â¢ 0:00:00 Finished
-operation in 0:00:06 files/monaco_nofilter_noclip_compact.geoparquet ``` ###
-Let the QuackOSM automatically download the required OSM PBF files for you
-ðð #### Load data as a GeoDataFrame ```python >>> import quackosm as qosm
->>> import osmnx as ox >>> geometry = ox.geocode_to_gdf("Vatican
-City").unary_union >>> qosm.get_features_gdf_from_geometry(geometry) tags
-geometry feature_id node/10253371713 {'crossing': 'uncontrolled',... POINT
-(12.45603 41.90454) node/10253371714 {'highway': 'stop'} POINT (12.45705
-41.90400) node/10253371715 {'highway': 'stop'} POINT (12.45242 41.90164) node/
-10253371720 {'artwork_type': 'statue',... POINT (12.45147 41.90484) node/
-10253371738 {'natural': 'tree'} POINT (12.45595 41.90609) ... ... ... way/
-983015528 {'barrier': 'hedge', 'height'... POLYGON ((12.45027 41.901... way/
-983015529 {'barrier': 'hedge', 'height'... POLYGON ((12.45028 41.901... way/
-983015530 {'barrier': 'hedge', 'height'... POLYGON ((12.45023 41.901... way/
-998561138 {'barrier': 'bollard', 'bicyc... LINESTRING (12.45821 41.9... way/
-998561139 {'barrier': 'bollard', 'bicyc... LINESTRING (12.45828 41.9... [3286
-rows x 2 columns] ``` #### Just convert geometry to GeoParquet ```python >>>
-import quackosm as qosm >>> from shapely import from_wkt >>> geometry =
-from_wkt( ... "POLYGON ((14.4861 35.9107, 14.4861 35.8811, 14.5331 35.8811,
-14.5331 35.9107, 14.4861 35.9107))" ... ) >>> gpq_path =
-qosm.convert_geometry_to_gpq(geometry) >>> gpq_path.as_posix() 'files/
-4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.geoparquet'
+operation in 0:00:06 files/monaco_nofilter_noclip_compact.parquet ``` ### Let
+the QuackOSM automatically download the required OSM PBF files for you ðð
+#### Load data as a GeoDataFrame ```python >>> import quackosm as qosm >>>
+import osmnx as ox >>> geometry = ox.geocode_to_gdf("Vatican City").unary_union
+>>> qosm.get_features_gdf_from_geometry(geometry) tags geometry feature_id
+node/10253371713 {'crossing': 'uncontrolled',... POINT (12.45603 41.90454)
+node/10253371714 {'highway': 'stop'} POINT (12.45705 41.90400) node/10253371715
+{'highway': 'stop'} POINT (12.45242 41.90164) node/10253371720 {'artwork_type':
+'statue',... POINT (12.45147 41.90484) node/10253371738 {'natural': 'tree'}
+POINT (12.45595 41.90609) ... ... ... way/983015528 {'barrier': 'hedge',
+'height'... POLYGON ((12.45027 41.901... way/983015529 {'barrier': 'hedge',
+'height'... POLYGON ((12.45028 41.901... way/983015530 {'barrier': 'hedge',
+'height'... POLYGON ((12.45023 41.901... way/998561138 {'barrier': 'bollard',
+'bicyc... LINESTRING (12.45821 41.9... way/998561139 {'barrier': 'bollard',
+'bicyc... LINESTRING (12.45828 41.9... [3286 rows x 2 columns] ``` #### Just
+convert geometry to GeoParquet ```python >>> import quackosm as qosm >>> from
+shapely import from_wkt >>> geometry = from_wkt( ... "POLYGON ((14.4861
+35.9107, 14.4861 35.8811, 14.5331 35.8811, 14.5331 35.9107, 14.4861 35.9107))"
+... ) >>> gpq_path = qosm.convert_geometry_to_gpq(geometry) >>>
+gpq_path.as_posix() 'files/
+4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.parquet'
 ``` #### Inspect the file with duckdb ```python >>> import duckdb >>>
 duckdb.load_extension('spatial') >>> duckdb.read_parquet(str(gpq_path)).project
 ( ... "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)" ... ).order
 ("feature_id")
 ââââââââââââââââââââ¬âââââââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââ
 â feature_id â tags â geometry â â varchar â map(varchar, varchâ¦
 â geometry â
@@ -237,15 +239,15 @@
 Saving relations outer parts - valid geometries â¢ 0:00:00 â  [27.2/32]
 Saving relations outer parts - invalid geometries â¢ 0:00:00 â  [ 28/32]
 Saving relations outer parts with holes â¢ 0:00:00 â  [ 29/32] Saving
 relations outer parts without holes â¢ 0:00:00 â  [ 30/32] Saving filtered
 relations with geometries â¢ 0:00:00 â ¸ [31.1/32] Saving valid features â¢
 0:00:00 â  [ 32/32] Saving final geoparquet file â¢ 0:00:00 Finished
 operation in 0:00:39 files/
-9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.geoparquet
+9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.parquet
 ``` CLI Help output (`QuackOSM -h`): ![CLI Help output](https://
 raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
 cli_help.png) You can find full API + more examples in the [docs](https://
 kraina-ai.github.io/quackosm/). ## How does it work? ### Basic logic QuackOSM
 utilizes `ST_ReadOSM` function from `DuckDB`'s `Spatial` extension to read raw
 data from the PBF file: - **Nodes** with coordinates and tags; - **Ways** with
 nodes refs and tags; - **Relations** with nodes and ways refs, ref roles and
@@ -274,52 +276,51 @@
 with weird artifacts by `GDAL`. You can inspect the comparison algorithm in the
 `test_gdal_parity` function from `tests/base/test_pbf_file_reader.py` file. ###
 Caching Library utilizes caching system to reduce repeatable computations. By
 default, the library is saving results in the `files` directory created in the
 working directory. Result file name is generated based on the original
 `*.osm.pbf` file name. Original file name to be converted: `example.osm.pbf`.
 Default output without any filtering:
-`example_nofilter_noclip_compact.geoparquet`. The nofilter part can be replaced
-by the hash of OSM tags provided for filtering.
-`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.geoparquet`
+`example_nofilter_noclip_compact.parquet`. The nofilter part can be replaced by
+the hash of OSM tags provided for filtering.
+`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_noclip_exploded.parquet`
 The noclip part can be replaced by the hash of geometry used for filtering.
-`example_nofilter_430020b6b1ba7bef8ea919b2fb4472dab2972c70a2abae253760a56c29f449c4_compact.geoparquet`
+`example_nofilter_430020b6b1ba7bef8ea919b2fb4472dab2972c70a2abae253760a56c29f449c4_compact.parquet`
 The `compact` part can also take the form of `exploded`, it represents the form
 of OSM tags - either kept together in a single dictionary or split into
 columns. When filtering by selecting individual features IDs, an additional
 hash based on those IDs is appended to the file.
-`example_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.geoparquet`
+`example_nofilter_noclip_compact_c740a1597e53ae8c5e98c5119eaa1893ddc177161afe8642addcbe54a6dc089d.parquet`
 When the `keep_all_tags` parameter is passed while filtering by OSM tags, and
 additional `alltags` component is added after the osm filter hash part.
-`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.geoparquet`
+`example_a9dd1c3c2e3d6a94354464e9a1a536ef44cca77eebbd882f48ca52799eb4ca91_alltags_noclip_compact.parquet`
 General schema of multiple segments that are concatenated together:
 `pbf_file_name`\_(`osm_filter_tags_hash_part`/`nofilter`)(\_`alltags`)\_
 (`clipping_geometry_hash_part`/`noclip`)\_(`compact`/`exploded`)
-(\_`filter_osm_ids_hash_part`).geoparquet > If the WKT mode is turned on, then
-the result file will be saved with a `parquet` extension and a `_wkt` suffix.
-### Memory usage DuckDB queries requiring `JOIN`, `GROUP` and `ORDER BY`
-operations are very memory intensive. Because of that, some steps are divided
-into chunks (groups) with a set number of rows per chunk. QuackOSM has been
-roughly tuned to different workloads. The `rows_per_group` variable is set
-based on an available memory in the system: | Memory | Rows per group | | -----
-----: | -------------: | | < 8 GB | 100 000 | | 8 - 16 GB | 500 000 | | 16 - 24
-GB | 1 000 000 | | > 24 GB | 5 000 000 | > WSL usage: sometimes code can break
-since DuckDB is trying to use all available memory, that can be occupied by
-Windows. ### Disk usage The algorithm depends on saving intermediate `.parquet`
-files between queries. As a rule of thumb, when parsing a full file without
-filtering, you should have at least 10x more free space on disk than the base
-file size (100MB pbf file -> 1GB free space to parse it). Below you can see the
-chart of disk usage during operation. Generated on a machine with AMD Ryzen 7
-5800X CPU (16 threads, 3.8 GHz clock speed) and 24 GB of RAM. #### Monaco PBF
-file size: 525 KB [Geofabrik link](https://download.geofabrik.de/europe/
-monaco.html) ![Monaco PBF file result](https://raw.githubusercontent.com/
-kraina-ai/quackosm/main/docs/assets/images/monaco_disk_spillage.png) ####
-Estonia PBF file size: 100 MB [Geofabrik link](https://download.geofabrik.de/
-europe/estonia.html) ![Estonia PBF file result](https://
+(\_`filter_osm_ids_hash_part`).parquet > If the WKT mode is turned on, then the
+result file will be saved with a `_wkt` suffix. ### Memory usage DuckDB queries
+requiring `JOIN`, `GROUP` and `ORDER BY` operations are very memory intensive.
+Because of that, some steps are divided into chunks (groups) with a set number
+of rows per chunk. QuackOSM has been roughly tuned to different workloads. The
+`rows_per_group` variable is set based on an available memory in the system: |
+Memory | Rows per group | | ---------: | -------------: | | < 8 GB | 100 000 |
+| 8 - 16 GB | 500 000 | | 16 - 24 GB | 1 000 000 | | > 24 GB | 5 000 000 | >
+WSL usage: sometimes code can break since DuckDB is trying to use all available
+memory, that can be occupied by Windows. ### Resources usage The algorithm
+depends on saving intermediate `.parquet` files between queries. As a rule of
+thumb, when parsing a full file without filtering, you should have at least 10x
+more free space on disk than the base file size (100MB pbf file -> 1GB free
+space to parse it). Below you can see the chart of resources usage during
+operation. Generated on a Github Actions Ubuntu virtual machine with 4 threads
+and 16 GB of memory. #### Monaco PBF file size: 525 KB [Geofabrik link](https:/
+/download.geofabrik.de/europe/monaco.html) ![Monaco PBF file result](https://
 raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
+monaco_disk_spillage.png) #### Estonia PBF file size: 100 MB [Geofabrik link]
+(https://download.geofabrik.de/europe/estonia.html) ![Estonia PBF file result]
+(https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
 estonia_disk_spillage.png) #### Poland PBF file size: 1.7 GB [Geofabrik link]
 (https://download.geofabrik.de/europe/poland.html) ![Poland PBF file result]
 (https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
 poland_disk_spillage.png) ## License The library is distributed under Apache-
 2.0 License. The free [OpenStreetMap](https://www.openstreetmap.org/) data,
 which is used for the development of QuackOSM, is licensed under the [Open Data
 Commons Open Database License](https://opendatacommons.org/licenses/odbl/)
```

