# Comparing `tmp/cirro-1.0.1.tar.gz` & `tmp/cirro-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirro-1.0.1.tar", max compression
+gzip compressed data, was "cirro-1.1.1.tar", max compression
```

## Comparing `cirro-1.0.1.tar` & `cirro-1.1.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0     1066 2024-03-01 17:22:37.598573 cirro-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     5971 2024-03-01 17:22:37.598573 cirro-1.0.1/README.md
--rw-r--r--   0        0        0      476 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/__init__.py
--rw-r--r--   0        0        0     1486 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/auth/__init__.py
--rw-r--r--   0        0        0      308 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/auth/base.py
--rw-r--r--   0        0        0     6940 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/auth/device_code.py
--rw-r--r--   0        0        0      432 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/auth/oauth_models.py
--rw-r--r--   0        0        0     3995 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cirro_client.py
--rw-r--r--   0        0        0      190 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/__init__.py
--rw-r--r--   0        0        0     2374 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/cli.py
--rw-r--r--   0        0        0     6568 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/controller.py
--rw-r--r--   0        0        0        0 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/interactive/__init__.py
--rw-r--r--   0        0        0      563 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/interactive/auth_args.py
--rw-r--r--   0        0        0      773 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/interactive/common_args.py
--rw-r--r--   0        0        0     5229 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/interactive/download_args.py
--rw-r--r--   0        0        0      576 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/interactive/list_dataset_args.py
--rw-r--r--   0        0        0     5945 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/interactive/upload_args.py
--rw-r--r--   0        0        0     2557 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/interactive/utils.py
--rw-r--r--   0        0        0      418 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/cli/models.py
--rw-r--r--   0        0        0       68 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/clients/__init__.py
--rw-r--r--   0        0        0     4456 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/clients/s3.py
--rw-r--r--   0        0        0     3833 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/config.py
--rw-r--r--   0        0        0     4033 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/file_utils.py
--rw-r--r--   0        0        0      164 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/helpers/__init__.py
--rw-r--r--   0        0        0     1708 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/helpers/constants.py
--rw-r--r--   0        0        0     5202 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/helpers/form.py
--rw-r--r--   0        0        0     5922 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/helpers/preprocess_dataset.py
--rw-r--r--   0        0        0        0 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/models/__init__.py
--rw-r--r--   0        0        0     3567 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/models/file.py
--rw-r--r--   0        0        0     2607 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/models/form_specification.py
--rw-r--r--   0        0        0      502 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/models/s3_path.py
--rw-r--r--   0        0        0        0 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/sdk/__init__.py
--rw-r--r--   0        0        0     2993 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/sdk/asset.py
--rw-r--r--   0        0        0     7080 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/sdk/dataset.py
--rw-r--r--   0        0        0      245 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/sdk/exceptions.py
--rw-r--r--   0        0        0     5496 2024-03-01 17:22:37.598573 cirro-1.0.1/cirro/sdk/file.py
--rw-r--r--   0        0        0     1536 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/sdk/helpers.py
--rw-r--r--   0        0        0     4111 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/sdk/portal.py
--rw-r--r--   0        0        0     2230 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/sdk/process.py
--rw-r--r--   0        0        0     7733 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/sdk/project.py
--rw-r--r--   0        0        0     1823 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/sdk/reference.py
--rw-r--r--   0        0        0     1188 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/sdk/reference_type.py
--rw-r--r--   0        0        0      544 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/__init__.py
--rw-r--r--   0        0        0      981 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/base.py
--rw-r--r--   0        0        0     1417 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/billing.py
--rw-r--r--   0        0        0     7475 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/dataset.py
--rw-r--r--   0        0        0     4680 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/execution.py
--rw-r--r--   0        0        0     6282 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/file.py
--rw-r--r--   0        0        0     2412 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/metadata.py
--rw-r--r--   0        0        0      608 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/metrics.py
--rw-r--r--   0        0        0     3754 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/process.py
--rw-r--r--   0        0        0     3826 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/projects.py
--rw-r--r--   0        0        0      789 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/services/references.py
--rw-r--r--   0        0        0     1514 2024-03-01 17:22:37.602573 cirro-1.0.1/cirro/utils.py
--rw-r--r--   0        0        0      924 2024-03-01 17:22:37.602573 cirro-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7112 1970-01-01 00:00:00.000000 cirro-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-09 20:28:42.450644 cirro-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     6113 2024-05-09 20:28:42.450644 cirro-1.1.1/README.md
+-rw-r--r--   0        0        0      476 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/__init__.py
+-rw-r--r--   0        0        0     1486 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/auth/__init__.py
+-rw-r--r--   0        0        0      308 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/auth/base.py
+-rw-r--r--   0        0        0     6983 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/auth/device_code.py
+-rw-r--r--   0        0        0      432 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/auth/oauth_models.py
+-rw-r--r--   0        0        0     4246 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cirro_client.py
+-rw-r--r--   0        0        0      190 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/__init__.py
+-rw-r--r--   0        0        0     2538 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/cli.py
+-rw-r--r--   0        0        0     6694 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/controller.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/__init__.py
+-rw-r--r--   0        0        0     1277 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/auth_args.py
+-rw-r--r--   0        0        0      773 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/common_args.py
+-rw-r--r--   0        0        0     5229 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/download_args.py
+-rw-r--r--   0        0        0      576 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/list_dataset_args.py
+-rw-r--r--   0        0        0     5672 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/upload_args.py
+-rw-r--r--   0        0        0     2557 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/utils.py
+-rw-r--r--   0        0        0      443 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/models.py
+-rw-r--r--   0        0        0       68 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/clients/__init__.py
+-rw-r--r--   0        0        0     4456 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/clients/s3.py
+-rw-r--r--   0        0        0     4335 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/config.py
+-rw-r--r--   0        0        0     4033 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/file_utils.py
+-rw-r--r--   0        0        0      164 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/helpers/__init__.py
+-rw-r--r--   0        0        0     1708 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/helpers/constants.py
+-rw-r--r--   0        0        0     5202 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/helpers/form.py
+-rw-r--r--   0        0        0     5922 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/helpers/preprocess_dataset.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/__init__.py
+-rw-r--r--   0        0        0     3567 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/file.py
+-rw-r--r--   0        0        0     2607 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/form_specification.py
+-rw-r--r--   0        0        0      502 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/s3_path.py
+-rw-r--r--   0        0        0      110 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/tenant.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/__init__.py
+-rw-r--r--   0        0        0     2993 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/asset.py
+-rw-r--r--   0        0        0     7080 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/dataset.py
+-rw-r--r--   0        0        0      245 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/exceptions.py
+-rw-r--r--   0        0        0     5496 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/file.py
+-rw-r--r--   0        0        0     1536 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/helpers.py
+-rw-r--r--   0        0        0     4607 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/portal.py
+-rw-r--r--   0        0        0     2230 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/process.py
+-rw-r--r--   0        0        0     7733 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/project.py
+-rw-r--r--   0        0        0     1823 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/reference.py
+-rw-r--r--   0        0        0     1188 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/reference_type.py
+-rw-r--r--   0        0        0      544 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/services/__init__.py
+-rw-r--r--   0        0        0      981 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/services/base.py
+-rw-r--r--   0        0        0     1417 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/billing.py
+-rw-r--r--   0        0        0     7475 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/dataset.py
+-rw-r--r--   0        0        0     4680 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/execution.py
+-rw-r--r--   0        0        0     6282 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/file.py
+-rw-r--r--   0        0        0     2412 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/metadata.py
+-rw-r--r--   0        0        0      831 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/metrics.py
+-rw-r--r--   0        0        0     3754 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/process.py
+-rw-r--r--   0        0        0     5572 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/projects.py
+-rw-r--r--   0        0        0      789 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/references.py
+-rw-r--r--   0        0        0     1514 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/utils.py
+-rw-r--r--   0        0        0      925 2024-05-09 20:28:42.454645 cirro-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7255 1970-01-01 00:00:00.000000 cirro-1.1.1/PKG-INFO
```

### Comparing `cirro-1.0.1/LICENSE.txt` & `cirro-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/README.md` & `cirro-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 or you can install the main branch of the repo by running:
 
 `pip install git+https://github.com/CirroBio/Cirro-client.git`
 
 ## Authentication
 
