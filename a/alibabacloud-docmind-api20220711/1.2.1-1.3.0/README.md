# Comparing `tmp/alibabacloud_docmind-api20220711-1.2.1.tar.gz` & `tmp/alibabacloud_docmind-api20220711-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_docmind-api20220711-1.2.1.tar", last modified: Tue Jan  9 06:53:38 2024, max compression
+gzip compressed data, was "dist/alibabacloud_docmind-api20220711-1.3.0.tar", last modified: Thu May  9 12:42:11 2024, max compression
```

## Comparing `alibabacloud_docmind-api20220711-1.2.1.tar` & `alibabacloud_docmind-api20220711-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      603 2024-01-09 06:53:37.000000 alibabacloud_docmind-api20220711-1.2.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-01-09 06:53:37.000000 alibabacloud_docmind-api20220711-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-01-09 06:53:37.000000 alibabacloud_docmind-api20220711-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2376 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2024-01-09 06:53:37.000000 alibabacloud_docmind-api20220711-1.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2024-01-09 06:53:37.000000 alibabacloud_docmind-api20220711-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711/
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-09 06:53:37.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711/__init__.py
--rw-r--r--   0 root         (0) root         (0)   120232 2024-01-09 06:53:37.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711/client.py
--rw-r--r--   0 root         (0) root         (0)    97384 2024-01-09 06:53:37.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2376 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-09 06:53:38.000000 alibabacloud_docmind-api20220711-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2844 2024-01-09 06:53:37.000000 alibabacloud_docmind-api20220711-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      677 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135724 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711/client.py
+-rw-r--r--   0 root         (0) root         (0)   105804 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-05-09 12:42:11.000000 alibabacloud_docmind-api20220711-1.3.0/setup.py
```

### Comparing `alibabacloud_docmind-api20220711-1.2.1/ChangeLog.md` & `alibabacloud_docmind-api20220711-1.3.0/ChangeLog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-01-09 Version: 1.2.1
+- Generated python 2022-07-11 for docmind-api.
+
 2023-11-01 Version: 1.2.0
 - Generated python 2022-07-11 for docmind-api.
 
 2023-09-19 Version: 1.1.0
 - Generated python 2022-07-11 for docmind-api.
 
 2023-06-13 Version: 1.0.4
