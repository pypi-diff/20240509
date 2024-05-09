# Comparing `tmp/virtualmachine-1.3.1.tar.gz` & `tmp/virtualmachine-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtualmachine-1.3.1.tar", last modified: Wed May  8 12:35:33 2024, max compression
+gzip compressed data, was "virtualmachine-1.3.2.tar", last modified: Thu May  9 11:54:58 2024, max compression
```

## Comparing `virtualmachine-1.3.1.tar` & `virtualmachine-1.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.837546 virtualmachine-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-08 12:35:33.837546 virtualmachine-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/configure.ac
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:35:33.837546 virtualmachine-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/include/private/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/include/private/python.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/include/vmdetect/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/include/vmdetect/defs.h
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/include/vmdetect/virtualmachine.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/libvmdetect/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/libvmdetect/common.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/libvmdetect/os/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/libvmdetect/os/linux/
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/libvmdetect/os/linux/virtualmachine.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.833546 virtualmachine-1.3.1/src/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/python/get.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-08 12:35:32.000000 virtualmachine-1.3.1/src/python/init.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:35:33.837546 virtualmachine-1.3.1/virtualmachine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-08 12:35:33.000000 virtualmachine-1.3.1/virtualmachine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 12:35:33.000000 virtualmachine-1.3.1/virtualmachine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:35:33.000000 virtualmachine-1.3.1/virtualmachine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 12:35:33.000000 virtualmachine-1.3.1/virtualmachine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.523053 virtualmachine-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-09 11:54:58.523053 virtualmachine-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:54:58.523053 virtualmachine-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.519053 virtualmachine-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.519053 virtualmachine-1.3.2/src/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.523053 virtualmachine-1.3.2/src/include/private/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/src/include/private/python.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.523053 virtualmachine-1.3.2/src/include/vmdetect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/src/include/vmdetect/defs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/src/include/vmdetect/virtualmachine.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.523053 virtualmachine-1.3.2/src/libvmdetect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/src/libvmdetect/common.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.519053 virtualmachine-1.3.2/src/libvmdetect/os/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.523053 virtualmachine-1.3.2/src/libvmdetect/os/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/src/libvmdetect/os/linux/virtualmachine.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.523053 virtualmachine-1.3.2/src/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/src/python/get.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-09 11:54:57.000000 virtualmachine-1.3.2/src/python/init.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:54:58.523053 virtualmachine-1.3.2/virtualmachine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-09 11:54:58.000000 virtualmachine-1.3.2/virtualmachine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-09 11:54:58.000000 virtualmachine-1.3.2/virtualmachine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:54:58.000000 virtualmachine-1.3.2/virtualmachine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 11:54:58.000000 virtualmachine-1.3.2/virtualmachine.egg-info/top_level.txt
```

### Comparing `virtualmachine-1.3.1/LICENSE` & `virtualmachine-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.3.1/PKG-INFO` & `virtualmachine-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtualmachine
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python library to identify virtual machine.
 Home-page: https://github.com/PerryWerneck/vmdetect
 Author: Perry Werneck
 Author-email: perry.werneck@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `virtualmachine-1.3.1/README.md` & `virtualmachine-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.3.1/configure.ac` & `virtualmachine-1.3.2/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -116,23 +116,23 @@
 dnl ---------------------------------------------------------------------------
 PKG_CHECK_EXISTS
 
 dnl ---------------------------------------------------------------------------
 dnl Check for systemd
 dnl ---------------------------------------------------------------------------
 
-PKG_CHECK_MODULES( [SYSTEMD], [libsystemd], AC_DEFINE(HAVE_SYSTEMD,[],[Do we have systemd?]), AC_MSG_NOTICE([libsystemd not present.]) )
+dnl PKG_CHECK_MODULES( [SYSTEMD], [libsystemd], AC_DEFINE(HAVE_SYSTEMD,[],[Do we have systemd?]), AC_MSG_NOTICE([libsystemd not present.]) )
 AC_SUBST(SYSTEMD_CFLAGS)
 AC_SUBST(SYSTEMD_LIBS)
 
 dnl ---------------------------------------------------------------------------
 dnl Check for libdbus
 dnl ---------------------------------------------------------------------------
 
-dnl PKG_CHECK_MODULES( [DBUS], [dbus-1], AC_DEFINE(HAVE_DBUS,[],[Do we have d-bus?]), AC_MSG_NOTICE([ No DBUS support.]) )
+PKG_CHECK_MODULES( [DBUS], [dbus-1], AC_DEFINE(HAVE_DBUS,[],[Do we have d-bus?]), AC_MSG_NOTICE([ No DBUS support.]) )
 AC_SUBST(DBUS_LIBS)
 AC_SUBST(DBUS_CFLAGS)
 
 dnl ---------------------------------------------------------------------------
 dnl Check for wmi++
 dnl ---------------------------------------------------------------------------
```

### Comparing `virtualmachine-1.3.1/setup.py` & `virtualmachine-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 with open(r'configure.ac', 'r') as fp:
     lines = fp.readlines()
     for line in lines:
         if line.find('AC_INIT') != -1:
             package_version = line.split('[')[2].split(']')[0].strip()
             break;
 
-package_version += '.1'
+package_version += '.2'
 extra_compile_args.append('-DPACKAGE_VERSION=\"' + package_version + '\"')
 
 if platform.system() == 'Windows':
 
 	include_dirs.append('src/libvmdetect/os/windows/wmi/include')
 	
 	for filename in glob.glob("src/libvmdetect/os/windows/*.cc"):
```

### Comparing `virtualmachine-1.3.1/src/include/private/python.h` & `virtualmachine-1.3.2/src/include/private/python.h`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.3.1/src/include/vmdetect/defs.h` & `virtualmachine-1.3.2/src/include/vmdetect/defs.h`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.3.1/src/include/vmdetect/virtualmachine.h` & `virtualmachine-1.3.2/src/include/vmdetect/virtualmachine.h`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.3.1/src/libvmdetect/common.cc` & `virtualmachine-1.3.2/src/libvmdetect/common.cc`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.3.1/src/python/get.cc` & `virtualmachine-1.3.2/src/python/get.cc`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.3.1/src/python/init.c` & `virtualmachine-1.3.2/src/python/init.c`

 * *Files identical despite different names*

### Comparing `virtualmachine-1.3.1/virtualmachine.egg-info/PKG-INFO` & `virtualmachine-1.3.2/virtualmachine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtualmachine
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python library to identify virtual machine.
 Home-page: https://github.com/PerryWerneck/vmdetect
 Author: Perry Werneck
 Author-email: perry.werneck@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

