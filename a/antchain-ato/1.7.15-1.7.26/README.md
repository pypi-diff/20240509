# Comparing `tmp/antchain_ato-1.7.15.tar.gz` & `tmp/antchain_ato-1.7.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ato-1.7.15.tar", last modified: Tue Mar 26 03:58:56 2024, max compression
+gzip compressed data, was "dist/antchain_ato-1.7.26.tar", last modified: Thu May  9 03:45:48 2024, max compression
```

## Comparing `antchain_ato-1.7.15.tar` & `antchain_ato-1.7.26.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 03:58:56.000000 antchain_ato-1.7.15/
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2024-03-26 03:58:56.000000 antchain_ato-1.7.15/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 03:58:56.000000 antchain_ato-1.7.15/antchain_ato.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/antchain_ato.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2024-03-26 03:58:56.000000 antchain_ato-1.7.15/antchain_ato.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/antchain_ato.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/antchain_ato.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/antchain_ato.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 03:58:56.000000 antchain_ato-1.7.15/antchain_sdk_ato/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/antchain_sdk_ato/__init__.py
--rw-r--r--   0 root         (0) root         (0)   117374 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/antchain_sdk_ato/client.py
--rw-r--r--   0 root         (0) root         (0)   227265 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/antchain_sdk_ato/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-26 03:58:56.000000 antchain_ato-1.7.15/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2489 2024-03-26 03:58:55.000000 antchain_ato-1.7.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_sdk_ato/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/antchain_sdk_ato/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126392 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/antchain_sdk_ato/client.py
+-rw-r--r--   0 root         (0) root         (0)   247593 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/antchain_sdk_ato/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/setup.py
```

### Comparing `antchain_ato-1.7.15/LICENSE` & `antchain_ato-1.7.26/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ato-1.7.15/PKG-INFO` & `antchain_ato-1.7.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ato
-Version: 1.7.15
+Version: 1.7.26
 Summary: Ant Chain ATO SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ato-1.7.15/README-CN.md` & `antchain_ato-1.7.26/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ato-1.7.15/README.md` & `antchain_ato-1.7.26/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ato-1.7.15/antchain_ato.egg-info/PKG-INFO` & `antchain_ato-1.7.26/antchain_ato.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ato
-Version: 1.7.15
+Version: 1.7.26
 Summary: Ant Chain ATO SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ato-1.7.15/antchain_sdk_ato/client.py` & `antchain_ato-1.7.26/antchain_sdk_ato/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.7.15',
+                    'sdk_version': '1.7.26',
                     '_prod_code': 'ATO',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.7.15',