```

### Comparing `alibabacloud_docmind-api20220711-1.2.1/LICENSE` & `alibabacloud_docmind-api20220711-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220711-1.2.1/PKG-INFO` & `alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_docmind-api20220711
-Version: 1.2.1
+Name: alibabacloud-docmind-api20220711
+Version: 1.3.0
 Summary: Alibaba Cloud docmind-api (20220711) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docmind-api-20220711/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_docmind-api20220711-1.2.1/README-CN.md` & `alibabacloud_docmind-api20220711-1.3.0/README-CN.md`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docmind-api-20220711/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_docmind-api20220711-1.2.1/README.md` & `alibabacloud_docmind-api20220711-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docmind-api-20220711/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711/client.py` & `alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -717,14 +717,104 @@
     async def submit_convert_image_to_excel_job_async(
         self,
         request: docmind_api_20220711_models.SubmitConvertImageToExcelJobRequest,
     ) -> docmind_api_20220711_models.SubmitConvertImageToExcelJobResponse:
         runtime = util_models.RuntimeOptions()
         return await self.submit_convert_image_to_excel_job_with_options_async(request, runtime)
 
+    def submit_convert_image_to_markdown_job_with_options(
+        self,
+        tmp_req: docmind_api_20220711_models.SubmitConvertImageToMarkdownJobRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> docmind_api_20220711_models.SubmitConvertImageToMarkdownJobResponse:
+        UtilClient.validate_model(tmp_req)
+        request = docmind_api_20220711_models.SubmitConvertImageToMarkdownJobShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.image_names):
+            request.image_names_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.image_names, 'ImageNames', 'simple')
+        if not UtilClient.is_unset(tmp_req.image_urls):
+            request.image_urls_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.image_urls, 'ImageUrls', 'simple')
+        query = {}
+        if not UtilClient.is_unset(request.image_name_extension):
+            query['ImageNameExtension'] = request.image_name_extension
+        if not UtilClient.is_unset(request.image_names_shrink):
+            query['ImageNames'] = request.image_names_shrink
+        if not UtilClient.is_unset(request.image_urls_shrink):
+            query['ImageUrls'] = request.image_urls_shrink
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SubmitConvertImageToMarkdownJob',
+            version='2022-07-11',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            docmind_api_20220711_models.SubmitConvertImageToMarkdownJobResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def submit_convert_image_to_markdown_job_with_options_async(
+        self,
+        tmp_req: docmind_api_20220711_models.SubmitConvertImageToMarkdownJobRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> docmind_api_20220711_models.SubmitConvertImageToMarkdownJobResponse:
+        UtilClient.validate_model(tmp_req)
+        request = docmind_api_20220711_models.SubmitConvertImageToMarkdownJobShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.image_names):
+            request.image_names_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.image_names, 'ImageNames', 'simple')
+        if not UtilClient.is_unset(tmp_req.image_urls):
+            request.image_urls_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.image_urls, 'ImageUrls', 'simple')
+        query = {}
+        if not UtilClient.is_unset(request.image_name_extension):
+            query['ImageNameExtension'] = request.image_name_extension
+        if not UtilClient.is_unset(request.image_names_shrink):
+            query['ImageNames'] = request.image_names_shrink
+        if not UtilClient.is_unset(request.image_urls_shrink):
+            query['ImageUrls'] = request.image_urls_shrink
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SubmitConvertImageToMarkdownJob',
+            version='2022-07-11',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            docmind_api_20220711_models.SubmitConvertImageToMarkdownJobResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def submit_convert_image_to_markdown_job(
+        self,
+        request: docmind_api_20220711_models.SubmitConvertImageToMarkdownJobRequest,
+    ) -> docmind_api_20220711_models.SubmitConvertImageToMarkdownJobResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.submit_convert_image_to_markdown_job_with_options(request, runtime)
+
+    async def submit_convert_image_to_markdown_job_async(
+        self,
+        request: docmind_api_20220711_models.SubmitConvertImageToMarkdownJobRequest,
+    ) -> docmind_api_20220711_models.SubmitConvertImageToMarkdownJobResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.submit_convert_image_to_markdown_job_with_options_async(request, runtime)
+
     def submit_convert_image_to_pdf_job_with_options(
         self,
         tmp_req: docmind_api_20220711_models.SubmitConvertImageToPdfJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> docmind_api_20220711_models.SubmitConvertImageToPdfJobResponse:
         UtilClient.validate_model(tmp_req)
         request = docmind_api_20220711_models.SubmitConvertImageToPdfJobShrinkRequest()
@@ -1337,14 +1427,230 @@
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
             submit_convert_pdf_to_image_job_req.file_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         submit_convert_pdf_to_image_job_resp = await self.submit_convert_pdf_to_image_job_with_options_async(submit_convert_pdf_to_image_job_req, runtime)
         return submit_convert_pdf_to_image_job_resp
 
+    def submit_convert_pdf_to_markdown_job_with_options(
+        self,
+        request: docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.file_name):
+            query['FileName'] = request.file_name
+        if not UtilClient.is_unset(request.file_url):
+            query['FileUrl'] = request.file_url
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SubmitConvertPdfToMarkdownJob',
+            version='2022-07-11',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def submit_convert_pdf_to_markdown_job_with_options_async(
+        self,
+        request: docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.file_name):
+            query['FileName'] = request.file_name
+        if not UtilClient.is_unset(request.file_url):
+            query['FileUrl'] = request.file_url
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SubmitConvertPdfToMarkdownJob',
+            version='2022-07-11',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def submit_convert_pdf_to_markdown_job(
+        self,
+        request: docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobRequest,
+    ) -> docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.submit_convert_pdf_to_markdown_job_with_options(request, runtime)
+
+    async def submit_convert_pdf_to_markdown_job_async(
+        self,
+        request: docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobRequest,
+    ) -> docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.submit_convert_pdf_to_markdown_job_with_options_async(request, runtime)
+
+    def submit_convert_pdf_to_markdown_job_advance(
+        self,
+        request: docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobAdvanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobResponse:
+        # Step 0: init client
+        access_key_id = self._credential.get_access_key_id()
+        access_key_secret = self._credential.get_access_key_secret()
+        security_token = self._credential.get_security_token()
+        credential_type = self._credential.get_type()
+        open_platform_endpoint = self._open_platform_endpoint
+        if UtilClient.is_unset(open_platform_endpoint):
+            open_platform_endpoint = 'openplatform.aliyuncs.com'
+        if UtilClient.is_unset(credential_type):
+            credential_type = 'access_key'
+        auth_config = open_api_models.Config(
+            access_key_id=access_key_id,
+            access_key_secret=access_key_secret,
+            security_token=security_token,
+            type=credential_type,
+            endpoint=open_platform_endpoint,
+            protocol=self._protocol,
+            region_id=self._region_id
+        )
+        auth_client = OpenPlatformClient(auth_config)
+        auth_request = open_platform_models.AuthorizeFileUploadRequest(
+            product='docmind-api',
+            region_id=self._region_id
+        )
+        auth_response = open_platform_models.AuthorizeFileUploadResponse()
+        oss_config = oss_models.Config(
+            access_key_secret=access_key_secret,
+            type='access_key',
+            protocol=self._protocol,
+            region_id=self._region_id
+        )
+        oss_client = None
+        file_obj = file_form_models.FileField()
+        oss_header = oss_models.PostObjectRequestHeader()
+        upload_request = oss_models.PostObjectRequest()
+        oss_runtime = ossutil_models.RuntimeOptions()
+        OpenApiUtilClient.convert(runtime, oss_runtime)
+        submit_convert_pdf_to_markdown_job_req = docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobRequest()
+        OpenApiUtilClient.convert(request, submit_convert_pdf_to_markdown_job_req)
+        if not UtilClient.is_unset(request.file_url_object):
+            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
+            oss_client = OSSClient(oss_config)
+            file_obj = file_form_models.FileField(
+                filename=auth_response.body.object_key,
+                content=request.file_url_object,
+                content_type=''
+            )
+            oss_header = oss_models.PostObjectRequestHeader(
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
+                file=file_obj,
+                success_action_status='201'
+            )
+            upload_request = oss_models.PostObjectRequest(
+                bucket_name=auth_response.body.bucket,
+                header=oss_header
+            )
+            oss_client.post_object(upload_request, oss_runtime)
+            submit_convert_pdf_to_markdown_job_req.file_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
+        submit_convert_pdf_to_markdown_job_resp = self.submit_convert_pdf_to_markdown_job_with_options(submit_convert_pdf_to_markdown_job_req, runtime)
+        return submit_convert_pdf_to_markdown_job_resp
+
+    async def submit_convert_pdf_to_markdown_job_advance_async(
+        self,
+        request: docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobAdvanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobResponse:
+        # Step 0: init client
+        access_key_id = await self._credential.get_access_key_id_async()
+        access_key_secret = await self._credential.get_access_key_secret_async()
+        security_token = await self._credential.get_security_token_async()
+        credential_type = self._credential.get_type()
+        open_platform_endpoint = self._open_platform_endpoint
+        if UtilClient.is_unset(open_platform_endpoint):
+            open_platform_endpoint = 'openplatform.aliyuncs.com'
+        if UtilClient.is_unset(credential_type):
+            credential_type = 'access_key'
+        auth_config = open_api_models.Config(
+            access_key_id=access_key_id,
+            access_key_secret=access_key_secret,
+            security_token=security_token,
+            type=credential_type,
+            endpoint=open_platform_endpoint,
+            protocol=self._protocol,
+            region_id=self._region_id
+        )
+        auth_client = OpenPlatformClient(auth_config)
+        auth_request = open_platform_models.AuthorizeFileUploadRequest(
+            product='docmind-api',
+            region_id=self._region_id
+        )
+        auth_response = open_platform_models.AuthorizeFileUploadResponse()
+        oss_config = oss_models.Config(
+            access_key_secret=access_key_secret,
+            type='access_key',
+            protocol=self._protocol,
+            region_id=self._region_id
+        )
+        oss_client = None
+        file_obj = file_form_models.FileField()
+        oss_header = oss_models.PostObjectRequestHeader()
+        upload_request = oss_models.PostObjectRequest()
+        oss_runtime = ossutil_models.RuntimeOptions()
+        OpenApiUtilClient.convert(runtime, oss_runtime)
+        submit_convert_pdf_to_markdown_job_req = docmind_api_20220711_models.SubmitConvertPdfToMarkdownJobRequest()
+        OpenApiUtilClient.convert(request, submit_convert_pdf_to_markdown_job_req)
+        if not UtilClient.is_unset(request.file_url_object):
+            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
+            oss_client = OSSClient(oss_config)
+            file_obj = file_form_models.FileField(
+                filename=auth_response.body.object_key,
+                content=request.file_url_object,
+                content_type=''
+            )
+            oss_header = oss_models.PostObjectRequestHeader(
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
+                file=file_obj,
+                success_action_status='201'
+            )
+            upload_request = oss_models.PostObjectRequest(
+                bucket_name=auth_response.body.bucket,
+                header=oss_header
+            )
+            await oss_client.post_object_async(upload_request, oss_runtime)
+            submit_convert_pdf_to_markdown_job_req.file_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
+        submit_convert_pdf_to_markdown_job_resp = await self.submit_convert_pdf_to_markdown_job_with_options_async(submit_convert_pdf_to_markdown_job_req, runtime)
+        return submit_convert_pdf_to_markdown_job_resp
+
     def submit_convert_pdf_to_word_job_with_options(
         self,
         request: docmind_api_20220711_models.SubmitConvertPdfToWordJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> docmind_api_20220711_models.SubmitConvertPdfToWordJobResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1798,14 +2104,16 @@
         query = {}
         if not UtilClient.is_unset(request.file_name):
             query['FileName'] = request.file_name
         if not UtilClient.is_unset(request.file_name_extension):
             query['FileNameExtension'] = request.file_name_extension
         if not UtilClient.is_unset(request.file_url):
             query['FileUrl'] = request.file_url
+        if not UtilClient.is_unset(request.formula_enhancement):
+            query['FormulaEnhancement'] = request.formula_enhancement
         if not UtilClient.is_unset(request.structure_type):
             query['StructureType'] = request.structure_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitDocStructureJob',
@@ -1832,14 +2140,16 @@
         query = {}
         if not UtilClient.is_unset(request.file_name):
             query['FileName'] = request.file_name
         if not UtilClient.is_unset(request.file_name_extension):
             query['FileNameExtension'] = request.file_name_extension
         if not UtilClient.is_unset(request.file_url):
             query['FileUrl'] = request.file_url
+        if not UtilClient.is_unset(request.formula_enhancement):
+            query['FormulaEnhancement'] = request.formula_enhancement
         if not UtilClient.is_unset(request.structure_type):
             query['StructureType'] = request.structure_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitDocStructureJob',
```

