# Comparing `tmp/dvuploader-0.2.2.tar.gz` & `tmp/dvuploader-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvuploader-0.2.2.tar", max compression
+gzip compressed data, was "dvuploader-0.2.3.tar", max compression
```

## Comparing `dvuploader-0.2.2.tar` & `dvuploader-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2024-04-04 09:46:19.384892 dvuploader-0.2.2/LICENSE
--rw-r--r--   0        0        0     4125 2024-04-04 09:46:19.384892 dvuploader-0.2.2/README.md
--rw-r--r--   0        0        0      134 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/__init__.py
--rw-r--r--   0        0        0     2436 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/checksum.py
--rw-r--r--   0        0        0     4719 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/cli.py
--rw-r--r--   0        0        0    17166 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/directupload.py
--rw-r--r--   0        0        0    10260 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/dvuploader.py
--rw-r--r--   0        0        0     3004 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/file.py
--rw-r--r--   0        0        0     6886 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/nativeupload.py
--rw-r--r--   0        0        0     3018 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/packaging.py
--rw-r--r--   0        0        0     4367 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/utils.py
--rw-r--r--   0        0        0      767 2024-04-04 09:46:19.384892 dvuploader-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5041 1970-01-01 00:00:00.000000 dvuploader-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-09 17:32:29.878905 dvuploader-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4130 2024-05-09 17:32:29.878905 dvuploader-0.2.3/README.md
+-rw-r--r--   0        0        0      134 2024-05-09 17:32:29.878905 dvuploader-0.2.3/dvuploader/__init__.py
+-rw-r--r--   0        0        0     2588 2024-05-09 17:32:29.878905 dvuploader-0.2.3/dvuploader/checksum.py
+-rw-r--r--   0        0        0     4719 2024-05-09 17:32:29.878905 dvuploader-0.2.3/dvuploader/cli.py
+-rw-r--r--   0        0        0    17362 2024-05-09 17:32:29.878905 dvuploader-0.2.3/dvuploader/directupload.py
+-rw-r--r--   0        0        0    10861 2024-05-09 17:32:29.878905 dvuploader-0.2.3/dvuploader/dvuploader.py
+-rw-r--r--   0        0        0     3679 2024-05-09 17:32:29.878905 dvuploader-0.2.3/dvuploader/file.py
+-rw-r--r--   0        0        0    10255 2024-05-09 17:32:29.878905 dvuploader-0.2.3/dvuploader/nativeupload.py
+-rw-r--r--   0        0        0     2976 2024-05-09 17:32:29.878905 dvuploader-0.2.3/dvuploader/packaging.py
+-rw-r--r--   0        0        0     4377 2024-05-09 17:32:29.878905 dvuploader-0.2.3/dvuploader/utils.py
+-rw-r--r--   0        0        0      767 2024-05-09 17:32:29.882905 dvuploader-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5046 1970-01-01 00:00:00.000000 dvuploader-0.2.3/PKG-INFO
```

### Comparing `dvuploader-0.2.2/LICENSE` & `dvuploader-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvuploader-0.2.2/README.md` & `dvuploader-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 ```python
 import dvuploader as dv
 
 
 # Add file individually
 files = [
     dv.File(filepath="./small.txt"),
-    dv.File(directoryLabel="some/dir", filepath="./medium.txt"),
-    dv.File(directoryLabel="some/dir", filepath="./big.txt"),
+    dv.File(directory_label="some/dir", filepath="./medium.txt"),
+    dv.File(directory_label="some/dir", filepath="./big.txt"),
     *dv.add_directory("./data"), # Add an entire directory
 ]
 
 DV_URL = "https://demo.dataverse.org/"
 API_TOKEN = "XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
 PID = "doi:10.70122/XXX/XXXXX"
 
@@ -84,15 +84,15 @@
 Alternatively, you can also supply a `config` file that contains all necessary informations for the uploader. The `config` file is a JSON/YAML file that contains the following keys:
 
 * `persistent_id`: Persistent identifier of the dataset to upload to.
 * `dataverse_url`: URL of the Dataverse instance.
 * `api_token`: API token of the Dataverse instance.
 * `files`: List of files to upload. Each file is a dictionary with the following keys:
   * `filepath`: Path to the file to upload.
-  * `directoryLabel`: Optional directory label to upload the file to.
+  * `directory_label`: Optional directory label to upload the file to.
   * `description`: Optional description of the file.
   * `mimetype`: Mimetype of the file.
   * `categories`: Optional list of categories to assign to the file.
   * `restrict`: Boolean to indicate that this is a restricted file. Defaults to False.
 
 In the following example, we upload three files to a Dataverse instance. The first file is uploaded to the root directory of the dataset, while the other two files are uploaded to the directory `some/dir`.
 
@@ -100,17 +100,17 @@
 # config.yml
 persistent_id: doi:10.70122/XXX/XXXXX
 dataverse_url: https://demo.dataverse.org/
 api_token: XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
 files:
     - filepath: ./small.txt
     - filepath: ./medium.txt
-      directoryLabel: some/dir
+      directory_label: some/dir
     - filepath: ./big.txt
-      directoryLabel: some/dir
+      directory_label: some/dir
 ```
 
 The `config` file can then be used as follows:
 
 ```bash
 dvuploader --config-path config.yml
 ```
```

#### html2text {}

```diff
@@ -12,17 +12,17 @@
 dvuploader ``` or by source ```bash git clone https://github.com/gdcc/python-
 dvuploader.git cd python-dvuploader python3 -m pip install . ``` ## Quickstart
 ### Programmatic usage In order to perform a direct upload, you need to have a
 Dataverse instance running and a cloud storage provider. The following example
 shows how to upload files to a Dataverse instance. Simply provide the files of
 interest and utilize the `upload` method of a `DVUploader` instance. ```python
 import dvuploader as dv # Add file individually files = [ dv.File(filepath="./
