# Comparing `tmp/idc_index-0.5.4.tar.gz` & `tmp/idc_index-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri May  3 21:49:01 2024, max compression
+gzip compressed data, last modified: Thu May  9 19:55:58 2024, max compression
```

## Comparing `idc_index-0.5.4.tar` & `idc_index-0.5.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      125 2024-05-03 21:49:01.000000 idc_index-0.5.4/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-05-03 21:49:01.000000 idc_index-0.5.4/.gitattributes
--rw-r--r--   0        0        0     2357 2024-05-03 21:49:01.000000 idc_index-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-05-03 21:49:01.000000 idc_index-0.5.4/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-05-03 21:49:01.000000 idc_index-0.5.4/noxfile.py
--rw-r--r--   0        0        0     2394 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1585 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      851 2024-05-03 21:49:01.000000 idc_index-0.5.4/docs/conf.py
--rw-r--r--   0        0        0      196 2024-05-03 21:49:01.000000 idc_index-0.5.4/docs/index.md
--rw-r--r--   0        0        0      263 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/_version.pyi
--rw-r--r--   0        0        0    51631 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/py.typed
--rw-r--r--   0        0        0        0 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0     8415 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      279 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/study_manifest_bogus.s5cmd
--rw-r--r--   0        0        0      419 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-05-03 21:49:01.000000 idc_index-0.5.4/.gitignore
--rw-r--r--   0        0        0     1077 2024-05-03 21:49:01.000000 idc_index-0.5.4/LICENSE
--rw-r--r--   0        0        0     4290 2024-05-03 21:49:01.000000 idc_index-0.5.4/README.md
--rw-r--r--   0        0        0     6130 2024-05-03 21:49:01.000000 idc_index-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     7551 2024-05-03 21:49:01.000000 idc_index-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-05-09 19:55:58.000000 idc_index-0.5.5/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-05-09 19:55:58.000000 idc_index-0.5.5/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-05-09 19:55:58.000000 idc_index-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-05-09 19:55:58.000000 idc_index-0.5.5/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-05-09 19:55:58.000000 idc_index-0.5.5/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1585 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-05-09 19:55:58.000000 idc_index-0.5.5/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      851 2024-05-09 19:55:58.000000 idc_index-0.5.5/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-05-09 19:55:58.000000 idc_index-0.5.5/docs/index.md
+-rw-r--r--   0        0        0      263 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/_version.pyi
+-rw-r--r--   0        0        0    61680 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-05-09 19:55:58.000000 idc_index-0.5.5/idc_index/py.typed
+-rw-r--r--   0        0        0        0 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/__init__.py
+-rw-r--r--   0        0        0    13853 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      279 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/study_manifest_bogus.s5cmd
+-rw-r--r--   0        0        0      419 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-05-09 19:55:58.000000 idc_index-0.5.5/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-05-09 19:55:58.000000 idc_index-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1077 2024-05-09 19:55:58.000000 idc_index-0.5.5/LICENSE
+-rw-r--r--   0        0        0     4290 2024-05-09 19:55:58.000000 idc_index-0.5.5/README.md
+-rw-r--r--   0        0        0     6130 2024-05-09 19:55:58.000000 idc_index-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     7551 2024-05-09 19:55:58.000000 idc_index-0.5.5/PKG-INFO
```

### Comparing `idc_index-0.5.4/.pre-commit-config.yaml` & `idc_index-0.5.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/noxfile.py` & `idc_index-0.5.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/.github/CONTRIBUTING.md` & `idc_index-0.5.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/.github/matchers/pylint.json` & `idc_index-0.5.5/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/.github/workflows/cd.yml` & `idc_index-0.5.5/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/.github/workflows/ci.yml` & `idc_index-0.5.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/docs/conf.py` & `idc_index-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/idc_index/index.py` & `idc_index-0.5.5/idc_index/index.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 logging.basicConfig(format="%(asctime)s - %(message)s", level=logging.DEBUG)
 
 aws_endpoint_url = "https://s3.amazonaws.com"
 gcp_endpoint_url = "https://storage.googleapis.com"
 
 
 class IDCClient:
+    DOWNLOAD_HIERARCHY_DEFAULT = (
+        "%collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID"
+    )
+
     def __init__(self):
         file_path = idc_index_data.IDC_INDEX_PARQUET_FILEPATH
 
         # Read index file
         logger.debug(f"Reading index file v{idc_index_data.__version__}")
         self.index = pd.read_parquet(file_path)
         # self.index = self.index.astype(str).replace("nan", "")