### Comparing `alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711/models.py` & `alibabacloud_docmind-api20220711-1.3.0/alibabacloud_docmind_api20220711/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,17 +171,14 @@
         body: AyncTradeDocumentPackageExtractSmartAppResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -311,17 +308,14 @@
         body: GetDocStructureResultResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -439,17 +433,14 @@
         body: GetDocumentCompareResultResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -620,17 +611,14 @@
         body: GetDocumentConvertResultResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -748,17 +736,14 @@
         body: GetDocumentExtractResultResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -905,17 +890,14 @@
         body: GetPageNumResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1033,17 +1015,14 @@
         body: GetTableUnderstandingResultResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1241,17 +1220,14 @@
         body: SubmitConvertImageToExcelJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1273,14 +1249,207 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SubmitConvertImageToExcelJobResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SubmitConvertImageToMarkdownJobRequest(TeaModel):
+    def __init__(
+        self,
+        image_name_extension: str = None,
+        image_names: List[str] = None,
+        image_urls: List[str] = None,
+    ):
+        self.image_name_extension = image_name_extension
+        self.image_names = image_names
+        self.image_urls = image_urls
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image_name_extension is not None:
+            result['ImageNameExtension'] = self.image_name_extension
+        if self.image_names is not None:
+            result['ImageNames'] = self.image_names
+        if self.image_urls is not None:
+            result['ImageUrls'] = self.image_urls
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ImageNameExtension') is not None:
+            self.image_name_extension = m.get('ImageNameExtension')
+        if m.get('ImageNames') is not None:
+            self.image_names = m.get('ImageNames')
+        if m.get('ImageUrls') is not None:
+            self.image_urls = m.get('ImageUrls')
+        return self
+
+
+class SubmitConvertImageToMarkdownJobShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        image_name_extension: str = None,
+        image_names_shrink: str = None,
+        image_urls_shrink: str = None,
+    ):
+        self.image_name_extension = image_name_extension
+        self.image_names_shrink = image_names_shrink
+        self.image_urls_shrink = image_urls_shrink
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image_name_extension is not None:
+            result['ImageNameExtension'] = self.image_name_extension
+        if self.image_names_shrink is not None:
+            result['ImageNames'] = self.image_names_shrink
+        if self.image_urls_shrink is not None:
+            result['ImageUrls'] = self.image_urls_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ImageNameExtension') is not None:
+            self.image_name_extension = m.get('ImageNameExtension')
+        if m.get('ImageNames') is not None:
+            self.image_names_shrink = m.get('ImageNames')
+        if m.get('ImageUrls') is not None:
+            self.image_urls_shrink = m.get('ImageUrls')
+        return self
+
+
+class SubmitConvertImageToMarkdownJobResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        id: str = None,
+    ):
+        self.id = id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        return self
+
+
+class SubmitConvertImageToMarkdownJobResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: SubmitConvertImageToMarkdownJobResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = SubmitConvertImageToMarkdownJobResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SubmitConvertImageToMarkdownJobResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SubmitConvertImageToMarkdownJobResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SubmitConvertImageToMarkdownJobResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SubmitConvertImageToPdfJobRequest(TeaModel):
     def __init__(
         self,
         image_name_extension: str = None,
         image_names: List[str] = None,
         image_urls: List[str] = None,
     ):
