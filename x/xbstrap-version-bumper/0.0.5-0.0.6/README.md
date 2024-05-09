# Comparing `tmp/xbstrap_version_bumper-0.0.5.tar.gz` & `tmp/xbstrap_version_bumper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbstrap_version_bumper-0.0.5.tar", last modified: Tue May  7 14:07:32 2024, max compression
+gzip compressed data, was "xbstrap_version_bumper-0.0.6.tar", last modified: Thu May  9 12:37:54 2024, max compression
```

## Comparing `xbstrap_version_bumper-0.0.5.tar` & `xbstrap_version_bumper-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-07 14:07:32.516481 xbstrap_version_bumper-0.0.5/
--rw-r--r--   0 alexander  (1000) wheel      (998)     1075 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/LICENSE
--rw-r--r--   0 alexander  (1000) wheel      (998)      873 2024-05-07 14:07:32.516481 xbstrap_version_bumper-0.0.5/PKG-INFO
--rw-r--r--   0 alexander  (1000) wheel      (998)      181 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/README.md
--rw-r--r--   0 alexander  (1000) wheel      (998)      834 2024-05-07 14:07:13.000000 xbstrap_version_bumper-0.0.5/pyproject.toml
--rw-r--r--   0 alexander  (1000) wheel      (998)       38 2024-05-07 14:07:32.516481 xbstrap_version_bumper-0.0.5/setup.cfg
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-07 14:07:32.514481 xbstrap_version_bumper-0.0.5/src/
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-07 14:07:32.515481 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/
--rw-r--r--   0 alexander  (1000) wheel      (998)        0 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/__init__.py
--rw-r--r--   0 alexander  (1000) wheel      (998)      102 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/__main__.py
--rw-r--r--   0 alexander  (1000) wheel      (998)     8430 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/linecounted_yaml.py
--rw-r--r--   0 alexander  (1000) wheel      (998)    14538 2024-05-07 14:06:27.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/main.py
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-07 14:07:32.515481 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/
--rw-r--r--   0 alexander  (1000) wheel      (998)      873 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/PKG-INFO
--rw-r--r--   0 alexander  (1000) wheel      (998)      494 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/SOURCES.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)        1 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/dependency_links.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       76 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/entry_points.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       73 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/requires.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       23 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/top_level.txt
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-09 12:37:54.867678 xbstrap_version_bumper-0.0.6/
+-rw-r--r--   0 alexander  (1000) wheel      (998)     1075 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.6/LICENSE
+-rw-r--r--   0 alexander  (1000) wheel      (998)      873 2024-05-09 12:37:54.867678 xbstrap_version_bumper-0.0.6/PKG-INFO
+-rw-r--r--   0 alexander  (1000) wheel      (998)      181 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.6/README.md
+-rw-r--r--   0 alexander  (1000) wheel      (998)      834 2024-05-09 12:37:44.000000 xbstrap_version_bumper-0.0.6/pyproject.toml
+-rw-r--r--   0 alexander  (1000) wheel      (998)       38 2024-05-09 12:37:54.867678 xbstrap_version_bumper-0.0.6/setup.cfg
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-09 12:37:54.866678 xbstrap_version_bumper-0.0.6/src/
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-09 12:37:54.866678 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper/
+-rw-r--r--   0 alexander  (1000) wheel      (998)        0 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper/__init__.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)      102 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper/__main__.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)     8430 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper/linecounted_yaml.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)    15707 2024-05-09 12:37:11.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper/main.py
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-09 12:37:54.867678 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper.egg-info/
+-rw-r--r--   0 alexander  (1000) wheel      (998)      873 2024-05-09 12:37:54.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper.egg-info/PKG-INFO
+-rw-r--r--   0 alexander  (1000) wheel      (998)      494 2024-05-09 12:37:54.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)        1 2024-05-09 12:37:54.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       76 2024-05-09 12:37:54.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper.egg-info/entry_points.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       73 2024-05-09 12:37:54.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper.egg-info/requires.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       23 2024-05-09 12:37:54.000000 xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper.egg-info/top_level.txt
```

### Comparing `xbstrap_version_bumper-0.0.5/LICENSE` & `xbstrap_version_bumper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xbstrap_version_bumper-0.0.5/PKG-INFO` & `xbstrap_version_bumper-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbstrap_version_bumper
-Version: 0.0.5
+Version: 0.0.6
 Summary: xbstrap distro auto version bumper
 Author-email: Alexander Richards <electrodeyt@gmail.com>
 Project-URL: Homepage, https://github.com/ElectrodeYT/xbstrap_version_bumper
 Project-URL: Issues, https://github.com/ElectrodeYT/xbstrap_version_bumper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xbstrap_version_bumper-0.0.5/pyproject.toml` & `xbstrap_version_bumper-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xbstrap_version_bumper"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="Alexander Richards", email="electrodeyt@gmail.com" },
 ]
 requires-python = ">=3.8"
 description="xbstrap distro auto version bumper"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/linecounted_yaml.py` & `xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper/linecounted_yaml.py`

 * *Files identical despite different names*

### Comparing `xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/main.py` & `xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 import xbstrap_version_bumper.linecounted_yaml
 
 global_yaml = ruamel.yaml.YAML(typ='safe')
 global_yaml.Constructor = xbstrap_version_bumper.linecounted_yaml.MyConstructor
 
 