@@ -147,28 +151,27 @@
             raise ValueError("outputFormat must be either 'dict', 'df', or 'list")
 
         patient_df = self._filter_by_collection_id(self.index, collection_id)
 
         if outputFormat == "list":
             response = patient_df["PatientID"].unique().tolist()
         else:
-            patient_df = patient_df.rename(columns={"collection_id": "Collection"})
-            patient_df = patient_df[["PatientID", "PatientSex", "PatientAge"]]
-            patient_df = (
-                patient_df.groupby("PatientID")
-                .agg(
-                    {
-                        "PatientSex": lambda x: ",".join(x[x != ""].unique()),
-                        "PatientAge": lambda x: ",".join(x[x != ""].unique()),
-                    }
-                )
-                .reset_index()
-            )
-
-            patient_df = patient_df.drop_duplicates().sort_values(by="PatientID")
+            sql = """
+                SELECT
+                    PatientID,
+                    STRING_AGG(DISTINCT PatientSex) as PatientSex,
+                    STRING_AGG(DISTINCT PatientAge) as PatientAge
+                FROM
+                    patient_df
+                GROUP BY
+                    PatientID
+                ORDER BY
+                    PatientID
+                """
+            patient_df = duckdb.sql(sql).df()
             # Convert DataFrame to a list of dictionaries for the API-like response
             if outputFormat == "dict":
                 response = patient_df.to_dict(orient="records")
             else:
                 response = patient_df
 
         logger.debug("Get patient response: %s", str(response))
@@ -196,53 +199,28 @@
             raise ValueError("outputFormat must be either 'dict' or 'df' or 'list'")
 
         studies_df = self._filter_by_patient_id(self.index, patientId)
 
         if outputFormat == "list":
             response = studies_df["StudyInstanceUID"].unique().tolist()
         else:
-            studies_df["patient_study_size_MB"] = studies_df.groupby(
-                ["PatientID", "StudyInstanceUID"]
-            )["series_size_MB"].transform("sum")
-            studies_df["patient_study_series_count"] = studies_df.groupby(
-                ["PatientID", "StudyInstanceUID"]
-            )["SeriesInstanceUID"].transform("count")
-            studies_df["patient_study_instance_count"] = studies_df.groupby(
-                ["PatientID", "StudyInstanceUID"]
-            )["instanceCount"].transform("count")
-
-            studies_df = studies_df.rename(
-                columns={
-                    "collection_id": "Collection",
-                    "patient_study_series_count": "SeriesCount",
-                }
-            )
-
-            # patient_study_df = patient_study_df[['PatientID', 'PatientSex', 'Collection', 'PatientAge', 'StudyInstanceUID', 'StudyDate', 'StudyDescription', 'patient_study_size_MB', 'SeriesCount', 'patient_study_instance_count']]
-            studies_df = studies_df[
-                ["StudyInstanceUID", "StudyDate", "StudyDescription", "SeriesCount"]
-            ]
-            # Group by 'StudyInstanceUID'
-            studies_df = (
-                studies_df.groupby("StudyInstanceUID")
-                .agg(
-                    {
-                        "StudyDate": lambda x: ",".join(x[x != ""].unique()),
-                        "StudyDescription": lambda x: ",".join(x[x != ""].unique()),
-                        "SeriesCount": lambda x: int(x[x != ""].iloc[0])
-                        if len(x[x != ""]) > 0
-                        else 0,
-                    }
-                )
-                .reset_index()
-            )
-
-            studies_df = studies_df.drop_duplicates().sort_values(
-                by=["StudyDate", "StudyDescription", "SeriesCount"]
-            )
+            sql = """
+                SELECT
+                    StudyInstanceUID,
+                    STRING_AGG(DISTINCT StudyDate) as StudyDate,
+                    STRING_AGG(DISTINCT StudyDescription) as StudyDescription,
+                    COUNT(SeriesInstanceUID) as SeriesCount
+                FROM
+                    studies_df
+                GROUP BY
+                    StudyInstanceUID
+                ORDER BY
+                    2,3,4
+                """
+            studies_df = duckdb.query(sql).df()
 
             if outputFormat == "dict":
                 response = studies_df.to_dict(orient="records")
             else:
                 response = studies_df
 
         logger.debug("Get patient study response: %s", str(response))