@@ -1437,17 +1606,14 @@
         body: SubmitConvertImageToPdfJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1633,17 +1799,14 @@
         body: SubmitConvertImageToWordJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1841,17 +2004,14 @@
         body: SubmitConvertPdfToExcelJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2025,17 +2185,14 @@
         body: SubmitConvertPdfToImageJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2057,14 +2214,195 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SubmitConvertPdfToImageJobResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SubmitConvertPdfToMarkdownJobRequest(TeaModel):
+    def __init__(
+        self,
+        file_name: str = None,
+        file_url: str = None,
+    ):
+        self.file_name = file_name
+        self.file_url = file_url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.file_name is not None:
+            result['FileName'] = self.file_name
+        if self.file_url is not None:
+            result['FileUrl'] = self.file_url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FileName') is not None:
+            self.file_name = m.get('FileName')
+        if m.get('FileUrl') is not None:
+            self.file_url = m.get('FileUrl')
+        return self
+
+
+class SubmitConvertPdfToMarkdownJobAdvanceRequest(TeaModel):
+    def __init__(
+        self,
+        file_name: str = None,
+        file_url_object: BinaryIO = None,
+    ):
+        self.file_name = file_name
+        self.file_url_object = file_url_object
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.file_name is not None:
+            result['FileName'] = self.file_name
+        if self.file_url_object is not None:
+            result['FileUrl'] = self.file_url_object
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FileName') is not None:
+            self.file_name = m.get('FileName')
+        if m.get('FileUrl') is not None:
+            self.file_url_object = m.get('FileUrl')
+        return self
+
+
+class SubmitConvertPdfToMarkdownJobResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        id: str = None,
+    ):
+        self.id = id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        return self
+
+
+class SubmitConvertPdfToMarkdownJobResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: SubmitConvertPdfToMarkdownJobResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = SubmitConvertPdfToMarkdownJobResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SubmitConvertPdfToMarkdownJobResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SubmitConvertPdfToMarkdownJobResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SubmitConvertPdfToMarkdownJobResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SubmitConvertPdfToWordJobRequest(TeaModel):
     def __init__(
         self,
         file_name: str = None,
         file_url: str = None,
         force_export_inner_image: bool = None,
     ):
