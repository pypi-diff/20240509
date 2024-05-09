# Comparing `tmp/cf-ips-to-hcloud-fw-1.0.8.tar.gz` & `tmp/cf-ips-to-hcloud-fw-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf-ips-to-hcloud-fw-1.0.8.tar", last modified: Thu Feb  8 20:05:57 2024, max compression
+gzip compressed data, was "cf-ips-to-hcloud-fw-1.0.9.tar", last modified: Sat Mar 16 14:16:57 2024, max compression
```

## Comparing `cf-ips-to-hcloud-fw-1.0.8.tar` & `cf-ips-to-hcloud-fw-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 20:05:57.163836 cf-ips-to-hcloud-fw-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-02-08 20:05:57.163836 cf-ips-to-hcloud-fw-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-08 20:05:51.000000 cf-ips-to-hcloud-fw-1.0.8/requirements-dev-pep508.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-08 20:05:48.000000 cf-ips-to-hcloud-fw-1.0.8/requirements-pep508.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 20:05:57.163836 cf-ips-to-hcloud-fw-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 20:05:57.151836 cf-ips-to-hcloud-fw-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 20:05:57.155836 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 20:05:57.159836 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-02-08 20:05:57.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-08 20:05:57.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 20:05:57.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-08 20:05:57.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-08 20:05:57.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-08 20:05:57.000000 cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 20:05:57.159836 cf-ips-to-hcloud-fw-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/tests/test_cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/tests/test_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-08 20:05:18.000000 cf-ips-to-hcloud-fw-1.0.8/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:16:57.812780 cf-ips-to-hcloud-fw-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-03-16 14:16:57.812780 cf-ips-to-hcloud-fw-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-16 14:16:55.000000 cf-ips-to-hcloud-fw-1.0.9/requirements-dev-pep508.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-16 14:16:51.000000 cf-ips-to-hcloud-fw-1.0.9/requirements-pep508.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 14:16:57.812780 cf-ips-to-hcloud-fw-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:16:57.800780 cf-ips-to-hcloud-fw-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:16:57.804780 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:16:57.808780 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-03-16 14:16:57.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-16 14:16:57.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 14:16:57.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-16 14:16:57.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-16 14:16:57.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-16 14:16:57.000000 cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 14:16:57.808780 cf-ips-to-hcloud-fw-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/tests/test_cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/tests/test_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-16 14:16:12.000000 cf-ips-to-hcloud-fw-1.0.9/tests/test_version.py
```

### Comparing `cf-ips-to-hcloud-fw-1.0.8/LICENSE` & `cf-ips-to-hcloud-fw-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/PKG-INFO` & `cf-ips-to-hcloud-fw-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-ips-to-hcloud-fw
-Version: 1.0.8
+Version: 1.0.9
 Summary: Update Hetzner Cloud firewall rules with Cloudflare IP ranges
 Author: Jürgen Kreileder
 Author-email: jk@blackdown.de
 License: MIT
 Project-URL: Homepage, https://github.com/jkreileder/cf-ips-to-hcloud-fw
 Project-URL: Source, https://github.com/jkreileder/cf-ips-to-hcloud-fw
 Project-URL: Changelog, https://github.com/jkreileder/cf-ips-to-hcloud-fw/blob/main/CHANGELOG.md
@@ -34,47 +34,47 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: attrs==23.2.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: cloudflare==2.17.0
+Requires-Dist: cloudflare==2.19.2
 Requires-Dist: hcloud==1.33.2
 Requires-Dist: idna==3.6
 Requires-Dist: jsonlines==4.0.0
-Requires-Dist: pydantic==2.6.1
-Requires-Dist: pydantic-core==2.16.2
-Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic-core==2.16.3
+Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
-Requires-Dist: typing-extensions==4.9.0
-Requires-Dist: urllib3==2.2.0
+Requires-Dist: typing-extensions==4.10.0
+Requires-Dist: urllib3==2.2.1
 Provides-Extra: dev
-Requires-Dist: build==1.0.3; extra == "dev"
+Requires-Dist: build==1.1.1; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
-Requires-Dist: coverage[toml]==7.4.1; extra == "dev"
+Requires-Dist: coverage[toml]==7.4.4; extra == "dev"
 Requires-Dist: exceptiongroup==1.2.0; extra == "dev"
