# Comparing `tmp/ansible-deployer-0.0.44.tar.gz` & `tmp/ansible_deployer-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fazi/deploy-ans/ansible-deployer/dist/tmpaoixd94q/ansible-deployer-0.0.44.tar", last modified: Wed Feb 22 13:56:31 2023, max compression
+gzip compressed data, was "ansible_deployer-0.0.46.tar", last modified: Thu May  9 12:12:32 2024, max compression
```

## Comparing `ansible-deployer-0.0.44.tar` & `ansible_deployer-0.0.46.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/ansible_deployer.egg-info/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     2560 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/ansible_deployer.egg-info/PKG-INFO
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1160 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/ansible_deployer.egg-info/SOURCES.txt
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        1 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/ansible_deployer.egg-info/dependency_links.txt
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       65 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/ansible_deployer.egg-info/entry_points.txt
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        1 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/ansible_deployer.egg-info/not-zip-safe
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       54 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/ansible_deployer.egg-info/requires.txt
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       17 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/ansible_deployer.egg-info/top_level.txt
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/etc/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/etc/hooks/
--rwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)     1458 2023-02-13 07:41:14.000000 ansible-deployer-0.0.44/etc/hooks/setup_work_dir.sh
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1627 2023-01-02 00:58:08.000000 ansible-deployer-0.0.44/etc/acl.yaml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      282 2023-01-02 00:58:08.000000 ansible-deployer-0.0.44/etc/ansible-deploy.yaml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      499 2023-01-02 00:58:08.000000 ansible-deployer-0.0.44/etc/infra.yaml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     3389 2023-02-17 08:35:15.000000 ansible-deployer-0.0.44/etc/tasks.yaml
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/source/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/source/modules/
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/source/modules/configs/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/configs/__init__.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     6312 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/configs/config.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     7643 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/configs/schema.py
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/source/modules/database/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/database/__init__.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     2954 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/database/creator.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      655 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/database/schema.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     6049 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/database/writer.py
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/source/modules/locking/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/locking/__init__.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     2712 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/locking/locking.py
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/source/modules/outputs/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/outputs/__init__.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     3404 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/outputs/formatting.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     3615 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/outputs/logging.py
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/source/modules/runners/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/runners/__init__.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)    10793 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/runners/run.py
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/source/modules/validators/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/validators/__init__.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)    11649 2023-02-22 13:55:50.000000 ansible-deployer-0.0.44/source/modules/validators/validate.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/__init__.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)      465 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/globalvars.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     4670 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/modules/misc.py
-drwxr-xr-x   0 fazi      (1122) AptivHPCL3  (1112)        0 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/source/plugins/
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     3503 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/plugins/log_plays_adjusted.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     4331 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/plugins/sqlite_deployer.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     9082 2023-02-22 13:21:56.000000 ansible-deployer-0.0.44/source/main.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1063 2023-01-02 00:58:08.000000 ansible-deployer-0.0.44/LICENSE
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       24 2023-02-17 11:28:39.000000 ansible-deployer-0.0.44/MANIFEST.in
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1488 2023-02-13 03:04:06.000000 ansible-deployer-0.0.44/README.md
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)       41 2023-02-13 07:41:14.000000 ansible-deployer-0.0.44/pyproject.toml
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     1607 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/setup.cfg
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     2816 2023-02-13 07:41:14.000000 ansible-deployer-0.0.44/setup.py
--rw-r--r--   0 fazi      (1122) AptivHPCL3  (1112)     2560 2023-02-22 13:56:31.000000 ansible-deployer-0.0.44/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/ansible_deployer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-09 12:12:32.000000 ansible_deployer-0.0.46/ansible_deployer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 12:12:32.000000 ansible_deployer-0.0.46/ansible_deployer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:12:32.000000 ansible_deployer-0.0.46/ansible_deployer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 12:12:32.000000 ansible_deployer-0.0.46/ansible_deployer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:12:32.000000 ansible_deployer-0.0.46/ansible_deployer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 12:12:32.000000 ansible_deployer-0.0.46/ansible_deployer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 12:12:32.000000 ansible_deployer-0.0.46/ansible_deployer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.723451 ansible_deployer-0.0.46/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/etc/acl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/etc/ansible-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.723451 ansible_deployer-0.0.46/etc/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1458 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/etc/hooks/setup_work_dir.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/etc/infra.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/etc/tasks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-09 12:12:32.731451 ansible_deployer-0.0.46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.723451 ansible_deployer-0.0.46/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/source/modules/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/configs/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/source/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/database/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/database/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/database/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/globalvars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/source/modules/locking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/locking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/locking/locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/source/modules/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/outputs/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/outputs/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/source/modules/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/runners/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/source/modules/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/modules/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:12:32.727450 ansible_deployer-0.0.46/source/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/plugins/log_plays_adjusted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-09 12:12:28.000000 ansible_deployer-0.0.46/source/plugins/sqlite_deployer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ansible-deployer-0.0.44/ansible_deployer.egg-info/PKG-INFO` & `ansible_deployer-0.0.46/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-deployer
-Version: 0.0.44
+Version: 0.0.46
 Summary: Wrapper around ansible-playbook allowing configurable tasks and permissions
 Home-page: https://github.com/cinek810/ansible-deployer
 Author: J. Wierzbowski, M. Stolarek
 Author-email: 
 License: MIT
 Project-URL: Source, https://github.com/cinek810/ansible-deployer
 Platform: linux