@@ -2221,17 +2559,14 @@
         body: SubmitConvertPdfToWordJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2424,17 +2759,14 @@
         body: SubmitDigitalDocStructureJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2462,19 +2794,21 @@
 
 class SubmitDocStructureJobRequest(TeaModel):
     def __init__(
         self,
         file_name: str = None,
         file_name_extension: str = None,
         file_url: str = None,
+        formula_enhancement: bool = None,
         structure_type: str = None,
     ):
         self.file_name = file_name
         self.file_name_extension = file_name_extension
         self.file_url = file_url
+        self.formula_enhancement = formula_enhancement
         self.structure_type = structure_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2484,42 +2818,48 @@
         result = dict()
         if self.file_name is not None:
             result['FileName'] = self.file_name
         if self.file_name_extension is not None:
             result['FileNameExtension'] = self.file_name_extension
         if self.file_url is not None:
             result['FileUrl'] = self.file_url
+        if self.formula_enhancement is not None:
+            result['FormulaEnhancement'] = self.formula_enhancement
         if self.structure_type is not None:
             result['StructureType'] = self.structure_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('FileName') is not None:
             self.file_name = m.get('FileName')
         if m.get('FileNameExtension') is not None:
             self.file_name_extension = m.get('FileNameExtension')
         if m.get('FileUrl') is not None:
             self.file_url = m.get('FileUrl')
