# Comparing `tmp/jfk-django-core-0.0.0.tar.gz` & `tmp/jfk_django_core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jfk-django-core-0.0.0.tar", last modified: Sun May  5 21:24:54 2024, max compression
+gzip compressed data, was "jfk_django_core-0.0.3.tar", last modified: Thu May  9 10:44:09 2024, max compression
```

## Comparing `jfk-django-core-0.0.0.tar` & `jfk_django_core-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:24:54.869402 jfk-django-core-0.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      228 2024-05-05 21:24:54.869402 jfk-django-core-0.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:24:54.868402 jfk-django-core-0.0.0/jfk_django_core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/jfk_django_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:24:54.869402 jfk-django-core-0.0.0/jfk_django_core/admin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/jfk_django_core/admin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/jfk_django_core/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:24:54.869402 jfk-django-core-0.0.0/jfk_django_core/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/jfk_django_core/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:24:54.869402 jfk-django-core-0.0.0/jfk_django_core/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/jfk_django_core/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6747 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/jfk_django_core/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:24:54.869402 jfk-django-core-0.0.0/jfk_django_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)      228 2024-05-05 21:24:54.000000 jfk-django-core-0.0.0/jfk_django_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-05 21:24:54.000000 jfk-django-core-0.0.0/jfk_django_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:24:54.000000 jfk-django-core-0.0.0/jfk_django_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-05 21:24:54.000000 jfk-django-core-0.0.0/jfk_django_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 21:24:54.869402 jfk-django-core-0.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-05 21:24:49.000000 jfk-django-core-0.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.870851 jfk_django_core-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.866851 jfk_django_core-0.0.3/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/.vscode/launch.json
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      790 2024-05-09 10:44:09.869851 jfk_django_core-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.867851 jfk_django_core-0.0.3/jfk_django_core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.868851 jfk_django_core-0.0.3/jfk_django_core/admin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/admin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.868851 jfk_django_core-0.0.3/jfk_django_core/apis/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/apis/jfk_authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.869851 jfk_django_core-0.0.3/jfk_django_core/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.869851 jfk_django_core-0.0.3/jfk_django_core/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7188 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.869851 jfk_django_core-0.0.3/jfk_django_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      790 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 10:44:09.870851 jfk_django_core-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/setup.py
```

### Comparing `jfk-django-core-0.0.0/LICENSE` & `jfk_django_core-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jfk-django-core-0.0.0/jfk_django_core/settings.py` & `jfk_django_core-0.0.3/jfk_django_core/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     # 3rd party
     'rest_framework',
     "django_celery_results",
     "django_celery_beat",
     'corsheaders',
     'knox',
     'colorfield',
+    'drf_spectacular_sidecar',
+    'drf_spectacular',
     # Apps
     'jfk_django_core.apps.JfkDjangoCoreConfig',
 ]
 
 
 ALLOWED_HOSTS = ['*']
 
@@ -197,15 +199,16 @@
         'rest_framework.authentication.SessionAuthentication',
         'rest_framework.authentication.BasicAuthentication',
     ),
     'DEFAULT_PERMISSION_CLASSES': (
         'rest_framework.permissions.IsAuthenticated',
     ),
     'DEFAULT_PAGINATION_CLASS': 'rest_framework.pagination.LimitOffsetPagination',
-    'PAGE_SIZE': 100
+    'PAGE_SIZE': 100,
+    'DEFAULT_SCHEMA_CLASS': 'drf_spectacular.openapi.AutoSchema',
 }
 
 # Channel Layers
 layersHosts = os.getenv("DJANOG_CHANNEL_LAYERS_HOSTS")
 layersHosts = layersHosts.split(",") if layersHosts is not None else None
 
 if layersHosts is not None:
@@ -229,8 +232,19 @@
 REST_KNOX = {
     'SECURE_HASH_ALGORITHM': 'cryptography.hazmat.primitives.hashes.SHA512',
     'AUTH_TOKEN_CHARACTER_LENGTH': 64,
     'TOKEN_TTL': timedelta(days=14),
     'USER_SERIALIZER': 'knox.serializers.UserSerializer',
     'TOKEN_LIMIT_PER_USER': None,
     'AUTO_REFRESH': True,
+}
+
+# Spectacular
+SPECTACULAR_SETTINGS = {
+    'TITLE': 'JFK Django Core',
+    'DESCRIPTION': 'JFK Django Core API',
+    'VERSION': '1.0.0',
+    'SERVE_INCLUDE_SCHEMA': False,
+    'SWAGGER_UI_DIST': 'SIDECAR',  # shorthand to use the sidecar instead
+    'SWAGGER_UI_FAVICON_HREF': 'SIDECAR',
+    'REDOC_DIST': 'SIDECAR',
 }
```