@@ -20,14 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Clustering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
+Requires-Dist: pyyaml>=5.3.1
+Requires-Dist: cerberus>=1.3.1
+Requires-Dist: pytest-testinfra>=6.6.0
 
 # ansible-deployer
 However ansible is a great tool for IT infrastructure automation in certain cases it's hard to use
 it for the complete deployment, because of that tools like ansible-tower/AWX try to wrap it's
 activity making further assumptions on the way ansible code is stored (versioning repository), the
 way it's executed - certain combinations of inventory/playbook/tag options used to achieve specific
 goals. Having it in mind ansible-deployer may be treated as yet another ansible-playbook wrapper, but
@@ -47,9 +50,7 @@
 - `tasks.yaml` - Configuration of tasks (sets of playbooks to be executed)
 - `infra.yaml` - Configuration of infrastructures and stages of those mapping to ansible inventory
 
 ## Examples
 ```
 ansible-deployer run --task updateUsers --infra webServers --stage prod
 ```
-
-
```

### Comparing `ansible-deployer-0.0.44/ansible_deployer.egg-info/SOURCES.txt` & `ansible_deployer-0.0.46/ansible_deployer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/etc/hooks/setup_work_dir.sh` & `ansible_deployer-0.0.46/etc/hooks/setup_work_dir.sh`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/etc/acl.yaml` & `ansible_deployer-0.0.46/etc/acl.yaml`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/etc/tasks.yaml` & `ansible_deployer-0.0.46/etc/tasks.yaml`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/configs/config.py` & `ansible_deployer-0.0.46/source/modules/configs/config.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/configs/schema.py` & `ansible_deployer-0.0.46/source/modules/configs/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/database/creator.py` & `ansible_deployer-0.0.46/source/modules/database/creator.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/database/schema.py` & `ansible_deployer-0.0.46/source/modules/database/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/database/writer.py` & `ansible_deployer-0.0.46/source/modules/database/writer.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/locking/locking.py` & `ansible_deployer-0.0.46/source/modules/locking/locking.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/outputs/formatting.py` & `ansible_deployer-0.0.46/source/modules/outputs/formatting.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/outputs/logging.py` & `ansible_deployer-0.0.46/source/modules/outputs/logging.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/runners/run.py` & `ansible_deployer-0.0.46/source/modules/runners/run.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/modules/validators/validate.py` & `ansible_deployer-0.0.46/source/modules/validators/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,35 +138,35 @@
                         if stage["name"] == options["stage"]:
                             allow = stage.get("allow_user_checkout", None)
                             if not allow:
                                 self.logger.critical("Self setup is not allowed for infra %s!",
                                                      infra["name"])
                                 sys.exit(59)
                             else:
-                                ret = options["self_setup"]
+                                return options["self_setup"]
         else:
             self.logger.critical("Provided --self-setup path %s does not exist!",
                                  options["self_setup"])
             sys.exit(59)
-
-        return ret
+        return None
 
     def validate_commit(self, options: dict, config: dict):
         """Function to validate commit value against config and assign final value"""
         if not options["commit"]:
             commit_id = None
             self.logger.debug("Using default commit.")
         else:
             for item in config["tasks"]["tasks"]:
                 if item["name"] == options["task"]:
                     for elem in item["allowed_for"]:
                         available_commits = elem.get("commit", [])
                         for commit in available_commits:
-                            if re.fullmatch(commit, options["commit"]):
-                                commit_id = commit
+                            commit_id = re.fullmatch(commit, options["commit"])
+                            if commit_id:
+                                commit_id = commit_id.group()
                                 self.logger.debug("Using commit: %s .", commit_id)
                                 break
                         else:
                             continue
                         break
                     else:
                         self.logger.error("Requested commit %s is not valid for task %s.",
```

