# Comparing `tmp/CLUEstering-2.2.0.tar.gz` & `tmp/CLUEstering-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CLUEstering-2.2.0.tar", last modified: Tue Mar 19 17:23:11 2024, max compression
+gzip compressed data, was "CLUEstering-2.2.1.tar", last modified: Thu May  9 15:35:16 2024, max compression
```

## Comparing `CLUEstering-2.2.0.tar` & `CLUEstering-2.2.1.tar`

### file list

```diff
@@ -1,1711 +1,1714 @@
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.948049 CLUEstering-2.2.0/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.722047 CLUEstering-2.2.0/CLUEstering/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    41149 2024-03-19 17:22:14.000000 CLUEstering-2.2.0/CLUEstering/CLUEstering.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       93 2024-03-11 17:25:53.000000 CLUEstering-2.2.0/CLUEstering/__init__.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.702047 CLUEstering-2.2.0/CLUEstering/alpaka/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.725047 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1077 2024-03-16 23:51:45.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/AllocatorConfig.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1784 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/AllocatorPolicy.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7285 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/CachedBufAlloc.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18294 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/CachingAllocator.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2462 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/HostOnlyTask.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1824 2024-03-18 11:09:39.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/StreamCache.h
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.726047 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpaka/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1047 2024-03-16 23:52:18.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpaka/initialise.cc
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4610 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaConfig.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1047 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaDevices.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2861 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaFwd.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9987 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaMemory.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17312 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaWorkDiv.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      448 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/backend.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      774 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/chooseDevice.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2339 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/getDeviceCachingAllocator.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      891 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/getDeviceIndex.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      832 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/getHostCachingAllocator.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      740 2024-03-11 17:25:53.000000 CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/initialise.h
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.726047 CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4136 2024-03-11 17:25:53.000000 CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/Makefile
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9459 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_cpu.cc
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9425 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_cpu_tbb.cc
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9535 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_gpu_cuda.cc
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9485 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_gpu_hip.cc
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      596 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_kernels.cc
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.727047 CLUEstering-2.2.0/CLUEstering/alpaka/CLUE/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9818 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/CLUE/CLUEAlgoAlpaka.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13542 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/CLUE/CLUEAlpakaKernels.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2296 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/CLUE/ConvolutionalKernel.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25011 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/CLUE/Run.h
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.727047 CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1353 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/Points.h
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.727047 CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/alpaka/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3062 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/alpaka/AlpakaVecArray.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2928 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/alpaka/PointsAlpaka.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3566 2024-03-19 15:28:58.000000 CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/alpaka/TilesAlpaka.h
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.723047 CLUEstering-2.2.0/CLUEstering.egg-info/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11695 2024-03-19 17:23:11.000000 CLUEstering-2.2.0/CLUEstering.egg-info/PKG-INFO
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    82995 2024-03-19 17:23:11.000000 CLUEstering-2.2.0/CLUEstering.egg-info/SOURCES.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        1 2024-03-19 17:23:11.000000 CLUEstering-2.2.0/CLUEstering.egg-info/dependency_links.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       37 2024-03-19 17:23:11.000000 CLUEstering-2.2.0/CLUEstering.egg-info/requires.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       12 2024-03-19 17:23:11.000000 CLUEstering-2.2.0/CLUEstering.egg-info/top_level.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7749 2024-03-17 09:03:55.000000 CLUEstering-2.2.0/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    35149 2024-03-11 17:25:53.000000 CLUEstering-2.2.0/LICENSE
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       99 2024-03-11 17:25:53.000000 CLUEstering-2.2.0/MANIFEST.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11695 2024-03-19 17:23:11.948049 CLUEstering-2.2.0/PKG-INFO
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11153 2024-03-18 11:09:39.000000 CLUEstering-2.2.0/README.md
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.719047 CLUEstering-2.2.0/extern/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.729047 CLUEstering-2.2.0/extern/alpaka/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3509 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/.clang-format
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        5 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/.dockerignore
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       41 2024-03-11 23:17:10.000000 CLUEstering-2.2.0/extern/alpaka/.git
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.702047 CLUEstering-2.2.0/extern/alpaka/.github/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.730047 CLUEstering-2.2.0/extern/alpaka/.github/workflows/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    19162 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/.github/workflows/ci.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      553 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/.github/workflows/gh-pages.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      602 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/.gitignore
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1382 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/.gitlab-ci.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      362 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/.readthedocs.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4646 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/.zenodo.json
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    31544 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/CHANGELOG.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9451 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      797 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/CONTRIBUTING.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16725 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/LICENSE
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18694 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/README.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2450 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/README_OACC.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8040 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/README_OMP5.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9460 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/README_SYCL.md
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.730047 CLUEstering-2.2.0/extern/alpaka/cmake/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1172 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/cmake/addExecutable.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4013 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/cmake/addLibrary.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    45610 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/cmake/alpakaCommon.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2267 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/cmake/alpakaConfig.cmake.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8323 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/cmake/common.cmake
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.731047 CLUEstering-2.2.0/extern/alpaka/cmake/tests/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      460 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/cmake/tests/MathConstants.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      451 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/cmake/tests/StdAtomicRef.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.731047 CLUEstering-2.2.0/extern/alpaka/docs/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   112539 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/Doxyfile
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      742 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/Makefile
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.731047 CLUEstering-2.2.0/extern/alpaka/docs/cheatsheet/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      274 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/cheatsheet/README.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4066 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/cheatsheet/cheatsheet.style
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.732047 CLUEstering-2.2.0/extern/alpaka/docs/logo/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2381 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka.pdf
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7727 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka.svg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14785 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka_401x135.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5925 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka_doxygen.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9092 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka_inkscape.svg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      213 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/requirements.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.732047 CLUEstering-2.2.0/extern/alpaka/docs/source/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.733047 CLUEstering-2.2.0/extern/alpaka/docs/source/_static/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       38 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/_static/custom.css
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       75 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/_static/general.css
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.733047 CLUEstering-2.2.0/extern/alpaka/docs/source/advanced/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7072 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/advanced/cmake.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2960 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/advanced/compiler.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8330 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/advanced/mapping.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21301 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/advanced/rationale.rst
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.734047 CLUEstering-2.2.0/extern/alpaka/docs/source/basic/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    23216 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/basic/abstraction.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7398 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/basic/cheatsheet.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2502 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/basic/example.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2575 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/basic/install.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4364 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/basic/intro.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14041 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/basic/library.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5419 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/conf.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.735047 CLUEstering-2.2.0/extern/alpaka/docs/source/dev/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    60358 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/dev/backends.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9163 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/dev/ci.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15217 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/dev/details.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3837 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/dev/sphinx.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5006 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/dev/style.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4523 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/dev/test.rst
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.739047 CLUEstering-2.2.0/extern/alpaka/docs/source/images/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   190358 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/arch_gitlab_mirror.svg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    79386 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/block.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    56667 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/block_scale.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17754 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/element.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25138 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/execution_domain.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    41233 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/execution_domain.svg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    48669 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/job_generator_flow.svg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   146807 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/structure.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   555186 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/structure.svg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    44965 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/structure_assoc.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   151677 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/structure_assoc.svg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    61721 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/thread.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    71863 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/warp.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    45242 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/x86_cpu.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    35114 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/images/x86_cpu_mapping.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1792 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/index.rst
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.739047 CLUEstering-2.2.0/extern/alpaka/docs/source/info/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2501 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/docs/source/info/similar_projects.rst
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.739047 CLUEstering-2.2.0/extern/alpaka/example/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1827 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.739047 CLUEstering-2.2.0/extern/alpaka/example/babelstream/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1657 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/babelstream/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.740047 CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7853 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/AlpakaStream.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1668 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/AlpakaStream.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1999 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/LICENSE
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      480 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/README.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      987 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/Stream.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    19493 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/main.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.740047 CLUEstering-2.2.0/extern/alpaka/example/bufferCopy/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2219 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/bufferCopy/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.740047 CLUEstering-2.2.0/extern/alpaka/example/bufferCopy/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11283 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/bufferCopy/src/bufferCopy.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.740047 CLUEstering-2.2.0/extern/alpaka/example/complex/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2041 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/complex/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.740047 CLUEstering-2.2.0/extern/alpaka/example/complex/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3695 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/complex/src/complex.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.741047 CLUEstering-2.2.0/extern/alpaka/example/counterBasedRng/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2051 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/counterBasedRng/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.741047 CLUEstering-2.2.0/extern/alpaka/example/counterBasedRng/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9459 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/counterBasedRng/src/counterBasedRng.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.741047 CLUEstering-2.2.0/extern/alpaka/example/heatEquation/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2028 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/heatEquation/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.741047 CLUEstering-2.2.0/extern/alpaka/example/heatEquation/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7120 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/heatEquation/src/heatEquation.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.741047 CLUEstering-2.2.0/extern/alpaka/example/helloWorld/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2036 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/helloWorld/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.741047 CLUEstering-2.2.0/extern/alpaka/example/helloWorld/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8167 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/helloWorld/src/helloWorld.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.741047 CLUEstering-2.2.0/extern/alpaka/example/helloWorldLambda/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2048 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/helloWorldLambda/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.742047 CLUEstering-2.2.0/extern/alpaka/example/helloWorldLambda/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5592 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/helloWorldLambda/src/helloWorldLambda.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.742047 CLUEstering-2.2.0/extern/alpaka/example/kernelSpecialization/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2074 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/kernelSpecialization/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.742047 CLUEstering-2.2.0/extern/alpaka/example/kernelSpecialization/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4839 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/kernelSpecialization/src/kernelSpecialization.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.742047 CLUEstering-2.2.0/extern/alpaka/example/monteCarloIntegration/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2046 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/monteCarloIntegration/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.742047 CLUEstering-2.2.0/extern/alpaka/example/monteCarloIntegration/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5786 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/monteCarloIntegration/src/monteCarloIntegration.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.742047 CLUEstering-2.2.0/extern/alpaka/example/openMPSchedule/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2062 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/openMPSchedule/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.742047 CLUEstering-2.2.0/extern/alpaka/example/openMPSchedule/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6269 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/openMPSchedule/src/openMPSchedule.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.743047 CLUEstering-2.2.0/extern/alpaka/example/parallelLoopPatterns/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2044 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/parallelLoopPatterns/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.743047 CLUEstering-2.2.0/extern/alpaka/example/parallelLoopPatterns/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22365 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/parallelLoopPatterns/src/parallelLoopPatterns.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.743047 CLUEstering-2.2.0/extern/alpaka/example/randomCells2D/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2045 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/randomCells2D/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.743047 CLUEstering-2.2.0/extern/alpaka/example/randomCells2D/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11232 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/randomCells2D/src/randomCells2D.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.743047 CLUEstering-2.2.0/extern/alpaka/example/randomStrategies/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2051 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/randomStrategies/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.743047 CLUEstering-2.2.0/extern/alpaka/example/randomStrategies/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11677 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/randomStrategies/src/randomStrategies.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.743047 CLUEstering-2.2.0/extern/alpaka/example/reduce/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2093 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/reduce/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      554 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/reduce/README.md
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.744047 CLUEstering-2.2.0/extern/alpaka/example/reduce/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4793 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/reduce/src/alpakaConfig.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10582 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/reduce/src/iterator.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5377 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/reduce/src/kernel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6189 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/reduce/src/reduce.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.744047 CLUEstering-2.2.0/extern/alpaka/example/tagSpecialization/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2069 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/tagSpecialization/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.744047 CLUEstering-2.2.0/extern/alpaka/example/tagSpecialization/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4807 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/tagSpecialization/src/tagSpecialization.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.744047 CLUEstering-2.2.0/extern/alpaka/example/vectorAdd/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2022 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/vectorAdd/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.745047 CLUEstering-2.2.0/extern/alpaka/example/vectorAdd/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7917 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/example/vectorAdd/src/vectorAdd.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.706047 CLUEstering-2.2.0/extern/alpaka/include/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.745047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.748047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8658 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuOmp2Blocks.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9113 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuOmp2Threads.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8225 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuSerial.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3426 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8120 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuTbbBlocks.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9527 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuThreads.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2657 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccDevProps.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3442 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccFpgaSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3431 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccFpgaSyclXilinx.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8408 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1061 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGpuCudaRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1052 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGpuHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3403 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13963 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGpuUniformCudaHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14782 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccOacc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12192 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccOmp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2351 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/Tag.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2837 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/Traits.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9721 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/alpaka.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.751047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8097 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicAtomicRef.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      830 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicCpu.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11596 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1680 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicHierarchy.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1215 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicNoOp.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5103 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicOaccBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7531 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicOaccExtended.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11011 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicOmpBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3849 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicStdLibLock.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15345 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicUniformCudaHip.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14966 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicUniformCudaHipBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7741 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/Op.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10912 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.706047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.751047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      802 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/OffloadUseBuiltInSharedMem.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.752047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      568 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedDynMemberAllocKiB.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1623 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4541 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynMember.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4149 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynOmp5BuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2033 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynUniformCudaHipBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1734 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.753047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2174 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2245 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStMember.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3455 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStMemberMasterSync.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2151 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStOmp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1971 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStOmp5BuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2124 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStUniformCudaHipBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2591 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.753047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/detail/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5720 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/detail/BlockSharedMemStMemberImpl.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.755047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1061 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierOacc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3422 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierOmp.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2078 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierThread.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2721 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1328 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncNoOp.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4310 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncUniformCudaHipBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3643 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.761047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2514 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Align.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      786 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/AlignedAlloc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14027 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ApiCudaRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14710 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ApiHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3486 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Assert.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5524 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/BarrierThread.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3214 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/BoostPredef.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2352 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/CallbackThread.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1025 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ClipCast.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7308 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Common.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2695 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Concepts.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15371 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ConcurrentExecPool.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2239 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Cuda.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13234 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/CudaHipCommon.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2351 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Debug.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1440 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Decay.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      802 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/DemangleTypeNames.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      648 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Hip.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1665 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Omp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3145 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/OmpSchedule.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1543 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Positioning.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      887 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/RemoveRestrict.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.761047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/STLTuple/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1306 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/STLTuple/LICENSE.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11822 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/STLTuple/STLTuple.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7945 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Sycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1259 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ThreadTraits.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1110 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Tuple.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8484 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/UniformCudaHip.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1134 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Unreachable.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      982 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Unroll.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2098 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Utility.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12035 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Vectorize.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.707047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/ctx/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.762047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/ctx/block/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9069 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/ctx/block/CtxBlockOacc.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.763047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5868 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevCpu.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      634 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevCpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      587 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevCudaRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      638 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevFpgaSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      571 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevFpgaSyclXilinx.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8157 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      600 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevGpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      581 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10945 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevOacc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9181 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevOmp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7985 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevUniformCudaHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3679 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.764047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/common/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3186 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/common/QueueRegistry.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.764047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/cpu/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7999 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/cpu/SysInfo.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1087 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/cpu/Wait.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.764047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dim/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      645 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dim/DimArithmetic.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      532 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dim/DimIntegralConst.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      709 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/dim/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.765047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/elem/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1083 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/elem/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.767048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      471 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventCpu.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      639 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventCpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      594 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventCudaRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      643 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventFpgaSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      610 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventFpgaSyclXilinx.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5567 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17228 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventGenericThreads.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      639 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventGpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      588 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      675 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventOacc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      673 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventOmp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10765 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventUniformCudaHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1412 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.767048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/example/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2863 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/example/ExampleDefaultAcc.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.767048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/extent/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5233 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/extent/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.768047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5073 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/Accessors.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10906 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/MapIdx.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1157 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.769047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2709 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2654 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtLinear.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2885 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtOmp.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2922 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtRefThreadIdMap.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3131 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtUniformCudaHipBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1902 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtZero.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.769047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/gb/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2652 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/gb/IdxGbGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2707 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/gb/IdxGbLinear.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2060 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/gb/IdxGbRef.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3119 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/gb/IdxGbUniformCudaHipBuiltIn.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.770048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2937 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/IntrinsicCpu.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2388 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/IntrinsicFallback.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1902 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/IntrinsicGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2747 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/IntrinsicUniformCudaHipBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3249 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.774047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    41708 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuOmp2Blocks.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8575 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuOmp2Threads.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5505 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuSerial.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      821 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6014 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuTbbBlocks.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11379 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuThreads.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      826 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelFpgaSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      793 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelFpgaSyclXilinx.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10306 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      707 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGpuCudaRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      702 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGpuHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      822 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20385 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGpuUniformCudaHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10008 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelOacc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11715 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelOmp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12386 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.775047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18541 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/Complex.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2439 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/FloatEqualExact.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22690 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/MathGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9713 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/MathStdLib.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    50999 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/MathUniformCudaHipBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    49121 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.709047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.775047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/alloc/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3113 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/alloc/AllocCpuAligned.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1293 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/alloc/AllocCpuNew.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1643 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/alloc/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.778047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13064 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufCpu.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      679 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufCpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      614 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufCudaRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      684 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufFpgaSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      717 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufFpgaSyclXilinx.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9147 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      680 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufGpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      609 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10521 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufOacc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10478 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufOmp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16723 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufUniformCudaHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2356 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/SetKernel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8698 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.778047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/cpu/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9859 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/cpu/Copy.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7684 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/cpu/Set.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.779048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/oacc/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14135 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/oacc/Copy.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4541 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/oacc/Set.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.779048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/omp5/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14082 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/omp5/Copy.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4558 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/omp5/Set.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.780048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/sycl/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5057 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/sycl/Accessor.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1494 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/sycl/Common.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5643 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/sycl/Copy.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2935 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/sycl/Set.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.780048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29263 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/Copy.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15743 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/Set.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.782048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2562 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceCpu.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1984 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceCpuSerial.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3081 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2530 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceOacc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1670 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp2Blocks.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2371 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp2Threads.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1155 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2179 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceUniformCudaHipBuiltIn.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2529 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.784047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6888 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/Accessor.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25714 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/Traits.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5769 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewAccessOps.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9709 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewAccessor.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3702 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewConst.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11690 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewPlainPtr.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3094 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewStdArray.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3210 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewStdVector.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12638 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewSubView.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.787047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      885 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Apply.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3262 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/CartesianProduct.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      980 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Concatenate.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9804 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/CudaVectorArrayWrapper.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      656 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/DependentFalseType.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1715 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Filter.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      883 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Fold.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2071 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/ForEachType.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      902 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Functional.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      577 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/InheritFromList.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4468 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/IntegerSequence.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2691 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Integral.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1872 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/IsArrayOrVector.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      679 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/IsStrictBase.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4116 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/NdLoop.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1949 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Set.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      860 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Transform.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1129 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/TypeListOps.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1392 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Unique.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.787047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/offset/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4483 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/offset/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.789048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1963 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfCpu.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1901 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfCpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      586 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfCudaRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1251 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfFpgaSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1835 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfFpgaSyclXilinx.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29875 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1896 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfGpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      580 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1296 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfOacc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2973 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfOmp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15677 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfUniformCudaHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2834 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.793048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      684 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/Properties.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      499 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCpuBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      508 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCpuNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      629 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCpuSyclIntelBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      638 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCpuSyclIntelNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      620 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCudaRtBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      633 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCudaRtNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      634 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueFpgaSyclIntelBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      642 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueFpgaSyclIntelNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      600 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueFpgaSyclXilinxBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      609 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueFpgaSyclXilinxNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      610 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGenericSyclBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      580 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGenericSyclNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6101 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGenericThreadsBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7379 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGenericThreadsNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      629 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGpuSyclIntelBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      638 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGpuSyclIntelNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      614 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueHipRtBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      627 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueHipRtNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      714 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueOaccBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      723 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueOaccNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      712 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueOmp5Blocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      721 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueOmp5NonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      656 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueUniformCudaHipRtBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      664 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueUniformCudaHipRtNonBlocking.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2780 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.793048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/cpu/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      570 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/cpu/ICpuQueue.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1221 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/cpu/IGenericThreadsQueue.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.793048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/cuda_hip/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12770 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/cuda_hip/QueueUniformCudaHipRt.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.794048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/sycl/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9445 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/sycl/QueueGenericSyclBase.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.795048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.796048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1547 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/MultiplyAndSplit64to32.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3468 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseCommon.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2299 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseCudaArray.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1030 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseStdArray.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4198 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseTraits.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2344 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxConstants.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5822 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxSingle.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4604 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxStateless.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1324 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxStatelessKeyedBase.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1103 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxStatelessVector.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3654 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxVector.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7719 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandDefault.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7696 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandPhilox.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1729 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandPhiloxStateless.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8983 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandStdLib.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9900 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandUniformCudaHipRand.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.797048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/TinyMT/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1666 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/TinyMT/Engine.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1884 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/TinyMT/LICENSE.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12410 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/TinyMT/tinymt32.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4156 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.799048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      382 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/AnyOacc.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      383 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/AnyOmp5.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      393 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/CpuOmp2Blocks.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      393 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/CpuOmp2Threads.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      391 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/CpuSerial.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      550 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/CpuSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      391 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/CpuTbbBlocks.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      399 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/CpuThreads.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      554 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/FpgaSyclIntel.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      478 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/FpgaSyclXilinx.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      364 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/GenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      714 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/GpuCudaRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      375 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/GpuHipRt.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      550 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/GpuSyclIntel.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.799048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      845 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/Array.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2488 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/Check.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1471 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/Extent.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2757 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/KernelExecutionFixture.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1863 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/MeasureKernelRunTime.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.800048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/acc/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12217 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/acc/TestAccs.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.800048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/dim/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      911 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/dim/TestDims.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.800048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/event/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29108 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/event/EventHostManualTrigger.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.800048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/idx/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      912 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/idx/TestIdxs.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.710047 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/mem/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.800048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/mem/view/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6100 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/mem/view/Iterator.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9422 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/mem/view/ViewTest.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.801048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/queue/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9066 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/queue/Queue.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11686 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/queue/QueueCpuOmp2Collective.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      761 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/queue/QueueTestFixture.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.801048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/traits/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1273 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/traits/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.801048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/vec/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3862 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/vec/Traits.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    28372 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/vec/Vec.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      604 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/version.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.801048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/wait/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1512 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/wait/Traits.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.802048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/warp/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8440 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/warp/Traits.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4504 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/warp/WarpGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2376 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/warp/WarpSingleThread.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4857 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/warp/WarpUniformCudaHipBuiltIn.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.803048 CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2825 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/Traits.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4424 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/WorkDivGenericSycl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18369 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/WorkDivHelpers.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5835 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/WorkDivMembers.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4977 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/WorkDivUniformCudaHipBuiltIn.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.807048 CLUEstering-2.2.0/extern/alpaka/script/
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      439 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/after_failure.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     3857 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/before_install.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      574 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/ci.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     7813 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/docker_ci.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      922 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/docker_retry.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      668 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/gitlab_ci_run.sh
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.808048 CLUEstering-2.2.0/extern/alpaka/script/gitlabci/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      306 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/gitlabci/fake_sudo.sh
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      312 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/gitlabci/job_analysis.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3830 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/gitlabci/job_base.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1007 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/gitlabci/job_clang.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      922 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/gitlabci/job_cuda11.0.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      769 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/gitlabci/job_cuda11.8.yml
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1806 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/gitlabci/print_env.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     3646 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1239 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_analysis.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     6780 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_boost.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     3890 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_clang.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2485 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_cmake.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     9106 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_cuda.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      429 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_doxygen.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1344 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_gcc.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2583 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_hip.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      415 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_omp.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1440 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_oneapi.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2063 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/install_tbb.sh
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.810048 CLUEstering-2.2.0/extern/alpaka/script/job_generator/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1639 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/alpaka_filter.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      925 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/alpaka_globals.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2619 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/custom_job.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20508 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/generate_job_yaml.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7170 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/job_generator.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6277 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/job_modifier.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      847 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/reorder_jobs.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       78 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/requirements.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1021 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/verify.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3423 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/job_generator/versions.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     5047 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/prepare_sanitizers.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      787 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/print_env.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      637 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/push_doc.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     4266 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/run.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      889 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/run_analysis.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      729 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/run_build.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1131 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/run_doxygen.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     4016 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/run_generate.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      540 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/run_install.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1362 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/run_tests.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      687 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/set.sh
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1685 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/script/travis_retry.sh
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.810048 CLUEstering-2.2.0/extern/alpaka/test/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      618 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.810048 CLUEstering-2.2.0/extern/alpaka/test/analysis/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      776 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/analysis/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.810048 CLUEstering-2.2.0/extern/alpaka/test/analysis/headerCheck/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2181 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/analysis/headerCheck/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.811048 CLUEstering-2.2.0/extern/alpaka/test/analysis/headerCheck/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      416 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/analysis/headerCheck/src/main.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.811048 CLUEstering-2.2.0/extern/alpaka/test/common/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2719 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/common/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10684 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/common/devCompileOptions.cmake
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.811048 CLUEstering-2.2.0/extern/alpaka/test/integ/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      997 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.811048 CLUEstering-2.2.0/extern/alpaka/test/integ/axpy/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      688 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/axpy/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.811048 CLUEstering-2.2.0/extern/alpaka/test/integ/axpy/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7077 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/axpy/src/axpy.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.811048 CLUEstering-2.2.0/extern/alpaka/test/integ/cudaOnly/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      769 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/cudaOnly/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.812048 CLUEstering-2.2.0/extern/alpaka/test/integ/cudaOnly/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1633 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/cudaOnly/src/cudaNativeFunctions.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.812048 CLUEstering-2.2.0/extern/alpaka/test/integ/hostOnlyAPI/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      796 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/hostOnlyAPI/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.812048 CLUEstering-2.2.0/extern/alpaka/test/integ/hostOnlyAPI/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4547 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/hostOnlyAPI/src/hostOnlyAPI.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.812048 CLUEstering-2.2.0/extern/alpaka/test/integ/mandelbrot/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      694 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/mandelbrot/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.812048 CLUEstering-2.2.0/extern/alpaka/test/integ/mandelbrot/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13253 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/mandelbrot/src/mandelbrot.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.812048 CLUEstering-2.2.0/extern/alpaka/test/integ/matMul/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      690 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/matMul/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.812048 CLUEstering-2.2.0/extern/alpaka/test/integ/matMul/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12437 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/matMul/src/matMul.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.813048 CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1171 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.813048 CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/include/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      362 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/include/mysqrt.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.813048 CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5886 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/src/main.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      711 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/src/mysqrt.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.813048 CLUEstering-2.2.0/extern/alpaka/test/integ/sharedMem/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      693 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/sharedMem/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.813048 CLUEstering-2.2.0/extern/alpaka/test/integ/sharedMem/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6902 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/sharedMem/src/sharedMem.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.813048 CLUEstering-2.2.0/extern/alpaka/test/integ/zeroDimBuffer/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      735 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/zeroDimBuffer/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.814048 CLUEstering-2.2.0/extern/alpaka/test/integ/zeroDimBuffer/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4856 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/integ/zeroDimBuffer/src/zeroDimBuffer.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      473 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/sanitizer_lsan_blacklist.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      928 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/sanitizer_ubsan_blacklist.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.814048 CLUEstering-2.2.0/extern/alpaka/test/unit/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1406 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.814048 CLUEstering-2.2.0/extern/alpaka/test/unit/acc/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/acc/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.814048 CLUEstering-2.2.0/extern/alpaka/test/unit/acc/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1212 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/acc/src/AccDevPropsTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      612 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/acc/src/AccNameTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9113 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/acc/src/AccTagTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.815048 CLUEstering-2.2.0/extern/alpaka/test/unit/atomic/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      762 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/atomic/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.815048 CLUEstering-2.2.0/extern/alpaka/test/unit/atomic/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14908 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/atomic/src/AtomicTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.713047 CLUEstering-2.2.0/extern/alpaka/test/unit/block/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.815048 CLUEstering-2.2.0/extern/alpaka/test/unit/block/shared/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      773 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/block/shared/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.815048 CLUEstering-2.2.0/extern/alpaka/test/unit/block/shared/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2512 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/block/shared/src/BlockSharedMemDyn.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6079 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/block/shared/src/BlockSharedMemSt.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.815048 CLUEstering-2.2.0/extern/alpaka/test/unit/block/sharedSharing/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      800 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/block/sharedSharing/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.816048 CLUEstering-2.2.0/extern/alpaka/test/unit/block/sharedSharing/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5202 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/block/sharedSharing/src/BlockSharedMemSharing.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.816048 CLUEstering-2.2.0/extern/alpaka/test/unit/block/sync/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      769 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/block/sync/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.816048 CLUEstering-2.2.0/extern/alpaka/test/unit/block/sync/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3117 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/block/sync/src/BlockSync.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4115 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/block/sync/src/BlockSyncPredicate.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.816048 CLUEstering-2.2.0/extern/alpaka/test/unit/core/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      687 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/core/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.817048 CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1991 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/BoostPredefTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4292 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/ClipCastTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4905 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/ConceptsTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2103 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/OmpScheduleTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1170 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/Utility.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.817048 CLUEstering-2.2.0/extern/alpaka/test/unit/dev/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/dev/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.817048 CLUEstering-2.2.0/extern/alpaka/test/unit/dev/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      937 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/dev/src/DevWarpSizeTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.818048 CLUEstering-2.2.0/extern/alpaka/test/unit/event/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      688 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/event/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.818048 CLUEstering-2.2.0/extern/alpaka/test/unit/event/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8973 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/event/src/EventTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.818048 CLUEstering-2.2.0/extern/alpaka/test/unit/idx/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/idx/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.818048 CLUEstering-2.2.0/extern/alpaka/test/unit/idx/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1153 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/idx/src/MapIdx.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1972 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/idx/src/MapIdxPitchBytes.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.818048 CLUEstering-2.2.0/extern/alpaka/test/unit/intrinsic/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      768 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/intrinsic/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.819048 CLUEstering-2.2.0/extern/alpaka/test/unit/intrinsic/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2104 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/intrinsic/src/Ffs.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2111 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/intrinsic/src/Popcount.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.819048 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      762 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.820048 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1878 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelGenericLambda.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2922 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelLambda.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1883 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithAdditionalParam.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1717 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithConstructorAndMember.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1561 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithHostConstexpr.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5968 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithOmpSchedule.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2363 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithTemplate.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6113 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithTemplateArgumentDeduction.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4530 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithoutTemplatedAccParam.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.820048 CLUEstering-2.2.0/extern/alpaka/test/unit/math/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1317 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.822048 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4599 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/Buffer.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9707 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/DataGen.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4849 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/Defines.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2136 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/FloatEqualExactTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18799 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/Functor.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7264 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/TestTemplate.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9271 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathADL.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2783 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathComplexDouble.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2774 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathComplexFloat.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1379 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathDouble.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3865 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathFloat.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4063 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathLambda.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4616 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/powMixedTypes.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2078 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/sincos.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.715047 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.822048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/buf/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      763 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/buf/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.822048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/buf/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10888 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/buf/src/BufTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.823048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/copy/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1074 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/copy/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.823048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/copy/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6119 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/copy/src/BufSlicing.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.823048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/fence/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      742 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/fence/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.823048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/fence/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7404 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/fence/src/FenceTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.823048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/p2p/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      689 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/p2p/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.823048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/p2p/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2504 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/p2p/src/P2P.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.823048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      765 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.824048 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13635 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/Accessor.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5911 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/MdSpan.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4574 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/ViewConst.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7008 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/ViewPlainPtrTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4779 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/ViewStaticAccMem.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6799 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/ViewSubViewTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.824048 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      687 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.826048 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      773 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/ApplyTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1317 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/CartesianProductTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      929 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/ConcatenateTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7174 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/CudaVectorArrayWrapperTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      740 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/FilterTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    50223 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/IntegralTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1967 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/IsArrayOrVectorTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1609 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/IsStrictBaseTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      999 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/SetTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1226 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/TransformTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1386 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/TypeListOpsTest.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1063 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/UniqueTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.826048 CLUEstering-2.2.0/extern/alpaka/test/unit/queue/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      688 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/queue/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.827048 CLUEstering-2.2.0/extern/alpaka/test/unit/queue/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4512 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/queue/src/CollectiveQueue.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8039 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/queue/src/QueueTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.827048 CLUEstering-2.2.0/extern/alpaka/test/unit/rand/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      758 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/rand/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.827048 CLUEstering-2.2.0/extern/alpaka/test/unit/rand/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4873 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/rand/src/RandTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.827048 CLUEstering-2.2.0/extern/alpaka/test/unit/traits/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      708 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/traits/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.827048 CLUEstering-2.2.0/extern/alpaka/test/unit/traits/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      931 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/traits/src/NativeHandleTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.827048 CLUEstering-2.2.0/extern/alpaka/test/unit/vec/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/vec/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.828048 CLUEstering-2.2.0/extern/alpaka/test/unit/vec/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12541 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/vec/src/VecTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.828048 CLUEstering-2.2.0/extern/alpaka/test/unit/warp/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      758 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/warp/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.829048 CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4060 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/Activemask.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4036 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/All.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4036 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/Any.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4641 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/Ballot.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1526 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/GetSize.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5448 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/Shfl.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.829048 CLUEstering-2.2.0/extern/alpaka/test/unit/workDiv/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      690 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/workDiv/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.830048 CLUEstering-2.2.0/extern/alpaka/test/unit/workDiv/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4941 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/test/unit/workDiv/src/WorkDivHelpersTest.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.830048 CLUEstering-2.2.0/extern/alpaka/thirdParty/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       48 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/.clang-format
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1536 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.833048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      262 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.bazelrc
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1114 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.clang-format
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.716047 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.conan/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.833048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.conan/test_package/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      354 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.conan/test_package/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      592 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.conan/test_package/conanfile.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      365 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.conan/test_package/test_package.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      613 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.gitattributes
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.834048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       60 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/FUNDING.yml
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.834048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      711 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      308 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1066 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/pull_request_template.md
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.835048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      540 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/linux-bazel-builds.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1150 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/linux-meson-builds.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3756 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/linux-other-builds.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3562 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/linux-simple-builds.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1565 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/mac-builds.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      976 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/validate-header-guards.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      560 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.gitignore
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4063 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/BUILD.bazel
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.837048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      250 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/Catch2Config.cmake.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2432 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/CatchConfigOptions.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4238 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/CatchMiscFunctions.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5086 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/FindGcov.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12328 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/FindLcov.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8419 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/Findcodecov.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      337 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/catch2-with-main.pc.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      331 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/catch2.pc.in
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1071 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/llvm-cov-wrapper
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6750 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      837 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMakePresets.json
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3215 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CODE_OF_CONDUCT.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   108911 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/Doxyfile
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1338 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/LICENSE.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4045 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/README.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/SECURITY.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      559 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/WORKSPACE.bazel
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4361 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/appveyor.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      297 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/codecov.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2592 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/conanfile.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.717047 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.838048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/artwork/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10636 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/artwork/catch2-c-logo.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    33761 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/artwork/catch2-hand-logo.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25330 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/artwork/catch2-logo-small-with-background.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20939 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/artwork/catch2-logo-small.png
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.843048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1608 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/Readme.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6834 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/assertions.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11326 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/benchmarks.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5257 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/ci-and-misc.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13910 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/cmake-integration.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    27308 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/command-line.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      570 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/commercial-users.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6588 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/comparing-floating-point-numbers.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12560 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/configuration.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13234 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/contributing.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1292 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/deprecations.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1494 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/event-listeners.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3983 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/faq.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8484 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/generators.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6340 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/limitations.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2733 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/list-of-examples.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4954 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/logging.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13819 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/matchers.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4270 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/migrate-v2-to-v3.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6696 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/opensource-users.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4192 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/other-macros.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4137 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/own-main.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    75415 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/release-notes.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2822 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/release-process.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5861 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/reporter-events.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8414 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/reporters.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15309 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/test-cases-and-sections.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5668 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/test-fixtures.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4783 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/tostring.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8230 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/tutorial.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4163 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/usage-tips.md
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2992 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/why-catch.md
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.845048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1322 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/010-TestCase.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1031 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/020-TestCase-1.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1187 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/020-TestCase-2.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2784 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/030-Asn-Require-Check.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2517 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/100-Fix-Section.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2134 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/110-Fix-ClassFixture.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3028 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/120-Bdd-ScenarioGivenWhenThen.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14840 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/210-Evt-EventListeners.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1435 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/231-Cfg-OutputStreams.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2182 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/300-Gen-OwnGenerator.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1901 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/301-Gen-MapTypeConversion.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2183 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/302-Gen-Table.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1358 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/310-Gen-VariablesInGenerators.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1622 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/311-Gen-CustomCapture.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1561 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.847048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9169 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/Catch.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4389 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/CatchAddTests.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2136 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/CatchShardTests.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1642 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/CatchShardTestsImpl.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15008 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/ParseAndAddCatchTests.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   368375 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/catch_amalgamated.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   464259 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/catch_amalgamated.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      645 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/gdbinit
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      624 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/lldbinit
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.848048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/fuzzing/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      753 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/fuzzing/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      233 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/fuzzing/NullOStream.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      451 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/fuzzing/NullOStream.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      373 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/fuzzing/fuzz_TestSpecParser.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      327 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/fuzzing/fuzz_XmlWriter.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1127 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/fuzzing/fuzz_textflow.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      139 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/mdsnippets.json
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      417 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/meson.build
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.848048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20289 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.854048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.856048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6268 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_benchmark.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1903 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_benchmark_all.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      509 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_chronometer.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2624 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_chronometer.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1110 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_clock.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2642 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_constructor.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1168 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_environment.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      884 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_estimate.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2394 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_execution_plan.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2191 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_optimizer.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1005 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_outlier_classification.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1633 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_sample_analysis.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.858048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3411 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_analyse.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      522 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_benchmark_function.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4259 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_benchmark_function.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2308 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_complete_invoke.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5421 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_estimate_clock.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1176 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_measure.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1045 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_repeat.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      952 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_run_for_at_least.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2560 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_run_for_at_least.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10472 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_stats.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5905 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_stats.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      964 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_timing.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5882 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_all.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2565 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_approx.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4647 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_approx.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      791 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_info.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3367 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_result.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1835 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_result.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10544 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_config.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5314 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_config.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      483 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_get_random_seed.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      486 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_get_random_seed.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3930 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_message.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5609 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_message.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4462 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_registry_hub.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1239 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_section_info.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13135 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_session.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1764 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_session.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      698 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      879 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias_autoregistrar.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1083 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias_autoregistrar.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10642 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_template_test_macros.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9705 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_case_info.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3721 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_case_info.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14216 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_macros.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4187 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_spec.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3824 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_spec.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1195 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_timer.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      724 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_timer.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7497 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tostring.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20853 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tostring.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1744 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_totals.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      981 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_totals.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3168 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_translate_exception.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5805 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_user_config.hpp.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1286 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_version.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1182 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_version.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      461 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_version_macros.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.859048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      435 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generator_exception.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      868 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generator_exception.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1054 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8929 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8630 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_adapters.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1169 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_all.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      423 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_random.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2841 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_random.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3479 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_range.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.862048 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1573 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_all.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      370 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_capture.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3445 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_capture.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      355 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_config.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3235 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_config.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1540 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_enum_values_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      461 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_exception.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1194 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_exception.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      901 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_generatortracker.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3360 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_generatortracker.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      430 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_registry_hub.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2411 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_registry_hub.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3873 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10200 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      444 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_factory.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1433 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_factory.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      386 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_registry.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1400 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      854 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_tag_alias_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      422 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_testcase.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1532 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_testcase.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.880049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3347 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_assertion_handler.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2079 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_assertion_handler.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1164 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_insensitive_comparisons.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      975 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_insensitive_comparisons.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      454 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_sensitive.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17469 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_clara.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24910 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_clara.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14840 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_commandline.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      538 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_commandline.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3087 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_compare_traits.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16928 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_compiler_capabilities.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      955 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_android_logwrite.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      963 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_counter.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1315 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_uncaught_exceptions.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1010 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_wchar.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10897 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_colour.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4286 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_colour.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      624 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_width.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2160 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_container_nonmembers.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1689 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_context.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1595 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_context.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1228 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debug_console.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      464 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debug_console.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4416 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debugger.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2123 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debugger.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      771 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_decomposer.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16801 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_decomposer.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1152 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enforce.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1635 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enforce.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2716 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enum_values_registry.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1130 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enum_values_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      442 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_errno_guard.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      697 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_errno_guard.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3062 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_exception_translator_registry.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      984 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_exception_translator_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9067 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_fatal_condition_handler.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2271 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_fatal_condition_handler.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      923 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_floating_point_helpers.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3652 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_floating_point_helpers.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      933 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_getenv.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      526 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_getenv.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5195 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_istream.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1651 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_istream.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      913 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_lazy_expr.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1132 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_lazy_expr.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1144 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_leak_detector.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      471 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_leak_detector.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4364 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_list.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      928 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_list.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1285 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_logical_traits.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1407 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_main.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      753 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_message_info.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1219 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_message_info.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1468 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_meta.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      715 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_move_and_forward.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      856 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_noncopyable.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2756 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_optional.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4198 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_output_redirect.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3479 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_output_redirect.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1694 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_parse_numbers.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      765 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_parse_numbers.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1222 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_platform.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      807 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_polyfills.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      427 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_polyfills.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22187 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_preprocessor.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      765 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_preprocessor_remove_parens.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1869 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_number_generator.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2055 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_number_generator.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1020 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_seed_generation.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      685 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_seed_generation.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2934 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_registry.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1195 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6248 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_spec_parser.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2702 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_spec_parser.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      977 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_result_type.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1582 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_result_type.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2028 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reusable_string_stream.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1700 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reusable_string_stream.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25737 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_run_context.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5379 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_run_context.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1382 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_section.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1746 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_section.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1387 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_sharding.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1005 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_singletons.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1226 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_singletons.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1181 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_source_line_info.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1056 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_source_line_info.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      975 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_startup_exception_registry.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      812 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_startup_exception_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      638 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stdstreams.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      465 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stdstreams.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      827 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stream_end_stop.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3746 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_string_manip.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2062 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_string_manip.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2088 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stringref.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3779 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stringref.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2259 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_tag_alias_registry.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1042 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_tag_alias_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24029 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_template_test_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1283 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_info_hasher.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      710 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_info_hasher.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6100 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_registry_impl.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2733 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_registry_impl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7859 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_tracker.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5528 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_tracker.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      639 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_failure_exception.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      738 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_failure_exception.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7686 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_macro_impl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2916 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_registry.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5530 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_registry.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7560 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_spec_parser.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2219 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_spec_parser.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8596 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_textflow.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6125 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_textflow.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      777 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_to_string.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      788 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_uncaught_exceptions.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      461 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_uncaught_exceptions.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      815 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_unique_name.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3002 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_unique_ptr.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      619 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_void_type.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1777 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_wildcard_pattern.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1063 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_wildcard_pattern.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      764 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_windows_h_proxy.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11198 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_xmlwriter.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5373 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_xmlwriter.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.882049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      621 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10210 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1478 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_all.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      862 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_container_properties.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2905 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_container_properties.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3779 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_contains.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      721 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_exception.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      976 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_exception.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7531 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_floating_point.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3068 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_floating_point.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      529 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_predicate.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1857 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_predicate.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      851 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_quantifiers.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5494 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_quantifiers.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4488 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_string.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3313 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_string.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1424 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_templated.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13392 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_templated.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7649 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_vector.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.883049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1058 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/catch_matchers_impl.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3327 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/catch_matchers_impl.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12847 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/meson.build
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.887049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1175 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_automake.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1318 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_automake.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1690 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_common_base.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2950 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_common_base.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8792 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_compact.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1081 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_compact.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22030 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_console.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2356 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_console.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5917 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_cumulative_base.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6492 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_cumulative_base.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1944 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_event_listener.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2671 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_event_listener.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12937 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_helpers.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3289 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_helpers.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11976 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_junit.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1822 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_junit.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7106 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_multi.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2989 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_multi.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      993 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_registrars.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4763 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_registrars.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6175 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_sonarqube.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1963 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_sonarqube.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      667 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_streaming_base.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2909 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_streaming_base.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8662 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_tap.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1359 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_tap.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6635 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_teamcity.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1908 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_teamcity.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14298 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_xml.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2154 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_xml.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1763 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporters_all.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.887049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25205 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.891049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    19401 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      624 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/ToDo.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3612 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X01-PrefixedMacros.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1669 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X02-DisabledMacros.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1191 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X03-DisabledExceptions-DefaultHandler.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1061 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X04-DisabledExceptions-CustomHandler.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      567 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X05-DeferredStaticChecks.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      809 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X10-FallbackStringifier.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      646 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X11-DisableStringification.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      644 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X12-CustomDebugBreakMacro.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2474 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X21-PartialTestCaseEvents.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2362 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X22-BenchmarksInCumulativeReporter.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1182 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X23-CasingInReporterNames.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1330 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X24-ListenerStdoutCaptureInMultireporter.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1479 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X25-ListenerCanAskForCapturedStdout.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1363 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X26-ReporterPreferencesForPassingAssertionsIsRespected.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2837 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X27-CapturedStdoutInTestCaseEvents.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3235 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X28-ListenersGetEventsBeforeReporters.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1702 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X29-CustomArgumentsForReporters.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      490 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X30-BazelReporter.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      522 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X31-DuplicatedTestCases.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      551 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X32-DuplicatedTestCasesDifferentTags.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      625 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X33-DuplicatedTestCaseMethods.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      705 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X34-DuplicatedTestCaseMethodsDifferentFixtures.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      993 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X35-DuplicatedReporterNames.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      569 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X90-WindowsHeaderInclusion.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      950 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X91-AmalgamatedCatch.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      321 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X92-NoTests.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.892049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.897049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9171 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.std.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24238 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.sw.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24018 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.sw.multi.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   214711 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/compact.sw.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   214491 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/compact.sw.multi.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    50055 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.std.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   578273 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.sw.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   578053 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.sw.multi.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    32602 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.swa4.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      220 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/default.sw.multi.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   138530 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/junit.sw.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   138510 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/junit.sw.multi.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   110409 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/sonarqube.sw.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   110389 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/sonarqube.sw.multi.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   239558 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/tap.sw.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   239338 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/tap.sw.multi.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    91238 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/teamcity.sw.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    91218 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/teamcity.sw.multi.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   794014 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/xml.sw.approved.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   793994 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/xml.sw.multi.approved.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.901049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2993 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Clara.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15944 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/CmdLine.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4878 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/CmdLineHelpers.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1944 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/ColourImpl.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4418 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Details.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3092 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/FloatingPoint.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18674 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/GeneratorsImpl.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14665 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/InternalBenchmark.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1308 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Parse.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7792 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/PartTracker.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2078 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/RandomNumberGeneration.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13409 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Reporters.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1382 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Sharding.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1049 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Stream.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6719 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/String.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3386 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/StringManip.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3872 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Tag.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2368 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestCaseInfoHasher.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15392 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestSpec.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1770 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestSpecParser.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6606 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TextFlow.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4016 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/ToString.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2234 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Traits.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4500 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/UniquePtr.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7360 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Xml.tests.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.901049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Misc/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       41 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Misc/invalid-test-names.input
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       42 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Misc/plain-old-tests.input
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       41 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Misc/special-characters-in-file.input
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6734 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/TestRegistrations.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.901049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/TimingTests/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      632 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/TimingTests/Sleep.tests.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.905049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6686 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Approx.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3383 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/BDD.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5144 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Benchmark.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4575 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Class.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10150 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Compilation.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9154 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Condition.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      994 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Decomposition.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3758 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/EnumToString.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6414 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Exception.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9966 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Generators.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    38790 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Matchers.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29106 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/MatchersRanges.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8683 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Message.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16017 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Misc.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      767 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringByte.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1910 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringChrono.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5986 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringGeneral.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1176 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringOptional.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1506 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringPair.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1688 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringTuple.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3447 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringVariant.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3433 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringVector.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5234 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringWhich.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8730 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Tricky.tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      570 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/VariadicMacros.tests.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.905049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      617 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/parse_test_spec.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      546 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/parse_test_spec.hpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1596 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/type_with_lit_0_comparisons.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.907049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3039 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/ConfigureTestsCommon.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3048 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testBazelReporter.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2238 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testBazelSharding.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1337 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDefaultReporter.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1643 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDisable.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1488 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDisableStringification.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1564 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureExperimentalRedirect.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2368 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testPartialTestCaseEvent.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2689 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testRandomOrder.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     5608 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testSharding.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3266 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/meson.build
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.907049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/third_party/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    43554 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/third_party/clara.hpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.719047 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.908049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      416 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1273 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/appveyorBuildConfigurationScript.bat
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      317 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/appveyorMergeCoverageScript.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      708 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/appveyorTestRunScript.bat
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3997 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/coverage-helper.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1020 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/installOpenCppCoverage.ps1
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.910049 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     8687 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/approvalTests.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      916 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/approve.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     5030 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/checkConvenienceHeaders.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      288 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/checkDuplicateFilenames.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1213 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/checkLicense.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      196 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/developBuild.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3542 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/extractFeaturesFromReleaseNotes.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1401 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/fixWhitespace.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     5239 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/generateAmalgamatedFiles.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      197 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/majorRelease.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      197 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/minorRelease.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      196 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/patchRelease.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5725 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/releaseCommon.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      116 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/scriptCommon.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      816 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/updateDocumentSnippets.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)    13736 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/updateDocumentToC.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.912049 CLUEstering-2.2.0/extern/pybind11/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1271 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.appveyor.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      996 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.clang-format
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2605 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.clang-tidy
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2196 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.cmake-format.yaml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1308 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.codespell-ignore-lines
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       43 2024-03-11 23:17:33.000000 CLUEstering-2.2.0/extern/pybind11/.git
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       18 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.gitattributes
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.913049 CLUEstering-2.2.0/extern/pybind11/.github/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      182 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/CODEOWNERS
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15285 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.914049 CLUEstering-2.2.0/extern/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2561 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      328 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      162 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/dependabot.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      116 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/labeler.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       50 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/labeler_merged.yml
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.914049 CLUEstering-2.2.0/extern/pybind11/.github/matchers/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      668 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/matchers/pylint.json
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      645 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.915049 CLUEstering-2.2.0/extern/pybind11/.github/workflows/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    34361 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2272 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1491 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/workflows/format.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      641 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2628 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2876 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      502 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.gitignore
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3726 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      276 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/.readthedocs.yml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12422 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1684 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/LICENSE
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      247 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/MANIFEST.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7687 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/README.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      688 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/SECURITY.md
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.918049 CLUEstering-2.2.0/extern/pybind11/docs/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      607 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/Doxyfile
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7417 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/Makefile
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.719047 CLUEstering-2.2.0/extern/pybind11/docs/_static/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.918049 CLUEstering-2.2.0/extern/pybind11/docs/_static/css/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       37 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/_static/css/custom.css
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.919049 CLUEstering-2.2.0/extern/pybind11/docs/advanced/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.921049 CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3937 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3429 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14283 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3889 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1556 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12371 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9586 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9119 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    47796 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8460 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17846 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    26727 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16583 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.921049 CLUEstering-2.2.0/extern/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      278 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17161 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9030 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5710 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6377 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9240 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/basics.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2853 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/benchmark.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3168 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/benchmark.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   119653 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/changelog.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17090 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/classes.rst
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.922049 CLUEstering-2.2.0/extern/pybind11/docs/cmake/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      273 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/cmake/index.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25828 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/compiling.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11574 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/conf.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13293 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/faq.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      613 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/index.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3277 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/installing.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3079 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/limitations.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    61034 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    44653 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    87708 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    41121 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    85853 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2647 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/reference.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4957 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/release.rst
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      149 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/requirements.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24035 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.720047 CLUEstering-2.2.0/extern/pybind11/include/
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.925049 CLUEstering-2.2.0/extern/pybind11/include/pybind11/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24334 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/attr.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7750 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    67899 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/cast.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8458 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      120 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/common.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2096 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.926049 CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    28500 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    53681 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5962 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17858 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    28553 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    48358 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1625 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.926049 CLUEstering-2.2.0/extern/pybind11/include/pybind11/eigen/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      378 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/eigen/common.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    32135 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18442 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      316 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13459 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/embed.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4731 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/eval.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5002 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/functional.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8517 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/gil.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3876 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/gil_safe_call_once.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8862 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    80720 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9103 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/operators.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2734 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/options.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   128750 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    98893 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.927049 CLUEstering-2.2.0/extern/pybind11/include/pybind11/stl/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4185 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15477 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/stl.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29897 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1929 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/type_caster_pyobject_ptr.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3296 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/include/pybind11/typing.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2765 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/noxfile.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.927049 CLUEstering-2.2.0/extern/pybind11/pybind11/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      429 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/pybind11/__init__.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1544 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/pybind11/__main__.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      233 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/pybind11/_version.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1207 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/pybind11/commands.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/pybind11/py.typed
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17475 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2306 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/pyproject.toml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1495 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/setup.cfg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4855 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/setup.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.942049 CLUEstering-2.2.0/extern/pybind11/tests/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21733 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5619 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/conftest.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11736 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/constructor_stats.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3578 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1772 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      396 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      926 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/env.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.943049 CLUEstering-2.2.0/extern/pybind11/tests/extra_python_package/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8481 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.943049 CLUEstering-2.2.0/extern/pybind11/tests/extra_setuptools/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4153 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2847 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/local_bindings.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5743 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/object.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6256 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4517 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2685 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      768 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/pytest.ini
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      601 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/requirements.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      855 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_async.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      536 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_async.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10548 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7124 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_buffers.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16025 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17243 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4118 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6549 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_call_policies.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10858 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6955 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_callbacks.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3370 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5691 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_chrono.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24849 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_class.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14757 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_class.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.943049 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2584 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      673 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.944049 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1171 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.944049 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1293 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.944049 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1685 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      152 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.944049 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1353 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.944049 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1163 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.944049 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1368 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      198 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3831 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      593 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_const_name.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5710 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1551 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    26064 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4796 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_copy_move.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7280 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3992 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1259 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1091 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4557 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2423 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    19958 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_eigen_matrix.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29150 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_eigen_matrix.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      473 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_eigen_tensor.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10590 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_eigen_tensor.inl
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9414 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_eigen_tensor.py
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.945049 CLUEstering-2.2.0/extern/pybind11/tests/test_embed/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1798 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1315 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      543 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17396 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      237 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      275 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5722 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_enum.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9083 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_enum.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3168 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_eval.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1143 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_eval.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      119 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_eval_call.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13681 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      397 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_exceptions.h
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14165 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_exceptions.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18155 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16491 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5311 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8507 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3960 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7144 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_iostream.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11034 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14856 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4401 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8054 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22211 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18346 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4121 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_modules.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3963 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_modules.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12305 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11874 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20936 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22892 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21114 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14272 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4487 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9658 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2777 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1847 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9132 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4332 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6719 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2720 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_pickling.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    31789 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25066 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_pytypes.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21920 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8155 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18898 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9530 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21587 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_stl.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12307 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_stl.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6205 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9795 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4617 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      741 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1855 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_thread.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      826 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_thread.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4497 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_type_caster_pyobject_ptr.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3260 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_type_caster_pyobject_ptr.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      603 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_union.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      148 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_union.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      845 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_unnamed_namespace_a.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1141 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_unnamed_namespace_a.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      341 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_unnamed_namespace_b.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      143 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_unnamed_namespace_b.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1471 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_vector_unique_ptr_member.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      329 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_vector_unique_ptr_member.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22991 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12913 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3226 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2657 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-19 17:23:11.947049 CLUEstering-2.2.0/extern/pybind11/tools/
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2449 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3105 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12183 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      817 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1423 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/check-style.sh
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      952 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1117 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1031 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/libsize.py
--rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1311 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/make_changelog.py
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      196 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14449 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7101 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9607 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8564 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       94 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/pyproject.toml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2104 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/setup_global.py.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1234 2024-03-11 23:17:34.000000 CLUEstering-2.2.0/extern/pybind11/tools/setup_main.py.in
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      173 2024-03-11 17:25:53.000000 CLUEstering-2.2.0/pyproject.toml
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       38 2024-03-19 17:23:11.948049 CLUEstering-2.2.0/setup.cfg
--rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1035 2024-03-19 17:22:14.000000 CLUEstering-2.2.0/setup.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.716979 CLUEstering-2.2.1/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.324972 CLUEstering-2.2.1/CLUEstering/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    41702 2024-05-09 15:34:55.000000 CLUEstering-2.2.1/CLUEstering/CLUEstering.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       93 2024-03-11 17:25:53.000000 CLUEstering-2.2.1/CLUEstering/__init__.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.299971 CLUEstering-2.2.1/CLUEstering/alpaka/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.329972 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1077 2024-03-16 23:51:45.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/AllocatorConfig.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1784 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/AllocatorPolicy.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7285 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/CachedBufAlloc.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18294 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/CachingAllocator.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2462 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/HostOnlyTask.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1824 2024-04-08 19:33:54.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/StreamCache.h
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.329972 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpaka/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1047 2024-03-16 23:52:18.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpaka/initialise.cc
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4610 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaConfig.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1047 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaDevices.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2861 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaFwd.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9987 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaMemory.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17816 2024-05-09 15:33:20.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaWorkDiv.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      448 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/backend.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      774 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/chooseDevice.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2339 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/getDeviceCachingAllocator.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      891 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/getDeviceIndex.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      832 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/getHostCachingAllocator.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      740 2024-03-11 17:25:53.000000 CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/initialise.h
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.331972 CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4136 2024-05-03 09:19:25.000000 CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/Makefile
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9459 2024-05-03 10:03:42.000000 CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_cpu.cc
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9425 2024-05-03 10:03:42.000000 CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_cpu_tbb.cc
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9535 2024-05-03 10:03:42.000000 CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_gpu_cuda.cc
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9485 2024-05-03 10:03:42.000000 CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_gpu_hip.cc
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      596 2024-05-03 10:03:42.000000 CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_kernels.cc
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.332972 CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9818 2024-05-09 15:32:27.000000 CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/CLUEAlgoAlpaka.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13542 2024-05-09 15:32:27.000000 CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/CLUEAlpakaKernels.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2296 2024-05-03 10:03:42.000000 CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/ConvolutionalKernel.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25011 2024-05-03 10:03:42.000000 CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/Run.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4989 2024-05-03 07:59:59.000000 CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/binding.cc
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.332972 CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1353 2024-05-03 10:03:42.000000 CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/Points.h
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.333972 CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/alpaka/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3062 2024-05-09 15:32:27.000000 CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/alpaka/AlpakaVecArray.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2928 2024-04-29 14:58:04.000000 CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/alpaka/PointsAlpaka.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3566 2024-05-09 15:32:27.000000 CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/alpaka/TilesAlpaka.h
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.325971 CLUEstering-2.2.1/CLUEstering.egg-info/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11695 2024-05-09 15:35:16.000000 CLUEstering-2.2.1/CLUEstering.egg-info/PKG-INFO
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    83102 2024-05-09 15:35:16.000000 CLUEstering-2.2.1/CLUEstering.egg-info/SOURCES.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        1 2024-05-09 15:35:16.000000 CLUEstering-2.2.1/CLUEstering.egg-info/dependency_links.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       37 2024-05-09 15:35:16.000000 CLUEstering-2.2.1/CLUEstering.egg-info/requires.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       12 2024-05-09 15:35:16.000000 CLUEstering-2.2.1/CLUEstering.egg-info/top_level.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8234 2024-05-03 08:17:12.000000 CLUEstering-2.2.1/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    35149 2024-03-11 17:25:53.000000 CLUEstering-2.2.1/LICENSE
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       99 2024-03-11 17:25:53.000000 CLUEstering-2.2.1/MANIFEST.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11695 2024-05-09 15:35:16.716979 CLUEstering-2.2.1/PKG-INFO
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11153 2024-04-08 19:33:54.000000 CLUEstering-2.2.1/README.md
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.320971 CLUEstering-2.2.1/extern/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.337972 CLUEstering-2.2.1/extern/alpaka/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3509 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/.clang-format
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        5 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/.dockerignore
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       41 2024-03-11 23:17:10.000000 CLUEstering-2.2.1/extern/alpaka/.git
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.300971 CLUEstering-2.2.1/extern/alpaka/.github/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.337972 CLUEstering-2.2.1/extern/alpaka/.github/workflows/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    19162 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/.github/workflows/ci.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      553 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/.github/workflows/gh-pages.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      602 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/.gitignore
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1382 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/.gitlab-ci.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      362 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/.readthedocs.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4646 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/.zenodo.json
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    31544 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/CHANGELOG.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9451 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      797 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/CONTRIBUTING.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16725 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/LICENSE
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18694 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/README.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2450 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/README_OACC.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8040 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/README_OMP5.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9460 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/README_SYCL.md
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.338972 CLUEstering-2.2.1/extern/alpaka/cmake/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1172 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/cmake/addExecutable.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4013 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/cmake/addLibrary.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    45610 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/cmake/alpakaCommon.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2267 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/cmake/alpakaConfig.cmake.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8323 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/cmake/common.cmake
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.339972 CLUEstering-2.2.1/extern/alpaka/cmake/tests/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      460 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/cmake/tests/MathConstants.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      451 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/cmake/tests/StdAtomicRef.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.340972 CLUEstering-2.2.1/extern/alpaka/docs/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   112539 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/Doxyfile
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      742 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/Makefile
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.340972 CLUEstering-2.2.1/extern/alpaka/docs/cheatsheet/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      274 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/cheatsheet/README.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4066 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/cheatsheet/cheatsheet.style
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.343972 CLUEstering-2.2.1/extern/alpaka/docs/logo/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2381 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka.pdf
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7727 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka.svg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14785 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka_401x135.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5925 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka_doxygen.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9092 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka_inkscape.svg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      213 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/requirements.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.344972 CLUEstering-2.2.1/extern/alpaka/docs/source/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.344972 CLUEstering-2.2.1/extern/alpaka/docs/source/_static/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       38 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/_static/custom.css
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       75 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/_static/general.css
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.346972 CLUEstering-2.2.1/extern/alpaka/docs/source/advanced/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7072 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/advanced/cmake.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2960 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/advanced/compiler.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8330 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/advanced/mapping.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21301 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/advanced/rationale.rst
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.349972 CLUEstering-2.2.1/extern/alpaka/docs/source/basic/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    23216 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/basic/abstraction.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7398 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/basic/cheatsheet.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2502 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/basic/example.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2575 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/basic/install.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4364 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/basic/intro.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14041 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/basic/library.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5419 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/conf.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.351972 CLUEstering-2.2.1/extern/alpaka/docs/source/dev/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    60358 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/dev/backends.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9163 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/dev/ci.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15217 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/dev/details.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3837 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/dev/sphinx.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5006 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/dev/style.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4523 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/dev/test.rst
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.363972 CLUEstering-2.2.1/extern/alpaka/docs/source/images/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   190358 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/arch_gitlab_mirror.svg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    79386 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/block.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    56667 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/block_scale.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17754 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/element.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25138 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/execution_domain.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    41233 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/execution_domain.svg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    48669 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/job_generator_flow.svg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   146807 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/structure.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   555186 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/structure.svg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    44965 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/structure_assoc.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   151677 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/structure_assoc.svg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    61721 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/thread.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    71863 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/warp.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    45242 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/x86_cpu.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    35114 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/images/x86_cpu_mapping.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1792 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/index.rst
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.363972 CLUEstering-2.2.1/extern/alpaka/docs/source/info/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2501 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/docs/source/info/similar_projects.rst
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.363972 CLUEstering-2.2.1/extern/alpaka/example/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1827 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.364972 CLUEstering-2.2.1/extern/alpaka/example/babelstream/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1657 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/babelstream/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.365972 CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7853 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/AlpakaStream.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1668 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/AlpakaStream.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1999 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/LICENSE
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      480 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/README.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      987 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/Stream.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    19493 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/main.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.366972 CLUEstering-2.2.1/extern/alpaka/example/bufferCopy/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2219 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/bufferCopy/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.366972 CLUEstering-2.2.1/extern/alpaka/example/bufferCopy/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11283 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/bufferCopy/src/bufferCopy.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.366972 CLUEstering-2.2.1/extern/alpaka/example/complex/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2041 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/complex/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.366972 CLUEstering-2.2.1/extern/alpaka/example/complex/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3695 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/complex/src/complex.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.367972 CLUEstering-2.2.1/extern/alpaka/example/counterBasedRng/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2051 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/counterBasedRng/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.367972 CLUEstering-2.2.1/extern/alpaka/example/counterBasedRng/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9459 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/counterBasedRng/src/counterBasedRng.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.367972 CLUEstering-2.2.1/extern/alpaka/example/heatEquation/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2028 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/heatEquation/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.367972 CLUEstering-2.2.1/extern/alpaka/example/heatEquation/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7120 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/heatEquation/src/heatEquation.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.368972 CLUEstering-2.2.1/extern/alpaka/example/helloWorld/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2036 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/helloWorld/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.368972 CLUEstering-2.2.1/extern/alpaka/example/helloWorld/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8167 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/helloWorld/src/helloWorld.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.369972 CLUEstering-2.2.1/extern/alpaka/example/helloWorldLambda/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2048 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/helloWorldLambda/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.369972 CLUEstering-2.2.1/extern/alpaka/example/helloWorldLambda/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5592 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/helloWorldLambda/src/helloWorldLambda.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.369972 CLUEstering-2.2.1/extern/alpaka/example/kernelSpecialization/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2074 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/kernelSpecialization/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.370972 CLUEstering-2.2.1/extern/alpaka/example/kernelSpecialization/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4839 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/kernelSpecialization/src/kernelSpecialization.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.370972 CLUEstering-2.2.1/extern/alpaka/example/monteCarloIntegration/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2046 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/monteCarloIntegration/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.370972 CLUEstering-2.2.1/extern/alpaka/example/monteCarloIntegration/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5786 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/monteCarloIntegration/src/monteCarloIntegration.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.371972 CLUEstering-2.2.1/extern/alpaka/example/openMPSchedule/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2062 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/openMPSchedule/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.371972 CLUEstering-2.2.1/extern/alpaka/example/openMPSchedule/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6269 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/openMPSchedule/src/openMPSchedule.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.371972 CLUEstering-2.2.1/extern/alpaka/example/parallelLoopPatterns/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2044 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/parallelLoopPatterns/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.372972 CLUEstering-2.2.1/extern/alpaka/example/parallelLoopPatterns/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22365 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/parallelLoopPatterns/src/parallelLoopPatterns.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.372972 CLUEstering-2.2.1/extern/alpaka/example/randomCells2D/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2045 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/randomCells2D/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.372972 CLUEstering-2.2.1/extern/alpaka/example/randomCells2D/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11232 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/randomCells2D/src/randomCells2D.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.373972 CLUEstering-2.2.1/extern/alpaka/example/randomStrategies/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2051 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/randomStrategies/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.373972 CLUEstering-2.2.1/extern/alpaka/example/randomStrategies/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11677 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/randomStrategies/src/randomStrategies.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.374972 CLUEstering-2.2.1/extern/alpaka/example/reduce/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2093 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/reduce/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      554 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/reduce/README.md
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.375972 CLUEstering-2.2.1/extern/alpaka/example/reduce/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4793 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/reduce/src/alpakaConfig.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10582 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/reduce/src/iterator.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5377 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/reduce/src/kernel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6189 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/reduce/src/reduce.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.376973 CLUEstering-2.2.1/extern/alpaka/example/tagSpecialization/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2069 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/tagSpecialization/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.376973 CLUEstering-2.2.1/extern/alpaka/example/tagSpecialization/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4807 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/tagSpecialization/src/tagSpecialization.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.376973 CLUEstering-2.2.1/extern/alpaka/example/vectorAdd/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2022 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/vectorAdd/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.376973 CLUEstering-2.2.1/extern/alpaka/example/vectorAdd/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7917 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/example/vectorAdd/src/vectorAdd.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.304971 CLUEstering-2.2.1/extern/alpaka/include/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.377972 CLUEstering-2.2.1/extern/alpaka/include/alpaka/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.384973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8658 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuOmp2Blocks.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9113 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuOmp2Threads.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8225 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuSerial.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3426 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8120 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuTbbBlocks.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9527 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuThreads.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2657 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccDevProps.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3442 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccFpgaSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3431 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccFpgaSyclXilinx.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8408 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1061 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGpuCudaRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1052 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGpuHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3403 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13963 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGpuUniformCudaHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14782 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccOacc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12192 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccOmp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2351 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/Tag.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2837 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/Traits.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9721 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/alpaka.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.388973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8097 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicAtomicRef.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      830 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicCpu.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11596 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1680 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicHierarchy.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1215 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicNoOp.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5103 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicOaccBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7531 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicOaccExtended.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11011 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicOmpBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3849 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicStdLibLock.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15345 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicUniformCudaHip.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14966 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicUniformCudaHipBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7741 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/Op.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10912 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.304971 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.388973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      802 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/OffloadUseBuiltInSharedMem.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.389973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      568 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedDynMemberAllocKiB.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1623 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4541 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynMember.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4149 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynOmp5BuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2033 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynUniformCudaHipBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1734 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.391973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2174 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2245 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStMember.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3455 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStMemberMasterSync.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2151 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStOmp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1971 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStOmp5BuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2124 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStUniformCudaHipBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2591 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.391973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/detail/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5720 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/detail/BlockSharedMemStMemberImpl.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.393973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1061 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierOacc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3422 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierOmp.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2078 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierThread.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2721 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1328 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncNoOp.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4310 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncUniformCudaHipBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3643 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.400973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2514 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Align.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      786 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/AlignedAlloc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14027 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ApiCudaRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14710 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ApiHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3486 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Assert.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5524 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/BarrierThread.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3214 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/BoostPredef.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2352 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/CallbackThread.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1025 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ClipCast.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7308 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Common.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2695 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Concepts.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15371 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ConcurrentExecPool.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2239 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Cuda.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13234 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/CudaHipCommon.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2351 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Debug.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1440 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Decay.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      802 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/DemangleTypeNames.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      648 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Hip.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1665 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Omp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3145 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/OmpSchedule.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1543 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Positioning.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      887 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/RemoveRestrict.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.401973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/STLTuple/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1306 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/STLTuple/LICENSE.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11822 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/STLTuple/STLTuple.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7945 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Sycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1259 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ThreadTraits.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1110 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Tuple.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8484 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/UniformCudaHip.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1134 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Unreachable.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      982 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Unroll.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2098 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Utility.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12035 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Vectorize.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.305971 CLUEstering-2.2.1/extern/alpaka/include/alpaka/ctx/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.402973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/ctx/block/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9069 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/ctx/block/CtxBlockOacc.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.405973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5868 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevCpu.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      634 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevCpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      587 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevCudaRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      638 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevFpgaSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      571 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevFpgaSyclXilinx.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8157 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      600 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevGpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      581 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10945 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevOacc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9181 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevOmp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7985 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevUniformCudaHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3679 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.405973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/common/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3186 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/common/QueueRegistry.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.406973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/cpu/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7999 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/cpu/SysInfo.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1087 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/cpu/Wait.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.406973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dim/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      645 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dim/DimArithmetic.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      532 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dim/DimIntegralConst.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      709 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/dim/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.406973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/elem/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1083 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/elem/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.409973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      471 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventCpu.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      639 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventCpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      594 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventCudaRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      643 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventFpgaSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      610 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventFpgaSyclXilinx.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5567 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17228 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventGenericThreads.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      639 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventGpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      588 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      675 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventOacc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      673 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventOmp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10765 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventUniformCudaHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1412 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.410973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/example/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2863 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/example/ExampleDefaultAcc.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.410973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/extent/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5233 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/extent/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.411973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5073 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/Accessors.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10906 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/MapIdx.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1157 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.413973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2709 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2654 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtLinear.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2885 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtOmp.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2922 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtRefThreadIdMap.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3131 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtUniformCudaHipBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1902 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtZero.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.413973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/gb/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2652 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/gb/IdxGbGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2707 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/gb/IdxGbLinear.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2060 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/gb/IdxGbRef.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3119 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/gb/IdxGbUniformCudaHipBuiltIn.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.414973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2937 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/IntrinsicCpu.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2388 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/IntrinsicFallback.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1902 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/IntrinsicGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2747 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/IntrinsicUniformCudaHipBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3249 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.419973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    41708 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuOmp2Blocks.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8575 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuOmp2Threads.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5505 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuSerial.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      821 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6014 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuTbbBlocks.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11379 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuThreads.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      826 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelFpgaSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      793 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelFpgaSyclXilinx.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10306 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      707 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGpuCudaRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      702 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGpuHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      822 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20385 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGpuUniformCudaHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10008 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelOacc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11715 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelOmp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12386 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.421973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18541 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/Complex.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2439 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/FloatEqualExact.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22690 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/MathGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9713 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/MathStdLib.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    50999 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/MathUniformCudaHipBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    49121 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.308971 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.421973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/alloc/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3113 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/alloc/AllocCpuAligned.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1293 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/alloc/AllocCpuNew.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1643 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/alloc/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.425973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13064 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufCpu.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      679 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufCpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      614 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufCudaRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      684 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufFpgaSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      717 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufFpgaSyclXilinx.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9147 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      680 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufGpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      609 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10521 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufOacc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10478 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufOmp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16723 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufUniformCudaHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2356 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/SetKernel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8698 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.426973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/cpu/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9859 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/cpu/Copy.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7684 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/cpu/Set.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.426973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/oacc/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14135 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/oacc/Copy.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4541 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/oacc/Set.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.427973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/omp5/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14082 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/omp5/Copy.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4558 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/omp5/Set.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.428973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/sycl/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5057 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/sycl/Accessor.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1494 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/sycl/Common.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5643 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/sycl/Copy.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2935 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/sycl/Set.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.428973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29263 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/Copy.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15743 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/Set.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.431973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2562 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceCpu.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1984 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceCpuSerial.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3081 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2530 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceOacc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1670 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp2Blocks.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2371 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp2Threads.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1155 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2179 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceUniformCudaHipBuiltIn.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2529 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.433973 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6888 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/Accessor.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25714 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/Traits.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5769 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewAccessOps.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9709 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewAccessor.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3702 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewConst.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11690 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewPlainPtr.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3094 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewStdArray.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3210 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewStdVector.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12638 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewSubView.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.437974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      885 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Apply.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3262 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/CartesianProduct.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      980 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Concatenate.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9804 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/CudaVectorArrayWrapper.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      656 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/DependentFalseType.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1715 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Filter.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      883 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Fold.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2071 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/ForEachType.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      902 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Functional.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      577 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/InheritFromList.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4468 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/IntegerSequence.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2691 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Integral.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1872 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/IsArrayOrVector.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      679 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/IsStrictBase.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4116 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/NdLoop.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1949 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Set.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      860 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Transform.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1129 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/TypeListOps.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1392 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Unique.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.437974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/offset/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4483 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/offset/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.440974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1963 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfCpu.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1901 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfCpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      586 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfCudaRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1251 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfFpgaSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1835 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfFpgaSyclXilinx.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29875 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1896 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfGpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      580 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1296 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfOacc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2973 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfOmp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15677 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfUniformCudaHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2834 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.444974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      684 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/Properties.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      499 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCpuBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      508 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCpuNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      629 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCpuSyclIntelBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      638 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCpuSyclIntelNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      620 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCudaRtBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      633 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCudaRtNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      634 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueFpgaSyclIntelBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      642 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueFpgaSyclIntelNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      600 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueFpgaSyclXilinxBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      609 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueFpgaSyclXilinxNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      610 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGenericSyclBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      580 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGenericSyclNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6101 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGenericThreadsBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7379 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGenericThreadsNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      629 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGpuSyclIntelBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      638 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGpuSyclIntelNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      614 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueHipRtBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      627 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueHipRtNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      714 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueOaccBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      723 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueOaccNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      712 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueOmp5Blocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      721 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueOmp5NonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      656 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueUniformCudaHipRtBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      664 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueUniformCudaHipRtNonBlocking.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2780 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.444974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/cpu/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      570 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/cpu/ICpuQueue.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1221 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/cpu/IGenericThreadsQueue.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.445974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/cuda_hip/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12770 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/cuda_hip/QueueUniformCudaHipRt.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.445974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/sycl/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9445 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/sycl/QueueGenericSyclBase.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.448974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.451974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1547 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/MultiplyAndSplit64to32.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3468 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseCommon.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2299 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseCudaArray.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1030 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseStdArray.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4198 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseTraits.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2344 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxConstants.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5822 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxSingle.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4604 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxStateless.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1324 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxStatelessKeyedBase.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1103 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxStatelessVector.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3654 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxVector.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7719 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandDefault.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7696 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandPhilox.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1729 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandPhiloxStateless.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8983 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandStdLib.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9900 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandUniformCudaHipRand.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.451974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/TinyMT/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1666 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/TinyMT/Engine.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1884 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/TinyMT/LICENSE.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12410 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/TinyMT/tinymt32.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4156 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.454974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      382 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/AnyOacc.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      383 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/AnyOmp5.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      393 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/CpuOmp2Blocks.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      393 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/CpuOmp2Threads.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      391 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/CpuSerial.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      550 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/CpuSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      391 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/CpuTbbBlocks.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      399 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/CpuThreads.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      554 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/FpgaSyclIntel.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      478 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/FpgaSyclXilinx.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      364 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/GenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      714 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/GpuCudaRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      375 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/GpuHipRt.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      550 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/GpuSyclIntel.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.455974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      845 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/Array.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2488 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/Check.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1471 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/Extent.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2757 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/KernelExecutionFixture.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1863 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/MeasureKernelRunTime.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.456974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/acc/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12217 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/acc/TestAccs.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.456974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/dim/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      911 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/dim/TestDims.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.456974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/event/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29108 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/event/EventHostManualTrigger.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.457974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/idx/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      912 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/idx/TestIdxs.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.309971 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/mem/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.457974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/mem/view/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6100 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/mem/view/Iterator.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9422 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/mem/view/ViewTest.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.458974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/queue/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9066 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/queue/Queue.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11686 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/queue/QueueCpuOmp2Collective.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      761 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/queue/QueueTestFixture.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.458974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/traits/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1273 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/traits/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.458974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/vec/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3862 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/vec/Traits.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    28372 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/vec/Vec.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      604 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/version.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.459974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/wait/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1512 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/wait/Traits.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.459974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/warp/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8440 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/warp/Traits.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4504 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/warp/WarpGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2376 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/warp/WarpSingleThread.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4857 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/warp/WarpUniformCudaHipBuiltIn.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.461974 CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2825 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/Traits.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4424 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/WorkDivGenericSycl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18369 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/WorkDivHelpers.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5835 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/WorkDivMembers.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4977 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/WorkDivUniformCudaHipBuiltIn.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.468974 CLUEstering-2.2.1/extern/alpaka/script/
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      439 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/after_failure.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     3857 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/before_install.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      574 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/ci.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     7813 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/docker_ci.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      922 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/docker_retry.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      668 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/gitlab_ci_run.sh
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.469974 CLUEstering-2.2.1/extern/alpaka/script/gitlabci/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      306 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/gitlabci/fake_sudo.sh
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      312 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/gitlabci/job_analysis.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3830 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/gitlabci/job_base.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1007 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/gitlabci/job_clang.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      922 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/gitlabci/job_cuda11.0.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      769 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/gitlabci/job_cuda11.8.yml
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1806 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/gitlabci/print_env.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     3646 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1239 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_analysis.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     6780 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_boost.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     3890 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_clang.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2485 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_cmake.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     9106 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_cuda.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      429 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_doxygen.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1344 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_gcc.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2583 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_hip.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      415 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_omp.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1440 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_oneapi.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2063 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/install_tbb.sh
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.471974 CLUEstering-2.2.1/extern/alpaka/script/job_generator/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1639 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/alpaka_filter.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      925 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/alpaka_globals.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2619 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/custom_job.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20508 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/generate_job_yaml.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7170 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/job_generator.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6277 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/job_modifier.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      847 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/reorder_jobs.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       78 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/requirements.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1021 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/verify.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3423 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/job_generator/versions.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     5047 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/prepare_sanitizers.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      787 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/print_env.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      637 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/push_doc.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     4266 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/run.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      889 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/run_analysis.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      729 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/run_build.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1131 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/run_doxygen.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     4016 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/run_generate.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      540 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/run_install.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1362 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/run_tests.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      687 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/set.sh
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1685 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/script/travis_retry.sh
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.472974 CLUEstering-2.2.1/extern/alpaka/test/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      618 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.472974 CLUEstering-2.2.1/extern/alpaka/test/analysis/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      776 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/analysis/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.472974 CLUEstering-2.2.1/extern/alpaka/test/analysis/headerCheck/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2181 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/analysis/headerCheck/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.473974 CLUEstering-2.2.1/extern/alpaka/test/analysis/headerCheck/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      416 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/analysis/headerCheck/src/main.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.473974 CLUEstering-2.2.1/extern/alpaka/test/common/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2719 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/common/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10684 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/common/devCompileOptions.cmake
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.473974 CLUEstering-2.2.1/extern/alpaka/test/integ/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      997 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.474974 CLUEstering-2.2.1/extern/alpaka/test/integ/axpy/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      688 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/axpy/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.474974 CLUEstering-2.2.1/extern/alpaka/test/integ/axpy/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7077 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/axpy/src/axpy.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.474974 CLUEstering-2.2.1/extern/alpaka/test/integ/cudaOnly/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      769 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/cudaOnly/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.474974 CLUEstering-2.2.1/extern/alpaka/test/integ/cudaOnly/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1633 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/cudaOnly/src/cudaNativeFunctions.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.475974 CLUEstering-2.2.1/extern/alpaka/test/integ/hostOnlyAPI/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      796 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/hostOnlyAPI/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.475974 CLUEstering-2.2.1/extern/alpaka/test/integ/hostOnlyAPI/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4547 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/hostOnlyAPI/src/hostOnlyAPI.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.475974 CLUEstering-2.2.1/extern/alpaka/test/integ/mandelbrot/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      694 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/mandelbrot/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.475974 CLUEstering-2.2.1/extern/alpaka/test/integ/mandelbrot/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13253 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/mandelbrot/src/mandelbrot.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.475974 CLUEstering-2.2.1/extern/alpaka/test/integ/matMul/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      690 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/matMul/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.476974 CLUEstering-2.2.1/extern/alpaka/test/integ/matMul/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12437 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/matMul/src/matMul.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.476974 CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1171 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.476974 CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/include/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      362 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/include/mysqrt.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.476974 CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5886 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/src/main.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      711 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/src/mysqrt.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.477974 CLUEstering-2.2.1/extern/alpaka/test/integ/sharedMem/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      693 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/sharedMem/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.477974 CLUEstering-2.2.1/extern/alpaka/test/integ/sharedMem/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6902 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/sharedMem/src/sharedMem.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.477974 CLUEstering-2.2.1/extern/alpaka/test/integ/zeroDimBuffer/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      735 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/zeroDimBuffer/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.477974 CLUEstering-2.2.1/extern/alpaka/test/integ/zeroDimBuffer/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4856 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/integ/zeroDimBuffer/src/zeroDimBuffer.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      473 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/sanitizer_lsan_blacklist.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      928 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/sanitizer_ubsan_blacklist.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.478974 CLUEstering-2.2.1/extern/alpaka/test/unit/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1406 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.478974 CLUEstering-2.2.1/extern/alpaka/test/unit/acc/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/acc/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.479974 CLUEstering-2.2.1/extern/alpaka/test/unit/acc/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1212 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/acc/src/AccDevPropsTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      612 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/acc/src/AccNameTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9113 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/acc/src/AccTagTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.479974 CLUEstering-2.2.1/extern/alpaka/test/unit/atomic/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      762 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/atomic/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.479974 CLUEstering-2.2.1/extern/alpaka/test/unit/atomic/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14908 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/atomic/src/AtomicTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.314971 CLUEstering-2.2.1/extern/alpaka/test/unit/block/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.480974 CLUEstering-2.2.1/extern/alpaka/test/unit/block/shared/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      773 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/block/shared/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.480974 CLUEstering-2.2.1/extern/alpaka/test/unit/block/shared/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2512 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/block/shared/src/BlockSharedMemDyn.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6079 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/block/shared/src/BlockSharedMemSt.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.481974 CLUEstering-2.2.1/extern/alpaka/test/unit/block/sharedSharing/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      800 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/block/sharedSharing/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.481974 CLUEstering-2.2.1/extern/alpaka/test/unit/block/sharedSharing/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5202 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/block/sharedSharing/src/BlockSharedMemSharing.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.481974 CLUEstering-2.2.1/extern/alpaka/test/unit/block/sync/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      769 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/block/sync/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.482974 CLUEstering-2.2.1/extern/alpaka/test/unit/block/sync/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3117 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/block/sync/src/BlockSync.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4115 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/block/sync/src/BlockSyncPredicate.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.482974 CLUEstering-2.2.1/extern/alpaka/test/unit/core/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      687 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/core/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.483974 CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1991 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/BoostPredefTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4292 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/ClipCastTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4905 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/ConceptsTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2103 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/OmpScheduleTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1170 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/Utility.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.483974 CLUEstering-2.2.1/extern/alpaka/test/unit/dev/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/dev/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.483974 CLUEstering-2.2.1/extern/alpaka/test/unit/dev/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      937 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/dev/src/DevWarpSizeTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.483974 CLUEstering-2.2.1/extern/alpaka/test/unit/event/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      688 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/event/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.484974 CLUEstering-2.2.1/extern/alpaka/test/unit/event/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8973 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/event/src/EventTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.484974 CLUEstering-2.2.1/extern/alpaka/test/unit/idx/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/idx/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.484974 CLUEstering-2.2.1/extern/alpaka/test/unit/idx/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1153 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/idx/src/MapIdx.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1972 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/idx/src/MapIdxPitchBytes.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.485974 CLUEstering-2.2.1/extern/alpaka/test/unit/intrinsic/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      768 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/intrinsic/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.485974 CLUEstering-2.2.1/extern/alpaka/test/unit/intrinsic/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2104 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/intrinsic/src/Ffs.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2111 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/intrinsic/src/Popcount.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.485974 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      762 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.487975 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1878 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelGenericLambda.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2922 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelLambda.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1883 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithAdditionalParam.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1717 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithConstructorAndMember.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1561 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithHostConstexpr.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5968 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithOmpSchedule.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2363 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithTemplate.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6113 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithTemplateArgumentDeduction.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4530 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithoutTemplatedAccParam.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.487975 CLUEstering-2.2.1/extern/alpaka/test/unit/math/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1317 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.491974 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4599 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/Buffer.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9707 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/DataGen.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4849 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/Defines.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2136 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/FloatEqualExactTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18799 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/Functor.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7264 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/TestTemplate.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9271 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathADL.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2783 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathComplexDouble.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2774 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathComplexFloat.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1379 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathDouble.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3865 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathFloat.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4063 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathLambda.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4616 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/powMixedTypes.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2078 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/sincos.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.316971 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.491974 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/buf/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      763 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/buf/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.492975 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/buf/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10888 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/buf/src/BufTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.492975 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/copy/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1074 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/copy/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.492975 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/copy/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6119 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/copy/src/BufSlicing.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.492975 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/fence/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      742 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/fence/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.492975 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/fence/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7404 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/fence/src/FenceTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.493975 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/p2p/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      689 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/p2p/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.493975 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/p2p/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2504 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/p2p/src/P2P.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.493975 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      765 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.494974 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13635 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/Accessor.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5911 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/MdSpan.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4574 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/ViewConst.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7008 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/ViewPlainPtrTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4779 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/ViewStaticAccMem.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6799 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/ViewSubViewTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.495975 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      687 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.499975 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      773 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/ApplyTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1317 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/CartesianProductTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      929 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/ConcatenateTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7174 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/CudaVectorArrayWrapperTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      740 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/FilterTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    50223 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/IntegralTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1967 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/IsArrayOrVectorTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1609 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/IsStrictBaseTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      999 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/SetTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1226 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/TransformTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1386 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/TypeListOpsTest.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1063 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/UniqueTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.499975 CLUEstering-2.2.1/extern/alpaka/test/unit/queue/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      688 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/queue/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.499975 CLUEstering-2.2.1/extern/alpaka/test/unit/queue/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4512 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/queue/src/CollectiveQueue.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8039 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/queue/src/QueueTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.500975 CLUEstering-2.2.1/extern/alpaka/test/unit/rand/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      758 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/rand/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.500975 CLUEstering-2.2.1/extern/alpaka/test/unit/rand/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4873 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/rand/src/RandTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.500975 CLUEstering-2.2.1/extern/alpaka/test/unit/traits/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      708 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/traits/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.500975 CLUEstering-2.2.1/extern/alpaka/test/unit/traits/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      931 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/traits/src/NativeHandleTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.501975 CLUEstering-2.2.1/extern/alpaka/test/unit/vec/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/vec/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.501975 CLUEstering-2.2.1/extern/alpaka/test/unit/vec/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12541 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/vec/src/VecTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.501975 CLUEstering-2.2.1/extern/alpaka/test/unit/warp/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      758 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/warp/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.502975 CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4060 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/Activemask.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4036 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/All.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4036 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/Any.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4641 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/Ballot.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1526 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/GetSize.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5448 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/Shfl.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.502975 CLUEstering-2.2.1/extern/alpaka/test/unit/workDiv/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      690 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/workDiv/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.503975 CLUEstering-2.2.1/extern/alpaka/test/unit/workDiv/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4941 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/test/unit/workDiv/src/WorkDivHelpersTest.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.503975 CLUEstering-2.2.1/extern/alpaka/thirdParty/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       48 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/.clang-format
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1536 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.508975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      262 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.bazelrc
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1114 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.clang-format
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.318971 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.conan/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.508975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.conan/test_package/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      354 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.conan/test_package/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      592 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.conan/test_package/conanfile.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      365 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.conan/test_package/test_package.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      613 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.gitattributes
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.508975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       60 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/FUNDING.yml
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.509975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      711 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      308 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1066 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/pull_request_template.md
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.510975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      540 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/linux-bazel-builds.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1150 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/linux-meson-builds.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3756 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/linux-other-builds.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3562 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/linux-simple-builds.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1565 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/mac-builds.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      976 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/validate-header-guards.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      560 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.gitignore
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4063 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/BUILD.bazel
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.512975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      250 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/Catch2Config.cmake.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2432 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/CatchConfigOptions.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4238 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/CatchMiscFunctions.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5086 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/FindGcov.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12328 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/FindLcov.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8419 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/Findcodecov.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      337 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/catch2-with-main.pc.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      331 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/catch2.pc.in
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1071 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/llvm-cov-wrapper
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6750 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      837 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMakePresets.json
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3215 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   108911 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/Doxyfile
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1338 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/LICENSE.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4045 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/README.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      686 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/SECURITY.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      559 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/WORKSPACE.bazel
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4361 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/appveyor.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      297 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/codecov.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2592 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/conanfile.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.318971 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.514975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/artwork/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10636 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/artwork/catch2-c-logo.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    33761 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/artwork/catch2-hand-logo.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25330 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/artwork/catch2-logo-small-with-background.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20939 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/artwork/catch2-logo-small.png
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.524975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1608 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/Readme.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6834 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/assertions.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11326 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/benchmarks.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5257 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/ci-and-misc.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13910 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/cmake-integration.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    27308 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/command-line.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      570 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/commercial-users.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6588 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/comparing-floating-point-numbers.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12560 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/configuration.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13234 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/contributing.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1292 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/deprecations.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1494 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/event-listeners.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3983 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/faq.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8484 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/generators.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6340 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/limitations.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2733 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/list-of-examples.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4954 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/logging.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13819 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/matchers.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4270 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/migrate-v2-to-v3.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6696 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/opensource-users.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4192 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/other-macros.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4137 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/own-main.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    75415 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/release-notes.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2822 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/release-process.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5861 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/reporter-events.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8414 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/reporters.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15309 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/test-cases-and-sections.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5668 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/test-fixtures.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4783 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/tostring.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8230 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/tutorial.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4163 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/usage-tips.md
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2992 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/why-catch.md
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.527975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1322 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/010-TestCase.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1031 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/020-TestCase-1.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1187 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/020-TestCase-2.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2784 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/030-Asn-Require-Check.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2517 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/100-Fix-Section.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2134 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/110-Fix-ClassFixture.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3028 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/120-Bdd-ScenarioGivenWhenThen.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14840 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/210-Evt-EventListeners.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1435 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/231-Cfg-OutputStreams.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2182 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/300-Gen-OwnGenerator.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1901 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/301-Gen-MapTypeConversion.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2183 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/302-Gen-Table.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1358 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/310-Gen-VariablesInGenerators.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1622 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/311-Gen-CustomCapture.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1561 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.532975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9169 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/Catch.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4389 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/CatchAddTests.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2136 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/CatchShardTests.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1642 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/CatchShardTestsImpl.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15008 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/ParseAndAddCatchTests.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   368375 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/catch_amalgamated.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   464259 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/catch_amalgamated.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      645 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/gdbinit
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      624 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/lldbinit
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.534975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/fuzzing/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      753 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/fuzzing/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      233 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/fuzzing/NullOStream.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      451 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/fuzzing/NullOStream.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      373 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/fuzzing/fuzz_TestSpecParser.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      327 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/fuzzing/fuzz_XmlWriter.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1127 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/fuzzing/fuzz_textflow.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      139 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/mdsnippets.json
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      417 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/meson.build
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.534975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20289 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.542976 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.545976 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6268 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_benchmark.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1903 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_benchmark_all.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      509 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_chronometer.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2624 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_chronometer.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1110 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_clock.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2642 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_constructor.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1168 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_environment.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      884 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_estimate.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2394 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_execution_plan.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2191 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_optimizer.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1005 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_outlier_classification.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1633 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_sample_analysis.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.549975 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3411 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_analyse.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      522 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_benchmark_function.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4259 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_benchmark_function.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2308 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_complete_invoke.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5421 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_estimate_clock.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1176 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_measure.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1045 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_repeat.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      952 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_run_for_at_least.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2560 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_run_for_at_least.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10472 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_stats.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5905 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_stats.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      964 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_timing.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5882 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_all.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2565 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_approx.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4647 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_approx.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      791 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_info.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3367 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_result.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1835 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_result.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10544 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_config.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5314 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_config.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      483 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_get_random_seed.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      486 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_get_random_seed.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3930 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_message.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5609 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_message.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4462 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_registry_hub.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1239 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_section_info.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13135 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_session.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1764 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_session.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      698 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      879 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias_autoregistrar.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1083 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias_autoregistrar.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10642 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_template_test_macros.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9705 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_case_info.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3721 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_case_info.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14216 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_macros.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4187 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_spec.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3824 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_spec.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1195 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_timer.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      724 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_timer.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7497 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tostring.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20853 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tostring.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1744 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_totals.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      981 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_totals.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3168 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_translate_exception.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5805 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_user_config.hpp.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1286 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_version.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1182 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_version.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      461 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_version_macros.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.551976 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      435 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generator_exception.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      868 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generator_exception.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1054 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8929 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8630 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_adapters.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1169 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_all.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      423 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_random.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2841 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_random.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3479 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_range.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.555976 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1573 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_all.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      370 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_capture.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3445 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_capture.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      355 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_config.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3235 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_config.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1540 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_enum_values_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      461 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_exception.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1194 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_exception.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      901 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_generatortracker.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3360 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_generatortracker.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      430 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_registry_hub.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2411 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_registry_hub.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3873 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10200 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      444 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_factory.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1433 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_factory.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      386 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_registry.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1400 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      854 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_tag_alias_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      422 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_testcase.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1532 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_testcase.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.585976 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3347 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_assertion_handler.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2079 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_assertion_handler.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1164 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_insensitive_comparisons.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      975 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_insensitive_comparisons.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      454 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_sensitive.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17469 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_clara.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24910 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_clara.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14840 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_commandline.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      538 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_commandline.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3087 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_compare_traits.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16928 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_compiler_capabilities.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      955 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_android_logwrite.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      963 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_counter.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1315 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_uncaught_exceptions.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1010 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_wchar.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10897 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_colour.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4286 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_colour.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      624 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_width.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2160 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_container_nonmembers.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1689 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_context.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1595 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_context.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1228 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debug_console.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      464 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debug_console.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4416 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debugger.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2123 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debugger.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      771 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_decomposer.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16801 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_decomposer.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1152 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enforce.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1635 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enforce.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2716 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enum_values_registry.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1130 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enum_values_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      442 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_errno_guard.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      697 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_errno_guard.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3062 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_exception_translator_registry.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      984 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_exception_translator_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9067 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_fatal_condition_handler.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2271 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_fatal_condition_handler.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      923 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_floating_point_helpers.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3652 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_floating_point_helpers.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      933 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_getenv.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      526 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_getenv.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5195 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_istream.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1651 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_istream.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      913 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_lazy_expr.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1132 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_lazy_expr.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1144 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_leak_detector.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      471 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_leak_detector.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4364 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_list.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      928 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_list.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1285 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_logical_traits.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1407 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_main.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      753 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_message_info.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1219 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_message_info.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1468 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_meta.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      715 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_move_and_forward.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      856 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_noncopyable.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2756 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_optional.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4198 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_output_redirect.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3479 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_output_redirect.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1694 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_parse_numbers.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      765 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_parse_numbers.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1222 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_platform.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      807 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_polyfills.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      427 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_polyfills.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22187 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_preprocessor.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      765 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_preprocessor_remove_parens.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1869 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_number_generator.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2055 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_number_generator.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1020 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_seed_generation.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      685 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_seed_generation.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2934 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_registry.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1195 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6248 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_spec_parser.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2702 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_spec_parser.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      977 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_result_type.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1582 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_result_type.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2028 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reusable_string_stream.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1700 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reusable_string_stream.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25737 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_run_context.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5379 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_run_context.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1382 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_section.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1746 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_section.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1387 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_sharding.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1005 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_singletons.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1226 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_singletons.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1181 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_source_line_info.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1056 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_source_line_info.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      975 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_startup_exception_registry.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      812 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_startup_exception_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      638 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stdstreams.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      465 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stdstreams.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      827 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stream_end_stop.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3746 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_string_manip.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2062 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_string_manip.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2088 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stringref.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3779 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stringref.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2259 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_tag_alias_registry.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1042 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_tag_alias_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24029 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_template_test_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1283 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_info_hasher.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      710 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_info_hasher.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6100 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_registry_impl.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2733 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_registry_impl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7859 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_tracker.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5528 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_tracker.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      639 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_failure_exception.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      738 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_failure_exception.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7686 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_macro_impl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2916 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_registry.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5530 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_registry.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7560 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_spec_parser.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2219 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_spec_parser.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8596 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_textflow.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6125 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_textflow.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      777 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_to_string.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      788 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_uncaught_exceptions.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      461 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_uncaught_exceptions.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      815 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_unique_name.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3002 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_unique_ptr.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      619 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_void_type.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1777 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_wildcard_pattern.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1063 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_wildcard_pattern.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      764 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_windows_h_proxy.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11198 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_xmlwriter.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5373 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_xmlwriter.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.590976 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      621 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10210 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1478 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_all.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      862 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_container_properties.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2905 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_container_properties.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3779 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_contains.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      721 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_exception.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      976 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_exception.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7531 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_floating_point.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3068 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_floating_point.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      529 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_predicate.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1857 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_predicate.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      851 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_quantifiers.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5494 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_quantifiers.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4488 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_string.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3313 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_string.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1424 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_templated.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13392 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_templated.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7649 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_vector.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.590976 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1058 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/catch_matchers_impl.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3327 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/catch_matchers_impl.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12847 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/meson.build
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.598976 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1175 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_automake.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1318 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_automake.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1690 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_common_base.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2950 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_common_base.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8792 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_compact.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1081 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_compact.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22030 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_console.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2356 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_console.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5917 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_cumulative_base.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6492 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_cumulative_base.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1944 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_event_listener.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2671 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_event_listener.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12937 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_helpers.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3289 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_helpers.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11976 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_junit.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1822 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_junit.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7106 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_multi.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2989 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_multi.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      993 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_registrars.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4763 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_registrars.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6175 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_sonarqube.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1963 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_sonarqube.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      667 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_streaming_base.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2909 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_streaming_base.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8662 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_tap.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1359 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_tap.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6635 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_teamcity.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1908 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_teamcity.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14298 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_xml.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2154 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_xml.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1763 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporters_all.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.599976 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25205 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.605977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    19401 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      624 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/ToDo.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3612 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X01-PrefixedMacros.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1669 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X02-DisabledMacros.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1191 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X03-DisabledExceptions-DefaultHandler.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1061 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X04-DisabledExceptions-CustomHandler.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      567 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X05-DeferredStaticChecks.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      809 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X10-FallbackStringifier.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      646 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X11-DisableStringification.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      644 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X12-CustomDebugBreakMacro.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2474 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X21-PartialTestCaseEvents.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2362 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X22-BenchmarksInCumulativeReporter.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1182 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X23-CasingInReporterNames.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1330 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X24-ListenerStdoutCaptureInMultireporter.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1479 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X25-ListenerCanAskForCapturedStdout.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1363 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X26-ReporterPreferencesForPassingAssertionsIsRespected.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2837 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X27-CapturedStdoutInTestCaseEvents.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3235 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X28-ListenersGetEventsBeforeReporters.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1702 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X29-CustomArgumentsForReporters.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      490 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X30-BazelReporter.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      522 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X31-DuplicatedTestCases.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      551 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X32-DuplicatedTestCasesDifferentTags.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      625 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X33-DuplicatedTestCaseMethods.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      705 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X34-DuplicatedTestCaseMethodsDifferentFixtures.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      993 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X35-DuplicatedReporterNames.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      569 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X90-WindowsHeaderInclusion.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      950 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X91-AmalgamatedCatch.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      321 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X92-NoTests.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.605977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.621977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9171 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.std.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24238 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.sw.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24018 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.sw.multi.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   214711 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/compact.sw.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   214491 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/compact.sw.multi.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    50055 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.std.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   578273 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.sw.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   578053 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.sw.multi.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    32602 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.swa4.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      220 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/default.sw.multi.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   138530 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/junit.sw.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   138510 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/junit.sw.multi.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   110409 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/sonarqube.sw.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   110389 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/sonarqube.sw.multi.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   239558 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/tap.sw.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   239338 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/tap.sw.multi.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    91238 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/teamcity.sw.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    91218 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/teamcity.sw.multi.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   794014 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/xml.sw.approved.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   793994 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/xml.sw.multi.approved.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.630977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2993 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Clara.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15944 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/CmdLine.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4878 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/CmdLineHelpers.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1944 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/ColourImpl.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4418 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Details.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3092 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/FloatingPoint.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18674 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/GeneratorsImpl.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14665 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/InternalBenchmark.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1308 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Parse.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7792 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/PartTracker.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2078 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/RandomNumberGeneration.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13409 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Reporters.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1382 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Sharding.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1049 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Stream.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6719 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/String.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3386 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/StringManip.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3872 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Tag.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2368 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestCaseInfoHasher.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15392 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestSpec.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1770 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestSpecParser.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6606 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TextFlow.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4016 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/ToString.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2234 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Traits.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4500 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/UniquePtr.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7360 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Xml.tests.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.631977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Misc/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       41 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Misc/invalid-test-names.input
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       42 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Misc/plain-old-tests.input
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       41 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Misc/special-characters-in-file.input
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6734 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/TestRegistrations.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.631977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/TimingTests/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      632 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/TimingTests/Sleep.tests.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.638977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6686 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Approx.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3383 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/BDD.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5144 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Benchmark.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4575 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Class.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10150 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Compilation.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9154 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Condition.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      994 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Decomposition.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3758 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/EnumToString.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6414 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Exception.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9966 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Generators.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    38790 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Matchers.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29106 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/MatchersRanges.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8683 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Message.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16017 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Misc.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      767 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringByte.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1910 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringChrono.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5986 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringGeneral.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1176 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringOptional.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1506 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringPair.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1688 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringTuple.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3447 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringVariant.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3433 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringVector.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5234 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringWhich.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8730 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Tricky.tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      570 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/VariadicMacros.tests.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.639977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      617 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/parse_test_spec.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      546 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/parse_test_spec.hpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1596 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/type_with_lit_0_comparisons.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.641977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3039 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/ConfigureTestsCommon.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3048 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testBazelReporter.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2238 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testBazelSharding.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1337 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDefaultReporter.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1643 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDisable.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1488 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDisableStringification.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1564 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureExperimentalRedirect.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2368 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testPartialTestCaseEvent.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     2689 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testRandomOrder.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     5608 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testSharding.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3266 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/meson.build
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.641977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/third_party/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    43554 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/third_party/clara.hpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.320971 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.642977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      416 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1273 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/appveyorBuildConfigurationScript.bat
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      317 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/appveyorMergeCoverageScript.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      708 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/appveyorTestRunScript.bat
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3997 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/coverage-helper.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1020 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/installOpenCppCoverage.ps1
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.645977 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     8687 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/approvalTests.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      916 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/approve.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     5030 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/checkConvenienceHeaders.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      288 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/checkDuplicateFilenames.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1213 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/checkLicense.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      196 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/developBuild.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3542 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/extractFeaturesFromReleaseNotes.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1401 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/fixWhitespace.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     5239 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/generateAmalgamatedFiles.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      197 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/majorRelease.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      197 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/minorRelease.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      196 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/patchRelease.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5725 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/releaseCommon.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      116 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/scriptCommon.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)      816 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/updateDocumentSnippets.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)    13736 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/updateDocumentToC.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.650977 CLUEstering-2.2.1/extern/pybind11/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1271 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.appveyor.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      996 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.clang-format
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2605 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.clang-tidy
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2196 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.cmake-format.yaml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1308 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       43 2024-03-11 23:17:33.000000 CLUEstering-2.2.1/extern/pybind11/.git
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       18 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.gitattributes
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.651977 CLUEstering-2.2.1/extern/pybind11/.github/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      182 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15285 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.651977 CLUEstering-2.2.1/extern/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2561 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      328 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      162 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/dependabot.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      116 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/labeler.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       50 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.652978 CLUEstering-2.2.1/extern/pybind11/.github/matchers/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      668 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      645 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.653977 CLUEstering-2.2.1/extern/pybind11/.github/workflows/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    34361 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2272 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1491 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      641 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2628 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2876 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      502 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.gitignore
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3726 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      276 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/.readthedocs.yml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12422 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1684 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/LICENSE
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      247 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/MANIFEST.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7687 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/README.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      688 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/SECURITY.md
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.659978 CLUEstering-2.2.1/extern/pybind11/docs/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      607 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/Doxyfile
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7417 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/Makefile
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.321972 CLUEstering-2.2.1/extern/pybind11/docs/_static/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.660978 CLUEstering-2.2.1/extern/pybind11/docs/_static/css/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       37 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.663978 CLUEstering-2.2.1/extern/pybind11/docs/advanced/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.666978 CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3937 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3429 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14283 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3889 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1556 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12371 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9586 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9119 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    47796 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8460 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17846 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    26727 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16583 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.667978 CLUEstering-2.2.1/extern/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      278 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17161 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9030 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5710 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6377 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9240 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/basics.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2853 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/benchmark.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3168 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/benchmark.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   119653 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/changelog.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17090 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/classes.rst
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.667978 CLUEstering-2.2.1/extern/pybind11/docs/cmake/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      273 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25828 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/compiling.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11574 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/conf.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13293 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/faq.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      613 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/index.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3277 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/installing.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3079 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/limitations.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    61034 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    44653 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    87708 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    41121 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    85853 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2647 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/reference.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4957 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/release.rst
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      149 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/requirements.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24035 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.321972 CLUEstering-2.2.1/extern/pybind11/include/
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.675978 CLUEstering-2.2.1/extern/pybind11/include/pybind11/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24334 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7750 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    67899 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8458 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      120 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/common.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2096 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.677978 CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    28500 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    53681 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5962 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17858 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    28553 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    48358 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1625 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.678978 CLUEstering-2.2.1/extern/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      378 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    32135 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18442 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      316 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13459 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4731 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5002 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8517 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3876 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/gil_safe_call_once.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8862 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    80720 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9103 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2734 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/options.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)   128750 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    98893 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.678978 CLUEstering-2.2.1/extern/pybind11/include/pybind11/stl/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4185 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    15477 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29897 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1929 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3296 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/include/pybind11/typing.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2765 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/noxfile.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.679978 CLUEstering-2.2.1/extern/pybind11/pybind11/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      429 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/pybind11/__init__.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1544 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/pybind11/__main__.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      233 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/pybind11/_version.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1207 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/pybind11/commands.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/pybind11/py.typed
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17475 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2306 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/pyproject.toml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1495 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/setup.cfg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4855 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/setup.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.707978 CLUEstering-2.2.1/extern/pybind11/tests/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21733 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.707978 CLUEstering-2.2.1/extern/pybind11/tests/__pycache__/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10601 2024-04-04 14:47:28.000000 CLUEstering-2.2.1/extern/pybind11/tests/__pycache__/conftest.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5619 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/conftest.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11736 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3578 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1772 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      396 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      926 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/env.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.708979 CLUEstering-2.2.1/extern/pybind11/tests/extra_python_package/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8481 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.708979 CLUEstering-2.2.1/extern/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)        0 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4153 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2847 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/local_bindings.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5743 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/object.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6256 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4517 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2685 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      768 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/pytest.ini
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      601 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/requirements.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      855 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_async.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      536 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_async.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10548 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7124 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_buffers.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16025 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17243 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4118 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6549 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10858 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6955 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3370 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5691 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_chrono.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    24849 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_class.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14757 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_class.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.709978 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2584 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      673 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.709978 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1171 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.709978 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1293 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.709978 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1685 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      152 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.709978 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1353 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.709978 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1163 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.710979 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1368 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      198 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3831 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      593 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_const_name.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5710 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1551 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    26064 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4796 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7280 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3992 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1259 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1091 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4557 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2423 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    19958 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    29150 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      473 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    10590 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9414 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_eigen_tensor.py
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.711979 CLUEstering-2.2.1/extern/pybind11/tests/test_embed/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1798 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1315 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      543 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    17396 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      237 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      275 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5722 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9083 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_enum.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3168 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1143 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_eval.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      119 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    13681 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      397 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14165 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18155 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    16491 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     5311 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8507 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3960 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7144 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_iostream.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11034 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14856 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4401 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8054 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22211 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18346 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4121 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3963 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_modules.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12305 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    11874 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    20936 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22892 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21114 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14272 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4487 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9658 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2777 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1847 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9132 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4332 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6719 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2720 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_pickling.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    31789 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    25066 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21920 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8155 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    18898 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9530 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    21587 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12307 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_stl.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     6205 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9795 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4617 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      741 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1855 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      826 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_thread.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     4497 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_type_caster_pyobject_ptr.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3260 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_type_caster_pyobject_ptr.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      603 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_union.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      148 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_union.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      845 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_unnamed_namespace_a.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1141 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_unnamed_namespace_a.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      341 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_unnamed_namespace_b.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      143 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_unnamed_namespace_b.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1471 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_vector_unique_ptr_member.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      329 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_vector_unique_ptr_member.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    22991 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12913 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3226 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2657 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)        0 2024-05-09 15:35:16.716979 CLUEstering-2.2.1/extern/pybind11/tools/
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2449 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     3105 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    12183 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      817 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1423 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/check-style.sh
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      952 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1117 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1031 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/libsize.py
+-rwxr-xr-x   0 sbaldu    (1000) sbaldu    (1000)     1311 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/make_changelog.py
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      196 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)    14449 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     7101 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     9607 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     8564 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       94 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/pyproject.toml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     2104 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1234 2024-03-11 23:17:34.000000 CLUEstering-2.2.1/extern/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)      173 2024-03-11 17:25:53.000000 CLUEstering-2.2.1/pyproject.toml
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)       38 2024-05-09 15:35:16.716979 CLUEstering-2.2.1/setup.cfg
+-rw-r--r--   0 sbaldu    (1000) sbaldu    (1000)     1035 2024-05-09 15:34:55.000000 CLUEstering-2.2.1/setup.py
```

### Comparing `CLUEstering-2.2.0/CLUEstering/CLUEstering.py` & `CLUEstering-2.2.1/CLUEstering/CLUEstering.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,55 @@
 from sklearn.datasets import make_blobs
 from sklearn.preprocessing import StandardScaler
 from os.path import dirname, exists, join
 path = dirname(__file__)
 sys.path.insert(1, join(path, 'lib'))
 import CLUE_Convolutional_Kernels as clue_kernels
 import CLUE_CPU_Serial as cpu_serial