@@ -470,26 +448,28 @@
         return viewer_url
 
     def _validate_update_manifest_and_get_download_size(
         self,
         manifestFile,
         downloadDir,
         validate_manifest,
-        show_progress_bar,
-        use_s5cmd_sync_dry_run,
+        use_s5cmd_sync,
+        dirTemplate,
     ) -> tuple[float, str, Path]:
         """
         Validates the manifest file by checking the URLs in the manifest
 
         Args:
             manifestFile (str): The path to the manifest file.
             downloadDir (str): The path to the download directory.
             validate_manifest (bool, optional): If True, validates the manifest for any errors. Defaults to True.
             show_progress_bar (bool, optional): If True, tracks the progress of download
-            use_s5cmd_sync_dry_run (bool, optional): If True, improves the accuracy of progress bar in unusual circumstances
+            use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            dirTemplate (str): A template string for the directory path. Must start with %. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT. It can contain attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) wrapped in '%'. Special characters can be used as connectors: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). Can be disabled by None.
+
         Returns:
             total_size (float): The total size of all series in the manifest file.
             endpoint_to_use (str): The endpoint URL to use (either AWS or GCP).
             temp_manifest_file(Path): Path to the temporary manifest file for downstream steps
         Raises:
             ValueError: If the manifest file does not exist, if any URL in the manifest file is invalid, or if any URL is inaccessible in both AWS and GCP.
             Exception: If the manifest contains URLs from both AWS and GCP.
@@ -608,79 +588,163 @@
             # in the future, see https://github.com/ImagingDataCommons/idc-index/pull/56#discussion_r1582157048
             endpoint_to_use = gcp_endpoint_url
 
         # Calculate total size
         total_size = merged_df["series_size_MB"].sum()
         total_size = round(total_size, 2)
 
+        if dirTemplate is not None:
+            hierarchy = self._generate_sql_concat_for_building_directory(
+                dirTemplate=dirTemplate, downloadDir=downloadDir
+            )
+            sql = f"""
+                WITH temp as
+                    (
+                        SELECT
+                            seriesInstanceUID,
+                            s3_url
+                        FROM
+                            merged_df
+                    )
+                SELECT
+                    s3_url,
+                    {hierarchy} as path
+                FROM
+                    temp
+                JOIN
+                    index using (seriesInstanceUID)
+                """
+            logger.debug(f"About to run this query:\n{sql}")
+            merged_df = self.sql_query(sql)
         # Write a temporary manifest file
         with tempfile.NamedTemporaryFile(mode="w", delete=False) as temp_manifest_file:
-            if (
-                show_progress_bar
-                and use_s5cmd_sync_dry_run
-                and len(os.listdir(downloadDir)) != 0
-            ):
+            if use_s5cmd_sync and len(os.listdir(downloadDir)) != 0:
+                if dirTemplate is not None:
+                    merged_df["s5cmd_cmd"] = (
+                        "sync " + merged_df["s3_url"] + " " + merged_df["path"]
+                    )
+                else:
+                    merged_df["s5cmd_cmd"] = (
+                        "sync " + merged_df["s3_url"] + " " + downloadDir
+                    )
+            elif dirTemplate is not None:
                 merged_df["s5cmd_cmd"] = (
-                    "sync " + merged_df["s3_url"] + " " + downloadDir
+                    "cp " + merged_df["s3_url"] + " " + merged_df["path"]
                 )
             else:
                 merged_df["s5cmd_cmd"] = "cp " + merged_df["s3_url"] + " " + downloadDir
+
             merged_df["s5cmd_cmd"].to_csv(temp_manifest_file, header=False, index=False)
             logger.info("Parsing the manifest is finished. Download will begin soon")
-        return total_size, endpoint_to_use, Path(temp_manifest_file.name)
+
+        if dirTemplate is not None:
+            list_of_directories = merged_df.path.to_list()
+        else:
+            list_of_directories = [downloadDir]
+        return (
+            total_size,
+            endpoint_to_use,
+            Path(temp_manifest_file.name),
+            list_of_directories,
+        )
+
+    @staticmethod
+    def _generate_sql_concat_for_building_directory(dirTemplate, downloadDir):
+        # for now, we limit the allowed columns to this list to make sure that all
+        # values are guaranteed to be non-empty and to not contain any special characters
+        # in the future, we should consider including more attributes
+        # also, if we allow any column, we should decide what we would do if the value is NULL
+        valid_attributes = [
+            "PatientID",
+            "collection_id",
+            "Modality",
+            "StudyInstanceUID",
+            "SeriesInstanceUID",
+        ]
+        valid_separators = ["_", "-", "/"]
+
+        updated_template = dirTemplate
+
+        # validate input template by removing all valid attributes and separators
+        for attr in valid_attributes:
+            updated_template = updated_template.replace("%" + attr, "")
+        for sep in valid_separators:
+            updated_template = updated_template.replace(sep, "")
+
+        if updated_template != "":
+            logger.error("Invalid download hierarchy template:" + updated_template)
+            logger.error(
+                "Make sure your template uses only valid attributes and separators"
+            )
+            logger.error("Valid attributes: " + str(valid_attributes))
+            logger.error("Valid separators: " + str(valid_separators))
+            raise ValueError
+
+        concat_command = dirTemplate
+        for attr in valid_attributes:
+            concat_command = concat_command.replace("%" + attr, f"', {attr},'")
+
+        # CONCAT command may contain empty strings, and they are not harmless -
+        # duckdb does not like them!
+        # NB: double-quotes are not allowed by duckdb!
+        concat_command = f"CONCAT('{downloadDir}/','" + concat_command + "')"
+        concat_command = concat_command.replace(",''", "")
+        concat_command = concat_command.replace("'',", "")
+        concat_command = concat_command.replace(",'',", "")
+        return concat_command
 
     @staticmethod
     def _track_download_progress(
         size_MB: int,
         downloadDir: str,
         process: subprocess.Popen,
         show_progress_bar: bool = True,
+        list_of_directories=None,
     ):
         logger.info("Inputs received for tracking download:")
         logger.info(f"size_MB: {size_MB}")
         logger.info(f"downloadDir: {downloadDir}")
         logger.info(f"show_progress_bar: {show_progress_bar}")
 
         runtime_errors = []
 
         if show_progress_bar:
             total_size_bytes = size_MB * 10**6  # Convert MB to bytes
-
+            # temporary place holder. Accurate size is calculated in the next step
+            initial_size_bytes = 0
             # Calculate the initial size of the directory
-            initial_size_bytes = sum(
-                f.stat().st_size for f in Path(downloadDir).iterdir() if f.is_file()
-            )
+            for directory in list_of_directories:
+                path = Path(directory)
+                if path.exists() and path.is_dir():
+                    initial_size_bytes += sum(
+                        f.stat().st_size for f in path.iterdir() if f.is_file()
+                    )
 
             logger.info("Initial size of the directory: %s bytes", initial_size_bytes)
             logger.info(
                 "Approx. Size of the files need to be downloaded: %s bytes",
                 total_size_bytes,
             )
 
             pbar = tqdm(
                 total=total_size_bytes,
                 unit="B",
                 unit_scale=True,
                 desc="Downloading data",
             )
 
-            # TODO: this is suboptimal, since we are checking every file, while we could just
-            # check the size of the files in the folders corresponding to the series being downloaded;
-            # this approach will also be problematic if user adds or deletes unrelated files from
-            # the download directory; we will address this in the future by preserving the folder structure
-            # at the destination, see https://github.com/ImagingDataCommons/idc-index/pull/56#discussion_r1582854525
             while True:
-                downloaded_bytes = (
-                    sum(
-                        f.stat().st_size
-                        for f in Path(downloadDir).iterdir()
-                        if f.is_file()
-                    )
-                    - initial_size_bytes
-                )
+                downloaded_bytes = 0
+                for directory in list_of_directories:
+                    path = Path(directory)
+                    if path.exists() and path.is_dir():
+                        downloaded_bytes += sum(
+                            f.stat().st_size for f in path.iterdir() if f.is_file()
+                        )
+                downloaded_bytes -= initial_size_bytes
                 pbar.n = min(
                     downloaded_bytes, total_size_bytes
                 )  # Prevent the progress bar from exceeding 100%
                 pbar.refresh()
 
                 if process.poll() is not None:
                     break
@@ -692,22 +756,23 @@
             pbar.close()
 
         else:
             while process.poll() is None:
                 time.sleep(0.5)
 
     def _parse_s5cmd_sync_output_and_generate_synced_manifest(
-        self, stdout, downloadDir
+        self, stdout, downloadDir, dirTemplate
     ) -> Path:
         """
         Parse the output of s5cmd sync --dry-run to extract distinct folders and generate a synced manifest.
 
         Args:
             output (str): The output of s5cmd sync --dry-run command.
             downloadDir (str): The directory to download the files to.