### Comparing `ansible-deployer-0.0.44/source/modules/misc.py` & `ansible_deployer-0.0.46/source/modules/misc.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/plugins/log_plays_adjusted.py` & `ansible_deployer-0.0.46/source/plugins/log_plays_adjusted.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/plugins/sqlite_deployer.py` & `ansible_deployer-0.0.46/source/plugins/sqlite_deployer.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/source/main.py` & `ansible_deployer-0.0.46/source/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     parser = argparse.ArgumentParser(add_help=True)
 
     parser.add_argument("subcommand", nargs='*', default=None, metavar="SUBCOMMAND",
                         help='Specify subcommand to execute. Available commands: '+ \
                         str(globalvars.SUBCOMMANDS))
     parser.add_argument("--infrastructure", "-i", nargs=1, default=[None], metavar="INFRASTRUCTURE",
                         help='Specify infrastructure for deploy.')
+    parser.add_argument("--inventory", "-I", nargs=1, default=[None], metavar="INVENTORY",
+                        help='Specify inventory, only allowed if not set in configuration')
     parser.add_argument("--stage", "-s", nargs=1, default=[None], metavar="STAGE",
                         help='Specify stage type. Available types are: "testing" and "prod".')
     parser.add_argument("--commit", "-c", nargs=1, default=[None], metavar="COMMIT",
                         help='Provide commit ID.')
     parser.add_argument("--task", "-t", nargs=1, default=[None], metavar='TASK_NAME',
                         help='Provide task_name.')
     parser.add_argument("--conf-validation", default=False, action='store_true', help='Execute '
@@ -51,14 +53,16 @@
                         ' original messages in real time during runner execution.')
     parser.add_argument("--self-setup", nargs=1, default=[None], metavar="LOCAL_SETUP_PATH",
                         help='Setup repo outside of workdir in requested path. This option applies'
                         ' only to infrastructures with allow_user_checkout enabled in infra'
                         ' config!')
     parser.add_argument("--no-color", default=False, action="store_true", help='Disable coloring'
                         'of console messages.')
+    parser.add_argument("--no-lock", default=False, action="store_true",
+                        help='Do not lock the infrastructure')
     parser.add_argument("--check-mode", "-C", action="store_true", help='Enable --check-mode/-C'
                         ' when using default runner (ansible-playbook).')
     parser.add_argument("--dry-mode", "-D", action="store_true", help='Execute default runner'
                         ' (ansible-playbook) with "ansible_deployer_dry_mode" tag, triggering only'
                         ' required variable validation in pre_tasks. This tag is not predefined!')
 
     arguments = parser.parse_args(argv)
@@ -83,27 +87,29 @@
     options = {}
     options["subcommand"] = arguments.subcommand[0].lower()
     Validators.verify_subcommand(options["subcommand"], arguments.no_color)
     Validators.verify_switches(arguments.subcommand, arguments.no_color)
 
     options["switches"] = arguments.subcommand[1:]
     options["infra"] = arguments.infrastructure[0]
+    options['inventory'] = arguments.inventory[0]
     options["stage"] = arguments.stage[0]
     options["commit"] = arguments.commit[0]
     options["task"] = arguments.task[0]
     options["conf_val"] = arguments.conf_validation
     options["keep_locked"] = arguments.keep_locked
     options["debug"] = arguments.debug
     options["syslog"] = arguments.syslog
     options["limit"] = arguments.limit[0]
     options["raw_output"] = arguments.raw_runner_output
     options["self_setup"] = os.path.abspath(arguments.self_setup[0]) if arguments.self_setup[0] \
                             else None
     options["conf_dir"] = os.path.abspath(arguments.conf_dir[0]) if arguments.conf_dir[0] else None
     options["no_color"] = arguments.no_color
+    options["lock"] = not arguments.no_lock
     options["check_mode"] = arguments.check_mode
     options["dry_mode"] = arguments.dry_mode
 
     return options
 
 def main():
     """ansible-deploy endpoint function"""