+
+backends = ["cpu serial"]
 tbb_found = exists(str(*glob(join(path, 'lib/CLUE_CPU_TBB*.so'))))
 if tbb_found:
     import CLUE_CPU_TBB as cpu_tbb
+    backends.append("cpu tbb")
 cuda_found = exists(str(*glob(join(path, 'lib/CLUE_GPU_CUDA*.so'))))
 if cuda_found:
     import CLUE_GPU_CUDA as gpu_cuda
+    backends.append("gpu cuda")
 hip_found = exists(str(*glob(join(path, 'lib/CLUE_GPU_HIP*.so'))))
 if hip_found:
     import CLUE_GPU_HIP as gpu_hip
+    backends.append("gpu hip")
+
+
+def is_tbb_available():
+    """
+    Returns True if the library is compiled with TBB support, False otherwise.
+    """
+
+    return tbb_found
+
+
+def is_cuda_available():
+    """
+    Returns True if the library is compiled with CUDA support, False otherwise.
+    """
+
+    return cuda_found
+
+
+def is_hip_available():
+    """
+    Returns True if the library is compiled with HIP support, False otherwise.
+    """
+
+    return hip_found
+
 
-def test_blobs(n_samples: int, n_dim: int , n_blobs: int = 4, mean: float = 0,
+def test_blobs(n_samples: int, n_dim: int, n_blobs: int = 4, mean: float = 0,
                sigma: float = 0.5, x_max: float = 30, y_max: float = 30) -> pd.DataFrame:
     """
     Returns a dataframe containing randomly generated 2-dimensional or 3-dimensional blobs.
 
     This functions serves as a tool for generating a random dataset to test the library.
 
     Parameters
```

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/AllocatorConfig.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/AllocatorConfig.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/AllocatorPolicy.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/AllocatorPolicy.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/CachedBufAlloc.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/CachedBufAlloc.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/CachingAllocator.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/CachingAllocator.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/HostOnlyTask.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/HostOnlyTask.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/StreamCache.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/StreamCache.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpaka/initialise.cc` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpaka/initialise.cc`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaConfig.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaConfig.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaDevices.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaDevices.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaFwd.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaFwd.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaMemory.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaMemory.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/alpakaWorkDiv.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/alpakaWorkDiv.h`

 * *Files 2% similar despite different names*

```diff
@@ -357,14 +357,26 @@
       }
       for (Idx i = threadIdx; i < endElementIdx; ++i) {
         func(i);
       }
     }
   }
 
+  /* once_per_grid
+   *
+   * `once_per_grid(acc)` returns true for a single thread within the kernel execution grid.
+   *
+   * Usually the condition is true for block 0 and thread 0, but these indices should not be relied upon.
+   */
+  template <typename TAcc, typename = std::enable_if_t<alpaka::isAccelerator<TAcc>>>
+  ALPAKA_FN_ACC inline constexpr bool once_per_grid(TAcc const& acc) {
+    return alpaka::getIdx<alpaka::Grid, alpaka::Threads>(acc) ==
+           Vec<alpaka::Dim<TAcc>>::zeros();
+  }
+
   /*
    * Overload for elementIdxShift = 0
    */
   template <typename TAcc, typename Func>
   ALPAKA_FN_ACC void for_each_element_in_grid_strided(const TAcc& acc,
                                                       const Idx maxNumberOfElements,
                                                       const Func func,
```

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/chooseDevice.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/chooseDevice.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/getDeviceCachingAllocator.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/getDeviceCachingAllocator.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/getDeviceIndex.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/getDeviceIndex.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/getHostCachingAllocator.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/getHostCachingAllocator.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/AlpakaCore/initialise.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/AlpakaCore/initialise.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/Makefile` & `CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/Makefile`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_cpu.cc` & `CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_cpu.cc`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_cpu_tbb.cc` & `CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_cpu_tbb.cc`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_gpu_cuda.cc` & `CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_gpu_cuda.cc`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_gpu_hip.cc` & `CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_gpu_hip.cc`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/BindingModules/binding_kernels.cc` & `CLUEstering-2.2.1/CLUEstering/alpaka/BindingModules/binding_kernels.cc`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/CLUE/CLUEAlgoAlpaka.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/CLUEAlgoAlpaka.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/CLUE/CLUEAlpakaKernels.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/CLUEAlpakaKernels.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/CLUE/ConvolutionalKernel.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/ConvolutionalKernel.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/CLUE/Run.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/CLUE/Run.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/Points.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/Points.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/alpaka/AlpakaVecArray.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/alpaka/AlpakaVecArray.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/alpaka/PointsAlpaka.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/alpaka/PointsAlpaka.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering/alpaka/DataFormats/alpaka/TilesAlpaka.h` & `CLUEstering-2.2.1/CLUEstering/alpaka/DataFormats/alpaka/TilesAlpaka.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/CLUEstering.egg-info/PKG-INFO` & `CLUEstering-2.2.1/CLUEstering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLUEstering
-Version: 2.2.0
+Version: 2.2.1
 Summary: A library that generalizes the original 2-dimensional CLUE
 Author: Simone Balducci
 Author-email: simone.balducci00@gmail.com
 Keywords: Python,Clustering,Binding
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `CLUEstering-2.2.0/CLUEstering.egg-info/SOURCES.txt` & `CLUEstering-2.2.1/CLUEstering.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 CLUEstering/alpaka/BindingModules/binding_gpu_cuda.cc
 CLUEstering/alpaka/BindingModules/binding_gpu_hip.cc
 CLUEstering/alpaka/BindingModules/binding_kernels.cc
 CLUEstering/alpaka/CLUE/CLUEAlgoAlpaka.h
 CLUEstering/alpaka/CLUE/CLUEAlpakaKernels.h
 CLUEstering/alpaka/CLUE/ConvolutionalKernel.h
 CLUEstering/alpaka/CLUE/Run.h
+CLUEstering/alpaka/CLUE/binding.cc
 CLUEstering/alpaka/DataFormats/Points.h
 CLUEstering/alpaka/DataFormats/alpaka/AlpakaVecArray.h
 CLUEstering/alpaka/DataFormats/alpaka/PointsAlpaka.h
 CLUEstering/alpaka/DataFormats/alpaka/TilesAlpaka.h
 extern/alpaka/.clang-format
 extern/alpaka/.dockerignore
 extern/alpaka/.git
@@ -1400,14 +1401,15 @@
 extern/pybind11/tests/test_unnamed_namespace_b.py
 extern/pybind11/tests/test_vector_unique_ptr_member.cpp
 extern/pybind11/tests/test_vector_unique_ptr_member.py
 extern/pybind11/tests/test_virtual_functions.cpp
 extern/pybind11/tests/test_virtual_functions.py
 extern/pybind11/tests/valgrind-numpy-scipy.supp
 extern/pybind11/tests/valgrind-python.supp
+extern/pybind11/tests/__pycache__/conftest.cpython-312-pytest-8.1.1.pyc
 extern/pybind11/tests/extra_python_package/pytest.ini
 extern/pybind11/tests/extra_python_package/test_files.py
 extern/pybind11/tests/extra_setuptools/pytest.ini
 extern/pybind11/tests/extra_setuptools/test_setuphelper.py
 extern/pybind11/tests/test_cmake_build/CMakeLists.txt
 extern/pybind11/tests/test_cmake_build/embed.cpp
 extern/pybind11/tests/test_cmake_build/main.cpp
```

### Comparing `CLUEstering-2.2.0/CMakeLists.txt` & `CLUEstering-2.2.1/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 cmake_minimum_required(VERSION 3.16.0)
 project(CLUEstering LANGUAGES CXX)
 
 set(CMAKE_CXX_STANDARD 17)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
-set(CMAKE_CXX_FLAGS "-Wall -Wextra -g -O2")
+if(NOT CMAKE_BUILD_TYPE)
+  set(CMAKE_BUILD_TYPE Release)
+endif()
+
+if(${CMAKE_BUILD_TYPE} STREQUAL "Debug")
+  set(CMAKE_CXX_FLAGS "-Wall -Wextra -g -O0")
+elseif(${CMAKE_BUILD_TYPE} STREQUAL "Release")
+  set(CMAKE_CXX_FLAGS "-O2")
+endif()
 
 # include alpaka extern subfolder
 include_directories(extern/alpaka/include)
 # include pybind11 extern subfolder
 set(PYBIND11_FINDPYTHON ON)
 set(PYBIND11_PYTHON_VERSION ">=3.8")
 add_subdirectory(extern/pybind11)
@@ -29,14 +37,21 @@
     FetchContent_Populate(boost)
   endif()
   set(Boost_PATH ./build/_deps/boost-src)
 else()
   set(Boost_PATH ${Boost_INCLUDE_DIRS})
 endif()
 
+if(NOT DEFINED CPU_ONLY)
+  set(CPU_ONLY OFF)
+endif()
+if(NOT DEFINED SERIAL_ONLY)
+  set(SERIAL_ONLY OFF)
+endif()
+
 # create lib directory in CLUEstering folder
 execute_process(COMMAND mkdir -p ./CLUEstering/lib)
 
 # Convolutional Kernels compile convolutional kernel module
 pybind11_add_module(CLUE_Convolutional_Kernels SHARED
                     ./CLUEstering/alpaka/BindingModules/binding_kernels.cc)
 # link boost
@@ -78,121 +93,123 @@
 # create link of shared object to lib folder inside CLUEstering directory
 file(GLOB CONV_MODULE ./build/lib/CLUEstering/lib/CLUE_CPU_Serial*.so)
 foreach(CONV_MODULE ${CONV_MODULE})
   execute_process(COMMAND ln -sf ${CONV_MODULE}
                           ./CLUEstering/lib/CLUE_CPU_Serial.so)
 endforeach()
 
-find_package(TBB)
+if(NOT ${SERIAL_ONLY})
+  find_package(TBB)
 
-# CPU TBB
-if(TBB_FOUND)
-  # compile cpu tbb module
-  pybind11_add_module(CLUE_CPU_TBB SHARED
-                      ./CLUEstering/alpaka/BindingModules/binding_cpu_tbb.cc)
-  target_link_libraries(CLUE_CPU_TBB PRIVATE ${Boost_LIBRARIES})
-  target_include_directories(CLUE_CPU_TBB PRIVATE ${Boost_PATH})
-  target_compile_options(
-    CLUE_CPU_TBB
-    PRIVATE -ltbb -DALPAKA_ACC_CPU_B_TBB_T_SEQ_PRESENT
-            -DALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLED
-            -DALPAKA_ACC_CPU_B_TBB_T_SEQ_ASYNC_BACKEND)
-  target_link_libraries(CLUE_CPU_TBB PRIVATE TBB::tbb)
-  set_target_properties(CLUE_CPU_TBB PROPERTIES LIBRARY_OUTPUT_DIRECTORY
-                                                ./lib/CLUEstering/lib/)
-  # create link of shared object to lib folder inside CLUEstering directory
-  file(GLOB CONV_MODULE ./build/lib/CLUEstering/lib/CLUE_CPU_TBB*.so)
-  foreach(CONV_MODULE ${CONV_MODULE})
-    execute_process(COMMAND ln -sf ${CONV_MODULE}
-                            ./CLUEstering/lib/CLUE_CPU_TBB.so)
-  endforeach()
-endif()
-
-# check if CUDA is available
-include(CheckLanguage)
-check_language(CUDA)
-
-# GPU CUDA
-if(CMAKE_CUDA_COMPILER)
-  # enable CUDA
-  enable_language(CUDA)
-  set(CMAKE_CUDA_HOST_COMPILER ${CMAKE_CUDA_COMPILER})
-
-  # set the CUDA standard
-  if(NOT DEFINED CMAKE_CUDA_STANDARD)
-    set(CMAKE_CUDA_STANDARD 17)
-    set(CMAKE_CUDA_STANDARD_REQUIRED ON)
+  # CPU TBB
+  if(TBB_FOUND)
+    # compile cpu tbb module
+    pybind11_add_module(CLUE_CPU_TBB SHARED
+                        ./CLUEstering/alpaka/BindingModules/binding_cpu_tbb.cc)
+    target_link_libraries(CLUE_CPU_TBB PRIVATE ${Boost_LIBRARIES})
+    target_include_directories(CLUE_CPU_TBB PRIVATE ${Boost_PATH})
+    target_compile_options(
+      CLUE_CPU_TBB
+      PRIVATE -ltbb -DALPAKA_ACC_CPU_B_TBB_T_SEQ_PRESENT
+              -DALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLED
+              -DALPAKA_ACC_CPU_B_TBB_T_SEQ_ASYNC_BACKEND)
+    target_link_libraries(CLUE_CPU_TBB PRIVATE TBB::tbb)
+    set_target_properties(CLUE_CPU_TBB PROPERTIES LIBRARY_OUTPUT_DIRECTORY
+                                                  ./lib/CLUEstering/lib/)
+    # create link of shared object to lib folder inside CLUEstering directory
+    file(GLOB CONV_MODULE ./build/lib/CLUEstering/lib/CLUE_CPU_TBB*.so)
+    foreach(CONV_MODULE ${CONV_MODULE})
+      execute_process(COMMAND ln -sf ${CONV_MODULE}
+                              ./CLUEstering/lib/CLUE_CPU_TBB.so)
+    endforeach()
   endif()
+endif()
 
-  set(CMAKE_CUDA_FLAGS "-Wall -Wextra -g -O2")
+if((NOT ${CPU_ONLY}) AND (NOT ${SERIAL_ONLY}))
+  # check if CUDA is available
+  include(CheckLanguage)
+  check_language(CUDA)
+
+  # GPU CUDA
+  if(CMAKE_CUDA_COMPILER)
+    # enable CUDA
+    enable_language(CUDA)
+    set(CMAKE_CUDA_HOST_COMPILER ${CMAKE_CUDA_COMPILER})
+
+    # set the CUDA standard
+    if(NOT DEFINED CMAKE_CUDA_STANDARD)
+      set(CMAKE_CUDA_STANDARD 17)
+      set(CMAKE_CUDA_STANDARD_REQUIRED ON)
+    endif()
+
+    # compile the file with .cc extension using nvcc
+    set_source_files_properties(
+      ./CLUEstering/alpaka/BindingModules/binding_gpu_cuda.cc
+      PROPERTIES LANGUAGE CUDA)
+    # compile gpu cuda module
+    pybind11_add_module(CLUE_GPU_CUDA SHARED
+                        ./CLUEstering/alpaka/BindingModules/binding_gpu_cuda.cc)
+    # link boost
+    target_link_libraries(CLUE_Convolutional_Kernels PRIVATE ${Boost_LIBRARIES})
+    target_include_directories(CLUE_Convolutional_Kernels PRIVATE ${Boost_PATH})
+    # set the cuda architectures
+    set_target_properties(CLUE_GPU_CUDA PROPERTIES CUDA_ARCHITECTURES
+                                                   "50;60;61;62;70")
+    # alpaka build flags
+    target_compile_options(
+      CLUE_GPU_CUDA
+      PRIVATE -DALPAKA_ACC_GPU_CUDA_PRESENT -DALPAKA_ACC_GPU_CUDA_ENABLED
+              -DALPAKA_ACC_GPU_CUDA_ASYNC_BACKEND)
+    # nvcc compilation flags
+    target_compile_options(
+      CLUE_GPU_CUDA PRIVATE --expt-relaxed-constexpr -gencode
+                            arch=compute_61,code=[sm_61,compute_61])
+    # set output directory
+    set_target_properties(CLUE_GPU_CUDA PROPERTIES LIBRARY_OUTPUT_DIRECTORY
+                                                   ./lib/CLUEstering/lib/)
+    # create link of shared object to lib folder inside CLUEstering directory
+    file(GLOB CONV_MODULE ./build/lib/CLUEstering/lib/CLUE_GPU_CUDA*.so)
+    foreach(CONV_MODULE ${CONV_MODULE})
+      execute_process(COMMAND ln -sf ${CONV_MODULE}
+                              ./CLUEstering/lib/CLUE_GPU_CUDA.so)
+    endforeach()
+  endif()
 
-  # compile the file with .cc extension using nvcc
-  set_source_files_properties(
-    ./CLUEstering/alpaka/BindingModules/binding_gpu_cuda.cc PROPERTIES LANGUAGE
-                                                                       CUDA)
-  # compile gpu cuda module
-  pybind11_add_module(CLUE_GPU_CUDA SHARED
-                      ./CLUEstering/alpaka/BindingModules/binding_gpu_cuda.cc)
-  # link boost
-  target_link_libraries(CLUE_Convolutional_Kernels PRIVATE ${Boost_LIBRARIES})
-  target_include_directories(CLUE_Convolutional_Kernels PRIVATE ${Boost_PATH})
-  # set the cuda architectures
-  set_target_properties(CLUE_GPU_CUDA PROPERTIES CUDA_ARCHITECTURES
-                                                 "50;60;61;62;70")
-  # alpaka build flags
-  target_compile_options(
-    CLUE_GPU_CUDA
-    PRIVATE -DALPAKA_ACC_GPU_CUDA_PRESENT -DALPAKA_ACC_GPU_CUDA_ENABLED
-            -DALPAKA_ACC_GPU_CUDA_ASYNC_BACKEND)
-  # nvcc compilation flags
-  target_compile_options(
-    CLUE_GPU_CUDA PRIVATE --expt-relaxed-constexpr -gencode
-                          arch=compute_61,code=[sm_61,compute_61])
-  # set output directory
-  set_target_properties(CLUE_GPU_CUDA PROPERTIES LIBRARY_OUTPUT_DIRECTORY
-                                                 ./lib/CLUEstering/lib/)
-  # create link of shared object to lib folder inside CLUEstering directory
-  file(GLOB CONV_MODULE ./build/lib/CLUEstering/lib/CLUE_GPU_CUDA*.so)
-  foreach(CONV_MODULE ${CONV_MODULE})
-    execute_process(COMMAND ln -sf ${CONV_MODULE}
-                            ./CLUEstering/lib/CLUE_GPU_CUDA.so)
-  endforeach()
-endif()
-
-# GPU HIP check if HIP is available
-check_language(HIP)
-if(CMAKE_HIP_COMPILER)
-  # enable HIP
-  enable_language(HIP)
-  set(CMAKE_HIP_HOST_COMPILER ${CMAKE_HIP_COMPILER})
-
-  # look for the hip package folder
-  find_package(hip)
-
-  set(hip_BASE "${hip_INCLUDE_DIRS}/..")
-  # set the hipcc compiler
-  set(CMAKE_CXX_COMPILER "${hip_BASE}/bin/hipcc")
-  # compile gpu hip module
-  pybind11_add_module(CLUE_GPU_HIP SHARED
-                      ./CLUEstering/alpaka/BindingModules/binding_gpu_hip.cc)
-  # link boost
-  target_link_libraries(CLUE_Convolutional_Kernels PRIVATE ${Boost_LIBRARIES})
-  target_include_directories(CLUE_Convolutional_Kernels PRIVATE ${Boost_PATH})
-  # alpaka build flags
-  target_compile_options(
-    CLUE_GPU_HIP
-    PRIVATE -DALPAKA_ACC_GPU_HIP_PRESENT -DALPAKA_ACC_GPU_HIP_ENABLED
-            -DALPAKA_ACC_GPU_HIP_ASYNC_BACKEND)
-  # link hip-rand libraries
-  target_include_directories(CLUE_GPU_HIP PRIVATE ${hip_INCLUDE_DIRS})
-  target_include_directories(CLUE_GPU_HIP PRIVATE ${hip_BASE}/hiprand/include)
-  target_include_directories(CLUE_GPU_HIP PRIVATE ${hip_BASE}/rocrand/include)
-  # set output directory
-  set_target_properties(CLUE_GPU_HIP PROPERTIES LIBRARY_OUTPUT_DIRECTORY
-                                                ./lib/CLUEstering/lib/)
-  # create link of shared object to lib folder inside CLUEstering directory
-  file(GLOB CONV_MODULE ./build/lib/CLUEstering/lib/CLUE_GPU_HIP*.so)
-  foreach(CONV_MODULE ${CONV_MODULE})
-    execute_process(COMMAND ln -sf ${CONV_MODULE}
-                            ./CLUEstering/lib/CLUE_GPU_HIP.so)
-  endforeach()
+  # GPU HIP check if HIP is available
+  check_language(HIP)
+  if(CMAKE_HIP_COMPILER)
+    # enable HIP
+    enable_language(HIP)
+    set(CMAKE_HIP_HOST_COMPILER ${CMAKE_HIP_COMPILER})
+
+    # look for the hip package folder
+    find_package(hip)
+
+    set(hip_BASE "${hip_INCLUDE_DIRS}/..")
+    # set the hipcc compiler
+    set(CMAKE_CXX_COMPILER "${hip_BASE}/bin/hipcc")
+    # compile gpu hip module
+    pybind11_add_module(CLUE_GPU_HIP SHARED
+                        ./CLUEstering/alpaka/BindingModules/binding_gpu_hip.cc)
+    # link boost
+    target_link_libraries(CLUE_Convolutional_Kernels PRIVATE ${Boost_LIBRARIES})
+    target_include_directories(CLUE_Convolutional_Kernels PRIVATE ${Boost_PATH})
+    # alpaka build flags
+    target_compile_options(
+      CLUE_GPU_HIP
+      PRIVATE -DALPAKA_ACC_GPU_HIP_PRESENT -DALPAKA_ACC_GPU_HIP_ENABLED
+              -DALPAKA_ACC_GPU_HIP_ASYNC_BACKEND)
+    # link hip-rand libraries
+    target_include_directories(CLUE_GPU_HIP PRIVATE ${hip_INCLUDE_DIRS})
+    target_include_directories(CLUE_GPU_HIP PRIVATE ${hip_BASE}/hiprand/include)
+    target_include_directories(CLUE_GPU_HIP PRIVATE ${hip_BASE}/rocrand/include)
+    # set output directory
+    set_target_properties(CLUE_GPU_HIP PROPERTIES LIBRARY_OUTPUT_DIRECTORY
+                                                  ./lib/CLUEstering/lib/)
+    # create link of shared object to lib folder inside CLUEstering directory
+    file(GLOB CONV_MODULE ./build/lib/CLUEstering/lib/CLUE_GPU_HIP*.so)
+    foreach(CONV_MODULE ${CONV_MODULE})
+      execute_process(COMMAND ln -sf ${CONV_MODULE}
+                              ./CLUEstering/lib/CLUE_GPU_HIP.so)
+    endforeach()
+  endif()
 endif()
```

### Comparing `CLUEstering-2.2.0/LICENSE` & `CLUEstering-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/PKG-INFO` & `CLUEstering-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLUEstering
-Version: 2.2.0
+Version: 2.2.1
 Summary: A library that generalizes the original 2-dimensional CLUE
 Author: Simone Balducci
 Author-email: simone.balducci00@gmail.com
 Keywords: Python,Clustering,Binding
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `CLUEstering-2.2.0/README.md` & `CLUEstering-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/.clang-format` & `CLUEstering-2.2.1/extern/alpaka/.clang-format`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/.github/workflows/ci.yml` & `CLUEstering-2.2.1/extern/alpaka/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/.github/workflows/gh-pages.yml` & `CLUEstering-2.2.1/extern/alpaka/.github/workflows/gh-pages.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/.gitignore` & `CLUEstering-2.2.1/extern/alpaka/.gitignore`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/.gitlab-ci.yml` & `CLUEstering-2.2.1/extern/alpaka/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/.zenodo.json` & `CLUEstering-2.2.1/extern/alpaka/.zenodo.json`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/CHANGELOG.md` & `CLUEstering-2.2.1/extern/alpaka/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/CONTRIBUTING.md` & `CLUEstering-2.2.1/extern/alpaka/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/LICENSE` & `CLUEstering-2.2.1/extern/alpaka/LICENSE`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/README.md` & `CLUEstering-2.2.1/extern/alpaka/README.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/README_OACC.md` & `CLUEstering-2.2.1/extern/alpaka/README_OACC.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/README_OMP5.md` & `CLUEstering-2.2.1/extern/alpaka/README_OMP5.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/README_SYCL.md` & `CLUEstering-2.2.1/extern/alpaka/README_SYCL.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/cmake/addExecutable.cmake` & `CLUEstering-2.2.1/extern/alpaka/cmake/addExecutable.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/cmake/addLibrary.cmake` & `CLUEstering-2.2.1/extern/alpaka/cmake/addLibrary.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/cmake/alpakaCommon.cmake` & `CLUEstering-2.2.1/extern/alpaka/cmake/alpakaCommon.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/cmake/alpakaConfig.cmake.in` & `CLUEstering-2.2.1/extern/alpaka/cmake/alpakaConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/cmake/common.cmake` & `CLUEstering-2.2.1/extern/alpaka/cmake/common.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/Doxyfile` & `CLUEstering-2.2.1/extern/alpaka/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/Makefile` & `CLUEstering-2.2.1/extern/alpaka/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/cheatsheet/cheatsheet.style` & `CLUEstering-2.2.1/extern/alpaka/docs/cheatsheet/cheatsheet.style`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka.pdf` & `CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka.pdf`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka.svg` & `CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka.svg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka_401x135.png` & `CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka_401x135.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka_doxygen.png` & `CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka_doxygen.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/logo/alpaka_inkscape.svg` & `CLUEstering-2.2.1/extern/alpaka/docs/logo/alpaka_inkscape.svg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/advanced/cmake.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/advanced/cmake.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/advanced/compiler.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/advanced/compiler.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/advanced/mapping.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/advanced/mapping.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/advanced/rationale.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/advanced/rationale.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/basic/abstraction.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/basic/abstraction.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/basic/cheatsheet.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/basic/cheatsheet.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/basic/example.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/basic/example.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/basic/install.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/basic/install.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/basic/intro.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/basic/intro.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/basic/library.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/basic/library.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/conf.py` & `CLUEstering-2.2.1/extern/alpaka/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/dev/backends.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/dev/backends.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/dev/ci.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/dev/ci.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/dev/details.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/dev/details.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/dev/sphinx.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/dev/sphinx.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/dev/style.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/dev/style.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/dev/test.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/dev/test.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/arch_gitlab_mirror.svg` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/arch_gitlab_mirror.svg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/block.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/block.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/block_scale.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/block_scale.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/element.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/element.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/execution_domain.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/execution_domain.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/execution_domain.svg` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/execution_domain.svg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/job_generator_flow.svg` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/job_generator_flow.svg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/structure.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/structure.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/structure.svg` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/structure.svg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/structure_assoc.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/structure_assoc.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/structure_assoc.svg` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/structure_assoc.svg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/thread.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/thread.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/warp.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/warp.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/x86_cpu.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/x86_cpu.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/images/x86_cpu_mapping.png` & `CLUEstering-2.2.1/extern/alpaka/docs/source/images/x86_cpu_mapping.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/index.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/docs/source/info/similar_projects.rst` & `CLUEstering-2.2.1/extern/alpaka/docs/source/info/similar_projects.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/babelstream/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/babelstream/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/AlpakaStream.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/AlpakaStream.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/AlpakaStream.h` & `CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/AlpakaStream.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/LICENSE` & `CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/LICENSE`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/Stream.h` & `CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/Stream.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/babelstream/src/main.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/babelstream/src/main.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/bufferCopy/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/bufferCopy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/bufferCopy/src/bufferCopy.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/bufferCopy/src/bufferCopy.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/complex/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/complex/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/complex/src/complex.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/complex/src/complex.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/counterBasedRng/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/counterBasedRng/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/counterBasedRng/src/counterBasedRng.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/counterBasedRng/src/counterBasedRng.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/heatEquation/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/heatEquation/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/heatEquation/src/heatEquation.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/heatEquation/src/heatEquation.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/helloWorld/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/helloWorld/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/helloWorld/src/helloWorld.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/helloWorld/src/helloWorld.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/helloWorldLambda/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/helloWorldLambda/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/helloWorldLambda/src/helloWorldLambda.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/helloWorldLambda/src/helloWorldLambda.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/kernelSpecialization/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/kernelSpecialization/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/kernelSpecialization/src/kernelSpecialization.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/kernelSpecialization/src/kernelSpecialization.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/monteCarloIntegration/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/monteCarloIntegration/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/monteCarloIntegration/src/monteCarloIntegration.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/monteCarloIntegration/src/monteCarloIntegration.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/openMPSchedule/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/openMPSchedule/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/openMPSchedule/src/openMPSchedule.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/openMPSchedule/src/openMPSchedule.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/parallelLoopPatterns/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/parallelLoopPatterns/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/parallelLoopPatterns/src/parallelLoopPatterns.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/parallelLoopPatterns/src/parallelLoopPatterns.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/randomCells2D/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/randomCells2D/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/randomCells2D/src/randomCells2D.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/randomCells2D/src/randomCells2D.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/randomStrategies/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/randomStrategies/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/randomStrategies/src/randomStrategies.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/randomStrategies/src/randomStrategies.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/reduce/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/reduce/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/reduce/README.md` & `CLUEstering-2.2.1/extern/alpaka/example/reduce/README.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/reduce/src/alpakaConfig.hpp` & `CLUEstering-2.2.1/extern/alpaka/example/reduce/src/alpakaConfig.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/reduce/src/iterator.hpp` & `CLUEstering-2.2.1/extern/alpaka/example/reduce/src/iterator.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/reduce/src/kernel.hpp` & `CLUEstering-2.2.1/extern/alpaka/example/reduce/src/kernel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/reduce/src/reduce.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/reduce/src/reduce.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/tagSpecialization/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/tagSpecialization/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/tagSpecialization/src/tagSpecialization.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/tagSpecialization/src/tagSpecialization.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/vectorAdd/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/example/vectorAdd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/example/vectorAdd/src/vectorAdd.cpp` & `CLUEstering-2.2.1/extern/alpaka/example/vectorAdd/src/vectorAdd.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuOmp2Blocks.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuOmp2Blocks.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuOmp2Threads.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuOmp2Threads.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuSerial.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuSerial.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuTbbBlocks.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuTbbBlocks.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccCpuThreads.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccCpuThreads.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccDevProps.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccDevProps.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccFpgaSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccFpgaSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccFpgaSyclXilinx.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccFpgaSyclXilinx.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGpuCudaRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGpuCudaRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGpuHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGpuHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccGpuUniformCudaHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccGpuUniformCudaHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccOacc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccOacc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/AccOmp5.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/AccOmp5.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/Tag.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/Tag.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/acc/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/acc/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/alpaka.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/alpaka.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicAtomicRef.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicAtomicRef.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicCpu.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicCpu.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicHierarchy.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicHierarchy.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicNoOp.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicNoOp.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicOaccBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicOaccBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicOaccExtended.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicOaccExtended.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicOmpBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicOmpBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicStdLibLock.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicStdLibLock.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicUniformCudaHip.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicUniformCudaHip.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/AtomicUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/AtomicUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/Op.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/Op.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/atomic/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/atomic/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/OffloadUseBuiltInSharedMem.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/OffloadUseBuiltInSharedMem.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedDynMemberAllocKiB.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedDynMemberAllocKiB.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynMember.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynMember.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynOmp5BuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynOmp5BuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/BlockSharedMemDynUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/dyn/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/dyn/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStMember.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStMember.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStMemberMasterSync.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStMemberMasterSync.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStOmp5.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStOmp5.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStOmp5BuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStOmp5BuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/BlockSharedMemStUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/shared/st/detail/BlockSharedMemStMemberImpl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/shared/st/detail/BlockSharedMemStMemberImpl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierOacc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierOacc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierOmp.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierOmp.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierThread.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncBarrierThread.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncNoOp.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncNoOp.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/BlockSyncUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/BlockSyncUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/block/sync/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/block/sync/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Align.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Align.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/AlignedAlloc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/AlignedAlloc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ApiCudaRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ApiCudaRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ApiHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ApiHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Assert.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Assert.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/BarrierThread.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/BarrierThread.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/BoostPredef.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/BoostPredef.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/CallbackThread.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/CallbackThread.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ClipCast.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ClipCast.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Common.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Common.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Concepts.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Concepts.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ConcurrentExecPool.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ConcurrentExecPool.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Cuda.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Cuda.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/CudaHipCommon.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/CudaHipCommon.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Debug.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Debug.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Decay.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Decay.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/DemangleTypeNames.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/DemangleTypeNames.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Hip.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Hip.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Omp5.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Omp5.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/OmpSchedule.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/OmpSchedule.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Positioning.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Positioning.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/RemoveRestrict.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/RemoveRestrict.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/STLTuple/LICENSE.txt` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/STLTuple/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/STLTuple/STLTuple.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/STLTuple/STLTuple.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Sycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Sycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/ThreadTraits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/ThreadTraits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Tuple.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Tuple.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/UniformCudaHip.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/UniformCudaHip.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Unreachable.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Unreachable.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Unroll.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Unroll.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Utility.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Utility.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/core/Vectorize.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/core/Vectorize.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/ctx/block/CtxBlockOacc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/ctx/block/CtxBlockOacc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevCpu.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevCpu.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevCpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevCpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevCudaRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevCudaRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevFpgaSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevFpgaSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevFpgaSyclXilinx.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevFpgaSyclXilinx.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevGpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevGpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevOacc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevOacc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevOmp5.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevOmp5.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/DevUniformCudaHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/DevUniformCudaHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/common/QueueRegistry.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/common/QueueRegistry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/cpu/SysInfo.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/cpu/SysInfo.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dev/cpu/Wait.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dev/cpu/Wait.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dim/DimArithmetic.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dim/DimArithmetic.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dim/DimIntegralConst.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dim/DimIntegralConst.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/dim/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/dim/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/elem/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/elem/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventCpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventCpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventCudaRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventCudaRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventFpgaSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventFpgaSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventFpgaSyclXilinx.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventFpgaSyclXilinx.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventGenericThreads.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventGenericThreads.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventGpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventGpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventOacc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventOacc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventOmp5.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventOmp5.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/EventUniformCudaHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/EventUniformCudaHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/event/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/event/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/example/ExampleDefaultAcc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/example/ExampleDefaultAcc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/extent/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/extent/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/Accessors.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/Accessors.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/MapIdx.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/MapIdx.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtLinear.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtLinear.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtOmp.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtOmp.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtRefThreadIdMap.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtRefThreadIdMap.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/bt/IdxBtZero.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/bt/IdxBtZero.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/gb/IdxGbGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/gb/IdxGbGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/gb/IdxGbLinear.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/gb/IdxGbLinear.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/gb/IdxGbRef.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/gb/IdxGbRef.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/idx/gb/IdxGbUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/idx/gb/IdxGbUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/IntrinsicCpu.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/IntrinsicCpu.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/IntrinsicFallback.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/IntrinsicFallback.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/IntrinsicGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/IntrinsicGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/IntrinsicUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/IntrinsicUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/intrinsic/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/intrinsic/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuOmp2Blocks.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuOmp2Blocks.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuOmp2Threads.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuOmp2Threads.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuSerial.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuSerial.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuTbbBlocks.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuTbbBlocks.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelCpuThreads.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelCpuThreads.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelFpgaSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelFpgaSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelFpgaSyclXilinx.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelFpgaSyclXilinx.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGpuCudaRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGpuCudaRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGpuHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGpuHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelGpuUniformCudaHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelGpuUniformCudaHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelOacc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelOacc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/TaskKernelOmp5.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/TaskKernelOmp5.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/kernel/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/kernel/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/Complex.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/Complex.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/FloatEqualExact.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/FloatEqualExact.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/MathGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/MathGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/MathStdLib.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/MathStdLib.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/MathUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/MathUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/math/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/math/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/alloc/AllocCpuAligned.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/alloc/AllocCpuAligned.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/alloc/AllocCpuNew.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/alloc/AllocCpuNew.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/alloc/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/alloc/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufCpu.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufCpu.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufCpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufCpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufCudaRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufCudaRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufFpgaSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufFpgaSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufFpgaSyclXilinx.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufFpgaSyclXilinx.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufGpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufGpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufOacc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufOacc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufOmp5.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufOmp5.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/BufUniformCudaHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/BufUniformCudaHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/SetKernel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/SetKernel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/cpu/Copy.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/cpu/Copy.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/cpu/Set.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/cpu/Set.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/oacc/Copy.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/oacc/Copy.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/oacc/Set.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/oacc/Set.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/omp5/Copy.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/omp5/Copy.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/omp5/Set.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/omp5/Set.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/sycl/Accessor.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/sycl/Accessor.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/sycl/Common.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/sycl/Common.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/sycl/Copy.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/sycl/Copy.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/sycl/Set.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/sycl/Set.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/Copy.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/Copy.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/Set.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/buf/uniformCudaHip/Set.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceCpu.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceCpu.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceCpuSerial.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceCpuSerial.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceOacc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceOacc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp2Blocks.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp2Blocks.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp2Threads.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp2Threads.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp5.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceOmp5.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/MemFenceUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/MemFenceUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/fence/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/fence/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/Accessor.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/Accessor.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewAccessOps.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewAccessOps.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewAccessor.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewAccessor.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewConst.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewConst.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewPlainPtr.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewPlainPtr.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewStdArray.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewStdArray.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewStdVector.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewStdVector.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/mem/view/ViewSubView.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/mem/view/ViewSubView.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Apply.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Apply.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/CartesianProduct.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/CartesianProduct.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Concatenate.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Concatenate.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/CudaVectorArrayWrapper.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/CudaVectorArrayWrapper.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/DependentFalseType.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/DependentFalseType.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Filter.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Filter.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Fold.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Fold.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/ForEachType.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/ForEachType.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Functional.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Functional.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/InheritFromList.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/InheritFromList.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/IntegerSequence.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/IntegerSequence.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Integral.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Integral.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/IsArrayOrVector.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/IsArrayOrVector.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/IsStrictBase.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/IsStrictBase.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/NdLoop.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/NdLoop.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Set.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Set.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Transform.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Transform.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/TypeListOps.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/TypeListOps.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/meta/Unique.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/meta/Unique.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/offset/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/offset/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfCpu.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfCpu.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfCpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfCpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfCudaRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfCudaRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfFpgaSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfFpgaSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfFpgaSyclXilinx.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfFpgaSyclXilinx.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfGpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfGpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfOacc.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfOacc.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfOmp5.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfOmp5.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/PltfUniformCudaHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/PltfUniformCudaHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/pltf/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/pltf/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/Properties.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/Properties.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCpuSyclIntelBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCpuSyclIntelBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCpuSyclIntelNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCpuSyclIntelNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCudaRtBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCudaRtBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueCudaRtNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueCudaRtNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueFpgaSyclIntelBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueFpgaSyclIntelBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueFpgaSyclIntelNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueFpgaSyclIntelNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueFpgaSyclXilinxBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueFpgaSyclXilinxBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueFpgaSyclXilinxNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueFpgaSyclXilinxNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGenericSyclBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGenericSyclBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGenericSyclNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGenericSyclNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGenericThreadsBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGenericThreadsBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGenericThreadsNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGenericThreadsNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGpuSyclIntelBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGpuSyclIntelBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueGpuSyclIntelNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueGpuSyclIntelNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueHipRtBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueHipRtBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueHipRtNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueHipRtNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueOaccBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueOaccBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueOaccNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueOaccNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueOmp5Blocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueOmp5Blocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueOmp5NonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueOmp5NonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueUniformCudaHipRtBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueUniformCudaHipRtBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/QueueUniformCudaHipRtNonBlocking.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/QueueUniformCudaHipRtNonBlocking.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/cpu/ICpuQueue.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/cpu/ICpuQueue.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/cpu/IGenericThreadsQueue.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/cpu/IGenericThreadsQueue.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/cuda_hip/QueueUniformCudaHipRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/cuda_hip/QueueUniformCudaHipRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/queue/sycl/QueueGenericSyclBase.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/queue/sycl/QueueGenericSyclBase.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/MultiplyAndSplit64to32.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/MultiplyAndSplit64to32.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseCommon.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseCommon.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseCudaArray.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseCudaArray.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseStdArray.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseStdArray.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseTraits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxBaseTraits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxConstants.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxConstants.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxSingle.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxSingle.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxStateless.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxStateless.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxStatelessKeyedBase.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxStatelessKeyedBase.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxStatelessVector.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxStatelessVector.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Philox/PhiloxVector.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Philox/PhiloxVector.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandDefault.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandDefault.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandPhilox.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandPhilox.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandPhiloxStateless.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandPhiloxStateless.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandStdLib.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandStdLib.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/RandUniformCudaHipRand.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/RandUniformCudaHipRand.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/TinyMT/Engine.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/TinyMT/Engine.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/TinyMT/LICENSE.txt` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/TinyMT/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/TinyMT/tinymt32.h` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/TinyMT/tinymt32.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/rand/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/rand/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/CpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/CpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/FpgaSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/FpgaSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/GpuCudaRt.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/GpuCudaRt.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/standalone/GpuSyclIntel.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/standalone/GpuSyclIntel.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/Array.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/Array.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/Check.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/Check.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/Extent.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/Extent.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/KernelExecutionFixture.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/KernelExecutionFixture.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/MeasureKernelRunTime.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/MeasureKernelRunTime.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/acc/TestAccs.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/acc/TestAccs.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/dim/TestDims.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/dim/TestDims.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/event/EventHostManualTrigger.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/event/EventHostManualTrigger.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/idx/TestIdxs.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/idx/TestIdxs.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/mem/view/Iterator.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/mem/view/Iterator.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/mem/view/ViewTest.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/mem/view/ViewTest.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/queue/Queue.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/queue/Queue.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/queue/QueueCpuOmp2Collective.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/queue/QueueCpuOmp2Collective.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/test/queue/QueueTestFixture.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/test/queue/QueueTestFixture.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/traits/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/traits/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/vec/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/vec/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/vec/Vec.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/vec/Vec.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/version.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/version.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/wait/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/wait/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/warp/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/warp/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/warp/WarpGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/warp/WarpGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/warp/WarpSingleThread.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/warp/WarpSingleThread.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/warp/WarpUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/warp/WarpUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/Traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/Traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/WorkDivGenericSycl.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/WorkDivGenericSycl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/WorkDivHelpers.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/WorkDivHelpers.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/WorkDivMembers.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/WorkDivMembers.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/include/alpaka/workdiv/WorkDivUniformCudaHipBuiltIn.hpp` & `CLUEstering-2.2.1/extern/alpaka/include/alpaka/workdiv/WorkDivUniformCudaHipBuiltIn.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/before_install.sh` & `CLUEstering-2.2.1/extern/alpaka/script/before_install.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/ci.sh` & `CLUEstering-2.2.1/extern/alpaka/script/ci.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/docker_ci.sh` & `CLUEstering-2.2.1/extern/alpaka/script/docker_ci.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/docker_retry.sh` & `CLUEstering-2.2.1/extern/alpaka/script/docker_retry.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/gitlab_ci_run.sh` & `CLUEstering-2.2.1/extern/alpaka/script/gitlab_ci_run.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/gitlabci/job_base.yml` & `CLUEstering-2.2.1/extern/alpaka/script/gitlabci/job_base.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/gitlabci/job_clang.yml` & `CLUEstering-2.2.1/extern/alpaka/script/gitlabci/job_clang.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/gitlabci/job_cuda11.0.yml` & `CLUEstering-2.2.1/extern/alpaka/script/gitlabci/job_cuda11.0.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/gitlabci/job_cuda11.8.yml` & `CLUEstering-2.2.1/extern/alpaka/script/gitlabci/job_cuda11.8.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/gitlabci/print_env.sh` & `CLUEstering-2.2.1/extern/alpaka/script/gitlabci/print_env.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install_analysis.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install_analysis.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install_boost.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install_boost.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install_clang.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install_clang.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install_cmake.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install_cmake.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install_cuda.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install_cuda.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install_gcc.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install_gcc.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install_hip.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install_hip.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install_oneapi.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install_oneapi.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/install_tbb.sh` & `CLUEstering-2.2.1/extern/alpaka/script/install_tbb.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/job_generator/alpaka_filter.py` & `CLUEstering-2.2.1/extern/alpaka/script/job_generator/alpaka_filter.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/job_generator/alpaka_globals.py` & `CLUEstering-2.2.1/extern/alpaka/script/job_generator/alpaka_globals.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/job_generator/custom_job.py` & `CLUEstering-2.2.1/extern/alpaka/script/job_generator/custom_job.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/job_generator/generate_job_yaml.py` & `CLUEstering-2.2.1/extern/alpaka/script/job_generator/generate_job_yaml.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/job_generator/job_generator.py` & `CLUEstering-2.2.1/extern/alpaka/script/job_generator/job_generator.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/job_generator/job_modifier.py` & `CLUEstering-2.2.1/extern/alpaka/script/job_generator/job_modifier.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/job_generator/reorder_jobs.py` & `CLUEstering-2.2.1/extern/alpaka/script/job_generator/reorder_jobs.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/job_generator/verify.py` & `CLUEstering-2.2.1/extern/alpaka/script/job_generator/verify.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/job_generator/versions.py` & `CLUEstering-2.2.1/extern/alpaka/script/job_generator/versions.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/prepare_sanitizers.sh` & `CLUEstering-2.2.1/extern/alpaka/script/prepare_sanitizers.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/print_env.sh` & `CLUEstering-2.2.1/extern/alpaka/script/print_env.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/push_doc.sh` & `CLUEstering-2.2.1/extern/alpaka/script/push_doc.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/run.sh` & `CLUEstering-2.2.1/extern/alpaka/script/run.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/run_analysis.sh` & `CLUEstering-2.2.1/extern/alpaka/script/run_analysis.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/run_build.sh` & `CLUEstering-2.2.1/extern/alpaka/script/run_build.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/run_doxygen.sh` & `CLUEstering-2.2.1/extern/alpaka/script/run_doxygen.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/run_generate.sh` & `CLUEstering-2.2.1/extern/alpaka/script/run_generate.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/run_install.sh` & `CLUEstering-2.2.1/extern/alpaka/script/run_install.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/run_tests.sh` & `CLUEstering-2.2.1/extern/alpaka/script/run_tests.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/set.sh` & `CLUEstering-2.2.1/extern/alpaka/script/set.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/script/travis_retry.sh` & `CLUEstering-2.2.1/extern/alpaka/script/travis_retry.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/analysis/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/analysis/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/analysis/headerCheck/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/analysis/headerCheck/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/common/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/common/devCompileOptions.cmake` & `CLUEstering-2.2.1/extern/alpaka/test/common/devCompileOptions.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/integ/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/axpy/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/integ/axpy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/axpy/src/axpy.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/integ/axpy/src/axpy.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/cudaOnly/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/integ/cudaOnly/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/cudaOnly/src/cudaNativeFunctions.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/integ/cudaOnly/src/cudaNativeFunctions.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/hostOnlyAPI/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/integ/hostOnlyAPI/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/hostOnlyAPI/src/hostOnlyAPI.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/integ/hostOnlyAPI/src/hostOnlyAPI.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/mandelbrot/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/integ/mandelbrot/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/mandelbrot/src/mandelbrot.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/integ/mandelbrot/src/mandelbrot.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/matMul/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/integ/matMul/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/matMul/src/matMul.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/integ/matMul/src/matMul.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/src/main.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/src/main.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/separableCompilation/src/mysqrt.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/integ/separableCompilation/src/mysqrt.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/sharedMem/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/integ/sharedMem/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/sharedMem/src/sharedMem.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/integ/sharedMem/src/sharedMem.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/zeroDimBuffer/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/integ/zeroDimBuffer/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/integ/zeroDimBuffer/src/zeroDimBuffer.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/integ/zeroDimBuffer/src/zeroDimBuffer.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/sanitizer_ubsan_blacklist.txt` & `CLUEstering-2.2.1/extern/alpaka/test/sanitizer_ubsan_blacklist.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/acc/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/acc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/acc/src/AccDevPropsTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/acc/src/AccDevPropsTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/acc/src/AccNameTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/acc/src/AccNameTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/acc/src/AccTagTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/acc/src/AccTagTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/atomic/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/atomic/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/atomic/src/AtomicTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/atomic/src/AtomicTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/block/shared/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/block/shared/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/block/shared/src/BlockSharedMemDyn.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/block/shared/src/BlockSharedMemDyn.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/block/shared/src/BlockSharedMemSt.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/block/shared/src/BlockSharedMemSt.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/block/sharedSharing/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/block/sharedSharing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/block/sharedSharing/src/BlockSharedMemSharing.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/block/sharedSharing/src/BlockSharedMemSharing.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/block/sync/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/block/sync/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/block/sync/src/BlockSync.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/block/sync/src/BlockSync.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/block/sync/src/BlockSyncPredicate.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/block/sync/src/BlockSyncPredicate.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/core/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/BoostPredefTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/BoostPredefTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/ClipCastTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/ClipCastTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/ConceptsTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/ConceptsTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/OmpScheduleTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/OmpScheduleTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/core/src/Utility.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/core/src/Utility.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/dev/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/dev/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/dev/src/DevWarpSizeTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/dev/src/DevWarpSizeTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/event/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/event/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/event/src/EventTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/event/src/EventTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/idx/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/idx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/idx/src/MapIdx.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/idx/src/MapIdx.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/idx/src/MapIdxPitchBytes.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/idx/src/MapIdxPitchBytes.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/intrinsic/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/intrinsic/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/intrinsic/src/Ffs.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/intrinsic/src/Ffs.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/intrinsic/src/Popcount.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/intrinsic/src/Popcount.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelGenericLambda.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelGenericLambda.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelLambda.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelLambda.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithAdditionalParam.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithAdditionalParam.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithConstructorAndMember.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithConstructorAndMember.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithHostConstexpr.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithHostConstexpr.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithOmpSchedule.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithOmpSchedule.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithTemplate.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithTemplate.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithTemplateArgumentDeduction.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithTemplateArgumentDeduction.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/kernel/src/KernelWithoutTemplatedAccParam.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/kernel/src/KernelWithoutTemplatedAccParam.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/Buffer.hpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/Buffer.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/DataGen.hpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/DataGen.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/Defines.hpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/Defines.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/FloatEqualExactTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/FloatEqualExactTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/Functor.hpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/Functor.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/TestTemplate.hpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/TestTemplate.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathADL.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathADL.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathComplexDouble.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathComplexDouble.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathComplexFloat.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathComplexFloat.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathDouble.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathDouble.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathFloat.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathFloat.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/mathLambda.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/mathLambda.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/powMixedTypes.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/powMixedTypes.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/math/src/sincos.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/math/src/sincos.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/buf/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/buf/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/buf/src/BufTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/buf/src/BufTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/copy/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/copy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/copy/src/BufSlicing.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/copy/src/BufSlicing.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/fence/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/fence/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/fence/src/FenceTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/fence/src/FenceTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/p2p/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/p2p/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/p2p/src/P2P.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/p2p/src/P2P.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/Accessor.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/Accessor.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/MdSpan.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/MdSpan.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/ViewConst.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/ViewConst.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/ViewPlainPtrTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/ViewPlainPtrTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/ViewStaticAccMem.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/ViewStaticAccMem.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/mem/view/src/ViewSubViewTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/mem/view/src/ViewSubViewTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/ApplyTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/ApplyTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/CartesianProductTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/CartesianProductTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/ConcatenateTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/ConcatenateTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/CudaVectorArrayWrapperTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/CudaVectorArrayWrapperTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/FilterTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/FilterTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/IntegralTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/IntegralTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/IsArrayOrVectorTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/IsArrayOrVectorTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/IsStrictBaseTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/IsStrictBaseTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/SetTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/SetTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/TransformTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/TransformTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/TypeListOpsTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/TypeListOpsTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/meta/src/UniqueTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/meta/src/UniqueTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/queue/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/queue/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/queue/src/CollectiveQueue.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/queue/src/CollectiveQueue.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/queue/src/QueueTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/queue/src/QueueTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/rand/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/rand/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/rand/src/RandTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/rand/src/RandTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/traits/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/traits/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/traits/src/NativeHandleTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/traits/src/NativeHandleTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/vec/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/vec/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/vec/src/VecTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/vec/src/VecTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/warp/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/warp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/Activemask.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/Activemask.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/All.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/All.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/Any.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/Any.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/Ballot.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/Ballot.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/GetSize.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/GetSize.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/warp/src/Shfl.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/warp/src/Shfl.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/workDiv/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/test/unit/workDiv/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/test/unit/workDiv/src/WorkDivHelpersTest.cpp` & `CLUEstering-2.2.1/extern/alpaka/test/unit/workDiv/src/WorkDivHelpersTest.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.clang-format` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.clang-format`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.conan/test_package/conanfile.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.conan/test_package/conanfile.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.gitattributes` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.gitattributes`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/ISSUE_TEMPLATE/bug_report.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/pull_request_template.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/linux-bazel-builds.yml` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/linux-bazel-builds.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/linux-meson-builds.yml` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/linux-meson-builds.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/linux-other-builds.yml` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/linux-other-builds.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/linux-simple-builds.yml` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/linux-simple-builds.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/mac-builds.yml` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/mac-builds.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.github/workflows/validate-header-guards.yml` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.github/workflows/validate-header-guards.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/.gitignore` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/.gitignore`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/BUILD.bazel` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/CatchConfigOptions.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/CatchConfigOptions.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/CatchMiscFunctions.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/CatchMiscFunctions.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/FindGcov.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/FindLcov.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/Findcodecov.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMake/llvm-cov-wrapper` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CMakePresets.json` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CMakePresets.json`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/CODE_OF_CONDUCT.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/Doxyfile` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/Doxyfile`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/LICENSE.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/README.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/README.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/SECURITY.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/WORKSPACE.bazel` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/WORKSPACE.bazel`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/appveyor.yml` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/appveyor.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/conanfile.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/conanfile.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/artwork/catch2-c-logo.png` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/artwork/catch2-c-logo.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/artwork/catch2-hand-logo.png` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/artwork/catch2-hand-logo.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/artwork/catch2-logo-small-with-background.png` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/artwork/catch2-logo-small-with-background.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/data/artwork/catch2-logo-small.png` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/data/artwork/catch2-logo-small.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/Readme.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/Readme.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/assertions.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/assertions.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/benchmarks.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/ci-and-misc.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/ci-and-misc.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/cmake-integration.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/cmake-integration.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/command-line.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/command-line.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/commercial-users.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/commercial-users.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/comparing-floating-point-numbers.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/comparing-floating-point-numbers.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/configuration.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/contributing.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/deprecations.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/deprecations.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/event-listeners.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/event-listeners.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/faq.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/faq.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/generators.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/generators.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/limitations.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/limitations.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/list-of-examples.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/list-of-examples.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/logging.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/logging.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/matchers.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/matchers.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/migrate-v2-to-v3.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/migrate-v2-to-v3.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/opensource-users.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/opensource-users.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/other-macros.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/other-macros.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/own-main.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/own-main.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/release-notes.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/release-notes.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/release-process.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/release-process.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/reporter-events.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/reporter-events.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/reporters.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/reporters.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/test-cases-and-sections.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/test-cases-and-sections.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/test-fixtures.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/test-fixtures.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/tostring.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/tostring.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/tutorial.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/usage-tips.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/usage-tips.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/docs/why-catch.md` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/docs/why-catch.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/010-TestCase.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/010-TestCase.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/020-TestCase-1.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/020-TestCase-1.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/020-TestCase-2.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/020-TestCase-2.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/030-Asn-Require-Check.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/030-Asn-Require-Check.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/100-Fix-Section.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/100-Fix-Section.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/110-Fix-ClassFixture.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/110-Fix-ClassFixture.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/120-Bdd-ScenarioGivenWhenThen.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/120-Bdd-ScenarioGivenWhenThen.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/210-Evt-EventListeners.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/210-Evt-EventListeners.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/231-Cfg-OutputStreams.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/231-Cfg-OutputStreams.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/300-Gen-OwnGenerator.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/300-Gen-OwnGenerator.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/301-Gen-MapTypeConversion.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/301-Gen-MapTypeConversion.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/302-Gen-Table.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/302-Gen-Table.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/310-Gen-VariablesInGenerators.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/310-Gen-VariablesInGenerators.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/311-Gen-CustomCapture.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/311-Gen-CustomCapture.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/examples/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/Catch.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/Catch.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/CatchAddTests.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/CatchAddTests.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/CatchShardTests.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/CatchShardTests.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/CatchShardTestsImpl.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/CatchShardTestsImpl.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/ParseAndAddCatchTests.cmake` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/ParseAndAddCatchTests.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/catch_amalgamated.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/catch_amalgamated.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/catch_amalgamated.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/catch_amalgamated.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/gdbinit` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/gdbinit`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/extras/lldbinit` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/extras/lldbinit`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/fuzzing/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/fuzzing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/fuzzing/fuzz_textflow.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/fuzzing/fuzz_textflow.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_benchmark.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_benchmark.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_benchmark_all.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_benchmark_all.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_chronometer.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_chronometer.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_clock.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_clock.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_constructor.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_constructor.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_environment.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_environment.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_estimate.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_estimate.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_execution_plan.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_execution_plan.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_optimizer.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_optimizer.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_outlier_classification.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_outlier_classification.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_sample_analysis.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/catch_sample_analysis.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_analyse.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_analyse.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_benchmark_function.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_benchmark_function.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_benchmark_function.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_benchmark_function.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_complete_invoke.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_complete_invoke.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_estimate_clock.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_estimate_clock.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_measure.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_measure.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_repeat.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_repeat.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_run_for_at_least.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_run_for_at_least.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_run_for_at_least.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_run_for_at_least.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_stats.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_stats.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_stats.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_stats.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_timing.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/benchmark/detail/catch_timing.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_all.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_all.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_approx.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_approx.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_approx.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_approx.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_info.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_info.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_result.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_result.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_result.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_assertion_result.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_config.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_config.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_config.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_config.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_message.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_message.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_message.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_message.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_registry_hub.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_registry_hub.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_section_info.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_section_info.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_session.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_session.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_session.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_session.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias_autoregistrar.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias_autoregistrar.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias_autoregistrar.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tag_alias_autoregistrar.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_template_test_macros.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_template_test_macros.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_case_info.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_case_info.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_case_info.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_case_info.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_macros.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_macros.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_spec.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_spec.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_spec.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_test_spec.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_timer.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_timer.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_timer.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_timer.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tostring.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tostring.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_tostring.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_tostring.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_totals.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_totals.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_totals.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_totals.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_translate_exception.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_translate_exception.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_user_config.hpp.in` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_user_config.hpp.in`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_version.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_version.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/catch_version.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/catch_version.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generator_exception.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generator_exception.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_adapters.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_adapters.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_all.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_all.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_random.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_random.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_range.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/generators/catch_generators_range.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_all.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_all.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_capture.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_capture.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_config.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_config.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_enum_values_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_enum_values_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_exception.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_exception.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_generatortracker.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_generatortracker.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_generatortracker.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_generatortracker.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_registry_hub.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_registry_hub.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_factory.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_factory.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_reporter_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_tag_alias_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_tag_alias_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_testcase.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/interfaces/catch_interfaces_testcase.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_assertion_handler.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_assertion_handler.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_assertion_handler.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_assertion_handler.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_insensitive_comparisons.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_insensitive_comparisons.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_insensitive_comparisons.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_case_insensitive_comparisons.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_clara.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_clara.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_clara.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_clara.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_commandline.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_commandline.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_commandline.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_commandline.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_compare_traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_compare_traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_compiler_capabilities.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_compiler_capabilities.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_android_logwrite.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_android_logwrite.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_counter.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_counter.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_uncaught_exceptions.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_uncaught_exceptions.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_wchar.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_config_wchar.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_colour.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_colour.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_colour.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_colour.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_width.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_console_width.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_container_nonmembers.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_container_nonmembers.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_context.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_context.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_context.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_context.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debug_console.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debug_console.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debugger.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debugger.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debugger.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_debugger.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_decomposer.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_decomposer.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_decomposer.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_decomposer.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enforce.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enforce.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enforce.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enforce.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enum_values_registry.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enum_values_registry.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enum_values_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_enum_values_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_errno_guard.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_errno_guard.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_exception_translator_registry.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_exception_translator_registry.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_exception_translator_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_exception_translator_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_fatal_condition_handler.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_fatal_condition_handler.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_fatal_condition_handler.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_fatal_condition_handler.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_floating_point_helpers.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_floating_point_helpers.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_floating_point_helpers.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_floating_point_helpers.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_getenv.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_getenv.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_getenv.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_getenv.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_istream.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_istream.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_istream.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_istream.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_lazy_expr.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_lazy_expr.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_lazy_expr.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_lazy_expr.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_leak_detector.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_leak_detector.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_list.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_list.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_list.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_list.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_logical_traits.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_logical_traits.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_main.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_main.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_message_info.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_message_info.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_message_info.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_message_info.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_meta.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_meta.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_move_and_forward.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_move_and_forward.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_noncopyable.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_noncopyable.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_optional.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_optional.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_output_redirect.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_output_redirect.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_output_redirect.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_output_redirect.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_parse_numbers.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_parse_numbers.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_parse_numbers.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_parse_numbers.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_platform.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_platform.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_polyfills.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_polyfills.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_preprocessor.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_preprocessor.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_preprocessor_remove_parens.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_preprocessor_remove_parens.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_number_generator.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_number_generator.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_number_generator.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_number_generator.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_seed_generation.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_seed_generation.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_seed_generation.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_random_seed_generation.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_registry.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_registry.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_spec_parser.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_spec_parser.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_spec_parser.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reporter_spec_parser.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_result_type.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_result_type.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_result_type.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_result_type.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reusable_string_stream.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reusable_string_stream.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reusable_string_stream.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_reusable_string_stream.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_run_context.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_run_context.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_run_context.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_run_context.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_section.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_section.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_section.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_section.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_sharding.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_sharding.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_singletons.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_singletons.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_singletons.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_singletons.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_source_line_info.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_source_line_info.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_source_line_info.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_source_line_info.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_startup_exception_registry.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_startup_exception_registry.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_startup_exception_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_startup_exception_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stdstreams.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stdstreams.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stream_end_stop.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stream_end_stop.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_string_manip.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_string_manip.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_string_manip.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_string_manip.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stringref.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stringref.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stringref.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_stringref.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_tag_alias_registry.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_tag_alias_registry.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_tag_alias_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_tag_alias_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_template_test_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_template_test_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_info_hasher.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_info_hasher.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_info_hasher.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_info_hasher.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_registry_impl.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_registry_impl.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_registry_impl.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_registry_impl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_tracker.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_tracker.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_tracker.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_case_tracker.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_failure_exception.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_failure_exception.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_failure_exception.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_failure_exception.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_macro_impl.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_macro_impl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_registry.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_registry.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_registry.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_registry.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_spec_parser.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_spec_parser.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_spec_parser.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_test_spec_parser.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_textflow.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_textflow.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_textflow.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_textflow.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_to_string.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_to_string.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_uncaught_exceptions.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_uncaught_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_unique_name.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_unique_name.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_unique_ptr.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_unique_ptr.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_void_type.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_void_type.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_wildcard_pattern.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_wildcard_pattern.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_wildcard_pattern.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_wildcard_pattern.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_windows_h_proxy.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_windows_h_proxy.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_xmlwriter.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_xmlwriter.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_xmlwriter.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/internal/catch_xmlwriter.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_all.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_all.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_container_properties.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_container_properties.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_container_properties.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_container_properties.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_contains.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_contains.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_exception.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_exception.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_exception.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_exception.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_floating_point.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_floating_point.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_floating_point.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_floating_point.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_predicate.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_predicate.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_predicate.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_predicate.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_quantifiers.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_quantifiers.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_quantifiers.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_quantifiers.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_string.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_string.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_string.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_string.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_templated.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_templated.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_templated.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_templated.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_vector.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/catch_matchers_vector.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/catch_matchers_impl.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/catch_matchers_impl.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/catch_matchers_impl.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/matchers/internal/catch_matchers_impl.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/meson.build` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/meson.build`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_automake.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_automake.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_automake.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_automake.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_common_base.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_common_base.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_common_base.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_common_base.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_compact.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_compact.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_compact.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_compact.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_console.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_console.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_console.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_console.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_cumulative_base.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_cumulative_base.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_cumulative_base.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_cumulative_base.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_event_listener.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_event_listener.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_event_listener.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_event_listener.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_helpers.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_helpers.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_helpers.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_helpers.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_junit.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_junit.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_junit.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_junit.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_multi.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_multi.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_multi.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_multi.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_registrars.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_registrars.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_registrars.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_registrars.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_sonarqube.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_sonarqube.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_sonarqube.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_sonarqube.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_streaming_base.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_streaming_base.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_streaming_base.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_streaming_base.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_tap.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_tap.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_tap.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_tap.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_teamcity.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_teamcity.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_teamcity.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_teamcity.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_xml.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_xml.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_xml.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporter_xml.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporters_all.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/src/catch2/reporters/catch_reporters_all.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/CMakeLists.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/ToDo.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/ToDo.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X01-PrefixedMacros.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X01-PrefixedMacros.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X02-DisabledMacros.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X02-DisabledMacros.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X03-DisabledExceptions-DefaultHandler.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X03-DisabledExceptions-DefaultHandler.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X04-DisabledExceptions-CustomHandler.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X04-DisabledExceptions-CustomHandler.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X05-DeferredStaticChecks.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X05-DeferredStaticChecks.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X10-FallbackStringifier.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X10-FallbackStringifier.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X11-DisableStringification.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X11-DisableStringification.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X12-CustomDebugBreakMacro.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X12-CustomDebugBreakMacro.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X21-PartialTestCaseEvents.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X21-PartialTestCaseEvents.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X22-BenchmarksInCumulativeReporter.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X22-BenchmarksInCumulativeReporter.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X23-CasingInReporterNames.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X23-CasingInReporterNames.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X24-ListenerStdoutCaptureInMultireporter.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X24-ListenerStdoutCaptureInMultireporter.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X25-ListenerCanAskForCapturedStdout.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X25-ListenerCanAskForCapturedStdout.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X26-ReporterPreferencesForPassingAssertionsIsRespected.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X26-ReporterPreferencesForPassingAssertionsIsRespected.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X27-CapturedStdoutInTestCaseEvents.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X27-CapturedStdoutInTestCaseEvents.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X28-ListenersGetEventsBeforeReporters.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X28-ListenersGetEventsBeforeReporters.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X29-CustomArgumentsForReporters.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X29-CustomArgumentsForReporters.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X31-DuplicatedTestCases.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X31-DuplicatedTestCases.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X32-DuplicatedTestCasesDifferentTags.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X32-DuplicatedTestCasesDifferentTags.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X33-DuplicatedTestCaseMethods.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X33-DuplicatedTestCaseMethods.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X34-DuplicatedTestCaseMethodsDifferentFixtures.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X34-DuplicatedTestCaseMethodsDifferentFixtures.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X35-DuplicatedReporterNames.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X35-DuplicatedReporterNames.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X90-WindowsHeaderInclusion.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X90-WindowsHeaderInclusion.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X91-AmalgamatedCatch.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/ExtraTests/X91-AmalgamatedCatch.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.std.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.std.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.sw.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.sw.multi.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/automake.sw.multi.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/compact.sw.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/compact.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/compact.sw.multi.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/compact.sw.multi.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.std.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.std.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.sw.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.sw.multi.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.sw.multi.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.swa4.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/console.swa4.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/junit.sw.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/junit.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/junit.sw.multi.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/junit.sw.multi.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/sonarqube.sw.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/sonarqube.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/sonarqube.sw.multi.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/sonarqube.sw.multi.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/tap.sw.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/tap.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/tap.sw.multi.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/tap.sw.multi.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/teamcity.sw.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/teamcity.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/teamcity.sw.multi.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/teamcity.sw.multi.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/xml.sw.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/xml.sw.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/xml.sw.multi.approved.txt` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/Baselines/xml.sw.multi.approved.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Clara.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Clara.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/CmdLine.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/CmdLine.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/CmdLineHelpers.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/CmdLineHelpers.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/ColourImpl.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/ColourImpl.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Details.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Details.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/FloatingPoint.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/FloatingPoint.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/GeneratorsImpl.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/GeneratorsImpl.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/InternalBenchmark.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/InternalBenchmark.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Parse.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Parse.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/PartTracker.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/PartTracker.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/RandomNumberGeneration.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/RandomNumberGeneration.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Reporters.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Reporters.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Sharding.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Sharding.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Stream.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Stream.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/String.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/String.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/StringManip.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/StringManip.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Tag.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Tag.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestCaseInfoHasher.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestCaseInfoHasher.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestSpec.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestSpec.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestSpecParser.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TestSpecParser.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TextFlow.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/TextFlow.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/ToString.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/ToString.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Traits.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Traits.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/UniquePtr.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/UniquePtr.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Xml.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/IntrospectiveTests/Xml.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/TestRegistrations.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/TestRegistrations.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/TimingTests/Sleep.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/TimingTests/Sleep.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Approx.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Approx.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/BDD.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/BDD.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Benchmark.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Benchmark.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Class.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Class.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Compilation.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Compilation.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Condition.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Condition.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Decomposition.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Decomposition.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/EnumToString.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/EnumToString.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Exception.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Exception.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Generators.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Generators.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Matchers.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Matchers.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/MatchersRanges.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/MatchersRanges.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Message.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Message.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Misc.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Misc.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringByte.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringByte.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringChrono.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringChrono.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringGeneral.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringGeneral.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringOptional.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringOptional.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringPair.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringPair.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringTuple.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringTuple.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringVariant.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringVariant.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringVector.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringVector.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringWhich.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/ToStringWhich.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Tricky.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/Tricky.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/VariadicMacros.tests.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/UsageTests/VariadicMacros.tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/parse_test_spec.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/parse_test_spec.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/parse_test_spec.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/parse_test_spec.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/type_with_lit_0_comparisons.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/SelfTest/helpers/type_with_lit_0_comparisons.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/ConfigureTestsCommon.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/ConfigureTestsCommon.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testBazelReporter.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testBazelReporter.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testBazelSharding.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testBazelSharding.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDefaultReporter.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDefaultReporter.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDisable.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDisable.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDisableStringification.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureDisableStringification.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureExperimentalRedirect.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testConfigureExperimentalRedirect.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testPartialTestCaseEvent.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testPartialTestCaseEvent.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testRandomOrder.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testRandomOrder.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/TestScripts/testSharding.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/TestScripts/testSharding.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tests/meson.build` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tests/meson.build`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/third_party/clara.hpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/third_party/clara.hpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/appveyorBuildConfigurationScript.bat` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/appveyorBuildConfigurationScript.bat`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/appveyorTestRunScript.bat` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/appveyorTestRunScript.bat`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/coverage-helper.cpp` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/coverage-helper.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/misc/installOpenCppCoverage.ps1` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/misc/installOpenCppCoverage.ps1`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/approvalTests.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/approvalTests.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/approve.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/approve.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/checkConvenienceHeaders.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/checkConvenienceHeaders.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/checkLicense.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/checkLicense.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/extractFeaturesFromReleaseNotes.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/extractFeaturesFromReleaseNotes.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/fixWhitespace.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/fixWhitespace.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/generateAmalgamatedFiles.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/generateAmalgamatedFiles.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/releaseCommon.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/releaseCommon.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/updateDocumentSnippets.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/updateDocumentSnippets.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/alpaka/thirdParty/catch2/tools/scripts/updateDocumentToC.py` & `CLUEstering-2.2.1/extern/alpaka/thirdParty/catch2/tools/scripts/updateDocumentToC.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.appveyor.yml` & `CLUEstering-2.2.1/extern/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.clang-format` & `CLUEstering-2.2.1/extern/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.clang-tidy` & `CLUEstering-2.2.1/extern/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.cmake-format.yaml` & `CLUEstering-2.2.1/extern/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.codespell-ignore-lines` & `CLUEstering-2.2.1/extern/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/CONTRIBUTING.md` & `CLUEstering-2.2.1/extern/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `CLUEstering-2.2.1/extern/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/matchers/pylint.json` & `CLUEstering-2.2.1/extern/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/pull_request_template.md` & `CLUEstering-2.2.1/extern/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/workflows/ci.yml` & `CLUEstering-2.2.1/extern/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/workflows/configure.yml` & `CLUEstering-2.2.1/extern/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/workflows/format.yml` & `CLUEstering-2.2.1/extern/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/workflows/labeler.yml` & `CLUEstering-2.2.1/extern/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/workflows/pip.yml` & `CLUEstering-2.2.1/extern/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.github/workflows/upstream.yml` & `CLUEstering-2.2.1/extern/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/.pre-commit-config.yaml` & `CLUEstering-2.2.1/extern/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/LICENSE` & `CLUEstering-2.2.1/extern/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/README.rst` & `CLUEstering-2.2.1/extern/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/SECURITY.md` & `CLUEstering-2.2.1/extern/pybind11/SECURITY.md`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/Doxyfile` & `CLUEstering-2.2.1/extern/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/Makefile` & `CLUEstering-2.2.1/extern/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/chrono.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/custom.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/eigen.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/functional.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/index.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/overview.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/stl.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/cast/strings.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/classes.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/embedding.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/exceptions.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/functions.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/misc.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/pycpp/numpy.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/pycpp/object.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/pycpp/utilities.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/advanced/smart_ptrs.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/basics.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/benchmark.py` & `CLUEstering-2.2.1/extern/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/benchmark.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/changelog.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/classes.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/compiling.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/conf.py` & `CLUEstering-2.2.1/extern/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/faq.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/index.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/installing.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/limitations.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/pybind11-logo.png` & `CLUEstering-2.2.1/extern/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/pybind11_vs_boost_python1.png` & `CLUEstering-2.2.1/extern/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/pybind11_vs_boost_python1.svg` & `CLUEstering-2.2.1/extern/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/pybind11_vs_boost_python2.png` & `CLUEstering-2.2.1/extern/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/pybind11_vs_boost_python2.svg` & `CLUEstering-2.2.1/extern/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/reference.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/release.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/docs/upgrade.rst` & `CLUEstering-2.2.1/extern/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/attr.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/buffer_info.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/cast.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/chrono.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/complex.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/class.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/common.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/descr.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/init.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/internals.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/type_caster_base.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/detail/typeid.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/eigen/matrix.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/eigen/tensor.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/embed.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/eval.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/functional.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/gil.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/gil_safe_call_once.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/gil_safe_call_once.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/iostream.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/numpy.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/operators.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/options.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/pybind11.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/pytypes.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/stl/filesystem.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/stl.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/stl_bind.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/include/pybind11/typing.h` & `CLUEstering-2.2.1/extern/pybind11/include/pybind11/typing.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/noxfile.py` & `CLUEstering-2.2.1/extern/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/pybind11/__main__.py` & `CLUEstering-2.2.1/extern/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/pybind11/commands.py` & `CLUEstering-2.2.1/extern/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/pybind11/setup_helpers.py` & `CLUEstering-2.2.1/extern/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/pyproject.toml` & `CLUEstering-2.2.1/extern/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/setup.cfg` & `CLUEstering-2.2.1/extern/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/setup.py` & `CLUEstering-2.2.1/extern/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/conftest.py` & `CLUEstering-2.2.1/extern/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/constructor_stats.h` & `CLUEstering-2.2.1/extern/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/cross_module_gil_utils.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/env.py` & `CLUEstering-2.2.1/extern/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/extra_python_package/test_files.py` & `CLUEstering-2.2.1/extern/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/extra_setuptools/test_setuphelper.py` & `CLUEstering-2.2.1/extern/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/local_bindings.h` & `CLUEstering-2.2.1/extern/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/object.h` & `CLUEstering-2.2.1/extern/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/pybind11_cross_module_tests.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/pybind11_tests.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/pybind11_tests.h` & `CLUEstering-2.2.1/extern/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/pytest.ini` & `CLUEstering-2.2.1/extern/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/requirements.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_async.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_async.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_buffers.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_buffers.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_builtin_casters.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_builtin_casters.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_call_policies.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_call_policies.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_callbacks.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_callbacks.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_chrono.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_chrono.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_class.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_class.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/embed.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_const_name.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_const_name.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_constants_and_functions.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_constants_and_functions.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_copy_move.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_copy_move.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_custom_type_casters.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_custom_type_casters.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_custom_type_setup.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_custom_type_setup.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_docstring_options.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_docstring_options.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_eigen_matrix.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_eigen_matrix.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_eigen_tensor.inl` & `CLUEstering-2.2.1/extern/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_eigen_tensor.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_embed/CMakeLists.txt` & `CLUEstering-2.2.1/extern/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_embed/catch.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_embed/external_module.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_embed/test_interpreter.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_enum.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_enum.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_eval.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_eval.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_exceptions.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_exceptions.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_factory_constructors.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_factory_constructors.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_gil_scoped.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_gil_scoped.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_iostream.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_iostream.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_kwargs_and_defaults.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_kwargs_and_defaults.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_local_bindings.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_local_bindings.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_methods_and_attributes.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_methods_and_attributes.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_modules.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_modules.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_multiple_inheritance.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_multiple_inheritance.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_array.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_array.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_dtypes.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_dtypes.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_vectorize.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_numpy_vectorize.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_opaque_types.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_opaque_types.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_operator_overloading.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_operator_overloading.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_pickling.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_pickling.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_pytypes.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_pytypes.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_sequences_and_iterators.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_sequences_and_iterators.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_smart_ptr.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_smart_ptr.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_stl.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_stl.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_stl_binders.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_stl_binders.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_tagbased_polymorphic.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_tagbased_polymorphic.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_thread.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_thread.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_type_caster_pyobject_ptr.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_type_caster_pyobject_ptr.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_type_caster_pyobject_ptr.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_type_caster_pyobject_ptr.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_union.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_unnamed_namespace_a.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_unnamed_namespace_a.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_unnamed_namespace_a.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_unnamed_namespace_a.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_vector_unique_ptr_member.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_vector_unique_ptr_member.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_virtual_functions.cpp` & `CLUEstering-2.2.1/extern/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/test_virtual_functions.py` & `CLUEstering-2.2.1/extern/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/valgrind-numpy-scipy.supp` & `CLUEstering-2.2.1/extern/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tests/valgrind-python.supp` & `CLUEstering-2.2.1/extern/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/FindCatch.cmake` & `CLUEstering-2.2.1/extern/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/FindEigen3.cmake` & `CLUEstering-2.2.1/extern/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/FindPythonLibsNew.cmake` & `CLUEstering-2.2.1/extern/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/JoinPaths.cmake` & `CLUEstering-2.2.1/extern/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/check-style.sh` & `CLUEstering-2.2.1/extern/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/cmake_uninstall.cmake.in` & `CLUEstering-2.2.1/extern/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/codespell_ignore_lines_from_errors.py` & `CLUEstering-2.2.1/extern/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/libsize.py` & `CLUEstering-2.2.1/extern/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/make_changelog.py` & `CLUEstering-2.2.1/extern/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/pybind11Common.cmake` & `CLUEstering-2.2.1/extern/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/pybind11Config.cmake.in` & `CLUEstering-2.2.1/extern/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/pybind11NewTools.cmake` & `CLUEstering-2.2.1/extern/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/pybind11Tools.cmake` & `CLUEstering-2.2.1/extern/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/setup_global.py.in` & `CLUEstering-2.2.1/extern/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/extern/pybind11/tools/setup_main.py.in` & `CLUEstering-2.2.1/extern/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `CLUEstering-2.2.0/setup.py` & `CLUEstering-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import os
 import sys
 from pathlib import Path
 from setuptools import setup
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 this_directory = Path(__file__).parent
 long_description = (this_directory/'README.md').read_text()
 
 if sys.argv[1] != 'sdist':
     os.system("cmake -B build && make -C build")
 
 setup(
```