-Upon first use, the Cirro client will ask if you would like to save your login information and give you a link to authenticate through the web browser.
+Upon first use, the Cirro client will ask you what Cirro instance to use and if you would like to save your login information.
+It will then give you a link to authenticate through the web browser.
+
+You can change your Cirro instance by running `cirro configure` and selecting the desired instance.
 
 If you need to change your credentials after this point, and you've opted to save your login, please see the [clearing saved login](#clearing-saved-login) section.
 
 ## Command Line Usage
 
 #### Downloading a dataset:
 ```bash
@@ -105,18 +108,18 @@
 
 ## Advanced Usage
 
 View the API documentation for this library [here](https://cirrobio.github.io/Cirro-client/).
 
 ### Supported environment variables
 
-| Name           | Description                   | Default   |
-|----------------|-------------------------------|-----------|
-| CIRRO_HOME     | Local configuration directory | ~/.cirro  |
-| CIRRO_BASE_URL | Base URL of the data portal   | cirro.bio |
+| Name           | Description                   | Default  |
+|----------------|-------------------------------|----------|
+| CIRRO_HOME     | Local configuration directory | ~/.cirro |
+| CIRRO_BASE_URL | Base URL of the data portal   |          |
 
 ### Configuration
 
 The `cirro configure` command creates a file in `CIRRO_HOME` called `config.ini`.
 
 You can set the `base_url` property in the config file rather than using the environment variable.
```