-Requires-Dist: importlib-metadata==7.0.1; extra == "dev"
+Requires-Dist: importlib-metadata==7.0.2; extra == "dev"
 Requires-Dist: iniconfig==2.0.0; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
-Requires-Dist: packaging==23.2; extra == "dev"
-Requires-Dist: pip-tools==7.3.0; extra == "dev"
+Requires-Dist: packaging==24.0; extra == "dev"
+Requires-Dist: pip-tools==7.4.1; extra == "dev"
 Requires-Dist: pluggy==1.4.0; extra == "dev"
 Requires-Dist: pyproject-hooks==1.0.0; extra == "dev"
-Requires-Dist: pyright==1.1.350; extra == "dev"
-Requires-Dist: pytest==8.0.0; extra == "dev"
+Requires-Dist: pyright==1.1.354; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
-Requires-Dist: ruff==0.2.1; extra == "dev"
+Requires-Dist: ruff==0.3.3; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
-Requires-Dist: wheel==0.42.0; extra == "dev"
-Requires-Dist: zipp==3.17.0; extra == "dev"
+Requires-Dist: wheel==0.43.0; extra == "dev"
+Requires-Dist: zipp==3.18.1; extra == "dev"
 Requires-Dist: pip==24.0; extra == "dev"
-Requires-Dist: setuptools==69.0.3; extra == "dev"
+Requires-Dist: setuptools==69.2.0; extra == "dev"
 
 # Update Hetzner Cloud Firewall Rules with Current Cloudflare IP Ranges  <!-- omit in toc -->
 
 [![codecov](https://codecov.io/gh/jkreileder/cf-ips-to-hcloud-fw/graph/badge.svg?token=PCP1F2XWAT)](https://codecov.io/gh/jkreileder/cf-ips-to-hcloud-fw)
 [![OpenSSF Best Practices](https://www.bestpractices.dev/projects/8275/badge)](https://www.bestpractices.dev/projects/8275)
 [![CodeQL](https://github.com/jkreileder/cf-ips-to-hcloud-fw/actions/workflows/codeql.yaml/badge.svg)](https://github.com/jkreileder/cf-ips-to-hcloud-fw/actions/workflows/codeql.yaml)
 [![Python package](https://github.com/jkreileder/cf-ips-to-hcloud-fw/actions/workflows/python-package.yaml/badge.svg)](https://github.com/jkreileder/cf-ips-to-hcloud-fw/actions/workflows/python-package.yaml)
@@ -182,25 +182,25 @@
 CronJob.  Simply mount your configuration file as `/usr/src/app/config.yaml`.
 
 Here's an example using Docker:
 
 ```shell
 docker run --rm \
   --mount type=bind,source=$(pwd)/config.yaml,target=/usr/src/app/config.yaml,readonly \
-  jkreileder/cf-ips-to-hcloud-fw:1.0.8
+  jkreileder/cf-ips-to-hcloud-fw:1.0.9
 ```
 
 (Add `--pull=always` if you use a rolling image tag.)
 
 Docker images for `cf-ips-to-hcloud-fw` are available for both `linux/amd64` and
 `linux/arm64` architectures.  The Docker images support the following tags:
 
 - `1`: This tag always points to the latest `1.x.x` release.
 - `1.0`: This tag always points to the latest `1.0.x` release.
-- `1.0.8`: This tag points to the specific `1.0.8` release.
+- `1.0.9`: This tag points to the specific `1.0.9` release.
 - `main`: This tag points to the most recent development version of
   `cf-ips-to-hcloud-fw`. Use this at your own risk as it may contain unstable
   changes.
 
 You can find the Docker images at:
 
 - [Docker Hub](https://hub.docker.com/r/jkreileder/cf-ips-to-hcloud-fw)
@@ -241,15 +241,15 @@
       template:
         spec:
           securityContext:
             runAsNonRoot: true
             runAsUser: 65534
           containers:
             - name: cf-ips-to-hcloud-fw
-              image: jkreileder/cf-ips-to-hcloud-fw:1.0.8
+              image: jkreileder/cf-ips-to-hcloud-fw:1.0.9
               # imagePullPolicy: Always # Uncomment this if you use a rolling image tag
               securityContext:
                 allowPrivilegeEscalation: false
                 readOnlyRootFilesystem: true
                 capabilities:
                   drop:
                     - ALL
```

### Comparing `cf-ips-to-hcloud-fw-1.0.8/README.md` & `cf-ips-to-hcloud-fw-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -108,25 +108,25 @@
 CronJob.  Simply mount your configuration file as `/usr/src/app/config.yaml`.
 
 Here's an example using Docker:
 
 ```shell
 docker run --rm \
   --mount type=bind,source=$(pwd)/config.yaml,target=/usr/src/app/config.yaml,readonly \
-  jkreileder/cf-ips-to-hcloud-fw:1.0.8
+  jkreileder/cf-ips-to-hcloud-fw:1.0.9
 ```
 
 (Add `--pull=always` if you use a rolling image tag.)
 
 Docker images for `cf-ips-to-hcloud-fw` are available for both `linux/amd64` and
 `linux/arm64` architectures.  The Docker images support the following tags:
 
 - `1`: This tag always points to the latest `1.x.x` release.
 - `1.0`: This tag always points to the latest `1.0.x` release.
-- `1.0.8`: This tag points to the specific `1.0.8` release.
+- `1.0.9`: This tag points to the specific `1.0.9` release.
 - `main`: This tag points to the most recent development version of
   `cf-ips-to-hcloud-fw`. Use this at your own risk as it may contain unstable
   changes.
 
 You can find the Docker images at:
 
 - [Docker Hub](https://hub.docker.com/r/jkreileder/cf-ips-to-hcloud-fw)
@@ -167,15 +167,15 @@
       template:
         spec:
           securityContext:
             runAsNonRoot: true
             runAsUser: 65534
           containers:
             - name: cf-ips-to-hcloud-fw
-              image: jkreileder/cf-ips-to-hcloud-fw:1.0.8
+              image: jkreileder/cf-ips-to-hcloud-fw:1.0.9
               # imagePullPolicy: Always # Uncomment this if you use a rolling image tag
               securityContext:
                 allowPrivilegeEscalation: false
                 readOnlyRootFilesystem: true
                 capabilities:
                   drop:
                     - ALL
```

### Comparing `cf-ips-to-hcloud-fw-1.0.8/pyproject.toml` & `cf-ips-to-hcloud-fw-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/requirements-dev-pep508.txt` & `cf-ips-to-hcloud-fw-1.0.9/requirements-dev-pep508.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --allow-unsafe --newline=LF --output-file=requirements-dev-pep508.txt requirements-dev.txt
 #
-build==1.0.3
+build==1.1.1
     # via
     #   -r requirements-dev.txt
     #   pip-tools
 click==8.1.7
     # via
     #   -r requirements-dev.txt
     #   pip-tools
-coverage[toml]==7.4.1
+coverage[toml]==7.4.4
     # via
     #   -r requirements-dev.txt
-    #   coverage
     #   pytest-cov
 exceptiongroup==1.2.0
     # via -r requirements-dev.txt
-importlib-metadata==7.0.1
+importlib-metadata==7.0.2
     # via -r requirements-dev.txt
 iniconfig==2.0.0
     # via
     #   -r requirements-dev.txt
     #   pytest
 nodeenv==1.8.0
     # via
     #   -r requirements-dev.txt
     #   pyright
-packaging==23.2
+packaging==24.0
     # via
     #   -r requirements-dev.txt
     #   build
     #   pytest
-pip-tools==7.3.0
+pip-tools==7.4.1
     # via -r requirements-dev.txt
 pluggy==1.4.0
     # via
     #   -r requirements-dev.txt
     #   pytest
 pyproject-hooks==1.0.0
     # via
     #   -r requirements-dev.txt
     #   build
-pyright==1.1.350
+    #   pip-tools
+pyright==1.1.354
     # via -r requirements-dev.txt
-pytest==8.0.0
+pytest==8.1.1
     # via
     #   -r requirements-dev.txt
     #   pytest-cov
 pytest-cov==4.1.0
     # via -r requirements-dev.txt
-ruff==0.2.1
+ruff==0.3.3
     # via -r requirements-dev.txt
 tomli==2.0.1
     # via -r requirements-dev.txt
-wheel==0.42.0
+wheel==0.43.0
     # via
     #   -r requirements-dev.txt
     #   pip-tools
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   -r requirements-dev.txt
     #   importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0
     # via
     #   -r requirements-dev.txt
     #   pip-tools
-setuptools==69.0.3
+setuptools==69.2.0
     # via
     #   -r requirements-dev.txt
     #   nodeenv
     #   pip-tools
```

### Comparing `cf-ips-to-hcloud-fw-1.0.8/requirements-pep508.txt` & `cf-ips-to-hcloud-fw-1.0.9/requirements-pep508.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,33 +16,33 @@
     # via
     #   -r requirements.txt
     #   requests
 charset-normalizer==3.3.2
     # via
     #   -r requirements.txt
     #   requests
-cloudflare==2.17.0
+cloudflare==2.19.2
     # via -r requirements.txt
 hcloud==1.33.2
     # via -r requirements.txt
 idna==3.6
     # via
     #   -r requirements.txt
     #   requests
 jsonlines==4.0.0
     # via
     #   -r requirements.txt
     #   cloudflare
-pydantic==2.6.1
+pydantic==2.6.4
     # via -r requirements.txt
-pydantic-core==2.16.2
+pydantic-core==2.16.3
     # via
     #   -r requirements.txt
     #   pydantic
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   -r requirements.txt
     #   hcloud
 pyyaml==6.0.1
     # via
     #   -r requirements.txt
     #   cloudflare
@@ -51,16 +51,16 @@
     #   -r requirements.txt
     #   cloudflare
     #   hcloud
 six==1.16.0
     # via
     #   -r requirements.txt
     #   python-dateutil
-typing-extensions==4.9.0
+typing-extensions==4.10.0
     # via
     #   -r requirements.txt
     #   pydantic
     #   pydantic-core
-urllib3==2.2.0
+urllib3==2.2.1
     # via
     #   -r requirements.txt
     #   requests
```

### Comparing `cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/__main__.py` & `cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/__main__.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/cloudflare.py` & `cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/cloudflare.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/config.py` & `cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/config.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/firewall.py` & `cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/firewall.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw/logging.py` & `cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw/logging.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw.egg-info/PKG-INFO` & `cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-ips-to-hcloud-fw
-Version: 1.0.8
+Version: 1.0.9
 Summary: Update Hetzner Cloud firewall rules with Cloudflare IP ranges
 Author: Jürgen Kreileder
 Author-email: jk@blackdown.de
 License: MIT
 Project-URL: Homepage, https://github.com/jkreileder/cf-ips-to-hcloud-fw
 Project-URL: Source, https://github.com/jkreileder/cf-ips-to-hcloud-fw
 Project-URL: Changelog, https://github.com/jkreileder/cf-ips-to-hcloud-fw/blob/main/CHANGELOG.md
@@ -34,47 +34,47 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: attrs==23.2.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: cloudflare==2.17.0
+Requires-Dist: cloudflare==2.19.2
 Requires-Dist: hcloud==1.33.2
 Requires-Dist: idna==3.6
 Requires-Dist: jsonlines==4.0.0
-Requires-Dist: pydantic==2.6.1
-Requires-Dist: pydantic-core==2.16.2
-Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic-core==2.16.3
+Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
-Requires-Dist: typing-extensions==4.9.0
-Requires-Dist: urllib3==2.2.0
+Requires-Dist: typing-extensions==4.10.0
+Requires-Dist: urllib3==2.2.1
 Provides-Extra: dev
-Requires-Dist: build==1.0.3; extra == "dev"
+Requires-Dist: build==1.1.1; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
-Requires-Dist: coverage[toml]==7.4.1; extra == "dev"
+Requires-Dist: coverage[toml]==7.4.4; extra == "dev"
 Requires-Dist: exceptiongroup==1.2.0; extra == "dev"
-Requires-Dist: importlib-metadata==7.0.1; extra == "dev"
+Requires-Dist: importlib-metadata==7.0.2; extra == "dev"
 Requires-Dist: iniconfig==2.0.0; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
-Requires-Dist: packaging==23.2; extra == "dev"
-Requires-Dist: pip-tools==7.3.0; extra == "dev"
+Requires-Dist: packaging==24.0; extra == "dev"
+Requires-Dist: pip-tools==7.4.1; extra == "dev"
 Requires-Dist: pluggy==1.4.0; extra == "dev"
 Requires-Dist: pyproject-hooks==1.0.0; extra == "dev"
-Requires-Dist: pyright==1.1.350; extra == "dev"
-Requires-Dist: pytest==8.0.0; extra == "dev"
+Requires-Dist: pyright==1.1.354; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
-Requires-Dist: ruff==0.2.1; extra == "dev"
+Requires-Dist: ruff==0.3.3; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
-Requires-Dist: wheel==0.42.0; extra == "dev"
-Requires-Dist: zipp==3.17.0; extra == "dev"
+Requires-Dist: wheel==0.43.0; extra == "dev"
+Requires-Dist: zipp==3.18.1; extra == "dev"
 Requires-Dist: pip==24.0; extra == "dev"
-Requires-Dist: setuptools==69.0.3; extra == "dev"
+Requires-Dist: setuptools==69.2.0; extra == "dev"
 
 # Update Hetzner Cloud Firewall Rules with Current Cloudflare IP Ranges  <!-- omit in toc -->
 
 [![codecov](https://codecov.io/gh/jkreileder/cf-ips-to-hcloud-fw/graph/badge.svg?token=PCP1F2XWAT)](https://codecov.io/gh/jkreileder/cf-ips-to-hcloud-fw)
 [![OpenSSF Best Practices](https://www.bestpractices.dev/projects/8275/badge)](https://www.bestpractices.dev/projects/8275)
 [![CodeQL](https://github.com/jkreileder/cf-ips-to-hcloud-fw/actions/workflows/codeql.yaml/badge.svg)](https://github.com/jkreileder/cf-ips-to-hcloud-fw/actions/workflows/codeql.yaml)
 [![Python package](https://github.com/jkreileder/cf-ips-to-hcloud-fw/actions/workflows/python-package.yaml/badge.svg)](https://github.com/jkreileder/cf-ips-to-hcloud-fw/actions/workflows/python-package.yaml)
@@ -182,25 +182,25 @@
 CronJob.  Simply mount your configuration file as `/usr/src/app/config.yaml`.
 
 Here's an example using Docker:
 
 ```shell
 docker run --rm \
   --mount type=bind,source=$(pwd)/config.yaml,target=/usr/src/app/config.yaml,readonly \
-  jkreileder/cf-ips-to-hcloud-fw:1.0.8
+  jkreileder/cf-ips-to-hcloud-fw:1.0.9
 ```
 
 (Add `--pull=always` if you use a rolling image tag.)
 
 Docker images for `cf-ips-to-hcloud-fw` are available for both `linux/amd64` and
 `linux/arm64` architectures.  The Docker images support the following tags:
 
 - `1`: This tag always points to the latest `1.x.x` release.
 - `1.0`: This tag always points to the latest `1.0.x` release.
-- `1.0.8`: This tag points to the specific `1.0.8` release.
+- `1.0.9`: This tag points to the specific `1.0.9` release.
 - `main`: This tag points to the most recent development version of
   `cf-ips-to-hcloud-fw`. Use this at your own risk as it may contain unstable
   changes.
 
 You can find the Docker images at:
 
 - [Docker Hub](https://hub.docker.com/r/jkreileder/cf-ips-to-hcloud-fw)
@@ -241,15 +241,15 @@
       template:
         spec:
           securityContext:
             runAsNonRoot: true
             runAsUser: 65534
           containers:
             - name: cf-ips-to-hcloud-fw
-              image: jkreileder/cf-ips-to-hcloud-fw:1.0.8
+              image: jkreileder/cf-ips-to-hcloud-fw:1.0.9
               # imagePullPolicy: Always # Uncomment this if you use a rolling image tag
               securityContext:
                 allowPrivilegeEscalation: false
                 readOnlyRootFilesystem: true
                 capabilities:
                   drop:
                     - ALL
```

### Comparing `cf-ips-to-hcloud-fw-1.0.8/src/cf_ips_to_hcloud_fw.egg-info/SOURCES.txt` & `cf-ips-to-hcloud-fw-1.0.9/src/cf_ips_to_hcloud_fw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/tests/test_cloudflare.py` & `cf-ips-to-hcloud-fw-1.0.9/tests/test_cloudflare.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/tests/test_config.py` & `cf-ips-to-hcloud-fw-1.0.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/tests/test_firewall.py` & `cf-ips-to-hcloud-fw-1.0.9/tests/test_firewall.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/tests/test_logging.py` & `cf-ips-to-hcloud-fw-1.0.9/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/tests/test_main.py` & `cf-ips-to-hcloud-fw-1.0.9/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `cf-ips-to-hcloud-fw-1.0.8/tests/test_version.py` & `cf-ips-to-hcloud-fw-1.0.9/tests/test_version.py`

 * *Files identical despite different names*

