# Comparing `tmp/visier-connector-0.9.8.tar.gz` & `tmp/visier-connector-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visier-connector-0.9.8.tar", last modified: Thu Jul 27 20:01:47 2023, max compression
+gzip compressed data, was "visier-connector-0.9.9.tar", last modified: Fri Aug 25 16:57:30 2023, max compression
```

## Comparing `visier-connector-0.9.8.tar` & `visier-connector-0.9.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.153149 visier-connector-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 20:01:35.000000 visier-connector-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28774 2023-07-27 20:01:47.153149 visier-connector-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-07-27 20:01:35.000000 visier-connector-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-27 20:01:35.000000 visier-connector-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:01:47.153149 visier-connector-0.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.149149 visier-connector-0.9.8/visier/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.149149 visier-connector-0.9.8/visier/api/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/direct_intake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.149149 visier-connector-0.9.8/visier/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.149149 visier-connector-0.9.8/visier_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28774 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 16:57:30.967841 visier-connector-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (999)    11357 2023-08-25 16:57:18.000000 visier-connector-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)    31688 2023-08-25 16:57:30.967841 visier-connector-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)    18425 2023-08-25 16:57:18.000000 visier-connector-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (999)      609 2023-08-25 16:57:18.000000 visier-connector-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-25 16:57:30.967841 visier-connector-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 16:57:30.963842 visier-connector-0.9.9/visier/
+-rw-r--r--   0 runner    (1001) docker     (999)      691 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 16:57:30.967841 visier-connector-0.9.9/visier/api/
+-rw-r--r--   0 runner    (1001) docker     (999)      853 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2315 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5018 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/api/direct_intake.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4009 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2061 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/api/query.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 16:57:30.967841 visier-connector-0.9.9/visier/connector/
+-rw-r--r--   0 runner    (1001) docker     (999)      862 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6963 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/connector/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2411 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/connector/callback.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1086 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9608 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/connector/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1371 2023-08-25 16:57:18.000000 visier-connector-0.9.9/visier/connector/table.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 16:57:30.967841 visier-connector-0.9.9/visier_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)    31688 2023-08-25 16:57:30.000000 visier-connector-0.9.9/visier_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      538 2023-08-25 16:57:30.000000 visier-connector-0.9.9/visier_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-25 16:57:30.000000 visier-connector-0.9.9/visier_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       46 2023-08-25 16:57:30.000000 visier-connector-0.9.9/visier_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-25 16:57:30.000000 visier-connector-0.9.9/visier_connector.egg-info/top_level.txt
```

### Comparing `visier-connector-0.9.8/LICENSE` & `visier-connector-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/PKG-INFO` & `visier-connector-0.9.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.8
+Version: 0.9.9
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,29 +213,28 @@
 ![linting](https://github.com/visier/connector-python/actions/workflows/pylint.yml/badge.svg) ![pypi publishing](https://github.com/visier/connector-python/actions/workflows/publish-to-test-pypi.yml/badge.svg)
 # Visier Python Connector
 Use the Visier Python Connector to query Visier People data.
 
 The connector enables Python developers to query Visier People data using Visier's SQL-like query language. 
 
 ## Prerequisites
-The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
+The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-based service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
-* A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
-* That user's password
+* Either an OAuth connector application registration in your Visier tenant or a username and password pair with API access capabilities.
 
 ## Authentication Environment
 As of version `0.9.8`, the Visier Python Connector supports two means of authentication:
 1. OAuth2.0: The connector supports the so called three-legged authentication flow. This means that authentication (and consent) have to be provided through the authorization server. In accordance with the OAuth2.0 protocol, no user credentials are provided directly to Visier. This is the preferred authentication method.
 1. Basic Authentication: This is a traditional authentication mechanism where Visier username and password are provided directly to Visier for authentication.
 
 In order to avoid passing authentication credentials in via command line arguments, Visier recommends that at least basic authentication credentials such as username and password are provided via environment variables. However, using a new function, `make_auth()`, the appropriate authentication configuration object will be created from `VISIER_`-prefixed environment variables, as outlined  below.
 
 ### OAuth2.0
-Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the OAuth2.0 authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
+The following list and example below illustrate the OAuth2.0 authentication parameters. These are also the environment and `dotenv` variables the `make_auth()` utility function will use when instantiating an authentication object.
 * `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant as well as to initiate the OAuth2.0 authentication process
 * `VISIER_APIKEY`: The API key granted by Visier
 * `VISIER_CLIENT_ID`: The identifier of the pre-registered application
 * `VISIER_REDIRECT_URI`: The URI the `authorize` call will ultimately redirect to upon a successful authorization code generation. By default, this will be `http://localhost:5000/oauth2/callback` however note that it must match the `redirect_uri` in the client application definition exactly. If the client application setting is different, it is essential that that exact value is provided to the connector.
 * `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations
 
 On Linux-like systems, with an X-display available, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
@@ -251,14 +250,17 @@
 ```
 
 Source this file in and the environment is ready for using the connector with OAuth2.0 authentication:
 ```sh
 $ source .env
 ```
 
+#### Callback URI
+The OAuth flow requires that the authorizing server can call back to the initiating client with an authorization code. In OAuth mode, the connector starts a transient web server that listens for an authorization code on http://localhost:5000/oauth2/callback. You can modify the URL by setting a different value for VISIER_REDIRECT_URI. The VISIER_DIRECT_URI value must exactly match the URI value in your Visier OAuth 2.0 client registration and must abide by Visier's callback URI rules, such as a limited set of permissible subnets.
+
 ### Basic Authentication
 Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the basic authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
 * `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant
 * `VISIER_USERNAME`: The user name with sufficient API capabilities
 * `VISIER_PASSWORD`: The password of that user
 * `VISIER_APIKEY`: The API key granted by Visier
 * `VISIER_VANITY`: The readable name of the customer organization
@@ -280,26 +282,84 @@
 ```
 
 Source this environment in and provide the password when prompted:
 ```sh
 $ source .env
 ```
 
+## Jupyter Notebooks
+Jupyter notebooks and lab are well-suited to run Visier connector code. However, some users may not find OS-level variables ideal. As of version `0.9.9`, the Visier Python connector supports [dotenv](https://pypi.org/project/python-dotenv/) to facilitate a more dynamic switching of Visier authentication parameters. If the file is called `.env`, the Python package `dotenv` attempts to load the file. If the file has a different name, you must provide that file name when loading the environment with `dotenv`.
+
+### Jupyter Basic Authentication Example
+Basic Authentication is the most practical means of authenticating against Visier for Jupyter notebooks.
+
+Create an environment file to store the authentication parameters.
+
+Example environment file:
+```
+VISIER_VANITY=customer-specific
+VISIER_HOST=https://customer-specific.api.visier.io
+VISIER_APIKEY=the-api-key-issued-by-visier
+VISIER_USERNAME=apiuser@example.com
+VISIER_PASSWORD=password-or-variable-reference
+```
+
+Create a basic authentication object as described in the following snippet:
+```python
+from dotenv import dotenv_values
+from visier.connector import VisierSession, make_auth
+from visier.api import QueryApiClient
+
+env_creds = dotenv_values()
+auth = make_auth(env_values=env_creds)
+
+with VisierSession(auth) as s:
+    query_client = QueryApiClient(s)
+    ...
+```
+
+### Jupyter OAuth 2.0 Example
+Note that OAuth authentication to Visier in Jupyter notebooks is only supported when the Jupyter server runs on your local computer, bound to `localhost`. Therefore, OAuth in Jupyter notebooks against Visier is only recommended for test and development uses.
+To authenticate with OAuth, you must first register an OAuth 2.0 client in Visier. Visier administrators can register OAuth clients.
+
+After the OAuth client is registered in Visier, create an environment file to store the authentication parameters.
+
+Example environment file:
+```
+VISIER_HOST=https://customer-specific.api.visier.io
+VISIER_CLIENT_ID=client-id-from-registration
+VISIER_APIKEY=the-api-key-issued-by-visier
+```
+
+Create an OAuth authentication object as described in the following snippet:
+```python
+from dotenv import dotenv_values
+from visier.connector import VisierSession, make_auth
+from visier.api import QueryApiClient
+
+env_creds = dotenv_values()
+auth = make_auth(env_values=env_creds)
+
+with VisierSession(auth) as s:
+    query_client = QueryApiClient(s)
+    ...
+```
+
 ## Connector Separation
-As of version `0.9.5`, the Python connector has separated the API calls from the `VisierSession` object. As a result of this change, the query execution methods on the `VisierSession` have been deprecated and will be subject to removal in a future release.
+As of version `0.9.5`, the Python connector separates API calls from the `VisierSession` object. As a result of this change, query execution methods on the `VisierSession` are deprecated and will be removed in a future release.
 
 The new way of invoking Visier public APIs through the Visier Python connector requires instantiating the appropriate API client and calling the methods defined on the client object. The following example, invokes the `analytic-objects` Model API to obtain the metadata for two analytic objects:
 ```python
     with VisierSession(auth) as session:
         model_client = ModelApiClient(session)
 
         objs = model_client.get_analytic_objects(["Requisition", "Employee_Exit"])
         print(objs.text)
 ```
-### Error handling
+### Error Handling
 By default, a failed API call will return `None` and information about the error is available on the client object. Using the example above, the last error in the event `objs` was `None` would be `model_client.last_error()`.
 
 It is however possible to force the API client to instead raise a `QueryExecutionException`. This is accomplished when instantiating the API client with the following parameter value `raise_on_error=True`. Using the example above, the `model_client` instantiation would look like this: `model_client = ModelApiClient(session, raise_on_error=True)`.
 
 # Examples
 ## Query API
 The Query API Client is used to make calls to Visier's Query APIs.
```

### Comparing `visier-connector-0.9.8/README.md` & `visier-connector-0.9.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 ![linting](https://github.com/visier/connector-python/actions/workflows/pylint.yml/badge.svg) ![pypi publishing](https://github.com/visier/connector-python/actions/workflows/publish-to-test-pypi.yml/badge.svg)
 # Visier Python Connector
 Use the Visier Python Connector to query Visier People data.
 
 The connector enables Python developers to query Visier People data using Visier's SQL-like query language. 
 
 ## Prerequisites
-The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
+The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-based service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
-* A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
-* That user's password
+* Either an OAuth connector application registration in your Visier tenant or a username and password pair with API access capabilities.
 
 ## Authentication Environment
 As of version `0.9.8`, the Visier Python Connector supports two means of authentication:
 1. OAuth2.0: The connector supports the so called three-legged authentication flow. This means that authentication (and consent) have to be provided through the authorization server. In accordance with the OAuth2.0 protocol, no user credentials are provided directly to Visier. This is the preferred authentication method.
 1. Basic Authentication: This is a traditional authentication mechanism where Visier username and password are provided directly to Visier for authentication.
 
 In order to avoid passing authentication credentials in via command line arguments, Visier recommends that at least basic authentication credentials such as username and password are provided via environment variables. However, using a new function, `make_auth()`, the appropriate authentication configuration object will be created from `VISIER_`-prefixed environment variables, as outlined  below.
 
 ### OAuth2.0
-Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the OAuth2.0 authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
+The following list and example below illustrate the OAuth2.0 authentication parameters. These are also the environment and `dotenv` variables the `make_auth()` utility function will use when instantiating an authentication object.
 * `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant as well as to initiate the OAuth2.0 authentication process
 * `VISIER_APIKEY`: The API key granted by Visier
 * `VISIER_CLIENT_ID`: The identifier of the pre-registered application
 * `VISIER_REDIRECT_URI`: The URI the `authorize` call will ultimately redirect to upon a successful authorization code generation. By default, this will be `http://localhost:5000/oauth2/callback` however note that it must match the `redirect_uri` in the client application definition exactly. If the client application setting is different, it is essential that that exact value is provided to the connector.
 * `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations
 
 On Linux-like systems, with an X-display available, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
@@ -39,14 +38,17 @@
 ```
 
 Source this file in and the environment is ready for using the connector with OAuth2.0 authentication:
 ```sh
 $ source .env
 ```
 
+#### Callback URI
+The OAuth flow requires that the authorizing server can call back to the initiating client with an authorization code. In OAuth mode, the connector starts a transient web server that listens for an authorization code on http://localhost:5000/oauth2/callback. You can modify the URL by setting a different value for VISIER_REDIRECT_URI. The VISIER_DIRECT_URI value must exactly match the URI value in your Visier OAuth 2.0 client registration and must abide by Visier's callback URI rules, such as a limited set of permissible subnets.
+
 ### Basic Authentication
 Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the basic authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
 * `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant
 * `VISIER_USERNAME`: The user name with sufficient API capabilities
 * `VISIER_PASSWORD`: The password of that user
 * `VISIER_APIKEY`: The API key granted by Visier
 * `VISIER_VANITY`: The readable name of the customer organization
@@ -68,26 +70,84 @@
 ```
 
 Source this environment in and provide the password when prompted:
 ```sh
 $ source .env
 ```
 
+## Jupyter Notebooks
+Jupyter notebooks and lab are well-suited to run Visier connector code. However, some users may not find OS-level variables ideal. As of version `0.9.9`, the Visier Python connector supports [dotenv](https://pypi.org/project/python-dotenv/) to facilitate a more dynamic switching of Visier authentication parameters. If the file is called `.env`, the Python package `dotenv` attempts to load the file. If the file has a different name, you must provide that file name when loading the environment with `dotenv`.
+
+### Jupyter Basic Authentication Example
+Basic Authentication is the most practical means of authenticating against Visier for Jupyter notebooks.
+
+Create an environment file to store the authentication parameters.
+
+Example environment file:
+```
+VISIER_VANITY=customer-specific
+VISIER_HOST=https://customer-specific.api.visier.io
+VISIER_APIKEY=the-api-key-issued-by-visier
+VISIER_USERNAME=apiuser@example.com
+VISIER_PASSWORD=password-or-variable-reference
+```
+
+Create a basic authentication object as described in the following snippet:
+```python
+from dotenv import dotenv_values
+from visier.connector import VisierSession, make_auth
+from visier.api import QueryApiClient
+
+env_creds = dotenv_values()
+auth = make_auth(env_values=env_creds)
+
+with VisierSession(auth) as s:
+    query_client = QueryApiClient(s)
+    ...
+```
+
+### Jupyter OAuth 2.0 Example
+Note that OAuth authentication to Visier in Jupyter notebooks is only supported when the Jupyter server runs on your local computer, bound to `localhost`. Therefore, OAuth in Jupyter notebooks against Visier is only recommended for test and development uses.
+To authenticate with OAuth, you must first register an OAuth 2.0 client in Visier. Visier administrators can register OAuth clients.
+
+After the OAuth client is registered in Visier, create an environment file to store the authentication parameters.
+
+Example environment file:
+```
+VISIER_HOST=https://customer-specific.api.visier.io
+VISIER_CLIENT_ID=client-id-from-registration
+VISIER_APIKEY=the-api-key-issued-by-visier
+```
+
+Create an OAuth authentication object as described in the following snippet:
+```python
+from dotenv import dotenv_values
+from visier.connector import VisierSession, make_auth
+from visier.api import QueryApiClient
+
+env_creds = dotenv_values()
+auth = make_auth(env_values=env_creds)
+
+with VisierSession(auth) as s:
+    query_client = QueryApiClient(s)
+    ...
+```
+
 ## Connector Separation
-As of version `0.9.5`, the Python connector has separated the API calls from the `VisierSession` object. As a result of this change, the query execution methods on the `VisierSession` have been deprecated and will be subject to removal in a future release.
+As of version `0.9.5`, the Python connector separates API calls from the `VisierSession` object. As a result of this change, query execution methods on the `VisierSession` are deprecated and will be removed in a future release.
 
 The new way of invoking Visier public APIs through the Visier Python connector requires instantiating the appropriate API client and calling the methods defined on the client object. The following example, invokes the `analytic-objects` Model API to obtain the metadata for two analytic objects:
 ```python
     with VisierSession(auth) as session:
         model_client = ModelApiClient(session)
 
         objs = model_client.get_analytic_objects(["Requisition", "Employee_Exit"])
         print(objs.text)
 ```
-### Error handling
+### Error Handling
 By default, a failed API call will return `None` and information about the error is available on the client object. Using the example above, the last error in the event `objs` was `None` would be `model_client.last_error()`.
 
 It is however possible to force the API client to instead raise a `QueryExecutionException`. This is accomplished when instantiating the API client with the following parameter value `raise_on_error=True`. Using the example above, the `model_client` instantiation would look like this: `model_client = ModelApiClient(session, raise_on_error=True)`.
 
 # Examples
 ## Query API
 The Query API Client is used to make calls to Visier's Query APIs.
```

### Comparing `visier-connector-0.9.8/pyproject.toml` & `visier-connector-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 keywords = ["visier", "data", "query", "connector", "api"]
 license = {file = "LICENSE"}
 dynamic = ["version"]
 dependencies = [
     "requests >= 2.31",
     "deprecated",
     "flask",
+    "python-dotenv",
 ]
 
 [tool.poetry]
 readme = "README.md"
 
 [tool.setuptools.dynamic]
 version = {attr = "visier.__version__"}
```

### Comparing `visier-connector-0.9.8/visier/__init__.py` & `visier-connector-0.9.9/visier/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
```

### Comparing `visier-connector-0.9.8/visier/api/__init__.py` & `visier-connector-0.9.9/visier/api/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier/api/base.py` & `visier-connector-0.9.9/visier/api/base.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier/api/direct_intake.py` & `visier-connector-0.9.9/visier/api/direct_intake.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier/api/model.py` & `visier-connector-0.9.9/visier/api/model.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier/api/query.py` & `visier-connector-0.9.9/visier/api/query.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier/connector/__init__.py` & `visier-connector-0.9.9/visier/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier/connector/authentication.py` & `visier-connector-0.9.9/visier/connector/authentication.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Basic Authentication class for Visier Connector
 """
 
 import os
 from argparse import ArgumentParser, Namespace
 import dataclasses
 from abc import ABC
-from typing import Any
+from typing import Any, OrderedDict
 from .constants import (ENV_VISIER_USERNAME, ENV_VISIER_PASSWORD, ENV_VISIER_HOST,
                         ENV_VISIER_APIKEY, ENV_VISIER_VANITY, ENV_VISIER_CLIENT_ID,
                         ENV_VISIER_REDIRECT_URI, ENV_VISIER_TARGET_TENANT_ID)
 
 
 @dataclasses.dataclass
 class Authentication(ABC):
@@ -106,40 +106,50 @@
     parser.add_argument("-H", "--host", help="Visier host", type=str)
     parser.add_argument("-p", "--password", help="Visier password", type=str)
     parser.add_argument("-r", "--redirect-uri", help="Visier OAuth redirect URI", type=str)
     parser.add_argument("-t", "--target-tenant-id", help="Visier partner tenant name", type=str)
     parser.add_argument("-u", "--username", help="Visier username", type=str)
     parser.add_argument("-v", "--vanity", help="Visier vanity", type=str)
 
-def make_auth(args: Namespace = None) -> Authentication:
+def make_auth(args: Namespace = None,
+              env_values: OrderedDict = None) -> Authentication:
     """Returns an Authentication subclass object based on parsed arguments or environment variable values.
-    Delegates more detailed credential completeness checks to the Authentication classes."""
+    Delegates more detailed credential completeness checks to the Authentication classes.
+    
+    Keyword arguments:
+    args -- Parsed arguments from ArgumentParser
+    env_values -- Ordered dictionary of variable values from dotenv_values"""
     args = args or NoArgs()
-    host = args.host or os.getenv(ENV_VISIER_HOST)
-    api_key = args.apikey or os.getenv(ENV_VISIER_APIKEY)
-    target_tenant_id = args.target_tenant_id or os.getenv(ENV_VISIER_TARGET_TENANT_ID)
+    env_values = env_values or OrderedDict()
+
+    def dot_or_os(var_name: str) -> str:
+        return env_values.get(var_name) or os.getenv(var_name)
+
+    host = args.host or dot_or_os(ENV_VISIER_HOST)
+    api_key = args.apikey or dot_or_os(ENV_VISIER_APIKEY)
+    target_tenant_id = args.target_tenant_id or dot_or_os(ENV_VISIER_TARGET_TENANT_ID)
 
-    username = args.username or os.getenv(ENV_VISIER_USERNAME)
-    password = args.password or os.getenv(ENV_VISIER_PASSWORD)
+    username = args.username or dot_or_os(ENV_VISIER_USERNAME)
+    password = args.password or dot_or_os(ENV_VISIER_PASSWORD)
     if (username and password):
         return Basic(
             username = username,
             password = password,
             host = host,
             api_key = api_key,
-            vanity = args.vanity or os.getenv(ENV_VISIER_VANITY),
+            vanity = args.vanity or dot_or_os(ENV_VISIER_VANITY),
             target_tenant_id = target_tenant_id)
 
-    client_id = args.client_id or os.getenv(ENV_VISIER_CLIENT_ID)
+    client_id = args.client_id or dot_or_os(ENV_VISIER_CLIENT_ID)
     if client_id:
         return OAuth2(
             host = host,
             api_key = api_key,
             client_id = client_id,
-            redirect_uri = args.redirect_uri or os.getenv(ENV_VISIER_REDIRECT_URI),
+            redirect_uri = args.redirect_uri or dot_or_os(ENV_VISIER_REDIRECT_URI),
             target_tenant_id = target_tenant_id)
 
     raise ValueError("""ERROR: Missing required credentials.
                      Please provide either Basic or OAuth2 credentials.
                      Both methods require host and api_key.
                      Basic also requires username and password.
                      OAuth2 also requires client_id.""")
```

### Comparing `visier-connector-0.9.8/visier/connector/callback.py` & `visier-connector-0.9.9/visier/connector/callback.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier/connector/constants.py` & `visier-connector-0.9.9/visier/connector/constants.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier/connector/sessions.py` & `visier-connector-0.9.9/visier/connector/sessions.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier/connector/table.py` & `visier-connector-0.9.9/visier/connector/table.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.8/visier_connector.egg-info/PKG-INFO` & `visier-connector-0.9.9/visier_connector.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.8
+Version: 0.9.9
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,29 +213,28 @@
 ![linting](https://github.com/visier/connector-python/actions/workflows/pylint.yml/badge.svg) ![pypi publishing](https://github.com/visier/connector-python/actions/workflows/publish-to-test-pypi.yml/badge.svg)
 # Visier Python Connector
 Use the Visier Python Connector to query Visier People data.
 
 The connector enables Python developers to query Visier People data using Visier's SQL-like query language. 
 
 ## Prerequisites
-The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
+The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-based service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
-* A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
-* That user's password
+* Either an OAuth connector application registration in your Visier tenant or a username and password pair with API access capabilities.
 
 ## Authentication Environment
 As of version `0.9.8`, the Visier Python Connector supports two means of authentication:
 1. OAuth2.0: The connector supports the so called three-legged authentication flow. This means that authentication (and consent) have to be provided through the authorization server. In accordance with the OAuth2.0 protocol, no user credentials are provided directly to Visier. This is the preferred authentication method.
 1. Basic Authentication: This is a traditional authentication mechanism where Visier username and password are provided directly to Visier for authentication.
 
 In order to avoid passing authentication credentials in via command line arguments, Visier recommends that at least basic authentication credentials such as username and password are provided via environment variables. However, using a new function, `make_auth()`, the appropriate authentication configuration object will be created from `VISIER_`-prefixed environment variables, as outlined  below.
 
 ### OAuth2.0
-Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the OAuth2.0 authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
+The following list and example below illustrate the OAuth2.0 authentication parameters. These are also the environment and `dotenv` variables the `make_auth()` utility function will use when instantiating an authentication object.
 * `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant as well as to initiate the OAuth2.0 authentication process
 * `VISIER_APIKEY`: The API key granted by Visier
 * `VISIER_CLIENT_ID`: The identifier of the pre-registered application
 * `VISIER_REDIRECT_URI`: The URI the `authorize` call will ultimately redirect to upon a successful authorization code generation. By default, this will be `http://localhost:5000/oauth2/callback` however note that it must match the `redirect_uri` in the client application definition exactly. If the client application setting is different, it is essential that that exact value is provided to the connector.
 * `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations
 
 On Linux-like systems, with an X-display available, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
@@ -251,14 +250,17 @@
 ```
 
 Source this file in and the environment is ready for using the connector with OAuth2.0 authentication:
 ```sh
 $ source .env
 ```
 
+#### Callback URI
+The OAuth flow requires that the authorizing server can call back to the initiating client with an authorization code. In OAuth mode, the connector starts a transient web server that listens for an authorization code on http://localhost:5000/oauth2/callback. You can modify the URL by setting a different value for VISIER_REDIRECT_URI. The VISIER_DIRECT_URI value must exactly match the URI value in your Visier OAuth 2.0 client registration and must abide by Visier's callback URI rules, such as a limited set of permissible subnets.
+
 ### Basic Authentication
 Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the basic authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
 * `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant
 * `VISIER_USERNAME`: The user name with sufficient API capabilities
 * `VISIER_PASSWORD`: The password of that user
 * `VISIER_APIKEY`: The API key granted by Visier
 * `VISIER_VANITY`: The readable name of the customer organization
@@ -280,26 +282,84 @@
 ```
 
 Source this environment in and provide the password when prompted:
 ```sh
 $ source .env
 ```
 
+## Jupyter Notebooks
+Jupyter notebooks and lab are well-suited to run Visier connector code. However, some users may not find OS-level variables ideal. As of version `0.9.9`, the Visier Python connector supports [dotenv](https://pypi.org/project/python-dotenv/) to facilitate a more dynamic switching of Visier authentication parameters. If the file is called `.env`, the Python package `dotenv` attempts to load the file. If the file has a different name, you must provide that file name when loading the environment with `dotenv`.
+
+### Jupyter Basic Authentication Example
+Basic Authentication is the most practical means of authenticating against Visier for Jupyter notebooks.
+
+Create an environment file to store the authentication parameters.
+
+Example environment file:
+```
+VISIER_VANITY=customer-specific
+VISIER_HOST=https://customer-specific.api.visier.io
+VISIER_APIKEY=the-api-key-issued-by-visier
+VISIER_USERNAME=apiuser@example.com
+VISIER_PASSWORD=password-or-variable-reference
+```
+
+Create a basic authentication object as described in the following snippet:
+```python
+from dotenv import dotenv_values
+from visier.connector import VisierSession, make_auth
+from visier.api import QueryApiClient
+
+env_creds = dotenv_values()
+auth = make_auth(env_values=env_creds)
+
+with VisierSession(auth) as s:
+    query_client = QueryApiClient(s)
+    ...
+```
+
+### Jupyter OAuth 2.0 Example
+Note that OAuth authentication to Visier in Jupyter notebooks is only supported when the Jupyter server runs on your local computer, bound to `localhost`. Therefore, OAuth in Jupyter notebooks against Visier is only recommended for test and development uses.
+To authenticate with OAuth, you must first register an OAuth 2.0 client in Visier. Visier administrators can register OAuth clients.
+
+After the OAuth client is registered in Visier, create an environment file to store the authentication parameters.
+
+Example environment file:
+```
+VISIER_HOST=https://customer-specific.api.visier.io
+VISIER_CLIENT_ID=client-id-from-registration
+VISIER_APIKEY=the-api-key-issued-by-visier
+```
+
+Create an OAuth authentication object as described in the following snippet:
+```python
+from dotenv import dotenv_values
+from visier.connector import VisierSession, make_auth
+from visier.api import QueryApiClient
+
+env_creds = dotenv_values()
+auth = make_auth(env_values=env_creds)
+
+with VisierSession(auth) as s:
+    query_client = QueryApiClient(s)
+    ...
+```
+
 ## Connector Separation
-As of version `0.9.5`, the Python connector has separated the API calls from the `VisierSession` object. As a result of this change, the query execution methods on the `VisierSession` have been deprecated and will be subject to removal in a future release.
+As of version `0.9.5`, the Python connector separates API calls from the `VisierSession` object. As a result of this change, query execution methods on the `VisierSession` are deprecated and will be removed in a future release.
 
 The new way of invoking Visier public APIs through the Visier Python connector requires instantiating the appropriate API client and calling the methods defined on the client object. The following example, invokes the `analytic-objects` Model API to obtain the metadata for two analytic objects:
 ```python
     with VisierSession(auth) as session:
         model_client = ModelApiClient(session)
 
         objs = model_client.get_analytic_objects(["Requisition", "Employee_Exit"])
         print(objs.text)
 ```
-### Error handling
+### Error Handling
 By default, a failed API call will return `None` and information about the error is available on the client object. Using the example above, the last error in the event `objs` was `None` would be `model_client.last_error()`.
 
 It is however possible to force the API client to instead raise a `QueryExecutionException`. This is accomplished when instantiating the API client with the following parameter value `raise_on_error=True`. Using the example above, the `model_client` instantiation would look like this: `model_client = ModelApiClient(session, raise_on_error=True)`.
 
 # Examples
 ## Query API
 The Query API Client is used to make calls to Visier's Query APIs.
```

### Comparing `visier-connector-0.9.8/visier_connector.egg-info/SOURCES.txt` & `visier-connector-0.9.9/visier_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

