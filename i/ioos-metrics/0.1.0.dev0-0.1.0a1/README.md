# Comparing `tmp/ioos_metrics-0.1.0.dev0.tar.gz` & `tmp/ioos_metrics-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioos_metrics-0.1.0.dev0.tar", last modified: Sun Apr 14 15:18:57 2024, max compression
+gzip compressed data, was "ioos_metrics-0.1.0a1.tar", last modified: Thu May  9 08:01:00 2024, max compression
```

## Comparing `ioos_metrics-0.1.0.dev0.tar` & `ioos_metrics-0.1.0a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-04-14 15:18:57.124574 ioos_metrics-0.1.0.dev0/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1070 2023-09-28 14:26:25.000000 ioos_metrics-0.1.0.dev0/LICENSE
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      411 2024-04-14 15:16:56.000000 ioos_metrics-0.1.0.dev0/MANIFEST.in
--rw-r--r--   0 filipe    (1000) filipe    (1000)     4086 2024-04-14 15:18:57.124574 ioos_metrics-0.1.0.dev0/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1908 2024-02-13 16:43:47.000000 ioos_metrics-0.1.0.dev0/README.md
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-04-14 15:18:57.124574 ioos_metrics-0.1.0.dev0/ioos_metrics/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      124 2024-04-03 18:54:15.000000 ioos_metrics-0.1.0.dev0/ioos_metrics/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    21416 2024-04-09 15:55:50.000000 ioos_metrics-0.1.0.dev0/ioos_metrics/ioos_metrics.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     4904 2024-04-09 13:43:56.000000 ioos_metrics-0.1.0.dev0/ioos_metrics/national_platforms.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-04-14 15:18:57.124574 ioos_metrics-0.1.0.dev0/ioos_metrics.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      133 2024-04-14 15:18:57.000000 ioos_metrics-0.1.0.dev0/ioos_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1313 2024-04-14 15:11:41.000000 ioos_metrics-0.1.0.dev0/pyproject.toml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2024-04-14 15:18:57.124574 ioos_metrics-0.1.0.dev0/setup.cfg
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1070 2024-04-17 14:27:47.000000 ioos_metrics-0.1.0a1/LICENSE
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      427 2024-05-09 07:56:45.000000 ioos_metrics-0.1.0a1/MANIFEST.in
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     4083 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/PKG-INFO
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1908 2024-04-17 14:27:47.000000 ioos_metrics-0.1.0a1/README.md
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/ioos_metrics/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      124 2024-04-17 14:27:47.000000 ioos_metrics-0.1.0a1/ioos_metrics/__init__.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    21689 2024-05-08 18:41:21.000000 ioos_metrics-0.1.0a1/ioos_metrics/ioos_metrics.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     5037 2024-05-02 14:12:37.000000 ioos_metrics-0.1.0a1/ioos_metrics/national_platforms.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/ioos_metrics.egg-info/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      133 2024-05-09 08:01:00.000000 ioos_metrics-0.1.0a1/ioos_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1313 2024-05-02 14:12:37.000000 ioos_metrics-0.1.0a1/pyproject.toml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/setup.cfg
```

### Comparing `ioos_metrics-0.1.0.dev0/LICENSE` & `ioos_metrics-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ioos_metrics-0.1.0.dev0/PKG-INFO` & `ioos_metrics-0.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioos_metrics
-Version: 0.1.0.dev0
+Version: 0.1.0a1
 Summary: Package to fetch various metrics for IOOS by the numbers
 Maintainer: Filipe Fernandes
 License: MIT License
         
         Copyright (c) 2021 Mathew Biddle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ioos_metrics-0.1.0.dev0/README.md` & `ioos_metrics-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `ioos_metrics-0.1.0.dev0/ioos_metrics/ioos_metrics.py` & `ioos_metrics-0.1.0a1/ioos_metrics/ioos_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 """Code extracted from IOOS_BTN.ipynb."""
 
 import functools
 import io
 import logging
 
+import httpx
 import joblib
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from fake_useragent import UserAgent
 from gliderpy.fetchers import GliderDataFetcher
+from shapely.geometry import LineString
 
-from ioos_metrics.national_platforms import (
-    get_cbibs,
-    get_cdip,
-    get_coops,
-    get_ndbc,
-    get_nerrs,
-    get_oap,
-)
+from ioos_metrics.national_platforms import national_platforms
 
+logger = logging.getLogger(__name__)
 logging.basicConfig(
-    filename="metric.log",
+    filename="metrics.log",
     encoding="utf-8",
-    level=logging.DEBUG,
+    level=logging.INFO,
 )
 
 ua = UserAgent()
 _HEADERS = {
     "User-Agent": ua.random,
 }
 
@@ -61,15 +57,15 @@
 
 
 def _compare_metrics(column, num) -> str:
     """Compares last stored metric against the new one and report if it is up, down, or the same."""
     last_row = previous_metrics().iloc[-1]
     date = last_row["date_UTC"]
     if num is None:
-        msg = f"[{date}] : {column} failed."
+        return f"[{date}] : {column} failed."
 
     old = last_row[column]
     if old == num:
         msg = f"[{date}] : {column} equal {num} = {old}."
     elif num < old:
         msg = f"[{date}] : {column} down {num} < {old}."
     elif num > old:
@@ -89,15 +85,15 @@
     url = "https://ioos.noaa.gov/community/national#federal"
 
     html = requests.get(url, headers=_HEADERS, timeout=10).text
 
     df = pd.read_html(io.StringIO(html))
     df_clean = df[1].drop(columns=[0, 2])
     df_fed_partners = pd.concat([df_clean[1], df_clean[3]]).dropna().reset_index()
-    logging.info(f"{df_fed_partners[0].to_string()=}")
+    logger.info(f"{df_fed_partners[0].to_string()=}")
     return df_fed_partners.shape[0]
 
 
 @functools.lru_cache(maxsize=128)
 def ngdac_gliders_fast(min_time="2000-01-01T00:00:00Z", max_time="2023-12-31T23:59:59Z") -> int:
     """NGDAC Glider Days.
 
@@ -131,15 +127,15 @@
 
     # We don't want allDatasets in our numbers.
     df = df.loc[~(df["datasetID"] == "allDatasets")]
 
     # Check if any value is NaN and report it.
     if df.isna().sum().sum():
         rows = df.loc[df.isna().sum(axis=1).astype(bool)]
-        logging.warning(f"The following rows have missing data:\n{rows}")
+        logger.warning(f"The following rows have missing data:\n{rows}")
 
     df = df.dropna(
         axis=0,
     )
 
     # drop delayed datasets
     df = df.loc[~df["datasetID"].str.contains("delayed")]
@@ -154,31 +150,28 @@
     df = df["maxTime (UTC)"].apply(lambda x: x.ceil("D")) - df["minTime (UTC)"].apply(
         lambda x: x.floor("D"),
     )
     return df.sum().days
 
 
 @functools.lru_cache(maxsize=128)
-def _ngdac_gliders(  # noqa: PLR0913
-    *,
-    min_time="2000-01-01T00:00:00",
-    max_time="2023-12-31T23:59:59",
-    min_lat=-90.0,
-    max_lat=90.0,
-    min_lon=-180,
-    max_lon=180,
-) -> pd.DataFrame:
-    """Same as ngdac_gliders but loops over all datasets to return a more accurate estimate for this metric.
-    This approach is slower but can also compute more refined metrics and other variables, like glider profiles.
+def _ngdac_gliders(*, min_time, max_time, min_lat, max_lat, min_lon, max_lon) -> pd.DataFrame:  # noqa: PLR0913
+    """Loops over all datasets found within the bounding box and time-range,
+    and returns a more accurate estimate for this metric.
 
+    This approach can compute more refined metrics and other variables,
+    like glider profiles and hurricane overlaps.
     """
 
     def _extra_info(info_df, attribute_name) -> str:
         """Get 'Attribute Name' 'Value' metadata."""
-        return info_df.loc[info_df["Attribute Name"] == attribute_name]["Value"].squeeze()
+        att = info_df.loc[info_df["Attribute Name"] == attribute_name]["Value"].squeeze()
+        if hasattr(att, "empty"):
+            att = "unknown"
+        return att
 
     def _metadata(info_df) -> dict:
         """Build the metadata a specific dataset_id."""
         return {
             "wmo_id": _extra_info(info_df, attribute_name="wmo_id"),
             "time_coverage_start": _extra_info(
                 info_df,
@@ -203,20 +196,26 @@
             ),
             "geospatial_lon_max": _extra_info(
                 info_df,
                 attribute_name="geospatial_lon_max",
             ),
             "institution": _extra_info(info_df, attribute_name="institution"),
             "sea_name": _extra_info(info_df, attribute_name="sea_name"),
-            "acknowledgment": _extra_info(info_df, attribute_name="acknowledgment"),
+            "acknowledgment": _extra_info(
+                info_df,
+                attribute_name="acknowledgment",
+            ),
         }
 
     def _computed_metadata(dataset_id) -> dict:
-        """Download the minimum amount of data possible for the computed metadata,
-        We cannot get first and last b/c the profile_id is not a contiguous sequence.
+        """Download the minimum amount of data possible for the computed
+        metadata.
+
+        Note that we cannot get first and last b/c the profile_id is not a
+        contiguous sequence.
         """
         glider_grab.fetcher.dataset_id = dataset_id
         glider_grab.fetcher.variables = [
             "profile_id",
             "latitude",
             "longitude",
             "time",
@@ -224,15 +223,15 @@
         df = glider_grab.to_pandas()
         df = df.sort_index()
         days = df.index[-1].ceil("D") - df.index[0].floor("D")
         return {
             "deployment_lat": df["latitude"].iloc[0],
             "deployment_lon": df["longitude"].iloc[0],
             "num_profiles": len(df),
-            # Profiles are not unique! This will results in a smaller profile count.
+            # Profiles are not unique! Cannot use this!!
             # "num_profiles": len(set(df['profile_id']))
             "days": days,
         }
 
     glider_grab = GliderDataFetcher()
 
     df = glider_grab.query(
@@ -242,20 +241,41 @@
         max_lon=max_lon,
         min_time=min_time,
         max_time=max_time,
         delayed=False,  # We do not want delayed gliders.
     )
 
     metadata = {}
+    glider_grab.fetcher.variables = ["longitude", "latitude"]
     for _, row in list(df.iterrows()):
         dataset_id = row["Dataset ID"]
+
+        glider_grab.fetcher.dataset_id = dataset_id
+        track = glider_grab.fetcher.to_pandas(distinct=True)
+        track = LineString(
+            (lon, lat)
+            for (lon, lat) in zip(
+                track["longitude (degrees_east)"],
+                track["latitude (degrees_north)"],
+                strict=False,
+            )
+        )
+
         info_url = row["info_url"].replace("html", "csv")
         info_df = pd.read_csv(info_url)
         info = _metadata(info_df)
-        info.update(_computed_metadata(dataset_id=dataset_id))
+        try:
+            info.update(_computed_metadata(dataset_id=dataset_id))
+        except (httpx.HTTPError, httpx.HTTPStatusError):
+            print(  # noqa: T201
+                f"Could not fetch glider {dataset_id=}. "
+                "This could be a server side error and the metrics will be incomplete!",
+            )
+            continue
+        info.update({"track": track})
         metadata.update({dataset_id: info})
     return pd.DataFrame(metadata).T
 
 
 def ngdac_gliders():
     """Runs _ngdac_gliders for the whole server and returns only the glider days to compare with ngdac_gliders_fast."""
     metadata = _ngdac_gliders()
@@ -282,15 +302,15 @@
 
     html = requests.get(url, headers=_HEADERS, timeout=10).text
 
     soup = BeautifulSoup(html, "html.parser")
 
     for tag in soup.find_all("h2"):
         if tag.text == "Current Projects":
-            logging.info(f"{tag.next_sibling.find_all('li')=}")
+            logger.info(f"{tag.next_sibling.find_all('li')=}")
             comt = len(tag.next_sibling.find_all("li"))
 
     return comt
 
 
 @functools.lru_cache(maxsize=128)
 def regional_associations():
@@ -299,15 +319,15 @@
     url = "https://ioos.noaa.gov/regions/regions-at-a-glance/"
 
     html = requests.get(url, headers=_HEADERS, timeout=10).text
     soup = BeautifulSoup(html, "html.parser")
 
     for tag in soup.find_all("a"):
         if tag.find("strong") is not None:
-            logging.info(f"{tag.find('strong').text=}")
+            logger.info(f"{tag.find('strong').text=}")
             ras += 1
 
     return ras
 
 
 @functools.lru_cache(maxsize=128)
 def regional_platforms():
@@ -369,15 +389,15 @@
     df = pd.read_html(
         io.StringIO(table),
         header=0,
     )
 
     ott_projects = 0
     for entry in df[0]:
-        logging.info(f"{df[0][entry][0].count('new in')=}")
+        logger.info(f"{df[0][entry][0].count('new in')=}")
         ott_projects += df[0][entry][0].count("new in")
     return ott_projects
 
 
 @functools.lru_cache(maxsize=128)
 def qartod_manuals():
     """As of the last update there are twelve QARTOD manuals in-place for IOOS.
@@ -399,15 +419,15 @@
     soup = BeautifulSoup(
         requests.get(url, headers=_HEADERS, timeout=10).text,
         "html.parser",
     )
     qartod = 0
     for tag in soup.find_all("li"):
         if "Real-Time Quality Control of" in tag.text:
-            logging.info(f"{tag.text=}")
+            logger.info(f"{tag.text=}")
             qartod += 1
 
     return qartod
 
 
 @functools.lru_cache(maxsize=128)
 def ioos_core_variables():
@@ -550,58 +570,42 @@
         "Federal Partners": federal_partners,
         "HAB Pilot Projects": hab_pilot_projects,
         "HF Radar Stations": hf_radar_installations,
         "IOOS Core Variables": ioos_core_variables,
         "IOOS": ioos,
         "MBON Projects": mbon_projects,
         "Metadata Records": metadata_records,
+        "National Platforms": national_platforms,
         "NGDAC Glider Days": ngdac_gliders_fast,
         "OTT Projects": ott_projects,
         "QARTOD Manuals": qartod_manuals,
         "Regional Associations": regional_associations,
         "Regional Platforms": regional_platforms,
     }
-    # We do the national platforms separately b/c this one hits multiple services.
-    national_platforms_functions = [
-        get_cbibs,
-        get_cdip,
-        get_coops,
-        get_ndbc,
-        get_nerrs,
-        get_oap,
-    ]
 
     # We cannot write the log in parallel. When debugging we should run the queries in seral mode.
     if debug:
         for column, function in functions.items():
             try:
                 num = function()
             except Exception:
-                logging.exception(f"{function=} failed.")
+                logger.exception(f"{column=} failed.")
                 num = None
             new_row.update({column: num})
             # Log status.
             message = _compare_metrics(column=column, num=num)
-            logging.info(f"{message}")
-
-        national_platforms = [function() for function in national_platforms_functions]
-        new_row.update({"National Platforms": national_platforms})
+            logger.info(f"{message}")
     else:
         cpu_count = joblib.cpu_count()
         parallel = joblib.Parallel(n_jobs=cpu_count, return_as="generator")
 
         values = parallel(joblib.delayed(function)() for function in functions.values())
         columns = dict(zip(functions.keys(), values, strict=False))
         new_row.update(columns)
 
-        national_platforms = sum(
-            parallel(joblib.delayed(function)() for function in national_platforms_functions),
-        )
-        new_row.update({"National Platforms": national_platforms})
-
     new_row = pd.DataFrame.from_dict(data=new_row, orient="index").T
 
     # only update numbers if it's a new day
     if today not in df["date_UTC"].to_list():
         df = pd.concat(
             [df, new_row],
             ignore_index=True,
```