+                    'sdk_version': '1.7.26',
                     '_prod_code': 'ATO',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1257,14 +1257,238 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ato_models.GetFundOrderfullinfoResponse(),
             await self.do_request_async('1.0', 'antchain.ato.fund.orderfullinfo.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def get_inner_product(
+        self,
+        request: ato_models.GetInnerProductRequest,
+    ) -> ato_models.GetInnerProductResponse:
+        """
+        Description: 内部调用,商品信息获取
+        Summary: 商品信息获取
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_inner_product_ex(request, headers, runtime)
+
+    async def get_inner_product_async(
+        self,
+        request: ato_models.GetInnerProductRequest,
+    ) -> ato_models.GetInnerProductResponse:
+        """
+        Description: 内部调用,商品信息获取
+        Summary: 商品信息获取
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_inner_product_ex_async(request, headers, runtime)
+
+    def get_inner_product_ex(
+        self,
+        request: ato_models.GetInnerProductRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.GetInnerProductResponse:
+        """
+        Description: 内部调用,商品信息获取
+        Summary: 商品信息获取
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.GetInnerProductResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.product.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_inner_product_ex_async(
+        self,
+        request: ato_models.GetInnerProductRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.GetInnerProductResponse:
+        """
+        Description: 内部调用,商品信息获取
+        Summary: 商品信息获取
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.GetInnerProductResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.product.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_inner_tenant(
+        self,
+        request: ato_models.GetInnerTenantRequest,
+    ) -> ato_models.GetInnerTenantResponse:
+        """
+        Description: ato内部服务，客户系统不可访问；租户信息获取
+        Summary: 租户信息获取
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_inner_tenant_ex(request, headers, runtime)
+
+    async def get_inner_tenant_async(
+        self,
+        request: ato_models.GetInnerTenantRequest,
+    ) -> ato_models.GetInnerTenantResponse:
+        """
+        Description: ato内部服务，客户系统不可访问；租户信息获取
+        Summary: 租户信息获取
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_inner_tenant_ex_async(request, headers, runtime)
+
+    def get_inner_tenant_ex(
+        self,
+        request: ato_models.GetInnerTenantRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.GetInnerTenantResponse:
+        """
+        Description: ato内部服务，客户系统不可访问；租户信息获取
+        Summary: 租户信息获取
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.GetInnerTenantResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.tenant.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_inner_tenant_ex_async(
+        self,
+        request: ato_models.GetInnerTenantRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.GetInnerTenantResponse:
+        """
+        Description: ato内部服务，客户系统不可访问；租户信息获取
+        Summary: 租户信息获取
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.GetInnerTenantResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.tenant.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def sync_inner_meterforwholeorder(
+        self,
+        request: ato_models.SyncInnerMeterforwholeorderRequest,
+    ) -> ato_models.SyncInnerMeterforwholeorderResponse:
+        """
+        Description: 内部接口，客户系统不能调用。上报整单结算计量信息
+        Summary: 上报整单结算计量信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_inner_meterforwholeorder_ex(request, headers, runtime)
+
+    async def sync_inner_meterforwholeorder_async(
+        self,
+        request: ato_models.SyncInnerMeterforwholeorderRequest,
+    ) -> ato_models.SyncInnerMeterforwholeorderResponse:
+        """
+        Description: 内部接口，客户系统不能调用。上报整单结算计量信息
+        Summary: 上报整单结算计量信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_inner_meterforwholeorder_ex_async(request, headers, runtime)
+
+    def sync_inner_meterforwholeorder_ex(
+        self,
+        request: ato_models.SyncInnerMeterforwholeorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncInnerMeterforwholeorderResponse:
+        """
+        Description: 内部接口，客户系统不能调用。上报整单结算计量信息
+        Summary: 上报整单结算计量信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncInnerMeterforwholeorderResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.meterforwholeorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_inner_meterforwholeorder_ex_async(
+        self,
+        request: ato_models.SyncInnerMeterforwholeorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncInnerMeterforwholeorderResponse:
+        """
+        Description: 内部接口，客户系统不能调用。上报整单结算计量信息
+        Summary: 上报整单结算计量信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncInnerMeterforwholeorderResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.meterforwholeorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def sync_inner_meterforagsign(
+        self,
+        request: ato_models.SyncInnerMeterforagsignRequest,
+    ) -> ato_models.SyncInnerMeterforagsignResponse:
+        """
+        Description: 内部调用，合同签署计量上报接口
+        Summary: 合同签署计量上报同步接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_inner_meterforagsign_ex(request, headers, runtime)
+
+    async def sync_inner_meterforagsign_async(
+        self,
+        request: ato_models.SyncInnerMeterforagsignRequest,
+    ) -> ato_models.SyncInnerMeterforagsignResponse:
+        """
+        Description: 内部调用，合同签署计量上报接口
+        Summary: 合同签署计量上报同步接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_inner_meterforagsign_ex_async(request, headers, runtime)
+
+    def sync_inner_meterforagsign_ex(
+        self,
+        request: ato_models.SyncInnerMeterforagsignRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncInnerMeterforagsignResponse:
+        """
+        Description: 内部调用，合同签署计量上报接口
+        Summary: 合同签署计量上报同步接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncInnerMeterforagsignResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.meterforagsign.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_inner_meterforagsign_ex_async(
+        self,
+        request: ato_models.SyncInnerMeterforagsignRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncInnerMeterforagsignResponse:
+        """
+        Description: 内部调用，合同签署计量上报接口
+        Summary: 合同签署计量上报同步接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncInnerMeterforagsignResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.meterforagsign.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_realperson_facevrf(
         self,
         request: ato_models.CreateRealpersonFacevrfRequest,
     ) -> ato_models.CreateRealpersonFacevrfResponse:
         """
         Description: 可信身份认证，创建认证
         Summary: 创建认证
```

### Comparing `antchain_ato-1.7.15/antchain_sdk_ato/models.py` & `antchain_ato-1.7.26/antchain_sdk_ato/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -2452,14 +2452,527 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('response_data') is not None:
             self.response_data = m.get('response_data')
         return self
 
 
+class GetInnerProductRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        merchant_tenant_id: str = None,
+        merchant_id: str = None,
+        product_id: str = None,
+        product_version: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户在数科的租户id
+        self.merchant_tenant_id = merchant_tenant_id
+        # 商户统一社会信用代码
+        self.merchant_id = merchant_id
+        # 商品id
+        self.product_id = product_id
+        # 商品版本
+        self.product_version = product_version
+
+    def validate(self):
+        self.validate_required(self.merchant_tenant_id, 'merchant_tenant_id')
+        if self.merchant_tenant_id is not None:
+            self.validate_max_length(self.merchant_tenant_id, 'merchant_tenant_id', 32)
+        self.validate_required(self.merchant_id, 'merchant_id')
+        if self.merchant_id is not None:
+            self.validate_max_length(self.merchant_id, 'merchant_id', 199)
+        self.validate_required(self.product_id, 'product_id')
+        if self.product_id is not None:
+            self.validate_max_length(self.product_id, 'product_id', 32)
+        self.validate_required(self.product_version, 'product_version')
+        if self.product_version is not None:
+            self.validate_max_length(self.product_version, 'product_version', 10)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.merchant_tenant_id is not None:
+            result['merchant_tenant_id'] = self.merchant_tenant_id
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        if self.product_id is not None:
+            result['product_id'] = self.product_id
+        if self.product_version is not None:
+            result['product_version'] = self.product_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('merchant_tenant_id') is not None:
+            self.merchant_tenant_id = m.get('merchant_tenant_id')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        if m.get('product_id') is not None:
+            self.product_id = m.get('product_id')
+        if m.get('product_version') is not None:
+            self.product_version = m.get('product_version')
+        return self
+
+
+class GetInnerProductResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        response_data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # {}json字符串
+        self.response_data = response_data
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.response_data is not None:
+            result['response_data'] = self.response_data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('response_data') is not None:
+            self.response_data = m.get('response_data')
+        return self
+
+
+class GetInnerTenantRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        merchant_tenant_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户在数科的租户id
+        self.merchant_tenant_id = merchant_tenant_id
+
+    def validate(self):
+        self.validate_required(self.merchant_tenant_id, 'merchant_tenant_id')
+        if self.merchant_tenant_id is not None:
+            self.validate_max_length(self.merchant_tenant_id, 'merchant_tenant_id', 32)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.merchant_tenant_id is not None:
+            result['merchant_tenant_id'] = self.merchant_tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('merchant_tenant_id') is not None:
+            self.merchant_tenant_id = m.get('merchant_tenant_id')
+        return self
+
+
+class GetInnerTenantResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        response_data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # {}租户信息
+        self.response_data = response_data
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.response_data is not None:
+            result['response_data'] = self.response_data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('response_data') is not None:
+            self.response_data = m.get('response_data')
+        return self
+
+
+class SyncInnerMeterforwholeorderRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        merchant_tenant_id: str = None,
+        merchant_id: str = None,
+        meter_product_code: str = None,
+        order_id: str = None,
+        order_product_id: str = None,
+        order_product_version: str = None,
+        order_rent_term: int = None,
+        order_total_money: int = None,
+        sys_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户租户id
+        self.merchant_tenant_id = merchant_tenant_id
+        # 商户统一社会信用代码
+        self.merchant_id = merchant_id
+        # 商户购买的产品code
+        self.meter_product_code = meter_product_code
+        # 订单id
+        self.order_id = order_id
+        # 订单关联的商品id
+        self.order_product_id = order_product_id
+        # 商品的版本
+        self.order_product_version = order_product_version
+        # 订单总租期
+        self.order_rent_term = order_rent_term
+        # 订单总租金，单位为分
+        self.order_total_money = order_total_money
+        # 系统名称
+        self.sys_name = sys_name
+
+    def validate(self):
+        self.validate_required(self.merchant_tenant_id, 'merchant_tenant_id')
+        if self.merchant_tenant_id is not None:
+            self.validate_max_length(self.merchant_tenant_id, 'merchant_tenant_id', 32)
+        self.validate_required(self.merchant_id, 'merchant_id')
+        if self.merchant_id is not None:
+            self.validate_max_length(self.merchant_id, 'merchant_id', 199)
+        self.validate_required(self.meter_product_code, 'meter_product_code')
+        if self.meter_product_code is not None:
+            self.validate_max_length(self.meter_product_code, 'meter_product_code', 64)
+        self.validate_required(self.order_id, 'order_id')
+        if self.order_id is not None:
+            self.validate_max_length(self.order_id, 'order_id', 49)
+        self.validate_required(self.order_product_id, 'order_product_id')
+        if self.order_product_id is not None:
+            self.validate_max_length(self.order_product_id, 'order_product_id', 32)
+        self.validate_required(self.order_product_version, 'order_product_version')
+        if self.order_product_version is not None:
+            self.validate_max_length(self.order_product_version, 'order_product_version', 10)
+        self.validate_required(self.order_rent_term, 'order_rent_term')
+        if self.order_rent_term is not None:
+            self.validate_maximum(self.order_rent_term, 'order_rent_term', 200)
+            self.validate_minimum(self.order_rent_term, 'order_rent_term', 1)
+        self.validate_required(self.order_total_money, 'order_total_money')
+        self.validate_required(self.sys_name, 'sys_name')
+        if self.sys_name is not None:
+            self.validate_max_length(self.sys_name, 'sys_name', 32)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.merchant_tenant_id is not None:
+            result['merchant_tenant_id'] = self.merchant_tenant_id
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        if self.meter_product_code is not None:
+            result['meter_product_code'] = self.meter_product_code
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        if self.order_product_id is not None:
+            result['order_product_id'] = self.order_product_id
+        if self.order_product_version is not None:
+            result['order_product_version'] = self.order_product_version
+        if self.order_rent_term is not None:
+            result['order_rent_term'] = self.order_rent_term
+        if self.order_total_money is not None:
+            result['order_total_money'] = self.order_total_money
+        if self.sys_name is not None:
+            result['sys_name'] = self.sys_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('merchant_tenant_id') is not None:
+            self.merchant_tenant_id = m.get('merchant_tenant_id')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        if m.get('meter_product_code') is not None:
+            self.meter_product_code = m.get('meter_product_code')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        if m.get('order_product_id') is not None:
+            self.order_product_id = m.get('order_product_id')
+        if m.get('order_product_version') is not None:
+            self.order_product_version = m.get('order_product_version')
+        if m.get('order_rent_term') is not None:
+            self.order_rent_term = m.get('order_rent_term')
+        if m.get('order_total_money') is not None:
+            self.order_total_money = m.get('order_total_money')
+        if m.get('sys_name') is not None:
+            self.sys_name = m.get('sys_name')
+        return self
+
+
+class SyncInnerMeterforwholeorderResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class SyncInnerMeterforagsignRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        merchant_tenant_id: str = None,
+        merchant_id: str = None,
+        meter_product_code: str = None,
+        sys_name: str = None,
+        order_id: str = None,
+        sign_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户租户id
+        self.merchant_tenant_id = merchant_tenant_id
+        # 商户社会信用代码
+        self.merchant_id = merchant_id
+        # 计量上报Code
+        self.meter_product_code = meter_product_code
+        # 系统名字
+        self.sys_name = sys_name
+        # 订单id
+        self.order_id = order_id
+        # 合同编号
+        self.sign_no = sign_no
+
+    def validate(self):
+        self.validate_required(self.merchant_tenant_id, 'merchant_tenant_id')
+        if self.merchant_tenant_id is not None:
+            self.validate_max_length(self.merchant_tenant_id, 'merchant_tenant_id', 32)
+        self.validate_required(self.merchant_id, 'merchant_id')
+        if self.merchant_id is not None:
+            self.validate_max_length(self.merchant_id, 'merchant_id', 199)
+        self.validate_required(self.meter_product_code, 'meter_product_code')
+        if self.meter_product_code is not None:
+            self.validate_max_length(self.meter_product_code, 'meter_product_code', 64)
+        self.validate_required(self.sys_name, 'sys_name')
+        if self.sys_name is not None:
+            self.validate_max_length(self.sys_name, 'sys_name', 32)
+        self.validate_required(self.order_id, 'order_id')
+        if self.order_id is not None:
+            self.validate_max_length(self.order_id, 'order_id', 49)
+        self.validate_required(self.sign_no, 'sign_no')
+        if self.sign_no is not None:
+            self.validate_max_length(self.sign_no, 'sign_no', 64)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.merchant_tenant_id is not None:
+            result['merchant_tenant_id'] = self.merchant_tenant_id
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        if self.meter_product_code is not None:
+            result['meter_product_code'] = self.meter_product_code
+        if self.sys_name is not None:
+            result['sys_name'] = self.sys_name
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        if self.sign_no is not None:
+            result['sign_no'] = self.sign_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('merchant_tenant_id') is not None:
+            self.merchant_tenant_id = m.get('merchant_tenant_id')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        if m.get('meter_product_code') is not None:
+            self.meter_product_code = m.get('meter_product_code')
+        if m.get('sys_name') is not None:
+            self.sys_name = m.get('sys_name')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        if m.get('sign_no') is not None:
+            self.sign_no = m.get('sign_no')
+        return self
+
+
+class SyncInnerMeterforagsignResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
 class CreateRealpersonFacevrfRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         cert_name: str = None,
         cert_no: str = None,
@@ -3165,14 +3678,15 @@
         order_id: str = None,
         account_id: str = None,
         status: str = None,
         flow_id: str = None,
         doc_list: str = None,
         business_scene: str = None,
         alipay_user_id: str = None,
+        sign_info: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -3190,14 +3704,16 @@
         # 签署文件列表，参考：
         # _[{"fileItemNo":"10090801000001699892007791144960","agreementType":"COMMON","fileName":"xxx合同","fileSize":228530,"signAccountId":"fe2eb3814c4e49edba2bc012f790771f","fileId":"2c7684461a0f4d33bc02f6d77f7b3937","downloadUrl":"https://dev.oss-cn-shanghai.aliyuncs.com/ag/ord/xxx/16939683744483057_%E6%B5%8B%E8%AF%95%E6%A8%A1%E6%9D%BF%E4%B9%8B%E5%8D%8F%E8%AE%AE%E7%AD%BE%E7%BD%B2%E8%AF%81%E6%98%8E.pdf?Expires=1693971989&OSSAccessKeyId=LTAI5tR3hHiaXPAh8YsY9Dce&Signature=i%2FfAgDem33guI%2F0KjIFj24XZNCc%3D"}]_
         self.doc_list = doc_list
         # 业务场景，主要用于签署合同的标题描述
         self.business_scene = business_scene
         # 签署合同中的订单的uid。
         self.alipay_user_id = alipay_user_id
+        # 签署扩展信息，用于获取签署链接等。JSON格式字符串。
+        self.sign_info = sign_info
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -3222,14 +3738,16 @@
             result['flow_id'] = self.flow_id
         if self.doc_list is not None:
             result['doc_list'] = self.doc_list
         if self.business_scene is not None:
             result['business_scene'] = self.business_scene
         if self.alipay_user_id is not None:
             result['alipay_user_id'] = self.alipay_user_id
+        if self.sign_info is not None:
+            result['sign_info'] = self.sign_info
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -3248,14 +3766,16 @@
             self.flow_id = m.get('flow_id')
         if m.get('doc_list') is not None:
             self.doc_list = m.get('doc_list')
         if m.get('business_scene') is not None:
             self.business_scene = m.get('business_scene')
         if m.get('alipay_user_id') is not None:
             self.alipay_user_id = m.get('alipay_user_id')
+        if m.get('sign_info') is not None:
+            self.sign_info = m.get('sign_info')
         return self
 
 
 class AuthSignFlowRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -5698,14 +6218,16 @@
         # 1234=12.34元
         self.refund_money = refund_money
         # 退款原因
         self.refund_reason = refund_reason
 
     def validate(self):
         self.validate_required(self.order_id, 'order_id')
+        if self.order_id is not None:
+            self.validate_max_length(self.order_id, 'order_id', 128)
         self.validate_required(self.period_num, 'period_num')
         if self.period_num is not None:
             self.validate_minimum(self.period_num, 'period_num', 1)
         self.validate_required(self.refund_request_no, 'refund_request_no')
         if self.refund_request_no is not None:
             self.validate_max_length(self.refund_request_no, 'refund_request_no', 128)
         self.validate_required(self.refund_money, 'refund_money')
@@ -5836,14 +6358,16 @@
         # 针对用户履约的第几期进行退款申请
         self.period_num = period_num
         # 外部系统传入的退款请求号
         self.refund_request_no = refund_request_no
 
     def validate(self):
         self.validate_required(self.order_id, 'order_id')
+        if self.order_id is not None:
+            self.validate_max_length(self.order_id, 'order_id', 128)
         self.validate_required(self.period_num, 'period_num')
         if self.period_num is not None:
             self.validate_minimum(self.period_num, 'period_num', 1)
         self.validate_required(self.refund_request_no, 'refund_request_no')
         if self.refund_request_no is not None:
             self.validate_max_length(self.refund_request_no, 'refund_request_no', 128)
```

### Comparing `antchain_ato-1.7.15/setup.py` & `antchain_ato-1.7.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ato.
 
-Created on 26/03/2024
+Created on 09/05/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ato"
 NAME = "antchain_ato" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain ATO SDK Library for Python"
```