+            dirTemplate (str): Download directory hierarchy template.
 
         Returns:
             Path: The path to the generated synced manifest file.
             float: Download size in MB
         """
         logger.info("Parsing the s5cmd sync dry run output...")
 
@@ -747,30 +812,62 @@
         # ruff: noqa: end
         merged_df = duckdb.query(sql).df()
         sync_size = merged_df["series_size_MB"].sum()
         sync_size_rounded = round(sync_size, 2)
 
         logger.info(f"sync_size_rounded: {sync_size_rounded}")
 
+        if dirTemplate is not None:
+            hierarchy = self._generate_sql_concat_for_building_directory(
+                dirTemplate=dirTemplate, downloadDir=downloadDir
+            )
+            sql = f"""
+                WITH temp as
+                    (
+                        SELECT
+                            seriesInstanceUID
+                        FROM
+                            merged_df
+                    )
+                SELECT
+                    series_aws_url,
+                    {hierarchy} as path
+                FROM
+                    temp
+                JOIN
+                    index using (seriesInstanceUID)
+                """
+            synced_df = self.sql_query(sql)
         # Write a temporary manifest file
         with tempfile.NamedTemporaryFile(mode="w", delete=False) as synced_manifest:
-            merged_df["s5cmd_cmd"] = "sync " + merged_df["s3_url"] + " " + downloadDir
-            merged_df["s5cmd_cmd"].to_csv(synced_manifest, header=False, index=False)
+            if dirTemplate is not None:
+                synced_df["s5cmd_cmd"] = (
+                    "sync " + synced_df["s3_url"] + " " + synced_df["path"]
+                )
+                list_of_directories = synced_df.path.to_list()
+            else:
+                synced_df["s5cmd_cmd"] = (
+                    "sync " + synced_df["s3_url"] + " " + downloadDir
+                )
+                list_of_directories = [downloadDir]
+            synced_df["s5cmd_cmd"].to_csv(synced_manifest, header=False, index=False)
             logger.info("Parsing the s5cmd sync dry run output finished")
-        return Path(synced_manifest.name), sync_size_rounded
+        return Path(synced_manifest.name), sync_size_rounded, list_of_directories
 
     def _s5cmd_run(
         self,
         endpoint_to_use,
         manifest_file,
         total_size,
         downloadDir,
         quiet,
         show_progress_bar,
         use_s5cmd_sync,
+        dirTemplate,
+        list_of_directories,
     ):
         """
         Executes the s5cmd command to sync files from a given endpoint to a local directory.
 
         This function first performs a dry run of the s5cmd command to check which files need to be downloaded.
         If there are files to be downloaded, it generates a new manifest file with the files to be synced and
         runs the s5cmd command again to download the files. The progress of the download is tracked and printed