+        if m.get('FormulaEnhancement') is not None:
+            self.formula_enhancement = m.get('FormulaEnhancement')
         if m.get('StructureType') is not None:
             self.structure_type = m.get('StructureType')
         return self
 
 
 class SubmitDocStructureJobAdvanceRequest(TeaModel):
     def __init__(
         self,
         file_name: str = None,
         file_name_extension: str = None,
         file_url_object: BinaryIO = None,
+        formula_enhancement: bool = None,
         structure_type: str = None,
     ):
         self.file_name = file_name
         self.file_name_extension = file_name_extension
         self.file_url_object = file_url_object
+        self.formula_enhancement = formula_enhancement
         self.structure_type = structure_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2529,26 +2869,30 @@
         result = dict()
         if self.file_name is not None:
             result['FileName'] = self.file_name
         if self.file_name_extension is not None:
             result['FileNameExtension'] = self.file_name_extension
         if self.file_url_object is not None:
             result['FileUrl'] = self.file_url_object
+        if self.formula_enhancement is not None:
+            result['FormulaEnhancement'] = self.formula_enhancement
         if self.structure_type is not None:
             result['StructureType'] = self.structure_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('FileName') is not None:
             self.file_name = m.get('FileName')
         if m.get('FileNameExtension') is not None:
             self.file_name_extension = m.get('FileNameExtension')
         if m.get('FileUrl') is not None:
             self.file_url_object = m.get('FileUrl')
+        if m.get('FormulaEnhancement') is not None:
+            self.formula_enhancement = m.get('FormulaEnhancement')
         if m.get('StructureType') is not None:
             self.structure_type = m.get('StructureType')
         return self
 
 
 class SubmitDocStructureJobResponseBodyData(TeaModel):
     def __init__(
@@ -2632,17 +2976,14 @@
         body: SubmitDocStructureJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2795,17 +3136,14 @@
         body: SubmitDocumentCompareJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2991,17 +3329,14 @@
         body: SubmitDocumentExtractJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3187,17 +3522,14 @@
         body: SubmitTableUnderstandingJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_docmind-api20220711-1.2.1/alibabacloud_docmind_api20220711.egg-info/PKG-INFO` & `alibabacloud_docmind-api20220711-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-docmind-api20220711
-Version: 1.2.1
+Name: alibabacloud_docmind-api20220711
+Version: 1.3.0
 Summary: Alibaba Cloud docmind-api (20220711) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docmind-api-20220711/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_docmind-api20220711-1.2.1/setup.py` & `alibabacloud_docmind-api20220711-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_docmind-api20220711.
 
-Created on 09/01/2024
+Created on 09/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_docmind_api20220711"
 NAME = "alibabacloud_docmind-api20220711" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud docmind-api (20220711) SDK Library for Python"
```