-small.txt"), dv.File(directoryLabel="some/dir", filepath="./medium.txt"),
-dv.File(directoryLabel="some/dir", filepath="./big.txt"), *dv.add_directory("./
-data"), # Add an entire directory ] DV_URL = "https://demo.dataverse.org/
+small.txt"), dv.File(directory_label="some/dir", filepath="./medium.txt"),
+dv.File(directory_label="some/dir", filepath="./big.txt"), *dv.add_directory
+("./data"), # Add an entire directory ] DV_URL = "https://demo.dataverse.org/
 " API_TOKEN = "XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX" PID = "doi:10.70122/XXX/
 XXXXX" dvuploader = dv.DVUploader(files=files) dvuploader.upload
 ( api_token=API_TOKEN, dataverse_url=DV_URL, persistent_id=PID,
 n_parallel_uploads=2, # Whatever your instance can handle ) ``` ### Command
 Line Interface DVUploader ships with a CLI ready to use outside scripts. In
 order to upload files to a Dataverse instance, simply provide the files of
 interest, persistent identifier and credentials. #### Using arguments ```bash
@@ -31,19 +31,19 @@
 demo.dataverse.org/ \ ``` #### Using a config file Alternatively, you can also
 supply a `config` file that contains all necessary informations for the
 uploader. The `config` file is a JSON/YAML file that contains the following
 keys: * `persistent_id`: Persistent identifier of the dataset to upload to. *
 `dataverse_url`: URL of the Dataverse instance. * `api_token`: API token of the
 Dataverse instance. * `files`: List of files to upload. Each file is a
 dictionary with the following keys: * `filepath`: Path to the file to upload. *
-`directoryLabel`: Optional directory label to upload the file to. *
+`directory_label`: Optional directory label to upload the file to. *
 `description`: Optional description of the file. * `mimetype`: Mimetype of the
 file. * `categories`: Optional list of categories to assign to the file. *
 `restrict`: Boolean to indicate that this is a restricted file. Defaults to
 False. In the following example, we upload three files to a Dataverse instance.
 The first file is uploaded to the root directory of the dataset, while the
 other two files are uploaded to the directory `some/dir`. ```yaml # config.yml
 persistent_id: doi:10.70122/XXX/XXXXX dataverse_url: https://
 demo.dataverse.org/ api_token: XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX files: -
-filepath: ./small.txt - filepath: ./medium.txt directoryLabel: some/dir -
-filepath: ./big.txt directoryLabel: some/dir ``` The `config` file can then be
+filepath: ./small.txt - filepath: ./medium.txt directory_label: some/dir -
+filepath: ./big.txt directory_label: some/dir ``` The `config` file can then be
 used as follows: ```bash dvuploader --config-path config.yml ```
```

### Comparing `dvuploader-0.2.2/dvuploader/cli.py` & `dvuploader-0.2.3/dvuploader/cli.py`

 * *Files identical despite different names*

### Comparing `dvuploader-0.2.2/dvuploader/directupload.py` & `dvuploader-0.2.3/dvuploader/directupload.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         upload_results = await asyncio.gather(*tasks)
 
     for status, file in upload_results:
         if status is True:
             continue
 
-        print(f"❌ Failed to upload file '{file.fileName}' to the S3 storage")
+        print(f"❌ Failed to upload file '{file.file_name}' to the S3 storage")
 
     headers = {
         "X-Dataverse-key": api_token,
         "x-amz-tagging": "dv-state=temp",
     }
 
     pbar = progress.add_task("╰── [bold white]Registering files", total=1)
@@ -125,42 +125,38 @@
 
     Returns:
         tuple: A tuple containing the upload status (bool) and the file object.
     """
 
     await asyncio.sleep(delay)
 
-    assert file.fileName is not None, "File name is None"
-    assert os.path.exists(file.filepath), f"File {file.filepath} does not exist"
-
-    file_size = os.path.getsize(file.filepath)
     ticket = await _request_ticket(
         session=session,
         dataverse_url=dataverse_url,
         api_token=api_token,
-        file_size=file_size,
+        file_size=file._size,
         persistent_id=persistent_id,
     )
 
     if not "urls" in ticket:
         status, storage_identifier = await _upload_singlepart(
             session=session,
             ticket=ticket,
-            filepath=file.filepath,
+            file=file,
             pbar=pbar,
             progress=progress,
             api_token=api_token,
             leave_bar=leave_bar,
         )
 
     else:
         status, storage_identifier = await _upload_multipart(
             session=session,
             response=ticket,
-            filepath=file.filepath,
+            file=file,
             dataverse_url=dataverse_url,
             pbar=pbar,
             progress=progress,
             api_token=api_token,
         )
 
     file.storageIdentifier = storage_identifier
@@ -203,15 +199,15 @@
         payload = await response.json()
         return payload["data"]
 
 
 async def _upload_singlepart(
     session: aiohttp.ClientSession,
     ticket: Dict,
-    filepath: str,
+    file: File,
     pbar,
     progress,
     api_token: str,
     leave_bar: bool,
 ) -> Tuple[bool, str]:
     """
     Uploads a single part of a file to a remote server using HTTP PUT method.
@@ -237,53 +233,48 @@
         "X-Dataverse-key": api_token,
         "x-amz-tagging": "dv-state=temp",
     }
     storage_identifier = ticket["storageIdentifier"]
     params = {
         "headers": headers,
         "url": ticket["url"],
-        "data": open(filepath, "rb"),
+        "data": file.handler,
     }
 
     async with session.put(**params) as response:
         status = response.status == 200
         response.raise_for_status()
 
         if status:
-            progress.update(
-                pbar,
-                advance=os.path.getsize(filepath),
-            )
-
+            progress.update(pbar, advance=file._size)
             await asyncio.sleep(0.1)
-
             progress.update(
                 pbar,
                 visible=leave_bar,
             )
 
         return status, storage_identifier
 
 
 async def _upload_multipart(
     session: aiohttp.ClientSession,
     response: Dict,
-    filepath: str,
+    file: File,
     dataverse_url: str,
     pbar,
     progress,
     api_token: str,
 ):
     """
     Uploads a file to Dataverse using multipart upload.
 
     Args:
         session (aiohttp.ClientSession): The aiohttp client session.
         response (Dict): The response from the Dataverse API containing the upload ticket information.
-        filepath (str): The path to the file to be uploaded.
+        file (File): The file object to be uploaded.
         dataverse_url (str): The URL of the Dataverse instance.
         pbar (tqdm): A progress bar to track the upload progress.
         progress: The progress callback function.
 
     Returns:
         Tuple[bool, str]: A tuple containing a boolean indicating the success of the upload and the storage identifier for the uploaded file.
     """
@@ -297,27 +288,28 @@
     storage_identifier = response["storageIdentifier"]
 
     # Chunk file and retrieve paths and urls
     chunk_size = int(part_size)
 
     try:
         e_tags = await _chunked_upload(
-            filepath=filepath,
+            file=file,
             session=session,
             urls=urls,
             chunk_size=chunk_size,
             pbar=pbar,
             progress=progress,
         )
     except Exception as e:
-        print(f"❌ Failed to upload file '{filepath}' to the S3 storage")
+        print(f"❌ Failed to upload file '{file.file_name}' to the S3 storage")
         await _abort_upload(
             session=session,
             url=abort,
             dataverse_url=dataverse_url,
+            api_token=api_token,
         )
         raise e
 
     await _complete_upload(
         session=session,
         url=complete,
         dataverse_url=dataverse_url,
@@ -325,37 +317,47 @@
         api_token=api_token,
     )
 
     return True, storage_identifier
 
 
 async def _chunked_upload(
-    filepath: str,
+    file: File,
     session: aiohttp.ClientSession,
     urls,
     chunk_size: int,
     pbar,
     progress,
 ):
     """
     Uploads a file in chunks to multiple URLs using the provided session.
 
     Args:
-        filepath (str): The path of the file to upload.
+        file (File): The file object to upload.
         session (aiohttp.ClientSession): The aiohttp client session to use for the upload.
         urls: An iterable of URLs to upload the file chunks to.
         chunk_size (int): The size of each chunk in bytes.
         pbar (tqdm): The progress bar to update during the upload.
         progress: The progress object to track the upload progress.
 
     Returns:
         List[str]: A list of ETags returned by the server for each uploaded chunk.
     """
     e_tags = []
-    async with aiofiles.open(filepath, "rb") as f:
+
+    if not os.path.exists(file.filepath):
+        raise NotImplementedError(
+            """
+
+            Multipart chunked upload is currently only supported for local files and no in-memory objects.
+            Please save the handlers content to a local file and try again.
+            """
+        )
+
+    async with aiofiles.open(file.filepath, "rb") as f:
         chunk = await f.read(chunk_size)
         e_tags.append(
             await _upload_chunk(
                 session=session,
                 url=next(urls),
                 file=BytesIO(chunk),
             )
@@ -455,27 +457,34 @@
         response.raise_for_status()
 
 
 async def _abort_upload(
     session: aiohttp.ClientSession,
     url: str,
     dataverse_url: str,
+    api_token: str,
 ):
     """
     Aborts an ongoing upload by sending a DELETE request to the specified URL.
 
     Args:
         session (aiohttp.ClientSession): The aiohttp client session.
         url (str): The URL to send the DELETE request to.
         dataverse_url (str): The base URL of the Dataverse instance.
+        api_token (str): The API token to use for the request.
 
     Raises:
         aiohttp.ClientResponseError: If the DELETE request fails.
     """
-    async with session.delete(urljoin(dataverse_url, url)) as response:
+
+    headers = {
+        "X-Dataverse-key": api_token,
+    }
+
+    async with session.delete(urljoin(dataverse_url, url), headers=headers) as response:
         response.raise_for_status()
 
 
 async def _add_files_to_ds(
     session: aiohttp.ClientSession,
     dataverse_url: str,
     pid: str,
@@ -559,13 +568,14 @@
 
     Raises:
         aiohttp.ClientResponseError: If the response status code is not successful.
 
     Returns:
         None
     """
+
     with aiohttp.MultipartWriter("form-data") as writer:
         json_part = writer.append(json_data)
         json_part.set_content_disposition("form-data", name="jsonData")
 
         async with session.post(url, data=writer) as response:
             response.raise_for_status()
```

### Comparing `dvuploader-0.2.2/dvuploader/dvuploader.py` & `dvuploader-0.2.3/dvuploader/dvuploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import json
 from urllib.parse import urljoin
 import requests
 import os
 import rich
 from typing import Dict, List, Optional
 
 from pydantic import BaseModel
@@ -30,14 +31,15 @@
     Methods:
         upload(persistent_id: str, dataverse_url: str, api_token: str) -> None:
             Uploads the files to the specified Dataverse repository in parallel.
 
     """
 
     files: List[File]
+    verbose: bool = True
 
     def upload(
         self,
         persistent_id: str,
         dataverse_url: str,
         api_token: str,
         n_parallel_uploads: int = 1,
@@ -52,64 +54,68 @@
             api_token (str): The API token for the Dataverse repository.
             n_parallel_uploads (int): The number of parallel uploads to execute. In the case of direct upload, this restricts the amount of parallel chunks per upload. Please use n_jobs to control parallel files.
 
         Returns:
             None
         """
 
-        print("\n")
+        if self.verbose:
+            print("\n")
+
         info = "\n".join(
             [
                 f"Server: [bold]{dataverse_url}[/bold]",  # type: ignore
                 f"PID: [bold]{persistent_id}[/bold]",  # type: ignore
                 f"Files: {len(self.files)}",
             ]
         )
 
         panel = Panel(
             info,
             title="[bold]DVUploader[/bold]",
             expand=False,
         )
 
-        rich.print(panel)
+        if self.verbose:
+            rich.print(panel)
 
-        asyncio.run(self._validate_and_hash_files())
+        asyncio.run(self._validate_and_hash_files(verbose=self.verbose))
 
         # Check for duplicates
         self._check_duplicates(
             dataverse_url=dataverse_url,
             persistent_id=persistent_id,
             api_token=api_token,
         )
 
         # Sort files by size
         files = sorted(
             self.files,
-            key=lambda x: os.path.getsize(x.filepath),
+            key=lambda x: x._size,
             reverse=False,
         )
 
         if not self.files:
             rich.print("\n[bold italic white]❌ No files to upload\n")
             return
 
         # Check if direct upload is supported
         has_direct_upload = self._has_direct_upload(
             dataverse_url=dataverse_url,
             api_token=api_token,
             persistent_id=persistent_id,
         )
 
-        if not has_direct_upload and not force_native:
+        if not has_direct_upload and not force_native and self.verbose:
             rich.print(
                 "\n[bold italic white]⚠️  Direct upload not supported. Falling back to Native API."
             )
 
-        rich.print(f"\n[bold italic white]🚀 Uploading files\n")
+        if self.verbose:
+            rich.print(f"\n[bold italic white]🚀 Uploading files\n")
 
         progress, pbars = self.setup_progress_bars(files=files)
 
         if not has_direct_upload or force_native:
             with progress:
                 asyncio.run(
                     native_upload(
@@ -132,53 +138,66 @@
                         persistent_id=persistent_id,
                         pbars=pbars,
                         progress=progress,
                         n_parallel_uploads=n_parallel_uploads,
                     )
                 )
 
-        rich.print("\n[bold italic white]✅ Upload complete\n")
+        if self.verbose:
+            rich.print("\n[bold italic white]✅ Upload complete\n")
 
-    async def _validate_and_hash_files(self):
+    async def _validate_and_hash_files(self, verbose: bool):
         """
         Validates and hashes the files to be uploaded.
 
         Returns:
             None
         """
 
+        if not verbose:
+            tasks = [
+                self._validate_and_hash_file(file=file, verbose=self.verbose)
+                for file in self.files
+            ]
+
+            await asyncio.gather(*tasks)
+            return
+
         print("\n")
 
         progress = Progress()
         task = progress.add_task(
-            "[bold italic white]📦 Preparing upload[/bold italic white]",
+            "[bold italic white]\n📦 Preparing upload[/bold italic white]",
             total=len(self.files),
         )
+
         with progress:
+
             tasks = [
                 self._validate_and_hash_file(
-                    file=file,
-                    progress=progress,
-                    task_id=task,
+                    file=file, progress=progress, task_id=task, verbose=self.verbose
                 )
                 for file in self.files
             ]
 
             await asyncio.gather(*tasks)
 
         print("\n")
 
     @staticmethod
     async def _validate_and_hash_file(
         file: File,
-        progress: Progress,
-        task_id: TaskID,
+        verbose: bool,
+        progress: Optional[Progress] = None,
+        task_id: Optional[TaskID] = None,
     ):
-        file.extract_filename_hash_file()
-        progress.update(task_id, advance=1)
+        file.extract_file_name_hash_file()
+
+        if verbose:
+            progress.update(task_id, advance=1)  # type: ignore
 
     def _check_duplicates(
         self,
         dataverse_url: str,
         persistent_id: str,
         api_token: str,
     ):
@@ -213,24 +232,24 @@
         n_skip_files = 0
 
         for file in self.files:
             has_same_hash = any(
                 map(lambda dsFile: self._check_hashes(file, dsFile), ds_files)
             )
 
-            if has_same_hash and file.checksum:
+            if has_same_hash:
                 n_skip_files += 1
                 table.add_row(
-                    file.fileName, "[bright_black]Same hash", "[bright_black]Skip"
+                    file.file_name, "[bright_black]Same hash", "[bright_black]Skip"
                 )
                 to_remove.append(file)
             else:
                 n_new_files += 1
                 table.add_row(
-                    file.fileName, "[spring_green3]New", "[spring_green3]Upload"
+                    file.file_name, "[spring_green3]New", "[spring_green3]Upload"
                 )
 
                 # If present in dataset, replace file
                 file.file_id = self._get_file_id(file, ds_files)
                 file.to_replace = True if file.file_id else False
 
         for file in to_remove:
@@ -241,15 +260,16 @@
         if over_threshold:
             table = Table(title="[bold white]🔎 Checking dataset files")
 
             table.add_column("New", style="spring_green3", no_wrap=True)
             table.add_column("Skipped", style="bright_black", no_wrap=True)
             table.add_row(str(n_new_files), str(n_skip_files))
 
-        console.print(table)
+        if self.verbose:
+            console.print(table)
 
     @staticmethod
     def _get_file_id(
         file: File,
         ds_files: List[Dict],
     ) -> Optional[str]:
         """
@@ -263,18 +283,18 @@
         Returns:
             str: The ID of the file.
 
         Raises:
             ValueError: If the file cannot be found in the dataset.
         """
 
-        # Find the file that matches label and directoryLabel
+        # Find the file that matches label and directory_label
         for ds_file in ds_files:
             dspath = os.path.join(ds_file.get("directoryLabel", ""), ds_file["label"])
-            fpath = os.path.join(file.directoryLabel, file.fileName)  # type: ignore
+            fpath = os.path.join(file.directory_label, file.file_name)  # type: ignore
 
             if dspath == fpath:
                 return ds_file["dataFile"]["id"]
 
     @staticmethod
     def _check_hashes(file: File, dsFile: Dict):
         """
@@ -288,20 +308,22 @@
             bool: True if the files have the same checksum, False otherwise.
         """
 
         if not file.checksum:
             return False
 
         hash_algo, hash_value = tuple(dsFile["dataFile"]["checksum"].values())
+        path = os.path.join(
+            dsFile.get("directoryLabel", ""), dsFile["dataFile"]["filename"]
+        )
 
         return (
             file.checksum.value == hash_value
             and file.checksum.type == hash_algo
-            and file.fileName == dsFile["label"]
-            and file.directoryLabel == dsFile.get("directoryLabel", "")
+            and path == os.path.join(file.directory_label, file.file_name)  # type: ignore
         )
 
     @staticmethod
     def _has_direct_upload(
         dataverse_url: str,
         api_token: str,
         persistent_id: str,
@@ -330,14 +352,14 @@
         Returns:
             A list of progress bars, one for each file in the uploader.
         """
 
         progress = Progress()
         tasks = [
             setup_pbar(
-                fpath=file.filepath,
+                file=file,
                 progress=progress,
             )
             for file in files
         ]
 
         return progress, tasks
```

### Comparing `dvuploader-0.2.2/dvuploader/file.py` & `dvuploader-0.2.3/dvuploader/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,88 @@
+from io import BytesIO, StringIO
 import os
-from typing import List, Optional, Union
+from typing import List, Optional, Union, IO
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
+from pydantic.fields import PrivateAttr
 import rich
 
 from dvuploader.checksum import Checksum, ChecksumTypes
 
 
 class File(BaseModel):
     """
     Represents a file with its properties and methods.
 
     Attributes:
         filepath (str): The path to the file.
         description (str): The description of the file.
-        directoryLabel (str): The label of the directory where the file is stored.
+        directory_label (str): The label of the directory where the file is stored.
         mimeType (str): The MIME type of the file.
         categories (List[str]): The categories associated with the file.
         restrict (bool): Indicates if the file is restricted.
         checksum_type (ChecksumTypes): The type of checksum used for the file.
         storageIdentifier (Optional[str]): The identifier of the storage where the file is stored.
-        fileName (Optional[str]): The name of the file.
+        file_name (Optional[str]): The name of the file.
         checksum (Optional[Checksum]): The checksum of the file.
         to_replace (bool): Indicates if the file should be replaced.
         file_id (Optional[str]): The ID of the file.
 
     Methods:
         _validate_filepath(path): Validates if the file path exists and is a file.
-        _extract_filename_hash_file(): Extracts the filename from the filepath and calculates the file's checksum.
+        _extract_file_name_hash_file(): Extracts the file_name from the filepath and calculates the file's checksum.
 
     """
 
-    model_config: ConfigDict = ConfigDict(populate_by_alias=True)
+    model_config = ConfigDict(
+        populate_by_name=True,
+        arbitrary_types_allowed=True,
+    )
 
     filepath: str = Field(..., exclude=True)
+    handler: Union[BytesIO, StringIO, IO, None] = Field(default=None, exclude=True)
     description: str = ""
-    directoryLabel: str = ""
+    directory_label: str = Field(default="", alias="directoryLabel")
     mimeType: str = "text/plain"
     categories: List[str] = ["DATA"]
     restrict: bool = False
     checksum_type: ChecksumTypes = Field(default=ChecksumTypes.MD5, exclude=True)
     storageIdentifier: Optional[str] = None
-    fileName: Optional[str] = None
+    file_name: Optional[str] = Field(default=None, alias="fileName")
     checksum: Optional[Checksum] = None
     to_replace: bool = False
     file_id: Optional[Union[str, int]] = Field(default=None, alias="fileToReplaceId")
 
-    def extract_filename_hash_file(self):
+    _size: int = PrivateAttr(default=0)
+
+    def extract_file_name_hash_file(self):
         """
-        Extracts the filename and calculates the hash of the file.
+        Extracts the file_name and calculates the hash of the file.
 
         Returns:
             self: The current instance of the class.
         """
-        self._validate_filepath(self.filepath)
-        self.fileName = os.path.basename(self.filepath)
 
         # Hash file
         hash_algo, hash_fun = self.checksum_type.value
+
+        if self.handler is None:
+            self._validate_filepath(self.filepath)
+            self.handler = open(self.filepath, "rb")
+            self._size = os.path.getsize(self.filepath)
+        else:
+            self._size = len(self.handler.read())
+            self.directory_label = os.path.dirname(self.filepath)
+            self.handler.seek(0)
+
+        if self.file_name is None:
+            self.file_name = os.path.basename(self.filepath)
+
         self.checksum = Checksum.from_file(
-            fpath=self.filepath,
+            handler=self.handler,
             hash_fun=hash_fun,
             hash_algo=hash_algo,
         )
 
         return self
 
     @staticmethod
```

### Comparing `dvuploader-0.2.2/dvuploader/nativeupload.py` & `dvuploader-0.2.3/dvuploader/nativeupload.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import asyncio
 import json
 import os
 import tempfile
 from typing import List, Tuple
+from typing_extensions import Dict
 import aiofiles
 import aiohttp
 
 from rich.progress import Progress, TaskID
 
 from dvuploader.file import File
 from dvuploader.packaging import distribute_files, zip_files
-from dvuploader.utils import build_url
+from dvuploader.utils import build_url, retrieve_dataset_files
 
 MAX_RETRIES = os.environ.get("DVUPLOADER_MAX_RETRIES", 15)
 NATIVE_UPLOAD_ENDPOINT = "/api/datasets/:persistentId/add"
 NATIVE_REPLACE_ENDPOINT = "/api/files/{FILE_ID}/replace"
+NATIVE_METADATA_ENDPOINT = "/api/files/{FILE_ID}/metadata"
 
 assert isinstance(MAX_RETRIES, int), "DVUPLOADER_MAX_RETRIES must be an integer"
 
 
 async def native_upload(
     files: List[File],
     dataverse_url: str,
@@ -70,20 +72,36 @@
                     pbar=pbar,  # type: ignore
                     progress=progress,
                 )
                 for pbar, file in packaged_files
             ]
 
             responses = await asyncio.gather(*tasks)
+            _validate_upload_responses(responses, files)
+
+            await _update_metadata(
+                session=session,
+                files=files,
+                persistent_id=persistent_id,
+                dataverse_url=dataverse_url,
+                api_token=api_token,
+            )
+
+
+def _validate_upload_responses(
+    responses: List[Tuple],
+    files: List[File],
+) -> None:
+    """Validates the responses of the native upload requests."""
 
     for (status, response), file in zip(responses, files):
         if status == 200:
             continue
 
-        print(f"❌ Failed to upload file '{file.fileName}': {response['message']}")
+        print(f"❌ Failed to upload file '{file.file_name}': {response['message']}")
 
 
 def _zip_packages(
     packages: List[Tuple[int, List[File]]],
     tmp_dir: str,
     progress: Progress,
 ) -> List[Tuple[TaskID, File]]:
@@ -108,20 +126,20 @@
                 filepath=zip_files(
                     files=package,
                     tmp_dir=tmp_dir,
                     index=index,
                 ),
             )
 
-            file.extract_filename_hash_file()
+            file.extract_file_name_hash_file()
             file.mimeType = "application/zip"
 
         pbar = progress.add_task(
-            file.fileName,  # type: ignore
-            total=os.path.getsize(file.filepath),
+            file.file_name,  # type: ignore
+            total=file._size,
         )
 
         files.append((pbar, file))
 
     return files
 
 
@@ -170,62 +188,49 @@
             persistentId=persistent_id,
         )
     else:
         endpoint = build_url(
             endpoint=NATIVE_REPLACE_ENDPOINT.format(FILE_ID=file.file_id),
         )
 
-    json_data = {
-        "description": file.description,
-        "forceReplace": True,
-        "directoryLabel": file.directoryLabel,
-        "categories": file.categories,
-        "restrict": file.restrict,
-        "forceReplace": True,
-    }
+    json_data = _get_json_data(file)
 
     for _ in range(MAX_RETRIES):
-        with aiohttp.MultipartWriter("form-data") as writer:
-            json_part = writer.append(json.dumps(json_data))
-            json_part.set_content_disposition("form-data", name="jsonData")
-
-            file_part = writer.append(
-                file_sender(
-                    file_name=file.filepath,
-                    progress=progress,
-                    pbar=pbar,
-                )
-            )
-            file_part.set_content_disposition(
-                "form-data",
-                name="file",
-                filename=file.fileName,
-            )
-            async with session.post(endpoint, data=writer) as response:
-                status = response.status
 
-                if status == 200:
-                    progress.update(
-                        pbar,
-                        advance=os.path.getsize(file.filepath),
-                    )
+        formdata = aiohttp.FormData()
+        formdata.add_field(
+            "jsonData",
+            json.dumps(json_data),
+            content_type="application/json",
+        )
+        formdata.add_field(
+            "file",
+            file.handler,
+            filename=file.file_name,
+        )
+
+        async with session.post(endpoint, data=formdata) as response:
+            status = response.status
+
+            if status == 200:
+                progress.update(pbar, advance=file._size, complete=file._size)
 
-                    # Wait to avoid rate limiting
-                    await asyncio.sleep(0.7)
+                # Wait to avoid rate limiting
+                await asyncio.sleep(0.7)
 
-                    return status, await response.json()
+                return status, await response.json()
 
         # Wait to avoid rate limiting
         await asyncio.sleep(1.0)
 
     return False, {"message": "Failed to upload file"}
 
 
-async def file_sender(
-    file_name: str,
+def file_sender(
+    file: File,
     progress: Progress,
     pbar: TaskID,
 ):
     """
     Asynchronously reads and yields chunks of a file.
 
     Args:
@@ -233,15 +238,142 @@
         progress (Progress): The progress object to track the file upload progress.
         pbar (TaskID): The ID of the progress bar associated with the file upload.
 
     Yields:
         bytes: The chunks of the file.
 
     """
+
+    assert file.handler is not None, "File handler is not set."
+
     chunk_size = 64 * 1024  # 10 MB
-    async with aiofiles.open(file_name, "rb") as f:
-        chunk = await f.read(chunk_size)
+    chunk = file.handler.read(chunk_size)
+    progress.advance(pbar, advance=chunk_size)
+
+    while chunk:
+        yield chunk
+        chunk = file.handler.read(chunk_size)
         progress.advance(pbar, advance=chunk_size)
-        while chunk:
-            yield chunk
-            chunk = await f.read(chunk_size)
-            progress.advance(pbar, advance=chunk_size)
+
+
+def _get_json_data(file: File) -> Dict:
+    """Returns the JSON data for the native upload request."""
+    return {
+        "description": file.description,
+        "directoryLabel": file.directory_label,
+        "categories": file.categories,
+        "restrict": file.restrict,
+        "forceReplace": True,
+    }
+
+
+async def _update_metadata(
+    session: aiohttp.ClientSession,
+    files: List[File],
+    dataverse_url: str,
+    api_token: str,
+    persistent_id: str,
+):
+    """Updates the metadata of the given files in a Dataverse repository.
+
+    Args:
+
+        session (aiohttp.ClientSession): The aiohttp client session.
+        files (List[File]): The files to update the metadata for.
+        dataverse_url (str): The URL of the Dataverse repository.
+        api_token (str): The API token of the Dataverse repository.
+        persistent_id (str): The persistent identifier of the dataset.
+    """
+
+    file_mapping = _retrieve_file_ids(
+        persistent_id=persistent_id,
+        dataverse_url=dataverse_url,
+        api_token=api_token,
+    )
+
+    tasks = []
+
+    for file in files:
+        dv_path = os.path.join(file.directory_label, file.file_name)  # type: ignore
+
+        try:
+            file_id = file_mapping[dv_path]
+        except KeyError:
+            raise ValueError(
+                (
+                    f"File {dv_path} not found in Dataverse repository.",
+                    "This may be due to the file not being uploaded to the repository.",
+                )
+            )
+
+        task = _update_single_metadata(
+            session=session,
+            url=NATIVE_METADATA_ENDPOINT.format(FILE_ID=file_id),
+            file=file,
+        )
+
+        tasks.append(task)
+
+    await asyncio.gather(*tasks)
+
+
+async def _update_single_metadata(
+    session: aiohttp.ClientSession,
+    url: str,
+    file: File,
+) -> None:
+    """Updates the metadata of a single file in a Dataverse repository."""
+
+    json_data = _get_json_data(file)
+
+    del json_data["forceReplace"]
+    del json_data["restrict"]
+
+    formdata = aiohttp.FormData()
+    formdata.add_field(
+        "jsonData",
+        json.dumps(json_data),
+        content_type="application/json",
+    )
+
+    async with session.post(url, data=formdata) as response:
+        response.raise_for_status()
+
+
+def _retrieve_file_ids(
+    persistent_id: str,
+    dataverse_url: str,
+    api_token: str,
+) -> Dict[str, str]:
+    """Retrieves the file IDs of the given files.
+
+    Args:
+        files (List[File]): The files to retrieve the IDs for.
+        persistent_id (str): The persistent identifier of the dataset.
+        dataverse_url (str): The URL of the Dataverse repository.
+        api_token (str): The API token of the Dataverse repository.
+
+    Returns:
+        Dict[str, str]: The list of file IDs.
+    """
+
+    # Fetch file metadata
+    ds_files = retrieve_dataset_files(
+        persistent_id=persistent_id,
+        dataverse_url=dataverse_url,
+        api_token=api_token,
+    )
+
+    return _create_file_id_path_mapping(ds_files)
+
+
+def _create_file_id_path_mapping(files):
+    """Creates dictionary that maps from directoryLabel + filename to ID"""
+    mapping = {}
+
+    for file in files:
+        directory_label = file.get("directoryLabel", "")
+        file = file["dataFile"]
+        path = os.path.join(directory_label, file["filename"])
+        mapping[path] = file["id"]
+
+    return mapping
```

### Comparing `dvuploader-0.2.2/dvuploader/packaging.py` & `dvuploader-0.2.3/dvuploader/packaging.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,31 +23,30 @@
         List[List[File]]: The distributed packages of files.
     """
     packages = []
     current_package = []
     package_index = 0
     current_size = 0
     for file in dv_files:
-        file_size = os.path.getsize(file.filepath)
 
-        if file_size > MAXIMUM_PACKAGE_SIZE:
+        if file._size > MAXIMUM_PACKAGE_SIZE:
             current_package, current_size, package_index = _append_and_reset(
                 (package_index, [file]),
                 packages,
             )
             continue
 
-        if current_size + file_size > MAXIMUM_PACKAGE_SIZE:
+        if current_size + file._size > MAXIMUM_PACKAGE_SIZE:
             current_package, current_size, package_index = _append_and_reset(
                 (package_index, current_package),
                 packages,
             )
 
         current_package.append(file)
-        current_size += os.path.getsize(file.filepath)
+        current_size += file._size
     else:
         if current_package:
             _append_and_reset(
                 (package_index, current_package),
                 packages,
             )
 
@@ -87,17 +86,17 @@
     Returns:
         str: The path to the zip file.
     """
     path = os.path.join(tmp_dir, f"package_{index}.zip")
 
     with zipfile.ZipFile(path, "w") as zip_file:
         for file in files:
-            zip_file.write(
-                file.filepath,
-                arcname=_create_arcname(file),
+            zip_file.writestr(
+                data=file.handler.read(),
+                zinfo_or_arcname=_create_arcname(file),
             )
 
     return path
 
 
 def _create_arcname(file: "File"):  # type: ignore
     """
@@ -105,11 +104,11 @@
 
     Args:
         file (File): The file to create the arcname for.
 
     Returns:
         str: The arcname for the given file.
     """
-    if file.directoryLabel is not None:
-        return os.path.join(file.directoryLabel, file.fileName)  # type: ignore
+    if file.directory_label is not None:
+        return os.path.join(file.directory_label, file.file_name)  # type: ignore
     else:
-        return file.fileName
+        return file.file_name
```

### Comparing `dvuploader-0.2.2/dvuploader/utils.py` & `dvuploader-0.2.3/dvuploader/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,23 +68,23 @@
 
     return response.json()["data"]["latestVersion"]["files"]
 
 
 def add_directory(
     directory: str,
     ignore: List[str] = [r"^\."],
-    directory_label: str = "",
+    rootDirectoryLabel: str = "",
 ):
     """
     Recursively adds all files in the specified directory to a list of File objects.
 
     Args:
         directory (str): The directory path.
         ignore (List[str], optional): A list of regular expressions to ignore certain files or directories. Defaults to [r"^\."].
-        directory_label (str, optional): The label to be added to the directory path of each file. Defaults to "".
+        rootDirectoryLabel (str, optional): The label to be added to the directory path of each file. Defaults to "".
 
     Returns:
         List[File]: A list of File objects representing the files in the directory.
     """
     files = []
 
     # Part of the path to remove from the directory
@@ -92,25 +92,25 @@
         if not file.is_file():
             continue
         if part_is_ignored(str(file.name), ignore):
             continue
         if any(part_is_ignored(part, ignore) for part in list(file.parts)):
             continue
 
-        directoryLabel = _truncate_path(
+        directory_label = _truncate_path(
             file.parent,
             pathlib.Path(directory),
         )
 
         files.append(
             File(
                 filepath=str(file),
                 directoryLabel=os.path.join(
+                    rootDirectoryLabel,
                     directory_label,
-                    directoryLabel,
                 ),
             )
         )
 
     return files
 
 
@@ -148,28 +148,29 @@
     for pattern in ignore:
         if re.match(pattern, part):
             return True
     return False
 
 
 def setup_pbar(
-    fpath: str,
+    file: File,
     progress: Progress,
 ) -> int:
     """
     Set up a progress bar for a file.
 
     Args:
         fpath (str): The path to the file.
         progress (Progress): The progress bar object.
 
     Returns:
         int: The task ID of the progress bar.
     """
 
-    file_size = os.path.getsize(fpath)
-    fname = os.path.basename(fpath)
+    file_size = file._size
+    fname = file.file_name
 
     return progress.add_task(
         f"[pink]├── {fname}",
+        start=True,
         total=file_size,
     )
```

### Comparing `dvuploader-0.2.2/pyproject.toml` & `dvuploader-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dvuploader"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python library for uploading (bulk) data to Dataverse"
 authors = ["Jan Range"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^2.5.3"
```

### Comparing `dvuploader-0.2.2/PKG-INFO` & `dvuploader-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvuploader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python library for uploading (bulk) data to Dataverse
 Author: Jan Range
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -68,16 +68,16 @@
 ```python
 import dvuploader as dv
 
 
 # Add file individually
 files = [
     dv.File(filepath="./small.txt"),
-    dv.File(directoryLabel="some/dir", filepath="./medium.txt"),
-    dv.File(directoryLabel="some/dir", filepath="./big.txt"),
+    dv.File(directory_label="some/dir", filepath="./medium.txt"),
+    dv.File(directory_label="some/dir", filepath="./big.txt"),
     *dv.add_directory("./data"), # Add an entire directory
 ]
 
 DV_URL = "https://demo.dataverse.org/"
 API_TOKEN = "XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
 PID = "doi:10.70122/XXX/XXXXX"
 
@@ -108,15 +108,15 @@
 Alternatively, you can also supply a `config` file that contains all necessary informations for the uploader. The `config` file is a JSON/YAML file that contains the following keys:
 
 * `persistent_id`: Persistent identifier of the dataset to upload to.
 * `dataverse_url`: URL of the Dataverse instance.
 * `api_token`: API token of the Dataverse instance.
 * `files`: List of files to upload. Each file is a dictionary with the following keys:
   * `filepath`: Path to the file to upload.
-  * `directoryLabel`: Optional directory label to upload the file to.
+  * `directory_label`: Optional directory label to upload the file to.
   * `description`: Optional description of the file.
   * `mimetype`: Mimetype of the file.
   * `categories`: Optional list of categories to assign to the file.
   * `restrict`: Boolean to indicate that this is a restricted file. Defaults to False.
 
 In the following example, we upload three files to a Dataverse instance. The first file is uploaded to the root directory of the dataset, while the other two files are uploaded to the directory `some/dir`.
 
@@ -124,17 +124,17 @@
 # config.yml
 persistent_id: doi:10.70122/XXX/XXXXX
 dataverse_url: https://demo.dataverse.org/
 api_token: XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
 files:
     - filepath: ./small.txt
     - filepath: ./medium.txt
-      directoryLabel: some/dir
+      directory_label: some/dir
     - filepath: ./big.txt
-      directoryLabel: some/dir
+      directory_label: some/dir
 ```
 
 The `config` file can then be used as follows:
 
 ```bash
 dvuploader --config-path config.yml
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvuploader Version: 0.2.2 Summary: Python library
+Metadata-Version: 2.1 Name: dvuploader Version: 0.2.3 Summary: Python library
 for uploading (bulk) data to Dataverse Author: Jan Range Requires-Python:
 >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiodns (>=3.1.1,<4.0.0) Requires-Dist: aiofiles
 (>=23.2.1,<24.0.0) Requires-Dist: aiohttp (>=3.9.1,<4.0.0) Requires-Dist:
@@ -25,17 +25,17 @@
 dvuploader ``` or by source ```bash git clone https://github.com/gdcc/python-
 dvuploader.git cd python-dvuploader python3 -m pip install . ``` ## Quickstart
 ### Programmatic usage In order to perform a direct upload, you need to have a
 Dataverse instance running and a cloud storage provider. The following example
 shows how to upload files to a Dataverse instance. Simply provide the files of
 interest and utilize the `upload` method of a `DVUploader` instance. ```python
 import dvuploader as dv # Add file individually files = [ dv.File(filepath="./
-small.txt"), dv.File(directoryLabel="some/dir", filepath="./medium.txt"),
-dv.File(directoryLabel="some/dir", filepath="./big.txt"), *dv.add_directory("./
-data"), # Add an entire directory ] DV_URL = "https://demo.dataverse.org/
+small.txt"), dv.File(directory_label="some/dir", filepath="./medium.txt"),
+dv.File(directory_label="some/dir", filepath="./big.txt"), *dv.add_directory
+("./data"), # Add an entire directory ] DV_URL = "https://demo.dataverse.org/
 " API_TOKEN = "XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX" PID = "doi:10.70122/XXX/
 XXXXX" dvuploader = dv.DVUploader(files=files) dvuploader.upload
 ( api_token=API_TOKEN, dataverse_url=DV_URL, persistent_id=PID,
 n_parallel_uploads=2, # Whatever your instance can handle ) ``` ### Command
 Line Interface DVUploader ships with a CLI ready to use outside scripts. In
 order to upload files to a Dataverse instance, simply provide the files of
 interest, persistent identifier and credentials. #### Using arguments ```bash
@@ -44,19 +44,19 @@
 demo.dataverse.org/ \ ``` #### Using a config file Alternatively, you can also
 supply a `config` file that contains all necessary informations for the
 uploader. The `config` file is a JSON/YAML file that contains the following
 keys: * `persistent_id`: Persistent identifier of the dataset to upload to. *
 `dataverse_url`: URL of the Dataverse instance. * `api_token`: API token of the
 Dataverse instance. * `files`: List of files to upload. Each file is a
 dictionary with the following keys: * `filepath`: Path to the file to upload. *
-`directoryLabel`: Optional directory label to upload the file to. *
+`directory_label`: Optional directory label to upload the file to. *
 `description`: Optional description of the file. * `mimetype`: Mimetype of the
 file. * `categories`: Optional list of categories to assign to the file. *
 `restrict`: Boolean to indicate that this is a restricted file. Defaults to
 False. In the following example, we upload three files to a Dataverse instance.
 The first file is uploaded to the root directory of the dataset, while the
 other two files are uploaded to the directory `some/dir`. ```yaml # config.yml
 persistent_id: doi:10.70122/XXX/XXXXX dataverse_url: https://
 demo.dataverse.org/ api_token: XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX files: -
-filepath: ./small.txt - filepath: ./medium.txt directoryLabel: some/dir -
-filepath: ./big.txt directoryLabel: some/dir ``` The `config` file can then be
+filepath: ./small.txt - filepath: ./medium.txt directory_label: some/dir -
+filepath: ./big.txt directory_label: some/dir ``` The `config` file can then be
 used as follows: ```bash dvuploader --config-path config.yml ```
```