@@ -780,14 +877,15 @@
             endpoint_to_use (str): The endpoint URL to download the files from.
             manifest_file (str): The path to the manifest file listing the files to be downloaded.
             total_size (float): The total size of the files to be downloaded in MB.
             downloadDir (str): The local directory where the files will be downloaded.
             quiet (bool, optional): If True, suppresses the stdout and stderr of the s5cmd command.
             show_progress_bar (bool, optional): If True, tracks the progress of download
             use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            dirTemplate (str): Download directory hierarchy template.
 
         Raises:
             subprocess.CalledProcessError: If the s5cmd command fails.
 
         Returns:
             None
         """
@@ -795,14 +893,15 @@
         logger.debug(f"endpoint_to_use: {endpoint_to_use}")
         logger.debug(f"manifest_file: {manifest_file}")
         logger.debug(f"total_size: {total_size}")
         logger.debug(f"downloadDir: {downloadDir}")
         logger.debug(f"quiet: {quiet}")
         logger.debug(f"show_progress_bar: {show_progress_bar}")
         logger.debug(f"use_s5cmd_sync: {use_s5cmd_sync}")
+        logger.debug(f"dirTemplate: {dirTemplate}")
 
         if quiet:
             stdout = subprocess.DEVNULL
             stderr = subprocess.DEVNULL
         else:
             stdout = None
             stderr = None
@@ -833,16 +932,19 @@
 stoud from s5cmd sync dry run is not empty. Parsing the output to
 evaluate what to download and corresponding size with only series level precision
 """
                 )
                 (
                     synced_manifest,
                     sync_size,
+                    list_of_directories,
                 ) = self._parse_s5cmd_sync_output_and_generate_synced_manifest(
-                    stdout=process.stdout, downloadDir=downloadDir
+                    stdout=process.stdout,
+                    downloadDir=downloadDir,
+                    dirTemplate=dirTemplate,
                 )
                 logger.info(f"sync_size (MB): {sync_size}")
 
                 cmd = [
                     self.s5cmdPath,
                     "--no-sign-request",
                     "--endpoint-url",
@@ -898,15 +1000,19 @@
             with subprocess.Popen(
                 cmd,
                 stdout=stdout,
                 stderr=stderr_log_file,
                 universal_newlines=True,
             ) as process:
                 self._track_download_progress(
-                    total_size, downloadDir, process, show_progress_bar
+                    total_size,
+                    downloadDir,
+                    process,
+                    show_progress_bar,
+                    list_of_directories,
                 )
 
                 stderr_log_file.close()
 
                 runtime_errors = []
                 with open(stderr_log_file.name) as stderr_log_file:
                     for line in stderr_log_file.readlines():
@@ -946,93 +1052,96 @@
         self,
         manifestFile: str,
         downloadDir: str,
         quiet: bool = True,
         validate_manifest: bool = True,
         show_progress_bar: bool = True,
         use_s5cmd_sync: bool = False,
+        dirTemplate=DOWNLOAD_HIERARCHY_DEFAULT,
     ) -> None:
         """
         Download the manifest file. In a series of steps, the manifest file
         is first validated to ensure every line contains a valid urls. It then
         gets the total size to be downloaded and runs download process on one
         process and download progress on another process.
 
         Args:
             manifestFile (str): The path to the manifest file.
             downloadDir (str): The directory to download the files to.
             quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
             validate_manifest (bool, optional): If True, validates the manifest for any errors. Defaults to True.
             show_progress_bar (bool, optional): If True, tracks the progress of download
             use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Raises:
             ValueError: If the download directory does not exist.
         """
 
         downloadDir = os.path.abspath(downloadDir).replace("\\", "/")
         if not os.path.exists(downloadDir):
             raise ValueError("Download directory does not exist.")
 
         # validate the manifest
         (
             total_size,
             endpoint_to_use,
             temp_manifest_file,
+            list_of_directories,
         ) = self._validate_update_manifest_and_get_download_size(
-            manifestFile,
-            downloadDir,
-            validate_manifest,
-            show_progress_bar,
-            use_s5cmd_sync,
+            manifestFile=manifestFile,
+            downloadDir=downloadDir,
+            validate_manifest=validate_manifest,
+            use_s5cmd_sync=use_s5cmd_sync,
+            dirTemplate=dirTemplate,
         )
 
         total_size_rounded = round(total_size, 2)
         logger.info("Total size: " + self._format_size(total_size_rounded))
 
         self._s5cmd_run(
             endpoint_to_use=endpoint_to_use,
             manifest_file=temp_manifest_file,
             total_size=total_size_rounded,
             downloadDir=downloadDir,
             quiet=quiet,
             show_progress_bar=show_progress_bar,
             use_s5cmd_sync=use_s5cmd_sync,
+            dirTemplate=dirTemplate,
+            list_of_directories=list_of_directories,
         )
 
     def download_from_selection(
         self,
         downloadDir,
         dry_run=False,
         collection_id=None,
         patientId=None,
         studyInstanceUID=None,
         seriesInstanceUID=None,
         quiet=True,
         show_progress_bar=True,
         use_s5cmd_sync=False,
+        dirTemplate=DOWNLOAD_HIERARCHY_DEFAULT,
     ):
         """Download the files corresponding to the selection. The filtering will be applied in sequence (but does it matter?) by first selecting the collection(s), followed by
         patient(s), study(studies) and series. If no filtering is applied, all the files will be downloaded.
 
         Args:
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
             collection_id: string or list of strings containing the values of collection_id to filter by
             patientId: string or list of strings containing the values of PatientID to filter by
             studyInstanceUID: string or list of strings containing the values of DICOM StudyInstanceUID to filter by
             seriesInstanceUID: string or list of strings containing the values of DICOM SeriesInstanceUID to filter by
-            quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
+            quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True
             show_progress_bar (bool, optional): If True, tracks the progress of download
             use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
-        Returns:
-
-        Raises:
-            TypeError: If any of the parameters are not of the expected type
         """
 
         downloadDir = os.path.abspath(downloadDir).replace("\\", "/")
         if not os.path.exists(downloadDir):
             raise ValueError("Download directory does not exist.")
 
         if collection_id is not None:
@@ -1080,177 +1189,229 @@
 
         if dry_run:
             logger.info(
                 "Dry run. Not downloading files. Rerun with dry_run=False to download the files."
             )
         else:
             logger.info("Total size: " + self._format_size(total_size))
+
+        if dirTemplate is not None:
+            hierarchy = self._generate_sql_concat_for_building_directory(
+                downloadDir=downloadDir,
+                dirTemplate=dirTemplate,
+            )
+            sql = f"""
+                WITH temp as
+                    (
+                        SELECT
+                            seriesInstanceUID
+                        FROM
+                            result_df
+                    )
+                SELECT
+                    series_aws_url,
+                    {hierarchy} as path
+                FROM
+                    temp
+                JOIN
+                    index using (seriesInstanceUID)
+                """
+            result_df = self.sql_query(sql)
             # Download the files
             # make temporary file to store the list of files to download
-            with tempfile.NamedTemporaryFile(mode="w", delete=False) as manifest_file:
-                if use_s5cmd_sync and len(os.listdir(downloadDir)) != 0:
+        with tempfile.NamedTemporaryFile(mode="w", delete=False) as manifest_file:
+            if use_s5cmd_sync and len(os.listdir(downloadDir)) != 0:
+                if dirTemplate is not None:
                     result_df["s5cmd_cmd"] = (
-                        "sync " + result_df["series_aws_url"] + " " + downloadDir
+                        "sync " + result_df["series_aws_url"] + " " + result_df["path"]
                     )
                 else:
                     result_df["s5cmd_cmd"] = (
-                        "cp " + result_df["series_aws_url"] + " " + downloadDir
+                        "sync " + result_df["series_aws_url"] + " " + downloadDir
                     )