### Comparing `ioos_metrics-0.1.0.dev0/ioos_metrics/national_platforms.py` & `ioos_metrics-0.1.0a1/ioos_metrics/national_platforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,15 @@
 import re
 
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from fake_useragent import UserAgent
 
-logging.basicConfig(
-    filename="national_platforms.log",
-    encoding="utf-8",
-    level=logging.DEBUG,
-)
+logger = logging.getLogger(__name__)
 
 ua = UserAgent()
 _HEADERS = {
     "User-Agent": ua.random,
 }
 
 
@@ -49,15 +45,16 @@
 
     """
     xml = requests.get(
         "https://opendap.co-ops.nos.noaa.gov/stations/stationsXML.jsp",
         timeout=10,
     ).text
 
-    return sum(1 for _ in re.finditer(r"\b%s\b" % re.escape("station name"), xml))
+    station_name = re.escape("station name")
+    return sum(1 for _ in re.finditer(rf"\b{station_name}\b", xml))
 
 
 @functools.lru_cache(maxsize=128)
 def get_ndbc():
     """Fetches NDBC buoys.
 
     * Buoys: 106 (103 base-funded)
@@ -163,7 +160,12 @@
     """
     url = "https://cdip.ucsd.edu/themes/?d2=p1:m:mobile&regions=all&units=standard&zoom=auto&pub_set=public&tz=UTC&ll_fmt=dm&numcolorbands=10&palette=cdip_classic&high=6.096"
     table_list = pd.read_html(url, match="Stn")
 
     df = table_list[0]
 
     return df["Stn"].unique().size
+
+
+def national_platforms() -> int:
+    """Adds all the national platforms metrics."""
+    return get_cbibs() + get_cdip() + get_coops() + get_ndbc() + get_nerrs() + get_oap()
```

### Comparing `ioos_metrics-0.1.0.dev0/pyproject.toml` & `ioos_metrics-0.1.0a1/pyproject.toml`

 * *Files identical despite different names*

