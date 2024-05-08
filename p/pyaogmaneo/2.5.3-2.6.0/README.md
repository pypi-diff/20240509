# Comparing `tmp/pyaogmaneo-2.5.3.tar.gz` & `tmp/pyaogmaneo-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.5.3.tar", last modified: Wed May  8 17:41:17 2024, max compression
+gzip compressed data, was "pyaogmaneo-2.6.0.tar", last modified: Wed May  8 22:24:20 2024, max compression
```

## Comparing `pyaogmaneo-2.5.3.tar` & `pyaogmaneo-2.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:41:17.221796 pyaogmaneo-2.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:41:17.221796 pyaogmaneo-2.5.3/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-08 17:41:17.221796 pyaogmaneo-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:41:17.221796 pyaogmaneo-2.5.3/pyaogmaneo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-08 17:41:17.000000 pyaogmaneo-2.5.3/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-08 17:41:17.000000 pyaogmaneo-2.5.3/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:41:17.000000 pyaogmaneo-2.5.3/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:41:17.000000 pyaogmaneo-2.5.3/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 17:41:17.000000 pyaogmaneo-2.5.3/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:41:17.221796 pyaogmaneo-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:41:17.217796 pyaogmaneo-2.5.3/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:41:17.221796 pyaogmaneo-2.5.3/source/pyaogmaneo/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-05-08 17:41:06.000000 pyaogmaneo-2.5.3/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:24:20.457277 pyaogmaneo-2.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:24:20.453277 pyaogmaneo-2.6.0/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-08 22:24:20.457277 pyaogmaneo-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:24:20.457277 pyaogmaneo-2.6.0/pyaogmaneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-08 22:24:20.000000 pyaogmaneo-2.6.0/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-08 22:24:20.000000 pyaogmaneo-2.6.0/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:24:20.000000 pyaogmaneo-2.6.0/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:24:20.000000 pyaogmaneo-2.6.0/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 22:24:20.000000 pyaogmaneo-2.6.0/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:24:20.457277 pyaogmaneo-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:24:20.453277 pyaogmaneo-2.6.0/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:24:20.457277 pyaogmaneo-2.6.0/source/pyaogmaneo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-08 22:24:10.000000 pyaogmaneo-2.6.0/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.5.3/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.6.0/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.3/CMakeLists.txt` & `pyaogmaneo-2.6.0/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG bb4dc1534e88351e2b331da2865e6746fcf1586a
+        GIT_TAG 4785a9cb987c3d7d8b9829dec46736cf708c77a5
     )
 
     FetchContent_MakeAvailable(AOgmaNeo)
 endif()
 
 FetchContent_Declare(
     pybind11
```

### Comparing `pyaogmaneo-2.5.3/LICENSE.md` & `pyaogmaneo-2.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.3/PKG-INFO` & `pyaogmaneo-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.5.3
+Version: 2.6.0
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.5.3/README.md` & `pyaogmaneo-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.3/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.6.0/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.5.3
+Version: 2.6.0
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.5.3/setup.py` & `pyaogmaneo-2.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.5.3",
+    version="2.6.0",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.5.3/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.6.0/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.3/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.6.0/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.3/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.6.0/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.3/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.6.0/source/pyaogmaneo/py_hierarchy.h`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #include "py_helpers.h"
 #include <aogmaneo/hierarchy.h>
 
 namespace py = pybind11;
 
 namespace pyaon {
-const int hierarchy_magic = 8221313;
+const int hierarchy_magic = 2121824;
 
 enum IO_Type {
     none = 0,
     prediction = 1,
     action = 2
 };
```

### Comparing `pyaogmaneo-2.5.3/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.6.0/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.3/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.6.0/source/pyaogmaneo/py_image_encoder.h`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #include "py_helpers.h"
 #include <aogmaneo/image_encoder.h>
 
 namespace py = pybind11;
 
 namespace pyaon {
-const int image_encoder_magic = 4153116;
+const int image_encoder_magic = 7557115;
 
 struct Image_Visible_Layer_Desc {
     std::tuple<int, int, int> size;
 
     int radius;
 
     Image_Visible_Layer_Desc(
```

### Comparing `pyaogmaneo-2.5.3/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.6.0/source/pyaogmaneo/py_module.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -94,17 +94,19 @@
                 return other;
             }
         );
 
     // bind params
     py::class_<aon::Encoder::Params>(m, "EncoderParams")
         .def(py::init<>())
-        .def_readwrite("scale", &aon::Encoder::Params::scale)
+        .def_readwrite("choice", &aon::Encoder::Params::choice)
+        .def_readwrite("vigilance", &aon::Encoder::Params::vigilance)
         .def_readwrite("lr", &aon::Encoder::Params::lr)
-        .def_readwrite("early_stop_cells", &aon::Encoder::Params::early_stop_cells);
+        .def_readwrite("active_ratio", &aon::Encoder::Params::active_ratio)
+        .def_readwrite("l_radius", &aon::Encoder::Params::l_radius);
 
     py::class_<aon::Decoder::Params>(m, "DecoderParams")
         .def(py::init<>())
         .def_readwrite("scale", &aon::Decoder::Params::scale)
         .def_readwrite("lr", &aon::Decoder::Params::lr)
         .def_readwrite("leak", &aon::Decoder::Params::leak);
 
@@ -201,19 +203,19 @@
         )
         .def_readwrite("size", &pyaon::Image_Visible_Layer_Desc::size)
         .def_readwrite("radius", &pyaon::Image_Visible_Layer_Desc::radius);
 
     // bind params
     py::class_<aon::Image_Encoder::Params>(m, "ImageEncoderParams")
         .def(py::init<>())
-        .def_readwrite("falloff", &aon::Image_Encoder::Params::falloff)
+        .def_readwrite("choice", &aon::Image_Encoder::Params::choice)
+        .def_readwrite("vigilance", &aon::Image_Encoder::Params::vigilance)
         .def_readwrite("lr", &aon::Image_Encoder::Params::lr)
         .def_readwrite("scale", &aon::Image_Encoder::Params::scale)
-        .def_readwrite("rr", &aon::Image_Encoder::Params::rr)
-        .def_readwrite("radius", &aon::Image_Encoder::Params::radius);
+        .def_readwrite("rr", &aon::Image_Encoder::Params::rr);
 
     py::class_<pyaon::Image_Encoder>(m, "ImageEncoder")
         .def(py::init<
                 const std::tuple<int, int, int>&,
                 const std::vector<pyaon::Image_Visible_Layer_Desc>&,
                 const std::string&,
                 const py::array_t<unsigned char>&
```