-                result_df["s5cmd_cmd"].to_csv(manifest_file, header=False, index=False)
-            logger.debug(
-                "Temporary download manifest is generated and is passed to self._s5cmd_run"
-            )
-            self._s5cmd_run(
-                endpoint_to_use=aws_endpoint_url,
-                manifest_file=Path(manifest_file.name),
-                total_size=total_size,
-                downloadDir=downloadDir,
-                quiet=quiet,
-                show_progress_bar=show_progress_bar,
-                use_s5cmd_sync=use_s5cmd_sync,
-            )
+            elif dirTemplate is not None:
+                result_df["s5cmd_cmd"] = (
+                    "cp " + result_df["series_aws_url"] + " " + result_df["path"]
+                )
+            else:
+                result_df["s5cmd_cmd"] = (
+                    "cp " + result_df["series_aws_url"] + " " + downloadDir
+                )
+            result_df["s5cmd_cmd"].to_csv(manifest_file, header=False, index=False)
+            if dirTemplate is not None:
+                list_of_directories = result_df.path.to_list()
+            else:
+                list_of_directories = [downloadDir]
+        logger.info(
+            """
+Temporary download manifest is generated and is passed to self._s5cmd_run
+"""
+        )
+        self._s5cmd_run(
+            endpoint_to_use=aws_endpoint_url,
+            manifest_file=Path(manifest_file.name),
+            total_size=total_size,
+            downloadDir=downloadDir,
+            quiet=quiet,
+            show_progress_bar=show_progress_bar,
+            use_s5cmd_sync=use_s5cmd_sync,
+            dirTemplate=dirTemplate,
+            list_of_directories=list_of_directories,
+        )
 
     def download_dicom_series(
         self,
         seriesInstanceUID,
         downloadDir,
         dry_run=False,
         quiet=True,
         show_progress_bar=True,
         use_s5cmd_sync=False,
+        dirTemplate=DOWNLOAD_HIERARCHY_DEFAULT,
     ) -> None:
         """
         Download the files corresponding to the seriesInstanceUID to the specified directory.
 
         Args:
             seriesInstanceUID: string or list of strings containing the values of DICOM SeriesInstanceUID to filter by
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
             quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
             show_progress_bar (bool, optional): If True, tracks the progress of download
             use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Returns: None
 
         Raises:
             TypeError: If seriesInstanceUID(s) passed is(are) not a string or list
 
         """
         self.download_from_selection(
             downloadDir,
             seriesInstanceUID=seriesInstanceUID,
             dry_run=dry_run,
             quiet=quiet,
             show_progress_bar=show_progress_bar,
             use_s5cmd_sync=use_s5cmd_sync,
+            dirTemplate=dirTemplate,
         )
 
     def download_dicom_studies(
         self,
         studyInstanceUID,
         downloadDir,
         dry_run=False,
         quiet=True,
         show_progress_bar=True,
         use_s5cmd_sync=False,
+        dirTemplate=DOWNLOAD_HIERARCHY_DEFAULT,
     ) -> None:
         """
         Download the files corresponding to the studyInstanceUID to the specified directory.
 
         Args:
             studyInstanceUID: string or list of strings containing the values of DICOM studyInstanceUID to filter by
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
             quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
             show_progress_bar (bool, optional): If True, tracks the progress of download
             use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Returns: None
 
         Raises:
             TypeError: If seriesInstanceUID(s) passed is(are) not a string or list
 
         """
         self.download_from_selection(
             downloadDir,
             studyInstanceUID=studyInstanceUID,
             dry_run=dry_run,
             quiet=quiet,
             show_progress_bar=show_progress_bar,
             use_s5cmd_sync=use_s5cmd_sync,
+            dirTemplate=dirTemplate,
         )
 
     def download_dicom_patients(
         self,
         patientId,
         downloadDir,
         dry_run=False,
         quiet=True,
         show_progress_bar=True,
         use_s5cmd_sync=False,
+        dirTemplate=DOWNLOAD_HIERARCHY_DEFAULT,
     ) -> None:
         """
         Download the files corresponding to the studyInstanceUID to the specified directory.
 
         Args:
             patientId: string or list of strings containing the values of DICOM patientId to filter by
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
             quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
             show_progress_bar (bool, optional): If True, tracks the progress of download
             use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Returns: None
 
         Raises:
             TypeError: If patientId(s) passed is(are) not a string or list
 
         """
         self.download_from_selection(
             downloadDir,
             patientId=patientId,
             dry_run=dry_run,
             quiet=quiet,
             show_progress_bar=show_progress_bar,
             use_s5cmd_sync=use_s5cmd_sync,
+            dirTemplate=dirTemplate,
         )
 
     def download_collection(
         self,
         collection_id,
         downloadDir,
         dry_run=False,
         quiet=True,
         show_progress_bar=True,
         use_s5cmd_sync=False,
+        dirTemplate=DOWNLOAD_HIERARCHY_DEFAULT,
     ) -> None:
         """
         Download the files corresponding to the studyInstanceUID to the specified directory.
 
         Args:
             collection_id: string or list of strings containing the values of DICOM patientId to filter by
             downloadDir: string containing the path to the directory to download the files to
             dry_run: calculates the size of the cohort but download does not start
             quiet (bool, optional): If True, suppresses the output of the subprocess. Defaults to True.
             show_progress_bar (bool, optional): If True, tracks the progress of download
             use_s5cmd_sync (bool, optional): If True, will use s5cmd sync operation instead of cp when downloadDirectory is not empty; this can significantly improve the download speed if the content is partially downloaded
+            dirTemplate (str): Download directory hierarchy template. This variable defines the folder hierarchy for the organizing the downloaded files in downloadDirectory. Defaults to index.DOWNLOAD_HIERARCHY_DEFAULT set to %collection_id/%PatientID/%StudyInstanceUID/%Modality_%SeriesInstanceUID. The template string can be built using a combination of selected metadata attributes (PatientID, collection_id, Modality, StudyInstanceUID, SeriesInstanceUID) that must be prefixed by '%'. The following special characters can be used as separators: '-' (hyphen), '/' (slash for subdirectories), '_' (underscore). When set to None all files will be downloaded to the download directory with no subdirectories.
 
         Returns: None
 
         Raises:
             TypeError: If collection_id(s) passed is(are) not a string or list
 
         """
         self.download_from_selection(
             downloadDir,
             collection_id=collection_id,
             dry_run=dry_run,
             quiet=quiet,
             show_progress_bar=show_progress_bar,
             use_s5cmd_sync=use_s5cmd_sync,
+            dirTemplate=dirTemplate,
         )
 
     def sql_query(self, sql_query):
         """Execute SQL query against the table in the index using duckdb.
 
         Args:
             sql_query: string containing the SQL query to execute. The table name to use in the FROM clause is 'index' (without quotes).
```

### Comparing `idc_index-0.5.4/.gitignore` & `idc_index-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/LICENSE` & `idc_index-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/README.md` & `idc_index-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/pyproject.toml` & `idc_index-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.4/PKG-INFO` & `idc_index-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.5.4
+Version: 0.5.5
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
```