@@ -142,14 +148,21 @@
                            ".")
         sys.exit(0)
 
     if options["subcommand"] == "show":
         misc.show_deployer(config, options)
     else:
         inv_file = misc.get_inventory_file(config, options)
+        if not inv_file and options['inventory']:
+            inv_file = options['inventory']
+        elif options['inventory']:
+            logger.logger.info("Ignoring specified inventory file. Using the configured one")
+        else:
+            logger.logger.fatal("No inventory")
+
         lockpath = os.path.join(os.path.join(configuration.conf["global_paths"]["work_dir"],
                                 "locks") , inv_file.lstrip(f".{os.sep}").replace(os.sep, "_"))
         lock = Locking(logger.logger, options["keep_locked"], (options["infra"], options["stage"]),
                        configuration.conf)
         if options["subcommand"] in ("run", "verify"):
             if not validators.verify_task_permissions(selected_items, user_groups, config):
                 logger.logger.critical("Task forbidden")
@@ -157,18 +170,20 @@
             db_connector, db_path = DbSetup.connect_to_db(DbSetup(logger.logger, start_ts,
                                                           configuration.conf, options))
             db_writer = DbWriter(logger.logger, db_connector, db_path)
             runner = Runners(logger.logger, lock, workdir, start_ts_raw,
                              config["tasks"]["setup_hooks"], log_path, db_path)
             if not options["self_setup"]:
                 runner.setup_ansible(selected_items["commit"], configuration.conf_dir)
-            lock.lock_inventory(lockpath)
+            if options["lock"]:
+                lock.lock_inventory(lockpath)
             sequence_record_dict = runner.run_playitem(config, options, inv_file, lockpath,
                                                        db_writer)
-            lock.unlock_inventory(lockpath)
+            if options["lock"]:
+                lock.unlock_inventory(lockpath)
             db_writer.finalize_db_write(sequence_record_dict, False)
         elif options["subcommand"] == "lock":
             lock.lock_inventory(lockpath)
         elif options["subcommand"] == "unlock":
             lock.unlock_inventory(lockpath)
 
     sys.exit(0)
```

### Comparing `ansible-deployer-0.0.44/LICENSE` & `ansible_deployer-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/README.md` & `ansible_deployer-0.0.46/README.md`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/setup.cfg` & `ansible_deployer-0.0.46/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansible-deployer
-version = 0.0.44
+version = 0.0.46
 description = Wrapper around ansible-playbook allowing configurable tasks and permissions
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/cinek810/ansible-deployer
 author = J. Wierzbowski, M. Stolarek
 author_email = 
 license = MIT
```

### Comparing `ansible-deployer-0.0.44/setup.py` & `ansible_deployer-0.0.46/setup.py`

 * *Files identical despite different names*

### Comparing `ansible-deployer-0.0.44/PKG-INFO` & `ansible_deployer-0.0.46/ansible_deployer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-deployer
-Version: 0.0.44
+Version: 0.0.46
 Summary: Wrapper around ansible-playbook allowing configurable tasks and permissions
 Home-page: https://github.com/cinek810/ansible-deployer
 Author: J. Wierzbowski, M. Stolarek
 Author-email: 
 License: MIT
 Project-URL: Source, https://github.com/cinek810/ansible-deployer
 Platform: linux
@@ -20,14 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Clustering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
+Requires-Dist: pyyaml>=5.3.1
+Requires-Dist: cerberus>=1.3.1
+Requires-Dist: pytest-testinfra>=6.6.0
 
 # ansible-deployer
 However ansible is a great tool for IT infrastructure automation in certain cases it's hard to use
 it for the complete deployment, because of that tools like ansible-tower/AWX try to wrap it's
 activity making further assumptions on the way ansible code is stored (versioning repository), the
 way it's executed - certain combinations of inventory/playbook/tag options used to achieve specific
 goals. Having it in mind ansible-deployer may be treated as yet another ansible-playbook wrapper, but
@@ -47,9 +50,7 @@
 - `tasks.yaml` - Configuration of tasks (sets of playbooks to be executed)
 - `infra.yaml` - Configuration of infrastructures and stages of those mapping to ansible inventory
 
 ## Examples
 ```
 ansible-deployer run --task updateUsers --infra webServers --stage prod
 ```
-
-
```