### Comparing `cirro-1.0.1/cirro/auth/__init__.py` & `cirro-1.1.1/cirro/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/auth/device_code.py` & `cirro-1.1.1/cirro/auth/device_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 from msal_extensions.persistence import BasePersistence
 
 from cirro.auth.base import AuthInfo
 from cirro.auth.oauth_models import DeviceTokenResponse, OAuthTokenResponse
 from cirro.config import Constants
 
 logger = logging.getLogger()
-TOKEN_PATH = Path(Constants.home, '.token.dat').expanduser()
 
 
-def _build_token_persistence(location, fallback_to_plaintext=False):
+def _build_token_persistence(location: str, fallback_to_plaintext=False):
     try:
         if sys.platform.startswith('win'):
             from msal_extensions import FilePersistenceWithDataProtection
             return FilePersistenceWithDataProtection(location)
         if sys.platform.startswith('darwin'):
             from msal_extensions import KeychainPersistence
             return KeychainPersistence(location, service_name='cirro-client')
@@ -95,17 +94,18 @@
         enable_cache=False,
         auth_io: Optional[StringIO] = None
     ):
         self.client_id = client_id
         self.region = region
         self._token_info: Optional[OAuthTokenResponse] = None
         self._persistence: Optional[BasePersistence] = None
+        self._token_path = Path(Constants.home, f'{client_id}.token.dat').expanduser()
 
         if enable_cache:
-            self._persistence = _build_token_persistence(str(TOKEN_PATH), fallback_to_plaintext=True)
+            self._persistence = _build_token_persistence(str(self._token_path), fallback_to_plaintext=True)
             self._token_info = self._load_token_info()
 
         # Check saved token for change in endpoint
         if self._token_info and self._token_info.get('client_id') != client_id:
             logger.debug('Different client ID found, clearing saved token info')
             self._clear_token_info()
 
@@ -163,15 +163,15 @@
     def _update_token_metadata(self):
         decoded_access_token = jwt.decode(self._token_info['access_token'],
                                           options={"verify_signature": False})
         self.access_token_expiry = datetime.fromtimestamp(decoded_access_token['exp'])
         self._username = decoded_access_token['username']
 
     def _load_token_info(self) -> Optional[OAuthTokenResponse]:
-        if not self._persistence or not TOKEN_PATH.exists():
+        if not self._persistence or not self._token_path.exists():
             return None
 
         token_info = json.loads(self._persistence.load())
         if 'access_token' not in token_info:
             return None
 
         return token_info
```

### Comparing `cirro-1.0.1/cirro/cirro_client.py` & `cirro-1.1.1/cirro/cirro_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,25 @@
     """
     def __init__(self, auth_info: AuthInfo = None, base_url: str = None):
         """
         Instantiates the Cirro API object
 
         Args:
             auth_info (cirro.auth.base.AuthInfo):
-            base_url (str): Optional base URL for connection (default: `CIRRO_HOME` or 'cirro.bio')
+            base_url (str): Optional base URL of the Cirro instance
+             (if not provided, it uses the `CIRRO_BASE_URL` environment variable, or the config file)
 
         Returns:
-            Authenticated Cirro API object which can be used to call endpoint functions.
-            For example:
+            Authenticated Cirro API object, which can be used to call endpoint functions.
 