-def sort_versions(version_list: list) -> str:
-    return sorted(version_list, key=cmp_to_key(libversion.version_compare2))[-1]
+def sort_versions(version_list: list) -> []:
+    return sorted(version_list, key=cmp_to_key(libversion.version_compare2))
 
 
 class ProgressPrinter(RemoteProgress):
     def update(self, op_code, cur_count, max_count=None, message=""):
         print(
             op_code,
             cur_count,
@@ -150,17 +150,17 @@
 
         return False, False
 
     def __locate_package(self, package_name) -> tuple[Any, Any] | tuple[bool, bool]:
         for strapfile in self.strapfiles:
             if 'packages' in strapfile.yaml:
                 for package in strapfile.yaml['packages']:
-                    if 'source' in package and package['name'] == package_name:
+                    if package['name'] == package_name:
                         return strapfile, package
-
+        print(f'Could not find package: {package_name}')
         return False, False
 
     def __add_changes_to_stapfile(self, strapfile: StrapFile, changes: []):
         for i, actual_strapfile in enumerate(self.strapfiles):
             if actual_strapfile.path != strapfile.path:
                 continue
 
@@ -242,39 +242,62 @@
 
         if 'build' in package:
             for build in package['build']:
                 changes += self.__args_to_changes(build['args'], old_version, new_version, update_is_version=True)
 
         self.__add_changes_to_stapfile(strapfile, changes)
 
-    def __get_latest_git_version(self, source):
+    def __get_latest_git_version(self, source, package_name=None):
         if 'git' not in source:
             return False
         g = git.cmd.Git()
         blob = g.ls_remote(source['git'], sort='-v:refname', tags=True)
         available_versions = []
         for line in blob.split('\n'):
-            available_versions.append(line.split('/')[-1])
-        newest_version = sort_versions(available_versions)
-        print(f'---> Latest git tag: {newest_version}')
-
-        if newest_version[0] == 'v':
-            newest_version = newest_version[1:]
-        print(f'---> Latest version: {newest_version}')
+            ver = line.split('/')[-1]
+            if '^{}' in ver:
+                continue
+            if not any(char.isdigit() for char in ver):
+                print(f'-> NOTE: skipping version {ver} because it does not contain any number')
+                continue
+            if package_name is not None and package_name in ver:
+                ver = ver.replace(package_name, '')
+                if ver[0] in ['-', '_']:
+                    ver = ver[1:]
+            if ver[0] == 'v':
+                ver = ver[1:]
+            available_versions.append(ver)
+        sorted_versions = sort_versions(available_versions)
+        print(f'---> Latest git tag: {sorted_versions[-1]}')
+
+        # Try and find the latest version which is not a prerelease, fallback to latest git tag if
+        # none are found
+        newest_non_prerelease = None
+        for version in reversed(sorted_versions):
+            prerelease_chars = ['a', 'b']
+            if any(char in version for char in prerelease_chars):
+                print(f'-> NOTE: skipping version {version} because it appears to be a prerelease version')
+                continue
+            newest_non_prerelease = version
+            break
+
+        if newest_non_prerelease is None:
+            print('-> NOTE: couldnt find a non-prerelease version, falling back to prerelease version')
+            newest_non_prerelease = sorted_versions[-1]
 
-        return newest_version
+        return newest_non_prerelease
 
     def get_latest_git_version_of_package(self, package_name):
         strapfile, package = self.__locate_package(package_name)
         if 'source' in package:
-            return self.__get_latest_git_version(package['source'])
+            return self.__get_latest_git_version(package['source'], package_name)
         else:
             assert 'from_source' in package
             strapfile, source_in_package, source = self.__locate_source(package['from_source'])
-            return self.__get_latest_git_version(source)
+            return self.__get_latest_git_version(source, package_name)
 
     def get_latest_git_version_of_source(self, source_name):
         strapfile, source_in_package, source = self.__locate_source(source_name)
         return self.__get_latest_git_version(source)
 
     def emit_modified_yaml(self):
         for strapfile in self.strapfiles:
```

### Comparing `xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/PKG-INFO` & `xbstrap_version_bumper-0.0.6/src/xbstrap_version_bumper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbstrap_version_bumper
-Version: 0.0.5
+Version: 0.0.6
 Summary: xbstrap distro auto version bumper
 Author-email: Alexander Richards <electrodeyt@gmail.com>
 Project-URL: Homepage, https://github.com/ElectrodeYT/xbstrap_version_bumper
 Project-URL: Issues, https://github.com/ElectrodeYT/xbstrap_version_bumper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