+        Example:
         ```python
         from cirro.cirro_client import CirroApi
-        cirro = CirroApi()
+
+        cirro = CirroApi(base_url="app.cirro.bio")
         print(cirro.projects.list())
         ```
         """
 
         self._configuration = AppConfig(base_url=base_url)
         if not auth_info:
             auth_info = get_auth_info_from_config(self._configuration, auth_io=None)
@@ -119,7 +121,14 @@
 
     @property
     def api_client(self) -> CirroApiClient:
         """
         Gets the underlying API client
         """
         return self._api_client
+
+    @property
+    def configuration(self) -> AppConfig:
+        """
+        Gets the configuration of the instance
+        """
+        return self._configuration
```

### Comparing `cirro-1.0.1/cirro/cli/cli.py` & `cirro-1.1.1/cirro/cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 @click.option('--process',
               help='Name or ID of the ingest process')
 @click.option('--data-directory',
               help='Directory you wish to upload')
 @click.option('-i', '--interactive',
               help='Gather arguments interactively',
               is_flag=True, default=False)
+@click.option('--include-hidden',
+              help='Include hidden files in the upload (e.g., files starting with .)',
+              is_flag=True, default=False)
 def upload(**kwargs):
     check_required_args(kwargs)
     run_ingest(kwargs, interactive=kwargs.get('interactive'))
 
 
 @run.command(help='Configure authentication')
 def configure():
```

### Comparing `cirro-1.0.1/cirro/cli/controller.py` & `cirro-1.1.1/cirro/cli/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 def run_list_datasets(input_params: ListArguments, interactive=False):
     """List the datasets available in a particular project."""
     _check_configure()
     cirro = CirroApi()
     logger = _get_logger()
-    logger.info(f"Collecting data from {cirro._configuration.base_url}")
+    logger.info(f"Collecting data from {cirro.configuration.base_url}")
 
     # If the user provided the --interactive flag
     if interactive:
 
         # Get the list of projects available to the user
         projects = cirro.projects.list()
 
@@ -46,15 +46,15 @@
     print(df.to_string())
 
 
 def run_ingest(input_params: UploadArguments, interactive=False):
     _check_configure()
     cirro = CirroApi()
     logger = _get_logger()
-    logger.info(f"Collecting data from {cirro._configuration.base_url}")
+    logger.info(f"Collecting data from {cirro.configuration.base_url}")
     processes = cirro.processes.list(process_type=Executor.INGEST)
 
     logger.info("Listing available projects")
     projects = cirro.projects.list()
 
     if len(projects) == 0:
         logger.warning(NO_PROJECTS)
@@ -88,26 +88,26 @@
 
     logger.info("Uploading files")
     cirro.datasets.upload_files(project_id=project_id,
                                 dataset_id=create_resp.id,
                                 local_directory=directory,
                                 files=files)
 
-    if cirro._configuration.enable_additional_checksum:
+    if cirro.configuration.enable_additional_checksum:
         checksum_method = "SHA256"
     else:
         checksum_method = "MD5"
     logger.info(f"File content validated by {checksum_method}")
 
 
 def run_download(input_params: DownloadArguments, interactive=False):
     _check_configure()
     cirro = CirroApi()
     logger = _get_logger()
-    logger.info(f"Collecting data from {cirro._configuration.base_url}")
+    logger.info(f"Collecting data from {cirro.configuration.base_url}")
 
     logger.info("Listing available projects")
     projects = cirro.projects.list()
 
     if len(projects) == 0:
         logger.warning(NO_PROJECTS)
         return
@@ -126,45 +126,49 @@
         if len(files) == 0:
             logger.info('There are no files in this dataset')
             return
 
         files_to_download = ask_dataset_files(files)
 
     logger.info("Downloading files")
-    if cirro._configuration.enable_additional_checksum:
+    if cirro.configuration.enable_additional_checksum:
         checksum_method = "SHA256"
     else:
         checksum_method = "MD5"
     logger.info(f"File content validated by {checksum_method}")
 
     project_id = get_id_from_name(projects, input_params['project'])
     dataset_id = input_params['dataset']
     cirro.datasets.download_files(project_id=project_id,
                                   dataset_id=dataset_id,
                                   download_location=input_params['data_directory'],
                                   files=files_to_download)
 
 
 def run_configure():
-    auth_method, auth_method_config, enable_additional_checksum = gather_auth_config()
+    auth_method, base_url, auth_method_config, enable_additional_checksum = gather_auth_config()
     save_user_config(UserConfig(auth_method=auth_method,
                                 auth_method_config=auth_method_config,
-                                base_url=None,
+                                base_url=base_url,
                                 transfer_max_retries=None,
                                 enable_additional_checksum=enable_additional_checksum))
 
 
 def _check_configure():
     """
     Prompts the user to do initial configuration if needed
     """
-    if load_user_config() is not None:
+    config = load_user_config()
+    if config is None:
+        run_configure()
         return
 
-    run_configure()
+    # Legacy check for old config
+    if config.base_url == 'cirro.bio':
+        run_configure()
 
 
 def _get_logger() -> logging.Logger:
     # Log to STDOUT
     log_formatter = logging.Formatter(
         '%(asctime)s %(levelname)-8s [Cirro CLI] %(message)s'
     )
```

### Comparing `cirro-1.0.1/cirro/cli/interactive/common_args.py` & `cirro-1.1.1/cirro/cli/interactive/common_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/cli/interactive/download_args.py` & `cirro-1.1.1/cirro/cli/interactive/download_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/cli/interactive/list_dataset_args.py` & `cirro-1.1.1/cirro/cli/interactive/list_dataset_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/cli/interactive/upload_args.py` & `cirro-1.1.1/cirro/cli/interactive/upload_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,28 +84,15 @@
         'What type of files?',
         default=input_value if input_value in process_names else None,
         choices=process_names,
         use_shortcuts=len(process_names) < 30
     )
 
 
-def ask_include_hidden() -> bool:
-    return prompt_wrapper({
-        'type': 'confirm',
-        'message': "Include hidden files (expert: e.g. Zarr)",
-        'name': 'include_hidden',
-        'default': False
-    })['include_hidden']
-
-
-def ask_files_in_directory(data_directory) -> List[str]:
-
-    # Ask whether hidden files should be included
-    include_hidden = ask_include_hidden()
-
+def ask_files_in_directory(data_directory: str, include_hidden: bool) -> List[str]:
     # Get the list of all files in the directory
     # (relative to the data_directory)
     files = get_files_in_directory(
         data_directory,
         include_hidden=include_hidden
     )
 
@@ -184,15 +171,15 @@
     return selected_files
 
 
 def gather_upload_arguments(input_params: UploadArguments, projects: List[Project], processes: List[Process]):
     input_params['project'] = ask_project(projects, input_params.get('project'))
 
     input_params['data_directory'] = ask_data_directory(input_params.get('data_directory'))
-    files = ask_files_in_directory(input_params['data_directory'])
+    files = ask_files_in_directory(input_params['data_directory'], input_params['include_hidden'])
 
     confirm_data_files(input_params['data_directory'], files)
 
     input_params['process'] = ask_process(processes, input_params.get('process'))
 
     data_directory_name = Path(input_params['data_directory']).name
     default_name = input_params.get('name') or data_directory_name
```

### Comparing `cirro-1.0.1/cirro/cli/interactive/utils.py` & `cirro-1.1.1/cirro/cli/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/clients/s3.py` & `cirro-1.1.1/cirro/clients/s3.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/config.py` & `cirro-1.1.1/cirro/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import configparser
 import os
+import re
 from pathlib import Path
-from typing import NamedTuple, Dict, Optional
+from typing import NamedTuple, Dict, Optional, List
 
 import requests
-from requests import HTTPError
+from requests import RequestException
+
+from cirro.models.tenant import Tenant
 
 
 class Constants:
     home = os.environ.get('CIRRO_HOME', '~/.cirro')
     config_path = Path(home, 'config.ini').expanduser()
     default_base_url = 'cirro.bio'
     default_max_retries = 10
@@ -18,24 +21,29 @@
     auth_method: str
     auth_method_config: Dict  # This needs to match the init params of the auth method
     base_url: Optional[str]
     transfer_max_retries: Optional[int]
     enable_additional_checksum: Optional[bool]
 
 
+def list_tenants() -> List[Tenant]:
+    resp = requests.get(f'https://nexus.{Constants.default_base_url}/info')
+    resp.raise_for_status()
+    return resp.json()['tenants']
+
+
 def save_user_config(user_config: UserConfig):
     original_user_config = load_user_config()
     ini_config = configparser.ConfigParser()
     ini_config['General'] = {
         'auth_method': user_config.auth_method,
-        'base_url': Constants.default_base_url,
+        'base_url': user_config.base_url,
         'transfer_max_retries': Constants.default_max_retries
     }
     if original_user_config:
-        ini_config['General']['base_url'] = original_user_config.base_url
         ini_config['General']['transfer_max_retries'] = str(original_user_config.transfer_max_retries)
 
     ini_config[user_config.auth_method] = user_config.auth_method_config
     Constants.config_path.parent.mkdir(exist_ok=True)
     with Constants.config_path.open('w') as configfile:
         ini_config.write(configfile)
 
@@ -70,31 +78,35 @@
 
 
 class AppConfig:
     def __init__(self, base_url: str = None):
         self.user_config = load_user_config()
         self.base_url = (base_url or
                          os.environ.get('CIRRO_BASE_URL') or
-                         (self.user_config.base_url if self.user_config else None) or
-                         Constants.default_base_url)
+                         (self.user_config.base_url if self.user_config else None))
+        if not self.base_url:
+            raise RuntimeError('No base URL provided, please run cirro configure,'
+                               ' set the CIRRO_BASE_URL environment variable, or provide the base_url parameter.')
+        # remove http(s):// if it's there
+        self.base_url = re.compile(r'https?://').sub('', self.base_url).strip()
         self.transfer_max_retries = self.user_config.transfer_max_retries\
             if self.user_config else Constants.default_max_retries
         self.enable_additional_checksum = self.user_config.enable_additional_checksum\
             if self.user_config else False
         self._init_config()
 
     def _init_config(self):
-        self.rest_endpoint = f'https://api.{self.base_url}'
-        self.auth_endpoint = f'https://api.{self.base_url}/auth'
+        self.rest_endpoint = f'https://{self.base_url}/api'
+        self.auth_endpoint = f'https://{self.base_url}/api/auth'
 
         try:
             info_resp = requests.get(f'{self.rest_endpoint}/info/system')
             info_resp.raise_for_status()
 
             info = info_resp.json()
             self.client_id = info['auth']['sdkAppId']
             self.user_pool_id = info['auth']['userPoolId']
             self.references_bucket = info['referencesBucket']
             self.resources_bucket = info['resourcesBucket']
             self.region = info['region']
-        except HTTPError:
-            raise RuntimeError('Failed to get system metadata')
+        except RequestException:
+            raise RuntimeError(f'Failed connecting to {self.base_url}, please check your configuration')
```

### Comparing `cirro-1.0.1/cirro/file_utils.py` & `cirro-1.1.1/cirro/file_utils.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/helpers/constants.py` & `cirro-1.1.1/cirro/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/helpers/form.py` & `cirro-1.1.1/cirro/helpers/form.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/helpers/preprocess_dataset.py` & `cirro-1.1.1/cirro/helpers/preprocess_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/models/file.py` & `cirro-1.1.1/cirro/models/file.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/models/form_specification.py` & `cirro-1.1.1/cirro/models/form_specification.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/sdk/asset.py` & `cirro-1.1.1/cirro/sdk/asset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/sdk/dataset.py` & `cirro-1.1.1/cirro/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/sdk/file.py` & `cirro-1.1.1/cirro/sdk/file.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/sdk/helpers.py` & `cirro-1.1.1/cirro/sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/sdk/portal.py` & `cirro-1.1.1/cirro/sdk/portal.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,38 @@
 
 class DataPortal:
     """
     Helper functions for exploring the Projects, Datasets, Samples, and Files
     available in the Data Portal.
     """
 
-    def __init__(self, client: CirroApi = None):
-        """Set up the DataPortal object, establishing an authenticated connection."""
+    def __init__(self, base_url: str = None, client: CirroApi = None):
+        """
+        Set up the DataPortal object, establishing an authenticated connection.
+
+        Args:
+            base_url (str): Optional base URL of the Cirro instance
+             (if not provided, it uses the `CIRRO_BASE_URL` environment variable, or the config file)
+            client (`cirro.cirro_client.CirroApi`): Optional pre-configured client
+
+        Example:
+        ```python
+        from cirro import DataPortal
+
+        Portal = DataPortal(base_url="app.cirro.bio")
+        portal.list_projects()
+        ```
+        """
 
         if client is not None:
             self._client = client
 
         # Set up default client if not provided
         else:
-            self._client = CirroApi()
+            self._client = CirroApi(base_url=base_url)
 
     def list_projects(self) -> DataPortalProjects:
         """List all the projects available in the Data Portal."""
 
         return DataPortalProjects(
             [
                 DataPortalProject(proj, self._client)
```

### Comparing `cirro-1.0.1/cirro/sdk/process.py` & `cirro-1.1.1/cirro/sdk/process.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/sdk/project.py` & `cirro-1.1.1/cirro/sdk/project.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/sdk/reference.py` & `cirro-1.1.1/cirro/sdk/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/sdk/reference_type.py` & `cirro-1.1.1/cirro/sdk/reference_type.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/services/__init__.py` & `cirro-1.1.1/cirro/services/__init__.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/services/base.py` & `cirro-1.1.1/cirro/services/base.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/services/billing.py` & `cirro-1.1.1/cirro/services/billing.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/services/dataset.py` & `cirro-1.1.1/cirro/services/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/services/execution.py` & `cirro-1.1.1/cirro/services/execution.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/services/file.py` & `cirro-1.1.1/cirro/services/file.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/services/metadata.py` & `cirro-1.1.1/cirro/services/metadata.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/services/process.py` & `cirro-1.1.1/cirro/services/process.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/services/references.py` & `cirro-1.1.1/cirro/services/references.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/cirro/utils.py` & `cirro-1.1.1/cirro/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-1.0.1/pyproject.toml` & `cirro-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "cirro"
-version = "1.0.1"
+version = "1.1.1"
 description = "CLI tool and SDK for interacting with the Cirro platform"
 authors = ["Cirro Bio <support@cirro.bio>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CirroBio/Cirro-client"
 packages = [{include = "cirro"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 attrs = ">=21.3.0"
-cirro_api_client = "0.0.9"
+cirro_api_client = "0.0.10"
 click = "^8.1.3"
 boto3 = "~=1.34"
 questionary = "^2.0.1"
 requests = "^2.31.0"
 tqdm = "^4.62.3"
 jsonschema = "^4.21.1"
 pandas = "^2.2.0"
```

### Comparing `cirro-1.0.1/PKG-INFO` & `cirro-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cirro
-Version: 1.0.1
+Version: 1.1.1
 Summary: CLI tool and SDK for interacting with the Cirro platform
 Home-page: https://github.com/CirroBio/Cirro-client
 License: MIT
 Author: Cirro Bio
 Author-email: support@cirro.bio
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=21.3.0)
 Requires-Dist: boto3 (>=1.34,<2.0)
-Requires-Dist: cirro_api_client (==0.0.9)
+Requires-Dist: cirro_api_client (==0.0.10)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
 Requires-Dist: msal-extensions (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
@@ -45,15 +45,18 @@
 
 or you can install the main branch of the repo by running:
 
 `pip install git+https://github.com/CirroBio/Cirro-client.git`
 
 ## Authentication
 
-Upon first use, the Cirro client will ask if you would like to save your login information and give you a link to authenticate through the web browser.
+Upon first use, the Cirro client will ask you what Cirro instance to use and if you would like to save your login information.
+It will then give you a link to authenticate through the web browser.
+
+You can change your Cirro instance by running `cirro configure` and selecting the desired instance.
 
 If you need to change your credentials after this point, and you've opted to save your login, please see the [clearing saved login](#clearing-saved-login) section.
 
 ## Command Line Usage
 
 #### Downloading a dataset:
 ```bash
@@ -135,18 +138,18 @@
 
 ## Advanced Usage
 
 View the API documentation for this library [here](https://cirrobio.github.io/Cirro-client/).
 
 ### Supported environment variables
 
-| Name           | Description                   | Default   |
-|----------------|-------------------------------|-----------|
-| CIRRO_HOME     | Local configuration directory | ~/.cirro  |
-| CIRRO_BASE_URL | Base URL of the data portal   | cirro.bio |
+| Name           | Description                   | Default  |
+|----------------|-------------------------------|----------|
+| CIRRO_HOME     | Local configuration directory | ~/.cirro |
+| CIRRO_BASE_URL | Base URL of the data portal   |          |
 
 ### Configuration
 
 The `cirro configure` command creates a file in `CIRRO_HOME` called `config.ini`.
 
 You can set the `base_url` property in the config file rather than using the environment variable.
```

